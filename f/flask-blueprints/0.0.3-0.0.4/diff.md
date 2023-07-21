# Comparing `tmp/flask-blueprints-0.0.3.tar.gz` & `tmp/flask-blueprints-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-blueprints-0.0.3.tar", last modified: Fri Jul 21 12:11:57 2023, max compression
+gzip compressed data, was "flask-blueprints-0.0.4.tar", last modified: Fri Jul 21 12:54:53 2023, max compression
```

## Comparing `flask-blueprints-0.0.3.tar` & `flask-blueprints-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-07-21 12:11:57.355502 flask-blueprints-0.0.3/
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     1515 2023-07-21 11:43:15.000000 flask-blueprints-0.0.3/LICENSE
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      726 2023-07-21 12:11:57.355502 flask-blueprints-0.0.3/PKG-INFO
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)       95 2023-07-21 11:57:54.000000 flask-blueprints-0.0.3/README.md
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      612 2023-07-21 12:11:46.000000 flask-blueprints-0.0.3/pyproject.toml
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)       38 2023-07-21 12:11:57.355502 flask-blueprints-0.0.3/setup.cfg
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-07-21 12:11:57.353502 flask-blueprints-0.0.3/src/
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-07-21 12:11:57.354502 flask-blueprints-0.0.3/src/flask_blueprints/
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      902 2023-07-21 11:46:19.000000 flask-blueprints-0.0.3/src/flask_blueprints/__init__.py
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-07-21 12:11:57.355502 flask-blueprints-0.0.3/src/flask_blueprints.egg-info/
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      726 2023-07-21 12:11:57.000000 flask-blueprints-0.0.3/src/flask_blueprints.egg-info/PKG-INFO
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      241 2023-07-21 12:11:57.000000 flask-blueprints-0.0.3/src/flask_blueprints.egg-info/SOURCES.txt
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)        1 2023-07-21 12:11:57.000000 flask-blueprints-0.0.3/src/flask_blueprints.egg-info/dependency_links.txt
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)       17 2023-07-21 12:11:57.000000 flask-blueprints-0.0.3/src/flask_blueprints.egg-info/top_level.txt
+drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-07-21 12:54:53.038217 flask-blueprints-0.0.4/
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     1504 2023-07-21 12:53:12.000000 flask-blueprints-0.0.4/LICENSE
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     3156 2023-07-21 12:54:53.038217 flask-blueprints-0.0.4/PKG-INFO
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     2525 2023-07-21 12:51:46.000000 flask-blueprints-0.0.4/README.md
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      612 2023-07-21 12:52:02.000000 flask-blueprints-0.0.4/pyproject.toml
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)       38 2023-07-21 12:54:53.038217 flask-blueprints-0.0.4/setup.cfg
+drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-07-21 12:54:53.036217 flask-blueprints-0.0.4/src/
+drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-07-21 12:54:53.037217 flask-blueprints-0.0.4/src/flask_blueprints/
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      902 2023-07-21 11:46:19.000000 flask-blueprints-0.0.4/src/flask_blueprints/__init__.py
+drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-07-21 12:54:53.038217 flask-blueprints-0.0.4/src/flask_blueprints.egg-info/
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     3156 2023-07-21 12:54:53.000000 flask-blueprints-0.0.4/src/flask_blueprints.egg-info/PKG-INFO
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      241 2023-07-21 12:54:53.000000 flask-blueprints-0.0.4/src/flask_blueprints.egg-info/SOURCES.txt
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)        1 2023-07-21 12:54:53.000000 flask-blueprints-0.0.4/src/flask_blueprints.egg-info/dependency_links.txt
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)       17 2023-07-21 12:54:53.000000 flask-blueprints-0.0.4/src/flask_blueprints.egg-info/top_level.txt
```

### Comparing `flask-blueprints-0.0.3/LICENSE` & `flask-blueprints-0.0.4/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2023, Безбородов, Д.Р.
+Copyright (c) 2023, Damien Bezborodov
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `flask-blueprints-0.0.3/pyproject.toml` & `flask-blueprints-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "flask-blueprints"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Damien Bezborodov", email="dbezborodov@gmail.com" },
 ]
 description = "Register all Flask Blueprints (including nested) from a package directory."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `flask-blueprints-0.0.3/src/flask_blueprints/__init__.py` & `flask-blueprints-0.0.4/src/flask_blueprints/__init__.py`

 * *Files identical despite different names*

