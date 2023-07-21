# Comparing `tmp/macaquedb-0.1.4.tar.gz` & `tmp/macaquedb-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macaquedb-0.1.4.tar", last modified: Fri Jul 21 14:58:02 2023, max compression
+gzip compressed data, was "macaquedb-0.1.5.tar", last modified: Fri Jul 21 14:59:17 2023, max compression
```

## Comparing `macaquedb-0.1.4.tar` & `macaquedb-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-21 14:58:02.751375 macaquedb-0.1.4/
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      268 2023-07-21 14:58:02.751228 macaquedb-0.1.4/PKG-INFO
-drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-21 14:58:02.749752 macaquedb-0.1.4/macaquedb.egg-info/
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      268 2023-07-21 14:58:02.000000 macaquedb-0.1.4/macaquedb.egg-info/PKG-INFO
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      288 2023-07-21 14:58:02.000000 macaquedb-0.1.4/macaquedb.egg-info/SOURCES.txt
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)        1 2023-07-21 14:58:02.000000 macaquedb-0.1.4/macaquedb.egg-info/dependency_links.txt
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       15 2023-07-21 14:58:02.000000 macaquedb-0.1.4/macaquedb.egg-info/requires.txt
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)        8 2023-07-21 14:58:02.000000 macaquedb-0.1.4/macaquedb.egg-info/top_level.txt
-drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-21 14:58:02.750913 macaquedb-0.1.4/package/
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)    12007 2023-07-21 14:36:48.000000 macaquedb-0.1.4/package/Database.py
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      489 2023-07-21 14:36:48.000000 macaquedb-0.1.4/package/Image.py
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      306 2023-07-21 14:36:48.000000 macaquedb-0.1.4/package/Session.py
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      321 2023-07-21 14:36:48.000000 macaquedb-0.1.4/package/Subject.py
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-21 14:36:48.000000 macaquedb-0.1.4/package/__init__.py
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      451 2023-07-21 14:36:48.000000 macaquedb-0.1.4/package/utilities.py
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       38 2023-07-21 14:58:02.751420 macaquedb-0.1.4/setup.cfg
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      373 2023-07-21 14:58:01.000000 macaquedb-0.1.4/setup.py
+drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-21 14:59:17.444915 macaquedb-0.1.5/
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      268 2023-07-21 14:59:17.444774 macaquedb-0.1.5/PKG-INFO
+drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-21 14:59:17.443326 macaquedb-0.1.5/macaquedb.egg-info/
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      268 2023-07-21 14:59:17.000000 macaquedb-0.1.5/macaquedb.egg-info/PKG-INFO
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      256 2023-07-21 14:59:17.000000 macaquedb-0.1.5/macaquedb.egg-info/SOURCES.txt
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)        1 2023-07-21 14:59:17.000000 macaquedb-0.1.5/macaquedb.egg-info/dependency_links.txt
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)        8 2023-07-21 14:59:17.000000 macaquedb-0.1.5/macaquedb.egg-info/top_level.txt
+drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-21 14:59:17.444497 macaquedb-0.1.5/package/
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)    12007 2023-07-21 14:36:48.000000 macaquedb-0.1.5/package/Database.py
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      489 2023-07-21 14:36:48.000000 macaquedb-0.1.5/package/Image.py
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      306 2023-07-21 14:36:48.000000 macaquedb-0.1.5/package/Session.py
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      321 2023-07-21 14:36:48.000000 macaquedb-0.1.5/package/Subject.py
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-21 14:36:48.000000 macaquedb-0.1.5/package/__init__.py
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      451 2023-07-21 14:36:48.000000 macaquedb-0.1.5/package/utilities.py
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       38 2023-07-21 14:59:17.444961 macaquedb-0.1.5/setup.cfg
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      343 2023-07-21 14:59:08.000000 macaquedb-0.1.5/setup.py
```

### Comparing `macaquedb-0.1.4/package/Database.py` & `macaquedb-0.1.5/package/Database.py`

 * *Files identical despite different names*

