# Comparing `tmp/aiohttp_s3_client-0.8.2.tar.gz` & `tmp/aiohttp_s3_client-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp_s3_client-0.8.2.tar", max compression
+gzip compressed data, was "aiohttp_s3_client-0.8.7.tar", max compression
```

## Comparing `aiohttp_s3_client-0.8.2.tar` & `aiohttp_s3_client-0.8.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11358 2023-03-09 14:25:51.490304 aiohttp_s3_client-0.8.2/LICENSE
--rw-r--r--   0        0        0    10495 2023-03-09 14:25:51.490304 aiohttp_s3_client-0.8.2/LICENSE.md
--rw-r--r--   0        0        0     4323 2023-03-09 14:25:51.490304 aiohttp_s3_client-0.8.2/README.md
--rw-r--r--   0        0        0      199 2023-03-09 14:25:51.490304 aiohttp_s3_client-0.8.2/aiohttp_s3_client/__init__.py
--rw-r--r--   0        0        0    24325 2023-03-09 14:25:51.490304 aiohttp_s3_client-0.8.2/aiohttp_s3_client/client.py
--rw-r--r--   0        0        0        0 2023-03-09 14:25:51.490304 aiohttp_s3_client-0.8.2/aiohttp_s3_client/py.typed
--rw-r--r--   0        0        0      152 2023-03-09 14:26:15.886224 aiohttp_s3_client-0.8.2/aiohttp_s3_client/version.py
--rw-r--r--   0        0        0     2573 2023-03-09 14:25:51.490304 aiohttp_s3_client-0.8.2/aiohttp_s3_client/xml.py
--rw-r--r--   0        0        0     2160 2023-03-09 14:26:15.886224 aiohttp_s3_client-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     6112 1970-01-01 00:00:00.000000 aiohttp_s3_client-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-22 08:10:34.021383 aiohttp_s3_client-0.8.7/LICENSE
+-rw-r--r--   0        0        0    10495 2023-06-22 08:10:34.021383 aiohttp_s3_client-0.8.7/LICENSE.md
+-rw-r--r--   0        0        0     4558 2023-06-22 08:10:34.021383 aiohttp_s3_client-0.8.7/README.md
+-rw-r--r--   0        0        0      199 2023-06-22 08:10:34.021383 aiohttp_s3_client-0.8.7/aiohttp_s3_client/__init__.py
+-rw-r--r--   0        0        0    24400 2023-06-22 08:10:34.021383 aiohttp_s3_client-0.8.7/aiohttp_s3_client/client.py
+-rw-r--r--   0        0        0        0 2023-06-22 08:10:34.021383 aiohttp_s3_client-0.8.7/aiohttp_s3_client/py.typed
+-rw-r--r--   0        0        0      152 2023-06-22 08:10:56.388892 aiohttp_s3_client-0.8.7/aiohttp_s3_client/version.py
+-rw-r--r--   0        0        0     2573 2023-06-22 08:10:34.021383 aiohttp_s3_client-0.8.7/aiohttp_s3_client/xml.py
+-rw-r--r--   0        0        0     2160 2023-06-22 08:10:56.388892 aiohttp_s3_client-0.8.7/pyproject.toml
+-rw-r--r--   0        0        0     6149 1970-01-01 00:00:00.000000 aiohttp_s3_client-0.8.7/PKG-INFO
```

### Comparing `aiohttp_s3_client-0.8.2/LICENSE` & `aiohttp_s3_client-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohttp_s3_client-0.8.2/LICENSE.md` & `aiohttp_s3_client-0.8.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aiohttp_s3_client-0.8.2/README.md` & `aiohttp_s3_client-0.8.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -83,14 +83,22 @@
 ```python
 client = S3Client(url="http://your-s3-host", access_key_id="key_id",
                   secret_access_key="access_key", ...)
 
 client = S3Client(url="http://key_id:access_key@your-s3-host", ...)
 ```
 
