# Comparing `tmp/s2stools-0.3.3.tar.gz` & `tmp/s2stools-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2stools-0.3.3.tar", last modified: Fri Jul 21 12:52:15 2023, max compression
+gzip compressed data, was "s2stools-0.3.4.tar", last modified: Fri Jul 21 15:39:28 2023, max compression
```

## Comparing `s2stools-0.3.3.tar` & `s2stools-0.3.4.tar`

### file list

```diff
@@ -1,50 +1,63 @@
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 12:52:15.000000 s2stools-0.3.3/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       99 2023-07-20 08:28:10.000000 s2stools-0.3.3/AUTHORS.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       52 2023-07-20 08:28:10.000000 s2stools-0.3.3/CONTRIBUTING.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       15 2023-07-20 08:28:10.000000 s2stools-0.3.3/LICENSE
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      359 2023-07-20 08:28:10.000000 s2stools-0.3.3/MANIFEST.in
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1642 2023-07-21 12:52:15.000000 s2stools-0.3.3/PKG-INFO
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      913 2023-07-20 08:28:10.000000 s2stools-0.3.3/README.rst
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 12:52:15.000000 s2stools-0.3.3/docs/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      638 2023-07-20 08:28:10.000000 s2stools-0.3.3/docs/Makefile
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      769 2023-07-20 08:28:10.000000 s2stools-0.3.3/docs/make.bat
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 12:52:15.000000 s2stools-0.3.3/docs/source/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      260 2023-07-20 08:28:10.000000 s2stools-0.3.3/docs/source/clim.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      190 2023-07-21 09:20:50.000000 s2stools-0.3.3/docs/source/compute.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1247 2023-07-20 08:28:10.000000 s2stools-0.3.3/docs/source/conf.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     3141 2023-07-21 12:11:20.000000 s2stools-0.3.3/docs/source/download.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      598 2023-07-21 09:20:50.000000 s2stools-0.3.3/docs/source/events.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      588 2023-07-21 11:42:58.000000 s2stools-0.3.3/docs/source/index.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      539 2023-07-21 09:20:50.000000 s2stools-0.3.3/docs/source/indices.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      306 2023-07-21 12:49:12.000000 s2stools-0.3.3/docs/source/install.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     3432 2023-07-20 08:28:10.000000 s2stools-0.3.3/docs/source/intro.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      301 2023-07-20 08:28:10.000000 s2stools-0.3.3/docs/source/plot.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      189 2023-07-20 08:28:10.000000 s2stools-0.3.3/docs/source/process.rst
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      975 2023-07-21 12:52:08.000000 s2stools-0.3.3/pyproject.toml
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      105 2023-07-21 12:48:44.000000 s2stools-0.3.3/requirements.txt
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 12:52:15.000000 s2stools-0.3.3/s2stools/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      100 2023-07-21 12:52:12.000000 s2stools-0.3.3/s2stools/__init__.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      211 2023-07-20 08:28:10.000000 s2stools-0.3.3/s2stools/_version.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)    13035 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/clim.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     9421 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/compute.py
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 12:52:15.000000 s2stools-0.3.3/s2stools/download/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      825 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/download/S2SDownloader.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       61 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/download/__init__.py
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 12:52:15.000000 s2stools-0.3.3/s2stools/download/ecmwf/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     6725 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/download/ecmwf/S2SDownloaderECMWF.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       33 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/download/ecmwf/__init__.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     2430 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/download/ecmwf/model_setup.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      530 2023-07-21 10:10:48.000000 s2stools-0.3.3/s2stools/download/utils.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)    21424 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/events.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     4685 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/indices.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     7252 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/plot.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)    16985 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/process.py
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     2459 2023-07-21 09:20:50.000000 s2stools-0.3.3/s2stools/utils.py
-drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 12:52:15.000000 s2stools-0.3.3/s2stools.egg-info/
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1642 2023-07-21 12:52:15.000000 s2stools-0.3.3/s2stools.egg-info/PKG-INFO
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      923 2023-07-21 12:52:15.000000 s2stools-0.3.3/s2stools.egg-info/SOURCES.txt
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)        1 2023-07-21 12:52:15.000000 s2stools-0.3.3/s2stools.egg-info/dependency_links.txt
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       64 2023-07-21 12:52:15.000000 s2stools-0.3.3/s2stools.egg-info/requires.txt
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)        9 2023-07-21 12:52:15.000000 s2stools-0.3.3/s2stools.egg-info/top_level.txt
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       38 2023-07-21 12:52:15.000000 s2stools-0.3.3/setup.cfg
--rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       69 2023-07-20 08:28:10.000000 s2stools-0.3.3/setup.py
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 15:39:28.000000 s2stools-0.3.4/
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       99 2023-07-20 08:28:10.000000 s2stools-0.3.4/AUTHORS.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       52 2023-07-20 08:28:10.000000 s2stools-0.3.4/CONTRIBUTING.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       15 2023-07-20 08:28:10.000000 s2stools-0.3.4/LICENSE
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      359 2023-07-20 08:28:10.000000 s2stools-0.3.4/MANIFEST.in
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1751 2023-07-21 15:39:28.000000 s2stools-0.3.4/PKG-INFO
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1022 2023-07-21 13:09:08.000000 s2stools-0.3.4/README.rst
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 15:39:27.000000 s2stools-0.3.4/docs/
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      638 2023-07-20 08:28:10.000000 s2stools-0.3.4/docs/Makefile
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 15:39:27.000000 s2stools-0.3.4/docs/build/
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 15:39:27.000000 s2stools-0.3.4/docs/build/html/
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 15:39:27.000000 s2stools-0.3.4/docs/build/html/_sources/
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      260 2023-07-20 08:28:10.000000 s2stools-0.3.4/docs/build/html/_sources/clim.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      190 2023-07-21 09:20:50.000000 s2stools-0.3.4/docs/build/html/_sources/compute.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     3141 2023-07-21 12:11:20.000000 s2stools-0.3.4/docs/build/html/_sources/download.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      598 2023-07-21 09:20:50.000000 s2stools-0.3.4/docs/build/html/_sources/events.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      588 2023-07-21 11:42:58.000000 s2stools-0.3.4/docs/build/html/_sources/index.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      539 2023-07-21 09:20:50.000000 s2stools-0.3.4/docs/build/html/_sources/indices.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      306 2023-07-21 12:49:12.000000 s2stools-0.3.4/docs/build/html/_sources/install.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     3432 2023-07-20 08:28:10.000000 s2stools-0.3.4/docs/build/html/_sources/intro.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      301 2023-07-20 08:28:10.000000 s2stools-0.3.4/docs/build/html/_sources/plot.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      189 2023-07-20 08:28:10.000000 s2stools-0.3.4/docs/build/html/_sources/process.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      769 2023-07-20 08:28:10.000000 s2stools-0.3.4/docs/make.bat
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 15:39:27.000000 s2stools-0.3.4/docs/source/
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      260 2023-07-20 08:28:10.000000 s2stools-0.3.4/docs/source/clim.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      190 2023-07-21 09:20:50.000000 s2stools-0.3.4/docs/source/compute.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1247 2023-07-21 15:38:52.000000 s2stools-0.3.4/docs/source/conf.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     3141 2023-07-21 12:11:20.000000 s2stools-0.3.4/docs/source/download.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      598 2023-07-21 09:20:50.000000 s2stools-0.3.4/docs/source/events.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      588 2023-07-21 11:42:58.000000 s2stools-0.3.4/docs/source/index.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      539 2023-07-21 09:20:50.000000 s2stools-0.3.4/docs/source/indices.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      306 2023-07-21 12:49:12.000000 s2stools-0.3.4/docs/source/install.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     3432 2023-07-20 08:28:10.000000 s2stools-0.3.4/docs/source/intro.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      301 2023-07-20 08:28:10.000000 s2stools-0.3.4/docs/source/plot.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      189 2023-07-20 08:28:10.000000 s2stools-0.3.4/docs/source/process.rst
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      975 2023-07-21 15:38:28.000000 s2stools-0.3.4/pyproject.toml
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      105 2023-07-21 12:48:44.000000 s2stools-0.3.4/requirements.txt
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 15:39:27.000000 s2stools-0.3.4/s2stools/
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      100 2023-07-21 15:38:34.000000 s2stools-0.3.4/s2stools/__init__.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      211 2023-07-20 08:28:10.000000 s2stools-0.3.4/s2stools/_version.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)    13035 2023-07-21 09:20:50.000000 s2stools-0.3.4/s2stools/clim.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     9421 2023-07-21 09:20:50.000000 s2stools-0.3.4/s2stools/compute.py
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 15:39:28.000000 s2stools-0.3.4/s2stools/download/
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      825 2023-07-21 09:20:50.000000 s2stools-0.3.4/s2stools/download/S2SDownloader.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       61 2023-07-21 09:20:50.000000 s2stools-0.3.4/s2stools/download/__init__.py
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 15:39:28.000000 s2stools-0.3.4/s2stools/download/ecmwf/
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     6725 2023-07-21 09:20:50.000000 s2stools-0.3.4/s2stools/download/ecmwf/S2SDownloaderECMWF.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       33 2023-07-21 09:20:50.000000 s2stools-0.3.4/s2stools/download/ecmwf/__init__.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     2430 2023-07-21 09:20:50.000000 s2stools-0.3.4/s2stools/download/ecmwf/model_setup.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)      530 2023-07-21 10:10:48.000000 s2stools-0.3.4/s2stools/download/utils.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)    21424 2023-07-21 09:20:50.000000 s2stools-0.3.4/s2stools/events.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     4685 2023-07-21 09:20:50.000000 s2stools-0.3.4/s2stools/indices.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     9225 2023-07-21 13:49:25.000000 s2stools-0.3.4/s2stools/plot.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)    17811 2023-07-21 15:37:12.000000 s2stools-0.3.4/s2stools/process.py
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     2459 2023-07-21 09:20:50.000000 s2stools-0.3.4/s2stools/utils.py
+drwxr-xr-x   0 jonas.spaeth (14484) ag-birner (11658)        0 2023-07-21 15:39:28.000000 s2stools-0.3.4/s2stools.egg-info/
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1751 2023-07-21 15:39:27.000000 s2stools-0.3.4/s2stools.egg-info/PKG-INFO
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)     1283 2023-07-21 15:39:27.000000 s2stools-0.3.4/s2stools.egg-info/SOURCES.txt
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)        1 2023-07-21 15:39:27.000000 s2stools-0.3.4/s2stools.egg-info/dependency_links.txt
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       64 2023-07-21 15:39:27.000000 s2stools-0.3.4/s2stools.egg-info/requires.txt
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)        9 2023-07-21 15:39:27.000000 s2stools-0.3.4/s2stools.egg-info/top_level.txt
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       38 2023-07-21 15:39:28.000000 s2stools-0.3.4/setup.cfg
+-rw-r--r--   0 jonas.spaeth (14484) ag-birner (11658)       69 2023-07-20 08:28:10.000000 s2stools-0.3.4/setup.py
```

### Comparing `s2stools-0.3.3/PKG-INFO` & `s2stools-0.3.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s2stools
-Version: 0.3.3
+Version: 0.3.4
 Summary: Tools for working with s2s forecast data
 Author-email: Jonas Spaeth <jonas.spaeth@physik.uni-muenchen.de>
 License: BSD-3-Clause
 Project-URL: Source Code, https://github.com/jonas-spaeth/s2stools
 Project-URL: Bug Tracker, https://github.com/jonas-spaeth/s2stools/issues
 Keywords: atmosphere,weather,climate
 Classifier: Development Status :: 3 - Alpha
