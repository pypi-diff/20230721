# Comparing `tmp/lighthouseweb3-0.1.3.tar.gz` & `tmp/lighthouseweb3-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lighthouseweb3-0.1.3.tar", last modified: Tue May 23 09:34:14 2023, max compression
+gzip compressed data, was "lighthouseweb3-0.1.4.tar", last modified: Fri Jul 21 08:01:36 2023, max compression
```

## Comparing `lighthouseweb3-0.1.3.tar` & `lighthouseweb3-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 09:34:14.345396 lighthouseweb3-0.1.3/
--rw-rw-rw-   0        0        0    35562 2023-05-23 09:30:22.000000 lighthouseweb3-0.1.3/LICENSE.md
--rw-rw-rw-   0        0        0     2619 2023-05-23 09:34:14.345396 lighthouseweb3-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1650 2023-05-23 09:30:22.000000 lighthouseweb3-0.1.3/README.md
--rw-rw-rw-   0        0        0      113 2023-05-23 09:34:14.347926 lighthouseweb3-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1323 2023-05-23 09:33:55.000000 lighthouseweb3-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:34:14.293807 lighthouseweb3-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 09:34:14.302984 lighthouseweb3-0.1.3/src/lighthouseweb3/
--rw-rw-rw-   0        0        0     4600 2023-05-23 09:30:22.000000 lighthouseweb3-0.1.3/src/lighthouseweb3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:34:14.343999 lighthouseweb3-0.1.3/src/lighthouseweb3/functions/
--rw-rw-rw-   0        0        0        0 2023-05-23 09:30:22.000000 lighthouseweb3-0.1.3/src/lighthouseweb3/functions/__init__.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 09:30:22.000000 lighthouseweb3-0.1.3/src/lighthouseweb3/functions/axios.py
--rw-rw-rw-   0        0        0      419 2023-05-23 09:30:22.000000 lighthouseweb3-0.1.3/src/lighthouseweb3/functions/config.py
--rw-rw-rw-   0        0        0      435 2023-05-23 09:30:22.000000 lighthouseweb3-0.1.3/src/lighthouseweb3/functions/deal_status.py
--rw-rw-rw-   0        0        0     1633 2023-05-23 09:30:22.000000 lighthouseweb3-0.1.3/src/lighthouseweb3/functions/download.py
--rw-rw-rw-   0        0        0      712 2023-05-23 09:30:22.000000 lighthouseweb3-0.1.3/src/lighthouseweb3/functions/get_uploads.py
--rw-rw-rw-   0        0        0     1020 2023-05-23 09:30:22.000000 lighthouseweb3-0.1.3/src/lighthouseweb3/functions/types.py
--rw-rw-rw-   0        0        0     3073 2023-05-23 09:30:22.000000 lighthouseweb3-0.1.3/src/lighthouseweb3/functions/upload.py
--rw-rw-rw-   0        0        0     2183 2023-05-23 09:30:22.000000 lighthouseweb3-0.1.3/src/lighthouseweb3/functions/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:34:14.327545 lighthouseweb3-0.1.3/src/lighthouseweb3.egg-info/
--rw-rw-rw-   0        0        0     2619 2023-05-23 09:34:14.000000 lighthouseweb3-0.1.3/src/lighthouseweb3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      641 2023-05-23 09:34:14.000000 lighthouseweb3-0.1.3/src/lighthouseweb3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 09:34:14.000000 lighthouseweb3-0.1.3/src/lighthouseweb3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-23 09:34:14.000000 lighthouseweb3-0.1.3/src/lighthouseweb3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-23 09:34:14.000000 lighthouseweb3-0.1.3/src/lighthouseweb3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 08:01:36.838327 lighthouseweb3-0.1.4/
+-rw-rw-rw-   0        0        0    35562 2023-07-21 06:21:07.000000 lighthouseweb3-0.1.4/LICENSE.md
+-rw-rw-rw-   0        0        0     2619 2023-07-21 08:01:36.838327 lighthouseweb3-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1650 2023-07-21 06:21:07.000000 lighthouseweb3-0.1.4/README.md
+-rw-rw-rw-   0        0        0      113 2023-07-21 08:01:36.842885 lighthouseweb3-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1323 2023-07-21 07:59:59.000000 lighthouseweb3-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:01:36.796963 lighthouseweb3-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-21 08:01:36.802473 lighthouseweb3-0.1.4/src/lighthouseweb3/
+-rw-rw-rw-   0        0        0     3801 2023-07-21 07:14:52.000000 lighthouseweb3-0.1.4/src/lighthouseweb3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:01:36.836250 lighthouseweb3-0.1.4/src/lighthouseweb3/functions/
+-rw-rw-rw-   0        0        0        0 2023-07-21 06:21:07.000000 lighthouseweb3-0.1.4/src/lighthouseweb3/functions/__init__.py
+-rw-rw-rw-   0        0        0     2623 2023-07-21 06:21:41.000000 lighthouseweb3-0.1.4/src/lighthouseweb3/functions/axios.py
+-rw-rw-rw-   0        0        0      419 2023-07-21 06:21:07.000000 lighthouseweb3-0.1.4/src/lighthouseweb3/functions/config.py
+-rw-rw-rw-   0        0        0      364 2023-07-21 06:21:41.000000 lighthouseweb3-0.1.4/src/lighthouseweb3/functions/deal_status.py
+-rw-rw-rw-   0        0        0     1633 2023-07-21 06:21:07.000000 lighthouseweb3-0.1.4/src/lighthouseweb3/functions/download.py
+-rw-rw-rw-   0        0        0      662 2023-07-21 06:21:41.000000 lighthouseweb3-0.1.4/src/lighthouseweb3/functions/get_uploads.py
+-rw-rw-rw-   0        0        0     2967 2023-07-21 06:21:41.000000 lighthouseweb3-0.1.4/src/lighthouseweb3/functions/upload.py
+-rw-rw-rw-   0        0        0     1961 2023-07-21 06:21:41.000000 lighthouseweb3-0.1.4/src/lighthouseweb3/functions/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:01:36.826954 lighthouseweb3-0.1.4/src/lighthouseweb3.egg-info/
+-rw-rw-rw-   0        0        0     2619 2023-07-21 08:01:36.000000 lighthouseweb3-0.1.4/src/lighthouseweb3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      603 2023-07-21 08:01:36.000000 lighthouseweb3-0.1.4/src/lighthouseweb3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 08:01:36.000000 lighthouseweb3-0.1.4/src/lighthouseweb3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-21 08:01:36.000000 lighthouseweb3-0.1.4/src/lighthouseweb3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-21 08:01:36.000000 lighthouseweb3-0.1.4/src/lighthouseweb3.egg-info/top_level.txt
```

### Comparing `lighthouseweb3-0.1.3/LICENSE.md` & `lighthouseweb3-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lighthouseweb3-0.1.3/PKG-INFO` & `lighthouseweb3-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lighthouseweb3
-Version: 0.1.3
+Version: 0.1.4
 Summary: Lighthouse Python SDK
 Home-page: https://github.com/lighthouse-web3/lighthouse-python-sdk
 Author: Ravish Sharma | Ayobami Oki | Nandit Mehra
 Author-email: nandit123@lighthouse.storage
 License: GNU GENERAL PUBLIC LICENSE
 Keywords: lighthouse storage sdk python filecoin ipfs web3 perpetual
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lighthouseweb3-0.1.3/README.md` & `lighthouseweb3-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `lighthouseweb3-0.1.3/setup.py` & `lighthouseweb3-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 import pathlib
 from setuptools import setup, find_packages
 
 setup(
     name="lighthouseweb3",
-    version="0.1.3",
+    version="0.1.4",
     license="GNU GENERAL PUBLIC LICENSE",
     description="Lighthouse Python SDK",
     author="Ravish Sharma | Ayobami Oki | Nandit Mehra",
     author_email="nandit123@lighthouse.storage",
     url="https://github.com/lighthouse-web3/lighthouse-python-sdk",
     packages=find_packages("src"),
     package_dir={"": "src"},
```

