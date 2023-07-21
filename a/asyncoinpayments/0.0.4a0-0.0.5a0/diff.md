# Comparing `tmp/asyncoinpayments-0.0.4a0.tar.gz` & `tmp/asyncoinpayments-0.0.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncoinpayments-0.0.4a0.tar", last modified: Fri Jul 21 09:16:55 2023, max compression
+gzip compressed data, was "asyncoinpayments-0.0.5a0.tar", last modified: Fri Jul 21 09:49:17 2023, max compression
```

## Comparing `asyncoinpayments-0.0.4a0.tar` & `asyncoinpayments-0.0.5a0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-21 09:16:55.688109 asyncoinpayments-0.0.4a0/
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       58 2023-07-21 09:11:52.000000 asyncoinpayments-0.0.4a0/.gitignore
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)    11328 2023-07-08 21:40:35.000000 asyncoinpayments-0.0.4a0/LICENSE.txt
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)     1044 2023-07-21 09:16:55.688109 asyncoinpayments-0.0.4a0/PKG-INFO
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      432 2023-07-08 20:18:04.000000 asyncoinpayments-0.0.4a0/README.md
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      842 2023-07-21 09:16:38.000000 asyncoinpayments-0.0.4a0/pyproject.toml
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       38 2023-07-21 09:16:55.688109 asyncoinpayments-0.0.4a0/setup.cfg
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       68 2023-07-20 21:25:48.000000 asyncoinpayments-0.0.4a0/setup.py
-drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-21 09:16:55.684110 asyncoinpayments-0.0.4a0/src/
-drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-21 09:16:55.688109 asyncoinpayments-0.0.4a0/src/asyncoinpayments/
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       92 2023-07-18 17:18:09.000000 asyncoinpayments-0.0.4a0/src/asyncoinpayments/__init__.py
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)    21181 2023-07-20 21:49:59.000000 asyncoinpayments-0.0.4a0/src/asyncoinpayments/coinpayments.py
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      155 2023-07-08 15:55:02.000000 asyncoinpayments-0.0.4a0/src/asyncoinpayments/errors.py
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      647 2023-07-20 21:10:50.000000 asyncoinpayments-0.0.4a0/src/asyncoinpayments/utils.py
-drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-21 09:16:55.688109 asyncoinpayments-0.0.4a0/src/asyncoinpayments.egg-info/
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)     1044 2023-07-21 09:16:55.000000 asyncoinpayments-0.0.4a0/src/asyncoinpayments.egg-info/PKG-INFO
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      406 2023-07-21 09:16:55.000000 asyncoinpayments-0.0.4a0/src/asyncoinpayments.egg-info/SOURCES.txt
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)        1 2023-07-21 09:16:55.000000 asyncoinpayments-0.0.4a0/src/asyncoinpayments.egg-info/dependency_links.txt
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       17 2023-07-21 09:16:55.000000 asyncoinpayments-0.0.4a0/src/asyncoinpayments.egg-info/requires.txt
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       17 2023-07-21 09:16:55.000000 asyncoinpayments-0.0.4a0/src/asyncoinpayments.egg-info/top_level.txt
+drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-21 09:49:17.682250 asyncoinpayments-0.0.5a0/
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       58 2023-07-21 09:11:52.000000 asyncoinpayments-0.0.5a0/.gitignore
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)    11328 2023-07-08 21:40:35.000000 asyncoinpayments-0.0.5a0/LICENSE.txt
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)     1044 2023-07-21 09:49:17.682250 asyncoinpayments-0.0.5a0/PKG-INFO
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      432 2023-07-08 20:18:04.000000 asyncoinpayments-0.0.5a0/README.md
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      842 2023-07-21 09:48:36.000000 asyncoinpayments-0.0.5a0/pyproject.toml
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       38 2023-07-21 09:49:17.682250 asyncoinpayments-0.0.5a0/setup.cfg
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       68 2023-07-20 21:25:48.000000 asyncoinpayments-0.0.5a0/setup.py
+drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-21 09:49:17.678250 asyncoinpayments-0.0.5a0/src/
+drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-21 09:49:17.682250 asyncoinpayments-0.0.5a0/src/asyncoinpayments/
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       92 2023-07-18 17:18:09.000000 asyncoinpayments-0.0.5a0/src/asyncoinpayments/__init__.py
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)    21174 2023-07-21 09:27:52.000000 asyncoinpayments-0.0.5a0/src/asyncoinpayments/coinpayments.py
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      155 2023-07-08 15:55:02.000000 asyncoinpayments-0.0.5a0/src/asyncoinpayments/errors.py
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      643 2023-07-21 09:47:09.000000 asyncoinpayments-0.0.5a0/src/asyncoinpayments/utils.py
+drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-21 09:49:17.682250 asyncoinpayments-0.0.5a0/src/asyncoinpayments.egg-info/
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)     1044 2023-07-21 09:49:17.000000 asyncoinpayments-0.0.5a0/src/asyncoinpayments.egg-info/PKG-INFO
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      406 2023-07-21 09:49:17.000000 asyncoinpayments-0.0.5a0/src/asyncoinpayments.egg-info/SOURCES.txt
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)        1 2023-07-21 09:49:17.000000 asyncoinpayments-0.0.5a0/src/asyncoinpayments.egg-info/dependency_links.txt
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       17 2023-07-21 09:49:17.000000 asyncoinpayments-0.0.5a0/src/asyncoinpayments.egg-info/requires.txt
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       17 2023-07-21 09:49:17.000000 asyncoinpayments-0.0.5a0/src/asyncoinpayments.egg-info/top_level.txt
```

### Comparing `asyncoinpayments-0.0.4a0/LICENSE.txt` & `asyncoinpayments-0.0.5a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `asyncoinpayments-0.0.4a0/PKG-INFO` & `asyncoinpayments-0.0.5a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncoinpayments
-Version: 0.0.4a0
+Version: 0.0.5a0
 Summary: Python Asynchronous Wrapper of the CoinPayments API
 Author-email: flalugli <flalugli.dev@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/flalugli/asyncoinpayments
 Keywords: python,crypto,cryptocurrency,payment gateway,async,aiohttp
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `asyncoinpayments-0.0.4a0/pyproject.toml` & `asyncoinpayments-0.0.5a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asyncoinpayments"
-version = "0.0.4a"
+version = "0.0.5a"
 description = "Python Asynchronous Wrapper of the CoinPayments API"
 authors = [
   { name="flalugli", email="flalugli.dev@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ['python', 'crypto', 'cryptocurrency', 'payment gateway', 'async', 'aiohttp']
```

### Comparing `asyncoinpayments-0.0.4a0/src/asyncoinpayments/coinpayments.py` & `asyncoinpayments-0.0.5a0/src/asyncoinpayments/coinpayments.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 import hashlib
 from typing import Union
 from tenacity import retry, stop_after_attempt
 from .errors import CoinPayementsError,CoinPaymentsInputError,FormatError 
 from .utils import ResponseFormat, JsonResponse, ApiResponseJson
 
 
-class AsyncCoinPayments:
+class AsynCoinPayments:
     
     REQUEST_TRIES=3
 
-    def __init__(self,_private_key:str,_public_key:str,_version:str='1', _format:ResponseFormat = ResponseFormat.JSON, _proxy:str = None, _proxy_auth:str = None) -> None:
+    def __init__(self,private_key:str,public_key:str,version:str='1', _format:ResponseFormat = ResponseFormat.JSON, _proxy:str = None, _proxy_auth:str = None) -> None:
         
-        self._private_key = _private_key
-        self._public_key = _public_key
-        self._version = _version
+        self._private_key = private_key
+        self._public_key = public_key
+        self._version = version
 
         self.proxy=_proxy
         self._proxy_auth=_proxy_auth
         
         self.base_url='https://www.coinpayments.net/api.php'
         self._format=_format #the format of the http response can be json/xml
```

### Comparing `asyncoinpayments-0.0.4a0/src/asyncoinpayments/utils.py` & `asyncoinpayments-0.0.5a0/src/asyncoinpayments/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     
     def __init__(self, data : ApiResponseJson) -> None:
 
         self.error = data['error']
         self.result = data['result']
 
     def __str__(self):
-        return f"(error: {self._error}, result: {self._result})"
+        return f"(error: {self.error}, result: {self.error})"
 
     def raise_for_errors(self) -> None:
         """
         If an error accours it will be raised as CoinPaymentsError
         """
         if self.error != "ok":
-            raise CoinPayementsError(self._error)
+            raise CoinPayementsError(self.error)
```

### Comparing `asyncoinpayments-0.0.4a0/src/asyncoinpayments.egg-info/PKG-INFO` & `asyncoinpayments-0.0.5a0/src/asyncoinpayments.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncoinpayments
-Version: 0.0.4a0
+Version: 0.0.5a0
 Summary: Python Asynchronous Wrapper of the CoinPayments API
 Author-email: flalugli <flalugli.dev@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/flalugli/asyncoinpayments
 Keywords: python,crypto,cryptocurrency,payment gateway,async,aiohttp
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

