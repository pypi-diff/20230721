# Comparing `tmp/gaohn-common-utils-0.0.94.tar.gz` & `tmp/gaohn-common-utils-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.94.tar", last modified: Wed Jul 19 07:57:16 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.95.tar", last modified: Fri Jul 21 02:51:14 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.94.tar` & `gaohn-common-utils-0.0.95.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:57:16.672469 gaohn-common-utils-0.0.94/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-19 07:57:16.672469 gaohn-common-utils-0.0.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:57:16.668469 gaohn-common-utils-0.0.94/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:57:16.668469 gaohn-common-utils-0.0.94/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:57:16.668469 gaohn-common-utils-0.0.94/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:57:16.668469 gaohn-common-utils-0.0.94/common_utils/cloud/gcp/database/
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/common_utils/cloud/gcp/database/bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:57:16.668469 gaohn-common-utils-0.0.94/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:57:16.668469 gaohn-common-utils-0.0.94/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/common_utils/core/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:57:16.668469 gaohn-common-utils-0.0.94/common_utils/core/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/common_utils/core/decorators/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/common_utils/core/decorators/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:57:16.668469 gaohn-common-utils-0.0.94/common_utils/data_validator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/common_utils/data_validator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/common_utils/data_validator/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:57:16.668469 gaohn-common-utils-0.0.94/common_utils/experiment_tracking/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:57:16.668469 gaohn-common-utils-0.0.94/common_utils/experiment_tracking/promoter/
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/common_utils/experiment_tracking/promoter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/common_utils/experiment_tracking/promoter/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:57:16.668469 gaohn-common-utils-0.0.94/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/common_utils/orchestrator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/common_utils/orchestrator/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:57:16.668469 gaohn-common-utils-0.0.94/common_utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/common_utils/tests/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:57:16.668469 gaohn-common-utils-0.0.94/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:57:16.672469 gaohn-common-utils-0.0.94/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/common_utils/versioning/dvc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/common_utils/versioning/dvc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:57:16.672469 gaohn-common-utils-0.0.94/common_utils/versioning/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/common_utils/versioning/git/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/common_utils/versioning/git/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:57:16.672469 gaohn-common-utils-0.0.94/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-19 07:57:16.000000 gaohn-common-utils-0.0.94/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-19 07:57:16.000000 gaohn-common-utils-0.0.94/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 07:57:16.000000 gaohn-common-utils-0.0.94/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-19 07:57:16.000000 gaohn-common-utils-0.0.94/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-19 07:57:16.000000 gaohn-common-utils-0.0.94/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-19 07:56:55.000000 gaohn-common-utils-0.0.94/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 07:57:16.672469 gaohn-common-utils-0.0.94/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:51:14.879176 gaohn-common-utils-0.0.95/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-21 02:51:14.879176 gaohn-common-utils-0.0.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:51:14.875176 gaohn-common-utils-0.0.95/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:51:14.875176 gaohn-common-utils-0.0.95/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:51:14.875176 gaohn-common-utils-0.0.95/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:51:14.875176 gaohn-common-utils-0.0.95/common_utils/cloud/gcp/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/common_utils/cloud/gcp/database/bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:51:14.875176 gaohn-common-utils-0.0.95/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:51:14.875176 gaohn-common-utils-0.0.95/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/common_utils/core/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:51:14.879176 gaohn-common-utils-0.0.95/common_utils/core/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/common_utils/core/decorators/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/common_utils/core/decorators/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:51:14.879176 gaohn-common-utils-0.0.95/common_utils/data_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/common_utils/data_validator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/common_utils/data_validator/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:51:14.875176 gaohn-common-utils-0.0.95/common_utils/experiment_tracking/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:51:14.879176 gaohn-common-utils-0.0.95/common_utils/experiment_tracking/promoter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/common_utils/experiment_tracking/promoter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/common_utils/experiment_tracking/promoter/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:51:14.879176 gaohn-common-utils-0.0.95/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/common_utils/orchestrator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/common_utils/orchestrator/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:51:14.879176 gaohn-common-utils-0.0.95/common_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/common_utils/tests/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:51:14.875176 gaohn-common-utils-0.0.95/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:51:14.879176 gaohn-common-utils-0.0.95/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/common_utils/versioning/dvc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/common_utils/versioning/dvc/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:51:14.879176 gaohn-common-utils-0.0.95/common_utils/versioning/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/common_utils/versioning/git/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/common_utils/versioning/git/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:51:14.879176 gaohn-common-utils-0.0.95/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-21 02:51:14.000000 gaohn-common-utils-0.0.95/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-21 02:51:14.000000 gaohn-common-utils-0.0.95/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 02:51:14.000000 gaohn-common-utils-0.0.95/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-21 02:51:14.000000 gaohn-common-utils-0.0.95/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 02:51:14.000000 gaohn-common-utils-0.0.95/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-21 02:50:53.000000 gaohn-common-utils-0.0.95/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 02:51:14.879176 gaohn-common-utils-0.0.95/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.94/LICENSE` & `gaohn-common-utils-0.0.95/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.94/PKG-INFO` & `gaohn-common-utils-0.0.95/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.94
+Version: 0.0.95
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.94/README.md` & `gaohn-common-utils-0.0.95/README.md`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.94/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.95/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.94/common_utils/cloud/gcp/database/bigquery.py` & `gaohn-common-utils-0.0.95/common_utils/cloud/gcp/database/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.94/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.95/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.94/common_utils/core/base.py` & `gaohn-common-utils-0.0.95/common_utils/core/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.94/common_utils/core/common.py` & `gaohn-common-utils-0.0.95/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.94/common_utils/core/decorators/decorators.py` & `gaohn-common-utils-0.0.95/common_utils/core/decorators/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.94/common_utils/core/decorators/timer.py` & `gaohn-common-utils-0.0.95/common_utils/core/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.94/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.95/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.94/common_utils/core/logger.py` & `gaohn-common-utils-0.0.95/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.94/common_utils/data_validator/core.py` & `gaohn-common-utils-0.0.95/common_utils/data_validator/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.94/common_utils/experiment_tracking/promoter/base.py` & `gaohn-common-utils-0.0.95/common_utils/experiment_tracking/promoter/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.94/common_utils/experiment_tracking/promoter/core.py` & `gaohn-common-utils-0.0.95/common_utils/experiment_tracking/promoter/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.94/common_utils/orchestrator/core.py` & `gaohn-common-utils-0.0.95/common_utils/orchestrator/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.94/common_utils/tests/core.py` & `gaohn-common-utils-0.0.95/common_utils/tests/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.94/common_utils/versioning/dvc/core.py` & `gaohn-common-utils-0.0.95/common_utils/versioning/dvc/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.94/common_utils/versioning/git/core.py` & `gaohn-common-utils-0.0.95/common_utils/versioning/git/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.94/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.95/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.94
+Version: 0.0.95
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.94/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.95/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.94/pyproject.toml` & `gaohn-common-utils-0.0.95/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.94"
+version = "0.0.95"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -164,8 +164,9 @@
 minversion = "6.0"
 addopts = "-ra" # -ra -q
 testpaths = [
     "tests",
     # "tests/unit",
     # "tests/integration",
     # "tests/system",
-]
+]
+filterwarnings = "ignore::DeprecationWarning" # ignore deprecation warnings when running tests
```

