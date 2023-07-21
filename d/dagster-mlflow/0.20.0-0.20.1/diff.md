# Comparing `tmp/dagster-mlflow-0.20.0.tar.gz` & `tmp/dagster-mlflow-0.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-mlflow-0.20.0.tar", last modified: Thu Jul 20 22:02:57 2023, max compression
+gzip compressed data, was "dagster-mlflow-0.20.1.tar", last modified: Fri Jul 21 15:38:16 2023, max compression
```

## Comparing `dagster-mlflow-0.20.0.tar` & `dagster-mlflow-0.20.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:57.374833 dagster-mlflow-0.20.0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-07-20 21:53:16.000000 dagster-mlflow-0.20.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       66 2023-07-20 21:53:16.000000 dagster-mlflow-0.20.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      571 2023-07-20 22:02:57.374833 dagster-mlflow-0.20.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2023-07-20 21:53:16.000000 dagster-mlflow-0.20.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:57.370833 dagster-mlflow-0.20.0/dagster_mlflow/
--rw-r--r--   0 root         (0) root         (0)      303 2023-07-20 21:53:16.000000 dagster-mlflow-0.20.0/dagster_mlflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1211 2023-07-20 21:53:16.000000 dagster-mlflow-0.20.0/dagster_mlflow/hooks.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-20 21:53:16.000000 dagster-mlflow-0.20.0/dagster_mlflow/py.typed
--rw-r--r--   0 root         (0) root         (0)    10915 2023-07-20 21:53:16.000000 dagster-mlflow-0.20.0/dagster_mlflow/resources.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-mlflow-0.20.0/dagster_mlflow/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:57.374833 dagster-mlflow-0.20.0/dagster_mlflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)      571 2023-07-20 22:02:57.000000 dagster-mlflow-0.20.0/dagster_mlflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      403 2023-07-20 22:02:57.000000 dagster-mlflow-0.20.0/dagster_mlflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:02:57.000000 dagster-mlflow-0.20.0/dagster_mlflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:02:57.000000 dagster-mlflow-0.20.0/dagster_mlflow.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-20 22:02:57.000000 dagster-mlflow-0.20.0/dagster_mlflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-20 22:02:57.000000 dagster-mlflow-0.20.0/dagster_mlflow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      161 2023-07-20 22:02:57.374833 dagster-mlflow-0.20.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1183 2023-07-20 21:53:16.000000 dagster-mlflow-0.20.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:16.443204 dagster-mlflow-0.20.1/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-21 15:29:00.000000 dagster-mlflow-0.20.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-21 15:29:00.000000 dagster-mlflow-0.20.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      571 2023-07-21 15:38:16.443204 dagster-mlflow-0.20.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2023-07-21 15:29:00.000000 dagster-mlflow-0.20.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:16.439205 dagster-mlflow-0.20.1/dagster_mlflow/
+-rw-r--r--   0 root         (0) root         (0)      303 2023-07-21 15:29:00.000000 dagster-mlflow-0.20.1/dagster_mlflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2023-07-21 15:29:00.000000 dagster-mlflow-0.20.1/dagster_mlflow/hooks.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-21 15:29:00.000000 dagster-mlflow-0.20.1/dagster_mlflow/py.typed
+-rw-r--r--   0 root         (0) root         (0)    10915 2023-07-21 15:29:00.000000 dagster-mlflow-0.20.1/dagster_mlflow/resources.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-21 15:29:00.000000 dagster-mlflow-0.20.1/dagster_mlflow/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:16.443204 dagster-mlflow-0.20.1/dagster_mlflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      571 2023-07-21 15:38:16.000000 dagster-mlflow-0.20.1/dagster_mlflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      403 2023-07-21 15:38:16.000000 dagster-mlflow-0.20.1/dagster_mlflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:38:16.000000 dagster-mlflow-0.20.1/dagster_mlflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:38:16.000000 dagster-mlflow-0.20.1/dagster_mlflow.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-21 15:38:16.000000 dagster-mlflow-0.20.1/dagster_mlflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-21 15:38:16.000000 dagster-mlflow-0.20.1/dagster_mlflow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2023-07-21 15:38:16.443204 dagster-mlflow-0.20.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1183 2023-07-21 15:29:00.000000 dagster-mlflow-0.20.1/setup.py
```

### Comparing `dagster-mlflow-0.20.0/LICENSE` & `dagster-mlflow-0.20.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-mlflow-0.20.0/PKG-INFO` & `dagster-mlflow-0.20.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-mlflow
-Version: 0.20.0
+Version: 0.20.1
 Summary: Package for mlflow Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mlflow
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-mlflow-0.20.0/dagster_mlflow/hooks.py` & `dagster-mlflow-0.20.1/dagster_mlflow/hooks.py`

 * *Files identical despite different names*

### Comparing `dagster-mlflow-0.20.0/dagster_mlflow/resources.py` & `dagster-mlflow-0.20.1/dagster_mlflow/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-mlflow-0.20.0/dagster_mlflow.egg-info/PKG-INFO` & `dagster-mlflow-0.20.1/dagster_mlflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-mlflow
-Version: 0.20.0
+Version: 0.20.1
 Summary: Package for mlflow Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mlflow
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-mlflow-0.20.0/setup.py` & `dagster-mlflow-0.20.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,10 +27,10 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_mlflow_tests*"]),
-    install_requires=["dagster==1.4.0", "mlflow", "pandas"],
+    install_requires=["dagster==1.4.1", "mlflow", "pandas"],
     zip_safe=False,
 )
```

