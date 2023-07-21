# Comparing `tmp/pyracer-1.1.0.tar.gz` & `tmp/pyracer-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyracer-1.1.0.tar", last modified: Thu Jul 20 19:23:29 2023, max compression
+gzip compressed data, was "pyracer-1.1.1.tar", last modified: Fri Jul 21 07:59:28 2023, max compression
```

## Comparing `pyracer-1.1.0.tar` & `pyracer-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:23:29.132282 pyracer-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-20 19:23:20.000000 pyracer-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-20 19:23:29.132282 pyracer-1.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:23:29.132282 pyracer-1.1.0/RACER/
--rw-r--r--   0 runner    (1001) docker     (123)    14422 2023-07-20 19:23:20.000000 pyracer-1.1.0/RACER/RACER.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-20 19:23:20.000000 pyracer-1.1.0/RACER/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-20 19:23:20.000000 pyracer-1.1.0/RACER/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 19:23:20.000000 pyracer-1.1.0/RACER/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-20 19:23:20.000000 pyracer-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:23:29.132282 pyracer-1.1.0/pyracer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-20 19:23:29.000000 pyracer-1.1.0/pyracer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-20 19:23:29.000000 pyracer-1.1.0/pyracer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:23:29.000000 pyracer-1.1.0/pyracer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 19:23:29.000000 pyracer-1.1.0/pyracer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 19:23:29.000000 pyracer-1.1.0/pyracer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:23:29.132282 pyracer-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-20 19:23:20.000000 pyracer-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:59:28.475448 pyracer-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-21 07:59:13.000000 pyracer-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-21 07:59:28.475448 pyracer-1.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:59:28.471449 pyracer-1.1.1/RACER/
+-rw-r--r--   0 runner    (1001) docker     (123)    14422 2023-07-21 07:59:13.000000 pyracer-1.1.1/RACER/RACER.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-21 07:59:13.000000 pyracer-1.1.1/RACER/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-07-21 07:59:13.000000 pyracer-1.1.1/RACER/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 07:59:13.000000 pyracer-1.1.1/RACER/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-21 07:59:13.000000 pyracer-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:59:28.475448 pyracer-1.1.1/pyracer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-21 07:59:28.000000 pyracer-1.1.1/pyracer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-21 07:59:28.000000 pyracer-1.1.1/pyracer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:59:28.000000 pyracer-1.1.1/pyracer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-21 07:59:28.000000 pyracer-1.1.1/pyracer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 07:59:28.000000 pyracer-1.1.1/pyracer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 07:59:28.475448 pyracer-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-21 07:59:13.000000 pyracer-1.1.1/setup.py
```

### Comparing `pyracer-1.1.0/LICENSE` & `pyracer-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyracer-1.1.0/PKG-INFO` & `pyracer-1.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracer
-Version: 1.1.0
+Version: 1.1.1
 Summary: Unofficial Python implementation of the RACER classification algorithm.
 Home-page: https://github.com/Adversarian/RACER
 Author: Arian Tashakkor, Mohammad Safaiyan
 Author-email: a77physics@gmail.com
 License: MIT
 Keywords: machine learning,classification,RACER
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyracer-1.1.0/RACER/RACER.py` & `pyracer-1.1.1/RACER/RACER.py`

 * *Files identical despite different names*

### Comparing `pyracer-1.1.0/RACER/preprocessing.py` & `pyracer-1.1.1/RACER/preprocessing.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,29 +3,33 @@
 import numpy as np
 import pandas as pd
 
 from optbinning import MulticlassOptimalBinning as MOB, MDLP
 
 
 class RACERPreprocessor:
-    def __init__(self, target: str="multiclass", max_n_bins=32, max_num_splits=32):
+    def __init__(self, target: str="auto", max_n_bins=32, max_num_splits=32):
         """RACER preprocessing step that quantizes numerical columns and dummy encodes the categorical ones.
         Quantization is based on the optimal binning algorithm for "multiclass" tasks and the entropy-based MDLP
         algorithm for "binary" tasks.
 
         Args:
-            target (str, optional): Whether the task if "multiclass" or "binary" classification. Defaults to "multiclass".
+            target (str, optional): Whether the task is "multiclass" or "binary" classification. Defaults to "auto" which attempts automatically infer the task from `y`.
             max_n_bins (int, optional): Maximum number of bins to quantize in. Defaults to 32.
             max_num_splits (int, optional): Maximum number of splits to consider at each partition for MDLP. Defaults to 32.
         """
-        assert target in ["multiclass", "binary"], "`target` must either be 'multiclass' or 'binary'"
+        assert target in ["multiclass", "binary", "auto"], "`target` must either be 'multiclass', 'binary' or 'auto'."
         if target == "multiclass":
             self._quantizer = MOB(max_n_bins=max_n_bins)
         elif target == "binary":
             self._quantizer = MDLP(max_candidates=max_num_splits)
+        else:
+            self._quantizer = "infer"
+            self._max_n_bins = max_n_bins
+            self._max_candidates = max_num_splits
 
     def fit_transform(
         self, X: Union[pd.DataFrame, np.ndarray], y: Union[pd.DataFrame, np.ndarray]
     ) -> Tuple[Union[pd.DataFrame, np.ndarray], Union[pd.DataFrame, np.ndarray]]:
         """Preprocesses the dataset by replacing nominal vaues with dummy variables.
         Converts to numpy boolean arrays and returns the dataset. All numerical values are discretized
         using an optimal binning strategy that employs a decision tree as a preprocessing step.
@@ -34,14 +38,20 @@
             X (Union[pd.DataFrame, np.ndarray]): Features vector
             y (Union[pd.DataFrame, np.ndarray]): Targets vector
 
         Returns:
             Tuple[Union[pd.DataFrame, np.ndarray], Union[pd.DataFrame, np.ndarray]]: Transformed features and targets vectors.
         """
         X, y = pd.DataFrame(X), pd.DataFrame(y)
+        if self._quantizer == "infer":
+            uniques = y.nunique()
+            if uniques > 2:
+                self._quantizer = MOB(max_candidates=self._max_num_splits)
+            else:
+                self._quantizer = MDLP(max_n_bins=self._max_n_bins)
         numerics_X = X.select_dtypes(include=[np.number]).columns.tolist()
         if numerics_X:
             for col in numerics_X:
                 self._quantizer.fit(X[col].values, np.squeeze(y.values))
                 bins = [X[col].min()] + self._quantizer.splits.tolist() + [X[col].max()]
                 X[col] = pd.cut(X[col], bins=bins, include_lowest=True, labels=False)
         X, y = X.astype("category"), y.astype("category")