@@ -21,14 +21,19 @@
 s2stools
 ========
 
 .. image:: https://readthedocs.org/projects/s2stools/badge/?version=latest
     :target: https://pyzome.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
+
+.. image:: https://img.shields.io/pypi/v/s2stools.svg
+    :target: https://img.shields.io/pypi/v/s2stools
+
+
 Documentation
 -------------
 
 Documentation on readthedocs: https://s2stools.readthedocs.io
 
 Install
 -------
```

### Comparing `s2stools-0.3.3/README.rst` & `s2stools-0.3.4/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 s2stools
 ========
 
 .. image:: https://readthedocs.org/projects/s2stools/badge/?version=latest
     :target: https://pyzome.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
+
+.. image:: https://img.shields.io/pypi/v/s2stools.svg
+    :target: https://img.shields.io/pypi/v/s2stools
+
+
 Documentation
 -------------
 
 Documentation on readthedocs: https://s2stools.readthedocs.io
 
 Install
 -------
```

### Comparing `s2stools-0.3.3/docs/Makefile` & `s2stools-0.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.3/docs/make.bat` & `s2stools-0.3.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.3/docs/source/conf.py` & `s2stools-0.3.4/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import sys
 
 sys.path.insert(0, os.path.abspath('../s2stools'))
 
 project = "s2stools"
 copyright = "2023, Jonas Spaeth"
 author = "Jonas Spaeth"
