# Comparing `tmp/dbt-rockset-0.1.6.tar.gz` & `tmp/dbt-rockset-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-rockset-0.1.6.tar", last modified: Thu Dec  8 22:11:20 2022, max compression
+gzip compressed data, was "dbt-rockset-0.2.0.tar", last modified: Thu Jul 20 21:57:44 2023, max compression
```

## Comparing `dbt-rockset-0.1.6.tar` & `dbt-rockset-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 julius     (501) staff       (20)        0 2022-12-08 22:11:20.355445 dbt-rockset-0.1.6/
--rw-r--r--   0 julius     (501) staff       (20)      282 2022-12-08 22:11:20.354940 dbt-rockset-0.1.6/PKG-INFO
--rw-r--r--   0 julius     (501) staff       (20)     2431 2022-12-07 02:03:19.000000 dbt-rockset-0.1.6/README.md
-drwxr-xr-x   0 julius     (501) staff       (20)        0 2022-12-08 22:11:20.294559 dbt-rockset-0.1.6/dbt/
--rw-r--r--   0 julius     (501) staff       (20)       65 2022-09-12 21:49:05.000000 dbt-rockset-0.1.6/dbt/__init__.py
-drwxr-xr-x   0 julius     (501) staff       (20)        0 2022-12-08 22:11:20.295900 dbt-rockset-0.1.6/dbt/adapters/
--rw-r--r--   0 julius     (501) staff       (20)       65 2022-09-12 21:49:05.000000 dbt-rockset-0.1.6/dbt/adapters/__init__.py
-drwxr-xr-x   0 julius     (501) staff       (20)        0 2022-12-08 22:11:20.314547 dbt-rockset-0.1.6/dbt/adapters/rockset/
--rw-r--r--   0 julius     (501) staff       (20)      505 2022-09-12 21:49:05.000000 dbt-rockset-0.1.6/dbt/adapters/rockset/__init__.py
--rw-r--r--   0 julius     (501) staff       (20)       19 2022-09-12 21:49:05.000000 dbt-rockset-0.1.6/dbt/adapters/rockset/__version__.py
--rw-r--r--   0 julius     (501) staff       (20)      696 2022-09-12 21:49:05.000000 dbt-rockset-0.1.6/dbt/adapters/rockset/column.py
--rw-r--r--   0 julius     (501) staff       (20)     4820 2022-12-07 02:11:36.000000 dbt-rockset-0.1.6/dbt/adapters/rockset/connections.py
--rw-r--r--   0 julius     (501) staff       (20)    30898 2022-12-07 02:11:43.000000 dbt-rockset-0.1.6/dbt/adapters/rockset/impl.py
--rw-r--r--   0 julius     (501) staff       (20)     1006 2022-09-12 21:49:05.000000 dbt-rockset-0.1.6/dbt/adapters/rockset/relation.py
-drwxr-xr-x   0 julius     (501) staff       (20)        0 2022-12-08 22:11:20.315888 dbt-rockset-0.1.6/dbt/include/
--rw-r--r--   0 julius     (501) staff       (20)       65 2022-09-12 21:49:05.000000 dbt-rockset-0.1.6/dbt/include/__init__.py
-drwxr-xr-x   0 julius     (501) staff       (20)        0 2022-12-08 22:11:20.318458 dbt-rockset-0.1.6/dbt/include/rockset/
--rw-r--r--   0 julius     (501) staff       (20)       51 2022-09-12 21:49:05.000000 dbt-rockset-0.1.6/dbt/include/rockset/__init__.py
--rw-r--r--   0 julius     (501) staff       (20)       91 2022-09-12 21:49:05.000000 dbt-rockset-0.1.6/dbt/include/rockset/dbt_project.yml
-drwxr-xr-x   0 julius     (501) staff       (20)        0 2022-12-08 22:11:20.320595 dbt-rockset-0.1.6/dbt/include/rockset/macros/
--rw-r--r--   0 julius     (501) staff       (20)      451 2022-09-12 21:49:05.000000 dbt-rockset-0.1.6/dbt/include/rockset/macros/adapters.sql
--rw-r--r--   0 julius     (501) staff       (20)      132 2022-09-12 21:49:05.000000 dbt-rockset-0.1.6/dbt/include/rockset/macros/catalog.sql
-drwxr-xr-x   0 julius     (501) staff       (20)        0 2022-12-08 22:11:20.326328 dbt-rockset-0.1.6/dbt/include/rockset/macros/materializations/
--rw-r--r--   0 julius     (501) staff       (20)     1044 2022-09-12 21:49:05.000000 dbt-rockset-0.1.6/dbt/include/rockset/macros/materializations/incremental.sql
--rw-r--r--   0 julius     (501) staff       (20)     1607 2022-09-12 21:49:05.000000 dbt-rockset-0.1.6/dbt/include/rockset/macros/materializations/seed.sql
--rw-r--r--   0 julius     (501) staff       (20)      655 2022-09-12 21:49:05.000000 dbt-rockset-0.1.6/dbt/include/rockset/macros/materializations/table.sql
--rw-r--r--   0 julius     (501) staff       (20)      512 2022-09-12 21:49:05.000000 dbt-rockset-0.1.6/dbt/include/rockset/macros/materializations/view.sql
-drwxr-xr-x   0 julius     (501) staff       (20)        0 2022-12-08 22:11:20.353992 dbt-rockset-0.1.6/dbt_rockset.egg-info/
--rw-r--r--   0 julius     (501) staff       (20)      282 2022-12-08 22:11:20.000000 dbt-rockset-0.1.6/dbt_rockset.egg-info/PKG-INFO
--rw-r--r--   0 julius     (501) staff       (20)      822 2022-12-08 22:11:20.000000 dbt-rockset-0.1.6/dbt_rockset.egg-info/SOURCES.txt
--rw-r--r--   0 julius     (501) staff       (20)        1 2022-12-08 22:11:20.000000 dbt-rockset-0.1.6/dbt_rockset.egg-info/dependency_links.txt
--rw-r--r--   0 julius     (501) staff       (20)       31 2022-12-08 22:11:20.000000 dbt-rockset-0.1.6/dbt_rockset.egg-info/requires.txt
--rw-r--r--   0 julius     (501) staff       (20)        4 2022-12-08 22:11:20.000000 dbt-rockset-0.1.6/dbt_rockset.egg-info/top_level.txt
--rw-r--r--   0 julius     (501) staff       (20)       38 2022-12-08 22:11:20.355665 dbt-rockset-0.1.6/setup.cfg
--rw-r--r--   0 julius     (501) staff       (20)      771 2022-12-08 22:10:43.000000 dbt-rockset-0.1.6/setup.py
+drwxr-xr-x   0 julius     (501) staff       (20)        0 2023-07-20 21:57:44.712128 dbt-rockset-0.2.0/
+-rw-r--r--   0 julius     (501) staff       (20)      282 2023-07-20 21:57:44.711580 dbt-rockset-0.2.0/PKG-INFO
+-rw-r--r--   0 julius     (501) staff       (20)     2431 2023-07-20 21:55:35.000000 dbt-rockset-0.2.0/README.md
+drwxr-xr-x   0 julius     (501) staff       (20)        0 2023-07-20 21:57:44.687476 dbt-rockset-0.2.0/dbt/
+-rw-r--r--   0 julius     (501) staff       (20)       65 2023-07-20 21:55:35.000000 dbt-rockset-0.2.0/dbt/__init__.py
+drwxr-xr-x   0 julius     (501) staff       (20)        0 2023-07-20 21:57:44.688611 dbt-rockset-0.2.0/dbt/adapters/
+-rw-r--r--   0 julius     (501) staff       (20)       65 2023-07-20 21:55:35.000000 dbt-rockset-0.2.0/dbt/adapters/__init__.py
+drwxr-xr-x   0 julius     (501) staff       (20)        0 2023-07-20 21:57:44.698072 dbt-rockset-0.2.0/dbt/adapters/rockset/
+-rw-r--r--   0 julius     (501) staff       (20)      505 2023-07-20 21:55:35.000000 dbt-rockset-0.2.0/dbt/adapters/rockset/__init__.py
+-rw-r--r--   0 julius     (501) staff       (20)       19 2023-07-20 21:55:35.000000 dbt-rockset-0.2.0/dbt/adapters/rockset/__version__.py
+-rw-r--r--   0 julius     (501) staff       (20)      694 2023-07-20 21:55:35.000000 dbt-rockset-0.2.0/dbt/adapters/rockset/column.py
+-rw-r--r--   0 julius     (501) staff       (20)     4800 2023-07-20 21:55:35.000000 dbt-rockset-0.2.0/dbt/adapters/rockset/connections.py
+-rw-r--r--   0 julius     (501) staff       (20)    31474 2023-07-20 21:55:35.000000 dbt-rockset-0.2.0/dbt/adapters/rockset/impl.py
+-rw-r--r--   0 julius     (501) staff       (20)     1093 2023-07-20 21:55:35.000000 dbt-rockset-0.2.0/dbt/adapters/rockset/relation.py
+drwxr-xr-x   0 julius     (501) staff       (20)        0 2023-07-20 21:57:44.698893 dbt-rockset-0.2.0/dbt/include/
+-rw-r--r--   0 julius     (501) staff       (20)       65 2023-07-20 21:55:35.000000 dbt-rockset-0.2.0/dbt/include/__init__.py
+drwxr-xr-x   0 julius     (501) staff       (20)        0 2023-07-20 21:57:44.701130 dbt-rockset-0.2.0/dbt/include/rockset/
+-rw-r--r--   0 julius     (501) staff       (20)       51 2023-07-20 21:55:35.000000 dbt-rockset-0.2.0/dbt/include/rockset/__init__.py
+-rw-r--r--   0 julius     (501) staff       (20)       91 2023-07-20 21:55:35.000000 dbt-rockset-0.2.0/dbt/include/rockset/dbt_project.yml
+drwxr-xr-x   0 julius     (501) staff       (20)        0 2023-07-20 21:57:44.703065 dbt-rockset-0.2.0/dbt/include/rockset/macros/
+-rw-r--r--   0 julius     (501) staff       (20)      451 2023-07-20 21:55:35.000000 dbt-rockset-0.2.0/dbt/include/rockset/macros/adapters.sql
+-rw-r--r--   0 julius     (501) staff       (20)      132 2023-07-20 21:55:35.000000 dbt-rockset-0.2.0/dbt/include/rockset/macros/catalog.sql
+drwxr-xr-x   0 julius     (501) staff       (20)        0 2023-07-20 21:57:44.706508 dbt-rockset-0.2.0/dbt/include/rockset/macros/materializations/
+-rw-r--r--   0 julius     (501) staff       (20)     1044 2023-07-20 21:55:35.000000 dbt-rockset-0.2.0/dbt/include/rockset/macros/materializations/incremental.sql
+-rw-r--r--   0 julius     (501) staff       (20)     1607 2023-07-20 21:55:35.000000 dbt-rockset-0.2.0/dbt/include/rockset/macros/materializations/seed.sql
+-rw-r--r--   0 julius     (501) staff       (20)      655 2023-07-20 21:55:35.000000 dbt-rockset-0.2.0/dbt/include/rockset/macros/materializations/table.sql
+-rw-r--r--   0 julius     (501) staff       (20)      512 2023-07-20 21:55:35.000000 dbt-rockset-0.2.0/dbt/include/rockset/macros/materializations/view.sql
+drwxr-xr-x   0 julius     (501) staff       (20)        0 2023-07-20 21:57:44.710824 dbt-rockset-0.2.0/dbt_rockset.egg-info/
+-rw-r--r--   0 julius     (501) staff       (20)      282 2023-07-20 21:57:44.000000 dbt-rockset-0.2.0/dbt_rockset.egg-info/PKG-INFO
+-rw-r--r--   0 julius     (501) staff       (20)      822 2023-07-20 21:57:44.000000 dbt-rockset-0.2.0/dbt_rockset.egg-info/SOURCES.txt
+-rw-r--r--   0 julius     (501) staff       (20)        1 2023-07-20 21:57:44.000000 dbt-rockset-0.2.0/dbt_rockset.egg-info/dependency_links.txt
+-rw-r--r--   0 julius     (501) staff       (20)       52 2023-07-20 21:57:44.000000 dbt-rockset-0.2.0/dbt_rockset.egg-info/requires.txt
+-rw-r--r--   0 julius     (501) staff       (20)        4 2023-07-20 21:57:44.000000 dbt-rockset-0.2.0/dbt_rockset.egg-info/top_level.txt
+-rw-r--r--   0 julius     (501) staff       (20)       38 2023-07-20 21:57:44.712284 dbt-rockset-0.2.0/setup.cfg
+-rw-r--r--   0 julius     (501) staff       (20)      794 2023-07-20 21:55:35.000000 dbt-rockset-0.2.0/setup.py
```

### Comparing `dbt-rockset-0.1.6/README.md` & `dbt-rockset-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt-rockset-0.1.6/dbt/adapters/rockset/column.py` & `dbt-rockset-0.2.0/dbt/adapters/rockset/column.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 
 from dbt.adapters.base.column import Column
