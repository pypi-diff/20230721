# Comparing `tmp/botocore-a-la-carte-iotfleetwise-1.31.6.tar.gz` & `tmp/botocore-a-la-carte-iotfleetwise-1.31.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-iotfleetwise-1.31.6.tar", last modified: Thu Jul 20 01:20:22 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-iotfleetwise-1.31.8.tar", last modified: Fri Jul 21 01:21:31 2023, max compression
```

## Comparing `botocore-a-la-carte-iotfleetwise-1.31.6.tar` & `botocore-a-la-carte-iotfleetwise-1.31.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:22.134699 botocore-a-la-carte-iotfleetwise-1.31.6/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-20 01:20:21.000000 botocore-a-la-carte-iotfleetwise-1.31.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-20 01:20:22.134699 botocore-a-la-carte-iotfleetwise-1.31.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:22.134699 botocore-a-la-carte-iotfleetwise-1.31.6/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:22.134699 botocore-a-la-carte-iotfleetwise-1.31.6/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:22.134699 botocore-a-la-carte-iotfleetwise-1.31.6/botocore/data/iotfleetwise/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:22.134699 botocore-a-la-carte-iotfleetwise-1.31.6/botocore/data/iotfleetwise/2021-06-17/
--rw-r--r--   0 runner    (1001) docker     (123)    17648 2023-07-20 01:19:55.000000 botocore-a-la-carte-iotfleetwise-1.31.6/botocore/data/iotfleetwise/2021-06-17/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-20 01:19:55.000000 botocore-a-la-carte-iotfleetwise-1.31.6/botocore/data/iotfleetwise/2021-06-17/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   176179 2023-07-20 01:19:55.000000 botocore-a-la-carte-iotfleetwise-1.31.6/botocore/data/iotfleetwise/2021-06-17/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-20 01:19:55.000000 botocore-a-la-carte-iotfleetwise-1.31.6/botocore/data/iotfleetwise/2021-06-17/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:22.134699 botocore-a-la-carte-iotfleetwise-1.31.6/botocore_a_la_carte_iotfleetwise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-20 01:20:22.000000 botocore-a-la-carte-iotfleetwise-1.31.6/botocore_a_la_carte_iotfleetwise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-20 01:20:22.000000 botocore-a-la-carte-iotfleetwise-1.31.6/botocore_a_la_carte_iotfleetwise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 01:20:22.000000 botocore-a-la-carte-iotfleetwise-1.31.6/botocore_a_la_carte_iotfleetwise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 01:20:22.000000 botocore-a-la-carte-iotfleetwise-1.31.6/botocore_a_la_carte_iotfleetwise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 01:20:22.134699 botocore-a-la-carte-iotfleetwise-1.31.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-20 01:20:21.000000 botocore-a-la-carte-iotfleetwise-1.31.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:31.375106 botocore-a-la-carte-iotfleetwise-1.31.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 01:21:31.000000 botocore-a-la-carte-iotfleetwise-1.31.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-21 01:21:31.375106 botocore-a-la-carte-iotfleetwise-1.31.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:31.371106 botocore-a-la-carte-iotfleetwise-1.31.8/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:31.371106 botocore-a-la-carte-iotfleetwise-1.31.8/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:31.371106 botocore-a-la-carte-iotfleetwise-1.31.8/botocore/data/iotfleetwise/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:31.371106 botocore-a-la-carte-iotfleetwise-1.31.8/botocore/data/iotfleetwise/2021-06-17/
+-rw-r--r--   0 runner    (1001) docker     (123)    17648 2023-07-21 01:21:06.000000 botocore-a-la-carte-iotfleetwise-1.31.8/botocore/data/iotfleetwise/2021-06-17/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-21 01:21:06.000000 botocore-a-la-carte-iotfleetwise-1.31.8/botocore/data/iotfleetwise/2021-06-17/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   176179 2023-07-21 01:21:06.000000 botocore-a-la-carte-iotfleetwise-1.31.8/botocore/data/iotfleetwise/2021-06-17/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-21 01:21:06.000000 botocore-a-la-carte-iotfleetwise-1.31.8/botocore/data/iotfleetwise/2021-06-17/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:31.375106 botocore-a-la-carte-iotfleetwise-1.31.8/botocore_a_la_carte_iotfleetwise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-21 01:21:31.000000 botocore-a-la-carte-iotfleetwise-1.31.8/botocore_a_la_carte_iotfleetwise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-21 01:21:31.000000 botocore-a-la-carte-iotfleetwise-1.31.8/botocore_a_la_carte_iotfleetwise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:21:31.000000 botocore-a-la-carte-iotfleetwise-1.31.8/botocore_a_la_carte_iotfleetwise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:21:31.000000 botocore-a-la-carte-iotfleetwise-1.31.8/botocore_a_la_carte_iotfleetwise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:21:31.375106 botocore-a-la-carte-iotfleetwise-1.31.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-21 01:21:31.000000 botocore-a-la-carte-iotfleetwise-1.31.8/setup.py
```

### Comparing `botocore-a-la-carte-iotfleetwise-1.31.6/LICENSE.txt` & `botocore-a-la-carte-iotfleetwise-1.31.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-iotfleetwise-1.31.6/PKG-INFO` & `botocore-a-la-carte-iotfleetwise-1.31.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-iotfleetwise
-Version: 1.31.6
+Version: 1.31.8
 Summary: iotfleetwise data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-iotfleetwise-1.31.6/botocore/data/iotfleetwise/2021-06-17/endpoint-rule-set-1.json` & `botocore-a-la-carte-iotfleetwise-1.31.8/botocore/data/iotfleetwise/2021-06-17/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-iotfleetwise-1.31.6/botocore/data/iotfleetwise/2021-06-17/paginators-1.json` & `botocore-a-la-carte-iotfleetwise-1.31.8/botocore/data/iotfleetwise/2021-06-17/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-iotfleetwise-1.31.6/botocore/data/iotfleetwise/2021-06-17/service-2.json` & `botocore-a-la-carte-iotfleetwise-1.31.8/botocore/data/iotfleetwise/2021-06-17/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-iotfleetwise-1.31.6/botocore_a_la_carte_iotfleetwise.egg-info/PKG-INFO` & `botocore-a-la-carte-iotfleetwise-1.31.8/botocore_a_la_carte_iotfleetwise.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-iotfleetwise
-Version: 1.31.6
+Version: 1.31.8
 Summary: iotfleetwise data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-iotfleetwise-1.31.6/setup.py` & `botocore-a-la-carte-iotfleetwise-1.31.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-iotfleetwise',
-    version="1.31.6",
+    version="1.31.8",
     description='iotfleetwise data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/iotfleetwise/*/*.json'],
```

