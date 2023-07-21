# Comparing `tmp/botoful-0.4.0.tar.gz` & `tmp/botoful-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botoful-0.4.0.tar", max compression
+gzip compressed data, was "botoful-0.4.1.tar", max compression
```

## Comparing `botoful-0.4.0.tar` & `botoful-0.4.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2023-07-20 07:25:54.490522 botoful-0.4.0/LICENSE
--rw-r--r--   0        0        0       78 2023-07-20 11:03:03.737257 botoful-0.4.0/botoful/__init__.py
--rw-r--r--   0        0        0      738 2023-07-20 07:25:54.490522 botoful-0.4.0/botoful/filters.py
--rw-r--r--   0        0        0     8653 2023-07-20 08:36:05.228656 botoful-0.4.0/botoful/query.py
--rw-r--r--   0        0        0     7158 2023-07-20 07:25:54.490522 botoful-0.4.0/botoful/reserved.py
--rw-r--r--   0        0        0      274 2023-07-20 07:25:54.490522 botoful-0.4.0/botoful/serializers.py
--rw-r--r--   0        0        0     4109 2023-07-20 11:11:31.681387 botoful-0.4.0/botoful/table.py
--rw-r--r--   0        0        0      677 2023-07-20 11:09:26.123384 botoful-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 botoful-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-07-20 07:25:54.490522 botoful-0.4.1/LICENSE
+-rw-r--r--   0        0        0       78 2023-07-20 11:03:03.737257 botoful-0.4.1/botoful/__init__.py
+-rw-r--r--   0        0        0      738 2023-07-20 07:25:54.490522 botoful-0.4.1/botoful/filters.py
+-rw-r--r--   0        0        0     8653 2023-07-20 08:36:05.228656 botoful-0.4.1/botoful/query.py
+-rw-r--r--   0        0        0     7158 2023-07-20 07:25:54.490522 botoful-0.4.1/botoful/reserved.py
+-rw-r--r--   0        0        0      274 2023-07-20 07:25:54.490522 botoful-0.4.1/botoful/serializers.py
+-rw-r--r--   0        0        0     4109 2023-07-20 11:11:31.681387 botoful-0.4.1/botoful/table.py
+-rw-r--r--   0        0        0      677 2023-07-21 06:58:26.230600 botoful-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      715 1970-01-01 00:00:00.000000 botoful-0.4.1/PKG-INFO
```

### Comparing `botoful-0.4.0/LICENSE` & `botoful-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `botoful-0.4.0/botoful/filters.py` & `botoful-0.4.1/botoful/filters.py`

 * *Files identical despite different names*

### Comparing `botoful-0.4.0/botoful/query.py` & `botoful-0.4.1/botoful/query.py`

 * *Files identical despite different names*

### Comparing `botoful-0.4.0/botoful/reserved.py` & `botoful-0.4.1/botoful/reserved.py`

 * *Files identical despite different names*

### Comparing `botoful-0.4.0/botoful/table.py` & `botoful-0.4.1/botoful/table.py`

 * *Files identical despite different names*

### Comparing `botoful-0.4.0/pyproject.toml` & `botoful-0.4.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "botoful"
-version = "0.4.0"
+version = "0.4.1"
 description = "A beautiful boto wrapper"
 authors = ["Imtiaz Mangerah <Imtiaz_Mangerah@a2d24.com>"]
 license = "MIT"
 homepage = "https://www.botoful.com"
 repository = "https://github.com/a2d24/botoful"
 documentation = "https://www.botoful.com"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 boto3 = {version = "^1.17.23", optional = true}
-moto = {extras = ["dynamodb"], version = "^4.1.13"}
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.2"
 pytest-cov = "^2.11.1"
 Pygments = "^2.8.1"
 boto3 = "^1.17.23"
+moto = {extras = ["dynamodb"], version = "^4.1.13"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.extras]
 boto = ["boto3"]
```

### Comparing `botoful-0.4.0/PKG-INFO` & `botoful-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: botoful
-Version: 0.4.0
+Version: 0.4.1
 Summary: A beautiful boto wrapper
 Home-page: https://www.botoful.com
 License: MIT
 Author: Imtiaz Mangerah
 Author-email: Imtiaz_Mangerah@a2d24.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: boto
 Requires-Dist: boto3 (>=1.17.23,<2.0.0) ; extra == "boto"
-Requires-Dist: moto[dynamodb] (>=4.1.13,<5.0.0)
 Project-URL: Documentation, https://www.botoful.com
 Project-URL: Repository, https://github.com/a2d24/botoful
```

