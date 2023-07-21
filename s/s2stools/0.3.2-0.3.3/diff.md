# Comparing `tmp/s2stools-0.3.2.tar.gz` & `tmp/s2stools-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2stools-0.3.2.tar", last modified: Fri Jul 21 12:49:39 2023, max compression
+gzip compressed data, was "s2stools-0.3.3.tar", last modified: Fri Jul 21 12:52:15 2023, max compression
```

## Comparing `s2stools-0.3.2.tar` & `s2stools-0.3.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 12:49:39.000000 s2stools-0.3.2/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       99 2023-07-20 08:28:10.000000 s2stools-0.3.2/AUTHORS.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       52 2023-07-20 08:28:10.000000 s2stools-0.3.2/CONTRIBUTING.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       15 2023-07-20 08:28:10.000000 s2stools-0.3.2/LICENSE
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      359 2023-07-20 08:28:10.000000 s2stools-0.3.2/MANIFEST.in
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1642 2023-07-21 12:49:39.000000 s2stools-0.3.2/PKG-INFO
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      913 2023-07-20 08:28:10.000000 s2stools-0.3.2/README.rst
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 12:49:39.000000 s2stools-0.3.2/docs/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      638 2023-07-20 08:28:10.000000 s2stools-0.3.2/docs/Makefile
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      769 2023-07-20 08:28:10.000000 s2stools-0.3.2/docs/make.bat
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 12:49:39.000000 s2stools-0.3.2/docs/source/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      260 2023-07-20 08:28:10.000000 s2stools-0.3.2/docs/source/clim.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      190 2023-07-21 09:20:50.000000 s2stools-0.3.2/docs/source/compute.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1247 2023-07-20 08:28:10.000000 s2stools-0.3.2/docs/source/conf.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     3141 2023-07-21 12:11:20.000000 s2stools-0.3.2/docs/source/download.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      598 2023-07-21 09:20:50.000000 s2stools-0.3.2/docs/source/events.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      588 2023-07-21 11:42:58.000000 s2stools-0.3.2/docs/source/index.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      539 2023-07-21 09:20:50.000000 s2stools-0.3.2/docs/source/indices.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      306 2023-07-21 12:49:12.000000 s2stools-0.3.2/docs/source/install.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     3432 2023-07-20 08:28:10.000000 s2stools-0.3.2/docs/source/intro.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      301 2023-07-20 08:28:10.000000 s2stools-0.3.2/docs/source/plot.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      189 2023-07-20 08:28:10.000000 s2stools-0.3.2/docs/source/process.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      951 2023-07-21 12:49:28.000000 s2stools-0.3.2/pyproject.toml
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      105 2023-07-21 12:48:44.000000 s2stools-0.3.2/requirements.txt
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 12:49:39.000000 s2stools-0.3.2/s2stools/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      100 2023-07-21 12:49:24.000000 s2stools-0.3.2/s2stools/__init__.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      211 2023-07-20 08:28:10.000000 s2stools-0.3.2/s2stools/_version.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)    13035 2023-07-21 09:20:50.000000 s2stools-0.3.2/s2stools/clim.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     9421 2023-07-21 09:20:50.000000 s2stools-0.3.2/s2stools/compute.py
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 12:49:39.000000 s2stools-0.3.2/s2stools/download/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      825 2023-07-21 09:20:50.000000 s2stools-0.3.2/s2stools/download/S2SDownloader.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       61 2023-07-21 09:20:50.000000 s2stools-0.3.2/s2stools/download/__init__.py
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 12:49:39.000000 s2stools-0.3.2/s2stools/download/ecmwf/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     6725 2023-07-21 09:20:50.000000 s2stools-0.3.2/s2stools/download/ecmwf/S2SDownloaderECMWF.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       33 2023-07-21 09:20:50.000000 s2stools-0.3.2/s2stools/download/ecmwf/__init__.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     2430 2023-07-21 09:20:50.000000 s2stools-0.3.2/s2stools/download/ecmwf/model_setup.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      530 2023-07-21 10:10:48.000000 s2stools-0.3.2/s2stools/download/utils.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)    21424 2023-07-21 09:20:50.000000 s2stools-0.3.2/s2stools/events.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     4685 2023-07-21 09:20:50.000000 s2stools-0.3.2/s2stools/indices.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     7252 2023-07-21 09:20:50.000000 s2stools-0.3.2/s2stools/plot.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)    16985 2023-07-21 09:20:50.000000 s2stools-0.3.2/s2stools/process.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     2459 2023-07-21 09:20:50.000000 s2stools-0.3.2/s2stools/utils.py
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 12:49:39.000000 s2stools-0.3.2/s2stools.egg-info/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1642 2023-07-21 12:49:39.000000 s2stools-0.3.2/s2stools.egg-info/PKG-INFO
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      923 2023-07-21 12:49:39.000000 s2stools-0.3.2/s2stools.egg-info/SOURCES.txt
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)        1 2023-07-21 12:49:39.000000 s2stools-0.3.2/s2stools.egg-info/dependency_links.txt
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       47 2023-07-21 12:49:39.000000 s2stools-0.3.2/s2stools.egg-info/requires.txt
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)        9 2023-07-21 12:49:39.000000 s2stools-0.3.2/s2stools.egg-info/top_level.txt
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       38 2023-07-21 12:49:39.000000 s2stools-0.3.2/setup.cfg
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       69 2023-07-20 08:28:10.000000 s2stools-0.3.2/setup.py
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 12:52:15.000000 s2stools-0.3.3/
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       99 2023-07-20 08:28:10.000000 s2stools-0.3.3/AUTHORS.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       52 2023-07-20 08:28:10.000000 s2stools-0.3.3/CONTRIBUTING.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       15 2023-07-20 08:28:10.000000 s2stools-0.3.3/LICENSE
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      359 2023-07-20 08:28:10.000000 s2stools-0.3.3/MANIFEST.in
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1642 2023-07-21 12:52:15.000000 s2stools-0.3.3/PKG-INFO
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      913 2023-07-20 08:28:10.000000 s2stools-0.3.3/README.rst
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 12:52:15.000000 s2stools-0.3.3/docs/
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      638 2023-07-20 08:28:10.000000 s2stools-0.3.3/docs/Makefile
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      769 2023-07-20 08:28:10.000000 s2stools-0.3.3/docs/make.bat
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 12:52:15.000000 s2stools-0.3.3/docs/source/
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      260 2023-07-20 08:28:10.000000 s2stools-0.3.3/docs/source/clim.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      190 2023-07-21 09:20:50.000000 s2stools-0.3.3/docs/source/compute.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1247 2023-07-20 08:28:10.000000 s2stools-0.3.3/docs/source/conf.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     3141 2023-07-21 12:11:20.000000 s2stools-0.3.3/docs/source/download.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      598 2023-07-21 09:20:50.000000 s2stools-0.3.3/docs/source/events.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      588 2023-07-21 11:42:58.000000 s2stools-0.3.3/docs/source/index.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      539 2023-07-21 09:20:50.000000 s2stools-0.3.3/docs/source/indices.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      306 2023-07-21 12:49:12.000000 s2stools-0.3.3/docs/source/install.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     3432 2023-07-20 08:28:10.000000 s2stools-0.3.3/docs/source/intro.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      301 2023-07-20 08:28:10.000000 s2stools-0.3.3/docs/source/plot.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      189 2023-07-20 08:28:10.000000 s2stools-0.3.3/docs/source/process.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      975 2023-07-21 12:52:08.000000 s2stools-0.3.3/pyproject.toml
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      105 2023-07-21 12:48:44.000000 s2stools-0.3.3/requirements.txt
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 12:52:15.000000 s2stools-0.3.3/s2stools/
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      100 2023-07-21 12:52:12.000000 s2stools-0.3.3/s2stools/__init__.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      211 2023-07-20 08:28:10.000000 s2stools-0.3.3/s2stools/_version.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)    13035 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/clim.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     9421 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/compute.py
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 12:52:15.000000 s2stools-0.3.3/s2stools/download/
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      825 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/download/S2SDownloader.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       61 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/download/__init__.py
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 12:52:15.000000 s2stools-0.3.3/s2stools/download/ecmwf/
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     6725 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/download/ecmwf/S2SDownloaderECMWF.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       33 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/download/ecmwf/__init__.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     2430 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/download/ecmwf/model_setup.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      530 2023-07-21 10:10:48.000000 s2stools-0.3.3/s2stools/download/utils.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)    21424 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/events.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     4685 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/indices.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     7252 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/plot.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)    16985 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/process.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     2459 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/utils.py
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 12:52:15.000000 s2stools-0.3.3/s2stools.egg-info/
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1642 2023-07-21 12:52:15.000000 s2stools-0.3.3/s2stools.egg-info/PKG-INFO
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      923 2023-07-21 12:52:15.000000 s2stools-0.3.3/s2stools.egg-info/SOURCES.txt
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)        1 2023-07-21 12:52:15.000000 s2stools-0.3.3/s2stools.egg-info/dependency_links.txt
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       64 2023-07-21 12:52:15.000000 s2stools-0.3.3/s2stools.egg-info/requires.txt
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)        9 2023-07-21 12:52:15.000000 s2stools-0.3.3/s2stools.egg-info/top_level.txt
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       38 2023-07-21 12:52:15.000000 s2stools-0.3.3/setup.cfg
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       69 2023-07-20 08:28:10.000000 s2stools-0.3.3/setup.py
```

### Comparing `s2stools-0.3.2/PKG-INFO` & `s2stools-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s2stools
-Version: 0.3.2
+Version: 0.3.3
 Summary: Tools for working with s2s forecast data
 Author-email: Jonas Spaeth <jonas.spaeth@physik.uni-muenchen.de>
 License: BSD-3-Clause
 Project-URL: Source Code, https://github.com/jonas-spaeth/s2stools
 Project-URL: Bug Tracker, https://github.com/jonas-spaeth/s2stools/issues
 Keywords: atmosphere,weather,climate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `s2stools-0.3.2/README.rst` & `s2stools-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.2/docs/Makefile` & `s2stools-0.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.2/docs/make.bat` & `s2stools-0.3.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.2/docs/source/conf.py` & `s2stools-0.3.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.2/docs/source/download.rst` & `s2stools-0.3.3/docs/source/download.rst`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.2/docs/source/events.rst` & `s2stools-0.3.3/docs/source/events.rst`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.2/docs/source/index.rst` & `s2stools-0.3.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.2/docs/source/indices.rst` & `s2stools-0.3.3/docs/source/indices.rst`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.2/docs/source/intro.rst` & `s2stools-0.3.3/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.2/pyproject.toml` & `s2stools-0.3.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "s2stools"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
     { name = "Jonas Spaeth", email = "jonas.spaeth@physik.uni-muenchen.de" },
 ]
 description = "Tools for working with s2s forecast data"
 readme = "README.rst"
 requires-python = ">=3.8"
 keywords = ["atmosphere", "weather", "climate"]
