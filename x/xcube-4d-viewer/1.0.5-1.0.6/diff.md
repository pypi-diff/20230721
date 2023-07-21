# Comparing `tmp/xcube_4d_viewer-1.0.5.tar.gz` & `tmp/xcube_4d_viewer-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcube_4d_viewer-1.0.5.tar", last modified: Fri Jul 21 10:12:47 2023, max compression
+gzip compressed data, was "xcube_4d_viewer-1.0.6.tar", last modified: Fri Jul 21 11:37:37 2023, max compression
```

## Comparing `xcube_4d_viewer-1.0.5.tar` & `xcube_4d_viewer-1.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:12:47.622701 xcube_4d_viewer-1.0.5/
--rw-r--r--   0 root         (0) root         (0)     1535 2023-07-21 10:12:45.000000 xcube_4d_viewer-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1516 2023-07-21 10:12:47.622701 xcube_4d_viewer-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5758 2023-07-21 10:12:45.000000 xcube_4d_viewer-1.0.5/README.md
--rw-r--r--   0 root         (0) root         (0)      282 2023-07-21 10:12:47.622701 xcube_4d_viewer-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1574 2023-07-21 10:12:45.000000 xcube_4d_viewer-1.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:12:47.618701 xcube_4d_viewer-1.0.5/tests/
--rw-r--r--   0 root         (0) root         (0)     5031 2023-07-21 10:12:45.000000 xcube_4d_viewer-1.0.5/tests/test_controllers.py
--rw-r--r--   0 root         (0) root         (0)     1791 2023-07-21 10:12:45.000000 xcube_4d_viewer-1.0.5/tests/test_middle_tier_registration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:12:47.622701 xcube_4d_viewer-1.0.5/xcube_4d_viewer/
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-21 10:12:45.000000 xcube_4d_viewer-1.0.5/xcube_4d_viewer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-07-21 10:12:45.000000 xcube_4d_viewer-1.0.5/xcube_4d_viewer/api.py
--rw-r--r--   0 root         (0) root         (0)      606 2023-07-21 10:12:45.000000 xcube_4d_viewer-1.0.5/xcube_4d_viewer/context.py
--rw-r--r--   0 root         (0) root         (0)    15191 2023-07-21 10:12:45.000000 xcube_4d_viewer-1.0.5/xcube_4d_viewer/controllers.py
--rw-r--r--   0 root         (0) root         (0)     2635 2023-07-21 10:12:45.000000 xcube_4d_viewer-1.0.5/xcube_4d_viewer/middle_tier_registration.py
--rw-r--r--   0 root         (0) root         (0)      454 2023-07-21 10:12:45.000000 xcube_4d_viewer-1.0.5/xcube_4d_viewer/plugin.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-07-21 10:12:45.000000 xcube_4d_viewer-1.0.5/xcube_4d_viewer/route_parameters.py
--rw-r--r--   0 root         (0) root         (0)     3079 2023-07-21 10:12:45.000000 xcube_4d_viewer-1.0.5/xcube_4d_viewer/routes.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-21 10:12:45.000000 xcube_4d_viewer-1.0.5/xcube_4d_viewer/tile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:12:47.622701 xcube_4d_viewer-1.0.5/xcube_4d_viewer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1516 2023-07-21 10:12:47.000000 xcube_4d_viewer-1.0.5/xcube_4d_viewer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      564 2023-07-21 10:12:47.000000 xcube_4d_viewer-1.0.5/xcube_4d_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 10:12:47.000000 xcube_4d_viewer-1.0.5/xcube_4d_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-07-21 10:12:47.000000 xcube_4d_viewer-1.0.5/xcube_4d_viewer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-21 10:12:47.000000 xcube_4d_viewer-1.0.5/xcube_4d_viewer.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:37:37.086606 xcube_4d_viewer-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-07-21 11:29:11.000000 xcube_4d_viewer-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1507 2023-07-21 11:37:37.086606 xcube_4d_viewer-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5758 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/README.md
+-rw-r--r--   0 root         (0) root         (0)      282 2023-07-21 11:37:37.086606 xcube_4d_viewer-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-07-21 11:29:11.000000 xcube_4d_viewer-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:37:37.086606 xcube_4d_viewer-1.0.6/tests/
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/tests/test_controllers.py
+-rw-r--r--   0 root         (0) root         (0)     1791 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/tests/test_middle_tier_registration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:37:37.086606 xcube_4d_viewer-1.0.6/xcube_4d_viewer/
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer/api.py
+-rw-r--r--   0 root         (0) root         (0)      606 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer/context.py
+-rw-r--r--   0 root         (0) root         (0)    15191 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer/controllers.py
+-rw-r--r--   0 root         (0) root         (0)     2635 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer/middle_tier_registration.py
+-rw-r--r--   0 root         (0) root         (0)      454 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer/route_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     3079 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer/routes.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer/tile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:37:37.086606 xcube_4d_viewer-1.0.6/xcube_4d_viewer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1507 2023-07-21 11:37:37.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      564 2023-07-21 11:37:37.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 11:37:37.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-21 11:37:37.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-21 11:37:37.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer.egg-info/top_level.txt
```

### Comparing `xcube_4d_viewer-1.0.5/PKG-INFO` & `xcube_4d_viewer-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: xcube_4d_viewer
-Version: 1.0.5
+Version: 1.0.6
 Summary: API extension to the xcube server allowing cubes to be viewed in the Earthwave 4D viewer.
 Home-page: https://github.com/earthwave/xcube_4d_viewer
 Author: Earthwave Ltd
 Author-email: info@earthwave.co.uk
