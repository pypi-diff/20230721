# Comparing `tmp/pyntone-0.2.2.tar.gz` & `tmp/pyntone-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyntone-0.2.2.tar", last modified: Sun Apr 16 13:06:07 2023, max compression
+gzip compressed data, was "pyntone-0.3.0.tar", last modified: Fri Jul 21 01:38:09 2023, max compression
```

## Comparing `pyntone-0.2.2.tar` & `pyntone-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:06:07.101910 pyntone-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-16 13:05:50.000000 pyntone-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-16 13:06:07.101910 pyntone-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-16 13:05:50.000000 pyntone-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:06:07.101910 pyntone-0.2.2/pyntone/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:06:07.101910 pyntone-0.2.2/pyntone/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/client/bulk_request_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19169 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/client/record_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:06:07.101910 pyntone-0.2.2/pyntone/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/http/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/kintone_request_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/kintone_rest_api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:06:07.101910 pyntone-0.2.2/pyntone/types/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/types/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/types/record.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyntone/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:06:07.101910 pyntone-0.2.2/pyntone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-16 13:06:07.000000 pyntone-0.2.2/pyntone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-16 13:06:07.000000 pyntone-0.2.2/pyntone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 13:06:07.000000 pyntone-0.2.2/pyntone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-16 13:06:07.000000 pyntone-0.2.2/pyntone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-16 13:06:07.000000 pyntone-0.2.2/pyntone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-16 13:05:50.000000 pyntone-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-16 13:06:07.101910 pyntone-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:06:07.101910 pyntone-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:05:50.000000 pyntone-0.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-04-16 13:05:50.000000 pyntone-0.2.2/tests/test_record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:38:09.447304 pyntone-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-21 01:37:58.000000 pyntone-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-21 01:38:09.447304 pyntone-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-21 01:37:58.000000 pyntone-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:38:09.447304 pyntone-0.3.0/pyntone/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:38:09.447304 pyntone-0.3.0/pyntone/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/client/app_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/client/bulk_request_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/client/file_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18029 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/client/record_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:38:09.447304 pyntone-0.3.0/pyntone/client/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/client/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:38:09.447304 pyntone-0.3.0/pyntone/client/types/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/client/types/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/client/types/app/customize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:38:09.447304 pyntone-0.3.0/pyntone/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/http/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/kintone_request_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/kintone_rest_api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:38:09.447304 pyntone-0.3.0/pyntone/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/types/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/types/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:38:09.447304 pyntone-0.3.0/pyntone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-21 01:38:09.000000 pyntone-0.3.0/pyntone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-21 01:38:09.000000 pyntone-0.3.0/pyntone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:38:09.000000 pyntone-0.3.0/pyntone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 01:38:09.000000 pyntone-0.3.0/pyntone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-21 01:38:09.000000 pyntone-0.3.0/pyntone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-21 01:38:09.447304 pyntone-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:38:09.447304 pyntone-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:37:58.000000 pyntone-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-21 01:37:58.000000 pyntone-0.3.0/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-21 01:37:58.000000 pyntone-0.3.0/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-21 01:37:58.000000 pyntone-0.3.0/tests/test_record.py
```

### Comparing `pyntone-0.2.2/LICENSE` & `pyntone-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyntone-0.2.2/PKG-INFO` & `pyntone-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyntone
-Version: 0.2.2
+Version: 0.3.0
 Summary: API client for Kintone REST API.
 Home-page: https://github.com/kashi03/pyntone
 Author: kashi03
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyntone-0.2.2/pyntone/client/bulk_request_client.py` & `pyntone-0.3.0/pyntone/client/bulk_request_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,60 +7,62 @@
     'record',
     'records',
     'record/status',
     'records/status',
     'record/assignees',
 ]
 
-HttpMethod = Literal[
-    'POST',
-    'PUT',
-    'DELETE'
-]
+HttpMethod = Literal['POST', 'PUT', 'DELETE']
+
 
 class ApiRequestParameter(TypedDict):
     method: HttpMethod
     api: str
     payload: dict
 
+
 class EndopintRequestParameter(TypedDict):
     method: HttpMethod
     endpoint_name: EndpointName
     payload: dict
 
+
 class BulkRequestClient:
     def __init__(
         self,
         client: HttpClent,
         guest_space_id: Union[int, str, None] = None,
     ) -> None:
         self.client = client
         self.guest_space_id = guest_space_id
         self.REQUESTS_LENGTH_LIMIT = 20
-    
+
     def send(
         self,
-        requests: Union[list[ApiRequestParameter], list[EndopintRequestParameter], list[Union[ApiRequestParameter, EndopintRequestParameter]]]
+        requests: Union[
+            list[ApiRequestParameter],
+            list[EndopintRequestParameter],
+            list[Union[ApiRequestParameter, EndopintRequestParameter]],
+        ],
     ):
         request_list = []
         for request in requests:
             endpoint_name = request.get('endpoint_name')
             if endpoint_name is not None:
-                request_list.append({
-                    'method': request['method'],
-                    'api': self.__build_path_with_guest_space_id(endpoint_name),
-                    'payload': request['payload']
-                })
+                request_list.append(
+                    {
+                        'method': request['method'],
+                        'api': self.__build_path_with_guest_space_id(endpoint_name),
+                        'payload': request['payload'],
+                    }
+                )
             else:
                 request_list.append(request)
-        
+
         path = self.__build_path_with_guest_space_id('bulkRequest')
