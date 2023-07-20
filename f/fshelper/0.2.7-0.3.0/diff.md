# Comparing `tmp/fshelper-0.2.7.tar.gz` & `tmp/fshelper-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fshelper-0.2.7.tar", last modified: Mon Aug 22 23:08:11 2022, max compression
+gzip compressed data, was "fshelper-0.3.0.tar", last modified: Thu Jul 20 22:29:35 2023, max compression
```

## Comparing `fshelper-0.2.7.tar` & `fshelper-0.3.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2022-08-22 23:08:11.514351 fshelper-0.2.7/
--rw-rw-rw-   0        0        0     1073 2021-11-30 19:17:58.000000 fshelper-0.2.7/LICENSE
--rw-rw-rw-   0        0        0      140 2021-11-30 19:17:58.000000 fshelper-0.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2479 2022-08-22 23:08:11.514351 fshelper-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0      370 2022-08-22 22:57:59.000000 fshelper-0.2.7/PUBLISH.md
--rw-rw-rw-   0        0        0     1427 2022-08-22 23:05:19.000000 fshelper-0.2.7/README.md
--rw-rw-rw-   0        0        0      445 2022-08-22 23:06:00.000000 fshelper-0.2.7/RELEASE_NOTES.md
--rw-rw-rw-   0        0        0       96 2022-08-22 22:57:58.000000 fshelper-0.2.7/pyproject.toml
--rw-rw-rw-   0        0        0      833 2022-08-22 23:08:11.524208 fshelper-0.2.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-22 23:08:11.352230 fshelper-0.2.7/src/
-drwxrwxrwx   0        0        0        0 2022-08-22 23:08:11.381994 fshelper-0.2.7/src/fshelper/
--rw-rw-rw-   0        0        0      342 2022-08-22 23:05:19.000000 fshelper-0.2.7/src/fshelper/__init__.py
--rw-rw-rw-   0        0        0     1832 2021-12-09 18:19:58.000000 fshelper-0.2.7/src/fshelper/api.py
--rw-rw-rw-   0        0        0     8702 2022-08-22 22:57:58.000000 fshelper-0.2.7/src/fshelper/endpoints.py
--rw-rw-rw-   0        0        0        0 2021-11-30 19:17:58.000000 fshelper-0.2.7/src/fshelper/errors.py
-drwxrwxrwx   0        0        0        0 2022-08-22 23:08:11.444418 fshelper-0.2.7/src/fshelper/models/
--rw-rw-rw-   0        0        0      171 2022-08-17 21:42:13.000000 fshelper-0.2.7/src/fshelper/models/__init__.py
--rw-rw-rw-   0        0        0     3848 2022-08-22 22:57:58.000000 fshelper-0.2.7/src/fshelper/models/asset.py
--rw-rw-rw-   0        0        0      789 2021-11-30 19:17:58.000000 fshelper-0.2.7/src/fshelper/models/service_request.py
-drwxrwxrwx   0        0        0        0 2022-08-22 23:08:11.454270 fshelper-0.2.7/src/fshelper/support/
--rw-rw-rw-   0        0        0      156 2022-08-17 20:57:29.000000 fshelper-0.2.7/src/fshelper/support/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-22 23:08:11.464811 fshelper-0.2.7/src/fshelper/support/factories/
--rw-rw-rw-   0        0        0       38 2022-08-17 21:09:09.000000 fshelper-0.2.7/src/fshelper/support/factories/__init__.py
--rw-rw-rw-   0        0        0      474 2022-08-17 21:09:09.000000 fshelper-0.2.7/src/fshelper/support/factories/asset.py
-drwxrwxrwx   0        0        0        0 2022-08-22 23:08:11.464811 fshelper-0.2.7/src/fshelper/v1/
--rw-rw-rw-   0        0        0        0 2021-11-30 19:17:58.000000 fshelper-0.2.7/src/fshelper/v1/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-22 23:08:11.514351 fshelper-0.2.7/src/fshelper/v2/
--rw-rw-rw-   0        0        0      279 2022-08-09 21:58:27.000000 fshelper-0.2.7/src/fshelper/v2/__init__.py
--rw-rw-rw-   0        0        0      509 2022-08-17 22:02:02.000000 fshelper-0.2.7/src/fshelper/v2/asset_types.py
--rw-rw-rw-   0        0        0     2366 2022-08-22 22:57:58.000000 fshelper-0.2.7/src/fshelper/v2/assets.py
--rw-rw-rw-   0        0        0      503 2022-08-17 22:03:00.000000 fshelper-0.2.7/src/fshelper/v2/locations.py
--rw-rw-rw-   0        0        0      713 2022-08-17 22:03:36.000000 fshelper-0.2.7/src/fshelper/v2/service_items_endpoint.py
--rw-rw-rw-   0        0        0      386 2022-08-17 22:05:18.000000 fshelper-0.2.7/src/fshelper/v2/ticket_form_fields.py
--rw-rw-rw-   0        0        0      330 2022-08-17 22:05:43.000000 fshelper-0.2.7/src/fshelper/v2/tickets_endpoint.py
-drwxrwxrwx   0        0        0        0 2022-08-22 23:08:11.415196 fshelper-0.2.7/src/fshelper.egg-info/
--rw-rw-rw-   0        0        0     2479 2022-08-22 23:08:11.000000 fshelper-0.2.7/src/fshelper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      864 2022-08-22 23:08:11.000000 fshelper-0.2.7/src/fshelper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-22 23:08:11.000000 fshelper-0.2.7/src/fshelper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-08-19 23:48:51.000000 fshelper-0.2.7/src/fshelper.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       28 2022-08-22 23:08:11.000000 fshelper-0.2.7/src/fshelper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-08-22 23:08:11.000000 fshelper-0.2.7/src/fshelper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 22:29:35.318131 fshelper-0.3.0/
+-rw-rw-rw-   0        0        0     1073 2021-11-30 19:17:58.000000 fshelper-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      140 2021-11-30 19:17:58.000000 fshelper-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2606 2023-07-20 22:29:35.318131 fshelper-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2023-07-20 22:26:44.000000 fshelper-0.3.0/PUBLISH.md
+-rw-rw-rw-   0        0        0     1427 2023-07-20 22:25:48.000000 fshelper-0.3.0/README.md
+-rw-rw-rw-   0        0        0      559 2023-07-20 22:24:40.000000 fshelper-0.3.0/RELEASE_NOTES.md
+-rw-rw-rw-   0        0        0       96 2022-08-22 22:57:58.000000 fshelper-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      833 2023-07-20 22:29:35.318131 fshelper-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-20 22:29:35.280691 fshelper-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-20 22:29:35.305389 fshelper-0.3.0/src/fshelper/
+-rw-rw-rw-   0        0        0      342 2023-07-20 22:25:48.000000 fshelper-0.3.0/src/fshelper/__init__.py
+-rw-rw-rw-   0        0        0     1832 2021-12-09 18:19:58.000000 fshelper-0.3.0/src/fshelper/api.py
+-rw-rw-rw-   0        0        0    10460 2023-07-20 21:14:13.000000 fshelper-0.3.0/src/fshelper/endpoints.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 19:17:58.000000 fshelper-0.3.0/src/fshelper/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-20 22:29:35.312144 fshelper-0.3.0/src/fshelper/models/
+-rw-rw-rw-   0        0        0      171 2022-08-17 21:42:13.000000 fshelper-0.3.0/src/fshelper/models/__init__.py
+-rw-rw-rw-   0        0        0     3848 2022-08-22 22:57:58.000000 fshelper-0.3.0/src/fshelper/models/asset.py
+-rw-rw-rw-   0        0        0      789 2021-11-30 19:17:58.000000 fshelper-0.3.0/src/fshelper/models/service_request.py
+drwxrwxrwx   0        0        0        0 2023-07-20 22:29:35.313676 fshelper-0.3.0/src/fshelper/support/
+-rw-rw-rw-   0        0        0      156 2022-08-17 20:57:29.000000 fshelper-0.3.0/src/fshelper/support/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 22:29:35.314682 fshelper-0.3.0/src/fshelper/support/factories/
+-rw-rw-rw-   0        0        0       38 2022-08-17 21:09:09.000000 fshelper-0.3.0/src/fshelper/support/factories/__init__.py
+-rw-rw-rw-   0        0        0      535 2023-07-20 22:14:28.000000 fshelper-0.3.0/src/fshelper/support/factories/asset.py
+drwxrwxrwx   0        0        0        0 2023-07-20 22:29:35.315682 fshelper-0.3.0/src/fshelper/v1/
+-rw-rw-rw-   0        0        0        0 2021-11-30 19:17:58.000000 fshelper-0.3.0/src/fshelper/v1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 22:29:35.318131 fshelper-0.3.0/src/fshelper/v2/
+-rw-rw-rw-   0        0        0      279 2022-08-09 21:58:27.000000 fshelper-0.3.0/src/fshelper/v2/__init__.py
+-rw-rw-rw-   0        0        0      509 2022-08-17 22:02:02.000000 fshelper-0.3.0/src/fshelper/v2/asset_types.py
+-rw-rw-rw-   0        0        0     3278 2023-07-20 21:01:27.000000 fshelper-0.3.0/src/fshelper/v2/assets.py
+-rw-rw-rw-   0        0        0      503 2022-08-17 22:03:00.000000 fshelper-0.3.0/src/fshelper/v2/locations.py
+-rw-rw-rw-   0        0        0      713 2022-08-17 22:03:36.000000 fshelper-0.3.0/src/fshelper/v2/service_items_endpoint.py
+-rw-rw-rw-   0        0        0      386 2022-08-17 22:05:18.000000 fshelper-0.3.0/src/fshelper/v2/ticket_form_fields.py
+-rw-rw-rw-   0        0        0      330 2022-08-17 22:05:43.000000 fshelper-0.3.0/src/fshelper/v2/tickets_endpoint.py
+drwxrwxrwx   0        0        0        0 2023-07-20 22:29:35.309567 fshelper-0.3.0/src/fshelper.egg-info/
+-rw-rw-rw-   0        0        0     2606 2023-07-20 22:29:35.000000 fshelper-0.3.0/src/fshelper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2023-07-20 22:29:35.000000 fshelper-0.3.0/src/fshelper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 22:29:35.000000 fshelper-0.3.0/src/fshelper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-08-19 23:48:51.000000 fshelper-0.3.0/src/fshelper.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       28 2023-07-20 22:29:35.000000 fshelper-0.3.0/src/fshelper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-20 22:29:35.000000 fshelper-0.3.0/src/fshelper.egg-info/top_level.txt
```

### Comparing `fshelper-0.2.7/LICENSE` & `fshelper-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fshelper-0.2.7/PKG-INFO` & `fshelper-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: fshelper
-Version: 0.2.7
+Version: 0.3.0
 Summary: Library for working with the FreshService API.
 Author: Matthew Larsen
 Author-email: matt.larsen@connorgp.com
 License: MIT License
 Project-URL: Source Code, https://github.com/matt-larsen-sld/freshservice-helper
 Keywords: freshservice
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fshelper
-FreshService API usage helper version: 0.2.7
+FreshService API usage helper version: 0.3.0
 
 ## Features
 ### Assets Endpoint v0.1.0
   Added an endpoint for working with assets
 
 ## Usage
 *Example:*
