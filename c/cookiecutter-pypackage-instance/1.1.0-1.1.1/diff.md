# Comparing `tmp/cookiecutter_pypackage_instance-1.1.0.tar.gz` & `tmp/cookiecutter_pypackage_instance-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookiecutter_pypackage_instance-1.1.0.tar", max compression
+gzip compressed data, was "cookiecutter_pypackage_instance-1.1.1.tar", max compression
```

## Comparing `cookiecutter_pypackage_instance-1.1.0.tar` & `cookiecutter_pypackage_instance-1.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1089 2023-07-21 06:17:50.180215 cookiecutter_pypackage_instance-1.1.0/LICENSE
--rw-r--r--   0        0        0     4320 2023-07-21 06:17:50.180215 cookiecutter_pypackage_instance-1.1.0/README.md
--rw-r--r--   0        0        0     5106 2023-07-21 06:17:51.556273 cookiecutter_pypackage_instance-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       82 2023-07-21 06:17:50.184215 cookiecutter_pypackage_instance-1.1.0/src/cookiecutter_pypackage_instance/__init__.py
--rw-r--r--   0        0        0      417 2023-07-21 06:17:50.184215 cookiecutter_pypackage_instance-1.1.0/src/cookiecutter_pypackage_instance/cookiecutter_pypackage_instance.py
--rw-r--r--   0        0        0        0 2023-07-21 06:17:50.184215 cookiecutter_pypackage_instance-1.1.0/src/cookiecutter_pypackage_instance/py.typed
--rw-r--r--   0        0        0     5421 1970-01-01 00:00:00.000000 cookiecutter_pypackage_instance-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-07-21 06:57:10.923065 cookiecutter_pypackage_instance-1.1.1/LICENSE
+-rw-r--r--   0        0        0     4320 2023-07-21 06:57:10.923065 cookiecutter_pypackage_instance-1.1.1/README.md
+-rw-r--r--   0        0        0     5106 2023-07-21 06:57:12.507074 cookiecutter_pypackage_instance-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       82 2023-07-21 06:57:10.927065 cookiecutter_pypackage_instance-1.1.1/src/cookiecutter_pypackage_instance/__init__.py
+-rw-r--r--   0        0        0      417 2023-07-21 06:57:10.927065 cookiecutter_pypackage_instance-1.1.1/src/cookiecutter_pypackage_instance/cookiecutter_pypackage_instance.py
+-rw-r--r--   0        0        0        0 2023-07-21 06:57:10.927065 cookiecutter_pypackage_instance-1.1.1/src/cookiecutter_pypackage_instance/py.typed
+-rw-r--r--   0        0        0     5421 1970-01-01 00:00:00.000000 cookiecutter_pypackage_instance-1.1.1/PKG-INFO
```

### Comparing `cookiecutter_pypackage_instance-1.1.0/LICENSE` & `cookiecutter_pypackage_instance-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cookiecutter_pypackage_instance-1.1.0/README.md` & `cookiecutter_pypackage_instance-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cookiecutter_pypackage_instance-1.1.0/pyproject.toml` & `cookiecutter_pypackage_instance-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
 strict = true
 
 [tool.poetry]
 name = "cookiecutter-pypackage-instance"
-version = "1.1.0"
+version = "1.1.1"
 description = "🐍 An awesome python package by the name Cookiecutter Pypackage Instance"
 readme = "README.md"
 authors = ["Vasilis Sioros <billsioros97@gmail.com>"]
 license = "MIT"
 homepage = "https://billsioros.github.io/cookiecutter-pypackage-instance"
 repository = "https://github.com/billsioros/cookiecutter-pypackage-instance"
 keywords = []
```

### Comparing `cookiecutter_pypackage_instance-1.1.0/PKG-INFO` & `cookiecutter_pypackage_instance-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiecutter-pypackage-instance
-Version: 1.1.0
+Version: 1.1.1
 Summary: 🐍 An awesome python package by the name Cookiecutter Pypackage Instance
 Home-page: https://billsioros.github.io/cookiecutter-pypackage-instance
 License: MIT
 Author: Vasilis Sioros
 Author-email: billsioros97@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cookiecutter-pypackage-instance Version: 1.1.0
+Metadata-Version: 2.1 Name: cookiecutter-pypackage-instance Version: 1.1.1
 Summary: ð An awesome python package by the name Cookiecutter Pypackage
 Instance Home-page: https://billsioros.github.io/cookiecutter-pypackage-
 instance License: MIT Author: Vasilis Sioros Author-email:
 billsioros97@gmail.com Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

