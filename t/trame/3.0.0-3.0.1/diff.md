# Comparing `tmp/trame-3.0.0.tar.gz` & `tmp/trame-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-3.0.0.tar", last modified: Thu Jul 20 21:25:05 2023, max compression
+gzip compressed data, was "trame-3.0.1.tar", last modified: Thu Jul 20 23:15:14 2023, max compression
```

## Comparing `trame-3.0.0.tar` & `trame-3.0.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:25:05.347894 trame-3.0.0/
--rw-r--r--   0 root         (0) root         (0)      552 2023-07-20 21:25:01.000000 trame-3.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-20 21:25:01.000000 trame-3.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6849 2023-07-20 21:25:05.347894 trame-3.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6111 2023-07-20 21:25:01.000000 trame-3.0.0/README.rst
--rw-r--r--   0 root         (0) root         (0)      922 2023-07-20 21:25:05.347894 trame-3.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 21:25:01.000000 trame-3.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:25:05.343894 trame-3.0.0/trame/
--rw-r--r--   0 root         (0) root         (0)      552 2023-07-20 21:25:01.000000 trame-3.0.0/trame/LICENSE
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-20 21:25:01.000000 trame-3.0.0/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:25:05.347894 trame-3.0.0/trame/app/
--rw-r--r--   0 root         (0) root         (0)     4766 2023-07-20 21:25:01.000000 trame-3.0.0/trame/app/__init__.py
--rw-r--r--   0 root         (0) root         (0)      271 2023-07-20 21:25:01.000000 trame-3.0.0/trame/app/asynchronous.py
--rw-r--r--   0 root         (0) root         (0)     1886 2023-07-20 21:25:01.000000 trame-3.0.0/trame/app/demo.py
--rw-r--r--   0 root         (0) root         (0)     1472 2023-07-20 21:25:01.000000 trame-3.0.0/trame/app/dev.py
--rw-r--r--   0 root         (0) root         (0)     1389 2023-07-20 21:25:01.000000 trame-3.0.0/trame/app/file_upload.py
--rw-r--r--   0 root         (0) root         (0)     2364 2023-07-20 21:25:01.000000 trame-3.0.0/trame/app/jupyter.py
--rw-r--r--   0 root         (0) root         (0)     1309 2023-07-20 21:25:01.000000 trame-3.0.0/trame/app/mimetypes.py
--rw-r--r--   0 root         (0) root         (0)      577 2023-07-20 21:25:01.000000 trame-3.0.0/trame/app/singleton.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-07-20 21:25:01.000000 trame-3.0.0/trame/app/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:25:05.347894 trame-3.0.0/trame/assets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 21:25:01.000000 trame-3.0.0/trame/assets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4337 2023-07-20 21:25:01.000000 trame-3.0.0/trame/assets/local.py
--rw-r--r--   0 root         (0) root         (0)     4362 2023-07-20 21:25:01.000000 trame-3.0.0/trame/assets/remote.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:25:05.347894 trame-3.0.0/trame/env/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:25:01.000000 trame-3.0.0/trame/env/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1863 2023-07-20 21:25:01.000000 trame-3.0.0/trame/env/paraview.py
--rw-r--r--   0 root         (0) root         (0)     3930 2023-07-20 21:25:01.000000 trame-3.0.0/trame/env/utils.py
--rw-r--r--   0 root         (0) root         (0)     1311 2023-07-20 21:25:01.000000 trame-3.0.0/trame/env/venv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:25:05.347894 trame-3.0.0/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 21:25:01.000000 trame-3.0.0/trame/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:25:05.347894 trame-3.0.0/trame/tools/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 21:25:01.000000 trame-3.0.0/trame/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1417 2023-07-20 21:25:01.000000 trame-3.0.0/trame/tools/app.py
--rw-r--r--   0 root         (0) root         (0)     2926 2023-07-20 21:25:01.000000 trame-3.0.0/trame/tools/www.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:25:05.347894 trame-3.0.0/trame/ui/
--rw-r--r--   0 root         (0) root         (0)       56 2023-07-20 21:25:01.000000 trame-3.0.0/trame/ui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:25:05.347894 trame-3.0.0/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 21:25:01.000000 trame-3.0.0/trame/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:25:05.343894 trame-3.0.0/trame.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6849 2023-07-20 21:25:05.000000 trame-3.0.0/trame.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      707 2023-07-20 21:25:05.000000 trame-3.0.0/trame.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 21:25:05.000000 trame-3.0.0/trame.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-20 21:25:05.000000 trame-3.0.0/trame.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-07-20 21:25:05.000000 trame-3.0.0/trame.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:15:14.493377 trame-3.0.1/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-07-20 23:15:11.000000 trame-3.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-20 23:15:11.000000 trame-3.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6849 2023-07-20 23:15:14.493377 trame-3.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6111 2023-07-20 23:15:11.000000 trame-3.0.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)      922 2023-07-20 23:15:14.493377 trame-3.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 23:15:11.000000 trame-3.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:15:14.489377 trame-3.0.1/trame/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-07-20 23:15:11.000000 trame-3.0.1/trame/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-20 23:15:11.000000 trame-3.0.1/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:15:14.493377 trame-3.0.1/trame/app/
+-rw-r--r--   0 root         (0) root         (0)     4881 2023-07-20 23:15:11.000000 trame-3.0.1/trame/app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      271 2023-07-20 23:15:11.000000 trame-3.0.1/trame/app/asynchronous.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-07-20 23:15:11.000000 trame-3.0.1/trame/app/demo.py
+-rw-r--r--   0 root         (0) root         (0)     1472 2023-07-20 23:15:11.000000 trame-3.0.1/trame/app/dev.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-07-20 23:15:11.000000 trame-3.0.1/trame/app/file_upload.py
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-07-20 23:15:11.000000 trame-3.0.1/trame/app/jupyter.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2023-07-20 23:15:11.000000 trame-3.0.1/trame/app/mimetypes.py
+-rw-r--r--   0 root         (0) root         (0)      577 2023-07-20 23:15:11.000000 trame-3.0.1/trame/app/singleton.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-07-20 23:15:11.000000 trame-3.0.1/trame/app/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:15:14.493377 trame-3.0.1/trame/assets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 23:15:11.000000 trame-3.0.1/trame/assets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4337 2023-07-20 23:15:11.000000 trame-3.0.1/trame/assets/local.py
+-rw-r--r--   0 root         (0) root         (0)     4362 2023-07-20 23:15:11.000000 trame-3.0.1/trame/assets/remote.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:15:14.493377 trame-3.0.1/trame/env/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 23:15:11.000000 trame-3.0.1/trame/env/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-07-20 23:15:11.000000 trame-3.0.1/trame/env/paraview.py
+-rw-r--r--   0 root         (0) root         (0)     3930 2023-07-20 23:15:11.000000 trame-3.0.1/trame/env/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-07-20 23:15:11.000000 trame-3.0.1/trame/env/venv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:15:14.493377 trame-3.0.1/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 23:15:11.000000 trame-3.0.1/trame/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:15:14.493377 trame-3.0.1/trame/tools/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 23:15:11.000000 trame-3.0.1/trame/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-07-20 23:15:11.000000 trame-3.0.1/trame/tools/app.py
+-rw-r--r--   0 root         (0) root         (0)     2926 2023-07-20 23:15:11.000000 trame-3.0.1/trame/tools/www.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:15:14.493377 trame-3.0.1/trame/ui/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-20 23:15:11.000000 trame-3.0.1/trame/ui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:15:14.493377 trame-3.0.1/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 23:15:11.000000 trame-3.0.1/trame/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:15:14.489377 trame-3.0.1/trame.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6849 2023-07-20 23:15:14.000000 trame-3.0.1/trame.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      707 2023-07-20 23:15:14.000000 trame-3.0.1/trame.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 23:15:14.000000 trame-3.0.1/trame.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-20 23:15:14.000000 trame-3.0.1/trame.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-20 23:15:14.000000 trame-3.0.1/trame.egg-info/top_level.txt
```

### Comparing `trame-3.0.0/LICENSE` & `trame-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-3.0.0/PKG-INFO` & `trame-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame
-Version: 3.0.0
+Version: 3.0.1
 Summary: Trame, a framework to build applications in plain Python
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-3.0.0/README.rst` & `trame-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `trame-3.0.0/setup.cfg` & `trame-3.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame
-version = 3.0.0
+version = 3.0.1
 description = Trame, a framework to build applications in plain Python
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache License 2.0
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-3.0.0/trame/LICENSE` & `trame-3.0.1/trame/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-3.0.0/trame/app/__init__.py` & `trame-3.0.1/trame/app/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,30 @@
+import logging
 from trame_server import Server, Client
 from trame_server.core import set_default_client_type, DEFAULT_CLIENT_TYPE
 from trame_client.widgets.core import VirtualNode
 
 # Ensure this is imported so that mimetypes.init() is decorated
 import trame.app.mimetypes  # noqa: F401
 
 DEFAULT_NAME = "trame"
 AVAILABLE_SERVERS = {}
 AVAILABLE_CLIENTS = {}
 
+logger = logging.getLogger(__name__)
+
 
 def trame_3_warning(*args, **kwargs):
-    print()
-    print("-" * 80)
-    print("   !!! You are currently using trame@3 which may break your application !!!")
-    print("-" * 80)
-    print(
+    logger.warn("")
+    logger.warn("-" * 80)
+    logger.warn(
+        "   !!! You are currently using trame@3 which may break your application !!!"
+    )
+    logger.warn("-" * 80)
+    logger.warn(
         "\n 1. trame@3 only provides by default trame.widgets.[html,client] and remove"
         "\n    everything else as implicit dependency. Those other widgets will still"
         "\n    exist and will be supported, but they will need to be defined as a"
         "\n    dependency of your application."
         "\n"
         "\n       $ pip install trame-vtk trame-vuetify trame-plotly"
         "\n"
@@ -44,18 +49,18 @@
         "\n"
         "\n Actions items"
         "\n ~~~~~~~~~~~~~"
         "\n   a. Make sure you set `server.client_type` to either 'vue2' or 'vue3'."
         "\n   b. List the expected dependencies or have a 'trame<3' dependency"
         "\n"
     )
-    print("-" * 80)
-    print(f" => Current client_type default: {DEFAULT_CLIENT_TYPE}")
-    print("-" * 80)
-    print(flush=True)
+    logger.warn("-" * 80)
+    logger.warn(f" => Current client_type default: {DEFAULT_CLIENT_TYPE}")
+    logger.warn("-" * 80)
+    logger.warn("")
 
 
 # ---------------------------------------------------------
 # After December 2023 we will switch to vue3
 # ---------------------------------------------------------
 set_default_client_type("vue2")
 trame_3_warning()
```

