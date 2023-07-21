# Comparing `tmp/xaitk-saliency-demo-2.2.1.tar.gz` & `tmp/xaitk-saliency-demo-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xaitk-saliency-demo-2.2.1.tar", last modified: Wed Jul 19 00:21:10 2023, max compression
+gzip compressed data, was "xaitk-saliency-demo-2.2.2.tar", last modified: Fri Jul 21 14:59:12 2023, max compression
```

## Comparing `xaitk-saliency-demo-2.2.1.tar` & `xaitk-saliency-demo-2.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:10.260391 xaitk-saliency-demo-2.2.1/
--rw-r--r--   0 root         (0) root         (0)     1504 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2648 2023-07-19 00:21:10.260391 xaitk-saliency-demo-2.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1866 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/README.rst
--rw-r--r--   0 root         (0) root         (0)     1356 2023-07-19 00:21:10.260391 xaitk-saliency-demo-2.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:10.256391 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/
--rw-r--r--   0 root         (0) root         (0)       49 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:10.256391 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/
--rw-r--r--   0 root         (0) root         (0)       50 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:10.260391 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/
--rw-r--r--   0 root         (0) root         (0)      197 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:10.260391 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/assets/
--rw-r--r--   0 root         (0) root         (0)      498 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/assets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10472 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/assets/imagenet_classes.txt
--rw-r--r--   0 root         (0) root         (0)     1974 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/main.py
--rw-r--r--   0 root         (0) root         (0)     9702 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/ml_models.py
--rw-r--r--   0 root         (0) root         (0)     5565 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/ml_xai.py
--rw-r--r--   0 root         (0) root         (0)     2443 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/options.py
--rw-r--r--   0 root         (0) root         (0)     5323 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/trame_exec.py
--rw-r--r--   0 root         (0) root         (0)     4031 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/trame_state.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/jupyter.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:10.260391 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/ui/
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4188 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/ui/main.py
--rw-r--r--   0 root         (0) root         (0)     1092 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/ui/options.py
--rw-r--r--   0 root         (0) root         (0)    16375 2023-07-19 00:21:06.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/ui/ui_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:10.256391 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2648 2023-07-19 00:21:10.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1005 2023-07-19 00:21:10.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:21:10.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-19 00:21:10.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      330 2023-07-19 00:21:10.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-19 00:21:10.000000 xaitk-saliency-demo-2.2.1/xaitk_saliency_demo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 14:59:12.928939 xaitk-saliency-demo-2.2.2/
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-07-21 14:59:08.000000 xaitk-saliency-demo-2.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-21 14:59:08.000000 xaitk-saliency-demo-2.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-07-21 14:59:12.928939 xaitk-saliency-demo-2.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-07-21 14:59:08.000000 xaitk-saliency-demo-2.2.2/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-07-21 14:59:12.928939 xaitk-saliency-demo-2.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 14:59:08.000000 xaitk-saliency-demo-2.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 14:59:12.920939 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-21 14:59:08.000000 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 14:59:12.920939 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-21 14:59:08.000000 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 14:59:12.924939 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/engine/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-07-21 14:59:08.000000 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/engine/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 14:59:12.924939 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/engine/assets/
+-rw-r--r--   0 root         (0) root         (0)      498 2023-07-21 14:59:08.000000 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/engine/assets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10472 2023-07-21 14:59:08.000000 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/engine/assets/imagenet_classes.txt
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-07-21 14:59:08.000000 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/engine/main.py
+-rw-r--r--   0 root         (0) root         (0)     9702 2023-07-21 14:59:08.000000 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/engine/ml_models.py
+-rw-r--r--   0 root         (0) root         (0)     5565 2023-07-21 14:59:08.000000 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/engine/ml_xai.py
+-rw-r--r--   0 root         (0) root         (0)     2443 2023-07-21 14:59:08.000000 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/engine/options.py
+-rw-r--r--   0 root         (0) root         (0)     5323 2023-07-21 14:59:08.000000 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/engine/trame_exec.py
+-rw-r--r--   0 root         (0) root         (0)     4031 2023-07-21 14:59:08.000000 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/engine/trame_state.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-07-21 14:59:08.000000 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/jupyter.py
+-rw-r--r--   0 root         (0) root         (0)      747 2023-07-21 14:59:08.000000 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 14:59:12.924939 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/ui/
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-21 14:59:08.000000 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4188 2023-07-21 14:59:08.000000 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/ui/main.py
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-07-21 14:59:08.000000 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/ui/options.py
+-rw-r--r--   0 root         (0) root         (0)    16375 2023-07-21 14:59:08.000000 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/ui/ui_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 14:59:12.920939 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-07-21 14:59:12.000000 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-07-21 14:59:12.000000 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 14:59:12.000000 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-21 14:59:12.000000 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      352 2023-07-21 14:59:12.000000 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-21 14:59:12.000000 xaitk-saliency-demo-2.2.2/xaitk_saliency_demo.egg-info/top_level.txt
```

### Comparing `xaitk-saliency-demo-2.2.1/LICENSE` & `xaitk-saliency-demo-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.1/PKG-INFO` & `xaitk-saliency-demo-2.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xaitk-saliency-demo
-Version: 2.2.1
+Version: 2.2.2
 Summary: Web application demonstrating XAITK Saliency functionality
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `xaitk-saliency-demo-2.2.1/README.rst` & `xaitk-saliency-demo-2.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.1/setup.cfg` & `xaitk-saliency-demo-2.2.2/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = xaitk-saliency-demo
-version = 2.2.1
+version = 2.2.2
 description = Web application demonstrating XAITK Saliency functionality
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = BSD License
 classifiers = 
 	Development Status :: 5 - Production/Stable
@@ -23,16 +23,18 @@
 	Application
 	Framework
 
 [options]
 packages = find:
 include_package_data = True
 install_requires = 
-	trame>=2.1.0
+	trame>3
+	trame-vuetify
 	trame-components>=2.0.4
+	trame-plotly
 	plotly==5.15.0
 	pandas
 	
 	smqtk-classifier==0.19.0
 	smqtk-core==0.19.0
 	smqtk-dataprovider==0.18.0
 	smqtk-descriptors==0.19.0
```