-from dbt.exceptions import RuntimeException
+from dbt.exceptions import DbtRuntimeError
 
 import rockset
 
 
 @dataclass
 class RocksetColumn(Column):
     def is_integer(self) -> bool:
@@ -18,10 +18,10 @@
         return self.dtype.lower() in ['float']
 
     def is_string(self):
         return self.dtype.lower() in ['string']
 
     def string_size(self) -> int:
         if not self.is_string():
-            raise RuntimeException("Called string_size() on non-string field!")
+            raise DbtRuntimeError("Called string_size() on non-string field!")
 
         return rockset.Client.MAX_FIELD_VALUE_BYTES
```

### Comparing `dbt-rockset-0.1.6/dbt/adapters/rockset/connections.py` & `dbt-rockset-0.2.0/dbt/adapters/rockset/connections.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 from dbt.adapters.base import BaseConnectionManager
 from dbt.clients import agate_helper
 from dbt.contracts.connection import AdapterResponse, Connection
 from dbt.logger import GLOBAL_LOGGER as logger
 
 import agate
 import dbt
-import rockset
-from rockset import Client, Q, F, sql
+import rockset_sqlalchemy as sql
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 
 RS_APISERVERS = [
     'api.euc1a1.rockset.com',
     'api.rs2.usw2.rockset.com',
     'api.usw2a1.rockset.com',
```

### Comparing `dbt-rockset-0.1.6/dbt/adapters/rockset/impl.py` & `dbt-rockset-0.2.0/dbt/adapters/rockset/impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 from time import sleep, time
 from typing import List, Optional, Set
 
 
 OK = 200
 NOT_FOUND = 404
 ASYNC_OPTIONS = {
-                "client_timeout_ms": 1000,  # arbitrary
-                "timeout_ms": 1800000,
-                "max_initial_results": 1,
-            }
+    "client_timeout_ms": 1000,  # arbitrary
+    "timeout_ms": 1800000,
+    "max_initial_results": 1,
+}
 
 
 class RocksetAdapter(BaseAdapter):
     RELATION_TYPES = {
         "TABLE": RelationType.Table,
     }
 