### Comparing `lighthouseweb3-0.1.3/src/lighthouseweb3/__init__.py` & `lighthouseweb3-0.1.4/src/lighthouseweb3/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,124 +1,107 @@
 #!/usr/bin/env python3
 
 import os
 import io
-from typing import List
-from .functions import upload as d, types as t, deal_status, get_uploads as getUploads, download as _download
+from .functions import upload as d,deal_status, get_uploads as getUploads, download as _download
 
 
 class Lighthouse:
     def __init__(self, token: str = ""):
         self.token = token or os.environ.get("LIGHTHOUSE_TOKEN", "")
         if not self.token:
             raise Exception(
                 "No token provided: Please provide a token or set the LIGHTHOUSE_TOKEN environment variable"
             )
 
-    def upload(self, source: str, tag: str = '') -> t.Upload:
+    def upload(self, source: str, tag: str = ''):
         """
         Upload a file or directory to the Lighthouse.
 
         :param source: str, path to file or directory
         :return: t.Upload, the upload result
         """
         try:
             return d.upload(source, self.token, tag)
         except Exception as e:
             raise e
 
-    def uploadBlob(self, source: io.BufferedReader, filename: str, tag: str = '') -> t.Upload:
+    def uploadBlob(self, source: io.BufferedReader, filename: str, tag: str = ''):
         """
         Upload Blob a file or directory to the Lighthouse.
 
         :param source: str, path to file or directory
         :return: t.Upload, the upload result
         """
         if not (hasattr(source, 'read') and hasattr(source, 'close')):
             raise TypeError("source must have 'read' and 'close' methods")
         try:
             return d.uploadBlob(source, filename, self.token, tag)
         except Exception as e:
             raise e
 
     @staticmethod
