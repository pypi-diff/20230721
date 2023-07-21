# Comparing `tmp/xcube_4d_viewer-1.0.6.tar.gz` & `tmp/xcube_4d_viewer-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcube_4d_viewer-1.0.6.tar", last modified: Fri Jul 21 11:37:37 2023, max compression
+gzip compressed data, was "xcube_4d_viewer-1.0.7.tar", last modified: Fri Jul 21 14:15:39 2023, max compression
```

## Comparing `xcube_4d_viewer-1.0.6.tar` & `xcube_4d_viewer-1.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:37:37.086606 xcube_4d_viewer-1.0.6/
--rw-r--r--   0 root         (0) root         (0)     1061 2023-07-21 11:29:11.000000 xcube_4d_viewer-1.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1507 2023-07-21 11:37:37.086606 xcube_4d_viewer-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5758 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/README.md
--rw-r--r--   0 root         (0) root         (0)      282 2023-07-21 11:37:37.086606 xcube_4d_viewer-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1566 2023-07-21 11:29:11.000000 xcube_4d_viewer-1.0.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:37:37.086606 xcube_4d_viewer-1.0.6/tests/
--rw-r--r--   0 root         (0) root         (0)     5031 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/tests/test_controllers.py
--rw-r--r--   0 root         (0) root         (0)     1791 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/tests/test_middle_tier_registration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:37:37.086606 xcube_4d_viewer-1.0.6/xcube_4d_viewer/
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer/api.py
--rw-r--r--   0 root         (0) root         (0)      606 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer/context.py
--rw-r--r--   0 root         (0) root         (0)    15191 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer/controllers.py
--rw-r--r--   0 root         (0) root         (0)     2635 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer/middle_tier_registration.py
--rw-r--r--   0 root         (0) root         (0)      454 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer/plugin.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer/route_parameters.py
--rw-r--r--   0 root         (0) root         (0)     3079 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer/routes.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-21 09:55:33.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer/tile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:37:37.086606 xcube_4d_viewer-1.0.6/xcube_4d_viewer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1507 2023-07-21 11:37:37.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      564 2023-07-21 11:37:37.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 11:37:37.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-07-21 11:37:37.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-21 11:37:37.000000 xcube_4d_viewer-1.0.6/xcube_4d_viewer.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 14:15:39.304958 xcube_4d_viewer-1.0.7/
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-07-21 14:15:37.000000 xcube_4d_viewer-1.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-07-21 14:15:39.304958 xcube_4d_viewer-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1376 2023-07-21 14:15:37.000000 xcube_4d_viewer-1.0.7/README.md
+-rw-r--r--   0 root         (0) root         (0)      282 2023-07-21 14:15:39.304958 xcube_4d_viewer-1.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-07-21 14:15:37.000000 xcube_4d_viewer-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 14:15:39.304958 xcube_4d_viewer-1.0.7/tests/
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-07-21 14:15:37.000000 xcube_4d_viewer-1.0.7/tests/test_controllers.py
+-rw-r--r--   0 root         (0) root         (0)     1791 2023-07-21 14:15:37.000000 xcube_4d_viewer-1.0.7/tests/test_middle_tier_registration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 14:15:39.304958 xcube_4d_viewer-1.0.7/xcube_4d_viewer/
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-21 14:15:37.000000 xcube_4d_viewer-1.0.7/xcube_4d_viewer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-07-21 14:15:37.000000 xcube_4d_viewer-1.0.7/xcube_4d_viewer/api.py
+-rw-r--r--   0 root         (0) root         (0)      606 2023-07-21 14:15:37.000000 xcube_4d_viewer-1.0.7/xcube_4d_viewer/context.py
+-rw-r--r--   0 root         (0) root         (0)    15191 2023-07-21 14:15:37.000000 xcube_4d_viewer-1.0.7/xcube_4d_viewer/controllers.py
+-rw-r--r--   0 root         (0) root         (0)     2635 2023-07-21 14:15:37.000000 xcube_4d_viewer-1.0.7/xcube_4d_viewer/middle_tier_registration.py
+-rw-r--r--   0 root         (0) root         (0)      454 2023-07-21 14:15:37.000000 xcube_4d_viewer-1.0.7/xcube_4d_viewer/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-07-21 14:15:37.000000 xcube_4d_viewer-1.0.7/xcube_4d_viewer/route_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     3079 2023-07-21 14:15:37.000000 xcube_4d_viewer-1.0.7/xcube_4d_viewer/routes.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-21 14:15:37.000000 xcube_4d_viewer-1.0.7/xcube_4d_viewer/tile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 14:15:39.304958 xcube_4d_viewer-1.0.7/xcube_4d_viewer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-07-21 14:15:39.000000 xcube_4d_viewer-1.0.7/xcube_4d_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      564 2023-07-21 14:15:39.000000 xcube_4d_viewer-1.0.7/xcube_4d_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 14:15:39.000000 xcube_4d_viewer-1.0.7/xcube_4d_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-21 14:15:39.000000 xcube_4d_viewer-1.0.7/xcube_4d_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-21 14:15:39.000000 xcube_4d_viewer-1.0.7/xcube_4d_viewer.egg-info/top_level.txt
```

### Comparing `xcube_4d_viewer-1.0.6/LICENSE` & `xcube_4d_viewer-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xcube_4d_viewer-1.0.6/PKG-INFO` & `xcube_4d_viewer-1.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: xcube_4d_viewer
-Version: 1.0.6
+Version: 1.0.7
 Summary: API extension to the xcube server allowing cubes to be viewed in the Earthwave 4D viewer.
 Home-page: https://github.com/earthwave/xcube_4d_viewer
 Author: Earthwave Ltd
 Author-email: info@earthwave.co.uk
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![example workflow](https://github.com/earthwave/xcube_4d_viewer/actions/workflows/xcube_4d_viewer_test.yml/badge.svg)
+![example workflow](https://github.com/earthwave/xcube_4d_viewer/actions/workflows/xcube_4d_viewer_deploy.yml/badge.svg)
 # xcube_4d_viewer
 This repository is a plugin for the xcube server.
 
 xcube (https://xcube.readthedocs.io/en/latest/overview.html) is a Python package for generating and exploiting data
-cubes powered by xarray, dask, and zarrP. It also provides a web API and server which can be used to access and
+cubes powered by xarray, dask, and zarr. It also provides a web API and server which can be used to access and
 visualise these data cubes.
 
 This repository serves as an API extension to the xcube server, allowing xcube data cubes to be analysed and
 visualised within Earthwave's 4D viewer. It computes configuration details and
 heatmap/3D heatmap/terrain tiles from the server's data cubes and provides them in a format expected by the 4D viewer.
 
 To make use of the API, a new MiddleTierURL key should be set in the xcube server config file. Please contact support@earthwave.co.uk for the current URL of the Middle Tier service.
```

### Comparing `xcube_4d_viewer-1.0.6/setup.py` & `xcube_4d_viewer-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Setup file for xcube_4d_viewer."""
 import os
 
 from setuptools import find_packages
 from setuptools import setup
 
-with open("PUBLIC_README.md", "r", encoding="utf-8") as fh:
+with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 if os.path.exists("full_version.txt"):
     with open("full_version.txt", "r", encoding="utf-8") as fh:
         """
         Note that this file is generated by the CI chain based on the git tag
         (by ew_continuous_integration/define_new_version_number.py)
```

### Comparing `xcube_4d_viewer-1.0.6/tests/test_controllers.py` & `xcube_4d_viewer-1.0.7/tests/test_controllers.py`

 * *Files identical despite different names*

### Comparing `xcube_4d_viewer-1.0.6/tests/test_middle_tier_registration.py` & `xcube_4d_viewer-1.0.7/tests/test_middle_tier_registration.py`

 * *Files identical despite different names*

### Comparing `xcube_4d_viewer-1.0.6/xcube_4d_viewer/api.py` & `xcube_4d_viewer-1.0.7/xcube_4d_viewer/api.py`

 * *Files identical despite different names*

### Comparing `xcube_4d_viewer-1.0.6/xcube_4d_viewer/context.py` & `xcube_4d_viewer-1.0.7/xcube_4d_viewer/context.py`

 * *Files identical despite different names*

### Comparing `xcube_4d_viewer-1.0.6/xcube_4d_viewer/controllers.py` & `xcube_4d_viewer-1.0.7/xcube_4d_viewer/controllers.py`

 * *Files identical despite different names*

### Comparing `xcube_4d_viewer-1.0.6/xcube_4d_viewer/middle_tier_registration.py` & `xcube_4d_viewer-1.0.7/xcube_4d_viewer/middle_tier_registration.py`

 * *Files identical despite different names*

### Comparing `xcube_4d_viewer-1.0.6/xcube_4d_viewer/route_parameters.py` & `xcube_4d_viewer-1.0.7/xcube_4d_viewer/route_parameters.py`

 * *Files identical despite different names*

### Comparing `xcube_4d_viewer-1.0.6/xcube_4d_viewer/routes.py` & `xcube_4d_viewer-1.0.7/xcube_4d_viewer/routes.py`

 * *Files identical despite different names*

### Comparing `xcube_4d_viewer-1.0.6/xcube_4d_viewer/tile.py` & `xcube_4d_viewer-1.0.7/xcube_4d_viewer/tile.py`

 * *Files identical despite different names*

### Comparing `xcube_4d_viewer-1.0.6/xcube_4d_viewer.egg-info/PKG-INFO` & `xcube_4d_viewer-1.0.7/xcube_4d_viewer.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: xcube-4d-viewer
-Version: 1.0.6
+Version: 1.0.7
 Summary: API extension to the xcube server allowing cubes to be viewed in the Earthwave 4D viewer.
 Home-page: https://github.com/earthwave/xcube_4d_viewer
 Author: Earthwave Ltd
 Author-email: info@earthwave.co.uk
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![example workflow](https://github.com/earthwave/xcube_4d_viewer/actions/workflows/xcube_4d_viewer_test.yml/badge.svg)
+![example workflow](https://github.com/earthwave/xcube_4d_viewer/actions/workflows/xcube_4d_viewer_deploy.yml/badge.svg)
 # xcube_4d_viewer
 This repository is a plugin for the xcube server.
 
 xcube (https://xcube.readthedocs.io/en/latest/overview.html) is a Python package for generating and exploiting data
-cubes powered by xarray, dask, and zarrP. It also provides a web API and server which can be used to access and
+cubes powered by xarray, dask, and zarr. It also provides a web API and server which can be used to access and
 visualise these data cubes.
 
 This repository serves as an API extension to the xcube server, allowing xcube data cubes to be analysed and
 visualised within Earthwave's 4D viewer. It computes configuration details and
 heatmap/3D heatmap/terrain tiles from the server's data cubes and provides them in a format expected by the 4D viewer.
 
 To make use of the API, a new MiddleTierURL key should be set in the xcube server config file. Please contact support@earthwave.co.uk for the current URL of the Middle Tier service.
```

### Comparing `xcube_4d_viewer-1.0.6/xcube_4d_viewer.egg-info/SOURCES.txt` & `xcube_4d_viewer-1.0.7/xcube_4d_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

