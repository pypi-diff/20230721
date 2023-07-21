# Comparing `tmp/botocore-a-la-carte-workmailmessageflow-1.31.5.tar.gz` & `tmp/botocore-a-la-carte-workmailmessageflow-1.31.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-workmailmessageflow-1.31.5.tar", last modified: Wed Jul 19 02:44:21 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-workmailmessageflow-1.31.6.tar", last modified: Thu Jul 20 01:20:48 2023, max compression
```

## Comparing `botocore-a-la-carte-workmailmessageflow-1.31.5.tar` & `botocore-a-la-carte-workmailmessageflow-1.31.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:21.263569 botocore-a-la-carte-workmailmessageflow-1.31.5/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-19 02:44:21.000000 botocore-a-la-carte-workmailmessageflow-1.31.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-19 02:44:21.263569 botocore-a-la-carte-workmailmessageflow-1.31.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:21.263569 botocore-a-la-carte-workmailmessageflow-1.31.5/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:21.263569 botocore-a-la-carte-workmailmessageflow-1.31.5/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:21.263569 botocore-a-la-carte-workmailmessageflow-1.31.5/botocore/data/workmailmessageflow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:21.263569 botocore-a-la-carte-workmailmessageflow-1.31.5/botocore/data/workmailmessageflow/2019-05-01/
--rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-07-19 02:43:32.000000 botocore-a-la-carte-workmailmessageflow-1.31.5/botocore/data/workmailmessageflow/2019-05-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-19 02:43:32.000000 botocore-a-la-carte-workmailmessageflow-1.31.5/botocore/data/workmailmessageflow/2019-05-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-19 02:43:32.000000 botocore-a-la-carte-workmailmessageflow-1.31.5/botocore/data/workmailmessageflow/2019-05-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-07-19 02:43:32.000000 botocore-a-la-carte-workmailmessageflow-1.31.5/botocore/data/workmailmessageflow/2019-05-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:21.263569 botocore-a-la-carte-workmailmessageflow-1.31.5/botocore_a_la_carte_workmailmessageflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-19 02:44:21.000000 botocore-a-la-carte-workmailmessageflow-1.31.5/botocore_a_la_carte_workmailmessageflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-19 02:44:21.000000 botocore-a-la-carte-workmailmessageflow-1.31.5/botocore_a_la_carte_workmailmessageflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 02:44:21.000000 botocore-a-la-carte-workmailmessageflow-1.31.5/botocore_a_la_carte_workmailmessageflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 02:44:21.000000 botocore-a-la-carte-workmailmessageflow-1.31.5/botocore_a_la_carte_workmailmessageflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 02:44:21.263569 botocore-a-la-carte-workmailmessageflow-1.31.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-19 02:44:21.000000 botocore-a-la-carte-workmailmessageflow-1.31.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:48.946944 botocore-a-la-carte-workmailmessageflow-1.31.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-20 01:20:48.000000 botocore-a-la-carte-workmailmessageflow-1.31.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-20 01:20:48.946944 botocore-a-la-carte-workmailmessageflow-1.31.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:48.946944 botocore-a-la-carte-workmailmessageflow-1.31.6/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:48.946944 botocore-a-la-carte-workmailmessageflow-1.31.6/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:48.946944 botocore-a-la-carte-workmailmessageflow-1.31.6/botocore/data/workmailmessageflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:48.946944 botocore-a-la-carte-workmailmessageflow-1.31.6/botocore/data/workmailmessageflow/2019-05-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-07-20 01:19:55.000000 botocore-a-la-carte-workmailmessageflow-1.31.6/botocore/data/workmailmessageflow/2019-05-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 01:19:55.000000 botocore-a-la-carte-workmailmessageflow-1.31.6/botocore/data/workmailmessageflow/2019-05-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 01:19:55.000000 botocore-a-la-carte-workmailmessageflow-1.31.6/botocore/data/workmailmessageflow/2019-05-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-07-20 01:19:55.000000 botocore-a-la-carte-workmailmessageflow-1.31.6/botocore/data/workmailmessageflow/2019-05-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:48.946944 botocore-a-la-carte-workmailmessageflow-1.31.6/botocore_a_la_carte_workmailmessageflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-20 01:20:48.000000 botocore-a-la-carte-workmailmessageflow-1.31.6/botocore_a_la_carte_workmailmessageflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-20 01:20:48.000000 botocore-a-la-carte-workmailmessageflow-1.31.6/botocore_a_la_carte_workmailmessageflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 01:20:48.000000 botocore-a-la-carte-workmailmessageflow-1.31.6/botocore_a_la_carte_workmailmessageflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 01:20:48.000000 botocore-a-la-carte-workmailmessageflow-1.31.6/botocore_a_la_carte_workmailmessageflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 01:20:48.946944 botocore-a-la-carte-workmailmessageflow-1.31.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-20 01:20:48.000000 botocore-a-la-carte-workmailmessageflow-1.31.6/setup.py
```

### Comparing `botocore-a-la-carte-workmailmessageflow-1.31.5/LICENSE.txt` & `botocore-a-la-carte-workmailmessageflow-1.31.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-workmailmessageflow-1.31.5/PKG-INFO` & `botocore-a-la-carte-workmailmessageflow-1.31.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-workmailmessageflow
-Version: 1.31.5
+Version: 1.31.6
 Summary: workmailmessageflow data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-workmailmessageflow-1.31.5/botocore/data/workmailmessageflow/2019-05-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-workmailmessageflow-1.31.6/botocore/data/workmailmessageflow/2019-05-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-workmailmessageflow-1.31.5/botocore/data/workmailmessageflow/2019-05-01/service-2.json` & `botocore-a-la-carte-workmailmessageflow-1.31.6/botocore/data/workmailmessageflow/2019-05-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-workmailmessageflow-1.31.5/botocore_a_la_carte_workmailmessageflow.egg-info/PKG-INFO` & `botocore-a-la-carte-workmailmessageflow-1.31.6/botocore_a_la_carte_workmailmessageflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-workmailmessageflow
-Version: 1.31.5
+Version: 1.31.6
 Summary: workmailmessageflow data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-workmailmessageflow-1.31.5/botocore_a_la_carte_workmailmessageflow.egg-info/SOURCES.txt` & `botocore-a-la-carte-workmailmessageflow-1.31.6/botocore_a_la_carte_workmailmessageflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-workmailmessageflow-1.31.5/setup.py` & `botocore-a-la-carte-workmailmessageflow-1.31.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-workmailmessageflow',
-    version="1.31.5",
+    version="1.31.6",
     description='workmailmessageflow data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/workmailmessageflow/*/*.json'],
```