-        params = KintoneRequestParams(
-            requests=request_list
-        )
+        params = KintoneRequestParams(requests=request_list)
         return self.client.post(path, params)
 
     def __build_path_with_guest_space_id(self, endpoint_name: str) -> str:
         return build_path(
-            endpoint_name=endpoint_name,
-            guest_space_id=self.guest_space_id
-        )
+            endpoint_name=endpoint_name, guest_space_id=self.guest_space_id
+        )
```

### Comparing `pyntone-0.2.2/pyntone/client/record_client.py` & `pyntone-0.3.0/pyntone/client/record_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,572 +1,495 @@
 from typing import Literal, Optional, Union
 
-from pyntone.client.bulk_request_client import (BulkRequestClient,
-                                                EndopintRequestParameter)
+from pyntone.client.bulk_request_client import (
+    BulkRequestClient,
+    EndopintRequestParameter,
+)
 from pyntone.http.http_client import HttpClent, KintoneRequestParams
 from pyntone.types import AppID, CommentID, RecordID, Revision
-from pyntone.types.record import (Comment, DeleteRecordParameter,
-                                  RecordForParameter, UpdateKey,
-                                  UpdateKeyRecordForParameter,
-                                  UpdateRecordForParameter,
-                                  UpdateRecordStatusParameter)
+from pyntone.types.record import (
+    Comment,
+    DeleteRecordParameter,
+    RecordForParameter,
+    UpdateKey,
+    UpdateKeyRecordForParameter,
+    UpdateRecordForParameter,
+    UpdateRecordStatusParameter,
+)
 from pyntone.url import build_path
 
 ADD_RECORDS_LIMIT = 100
 UPDATE_RECORDS_LIMIT = 100
 DELETE_RECORDS_LIMIT = 100
 GET_RECORDS_LIMIT = 500
 
+
 class RecordClient:
     def __init__(
         self,
         client: HttpClent,
         bulk_request_client: BulkRequestClient,
-        guest_space_id: Union[int, str, None]
+        guest_space_id: Union[int, str, None],
     ) -> None:
         self.client = client
         self.bulk_request_client = bulk_request_client
         self.guest_space_id = guest_space_id
         self.did_warn_maximum_offset_value = False
-    
+
     def get_record(self, app: AppID, record_id: RecordID):
         path = self.__build_path_with_guest_space_id(endpoint_name='record')
-        params = KintoneRequestParams(
-            app=app,
-            id=record_id
-        )
+        params = KintoneRequestParams(app=app, id=record_id)
         return self.client.get(path, params)
 
     def add_record(self, app: AppID, record: Optional[RecordForParameter] = None):
         path = self.__build_path_with_guest_space_id(endpoint_name='record')
-        params = KintoneRequestParams(
-            app=app,
-            record=record
-        )
+        params = KintoneRequestParams(app=app, record=record)
         return self.client.post(path, params)
 
     def update_record(
         self,
         app: AppID,
         record_id: Optional[RecordID] = None,
         update_key: Optional[UpdateKey] = None,
         record: Optional[RecordForParameter] = None,
-        revision: Optional[Revision] = None
+        revision: Optional[Revision] = None,
     ):
         if record_id is None and update_key is None:
             raise ValueError()
         path = self.__build_path_with_guest_space_id(endpoint_name='record')
         params = KintoneRequestParams(
             app=app,
             id=record_id,
-            update_key=update_key,
+            updateKey=update_key,
             record=record,
-            revision=revision
+            revision=revision,
         )
         return self.client.put(path, params)
 
     def upsert_record(
         self,
         app: AppID,
         update_key: UpdateKey,
         record: Optional[RecordForParameter] = None,
-        revision: Optional[Revision] = None
+        revision: Optional[Revision] = None,
     ):
         query = '{} = "{}"'.format(update_key['field'], update_key['value'])
         records = self.get_records(app, query=query)['records']
         if len(records) > 0:
             if records[0]['$id']['type'] == '__ID__':
-                result = self.update_record(app, update_key=update_key, record=record, revision=revision)
+                result = self.update_record(
+                    app, update_key=update_key, record=record, revision=revision
+                )
                 return {
                     'id': records[0]['$id']['value'],
-                    'revision': result['revision']
+                    'revision': result['revision'],
                 }
             raise Exception('Missing `$id` in `getRecords` response.')
         return self.add_record(
             app,
             {
-            f"{update_key['field']}": { 'value': update_key['value'] },
-            **({} if record is None else record)
-        }
+                f"{update_key['field']}": {'value': update_key['value']},
+                **({} if record is None else record),
+            },
         )
 
     def get_records(
         self,
         app: AppID,
         fields: Optional[list[str]] = None,
         query: Optional[str] = None,
-        total_count: Optional[bool] = None
+        total_count: Optional[bool] = None,
     ):
         path = self.__build_path_with_guest_space_id(endpoint_name='records')
         params = KintoneRequestParams(
-            app=app,
-            fields=fields,
-            query=query,
-            total_count=total_count
+            app=app, fields=fields, query=query, totalCount=total_count
         )
         return self.client.get(path, params)
 
     def add_records(self, app: AppID, records: list[RecordForParameter]):
         path = self.__build_path_with_guest_space_id(endpoint_name='records')
-        params = KintoneRequestParams(
-            app=app,
-            records=records
-        )
+        params = KintoneRequestParams(app=app, records=records)
         return self.client.post(path, params)
-    
+
     def update_records(
         self,
         app: AppID,
-        records: Union[list[UpdateRecordForParameter], list[UpdateKeyRecordForParameter], list[Union[UpdateRecordForParameter, UpdateKeyRecordForParameter]]]
+        records: Union[
+            list[UpdateRecordForParameter],
+            list[UpdateKeyRecordForParameter],
+            list[Union[UpdateRecordForParameter, UpdateKeyRecordForParameter]],
+        ],
     ):
         path = self.__build_path_with_guest_space_id(endpoint_name='records')
-        params = KintoneRequestParams(
-            app=app,
-            records=records
-        )
+        params = KintoneRequestParams(app=app, records=records)
         return self.client.put(path, params)
