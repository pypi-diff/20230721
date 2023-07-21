# Comparing `tmp/mec-0.0.1.3.tar.gz` & `tmp/mec-0.0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mec-0.0.1.3.tar", last modified: Thu Jul 20 21:47:28 2023, max compression
+gzip compressed data, was "mec-0.0.1.4.tar", last modified: Fri Jul 21 03:12:09 2023, max compression
```

## Comparing `mec-0.0.1.3.tar` & `mec-0.0.1.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:28.439468 mec-0.0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-20 21:47:28.439468 mec-0.0.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:28.439468 mec-0.0.1.3/mec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:20.000000 mec-0.0.1.3/mec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:28.439468 mec-0.0.1.3/mec/et/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:20.000000 mec-0.0.1.3/mec/et/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22636 2023-07-20 21:47:20.000000 mec-0.0.1.3/mec/et/ntu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8309 2023-07-20 21:47:20.000000 mec-0.0.1.3/mec/lp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-07-20 21:47:20.000000 mec-0.0.1.3/mec/ot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:28.439468 mec-0.0.1.3/mec/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:20.000000 mec-0.0.1.3/mec/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:28.439468 mec-0.0.1.3/mec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-20 21:47:28.000000 mec-0.0.1.3/mec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-20 21:47:28.000000 mec-0.0.1.3/mec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:47:28.000000 mec-0.0.1.3/mec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-20 21:47:28.000000 mec-0.0.1.3/mec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 21:47:28.439468 mec-0.0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-20 21:47:20.000000 mec-0.0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:12:09.618800 mec-0.0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-21 03:12:09.614800 mec-0.0.1.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:12:09.614800 mec-0.0.1.4/mec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:12:02.000000 mec-0.0.1.4/mec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:12:09.614800 mec-0.0.1.4/mec/et/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:12:02.000000 mec-0.0.1.4/mec/et/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22636 2023-07-21 03:12:02.000000 mec-0.0.1.4/mec/et/ntu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8309 2023-07-21 03:12:02.000000 mec-0.0.1.4/mec/lp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-07-21 03:12:02.000000 mec-0.0.1.4/mec/ot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:12:09.614800 mec-0.0.1.4/mec/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:12:02.000000 mec-0.0.1.4/mec/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:12:09.614800 mec-0.0.1.4/mec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-21 03:12:09.000000 mec-0.0.1.4/mec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-21 03:12:09.000000 mec-0.0.1.4/mec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 03:12:09.000000 mec-0.0.1.4/mec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 03:12:09.000000 mec-0.0.1.4/mec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-21 03:12:09.000000 mec-0.0.1.4/mec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 03:12:09.618800 mec-0.0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-21 03:12:02.000000 mec-0.0.1.4/setup.py
```

### Comparing `mec-0.0.1.3/mec/et/ntu.py` & `mec-0.0.1.4/mec/et/ntu.py`

 * *Files identical despite different names*

### Comparing `mec-0.0.1.3/mec/lp.py` & `mec-0.0.1.4/mec/lp.py`

 * *Files identical despite different names*

### Comparing `mec-0.0.1.3/mec/ot.py` & `mec-0.0.1.4/mec/ot.py`

 * *Files identical despite different names*