@@ -47,32 +47,45 @@
 Use this as a context manager or call the `RequestService.new_session()` method in a try, except, finally block with
 `RequestService.session.close()` in the finally block.
 
 
 ### Endpoints
 Different classes to work with different FreshService API endpoints.
 
+# 0.3.0
+
+Filter read-only and invalid fields from being sent to the FS API when defined for an end point.
+
 # 0.2.7
+
 Fixes for object create actions and delete actions for Assets
+
 - Start on implementation of Pydantic models for Assets
 - Change resource_key field to single and plural versions
 
 # 0.2.2
-Add Locations endpoint 
+
+Add Locations endpoint
 
 # 0.2.1
-Add Asset Types endpoint 
+
+Add Asset Types endpoint
 
 # 0.2.0
+
 Extended assets endpoint functionality
 
 # 0.1.0
+
 Delete capability for asset endpoints
 
 # 0.0.8
+
 Release to Azure devops
 
 # 0.0.6
+
 Addition of tbump
 
 # 0.0.5
+
 Added an endpoint for assets
```

### Comparing `fshelper-0.2.7/README.md` & `fshelper-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # fshelper
-FreshService API usage helper version: 0.2.7
+FreshService API usage helper version: 0.3.0
 
 ## Features
 ### Assets Endpoint v0.1.0
   Added an endpoint for working with assets
 
 ## Usage
 *Example:*
