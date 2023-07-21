# Comparing `tmp/vaex-ml-0.9.0.tar.gz` & `tmp/vaex-ml-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vaex-ml-0.9.0.tar", last modified: Mon May 25 19:32:00 2020, max compression
+gzip compressed data, was "dist/vaex-ml-1.0.0a1.tar", last modified: Fri Sep 10 11:02:02 2021, max compression
```

## Comparing `vaex-ml-0.9.0.tar` & `vaex-ml-1.0.0a1.tar`

### file list

```diff
@@ -1,37 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-25 19:32:00.000000 vaex-ml-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (116)     1087 2020-05-25 19:31:47.000000 vaex-ml-0.9.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)       93 2020-05-25 19:31:47.000000 vaex-ml-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      258 2020-05-25 19:32:00.000000 vaex-ml-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-05-25 19:32:00.000000 vaex-ml-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      930 2020-05-25 19:31:47.000000 vaex-ml-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-25 19:32:00.000000 vaex-ml-0.9.0/vaex/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-25 19:32:00.000000 vaex-ml-0.9.0/vaex/ml/
--rw-r--r--   0 runner    (1001) docker     (116)    10978 2020-05-25 19:31:47.000000 vaex-ml-0.9.0/vaex/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       52 2020-05-25 19:31:47.000000 vaex-ml-0.9.0/vaex/ml/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     7415 2020-05-25 19:31:47.000000 vaex-ml-0.9.0/vaex/ml/catboost.py
--rw-r--r--   0 runner    (1001) docker     (116)    10183 2020-05-25 19:31:47.000000 vaex-ml-0.9.0/vaex/ml/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-25 19:32:00.000000 vaex-ml-0.9.0/vaex/ml/datasets/
--rw-r--r--   0 runner    (1001) docker     (116)     3131 2020-05-25 19:31:47.000000 vaex-ml-0.9.0/vaex/ml/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    28712 2020-05-25 19:31:47.000000 vaex-ml-0.9.0/vaex/ml/datasets/iris.hdf5
--rw-r--r--   0 runner    (1001) docker     (116)   200901 2020-05-25 19:31:47.000000 vaex-ml-0.9.0/vaex/ml/datasets/titanic.hdf5
--rw-r--r--   0 runner    (1001) docker     (116)     2717 2020-05-25 19:31:47.000000 vaex-ml-0.9.0/vaex/ml/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-25 19:32:00.000000 vaex-ml-0.9.0/vaex/ml/incubator/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-25 19:31:47.000000 vaex-ml-0.9.0/vaex/ml/incubator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3344 2020-05-25 19:31:47.000000 vaex-ml-0.9.0/vaex/ml/incubator/annoy.py
--rw-r--r--   0 runner    (1001) docker     (116)     5033 2020-05-25 19:31:47.000000 vaex-ml-0.9.0/vaex/ml/incubator/pygbm.py
--rw-r--r--   0 runner    (1001) docker     (116)    11959 2020-05-25 19:31:47.000000 vaex-ml-0.9.0/vaex/ml/lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (116)     4090 2020-05-25 19:31:47.000000 vaex-ml-0.9.0/vaex/ml/linear_model.py
--rw-r--r--   0 runner    (1001) docker     (116)     1001 2020-05-25 19:31:47.000000 vaex-ml-0.9.0/vaex/ml/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (116)    10705 2020-05-25 19:31:47.000000 vaex-ml-0.9.0/vaex/ml/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (116)     1570 2020-05-25 19:31:47.000000 vaex-ml-0.9.0/vaex/ml/state.py
--rw-r--r--   0 runner    (1001) docker     (116)    29659 2020-05-25 19:31:47.000000 vaex-ml-0.9.0/vaex/ml/transformations.py
--rw-r--r--   0 runner    (1001) docker     (116)     2018 2020-05-25 19:31:47.000000 vaex-ml-0.9.0/vaex/ml/ui.py
--rw-r--r--   0 runner    (1001) docker     (116)     7000 2020-05-25 19:31:47.000000 vaex-ml-0.9.0/vaex/ml/xgboost.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-25 19:32:00.000000 vaex-ml-0.9.0/vaex_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      258 2020-05-25 19:32:00.000000 vaex-ml-0.9.0/vaex_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      679 2020-05-25 19:32:00.000000 vaex-ml-0.9.0/vaex_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-25 19:32:00.000000 vaex-ml-0.9.0/vaex_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       60 2020-05-25 19:32:00.000000 vaex-ml-0.9.0/vaex_ml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-25 19:32:00.000000 vaex-ml-0.9.0/vaex_ml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       43 2020-05-25 19:32:00.000000 vaex-ml-0.9.0/vaex_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        5 2020-05-25 19:32:00.000000 vaex-ml-0.9.0/vaex_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-09-10 11:02:02.000000 vaex-ml-1.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (116)     1087 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      157 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)      280 2021-09-10 11:02:02.000000 vaex-ml-1.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2021-09-10 11:02:02.000000 vaex-ml-1.0.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1235 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-09-10 11:02:02.000000 vaex-ml-1.0.0a1/vaex/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-09-10 11:02:02.000000 vaex-ml-1.0.0a1/vaex/ml/
+-rw-r--r--   0 runner    (1001) docker     (116)     4299 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)       71 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/_version.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10297 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/catboost.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10303 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-09-10 11:02:02.000000 vaex-ml-1.0.0a1/vaex/ml/datasets/
+-rw-r--r--   0 runner    (1001) docker     (116)     3110 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    28712 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/datasets/iris.hdf5
+-rw-r--r--   0 runner    (1001) docker     (116)   200901 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/datasets/titanic.hdf5
+-rw-r--r--   0 runner    (1001) docker     (116)     3521 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-09-10 11:02:02.000000 vaex-ml-1.0.0a1/vaex/ml/incubator/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/incubator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3344 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/incubator/annoy.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5033 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/incubator/pygbm.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6086 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/incubator/river.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7649 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4055 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/linear_model.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12703 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1001 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11657 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (116)    71052 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/spec.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1350 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/spec.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1859 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/state.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9004 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (116)    51516 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1902 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/ui.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7039 2021-09-10 11:01:52.000000 vaex-ml-1.0.0a1/vaex/ml/xgboost.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-09-10 11:02:02.000000 vaex-ml-1.0.0a1/vaex_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      280 2021-09-10 11:02:02.000000 vaex-ml-1.0.0a1/vaex_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      781 2021-09-10 11:02:02.000000 vaex-ml-1.0.0a1/vaex_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-09-10 11:02:02.000000 vaex-ml-1.0.0a1/vaex_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      177 2021-09-10 11:02:02.000000 vaex-ml-1.0.0a1/vaex_ml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-09-10 11:02:02.000000 vaex-ml-1.0.0a1/vaex_ml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       98 2021-09-10 11:02:02.000000 vaex-ml-1.0.0a1/vaex_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        5 2021-09-10 11:02:02.000000 vaex-ml-1.0.0a1/vaex_ml.egg-info/top_level.txt
```

### Comparing `vaex-ml-0.9.0/LICENSE.txt` & `vaex-ml-1.0.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vaex-ml-0.9.0/setup.py` & `vaex-ml-1.0.0a1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,22 +8,25 @@
 
 name        = 'vaex'
 author      = 'Jovan Veljanoski'
 author_email= 'jovan.veljanoski@gmail.com'
 license     = 'MIT'
 version     = version.__version__
 url         = 'https://www.github.com/vaexio/vaex'
-install_requires_ml = ['vaex-core>=2.0.0,<3', 'numba', 'traitlets', 'jinja2']
+install_requires_ml = ['vaex-core>=5.0.0-alpha.1,<6', 'numba', 'traitlets', 'jinja2']
 
 setup(name=name + '-ml',
       version=version,
       description='Machine learning support for vaex',
       url=url,
       author=author,
       author_email=author_email,
       install_requires=install_requires_ml,
+      extras_require={'all': ['tensorflow>=2.1.0', 'tensorflow-io>=0.12.0']},
       license=license,
       packages=['vaex.ml', 'vaex.ml.incubator', 'vaex.ml.datasets'],
       include_package_data=True,
       zip_safe=False,
-      entry_points={'vaex.dataframe.accessor': ['ml = vaex.ml:DataFrameAccessorML']}
+      entry_points={'vaex.dataframe.accessor': ['ml = vaex.ml:DataFrameAccessorML',
+                                                'ml.tensorflow = vaex.ml.tensorflow:DataFrameAccessorTensorflow',
+                                                'ml.metrics = vaex.ml.metrics:DataFrameAccessorMetrics']}
 )