```

### Comparing `pyracer-1.1.0/README.md` & `pyracer-1.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # RACER
 Unofficial Python implementation of the RACER classification algorithm described by [Basiri et. al, 2019](https://link.springer.com/article/10.1007/s00521-017-3117-2).
-RACER is designed specifically for discrete datasets and therefore uses the entropy-based MDLP discretization algorithm by [Fayyad and Irani, 1993](http://web.donga.ac.kr/kjunwoo/files/Multi%20interval%20discretization%20of%20continuous%20valued%20attributes%20for%20classification%20learning.pdf). 
-
-*(The maximum number of allowed splits in each partition is exposed through the `max_num_splits` keyword argument of the `RACERPreprocessor` which defaults to 32)*
+RACER is designed specifically for discrete datasets and therefore uses the entropy-based MDLP discretization algorithm by [Fayyad and Irani, 1993](http://web.donga.ac.kr/kjunwoo/files/Multi%20interval%20discretization%20of%20continuous%20valued%20attributes%20for%20classification%20learning.pdf) for binary tasks and an [optimal binning strategy](https://arxiv.org/abs/2001.08025) for the multiclass case. The code is also heavily documented for ease of usage.
 
 Please consider citing this work if you use it in an academic setting.
 
 [![DOI](https://zenodo.org/badge/656323287.svg)](https://zenodo.org/badge/latestdoi/656323287)
 
 ## Installation
 [![PyPI version](https://badge.fury.io/py/pyracer.svg)](https://badge.fury.io/py/pyracer)
@@ -51,17 +49,17 @@
 )
 
 X = df.drop(columns=['animal_name', 'type']).astype('category')
 Y = df[['type']].astype('category')
 ```
 
 ### RACER Preprocessing Step
-RACER requires a preprocessing step to be performed on the data **prior to** splitting into test and train portions. This step discretizes continous features and then converts each feature into a [dummy encoded](https://datascience.stackexchange.com/questions/98172/what-is-the-difference-between-one-hot-and-dummy-encoding) variable.
+RACER requires a preprocessing step to be performed on the data **prior to** splitting into test and train portions. This step discretizes continous features and then converts each feature into a [dummy encoded](https://datascience.stackexchange.com/questions/98172/what-is-the-difference-between-one-hot-and-dummy-encoding) variable. Note that since different discretization methods are used for multiclass and binary classification tasks you need to either specify the task using the `target` keyword argument or leave it to default to `"auto"` which attempts to infer your task when you call `fit_transform(X,y)` from the number of unique values in `y`.
 ```python
-X, Y = RACERPreprocessor().fit_transform(X, Y)
+X, Y = RACERPreprocessor(target="multiclass").fit_transform(X, Y)
 
 X_train, X_test, Y_train, Y_test = train_test_split(X,Y, random_state=1, test_size=0.3)
 ```
 
 ### Fitting RACER on the Dataset
 RACER provides a `benchmark` keyword argument that can be used to time the `fit` method. Moreover, the hyperparameter `alpha` can be set using its respective keyword argument. (Note that `beta` is uniquely determined as `1.0 - alpha` and is therefore not exposed through a keyword argument)
 ```python
@@ -85,16 +83,17 @@
 	[101001101001110101101101100000011111] --> [0001000] (3) | 0.9571428571428571
 	[101011101011011010111110101011111011] --> [0000001] (6) | 0.9542857142857143
 	[111001101110101010011110000010101010] --> [0000010] (5) | 0.9535714285714285
 	[101011101011111101111110101000011011] --> [0010000] (2) | 0.9528571428571428
 	[101001101001110101011110001000101010] --> [0000100] (4) | 0.9521428571428571
 	[101001101010101010011010100000101010] --> [0000001] (6) | 0.9507142857142856
 ```
-## TODO
-- Add another example notebook featuring Scikit-learn's built-in datasets.
+## To Do
+- ~Add another example notebook featuring Scikit-learn's built-in datasets.~
+- Unify discretization algorithms for all tasks.
 
 ## Issues and Feature Requests
 Found a problem within the implementation or an inconsistency with the original algorithm? Or maybe you would like to request a feature? Please feel free to [submit a PR](https://github.com/Adversarian/RACER/pulls) or [create a new issue](https://github.com/Adversarian/RACER/issues).
 
 ## Official Paper
 ```bibtex
 @Article{Basiri2019,
```

### Comparing `pyracer-1.1.0/pyracer.egg-info/PKG-INFO` & `pyracer-1.1.1/pyracer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracer
-Version: 1.1.0
+Version: 1.1.1
 Summary: Unofficial Python implementation of the RACER classification algorithm.
 Home-page: https://github.com/Adversarian/RACER
 Author: Arian Tashakkor, Mohammad Safaiyan
 Author-email: a77physics@gmail.com
 License: MIT
 Keywords: machine learning,classification,RACER
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyracer-1.1.0/setup.py` & `pyracer-1.1.1/setup.py`

 * *Files identical despite different names*