```

### Comparing `fshelper-0.2.7/setup.cfg` & `fshelper-0.3.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2066 7368 656c 7065 720d 0a76 6572   = fshelper..ver
-00000020: 7369 6f6e 203d 2030 2e32 2e37 0d0a 6465  sion = 0.2.7..de
+00000020: 7369 6f6e 203d 2030 2e33 2e30 0d0a 6465  sion = 0.3.0..de
 00000030: 7363 7269 7074 696f 6e20 3d20 4c69 6272  scription = Libr
 00000040: 6172 7920 666f 7220 776f 726b 696e 6720  ary for working 
 00000050: 7769 7468 2074 6865 2046 7265 7368 5365  with the FreshSe
 00000060: 7276 6963 6520 4150 492e 0d0a 6c6f 6e67  rvice API...long
 00000070: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000080: 696c 653a 2052 4541 444d 452e 6d64 2c20  ile: README.md, 
 00000090: 5245 4c45 4153 455f 4e4f 5445 532e 6d64  RELEASE_NOTES.md
```

### Comparing `fshelper-0.2.7/src/fshelper/api.py` & `fshelper-0.3.0/src/fshelper/api.py`

 * *Files identical despite different names*

### Comparing `fshelper-0.2.7/src/fshelper/endpoints.py` & `fshelper-0.3.0/src/fshelper/endpoints.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import logging
 import os
 import sys
 from json import JSONDecodeError