-    
-    def delete_records(self, app: AppID, ids: list[RecordID], revisions: Optional[list[Revision]]):
+
+    def delete_records(
+        self, app: AppID, ids: list[RecordID], revisions: Optional[list[Revision]]
+    ):
         path = self.__build_path_with_guest_space_id(endpoint_name='records')
-        params = KintoneRequestParams(
-            app=app,
-            ids=ids,
-            revisions=revisions
-        )
+        params = KintoneRequestParams(app=app, ids=ids, revisions=revisions)
         return self.client.delete(path, params)
-    
-    def create_cursor(self,
+
+    def create_cursor(
+        self,
         app: AppID,
         fields: Optional[list[str]] = None,
         query: Optional[str] = None,
-        size: Union[int, str, None] = None
+        size: Union[int, str, None] = None,
     ):
         path = self.__build_path_with_guest_space_id(endpoint_name='records/cursor')
-        params = KintoneRequestParams(
-            app=app,
-            fields=fields,
-            query=query,
-            size=size
-        )
+        params = KintoneRequestParams(app=app, fields=fields, query=query, size=size)
         return self.client.post(path, params)
-    
+
     def get_records_by_cursor(self, cursor_id: str):
         path = self.__build_path_with_guest_space_id(endpoint_name='records/cursor')
-        params = KintoneRequestParams(
-            id=cursor_id
-        )
+        params = KintoneRequestParams(id=cursor_id)
         return self.client.get(path, params)
-    
+
     def delete_cursor(self, cursor_id: str):
         path = self.__build_path_with_guest_space_id(endpoint_name='records/cursor')
-        params = KintoneRequestParams(
-            id=cursor_id
-        )
+        params = KintoneRequestParams(id=cursor_id)
         return self.client.delete(path, params)
-    
+
     def get_all_records(
         self,
         app: AppID,
         fields: Optional[list[str]] = None,
         condition: Optional[str] = None,
         order_by: Optional[str] = None,
-        with_cursor: bool = True
+        with_cursor: bool = True,
     ):
         if with_cursor:
             condition_query = f'{condition} ' if condition is not None else ''
             order_by_query = f'order by {order_by}' if order_by is not None else ''
             query = f'{condition_query}{order_by_query}'
             query = None if query == '' else query
             return self.get_all_records_with_cursor(app, fields, query)
         if order_by is None:
             return self.get_all_records_with_id(app, fields, condition)
         return self.get_all_records_with_offset(app, fields, condition, order_by)
-    
+
     def get_all_records_with_id(
         self,
         app: AppID,
         fields: Optional[list[str]] = None,
-        condition: Optional[str] = None
+        condition: Optional[str] = None,
     ):
         if fields is not None and len(fields) > 0 and not '$id' in fields:
             fields.append('$id')
         return self.__get_all_records_recursive_with_id(app, fields, condition, '0', [])
 
     def __get_all_records_recursive_with_id(
         self,
         app: AppID,
         fields: Optional[list[str]],
         condition: Optional[str],
         id: str,
-        records: list
+        records: list,
     ):
         condition_query = f'({condition}) and ' if condition is not None else ''
-        query = f'{condition_query}$id > {id} order by $id asc limit {GET_RECORDS_LIMIT}'
+        query = (
+            f'{condition_query}$id > {id} order by $id asc limit {GET_RECORDS_LIMIT}'
+        )
         result = self.get_records(app, fields, query)
         all_records = records + result['records']
         if len(result['records']) < GET_RECORDS_LIMIT:
             return all_records
         last_record = result['records'][-1]
         if last_record['$id']['type'] == '__ID__':
             last_id = last_record['$id']['value']
-            return self.__get_all_records_recursive_with_id(app, fields, condition, last_id, all_records)
+            return self.__get_all_records_recursive_with_id(
+                app, fields, condition, last_id, all_records
+            )
         raise Exception('Missing `$id` in `getRecords` response.')
-    
+
     def get_all_records_with_offset(
         self,
         app: AppID,
         fields: Optional[list[str]] = None,
         condition: Optional[str] = None,
         order_by: Optional[str] = None,
     ):
-        return self.__get_all_records_recursive_with_offset(app, fields, condition, order_by, 0, [])
+        return self.__get_all_records_recursive_with_offset(
+            app, fields, condition, order_by, 0, []
+        )
 
     def __get_all_records_recursive_with_offset(
         self,
         app: AppID,
         fields: Optional[list[str]],
         condition: Optional[str],
         order_by: Optional[str],
         offset: int,
-        records: list
+        records: list,
     ):
         condition_query = f'{condition} ' if condition is not None else ''
         order_by_query = f'order by {order_by} ' if order_by is not None else ''
         query = f'{condition_query}{order_by_query}limit {GET_RECORDS_LIMIT} offset {offset}'
         result = self.get_records(app, fields, query)
         all_records = records + result['records']
         if len(result['records']) < GET_RECORDS_LIMIT:
             return all_records
         return self.__get_all_records_recursive_with_offset(
-            app,
-            fields,
-            condition,
-            order_by,
-            offset + GET_RECORDS_LIMIT,
-            all_records
+            app, fields, condition, order_by, offset + GET_RECORDS_LIMIT, all_records
         )
 
     def get_all_records_with_cursor(
         self,
         app: AppID,
         fields: Optional[list[str]] = None,
-        query: Optional[str] = None
+        query: Optional[str] = None,
     ) -> list:
         res = self.create_cursor(app, fields, query, size=500)
         cursor_id = res['id']
         try:
             return self.__get_all_records_recursive_by_cursor(cursor_id, [])
         except Exception as e:
             self.delete_cursor(cursor_id)
             raise e
-    
+
     def __get_all_records_recursive_by_cursor(
-        self,
-        cursor_id: str,
-        records: list
+        self, cursor_id: str, records: list
     ) -> list:
         result = self.get_records_by_cursor(cursor_id)
         all_records = records + result['records']
         if result['next']:
             return self.__get_all_records_recursive_by_cursor(cursor_id, all_records)
         return all_records
 
-    def add_all_records(
-        self,
-        app: AppID,
-        records: list[RecordForParameter]
-    ):
-        if not all(not isinstance(record, list) and isinstance(record, dict) for record in records):
+    def add_all_records(self, app: AppID, records: list[RecordForParameter]):
+        if not all(
+            not isinstance(record, list) and isinstance(record, dict)
+            for record in records
+        ):
             raise ValueError('the `records` parameter must be an array of object.')
         return self.__add_all_records_recursive(app, records, len(records), [])
-    
+
     def __add_all_records_recursive(
         self,
         app: AppID,
         records: list[RecordForParameter],
         num_of_all_records: int,
-        results: list
+        results: list,
     ) -> dict:
-        CHUNK_LENGTH = self.bulk_request_client.REQUESTS_LENGTH_LIMIT * ADD_RECORDS_LIMIT
+        CHUNK_LENGTH = (
+            self.bulk_request_client.REQUESTS_LENGTH_LIMIT * ADD_RECORDS_LIMIT
+        )
         records_chunk = records[:CHUNK_LENGTH]
         if len(records_chunk) == 0:
-            return {
-                'records': results
-            }
+            return {'records': results}
         new_results = []
         try:
-            new_results = self.__add_all_records_with_bulk_request(
-                app,
-                records_chunk
-            )
+            new_results = self.__add_all_records_with_bulk_request(app, records_chunk)
         except Exception as e:
             # TODO
             raise e
         return self.__add_all_records_recursive(
-            app,
-            records[CHUNK_LENGTH:],
-            num_of_all_records,
-            results + new_results
+            app, records[CHUNK_LENGTH:], num_of_all_records, results + new_results
         )
-    
+
     def __add_all_records_with_bulk_request(
-        self,
-        app: AppID,
-        records: list[RecordForParameter]
+        self, app: AppID, records: list[RecordForParameter]
     ):
         separated_records = self.__separate_array_recursive(
-            ADD_RECORDS_LIMIT,
-            [],
-            records
+            ADD_RECORDS_LIMIT, [], records
         )
         requests: list[EndopintRequestParameter] = [
             {
                 'method': 'POST',
                 'endpoint_name': 'records',
-                'payload': {
-                    'app': app,
-                    'records': records_
-                }
-            } for records_ in separated_records
+                'payload': {'app': app, 'records': records_},
+            }
+            for records_ in separated_records
         ]
         results = self.bulk_request_client.send(requests)['results']
         return_value = []
         for result in results:
             ids = result['ids']
             revisions = result['revisions']
             return_value += [
-                {
-                    'id': val,
-                    'revision': revisions[num]
-                } for num, val in enumerate(ids)
+                {'id': val, 'revision': revisions[num]} for num, val in enumerate(ids)
             ]
         return return_value
 
     def update_all_records(
         self,
         app: AppID,
-        records: Union[list[UpdateRecordForParameter], list[UpdateKeyRecordForParameter], list[Union[UpdateRecordForParameter, UpdateKeyRecordForParameter]]]
+        records: Union[
+            list[UpdateRecordForParameter],
+            list[UpdateKeyRecordForParameter],
+            list[Union[UpdateRecordForParameter, UpdateKeyRecordForParameter]],
+        ],
     ):
         return self.__update_all_records_recursive(app, records, len(records), [])
