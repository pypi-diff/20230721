# Comparing `tmp/anysolve-1.0.1.tar.gz` & `tmp/anysolve-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anysolve-1.0.1.tar", last modified: Wed May  3 12:24:54 2023, max compression
+gzip compressed data, was "anysolve-1.0.2.tar", last modified: Fri Jul 21 19:28:16 2023, max compression
```

## Comparing `anysolve-1.0.1.tar` & `anysolve-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:24:54.305576 anysolve-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-03 12:24:52.000000 anysolve-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-03 12:24:54.305576 anysolve-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-03 12:24:52.000000 anysolve-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:24:54.305576 anysolve-1.0.1/anysolve/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-03 12:24:52.000000 anysolve-1.0.1/anysolve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:24:54.305576 anysolve-1.0.1/anysolve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-03 12:24:54.000000 anysolve-1.0.1/anysolve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-03 12:24:54.000000 anysolve-1.0.1/anysolve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:24:54.000000 anysolve-1.0.1/anysolve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:24:54.000000 anysolve-1.0.1/anysolve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 12:24:54.000000 anysolve-1.0.1/anysolve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 12:24:54.000000 anysolve-1.0.1/anysolve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-03 12:24:54.305576 anysolve-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-03 12:24:52.000000 anysolve-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:28:16.729768 anysolve-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-21 19:28:15.000000 anysolve-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-07-21 19:28:16.729768 anysolve-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-07-21 19:28:15.000000 anysolve-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:28:16.729768 anysolve-1.0.2/anysolve/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-21 19:28:15.000000 anysolve-1.0.2/anysolve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:28:16.729768 anysolve-1.0.2/anysolve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-07-21 19:28:16.000000 anysolve-1.0.2/anysolve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-21 19:28:16.000000 anysolve-1.0.2/anysolve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 19:28:16.000000 anysolve-1.0.2/anysolve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 19:28:16.000000 anysolve-1.0.2/anysolve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 19:28:16.000000 anysolve-1.0.2/anysolve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 19:28:16.000000 anysolve-1.0.2/anysolve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-21 19:28:16.729768 anysolve-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-21 19:28:15.000000 anysolve-1.0.2/setup.py
```

### Comparing `anysolve-1.0.1/LICENSE` & `anysolve-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anysolve-1.0.1/anysolve/__init__.py` & `anysolve-1.0.2/anysolve/__init__.py`

 * *Files identical despite different names*

### Comparing `anysolve-1.0.1/setup.py` & `anysolve-1.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 
 # Package metadata.
 
 name = "anysolve"
 description = "AnySolve.ai Client library"
-version = "1.0.1"
+version = "1.0.2"
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
     "requests",
 ]
 extras = {}
 
 
@@ -30,15 +30,15 @@
     name=name,
     version=version,
     description=description,
     long_description=readme,
     author="Simon Hecht",
     author_email="simon_hecht@hotmail.com",
     license="License :: OSI Approved :: The Unlicense (Unlicense)",
-    url="https://github.com/aaad/anysolve",
+    url="https://github.com/BlackriverBlockchain/anysolve",
     classifiers=[
         release_status,
         "Intended Audience :: Developers",
         "License :: OSI Approved :: The Unlicense (Unlicense)",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
```

