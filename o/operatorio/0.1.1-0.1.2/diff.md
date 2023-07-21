# Comparing `tmp/operatorio-0.1.1.tar.gz` & `tmp/operatorio-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "operatorio-0.1.1.tar", last modified: Fri Jul 21 05:04:20 2023, max compression
+gzip compressed data, was "operatorio-0.1.2.tar", last modified: Fri Jul 21 06:10:02 2023, max compression
```

## Comparing `operatorio-0.1.1.tar` & `operatorio-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 05:04:20.360718 operatorio-0.1.1/
--rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 05:04:20.360448 operatorio-0.1.1/PKG-INFO
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 05:04:20.360156 operatorio-0.1.1/operatorio.egg-info/
--rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 05:04:20.000000 operatorio-0.1.1/operatorio.egg-info/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)      177 2023-07-21 05:04:20.000000 operatorio-0.1.1/operatorio.egg-info/SOURCES.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2023-07-21 05:04:20.000000 operatorio-0.1.1/operatorio.egg-info/dependency_links.txt
--rw-r--r--   0 david      (501) staff       (20)        9 2023-07-21 05:04:20.000000 operatorio-0.1.1/operatorio.egg-info/requires.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2023-07-21 05:04:20.000000 operatorio-0.1.1/operatorio.egg-info/top_level.txt
--rw-r--r--   0 david      (501) staff       (20)       38 2023-07-21 05:04:20.360814 operatorio-0.1.1/setup.cfg
--rw-r--r--   0 david      (501) staff       (20)      530 2023-07-21 05:04:19.000000 operatorio-0.1.1/setup.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 06:10:02.510745 operatorio-0.1.2/
+-rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 06:10:02.510438 operatorio-0.1.2/PKG-INFO
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 06:10:02.509367 operatorio-0.1.2/operatorio.egg-info/
+-rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 06:10:02.000000 operatorio-0.1.2/operatorio.egg-info/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)      205 2023-07-21 06:10:02.000000 operatorio-0.1.2/operatorio.egg-info/SOURCES.txt
+-rw-r--r--   0 david      (501) staff       (20)        1 2023-07-21 06:10:02.000000 operatorio-0.1.2/operatorio.egg-info/dependency_links.txt
+-rw-r--r--   0 david      (501) staff       (20)        9 2023-07-21 06:10:02.000000 operatorio-0.1.2/operatorio.egg-info/requires.txt
+-rw-r--r--   0 david      (501) staff       (20)        4 2023-07-21 06:10:02.000000 operatorio-0.1.2/operatorio.egg-info/top_level.txt
+-rw-r--r--   0 david      (501) staff       (20)       38 2023-07-21 06:10:02.510813 operatorio-0.1.2/setup.cfg
+-rw-r--r--   0 david      (501) staff       (20)      530 2023-07-21 06:09:41.000000 operatorio-0.1.2/setup.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 06:10:02.510003 operatorio-0.1.2/src/
+-rw-r--r--   0 david      (501) staff       (20)      113 2023-07-21 06:08:03.000000 operatorio-0.1.2/src/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     1322 2023-07-21 04:30:59.000000 operatorio-0.1.2/src/main.py
```

### Comparing `operatorio-0.1.1/setup.py` & `operatorio-0.1.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="operatorio",
-    version="0.1.1",
+    version="0.1.2",
     description="A Python SDK for the Operator Search API.",
     author="David Shi",
     author_email="david@operator.io",
     url="https://github.com/operatorlabs/sdk/python",
     packages=find_packages(),
     install_requires=[
         'requests',
```