-    
+
     def __update_all_records_recursive(
         self,
         app: AppID,
-        records: Union[list[UpdateRecordForParameter], list[UpdateKeyRecordForParameter], list[Union[UpdateRecordForParameter, UpdateKeyRecordForParameter]]],
+        records: Union[
+            list[UpdateRecordForParameter],
+            list[UpdateKeyRecordForParameter],
+            list[Union[UpdateRecordForParameter, UpdateKeyRecordForParameter]],
+        ],
         num_of_all_records: int,
-        results: list
+        results: list,
     ):
-        CHUNK_LENGTH = self.bulk_request_client.REQUESTS_LENGTH_LIMIT * UPDATE_RECORDS_LIMIT
+        CHUNK_LENGTH = (
+            self.bulk_request_client.REQUESTS_LENGTH_LIMIT * UPDATE_RECORDS_LIMIT
+        )
         records_chunk = records[:CHUNK_LENGTH]
         if len(records_chunk) == 0:
-            return {
-                'records': results
-            }
+            return {'records': results}
         new_results = []
         try:
             new_results = self.__update_all_records_with_bulk_request(
-                app,
-                records_chunk
+                app, records_chunk
             )
         except Exception as e:
             # TODO
             raise e
         return self.__update_all_records_recursive(
-            app,
-            records[CHUNK_LENGTH:],
-            num_of_all_records,
-            results + new_results
+            app, records[CHUNK_LENGTH:], num_of_all_records, results + new_results
         )
-    
+
     def __update_all_records_with_bulk_request(
         self,
         app: AppID,
-        records: Union[list[UpdateRecordForParameter], list[UpdateKeyRecordForParameter], list[Union[UpdateRecordForParameter, UpdateKeyRecordForParameter]]],
+        records: Union[
+            list[UpdateRecordForParameter],
+            list[UpdateKeyRecordForParameter],
+            list[Union[UpdateRecordForParameter, UpdateKeyRecordForParameter]],
+        ],
     ):
         separated_records = self.__separate_array_recursive(
-            UPDATE_RECORDS_LIMIT,
-            [],
-            records
+            UPDATE_RECORDS_LIMIT, [], records
         )
         requests: list[EndopintRequestParameter] = [
             {
                 'method': 'PUT',
                 'endpoint_name': 'records',
                 'payload': {
                     'app': app,
                     'records': records_,
-                }
-            } for records_ in separated_records
+                },
+            }
+            for records_ in separated_records
         ]
         results = self.bulk_request_client.send(requests)['results']
         return_value = []
         for result in results:
             return_value += result['records']
         return return_value
