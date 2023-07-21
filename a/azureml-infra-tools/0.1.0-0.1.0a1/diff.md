# Comparing `tmp/azureml_infra_tools-0.1.0.tar.gz` & `tmp/azureml_infra_tools-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azureml_infra_tools-0.1.0.tar", max compression
+gzip compressed data, was "azureml_infra_tools-0.1.0a1.tar", max compression
```

## Comparing `azureml_infra_tools-0.1.0.tar` & `azureml_infra_tools-0.1.0a1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-07-21 10:06:29.298264 azureml_infra_tools-0.1.0/LICENSE
--rw-r--r--   0        0        0     2699 2023-07-21 10:08:45.712440 azureml_infra_tools-0.1.0/README.md
--rw-r--r--   0        0        0     2079 2023-07-21 10:08:45.741905 azureml_infra_tools-0.1.0/azureml_infra_tools/__init__.py
--rw-r--r--   0        0        0     2415 2023-07-21 10:08:45.725215 azureml_infra_tools-0.1.0/azureml_infra_tools/cluster.py
--rw-r--r--   0        0        0     2868 2023-07-21 10:06:29.299237 azureml_infra_tools-0.1.0/azureml_infra_tools/credential.py
--rw-r--r--   0        0        0     1980 2023-07-21 10:08:45.719320 azureml_infra_tools-0.1.0/azureml_infra_tools/data.py
--rw-r--r--   0        0        0     2058 2023-07-21 10:08:45.728772 azureml_infra_tools-0.1.0/azureml_infra_tools/environment.py
--rw-r--r--   0        0        0      773 2023-07-21 10:08:45.709763 azureml_infra_tools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3595 1970-01-01 00:00:00.000000 azureml_infra_tools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-21 10:06:29.298264 azureml_infra_tools-0.1.0a1/LICENSE
+-rw-r--r--   0        0        0     2699 2023-07-21 10:08:45.712440 azureml_infra_tools-0.1.0a1/README.md
+-rw-r--r--   0        0        0     2079 2023-07-21 10:08:45.741905 azureml_infra_tools-0.1.0a1/azureml_infra_tools/__init__.py
+-rw-r--r--   0        0        0     2415 2023-07-21 10:08:45.725215 azureml_infra_tools-0.1.0a1/azureml_infra_tools/cluster.py
+-rw-r--r--   0        0        0     2868 2023-07-21 10:06:29.299237 azureml_infra_tools-0.1.0a1/azureml_infra_tools/credential.py
+-rw-r--r--   0        0        0     1980 2023-07-21 10:08:45.719320 azureml_infra_tools-0.1.0a1/azureml_infra_tools/data.py
+-rw-r--r--   0        0        0     2058 2023-07-21 10:08:45.728772 azureml_infra_tools-0.1.0a1/azureml_infra_tools/environment.py
+-rw-r--r--   0        0        0      824 2023-07-21 10:14:01.712076 azureml_infra_tools-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0     3604 1970-01-01 00:00:00.000000 azureml_infra_tools-0.1.0a1/PKG-INFO
```

### Comparing `azureml_infra_tools-0.1.0/LICENSE` & `azureml_infra_tools-0.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `azureml_infra_tools-0.1.0/README.md` & `azureml_infra_tools-0.1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `azureml_infra_tools-0.1.0/azureml_infra_tools/__init__.py` & `azureml_infra_tools-0.1.0a1/azureml_infra_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `azureml_infra_tools-0.1.0/azureml_infra_tools/cluster.py` & `azureml_infra_tools-0.1.0a1/azureml_infra_tools/cluster.py`

 * *Files identical despite different names*

### Comparing `azureml_infra_tools-0.1.0/azureml_infra_tools/credential.py` & `azureml_infra_tools-0.1.0a1/azureml_infra_tools/credential.py`

 * *Files identical despite different names*

### Comparing `azureml_infra_tools-0.1.0/azureml_infra_tools/data.py` & `azureml_infra_tools-0.1.0a1/azureml_infra_tools/data.py`

 * *Files identical despite different names*

### Comparing `azureml_infra_tools-0.1.0/azureml_infra_tools/environment.py` & `azureml_infra_tools-0.1.0a1/azureml_infra_tools/environment.py`

 * *Files identical despite different names*

### Comparing `azureml_infra_tools-0.1.0/pyproject.toml` & `azureml_infra_tools-0.1.0a1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [tool.poetry]
 name = "azureml-infra-tools"
-version = "0.1.0"
-description = "azuremlutils is a Python package providing high-level APIs for Azure Machine Learning. It simplifies setup of Azure ML infrastructures, manages datasets, and streamlines authentication. Designed for AI researchers, data scientists, and ML engineers, it boosts productivity and accelerates Azure ML projects."
+version = "0.1.0a1"
+description = "azureml-infra-tools is a Python package providing high-level APIs for Azure Machine Learning. It simplifies setup of Azure ML infrastructures, manages datasets, and streamlines authentication. Designed for AI researchers, data scientists, and ML engineers, it boosts productivity and accelerates Azure ML projects."
 authors = ["Henrique Malta <vlezyitalia@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 azure-ai-ml = "^1.8.0"
 urllib3 = "1.26.9"
 azure-identity = "^1.13.0"
 python-dotenv = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 yapf = "^0.40.1"
 pylint = "^2.17.4"
+pytest = "^7.4.0"
+pytest-mock = "^3.11.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `azureml_infra_tools-0.1.0/PKG-INFO` & `azureml_infra_tools-0.1.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: azureml-infra-tools
-Version: 0.1.0
-Summary: azuremlutils is a Python package providing high-level APIs for Azure Machine Learning. It simplifies setup of Azure ML infrastructures, manages datasets, and streamlines authentication. Designed for AI researchers, data scientists, and ML engineers, it boosts productivity and accelerates Azure ML projects.
+Version: 0.1.0a1
+Summary: azureml-infra-tools is a Python package providing high-level APIs for Azure Machine Learning. It simplifies setup of Azure ML infrastructures, manages datasets, and streamlines authentication. Designed for AI researchers, data scientists, and ML engineers, it boosts productivity and accelerates Azure ML projects.
 License: MIT
 Author: Henrique Malta
 Author-email: vlezyitalia@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

