# Comparing `tmp/mlsteam-client-0.4.8.tar.gz` & `tmp/mlsteam-client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlsteam-client-0.4.8.tar", last modified: Thu Aug 18 08:39:02 2022, max compression
+gzip compressed data, was "mlsteam-client-0.5.0.tar", last modified: Fri Jul 21 08:14:39 2023, max compression
```

## Comparing `mlsteam-client-0.4.8.tar` & `mlsteam-client-0.5.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 simon     (1001) simon     (1001)        0 2022-08-18 08:39:02.811843 mlsteam-client-0.4.8/
--rw-rw-r--   0 simon     (1001) simon     (1001)       24 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/MANIFEST.in
--rw-rw-r--   0 simon     (1001) simon     (1001)     1628 2022-08-18 08:39:02.811843 mlsteam-client-0.4.8/PKG-INFO
--rw-rw-r--   0 simon     (1001) simon     (1001)      402 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/README.md
-drwxrwxr-x   0 simon     (1001) simon     (1001)        0 2022-08-18 08:39:02.795844 mlsteam-client-0.4.8/bin/
--rwxrwxr-x   0 simon     (1001) simon     (1001) 17491008 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/bin/mc
-drwxrwxr-x   0 simon     (1001) simon     (1001)        0 2022-08-18 08:39:02.811843 mlsteam-client-0.4.8/mlsteam/
--rw-rw-r--   0 simon     (1001) simon     (1001)     1582 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/__init__.py
--rw-rw-r--   0 simon     (1001) simon     (1001)    18573 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/api.py
-drwxrwxr-x   0 simon     (1001) simon     (1001)        0 2022-08-18 08:39:02.811843 mlsteam-client-0.4.8/mlsteam/api_clients/
--rw-rw-r--   0 simon     (1001) simon     (1001)        0 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/api_clients/__init__.py
--rw-rw-r--   0 simon     (1001) simon     (1001)     1446 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/api_clients/credential.py
--rw-rw-r--   0 simon     (1001) simon     (1001)     1082 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/auth.py
-drwxrwxr-x   0 simon     (1001) simon     (1001)        0 2022-08-18 08:39:02.811843 mlsteam-client-0.4.8/mlsteam/batch_processor/
--rw-rw-r--   0 simon     (1001) simon     (1001)        0 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/batch_processor/__init__.py
--rw-rw-r--   0 simon     (1001) simon     (1001)     1454 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/checkpoint.py
--rw-rw-r--   0 simon     (1001) simon     (1001)      994 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/cli.py
--rw-rw-r--   0 simon     (1001) simon     (1001)     8219 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/consumer.py
--rw-rw-r--   0 simon     (1001) simon     (1001)     1571 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/container.py
--rw-rw-r--   0 simon     (1001) simon     (1001)     5390 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/dataset.py
--rw-rw-r--   0 simon     (1001) simon     (1001)     5344 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/ds.py
--rw-rw-r--   0 simon     (1001) simon     (1001)      133 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/envs.py
--rw-rw-r--   0 simon     (1001) simon     (1001)     1076 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/exceptions.py
--rw-rw-r--   0 simon     (1001) simon     (1001)      572 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/info.py
--rw-rw-r--   0 simon     (1001) simon     (1001)     5231 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/job.py
--rw-rw-r--   0 simon     (1001) simon     (1001)     1175 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/keras.py
--rw-rw-r--   0 simon     (1001) simon     (1001)      687 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/metrics.py
--rw-rw-r--   0 simon     (1001) simon     (1001)     4923 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/model.py
--rw-rw-r--   0 simon     (1001) simon     (1001)     2841 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/project.py
--rw-rw-r--   0 simon     (1001) simon     (1001)     1059 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/service.py
--rw-rw-r--   0 simon     (1001) simon     (1001)     1403 2022-08-18 08:37:53.000000 mlsteam-client-0.4.8/mlsteam/stparams.py
--rw-rw-r--   0 simon     (1001) simon     (1001)     2602 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/track.py
--rw-rw-r--   0 simon     (1001) simon     (1001)     1275 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/utils.py
--rw-rw-r--   0 simon     (1001) simon     (1001)       22 2022-08-18 08:38:33.000000 mlsteam-client-0.4.8/mlsteam/version.py
--rw-rw-r--   0 simon     (1001) simon     (1001)     1756 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/mlsteam/work.py
-drwxrwxr-x   0 simon     (1001) simon     (1001)        0 2022-08-18 08:39:02.811843 mlsteam-client-0.4.8/mlsteam_client.egg-info/
--rw-rw-r--   0 simon     (1001) simon     (1001)     1628 2022-08-18 08:39:02.000000 mlsteam-client-0.4.8/mlsteam_client.egg-info/PKG-INFO
--rw-rw-r--   0 simon     (1001) simon     (1001)      992 2022-08-18 08:39:02.000000 mlsteam-client-0.4.8/mlsteam_client.egg-info/SOURCES.txt
--rw-rw-r--   0 simon     (1001) simon     (1001)        1 2022-08-18 08:39:02.000000 mlsteam-client-0.4.8/mlsteam_client.egg-info/dependency_links.txt
--rw-rw-r--   0 simon     (1001) simon     (1001)       45 2022-08-18 08:39:02.000000 mlsteam-client-0.4.8/mlsteam_client.egg-info/entry_points.txt
--rw-rw-r--   0 simon     (1001) simon     (1001)        1 2022-06-28 02:53:24.000000 mlsteam-client-0.4.8/mlsteam_client.egg-info/not-zip-safe
--rw-rw-r--   0 simon     (1001) simon     (1001)       73 2022-08-18 08:39:02.000000 mlsteam-client-0.4.8/mlsteam_client.egg-info/requires.txt
--rw-rw-r--   0 simon     (1001) simon     (1001)       14 2022-08-18 08:39:02.000000 mlsteam-client-0.4.8/mlsteam_client.egg-info/top_level.txt
--rw-rw-r--   0 simon     (1001) simon     (1001)       73 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/requirements.txt
--rw-rw-r--   0 simon     (1001) simon     (1001)      118 2022-08-18 08:39:02.811843 mlsteam-client-0.4.8/setup.cfg
--rw-rw-r--   0 simon     (1001) simon     (1001)     2425 2022-08-18 08:38:33.000000 mlsteam-client-0.4.8/setup.py
-drwxrwxr-x   0 simon     (1001) simon     (1001)        0 2022-08-18 08:39:02.811843 mlsteam-client-0.4.8/tests/
--rw-rw-r--   0 simon     (1001) simon     (1001)        0 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/tests/__init__.py
--rw-rw-r--   0 simon     (1001) simon     (1001)      303 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/tests/config.py
--rw-rw-r--   0 simon     (1001) simon     (1001)     7394 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/tests/test_api.py
--rw-rw-r--   0 simon     (1001) simon     (1001)     2915 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/tests/test_basic.py
--rw-rw-r--   0 simon     (1001) simon     (1001)     8212 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/tests/test_negative_api.py
--rw-rw-r--   0 simon     (1001) simon     (1001)     2799 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/tests/test_negative_basic.py
--rw-rw-r--   0 simon     (1001) simon     (1001)      187 2022-06-28 02:53:09.000000 mlsteam-client-0.4.8/tests/test_track.py
+drwxrwxr-x   0 simon     (1003) simon     (1003)        0 2023-07-21 08:14:39.595554 mlsteam-client-0.5.0/
+-rw-rw-r--   0 simon     (1003) simon     (1003)       24 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/MANIFEST.in
+-rw-rw-r--   0 simon     (1003) simon     (1003)     1628 2023-07-21 08:14:39.595554 mlsteam-client-0.5.0/PKG-INFO
+-rw-rw-r--   0 simon     (1003) simon     (1003)      402 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/README.md
+drwxrwxr-x   0 simon     (1003) simon     (1003)        0 2023-07-21 08:14:39.575554 mlsteam-client-0.5.0/bin/
+-rwxrwxr-x   0 simon     (1003) simon     (1003) 17491008 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/bin/mc
+drwxrwxr-x   0 simon     (1003) simon     (1003)        0 2023-07-21 08:14:39.595554 mlsteam-client-0.5.0/mlsteam/
+-rw-rw-r--   0 simon     (1003) simon     (1003)     1582 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/mlsteam/__init__.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)    18573 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/mlsteam/api.py
+drwxrwxr-x   0 simon     (1003) simon     (1003)        0 2023-07-21 08:14:39.595554 mlsteam-client-0.5.0/mlsteam/api_clients/
+-rw-rw-r--   0 simon     (1003) simon     (1003)        0 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/mlsteam/api_clients/__init__.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)     1446 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/mlsteam/api_clients/credential.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)     1082 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/mlsteam/auth.py
+drwxrwxr-x   0 simon     (1003) simon     (1003)        0 2023-07-21 08:14:39.595554 mlsteam-client-0.5.0/mlsteam/batch_processor/
+-rw-rw-r--   0 simon     (1003) simon     (1003)        0 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/mlsteam/batch_processor/__init__.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)     1454 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/mlsteam/checkpoint.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)      994 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/mlsteam/cli.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)     9354 2023-07-21 08:13:25.000000 mlsteam-client-0.5.0/mlsteam/consumer.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)     1571 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/mlsteam/container.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)     5390 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/mlsteam/dataset.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)     5344 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/mlsteam/ds.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)      133 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/mlsteam/envs.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)     1076 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/mlsteam/exceptions.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)      572 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/mlsteam/info.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)     5231 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/mlsteam/job.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)     1175 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/mlsteam/keras.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)      687 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/mlsteam/metrics.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)     4923 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/mlsteam/model.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)     2841 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/mlsteam/project.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)     1059 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/mlsteam/service.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)     1403 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/mlsteam/stparams.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)     2696 2023-07-21 08:13:25.000000 mlsteam-client-0.5.0/mlsteam/track.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)     1275 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/mlsteam/utils.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)       22 2023-07-21 08:14:12.000000 mlsteam-client-0.5.0/mlsteam/version.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)     1756 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/mlsteam/work.py
+drwxrwxr-x   0 simon     (1003) simon     (1003)        0 2023-07-21 08:14:39.595554 mlsteam-client-0.5.0/mlsteam_client.egg-info/
+-rw-rw-r--   0 simon     (1003) simon     (1003)     1628 2023-07-21 08:14:39.000000 mlsteam-client-0.5.0/mlsteam_client.egg-info/PKG-INFO
+-rw-rw-r--   0 simon     (1003) simon     (1003)      992 2023-07-21 08:14:39.000000 mlsteam-client-0.5.0/mlsteam_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon     (1003) simon     (1003)        1 2023-07-21 08:14:39.000000 mlsteam-client-0.5.0/mlsteam_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon     (1003) simon     (1003)       45 2023-07-21 08:14:39.000000 mlsteam-client-0.5.0/mlsteam_client.egg-info/entry_points.txt
+-rw-rw-r--   0 simon     (1003) simon     (1003)        1 2023-07-21 08:14:39.000000 mlsteam-client-0.5.0/mlsteam_client.egg-info/not-zip-safe
+-rw-rw-r--   0 simon     (1003) simon     (1003)       73 2023-07-21 08:14:39.000000 mlsteam-client-0.5.0/mlsteam_client.egg-info/requires.txt
+-rw-rw-r--   0 simon     (1003) simon     (1003)       14 2023-07-21 08:14:39.000000 mlsteam-client-0.5.0/mlsteam_client.egg-info/top_level.txt
+-rw-rw-r--   0 simon     (1003) simon     (1003)       73 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/requirements.txt
+-rw-rw-r--   0 simon     (1003) simon     (1003)      118 2023-07-21 08:14:39.595554 mlsteam-client-0.5.0/setup.cfg
+-rw-rw-r--   0 simon     (1003) simon     (1003)     2425 2023-07-21 08:14:12.000000 mlsteam-client-0.5.0/setup.py
+drwxrwxr-x   0 simon     (1003) simon     (1003)        0 2023-07-21 08:14:39.595554 mlsteam-client-0.5.0/tests/
+-rw-rw-r--   0 simon     (1003) simon     (1003)        0 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/tests/__init__.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)      303 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/tests/config.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)     7394 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/tests/test_api.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)     2915 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/tests/test_basic.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)     8212 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/tests/test_negative_api.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)     2799 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/tests/test_negative_basic.py
+-rw-rw-r--   0 simon     (1003) simon     (1003)      187 2023-07-11 05:18:05.000000 mlsteam-client-0.5.0/tests/test_track.py
```

### Comparing `mlsteam-client-0.4.8/PKG-INFO` & `mlsteam-client-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlsteam-client
-Version: 0.4.8
+Version: 0.5.0
 Summary: MLSteam Client
 Home-page: https://myelintek.com
 Author: MyelinTek inc.
 Author-email: simon@myelintek.com
 License: MIT
 Description: # MLSteam client - ML experiment tracking tool
         ---
