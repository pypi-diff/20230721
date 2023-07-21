# Comparing `tmp/axa-fr-splitter-0.0.2.tar.gz` & `tmp/axa-fr-splitter-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axa-fr-splitter-0.0.2.tar", last modified: Tue Jul 18 14:17:36 2023, max compression
+gzip compressed data, was "axa-fr-splitter-0.1.0.tar", last modified: Fri Jul 21 09:51:28 2023, max compression
```

## Comparing `axa-fr-splitter-0.0.2.tar` & `axa-fr-splitter-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:17:36.322157 axa-fr-splitter-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-18 14:17:36.322157 axa-fr-splitter-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 14:17:25.000000 axa-fr-splitter-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:17:36.322157 axa-fr-splitter-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-18 14:17:25.000000 axa-fr-splitter-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:17:36.318157 axa-fr-splitter-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:17:36.318157 axa-fr-splitter-0.0.2/src/axa_fr_splitter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-18 14:17:36.000000 axa-fr-splitter-0.0.2/src/axa_fr_splitter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-18 14:17:36.000000 axa-fr-splitter-0.0.2/src/axa_fr_splitter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:17:36.000000 axa-fr-splitter-0.0.2/src/axa_fr_splitter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-18 14:17:36.000000 axa-fr-splitter-0.0.2/src/axa_fr_splitter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 14:17:36.000000 axa-fr-splitter-0.0.2/src/axa_fr_splitter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:17:36.322157 axa-fr-splitter-0.0.2/src/splitter/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-18 14:17:25.000000 axa-fr-splitter-0.0.2/src/splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-18 14:17:25.000000 axa-fr-splitter-0.0.2/src/splitter/eml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-18 14:17:25.000000 axa-fr-splitter-0.0.2/src/splitter/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-18 14:17:25.000000 axa-fr-splitter-0.0.2/src/splitter/extension_handler_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-18 14:17:25.000000 axa-fr-splitter-0.0.2/src/splitter/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-18 14:17:25.000000 axa-fr-splitter-0.0.2/src/splitter/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-18 14:17:25.000000 axa-fr-splitter-0.0.2/src/splitter/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-18 14:17:25.000000 axa-fr-splitter-0.0.2/src/splitter/image_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-18 14:17:25.000000 axa-fr-splitter-0.0.2/src/splitter/magic_mime_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-18 14:17:25.000000 axa-fr-splitter-0.0.2/src/splitter/mime_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-18 14:17:25.000000 axa-fr-splitter-0.0.2/src/splitter/mime_reader_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-07-18 14:17:25.000000 axa-fr-splitter-0.0.2/src/splitter/pdf_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-18 14:17:25.000000 axa-fr-splitter-0.0.2/src/splitter/tiff_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:51:28.960329 axa-fr-splitter-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-21 09:51:20.000000 axa-fr-splitter-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-21 09:51:28.960329 axa-fr-splitter-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-21 09:51:20.000000 axa-fr-splitter-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 09:51:28.960329 axa-fr-splitter-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-21 09:51:20.000000 axa-fr-splitter-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:51:28.952329 axa-fr-splitter-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:51:28.956328 axa-fr-splitter-0.1.0/src/axa_fr_splitter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-21 09:51:28.000000 axa-fr-splitter-0.1.0/src/axa_fr_splitter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-21 09:51:28.000000 axa-fr-splitter-0.1.0/src/axa_fr_splitter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 09:51:28.000000 axa-fr-splitter-0.1.0/src/axa_fr_splitter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-21 09:51:28.000000 axa-fr-splitter-0.1.0/src/axa_fr_splitter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 09:51:28.000000 axa-fr-splitter-0.1.0/src/axa_fr_splitter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:51:28.960329 axa-fr-splitter-0.1.0/src/splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-21 09:51:20.000000 axa-fr-splitter-0.1.0/src/splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-21 09:51:20.000000 axa-fr-splitter-0.1.0/src/splitter/eml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-21 09:51:20.000000 axa-fr-splitter-0.1.0/src/splitter/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-21 09:51:20.000000 axa-fr-splitter-0.1.0/src/splitter/extension_handler_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-21 09:51:20.000000 axa-fr-splitter-0.1.0/src/splitter/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-21 09:51:20.000000 axa-fr-splitter-0.1.0/src/splitter/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-21 09:51:20.000000 axa-fr-splitter-0.1.0/src/splitter/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-21 09:51:20.000000 axa-fr-splitter-0.1.0/src/splitter/image_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-21 09:51:20.000000 axa-fr-splitter-0.1.0/src/splitter/magic_mime_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-21 09:51:20.000000 axa-fr-splitter-0.1.0/src/splitter/mime_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-21 09:51:20.000000 axa-fr-splitter-0.1.0/src/splitter/mime_reader_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-07-21 09:51:20.000000 axa-fr-splitter-0.1.0/src/splitter/pdf_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-21 09:51:20.000000 axa-fr-splitter-0.1.0/src/splitter/tiff_handler.py
```

### Comparing `axa-fr-splitter-0.0.2/PKG-INFO` & `axa-fr-splitter-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: axa-fr-splitter
-Version: 0.0.2
+Version: 0.1.0
 Summary: AXA France file splitter package
 Home-page: https://github.com/AxaFrance/axa-fr-splitter
 Author: AXA
 Author-email: guillaume.chervet@axa.fr
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.8
+License-File: LICENSE
 
 Utility library used to split pages from common file types (pdf, tiff) into separate png files. It also extracts text from input files.
