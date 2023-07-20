# Comparing `tmp/Flask_Limit-2.0.1.tar.gz` & `tmp/Flask_Limit-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask_Limit-2.0.1.tar", last modified: Thu Jun 22 23:10:57 2023, max compression
+gzip compressed data, was "Flask_Limit-2.0.2.tar", last modified: Thu Jul 20 23:24:11 2023, max compression
```

## Comparing `Flask_Limit-2.0.1.tar` & `Flask_Limit-2.0.2.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-06-22 23:10:57.140514 Flask_Limit-2.0.1/
--rw-r--r--   0 tabot      (501) staff       (20)       35 2023-06-11 23:35:14.000000 Flask_Limit-2.0.1/AUTHORS
--rw-r--r--   0 tabot      (501) staff       (20)     1068 2023-06-11 23:35:14.000000 Flask_Limit-2.0.1/LICENSE
--rw-r--r--   0 tabot      (501) staff       (20)       80 2023-06-11 23:35:14.000000 Flask_Limit-2.0.1/MANIFEST.in
--rw-r--r--   0 tabot      (501) staff       (20)     4104 2023-06-22 23:10:57.140574 Flask_Limit-2.0.1/PKG-INFO
--rw-r--r--   0 tabot      (501) staff       (20)     3443 2023-06-22 22:06:20.000000 Flask_Limit-2.0.1/README.md
-drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-06-22 23:10:57.137713 Flask_Limit-2.0.1/docs/
--rw-r--r--   0 tabot      (501) staff       (20)     4165 2023-06-22 23:09:02.000000 Flask_Limit-2.0.1/docs/index.rst
--rw-r--r--   0 tabot      (501) staff       (20)   850764 2023-06-22 21:19:36.000000 Flask_Limit-2.0.1/docs/proof.png
-drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-06-22 23:10:57.136247 Flask_Limit-2.0.1/flask_limit/
-drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-06-22 23:10:57.139326 Flask_Limit-2.0.1/flask_limit/Flask_Limit.egg-info/
--rw-r--r--   0 tabot      (501) staff       (20)     4104 2023-06-22 23:10:57.000000 Flask_Limit-2.0.1/flask_limit/Flask_Limit.egg-info/PKG-INFO
--rw-r--r--   0 tabot      (501) staff       (20)      525 2023-06-22 23:10:57.000000 Flask_Limit-2.0.1/flask_limit/Flask_Limit.egg-info/SOURCES.txt
--rw-r--r--   0 tabot      (501) staff       (20)        1 2023-06-22 23:10:57.000000 Flask_Limit-2.0.1/flask_limit/Flask_Limit.egg-info/dependency_links.txt
--rw-r--r--   0 tabot      (501) staff       (20)        1 2023-06-19 02:52:57.000000 Flask_Limit-2.0.1/flask_limit/Flask_Limit.egg-info/not-zip-safe
--rw-r--r--   0 tabot      (501) staff       (20)       32 2023-06-22 23:10:57.000000 Flask_Limit-2.0.1/flask_limit/Flask_Limit.egg-info/requires.txt
--rw-r--r--   0 tabot      (501) staff       (20)        9 2023-06-22 23:10:57.000000 Flask_Limit-2.0.1/flask_limit/Flask_Limit.egg-info/top_level.txt
-drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-06-22 23:10:57.140059 Flask_Limit-2.0.1/flask_limit/limiters/
--rw-r--r--   0 tabot      (501) staff       (20)      120 2023-06-19 02:52:18.000000 Flask_Limit-2.0.1/flask_limit/limiters/__init__.py
--rw-r--r--   0 tabot      (501) staff       (20)       44 2023-06-18 17:50:49.000000 Flask_Limit-2.0.1/flask_limit/limiters/exceptions.py
--rw-r--r--   0 tabot      (501) staff       (20)     2354 2023-06-18 17:48:16.000000 Flask_Limit-2.0.1/flask_limit/limiters/limiters.py
--rw-r--r--   0 tabot      (501) staff       (20)       95 2023-06-19 02:37:16.000000 Flask_Limit-2.0.1/pyproject.toml
--rw-r--r--   0 tabot      (501) staff       (20)      872 2023-06-22 23:10:57.140829 Flask_Limit-2.0.1/setup.cfg
--rwxr-xr-x   0 tabot      (501) staff       (20)       38 2023-06-19 01:33:15.000000 Flask_Limit-2.0.1/setup.py
-drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-06-22 23:10:57.140372 Flask_Limit-2.0.1/tests/
--rw-r--r--   0 tabot      (501) staff       (20)        0 2023-06-11 23:35:14.000000 Flask_Limit-2.0.1/tests/__init__.py
--rw-r--r--   0 tabot      (501) staff       (20)     2048 2023-06-22 20:24:17.000000 Flask_Limit-2.0.1/tests/test_rate_limit.py
+drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-07-20 23:24:11.427669 Flask_Limit-2.0.2/
+-rw-r--r--   0 tabot      (501) staff       (20)       35 2023-07-20 22:32:05.000000 Flask_Limit-2.0.2/AUTHORS
+-rw-r--r--   0 tabot      (501) staff       (20)     1068 2023-07-20 22:32:05.000000 Flask_Limit-2.0.2/LICENSE
+-rw-r--r--   0 tabot      (501) staff       (20)       80 2023-07-20 22:32:05.000000 Flask_Limit-2.0.2/MANIFEST.in
+-rw-r--r--   0 tabot      (501) staff       (20)     4104 2023-07-20 23:24:11.427731 Flask_Limit-2.0.2/PKG-INFO
+-rw-r--r--   0 tabot      (501) staff       (20)     3443 2023-07-20 22:32:05.000000 Flask_Limit-2.0.2/README.md
+drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-07-20 23:24:11.425471 Flask_Limit-2.0.2/docs/
+-rw-r--r--   0 tabot      (501) staff       (20)     4165 2023-07-20 22:32:05.000000 Flask_Limit-2.0.2/docs/index.rst
+-rw-r--r--   0 tabot      (501) staff       (20)   850764 2023-07-20 22:32:05.000000 Flask_Limit-2.0.2/docs/proof.png
+-rw-r--r--   0 tabot      (501) staff       (20)       95 2023-07-20 22:32:05.000000 Flask_Limit-2.0.2/pyproject.toml
+-rw-r--r--   0 tabot      (501) staff       (20)      856 2023-07-20 23:24:11.427981 Flask_Limit-2.0.2/setup.cfg
+-rwxr-xr-x   0 tabot      (501) staff       (20)       38 2023-07-20 22:32:05.000000 Flask_Limit-2.0.2/setup.py
+drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-07-20 23:24:11.424155 Flask_Limit-2.0.2/src/
+drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-07-20 23:24:11.426717 Flask_Limit-2.0.2/src/Flask_Limit.egg-info/
+-rw-r--r--   0 tabot      (501) staff       (20)     4104 2023-07-20 23:24:11.000000 Flask_Limit-2.0.2/src/Flask_Limit.egg-info/PKG-INFO
+-rw-r--r--   0 tabot      (501) staff       (20)      547 2023-07-20 23:24:11.000000 Flask_Limit-2.0.2/src/Flask_Limit.egg-info/SOURCES.txt
+-rw-r--r--   0 tabot      (501) staff       (20)        1 2023-07-20 23:24:11.000000 Flask_Limit-2.0.2/src/Flask_Limit.egg-info/dependency_links.txt
+-rw-r--r--   0 tabot      (501) staff       (20)        1 2023-07-20 23:05:20.000000 Flask_Limit-2.0.2/src/Flask_Limit.egg-info/not-zip-safe
+-rw-r--r--   0 tabot      (501) staff       (20)       32 2023-07-20 23:24:11.000000 Flask_Limit-2.0.2/src/Flask_Limit.egg-info/requires.txt
+-rw-r--r--   0 tabot      (501) staff       (20)       12 2023-07-20 23:24:11.000000 Flask_Limit-2.0.2/src/Flask_Limit.egg-info/top_level.txt
+drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-07-20 23:24:11.426975 Flask_Limit-2.0.2/src/flask_limit/
+-rw-r--r--   0 tabot      (501) staff       (20)       50 2023-07-20 22:32:05.000000 Flask_Limit-2.0.2/src/flask_limit/__init__.py
+drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-07-20 23:24:11.427337 Flask_Limit-2.0.2/src/flask_limit/limiters/
+-rw-r--r--   0 tabot      (501) staff       (20)      120 2023-07-20 22:32:05.000000 Flask_Limit-2.0.2/src/flask_limit/limiters/__init__.py
+-rw-r--r--   0 tabot      (501) staff       (20)       44 2023-07-20 22:32:05.000000 Flask_Limit-2.0.2/src/flask_limit/limiters/exceptions.py
+-rw-r--r--   0 tabot      (501) staff       (20)     2354 2023-07-20 22:32:05.000000 Flask_Limit-2.0.2/src/flask_limit/limiters/limiters.py
+-rwxr-xr-x   0 tabot      (501) staff       (20)     3682 2023-07-20 22:32:05.000000 Flask_Limit-2.0.2/src/flask_limit/rate_limit.py
+drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-07-20 23:24:11.427558 Flask_Limit-2.0.2/tests/
+-rw-r--r--   0 tabot      (501) staff       (20)        0 2023-07-20 22:32:05.000000 Flask_Limit-2.0.2/tests/__init__.py
+-rw-r--r--   0 tabot      (501) staff       (20)     2048 2023-07-20 22:32:05.000000 Flask_Limit-2.0.2/tests/test_rate_limit.py
```

### Comparing `Flask_Limit-2.0.1/LICENSE` & `Flask_Limit-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask_Limit-2.0.1/PKG-INFO` & `Flask_Limit-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask_Limit
-Version: 2.0.1
+Version: 2.0.2
 Summary: An extension that provides rate limiting for Flask routes.
 Home-page: https://github.com/tabotkevin/flask_limit
 Author: Tabot Kevin
 Author-email: tabot.kevin@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/tabotkevin/flask_limit/issues
 Classifier: Environment :: Web Environment
