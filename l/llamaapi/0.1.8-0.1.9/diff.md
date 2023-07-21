# Comparing `tmp/llamaapi-0.1.8.tar.gz` & `tmp/llamaapi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamaapi-0.1.8.tar", max compression
+gzip compressed data, was "llamaapi-0.1.9.tar", max compression
```

## Comparing `llamaapi-0.1.8.tar` & `llamaapi-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2023-07-20 16:25:58.963474 llamaapi-0.1.8/LICENSE
--rw-r--r--   0        0        0     1901 2023-07-20 16:44:53.762559 llamaapi-0.1.8/README.md
--rw-r--r--   0        0        0       70 2023-07-20 17:01:27.580634 llamaapi-0.1.8/llamaapi/__init__.py
--rw-r--r--   0        0        0     1842 2023-07-20 21:06:53.583921 llamaapi-0.1.8/llamaapi/llamaapi.py
--rw-r--r--   0        0        0      368 2023-07-20 21:12:19.392945 llamaapi-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2500 1970-01-01 00:00:00.000000 llamaapi-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-20 16:25:58.963474 llamaapi-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1901 2023-07-20 16:44:53.762559 llamaapi-0.1.9/README.md
+-rw-r--r--   0        0        0       70 2023-07-20 17:01:27.580634 llamaapi-0.1.9/llamaapi/__init__.py
+-rw-r--r--   0        0        0     1839 2023-07-20 21:15:39.974960 llamaapi-0.1.9/llamaapi/llamaapi.py
+-rw-r--r--   0        0        0      368 2023-07-20 21:15:44.715961 llamaapi-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2500 1970-01-01 00:00:00.000000 llamaapi-0.1.9/PKG-INFO
```

### Comparing `llamaapi-0.1.8/LICENSE` & `llamaapi-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `llamaapi-0.1.8/README.md` & `llamaapi-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `llamaapi-0.1.8/llamaapi/llamaapi.py` & `llamaapi-0.1.9/llamaapi/llamaapi.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,25 +24,24 @@
         return asyncio.run(self._run_async(api_request_json))
     
     def _run_stream_jupyter(self, api_request_json):
         # For Jupyter Notebook or Google Colab, we use asyncio's event loop through nest_asyncio
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(self._run_async(api_request_json))
 
-    def _run_simple(self, api_request_json):
+    def _run_sync(self, api_request_json):
         response = requests.post(f"{self.hostname}/api/chat", headers=self.headers, json=api_request_json)
         if response.status_code != 200:
             raise Exception(f"POST {response.status_code}")
         return response.json()
 
     def run(self, api_request_json):
         if api_request_json.get('stream', False):
-            return self.run_stream(api_request_json)
+            return self._run_stream(api_request_json)
         else:
-            return self.run_simple(api_request_json)
+            return self._run_sync(api_request_json)
         
     def run_jupyter(self, api_request_json):
         if api_request_json.get('stream', False):
-            return self.run_stream_jupyter(api_request_json)
+            return self._run_stream_jupyter(api_request_json)
         else:
-            return self.run_simple(api_request_json)
-
+            return self._run_sync(api_request_json)
```

### Comparing `llamaapi-0.1.8/PKG-INFO` & `llamaapi-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llamaapi
-Version: 0.1.8
+Version: 0.1.9
 Summary: Llama API python SDK
 License: MIT
 Author: Eduardo Reis
 Author-email: edu.pontes@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

