# Comparing `tmp/st_circular_progress-0.2.0.tar.gz` & `tmp/st_circular_progress-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_circular_progress-0.2.0.tar", last modified: Fri Jul 21 02:06:46 2023, max compression
+gzip compressed data, was "st_circular_progress-0.2.1.tar", last modified: Fri Jul 21 02:08:57 2023, max compression
```

## Comparing `st_circular_progress-0.2.0.tar` & `st_circular_progress-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 02:06:46.008530 st_circular_progress-0.2.0/
--rw-rw-r--   0 cserrano   (501) staff       (20)     1063 2023-07-12 21:17:31.000000 st_circular_progress-0.2.0/LICENSE
--rw-rw-r--   0 cserrano   (501) staff       (20)       43 2023-07-12 21:17:31.000000 st_circular_progress-0.2.0/MANIFEST.in
--rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 02:06:46.008138 st_circular_progress-0.2.0/PKG-INFO
--rw-r--r--   0 cserrano   (501) staff       (20)       38 2023-07-21 02:06:46.008659 st_circular_progress-0.2.0/setup.cfg
--rw-rw-r--   0 cserrano   (501) staff       (20)      631 2023-07-21 02:06:01.000000 st_circular_progress-0.2.0/setup.py
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 02:06:46.004233 st_circular_progress-0.2.0/st_circular_progress/
--rw-rw-r--   0 cserrano   (501) staff       (20)     2004 2023-07-21 02:05:44.000000 st_circular_progress-0.2.0/st_circular_progress/__init__.py
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 02:06:46.007407 st_circular_progress-0.2.0/st_circular_progress.egg-info/
--rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 02:06:45.000000 st_circular_progress-0.2.0/st_circular_progress.egg-info/PKG-INFO
--rw-r--r--   0 cserrano   (501) staff       (20)      280 2023-07-21 02:06:45.000000 st_circular_progress-0.2.0/st_circular_progress.egg-info/SOURCES.txt
--rw-r--r--   0 cserrano   (501) staff       (20)        1 2023-07-21 02:06:45.000000 st_circular_progress-0.2.0/st_circular_progress.egg-info/dependency_links.txt
--rw-r--r--   0 cserrano   (501) staff       (20)       16 2023-07-21 02:06:45.000000 st_circular_progress-0.2.0/st_circular_progress.egg-info/requires.txt
--rw-r--r--   0 cserrano   (501) staff       (20)       21 2023-07-21 02:06:45.000000 st_circular_progress-0.2.0/st_circular_progress.egg-info/top_level.txt
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 02:08:57.897716 st_circular_progress-0.2.1/
+-rw-rw-r--   0 cserrano   (501) staff       (20)     1063 2023-07-12 21:17:31.000000 st_circular_progress-0.2.1/LICENSE
+-rw-rw-r--   0 cserrano   (501) staff       (20)       43 2023-07-12 21:17:31.000000 st_circular_progress-0.2.1/MANIFEST.in
+-rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 02:08:57.897381 st_circular_progress-0.2.1/PKG-INFO
+-rw-r--r--   0 cserrano   (501) staff       (20)       38 2023-07-21 02:08:57.897827 st_circular_progress-0.2.1/setup.cfg
+-rw-rw-r--   0 cserrano   (501) staff       (20)      631 2023-07-21 02:08:50.000000 st_circular_progress-0.2.1/setup.py
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 02:08:57.893616 st_circular_progress-0.2.1/st_circular_progress/
+-rw-rw-r--   0 cserrano   (501) staff       (20)     2004 2023-07-21 02:07:50.000000 st_circular_progress-0.2.1/st_circular_progress/__init__.py
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 02:08:57.896793 st_circular_progress-0.2.1/st_circular_progress.egg-info/
+-rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 02:08:57.000000 st_circular_progress-0.2.1/st_circular_progress.egg-info/PKG-INFO
+-rw-r--r--   0 cserrano   (501) staff       (20)      280 2023-07-21 02:08:57.000000 st_circular_progress-0.2.1/st_circular_progress.egg-info/SOURCES.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)        1 2023-07-21 02:08:57.000000 st_circular_progress-0.2.1/st_circular_progress.egg-info/dependency_links.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)       16 2023-07-21 02:08:57.000000 st_circular_progress-0.2.1/st_circular_progress.egg-info/requires.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)       21 2023-07-21 02:08:57.000000 st_circular_progress-0.2.1/st_circular_progress.egg-info/top_level.txt
```

### Comparing `st_circular_progress-0.2.0/LICENSE` & `st_circular_progress-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `st_circular_progress-0.2.0/setup.py` & `st_circular_progress-0.2.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_circular_progress",
-    version="0.2.0",
+    version="0.2.1",
     author="Carlos D Serrano",
     author_email="sqlinsights@gmail.com",
     description="Circular progress wheel for Streamlit",
     long_description="Streamlit custom component based in VanillaJs that generates a Circular Shaped progress bar.",
     long_description_content_type="text/plain",
     url="https://github.com/sqlinsights/st-circular-progress",
     packages=setuptools.find_packages(),
```

### Comparing `st_circular_progress-0.2.0/st_circular_progress/__init__.py` & `st_circular_progress-0.2.1/st_circular_progress/__init__.py`

 * *Files identical despite different names*

