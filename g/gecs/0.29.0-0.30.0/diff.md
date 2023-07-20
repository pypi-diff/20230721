# Comparing `tmp/gecs-0.29.0.tar.gz` & `tmp/gecs-0.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gecs-0.29.0.tar", max compression
+gzip compressed data, was "gecs-0.30.0.tar", max compression
```

## Comparing `gecs-0.29.0.tar` & `gecs-0.30.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1060 2023-07-11 17:36:42.496116 gecs-0.29.0/LICENSE
--rw-r--r--   0        0        0     2220 2023-07-11 17:36:43.424133 gecs-0.29.0/README.md
--rw-r--r--   0        0        0      697 2023-07-11 18:17:15.906277 gecs-0.29.0/pyproject.toml
--rw-r--r--   0        0        0    47487 2023-07-11 18:17:15.906277 gecs-0.29.0/src/gecs/gec.py
--rw-r--r--   0        0        0     2152 2023-07-11 18:17:15.906277 gecs-0.29.0/src/gecs/utils/gaussian_process_visualisation.py
--rw-r--r--   0        0        0     3217 1970-01-01 00:00:00.000000 gecs-0.29.0/setup.py
--rw-r--r--   0        0        0     3184 1970-01-01 00:00:00.000000 gecs-0.29.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-07-11 17:36:42.496116 gecs-0.30.0/LICENSE
+-rw-r--r--   0        0        0     3370 2023-07-20 22:11:20.400795 gecs-0.30.0/README.md
+-rw-r--r--   0        0        0      697 2023-07-20 22:11:20.404795 gecs-0.30.0/pyproject.toml
+-rw-r--r--   0        0        0    49930 2023-07-20 22:11:20.404795 gecs-0.30.0/src/gecs/gec.py
+-rw-r--r--   0        0        0     2152 2023-07-11 18:17:15.906277 gecs-0.30.0/src/gecs/utils/gaussian_process_visualisation.py
+-rw-r--r--   0        0        0     4392 1970-01-01 00:00:00.000000 gecs-0.30.0/setup.py
+-rw-r--r--   0        0        0     4334 1970-01-01 00:00:00.000000 gecs-0.30.0/PKG-INFO
```

### Comparing `gecs-0.29.0/LICENSE` & `gecs-0.30.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gecs-0.29.0/src/gecs/gec.py` & `gecs-0.30.0/src/gecs/gec.py`

 * *Files 3% similar despite different names*

```diff
@@ -212,14 +212,19 @@
         self.set_params(**kwargs)
 
         self._init_kwargs = {
             k: v
             for k, v in kwargs.items()
             if k not in ["bagging_freq", "bagging_fraction"]
         }
+        self.bagging_fraction = kwargs.get("bagging_fraction", None)
+        self.bagging_freq = kwargs.get("bagging_freq", None)
+
+        self.fix_bagging = False
+        self.fix_boosting_type = False
 
         self.frozen = frozen
         non_optimized_init_args = [
             "max_depth",
             "subsample_for_bin",
             "objective",
             "class_weight",
@@ -265,22 +270,34 @@
         ]
 
         self._categorical_hyperparameter_names, _ = zip(
             *self.categorical_hyperparameters
         )
 
         prohibited_combinations = ["rf-no_bagging"]
+        if self.fix_bagging and (
+            self.bagging_fraction is None or self.bagging_freq is None
+        ):
+            prohibited_combinations += ["rf-yes_bagging"]
+
         self._categorical_hyperparameter_combinations = [
             "-".join(y)
             for y in itertools.product(
                 *[x[1] for x in self.categorical_hyperparameters]
             )
             if "-".join(y) not in prohibited_combinations
         ]
 