-    
-    def delete_all_reocrds(
-        self,
-        app: AppID,
-        records: list[DeleteRecordParameter]
-    ):
+
+    def delete_all_reocrds(self, app: AppID, records: list[DeleteRecordParameter]):
         return self.__delete_all_records_recursive(app, records, len(records))
-    
+
     def __delete_all_records_recursive(
-        self,
-        app: AppID,
-        records: list[DeleteRecordParameter],
-        num_of_all_records: int
+        self, app: AppID, records: list[DeleteRecordParameter], num_of_all_records: int
     ):
-        CHUNK_LENGTH = self.bulk_request_client.REQUESTS_LENGTH_LIMIT * DELETE_RECORDS_LIMIT
+        CHUNK_LENGTH = (
+            self.bulk_request_client.REQUESTS_LENGTH_LIMIT * DELETE_RECORDS_LIMIT
+        )
         records_chunk = records[:CHUNK_LENGTH]
         if len(records_chunk) == 0:
             return {}
         try:
-            self.__delete_all_records_with_bulk_request(
-                app,
-                records_chunk
-            )
+            self.__delete_all_records_with_bulk_request(app, records_chunk)
         except Exception as e:
             # TODO
             raise e
         return self.__delete_all_records_recursive(
-            app,
-            records[CHUNK_LENGTH:],
-            num_of_all_records
+            app, records[CHUNK_LENGTH:], num_of_all_records
         )
-    
+
     def __delete_all_records_with_bulk_request(
-        self,
-        app: AppID,
-        records: list[DeleteRecordParameter]
+        self, app: AppID, records: list[DeleteRecordParameter]
     ):
         separated_records = self.__separate_array_recursive(
-            DELETE_RECORDS_LIMIT,
-            [],
-            records
+            DELETE_RECORDS_LIMIT, [], records
         )
         requests: list[EndopintRequestParameter] = [
             {
                 'method': 'DELETE',
                 'endpoint_name': 'records',
                 'payload': {
                     'app': app,
-                    'ids': [ record['id'] for record in records_ ],
-                    'revisions': [ record.get('revision', -1) for record in records_ ]
-                }
-            } for records_ in separated_records
+                    'ids': [record['id'] for record in records_],
+                    'revisions': [record.get('revision', -1) for record in records_],
+                },
+            }
+            for records_ in separated_records
         ]
         self.bulk_request_client.send(requests)['results']
         return None
-    
+
     def __separate_array_recursive(
-        self,
-        size: int,
-        separated: list[list],
-        array: list
+        self, size: int, separated: list[list], array: list
     ) -> list[list]:
         chunk = array[:size]
         if len(chunk) == 0:
             return separated
-        return self.__separate_array_recursive(
-            size,
-            [*separated, chunk],
-            array[size:]
-        )
-    
-    def add_record_comment(
-        self,
-        app: AppID,
-        record: RecordID,
-        comment: Comment
-    ):
+        return self.__separate_array_recursive(size, [*separated, chunk], array[size:])
+
+    def add_record_comment(self, app: AppID, record: RecordID, comment: Comment):
         path = self.__build_path_with_guest_space_id('record/comment')
-        params = KintoneRequestParams(
-            app=app,
-            record=record,
-            comment=comment
-        )
+        params = KintoneRequestParams(app=app, record=record, comment=comment)
         return self.client.post(path, params)
-    
-    def delete_record_comment(
-        self,
-        app: AppID,
-        record: RecordID,
-        comment: CommentID
-    ):
+
+    def delete_record_comment(self, app: AppID, record: RecordID, comment: CommentID):
         path = self.__build_path_with_guest_space_id('record/comment')
-        params = KintoneRequestParams(
-            app=app,
-            record=record,
-            comment=comment
-        )
+        params = KintoneRequestParams(app=app, record=record, comment=comment)
         return self.client.delete(path, params)
-    
+
     def get_record_comments(
         self,
         app: AppID,
         record: RecordID,
         order: Optional[Literal['asc', 'desc']] = None,
         offset: Optional[int] = None,
-        limit: Optional[int] = None
+        limit: Optional[int] = None,
     ):
         path = self.__build_path_with_guest_space_id('record/comments')
         params = KintoneRequestParams(
-            app=app,
-            record=record,
-            order=order,
-            offset=offset,
-            limit=limit
+            app=app, record=record, order=order, offset=offset, limit=limit
         )
         return self.client.get(path, params)
-    
+
     def update_record_assigness(
         self,
         app: AppID,
         id: RecordID,
         assignees: list[str],
-        revision: Optional[Revision] = None
+        revision: Optional[Revision] = None,
     ):
         path = self.__build_path_with_guest_space_id('record/assignees')
         params = KintoneRequestParams(
-            app=app,
-            id=id,
-            assignees=assignees,
-            revision=revision
+            app=app, id=id, assignees=assignees, revision=revision
         )
         return self.client.put(path, params)
-    
+
     def update_record_status(
         self,
         app: AppID,
         id: RecordID,
         action: str,
         assignees: Optional[list[str]] = None,
-        revision: Optional[Revision] = None
+        revision: Optional[Revision] = None,
     ):
         path = self.__build_path_with_guest_space_id('record/status')
         params = KintoneRequestParams(
-            app=app,
-            id=id,
-            action=action,
-            assignees=assignees,
-            revision=revision
+            app=app, id=id, action=action, assignees=assignees, revision=revision
         )
         return self.client.put(path, params)
