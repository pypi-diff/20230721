# Comparing `tmp/mlflowops-0.1.0.tar.gz` & `tmp/mlflowops-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflowops-0.1.0.tar", max compression
+gzip compressed data, was "mlflowops-0.1.1.tar", max compression
```

## Comparing `mlflowops-0.1.0.tar` & `mlflowops-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1083 2023-07-21 04:35:41.952673 mlflowops-0.1.0/LICENSE
--rw-r--r--   0        0        0      926 2023-07-21 04:35:41.952673 mlflowops-0.1.0/README.md
--rw-r--r--   0        0        0       99 2023-07-21 04:35:41.952673 mlflowops-0.1.0/mlflowops/__init__.py
--rw-r--r--   0        0        0     6633 2023-07-21 04:35:41.952673 mlflowops-0.1.0/mlflowops/mlflowops.py
--rw-r--r--   0        0        0     4724 2023-07-21 04:35:41.952673 mlflowops-0.1.0/mlflowops/session.py
--rw-r--r--   0        0        0      556 2023-07-21 04:35:41.952673 mlflowops-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 mlflowops-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-21 04:49:46.014872 mlflowops-0.1.1/LICENSE
+-rw-r--r--   0        0        0      926 2023-07-21 04:49:46.014872 mlflowops-0.1.1/README.md
+-rw-r--r--   0        0        0       99 2023-07-21 04:49:46.014872 mlflowops-0.1.1/mlflowops/__init__.py
+-rw-r--r--   0        0        0     6633 2023-07-21 04:49:46.014872 mlflowops-0.1.1/mlflowops/mlflowops.py
+-rw-r--r--   0        0        0     4724 2023-07-21 04:49:46.014872 mlflowops-0.1.1/mlflowops/session.py
+-rw-r--r--   0        0        0      544 2023-07-21 04:49:46.014872 mlflowops-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1633 1970-01-01 00:00:00.000000 mlflowops-0.1.1/PKG-INFO
```

### Comparing `mlflowops-0.1.0/LICENSE` & `mlflowops-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlflowops-0.1.0/README.md` & `mlflowops-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mlflowops-0.1.0/mlflowops/mlflowops.py` & `mlflowops-0.1.1/mlflowops/mlflowops.py`

 * *Files identical despite different names*

### Comparing `mlflowops-0.1.0/mlflowops/session.py` & `mlflowops-0.1.1/mlflowops/session.py`

 * *Files identical despite different names*

### Comparing `mlflowops-0.1.0/pyproject.toml` & `mlflowops-0.1.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "mlflowops"
-version = "0.1.0"
+version = "0.1.1"
 description = "MLOps utils with MLFlow"
 authors = ["Carlos D. Escobar-Valbuena <carlosdavidescobar@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "mlflowops"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
+pandas = "^2.0.3"
+pydantic = "^2.0.3"
 mlflow = "^2.5.0"
-pydantic = "^1.10.9"
 python-dotenv = "^1.0.0"
-typing-extensions = "^4.7.0"
 azure-ai-ml = "^1.8.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 black = "^23.3.0"
 
 [build-system]
```

### Comparing `mlflowops-0.1.0/PKG-INFO` & `mlflowops-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: mlflowops
-Version: 0.1.0
+Version: 0.1.1
 Summary: MLOps utils with MLFlow
 License: MIT
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: azure-ai-ml (>=1.8.0,<2.0.0)
 Requires-Dist: mlflow (>=2.5.0,<3.0.0)
-Requires-Dist: pydantic (>=1.10.9,<2.0.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: pydantic (>=2.0.3,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: typing-extensions (>=4.7.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # mlflowops Util
 **MLOps utils with MLFlow**
 
 
 ## Setup
```