+        if self.fix_boosting_type:
+            self._categorical_hyperparameter_combinations = [
+                hp_comb
+                for hp_comb in self._categorical_hyperparameter_combinations
+                if hp_comb.startswith(self.boosting_type)
+            ]
+
         ten_to_ten_thousand = np.concatenate(
             [
                 np.arange(10, 100, 10),
                 np.arange(100, 200, 20),
                 np.arange(200, 500, 50),
                 np.arange(500, 100, 100),
                 np.arange(1000, 10001, 1000),
@@ -677,50 +694,93 @@
             "eval_init_score": eval_init_score,
             "eval_metric": eval_metric,
             "feature_name": feature_name,
             "categorical_feature": categorical_feature,
             "callbacks": callbacks,
             "init_model": init_model,
         }
+
+        self.fix_boosting_type = "boosting_type" in fixed_hyperparameters
+        fixed_hyperparameters = [
+            hp for hp in fixed_hyperparameters if hp != "boosting_type"
+        ]
+
+        self.fix_bagging = "bagging" in fixed_hyperparameters
+        fixed_hyperparameters = [hp for hp in fixed_hyperparameters if hp != "bagging"]
+
+        assert (
+            (not self.fix_bagging)
+            or (self.bagging_freq is not None)
+            or (self.boosting_type != "rf")
+            or (not self.fix_boosting_type)
+        ), 'boosting_type="rf" requires bagging'
         if not self.frozen:
             filtered_hyperparameters = list(
                 set(self.gec_hyperparameters["hyperparameters"]).difference(
                     set(fixed_hyperparameters)
                 )
             )
             self.set_gec_hyperparameters({"hyperparameters": filtered_hyperparameters})
 
             self.best_scores_gec = {}
             self.best_params_gec = {}
             (
                 self.best_params_gec["search"],
                 self.best_scores_gec["search"],
             ) = self._optimise_hyperparameters(n_iter, X, y)
-            self.best_params_gec["grid"] = self._find_best_parameters()
+
+            best_params_grid = self._find_best_parameters()
+            self.best_params_gec["grid"] = self._replace_fixed_args(best_params_grid)
             self.best_scores_gec["grid"] = self._calculate_cv_score(
                 X, y, self.best_params_gec["grid"]
             )
-            best_params_prep = copy.deepcopy(self.best_params_gec["search"])
-            self.best_params_gec[
-                "grid_from_search"
-            ] = self._find_best_parameters_from_search(best_params_prep)
 
+            best_params_prep = copy.deepcopy(self.best_params_gec["search"])
+            best_params_grid_from_search = self._find_best_parameters_from_search(
+                best_params_prep
+            )
+            self.best_params_gec["grid_from_search"] = self._replace_fixed_args(
+                best_params_grid_from_search
+            )
             self.best_scores_gec["grid_from_search"] = self._calculate_cv_score(
                 X, y, self.best_params_gec["grid_from_search"]
             )
 
             for source, score in self.best_scores_gec.items():
                 if self.best_score is None or score > self.best_score:
                     self.best_score = score
                     self.best_params_ = self.best_params_gec[source]
 
         self._fit_best_params(X, y)
 
         return self
 
+    def _replace_fixed_args(self, params):
+        if self.fix_boosting_type:
+            params["boosting_type"] = self.boosting_type
+        self.selected_arms = []
+        if (
+            self.fix_bagging
+            and "bagging_fraction" in params
+            and "bagging_freq" in params
+        ):
+            if self.bagging_fraction is not None and self.bagging_freq is not None:
+                params["bagging_fraction"] = self.bagging_fraction
+                params["bagging_freq"] = self.bagging_freq
+            else:
+                del params["bagging_fraction"]
+                del params["bagging_freq"]
+            self.bagging_scores = {
+                "inputs": [],
+                "output": [],
+                "means": [],
+                "sigmas": [],
+            }
+        return params
+
     def _calculate_cv_score(
         self,
         X: ndarray,
         y: ndarray,
         params: Dict[str, Optional[Union[str, float, int, float64]]],
     ) -> float64:
         clf = LGBMClassifier(**params)
@@ -784,14 +844,15 @@
                         arguments["bagging_freq"],
                         arguments["bagging_fraction"],
                     ) = selected_combination_bagging
 
             del arguments["bagging"]
             arguments["verbosity"] = -1
 
+            arguments = self._replace_fixed_args(arguments)
             score = self._calculate_cv_score(X, Y, arguments)
 
             self._update_gec_fields(
                 score, arguments, selected_arm, selected_combination, mean, sigma
             )
 
             if "bagging_freq" in arguments:
@@ -819,31 +880,38 @@
         )
         arguments = self._build_arguments(selected_arm.split("-"), random_combination)
         selected_combination = random_combination
         random_combination_bagging = self._bagging_combinations[
             np.random.choice(range(len(self._bagging_combinations)))
         ]
 
