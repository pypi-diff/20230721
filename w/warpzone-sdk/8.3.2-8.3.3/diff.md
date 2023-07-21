# Comparing `tmp/warpzone_sdk-8.3.2.tar.gz` & `tmp/warpzone_sdk-8.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warpzone_sdk-8.3.2.tar", max compression
+gzip compressed data, was "warpzone_sdk-8.3.3.tar", max compression
```

## Comparing `warpzone_sdk-8.3.2.tar` & `warpzone_sdk-8.3.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1071 2023-07-21 07:11:38.907779 warpzone_sdk-8.3.2/pyproject.toml
--rw-r--r--   0        0        0     1293 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/__init__.py
--rw-r--r--   0        0        0       21 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/blobstorage/__init__.py
--rw-r--r--   0        0        0     2844 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/blobstorage/client.py
--rw-r--r--   0        0        0       24 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/enums/__init__.py
--rw-r--r--   0        0        0      213 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/enums/topicenum.py
--rw-r--r--   0        0        0       27 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/function/__init__.py
--rw-r--r--   0        0        0     2108 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/function/functionize.py
--rw-r--r--   0        0        0     3840 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/function/integrations.py
--rw-r--r--   0        0        0     2223 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/function/monitor.py
--rw-r--r--   0        0        0     2105 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/function/process.py
--rw-r--r--   0        0        0       46 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/function/processors/__init__.py
--rw-r--r--   0        0        0      781 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/function/processors/dependencies.py
--rw-r--r--   0        0        0     2067 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/function/processors/outputs.py
--rw-r--r--   0        0        0     1727 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/function/processors/triggers.py
--rw-r--r--   0        0        0     2268 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/function/signature.py
--rw-r--r--   0        0        0      547 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/function/types.py
--rw-r--r--   0        0        0     2108 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/healthchecks/__init__.py
--rw-r--r--   0        0        0     1112 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/healthchecks/model.py
--rw-r--r--   0        0        0       87 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/monitor/__init__.py
--rw-r--r--   0        0        0     1650 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/monitor/logs.py
--rw-r--r--   0        0        0     4781 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/monitor/traces.py
--rw-r--r--   0        0        0       21 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/servicebus/data/__init__.py
--rw-r--r--   0        0        0     5636 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/servicebus/data/client.py
--rw-r--r--   0        0        0       21 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/servicebus/events/__init__.py
--rw-r--r--   0        0        0     4250 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/servicebus/events/client.py
--rw-r--r--   0        0        0       21 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/tablestorage/db/__init__.py
--rw-r--r--   0        0        0     1485 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/tablestorage/db/base_client.py
--rw-r--r--   0        0        0     1527 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/tablestorage/db/client.py
--rw-r--r--   0        0        0     1253 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/tablestorage/db/client_async.py
--rw-r--r--   0        0        0       47 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/tablestorage/tables/__init__.py
--rw-r--r--   0        0        0     2916 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/tablestorage/tables/client.py
--rw-r--r--   0        0        0     2516 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/tablestorage/tables/client_async.py
--rw-r--r--   0        0        0      521 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/tablestorage/tables/helpers.py
--rw-r--r--   0        0        0     2470 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/tablestorage/tables/operations.py
--rw-r--r--   0        0        0      248 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/testing/__init__.py
--rw-r--r--   0        0        0     3661 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/testing/assertions.py
--rw-r--r--   0        0        0     3661 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/testing/data.py
--rw-r--r--   0        0        0       27 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/transform/__init__.py
--rw-r--r--   0        0        0     1641 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/transform/data.py
--rw-r--r--   0        0        0     1968 2023-07-21 07:11:38.911779 warpzone_sdk-8.3.2/warpzone/transform/schema.py
--rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 warpzone_sdk-8.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1293 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/__init__.py
+-rw-r--r--   0        0        0       21 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/blobstorage/__init__.py
+-rw-r--r--   0        0        0     2844 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/blobstorage/client.py
+-rw-r--r--   0        0        0       24 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/enums/__init__.py
+-rw-r--r--   0        0        0      213 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/enums/topicenum.py
+-rw-r--r--   0        0        0       27 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/function/__init__.py
+-rw-r--r--   0        0        0     2108 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/function/functionize.py
+-rw-r--r--   0        0        0     3840 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/function/integrations.py
+-rw-r--r--   0        0        0     2223 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/function/monitor.py
+-rw-r--r--   0        0        0     2105 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/function/process.py
+-rw-r--r--   0        0        0       46 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/function/processors/__init__.py
+-rw-r--r--   0        0        0      781 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/function/processors/dependencies.py
+-rw-r--r--   0        0        0     2067 2023-07-21 11:21:06.514094 warpzone_sdk-8.3.3/warpzone/function/processors/outputs.py
+-rw-r--r--   0        0        0     1727 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/function/processors/triggers.py
+-rw-r--r--   0        0        0     2268 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/function/signature.py
+-rw-r--r--   0        0        0      547 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/function/types.py
+-rw-r--r--   0        0        0     2108 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/healthchecks/__init__.py
+-rw-r--r--   0        0        0     1112 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/healthchecks/model.py
+-rw-r--r--   0        0        0       87 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/monitor/__init__.py
+-rw-r--r--   0        0        0     1650 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/monitor/logs.py
+-rw-r--r--   0        0        0     4781 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/monitor/traces.py
+-rw-r--r--   0        0        0       21 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/servicebus/data/__init__.py
+-rw-r--r--   0        0        0     5636 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/servicebus/data/client.py
+-rw-r--r--   0        0        0       21 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/servicebus/events/__init__.py
+-rw-r--r--   0        0        0     4250 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/servicebus/events/client.py
+-rw-r--r--   0        0        0       21 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/tablestorage/db/__init__.py
+-rw-r--r--   0        0        0     1522 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/tablestorage/db/base_client.py
+-rw-r--r--   0        0        0     1960 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/tablestorage/db/client.py
+-rw-r--r--   0        0        0     1704 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/tablestorage/db/client_async.py
+-rw-r--r--   0        0        0       47 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/tablestorage/tables/__init__.py
+-rw-r--r--   0        0        0     2916 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/tablestorage/tables/client.py
+-rw-r--r--   0        0        0     2516 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/tablestorage/tables/client_async.py
+-rw-r--r--   0        0        0      521 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/tablestorage/tables/helpers.py
+-rw-r--r--   0        0        0     2470 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/tablestorage/tables/operations.py
+-rw-r--r--   0        0        0      248 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/testing/__init__.py
+-rw-r--r--   0        0        0     3661 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/testing/assertions.py
+-rw-r--r--   0        0        0     3661 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/testing/data.py
+-rw-r--r--   0        0        0       27 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/transform/__init__.py
+-rw-r--r--   0        0        0     1641 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/transform/data.py
+-rw-r--r--   0        0        0     1968 2023-07-21 11:21:06.518094 warpzone_sdk-8.3.3/warpzone/transform/schema.py
+-rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 warpzone_sdk-8.3.3/PKG-INFO
```

### Comparing `warpzone_sdk-8.3.2/pyproject.toml` & `warpzone_sdk-8.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "warpzone-sdk"
-version = "8.3.2"
+version = "8.3.3"
 description = "The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage"
 authors = ["Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "warpzone" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `warpzone_sdk-8.3.2/warpzone/__init__.py` & `warpzone_sdk-8.3.3/warpzone/__init__.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/blobstorage/client.py` & `warpzone_sdk-8.3.3/warpzone/blobstorage/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/function/functionize.py` & `warpzone_sdk-8.3.3/warpzone/function/functionize.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/function/integrations.py` & `warpzone_sdk-8.3.3/warpzone/function/integrations.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/function/monitor.py` & `warpzone_sdk-8.3.3/warpzone/function/monitor.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/function/process.py` & `warpzone_sdk-8.3.3/warpzone/function/process.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/function/processors/dependencies.py` & `warpzone_sdk-8.3.3/warpzone/function/processors/dependencies.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/function/processors/outputs.py` & `warpzone_sdk-8.3.3/warpzone/function/processors/outputs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/function/processors/triggers.py` & `warpzone_sdk-8.3.3/warpzone/function/processors/triggers.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/function/signature.py` & `warpzone_sdk-8.3.3/warpzone/function/signature.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/function/types.py` & `warpzone_sdk-8.3.3/warpzone/function/types.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/healthchecks/__init__.py` & `warpzone_sdk-8.3.3/warpzone/healthchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/healthchecks/model.py` & `warpzone_sdk-8.3.3/warpzone/healthchecks/model.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/monitor/logs.py` & `warpzone_sdk-8.3.3/warpzone/monitor/logs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/monitor/traces.py` & `warpzone_sdk-8.3.3/warpzone/monitor/traces.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/servicebus/data/client.py` & `warpzone_sdk-8.3.3/warpzone/servicebus/data/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/servicebus/events/client.py` & `warpzone_sdk-8.3.3/warpzone/servicebus/events/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/tablestorage/db/base_client.py` & `warpzone_sdk-8.3.3/warpzone/tablestorage/db/base_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     else:
         return ""
 
 
 def generate_dataframe_from_records(
     records: list[dict],
     blob_client: WarpzoneBlobClient,
-    filters: dict[str, object] = None,
 ) -> pd.DataFrame:
     # Return empty dataframe if the query result is empty
     if not records:
         return pd.DataFrame()
 
     # Download blobs and return the data stored if table entries contain blob_path
     if BLOB_NAME_COLUMN in records[0]:
@@ -35,12 +34,15 @@
             blob_data = blob_client.download(
                 DATA_CONTAINER_NAME, entity[BLOB_NAME_COLUMN]
             )
             df = pd.concat([df, blob_data.to_pandas()], ignore_index=True)
     else:
         df = pd.DataFrame.from_records(records)
 
-    if filters:
-        df = df[(df[filters.keys()] == filters.values()).all(axis=1)]
-        df = df.reset_index(drop=True)
-
     return df.drop(columns=["PartitionKey", "RowKey"])
+
+
+def filter_dataframe(df: pd.DataFrame, filters: dict[str, object]) -> pd.DataFrame:
+    df = df[(df[filters.keys()] == filters.values()).all(axis=1)]
+    df = df.reset_index(drop=True)
+
+    return df
```

### Comparing `warpzone_sdk-8.3.2/warpzone/tablestorage/db/client.py` & `warpzone_sdk-8.3.3/warpzone/tablestorage/db/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from functools import cache
+
 import pandas as pd
 
 from warpzone.blobstorage.client import WarpzoneBlobClient
 from warpzone.healthchecks import HealthCheckResult, check_health_of
 from warpzone.tablestorage.db import base_client
 from warpzone.tablestorage.tables.client import WarpzoneTableClient
 
@@ -19,28 +21,40 @@
 
     @classmethod
     def from_connection_string(cls, conn_str: str):
         table_client = WarpzoneTableClient.from_connection_string(conn_str)
         blob_client = WarpzoneBlobClient.from_connection_string(conn_str)
         return cls(table_client, blob_client)
 
+    @cache
+    def _query_to_pandas(self, table_name: str, query: str):
+        records = self._table_client.query(table_name, query)
+        df = base_client.generate_dataframe_from_records(records, self._blob_client)
+
+        return df
+
     def query(
         self,
         table_name: str,
         time_interval: pd.Interval = None,
         filters: dict[str, object] = None,
+        use_cache: bool = True,
     ):
-
         query = base_client.generate_query_string(time_interval)
 
-        records = self._table_client.query(table_name, query)
+        if use_cache:
+            df = self._query_to_pandas(table_name, query)
+        else:
+            # Use __wrapped__ to bypass cache
+            df = self._query_to_pandas.__wrapped__(self, table_name, query)
+
+        if filters:
+            df = base_client.filter_dataframe(df, filters)
 
-        return base_client.generate_dataframe_from_records(
-            records, self._blob_client, filters
-        )
+        return df
 
     def check_health(self) -> HealthCheckResult:
         """
         Pings the connections to the client's associated storage
         ressources in Azure.
         """
```

### Comparing `warpzone_sdk-8.3.2/warpzone/tablestorage/db/client_async.py` & `warpzone_sdk-8.3.3/warpzone/tablestorage/db/client_async.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from functools import cache
+
 import pandas as pd
 
 from warpzone.blobstorage.client import WarpzoneBlobClient
 from warpzone.tablestorage.db import base_client
 from warpzone.tablestorage.tables.client_async import WarpzoneTableClientAsync
 
 
@@ -18,21 +20,33 @@
 
     @classmethod
     def from_connection_string(cls, conn_str: str):
         table_client = WarpzoneTableClientAsync.from_connection_string(conn_str)
         blob_client = WarpzoneBlobClient.from_connection_string(conn_str)
         return cls(table_client, blob_client)
 
+    @cache
+    async def _query_to_pandas(self, table_name: str, query: str):
+        records = await self._table_client.query(table_name, query)
+        df = base_client.generate_dataframe_from_records(records, self._blob_client)
+
+        return df
+
     async def query(
         self,
         table_name: str,
         time_interval: pd.Interval = None,
         filters: dict[str, object] = None,
+        use_cache: bool = True,
     ):
-
         query = base_client.generate_query_string(time_interval)
 
-        records = await self._table_client.query(table_name, query)
+        if use_cache:
+            df = await self._query_to_pandas(table_name, query)
+        else:
+            # Use __wrapped__ to bypass cache
+            df = await self._query_to_pandas.__wrapped__(self, table_name, query)
+
+        if filters:
+            df = base_client.filter_dataframe(df, filters)
 
-        return base_client.generate_dataframe_from_records(
-            records, self._blob_client, filters
-        )
+        return df
```

### Comparing `warpzone_sdk-8.3.2/warpzone/tablestorage/tables/client.py` & `warpzone_sdk-8.3.3/warpzone/tablestorage/tables/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/tablestorage/tables/client_async.py` & `warpzone_sdk-8.3.3/warpzone/tablestorage/tables/client_async.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/tablestorage/tables/helpers.py` & `warpzone_sdk-8.3.3/warpzone/tablestorage/tables/helpers.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/tablestorage/tables/operations.py` & `warpzone_sdk-8.3.3/warpzone/tablestorage/tables/operations.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/testing/assertions.py` & `warpzone_sdk-8.3.3/warpzone/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/testing/data.py` & `warpzone_sdk-8.3.3/warpzone/testing/data.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/transform/data.py` & `warpzone_sdk-8.3.3/warpzone/transform/data.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/warpzone/transform/schema.py` & `warpzone_sdk-8.3.3/warpzone/transform/schema.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.2/PKG-INFO` & `warpzone_sdk-8.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warpzone-sdk
-Version: 8.3.2
+Version: 8.3.3
 Summary: The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage
 Author: Mikkel Ladekarl Folmersen Nygaard
 Author-email: mny@energinet.dk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

