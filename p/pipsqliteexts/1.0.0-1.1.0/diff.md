# Comparing `tmp/pipsqliteexts-1.0.0.tar.gz` & `tmp/pipsqliteexts-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipsqliteexts-1.0.0.tar", last modified: Fri Jul 21 12:19:21 2023, max compression
+gzip compressed data, was "pipsqliteexts-1.1.0.tar", last modified: Fri Jul 21 12:21:26 2023, max compression
```

## Comparing `pipsqliteexts-1.0.0.tar` & `pipsqliteexts-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:19:21.221685 pipsqliteexts-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      346 2023-07-21 12:19:21.221685 pipsqliteexts-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:19:21.217685 pipsqliteexts-1.0.0/pipsqliteexts/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-21 12:19:20.000000 pipsqliteexts-1.0.0/pipsqliteexts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:19:21.221685 pipsqliteexts-1.0.0/pipsqliteexts.egg-info/
--rw-r--r--   0 root         (0) root         (0)      346 2023-07-21 12:19:21.000000 pipsqliteexts-1.0.0/pipsqliteexts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2023-07-21 12:19:21.000000 pipsqliteexts-1.0.0/pipsqliteexts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 12:19:21.000000 pipsqliteexts-1.0.0/pipsqliteexts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-21 12:19:21.000000 pipsqliteexts-1.0.0/pipsqliteexts.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 12:19:21.221685 pipsqliteexts-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      559 2023-07-21 12:19:20.000000 pipsqliteexts-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:21:26.729303 pipsqliteexts-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      346 2023-07-21 12:21:26.729303 pipsqliteexts-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:21:26.729303 pipsqliteexts-1.1.0/pipsqliteexts/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-21 12:21:26.000000 pipsqliteexts-1.1.0/pipsqliteexts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:21:26.729303 pipsqliteexts-1.1.0/pipsqliteexts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      346 2023-07-21 12:21:26.000000 pipsqliteexts-1.1.0/pipsqliteexts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2023-07-21 12:21:26.000000 pipsqliteexts-1.1.0/pipsqliteexts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 12:21:26.000000 pipsqliteexts-1.1.0/pipsqliteexts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-21 12:21:26.000000 pipsqliteexts-1.1.0/pipsqliteexts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 12:21:26.729303 pipsqliteexts-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      559 2023-07-21 12:21:26.000000 pipsqliteexts-1.1.0/setup.py
```

### Comparing `pipsqliteexts-1.0.0/setup.py` & `pipsqliteexts-1.1.0/setup.py`

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
     name="pipsqliteexts",
     version=VERSION,
```

