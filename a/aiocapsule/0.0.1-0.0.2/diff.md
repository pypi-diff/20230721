# Comparing `tmp/aiocapsule-0.0.1.tar.gz` & `tmp/aiocapsule-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocapsule-0.0.1.tar", last modified: Thu Jul 13 13:08:08 2023, max compression
+gzip compressed data, was "aiocapsule-0.0.2.tar", last modified: Fri Jul 21 00:25:18 2023, max compression
```

## Comparing `aiocapsule-0.0.1.tar` & `aiocapsule-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-sr-x   0 jovyan    (1000) jovyan    (1000)        0 2023-07-13 13:08:08.807114 aiocapsule-0.0.1/
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)    11357 2023-07-13 11:56:08.000000 aiocapsule-0.0.1/LICENSE
--rw-rw-r--   0 jovyan    (1000) jovyan    (1000)      111 2023-04-27 10:12:58.000000 aiocapsule-0.0.1/MANIFEST.in
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)     1315 2023-07-13 13:08:08.807114 aiocapsule-0.0.1/PKG-INFO
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)      497 2023-07-13 12:58:52.000000 aiocapsule-0.0.1/README.md
-drwxr-sr-x   0 jovyan    (1000) jovyan    (1000)        0 2023-07-13 13:08:08.807114 aiocapsule-0.0.1/aiocapsule/
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)       22 2023-07-13 12:58:48.000000 aiocapsule-0.0.1/aiocapsule/__init__.py
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)      403 2023-07-13 12:58:48.000000 aiocapsule-0.0.1/aiocapsule/_modidx.py
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)     1209 2023-07-13 12:58:48.000000 aiocapsule-0.0.1/aiocapsule/core.py
-drwxr-sr-x   0 jovyan    (1000) jovyan    (1000)        0 2023-07-13 13:08:08.807114 aiocapsule-0.0.1/aiocapsule.egg-info/
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)     1315 2023-07-13 13:08:08.000000 aiocapsule-0.0.1/aiocapsule.egg-info/PKG-INFO
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)      354 2023-07-13 13:08:08.000000 aiocapsule-0.0.1/aiocapsule.egg-info/SOURCES.txt
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)        1 2023-07-13 13:08:08.000000 aiocapsule-0.0.1/aiocapsule.egg-info/dependency_links.txt
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)       63 2023-07-13 13:08:08.000000 aiocapsule-0.0.1/aiocapsule.egg-info/entry_points.txt
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)        1 2023-07-13 12:42:58.000000 aiocapsule-0.0.1/aiocapsule.egg-info/not-zip-safe
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)       22 2023-07-13 13:08:08.000000 aiocapsule-0.0.1/aiocapsule.egg-info/requires.txt
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)       11 2023-07-13 13:08:08.000000 aiocapsule-0.0.1/aiocapsule.egg-info/top_level.txt
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)      976 2023-07-13 12:42:19.000000 aiocapsule-0.0.1/settings.ini
--rw-r--r--   0 jovyan    (1000) jovyan    (1000)       38 2023-07-13 13:08:08.807114 aiocapsule-0.0.1/setup.cfg
--rw-rw-r--   0 jovyan    (1000) jovyan    (1000)     2596 2023-04-27 10:12:58.000000 aiocapsule-0.0.1/setup.py
+drwxr-sr-x   0 jovyan    (1000) jovyan    (1000)        0 2023-07-21 00:25:18.238351 aiocapsule-0.0.2/
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)    11357 2023-07-21 00:06:15.000000 aiocapsule-0.0.2/LICENSE
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)      111 2023-07-21 00:06:15.000000 aiocapsule-0.0.2/MANIFEST.in
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)     2774 2023-07-21 00:25:18.238351 aiocapsule-0.0.2/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)     1956 2023-07-21 00:21:12.000000 aiocapsule-0.0.2/README.md
+drwxr-sr-x   0 jovyan    (1000) jovyan    (1000)        0 2023-07-21 00:25:18.226351 aiocapsule-0.0.2/aiocapsule/
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)       22 2023-07-21 00:21:07.000000 aiocapsule-0.0.2/aiocapsule/__init__.py
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)      383 2023-07-21 00:21:07.000000 aiocapsule-0.0.2/aiocapsule/_modidx.py
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)     1320 2023-07-21 00:21:07.000000 aiocapsule-0.0.2/aiocapsule/core.py
+drwxr-sr-x   0 jovyan    (1000) jovyan    (1000)        0 2023-07-21 00:25:18.238351 aiocapsule-0.0.2/aiocapsule.egg-info/
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)     2774 2023-07-21 00:25:18.000000 aiocapsule-0.0.2/aiocapsule.egg-info/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)      354 2023-07-21 00:25:18.000000 aiocapsule-0.0.2/aiocapsule.egg-info/SOURCES.txt
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)        1 2023-07-21 00:25:18.000000 aiocapsule-0.0.2/aiocapsule.egg-info/dependency_links.txt
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)       63 2023-07-21 00:25:18.000000 aiocapsule-0.0.2/aiocapsule.egg-info/entry_points.txt
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)        1 2023-07-21 00:07:58.000000 aiocapsule-0.0.2/aiocapsule.egg-info/not-zip-safe
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)       22 2023-07-21 00:25:18.000000 aiocapsule-0.0.2/aiocapsule.egg-info/requires.txt
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)       11 2023-07-21 00:25:18.000000 aiocapsule-0.0.2/aiocapsule.egg-info/top_level.txt
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)      976 2023-07-21 00:25:06.000000 aiocapsule-0.0.2/settings.ini
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)       38 2023-07-21 00:25:18.238351 aiocapsule-0.0.2/setup.cfg
+-rw-r--r--   0 jovyan    (1000) jovyan    (1000)     2596 2023-07-21 00:06:15.000000 aiocapsule-0.0.2/setup.py
```

### Comparing `aiocapsule-0.0.1/LICENSE` & `aiocapsule-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocapsule-0.0.1/aiocapsule/core.py` & `aiocapsule-0.0.2/aiocapsule/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 # %% ../nbs/core.ipynb 2
 from __future__ import annotations
 
 import aiohttp
 
 # %% auto 0
-__all__ = ['send_http_request']
+__all__ = ['request']
 
-# %% ../nbs/core.ipynb 4
-async def send_http_request(
-    method:str,
-    url:str,
-    headers:dict|None=None,
+# %% ../nbs/core.ipynb 5
+async def request(
+    method:str, # HTTP method: GET, POST, DELETE, PUT
+    url:str, # Request URL
+    headers:dict|None=None, # HTTP headers
     params:dict|None=None,
     data:dict|str|None=None,
     json:dict|None=None,
     proxy:str|None=None,
     auth:aiohttp.BasicAuth|None=None,
-    text:bool=False,
-) -> str|dict:
+    text:bool=False, # Return string? If not, return dict
+) -> str|dict: # HTML string or JSON dict
     "Asynchronously send a HTTP request with a new session and return the response."
     async with aiohttp.ClientSession(
         headers=headers,
         auth=auth,
     ) as session:
         methods = {
             'GET': session.get,
```

### Comparing `aiocapsule-0.0.1/settings.ini` & `aiocapsule-0.0.2/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = aiocapsule
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = aiocapsule
```

### Comparing `aiocapsule-0.0.1/setup.py` & `aiocapsule-0.0.2/setup.py`

 * *Files identical despite different names*

