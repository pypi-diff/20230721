# Comparing `tmp/dvag_mon_shared-1.0.4.tar.gz` & `tmp/dvag_mon_shared-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvag_mon_shared-1.0.4.tar", last modified: Thu Jul 20 20:10:21 2023, max compression
+gzip compressed data, was "dvag_mon_shared-1.0.5.tar", last modified: Fri Jul 21 01:24:40 2023, max compression
```

## Comparing `dvag_mon_shared-1.0.4.tar` & `dvag_mon_shared-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 holge     (1000) holge     (1000)        0 2023-07-20 20:10:21.507300 dvag_mon_shared-1.0.4/
--rw-r--r--   0 holge     (1000) holge     (1000)        0 2023-07-20 17:27:36.000000 dvag_mon_shared-1.0.4/LICENSE
--rw-r--r--   0 holge     (1000) holge     (1000)     1215 2023-07-20 20:10:21.507300 dvag_mon_shared-1.0.4/PKG-INFO
--rw-r--r--   0 holge     (1000) holge     (1000)      746 2023-07-20 17:27:36.000000 dvag_mon_shared-1.0.4/README.md
--rw-r--r--   0 holge     (1000) holge     (1000)      698 2023-07-20 20:10:03.000000 dvag_mon_shared-1.0.4/pyproject.toml
--rw-r--r--   0 holge     (1000) holge     (1000)       38 2023-07-20 20:10:21.507300 dvag_mon_shared-1.0.4/setup.cfg
-drwxr-xr-x   0 holge     (1000) holge     (1000)        0 2023-07-20 20:10:21.497300 dvag_mon_shared-1.0.4/src/
-drwxr-xr-x   0 holge     (1000) holge     (1000)        0 2023-07-20 20:10:21.507300 dvag_mon_shared-1.0.4/src/dvag_mon_shared/
--rw-r--r--   0 holge     (1000) holge     (1000)     2892 2023-07-20 17:33:57.000000 dvag_mon_shared-1.0.4/src/dvag_mon_shared/AzureCredentials.py
--rw-r--r--   0 holge     (1000) holge     (1000)    16594 2023-07-20 17:27:36.000000 dvag_mon_shared-1.0.4/src/dvag_mon_shared/KqlClasses.py
--rw-r--r--   0 holge     (1000) holge     (1000)     2129 2023-07-20 17:36:43.000000 dvag_mon_shared-1.0.4/src/dvag_mon_shared/PushgwHeartbeat.py
--rw-r--r--   0 holge     (1000) holge     (1000)        0 2023-07-20 17:27:36.000000 dvag_mon_shared-1.0.4/src/dvag_mon_shared/__init__.py
--rw-r--r--   0 holge     (1000) holge     (1000)     1412 2023-07-20 17:27:36.000000 dvag_mon_shared-1.0.4/src/dvag_mon_shared/mapping_const.py
-drwxr-xr-x   0 holge     (1000) holge     (1000)        0 2023-07-20 20:10:21.507300 dvag_mon_shared-1.0.4/src/dvag_mon_shared.egg-info/
--rw-r--r--   0 holge     (1000) holge     (1000)     1215 2023-07-20 20:10:21.000000 dvag_mon_shared-1.0.4/src/dvag_mon_shared.egg-info/PKG-INFO
--rw-r--r--   0 holge     (1000) holge     (1000)      428 2023-07-20 20:10:21.000000 dvag_mon_shared-1.0.4/src/dvag_mon_shared.egg-info/SOURCES.txt
--rw-r--r--   0 holge     (1000) holge     (1000)        1 2023-07-20 20:10:21.000000 dvag_mon_shared-1.0.4/src/dvag_mon_shared.egg-info/dependency_links.txt
--rw-r--r--   0 holge     (1000) holge     (1000)      162 2023-07-20 20:10:21.000000 dvag_mon_shared-1.0.4/src/dvag_mon_shared.egg-info/requires.txt
--rw-r--r--   0 holge     (1000) holge     (1000)       16 2023-07-20 20:10:21.000000 dvag_mon_shared-1.0.4/src/dvag_mon_shared.egg-info/top_level.txt
+drwxr-xr-x   0 holge     (1000) holge     (1000)        0 2023-07-21 01:24:40.828250 dvag_mon_shared-1.0.5/
+-rw-r--r--   0 holge     (1000) holge     (1000)        0 2023-07-20 17:27:36.000000 dvag_mon_shared-1.0.5/LICENSE
+-rw-r--r--   0 holge     (1000) holge     (1000)     1215 2023-07-21 01:24:40.828250 dvag_mon_shared-1.0.5/PKG-INFO
+-rw-r--r--   0 holge     (1000) holge     (1000)      746 2023-07-20 17:27:36.000000 dvag_mon_shared-1.0.5/README.md
+-rw-r--r--   0 holge     (1000) holge     (1000)      698 2023-07-21 01:24:19.000000 dvag_mon_shared-1.0.5/pyproject.toml
+-rw-r--r--   0 holge     (1000) holge     (1000)       38 2023-07-21 01:24:40.828250 dvag_mon_shared-1.0.5/setup.cfg
+drwxr-xr-x   0 holge     (1000) holge     (1000)        0 2023-07-21 01:24:40.828250 dvag_mon_shared-1.0.5/src/
+drwxr-xr-x   0 holge     (1000) holge     (1000)        0 2023-07-21 01:24:40.828250 dvag_mon_shared-1.0.5/src/dvag_mon_shared/
+-rw-r--r--   0 holge     (1000) holge     (1000)     2892 2023-07-20 17:33:57.000000 dvag_mon_shared-1.0.5/src/dvag_mon_shared/AzureCredentials.py
+-rw-r--r--   0 holge     (1000) holge     (1000)    16595 2023-07-21 01:23:08.000000 dvag_mon_shared-1.0.5/src/dvag_mon_shared/KqlClasses.py
+-rw-r--r--   0 holge     (1000) holge     (1000)     2129 2023-07-20 17:36:43.000000 dvag_mon_shared-1.0.5/src/dvag_mon_shared/PushgwHeartbeat.py
+-rw-r--r--   0 holge     (1000) holge     (1000)        0 2023-07-20 17:27:36.000000 dvag_mon_shared-1.0.5/src/dvag_mon_shared/__init__.py
+-rw-r--r--   0 holge     (1000) holge     (1000)     1800 2023-07-21 01:23:06.000000 dvag_mon_shared-1.0.5/src/dvag_mon_shared/mapping_const.py
+drwxr-xr-x   0 holge     (1000) holge     (1000)        0 2023-07-21 01:24:40.828250 dvag_mon_shared-1.0.5/src/dvag_mon_shared.egg-info/
+-rw-r--r--   0 holge     (1000) holge     (1000)     1215 2023-07-21 01:24:40.000000 dvag_mon_shared-1.0.5/src/dvag_mon_shared.egg-info/PKG-INFO
+-rw-r--r--   0 holge     (1000) holge     (1000)      428 2023-07-21 01:24:40.000000 dvag_mon_shared-1.0.5/src/dvag_mon_shared.egg-info/SOURCES.txt
+-rw-r--r--   0 holge     (1000) holge     (1000)        1 2023-07-21 01:24:40.000000 dvag_mon_shared-1.0.5/src/dvag_mon_shared.egg-info/dependency_links.txt
+-rw-r--r--   0 holge     (1000) holge     (1000)      162 2023-07-21 01:24:40.000000 dvag_mon_shared-1.0.5/src/dvag_mon_shared.egg-info/requires.txt
+-rw-r--r--   0 holge     (1000) holge     (1000)       16 2023-07-21 01:24:40.000000 dvag_mon_shared-1.0.5/src/dvag_mon_shared.egg-info/top_level.txt
```

### Comparing `dvag_mon_shared-1.0.4/PKG-INFO` & `dvag_mon_shared-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvag_mon_shared
-Version: 1.0.4
+Version: 1.0.5
 Summary: infra-monitoring-functions shared libraries
 Author-email: Team Monitoring <monitoring@dvag.com>
 Project-URL: Github, https://github.com/dvag/infra-monitoring-functions
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `dvag_mon_shared-1.0.4/README.md` & `dvag_mon_shared-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dvag_mon_shared-1.0.4/pyproject.toml` & `dvag_mon_shared-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   "prometheus-client",
   "dataclasses",
   'python-dateutil',
   'pytimeparse',
   'azure-storage-blob'
 ]
 name = "dvag_mon_shared"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Team Monitoring", email="monitoring@dvag.com" },
 ]
 description = "infra-monitoring-functions shared libraries"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dvag_mon_shared-1.0.4/src/dvag_mon_shared/AzureCredentials.py` & `dvag_mon_shared-1.0.5/src/dvag_mon_shared/AzureCredentials.py`

 * *Files identical despite different names*

