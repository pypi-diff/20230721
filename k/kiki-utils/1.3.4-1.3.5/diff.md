# Comparing `tmp/kiki_utils-1.3.4.tar.gz` & `tmp/kiki_utils-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiki_utils-1.3.4.tar", last modified: Thu Jul 20 07:56:10 2023, max compression
+gzip compressed data, was "kiki_utils-1.3.5.tar", last modified: Fri Jul 21 11:12:17 2023, max compression
```

## Comparing `kiki_utils-1.3.4.tar` & `kiki_utils-1.3.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-07-20 07:56:10.092999 kiki_utils-1.3.4/
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1066 2023-07-19 07:09:04.000000 kiki_utils-1.3.4/LICENSE.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      255 2023-07-20 07:56:10.092999 kiki_utils-1.3.4/PKG-INFO
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)       63 2023-07-20 05:46:22.000000 kiki_utils-1.3.4/README.md
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-07-20 07:56:10.088999 kiki_utils-1.3.4/kiki_utils.egg-info/
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      255 2023-07-20 07:56:10.000000 kiki_utils-1.3.4/kiki_utils.egg-info/PKG-INFO
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      547 2023-07-20 07:56:10.000000 kiki_utils-1.3.4/kiki_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-07-20 07:56:10.000000 kiki_utils-1.3.4/kiki_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      151 2023-07-20 07:56:10.000000 kiki_utils-1.3.4/kiki_utils.egg-info/requires.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       10 2023-07-20 07:56:10.000000 kiki_utils-1.3.4/kiki_utils.egg-info/top_level.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-07-20 07:56:10.000000 kiki_utils-1.3.4/kiki_utils.egg-info/zip-safe
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-07-20 07:56:10.092999 kiki_utils-1.3.4/kikiutils/
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)       13 2022-11-28 02:36:38.000000 kiki_utils-1.3.4/kikiutils/__init__.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1936 2023-07-20 05:43:24.000000 kiki_utils-1.3.4/kikiutils/aes.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1863 2023-07-20 07:26:13.000000 kiki_utils-1.3.4/kikiutils/aiofile.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1950 2023-07-20 06:57:33.000000 kiki_utils-1.3.4/kikiutils/check.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      188 2022-11-28 02:36:38.000000 kiki_utils-1.3.4/kikiutils/cookie.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     4130 2023-07-20 06:38:45.000000 kiki_utils-1.3.4/kikiutils/decorators.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     2524 2023-07-20 07:48:43.000000 kiki_utils-1.3.4/kikiutils/file.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      795 2023-07-20 06:43:54.000000 kiki_utils-1.3.4/kikiutils/hash.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      152 2022-11-28 02:36:38.000000 kiki_utils-1.3.4/kikiutils/import_utils.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      979 2023-02-04 08:44:34.000000 kiki_utils-1.3.4/kikiutils/json.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      313 2022-11-28 02:36:38.000000 kiki_utils-1.3.4/kikiutils/log.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      528 2023-07-20 05:28:16.000000 kiki_utils-1.3.4/kikiutils/network.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1314 2023-07-20 07:02:43.000000 kiki_utils-1.3.4/kikiutils/string.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1599 2023-07-20 05:39:03.000000 kiki_utils-1.3.4/kikiutils/time.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      198 2023-07-20 05:42:54.000000 kiki_utils-1.3.4/kikiutils/typehint.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      592 2023-02-04 08:36:34.000000 kiki_utils-1.3.4/kikiutils/uuid.py
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       38 2023-07-20 07:56:10.092999 kiki_utils-1.3.4/setup.cfg
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      668 2023-07-20 07:55:57.000000 kiki_utils-1.3.4/setup.py
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-07-21 11:12:17.250683 kiki_utils-1.3.5/
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1066 2023-07-19 07:09:04.000000 kiki_utils-1.3.5/LICENSE.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      255 2023-07-21 11:12:17.250683 kiki_utils-1.3.5/PKG-INFO
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)       63 2023-07-20 05:46:22.000000 kiki_utils-1.3.5/README.md
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-07-21 11:12:17.250683 kiki_utils-1.3.5/kiki_utils.egg-info/
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      255 2023-07-21 11:12:17.000000 kiki_utils-1.3.5/kiki_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      547 2023-07-21 11:12:17.000000 kiki_utils-1.3.5/kiki_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-07-21 11:12:17.000000 kiki_utils-1.3.5/kiki_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      151 2023-07-21 11:12:17.000000 kiki_utils-1.3.5/kiki_utils.egg-info/requires.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       10 2023-07-21 11:12:17.000000 kiki_utils-1.3.5/kiki_utils.egg-info/top_level.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-07-21 11:12:17.000000 kiki_utils-1.3.5/kiki_utils.egg-info/zip-safe
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-07-21 11:12:17.250683 kiki_utils-1.3.5/kikiutils/
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)       13 2022-11-28 02:36:38.000000 kiki_utils-1.3.5/kikiutils/__init__.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1936 2023-07-20 05:43:24.000000 kiki_utils-1.3.5/kikiutils/aes.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1863 2023-07-20 07:26:13.000000 kiki_utils-1.3.5/kikiutils/aiofile.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1913 2023-07-21 11:10:53.000000 kiki_utils-1.3.5/kikiutils/check.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      188 2022-11-28 02:36:38.000000 kiki_utils-1.3.5/kikiutils/cookie.py
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     4130 2023-07-20 10:58:00.000000 kiki_utils-1.3.5/kikiutils/decorators.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     2524 2023-07-20 07:48:43.000000 kiki_utils-1.3.5/kikiutils/file.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      795 2023-07-20 06:43:54.000000 kiki_utils-1.3.5/kikiutils/hash.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      152 2022-11-28 02:36:38.000000 kiki_utils-1.3.5/kikiutils/import_utils.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      979 2023-02-04 08:44:34.000000 kiki_utils-1.3.5/kikiutils/json.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      313 2022-11-28 02:36:38.000000 kiki_utils-1.3.5/kikiutils/log.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      528 2023-07-20 05:28:16.000000 kiki_utils-1.3.5/kikiutils/network.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1314 2023-07-20 07:02:43.000000 kiki_utils-1.3.5/kikiutils/string.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1599 2023-07-20 05:39:03.000000 kiki_utils-1.3.5/kikiutils/time.py
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      198 2023-07-20 10:58:00.000000 kiki_utils-1.3.5/kikiutils/typehint.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      592 2023-02-04 08:36:34.000000 kiki_utils-1.3.5/kikiutils/uuid.py
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       38 2023-07-21 11:12:17.250683 kiki_utils-1.3.5/setup.cfg
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      668 2023-07-21 11:11:02.000000 kiki_utils-1.3.5/setup.py
```

### Comparing `kiki_utils-1.3.4/LICENSE.txt` & `kiki_utils-1.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kiki_utils-1.3.4/kiki_utils.egg-info/SOURCES.txt` & `kiki_utils-1.3.5/kiki_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiki_utils-1.3.4/kikiutils/aes.py` & `kiki_utils-1.3.5/kikiutils/aes.py`

 * *Files identical despite different names*

### Comparing `kiki_utils-1.3.4/kikiutils/aiofile.py` & `kiki_utils-1.3.5/kikiutils/aiofile.py`

 * *Files identical despite different names*

### Comparing `kiki_utils-1.3.4/kikiutils/check.py` & `kiki_utils-1.3.5/kikiutils/check.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 import re
 
 from functools import wraps
 from typing import Callable