```

### Comparing `vaex-ml-0.9.0/vaex/ml/catboost.py` & `vaex-ml-1.0.0a1/vaex/ml/lightgbm.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,146 +1,161 @@
 import base64
 import tempfile
+
+from vaex.strings import array
+
+import lightgbm
+
+import numpy as np
+
 import traitlets
 
 import vaex
 import vaex.serialize
-from . import state
-from . import generate
 
-import numpy as np
-import catboost
+from . import generate
+from . import state
 
 
 @vaex.serialize.register
 @generate.register
-class CatBoostModel(state.HasState):
-    '''The CatBoost algorithm.
+class LightGBMModel(state.HasState):
+    '''The LightGBM algorithm.
 
-    This class provides an interface to the CatBoost aloritham.
-    CatBoost is a fast, scalable, high performance Gradient Boosting on
-    Decision Trees library, used for ranking, classification, regression and
-    other machine learning tasks. For more information please visit
-    https://github.com/catboost/catboost
+    This class provides an interface to the LightGBM algorithm, with some optimizations
+    for better memory efficiency when training large datasets. The algorithm itself is
+    not modified at all.
+
+    LightGBM is a fast gradient boosting algorithm based on decision trees and is
+    mainly used for classification, regression and ranking tasks. It is under the
+    umbrella of the Distributed Machine Learning Toolkit (DMTK) project of Microsoft.
+    For more information, please visit https://github.com/Microsoft/LightGBM/.
 
     Example:
 
-    >>> import vaex
-    >>> import vaex.ml.catboost
+    >>> import vaex.ml
+    >>> import vaex.ml.lightgbm
     >>> df = vaex.ml.datasets.load_iris()
     >>> features = ['sepal_width', 'petal_length', 'sepal_length', 'petal_width']
     >>> df_train, df_test = df.ml.train_test_split()
     >>> params = {
-        'leaf_estimation_method': 'Gradient',
+        'boosting': 'gbdt',
+        'max_depth': 5,
         'learning_rate': 0.1,
-        'max_depth': 3,
-        'bootstrap_type': 'Bernoulli',
-        'objective': 'MultiClass',
-        'eval_metric': 'MultiClass',
-        'subsample': 0.8,
-        'random_state': 42,
-        'verbose': 0}
-    >>> booster = vaex.ml.catboost.CatBoostModel(features=features, target='class_', num_boost_round=100, params=params)
+        'application': 'multiclass',
+        'num_class': 3,
+        'subsample': 0.80,
+        'colsample_bytree': 0.80}
+    >>> booster = vaex.ml.lightgbm.LightGBMModel(features=features, target='class_', num_boost_round=100, params=params)
     >>> booster.fit(df_train)
     >>> df_train = booster.transform(df_train)
     >>> df_train.head(3)
-    #    sepal_length    sepal_width    petal_length    petal_width    class_  catboost_prediction
-    0             5.4            3               4.5            1.5         1  [0.00615039 0.98024259 0.01360702]
-    1             4.8            3.4             1.6            0.2         0  [0.99034267 0.00526382 0.0043935 ]
-    2             6.9            3.1             4.9            1.5         1  [0.00688241 0.95190908 0.04120851]
+     #    sepal_width    petal_length    sepal_length    petal_width    class_    lightgbm_prediction
+     0            3               4.5             5.4            1.5         1    [0.00165619 0.98097899 0.01736482]
+     1            3.4             1.6             4.8            0.2         0    [9.99803930e-01 1.17346471e-04 7.87235133e-05]
+     2            3.1             4.9             6.9            1.5         1    [0.00107541 0.9848717  0.01405289]
     >>> df_test = booster.transform(df_test)
     >>> df_test.head(3)
-    #    sepal_length    sepal_width    petal_length    petal_width    class_  catboost_prediction
-    0             5.9            3               4.2            1.5         1  [0.00464228 0.98883351 0.00652421]
-    1             6.1            3               4.6            1.4         1  [0.00350424 0.9882139  0.00828186]
-    2             6.6            2.9             4.6            1.3         1  [0.00325705 0.98891631 0.00782664]
+     #    sepal_width    petal_length    sepal_length    petal_width    class_    lightgbm_prediction
+     0            3               4.2             5.9            1.5         1    [0.00208904 0.9821348  0.01577616]
+     1            3               4.6             6.1            1.4         1    [0.00182039 0.98491357 0.01326604]
+     2            2.9             4.6             6.6            1.3         1    [2.50915444e-04 9.98431777e-01 1.31730785e-03]
     '''
-
-    features = traitlets.List(traitlets.Unicode(), help='List of features to use when fitting the CatBoostModel.')
+    snake_name = 'lightgbm_model'
+    features = traitlets.List(traitlets.Unicode(), help='List of features to use when fitting the LightGBMModel.')
     target = traitlets.Unicode(allow_none=False, help='The name of the target column.')
-    num_boost_round = traitlets.CInt(default_value=None, allow_none=True, help='Number of boosting iterations.')
-    params = traitlets.Dict(help='A dictionary of parameters to be passed on to the CatBoostModel model.')
-    pool_params = traitlets.Dict(default_value={}, help='A dictionary of parameters to be passed to the Pool data object construction')
-    prediction_name = traitlets.Unicode(default_value='catboost_prediction', help='The name of the virtual column housing the predictions.')
-    prediction_type = traitlets.Enum(values=['Probability', 'Class', 'RawFormulaVal'], default_value='Probability',
-                                     help='The form of the predictions. Can be "RawFormulaVal", "Probability" or "Class".')
+    num_boost_round = traitlets.CInt(help='Number of boosting iterations.')
+    params = traitlets.Dict(help='parameters to be passed on the to the LightGBM model.')
+    prediction_name = traitlets.Unicode(default_value='lightgbm_prediction', help='The name of the virtual column housing the predictions.')
 
     def __call__(self, *args):
-        data2d = np.vstack([arg.astype(np.float64) for arg in args]).T.copy()
-        dmatrix = catboost.Pool(data2d, **self.pool_params)
-        return self.booster.predict(dmatrix, prediction_type=self.prediction_type)
+        data2d = np.stack([np.asarray(arg, np.float64) for arg in args], axis=1)
+        return self.booster.predict(data2d)
 
     def transform(self, df):
-        '''Transform a DataFrame such that it contains the predictions of the CatBoostModel in form of a virtual column.
+        '''Transform a DataFrame such that it contains the predictions of the LightGBMModel
+        in form of a virtual column.
 
-        :param df: A vaex DataFrame. It should have the same columns as the DataFrame used to train the model.
+        :param df: A vaex DataFrame.
 
-        :return copy: A shallow copy of the DataFrame that includes the CatBoostModel prediction as a virtual column.
+        :return copy: A shallow copy of the DataFrame that includes the LightGBMModel prediction as a virtual column.
         :rtype: DataFrame
         '''
         copy = df.copy()
-        lazy_function = copy.add_function('catboost_prediction_function', self, unique=True)
+        lazy_function = copy.add_function('lightgbm_prediction_function', self, unique=True)
         expression = lazy_function(*self.features)
         copy.add_virtual_column(self.prediction_name, expression, unique=False)
         return copy
 
