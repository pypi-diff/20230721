# Comparing `tmp/pythoncolourmoduleV2-1.0.0.tar.gz` & `tmp/pythoncolourmoduleV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoncolourmoduleV2-1.0.0.tar", last modified: Fri Jul 21 14:41:55 2023, max compression
+gzip compressed data, was "pythoncolourmoduleV2-1.1.0.tar", last modified: Fri Jul 21 14:44:00 2023, max compression
```

## Comparing `pythoncolourmoduleV2-1.0.0.tar` & `pythoncolourmoduleV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 14:41:55.801083 pythoncolourmoduleV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      353 2023-07-21 14:41:55.801083 pythoncolourmoduleV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 14:41:55.797083 pythoncolourmoduleV2-1.0.0/pythoncolourmoduleV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-21 14:41:55.000000 pythoncolourmoduleV2-1.0.0/pythoncolourmoduleV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 14:41:55.801083 pythoncolourmoduleV2-1.0.0/pythoncolourmoduleV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      353 2023-07-21 14:41:55.000000 pythoncolourmoduleV2-1.0.0/pythoncolourmoduleV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      217 2023-07-21 14:41:55.000000 pythoncolourmoduleV2-1.0.0/pythoncolourmoduleV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 14:41:55.000000 pythoncolourmoduleV2-1.0.0/pythoncolourmoduleV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-21 14:41:55.000000 pythoncolourmoduleV2-1.0.0/pythoncolourmoduleV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 14:41:55.801083 pythoncolourmoduleV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      566 2023-07-21 14:41:55.000000 pythoncolourmoduleV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 14:44:00.864755 pythoncolourmoduleV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-07-21 14:44:00.864755 pythoncolourmoduleV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 14:44:00.864755 pythoncolourmoduleV2-1.1.0/pythoncolourmoduleV2/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-21 14:44:00.000000 pythoncolourmoduleV2-1.1.0/pythoncolourmoduleV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 14:44:00.864755 pythoncolourmoduleV2-1.1.0/pythoncolourmoduleV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-07-21 14:44:00.000000 pythoncolourmoduleV2-1.1.0/pythoncolourmoduleV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      217 2023-07-21 14:44:00.000000 pythoncolourmoduleV2-1.1.0/pythoncolourmoduleV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 14:44:00.000000 pythoncolourmoduleV2-1.1.0/pythoncolourmoduleV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-21 14:44:00.000000 pythoncolourmoduleV2-1.1.0/pythoncolourmoduleV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 14:44:00.864755 pythoncolourmoduleV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      566 2023-07-21 14:44:00.000000 pythoncolourmoduleV2-1.1.0/setup.py
```

### Comparing `pythoncolourmoduleV2-1.0.0/setup.py` & `pythoncolourmoduleV2-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pythoncolourmoduleV2",
     version=VERSION,
```

