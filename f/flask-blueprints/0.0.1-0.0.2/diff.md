# Comparing `tmp/flask-blueprints-0.0.1.tar.gz` & `tmp/flask-blueprints-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-blueprints-0.0.1.tar", last modified: Fri Jul 21 11:57:19 2023, max compression
+gzip compressed data, was "flask-blueprints-0.0.2.tar", last modified: Fri Jul 21 12:07:32 2023, max compression
```

## Comparing `flask-blueprints-0.0.1.tar` & `flask-blueprints-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-07-21 11:57:19.977672 flask-blueprints-0.0.1/
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     1515 2023-07-21 11:43:15.000000 flask-blueprints-0.0.1/LICENSE
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      734 2023-07-21 11:57:19.977672 flask-blueprints-0.0.1/PKG-INFO
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      103 2023-07-21 11:43:15.000000 flask-blueprints-0.0.1/README.md
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      612 2023-07-21 11:57:02.000000 flask-blueprints-0.0.1/pyproject.toml
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)       38 2023-07-21 11:57:19.977672 flask-blueprints-0.0.1/setup.cfg
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-07-21 11:57:19.975672 flask-blueprints-0.0.1/src/
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-07-21 11:57:19.976672 flask-blueprints-0.0.1/src/flask-register-blueprints/
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      902 2023-07-21 11:46:19.000000 flask-blueprints-0.0.1/src/flask-register-blueprints/__init__.py
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-07-21 11:57:19.977672 flask-blueprints-0.0.1/src/flask_blueprints.egg-info/
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      734 2023-07-21 11:57:19.000000 flask-blueprints-0.0.1/src/flask_blueprints.egg-info/PKG-INFO
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      250 2023-07-21 11:57:19.000000 flask-blueprints-0.0.1/src/flask_blueprints.egg-info/SOURCES.txt
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)        1 2023-07-21 11:57:19.000000 flask-blueprints-0.0.1/src/flask_blueprints.egg-info/dependency_links.txt
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)       26 2023-07-21 11:57:19.000000 flask-blueprints-0.0.1/src/flask_blueprints.egg-info/top_level.txt
+drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-07-21 12:07:32.259786 flask-blueprints-0.0.2/
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     1515 2023-07-21 11:43:15.000000 flask-blueprints-0.0.2/LICENSE
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      726 2023-07-21 12:07:32.259786 flask-blueprints-0.0.2/PKG-INFO
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)       95 2023-07-21 11:57:54.000000 flask-blueprints-0.0.2/README.md
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      612 2023-07-21 12:07:23.000000 flask-blueprints-0.0.2/pyproject.toml
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)       38 2023-07-21 12:07:32.259786 flask-blueprints-0.0.2/setup.cfg
+drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-07-21 12:07:32.257786 flask-blueprints-0.0.2/src/
+drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-07-21 12:07:32.258786 flask-blueprints-0.0.2/src/flask-blueprints/
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      902 2023-07-21 11:46:19.000000 flask-blueprints-0.0.2/src/flask-blueprints/__init__.py
+drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-07-21 12:07:32.259786 flask-blueprints-0.0.2/src/flask_blueprints.egg-info/
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      726 2023-07-21 12:07:32.000000 flask-blueprints-0.0.2/src/flask_blueprints.egg-info/PKG-INFO
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      241 2023-07-21 12:07:32.000000 flask-blueprints-0.0.2/src/flask_blueprints.egg-info/SOURCES.txt
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)        1 2023-07-21 12:07:32.000000 flask-blueprints-0.0.2/src/flask_blueprints.egg-info/dependency_links.txt
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)       17 2023-07-21 12:07:32.000000 flask-blueprints-0.0.2/src/flask_blueprints.egg-info/top_level.txt
```

### Comparing `flask-blueprints-0.0.1/LICENSE` & `flask-blueprints-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-blueprints-0.0.1/PKG-INFO` & `flask-blueprints-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: flask-blueprints
-Version: 0.0.1
+Version: 0.0.2
 Summary: Register all Flask Blueprints (including nested) from a package directory.
 Author-email: Damien Bezborodov <dbezborodov@gmail.com>
 Project-URL: Homepage, https://github.com/bezborodow/flask-register-blueprints
 Project-URL: Bug Tracker, https://github.com/bezborodow/flask-register-blueprints/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Flask
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# flask-register-blueprints
+# flask-blueprints
+
 Register all Flask Blueprints (including nested) from a package directory.
```

### Comparing `flask-blueprints-0.0.1/pyproject.toml` & `flask-blueprints-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "flask-blueprints"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Damien Bezborodov", email="dbezborodov@gmail.com" },
 ]
 description = "Register all Flask Blueprints (including nested) from a package directory."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `flask-blueprints-0.0.1/src/flask-register-blueprints/__init__.py` & `flask-blueprints-0.0.2/src/flask-blueprints/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-blueprints-0.0.1/src/flask_blueprints.egg-info/PKG-INFO` & `flask-blueprints-0.0.2/src/flask_blueprints.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: flask-blueprints
-Version: 0.0.1
+Version: 0.0.2
 Summary: Register all Flask Blueprints (including nested) from a package directory.
 Author-email: Damien Bezborodov <dbezborodov@gmail.com>
 Project-URL: Homepage, https://github.com/bezborodow/flask-register-blueprints
 Project-URL: Bug Tracker, https://github.com/bezborodow/flask-register-blueprints/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Flask
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# flask-register-blueprints
+# flask-blueprints
+
 Register all Flask Blueprints (including nested) from a package directory.
```