-    
+
     def update_records_status(
-        self,
-        app: AppID,
-        records: list[UpdateRecordStatusParameter]
+        self, app: AppID, records: list[UpdateRecordStatusParameter]
     ):
         path = self.__build_path_with_guest_space_id('records/status')
-        params = KintoneRequestParams(
-            app=app,
-            records=records
-        )
+        params = KintoneRequestParams(app=app, records=records)
         return self.client.put(path, params)
-    
+
     def __build_path_with_guest_space_id(self, endpoint_name: str) -> str:
         return build_path(
-            endpoint_name=endpoint_name,
-            guest_space_id=self.guest_space_id
-        )
+            endpoint_name=endpoint_name, guest_space_id=self.guest_space_id
+        )
```

### Comparing `pyntone-0.2.2/pyntone/http/http_client.py` & `pyntone-0.3.0/pyntone/http/http_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,59 @@
 from typing import Any
 
 import requests
 
 from pyntone.kintone_request_config_builder import (
-    HttpMethod, KintoneRequestConfigBuilder, KintoneRequestParams)
+    HttpMethod,
+    KintoneRequestConfigBuilder,
+    KintoneRequestFormData,
+    KintoneRequestParams,
+)
 
 
 class KintoneError(Exception):
     def __init__(self, message, text, json, status_code) -> None:
         self.text = text
         self.json = json
         self.status_code = status_code
         super().__init__(message)
 
+
 class HttpClent:
     def __init__(self, config_builder: KintoneRequestConfigBuilder) -> None:
         self.config_builder = config_builder
-    
+
     def get(self, path: str, params: KintoneRequestParams) -> dict[str, Any]:
         config = self.config_builder.build(HttpMethod.GET, path, params)
-        return self._send_request(config)
+        return self._send_request(config).json()
+
+    def get_data(self, path: str, params: KintoneRequestParams) -> bytes:
+        config = self.config_builder.build(HttpMethod.GET, path, params)
+        return self._send_request(config).content
 
     def post(self, path: str, params: KintoneRequestParams) -> dict[str, Any]:
         config = self.config_builder.build(HttpMethod.POST, path, params)
-        return self._send_request(config)
+        return self._send_request(config).json()
+
+    def post_data(self, path: str, form_data: KintoneRequestFormData) -> dict[str, Any]:
+        config = self.config_builder.build(HttpMethod.POST, path, form_data)
+        return self._send_request(config).json()
 
     def put(self, path: str, params: KintoneRequestParams) -> dict[str, Any]:
         config = self.config_builder.build(HttpMethod.PUT, path, params)
-        return self._send_request(config)
-    
+        return self._send_request(config).json()
+
     def delete(self, path: str, params: KintoneRequestParams) -> dict[str, Any]:
         config = self.config_builder.build(HttpMethod.DELETE, path, params)
-        return self._send_request(config)
-    
-    def _send_request(self, config: dict[str, Any]) -> dict[str, Any]:
+        return self._send_request(config).json()
+
+    def _send_request(self, config: dict[str, Any]):
         r = requests.request(**config)
         self._is_success(r)
-        return r.json()
+        return r
 
     def _is_success(self, response: requests.Response) -> None:
         if not (200 <= response.status_code < 300):
             json = response.json()
-            raise KintoneError(json['message'], response.text, json, response.status_code)
+            raise KintoneError(
+                json['message'], response.text, json, response.status_code
+            )
```

### Comparing `pyntone-0.2.2/pyntone/kintone_rest_api_client.py` & `pyntone-0.3.0/pyntone/kintone_rest_api_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from typing import Optional, TypedDict, Union
 
+from pyntone.client import AppClient, FileClient, RecordClient
 from pyntone.client.bulk_request_client import BulkRequestClient
-from pyntone.client.record_client import RecordClient
 from pyntone.http.http_client import HttpClent
 from pyntone.kintone_request_config_builder import KintoneRequestConfigBuilder
 from pyntone.types.auth import DiscriminatedAuth
 
 
 class FeatureFlags(TypedDict):
     enableAbortSearchError: bool
@@ -14,23 +14,25 @@
 
 class KintoneRestAPIClient:
     def __init__(
         self,
         base_url: str,
         auth: DiscriminatedAuth,
         guest_space_id: Union[int, str, None] = None,
-        basic_auth = None,
-        client_cert_auth = None,
-        proxy = None,
-        feature_flags = None,
-        user_agent: Optional[str] = None
+        # TODO
+        # basic_auth=None,
+        # client_cert_auth=None,
+        # proxy=None,
+        # feature_flags=None,
+        # user_agent: Optional[str] = None,
     ) -> None:
         self.__base_url = re.sub('/+$', '', base_url)
-        
-        
-        request_config_builder = KintoneRequestConfigBuilder(auth=auth, base_url=self.__base_url)
+
+        request_config_builder = KintoneRequestConfigBuilder(
+            auth=auth, base_url=self.__base_url
+        )
         httpClient = HttpClent(config_builder=request_config_builder)
-        
+
         self.bulkRequest = BulkRequestClient(httpClient, guest_space_id)
         self.record = RecordClient(httpClient, self.bulkRequest, guest_space_id)
-        # self.app = AppClient()
-        # self.file = FileClient()
+        self.app = AppClient(httpClient, guest_space_id)
+        self.file = FileClient(httpClient, guest_space_id)
```

### Comparing `pyntone-0.2.2/pyntone/types/record.py` & `pyntone-0.3.0/pyntone/types/record.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,49 @@
-from typing import Literal, TypedDict, Union
+from typing import Literal, TypedDict, Union, Any
 
 from pyntone.types import RecordID, Revision
 
 
 class RecordItem(TypedDict):