-from typing import Optional, Dict, Any
+from typing import Optional, Dict, Any, List, Union, Set, Tuple
 
 from requests import Request
 from requests.exceptions import HTTPError
 
 from .api import RequestService
 
 logger = logging.getLogger(__name__)
@@ -26,14 +26,18 @@
         """string extension from the base of the URL specific to each resource"""
         self.identifier: Any = None
         """Identifier to make the instance of the endpoint specific to a resource."""
         self.create_command = None
         """Some resources extend the endpoint URL with a verb when creating the resource"""
         self.single_resource_key = None
         """dict key for a single resource when returned from the API."""
+        self.creation_fields: Union[List[str], Set[str], Tuple[str], None] = None
+        """Optional collection of str to specify valid fields to send in create method."""
+        self.read_only_fields: Union[List[str], Set[str], Tuple[str], None] = None
+        """Read only fields you can't set during creation."""
 
     @property
     def endpoint(self):
         return self._endpoint
 
     @property
     def base_url(self):
@@ -73,14 +77,16 @@
         """Create a FreshService resource with the given data.
 
         :param data: Data to pass to FreshService API with the values for the resource
         :param enabled: A toggle to create the resource or not during development.
         """
         url = self.extended_url
         _data_to_send = _drop_none(data)
+        _data_to_send = self._drop_not_in_creation_fields(_data_to_send)
+        _data_to_send = self._drop_read_only_fields(_data_to_send)
         if self.create_command is not None:
             url = f"{url}/{self.create_command}"
         if self.fs_create_requests_enabled or enabled:
             response = self.send_request(url, method="POST", data=_data_to_send)
         else:
             logger.warning(
                 "Environment variable 'ALLOW_FS_CREATE_REQUESTS' must be set to 'True' to allow sending "
@@ -116,15 +122,15 @@
             self.identifier = identifier
         _method = "PUT"
         _url = f"{self.item_extended_url}"
         response = self.send_request(_url, method=_method, data=data)
         return response
 
     def send_request(
-        self, url: str, method: Optional[str] = "GET", data: Optional[Dict] = None
+            self, url: str, method: Optional[str] = "GET", data: Optional[Dict] = None
     ) -> Dict:
         """Send the HTTP request to the FreshService API using a requests library session.
 
         TODO: Send query strings as a dict for parameters to the requests API.
         """
         try:
             if isinstance(data, dict):
@@ -160,14 +166,42 @@
                 "status_code": getattr(resp, "status_code", None),
                 "url": getattr(resp, "url", None),
                 "ok": getattr(resp, "ok", None),
                 "reason": getattr(resp, "reason", None),
             }
             return resp_dict
 