```

### Comparing `axa-fr-splitter-0.0.2/setup.py` & `axa-fr-splitter-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `axa-fr-splitter-0.0.2/src/axa_fr_splitter.egg-info/PKG-INFO` & `axa-fr-splitter-0.1.0/src/axa_fr_splitter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: axa-fr-splitter
-Version: 0.0.2
+Version: 0.1.0
 Summary: AXA France file splitter package
 Home-page: https://github.com/AxaFrance/axa-fr-splitter
 Author: AXA
 Author-email: guillaume.chervet@axa.fr
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.8
+License-File: LICENSE
 
 Utility library used to split pages from common file types (pdf, tiff) into separate png files. It also extracts text from input files.
```

### Comparing `axa-fr-splitter-0.0.2/src/axa_fr_splitter.egg-info/SOURCES.txt` & `axa-fr-splitter-0.1.0/src/axa_fr_splitter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 src/axa_fr_splitter.egg-info/PKG-INFO
 src/axa_fr_splitter.egg-info/SOURCES.txt
 src/axa_fr_splitter.egg-info/dependency_links.txt
 src/axa_fr_splitter.egg-info/requires.txt
 src/axa_fr_splitter.egg-info/top_level.txt
```

### Comparing `axa-fr-splitter-0.0.2/src/splitter/eml_handler.py` & `axa-fr-splitter-0.1.0/src/splitter/eml_handler.py`

 * *Files identical despite different names*

### Comparing `axa-fr-splitter-0.0.2/src/splitter/file_handler.py` & `axa-fr-splitter-0.1.0/src/splitter/file_handler.py`

 * *Files identical despite different names*

### Comparing `axa-fr-splitter-0.0.2/src/splitter/image.py` & `axa-fr-splitter-0.1.0/src/splitter/image.py`

 * *Files identical despite different names*

### Comparing `axa-fr-splitter-0.0.2/src/splitter/image_handler.py` & `axa-fr-splitter-0.1.0/src/splitter/image_handler.py`

 * *Files identical despite different names*

### Comparing `axa-fr-splitter-0.0.2/src/splitter/pdf_handler.py` & `axa-fr-splitter-0.1.0/src/splitter/pdf_handler.py`

 * *Files identical despite different names*

### Comparing `axa-fr-splitter-0.0.2/src/splitter/tiff_handler.py` & `axa-fr-splitter-0.1.0/src/splitter/tiff_handler.py`

 * *Files identical despite different names*