```

### Comparing `mlsteam-client-0.4.8/bin/mc` & `mlsteam-client-0.5.0/bin/mc`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/mlsteam/__init__.py` & `mlsteam-client-0.5.0/mlsteam/__init__.py`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/mlsteam/api.py` & `mlsteam-client-0.5.0/mlsteam/api.py`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/mlsteam/api_clients/credential.py` & `mlsteam-client-0.5.0/mlsteam/api_clients/credential.py`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/mlsteam/auth.py` & `mlsteam-client-0.5.0/mlsteam/auth.py`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/mlsteam/checkpoint.py` & `mlsteam-client-0.5.0/mlsteam/checkpoint.py`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/mlsteam/cli.py` & `mlsteam-client-0.5.0/mlsteam/cli.py`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/mlsteam/consumer.py` & `mlsteam-client-0.5.0/mlsteam/consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 import click
 import platform
 import threading
 import queue
+import yaml
 from urllib.parse import urlparse
 from pathlib import Path
 from time import time
 from bravado.requests_client import RequestsClient
 from bravado.client import SwaggerClient
 from mlsteam.api_clients.credential import Credential
 from mlsteam.version import __version__
 from mlsteam.exceptions import MLSteamInvalidProjectNameException
 ROOT_PATH = ".mlsteam"
 MAX_AGGREGATE_LOG = 3000
 
 
 class ConsumerThread(threading.Thread):
     def __init__(self,
-        lock: threading.RLock,
-        cache: "DiskCache",
-        apiclient: "ApiClient",
-        project_uuid: str,
-        track_bucket_name: str,
-        sleep_time: int
-    ):
+                 lock: threading.RLock,
+                 cache: "DiskCache",
+                 apiclient: "ApiClient",
+                 project_uuid: str,
+                 track_id: int,
+                 track_bucket_name: str,
+                 sleep_time: int
+                 ):
         super().__init__(daemon=True)
         self._lock = lock
         self._sleep_time = sleep_time
         self._interrupted = False
         self._event = threading.Event()
         self._is_running = False
         self._cache = cache
         self._apiclient = apiclient
         self._puuid = project_uuid
+        self._track_id = track_id
         self._track_bucket_name = track_bucket_name
         click.echo("Initialized track background thread")
 
     def is_running(self):
         return self._is_running
 
     def disable_sleep(self):
@@ -47,25 +50,27 @@
 
     def wake_up(self):
         self._event.set()
 
     def run(self):
         self._is_running = True
         try:
+            self._apiclient.update_track(self._puuid, self._track_id, 'active')
             while not self._interrupted:
                 # print("consumer start")
                 self.work()
                 # print("consumer stop")
                 if self._sleep_time > 0 and not self._interrupted:
                     # print("sleep")
                     self._event.wait(timeout=self._sleep_time)
                     # print("wake")
                     self._event.clear()
                     # sleep for self._sleep_time
         finally:
+            self._apiclient.update_track(self._puuid, self._track_id, 'inactive')
             self._is_running = False
 
     def work(self):
         # while True:
         try:
             with self._lock:
                 self._cache.process(
@@ -78,14 +83,15 @@
 
 class DiskCache(object):
     def __init__(self, track_path, debug=False):
         from shutil import rmtree
         self._queue = queue.Queue()
         self._debug = debug
         self.track_path = Path(ROOT_PATH, track_path)
+        self._metadata = dict(logs=set())
         if not self.track_path.exists():
             self.track_path.mkdir(parents=True)
         else:
             for path in self.track_path.glob("**/*"):
                 if path.is_file():
                     path.unlink()
                 elif path.is_dir():
@@ -107,41 +113,29 @@
         i = MAX_AGGREGATE_LOG
         log_aggregate = {}
         while (not self._queue.empty()) and (i > 0):
             i = i - 1
             op = self._queue.get()
             if op.type == "config":
                 self._write_config(op.content)
-                for (keypath, value) in op.content.items():
-                    if isinstance(value, str):
-                        value = value.encode('utf-8')
-                    apiclient.put_file(
-                        bucket_name=bucket_name,
-                        obj_path=keypath,
-                        obj=value
-                    )
+                self._sync_file(apiclient, op.content, bucket_name)
             elif op.type == "log":
                 self._write_log(op.content)
                 for (key, value) in op.content.items():
+                    if key not in self._metadata['logs']:
+                        self._metadata['logs'].add(key)
+                        self._sync_metadata(apiclient, bucket_name)
                     if isinstance(value, str):
                         value = value.encode('utf-8')
                     if key in log_aggregate:
                         log_aggregate[key] = log_aggregate[key] + value
                     else:
                         log_aggregate[key] = value
         if log_aggregate:
-            for (keypath, value) in log_aggregate.items():
-                apiclient.put_file(
-                    bucket_name=bucket_name,
-                    obj_path=keypath,
-                    obj=value,
-                    part_offset='-1'
-                )
-            if self._debug:
-                click.echo("queue size: {}".format(self.queue_size()))
+            self._sync_file(apiclient, log_aggregate, bucket_name, "-1")
 
     def _write_config(self, content):
         for (key, value) in content.items():
             key_path = self.track_path.joinpath(key)
             if not key_path.parent.exists():
                 key_path.parent.mkdir(parents=True)
             with key_path.open('w') as f:
@@ -155,14 +149,35 @@
             key_path = self.track_path.joinpath(f"{key}.log")
             if not key_path.parent.exists():
                 key_path.parent.mkdir(parents=True)
             tm = time()
             with key_path.open('a') as f:
                 f.write(f"{tm}, {value}\n")
 
+    def _sync_metadata(self, apiclient: "ApiClient", bucket_name: str):
+        metadata_file = ".track_metadata.yaml"
+        data = {}
+        for meta in self._metadata:
+            data[meta] = list(self._metadata[meta])
+        content = {metadata_file: yaml.dump(data)}
+        self._sync_file(apiclient, content, bucket_name)
+
+    def _sync_file(self, apiclient: "ApiClient", content: dict, bucket_name: str, part_offset: str = None):
+        for (keypath, value) in content.items():
+            if isinstance(value, str):
+                value = value.encode('utf-8')
+            apiclient.put_file(
+                bucket_name=bucket_name,
+                obj_path=keypath,
+                obj=value,
+                part_offset=part_offset
+            )
+        if self._debug:
+            click.echo("queue size: {}".format(self.queue_size()))
+
 
 class QueueOp(object):
     def __init__(self, optype, content):
         self._optype = optype
         self._content = content
 
     @property
@@ -216,14 +231,23 @@
         result = self.swagger_client.track.getTrack(
             puuid=project_uuid,
             tid=track_id
         ).result()
         click.echo("Get track '{}' under project".format(result['name']))
         return result
 
+    def update_track(self, project_uuid, track_id, status):
+        result = self.swagger_client.track.updateTrack(
+            puuid=project_uuid,
+            tid=track_id,
+            status=status
+        ).result()
+        click.echo("Update track '{}' status: {}".format(track_id, status))
+        return result
+
     def put_file(self, bucket_name: str, obj_path: str, obj: bytes, part_offset: int = None):
         result = self.swagger_client.object.putObject(
             bucket_name=bucket_name,
             obj_path=obj_path,
             obj=obj,
             part_offset=part_offset,
             part_size=len(obj)
```

