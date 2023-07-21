# Comparing `tmp/mlforecast-0.8.0.tar.gz` & `tmp/mlforecast-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlforecast-0.8.0.tar", last modified: Thu Jul 20 06:18:48 2023, max compression
+gzip compressed data, was "mlforecast-0.8.1.tar", last modified: Fri Jul 21 02:46:31 2023, max compression
```

## Comparing `mlforecast-0.8.0.tar` & `mlforecast-0.8.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 06:18:48.711516 mlforecast-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-07-20 06:18:39.000000 mlforecast-0.8.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-07-20 06:18:39.000000 mlforecast-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-20 06:18:39.000000 mlforecast-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-07-20 06:18:48.711516 mlforecast-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-07-20 06:18:39.000000 mlforecast-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 06:18:48.707516 mlforecast-0.8.0/mlforecast/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-20 06:18:39.000000 mlforecast-0.8.0/mlforecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30980 2023-07-20 06:18:39.000000 mlforecast-0.8.0/mlforecast/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)    23291 2023-07-20 06:18:39.000000 mlforecast-0.8.0/mlforecast/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 06:18:48.711516 mlforecast-0.8.0/mlforecast/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-20 06:18:39.000000 mlforecast-0.8.0/mlforecast/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25805 2023-07-20 06:18:39.000000 mlforecast-0.8.0/mlforecast/distributed/forecast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 06:18:48.711516 mlforecast-0.8.0/mlforecast/distributed/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 06:18:39.000000 mlforecast-0.8.0/mlforecast/distributed/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 06:18:48.711516 mlforecast-0.8.0/mlforecast/distributed/models/dask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 06:18:39.000000 mlforecast-0.8.0/mlforecast/distributed/models/dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-20 06:18:39.000000 mlforecast-0.8.0/mlforecast/distributed/models/dask/lgb.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-20 06:18:39.000000 mlforecast-0.8.0/mlforecast/distributed/models/dask/xgb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 06:18:48.711516 mlforecast-0.8.0/mlforecast/distributed/models/ray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 06:18:39.000000 mlforecast-0.8.0/mlforecast/distributed/models/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-20 06:18:39.000000 mlforecast-0.8.0/mlforecast/distributed/models/ray/lgb.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-20 06:18:39.000000 mlforecast-0.8.0/mlforecast/distributed/models/ray/xgb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 06:18:48.711516 mlforecast-0.8.0/mlforecast/distributed/models/spark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 06:18:39.000000 mlforecast-0.8.0/mlforecast/distributed/models/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-20 06:18:39.000000 mlforecast-0.8.0/mlforecast/distributed/models/spark/lgb.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-20 06:18:39.000000 mlforecast-0.8.0/mlforecast/distributed/models/spark/xgb.py
--rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-07-20 06:18:39.000000 mlforecast-0.8.0/mlforecast/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-07-20 06:18:39.000000 mlforecast-0.8.0/mlforecast/grouped_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    22365 2023-07-20 06:18:39.000000 mlforecast-0.8.0/mlforecast/lgb_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-20 06:18:39.000000 mlforecast-0.8.0/mlforecast/target_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-07-20 06:18:39.000000 mlforecast-0.8.0/mlforecast/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 06:18:48.711516 mlforecast-0.8.0/mlforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-07-20 06:18:48.000000 mlforecast-0.8.0/mlforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-20 06:18:48.000000 mlforecast-0.8.0/mlforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 06:18:48.000000 mlforecast-0.8.0/mlforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 06:18:48.000000 mlforecast-0.8.0/mlforecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-20 06:18:48.000000 mlforecast-0.8.0/mlforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 06:18:48.000000 mlforecast-0.8.0/mlforecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-20 06:18:39.000000 mlforecast-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-20 06:18:39.000000 mlforecast-0.8.0/settings.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 06:18:48.711516 mlforecast-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-20 06:18:39.000000 mlforecast-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:31.589855 mlforecast-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-07-21 02:46:18.000000 mlforecast-0.8.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-07-21 02:46:18.000000 mlforecast-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-21 02:46:18.000000 mlforecast-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-07-21 02:46:31.589855 mlforecast-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-07-21 02:46:18.000000 mlforecast-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:31.585855 mlforecast-0.8.1/mlforecast/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30980 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23264 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:31.585855 mlforecast-0.8.1/mlforecast/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25805 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:31.585855 mlforecast-0.8.1/mlforecast/distributed/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:31.589855 mlforecast-0.8.1/mlforecast/distributed/models/dask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/models/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/models/dask/lgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/models/dask/xgb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:31.589855 mlforecast-0.8.1/mlforecast/distributed/models/ray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/models/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/models/ray/lgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/models/ray/xgb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:31.589855 mlforecast-0.8.1/mlforecast/distributed/models/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/models/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/models/spark/lgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/distributed/models/spark/xgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/grouped_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22365 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/lgb_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/target_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-07-21 02:46:18.000000 mlforecast-0.8.1/mlforecast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:46:31.585855 mlforecast-0.8.1/mlforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-07-21 02:46:31.000000 mlforecast-0.8.1/mlforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-21 02:46:31.000000 mlforecast-0.8.1/mlforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 02:46:31.000000 mlforecast-0.8.1/mlforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 02:46:31.000000 mlforecast-0.8.1/mlforecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-21 02:46:31.000000 mlforecast-0.8.1/mlforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 02:46:31.000000 mlforecast-0.8.1/mlforecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-21 02:46:18.000000 mlforecast-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-21 02:46:18.000000 mlforecast-0.8.1/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 02:46:31.589855 mlforecast-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-21 02:46:18.000000 mlforecast-0.8.1/setup.py
```

### Comparing `mlforecast-0.8.0/CONTRIBUTING.md` & `mlforecast-0.8.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.0/LICENSE` & `mlforecast-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.0/PKG-INFO` & `mlforecast-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlforecast
-Version: 0.8.0
+Version: 0.8.1
 Summary: Scalable machine learning based time series forecasting
 Home-page: https://github.com/Nixtla/mlforecast
 Author: José Morales
 Author-email: jmoralz92@gmail.com
 License: Apache Software License 2.0
 Keywords: python forecast forecasting machine-learning dask
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mlforecast-0.8.0/README.md` & `mlforecast-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.0/mlforecast/_modidx.py` & `mlforecast-0.8.1/mlforecast/_modidx.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.0/mlforecast/core.py` & `mlforecast-0.8.1/mlforecast/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,14 +231,15 @@
             static_features = [id_col] + static_features
         else:  # static_features defined and contain id_col
             to_drop = [time_col, target_col]
         self.static_features_ = (
             df[static_features]
             .groupby(id_col, observed=True)
             .head(1)
+            .sort_values(id_col)
             .reset_index(drop=True)
         )
         sort_idxs = pd.core.sorting.lexsort_indexer([df[id_col], df[time_col]])
         self.restore_idxs = np.empty(df.shape[0], dtype=np.int32)
         self.restore_idxs[sort_idxs] = np.arange(df.shape[0])
         sorted_df = df[[id_col, time_col, target_col]].iloc[sort_idxs]
         if self.target_transforms is not None:
@@ -592,13 +593,12 @@
                     categories=orig_categories + list(missing_categories)
                 )
         self.static_features_ = self.static_features_.set_index(self.id_col).reindex(
             self.uids
         )
         self.static_features_.update(new_statics)
         self.static_features_ = self.static_features_.reset_index().astype(orig_dtypes)
-        self.ga = self.ga.append_several(
+        self._ga = self._ga.append_several(
             new_sizes=sizes.values.astype(np.int32),
             new_values=values,
             new_groups=new_groups,
         )
-        self._ga = GroupedArray(self.ga.data, self.ga.indptr)
```

### Comparing `mlforecast-0.8.0/mlforecast/distributed/forecast.py` & `mlforecast-0.8.1/mlforecast/distributed/forecast.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.0/mlforecast/distributed/models/dask/lgb.py` & `mlforecast-0.8.1/mlforecast/distributed/models/dask/lgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.0/mlforecast/distributed/models/dask/xgb.py` & `mlforecast-0.8.1/mlforecast/distributed/models/dask/xgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.0/mlforecast/distributed/models/ray/xgb.py` & `mlforecast-0.8.1/mlforecast/distributed/models/ray/xgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.0/mlforecast/distributed/models/spark/lgb.py` & `mlforecast-0.8.1/mlforecast/distributed/models/spark/lgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.0/mlforecast/distributed/models/spark/xgb.py` & `mlforecast-0.8.1/mlforecast/distributed/models/spark/xgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.0/mlforecast/forecast.py` & `mlforecast-0.8.1/mlforecast/forecast.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.0/mlforecast/grouped_array.py` & `mlforecast-0.8.1/mlforecast/grouped_array.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.0/mlforecast/lgb_cv.py` & `mlforecast-0.8.1/mlforecast/lgb_cv.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.0/mlforecast/target_transforms.py` & `mlforecast-0.8.1/mlforecast/target_transforms.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.0/mlforecast/utils.py` & `mlforecast-0.8.1/mlforecast/utils.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.0/mlforecast.egg-info/PKG-INFO` & `mlforecast-0.8.1/mlforecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlforecast
-Version: 0.8.0
+Version: 0.8.1
 Summary: Scalable machine learning based time series forecasting
 Home-page: https://github.com/Nixtla/mlforecast
 Author: José Morales
 Author-email: jmoralz92@gmail.com
 License: Apache Software License 2.0
 Keywords: python forecast forecasting machine-learning dask
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mlforecast-0.8.0/mlforecast.egg-info/SOURCES.txt` & `mlforecast-0.8.1/mlforecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlforecast-0.8.0/settings.ini` & `mlforecast-0.8.1/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = Nixtla
 description = Scalable machine learning based time series forecasting
 keywords = python forecast forecasting machine-learning dask
 author = José Morales
 author_email = jmoralz92@gmail.com
 copyright = Nixtla
 branch = main
-version = 0.8.0
+version = 0.8.1
 min_python = 3.6
 audience = Developers
 language = English
 custom_sidebar = True
 license = apache2
 status = 3
 requirements = numba pandas scikit-learn window-ops
```

### Comparing `mlforecast-0.8.0/setup.py` & `mlforecast-0.8.1/setup.py`

 * *Files identical despite different names*