@@ -23,13 +23,14 @@
 dependencies = [
     "numpy",
     "scipy",
     "xarray",
     "tqdm",
     "matplotlib",
     "pandas",
-    "dask"
+    "dask",
+    "ecmwf-api-client"
 ]
 
 [project.urls]
 "Source Code" = "https://github.com/jonas-spaeth/s2stools"
 "Bug Tracker" = "https://github.com/jonas-spaeth/s2stools/issues"
```

### Comparing `s2stools-0.3.2/s2stools/clim.py` & `s2stools-0.3.3/s2stools/clim.py`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.2/s2stools/compute.py` & `s2stools-0.3.3/s2stools/compute.py`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.2/s2stools/download/S2SDownloader.py` & `s2stools-0.3.3/s2stools/download/S2SDownloader.py`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.2/s2stools/download/ecmwf/S2SDownloaderECMWF.py` & `s2stools-0.3.3/s2stools/download/ecmwf/S2SDownloaderECMWF.py`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.2/s2stools/download/ecmwf/model_setup.py` & `s2stools-0.3.3/s2stools/download/ecmwf/model_setup.py`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.2/s2stools/download/utils.py` & `s2stools-0.3.3/s2stools/download/utils.py`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.2/s2stools/events.py` & `s2stools-0.3.3/s2stools/events.py`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.2/s2stools/indices.py` & `s2stools-0.3.3/s2stools/indices.py`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.2/s2stools/plot.py` & `s2stools-0.3.3/s2stools/plot.py`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.2/s2stools/process.py` & `s2stools-0.3.3/s2stools/process.py`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.2/s2stools/utils.py` & `s2stools-0.3.3/s2stools/utils.py`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.2/s2stools.egg-info/PKG-INFO` & `s2stools-0.3.3/s2stools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s2stools
-Version: 0.3.2
+Version: 0.3.3
 Summary: Tools for working with s2s forecast data
 Author-email: Jonas Spaeth <jonas.spaeth@physik.uni-muenchen.de>
 License: BSD-3-Clause
 Project-URL: Source Code, https://github.com/jonas-spaeth/s2stools
 Project-URL: Bug Tracker, https://github.com/jonas-spaeth/s2stools/issues
 Keywords: atmosphere,weather,climate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `s2stools-0.3.2/s2stools.egg-info/SOURCES.txt` & `s2stools-0.3.3/s2stools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

