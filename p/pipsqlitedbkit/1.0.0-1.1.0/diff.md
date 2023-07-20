# Comparing `tmp/pipsqlitedbkit-1.0.0.tar.gz` & `tmp/pipsqlitedbkit-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipsqlitedbkit-1.0.0.tar", last modified: Thu Jul 20 21:57:12 2023, max compression
+gzip compressed data, was "pipsqlitedbkit-1.1.0.tar", last modified: Thu Jul 20 21:59:18 2023, max compression
```

## Comparing `pipsqlitedbkit-1.0.0.tar` & `pipsqlitedbkit-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:57:12.835749 pipsqlitedbkit-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      347 2023-07-20 21:57:12.831749 pipsqlitedbkit-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:57:12.831749 pipsqlitedbkit-1.0.0/pipsqlitedbkit/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-20 21:57:12.000000 pipsqlitedbkit-1.0.0/pipsqlitedbkit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:57:12.831749 pipsqlitedbkit-1.0.0/pipsqlitedbkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      347 2023-07-20 21:57:12.000000 pipsqlitedbkit-1.0.0/pipsqlitedbkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      187 2023-07-20 21:57:12.000000 pipsqlitedbkit-1.0.0/pipsqlitedbkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 21:57:12.000000 pipsqlitedbkit-1.0.0/pipsqlitedbkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-20 21:57:12.000000 pipsqlitedbkit-1.0.0/pipsqlitedbkit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 21:57:12.835749 pipsqlitedbkit-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      560 2023-07-20 21:57:12.000000 pipsqlitedbkit-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:59:18.391356 pipsqlitedbkit-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-07-20 21:59:18.391356 pipsqlitedbkit-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:59:18.391356 pipsqlitedbkit-1.1.0/pipsqlitedbkit/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-20 21:59:17.000000 pipsqlitedbkit-1.1.0/pipsqlitedbkit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:59:18.391356 pipsqlitedbkit-1.1.0/pipsqlitedbkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-07-20 21:59:18.000000 pipsqlitedbkit-1.1.0/pipsqlitedbkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      187 2023-07-20 21:59:18.000000 pipsqlitedbkit-1.1.0/pipsqlitedbkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 21:59:18.000000 pipsqlitedbkit-1.1.0/pipsqlitedbkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-20 21:59:18.000000 pipsqlitedbkit-1.1.0/pipsqlitedbkit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 21:59:18.391356 pipsqlitedbkit-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      560 2023-07-20 21:59:17.000000 pipsqlitedbkit-1.1.0/setup.py
```

### Comparing `pipsqlitedbkit-1.0.0/setup.py` & `pipsqlitedbkit-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pipsqlitedbkit",
     version=VERSION,
```