### Comparing `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/assets/imagenet_classes.txt` & `xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/engine/assets/imagenet_classes.txt`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/main.py` & `xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/engine/main.py`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/ml_models.py` & `xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/engine/ml_models.py`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/ml_xai.py` & `xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/engine/ml_xai.py`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/options.py` & `xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/engine/options.py`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/trame_exec.py` & `xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/engine/trame_exec.py`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/engine/trame_state.py` & `xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/engine/trame_state.py`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/jupyter.py` & `xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/jupyter.py`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/main.py` & `xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     # Get or create server
     if server is None:
         server = get_server()
 
     if isinstance(server, str):
         server = get_server(server)
 
+    # Fix version of vue
+    server.client_type = "vue2"
+
     # CLI
     server.cli.add_argument(
         "--cpu",
         help="Force usage of CPU even if a GPU is available",
         dest="cpu",
         action="store_true",
     )
```

### Comparing `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/ui/main.py` & `xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/ui/main.py`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/ui/options.py` & `xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/ui/options.py`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo/app/ui/ui_helper.py` & `xaitk-saliency-demo-2.2.2/xaitk_saliency_demo/app/ui/ui_helper.py`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo.egg-info/PKG-INFO` & `xaitk-saliency-demo-2.2.2/xaitk_saliency_demo.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xaitk-saliency-demo
-Version: 2.2.1
+Version: 2.2.2
 Summary: Web application demonstrating XAITK Saliency functionality
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `xaitk-saliency-demo-2.2.1/xaitk_saliency_demo.egg-info/SOURCES.txt` & `xaitk-saliency-demo-2.2.2/xaitk_saliency_demo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

