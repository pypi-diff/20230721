# Comparing `tmp/botocore-a-la-carte-appflow-1.31.6.tar.gz` & `tmp/botocore-a-la-carte-appflow-1.31.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-appflow-1.31.6.tar", last modified: Thu Jul 20 01:20:05 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-appflow-1.31.8.tar", last modified: Fri Jul 21 01:21:14 2023, max compression
```

## Comparing `botocore-a-la-carte-appflow-1.31.6.tar` & `botocore-a-la-carte-appflow-1.31.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:05.982566 botocore-a-la-carte-appflow-1.31.6/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-20 01:20:05.000000 botocore-a-la-carte-appflow-1.31.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-20 01:20:05.982566 botocore-a-la-carte-appflow-1.31.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:05.978566 botocore-a-la-carte-appflow-1.31.6/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:05.978566 botocore-a-la-carte-appflow-1.31.6/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:05.978566 botocore-a-la-carte-appflow-1.31.6/botocore/data/appflow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:05.978566 botocore-a-la-carte-appflow-1.31.6/botocore/data/appflow/2020-08-23/
--rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-07-20 01:19:55.000000 botocore-a-la-carte-appflow-1.31.6/botocore/data/appflow/2020-08-23/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 01:19:55.000000 botocore-a-la-carte-appflow-1.31.6/botocore/data/appflow/2020-08-23/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 01:19:55.000000 botocore-a-la-carte-appflow-1.31.6/botocore/data/appflow/2020-08-23/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   233245 2023-07-20 01:19:55.000000 botocore-a-la-carte-appflow-1.31.6/botocore/data/appflow/2020-08-23/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:05.982566 botocore-a-la-carte-appflow-1.31.6/botocore_a_la_carte_appflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-20 01:20:05.000000 botocore-a-la-carte-appflow-1.31.6/botocore_a_la_carte_appflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-20 01:20:05.000000 botocore-a-la-carte-appflow-1.31.6/botocore_a_la_carte_appflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 01:20:05.000000 botocore-a-la-carte-appflow-1.31.6/botocore_a_la_carte_appflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 01:20:05.000000 botocore-a-la-carte-appflow-1.31.6/botocore_a_la_carte_appflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 01:20:05.982566 botocore-a-la-carte-appflow-1.31.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-20 01:20:05.000000 botocore-a-la-carte-appflow-1.31.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:14.414797 botocore-a-la-carte-appflow-1.31.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 01:21:14.000000 botocore-a-la-carte-appflow-1.31.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-21 01:21:14.414797 botocore-a-la-carte-appflow-1.31.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:14.414797 botocore-a-la-carte-appflow-1.31.8/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:14.414797 botocore-a-la-carte-appflow-1.31.8/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:14.414797 botocore-a-la-carte-appflow-1.31.8/botocore/data/appflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:14.414797 botocore-a-la-carte-appflow-1.31.8/botocore/data/appflow/2020-08-23/
+-rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-07-21 01:21:06.000000 botocore-a-la-carte-appflow-1.31.8/botocore/data/appflow/2020-08-23/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 01:21:06.000000 botocore-a-la-carte-appflow-1.31.8/botocore/data/appflow/2020-08-23/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 01:21:06.000000 botocore-a-la-carte-appflow-1.31.8/botocore/data/appflow/2020-08-23/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   233245 2023-07-21 01:21:06.000000 botocore-a-la-carte-appflow-1.31.8/botocore/data/appflow/2020-08-23/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:14.414797 botocore-a-la-carte-appflow-1.31.8/botocore_a_la_carte_appflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-21 01:21:14.000000 botocore-a-la-carte-appflow-1.31.8/botocore_a_la_carte_appflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-21 01:21:14.000000 botocore-a-la-carte-appflow-1.31.8/botocore_a_la_carte_appflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:21:14.000000 botocore-a-la-carte-appflow-1.31.8/botocore_a_la_carte_appflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:21:14.000000 botocore-a-la-carte-appflow-1.31.8/botocore_a_la_carte_appflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:21:14.414797 botocore-a-la-carte-appflow-1.31.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-21 01:21:14.000000 botocore-a-la-carte-appflow-1.31.8/setup.py
```

### Comparing `botocore-a-la-carte-appflow-1.31.6/LICENSE.txt` & `botocore-a-la-carte-appflow-1.31.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-appflow-1.31.6/PKG-INFO` & `botocore-a-la-carte-appflow-1.31.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-appflow
-Version: 1.31.6
+Version: 1.31.8
 Summary: appflow data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-appflow-1.31.6/botocore/data/appflow/2020-08-23/endpoint-rule-set-1.json` & `botocore-a-la-carte-appflow-1.31.8/botocore/data/appflow/2020-08-23/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-appflow-1.31.6/botocore/data/appflow/2020-08-23/service-2.json` & `botocore-a-la-carte-appflow-1.31.8/botocore/data/appflow/2020-08-23/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-appflow-1.31.6/botocore_a_la_carte_appflow.egg-info/PKG-INFO` & `botocore-a-la-carte-appflow-1.31.8/botocore_a_la_carte_appflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-appflow
-Version: 1.31.6
+Version: 1.31.8
 Summary: appflow data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-appflow-1.31.6/setup.py` & `botocore-a-la-carte-appflow-1.31.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-appflow',
-    version="1.31.6",
+    version="1.31.8",
     description='appflow data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/appflow/*/*.json'],
```

