# Comparing `tmp/operatorio-0.1.3.tar.gz` & `tmp/operatorio-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "operatorio-0.1.3.tar", last modified: Fri Jul 21 06:13:47 2023, max compression
+gzip compressed data, was "operatorio-0.1.4.tar", last modified: Fri Jul 21 18:45:39 2023, max compression
```

## Comparing `operatorio-0.1.3.tar` & `operatorio-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 06:13:47.774939 operatorio-0.1.3/
--rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 06:13:47.774694 operatorio-0.1.3/PKG-INFO
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 06:13:47.773165 operatorio-0.1.3/operatorio/
--rw-r--r--   0 david      (501) staff       (20)      113 2023-07-21 06:08:03.000000 operatorio-0.1.3/operatorio/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     1322 2023-07-21 04:30:59.000000 operatorio-0.1.3/operatorio/main.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 06:13:47.774375 operatorio-0.1.3/operatorio.egg-info/
--rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 06:13:47.000000 operatorio-0.1.3/operatorio.egg-info/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)      219 2023-07-21 06:13:47.000000 operatorio-0.1.3/operatorio.egg-info/SOURCES.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2023-07-21 06:13:47.000000 operatorio-0.1.3/operatorio.egg-info/dependency_links.txt
--rw-r--r--   0 david      (501) staff       (20)        9 2023-07-21 06:13:47.000000 operatorio-0.1.3/operatorio.egg-info/requires.txt
--rw-r--r--   0 david      (501) staff       (20)       11 2023-07-21 06:13:47.000000 operatorio-0.1.3/operatorio.egg-info/top_level.txt
--rw-r--r--   0 david      (501) staff       (20)       38 2023-07-21 06:13:47.775004 operatorio-0.1.3/setup.cfg
--rw-r--r--   0 david      (501) staff       (20)      532 2023-07-21 06:13:39.000000 operatorio-0.1.3/setup.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 18:45:39.546040 operatorio-0.1.4/
+-rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 18:45:39.545863 operatorio-0.1.4/PKG-INFO
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 18:45:39.544365 operatorio-0.1.4/operatorio/
+-rw-r--r--   0 david      (501) staff       (20)      125 2023-07-21 18:45:08.000000 operatorio-0.1.4/operatorio/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     1622 2023-07-21 18:35:44.000000 operatorio-0.1.4/operatorio/main.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 18:45:39.545578 operatorio-0.1.4/operatorio.egg-info/
+-rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 18:45:39.000000 operatorio-0.1.4/operatorio.egg-info/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)      219 2023-07-21 18:45:39.000000 operatorio-0.1.4/operatorio.egg-info/SOURCES.txt
+-rw-r--r--   0 david      (501) staff       (20)        1 2023-07-21 18:45:39.000000 operatorio-0.1.4/operatorio.egg-info/dependency_links.txt
+-rw-r--r--   0 david      (501) staff       (20)        9 2023-07-21 18:45:39.000000 operatorio-0.1.4/operatorio.egg-info/requires.txt
+-rw-r--r--   0 david      (501) staff       (20)       11 2023-07-21 18:45:39.000000 operatorio-0.1.4/operatorio.egg-info/top_level.txt
+-rw-r--r--   0 david      (501) staff       (20)       38 2023-07-21 18:45:39.546091 operatorio-0.1.4/setup.cfg
+-rw-r--r--   0 david      (501) staff       (20)      532 2023-07-21 18:45:28.000000 operatorio-0.1.4/setup.py
```

### Comparing `operatorio-0.1.3/operatorio/main.py` & `operatorio-0.1.4/operatorio/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 import requests
 from dataclasses import dataclass
+from enum import Enum
 from typing import List, Union
 
 # Models
+class EntityType(Enum):
+    wallet = "wallet"
+    identity = "identity"
+    contract = "contract"
+    nft = "nft"
+    token = "token"
+
 @dataclass
 class Entity:
     address: str
     description: str
     semantic_similarity: float
     network_value: float = 0.0
     rank: float = 0.0
@@ -16,15 +24,16 @@
     entity: str
     matches: List[Entity]
 
 @dataclass
 class Query:
     query: str
     blockchain: str
-    entity_type: str
+    entity_type: EntityType
+    query_by: List[str]
 
 @dataclass
 class ValidationError:
     loc: List[Union[str, int]]
     msg: str
     type: str
 
@@ -47,16 +56,18 @@
 
     def __init__(self, api_key: str):
         self.api_key = api_key
 
     def search(self, query: Query) -> Entities:
         headers = {"X-API-Key": self.api_key}
         response = requests.post(
-            OperatorSearchAPI.BASE_URL + '/search/',
+            OperatorSearchAPI.BASE_URL + 'search/',
             headers=headers,
             json=query.__dict__
         )
         
         if response.status_code == 200:
             return Entities(**response.json())
+        elif response.status_code == 422:
+            raise ApiException(HTTPValidationError(**response.json()))
         else:
             raise ApiException(response.json())
```

### Comparing `operatorio-0.1.3/setup.py` & `operatorio-0.1.4/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="operatorio",
-    version="0.1.3",
+    version="0.1.4",
     description="A Python SDK for the Operator Search API.",
     author="David Shi",
     author_email="david@operator.io",
     url="https://github.com/operatorlabs/sdk/python",
     packages=['operatorio'],  
     install_requires=[
         'requests',
```