-    def downloadBlob(dist: io.BufferedWriter, cid: str, chunk_size=1024*1024*10) -> t.Upload:
+    def downloadBlob(dist: io.BufferedWriter, cid: str, chunk_size=1024*1024*10):
         """
         Download a Blob (file or directory) from the Lighthouse.
 
         :param dist: BufferedWriter, destination to write the downloaded data
         :param cid: str, Content Identifier for the data to be downloaded
         :param chunk_size: int, size of chunks in which the file will be downloaded (default: 10MB)
-        :param useCidAsTag: bool, flag to use CID as a tag (default: False)
         :return: t.Upload, the download result
         """
         if not (hasattr(dist, 'read') and hasattr(dist, 'close')):
             raise TypeError("source must have 'read' and 'close' methods")
         try:
             return _download.download_file_into_writable(cid, dist, chunk_size)
         except Exception as e:
             raise e
-
-    @staticmethod
-    def downloadBlob(dist: io.BufferedWriter, cid: str, chunk_size=1024*1024*10) -> t.Upload:
-        """
-        Download Blob a file or directory to the Lighthouse.
-
-        :param source: str, path to file or directory
-        :return: t.Upload, the upload result
-        """
-        if not (hasattr(dist, 'read') and hasattr(dist, 'close')):
-            raise TypeError("source must have 'read' and 'close' methods")
-        try:
-            return _download.download_file_into_writable(cid, dist, chunk_size)
-        except Exception as e:
-            raise e
-
+            
     @staticmethod
-    def getDealStatus(cid: str) -> List[t.DealData]:
+    def getDealStatus(cid: str):
         """
         Get deal status from the Lighthouse.
 
         :param cid: str, content identifier
         :return: List[t.DealData], list of deal data
         """
         try:
             return deal_status.get_deal_status(cid)
         except Exception as e:
             raise e
 
     @staticmethod
-    def getUploads(publicKey: str, pageNo: int = 1) -> List[t.DealData]:
+    def getUploads(publicKey: str, pageNo: int = 1):
         """
         Get uploads from the Lighthouse.
 
         :param publicKey: str, public key
         :param pageNo: int, page number (default: 1)
         :return: List[t.DealData], list of deal data
         """
         try:
             return getUploads.get_uploads(publicKey, pageNo)
         except Exception as e:
             raise e
 
     @staticmethod
-    def download(cid: str) -> bytes:
+    def download(cid: str):
         """
         Download content from the Lighthouse using its Content Identifier (CID).
 
         :param cid: str, Content Identifier for the data to be downloaded
         :param useCidAsTag: bool, flag to use CID as a tag (default: False)
         :return: bytes, the downloaded content
         """
         try:
             return _download.get_file(cid)
         except Exception as e:
             raise e
 
-    def getTagged(self, tag: str) -> t.Upload:
+    def getTagged(self, tag: str):
         """
         Retrieve an upload from the Lighthouse using its tag.
 
         :param tag: str, tag associated with the file or directory
         :return: t.Upload, the upload result
         """
         try:
```

### Comparing `lighthouseweb3-0.1.3/src/lighthouseweb3/functions/axios.py` & `lighthouseweb3-0.1.4/src/lighthouseweb3/functions/axios.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 #!/usr/bin/env python3
 
 from io import BufferedReader
 import json
-from typing import Dict, List, Tuple
 import requests as req
-from . import types as t
 from . import utils
 
 
 class Axios:
     """It's not axios, it's just a custom extensible wrapper for requests"""
 
     def __init__(self, url: str):
         self.url = url
 
-    def parse_url_query(self, query: Dict[str, str]):
+    def parse_url_query(self, query):
         try:
             if query is not None and isinstance(query, dict):
                 for key, value in query.items():
                     self.url += f"&{key}={value}"
         except Exception as e:
             raise e
 