-release = "0.3.0"
+release = "0.3.4"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ["sphinx.ext.autodoc", "sphinx.ext.napoleon", "sphinx.ext.todo"]
 
 templates_path = ["_templates"]
```

### Comparing `s2stools-0.3.3/docs/source/download.rst` & `s2stools-0.3.4/docs/build/html/_sources/download.rst`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.3/docs/source/events.rst` & `s2stools-0.3.4/docs/build/html/_sources/events.rst`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.3/docs/source/index.rst` & `s2stools-0.3.4/docs/build/html/_sources/index.rst`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.3/docs/source/indices.rst` & `s2stools-0.3.4/docs/build/html/_sources/indices.rst`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.3/docs/source/intro.rst` & `s2stools-0.3.4/docs/build/html/_sources/intro.rst`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.3/pyproject.toml` & `s2stools-0.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "s2stools"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
     { name = "Jonas Spaeth", email = "jonas.spaeth@physik.uni-muenchen.de" },
 ]
 description = "Tools for working with s2s forecast data"
 readme = "README.rst"
 requires-python = ">=3.8"
 keywords = ["atmosphere", "weather", "climate"]
```

### Comparing `s2stools-0.3.3/s2stools/clim.py` & `s2stools-0.3.4/s2stools/clim.py`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.3/s2stools/compute.py` & `s2stools-0.3.4/s2stools/compute.py`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.3/s2stools/download/S2SDownloader.py` & `s2stools-0.3.4/s2stools/download/S2SDownloader.py`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.3/s2stools/download/ecmwf/S2SDownloaderECMWF.py` & `s2stools-0.3.4/s2stools/download/ecmwf/S2SDownloaderECMWF.py`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.3/s2stools/download/ecmwf/model_setup.py` & `s2stools-0.3.4/s2stools/download/ecmwf/model_setup.py`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.3/s2stools/download/utils.py` & `s2stools-0.3.4/s2stools/download/utils.py`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.3/s2stools/events.py` & `s2stools-0.3.4/s2stools/events.py`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.3/s2stools/indices.py` & `s2stools-0.3.4/s2stools/indices.py`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.3/s2stools/plot.py` & `s2stools-0.3.4/s2stools/plot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 import matplotlib.pyplot as plt
 import matplotlib.ticker
 import numpy as np
 import xarray as xr
