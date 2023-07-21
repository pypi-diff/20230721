# Comparing `tmp/st_circular_progress-0.2.7.tar.gz` & `tmp/st_circular_progress-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_circular_progress-0.2.7.tar", last modified: Fri Jul 21 02:36:35 2023, max compression
+gzip compressed data, was "st_circular_progress-0.3.0.tar", last modified: Fri Jul 21 12:40:34 2023, max compression
```

## Comparing `st_circular_progress-0.2.7.tar` & `st_circular_progress-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 02:36:35.636664 st_circular_progress-0.2.7/
--rw-rw-r--   0 cserrano   (501) staff       (20)     1063 2023-07-12 21:17:31.000000 st_circular_progress-0.2.7/LICENSE
--rw-rw-r--   0 cserrano   (501) staff       (20)       43 2023-07-12 21:17:31.000000 st_circular_progress-0.2.7/MANIFEST.in
--rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 02:36:35.636328 st_circular_progress-0.2.7/PKG-INFO
--rw-r--r--   0 cserrano   (501) staff       (20)       38 2023-07-21 02:36:35.636778 st_circular_progress-0.2.7/setup.cfg
--rw-rw-r--   0 cserrano   (501) staff       (20)      631 2023-07-21 02:36:15.000000 st_circular_progress-0.2.7/setup.py
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 02:36:35.632539 st_circular_progress-0.2.7/st_circular_progress/
--rw-rw-r--   0 cserrano   (501) staff       (20)     2247 2023-07-21 02:26:27.000000 st_circular_progress-0.2.7/st_circular_progress/__init__.py
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 02:36:35.635579 st_circular_progress-0.2.7/st_circular_progress.egg-info/
--rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 02:36:35.000000 st_circular_progress-0.2.7/st_circular_progress.egg-info/PKG-INFO
--rw-r--r--   0 cserrano   (501) staff       (20)      280 2023-07-21 02:36:35.000000 st_circular_progress-0.2.7/st_circular_progress.egg-info/SOURCES.txt
--rw-r--r--   0 cserrano   (501) staff       (20)        1 2023-07-21 02:36:35.000000 st_circular_progress-0.2.7/st_circular_progress.egg-info/dependency_links.txt
--rw-r--r--   0 cserrano   (501) staff       (20)       16 2023-07-21 02:36:35.000000 st_circular_progress-0.2.7/st_circular_progress.egg-info/requires.txt
--rw-r--r--   0 cserrano   (501) staff       (20)       21 2023-07-21 02:36:35.000000 st_circular_progress-0.2.7/st_circular_progress.egg-info/top_level.txt
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 12:40:34.582759 st_circular_progress-0.3.0/
+-rw-rw-r--   0 cserrano   (501) staff       (20)     1063 2023-07-12 21:17:31.000000 st_circular_progress-0.3.0/LICENSE
+-rw-rw-r--   0 cserrano   (501) staff       (20)       43 2023-07-12 21:17:31.000000 st_circular_progress-0.3.0/MANIFEST.in
+-rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 12:40:34.582403 st_circular_progress-0.3.0/PKG-INFO
+-rw-r--r--   0 cserrano   (501) staff       (20)       38 2023-07-21 12:40:34.582879 st_circular_progress-0.3.0/setup.cfg
+-rw-rw-r--   0 cserrano   (501) staff       (20)      631 2023-07-21 12:40:30.000000 st_circular_progress-0.3.0/setup.py
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 12:40:34.578390 st_circular_progress-0.3.0/st_circular_progress/
+-rw-rw-r--   0 cserrano   (501) staff       (20)     2249 2023-07-21 12:38:40.000000 st_circular_progress-0.3.0/st_circular_progress/__init__.py
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 12:40:34.581693 st_circular_progress-0.3.0/st_circular_progress.egg-info/
+-rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 12:40:34.000000 st_circular_progress-0.3.0/st_circular_progress.egg-info/PKG-INFO
+-rw-r--r--   0 cserrano   (501) staff       (20)      280 2023-07-21 12:40:34.000000 st_circular_progress-0.3.0/st_circular_progress.egg-info/SOURCES.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)        1 2023-07-21 12:40:34.000000 st_circular_progress-0.3.0/st_circular_progress.egg-info/dependency_links.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)       16 2023-07-21 12:40:34.000000 st_circular_progress-0.3.0/st_circular_progress.egg-info/requires.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)       21 2023-07-21 12:40:34.000000 st_circular_progress-0.3.0/st_circular_progress.egg-info/top_level.txt
```

### Comparing `st_circular_progress-0.2.7/LICENSE` & `st_circular_progress-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `st_circular_progress-0.2.7/setup.py` & `st_circular_progress-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_circular_progress",
-    version="0.2.7",
+    version="0.3.0",
     author="Carlos D Serrano",
     author_email="sqlinsights@gmail.com",
     description="Circular progress wheel for Streamlit",
     long_description="Streamlit custom component based in VanillaJs that generates a Circular Shaped progress bar.",
     long_description_content_type="text/plain",
     url="https://github.com/sqlinsights/st-circular-progress",
     packages=setuptools.find_packages(),
```

### Comparing `st_circular_progress-0.2.7/st_circular_progress/__init__.py` & `st_circular_progress-0.3.0/st_circular_progress/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import streamlit.components.v1 as components
 import streamlit as st
 
-_RELEASE = True
+# _RELEASE = True
 
 
 # if not _RELEASE:
 #     _st_circular_progress_component = components.declare_component(
 #         "st_circular_progress",
 #         url="http://localhost:3001",
 #     )
```

