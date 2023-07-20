# Comparing `tmp/dagster-mlflow-0.19.9rc0.tar.gz` & `tmp/dagster-mlflow-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-mlflow-0.19.9rc0.tar", last modified: Thu Jun  8 18:28:31 2023, max compression
+gzip compressed data, was "dagster-mlflow-0.20.0.tar", last modified: Thu Jul 20 22:02:57 2023, max compression
```

## Comparing `dagster-mlflow-0.19.9rc0.tar` & `dagster-mlflow-0.20.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:31.986865 dagster-mlflow-0.19.9rc0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-mlflow-0.19.9rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       66 2023-06-08 18:20:46.000000 dagster-mlflow-0.19.9rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      624 2023-06-08 18:28:31.986865 dagster-mlflow-0.19.9rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2023-06-08 18:20:46.000000 dagster-mlflow-0.19.9rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:31.982865 dagster-mlflow-0.19.9rc0/dagster_mlflow/
--rw-r--r--   0 root         (0) root         (0)      303 2023-06-08 18:20:46.000000 dagster-mlflow-0.19.9rc0/dagster_mlflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1211 2023-06-08 18:20:46.000000 dagster-mlflow-0.19.9rc0/dagster_mlflow/hooks.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 18:20:46.000000 dagster-mlflow-0.19.9rc0/dagster_mlflow/py.typed
--rw-r--r--   0 root         (0) root         (0)    10800 2023-06-08 18:20:46.000000 dagster-mlflow-0.19.9rc0/dagster_mlflow/resources.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-mlflow-0.19.9rc0/dagster_mlflow/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:31.982865 dagster-mlflow-0.19.9rc0/dagster_mlflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)      624 2023-06-08 18:28:31.000000 dagster-mlflow-0.19.9rc0/dagster_mlflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      403 2023-06-08 18:28:31.000000 dagster-mlflow-0.19.9rc0/dagster_mlflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:28:31.000000 dagster-mlflow-0.19.9rc0/dagster_mlflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:28:31.000000 dagster-mlflow-0.19.9rc0/dagster_mlflow.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-08 18:28:31.000000 dagster-mlflow-0.19.9rc0/dagster_mlflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-08 18:28:31.000000 dagster-mlflow-0.19.9rc0/dagster_mlflow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      161 2023-06-08 18:28:31.986865 dagster-mlflow-0.19.9rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1103 2023-06-08 18:20:46.000000 dagster-mlflow-0.19.9rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:57.374833 dagster-mlflow-0.20.0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-20 21:53:16.000000 dagster-mlflow-0.20.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-20 21:53:16.000000 dagster-mlflow-0.20.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      571 2023-07-20 22:02:57.374833 dagster-mlflow-0.20.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2023-07-20 21:53:16.000000 dagster-mlflow-0.20.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:57.370833 dagster-mlflow-0.20.0/dagster_mlflow/
+-rw-r--r--   0 root         (0) root         (0)      303 2023-07-20 21:53:16.000000 dagster-mlflow-0.20.0/dagster_mlflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2023-07-20 21:53:16.000000 dagster-mlflow-0.20.0/dagster_mlflow/hooks.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-20 21:53:16.000000 dagster-mlflow-0.20.0/dagster_mlflow/py.typed
+-rw-r--r--   0 root         (0) root         (0)    10915 2023-07-20 21:53:16.000000 dagster-mlflow-0.20.0/dagster_mlflow/resources.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-mlflow-0.20.0/dagster_mlflow/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:57.374833 dagster-mlflow-0.20.0/dagster_mlflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      571 2023-07-20 22:02:57.000000 dagster-mlflow-0.20.0/dagster_mlflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      403 2023-07-20 22:02:57.000000 dagster-mlflow-0.20.0/dagster_mlflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:02:57.000000 dagster-mlflow-0.20.0/dagster_mlflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:02:57.000000 dagster-mlflow-0.20.0/dagster_mlflow.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-20 22:02:57.000000 dagster-mlflow-0.20.0/dagster_mlflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-20 22:02:57.000000 dagster-mlflow-0.20.0/dagster_mlflow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2023-07-20 22:02:57.374833 dagster-mlflow-0.20.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1183 2023-07-20 21:53:16.000000 dagster-mlflow-0.20.0/setup.py
```

### Comparing `dagster-mlflow-0.19.9rc0/LICENSE` & `dagster-mlflow-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-mlflow-0.19.9rc0/PKG-INFO` & `dagster-mlflow-0.20.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: dagster-mlflow
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for mlflow Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mlflow
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
```

### Comparing `dagster-mlflow-0.19.9rc0/dagster_mlflow/hooks.py` & `dagster-mlflow-0.20.0/dagster_mlflow/hooks.py`

 * *Files identical despite different names*

### Comparing `dagster-mlflow-0.19.9rc0/dagster_mlflow/resources.py` & `dagster-mlflow-0.20.0/dagster_mlflow/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import sys
 from itertools import islice
 from os import environ
 from typing import Any, Optional
 
 import mlflow
 from dagster import Field, Noneable, Permissive, StringSource, resource
+from dagster._core.definitions.resource_definition import dagster_maintained_resource
 from mlflow.entities.run_status import RunStatus
 
 CONFIG_SCHEMA = {
     "experiment_name": Field(StringSource, is_required=True, description="MlFlow experiment name."),
     "mlflow_tracking_uri": Field(
         Noneable(StringSource),
         default_value=None,
@@ -214,14 +215,15 @@
             (dict): Batch of dictionary
         """
         it = iter(params)
         for _ in range(0, len(params), size):
             yield {k: params[k] for k in islice(it, size)}
 
 
+@dagster_maintained_resource
 @resource(config_schema=CONFIG_SCHEMA)
 def mlflow_tracking(context):
     """This resource initializes an MLflow run that's used for all steps within a Dagster run.
 
     This resource provides access to all of mlflow's methods as well as the mlflow tracking client's
     methods.
```

### Comparing `dagster-mlflow-0.19.9rc0/dagster_mlflow.egg-info/PKG-INFO` & `dagster-mlflow-0.20.0/dagster_mlflow.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: dagster-mlflow
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for mlflow Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mlflow
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
```

### Comparing `dagster-mlflow-0.19.9rc0/setup.py` & `dagster-mlflow-0.20.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,27 +8,29 @@
     version: Dict[str, str] = {}
     with open(Path(__file__).parent / "dagster_mlflow/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)
 
     return version["__version__"]
 
 
+ver = get_version()
+# dont pin dev installs to avoid pip dep resolver issues
+pin = "" if ver == "1!0+dev" else f"=={ver}"
 setup(
     name="dagster-mlflow",
     version=get_version(),
     author="Elementl",
     author_email="hello@elementl.com",
     license="Apache-2.0",
     description="Package for mlflow Dagster framework components.",
     url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mlflow",
     classifiers=[
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_mlflow_tests*"]),
-    install_requires=["dagster", "mlflow", "pandas"],
+    install_requires=["dagster==1.4.0", "mlflow", "pandas"],
     zip_safe=False,
 )
```