### Comparing `dvag_mon_shared-1.0.4/src/dvag_mon_shared/KqlClasses.py` & `dvag_mon_shared-1.0.5/src/dvag_mon_shared/KqlClasses.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import json
 from typing import Callable
 from dataclasses import dataclass
 from azure.storage.blob import BlobServiceClient
 import os
 
 
+
 @dataclass
 class KQLQueryResponse:
     """Result of a KQLQuery"""
     ok: bool
     status_code: int
     result: LogsQueryResult | dict
```

### Comparing `dvag_mon_shared-1.0.4/src/dvag_mon_shared/PushgwHeartbeat.py` & `dvag_mon_shared-1.0.5/src/dvag_mon_shared/PushgwHeartbeat.py`

 * *Files identical despite different names*

### Comparing `dvag_mon_shared-1.0.4/src/dvag_mon_shared/mapping_const.py` & `dvag_mon_shared-1.0.5/src/dvag_mon_shared/mapping_const.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,7 +23,20 @@
     "abe03732-5b76-46da-89c9-7e837221329b":       "publicip-prod-01",
     "9966d0fb-f44f-41c9-8771-d15e3178db8b":       "slam-prod-01",
     "ca14d2a8-0e05-4312-91bc-d7112ffa2e3d":       "spielwiese-dev-01",
     "607da2f4-020a-4b0c-b0b7-5b9db8bbe6df":       "spielwiese-preprod-01",
     "e453ac6a-bb68-4b9e-86d0-e778836b3d5d":       "virtualdesktop-prod-01",
     "f297637f-5a4e-4187-b1a2-86e9d1b2448b":       "workai-prod-01"
 }
+
+def map_environment(env: str) -> str:
+    ENVIRONMENT_MAP = {
+        "ent":      "Entwicklung",
+        "dev":      "Entwicklung",
+        "int":      "Integration",
+        "prd":      "Produktion",
+        "prod":     "Produktion",
+        "abn":      "Abnahme",
+        "preprod":  "Abnahme",
+        "id":       "Innendienst"
+    }
+    return ENVIRONMENT_MAP.get(env, "Entwicklung")
```

### Comparing `dvag_mon_shared-1.0.4/src/dvag_mon_shared.egg-info/PKG-INFO` & `dvag_mon_shared-1.0.5/src/dvag_mon_shared.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvag-mon-shared
-Version: 1.0.4
+Version: 1.0.5
 Summary: infra-monitoring-functions shared libraries
 Author-email: Team Monitoring <monitoring@dvag.com>
 Project-URL: Github, https://github.com/dvag/infra-monitoring-functions
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

