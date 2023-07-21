# Comparing `tmp/warpzone_sdk-8.3.3.tar.gz` & `tmp/warpzone_sdk-8.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warpzone_sdk-8.3.3.tar", max compression
+gzip compressed data, was "warpzone_sdk-8.3.4.tar", max compression
```

## Comparing `warpzone_sdk-8.3.3.tar` & `warpzone_sdk-8.3.4.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0     1071 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/pyproject.toml
--rw-r--r--   0        0        0     1293 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/__init__.py
--rw-r--r--   0        0        0       21 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/blobstorage/__init__.py
--rw-r--r--   0        0        0     2844 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/blobstorage/client.py
--rw-r--r--   0        0        0       24 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/enums/__init__.py
--rw-r--r--   0        0        0      213 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/enums/topicenum.py
--rw-r--r--   0        0        0       27 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/function/__init__.py
--rw-r--r--   0        0        0     2108 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/function/functionize.py
--rw-r--r--   0        0        0     3840 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/function/integrations.py
--rw-r--r--   0        0        0     2223 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/function/monitor.py
--rw-r--r--   0        0        0     2105 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/function/process.py
--rw-r--r--   0        0        0       46 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/function/processors/__init__.py
--rw-r--r--   0        0        0      781 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/function/processors/dependencies.py
--rw-r--r--   0        0        0     2067 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/function/processors/outputs.py
--rw-r--r--   0        0        0     1727 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/function/processors/triggers.py
--rw-r--r--   0        0        0     2268 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/function/signature.py
--rw-r--r--   0        0        0      547 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/function/types.py
--rw-r--r--   0        0        0     2108 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/healthchecks/__init__.py
--rw-r--r--   0        0        0     1112 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/healthchecks/model.py
--rw-r--r--   0        0        0       87 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/monitor/__init__.py
--rw-r--r--   0        0        0     1650 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/monitor/logs.py
--rw-r--r--   0        0        0     4781 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/monitor/traces.py
--rw-r--r--   0        0        0       21 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/servicebus/data/__init__.py
--rw-r--r--   0        0        0     5636 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/servicebus/data/client.py
--rw-r--r--   0        0        0       21 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/servicebus/events/__init__.py
--rw-r--r--   0        0        0     4250 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/servicebus/events/client.py
--rw-r--r--   0        0        0       21 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/tablestorage/db/__init__.py
--rw-r--r--   0        0        0     1522 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/tablestorage/db/base_client.py
--rw-r--r--   0        0        0     1960 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/tablestorage/db/client.py
--rw-r--r--   0        0        0     1704 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/tablestorage/db/client_async.py
--rw-r--r--   0        0        0       47 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/tablestorage/tables/__init__.py
--rw-r--r--   0        0        0     2916 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/tablestorage/tables/client.py
--rw-r--r--   0        0        0     2516 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/tablestorage/tables/client_async.py
--rw-r--r--   0        0        0      521 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/tablestorage/tables/helpers.py
--rw-r--r--   0        0        0     2470 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/tablestorage/tables/operations.py
--rw-r--r--   0        0        0      248 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/testing/__init__.py
--rw-r--r--   0        0        0     3661 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/testing/assertions.py
--rw-r--r--   0        0        0     3661 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/testing/data.py
--rw-r--r--   0        0        0       27 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/transform/__init__.py
--rw-r--r--   0        0        0     1641 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/transform/data.py
--rw-r--r--   0        0        0     1968 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/transform/schema.py
--rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 warpzone_sdk-8.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1330 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/__init__.py
+-rw-r--r--   0        0        0       21 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/blobstorage/__init__.py
+-rw-r--r--   0        0        0     2844 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/blobstorage/client.py
+-rw-r--r--   0        0        0       24 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/enums/__init__.py
+-rw-r--r--   0        0        0      213 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/enums/topicenum.py
+-rw-r--r--   0        0        0       35 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/__init__.py
+-rw-r--r--   0        0        0     1018 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/checks.py
+-rw-r--r--   0        0        0     2108 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/functionize.py
+-rw-r--r--   0        0        0     3840 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/integrations.py
+-rw-r--r--   0        0        0     2223 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/monitor.py
+-rw-r--r--   0        0        0     2105 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/process.py
+-rw-r--r--   0        0        0       46 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/processors/__init__.py
+-rw-r--r--   0        0        0      781 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/processors/dependencies.py
+-rw-r--r--   0        0        0     2067 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/processors/outputs.py
+-rw-r--r--   0        0        0     1727 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/processors/triggers.py
+-rw-r--r--   0        0        0     2268 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/signature.py
+-rw-r--r--   0        0        0      547 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/types.py
+-rw-r--r--   0        0        0     2108 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/healthchecks/__init__.py
+-rw-r--r--   0        0        0     1112 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/healthchecks/model.py
+-rw-r--r--   0        0        0       87 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/monitor/__init__.py
+-rw-r--r--   0        0        0     1650 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/monitor/logs.py
+-rw-r--r--   0        0        0     4781 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/monitor/traces.py
+-rw-r--r--   0        0        0       21 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/servicebus/data/__init__.py
+-rw-r--r--   0        0        0     5636 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/servicebus/data/client.py
+-rw-r--r--   0        0        0       21 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/servicebus/events/__init__.py
+-rw-r--r--   0        0        0     4250 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/servicebus/events/client.py
+-rw-r--r--   0        0        0       21 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/tablestorage/db/__init__.py
+-rw-r--r--   0        0        0     1522 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/tablestorage/db/base_client.py
+-rw-r--r--   0        0        0     1960 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/tablestorage/db/client.py
+-rw-r--r--   0        0        0     1704 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/tablestorage/db/client_async.py
+-rw-r--r--   0        0        0       47 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/tablestorage/tables/__init__.py
+-rw-r--r--   0        0        0     2916 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/tablestorage/tables/client.py
+-rw-r--r--   0        0        0     2516 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/tablestorage/tables/client_async.py
+-rw-r--r--   0        0        0      521 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/tablestorage/tables/helpers.py
+-rw-r--r--   0        0        0     2470 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/tablestorage/tables/operations.py
+-rw-r--r--   0        0        0      248 2023-07-21 13:08:40.019096 warpzone_sdk-8.3.4/warpzone/testing/__init__.py
+-rw-r--r--   0        0        0     3661 2023-07-21 13:08:40.019096 warpzone_sdk-8.3.4/warpzone/testing/assertions.py
+-rw-r--r--   0        0        0     3661 2023-07-21 13:08:40.019096 warpzone_sdk-8.3.4/warpzone/testing/data.py
+-rw-r--r--   0        0        0       27 2023-07-21 13:08:40.019096 warpzone_sdk-8.3.4/warpzone/transform/__init__.py
+-rw-r--r--   0        0        0     1641 2023-07-21 13:08:40.019096 warpzone_sdk-8.3.4/warpzone/transform/data.py
+-rw-r--r--   0        0        0     1968 2023-07-21 13:08:40.019096 warpzone_sdk-8.3.4/warpzone/transform/schema.py
+-rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 warpzone_sdk-8.3.4/PKG-INFO
```

### Comparing `warpzone_sdk-8.3.3/pyproject.toml` & `warpzone_sdk-8.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "warpzone-sdk"
-version = "8.3.3"
+version = "8.3.4"
 description = "The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage"
 authors = ["Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "warpzone" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^1.4.3"
 pyarrow = "^9.0.0"
+datamazing = "^2.0.0"
 azure-data-tables = "^12.4.0"
 azure-servicebus = "~7.8.0"
 azure-storage-blob = "^12.14.1"
 aiohttp = "^3.8.3"
 azure-core-tracing-opentelemetry = "^1.0.0b9"
 azure-monitor-opentelemetry-exporter = "^1.0.0b11"
 opentelemetry-sdk = "1.14.0"
```

### Comparing `warpzone_sdk-8.3.3/warpzone/__init__.py` & `warpzone_sdk-8.3.4/warpzone/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from warpzone import healthchecks, testing
 from warpzone.blobstorage.client import BlobData, WarpzoneBlobClient
 from warpzone.enums.topicenum import Topic
+from warpzone.function import checks
 from warpzone.function.functionize import functionize
 from warpzone.function.integrations import (
     get_blob_client,
     get_data_client,
     get_db_client,
     get_db_client_async,
     get_event_client,
```

### Comparing `warpzone_sdk-8.3.3/warpzone/blobstorage/client.py` & `warpzone_sdk-8.3.4/warpzone/blobstorage/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/function/functionize.py` & `warpzone_sdk-8.3.4/warpzone/function/functionize.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/function/integrations.py` & `warpzone_sdk-8.3.4/warpzone/function/integrations.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/function/monitor.py` & `warpzone_sdk-8.3.4/warpzone/function/monitor.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/function/process.py` & `warpzone_sdk-8.3.4/warpzone/function/process.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/function/processors/dependencies.py` & `warpzone_sdk-8.3.4/warpzone/function/processors/dependencies.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/function/processors/outputs.py` & `warpzone_sdk-8.3.4/warpzone/function/processors/outputs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/function/processors/triggers.py` & `warpzone_sdk-8.3.4/warpzone/function/processors/triggers.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/function/signature.py` & `warpzone_sdk-8.3.4/warpzone/function/signature.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/function/types.py` & `warpzone_sdk-8.3.4/warpzone/function/types.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/healthchecks/__init__.py` & `warpzone_sdk-8.3.4/warpzone/healthchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/healthchecks/model.py` & `warpzone_sdk-8.3.4/warpzone/healthchecks/model.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/monitor/logs.py` & `warpzone_sdk-8.3.4/warpzone/monitor/logs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/monitor/traces.py` & `warpzone_sdk-8.3.4/warpzone/monitor/traces.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/servicebus/data/client.py` & `warpzone_sdk-8.3.4/warpzone/servicebus/data/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/servicebus/events/client.py` & `warpzone_sdk-8.3.4/warpzone/servicebus/events/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/tablestorage/db/base_client.py` & `warpzone_sdk-8.3.4/warpzone/tablestorage/db/base_client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/tablestorage/db/client.py` & `warpzone_sdk-8.3.4/warpzone/tablestorage/db/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/tablestorage/db/client_async.py` & `warpzone_sdk-8.3.4/warpzone/tablestorage/db/client_async.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/tablestorage/tables/client.py` & `warpzone_sdk-8.3.4/warpzone/tablestorage/tables/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/tablestorage/tables/client_async.py` & `warpzone_sdk-8.3.4/warpzone/tablestorage/tables/client_async.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/tablestorage/tables/helpers.py` & `warpzone_sdk-8.3.4/warpzone/tablestorage/tables/helpers.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/tablestorage/tables/operations.py` & `warpzone_sdk-8.3.4/warpzone/tablestorage/tables/operations.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/testing/assertions.py` & `warpzone_sdk-8.3.4/warpzone/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/testing/data.py` & `warpzone_sdk-8.3.4/warpzone/testing/data.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/transform/data.py` & `warpzone_sdk-8.3.4/warpzone/transform/data.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/warpzone/transform/schema.py` & `warpzone_sdk-8.3.4/warpzone/transform/schema.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.3/PKG-INFO` & `warpzone_sdk-8.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warpzone-sdk
-Version: 8.3.3
+Version: 8.3.4
 Summary: The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage
 Author: Mikkel Ladekarl Folmersen Nygaard
 Author-email: mny@energinet.dk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -12,11 +12,12 @@
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: azure-core-tracing-opentelemetry (>=1.0.0b9,<2.0.0)
 Requires-Dist: azure-data-tables (>=12.4.0,<13.0.0)
 Requires-Dist: azure-functions (>=1.12.0,<2.0.0)
 Requires-Dist: azure-monitor-opentelemetry-exporter (>=1.0.0b11,<2.0.0)
 Requires-Dist: azure-servicebus (>=7.8.0,<7.9.0)
 Requires-Dist: azure-storage-blob (>=12.14.1,<13.0.0)
+Requires-Dist: datamazing (>=2.0.0,<3.0.0)
 Requires-Dist: opentelemetry-sdk (==1.14.0)
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Requires-Dist: pyarrow (>=9.0.0,<10.0.0)
 Requires-Dist: typeguard (>=3.0.1,<4.0.0)
```