@@ -69,59 +69,60 @@
     @classmethod
     def date_function(cls):
         return "CURRENT_TIMESTAMP()"
 
     def create_schema(self, relation: RocksetRelation) -> None:
         rs = self._rs_client()
         logger.debug('Creating workspace "{}"', relation.schema)
-        rs.Workspace.create(relation.schema)
+        rs.Workspaces.create(name=relation.schema)
 
     def drop_schema(self, relation: RocksetRelation) -> None:
         rs = self._rs_client()
         ws = relation.schema
         logger.info('Dropping workspace "{}"', ws)
 
         # Drop all views in the ws
         for view in self._list_views(ws):
             self._delete_view_recursively(ws, view)
 
         # Drop all aliases in the ws
-        for alias in rs.Alias.list(workspace=ws):
+        for alias in rs.Aliases.workspace_aliases(workspace=ws):
             self._delete_alias(ws, alias.name)
 
         # Drop all collections in the ws
-        for collection in rs.Collection.list(workspace=ws):
-            self._delete_collection(ws, collection.name, wait_until_deleted=False)
+        for collection in rs.Collections.workspace_collections(workspace=ws).data:
+            self._delete_collection(
+                ws, collection.name, wait_until_deleted=False)
 
         try:
             # Wait until the ws has 0 collections. We do this so deletion of multiple collections
             # can happen in parallel
             while True:
-                workspace = rs.Workspace.retrieve(ws)
+                workspace = rs.Workspaces.get(workspace=ws).data
                 if workspace.collection_count == 0:
                     break
                 logger.debug(
                     f"Waiting for ws {ws} to have 0 collections, has {workspace.collection_count}"
                 )
                 sleep(3)
 
-            rs.Workspace.delete(ws)
+            rs.Workspaces.delete(workspace=ws)
         except Exception as e:
             logger.debug(f"Caught exception of type {e.__class__}")
             # Workspace does not exist
-            if isinstance(e, rockset.exception.Error) and e.code == NOT_FOUND:
+            if isinstance(e, rockset.exceptions.ApiException) and e.status == NOT_FOUND:
                 pass
             else:  # Unexpected error
                 raise e
 
     # Required by BaseAdapter
     @available
     def list_schemas(self, database: str) -> List[str]:
         rs = self._rs_client()
-        return [ws.name for ws in rs.Workspace.list()]
+        return [ws.name for ws in rs.Workspaces.list().data]
 
     # Relation/Collection related methods
     def truncate_relation(self, relation: RocksetRelation) -> None:
         raise dbt.exceptions.NotImplementedException(
             "`truncate` is not implemented for this adapter!"
         )
 
@@ -158,18 +159,19 @@
     @available.parse(lambda *a, **k: "")
     def get_collection(self, relation) -> RocksetRelation:
         ws = relation.schema
         cname = relation.identifier
 
         try:
             rs = self._rs_client()