-    value: Union[int, str]
+    value: Any
+
 
 RecordForParameter = dict[str, RecordItem]
 
+
 class UpdateKey(TypedDict):
     field: str
     value: Union[int, str]
 
+
 class UpdateRecordForParameter(TypedDict, total=False):
     id: RecordID
     record: RecordForParameter
     revision: Revision
 
+
 class UpdateKeyRecordForParameter(TypedDict, total=False):
     updateKey: UpdateKey
     record: RecordForParameter
     revision: Revision
 
+
 class DeleteRecordParameter(TypedDict, total=False):
     id: RecordID
     revision: Revision
 
+
 class Mention(TypedDict):
     code: str
     type: Literal['USER', 'GROUP', 'ORGANIZATION']
 
+
 class Comment(TypedDict, total=False):
     text: str
     mentions: list[Mention]
 
+
 class UpdateRecordStatusParameter(TypedDict, total=False):
     action: str
     assignee: str
     id: RecordID
-    revision: Revision
+    revision: Revision
```

### Comparing `pyntone-0.2.2/pyntone.egg-info/PKG-INFO` & `pyntone-0.3.0/pyntone.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyntone
-Version: 0.2.2
+Version: 0.3.0
 Summary: API client for Kintone REST API.
 Home-page: https://github.com/kashi03/pyntone
 Author: kashi03
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyntone-0.2.2/pyntone.egg-info/SOURCES.txt` & `pyntone-0.3.0/pyntone.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -8,16 +8,23 @@
 pyntone/url.py
 pyntone.egg-info/PKG-INFO
 pyntone.egg-info/SOURCES.txt
 pyntone.egg-info/dependency_links.txt
 pyntone.egg-info/requires.txt
 pyntone.egg-info/top_level.txt
 pyntone/client/__init__.py
+pyntone/client/app_client.py
 pyntone/client/bulk_request_client.py
+pyntone/client/file_client.py
 pyntone/client/record_client.py
+pyntone/client/types/__init__.py
+pyntone/client/types/app/__init__.py
+pyntone/client/types/app/customize.py
 pyntone/http/__init__.py
 pyntone/http/http_client.py
 pyntone/types/__init__.py
 pyntone/types/auth.py
 pyntone/types/record.py
 tests/__init__.py
+tests/test_app.py
+tests/test_file.py
 tests/test_record.py
```

### Comparing `pyntone-0.2.2/setup.cfg` & `pyntone-0.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyntone
-version = 0.2.2
+version = 0.3.0
 description = API client for Kintone REST API.
 url = https://github.com/kashi03/pyntone
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 author = kashi03
 classifiers =
```

### Comparing `pyntone-0.2.2/tests/test_record.py` & `pyntone-0.3.0/tests/test_record.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,177 +1,180 @@
 import os.path
 from os import environ as env
 from uuid import uuid4
 
 import dotenv
 import pytest
 from pyntone import KintoneRestAPIClient, ApiTokenAuth
+from pyntone.types.record import RecordForParameter
+
 
 @pytest.fixture(autouse=True, scope='session')
 def load_env():
     if os.path.exists('.env'):
         dotenv.load_dotenv()
 
+
 @pytest.fixture(autouse=True)
 def client():
     auth = ApiTokenAuth(api_token=env['API_TOKEN'])
-    client = KintoneRestAPIClient(
-        base_url=env['BASE_URL'],
-        auth=auth
-    )
+    client = KintoneRestAPIClient(base_url=env['BASE_URL'], auth=auth)
     return client
 
+
 def test_add_record(client):
     add_record = {
-        'column1': { 'value': str(uuid4()) },
-        'column2': { 'value': 'world' }
+        'column1': {'value': str(uuid4())},
+        'column2': {'value': 'world'},
     }
     result = client.record.add_record(env['APP_ID'], add_record)
     assert result.get('id') is not None
     assert result.get('revision') is not None
 
+
 def test_get_record(client):
     value = str(uuid4())
-    add_record = {
-        'column1': { 'value': value },
-        'column2': { 'value': 'world' }
-    }
+    add_record = {'column1': {'value': value}, 'column2': {'value': 'world'}}
     result = client.record.add_record(env['APP_ID'], add_record)
     resp = client.record.get_record(env['APP_ID'], result['id'])
     assert resp['record']['column1']['value'] == value
     assert resp['record']['column2']['value'] == 'world'
 
+
 def test_update_record(client):
-    add_record = {
-        'column1': { 'value': str(uuid4()) },
-        'column2': { 'value': 'world' }
-    }
+    add_record = {'column1': {'value': str(uuid4())}, 'column2': {'value': 'world'}}
     add_result = client.record.add_record(env['APP_ID'], add_record)
-    update_record = {
-        'column1': { 'value': str(uuid4()) }
-    }
+    update_record = {'column1': {'value': str(uuid4())}}
     update_result = client.record.update_record(
         1,
         record_id=add_result['id'],
         record=update_record,
-        revision=add_result['revision']
+        revision=add_result['revision'],
     )
     assert update_result.get('revision') is not None
 
+
 def test_upsert_record(client):
-    record = {
-        'column2': { 'value': 'upsert' }
-    }
-    update_key = {
-        'field': 'column1',
-        'value': str(uuid4())
-    }
+    record = {'column2': {'value': 'upsert'}}
+    update_key = {'field': 'column1', 'value': str(uuid4())}
     client.record.upsert_record(env['APP_ID'], update_key, record)
 
+
 def test_get_all_records_with_cursor(client):
     client.record.get_all_records_with_cursor(env['APP_ID'])
     assert True
 
