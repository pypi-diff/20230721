# Comparing `tmp/vango-1.1.1.tar.gz` & `tmp/vango-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vango-1.1.1.tar", last modified: Wed Jul 19 03:02:36 2023, max compression
+gzip compressed data, was "dist/vango-1.1.5.tar", last modified: Fri Jul 21 10:36:08 2023, max compression
```

## Comparing `vango-1.1.1.tar` & `vango-1.1.5.tar`

### file list

```diff
@@ -1,15 +1,40 @@
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-19 03:02:36.000000 vango-1.1.1/
--rw-r--r--   0 jan        (501) staff       (20)      280 2023-07-19 03:02:36.000000 vango-1.1.1/PKG-INFO
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-19 03:02:36.000000 vango-1.1.1/vango.egg-info/
--rw-r--r--   0 jan        (501) staff       (20)      280 2023-07-19 03:02:36.000000 vango-1.1.1/vango.egg-info/PKG-INFO
--rw-r--r--   0 jan        (501) staff       (20)      198 2023-07-19 03:02:36.000000 vango-1.1.1/vango.egg-info/SOURCES.txt
--rw-r--r--   0 jan        (501) staff       (20)       11 2023-07-19 03:02:36.000000 vango-1.1.1/vango.egg-info/top_level.txt
--rw-r--r--   0 jan        (501) staff       (20)        1 2023-07-19 03:02:36.000000 vango-1.1.1/vango.egg-info/dependency_links.txt
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-19 03:02:36.000000 vango-1.1.1/vango/
--rw-r--r--   0 jan        (501) staff       (20)     2337 2023-07-19 03:02:28.000000 vango-1.1.1/vango/openapi.py
--rw-r--r--   0 jan        (501) staff       (20)       22 2023-07-14 07:25:26.000000 vango-1.1.1/vango/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)      523 2023-07-19 03:02:28.000000 vango-1.1.1/setup.py
--rw-r--r--   0 jan        (501) staff       (20)       59 2023-07-19 03:02:36.000000 vango-1.1.1/setup.cfg
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-19 03:02:36.000000 vango-1.1.1/VGPY/
--rw-r--r--   0 jan        (501) staff       (20)     1848 2023-07-13 12:55:09.000000 vango-1.1.1/VGPY/vango_openapi.py
--rw-r--r--   0 jan        (501) staff       (20)       28 2023-07-14 07:12:13.000000 vango-1.1.1/VGPY/__init__.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-21 10:36:08.000000 vango-1.1.5/
+-rw-r--r--   0 jan        (501) staff       (20)      280 2023-07-21 10:36:08.000000 vango-1.1.5/PKG-INFO
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-21 10:36:08.000000 vango-1.1.5/VGPY.egg-info/
+-rw-r--r--   0 jan        (501) staff       (20)      268 2023-07-14 07:13:48.000000 vango-1.1.5/VGPY.egg-info/PKG-INFO
+-rw-r--r--   0 jan        (501) staff       (20)      159 2023-07-14 07:13:48.000000 vango-1.1.5/VGPY.egg-info/SOURCES.txt
+-rw-r--r--   0 jan        (501) staff       (20)        5 2023-07-14 07:13:48.000000 vango-1.1.5/VGPY.egg-info/top_level.txt
+-rw-r--r--   0 jan        (501) staff       (20)        1 2023-07-14 07:13:48.000000 vango-1.1.5/VGPY.egg-info/dependency_links.txt
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-21 10:36:08.000000 vango-1.1.5/dist/
+-rw-r--r--   0 jan        (501) staff       (20)     1784 2023-07-14 07:12:23.000000 vango-1.1.5/dist/VGPY-1.0.0.tar.gz
+-rw-r--r--   0 jan        (501) staff       (20)     1932 2023-07-14 10:17:25.000000 vango-1.1.5/dist/vango-1.0.3.tar.gz
+-rw-r--r--   0 jan        (501) staff       (20)    21371 2023-07-19 07:59:12.000000 vango-1.1.5/dist/vango-1.1.3.tar.gz
+-rw-r--r--   0 jan        (501) staff       (20)     2045 2023-07-19 03:02:36.000000 vango-1.1.5/dist/vango-1.1.1.tar.gz
+-rw-r--r--   0 jan        (501) staff       (20)    53722 2023-07-19 08:05:51.000000 vango-1.1.5/dist/vango-1.1.4.tar.gz
+-rw-r--r--   0 jan        (501) staff       (20)     1787 2023-07-14 07:13:48.000000 vango-1.1.5/dist/VGPY-1.0.1.tar.gz
+-rw-r--r--   0 jan        (501) staff       (20)     2123 2023-07-19 07:15:24.000000 vango-1.1.5/dist/vango-1.1.2.tar.gz
+-rw-r--r--   0 jan        (501) staff       (20)     2199 2023-07-14 07:25:31.000000 vango-1.1.5/dist/vango-1.0.2.tar.gz
+-rw-r--r--   0 jan        (501) staff       (20)     1943 2023-07-18 01:43:44.000000 vango-1.1.5/dist/vango-1.1.0.tar.gz
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-21 10:36:08.000000 vango-1.1.5/vango.egg-info/
+-rw-r--r--   0 jan        (501) staff       (20)      280 2023-07-21 10:36:08.000000 vango-1.1.5/vango.egg-info/PKG-INFO
+-rw-r--r--   0 jan        (501) staff       (20)      677 2023-07-21 10:36:08.000000 vango-1.1.5/vango.egg-info/SOURCES.txt
+-rw-r--r--   0 jan        (501) staff       (20)       11 2023-07-21 10:36:08.000000 vango-1.1.5/vango.egg-info/top_level.txt
+-rw-r--r--   0 jan        (501) staff       (20)        1 2023-07-21 10:36:08.000000 vango-1.1.5/vango.egg-info/dependency_links.txt
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-21 10:36:08.000000 vango-1.1.5/vango/
+-rw-r--r--   0 jan        (501) staff       (20)       16 2023-07-19 07:03:50.000000 vango-1.1.5/vango/sign.txt
+-rw-r--r--   0 jan        (501) staff       (20)     2790 2023-07-21 10:35:08.000000 vango-1.1.5/vango/openapi.py
+-rw-r--r--   0 jan        (501) staff       (20)       22 2023-07-14 07:25:26.000000 vango-1.1.5/vango/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)       16 2023-07-19 07:58:38.000000 vango-1.1.5/MANIFEST.in
+-rw-r--r--   0 jan        (501) staff       (20)      523 2023-07-21 10:35:08.000000 vango-1.1.5/setup.py
+-rw-r--r--   0 jan        (501) staff       (20)       59 2023-07-21 10:36:08.000000 vango-1.1.5/setup.cfg
+-rw-r--r--   0 jan        (501) staff       (20)       74 2023-07-14 03:50:32.000000 vango-1.1.5/.pypirc
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-21 10:36:08.000000 vango-1.1.5/VGPY/
+-rw-r--r--   0 jan        (501) staff       (20)     1848 2023-07-13 12:55:09.000000 vango-1.1.5/VGPY/vango_openapi.py
+-rw-r--r--   0 jan        (501) staff       (20)       15 2023-07-13 11:49:35.000000 vango-1.1.5/VGPY/user.txt
+-rw-r--r--   0 jan        (501) staff       (20)       28 2023-07-14 07:12:13.000000 vango-1.1.5/VGPY/__init__.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-21 10:36:08.000000 vango-1.1.5/.idea/
+-rw-r--r--   0 jan        (501) staff       (20)      187 2023-07-14 03:17:15.000000 vango-1.1.5/.idea/jsLibraryMappings.xml
+-rw-r--r--   0 jan        (501) staff       (20)    35392 2023-07-21 10:35:32.000000 vango-1.1.5/.idea/workspace.xml
+-rw-r--r--   0 jan        (501) staff       (20)      276 2023-07-14 03:17:09.000000 vango-1.1.5/.idea/modules.xml
+-rw-r--r--   0 jan        (501) staff       (20)     1540 2023-07-14 03:21:31.000000 vango-1.1.5/.idea/misc.xml
+-rw-r--r--   0 jan        (501) staff       (20)      455 2023-07-14 03:17:24.000000 vango-1.1.5/.idea/vangoOpenapi.iml
```

### Comparing `vango-1.1.1/vango/openapi.py` & `vango-1.1.5/VGPY/vango_openapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,78 +1,66 @@
 import os
 import time
 import calendar
 import hashlib
 import json
 import requests
 
