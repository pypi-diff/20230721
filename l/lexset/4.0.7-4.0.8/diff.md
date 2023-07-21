# Comparing `tmp/lexset-4.0.7.tar.gz` & `tmp/lexset-4.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexset-4.0.7.tar", last modified: Tue Jul 18 19:32:56 2023, max compression
+gzip compressed data, was "lexset-4.0.8.tar", last modified: Fri Jul 21 19:28:10 2023, max compression
```

## Comparing `lexset-4.0.7.tar` & `lexset-4.0.8.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:56.552623 lexset-4.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-18 19:32:56.552623 lexset-4.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-18 19:32:34.000000 lexset-4.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:56.548623 lexset-4.0.7/lexset/
--rw-r--r--   0 runner    (1001) docker     (123)    30595 2023-07-18 19:32:34.000000 lexset-4.0.7/lexset/LexsetManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-18 19:32:34.000000 lexset-4.0.7/lexset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-18 19:32:34.000000 lexset-4.0.7/lexset/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:56.552623 lexset-4.0.7/lexset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-18 19:32:56.000000 lexset-4.0.7/lexset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-18 19:32:56.000000 lexset-4.0.7/lexset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:56.000000 lexset-4.0.7/lexset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-18 19:32:56.000000 lexset-4.0.7/lexset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 19:32:56.000000 lexset-4.0.7/lexset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:32:56.552623 lexset-4.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-18 19:32:34.000000 lexset-4.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:28:10.700563 lexset-4.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-21 19:28:10.700563 lexset-4.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-21 19:27:55.000000 lexset-4.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:28:10.700563 lexset-4.0.8/lexset/
+-rw-r--r--   0 runner    (1001) docker     (123)    30595 2023-07-21 19:27:55.000000 lexset-4.0.8/lexset/LexsetManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-21 19:27:55.000000 lexset-4.0.8/lexset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-21 19:27:55.000000 lexset-4.0.8/lexset/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-07-21 19:27:55.000000 lexset-4.0.8/lexset/review.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:28:10.700563 lexset-4.0.8/lexset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-21 19:28:10.000000 lexset-4.0.8/lexset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-21 19:28:10.000000 lexset-4.0.8/lexset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 19:28:10.000000 lexset-4.0.8/lexset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-21 19:28:10.000000 lexset-4.0.8/lexset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-21 19:28:10.000000 lexset-4.0.8/lexset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 19:28:10.700563 lexset-4.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-21 19:27:55.000000 lexset-4.0.8/setup.py
```

### Comparing `lexset-4.0.7/lexset/LexsetManager.py` & `lexset-4.0.8/lexset/LexsetManager.py`

 * *Files identical despite different names*

### Comparing `lexset-4.0.7/lexset/credentials.py` & `lexset-4.0.8/lexset/credentials.py`

 * *Files identical despite different names*