-from unittest.case import _ClassInfo
 
 from .typehint import P, PathOrStr, T
 
 
 ALLOWED_EMAILS = [
     'gmail.com',
     'yahoo.com',
```

### Comparing `kiki_utils-1.3.4/kikiutils/decorators.py` & `kiki_utils-1.3.5/kikiutils/decorators.py`

 * *Files identical despite different names*

### Comparing `kiki_utils-1.3.4/kikiutils/file.py` & `kiki_utils-1.3.5/kikiutils/file.py`

 * *Files identical despite different names*

### Comparing `kiki_utils-1.3.4/kikiutils/hash.py` & `kiki_utils-1.3.5/kikiutils/hash.py`

 * *Files identical despite different names*

### Comparing `kiki_utils-1.3.4/kikiutils/json.py` & `kiki_utils-1.3.5/kikiutils/json.py`

 * *Files identical despite different names*

### Comparing `kiki_utils-1.3.4/kikiutils/network.py` & `kiki_utils-1.3.5/kikiutils/network.py`

 * *Files identical despite different names*

### Comparing `kiki_utils-1.3.4/kikiutils/string.py` & `kiki_utils-1.3.5/kikiutils/string.py`

 * *Files identical despite different names*

### Comparing `kiki_utils-1.3.4/kikiutils/time.py` & `kiki_utils-1.3.5/kikiutils/time.py`

 * *Files identical despite different names*

### Comparing `kiki_utils-1.3.4/kikiutils/uuid.py` & `kiki_utils-1.3.5/kikiutils/uuid.py`

 * *Files identical despite different names*

### Comparing `kiki_utils-1.3.4/setup.py` & `kiki_utils-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     name='kiki_utils',
     classifiers=[
         'License :: Freely Distributable'
     ],
     packages=find_packages(),
     include_package_data=True,
     zip_safe=True,
-    version='1.3.4',
+    version='1.3.5',
     description='Utils decorators and functions.',
     author='kiki-kanri',
     author_email='a470666@gmail.com',
     keywords=['Utils'],
     install_requires=[
         'aiofiles',
         'aioshutil',
```