-    def fit(self, df, evals=None, early_stopping_rounds=None, verbose_eval=None, plot=False, **kwargs):
-        '''Fit the CatBoostModel model given a DataFrame.
-        This method accepts all key word arguments for the catboost.train method.
+    def fit(self, df, valid_sets=None, valid_names=None, early_stopping_rounds=None, evals_result=None, verbose_eval=None, **kwargs):
+        """Fit the LightGBMModel to the DataFrame.
+
+        The model will train until the validation score stops improving.
+        Validation score needs to improve at least every *early_stopping_rounds* rounds
+        to continue training. Requires at least one validation DataFrame, metric
+        specified. If there's more than one, will check all of them, but the
+        training data is ignored anyway. If early stopping occurs, the model
+        will add ``best_iteration`` field to the booster object.
 
         :param df: A vaex DataFrame containing the features and target on which to train the model.
-        :param evals: A list of DataFrames to be evaluated during training.
-            This allows user to watch performance on the validation sets.
-        :param int early_stopping_rounds: Activates early stopping.
-        :param bool verbose_eval: Requires at least one item in *evals*.
+        :param list valid_sets: A list of DataFrames to be used for validation.
+        :param list valid_names: A list of strings to label the validation sets.
+        :param early_stopping_rounds int: Activates early stopping.
+        :param dict evals_result: A dictionary storing the evaluation results of all *valid_sets*.
+        :param bool verbose_eval: Requires at least one item in *valid_sets*.
             If *verbose_eval* is True then the evaluation metric on the validation set is printed at each boosting stage.
-        :param bool plot: if True, display an interactive widget in the Jupyter
-            notebook of how the train and validation sets score on each boosting iteration.
-        '''
+        """
+
+        dtrain = lightgbm.Dataset(df[self.features].values, df[self.target].to_numpy())
+        if valid_sets is not None:
+            for i, item in enumerate(valid_sets):
+                valid_sets[i] = lightgbm.Dataset(item[self.features].values, item[self.target].to_numpy())
+        else:
+            valid_sets = ()
 
-        data = df[self.features].values
-        target_data = df[self.target].values
-        dtrain = catboost.Pool(data=data, label=target_data, **self.pool_params)
-        if evals is not None:
-            for i, item in enumerate(evals):
-                data = item[self.features].values
-                target_data = item[self.target].values
-                evals[i] = catboost.Pool(data=data, label=target_data, **self.pool_params)
-
-        # This does the actual training/fitting of the catboost model
-        self.booster = catboost.train(params=self.params,
-                                      dtrain=dtrain,
+        self.booster = lightgbm.train(params=self.params,
+                                      train_set=dtrain,
                                       num_boost_round=self.num_boost_round,
-                                      evals=evals,
+                                      valid_sets=valid_sets,
+                                      valid_names=valid_names,
                                       early_stopping_rounds=early_stopping_rounds,
+                                      evals_result=evals_result,
                                       verbose_eval=verbose_eval,
-                                      plot=plot,
                                       **kwargs)
 
     def predict(self, df, **kwargs):
-        '''Provided a vaex DataFrame, get an in-memory numpy array with the predictions from the CatBoostModel model.
-        This method accepts the key word arguments of the predict method from catboost.
+        '''Get an in-memory numpy array with the predictions of the LightGBMModel on a vaex DataFrame.
+        This method accepts the key word arguments of the predict method from LightGBM.
 
-        :param df: a vaex DataFrame
+        :param df: A vaex DataFrame.
 
-        :returns: A in-memory numpy array containing the CatBoostModel predictions.
+        :returns: A in-memory numpy array containing the LightGBMModel predictions.
         :rtype: numpy.array
         '''
-        data = df[self.features].values
-        dmatrix = catboost.Pool(data, **self.pool_params)
-        return self.booster.predict(dmatrix, prediction_type=self.prediction_type, **kwargs)
+        # TODO: we want to go multithreaded/parallel/chunks
+        return self.booster.predict(df[self.features].values)
 
     def state_get(self):
         filename = tempfile.mktemp()
         self.booster.save_model(filename)
         with open(filename, 'rb') as f:
             data = f.read()
         return dict(tree_state=base64.encodebytes(data).decode('ascii'),
-                    substate=super(CatBoostModel, self).state_get())
+                    substate=super(LightGBMModel, self).state_get())
 
     def state_set(self, state, trusted=True):
-        super(CatBoostModel, self).state_set(state['substate'])
+        super(LightGBMModel, self).state_set(state['substate'])
         data = base64.decodebytes(state['tree_state'].encode('ascii'))
         filename = tempfile.mktemp()
         with open(filename, 'wb') as f:
             f.write(data)
-        self.booster = catboost.CatBoost().load_model(fname=filename)
+        self.booster = lightgbm.Booster(model_file=filename)
+
+
+if __name__ == "__main__":
+    df = vaex.ml.iris()
+    features = ['sepal_length', 'sepal_width', 'petal_length', 'petal_width']
+    ldf = lightgbm.Dataset(np.array(df[features]), df.data.class_)
+    param = {'num_leaves': 31, 'num_trees': 100, 'objective': 'softmax', 'num_class': 3}
+    num_boost_round = 30
+    booster = lightgbm.train(param, ldf, num_boost_round)
+    print(booster.predict(np.array(df[features])))
```

### Comparing `vaex-ml-0.9.0/vaex/ml/cluster.py` & `vaex-ml-1.0.0a1/vaex/ml/cluster.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import traitlets
-import vaex.ml.state
+import vaex.ml.transformations
 import logging
 import vaex
 import vaex.serialize
 from numba import jit
 from . import generate
 # vaex.set_log_level_debug()
 
@@ -59,15 +59,15 @@
                 counts[run, cls] += 1
 #    return inertia
         # for i in range(k):
 
 
 @vaex.serialize.register
 @generate.register
-class KMeans(vaex.ml.state.HasState):
+class KMeans(vaex.ml.transformations.Transformer):
     '''The KMeans clustering algorithm.
 
     Example:
 
     >>> import vaex.ml
     >>> import vaex.ml.cluster
     >>> df = vaex.ml.datasets.load_iris()
@@ -79,54 +79,55 @@
      #    sepal_width    petal_length    sepal_length    petal_width    class_    prediction_kmeans
      0            3               4.2             5.9            1.5         1                    2
      1            3               4.6             6.1            1.4         1                    2
      2            2.9             4.6             6.6            1.3         1                    2
      3            3.3             5.7             6.7            2.1         2                    0
      4            4.2             1.4             5.5            0.2         0                    1
     '''
+    snake_name = 'kmeans'
     features = traitlets.List(traitlets.Unicode(), help='List of features to cluster.')
     n_clusters = traitlets.CInt(default_value=2, help='Number of clusters to form.')
     init = traitlets.Union([Matrix(), traitlets.Unicode()], default_value='random', help='Method for initializing the centroids.')
     n_init = traitlets.CInt(default_value=1, help='Number of centroid initializations. \
                                                    The KMeans algorithm will be run for each initialization, \
                                                    and the final results will be the best output of the n_init \
                                                    consecutive runs in terms of inertia.')
     max_iter = traitlets.CInt(default_value=300, help='Maximum number of iterations of the KMeans algorithm for a single run.')
-    random_state = traitlets.CInt(default_value=None, allow_none=True, help='Random number generation for centroid initialization. \
-                                                                             If an int is specified, the randomness becomes deterministic.')
+    random_state = traitlets.CInt(default_value=None, allow_none=True, help='Random number generation for centroid initialization. If an int is specified, the randomness becomes deterministic.')
     verbose = traitlets.CBool(default_value=False, help='If True, enable verbosity mode.')
     cluster_centers = traitlets.List(traitlets.List(traitlets.CFloat()), help='Coordinates of cluster centers.')
     inertia = traitlets.CFloat(default_value=None, allow_none=True, help='Sum of squared distances of samples to their closest cluster center.')
     prediction_label = traitlets.Unicode(default_value='prediction_kmeans', help='The name of the virtual column that houses the cluster labels for each point.')
 
     def __call__(self, *blocks):
         return self._calculate_classes(*blocks)
 
     def _calculate_distances_squared(self, *blocks):
         N = len(blocks[0])  # they are all the same length
+        blocks = [np.asarray(k) for k in blocks]
         centroids = np.array(self.cluster_centers)
         k = centroids.shape[0]
         dimensions = centroids.shape[1]
         distances_sq = np.zeros((k, N))
-        if 1:
+        if True:
             distances_square(distances_sq, centroids, *blocks)
         else:
             for d in range(dimensions):
                 for i in range(k):
                     distances_sq[i] += (blocks[d] - centroids[i][d])**2
         return distances_sq
 
     def _calculate_classes(self, *blocks):
         distances_sq = self._calculate_distances_squared(*blocks)
         classes = np.argmin(distances_sq, axis=0)
         return classes
 
     def generate_cluster_centers_random(self, dataframe, rng):
         indices = rng.randint(0, len(dataframe), self.n_clusters)
-        return [[dataframe.evaluate(feature, i1=i, i2=i+1)[0] for feature in self.features] for i in indices]
+        return [[dataframe.evaluate(feature, i1=i, i2=i+1, array_type='python')[0] for feature in self.features] for i in indices]
 
     def transform(self, dataframe):
         '''
         Label a DataFrame with a fitted KMeans model.
 
         :param dataframe: A vaex DataFrame.
 
@@ -191,21 +192,22 @@
     def _find_centers_and_inertias(self, dataframe, done):
         done = np.array(done, dtype=np.int8)
         centroids = np.array(self.run_cluster_centers)
         runs = centroids.shape[0]
         clusters = centroids.shape[1]
         dimensions = centroids.shape[2]
         # print("k =", k)
-        assert dimensions == len(self.features), "nr of dimensions for centroid should equal nr of features"
+        assert dimensions == len(self.features), "The number of dimensions for the centroid should equal the number of features."
 
         def map(*blocks):  # this will be called with a chunk of the data
             sumpos = np.zeros((runs, clusters, dimensions))
             counts = np.zeros((runs, clusters))
             inertia = np.zeros((runs))
-            if 1:
+            blocks = [np.asarray(k) for k in blocks]
+            if True:
                 centroid_stats(centroids, counts, sumpos, inertia,  *blocks)
             else:
                 # this is the pure python code
                 # although not made for multiple runs yet
                 distances_sq = self._calculate_distances_squared(*blocks)
                 classes = np.argmin(distances_sq, axis=0)
                 distances_sq = np.choose(classes, distances_sq)
```

### Comparing `vaex-ml-0.9.0/vaex/ml/datasets/__init__.py` & `vaex-ml-1.0.0a1/vaex/ml/datasets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 def _iris(name, iris_previous, N):
     filename = os.path.join(vaex.utils.get_private_dir('data'), name + '.hdf5')
     if os.path.exists(filename):
         return vaex.open(filename)
     else:
         iris = iris_previous()
         repeat = int(np.ceil(N / len(iris)))
-        ds = vaex.dataset.DatasetConcatenated([iris] * repeat)
+        ds = vaex.concat([iris] * repeat)
         ds.export_hdf5(filename)
         return vaex.open(filename)
 
 
 def iris_subsample(N, error_percentage=5, ds=None):
     '''Returns the iris set repeated so it include ~1e4 rows'''
     # return _iris_subsample('iris_1e4', iris, int(1e4))
```

### Comparing `vaex-ml-0.9.0/vaex/ml/datasets/iris.hdf5` & `vaex-ml-1.0.0a1/vaex/ml/datasets/iris.hdf5`

 * *Files identical despite different names*

### Comparing `vaex-ml-0.9.0/vaex/ml/datasets/titanic.hdf5` & `vaex-ml-1.0.0a1/vaex/ml/datasets/titanic.hdf5`

 * *Files identical despite different names*

### Comparing `vaex-ml-0.9.0/vaex/ml/generate.py` & `vaex-ml-1.0.0a1/vaex/ml/generate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,44 @@
 from collections import defaultdict
+import functools
 import os
 import re
 import sys
 
 from jinja2 import Template
 import traitlets
 
 import vaex
 
 # registry = {}
 registry = []
 
 
+# 'copied' from vaex.dataframe, if ML transformers are normal transformers, get rid of this
+def _transformer(name=None):
+    def wrapper_outter(method):
+        method_name = name or method.__name__
+        @functools.wraps(method)
+        def wrapper(self, df, *args, **kwargs):
+            # if self._future_behaviour == 5:
+            previous = df.pipeline.transformer
+            df = method(self, df, *args, **kwargs)
+            transformer = vaex.transformer.ML(self, previous=previous)
+            df.pipeline.transformer = transformer
+            # else:
+            #     df = method(self, *args, **kwargs)
+            return df
+        return wrapper
+    return wrapper_outter
+
+
+
 def register(cls):
+    cls.transform = _transformer()(cls.transform)
+    registry.append(cls)
     docstring_args_template = Template("""
 {% for arg in docargs %}
 :param {{ arg.name }}: {{ arg.help }}{% endfor %}
 """)
 
     template_method = Template("""
 