+
 def test_add_all_records(client):
     add_records_num = 400
     add_records = [
-        {
-            'column1': { 'value': str(uuid4()) },
-            'column2': { 'value': 'world' }
-        } for _ in range(add_records_num)
+        {'column1': {'value': str(uuid4())}, 'column2': {'value': 'world'}}
+        for _ in range(add_records_num)
     ]
     results = client.record.add_all_records(env['APP_ID'], add_records)
     assert len(results['records']) == add_records_num
 
+
 def test_update_all_records(client):
     add_records_num = 400
     add_records = [
-        {
-            'column1': { 'value': str(uuid4()) },
-            'column2': { 'value': 'world' }
-        } for _ in range(add_records_num)
+        {'column1': {'value': str(uuid4())}, 'column2': {'value': 'world'}}
+        for _ in range(add_records_num)
     ]
     results = client.record.add_all_records(env['APP_ID'], add_records)
-    
+
     update_records = []
     for i in results['records']:
-        update_records.append({
-            'id': i['id'],
-            'record': {
-                'column1': { 'value': str(uuid4()) },
-                'column2': { 'value': 'fuga' }
-            },
-            'revision': i['revision']
-        })
+        update_records.append(
+            {
+                'id': i['id'],
+                'record': {
+                    'column1': {'value': str(uuid4())},
+                    'column2': {'value': 'fuga'},
+                },
+                'revision': i['revision'],
+            }
+        )
     results = client.record.update_all_records(env['APP_ID'], update_records)
     assert len(results['records']) == add_records_num
 
+
 def test_delete_all_reocrds(client):
     add_records_num = 400
     add_records = [
-        {
-            'column1': { 'value': str(uuid4()) },
-            'column2': { 'value': 'world' }
-        } for _ in range(add_records_num)
+        {'column1': {'value': str(uuid4())}, 'column2': {'value': 'world'}}
+        for _ in range(add_records_num)
     ]
     results = client.record.add_all_records(env['APP_ID'], add_records)
-    
+
     delete_records = []
     for i in results['records']:
-        delete_records.append({
-            'id': i['id'],
-            # 'revision': i['revision']
-        })
+        delete_records.append(
+            {
+                'id': i['id'],
+                # 'revision': i['revision']
+            }
+        )
     results = client.record.delete_all_reocrds(env['APP_ID'], delete_records)
     assert results == {}
 
+
 def test_add_record_comment(client):
-    add_record = {
-        'column1': { 'value': str(uuid4()) },
-        'column2': { 'value': 'world' }
-    }
+    add_record = {'column1': {'value': str(uuid4())}, 'column2': {'value': 'world'}}
     add_record_result = client.record.add_record(env['APP_ID'], add_record)
-    add_comment = {
-        'text': 'test comment'
-    }
-    add_comment_result = client.record.add_record_comment(env['APP_ID'], add_record_result.get('id'), add_comment)
+    add_comment = {'text': 'test comment'}
+    add_comment_result = client.record.add_record_comment(
+        env['APP_ID'], add_record_result.get('id'), add_comment
+    )
     assert add_comment_result.get('id') is not None
 
+
 def test_delete_record_comment(client):
     add_record = {
-        'column1': { 'value': str(uuid4()) },
+        'column1': {'value': str(uuid4())},
     }
     add_record_result = client.record.add_record(env['APP_ID'], add_record)
-    add_comment = {
-        'text': 'test comment'
-    }
-    add_comment_result = client.record.add_record_comment(env['APP_ID'], add_record_result['id'], add_comment)
-    delete_comment_result = client.record.delete_record_comment(env['APP_ID'], add_record_result['id'], add_comment_result['id'])
+    add_comment = {'text': 'test comment'}
+    add_comment_result = client.record.add_record_comment(
+        env['APP_ID'], add_record_result['id'], add_comment
+    )
+    delete_comment_result = client.record.delete_record_comment(
+        env['APP_ID'], add_record_result['id'], add_comment_result['id']
+    )
     assert delete_comment_result == {}
 
+
 def test_get_record_comments(client):
     add_record = {
-        'column1': { 'value': str(uuid4()) },
+        'column1': {'value': str(uuid4())},
     }
     add_record_result = client.record.add_record(env['APP_ID'], add_record)
-    add_comment = {
-        'text': 'test comment'
-    }
-    add_comment_result = client.record.add_record_comment(env['APP_ID'], add_record_result['id'], add_comment)
-    get_comment_result = client.record.get_record_comments(env['APP_ID'], add_record_result['id'])
+    add_comment = {'text': 'test comment'}
+    add_comment_result = client.record.add_record_comment(
+        env['APP_ID'], add_record_result['id'], add_comment
+    )
+    get_comment_result = client.record.get_record_comments(
+        env['APP_ID'], add_record_result['id']
+    )
     assert get_comment_result['comments'][0]['text'] == 'test comment '
 
+
 def test_update_record_assigness(client):
     add_record = {
-        'column1': { 'value': str(uuid4()) },
+        'column1': {'value': str(uuid4())},
     }
     add_record_result = client.record.add_record(env['APP_ID'], add_record)
-    result = client.record.update_record_assigness(env['APP_ID'], add_record_result['id'], ['testuser'])
+    result = client.record.update_record_assigness(
+        env['APP_ID'], add_record_result['id'], ['testuser']
+    )
     assert result.get('revision') is not None
 
+
 def test_update_record_status(client):
     add_record = {
-        'column1': { 'value': str(uuid4()) },
+        'column1': {'value': str(uuid4())},
     }
     add_record_result = client.record.add_record(env['APP_ID'], add_record)
-    result = client.record.update_record_status(env['APP_ID'], add_record_result['id'], '処理開始')
-    assert result.get('revision') is not None
+    result = client.record.update_record_status(
+        env['APP_ID'], add_record_result['id'], '処理開始'
+    )
+    assert result.get('revision') is not None
```