```

### Comparing `Flask_Limit-2.0.1/README.md` & `Flask_Limit-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `Flask_Limit-2.0.1/docs/index.rst` & `Flask_Limit-2.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Flask_Limit-2.0.1/docs/proof.png` & `Flask_Limit-2.0.2/docs/proof.png`

 * *Files identical despite different names*

### Comparing `Flask_Limit-2.0.1/flask_limit/Flask_Limit.egg-info/PKG-INFO` & `Flask_Limit-2.0.2/src/Flask_Limit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Limit
-Version: 2.0.1
+Version: 2.0.2
 Summary: An extension that provides rate limiting for Flask routes.
 Home-page: https://github.com/tabotkevin/flask_limit
 Author: Tabot Kevin
 Author-email: tabot.kevin@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/tabotkevin/flask_limit/issues
 Classifier: Environment :: Web Environment
```

### Comparing `Flask_Limit-2.0.1/flask_limit/Flask_Limit.egg-info/SOURCES.txt` & `Flask_Limit-2.0.2/src/Flask_Limit.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 docs/index.rst
 docs/proof.png
-flask_limit/Flask_Limit.egg-info/PKG-INFO
-flask_limit/Flask_Limit.egg-info/SOURCES.txt
-flask_limit/Flask_Limit.egg-info/dependency_links.txt
-flask_limit/Flask_Limit.egg-info/not-zip-safe
-flask_limit/Flask_Limit.egg-info/requires.txt
-flask_limit/Flask_Limit.egg-info/top_level.txt
-flask_limit/limiters/__init__.py
-flask_limit/limiters/exceptions.py
-flask_limit/limiters/limiters.py
+src/Flask_Limit.egg-info/PKG-INFO
+src/Flask_Limit.egg-info/SOURCES.txt
+src/Flask_Limit.egg-info/dependency_links.txt
+src/Flask_Limit.egg-info/not-zip-safe
+src/Flask_Limit.egg-info/requires.txt
+src/Flask_Limit.egg-info/top_level.txt
+src/flask_limit/__init__.py
+src/flask_limit/rate_limit.py
+src/flask_limit/limiters/__init__.py
+src/flask_limit/limiters/exceptions.py
+src/flask_limit/limiters/limiters.py
 tests/__init__.py
 tests/test_rate_limit.py
```

### Comparing `Flask_Limit-2.0.1/flask_limit/limiters/limiters.py` & `Flask_Limit-2.0.2/src/flask_limit/limiters/limiters.py`

 * *Files identical despite different names*

### Comparing `Flask_Limit-2.0.1/tests/test_rate_limit.py` & `Flask_Limit-2.0.2/tests/test_rate_limit.py`

 * *Files identical despite different names*

