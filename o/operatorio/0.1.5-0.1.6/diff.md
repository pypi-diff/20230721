# Comparing `tmp/operatorio-0.1.5.tar.gz` & `tmp/operatorio-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "operatorio-0.1.5.tar", last modified: Fri Jul 21 19:03:30 2023, max compression
+gzip compressed data, was "operatorio-0.1.6.tar", last modified: Fri Jul 21 19:15:37 2023, max compression
```

## Comparing `operatorio-0.1.5.tar` & `operatorio-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 19:03:30.587146 operatorio-0.1.5/
--rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 19:03:30.586979 operatorio-0.1.5/PKG-INFO
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 19:03:30.585435 operatorio-0.1.5/operatorio/
--rw-r--r--   0 david      (501) staff       (20)      125 2023-07-21 18:45:08.000000 operatorio-0.1.5/operatorio/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     1729 2023-07-21 19:03:10.000000 operatorio-0.1.5/operatorio/main.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 19:03:30.586779 operatorio-0.1.5/operatorio.egg-info/
--rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 19:03:30.000000 operatorio-0.1.5/operatorio.egg-info/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)      219 2023-07-21 19:03:30.000000 operatorio-0.1.5/operatorio.egg-info/SOURCES.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2023-07-21 19:03:30.000000 operatorio-0.1.5/operatorio.egg-info/dependency_links.txt
--rw-r--r--   0 david      (501) staff       (20)        9 2023-07-21 19:03:30.000000 operatorio-0.1.5/operatorio.egg-info/requires.txt
--rw-r--r--   0 david      (501) staff       (20)       11 2023-07-21 19:03:30.000000 operatorio-0.1.5/operatorio.egg-info/top_level.txt
--rw-r--r--   0 david      (501) staff       (20)       38 2023-07-21 19:03:30.587202 operatorio-0.1.5/setup.cfg
--rw-r--r--   0 david      (501) staff       (20)      532 2023-07-21 19:03:27.000000 operatorio-0.1.5/setup.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 19:15:37.663414 operatorio-0.1.6/
+-rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 19:15:37.663158 operatorio-0.1.6/PKG-INFO
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 19:15:37.661097 operatorio-0.1.6/operatorio/
+-rw-r--r--   0 david      (501) staff       (20)      125 2023-07-21 18:45:08.000000 operatorio-0.1.6/operatorio/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     1838 2023-07-21 19:15:07.000000 operatorio-0.1.6/operatorio/main.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 19:15:37.662860 operatorio-0.1.6/operatorio.egg-info/
+-rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 19:15:37.000000 operatorio-0.1.6/operatorio.egg-info/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)      219 2023-07-21 19:15:37.000000 operatorio-0.1.6/operatorio.egg-info/SOURCES.txt
+-rw-r--r--   0 david      (501) staff       (20)        1 2023-07-21 19:15:37.000000 operatorio-0.1.6/operatorio.egg-info/dependency_links.txt
+-rw-r--r--   0 david      (501) staff       (20)        9 2023-07-21 19:15:37.000000 operatorio-0.1.6/operatorio.egg-info/requires.txt
+-rw-r--r--   0 david      (501) staff       (20)       11 2023-07-21 19:15:37.000000 operatorio-0.1.6/operatorio.egg-info/top_level.txt
+-rw-r--r--   0 david      (501) staff       (20)       38 2023-07-21 19:15:37.663464 operatorio-0.1.6/setup.cfg
+-rw-r--r--   0 david      (501) staff       (20)      532 2023-07-21 19:15:34.000000 operatorio-0.1.6/setup.py
```

### Comparing `operatorio-0.1.5/operatorio/main.py` & `operatorio-0.1.6/operatorio/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
-from dataclasses import dataclass, asdict
+from dataclasses import dataclass
 from enum import Enum
-from typing import List, Union
+from typing import List, Union, Optional
+from requests.models import PreparedRequest
 
 # Models
 class EntityType(Enum):
     wallet = "wallet"
     identity = "identity"
     contract = "contract"
     nft = "nft"
@@ -17,15 +18,15 @@
     description: str
     semantic_similarity: float
     network_value: float = 0.0
     rank: float = 0.0
 
 @dataclass
 class Entities:
-    entity: str
+    entity: Optional[str]
     matches: List[Entity]
 
 @dataclass
 class Query:
     query: str
     blockchain: str
     entity_type: EntityType
@@ -55,21 +56,22 @@
     BASE_URL = 'https://api.operator.io/'
 
     def __init__(self, api_key: str):
         self.api_key = api_key
 
     def search(self, query: Query) -> Entities:
         headers = {"X-API-Key": self.api_key}
-        query_dict = asdict(query)
-        query_dict['entity_type'] = query_dict['entity_type'].value
         response = requests.post(
-            OperatorSearchAPI.BASE_URL + 'search/',
+            self.BASE_URL + 'search/',
             headers=headers,
-            json=query_dict
+            json=query.__dict__
         )
         
         if response.status_code == 200:
-            return Entities(**response.json())
+            data = response.json()
+            entity = data.get('entity')
+            matches = [Entity(**match) for match in data.get('matches', [])]
+            return Entities(entity=entity, matches=matches)
         elif response.status_code == 422:
             raise ApiException(HTTPValidationError(**response.json()))
         else:
             raise ApiException(response.json())
```

### Comparing `operatorio-0.1.5/setup.py` & `operatorio-0.1.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="operatorio",
-    version="0.1.5",
+    version="0.1.6",
     description="A Python SDK for the Operator Search API.",
     author="David Shi",
     author_email="david@operator.io",
     url="https://github.com/operatorlabs/sdk/python",
     packages=['operatorio'],  
     install_requires=[
         'requests',
```