-License: BSD-3-Clause
+License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # xcube_4d_viewer
 This repository is a plugin for the xcube server.
```

### Comparing `xcube_4d_viewer-1.0.5/README.md` & `xcube_4d_viewer-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `xcube_4d_viewer-1.0.5/setup.py` & `xcube_4d_viewer-1.0.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Earthwave Ltd',
     author_email='info@earthwave.co.uk',
     url='https://github.com/earthwave/xcube_4d_viewer',
     python_requires=">=3.9",
     packages=find_packages(),
-    license='BSD-3-Clause',
-    # note requirements listed ininstall_requires should be the *minimum required*
+    license='MIT',
+    # note requirements listed in install_requires should be the *minimum required*
     # in order to allow pip to resolve multiple installed packages properly.
     # requirements.txt should contain a specific known working version instead.
     install_requires=[
     ],
     entry_points={
         'xcube_plugins': [
             # This is xcube convention
```

### Comparing `xcube_4d_viewer-1.0.5/tests/test_controllers.py` & `xcube_4d_viewer-1.0.6/tests/test_controllers.py`

 * *Files identical despite different names*

### Comparing `xcube_4d_viewer-1.0.5/tests/test_middle_tier_registration.py` & `xcube_4d_viewer-1.0.6/tests/test_middle_tier_registration.py`

 * *Files identical despite different names*

### Comparing `xcube_4d_viewer-1.0.5/xcube_4d_viewer/api.py` & `xcube_4d_viewer-1.0.6/xcube_4d_viewer/api.py`

 * *Files identical despite different names*

### Comparing `xcube_4d_viewer-1.0.5/xcube_4d_viewer/context.py` & `xcube_4d_viewer-1.0.6/xcube_4d_viewer/context.py`

 * *Files identical despite different names*

### Comparing `xcube_4d_viewer-1.0.5/xcube_4d_viewer/controllers.py` & `xcube_4d_viewer-1.0.6/xcube_4d_viewer/controllers.py`

 * *Files identical despite different names*

### Comparing `xcube_4d_viewer-1.0.5/xcube_4d_viewer/middle_tier_registration.py` & `xcube_4d_viewer-1.0.6/xcube_4d_viewer/middle_tier_registration.py`

 * *Files identical despite different names*

### Comparing `xcube_4d_viewer-1.0.5/xcube_4d_viewer/route_parameters.py` & `xcube_4d_viewer-1.0.6/xcube_4d_viewer/route_parameters.py`

 * *Files identical despite different names*

### Comparing `xcube_4d_viewer-1.0.5/xcube_4d_viewer/routes.py` & `xcube_4d_viewer-1.0.6/xcube_4d_viewer/routes.py`

 * *Files identical despite different names*

### Comparing `xcube_4d_viewer-1.0.5/xcube_4d_viewer/tile.py` & `xcube_4d_viewer-1.0.6/xcube_4d_viewer/tile.py`

 * *Files identical despite different names*

### Comparing `xcube_4d_viewer-1.0.5/xcube_4d_viewer.egg-info/PKG-INFO` & `xcube_4d_viewer-1.0.6/xcube_4d_viewer.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: xcube-4d-viewer
-Version: 1.0.5
+Version: 1.0.6
 Summary: API extension to the xcube server allowing cubes to be viewed in the Earthwave 4D viewer.
 Home-page: https://github.com/earthwave/xcube_4d_viewer
 Author: Earthwave Ltd
 Author-email: info@earthwave.co.uk
-License: BSD-3-Clause
+License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # xcube_4d_viewer
 This repository is a plugin for the xcube server.
```

### Comparing `xcube_4d_viewer-1.0.5/xcube_4d_viewer.egg-info/SOURCES.txt` & `xcube_4d_viewer-1.0.6/xcube_4d_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

