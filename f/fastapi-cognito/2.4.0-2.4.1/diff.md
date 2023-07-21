# Comparing `tmp/fastapi-cognito-2.4.0.tar.gz` & `tmp/fastapi-cognito-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-cognito-2.4.0.tar", last modified: Fri Jul 21 14:26:34 2023, max compression
+gzip compressed data, was "fastapi-cognito-2.4.1.tar", last modified: Fri Jul 21 14:45:36 2023, max compression
```

## Comparing `fastapi-cognito-2.4.0.tar` & `fastapi-cognito-2.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-07-21 14:26:34.196895 fastapi-cognito-2.4.0/
--rw-rw-r--   0 marko     (1000) marko     (1000)     1073 2023-07-21 10:49:27.000000 fastapi-cognito-2.4.0/LICENSE.txt
--rw-rw-r--   0 marko     (1000) marko     (1000)     4675 2023-07-21 14:26:34.196895 fastapi-cognito-2.4.0/PKG-INFO
--rw-rw-r--   0 marko     (1000) marko     (1000)     4150 2023-07-21 14:24:49.000000 fastapi-cognito-2.4.0/README.md
--rw-rw-r--   0 marko     (1000) marko     (1000)      103 2023-07-21 10:49:27.000000 fastapi-cognito-2.4.0/pyproject.toml
--rw-rw-r--   0 marko     (1000) marko     (1000)       38 2023-07-21 14:26:34.196895 fastapi-cognito-2.4.0/setup.cfg
--rw-rw-r--   0 marko     (1000) marko     (1000)     1036 2023-07-21 14:20:30.000000 fastapi-cognito-2.4.0/setup.py
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-07-21 14:26:34.196895 fastapi-cognito-2.4.0/src/
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-07-21 14:26:34.196895 fastapi-cognito-2.4.0/src/fastapi_cognito/
--rw-rw-r--   0 marko     (1000) marko     (1000)      176 2023-07-21 10:49:27.000000 fastapi-cognito-2.4.0/src/fastapi_cognito/__init__.py
--rw-rw-r--   0 marko     (1000) marko     (1000)      525 2023-07-21 10:49:27.000000 fastapi-cognito-2.4.0/src/fastapi_cognito/exceptions.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     9290 2023-07-21 13:40:19.000000 fastapi-cognito-2.4.0/src/fastapi_cognito/fastapi_cognito.py
--rw-rw-r--   0 marko     (1000) marko     (1000)      527 2023-07-21 12:40:47.000000 fastapi-cognito-2.4.0/src/fastapi_cognito/models.py
--rw-rw-r--   0 marko     (1000) marko     (1000)     1490 2023-07-21 13:40:46.000000 fastapi-cognito-2.4.0/src/fastapi_cognito/settings_parsers.py
-drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-07-21 14:26:34.196895 fastapi-cognito-2.4.0/src/fastapi_cognito.egg-info/
--rw-rw-r--   0 marko     (1000) marko     (1000)     4675 2023-07-21 14:26:34.000000 fastapi-cognito-2.4.0/src/fastapi_cognito.egg-info/PKG-INFO
--rw-rw-r--   0 marko     (1000) marko     (1000)      434 2023-07-21 14:26:34.000000 fastapi-cognito-2.4.0/src/fastapi_cognito.egg-info/SOURCES.txt
--rw-rw-r--   0 marko     (1000) marko     (1000)        1 2023-07-21 14:26:34.000000 fastapi-cognito-2.4.0/src/fastapi_cognito.egg-info/dependency_links.txt
--rw-rw-r--   0 marko     (1000) marko     (1000)       88 2023-07-21 14:26:34.000000 fastapi-cognito-2.4.0/src/fastapi_cognito.egg-info/requires.txt
--rw-rw-r--   0 marko     (1000) marko     (1000)       16 2023-07-21 14:26:34.000000 fastapi-cognito-2.4.0/src/fastapi_cognito.egg-info/top_level.txt
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-07-21 14:45:36.319782 fastapi-cognito-2.4.1/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1073 2023-07-21 10:49:27.000000 fastapi-cognito-2.4.1/LICENSE.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4675 2023-07-21 14:45:36.319782 fastapi-cognito-2.4.1/PKG-INFO
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4150 2023-07-21 14:34:57.000000 fastapi-cognito-2.4.1/README.md
+-rw-rw-r--   0 marko     (1000) marko     (1000)      103 2023-07-21 10:49:27.000000 fastapi-cognito-2.4.1/pyproject.toml
+-rw-rw-r--   0 marko     (1000) marko     (1000)       38 2023-07-21 14:45:36.319782 fastapi-cognito-2.4.1/setup.cfg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1036 2023-07-21 14:44:50.000000 fastapi-cognito-2.4.1/setup.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-07-21 14:45:36.315782 fastapi-cognito-2.4.1/src/
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-07-21 14:45:36.315782 fastapi-cognito-2.4.1/src/fastapi_cognito/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      176 2023-07-21 10:49:27.000000 fastapi-cognito-2.4.1/src/fastapi_cognito/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      525 2023-07-21 10:49:27.000000 fastapi-cognito-2.4.1/src/fastapi_cognito/exceptions.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     8963 2023-07-21 14:44:46.000000 fastapi-cognito-2.4.1/src/fastapi_cognito/fastapi_cognito.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      527 2023-07-21 14:34:57.000000 fastapi-cognito-2.4.1/src/fastapi_cognito/models.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1490 2023-07-21 14:34:57.000000 fastapi-cognito-2.4.1/src/fastapi_cognito/settings_parsers.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-07-21 14:45:36.319782 fastapi-cognito-2.4.1/src/fastapi_cognito.egg-info/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4675 2023-07-21 14:45:36.000000 fastapi-cognito-2.4.1/src/fastapi_cognito.egg-info/PKG-INFO
+-rw-rw-r--   0 marko     (1000) marko     (1000)      434 2023-07-21 14:45:36.000000 fastapi-cognito-2.4.1/src/fastapi_cognito.egg-info/SOURCES.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)        1 2023-07-21 14:45:36.000000 fastapi-cognito-2.4.1/src/fastapi_cognito.egg-info/dependency_links.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)       88 2023-07-21 14:45:36.000000 fastapi-cognito-2.4.1/src/fastapi_cognito.egg-info/requires.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)       16 2023-07-21 14:45:36.000000 fastapi-cognito-2.4.1/src/fastapi_cognito.egg-info/top_level.txt
```

### Comparing `fastapi-cognito-2.4.0/LICENSE.txt` & `fastapi-cognito-2.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastapi-cognito-2.4.0/PKG-INFO` & `fastapi-cognito-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-cognito
-Version: 2.4.0
+Version: 2.4.1
 Summary: Basic AWS cognito authentication package for FastAPI
 Home-page: https://github.com/markomirosavljev/fastapi-cognito
 Author: Marko Mirosavljev
 Author-email: mirosavljevm023@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `fastapi-cognito-2.4.0/README.md` & `fastapi-cognito-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-cognito-2.4.0/setup.py` & `fastapi-cognito-2.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fastapi-cognito",
-    version="2.4.0",
+    version="2.4.1",
     author="Marko Mirosavljev",
     author_email="mirosavljevm023@gmail.com",
     description="Basic AWS cognito authentication package for FastAPI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/markomirosavljev/fastapi-cognito",
```