@@ -27,21 +49,21 @@
     obj = {{module}}.{{ class_name }}({{ args }})
     obj.fit(self{{ extra_fit }})
     return obj
 
 import vaex.dataframe
 # vaex.dataframe.DataFrame.ml._add({{ method_name }}={{ method_name }})
 
-def __init__(self, {{ full_signature }}):
+def __init__(self, {{ full_signature }}, **kwargs):
     \"\"\"
     {{ docstring_args }}
     \"\"\"
     given_kwargs = {key:value for key, value in dict({{ full_args }}).items() if value is not traitlets.Undefined}
 
-    super({{module}}.{{ class_name }}, self).__init__(**given_kwargs)
+    super({{module}}.{{ class_name }}, self).__init__(**given_kwargs, **kwargs)
 
 cls.__init__ = __init__
 cls.__signature__ = __init__
 del __init__
     """)
     traits = {key: value for key, value in cls.class_traits().items()
                 if 'output' not in value.metadata}
```

### Comparing `vaex-ml-0.9.0/vaex/ml/incubator/annoy.py` & `vaex-ml-1.0.0a1/vaex/ml/incubator/annoy.py`

 * *Files identical despite different names*

### Comparing `vaex-ml-0.9.0/vaex/ml/incubator/pygbm.py` & `vaex-ml-1.0.0a1/vaex/ml/incubator/pygbm.py`

 * *Files identical despite different names*

### Comparing `vaex-ml-0.9.0/vaex/ml/lightgbm.py` & `vaex-ml-1.0.0a1/vaex/ml/catboost.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,233 +1,193 @@
-import ctypes
-import math
-import warnings
+import base64
+import tempfile
+import traitlets
 
 import vaex
-import lightgbm
-import numpy as np
-import tempfile
-import base64
 import vaex.serialize
 from . import state
-import traitlets
 from . import generate
 
-
-lib = lightgbm.basic._LIB
+import numpy as np
+import catboost
 
 
 @vaex.serialize.register
 @generate.register
-class LightGBMModel(state.HasState):
-    '''The LightGBM algorithm.
+class CatBoostModel(state.HasState):
+    '''The CatBoost algorithm.
 
-    This class provides an interface to the LightGBM algorithm, with some optimizations
-    for better memory efficiency when training large datasets. The algorithm itself is
-    not modified at all.
-
-    LightGBM is a fast gradient boosting algorithm based on decision trees and is
-    mainly used for classification, regression and ranking tasks. It is under the
-    umbrella of the Distributed Machine Learning Toolkit (DMTK) project of Microsoft.
-    For more information, please visit https://github.com/Microsoft/LightGBM/.
+    This class provides an interface to the CatBoost aloritham.
+    CatBoost is a fast, scalable, high performance Gradient Boosting on
+    Decision Trees library, used for ranking, classification, regression and
+    other machine learning tasks. For more information please visit
+    https://github.com/catboost/catboost
 
     Example:
 
-    >>> import vaex.ml
-    >>> import vaex.ml.lightgbm
+    >>> import vaex
+    >>> import vaex.ml.catboost
     >>> df = vaex.ml.datasets.load_iris()
     >>> features = ['sepal_width', 'petal_length', 'sepal_length', 'petal_width']
     >>> df_train, df_test = df.ml.train_test_split()
     >>> params = {
-        'boosting': 'gbdt',
-        'max_depth': 5,
+        'leaf_estimation_method': 'Gradient',
         'learning_rate': 0.1,
-        'application': 'multiclass',
-        'num_class': 3,
-        'subsample': 0.80,
-        'colsample_bytree': 0.80}
-    >>> booster = vaex.ml.lightgbm.LightGBMModel(features=features, target='class_', num_boost_round=100, params=params)
+        'max_depth': 3,
+        'bootstrap_type': 'Bernoulli',
+        'objective': 'MultiClass',
+        'eval_metric': 'MultiClass',
+        'subsample': 0.8,
+        'random_state': 42,
+        'verbose': 0}
+    >>> booster = vaex.ml.catboost.CatBoostModel(features=features, target='class_', num_boost_round=100, params=params)
     >>> booster.fit(df_train)
     >>> df_train = booster.transform(df_train)
     >>> df_train.head(3)
-     #    sepal_width    petal_length    sepal_length    petal_width    class_    lightgbm_prediction
-     0            3               4.5             5.4            1.5         1    [0.00165619 0.98097899 0.01736482]
-     1            3.4             1.6             4.8            0.2         0    [9.99803930e-01 1.17346471e-04 7.87235133e-05]
-     2            3.1             4.9             6.9            1.5         1    [0.00107541 0.9848717  0.01405289]
+    #    sepal_length    sepal_width    petal_length    petal_width    class_  catboost_prediction
+    0             5.4            3               4.5            1.5         1  [0.00615039 0.98024259 0.01360702]
+    1             4.8            3.4             1.6            0.2         0  [0.99034267 0.00526382 0.0043935 ]
+    2             6.9            3.1             4.9            1.5         1  [0.00688241 0.95190908 0.04120851]
     >>> df_test = booster.transform(df_test)
     >>> df_test.head(3)
-     #    sepal_width    petal_length    sepal_length    petal_width    class_    lightgbm_prediction
-     0            3               4.2             5.9            1.5         1    [0.00208904 0.9821348  0.01577616]
-     1            3               4.6             6.1            1.4         1    [0.00182039 0.98491357 0.01326604]
-     2            2.9             4.6             6.6            1.3         1    [2.50915444e-04 9.98431777e-01 1.31730785e-03]
+    #    sepal_length    sepal_width    petal_length    petal_width    class_  catboost_prediction
+    0             5.9            3               4.2            1.5         1  [0.00464228 0.98883351 0.00652421]
+    1             6.1            3               4.6            1.4         1  [0.00350424 0.9882139  0.00828186]
+    2             6.6            2.9             4.6            1.3         1  [0.00325705 0.98891631 0.00782664]
     '''
-    features = traitlets.List(traitlets.Unicode(), help='List of features to use when fitting the LightGBMModel.')
+    snake_name = "catboost_model"
+    features = traitlets.List(traitlets.Unicode(), help='List of features to use when fitting the CatBoostModel.')
     target = traitlets.Unicode(allow_none=False, help='The name of the target column.')
-    num_boost_round = traitlets.CInt(help='Number of boosting iterations.')
-    params = traitlets.Dict(help='parameters to be passed on the to the LightGBM model.')
-    prediction_name = traitlets.Unicode(default_value='lightgbm_prediction', help='The name of the virtual column housing the predictions.')
+    num_boost_round = traitlets.CInt(default_value=None, allow_none=True, help='Number of boosting iterations.')
+    params = traitlets.Dict(help='A dictionary of parameters to be passed on to the CatBoostModel model.')
+    pool_params = traitlets.Dict(default_value={}, help='A dictionary of parameters to be passed to the Pool data object construction')
+    prediction_name = traitlets.Unicode(default_value='catboost_prediction', help='The name of the virtual column housing the predictions.')
+    prediction_type = traitlets.Enum(values=['Probability', 'Class', 'RawFormulaVal'], default_value='Probability',
+                                     help='The form of the predictions. Can be "RawFormulaVal", "Probability" or "Class".')
+    batch_size = traitlets.CInt(default_value=None, allow_none=True, help='If provided, will train in batches of this size.')
+    batch_weights = traitlets.List(traitlets.Float(), default_value=[], allow_none=True, help='Weights to sum models at the end of training in batches.')
+    evals_result_ = traitlets.List(traitlets.Dict(), default_value=[], help="Evaluation results")
+    ctr_merge_policy = traitlets.Enum(values=['FailIfCtrsIntersects', 'LeaveMostDiversifiedTable', 'IntersectingCountersAverage'],
+                                      default_value='IntersectingCountersAverage', help="Strategy for summing up models. Only used when training in batches. See the CatBoost documentation for more info.")
 
     def __call__(self, *args):
-        data2d = np.vstack([arg.astype(np.float64) for arg in args]).T.copy()
-        return self.booster.predict(data2d)
+        data2d = np.stack([np.asarray(arg, np.float64) for arg in args], axis=1)
+        dmatrix = catboost.Pool(data2d, **self.pool_params)
+        return self.booster.predict(dmatrix, prediction_type=self.prediction_type)
 
     def transform(self, df):
-        '''Transform a DataFrame such that it contains the predictions of the LightGBMModel
-        in form of a virtual column.
+        '''Transform a DataFrame such that it contains the predictions of the CatBoostModel in form of a virtual column.
 
-        :param df: A vaex DataFrame.
+        :param df: A vaex DataFrame. It should have the same columns as the DataFrame used to train the model.
 
-        :return copy: A shallow copy of the DataFrame that includes the LightGBMModel prediction as a virtual column.
+        :return copy: A shallow copy of the DataFrame that includes the CatBoostModel prediction as a virtual column.
         :rtype: DataFrame
         '''
         copy = df.copy()
-        lazy_function = copy.add_function('lightgbm_prediction_function', self, unique=True)
+        lazy_function = copy.add_function('catboost_prediction_function', self, unique=True)
         expression = lazy_function(*self.features)
         copy.add_virtual_column(self.prediction_name, expression, unique=False)
         return copy
 
-    def fit(self, df, valid_sets=None, valid_names=None, early_stopping_rounds=None, evals_result=None, verbose_eval=None,
-            copy=False, **kwargs):
-        """Fit the LightGBMModel to the DataFrame.
-
-        The model will train until the validation score stops improving.
-        Validation score needs to improve at least every *early_stopping_rounds* rounds
-        to continue training. Requires at least one validation DataFrame, metric
-        specified. If there's more than one, will check all of them, but the
-        training data is ignored anyway. If early stopping occurs, the model
-        will add ``best_iteration`` field to the booster object.
+    def fit(self, df, evals=None, early_stopping_rounds=None, verbose_eval=None, plot=False, progress=None, **kwargs):
+        '''Fit the CatBoostModel model given a DataFrame.
+        This method accepts all key word arguments for the catboost.train method.
 
         :param df: A vaex DataFrame containing the features and target on which to train the model.
-        :param list valid_sets: A list of DataFrames to be used for validation.
-        :param list valid_names: A list of strings to label the validation sets.
-        :param early_stopping_rounds int: Activates early stopping.
-        :param dict evals_result: A dictionary storing the evaluation results of all *valid_sets*.
-        :param bool verbose_eval: Requires at least one item in *valid_sets*.
+        :param evals: A list of DataFrames to be evaluated during training.
+            This allows user to watch performance on the validation sets.
+        :param int early_stopping_rounds: Activates early stopping.
+        :param bool verbose_eval: Requires at least one item in *evals*.
             If *verbose_eval* is True then the evaluation metric on the validation set is printed at each boosting stage.
-        :param bool copy: (default, False) If True, make an in memory copy of the data before passing it to LightGBMModel.
-        """
-
-        if copy:
-            dtrain = lightgbm.Dataset(df[self.features].values, df.evaluate(self.target))
-            if valid_sets is not None:
-                for i, item in enumerate(valid_sets):
-                    valid_sets[i] = lightgbm.Dataset(item[self.features].values, item[self.target].values)
-            else:
-                valid_sets = ()
+        :param bool plot: if True, display an interactive widget in the Jupyter
+            notebook of how the train and validation sets score on each boosting iteration.
+        :param progress: If True display a progressbar when the training is done in batches.
+        '''
+        self.pool_params['feature_names'] = self.features
+        if evals is not None:
+            for i, item in enumerate(evals):
+                data = item[self.features].values
+                target_data = item[self.target].to_numpy()
+                evals[i] = catboost.Pool(data=data, label=target_data, **self.pool_params)
+
+        # This does the actual training/fitting of the catboost model
+        if self.batch_size is None:
+            data = df[self.features].values
+            target_data = df[self.target].to_numpy()
+            dtrain = catboost.Pool(data=data, label=target_data, **self.pool_params)
+            model = catboost.train(params=self.params,
+                                   dtrain=dtrain,
+                                   num_boost_round=self.num_boost_round,
+                                   evals=evals,
+                                   early_stopping_rounds=early_stopping_rounds,
+                                   verbose_eval=verbose_eval,
+                                   plot=plot,
+                                   **kwargs)
+            self.booster = model
+            self.evals_result_ = [model.evals_result_]
+            self.feature_importances_ = list(model.feature_importances_)
         else:
-            dtrain = VaexDataset(df, self.target, features=self.features)
-            if valid_sets is not None:
-                for i, item in enumerate(valid_sets):
-                    # valid_sets[i] = VaexDataset(item, self.target, features=self.features)
-                    valid_sets[i] = lightgbm.Dataset(item[self.features].values, item[self.target].values)
-                    warnings.warn('''Validation sets do not obey the `copy=False` argument.
-                                  A standard in-memory copy is made for each validation set.''', UserWarning)
+            models = []
+
+            # Set up progressbar
+            n_samples = len(df)
+            progressbar = vaex.utils.progressbars(progress)
+
+            column_names = self.features + [self.target]
+            iterator = df[column_names].to_pandas_df(chunk_size=self.batch_size)
+            for i1, i2, chunk in iterator:
+                progressbar(i1 / n_samples)
+                data = chunk[self.features].values
+                target_data = chunk[self.target].values
+                dtrain = catboost.Pool(data=data, label=target_data, **self.pool_params)
+                model = catboost.train(params=self.params,
+                                       dtrain=dtrain,
+                                       num_boost_round=self.num_boost_round,
+                                       evals=evals,
+                                       early_stopping_rounds=early_stopping_rounds,
+                                       verbose_eval=verbose_eval,
+                                       plot=plot,
+                                       **kwargs)
+                self.evals_result_.append(model.evals_result_)
+                models.append(model)
+            progressbar(1.0)
+
+            # Weights are key when summing models
+            if len(self.batch_weights) == 0:
+                batch_weights = [1/len(models)] * len(models)
+            elif self.batch_weights is not None and len(self.batch_weights) != len(models):
+                raise ValueError("'batch_weights' must be te same length as the number of models.")
             else:
-                valid_sets = ()
+                batch_weights = self.batch_weights
+
+            # Sum the models
+            self.booster = catboost.sum_models(models, weights=batch_weights, ctr_merge_policy=self.ctr_merge_policy)
 
-        self.booster = lightgbm.train(params=self.params,
-                                      train_set=dtrain,
-                                      num_boost_round=self.num_boost_round,
-                                      valid_sets=valid_sets,
-                                      valid_names=valid_names,
-                                      early_stopping_rounds=early_stopping_rounds,
-                                      evals_result=evals_result,
-                                      verbose_eval=verbose_eval,
-                                      **kwargs)
 
     def predict(self, df, **kwargs):
-        '''Get an in-memory numpy array with the predictions of the LightGBMModel on a vaex DataFrame.
-        This method accepts the key word arguments of the predict method from LightGBM.
+        '''Provided a vaex DataFrame, get an in-memory numpy array with the predictions from the CatBoostModel model.
+        This method accepts the key word arguments of the predict method from catboost.
 
-        :param df: A vaex DataFrame.
+        :param df: a vaex DataFrame
 
-        :returns: A in-memory numpy array containing the LightGBMModel predictions.
+        :returns: A in-memory numpy array containing the CatBoostModel predictions.
         :rtype: numpy.array
         '''
-        # TODO: we want to go multithreaded/parallel/chunks
-        return self.booster.predict(df[self.features].values)
+        data = df[self.features].values
+        dmatrix = catboost.Pool(data, **self.pool_params)
+        return self.booster.predict(dmatrix, prediction_type=self.prediction_type, **kwargs)
 
     def state_get(self):
         filename = tempfile.mktemp()
         self.booster.save_model(filename)
         with open(filename, 'rb') as f:
             data = f.read()
         return dict(tree_state=base64.encodebytes(data).decode('ascii'),
-                    substate=super(LightGBMModel, self).state_get())
+                    substate=super(CatBoostModel, self).state_get())
 
     def state_set(self, state, trusted=True):
-        super(LightGBMModel, self).state_set(state['substate'])
+        super(CatBoostModel, self).state_set(state['substate'])
         data = base64.decodebytes(state['tree_state'].encode('ascii'))
         filename = tempfile.mktemp()
         with open(filename, 'wb') as f:
             f.write(data)
-        self.booster = lightgbm.Booster(model_file=filename)
-
-
-class VaexDataset(lightgbm.Dataset):
-    def __init__(self, df, label=None, features=None, blocksize=100*1000, sample_count=10*100, params={}):
-        super(VaexDataset, self).__init__(None)
-        self.df = df
-        self.features = features or self.df.get_column_names(virtual=True)
-        assert len(set(self.features)) == len(self.features), "using duplicate features"
-        self.blocksize = blocksize
-
-        self.data_references = {}
-
-        self.c_features = (ctypes.c_char_p * len(self.features))()
-        self.c_features[:] = [k.encode() for k in self.features]
-
-        self.handle = ctypes.c_void_p()
-
-        row_count = len(self.df)
-        ncol = len(self.features)
-        num_sample_row = min(sample_count, row_count)
-
-        data_list = [self.df.evaluate(k, i1=0, i2=num_sample_row).astype(np.float64) for k in self.features]
-        data_pointers = [k.ctypes.data_as(ctypes.POINTER(ctypes.c_double)) for k in data_list]
-        sample_data = (ctypes.POINTER(ctypes.c_double) * ncol)(*data_pointers)
-
-        indices = np.arange(num_sample_row, dtype=np.int32)
-        indices_pointers = [indices.ctypes.data_as(ctypes.POINTER(ctypes.c_int)) for k in range(ncol)]
-        sample_indices = (ctypes.POINTER(ctypes.c_int) * ncol)(*indices_pointers)
-        num_per_col = (ctypes.c_int * ncol)(*((num_sample_row,) * ncol))
-        parameters = ctypes.c_char_p(lightgbm.basic.param_dict_to_str(params).encode())
-
-        lightgbm.basic._safe_call(lib.LGBM_DatasetCreateFromSampledColumn(sample_data,
-                                                                          sample_indices,
-                                                                          ctypes.c_uint(ncol),
-                                                                          num_per_col,
-                                                                          ctypes.c_uint(num_sample_row),
-                                                                          ctypes.c_uint(row_count),
-                                                                          parameters,
-                                                                          ctypes.byref(self.handle)))
-
-        blocks = int(math.ceil(row_count / blocksize))
-        dtype = np.float64
-        for i in range(blocks):
-            i1 = i * blocksize
-            i2 = min(row_count, (i+1) * blocksize)
-            data = np.array([df.evaluate(k, i1=i1, i2=i2).astype(dtype) for k in self.features]).T.copy()
-            ctypemap = {np.float64: ctypes.c_double, np.float32: ctypes.c_float}
-            capi_typemap = {np.float64: lightgbm.basic.C_API_DTYPE_FLOAT64, np.float32: lightgbm.basic.C_API_DTYPE_FLOAT32}
-            lightgbm.basic._safe_call(lib.LGBM_DatasetPushRows(self.handle,
-                                                               data.ctypes.data_as(ctypes.POINTER(ctypemap[dtype])),
-                                                               ctypes.c_uint(capi_typemap[dtype]),
-                                                               ctypes.c_uint32(i2-i1),
-                                                               ctypes.c_uint32(ncol),
-                                                               ctypes.c_uint32(i1),
-                                                               ))
-
-        if label is not None:
-            self.label_data = self.df.evaluate(label)
-            self.set_label(self.label_data)
-
-
-if __name__ == "__main__":
-    df = vaex.ml.iris()
-    features = ['sepal_length', 'sepal_width', 'petal_length', 'petal_width']
-    # ldf = VaexDataset(df, 'class_', features=features)
-    ldf = lightgbm.Dataset(np.array(df[features]), df.data.class_)
-    param = {'num_leaves': 31, 'num_trees': 100, 'objective': 'softmax', 'num_class': 3}
-    num_boost_round = 30
-    booster = lightgbm.train(param, ldf, num_boost_round)
-    print(booster.predict(np.array(df[features])))
+        self.booster = catboost.CatBoost().load_model(fname=filename)
```

### Comparing `vaex-ml-0.9.0/vaex/ml/linear_model.py` & `vaex-ml-1.0.0a1/vaex/ml/linear_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,18 @@
 from . import state
 from . import generate
 
 
 def listify(l):
     if hasattr(l, 'tolist'):
         return l.tolist()
-    else:
-        try:
-            return [listify(k) for k in l]
-        except TypeError:
-            return l
+    try:
+        return [listify(k) for k in l]
+    except TypeError:
+        return l
 
 
 class _LinearBase(state.HasState):
     features = traitlets.List(traitlets.Unicode())
     binned = traitlets.CBool(True)
     shape = traitlets.CInt(64)
     limits = traitlets.List(traitlets.List(traitlets.CFloat(), allow_none=True),
@@ -62,16 +61,16 @@
             self.limits = listify(limits)
             counts = dataset.count(binby=binby, limits=limits, shape=shapes)
             mask = counts > 0
 
             def coordinates(expression, limits, shape):
                 if dataset.is_category(expression):
                     return np.arange(dataset.category_count(expression))
-                else:
-                    return dataset.bin_centers(expression, limits, shape)
+                return dataset.bin_centers(expression, limits, shape)
+                
             centers = [coordinates(expression, l, shape) for expression, l, shape
                        in zip(binby, self.limits, shapes)]
             # l = ds.bin_centers('y', limits[1], shape)
             centers = np.meshgrid(*centers, indexing='ij')
             centers = [c[mask] for c in centers]
             # m = lin.LinearRegression(fit_intercept=self.fit_intercept)
             m = self._make_model()
```

### Comparing `vaex-ml-0.9.0/vaex/ml/pipeline.py` & `vaex-ml-1.0.0a1/vaex/ml/pipeline.py`

 * *Files identical despite different names*

### Comparing `vaex-ml-0.9.0/vaex/ml/sklearn.py` & `vaex-ml-1.0.0a1/vaex/ml/sklearn.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,73 +47,75 @@
     >>> df_test = model.transform(df_test)
     >>> df_test.head(3)
      #    sepal_length    sepal_width    petal_length    petal_width    class_     pred
      0             5.9            3               4.2            1.5         1  1.39437
      1             6.1            3               4.6            1.4         1  1.56469
      2             6.6            2.9             4.6            1.3         1  1.44276
     '''
