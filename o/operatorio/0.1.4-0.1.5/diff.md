# Comparing `tmp/operatorio-0.1.4.tar.gz` & `tmp/operatorio-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "operatorio-0.1.4.tar", last modified: Fri Jul 21 18:45:39 2023, max compression
+gzip compressed data, was "operatorio-0.1.5.tar", last modified: Fri Jul 21 19:03:30 2023, max compression
```

## Comparing `operatorio-0.1.4.tar` & `operatorio-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 18:45:39.546040 operatorio-0.1.4/
--rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 18:45:39.545863 operatorio-0.1.4/PKG-INFO
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 18:45:39.544365 operatorio-0.1.4/operatorio/
--rw-r--r--   0 david      (501) staff       (20)      125 2023-07-21 18:45:08.000000 operatorio-0.1.4/operatorio/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     1622 2023-07-21 18:35:44.000000 operatorio-0.1.4/operatorio/main.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 18:45:39.545578 operatorio-0.1.4/operatorio.egg-info/
--rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 18:45:39.000000 operatorio-0.1.4/operatorio.egg-info/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)      219 2023-07-21 18:45:39.000000 operatorio-0.1.4/operatorio.egg-info/SOURCES.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2023-07-21 18:45:39.000000 operatorio-0.1.4/operatorio.egg-info/dependency_links.txt
--rw-r--r--   0 david      (501) staff       (20)        9 2023-07-21 18:45:39.000000 operatorio-0.1.4/operatorio.egg-info/requires.txt
--rw-r--r--   0 david      (501) staff       (20)       11 2023-07-21 18:45:39.000000 operatorio-0.1.4/operatorio.egg-info/top_level.txt
--rw-r--r--   0 david      (501) staff       (20)       38 2023-07-21 18:45:39.546091 operatorio-0.1.4/setup.cfg
--rw-r--r--   0 david      (501) staff       (20)      532 2023-07-21 18:45:28.000000 operatorio-0.1.4/setup.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 19:03:30.587146 operatorio-0.1.5/
+-rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 19:03:30.586979 operatorio-0.1.5/PKG-INFO
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 19:03:30.585435 operatorio-0.1.5/operatorio/
+-rw-r--r--   0 david      (501) staff       (20)      125 2023-07-21 18:45:08.000000 operatorio-0.1.5/operatorio/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     1729 2023-07-21 19:03:10.000000 operatorio-0.1.5/operatorio/main.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 19:03:30.586779 operatorio-0.1.5/operatorio.egg-info/
+-rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 19:03:30.000000 operatorio-0.1.5/operatorio.egg-info/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)      219 2023-07-21 19:03:30.000000 operatorio-0.1.5/operatorio.egg-info/SOURCES.txt
+-rw-r--r--   0 david      (501) staff       (20)        1 2023-07-21 19:03:30.000000 operatorio-0.1.5/operatorio.egg-info/dependency_links.txt
+-rw-r--r--   0 david      (501) staff       (20)        9 2023-07-21 19:03:30.000000 operatorio-0.1.5/operatorio.egg-info/requires.txt
+-rw-r--r--   0 david      (501) staff       (20)       11 2023-07-21 19:03:30.000000 operatorio-0.1.5/operatorio.egg-info/top_level.txt
+-rw-r--r--   0 david      (501) staff       (20)       38 2023-07-21 19:03:30.587202 operatorio-0.1.5/setup.cfg
+-rw-r--r--   0 david      (501) staff       (20)      532 2023-07-21 19:03:27.000000 operatorio-0.1.5/setup.py
```

### Comparing `operatorio-0.1.4/operatorio/main.py` & `operatorio-0.1.5/operatorio/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import requests
-from dataclasses import dataclass
+from dataclasses import dataclass, asdict
 from enum import Enum
 from typing import List, Union
 
 # Models
 class EntityType(Enum):
     wallet = "wallet"
     identity = "identity"
@@ -55,18 +55,20 @@
     BASE_URL = 'https://api.operator.io/'
 
     def __init__(self, api_key: str):
         self.api_key = api_key
 
     def search(self, query: Query) -> Entities:
         headers = {"X-API-Key": self.api_key}
+        query_dict = asdict(query)
+        query_dict['entity_type'] = query_dict['entity_type'].value
         response = requests.post(
             OperatorSearchAPI.BASE_URL + 'search/',
             headers=headers,
-            json=query.__dict__
+            json=query_dict
         )
         
         if response.status_code == 200:
             return Entities(**response.json())
         elif response.status_code == 422:
             raise ApiException(HTTPValidationError(**response.json()))
         else:
```

### Comparing `operatorio-0.1.4/setup.py` & `operatorio-0.1.5/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="operatorio",
-    version="0.1.4",
+    version="0.1.5",
     description="A Python SDK for the Operator Search API.",
     author="David Shi",
     author_email="david@operator.io",
     url="https://github.com/operatorlabs/sdk/python",
     packages=['operatorio'],  
     install_requires=[
         'requests',
```