-
+import matplotlib.patches as mpatches
 
 # from cartopy.util import add_cyclic_point
 
 
 def xaxis_unit_days(ax=None, multiple=7, minor_multiple=1):
     """
     Convert nanoseconds on x-axis to days.
@@ -98,15 +98,15 @@
         print("This function requires cartopy. Consider: pip install cartopy")
     else:
         field = field.transpose(latitude_name, longitude_name)
         lon = field.longitude
         lat = field.latitude
         adj_field, adj_lon = add_cyclic_point(field, coord=lon)
         return adj_lon, lat, adj_field
-    pass
+
 
 
 def xlim_days(ax=None, leftlim=None, rightlim=None):
     """
     Adjust limits.
 
     Parameters
@@ -267,7 +267,85 @@
     ax : plt.Axis
         Axis.
 
     """
     ylim = ax.get_ylim()
     absylim = np.max(np.abs(ylim))
     ax.set_ylim(-absylim, absylim)
+
+
+def add_map(ax, **kwargs):
+    """
+    Add a nicely formatted map to a proplot axis.
+    Works only with `proplot`  https://proplot.readthedocs.io/en/stable/.
+
+    Parameters
+    ----------
+    ax : proplot axis
+    kwargs : dict
+        parameters passed to ax.format(...). overwrites default parameters.
+
+    Returns
+    -------
+
+    """
+    default_kwargs = dict(
+        coast=True,
+        land=True,
+        landcolor="gray1",
+        landalpha=0.2,
+        landzorder=-100,
+        coastcolor="gray7",
+        coastlinewidth=0.4,
+        coastzorder=100,
+    )
+    plotting_kwargs = default_kwargs | kwargs
+    ax.format(**plotting_kwargs)
+
+def add_box(dict_lon_lat_slice, ax, **kwargs):
+    """
+    Add a box to a map projection plot.
+
+    Parameters
+    ----------
+    dict_lon_lat_slice : dict
+        E.g. {"longitude": slice(0, 180), "latitude": slice(40, 60)}
+    ax : axis
+        matplotlib axis
+    kwargs : dict
+        additional keyword arguments to format/ overwrite appearance, e.g.: facecolor, edgecolor, lw, zorder
+
+    Returns
+    -------
+
+    Warnings
+    --------
+    Requires ``cartopy`` (which is not a formal dependency of ``s2stools``.
+    """
+
+
+    try:
+        import cartopy.crs as ccrs
+    except:
+        print("This function requires cartopy. Consider: pip install cartopy")
+    else:
+        box = dict_lon_lat_slice
+        width = box["longitude"].stop - box["longitude"].start
+        height = box["latitude"].start - box["latitude"].stop
+        x, y = box["longitude"].start, box["latitude"].stop
+
+        plot_kwargs = dict(
+            facecolor=(0, 0, 1, 0.05),
+            edgecolor="k",
+            lw=1,
+            zorder=10,
+        ) | dict(kwargs)
+
+        ax.add_patch(
+            mpatches.Rectangle(
+                xy=[x, y],
+                width=width,
+                height=height,
+                transform=ccrs.PlateCarree(),
+                **plot_kwargs
+            )
+        )
```

### Comparing `s2stools-0.3.3/s2stools/process.py` & `s2stools-0.3.4/s2stools/process.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 IMPL_DATE = "ImplementationDate in S2S"
 
 
 def s2sparser(ds):
     """
     Will create dimensions reftime, hc_year, leadtime.
     Coordinate validtime is automatically added.
+    Files need to have the forecast realtime date somewhere in the filename, e.g., `s2s_something_2017-11-16.nc`.
 
     Parameters
     ----------
     ds : xr.Dataset
         dataset
     Returns
     -------
@@ -125,35 +126,61 @@
     filename = filepath.split("/")[-1]
     # split underscores, one item is probability the date
     filename_underscore_splitted = filename.split("_")
     # usually the second to last item is the date, therefore roll to save time
     filename_underscore_splitted = (
             filename_underscore_splitted[-2:] + filename_underscore_splitted[:-2]
     )
+    # split points
+    filename_underscore_splitted_point_splitted = [
+        i.split('.') for i in filename_underscore_splitted
+    ]
+    filename_underscore_splitted_point_splitted = _flatten_list(filename_underscore_splitted_point_splitted)
+
     # try to parse reftime from one of these items
-    for item in filename_underscore_splitted:
+    for item in filename_underscore_splitted_point_splitted:
         try:
             inferred_reftime = pd.Timestamp(item)
             inferred_reftime = np.datetime64(inferred_reftime)
             break
         except ValueError:
             continue
         except:
             print("unknown error")
     else:
         inferred_reftime = None
         print(
             "unable to identify correct reftime!"
-            + f"Infering reftime from one of these items: {filename_underscore_splitted} failed."
+            + f"Infering reftime from one of these items: {filename_underscore_splitted_point_splitted} failed."
             + "Make sure that the reftime appears in the filename, otherwise can't infer correct reftime."
             + "I mean, we could specify the reftime, e.g., as a list, but I'm not sure if that's convenient... let me know if yes."
+            + "\nValid file names are for example s2s_something_else_2017-11-01_foo_bar.nc, s2s_something_else_20171101.nc"
         )
     return inferred_reftime
 
 
+def _flatten_list(lst):
+    """
+    Convert a list of lists to a flattened list.
+
+    Parameters
+    ----------
+    lst
+
+    Returns
+    -------
+    flat_list : list
+    """
+    for item in lst:
+        if isinstance(item, list):
+            yield from _flatten_list(item)
+        else:
+            yield item
+
+
 def download_table_ecmwf_model():
     path = "https://confluence.ecmwf.int/display/S2S/ECMWF+Model"
     table_ecmwf_model_raw = pd.read_html(path)[0]
 
     table_ecmwf_model = table_ecmwf_model_raw.iloc[1:]
     table_ecmwf_model.loc[:, IMPL_DATE] = pd.to_datetime(
         table_ecmwf_model[IMPL_DATE], infer_datetime_format=True
```

### Comparing `s2stools-0.3.3/s2stools/utils.py` & `s2stools-0.3.4/s2stools/utils.py`

 * *Files identical despite different names*

### Comparing `s2stools-0.3.3/s2stools.egg-info/PKG-INFO` & `s2stools-0.3.4/s2stools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s2stools
-Version: 0.3.3
+Version: 0.3.4
 Summary: Tools for working with s2s forecast data
 Author-email: Jonas Spaeth <jonas.spaeth@physik.uni-muenchen.de>
 License: BSD-3-Clause
 Project-URL: Source Code, https://github.com/jonas-spaeth/s2stools
 Project-URL: Bug Tracker, https://github.com/jonas-spaeth/s2stools/issues
 Keywords: atmosphere,weather,climate
 Classifier: Development Status :: 3 - Alpha
@@ -21,14 +21,19 @@
 s2stools
 ========
 
 .. image:: https://readthedocs.org/projects/s2stools/badge/?version=latest
     :target: https://pyzome.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
+
+.. image:: https://img.shields.io/pypi/v/s2stools.svg
+    :target: https://img.shields.io/pypi/v/s2stools
+
+
 Documentation
 -------------
 
 Documentation on readthedocs: https://s2stools.readthedocs.io
 
 Install
 -------
```

### Comparing `s2stools-0.3.3/s2stools.egg-info/SOURCES.txt` & `s2stools-0.3.4/s2stools.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.txt
 setup.py
 docs/Makefile
 docs/make.bat
+docs/build/html/_sources/clim.rst
+docs/build/html/_sources/compute.rst
+docs/build/html/_sources/download.rst
+docs/build/html/_sources/events.rst
+docs/build/html/_sources/index.rst
+docs/build/html/_sources/indices.rst
+docs/build/html/_sources/install.rst
+docs/build/html/_sources/intro.rst
+docs/build/html/_sources/plot.rst
+docs/build/html/_sources/process.rst
 docs/source/clim.rst
 docs/source/compute.rst
 docs/source/conf.py
 docs/source/download.rst
 docs/source/events.rst
 docs/source/index.rst
 docs/source/indices.rst
```