-
+    snake_name = 'sklearn_predictor'
     model = traitlets.Any(default_value=None, allow_none=True, help='A scikit-learn estimator.').tag(**serialize_pickle)
     features = traitlets.List(traitlets.Unicode(), help='List of features to use.')
-    target = traitlets.Unicode(allow_none=False, help='The name of the target column.')
+    target = traitlets.Unicode(default_value=None, allow_none=True, help='The name of the target column.')
     prediction_name = traitlets.Unicode(default_value='prediction', help='The name of the virtual column housing the predictions.')
+    prediction_type = traitlets.Enum(values=['predict', 'predict_proba', 'predict_log_proba'], default_value='predict',
+                                     help='Which method to use to get the predictions. \
+                                     Can be "predict", "predict_proba" or "predict_log_proba".')
+
+    # if not hasattr(model, prediction_type):
+    #     raise AttributeError(f'The specified sklearn model does not have a {prediction_type} attribute')
 
     def __call__(self, *args):
-        X = np.vstack([arg.astype(np.float64) for arg in args]).T.copy()
-        return self.model.predict(X)
+        X = np.stack([np.asarray(arg, np.float64) for arg in args], axis=1)
+        if self.prediction_type == 'predict':
+            return self.model.predict(X)
+        elif self.prediction_type == 'predict_proba':
+            return self.model.predict_proba(X)
+        else:
+            return self.model.predict_log_proba(X)
 
     def predict(self, df):
-        '''Get an in-memory numpy array with the predictions of the SKLearnPredictor.self
+        '''Get an in-memory numpy array with the predictions of the Predictor.
 
         :param df: A vaex DataFrame, containing the input features.
-        :returns: A in-memory numpy array containing the SKLearnPredictor predictions.
+        :returns: A in-memory numpy array containing the Predictor predictions.
         :rtype: numpy.array
         '''
-        data = df[self.features].values
-        return self.model.predict(data)
+        return self.transform(df)[self.prediction_name].values
 
     def transform(self, df):
-        '''Transform a DataFrame such that it contains the predictions of the SKLearnPredictor.
+        '''Transform a DataFrame such that it contains the predictions of the Predictor.
         in form of a virtual column.
 
         :param df: A vaex DataFrame.
 
-        :return copy: A shallow copy of the DataFrame that includes the SKLearnPredictor prediction as a virtual column.
+        :return copy: A shallow copy of the DataFrame that includes the Predictor prediction as a virtual column.
         :rtype: DataFrame
         '''
         copy = df.copy()
         lazy_function = copy.add_function('sklearn_prediction_function', self, unique=True)
         expression = lazy_function(*self.features)
         copy.add_virtual_column(self.prediction_name, expression, unique=False)
         return copy
 
     def fit(self, df, **kwargs):
-        '''Fit the SKLearnPredictor to the DataFrame.
+        '''Fit the Predictor to the DataFrame.
 
         :param df: A vaex DataFrame containing the features and target on which to train the model.
         '''
 
         X = df[self.features].values
-        y = df.evaluate(self.target)
+        if self.target is not None:
+            y = df.evaluate(self.target)
+        else:
+            y = None
         self.model.fit(X=X, y=y, **kwargs)
 
 
 @vaex.serialize.register
 @generate.register
-class SKLearnPredictor(Predictor):
-
-    def __init__(self):
-        super(SKLearnPredictor, self).__init__()
-        warnings.warn(message='''This class is deprecated and it will be removed in vaex-ml 0.8.
-                      Please use vaex.ml.sklearn.Predictor instead.''',
-                      category=DeprecationWarning)
-
-
-@vaex.serialize.register
-@generate.register
 class IncrementalPredictor(state.HasState):
     '''This class wraps any scikit-learn estimator (a.k.a predictions) that has
     a `.partial_fit` method, and makes it a vaex pipeline object.
 
     By wrapping "on-line" scikit-learn estimators with this class, they become a vaex
     pipeline object. Thus, they can take full advantage of the serialization and
     pipeline system of vaex. While the underlying estimator need to call the
