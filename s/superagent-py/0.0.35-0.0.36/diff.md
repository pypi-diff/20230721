# Comparing `tmp/superagent_py-0.0.35.tar.gz` & `tmp/superagent_py-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superagent_py-0.0.35.tar", max compression
+gzip compressed data, was "superagent_py-0.0.36.tar", max compression
```

## Comparing `superagent_py-0.0.35.tar` & `superagent_py-0.0.36.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1073 2023-07-18 13:21:10.799642 superagent_py-0.0.35/LICENSE
--rw-r--r--   0        0        0     3251 2023-07-18 13:21:10.799642 superagent_py-0.0.35/README.md
--rw-r--r--   0        0        0      380 2023-07-18 13:21:10.799642 superagent_py-0.0.35/pyproject.toml
--rw-r--r--   0        0        0      656 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/__init__.py
--rw-r--r--   0        0        0     3186 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/client.py
--rw-r--r--   0        0        0      348 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      170 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/errors/__init__.py
--rw-r--r--   0        0        0      313 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/py.typed
--rw-r--r--   0        0        0      361 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/agent/__init__.py
--rw-r--r--   0        0        0    14309 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/agent/client.py
--rw-r--r--   0        0        0       65 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/agent_documents/__init__.py
--rw-r--r--   0        0        0     9260 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/agent_documents/client.py
--rw-r--r--   0        0        0       65 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/agent_tools/__init__.py
--rw-r--r--   0        0        0     9132 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/agent_tools/client.py
--rw-r--r--   0        0        0       65 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/api_token/__init__.py
--rw-r--r--   0        0        0     8538 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/api_token/client.py
--rw-r--r--   0        0        0       65 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/auth/__init__.py
--rw-r--r--   0        0        0     5901 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/auth/client.py
--rw-r--r--   0        0        0       65 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/documents/__init__.py
--rw-r--r--   0        0        0    10485 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/documents/client.py
--rw-r--r--   0        0        0       65 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/prompts/__init__.py
--rw-r--r--   0        0        0    10865 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/prompts/client.py
--rw-r--r--   0        0        0       65 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/tags/__init__.py
--rw-r--r--   0        0        0    10575 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/tags/client.py
--rw-r--r--   0        0        0       65 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/tools/__init__.py
--rw-r--r--   0        0        0    11638 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/tools/client.py
--rw-r--r--   0        0        0       65 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/traces/__init__.py
--rw-r--r--   0        0        0     2236 2023-07-18 13:21:10.803640 superagent_py-0.0.35/src/superagent/resources/traces/client.py
--rw-r--r--   0        0        0       65 2023-07-18 13:21:10.803640 superagent_py-0.0.35/src/superagent/resources/user/__init__.py
--rw-r--r--   0        0        0     4328 2023-07-18 13:21:10.803640 superagent_py-0.0.35/src/superagent/resources/user/client.py
--rw-r--r--   0        0        0      308 2023-07-18 13:21:10.803640 superagent_py-0.0.35/src/superagent/types/__init__.py
--rw-r--r--   0        0        0      843 2023-07-18 13:21:10.803640 superagent_py-0.0.35/src/superagent/types/http_validation_error.py
--rw-r--r--   0        0        0      869 2023-07-18 13:21:10.803640 superagent_py-0.0.35/src/superagent/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-07-18 13:21:10.803640 superagent_py-0.0.35/src/superagent/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     3762 1970-01-01 00:00:00.000000 superagent_py-0.0.35/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-21 11:06:39.951676 superagent_py-0.0.36/LICENSE
+-rw-r--r--   0        0        0     3251 2023-07-21 11:06:39.951676 superagent_py-0.0.36/README.md
+-rw-r--r--   0        0        0      380 2023-07-21 11:06:39.951676 superagent_py-0.0.36/pyproject.toml
+-rw-r--r--   0        0        0      656 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/__init__.py
+-rw-r--r--   0        0        0     3186 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/client.py
+-rw-r--r--   0        0        0      348 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      170 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/errors/__init__.py
+-rw-r--r--   0        0        0      313 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/py.typed
+-rw-r--r--   0        0        0      361 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/resources/agent/__init__.py
+-rw-r--r--   0        0        0    14309 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/resources/agent/client.py
+-rw-r--r--   0        0        0       65 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/resources/agent_documents/__init__.py
+-rw-r--r--   0        0        0     9260 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/resources/agent_documents/client.py
+-rw-r--r--   0        0        0       65 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/resources/agent_tools/__init__.py
+-rw-r--r--   0        0        0     9132 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/resources/agent_tools/client.py
+-rw-r--r--   0        0        0       65 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/resources/api_token/__init__.py
+-rw-r--r--   0        0        0     8538 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/resources/api_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/resources/auth/__init__.py
+-rw-r--r--   0        0        0     5901 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/resources/auth/client.py
+-rw-r--r--   0        0        0       65 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/resources/documents/__init__.py
+-rw-r--r--   0        0        0    12664 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/resources/documents/client.py
+-rw-r--r--   0        0        0       65 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/resources/prompts/__init__.py
+-rw-r--r--   0        0        0    10865 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/resources/prompts/client.py
+-rw-r--r--   0        0        0       65 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/resources/tags/__init__.py
+-rw-r--r--   0        0        0    10575 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/resources/tags/client.py
+-rw-r--r--   0        0        0       65 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/resources/tools/__init__.py
+-rw-r--r--   0        0        0    11638 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/resources/tools/client.py
+-rw-r--r--   0        0        0       65 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/resources/traces/__init__.py
+-rw-r--r--   0        0        0     2236 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/resources/traces/client.py
+-rw-r--r--   0        0        0       65 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/resources/user/__init__.py
+-rw-r--r--   0        0        0     4328 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/resources/user/client.py
+-rw-r--r--   0        0        0      308 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/types/__init__.py
+-rw-r--r--   0        0        0      843 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/types/http_validation_error.py
+-rw-r--r--   0        0        0      869 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-07-21 11:06:39.951676 superagent_py-0.0.36/src/superagent/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     3762 1970-01-01 00:00:00.000000 superagent_py-0.0.36/PKG-INFO
```

### Comparing `superagent_py-0.0.35/LICENSE` & `superagent_py-0.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.35/README.md` & `superagent_py-0.0.36/README.md`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.35/src/superagent/__init__.py` & `superagent_py-0.0.36/src/superagent/__init__.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.35/src/superagent/client.py` & `superagent_py-0.0.36/src/superagent/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.35/src/superagent/core/datetime_utils.py` & `superagent_py-0.0.36/src/superagent/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.35/src/superagent/core/jsonable_encoder.py` & `superagent_py-0.0.36/src/superagent/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.35/src/superagent/resources/agent/client.py` & `superagent_py-0.0.36/src/superagent/resources/agent/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.35/src/superagent/resources/agent_documents/client.py` & `superagent_py-0.0.36/src/superagent/resources/agent_documents/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.35/src/superagent/resources/agent_tools/client.py` & `superagent_py-0.0.36/src/superagent/resources/agent_tools/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.35/src/superagent/resources/api_token/client.py` & `superagent_py-0.0.36/src/superagent/resources/api_token/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.35/src/superagent/resources/auth/client.py` & `superagent_py-0.0.36/src/superagent/resources/auth/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.35/src/superagent/resources/documents/client.py` & `superagent_py-0.0.36/src/superagent/resources/documents/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -98,14 +98,34 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def patch_document(self, document_id: str, *, request: typing.Dict[str, typing.Any]) -> typing.Any:
+        _response = httpx.request(
+            "PATCH",
+            urllib.parse.urljoin(f"{self._environment}/", f"api/v1/documents/{document_id}"),
+            json=jsonable_encoder(request),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
+            timeout=60,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
     def delete_document(self, document_id: str) -> typing.Any:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/documents/{document_id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
@@ -198,14 +218,35 @@
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def patch_document(self, document_id: str, *, request: typing.Dict[str, typing.Any]) -> typing.Any:
+        async with httpx.AsyncClient() as _client:
+            _response = await _client.request(
+                "PATCH",
+                urllib.parse.urljoin(f"{self._environment}/", f"api/v1/documents/{document_id}"),
+                json=jsonable_encoder(request),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
+                timeout=60,
+            )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `superagent_py-0.0.35/src/superagent/resources/prompts/client.py` & `superagent_py-0.0.36/src/superagent/resources/prompts/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.35/src/superagent/resources/tags/client.py` & `superagent_py-0.0.36/src/superagent/resources/tags/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.35/src/superagent/resources/tools/client.py` & `superagent_py-0.0.36/src/superagent/resources/tools/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.35/src/superagent/resources/traces/client.py` & `superagent_py-0.0.36/src/superagent/resources/traces/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.35/src/superagent/resources/user/client.py` & `superagent_py-0.0.36/src/superagent/resources/user/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.35/src/superagent/types/http_validation_error.py` & `superagent_py-0.0.36/src/superagent/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.35/src/superagent/types/validation_error.py` & `superagent_py-0.0.36/src/superagent/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.35/PKG-INFO` & `superagent_py-0.0.36/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superagent-py
-Version: 0.0.35
+Version: 0.0.36
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

