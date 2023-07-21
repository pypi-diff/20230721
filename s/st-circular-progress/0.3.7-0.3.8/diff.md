# Comparing `tmp/st_circular_progress-0.3.7.tar.gz` & `tmp/st_circular_progress-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_circular_progress-0.3.7.tar", last modified: Fri Jul 21 16:14:47 2023, max compression
+gzip compressed data, was "st_circular_progress-0.3.8.tar", last modified: Fri Jul 21 16:15:46 2023, max compression
```

## Comparing `st_circular_progress-0.3.7.tar` & `st_circular_progress-0.3.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 16:14:47.103493 st_circular_progress-0.3.7/
--rw-rw-r--   0 cserrano   (501) staff       (20)     1063 2023-07-12 21:17:31.000000 st_circular_progress-0.3.7/LICENSE
--rw-rw-r--   0 cserrano   (501) staff       (20)       89 2023-07-21 15:17:58.000000 st_circular_progress-0.3.7/MANIFEST.in
--rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 16:14:47.103143 st_circular_progress-0.3.7/PKG-INFO
--rw-r--r--   0 cserrano   (501) staff       (20)     2874 2023-07-21 15:48:57.000000 st_circular_progress-0.3.7/README.md
--rw-r--r--   0 cserrano   (501) staff       (20)       38 2023-07-21 16:14:47.103612 st_circular_progress-0.3.7/setup.cfg
--rw-rw-r--   0 cserrano   (501) staff       (20)      633 2023-07-21 16:12:40.000000 st_circular_progress-0.3.7/setup.py
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 16:14:47.087774 st_circular_progress-0.3.7/st_circular_progress/
--rw-rw-r--   0 cserrano   (501) staff       (20)     2117 2023-07-21 16:14:36.000000 st_circular_progress-0.3.7/st_circular_progress/__init__.py
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 16:14:47.082678 st_circular_progress-0.3.7/st_circular_progress/frontend/
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 16:14:47.095441 st_circular_progress-0.3.7/st_circular_progress/frontend/build/
--rw-r--r--   0 cserrano   (501) staff       (20)      221 2023-07-21 16:05:51.000000 st_circular_progress-0.3.7/st_circular_progress/frontend/build/asset-manifest.json
--rw-rw-r--   0 cserrano   (501) staff       (20)   197459 2023-07-21 16:05:45.000000 st_circular_progress-0.3.7/st_circular_progress/frontend/build/bootstrap.min.css
--rw-r--r--   0 cserrano   (501) staff       (20)      194 2023-07-21 16:05:51.000000 st_circular_progress-0.3.7/st_circular_progress/frontend/build/index.html
--rw-r--r--   0 cserrano   (501) staff       (20)     1663 2023-07-21 16:05:45.000000 st_circular_progress-0.3.7/st_circular_progress/frontend/build/progress.css
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 16:14:47.083452 st_circular_progress-0.3.7/st_circular_progress/frontend/build/static/
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 16:14:47.099616 st_circular_progress-0.3.7/st_circular_progress/frontend/build/static/js/
--rw-r--r--   0 cserrano   (501) staff       (20)   254126 2023-07-21 16:05:51.000000 st_circular_progress-0.3.7/st_circular_progress/frontend/build/static/js/main.a9466aa5.js
--rw-r--r--   0 cserrano   (501) staff       (20)      692 2023-07-21 16:05:51.000000 st_circular_progress-0.3.7/st_circular_progress/frontend/build/static/js/main.a9466aa5.js.LICENSE.txt
--rw-r--r--   0 cserrano   (501) staff       (20)  1042918 2023-07-21 16:05:51.000000 st_circular_progress-0.3.7/st_circular_progress/frontend/build/static/js/main.a9466aa5.js.map
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 16:14:47.090700 st_circular_progress-0.3.7/st_circular_progress.egg-info/
--rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 16:14:46.000000 st_circular_progress-0.3.7/st_circular_progress.egg-info/PKG-INFO
--rw-r--r--   0 cserrano   (501) staff       (20)      701 2023-07-21 16:14:47.000000 st_circular_progress-0.3.7/st_circular_progress.egg-info/SOURCES.txt
--rw-r--r--   0 cserrano   (501) staff       (20)        1 2023-07-21 16:14:46.000000 st_circular_progress-0.3.7/st_circular_progress.egg-info/dependency_links.txt
--rw-r--r--   0 cserrano   (501) staff       (20)       18 2023-07-21 16:14:46.000000 st_circular_progress-0.3.7/st_circular_progress.egg-info/requires.txt
--rw-r--r--   0 cserrano   (501) staff       (20)       21 2023-07-21 16:14:46.000000 st_circular_progress-0.3.7/st_circular_progress.egg-info/top_level.txt
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 16:15:46.205343 st_circular_progress-0.3.8/
+-rw-rw-r--   0 cserrano   (501) staff       (20)     1063 2023-07-12 21:17:31.000000 st_circular_progress-0.3.8/LICENSE
+-rw-rw-r--   0 cserrano   (501) staff       (20)       89 2023-07-21 15:17:58.000000 st_circular_progress-0.3.8/MANIFEST.in
+-rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 16:15:46.205016 st_circular_progress-0.3.8/PKG-INFO
+-rw-r--r--   0 cserrano   (501) staff       (20)     2874 2023-07-21 15:48:57.000000 st_circular_progress-0.3.8/README.md
+-rw-r--r--   0 cserrano   (501) staff       (20)       38 2023-07-21 16:15:46.205455 st_circular_progress-0.3.8/setup.cfg
+-rw-rw-r--   0 cserrano   (501) staff       (20)      633 2023-07-21 16:15:35.000000 st_circular_progress-0.3.8/setup.py
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 16:15:46.195182 st_circular_progress-0.3.8/st_circular_progress/
+-rw-rw-r--   0 cserrano   (501) staff       (20)     2117 2023-07-21 16:15:02.000000 st_circular_progress-0.3.8/st_circular_progress/__init__.py
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 16:15:46.191909 st_circular_progress-0.3.8/st_circular_progress/frontend/
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 16:15:46.201109 st_circular_progress-0.3.8/st_circular_progress/frontend/build/
+-rw-r--r--   0 cserrano   (501) staff       (20)      221 2023-07-21 16:05:51.000000 st_circular_progress-0.3.8/st_circular_progress/frontend/build/asset-manifest.json
+-rw-rw-r--   0 cserrano   (501) staff       (20)   197459 2023-07-21 16:05:45.000000 st_circular_progress-0.3.8/st_circular_progress/frontend/build/bootstrap.min.css
+-rw-r--r--   0 cserrano   (501) staff       (20)      194 2023-07-21 16:05:51.000000 st_circular_progress-0.3.8/st_circular_progress/frontend/build/index.html
+-rw-r--r--   0 cserrano   (501) staff       (20)     1663 2023-07-21 16:05:45.000000 st_circular_progress-0.3.8/st_circular_progress/frontend/build/progress.css
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 16:15:46.192710 st_circular_progress-0.3.8/st_circular_progress/frontend/build/static/
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 16:15:46.203200 st_circular_progress-0.3.8/st_circular_progress/frontend/build/static/js/
+-rw-r--r--   0 cserrano   (501) staff       (20)   254126 2023-07-21 16:05:51.000000 st_circular_progress-0.3.8/st_circular_progress/frontend/build/static/js/main.a9466aa5.js
+-rw-r--r--   0 cserrano   (501) staff       (20)      692 2023-07-21 16:05:51.000000 st_circular_progress-0.3.8/st_circular_progress/frontend/build/static/js/main.a9466aa5.js.LICENSE.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)  1042918 2023-07-21 16:05:51.000000 st_circular_progress-0.3.8/st_circular_progress/frontend/build/static/js/main.a9466aa5.js.map
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 16:15:46.198478 st_circular_progress-0.3.8/st_circular_progress.egg-info/
+-rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 16:15:46.000000 st_circular_progress-0.3.8/st_circular_progress.egg-info/PKG-INFO
+-rw-r--r--   0 cserrano   (501) staff       (20)      701 2023-07-21 16:15:46.000000 st_circular_progress-0.3.8/st_circular_progress.egg-info/SOURCES.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)        1 2023-07-21 16:15:46.000000 st_circular_progress-0.3.8/st_circular_progress.egg-info/dependency_links.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)       18 2023-07-21 16:15:46.000000 st_circular_progress-0.3.8/st_circular_progress.egg-info/requires.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)       21 2023-07-21 16:15:46.000000 st_circular_progress-0.3.8/st_circular_progress.egg-info/top_level.txt
```

### Comparing `st_circular_progress-0.3.7/LICENSE` & `st_circular_progress-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `st_circular_progress-0.3.7/README.md` & `st_circular_progress-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `st_circular_progress-0.3.7/setup.py` & `st_circular_progress-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_circular_progress",
-    version="0.3.7",
+    version="0.3.8",
     author="Carlos D Serrano",
     author_email="sqlinsights@gmail.com",
     description="Circular progress wheel for Streamlit",
     long_description="Streamlit custom component based in VanillaJs that generates a Circular Shaped progress bar.",
     long_description_content_type="text/plain",
     url="https://github.com/sqlinsights/st-circular-progress",
     packages=setuptools.find_packages(),