-# 获取任务的详细信息
-# name 任务中文名 必填
-# code 资产编号 必填
-# options 额外参数 非必填
-def get_task_detail(name, code, options):
-    params = {"code": code, "name": name, "options": options}
+def get_task_detail(name, code):
+    params = {"code": code, "name": name}
 
-    sign, userName, timestamp = _get_sign()
+    sign, userName, timestamp = get_sign()
     headers = {"VG-Request-User": userName, "VG-Request-Sign": sign,
                "VG-Request-Time": str(timestamp)}
     url = 'http://dev.vango_tapd_1166744_openapi.data-ad.37ops.com/openapi/task/detail'
 
     response = requests.get(url=url, params=params, headers=headers)
     if response.status_code == 200:
         return json.loads(response.text)
-    return response.json()
+    return None;
 
-# 上传文件
-# task_id 任务ID 必填
-# file_path 本地文件路径 必填
-# options 额外参数 非必填
-def upload_task_file(task_id, file_path, options):
-    data = {"task_id": task_id, "options": options}
 
-    try:
-        with open(file_path, "rb") as upload_file:
-            files = {"file": upload_file}
+def upload_task_file(task_id, file_path):
+    data = {"task_id": task_id}
 
-            sign, userName, timestamp = _get_sign()
-            headers = {"VG-Request-User": userName, "VG-Request-Sign": sign,
-                       "VG-Request-Time": str(timestamp), "VG-Request-App": "openapi"}
-            url = 'http://internal.vango_openapi.data-ad.37ops.com/openapi/task/file_upload'
+    with open(file_path, "rb") as upload_file:
+        files = {"file": upload_file}
 