-    def get(self, headers: Dict[str, str] = None, **kwargs) -> dict | Exception:
+    def get(self, headers = None, **kwargs) :
         try:
             self.parse_url_query(kwargs.get("query", None))
             r = req.get(self.url, headers=headers)
             r.raise_for_status()
             return r.json()
         except Exception as e:
             raise e
 
     def post(
-        self, body=None, headers: Dict[str, str] = None, **kwargs
-    ) -> dict | Exception:
+        self, body=None, headers= None, **kwargs
+    ):
         try:
             self.parse_url_query(kwargs.get("query", None))
             r = req.post(self.url, data=body, headers=headers)
             r.raise_for_status()
             return r.json()
         except Exception as e:
             raise e
 
     def post_files(
-        self, file: t.FileDict, headers: Dict[str, str] = None, **kwargs
-    ) -> dict | Exception:
+        self, file, headers = None, **kwargs
+    ) :
         try:
             self.parse_url_query(kwargs.get("query", None))
             files = utils.read_files_for_upload(file)
             r = req.post(self.url, headers=headers, files=files)
             r.raise_for_status()
             utils.close_files_after_upload(files)
             try:
@@ -57,16 +55,16 @@
                 temp = r.text.split("\n")
                 return json.loads(temp[len(temp) - 2])
         except Exception as e:
             utils.close_files_after_upload(files)
             raise e
 
     def post_blob(
-        self, file: BufferedReader, filename: str, headers: Dict[str, str] = None, **kwargs
-    ) -> dict | Exception:
+        self, file: BufferedReader, filename: str, headers = None, **kwargs
+    ) :
         try:
             self.parse_url_query(kwargs.get("query", None))
             files = [(
                 "file",
                 (
                     utils.extract_file_name(filename),
                     file.read(),
```

### Comparing `lighthouseweb3-0.1.3/src/lighthouseweb3/functions/download.py` & `lighthouseweb3-0.1.4/src/lighthouseweb3/functions/download.py`

 * *Files identical despite different names*

### Comparing `lighthouseweb3-0.1.3/src/lighthouseweb3/functions/upload.py` & `lighthouseweb3-0.1.4/src/lighthouseweb3/functions/upload.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #!/usr/bin/env python3
 
 from io import BufferedReader
 from typing import Dict, List, Tuple
 from .axios import Axios
 from .utils import is_dir, walk_dir_tree, extract_file_name, NamedBufferedReader
 from .config import Config
-from . import types as t
 
 
-def upload(source: str | BufferedReader | NamedBufferedReader, token: str, tag: str = "") -> t.Upload:
+def upload(source, token: str, tag: str = ""):
     """
     Deploy a file or directory to the lighthouse network
     @params {source}: str, path to file or directory
     @params {token}: str, lighthouse api token
     """
     # create headers
     headers = {
@@ -23,15 +22,15 @@
     }
     try:
         # create http object
         axios = Axios(Config.lighthouse_node + "/api/v0/add")
         # create list of files to upload
 
         if (isinstance(source, str)):
-            file_dict: t.FileDict = {}
+            file_dict = {}
 
             # check if source is a directory
             if is_dir(source):
                 # walk directory tree and add files to list
                 file_dict["files"], root = walk_dir_tree(source)
                 file_dict["is_dir"] = True
                 file_dict["path"] = root
@@ -53,15 +52,15 @@
                 "Authorization": f"Bearer {token}", })
         return {"data": hashData}
     except Exception as e:
         print(e)
         raise e
 
 
-def uploadBlob(source:  BufferedReader, filename: str, token: str, tag: str = "") -> t.Upload:
+def uploadBlob(source:  BufferedReader, filename: str, token: str, tag: str = ""):
     """
     Upload a Buffer or readable Object
     @params {source}: str, path to file or directory
     @params {token}: str, lighthouse api token
     """
     # create headers
     headers = {
```

### Comparing `lighthouseweb3-0.1.3/src/lighthouseweb3.egg-info/PKG-INFO` & `lighthouseweb3-0.1.4/src/lighthouseweb3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lighthouseweb3
-Version: 0.1.3
+Version: 0.1.4
 Summary: Lighthouse Python SDK
 Home-page: https://github.com/lighthouse-web3/lighthouse-python-sdk
 Author: Ravish Sharma | Ayobami Oki | Nandit Mehra
 Author-email: nandit123@lighthouse.storage
 License: GNU GENERAL PUBLIC LICENSE
 Keywords: lighthouse storage sdk python filecoin ipfs web3 perpetual
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lighthouseweb3-0.1.3/src/lighthouseweb3.egg-info/SOURCES.txt` & `lighthouseweb3-0.1.4/src/lighthouseweb3.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,10 +10,9 @@
 src/lighthouseweb3.egg-info/top_level.txt
 src/lighthouseweb3/functions/__init__.py
 src/lighthouseweb3/functions/axios.py
 src/lighthouseweb3/functions/config.py
 src/lighthouseweb3/functions/deal_status.py
 src/lighthouseweb3/functions/download.py
 src/lighthouseweb3/functions/get_uploads.py
-src/lighthouseweb3/functions/types.py
 src/lighthouseweb3/functions/upload.py
 src/lighthouseweb3/functions/utils.py
```

