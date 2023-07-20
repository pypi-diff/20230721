# Comparing `tmp/dagster-census-0.19.9rc0.tar.gz` & `tmp/dagster-census-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-census-0.19.9rc0.tar", last modified: Thu Jun  8 18:27:58 2023, max compression
+gzip compressed data, was "dagster-census-0.20.0.tar", last modified: Thu Jul 20 22:00:58 2023, max compression
```

## Comparing `dagster-census-0.19.9rc0.tar` & `dagster-census-0.20.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:58.146390 dagster-census-0.19.9rc0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-census-0.19.9rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-08 18:20:46.000000 dagster-census-0.19.9rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      671 2023-06-08 18:27:58.146390 dagster-census-0.19.9rc0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:58.146390 dagster-census-0.19.9rc0/dagster_census/
--rw-r--r--   0 root         (0) root         (0)      394 2023-06-08 18:20:46.000000 dagster-census-0.19.9rc0/dagster_census/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3551 2023-06-08 18:20:46.000000 dagster-census-0.19.9rc0/dagster_census/ops.py
--rw-r--r--   0 root         (0) root         (0)    10169 2023-06-08 18:20:46.000000 dagster-census-0.19.9rc0/dagster_census/resources.py
--rw-r--r--   0 root         (0) root         (0)      677 2023-06-08 18:20:46.000000 dagster-census-0.19.9rc0/dagster_census/types.py
--rw-r--r--   0 root         (0) root         (0)     1325 2023-06-08 18:20:46.000000 dagster-census-0.19.9rc0/dagster_census/utils.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-census-0.19.9rc0/dagster_census/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:58.146390 dagster-census-0.19.9rc0/dagster_census.egg-info/
--rw-r--r--   0 root         (0) root         (0)      671 2023-06-08 18:27:58.000000 dagster-census-0.19.9rc0/dagster_census.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-08 18:27:58.000000 dagster-census-0.19.9rc0/dagster_census.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:27:58.000000 dagster-census-0.19.9rc0/dagster_census.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:27:58.000000 dagster-census-0.19.9rc0/dagster_census.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-08 18:27:58.000000 dagster-census-0.19.9rc0/dagster_census.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-08 18:27:58.000000 dagster-census-0.19.9rc0/dagster_census.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      161 2023-06-08 18:27:58.146390 dagster-census-0.19.9rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1251 2023-06-08 18:20:46.000000 dagster-census-0.19.9rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:00:58.613170 dagster-census-0.20.0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-20 21:53:16.000000 dagster-census-0.20.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       34 2023-07-20 21:53:16.000000 dagster-census-0.20.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      618 2023-07-20 22:00:58.613170 dagster-census-0.20.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:00:58.609170 dagster-census-0.20.0/dagster_census/
+-rw-r--r--   0 root         (0) root         (0)      394 2023-07-20 21:53:16.000000 dagster-census-0.20.0/dagster_census/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3551 2023-07-20 21:53:16.000000 dagster-census-0.20.0/dagster_census/ops.py
+-rw-r--r--   0 root         (0) root         (0)    10284 2023-07-20 21:53:16.000000 dagster-census-0.20.0/dagster_census/resources.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-07-20 21:53:16.000000 dagster-census-0.20.0/dagster_census/types.py
+-rw-r--r--   0 root         (0) root         (0)     1325 2023-07-20 21:53:16.000000 dagster-census-0.20.0/dagster_census/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-census-0.20.0/dagster_census/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:00:58.613170 dagster-census-0.20.0/dagster_census.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      618 2023-07-20 22:00:58.000000 dagster-census-0.20.0/dagster_census.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      415 2023-07-20 22:00:58.000000 dagster-census-0.20.0/dagster_census.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:00:58.000000 dagster-census-0.20.0/dagster_census.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:00:58.000000 dagster-census-0.20.0/dagster_census.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-20 22:00:58.000000 dagster-census-0.20.0/dagster_census.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-20 22:00:58.000000 dagster-census-0.20.0/dagster_census.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2023-07-20 22:00:58.613170 dagster-census-0.20.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-07-20 21:53:16.000000 dagster-census-0.20.0/setup.py
```

### Comparing `dagster-census-0.19.9rc0/LICENSE` & `dagster-census-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-census-0.19.9rc0/PKG-INFO` & `dagster-census-0.20.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-census
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for integrating Census with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-census
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
```

### Comparing `dagster-census-0.19.9rc0/dagster_census/ops.py` & `dagster-census-0.20.0/dagster_census/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-census-0.19.9rc0/dagster_census/resources.py` & `dagster-census-0.20.0/dagster_census/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import logging
 import time
 from typing import Any, Mapping, Optional
 
 import requests
 from dagster import Failure, Field, StringSource, __version__, get_dagster_logger, resource
+from dagster._core.definitions.resource_definition import dagster_maintained_resource
 from requests.auth import HTTPBasicAuth
 from requests.exceptions import RequestException
 
 from .types import CensusOutput
 
 CENSUS_API_BASE = "app.getcensus.com/api"
 CENSUS_VERSION = "v1"
@@ -234,14 +235,15 @@
         return CensusOutput(
             sync_run=sync_run_details,
             source=source_details,
             destination=destination_details,
         )
 
 
+@dagster_maintained_resource
 @resource(
     config_schema={
         "api_key": Field(
             StringSource,
             is_required=True,
             description="Census API Key.",
         ),
```

### Comparing `dagster-census-0.19.9rc0/dagster_census/types.py` & `dagster-census-0.20.0/dagster_census/types.py`

 * *Files identical despite different names*

### Comparing `dagster-census-0.19.9rc0/dagster_census/utils.py` & `dagster-census-0.20.0/dagster_census/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-census-0.19.9rc0/dagster_census.egg-info/PKG-INFO` & `dagster-census-0.20.0/dagster_census.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-census
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for integrating Census with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-census
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
```

### Comparing `dagster-census-0.19.9rc0/setup.py` & `dagster-census-0.20.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,19 +20,18 @@
     version=ver,
     author="Elementl",
     author_email="hello@elementl.com",
     license="Apache-2.0",
     description="Package for integrating Census with Dagster.",
     url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-census",
     classifiers=[
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_census_tests*"]),
-    install_requires=["dagster==1.3.9rc0"],
+    install_requires=["dagster==1.4.0"],
     zip_safe=False,
 )
```