```

### Comparing `st_circular_progress-0.3.7/st_circular_progress/__init__.py` & `st_circular_progress-0.3.8/st_circular_progress/__init__.py`

 * *Files identical despite different names*

### Comparing `st_circular_progress-0.3.7/st_circular_progress/frontend/build/bootstrap.min.css` & `st_circular_progress-0.3.8/st_circular_progress/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st_circular_progress-0.3.7/st_circular_progress/frontend/build/progress.css` & `st_circular_progress-0.3.8/st_circular_progress/frontend/build/progress.css`

 * *Files identical despite different names*

### Comparing `st_circular_progress-0.3.7/st_circular_progress/frontend/build/static/js/main.a9466aa5.js` & `st_circular_progress-0.3.8/st_circular_progress/frontend/build/static/js/main.a9466aa5.js`

 * *Files identical despite different names*

### Comparing `st_circular_progress-0.3.7/st_circular_progress/frontend/build/static/js/main.a9466aa5.js.LICENSE.txt` & `st_circular_progress-0.3.8/st_circular_progress/frontend/build/static/js/main.a9466aa5.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_circular_progress-0.3.7/st_circular_progress/frontend/build/static/js/main.a9466aa5.js.map` & `st_circular_progress-0.3.8/st_circular_progress/frontend/build/static/js/main.a9466aa5.js.map`

 * *Files identical despite different names*

### Comparing `st_circular_progress-0.3.7/st_circular_progress.egg-info/SOURCES.txt` & `st_circular_progress-0.3.8/st_circular_progress.egg-info/SOURCES.txt`

 * *Files identical despite different names*

