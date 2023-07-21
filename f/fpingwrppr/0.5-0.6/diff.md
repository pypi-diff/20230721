# Comparing `tmp/fpingwrppr-0.5.tar.gz` & `tmp/fpingwrppr-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpingwrppr-0.5.tar", last modified: Thu Jul 20 19:57:36 2023, max compression
+gzip compressed data, was "fpingwrppr-0.6.tar", last modified: Fri Jul 21 12:03:52 2023, max compression
```

## Comparing `fpingwrppr-0.5.tar` & `fpingwrppr-0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 19:57:36.505748 fpingwrppr-0.5/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      119 2023-07-20 19:57:36.505748 fpingwrppr-0.5/PKG-INFO
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 19:57:36.495748 fpingwrppr-0.5/fping/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      751 2023-07-20 19:53:40.000000 fpingwrppr-0.5/fping/__init__.py
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 19:57:36.495748 fpingwrppr-0.5/fping/backends/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)        2 2023-07-20 17:31:11.000000 fpingwrppr-0.5/fping/backends/__init__.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1374 2023-07-20 19:54:24.000000 fpingwrppr-0.5/fping/backends/base.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1403 2023-07-20 19:55:48.000000 fpingwrppr-0.5/fping/backends/fping.py
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 19:57:36.505748 fpingwrppr-0.5/fpingwrppr.egg-info/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      119 2023-07-20 19:57:36.000000 fpingwrppr-0.5/fpingwrppr.egg-info/PKG-INFO
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      317 2023-07-20 19:57:36.000000 fpingwrppr-0.5/fpingwrppr.egg-info/SOURCES.txt
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)        1 2023-07-20 19:57:36.000000 fpingwrppr-0.5/fpingwrppr.egg-info/dependency_links.txt
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)        6 2023-07-20 19:57:36.000000 fpingwrppr-0.5/fpingwrppr.egg-info/top_level.txt
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)        1 2023-07-20 19:57:36.000000 fpingwrppr-0.5/fpingwrppr.egg-info/zip-safe
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)       62 2023-07-20 19:57:36.505748 fpingwrppr-0.5/setup.cfg
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      630 2023-07-20 19:56:54.000000 fpingwrppr-0.5/setup.py
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-20 19:57:36.505748 fpingwrppr-0.5/tests/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      779 2023-07-20 17:34:56.000000 fpingwrppr-0.5/tests/test_backends.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      293 2023-07-20 17:34:56.000000 fpingwrppr-0.5/tests/test_base.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-21 12:03:52.343126 fpingwrppr-0.6/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      119 2023-07-21 12:03:52.343126 fpingwrppr-0.6/PKG-INFO
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-21 12:03:52.333127 fpingwrppr-0.6/fping/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      751 2023-07-20 20:00:59.000000 fpingwrppr-0.6/fping/__init__.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-21 12:03:52.343126 fpingwrppr-0.6/fping/backends/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        2 2023-07-20 17:31:11.000000 fpingwrppr-0.6/fping/backends/__init__.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1374 2023-07-20 19:54:24.000000 fpingwrppr-0.6/fping/backends/base.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1413 2023-07-20 20:01:55.000000 fpingwrppr-0.6/fping/backends/fping.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-21 12:03:52.343126 fpingwrppr-0.6/fpingwrppr.egg-info/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      119 2023-07-21 12:03:52.000000 fpingwrppr-0.6/fpingwrppr.egg-info/PKG-INFO
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      317 2023-07-21 12:03:52.000000 fpingwrppr-0.6/fpingwrppr.egg-info/SOURCES.txt
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        1 2023-07-21 12:03:52.000000 fpingwrppr-0.6/fpingwrppr.egg-info/dependency_links.txt
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        6 2023-07-21 12:03:52.000000 fpingwrppr-0.6/fpingwrppr.egg-info/top_level.txt
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        1 2023-07-21 12:03:52.000000 fpingwrppr-0.6/fpingwrppr.egg-info/zip-safe
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)       62 2023-07-21 12:03:52.343126 fpingwrppr-0.6/setup.cfg
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      630 2023-07-21 12:02:45.000000 fpingwrppr-0.6/setup.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-21 12:03:52.343126 fpingwrppr-0.6/tests/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      779 2023-07-20 17:34:56.000000 fpingwrppr-0.6/tests/test_backends.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      293 2023-07-20 17:34:56.000000 fpingwrppr-0.6/tests/test_base.py
```

### Comparing `fpingwrppr-0.5/fping/__init__.py` & `fpingwrppr-0.6/fping/__init__.py`

 * *Files identical despite different names*

### Comparing `fpingwrppr-0.5/fping/backends/base.py` & `fpingwrppr-0.6/fping/backends/base.py`

 * *Files identical despite different names*

### Comparing `fpingwrppr-0.5/fping/backends/fping.py` & `fpingwrppr-0.6/fping/backends/fping.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import subprocess, os
+import subprocess, os, tempfile
 from fping.backends.base import BasePinger
 
 def os_wait():
     try:
         os.wait()
     except OSError:
         pass
```

### Comparing `fpingwrppr-0.5/setup.py` & `fpingwrppr-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import sys, os
 
-version = '0.5'
+version = '0.6'
 
 setup(name='fpingwrppr',
       version=version,
       description="Fping Wrapper",
       long_description="""\
 """,
       classifiers=[], # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
```

### Comparing `fpingwrppr-0.5/tests/test_backends.py` & `fpingwrppr-0.6/tests/test_backends.py`

 * *Files identical despite different names*

