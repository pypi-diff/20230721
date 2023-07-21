# Comparing `tmp/st_circular_progress-0.1.4.tar.gz` & `tmp/st_circular_progress-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_circular_progress-0.1.4.tar", last modified: Fri Jul 21 01:49:06 2023, max compression
+gzip compressed data, was "st_circular_progress-0.1.5.tar", last modified: Fri Jul 21 01:52:53 2023, max compression
```

## Comparing `st_circular_progress-0.1.4.tar` & `st_circular_progress-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 01:49:06.873483 st_circular_progress-0.1.4/
--rw-rw-r--   0 cserrano   (501) staff       (20)     1063 2023-07-12 21:17:31.000000 st_circular_progress-0.1.4/LICENSE
--rw-rw-r--   0 cserrano   (501) staff       (20)       43 2023-07-12 21:17:31.000000 st_circular_progress-0.1.4/MANIFEST.in
--rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 01:49:06.873128 st_circular_progress-0.1.4/PKG-INFO
--rw-r--r--   0 cserrano   (501) staff       (20)       38 2023-07-21 01:49:06.873618 st_circular_progress-0.1.4/setup.cfg
--rw-rw-r--   0 cserrano   (501) staff       (20)      631 2023-07-21 01:49:03.000000 st_circular_progress-0.1.4/setup.py
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 01:49:06.868493 st_circular_progress-0.1.4/st_circular_progress/
--rw-rw-r--   0 cserrano   (501) staff       (20)     2004 2023-07-21 01:46:50.000000 st_circular_progress-0.1.4/st_circular_progress/__init__.py
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 01:49:06.872527 st_circular_progress-0.1.4/st_circular_progress.egg-info/
--rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 01:49:06.000000 st_circular_progress-0.1.4/st_circular_progress.egg-info/PKG-INFO
--rw-r--r--   0 cserrano   (501) staff       (20)      280 2023-07-21 01:49:06.000000 st_circular_progress-0.1.4/st_circular_progress.egg-info/SOURCES.txt
--rw-r--r--   0 cserrano   (501) staff       (20)        1 2023-07-21 01:49:06.000000 st_circular_progress-0.1.4/st_circular_progress.egg-info/dependency_links.txt
--rw-r--r--   0 cserrano   (501) staff       (20)       16 2023-07-21 01:49:06.000000 st_circular_progress-0.1.4/st_circular_progress.egg-info/requires.txt
--rw-r--r--   0 cserrano   (501) staff       (20)       21 2023-07-21 01:49:06.000000 st_circular_progress-0.1.4/st_circular_progress.egg-info/top_level.txt
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 01:52:53.698525 st_circular_progress-0.1.5/
+-rw-rw-r--   0 cserrano   (501) staff       (20)     1063 2023-07-12 21:17:31.000000 st_circular_progress-0.1.5/LICENSE
+-rw-rw-r--   0 cserrano   (501) staff       (20)       43 2023-07-12 21:17:31.000000 st_circular_progress-0.1.5/MANIFEST.in
+-rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 01:52:53.698220 st_circular_progress-0.1.5/PKG-INFO
+-rw-r--r--   0 cserrano   (501) staff       (20)       38 2023-07-21 01:52:53.698630 st_circular_progress-0.1.5/setup.cfg
+-rw-rw-r--   0 cserrano   (501) staff       (20)      631 2023-07-21 01:52:48.000000 st_circular_progress-0.1.5/setup.py
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 01:52:53.694944 st_circular_progress-0.1.5/st_circular_progress/
+-rw-rw-r--   0 cserrano   (501) staff       (20)     2004 2023-07-21 01:46:50.000000 st_circular_progress-0.1.5/st_circular_progress/__init__.py
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 01:52:53.697555 st_circular_progress-0.1.5/st_circular_progress.egg-info/
+-rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 01:52:53.000000 st_circular_progress-0.1.5/st_circular_progress.egg-info/PKG-INFO
+-rw-r--r--   0 cserrano   (501) staff       (20)      280 2023-07-21 01:52:53.000000 st_circular_progress-0.1.5/st_circular_progress.egg-info/SOURCES.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)        1 2023-07-21 01:52:53.000000 st_circular_progress-0.1.5/st_circular_progress.egg-info/dependency_links.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)       16 2023-07-21 01:52:53.000000 st_circular_progress-0.1.5/st_circular_progress.egg-info/requires.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)       21 2023-07-21 01:52:53.000000 st_circular_progress-0.1.5/st_circular_progress.egg-info/top_level.txt
```

### Comparing `st_circular_progress-0.1.4/LICENSE` & `st_circular_progress-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `st_circular_progress-0.1.4/setup.py` & `st_circular_progress-0.1.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_circular_progress",
-    version="0.1.4",
+    version="0.1.5",
     author="Carlos D Serrano",
     author_email="sqlinsights@gmail.com",
     description="Circular progress wheel for Streamlit",
     long_description="Streamlit custom component based in VanillaJs that generates a Circular Shaped progress bar.",
     long_description_content_type="text/plain",
     url="https://github.com/sqlinsights/st-circular-progress",
     packages=setuptools.find_packages(),
```

### Comparing `st_circular_progress-0.1.4/st_circular_progress/__init__.py` & `st_circular_progress-0.1.5/st_circular_progress/__init__.py`

 * *Files identical despite different names*

