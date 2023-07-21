# Comparing `tmp/plink_pipelines-0.1.6a0.tar.gz` & `tmp/plink_pipelines-0.1.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plink_pipelines-0.1.6a0.tar", max compression
+gzip compressed data, was "plink_pipelines-0.1.7a0.tar", max compression
```

## Comparing `plink_pipelines-0.1.6a0.tar` & `plink_pipelines-0.1.7a0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34523 2023-04-13 15:40:12.491581 plink_pipelines-0.1.6a0/LICENSE
--rw-r--r--   0        0        0        0 2023-04-13 15:40:12.491581 plink_pipelines-0.1.6a0/plink_pipelines/__init__.py
--rw-r--r--   0        0        0    15580 2023-04-13 15:40:12.491581 plink_pipelines-0.1.6a0/plink_pipelines/make_dataset.py
--rw-r--r--   0        0        0      417 2023-04-13 15:40:12.491581 plink_pipelines-0.1.6a0/plink_pipelines/validation_functions.py
--rw-r--r--   0        0        0      845 2023-04-13 15:40:12.495581 plink_pipelines-0.1.6a0/pyproject.toml
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 plink_pipelines-0.1.6a0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2021-06-10 12:58:24.000000 plink_pipelines-0.1.7a0/LICENSE
+-rw-r--r--   0        0        0        0 2021-06-10 12:58:24.000000 plink_pipelines-0.1.7a0/plink_pipelines/__init__.py
+-rw-r--r--   0        0        0    15580 2023-04-13 15:22:21.776348 plink_pipelines-0.1.7a0/plink_pipelines/make_dataset.py
+-rw-r--r--   0        0        0      417 2023-04-13 15:18:20.326181 plink_pipelines-0.1.7a0/plink_pipelines/validation_functions.py
+-rw-r--r--   0        0        0      845 2023-07-21 13:16:16.940552 plink_pipelines-0.1.7a0/pyproject.toml
+-rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 plink_pipelines-0.1.7a0/PKG-INFO
```

### Comparing `plink_pipelines-0.1.6a0/LICENSE` & `plink_pipelines-0.1.7a0/LICENSE`

 * *Files identical despite different names*

### Comparing `plink_pipelines-0.1.6a0/plink_pipelines/make_dataset.py` & `plink_pipelines-0.1.7a0/plink_pipelines/make_dataset.py`

 * *Files identical despite different names*

### Comparing `plink_pipelines-0.1.6a0/pyproject.toml` & `plink_pipelines-0.1.7a0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "plink_pipelines"
-version = "0.1.6-alpha"
+version = "0.1.7-alpha"
 description = ""
 authors = ["Arnor Sigurdsson <arnor-sigurdsson@users.noreply.github.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pandas = "^1.2.4"
+pandas = "^2.0.3"
 py = "^1.10.0"
 luigi = "^3.0.3"
 aislib = "^0.1.6-alpha.0"
 bed-reader = "^0.2.24"
 deeplake = "^3.0.13"
 # Freeze numpy due to some 1.24 compatibility issues
 numpy = "1.23.5"
```

### Comparing `plink_pipelines-0.1.6a0/PKG-INFO` & `plink_pipelines-0.1.7a0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: plink-pipelines
-Version: 0.1.6a0
+Version: 0.1.7a0
 Summary: 
 Author: Arnor Sigurdsson
 Author-email: arnor-sigurdsson@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aislib (>=0.1.6-alpha.0,<0.2.0)
 Requires-Dist: bed-reader (>=0.2.24,<0.3.0)
 Requires-Dist: deeplake (>=3.0.13,<4.0.0)
 Requires-Dist: luigi (>=3.0.3,<4.0.0)
 Requires-Dist: numpy (==1.23.5)
-Requires-Dist: pandas (>=1.2.4,<2.0.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: py (>=1.10.0,<2.0.0)
```

