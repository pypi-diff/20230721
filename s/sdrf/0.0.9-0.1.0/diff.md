# Comparing `tmp/sdrf-0.0.9.tar.gz` & `tmp/sdrf-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdrf-0.0.9.tar", last modified: Fri Jul 21 12:30:25 2023, max compression
+gzip compressed data, was "sdrf-0.1.0.tar", last modified: Fri Jul 21 13:24:20 2023, max compression
```

## Comparing `sdrf-0.0.9.tar` & `sdrf-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:30:25.567203 sdrf-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-21 12:30:15.000000 sdrf-0.0.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-07-21 12:30:25.567203 sdrf-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-07-21 12:30:15.000000 sdrf-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-21 12:30:15.000000 sdrf-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 12:30:25.567203 sdrf-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-21 12:30:15.000000 sdrf-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:30:25.563203 sdrf-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:30:25.563203 sdrf-0.0.9/src/sdrf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:30:15.000000 sdrf-0.0.9/src/sdrf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-21 12:30:15.000000 sdrf-0.0.9/src/sdrf/api_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-21 12:30:15.000000 sdrf-0.0.9/src/sdrf/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-07-21 12:30:15.000000 sdrf-0.0.9/src/sdrf/endpoint_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:30:25.567203 sdrf-0.0.9/src/sdrf/enums/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-21 12:30:15.000000 sdrf-0.0.9/src/sdrf/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-21 12:30:15.000000 sdrf-0.0.9/src/sdrf/enums/api_data_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-21 12:30:15.000000 sdrf-0.0.9/src/sdrf/enums/parameter_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-21 12:30:15.000000 sdrf-0.0.9/src/sdrf/model_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-21 12:30:15.000000 sdrf-0.0.9/src/sdrf/swagger_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-21 12:30:15.000000 sdrf-0.0.9/src/sdrf/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:30:25.567203 sdrf-0.0.9/src/sdrf/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-21 12:30:15.000000 sdrf-0.0.9/src/sdrf/utils/settings_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:30:25.567203 sdrf-0.0.9/src/sdrf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-07-21 12:30:25.000000 sdrf-0.0.9/src/sdrf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-21 12:30:25.000000 sdrf-0.0.9/src/sdrf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:30:25.000000 sdrf-0.0.9/src/sdrf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-21 12:30:25.000000 sdrf-0.0.9/src/sdrf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 12:30:25.000000 sdrf-0.0.9/src/sdrf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:24:20.012288 sdrf-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-21 13:24:05.000000 sdrf-0.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-07-21 13:24:20.008288 sdrf-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-07-21 13:24:05.000000 sdrf-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-21 13:24:05.000000 sdrf-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 13:24:20.012288 sdrf-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-21 13:24:05.000000 sdrf-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:24:20.004288 sdrf-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:24:20.008288 sdrf-0.1.0/src/sdrf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:24:05.000000 sdrf-0.1.0/src/sdrf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-21 13:24:05.000000 sdrf-0.1.0/src/sdrf/api_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-21 13:24:05.000000 sdrf-0.1.0/src/sdrf/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-07-21 13:24:05.000000 sdrf-0.1.0/src/sdrf/endpoint_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:24:20.008288 sdrf-0.1.0/src/sdrf/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-21 13:24:05.000000 sdrf-0.1.0/src/sdrf/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-21 13:24:05.000000 sdrf-0.1.0/src/sdrf/enums/api_data_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-21 13:24:05.000000 sdrf-0.1.0/src/sdrf/enums/parameter_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-21 13:24:05.000000 sdrf-0.1.0/src/sdrf/model_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-21 13:24:05.000000 sdrf-0.1.0/src/sdrf/swagger_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-21 13:24:05.000000 sdrf-0.1.0/src/sdrf/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:24:20.008288 sdrf-0.1.0/src/sdrf/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-21 13:24:05.000000 sdrf-0.1.0/src/sdrf/utils/settings_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:24:20.008288 sdrf-0.1.0/src/sdrf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-07-21 13:24:19.000000 sdrf-0.1.0/src/sdrf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-21 13:24:20.000000 sdrf-0.1.0/src/sdrf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:24:19.000000 sdrf-0.1.0/src/sdrf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-21 13:24:19.000000 sdrf-0.1.0/src/sdrf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 13:24:19.000000 sdrf-0.1.0/src/sdrf.egg-info/top_level.txt
```

### Comparing `sdrf-0.0.9/LICENSE.txt` & `sdrf-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sdrf-0.0.9/PKG-INFO` & `sdrf-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdrf
-Version: 0.0.9
+Version: 0.1.0
 Summary: Simple rest framework is an abstraction for building rest api with well written documentations
 Home-page: https://github.com/hus201/sdrf
 Author: Hussein Anabtawi
 Author-email: Hussein Anabtawi <husainanabtawi2001@hotmail.com>
 Project-URL: Homepage, https://github.com/hus201/sdrf
 Project-URL: Bug Tracker, https://github.com/hus201/sdrf/issues
 Keywords: django,rest apis,abstraction
```

### Comparing `sdrf-0.0.9/README.md` & `sdrf-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sdrf-0.0.9/pyproject.toml` & `sdrf-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sdrf"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Hussein Anabtawi", email="husainanabtawi2001@hotmail.com" },
 ]
 description = "Simple rest framework is an abstraction for building rest api with well written documentations"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sdrf-0.0.9/setup.py` & `sdrf-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='sdrf',
-    version='0.0.9',
+    version='0.1.0',
     author='Hussein Anabtawi',
     description='Simple rest framework an abstraction that combines django rest framework with drf_yasg ',
     long_description='Simple rest framework is an abstraction for building rest api with well written documentations ',
     url='https://github.com/hus201/sdrf',
     keywords='django, rest apis, abstraction',
     python_requires='>=3.8, <4',
     install_requires=[
```

### Comparing `sdrf-0.0.9/src/sdrf/api_endpoint.py` & `sdrf-0.1.0/src/sdrf/api_endpoint.py`

 * *Files identical despite different names*

### Comparing `sdrf-0.0.9/src/sdrf/endpoint_config.py` & `sdrf-0.1.0/src/sdrf/endpoint_config.py`

 * *Files identical despite different names*

### Comparing `sdrf-0.0.9/src/sdrf/model_endpoint.py` & `sdrf-0.1.0/src/sdrf/model_endpoint.py`

 * *Files identical despite different names*

### Comparing `sdrf-0.0.9/src/sdrf/swagger_config.py` & `sdrf-0.1.0/src/sdrf/swagger_config.py`

 * *Files identical despite different names*

### Comparing `sdrf-0.0.9/src/sdrf.egg-info/PKG-INFO` & `sdrf-0.1.0/src/sdrf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdrf
-Version: 0.0.9
+Version: 0.1.0
 Summary: Simple rest framework is an abstraction for building rest api with well written documentations
 Home-page: https://github.com/hus201/sdrf
 Author: Hussein Anabtawi
 Author-email: Hussein Anabtawi <husainanabtawi2001@hotmail.com>
 Project-URL: Homepage, https://github.com/hus201/sdrf
 Project-URL: Bug Tracker, https://github.com/hus201/sdrf/issues
 Keywords: django,rest apis,abstraction
```