-            response = requests.post(url=url, files=files, data=data, headers=headers)
-            if response.status_code == 200:
-                return json.loads(response.text)
-            return response.json()
+        sign, userName, timestamp = get_sign()
+        headers = {"VG-Request-User": userName, "VG-Request-Sign": sign,
+                   "VG-Request-Time": str(timestamp)}
+        url = 'http://10.16.23.3:8000/openapi/task/file_upload'
 
-    except Exception as e:
-            return '文件上传错误：{e}'
+        response = requests.post(url=url, files=files, data=data, headers=headers)
+        if response.status_code == 200:
+            return json.loads(response.text)
+        return None;
 
 
-
-def _get_sign():
-    user = _get_user_info()
+def get_sign():
+    user = get_user_info()
     userName = ''
     password = ''
     if user[0]:
         userName = user[0]
     if user[1]:
         password = user[1]
     timestamp = calendar.timegm(time.gmtime())
 
     md5 = hashlib.md5()
     md5.update(userName.encode('utf-8'))
     md5.update(password.encode('utf-8'))
     md5.update(str(timestamp).encode('utf-8'))
     sign = md5.hexdigest().upper()
 
-    return sign, userName, timestamp
+    return sign, userName, timestamp;
 
 
-def _get_user_info():
-    userFile = './user.txt'
+def get_user_info():
+    userFile = './user.txt';
     user = []
     if os.path.exists(userFile):
         with open(userFile, 'r') as f:
             userInfo = f.read()
             f.close()
         user = userInfo.split(' ')
-    return user
+    return user;
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `vango-1.1.1/setup.py` & `vango-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name='vango',
-    version='1.1.1',
+    version='1.1.5',
     description='van go open api',
     author='JanVee',
     author_email='814107539@qq.com',
     packages=find_packages(),
     install_requires=[],
     keywords = ("vango", "VGPY"),
     long_description = "An feature extraction algorithm, van_go open api",
```

