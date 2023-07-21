# Comparing `tmp/azureml_infra_tools-0.1.0a3.tar.gz` & `tmp/azureml_infra_tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azureml_infra_tools-0.1.0a3.tar", max compression
+gzip compressed data, was "azureml_infra_tools-0.1.1.tar", max compression
```

## Comparing `azureml_infra_tools-0.1.0a3.tar` & `azureml_infra_tools-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-07-21 11:51:19.763363 azureml_infra_tools-0.1.0a3/LICENSE
--rw-r--r--   0        0        0     5826 2023-07-21 11:51:19.763363 azureml_infra_tools-0.1.0a3/README.md
--rw-r--r--   0        0        0     3876 2023-07-21 11:51:19.763363 azureml_infra_tools-0.1.0a3/azureml_infra_tools/__init__.py
--rw-r--r--   0        0        0     3489 2023-07-21 11:51:19.763363 azureml_infra_tools-0.1.0a3/azureml_infra_tools/cluster.py
--rw-r--r--   0        0        0     3355 2023-07-21 11:51:19.763363 azureml_infra_tools-0.1.0a3/azureml_infra_tools/credential.py
--rw-r--r--   0        0        0     2931 2023-07-21 11:51:19.763363 azureml_infra_tools-0.1.0a3/azureml_infra_tools/data.py
--rw-r--r--   0        0        0     3283 2023-07-21 11:51:19.763363 azureml_infra_tools-0.1.0a3/azureml_infra_tools/environment.py
--rw-r--r--   0        0        0      824 2023-07-21 11:51:19.763363 azureml_infra_tools-0.1.0a3/pyproject.toml
--rw-r--r--   0        0        0     6731 1970-01-01 00:00:00.000000 azureml_infra_tools-0.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-21 14:02:44.113628 azureml_infra_tools-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5826 2023-07-21 14:02:44.113628 azureml_infra_tools-0.1.1/README.md
+-rw-r--r--   0        0        0     3876 2023-07-21 14:02:44.113628 azureml_infra_tools-0.1.1/azureml_infra_tools/__init__.py
+-rw-r--r--   0        0        0     3489 2023-07-21 14:02:44.113628 azureml_infra_tools-0.1.1/azureml_infra_tools/cluster.py
+-rw-r--r--   0        0        0     3355 2023-07-21 14:02:44.113628 azureml_infra_tools-0.1.1/azureml_infra_tools/credential.py
+-rw-r--r--   0        0        0     2931 2023-07-21 14:02:44.113628 azureml_infra_tools-0.1.1/azureml_infra_tools/data.py
+-rw-r--r--   0        0        0     3283 2023-07-21 14:02:44.113628 azureml_infra_tools-0.1.1/azureml_infra_tools/environment.py
+-rw-r--r--   0        0        0      822 2023-07-21 14:02:44.113628 azureml_infra_tools-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6729 1970-01-01 00:00:00.000000 azureml_infra_tools-0.1.1/PKG-INFO
```

### Comparing `azureml_infra_tools-0.1.0a3/LICENSE` & `azureml_infra_tools-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `azureml_infra_tools-0.1.0a3/README.md` & `azureml_infra_tools-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `azureml_infra_tools-0.1.0a3/azureml_infra_tools/__init__.py` & `azureml_infra_tools-0.1.1/azureml_infra_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `azureml_infra_tools-0.1.0a3/azureml_infra_tools/cluster.py` & `azureml_infra_tools-0.1.1/azureml_infra_tools/cluster.py`

 * *Files identical despite different names*

### Comparing `azureml_infra_tools-0.1.0a3/azureml_infra_tools/credential.py` & `azureml_infra_tools-0.1.1/azureml_infra_tools/credential.py`

 * *Files identical despite different names*

### Comparing `azureml_infra_tools-0.1.0a3/azureml_infra_tools/data.py` & `azureml_infra_tools-0.1.1/azureml_infra_tools/data.py`

 * *Files identical despite different names*

### Comparing `azureml_infra_tools-0.1.0a3/azureml_infra_tools/environment.py` & `azureml_infra_tools-0.1.1/azureml_infra_tools/environment.py`

 * *Files identical despite different names*

### Comparing `azureml_infra_tools-0.1.0a3/pyproject.toml` & `azureml_infra_tools-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "azureml-infra-tools"
-version = "0.1.0a3"
+version = "0.1.1"
 description = "azureml-infra-tools is a Python package providing high-level APIs for Azure Machine Learning. It simplifies setup of Azure ML infrastructures, manages datasets, and streamlines authentication. Designed for AI researchers, data scientists, and ML engineers, it boosts productivity and accelerates Azure ML projects."
 authors = ["Henrique Malta <vlezyitalia@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `azureml_infra_tools-0.1.0a3/PKG-INFO` & `azureml_infra_tools-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azureml-infra-tools
-Version: 0.1.0a3
+Version: 0.1.1
 Summary: azureml-infra-tools is a Python package providing high-level APIs for Azure Machine Learning. It simplifies setup of Azure ML infrastructures, manages datasets, and streamlines authentication. Designed for AI researchers, data scientists, and ML engineers, it boosts productivity and accelerates Azure ML projects.
 License: MIT
 Author: Henrique Malta
 Author-email: vlezyitalia@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