-            existing_collection = rs.Collection.retrieve(cname, workspace=ws)
+            existing_collection = rs.Collections.get(
+                collection=cname, workspace=ws)
             return self._rs_collection_to_relation(existing_collection)
         except Exception as e:
-            if e.code == NOT_FOUND:  # Collection does not exist
+            if hasattr(e, "status") and e.status == NOT_FOUND:  # Collection does not exist
                 return None
             else:  # Unexpected error
                 raise e
 
     # Required by BaseAdapter
     def list_relations_without_caching(
         self, schema_relation: RocksetRelation
@@ -184,15 +186,16 @@
     def list_relations(
         self, database: Optional[str], schema: str
     ) -> List[RocksetRelation]:
 
         rs = self._rs_client()
         relations = []
 
-        collections = rs.Collection.list(workspace=schema)
+        collections = rs.Collections.workspace_collections(
+            workspace=schema).data
         for collection in collections:
             relations.append(self._rs_collection_to_relation(collection))
         return relations
 
     # Required by BaseAdapter
     def get_columns_in_relation(self, relation: RocksetRelation) -> List[RocksetColumn]:
         logger.debug(f"Getting columns in relation {relation.identifier}")
@@ -249,15 +252,15 @@
             "stats:bytes:include",
             "column_type",
             "column_name",
             "column_index",
         ]
         catalog_rows = []
         for relation in schemas:
-            for collection in rs.Collection.list(workspace=relation.schema):
+            for collection in rs.Collections.workspace_collections(workspace=relation.schema).data:
                 rel = self.Relation.create(
                     schema=collection.workspace, identifier=collection.name
                 )
                 col_types = self._get_types_in_relation(rel)
                 for i, c in enumerate(col_types):
                     catalog_rows.append(
                         [
@@ -278,15 +281,16 @@
                             i,
                         ]
                     )
         catalog_table = agate.Table(
             rows=catalog_rows,
             column_names=columns,
             column_types=agate.TypeTester(
-                force={"table_database": agate.Text(cast_nulls=False, null_values=[])}
+                force={"table_database": agate.Text(
+                    cast_nulls=False, null_values=[])}
             ),
         )
 
         return catalog_table, []
 
     def expand_column_types(
         self, goal: RocksetRelation, current: RocksetRelation
@@ -324,15 +328,15 @@
             self._delete_alias(ws, cname)
 
         if self._does_view_exist(ws, cname):
             self._delete_view_recursively(ws, cname)
 
         logger.debug(f"Creating collection {ws}.{cname}")
 
-        c = rs.Collection.create(cname, workspace=ws)
+        c = rs.Collections.create_s3_collection(name=cname, workspace=ws)
         self._wait_until_collection_ready(ws, cname)
 
         # Run an INSERT INTO statement and wait for it to be fully ingested
         relation = self._rs_collection_to_relation(c)
         iis_query_id = self._execute_iis_query_and_wait_for_docs(relation, sql)
 
     # Used by dbt seed
@@ -349,30 +353,34 @@
             d = dict(row.dict())
             for k, v in d.items():
                 d[k] = self._convert_agate_data_type(v)
             json_docs.append(d)
 
         # The check for a view should happen before this point
         if self._does_view_exist(ws, cname):
-            raise dbt.exceptions.Exception(f"InternalError : View {ws}.{cname} exists")
+            raise dbt.exceptions.Exception(
+                f"InternalError : View {ws}.{cname} exists")
 
         # Create the Rockset collection
         if not self._does_collection_exist(ws, cname):
             rs = self._rs_client()
-            rs.Collection.create(cname, workspace=ws)
+            rs.Collections.create_s3_collection(name=cname, workspace=ws)
         self._wait_until_collection_ready(ws, cname)
 
         # Write the results to the collection and wait until the docs are ingested
         body = {"data": json_docs}
         write_api_endpoint = f"/v1/orgs/self/ws/{ws}/collections/{cname}/docs"
-        resp = json.loads(self._send_rs_request("POST", write_api_endpoint, body).text)
+        resp = json.loads(self._send_rs_request(
+            "POST", write_api_endpoint, body).text)
         self._wait_until_past_commit_fence(ws, cname, resp["last_offset"])
 
     def _convert_agate_data_type(self, v):
-        if isinstance(v, str):
+        if v is None:
+            return None
+        elif isinstance(v, str):
             return v
         elif isinstance(v, Decimal):
             return float(v)
         elif isinstance(v, datetime.datetime):
             return str(v)
         elif isinstance(v, datetime.date):
             return str(v)
@@ -416,15 +424,15 @@
         iis_query_id = self._execute_iis_query_and_wait_for_docs(relation, sql)
 
     ###
     # Internal Rockset helper methods
     ###
 
     def _rs_client(self):
-        return self.connections.get_thread_connection().handle._client()
+        return self.connections.get_thread_connection().handle._client
 
     def _rs_api_key(self):
         return self.connections.get_thread_connection().credentials.api_key
 
     def _rs_vi_rrn(self):
         return self.connections.get_thread_connection().credentials.vi_rrn
 
@@ -442,15 +450,16 @@
     def _execute_iis_query_and_wait_for_docs(self, relation, sql):
         query_id, num_docs_inserted = self._execute_iis_query(relation, sql)
         if num_docs_inserted > 0:
             self._wait_until_iis_query_processed(
                 relation.schema, relation.identifier, query_id
             )
         else:
-            logger.info(f"Query {query_id} inserted 0 docs; no ingest to wait for.")
+            logger.info(
+                f"Query {query_id} inserted 0 docs; no ingest to wait for.")
 
     # Execute a query not using the SQL cursor, but by hitting the REST api. This should be done
     # if you need the QueryResponse object returned
     # Returns: query_id (str), num_docs_inserted (int)
     def _execute_iis_query(self, relation, sql):
         iis_sql = f"INSERT INTO {relation} {sql}"
         logger.debug(f"Executing sql: {iis_sql}")
@@ -476,26 +485,28 @@
         if json_resp["status"] == "QUEUED" or json_resp["status"] == "RUNNING":
             self._wait_until_async_query_completed(query_id)
             # Async IIS queries do not have results saved in s3 so just assume docs were inserted
             # If this behavior changes in the future, then get the results of the async IIS query
             # and get num_docs_inserted
             return query_id, 1
 
-        assert len(json_resp["results"]) == 1, f"IIS queries should return only one document but got {len(json_resp['results'])}"
+        assert len(
+            json_resp["results"]) == 1, f"IIS queries should return only one document but got {len(json_resp['results'])}"
 
         return query_id, json_resp["results"][0]["num_docs_inserted"]
 
     def _wait_until_collection_does_not_exist(self, cname, ws):
         while True:
             try:
-                c = self._rs_client().Collection.retrieve(cname, workspace=ws)
-                logger.debug(f"Waiting for collection {ws}.{cname} to be deleted...")
+                self._rs_client().Collections.get(collection=cname, workspace=ws)
+                logger.debug(
+                    f"Waiting for collection {ws}.{cname} to be deleted...")
                 sleep(3)
             except Exception as e:
-                if e.code == NOT_FOUND:  # Collection does not exist
+                if hasattr(e, "status") and e.status == NOT_FOUND:  # Collection does not exist
                     return
                 raise e
 
     def _wait_until_view_does_not_exist(self, ws, view):
         while True:
             if self._does_view_exist(ws, view):
                 logger.debug(f"Waiting for view {ws}.{view} to be deleted")
@@ -513,31 +524,36 @@
                 logger.debug(
                     f"Collection {ws}.{cname} does not exist. This is likely a transient consistency error."
                 )
                 sleep(sleep_secs)
                 total_sleep_time += sleep_secs
                 continue
 
-            c = self._rs_client().Collection.retrieve(cname, workspace=ws)
-            if c.describe().data["status"] == "READY":
+            c = self._rs_client().Collections.get(collection=cname, workspace=ws)
+            if c.data["status"] == "READY":
                 logger.debug(f"{ws}.{cname} is ready!")
                 return
             else:
-                logger.debug(f"Waiting for collection {ws}.{cname} to become ready...")
+                logger.debug(
+                    f"Waiting for collection {ws}.{cname} to become ready...")
                 sleep(sleep_secs)
                 total_sleep_time += sleep_secs
 
         raise dbt.exceptions.Exception(
             f"Waited more than {max_wait_time_secs} secs for {ws}.{cname} to become ready. Something is wrong."
         )
 
     def _rs_collection_to_relation(self, collection):
+
         if collection is None:
             return None
 
+        if hasattr(collection, "data"):
+            collection = collection.data  # TODO: remove the need for this
+
         return self.Relation.create(
             database=None,
             schema=collection.workspace,
             identifier=collection.name,
             type="table",
             quote_policy=RocksetQuotePolicy(),
         )
@@ -549,47 +565,47 @@
                 sleep(3)
             else:
                 break
 
     def _wait_until_collection_deleted(self, ws, cname):
         while True:
             if self._does_collection_exist(ws, cname):
-                logger.debug(f"Waiting for collection {ws}.{cname} to be deleted")
+                logger.debug(
+                    f"Waiting for collection {ws}.{cname} to be deleted")
                 sleep(3)
             else:
                 break
 
     def _delete_collection(self, ws, cname, wait_until_deleted=True):
         rs = self._rs_client()
 
         for ref_view in self._get_referencing_views(ws, cname):
             self._delete_view_recursively(ref_view[0], ref_view[1])
 
         try:
-            c = rs.Collection.retrieve(cname, workspace=ws)
-            c.drop()
+            c = rs.Collections.delete(collection=cname, workspace=ws)
 
             if wait_until_deleted:
-                self._wait_until_collection_deleted(ws, cname)
+                self._wait_until_collection_deleted(
+                    ws, cname)
         except Exception as e:
-            if e.code != NOT_FOUND:
+            if hasattr(e, "status") and e.status != NOT_FOUND:
                 raise e  # Unexpected error
 
     def _delete_alias(self, ws, alias):
         rs = self._rs_client()
 
         for ref_view in self._get_referencing_views(ws, alias):
             self._delete_view_recursively(ref_view[0], ref_view[1])
 
         try:
-            a = rs.Alias.retrieve(alias, workspace=ws)
-            a.drop()
+            rs.Aliases.delete(alias=alias, workspace=ws)
             self._wait_until_alias_deleted(ws, alias)
         except Exception as e:
-            if e.code != NOT_FOUND:
+            if hasattr(e, "status") and e.status != NOT_FOUND:
                 raise e  # Unexpected error
 
     def _wait_until_past_commit_fence(self, ws, cname, fence):
         endpoint = (
             f"/v1/orgs/self/ws/{ws}/collections/{cname}/offsets/commit?fence={fence}"
         )
         while True:
@@ -609,32 +625,34 @@
                 sleep(3)
 
     def _wait_until_async_query_completed(self, query_id):
         endpoint = f"/v1/orgs/self/queries/{query_id}"
         while True:
             query_resp = self._send_rs_request("GET", endpoint)
             query_data = json.loads(query_resp.text)
-            
-            status = query_data.get("data").get("status") if "data" in query_data else None
+
+            status = query_data.get("data").get(
+                "status") if "data" in query_data else None
             if status == "COMPLETED":
                 return
             elif status == "ERROR" or status == "CANCELLED":
-                raise Exception(f"IIS query did not complete successfully. Query data: {query_resp.text}")
+                raise Exception(
+                    f"IIS query did not complete successfully. Query data: {query_resp.text}")
             else:
                 logger.debug(
                     f"Insert Into Query not completed yet"
                 )
                 sleep(3)
 
     def _wait_until_iis_fully_ingested(self, ws, cname, query_id):
         endpoint = f"/v1/orgs/self/queries/{query_id}"
         while True:
             query_resp = self._send_rs_request("GET", endpoint)
             query_data = json.loads(query_resp.text)
-            
+
             last_offset = query_data.get("last_offset")
             if last_offset is not None:
                 return last_offset
             else:
                 logger.debug(
                     f"Insert Into Query not yet finished processing; last offset not present"
                 )
@@ -681,29 +699,29 @@
             raise Exception(
                 f"throwing from 332 with status_code {response.status_code} and text {response.text}"
             )
 
     def _does_alias_exist(self, ws, alias):
         rs = self._rs_client()
         try:
-            rs.Alias.retrieve(workspace=ws, name=alias)
+            rs.Aliases.get(alias=alias, workspace=ws)
             return True
         except Exception as e:
-            if isinstance(e, rockset.exception.InputError) and e.code == NOT_FOUND:
+            if e.status == NOT_FOUND:
                 return False
             else:
                 raise e
 
     def _does_collection_exist(self, ws, cname):
         rs = self._rs_client()
         try:
-            rs.Collection.retrieve(workspace=ws, name=cname)
+            rs.Collections.get(workspace=ws, collection=cname)
             return True
         except Exception as e:
-            if isinstance(e, rockset.exception.InputError) and e.code == NOT_FOUND:
+            if e.status == NOT_FOUND:
                 return False
             else:
                 raise e
 
     def _create_view(self, ws, view, sql):
         # Check if alias or collection exist with same name
         rs = self._rs_client()
@@ -757,30 +775,32 @@
         sleep_secs = 3
         total_sleep_time = 0
 
         endpoint = f"{self._views_endpoint(ws)}/{view}"
         while total_sleep_time < max_wait_time_secs:
             if not self._does_view_exist(ws, view):
                 logger.debug(
-                    f"View {ws}.{cname} does not exist. This is likely a transient consistency error."
+                    f"View {ws}.{view} does not exist. This is likely a transient consistency error."
                 )
                 sleep(sleep_secs)
                 total_sleep_time += sleep_secs
                 continue
 
             resp = self._send_rs_request("GET", endpoint)
             view_json = json.loads(resp.text)["data"]
             state = view_json["state"]
 
             if state == "SYNCING":
-                logger.debug(f"Waiting for view {ws}.{view} to be fully synced")
+                logger.debug(
+                    f"Waiting for view {ws}.{view} to be fully synced")
                 sleep(sleep_secs)
                 total_sleep_time += sleep_secs
             else:
-                logger.debug(f"View {ws}.{view} is synced and ready to be queried")
+                logger.debug(
+                    f"View {ws}.{view} is synced and ready to be queried")
                 return
 
         raise dbt.exceptions.Exception(
             f"Waited more than {max_wait_time_secs} secs for view {ws}.{view} to become synced. Something is wrong."
         )
 
     # Overridden because Rockset generates columns not added during testing.
@@ -794,19 +814,21 @@
 
         names: List[str]
         # columns generated by Rockset
         skip_cmp_columns: Set[str] = {"_event_time", "_id", "_meta"}
         if column_names is None:
             columns = self.get_columns_in_relation(relation_a)
             names = sorted(
-                (self.quote(c.name) for c in columns if c.name not in skip_cmp_columns)
+                (self.quote(c.name)
+                 for c in columns if c.name not in skip_cmp_columns)
             )
         else:
             names = sorted(
-                (self.quote(n) for n in column_names if n not in skip_cmp_columns)
+                (self.quote(n)
+                 for n in column_names if n not in skip_cmp_columns)
             )
         columns_csv = ", ".join(names)
 
         sql = COLUMNS_EQUAL_SQL.format(
             columns=columns_csv,
             relation_a=str(relation_a),
             relation_b=str(relation_b),
```

### Comparing `dbt-rockset-0.1.6/dbt/adapters/rockset/relation.py` & `dbt-rockset-0.2.0/dbt/adapters/rockset/relation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from dbt.adapters.base.relation import BaseRelation, Policy
 
 import traceback
 from typing import List, Optional
 
 
 @dataclass
@@ -17,16 +17,18 @@
     database: bool = False
     schema: bool = True
     identifier: bool = True
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class RocksetRelation(BaseRelation):
-    quote_policy: RocksetQuotePolicy = RocksetQuotePolicy()
-    include_policy: RocksetIncludePolicy = RocksetIncludePolicy()
+    quote_policy: RocksetQuotePolicy = field(
+        default_factory=lambda: RocksetQuotePolicy())
+    include_policy: RocksetIncludePolicy = field(
+        default_factory=lambda: RocksetIncludePolicy())
 
     # We override this function with a very simple implementation. Database is not a concept
     # in Rockset, so we do not make such a comparison
     def matches(
         self,
         database: Optional[str] = None,
         schema: Optional[str] = None,
```

### Comparing `dbt-rockset-0.1.6/dbt/include/rockset/macros/materializations/incremental.sql` & `dbt-rockset-0.2.0/dbt/include/rockset/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-rockset-0.1.6/dbt/include/rockset/macros/materializations/seed.sql` & `dbt-rockset-0.2.0/dbt/include/rockset/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-rockset-0.1.6/dbt/include/rockset/macros/materializations/table.sql` & `dbt-rockset-0.2.0/dbt/include/rockset/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-rockset-0.1.6/dbt/include/rockset/macros/materializations/view.sql` & `dbt-rockset-0.2.0/dbt/include/rockset/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-rockset-0.1.6/dbt_rockset.egg-info/SOURCES.txt` & `dbt-rockset-0.2.0/dbt_rockset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-rockset-0.1.6/setup.py` & `dbt-rockset-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import find_packages
 from distutils.core import setup
 
 package_name = "dbt-rockset"
-package_version = "0.1.6"
+package_version = "0.2.0"
 description = """The Rockset adapter plugin for dbt (data build tool)"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=description,
@@ -19,11 +19,11 @@
         'dbt': [
             'include/rockset/macros/*.sql',
             'include/rockset/macros/**/*.sql',
             'include/rockset/dbt_project.yml',
         ]
     },
     install_requires=[
-        "dbt-core>=0.18",
-        "rockset==0.8.10"
+        "dbt-core>=1.5.0, <2.0",
+        "rockset-sqlalchemy>=0.0.1, <1.0"
     ]
 )
```