### Comparing `vango-1.1.1/VGPY/vango_openapi.py` & `vango-1.1.5/vango/openapi.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,94 @@
 import os
 import time
 import calendar
 import hashlib
 import json
 import requests
 
-def get_task_detail(name, code):
-    params = {"code": code, "name": name}
+# 获取任务的详细信息
+# name 任务中文名 必填
+# code 资产编号 必填
+# options 额外参数 非必填
+def get_task_detail(name, code, options):
+    params = {"code": code, "name": name, "options": options}
 
-    sign, userName, timestamp = get_sign()
+    sign, userName, timestamp, appSign = _get_sign()
     headers = {"VG-Request-User": userName, "VG-Request-Sign": sign,
                "VG-Request-Time": str(timestamp)}
-    url = 'http://dev.vango_tapd_1166744_openapi.data-ad.37ops.com/openapi/task/detail'
+    url = 'http://mvango.37wan.com/openapi/task/detail'
 
     response = requests.get(url=url, params=params, headers=headers)
     if response.status_code == 200:
         return json.loads(response.text)
-    return None;
+    return response.json()
 
+# 上传文件
+# task_id 任务ID 必填
+# file_path 本地文件路径 必填
+# options 额外参数 非必填
+def upload_task_file(task_id, file_path, options):
+    data = {"task_id": task_id, "options": options}
 
-def upload_task_file(task_id, file_path):
-    data = {"task_id": task_id}
+    try:
+        with open(file_path, "rb") as upload_file:
+            files = {"file": upload_file}
 
-    with open(file_path, "rb") as upload_file:
-        files = {"file": upload_file}
+            sign, userName, timestamp, appSign = _get_sign()
+            headers = {"VG-Request-User": userName, "VG-Request-Sign": sign,
+                       "VG-Request-Time": str(timestamp), "VG-Request-App": "openapi",
+                       "VG-Request-AppSign": appSign}
+            url = 'http://internal.vango-openapi.data-ad.37ops.com/openapi/task/file_upload'
 
-        sign, userName, timestamp = get_sign()
-        headers = {"VG-Request-User": userName, "VG-Request-Sign": sign,
-                   "VG-Request-Time": str(timestamp)}
-        url = 'http://10.16.23.3:8000/openapi/task/file_upload'
+            response = requests.post(url=url, files=files, data=data, headers=headers)
+            if response.status_code == 200:
+                return json.loads(response.text)
+            return response.json()
 
-        response = requests.post(url=url, files=files, data=data, headers=headers)
-        if response.status_code == 200:
-            return json.loads(response.text)
-        return None;
+    except Exception as e:
+            return '文件上传错误：{e}'
 
 
-def get_sign():
-    user = get_user_info()
+
+def _get_sign():
+    user = _get_user_info()
     userName = ''
     password = ''
     if user[0]:
         userName = user[0]
     if user[1]:
         password = user[1]
     timestamp = calendar.timegm(time.gmtime())
 
     md5 = hashlib.md5()
     md5.update(userName.encode('utf-8'))
     md5.update(password.encode('utf-8'))
     md5.update(str(timestamp).encode('utf-8'))
     sign = md5.hexdigest().upper()
 
-    return sign, userName, timestamp;
+    appSignStr = _get_app_sign()
+    md5 = hashlib.md5()
+    md5.update(appSignStr.encode('utf-8'))
+    md5.update(str(timestamp).encode('utf-8'))
+    appSign = md5.hexdigest().upper()
+
+    return sign, userName, timestamp, appSign
 
 
-def get_user_info():
-    userFile = './user.txt';
+def _get_user_info():
+    userFile = './user.txt'
     user = []
     if os.path.exists(userFile):
         with open(userFile, 'r') as f:
             userInfo = f.read()
             f.close()
         user = userInfo.split(' ')
-    return user;
+    return user
+
+def _get_app_sign():
+    signFile = './sign.txt'
+    sign = 'S*zVvcWOU*2p7$H%'
+    if os.path.exists(signFile):
+        with open(signFile, 'r') as f:
+            sign = f.read()
+            f.close()
+    return sign
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