### Comparing `mlsteam-client-0.4.8/mlsteam/container.py` & `mlsteam-client-0.5.0/mlsteam/container.py`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/mlsteam/dataset.py` & `mlsteam-client-0.5.0/mlsteam/dataset.py`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/mlsteam/ds.py` & `mlsteam-client-0.5.0/mlsteam/ds.py`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/mlsteam/exceptions.py` & `mlsteam-client-0.5.0/mlsteam/exceptions.py`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/mlsteam/info.py` & `mlsteam-client-0.5.0/mlsteam/info.py`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/mlsteam/job.py` & `mlsteam-client-0.5.0/mlsteam/job.py`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/mlsteam/keras.py` & `mlsteam-client-0.5.0/mlsteam/keras.py`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/mlsteam/metrics.py` & `mlsteam-client-0.5.0/mlsteam/metrics.py`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/mlsteam/model.py` & `mlsteam-client-0.5.0/mlsteam/model.py`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/mlsteam/project.py` & `mlsteam-client-0.5.0/mlsteam/project.py`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/mlsteam/service.py` & `mlsteam-client-0.5.0/mlsteam/service.py`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/mlsteam/stparams.py` & `mlsteam-client-0.5.0/mlsteam/stparams.py`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/mlsteam/track.py` & `mlsteam-client-0.5.0/mlsteam/track.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import click
+import os
 import atexit
 import threading
 import traceback
 from time import sleep
 from mlsteam.consumer import ApiClient, DiskCache, ConsumerThread
 
 
 class Track(object):
     def __init__(self,
-        track: dict,
-        project_uuid: str,
-        apiclient: ApiClient,
-        background_jobs: list,
-        debug: bool
-    ):
+                 track: dict,
+                 project_uuid: str,
+                 apiclient: ApiClient,
+                 background_jobs: list,
+                 debug: bool
+                 ):
         self._info = track
         self._project_uuid = project_uuid
         self._lock = threading.RLock()
         self._apiclient = apiclient
         self._background_jobs = background_jobs
         self._debug = debug
         self._waiting_cond = threading.Condition(lock=self._lock)
         self._cache = DiskCache(f"{project_uuid}/{track['name']}", debug=self._debug)
         self._consumer = ConsumerThread(
             self._lock,
             self._cache,
             self._apiclient,
             project_uuid,
+            track['id'],
             track['bucket_name'],
             sleep_time=1
         )
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if exc_tb is not None:
             traceback.print_exception(exc_type, exc_val, exc_tb)