### Comparing `trame-3.0.0/trame/app/demo.py` & `trame-3.0.1/trame/app/demo.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.0/trame/app/dev.py` & `trame-3.0.1/trame/app/dev.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.0/trame/app/file_upload.py` & `trame-3.0.1/trame/app/file_upload.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.0/trame/app/jupyter.py` & `trame-3.0.1/trame/app/jupyter.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.0/trame/app/mimetypes.py` & `trame-3.0.1/trame/app/mimetypes.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.0/trame/app/singleton.py` & `trame-3.0.1/trame/app/singleton.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.0/trame/app/testing.py` & `trame-3.0.1/trame/app/testing.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.0/trame/assets/local.py` & `trame-3.0.1/trame/assets/local.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.0/trame/assets/remote.py` & `trame-3.0.1/trame/assets/remote.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.0/trame/env/paraview.py` & `trame-3.0.1/trame/env/paraview.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.0/trame/env/utils.py` & `trame-3.0.1/trame/env/utils.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.0/trame/env/venv.py` & `trame-3.0.1/trame/env/venv.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.0/trame/tools/app.py` & `trame-3.0.1/trame/tools/app.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.0/trame/tools/www.py` & `trame-3.0.1/trame/tools/www.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.0/trame.egg-info/PKG-INFO` & `trame-3.0.1/trame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame
-Version: 3.0.0
+Version: 3.0.1
 Summary: Trame, a framework to build applications in plain Python
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-3.0.0/trame.egg-info/SOURCES.txt` & `trame-3.0.1/trame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

