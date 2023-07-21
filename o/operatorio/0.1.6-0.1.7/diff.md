# Comparing `tmp/operatorio-0.1.6.tar.gz` & `tmp/operatorio-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "operatorio-0.1.6.tar", last modified: Fri Jul 21 19:15:37 2023, max compression
+gzip compressed data, was "operatorio-0.1.7.tar", last modified: Fri Jul 21 19:18:31 2023, max compression
```

## Comparing `operatorio-0.1.6.tar` & `operatorio-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 19:15:37.663414 operatorio-0.1.6/
--rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 19:15:37.663158 operatorio-0.1.6/PKG-INFO
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 19:15:37.661097 operatorio-0.1.6/operatorio/
--rw-r--r--   0 david      (501) staff       (20)      125 2023-07-21 18:45:08.000000 operatorio-0.1.6/operatorio/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     1838 2023-07-21 19:15:07.000000 operatorio-0.1.6/operatorio/main.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 19:15:37.662860 operatorio-0.1.6/operatorio.egg-info/
--rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 19:15:37.000000 operatorio-0.1.6/operatorio.egg-info/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)      219 2023-07-21 19:15:37.000000 operatorio-0.1.6/operatorio.egg-info/SOURCES.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2023-07-21 19:15:37.000000 operatorio-0.1.6/operatorio.egg-info/dependency_links.txt
--rw-r--r--   0 david      (501) staff       (20)        9 2023-07-21 19:15:37.000000 operatorio-0.1.6/operatorio.egg-info/requires.txt
--rw-r--r--   0 david      (501) staff       (20)       11 2023-07-21 19:15:37.000000 operatorio-0.1.6/operatorio.egg-info/top_level.txt
--rw-r--r--   0 david      (501) staff       (20)       38 2023-07-21 19:15:37.663464 operatorio-0.1.6/setup.cfg
--rw-r--r--   0 david      (501) staff       (20)      532 2023-07-21 19:15:34.000000 operatorio-0.1.6/setup.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 19:18:31.873286 operatorio-0.1.7/
+-rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 19:18:31.873025 operatorio-0.1.7/PKG-INFO
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 19:18:31.871976 operatorio-0.1.7/operatorio/
+-rw-r--r--   0 david      (501) staff       (20)      125 2023-07-21 18:45:08.000000 operatorio-0.1.7/operatorio/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     1962 2023-07-21 19:17:57.000000 operatorio-0.1.7/operatorio/main.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 19:18:31.872789 operatorio-0.1.7/operatorio.egg-info/
+-rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 19:18:31.000000 operatorio-0.1.7/operatorio.egg-info/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)      219 2023-07-21 19:18:31.000000 operatorio-0.1.7/operatorio.egg-info/SOURCES.txt
+-rw-r--r--   0 david      (501) staff       (20)        1 2023-07-21 19:18:31.000000 operatorio-0.1.7/operatorio.egg-info/dependency_links.txt
+-rw-r--r--   0 david      (501) staff       (20)        9 2023-07-21 19:18:31.000000 operatorio-0.1.7/operatorio.egg-info/requires.txt
+-rw-r--r--   0 david      (501) staff       (20)       11 2023-07-21 19:18:31.000000 operatorio-0.1.7/operatorio.egg-info/top_level.txt
+-rw-r--r--   0 david      (501) staff       (20)       38 2023-07-21 19:18:31.873333 operatorio-0.1.7/setup.cfg
+-rw-r--r--   0 david      (501) staff       (20)      532 2023-07-21 19:18:04.000000 operatorio-0.1.7/setup.py
```

### Comparing `operatorio-0.1.6/operatorio/main.py` & `operatorio-0.1.7/operatorio/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import requests
-from dataclasses import dataclass
+from dataclasses import dataclass, asdict
 from enum import Enum
 from typing import List, Union, Optional
 from requests.models import PreparedRequest
 
 # Models
 class EntityType(Enum):
     wallet = "wallet"
@@ -28,14 +28,17 @@
 @dataclass
 class Query:
     query: str
     blockchain: str
     entity_type: EntityType
     query_by: List[str]
 
+    def to_dict(self):
+        return {k: v.value if isinstance(v, Enum) else v for k, v in asdict(self).items()}
+
 @dataclass
 class ValidationError:
     loc: List[Union[str, int]]
     msg: str
     type: str
 
 @dataclass
@@ -59,15 +62,15 @@
         self.api_key = api_key
 
     def search(self, query: Query) -> Entities:
         headers = {"X-API-Key": self.api_key}
         response = requests.post(
             self.BASE_URL + 'search/',
             headers=headers,
-            json=query.__dict__
+            json=query.to_dict()
         )
         
         if response.status_code == 200:
             data = response.json()
             entity = data.get('entity')
             matches = [Entity(**match) for match in data.get('matches', [])]
             return Entities(entity=entity, matches=matches)
```

### Comparing `operatorio-0.1.6/setup.py` & `operatorio-0.1.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="operatorio",
-    version="0.1.6",
+    version="0.1.7",
     description="A Python SDK for the Operator Search API.",
     author="David Shi",
     author_email="david@operator.io",
     url="https://github.com/operatorlabs/sdk/python",
     packages=['operatorio'],  
     install_requires=[
         'requests',
```

