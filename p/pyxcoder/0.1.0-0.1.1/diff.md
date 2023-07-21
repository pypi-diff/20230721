# Comparing `tmp/pyxcoder-0.1.0.tar.gz` & `tmp/pyxcoder-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxcoder-0.1.0.tar", last modified: Fri Jul 21 04:28:42 2023, max compression
+gzip compressed data, was "pyxcoder-0.1.1.tar", last modified: Fri Jul 21 04:39:15 2023, max compression
```

## Comparing `pyxcoder-0.1.0.tar` & `pyxcoder-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jinchang  (2008) nmt       (1300)        0 2023-07-21 04:28:42.673668 pyxcoder-0.1.0/
--rw-r--r--   0 jinchang  (2008) nmt       (1300)       99 2023-07-21 04:28:42.673668 pyxcoder-0.1.0/PKG-INFO
-drwxr-xr-x   0 jinchang  (2008) nmt       (1300)        0 2023-07-21 04:28:42.653668 pyxcoder-0.1.0/pyxcoder/
--rw-r--r--   0 jinchang  (2008) nmt       (1300)       73 2023-07-21 04:27:53.000000 pyxcoder-0.1.0/pyxcoder/__init__.py
-drwxr-xr-x   0 jinchang  (2008) nmt       (1300)        0 2023-07-21 04:28:42.669668 pyxcoder-0.1.0/pyxcoder/xfile/
--rw-r--r--   0 jinchang  (2008) nmt       (1300)       56 2023-07-21 04:28:08.000000 pyxcoder-0.1.0/pyxcoder/xfile/__init__.py
--rw-r--r--   0 jinchang  (2008) nmt       (1300)      972 2023-07-20 14:51:38.000000 pyxcoder-0.1.0/pyxcoder/xfile/xreader.py
--rw-r--r--   0 jinchang  (2008) nmt       (1300)      787 2023-07-20 14:51:38.000000 pyxcoder-0.1.0/pyxcoder/xfile/xwriter.py
-drwxr-xr-x   0 jinchang  (2008) nmt       (1300)        0 2023-07-21 04:28:42.665668 pyxcoder-0.1.0/pyxcoder.egg-info/
--rw-r--r--   0 jinchang  (2008) nmt       (1300)       99 2023-07-21 04:28:42.000000 pyxcoder-0.1.0/pyxcoder.egg-info/PKG-INFO
--rw-r--r--   0 jinchang  (2008) nmt       (1300)      267 2023-07-21 04:28:42.000000 pyxcoder-0.1.0/pyxcoder.egg-info/SOURCES.txt
--rw-r--r--   0 jinchang  (2008) nmt       (1300)        1 2023-07-21 04:28:42.000000 pyxcoder-0.1.0/pyxcoder.egg-info/dependency_links.txt
--rw-r--r--   0 jinchang  (2008) nmt       (1300)       13 2023-07-21 04:28:42.000000 pyxcoder-0.1.0/pyxcoder.egg-info/requires.txt
--rw-r--r--   0 jinchang  (2008) nmt       (1300)        9 2023-07-21 04:28:42.000000 pyxcoder-0.1.0/pyxcoder.egg-info/top_level.txt
--rw-r--r--   0 jinchang  (2008) nmt       (1300)       38 2023-07-21 04:28:42.673668 pyxcoder-0.1.0/setup.cfg
--rw-r--r--   0 jinchang  (2008) nmt       (1300)      248 2023-07-21 04:21:14.000000 pyxcoder-0.1.0/setup.py
+drwxr-xr-x   0 jinchang  (2008) nmt       (1300)        0 2023-07-21 04:39:15.311639 pyxcoder-0.1.1/
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)       99 2023-07-21 04:39:15.307639 pyxcoder-0.1.1/PKG-INFO
+drwxr-xr-x   0 jinchang  (2008) nmt       (1300)        0 2023-07-21 04:39:15.291639 pyxcoder-0.1.1/pyxcoder/
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)       21 2023-07-21 04:37:44.000000 pyxcoder-0.1.1/pyxcoder/__init__.py
+drwxr-xr-x   0 jinchang  (2008) nmt       (1300)        0 2023-07-21 04:39:15.307639 pyxcoder-0.1.1/pyxcoder/xfile/
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)       46 2023-07-21 04:34:12.000000 pyxcoder-0.1.1/pyxcoder/xfile/__init__.py
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)      972 2023-07-20 14:51:38.000000 pyxcoder-0.1.1/pyxcoder/xfile/xreader.py
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)      787 2023-07-20 14:51:38.000000 pyxcoder-0.1.1/pyxcoder/xfile/xwriter.py
+drwxr-xr-x   0 jinchang  (2008) nmt       (1300)        0 2023-07-21 04:39:15.299639 pyxcoder-0.1.1/pyxcoder.egg-info/
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)       99 2023-07-21 04:39:15.000000 pyxcoder-0.1.1/pyxcoder.egg-info/PKG-INFO
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)      267 2023-07-21 04:39:15.000000 pyxcoder-0.1.1/pyxcoder.egg-info/SOURCES.txt
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)        1 2023-07-21 04:39:15.000000 pyxcoder-0.1.1/pyxcoder.egg-info/dependency_links.txt
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)       13 2023-07-21 04:39:15.000000 pyxcoder-0.1.1/pyxcoder.egg-info/requires.txt
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)        9 2023-07-21 04:39:15.000000 pyxcoder-0.1.1/pyxcoder.egg-info/top_level.txt
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)       38 2023-07-21 04:39:15.311639 pyxcoder-0.1.1/setup.cfg
+-rw-r--r--   0 jinchang  (2008) nmt       (1300)      248 2023-07-21 04:38:21.000000 pyxcoder-0.1.1/setup.py
```

### Comparing `pyxcoder-0.1.0/pyxcoder/xfile/xreader.py` & `pyxcoder-0.1.1/pyxcoder/xfile/xreader.py`

 * *Files identical despite different names*

### Comparing `pyxcoder-0.1.0/pyxcoder/xfile/xwriter.py` & `pyxcoder-0.1.1/pyxcoder/xfile/xwriter.py`

 * *Files identical despite different names*

