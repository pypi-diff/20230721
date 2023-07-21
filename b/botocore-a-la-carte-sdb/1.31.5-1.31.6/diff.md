# Comparing `tmp/botocore-a-la-carte-sdb-1.31.5.tar.gz` & `tmp/botocore-a-la-carte-sdb-1.31.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-sdb-1.31.5.tar", last modified: Wed Jul 19 02:44:18 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-sdb-1.31.6.tar", last modified: Thu Jul 20 01:20:46 2023, max compression
```

## Comparing `botocore-a-la-carte-sdb-1.31.5.tar` & `botocore-a-la-carte-sdb-1.31.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:18.559571 botocore-a-la-carte-sdb-1.31.5/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-19 02:44:18.000000 botocore-a-la-carte-sdb-1.31.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-19 02:44:18.559571 botocore-a-la-carte-sdb-1.31.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:18.559571 botocore-a-la-carte-sdb-1.31.5/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:18.559571 botocore-a-la-carte-sdb-1.31.5/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:18.559571 botocore-a-la-carte-sdb-1.31.5/botocore/data/sdb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:18.559571 botocore-a-la-carte-sdb-1.31.5/botocore/data/sdb/2009-04-15/
--rw-r--r--   0 runner    (1001) docker     (123)    14172 2023-07-19 02:43:32.000000 botocore-a-la-carte-sdb-1.31.5/botocore/data/sdb/2009-04-15/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-19 02:43:32.000000 botocore-a-la-carte-sdb-1.31.5/botocore/data/sdb/2009-04-15/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    44405 2023-07-19 02:43:32.000000 botocore-a-la-carte-sdb-1.31.5/botocore/data/sdb/2009-04-15/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:18.559571 botocore-a-la-carte-sdb-1.31.5/botocore_a_la_carte_sdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-19 02:44:18.000000 botocore-a-la-carte-sdb-1.31.5/botocore_a_la_carte_sdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-19 02:44:18.000000 botocore-a-la-carte-sdb-1.31.5/botocore_a_la_carte_sdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 02:44:18.000000 botocore-a-la-carte-sdb-1.31.5/botocore_a_la_carte_sdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 02:44:18.000000 botocore-a-la-carte-sdb-1.31.5/botocore_a_la_carte_sdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 02:44:18.559571 botocore-a-la-carte-sdb-1.31.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-19 02:44:18.000000 botocore-a-la-carte-sdb-1.31.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:46.862929 botocore-a-la-carte-sdb-1.31.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-20 01:20:46.000000 botocore-a-la-carte-sdb-1.31.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-20 01:20:46.862929 botocore-a-la-carte-sdb-1.31.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:46.862929 botocore-a-la-carte-sdb-1.31.6/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:46.862929 botocore-a-la-carte-sdb-1.31.6/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:46.862929 botocore-a-la-carte-sdb-1.31.6/botocore/data/sdb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:46.862929 botocore-a-la-carte-sdb-1.31.6/botocore/data/sdb/2009-04-15/
+-rw-r--r--   0 runner    (1001) docker     (123)    14172 2023-07-20 01:19:55.000000 botocore-a-la-carte-sdb-1.31.6/botocore/data/sdb/2009-04-15/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 01:19:55.000000 botocore-a-la-carte-sdb-1.31.6/botocore/data/sdb/2009-04-15/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    44405 2023-07-20 01:19:55.000000 botocore-a-la-carte-sdb-1.31.6/botocore/data/sdb/2009-04-15/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:46.862929 botocore-a-la-carte-sdb-1.31.6/botocore_a_la_carte_sdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-20 01:20:46.000000 botocore-a-la-carte-sdb-1.31.6/botocore_a_la_carte_sdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-20 01:20:46.000000 botocore-a-la-carte-sdb-1.31.6/botocore_a_la_carte_sdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 01:20:46.000000 botocore-a-la-carte-sdb-1.31.6/botocore_a_la_carte_sdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 01:20:46.000000 botocore-a-la-carte-sdb-1.31.6/botocore_a_la_carte_sdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 01:20:46.862929 botocore-a-la-carte-sdb-1.31.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-20 01:20:46.000000 botocore-a-la-carte-sdb-1.31.6/setup.py
```

### Comparing `botocore-a-la-carte-sdb-1.31.5/LICENSE.txt` & `botocore-a-la-carte-sdb-1.31.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-sdb-1.31.5/PKG-INFO` & `botocore-a-la-carte-sdb-1.31.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-sdb
-Version: 1.31.5
+Version: 1.31.6
 Summary: sdb data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-sdb-1.31.5/botocore/data/sdb/2009-04-15/endpoint-rule-set-1.json` & `botocore-a-la-carte-sdb-1.31.6/botocore/data/sdb/2009-04-15/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-sdb-1.31.5/botocore/data/sdb/2009-04-15/service-2.json` & `botocore-a-la-carte-sdb-1.31.6/botocore/data/sdb/2009-04-15/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-sdb-1.31.5/botocore_a_la_carte_sdb.egg-info/PKG-INFO` & `botocore-a-la-carte-sdb-1.31.6/botocore_a_la_carte_sdb.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-sdb
-Version: 1.31.5
+Version: 1.31.6
 Summary: sdb data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-sdb-1.31.5/setup.py` & `botocore-a-la-carte-sdb-1.31.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-sdb',
-    version="1.31.5",
+    version="1.31.6",
     description='sdb data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/sdb/*/*.json'],
```

