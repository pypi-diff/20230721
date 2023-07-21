# Comparing `tmp/pandus-2.0.2.tar.gz` & `tmp/pandus-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandus-2.0.2.tar", max compression
+gzip compressed data, was "pandus-2.0.3.tar", max compression
```

## Comparing `pandus-2.0.2.tar` & `pandus-2.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2023-02-14 09:23:55.719510 pandus-2.0.2/LICENSE
--rw-r--r--   0        0        0      705 2023-04-03 15:05:57.050972 pandus-2.0.2/README.md
--rw-r--r--   0        0        0       80 2023-02-14 09:35:19.822392 pandus-2.0.2/pandus/__init__.py
--rw-r--r--   0        0        0      210 2023-02-14 17:46:26.960126 pandus-2.0.2/pandus/pandus.py
--rw-r--r--   0        0        0      774 2023-07-21 11:36:46.429373 pandus-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 pandus-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-02-14 09:23:55.719510 pandus-2.0.3/LICENSE
+-rw-r--r--   0        0        0      705 2023-04-03 15:05:57.050972 pandus-2.0.3/README.md
+-rw-r--r--   0        0        0       80 2023-02-14 09:35:19.822392 pandus-2.0.3/pandus/__init__.py
+-rw-r--r--   0        0        0      210 2023-02-14 17:46:26.960126 pandus-2.0.3/pandus/pandus.py
+-rw-r--r--   0        0        0      774 2023-07-21 11:41:06.037594 pandus-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 pandus-2.0.3/PKG-INFO
```

### Comparing `pandus-2.0.2/LICENSE` & `pandus-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pandus-2.0.2/README.md` & `pandus-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pandus-2.0.2/pyproject.toml` & `pandus-2.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandus"
-version = "2.0.2"
+version = "2.0.3"
 description = "A simple wrapper around Pandas"
 authors = ["Egor Georgiev"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/egor-georgiev/pandus"
 repository = "https://github.com/egor-georgiev/pandus"
 keywords = ["pandus", "pandas", "data-science", "data-analysis"]
@@ -15,14 +15,14 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-pandas = "2.0.2"
+pandas = "2.0.3"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pandus-2.0.2/PKG-INFO` & `pandus-2.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pandus
-Version: 2.0.2
+Version: 2.0.3
 Summary: A simple wrapper around Pandas
 Home-page: https://github.com/egor-georgiev/pandus
 License: MIT
 Keywords: pandus,pandas,data-science,data-analysis
 Author: Egor Georgiev
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: pandas (==2.0.2)
+Requires-Dist: pandas (==2.0.3)
 Project-URL: Repository, https://github.com/egor-georgiev/pandus
 Description-Content-Type: text/markdown
 
 # pandus
 [![PyPI version](https://badge.fury.io/py/pandus.svg)](https://badge.fury.io/py/pandus)
 
 ## What is it?
```

