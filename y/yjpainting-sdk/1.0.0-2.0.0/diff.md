# Comparing `tmp/yjpainting-sdk-1.0.0.tar.gz` & `tmp/yjpainting-sdk-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yjpainting-sdk-1.0.0.tar", last modified: Fri Jul 14 10:29:36 2023, max compression
+gzip compressed data, was "yjpainting-sdk-2.0.0.tar", last modified: Fri Jul 21 07:55:00 2023, max compression
```

## Comparing `yjpainting-sdk-1.0.0.tar` & `yjpainting-sdk-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 yangruiqi   (502) staff       (20)        0 2023-07-14 10:29:36.407641 yjpainting-sdk-1.0.0/
--rw-r--r--   0 yangruiqi   (502) staff       (20)      156 2023-07-14 10:29:36.404991 yjpainting-sdk-1.0.0/PKG-INFO
-drwxr-xr-x   0 yangruiqi   (502) staff       (20)        0 2023-07-14 10:29:36.371277 yjpainting-sdk-1.0.0/openapi/
--rw-r--r--   0 yangruiqi   (502) staff       (20)        0 2023-07-14 10:18:58.000000 yjpainting-sdk-1.0.0/openapi/__init__.py
--rw-r--r--   0 yangruiqi   (502) staff       (20)     1630 2023-07-14 10:02:13.000000 yjpainting-sdk-1.0.0/openapi/client.py
--rw-r--r--   0 yangruiqi   (502) staff       (20)     3291 2023-07-14 10:01:52.000000 yjpainting-sdk-1.0.0/openapi/service.py
--rw-r--r--   0 yangruiqi   (502) staff       (20)       38 2023-07-14 10:29:36.407965 yjpainting-sdk-1.0.0/setup.cfg
--rw-r--r--   0 yangruiqi   (502) staff       (20)      284 2023-07-14 10:27:25.000000 yjpainting-sdk-1.0.0/setup.py
-drwxr-xr-x   0 yangruiqi   (502) staff       (20)        0 2023-07-14 10:29:36.403617 yjpainting-sdk-1.0.0/yjpainting_sdk.egg-info/
--rw-r--r--   0 yangruiqi   (502) staff       (20)      156 2023-07-14 10:29:35.000000 yjpainting-sdk-1.0.0/yjpainting_sdk.egg-info/PKG-INFO
--rw-r--r--   0 yangruiqi   (502) staff       (20)      254 2023-07-14 10:29:36.000000 yjpainting-sdk-1.0.0/yjpainting_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 yangruiqi   (502) staff       (20)        1 2023-07-14 10:29:35.000000 yjpainting-sdk-1.0.0/yjpainting_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 yangruiqi   (502) staff       (20)        9 2023-07-14 10:29:35.000000 yjpainting-sdk-1.0.0/yjpainting_sdk.egg-info/requires.txt
--rw-r--r--   0 yangruiqi   (502) staff       (20)        8 2023-07-14 10:29:35.000000 yjpainting-sdk-1.0.0/yjpainting_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 yangruiqi   (502) staff       (20)        0 2023-07-21 07:55:00.760275 yjpainting-sdk-2.0.0/
+-rw-r--r--   0 yangruiqi   (502) staff       (20)      156 2023-07-21 07:55:00.759863 yjpainting-sdk-2.0.0/PKG-INFO
+drwxr-xr-x   0 yangruiqi   (502) staff       (20)        0 2023-07-21 07:55:00.755347 yjpainting-sdk-2.0.0/openapi/
+-rw-r--r--   0 yangruiqi   (502) staff       (20)       35 2023-07-21 07:45:04.000000 yjpainting-sdk-2.0.0/openapi/__init__.py
+-rw-r--r--   0 yangruiqi   (502) staff       (20)     1630 2023-07-20 03:37:22.000000 yjpainting-sdk-2.0.0/openapi/client.py
+-rw-r--r--   0 yangruiqi   (502) staff       (20)     3292 2023-07-21 07:45:30.000000 yjpainting-sdk-2.0.0/openapi/service.py
+-rw-r--r--   0 yangruiqi   (502) staff       (20)       38 2023-07-21 07:55:00.760429 yjpainting-sdk-2.0.0/setup.cfg
+-rw-r--r--   0 yangruiqi   (502) staff       (20)      284 2023-07-21 07:51:17.000000 yjpainting-sdk-2.0.0/setup.py
+drwxr-xr-x   0 yangruiqi   (502) staff       (20)        0 2023-07-21 07:55:00.759209 yjpainting-sdk-2.0.0/yjpainting_sdk.egg-info/
+-rw-r--r--   0 yangruiqi   (502) staff       (20)      156 2023-07-21 07:55:00.000000 yjpainting-sdk-2.0.0/yjpainting_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 yangruiqi   (502) staff       (20)      254 2023-07-21 07:55:00.000000 yjpainting-sdk-2.0.0/yjpainting_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 yangruiqi   (502) staff       (20)        1 2023-07-21 07:55:00.000000 yjpainting-sdk-2.0.0/yjpainting_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 yangruiqi   (502) staff       (20)        9 2023-07-21 07:55:00.000000 yjpainting-sdk-2.0.0/yjpainting_sdk.egg-info/requires.txt
+-rw-r--r--   0 yangruiqi   (502) staff       (20)        8 2023-07-21 07:55:00.000000 yjpainting-sdk-2.0.0/yjpainting_sdk.egg-info/top_level.txt
```

### Comparing `yjpainting-sdk-1.0.0/openapi/client.py` & `yjpainting-sdk-2.0.0/openapi/client.py`

 * *Files identical despite different names*

### Comparing `yjpainting-sdk-1.0.0/openapi/service.py` & `yjpainting-sdk-2.0.0/openapi/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from client import Client
+from .client import Client
 import time
 
 
 class YJPaintingSDK:
     def __init__(self, apiKey, apiSecret):
         self.client = Client(apiKey=apiKey, apiSecret=apiSecret)
```