@@ -161,33 +163,41 @@
       #        FeH    pred_FeH
       0  -2.30923     -1.66226
       1  -1.78874     -1.68218
       2  -0.761811    -1.59562
       3  -1.52088     -1.62225
       4  -2.65534     -1.61991
     '''
-
+    snake_name = 'sklearn_incremental_predictor'
     model = traitlets.Any(default_value=None, allow_none=True, help='A scikit-learn estimator with a `.fit_predict` method.').tag(**serialize_pickle)
     features = traitlets.List(traitlets.Unicode(), help='List of features to use.')
     target = traitlets.Unicode(allow_none=False, help='The name of the target column.')
     batch_size = traitlets.Int(default_value=1_000_000, allow_none=False, help='Number of samples to be sent to the model in each batch.')
     num_epochs = traitlets.Int(default_value=1, allow_none=False, help='Number of times each batch is sent to the model.')
     shuffle = traitlets.Bool(default_value=False, allow_none=False, help='If True, shuffle the samples before sending them to the model.')
     prediction_name = traitlets.Unicode(default_value='prediction', help='The name of the virtual column housing the predictions.')
+    prediction_type = traitlets.Enum(values=['predict', 'predict_proba', 'predict_log_proba'], default_value='predict',
+                                     help='Which method to use to get the predictions. \
+                                     Can be "predict", "predict_proba" or "predict_log_proba".')
     partial_fit_kwargs = traitlets.Dict(default_value={}, help='A dictionary of key word arguments to be passed on to the `fit_predict` method of the `model`.')
 
     def __call__(self, *args):
-        X = np.vstack([arg.astype(np.float64) for arg in args]).T.copy()
-        return self.model.predict(X)
+        X = np.stack([np.asarray(arg, np.float64) for arg in args], axis=1)
+        if self.prediction_type == 'predict':
+            return self.model.predict(X)
+        elif self.prediction_type == 'predict_proba':
+            return self.model.predict_proba(X)
+        else:
+            return self.model.predict_log_proba(X)
 
     def predict(self, df):
-        '''Get an in-memory numpy array with the predictions of the SKLearnPredictor.self
+        '''Get an in-memory numpy array with the predictions of the Predictor
 
         :param df: A vaex DataFrame, containing the input features.
-        :returns: A in-memory numpy array containing the SKLearnPredictor predictions.
+        :returns: A in-memory numpy array containing the Predictor predictions.
         :rtype: numpy.array
         '''
 
         return self.transform(df)[self.prediction_name].values
 
     def transform(self, df):
         '''Transform a DataFrame such that it contains the predictions of the IncrementalPredictor.
@@ -218,15 +228,15 @@
 
         progressbar = vaex.utils.progressbars(progress)
 
         # Portions of the DataFrame to evaluate
         expressions = self.features + [self.target]
 
         for epoch in range(self.num_epochs):
-            for i1, i2, chunks in df.evaluate_iterator(expressions, chunk_size=self.batch_size):
+            for i1, i2, chunks in df.evaluate_iterator(expressions, chunk_size=self.batch_size, array_type='numpy'):
                 progressbar((n_samples * epoch + i1) / (self.num_epochs * n_samples))
                 X = np.array(chunks[:-1]).T  # the most efficient way depends on the algorithm (row of column based access)
                 y = np.array(chunks[-1], copy=False)
 
                 if self.shuffle:
                     shuffle_index = np.arange(len(X))
                     np.random.shuffle(shuffle_index)
```

### Comparing `vaex-ml-0.9.0/vaex/ml/state.py` & `vaex-ml-1.0.0a1/vaex/ml/state.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def default_to_json(trait_name, value, state_obj):
     return value
 
 
 def default_from_json(trait_name, data, state_obj):
     return data
 
-
+# @vaex.transformer.register('ml')
 class HasState(traitlets.HasTraits):
 
     @classmethod
     def state_from(cls, state, trusted=True):
         obj = cls()
         obj.state_set(state)
         return obj
@@ -55,7 +55,16 @@
 
     def state_write(self, f):
         vaex.utils.write_json_or_yaml(f, self.state_get())
 
     def state_load(self, f):
         state = vaex.utils.read_json_or_yaml(f)
         self.state_set(state)
+
+    # def encode(self, encoding):
+    #     return {
+    #         'state': self.state_get(),
+    #     }
+
+    # @classmethod
+    # def decode(cls, encoding, spec, trusted=False):
+    #     return vaex.serialize.from_dict(spec['state'], trusted=trusted)
```

### Comparing `vaex-ml-0.9.0/vaex/ml/ui.py` & `vaex-ml-1.0.0a1/vaex/ml/ui.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,17 +36,15 @@
             if 'ui' in metadata:
                 widget_class = ui_dict_[metadata['ui']]
                 widget = widget_class(description=trait_name)
                 widget_list.append(widget)
 
                 if isinstance(widget, widgets.SelectMultiple):
                     widget.options = self.dataframe.get_column_names(virtual=True, strings=True)
-                    traitlets.link((self.pipeline_object, trait_name), (widget, 'value'))
-                else:
-                    traitlets.link((self.pipeline_object, trait_name), (widget, 'value'))
+                traitlets.link((self.pipeline_object, trait_name), (widget, 'value'))
 
         fit_button = widgets.Button(description='Fit', button_style='info')
         fit_button.on_click(lambda button: self.pipeline_object.fit(self.dataframe))
         # add it to the 'form'.
         widget_list.append(fit_button)
 
         # Adding all the  widget elements to the parent object
```

### Comparing `vaex-ml-0.9.0/vaex/ml/xgboost.py` & `vaex-ml-1.0.0a1/vaex/ml/xgboost.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,23 +50,23 @@
     >>> df_test = booster.transform(df_test)
     >>> df_test.head(3)
     #    sepal_length    sepal_width    petal_length    petal_width    class_    xgboost_prediction
     0             5.9            3               4.2            1.5         1                     1
     1             6.1            3               4.6            1.4         1                     1
     2             6.6            2.9             4.6            1.3         1                     1
     '''
-
+    snake_name = 'xgboost_model'
     features = traitlets.List(traitlets.Unicode(), help='List of features to use when fitting the XGBoostModel.')
     target = traitlets.Unicode(allow_none=False, help='The name of the target column.')
     num_boost_round = traitlets.CInt(help='Number of boosting iterations.')
     params = traitlets.Dict(help='A dictionary of parameters to be passed on to the XGBoost model.')
     prediction_name = traitlets.Unicode(default_value='xgboost_prediction', help='The name of the virtual column housing the predictions.')
 
     def __call__(self, *args):
-        data2d = np.vstack([arg.astype(np.float64) for arg in args]).T.copy()
+        data2d = np.stack([np.asarray(arg, np.float64) for arg in args], axis=1)
         dmatrix = xgboost.DMatrix(data2d)
         return self.booster.predict(dmatrix)
 
     def transform(self, df):
         '''Transform a DataFrame such that it contains the predictions of the XGBoostModel in form of a virtual column.
 
         :param df: A vaex DataFrame. It should have the same columns as the DataFrame used to train the model.
@@ -93,21 +93,21 @@
             from the last iteration (not the best one).
         :param dict evals_result: A dictionary storing the evaluation results of all the items in *evals*.
         :param bool verbose_eval: Requires at least one item in *evals*.
             If *verbose_eval* is True then the evaluation metric on the validation set is printed at each boosting stage.
         '''
 
         data = df[self.features].values
-        target_data = df.evaluate(self.target)
+        target_data = df[self.target].to_numpy()
         dtrain = xgboost.DMatrix(data, target_data)
         if evals is not None:
             evals = [list(elem) for elem in evals]
             for item in evals:
                 data = item[0][self.features].values
-                target_data = item[0].evaluate(self.target)
+                target_data = item[0][self.target].to_numpy()
                 item[0] = xgboost.DMatrix(data, target_data)
         else:
             evals = ()
 
         # This does the actual training / fitting of the xgboost model
         self.booster = xgboost.train(params=self.params,
                                      dtrain=dtrain,
```

### Comparing `vaex-ml-0.9.0/vaex_ml.egg-info/SOURCES.txt` & `vaex-ml-1.0.0a1/vaex_ml.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -4,26 +4,31 @@
 vaex/ml/__init__.py
 vaex/ml/_version.py
 vaex/ml/catboost.py
 vaex/ml/cluster.py
 vaex/ml/generate.py
 vaex/ml/lightgbm.py
 vaex/ml/linear_model.py
+vaex/ml/metrics.py
 vaex/ml/pipeline.py
 vaex/ml/sklearn.py
+vaex/ml/spec.json
+vaex/ml/spec.py
 vaex/ml/state.py
+vaex/ml/tensorflow.py
 vaex/ml/transformations.py
 vaex/ml/ui.py
 vaex/ml/xgboost.py
 vaex/ml/datasets/__init__.py
 vaex/ml/datasets/iris.hdf5
 vaex/ml/datasets/titanic.hdf5
 vaex/ml/incubator/__init__.py
 vaex/ml/incubator/annoy.py
 vaex/ml/incubator/pygbm.py
+vaex/ml/incubator/river.py
 vaex_ml.egg-info/PKG-INFO
 vaex_ml.egg-info/SOURCES.txt
 vaex_ml.egg-info/dependency_links.txt
 vaex_ml.egg-info/entry_points.txt
 vaex_ml.egg-info/not-zip-safe
 vaex_ml.egg-info/requires.txt
 vaex_ml.egg-info/top_level.txt
```