-        (
-            arguments["bagging_freq"],
-            arguments["bagging_fraction"],
-        ) = random_combination_bagging
-        selected_combination_bagging = random_combination_bagging
+        if "yes_bagging" in selected_arm:
+            (
+                arguments["bagging_freq"],
+                arguments["bagging_fraction"],
+            ) = random_combination_bagging
+            selected_combination_bagging = random_combination_bagging
+        else:
+            selected_combination_bagging = None
 
         return (
             selected_arm,
             selected_combination,
             selected_combination_bagging,
             arguments,
         )
 
     def _select_parameters(self) -> Tuple[str, ndarray, ndarray, ndarray]:
 
         sampled_reward = np.array(
-            [beta.rvs(reward["a"], reward["b"]) for _, reward in self.rewards.items()]
+            [
+                beta.rvs(reward["a"], reward["b"])
+                for arm, reward in self.rewards.items()
+                if arm in self._categorical_hyperparameter_combinations
+            ]
         )
         selected_arm_index = sampled_reward.argmax()
         selected_arm = self._categorical_hyperparameter_combinations[selected_arm_index]
 
         sets = np.array(
             [
                 np.random.choice(range_, self.gec_hyperparameters["n_sample_initial"])
@@ -1023,25 +1091,27 @@
         self.gaussian.fit(
             np.array(self.hyperparameter_scores["inputs"]),
             np.array(self.hyperparameter_scores["output"])
             - np.mean(self.hyperparameter_scores["output"]),
         )
 
     def _fit_gaussian_bagging(self) -> None:
-        self.gaussian_bagging.fit(
-            np.array(self.bagging_scores["inputs"]),
-            np.array(self.bagging_scores["output"])
-            - np.mean(self.bagging_scores["output"]),
-        )
+        if len(self.bagging_scores["output"]):
+            self.gaussian_bagging.fit(
+                np.array(self.bagging_scores["inputs"]),
+                np.array(self.bagging_scores["output"])
+                - np.mean(self.bagging_scores["output"]),
+            )
 
     def _get_best_arm(self) -> str:
         mean_reward = np.array(
             [
                 reward["a"] / (reward["a"] + reward["b"])
-                for _, reward in self.rewards.items()
+                for arm, reward in self.rewards.items()
+                if arm in self._categorical_hyperparameter_combinations
             ]
         )
         best_arm = self._categorical_hyperparameter_combinations[mean_reward.argmax()]
         return best_arm
 
     def _find_best_parameters(
         self, step_sizes: List[int] = [16, 8, 4, 2, 1]
@@ -1108,22 +1178,14 @@
     ) -> Dict[str, Optional[Union[int, float, str]]]:
         for step_size, previous_step_size in zip(step_sizes[1:], step_sizes[:-1]):
 
             neighbouring_combinations = self._get_neighbouring_combinations(
                 best_combination, step_size, previous_step_size
             )
 
-            new_ranges = [
-                (name, min(r), max(r))
-                for name, r in zip(
-                    self._real_hyperparameter_names, neighbouring_combinations
-                )
-            ]
-            # log.info(new_ranges)
-
             best_combination, best_score = self._find_best_parameters_iter(
                 neighbouring_combinations
             )
 
         arguments = self._build_arguments(best_arm.split("-"), best_combination)
 
         if "yes_bagging" in best_arm:
```

### Comparing `gecs-0.29.0/src/gecs/utils/gaussian_process_visualisation.py` & `gecs-0.30.0/src/gecs/utils/gaussian_process_visualisation.py`

 * *Files identical despite different names*

### Comparing `gecs-0.29.0/PKG-INFO` & `gecs-0.30.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gecs
-Version: 0.29.0
+Version: 0.30.0
 Summary: LightGBM Classifier with integrated bayesian hyperparameter optimization
 Home-page: https://github.com/0xideas/sequifier
 License: MIT
 Keywords: lightgbm,classification,machine learning,hyperparameter optimization,classifier
 Author: Leon Luithlen
 Author-email: leontimnaluithlen@gmail.com
 Requires-Python: >=3.10.0,<3.11.0
@@ -27,50 +27,75 @@
 ![a gecko looking at the camera with bayesian math in white on a pink and green background](documentation/assets/header.png)
 
 
 # (100)gecs
 
 Bayesian hyperparameter tuning for LGBMClassifier with a scikit-learn API
 
+
 ## Table of Contents
 
 - [Project Overview](#project-overview)
+- [Introduction](#introduction)
 - [Installation](#installation)
 - [Usage](#usage)
+- [Example](#example)
 - [Contributing](#contributing)
 - [License](#license)
 
+
 ## Project Overview
 
-The package `gecs` provides the class `GEC`, which is a child class of the class `LGBMClassifier` from the package `lightgbm`. It can be imported from `gecs.gec` and then used in place of `LGBMClassifier`, with the same API. The difference to `LGBMClassifier` lies in the fact that `GEC`automatically does bayesian hyperparameter optimization of the parameters `learning_rate`, `reg_alpha`, `reg_lambda`, `min_child_samples`, `min_child_weight`, `colsample_bytree` and optionally also of `num_leaves` and `n_estimators`.
+`gecs` is a tool to help automate the process of hyperparameter tuning for LightGBM classifiers, which can potentially save significant time and computational resources in model building and optimization processes. The `GEC` stands for **G**ood **E**nough **C**lassifier, which allows you to focus on other tasks such as feature engineering. If you deploy 100 of them, you get 100GECs.
+
+
+## Introduction
+
+The primary class in this package is `GEC`, which is derived from `LGBMClassifier`. Like its parent, GEC can be used to build and train gradient boosting models, but with the added feature of **automated bayesian hyperparameter optimization**. It can be imported from `gecs.gec` and then used in place of `LGBMClassifier`, with the same API.
 
-The fit method has two new parameters: `n_iter`, which sets the number of hyperparameter combinations that will be tried (the higher `n_iter` the higher the expected accuracy, but at a cost of compute) and `fixed_hyperparameters`, which determines which hyperparameters of the LGBM classifier won't get optimized. By default, these are `n_estimators` and `num_leaves`, as the highest possible value for these hyperparameters is almost always optimal. The idea then is to set these as high as makes sense in a specific context and then optimize the other hyperparameters.
+By default, `GEC` optimizes `boosting_type`, `learning_rate`, `reg_alpha`, `reg_lambda`, `min_child_samples`, `min_child_weight`, `colsample_bytree`, `bagging_freq`, `bagging_fraction` and optionally `num_leaves` and `n_estimators`. Which hyperparameters to tune is fully customizable.
 
 
 ## Installation
 
     pip install gecs
 
+
 ## Usage
 
+
+The `GEC` class provides the same API to the user as the `LGBMClassifier` class of `lightgbm`, and additionally:
+
+-   the two additional parameters to the fit method:
+    - `n_iter`: Defines the number of hyperparameter combinations that the model should try. More iterations could lead to better model performance, but at the expense of computational resources
+
+    - `fixed_hyperparameters`: Allows the user to specify hyperparameters that the GEC should not optimize. By default, these are `n_estimators` and `num_leaves`. Any of the LGBMClassifier init arguments can be fixed, and so can  `bagging_freq` and `bagging_fraction`, but only jointly. This is done by passing the value `bagging`.
+
+-   the methods `serialize` and `deserialize`, which stores the `GEC` state for the hyperparameter optimization process, **but not the fitted** `LGBMClassifier` **parameters**, to a json file. To store the boosted tree model itself, you have to provide your own serialization or use `pickle`
+
+-   the methods `freeze` and `unfreeze` that turn the `GEC` functionally into a `LGBMClassifier` and back
+
+
+## Example
+
+The default use of `GEC` would look like this:
+
     from gecs.gec import GEC
 
     gec.fit(X, y)
 
     gec.serialize(path) # stores gec data and settings, but not underlying LGBMClassifier attributes
 
     gec2 = GEC.deserialize(path, X, y) # X and y are necessary to fit the underlying LGBMClassifier
 
     yhat = gec.predict(X)
 
     gec.freeze() # freeze GEC so that it behaves like a LGBMClassifier
-    gec.unfreeze() # unfreeze to enable GEC hyperparameter optimisation
 
-
-    
+    gec.unfreeze() # unfreeze to enable GEC hyperparameter optimisation
 
 
 
 ## Contributing
 
 If you want to contribute, please reach out and I'll design a process around it.
```