@@ -87,7 +89,8 @@
     def assign(self, value):
         with self._track.lock():
             self._cache.assign(self._key, value)
 
     def log(self, value):
         with self._track.lock():
             self._cache.log(self._key, value)
+
```

### Comparing `mlsteam-client-0.4.8/mlsteam/utils.py` & `mlsteam-client-0.5.0/mlsteam/utils.py`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/mlsteam/work.py` & `mlsteam-client-0.5.0/mlsteam/work.py`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/mlsteam_client.egg-info/PKG-INFO` & `mlsteam-client-0.5.0/mlsteam_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlsteam-client
-Version: 0.4.8
+Version: 0.5.0
 Summary: MLSteam Client
 Home-page: https://myelintek.com
 Author: MyelinTek inc.
 Author-email: simon@myelintek.com
 License: MIT
 Description: # MLSteam client - ML experiment tracking tool
         ---
```

### Comparing `mlsteam-client-0.4.8/mlsteam_client.egg-info/SOURCES.txt` & `mlsteam-client-0.5.0/mlsteam_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/setup.py` & `mlsteam-client-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os.path
 from setuptools import find_packages, setup
 # from mlsteam.version import __version__
-__version__ = "0.4.8"
+__version__ = "0.5.0"
 
 with open(
     os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.md"),
     encoding="utf-8",
 ) as handler:
     long_description = handler.read()
```

### Comparing `mlsteam-client-0.4.8/tests/test_api.py` & `mlsteam-client-0.5.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/tests/test_basic.py` & `mlsteam-client-0.5.0/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/tests/test_negative_api.py` & `mlsteam-client-0.5.0/tests/test_negative_api.py`

 * *Files identical despite different names*

### Comparing `mlsteam-client-0.4.8/tests/test_negative_basic.py` & `mlsteam-client-0.5.0/tests/test_negative_basic.py`

 * *Files identical despite different names*