+    def _drop_not_in_creation_fields(self, data: Dict) -> Dict:
+        """drop fields from data Dict that are not in `self.creation_fields` if `self.creation_fields` is not None."""
+        if self.creation_fields is None:  # `self.creation_fields` is None so don't prune fields from data Dict
+            return data
+        for _key in list(data.keys()):
+            if _key not in self.creation_fields:
+                _dropped_value = data.pop(_key)
+                logger.info(
+                    "Removed key '%s' with value '%s' from data as it is not given in `creation_fields`.",
+                    _key,
+                    _dropped_value
+                )
+        return data
+
+    def _drop_read_only_fields(self, data: Dict) -> Dict:
+        """Drop fields from `data` with key matching items in `self.read_only_fields`."""
+        if self.read_only_fields is None:
+            return data
+        for _key in list(data.keys()):
+            if _key in self.read_only_fields:
+                _dropped_value = data.pop(_key)
+                logger.info(
+                    "Removed key '%s' with value '%s' from data as it is given as a read only field.",
+                    _key,
+                    _dropped_value,
+                )
+        return data
+
 
 class GenericPluralEndpoint(GenericEndPoint):
     DEFAULT_ITEMS_PER_PAGE = 30
 
     def __init__(self, request_service: RequestService):
         super(GenericPluralEndpoint, self).__init__(request_service)
         self._items_per_page = None
```

### Comparing `fshelper-0.2.7/src/fshelper/models/asset.py` & `fshelper-0.3.0/src/fshelper/models/asset.py`

 * *Files identical despite different names*

### Comparing `fshelper-0.2.7/src/fshelper/models/service_request.py` & `fshelper-0.3.0/src/fshelper/models/service_request.py`

 * *Files identical despite different names*

### Comparing `fshelper-0.2.7/src/fshelper/v2/service_items_endpoint.py` & `fshelper-0.3.0/src/fshelper/v2/service_items_endpoint.py`

 * *Files identical despite different names*

### Comparing `fshelper-0.2.7/src/fshelper.egg-info/PKG-INFO` & `fshelper-0.3.0/src/fshelper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: fshelper
-Version: 0.2.7
+Version: 0.3.0
 Summary: Library for working with the FreshService API.
 Author: Matthew Larsen
 Author-email: matt.larsen@connorgp.com
 License: MIT License
 Project-URL: Source Code, https://github.com/matt-larsen-sld/freshservice-helper
 Keywords: freshservice
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fshelper
-FreshService API usage helper version: 0.2.7
+FreshService API usage helper version: 0.3.0
 
 ## Features
 ### Assets Endpoint v0.1.0
   Added an endpoint for working with assets
 
 ## Usage
 *Example:*
@@ -47,32 +47,45 @@
 Use this as a context manager or call the `RequestService.new_session()` method in a try, except, finally block with
 `RequestService.session.close()` in the finally block.
 
 
 ### Endpoints
 Different classes to work with different FreshService API endpoints.
 
+# 0.3.0
+
+Filter read-only and invalid fields from being sent to the FS API when defined for an end point.
+
 # 0.2.7
+
 Fixes for object create actions and delete actions for Assets
+
 - Start on implementation of Pydantic models for Assets
 - Change resource_key field to single and plural versions
 
 # 0.2.2
-Add Locations endpoint 
+
+Add Locations endpoint
 
 # 0.2.1
-Add Asset Types endpoint 
+
+Add Asset Types endpoint
 
 # 0.2.0
+
 Extended assets endpoint functionality
 
 # 0.1.0
+
 Delete capability for asset endpoints
 
 # 0.0.8
+
 Release to Azure devops
 
 # 0.0.6
+
 Addition of tbump
 
 # 0.0.5
+
 Added an endpoint for assets
```

### Comparing `fshelper-0.2.7/src/fshelper.egg-info/SOURCES.txt` & `fshelper-0.3.0/src/fshelper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