+Temporary credentials are supported by using a token.
+
+```python
+client = S3Client(url="http://your-s3-host", access_key_id="key_id",
+                  secret_access_key="access_key", session_token="token",
+                  ...)
+```
+
 ## Multipart upload
 
 For uploading large files [multipart uploading](https://docs.aws.amazon.com/AmazonS3/latest/userguide/mpuoverview.html)
 can be used. It allows you to asynchronously upload multiple parts of a file
 to S3.
 S3Client handles retries of part uploads and calculates part hash for integrity checks.
```

### Comparing `aiohttp_s3_client-0.8.2/aiohttp_s3_client/client.py` & `aiohttp_s3_client-0.8.7/aiohttp_s3_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,15 @@
 
 
 class S3Client:
     def __init__(
         self, session: ClientSession, url: URL,
         secret_access_key: t.Optional[str] = None,
         access_key_id: t.Optional[str] = None,
+        session_token: t.Optional[str] = None,
         region: str = "",
     ):
         access_key_id = access_key_id or url.user
         secret_access_key = secret_access_key or url.password
 
         if not access_key_id:
             raise ValueError(
@@ -142,15 +143,15 @@
                 "or as username in the url",
             )
 
         self._url = URL(url).with_user(None).with_password(None)
         self._session = session
         self._signer = AwsRequestSigner(
             region=region, service="s3", access_key_id=access_key_id,
-            secret_access_key=secret_access_key,
+            secret_access_key=secret_access_key, session_token=session_token
         )
 
     @property
     def url(self) -> URL:
         return self._url
 
     def request(
```

### Comparing `aiohttp_s3_client-0.8.2/aiohttp_s3_client/xml.py` & `aiohttp_s3_client-0.8.7/aiohttp_s3_client/xml.py`

 * *Files identical despite different names*

### Comparing `aiohttp_s3_client-0.8.2/pyproject.toml` & `aiohttp_s3_client-0.8.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "aiohttp-s3-client"
 # Dummy version which will be rewritten with poem-plugins
-version = "0.8.2"
+version = "0.8.7"
 description = "The simple module for putting and getting object from Amazon S3 compatible endpoints"
 authors = [
     "Dmitry Orlov <me@mosquito.su>",
     "Yuri Shikanov <dizballanze@gmail.com>",
     "Alexander Vasin <hi@alvass.in>"
 ]
 license = "Apache Software License"
@@ -35,15 +35,15 @@
 [tool.poetry.urls]
 "Source" = "https://github.com/aiokitchen/aiohttp-s3-client"
 "Tracker" = "https://github.com/aiokitchen/aiohttp-s3-client/issues"
 
 [tool.poetry.dependencies]
 aiohttp = "^3"
 aiomisc = "^17"
-aws-request-signer = "1.0.0"
+aws-request-signer = "1.2.0"
 python = "^3.7"
 
 [tool.poetry.group.dev.dependencies]
 aiomisc-pytest = "^1.1"
 coverage = "!=4.3"
 coveralls = "^3.3.1"
 mypy = "^1.0.1"
```

### Comparing `aiohttp_s3_client-0.8.2/PKG-INFO` & `aiohttp_s3_client-0.8.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp-s3-client
-Version: 0.8.2
+Version: 0.8.7
 Summary: The simple module for putting and getting object from Amazon S3 compatible endpoints
 Home-page: https://github.com/aiokitchen/aiohttp-s3-client
 License: Apache Software License
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -18,26 +18,22 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: aiohttp (>=3,<4)
 Requires-Dist: aiomisc (>=17,<18)
-Requires-Dist: aws-request-signer (==1.0.0)
+Requires-Dist: aws-request-signer (==1.2.0)
 Project-URL: Source, https://github.com/aiokitchen/aiohttp-s3-client
 Project-URL: Tracker, https://github.com/aiokitchen/aiohttp-s3-client/issues
 Description-Content-Type: text/markdown
 
 aiohttp-s3-client
 ================
 
@@ -123,14 +119,22 @@
 ```python
 client = S3Client(url="http://your-s3-host", access_key_id="key_id",
                   secret_access_key="access_key", ...)
 
 client = S3Client(url="http://key_id:access_key@your-s3-host", ...)
 ```
 
+Temporary credentials are supported by using a token.
+
+```python
+client = S3Client(url="http://your-s3-host", access_key_id="key_id",
+                  secret_access_key="access_key", session_token="token",
+                  ...)
+```
+
 ## Multipart upload
 
 For uploading large files [multipart uploading](https://docs.aws.amazon.com/AmazonS3/latest/userguide/mpuoverview.html)
 can be used. It allows you to asynchronously upload multiple parts of a file
 to S3.
 S3Client handles retries of part uploads and calculates part hash for integrity checks.
```