### Comparing `fastapi-cognito-2.4.0/src/fastapi_cognito/exceptions.py` & `fastapi-cognito-2.4.1/src/fastapi_cognito/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi-cognito-2.4.0/src/fastapi_cognito/fastapi_cognito.py` & `fastapi-cognito-2.4.1/src/fastapi_cognito/fastapi_cognito.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Dict, Any
 
 from cognitojwt import CognitoJWTException, decode_async as cognito_jwt_decode
 from fastapi.exceptions import HTTPException
 from jose import JWTError
 from pydantic_settings import BaseSettings
-from requests.exceptions import ConnectionError as HttpConnectionError
 from starlette.requests import Request
 
 from .exceptions import CognitoAuthError
 from .models import UserpoolModel, CognitoToken
 
 
 class CognitoAuth(object):
@@ -195,20 +194,14 @@
                        " your userpool_id config might be incorrect."
             )
         except (ValueError, JWTError):
             raise HTTPException(
                 status_code=401,
                 detail="Malformed authentication token"
             )
-        except HttpConnectionError:
-            raise HTTPException(
-                status_code=500,
-                detail="Unable to establish connection with AWS, "
-                       "your userpool region config might be incorrect."
-            )
 
     async def auth_optional(self, request: Request) -> Any:
         """
         Optional authentication, method will try to parse `Authorization` header
         if present, else it will return None
         :param request: Incoming request
         :return: Token Model or None
```

### Comparing `fastapi-cognito-2.4.0/src/fastapi_cognito/models.py` & `fastapi-cognito-2.4.1/src/fastapi_cognito/models.py`

 * *Files identical despite different names*

### Comparing `fastapi-cognito-2.4.0/src/fastapi_cognito/settings_parsers.py` & `fastapi-cognito-2.4.1/src/fastapi_cognito/settings_parsers.py`

 * *Files identical despite different names*

### Comparing `fastapi-cognito-2.4.0/src/fastapi_cognito.egg-info/PKG-INFO` & `fastapi-cognito-2.4.1/src/fastapi_cognito.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-cognito
-Version: 2.4.0
+Version: 2.4.1
 Summary: Basic AWS cognito authentication package for FastAPI
 Home-page: https://github.com/markomirosavljev/fastapi-cognito
 Author: Marko Mirosavljev
 Author-email: mirosavljevm023@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

