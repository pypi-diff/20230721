# Comparing `tmp/st_circular_progress-0.2.5.tar.gz` & `tmp/st_circular_progress-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_circular_progress-0.2.5.tar", last modified: Fri Jul 21 02:28:25 2023, max compression
+gzip compressed data, was "st_circular_progress-0.2.6.tar", last modified: Fri Jul 21 02:31:29 2023, max compression
```

## Comparing `st_circular_progress-0.2.5.tar` & `st_circular_progress-0.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 02:28:25.538326 st_circular_progress-0.2.5/
--rw-rw-r--   0 cserrano   (501) staff       (20)     1063 2023-07-12 21:17:31.000000 st_circular_progress-0.2.5/LICENSE
--rw-rw-r--   0 cserrano   (501) staff       (20)       43 2023-07-12 21:17:31.000000 st_circular_progress-0.2.5/MANIFEST.in
--rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 02:28:25.537978 st_circular_progress-0.2.5/PKG-INFO
--rw-r--r--   0 cserrano   (501) staff       (20)       38 2023-07-21 02:28:25.538439 st_circular_progress-0.2.5/setup.cfg
--rw-rw-r--   0 cserrano   (501) staff       (20)      631 2023-07-21 02:28:21.000000 st_circular_progress-0.2.5/setup.py
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 02:28:25.534245 st_circular_progress-0.2.5/st_circular_progress/
--rw-rw-r--   0 cserrano   (501) staff       (20)     2247 2023-07-21 02:26:27.000000 st_circular_progress-0.2.5/st_circular_progress/__init__.py
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 02:28:25.537323 st_circular_progress-0.2.5/st_circular_progress.egg-info/
--rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 02:28:25.000000 st_circular_progress-0.2.5/st_circular_progress.egg-info/PKG-INFO
--rw-r--r--   0 cserrano   (501) staff       (20)      280 2023-07-21 02:28:25.000000 st_circular_progress-0.2.5/st_circular_progress.egg-info/SOURCES.txt
--rw-r--r--   0 cserrano   (501) staff       (20)        1 2023-07-21 02:28:25.000000 st_circular_progress-0.2.5/st_circular_progress.egg-info/dependency_links.txt
--rw-r--r--   0 cserrano   (501) staff       (20)       16 2023-07-21 02:28:25.000000 st_circular_progress-0.2.5/st_circular_progress.egg-info/requires.txt
--rw-r--r--   0 cserrano   (501) staff       (20)       21 2023-07-21 02:28:25.000000 st_circular_progress-0.2.5/st_circular_progress.egg-info/top_level.txt
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 02:31:29.552412 st_circular_progress-0.2.6/
+-rw-rw-r--   0 cserrano   (501) staff       (20)     1063 2023-07-12 21:17:31.000000 st_circular_progress-0.2.6/LICENSE
+-rw-rw-r--   0 cserrano   (501) staff       (20)       43 2023-07-12 21:17:31.000000 st_circular_progress-0.2.6/MANIFEST.in
+-rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 02:31:29.551903 st_circular_progress-0.2.6/PKG-INFO
+-rw-r--r--   0 cserrano   (501) staff       (20)       38 2023-07-21 02:31:29.552571 st_circular_progress-0.2.6/setup.cfg
+-rw-rw-r--   0 cserrano   (501) staff       (20)      631 2023-07-21 02:31:19.000000 st_circular_progress-0.2.6/setup.py
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 02:31:29.548104 st_circular_progress-0.2.6/st_circular_progress/
+-rw-rw-r--   0 cserrano   (501) staff       (20)     2247 2023-07-21 02:26:27.000000 st_circular_progress-0.2.6/st_circular_progress/__init__.py
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 02:31:29.551255 st_circular_progress-0.2.6/st_circular_progress.egg-info/
+-rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 02:31:29.000000 st_circular_progress-0.2.6/st_circular_progress.egg-info/PKG-INFO
+-rw-r--r--   0 cserrano   (501) staff       (20)      280 2023-07-21 02:31:29.000000 st_circular_progress-0.2.6/st_circular_progress.egg-info/SOURCES.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)        1 2023-07-21 02:31:29.000000 st_circular_progress-0.2.6/st_circular_progress.egg-info/dependency_links.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)       16 2023-07-21 02:31:29.000000 st_circular_progress-0.2.6/st_circular_progress.egg-info/requires.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)       21 2023-07-21 02:31:29.000000 st_circular_progress-0.2.6/st_circular_progress.egg-info/top_level.txt
```

### Comparing `st_circular_progress-0.2.5/LICENSE` & `st_circular_progress-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `st_circular_progress-0.2.5/setup.py` & `st_circular_progress-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_circular_progress",
-    version="0.2.5",
+    version="0.2.6",
     author="Carlos D Serrano",
     author_email="sqlinsights@gmail.com",
     description="Circular progress wheel for Streamlit",
     long_description="Streamlit custom component based in VanillaJs that generates a Circular Shaped progress bar.",
     long_description_content_type="text/plain",
     url="https://github.com/sqlinsights/st-circular-progress",
     packages=setuptools.find_packages(),
```

### Comparing `st_circular_progress-0.2.5/st_circular_progress/__init__.py` & `st_circular_progress-0.2.6/st_circular_progress/__init__.py`

 * *Files identical despite different names*

