# Comparing `tmp/mamon-utils-0.0.1.tar.gz` & `tmp/mamon_utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mamon-utils-0.0.1.tar", last modified: Tue Jul 18 14:57:35 2023, max compression
+gzip compressed data, was "mamon_utils-0.0.2.tar", max compression
```

## Comparing `mamon-utils-0.0.1.tar` & `mamon_utils-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,5 @@
-drwxrwxr-x   0 wc        (1000) wc        (1000)        0 2023-07-18 14:57:35.789228 mamon-utils-0.0.1/
--rw-rw-r--   0 wc        (1000) wc        (1000)      927 2023-07-18 14:57:35.789228 mamon-utils-0.0.1/PKG-INFO
--rw-rw-r--   0 wc        (1000) wc        (1000)      744 2023-07-18 14:57:13.000000 mamon-utils-0.0.1/README.md
-drwxrwxr-x   0 wc        (1000) wc        (1000)        0 2023-07-18 14:57:35.789228 mamon-utils-0.0.1/mamon_utils.egg-info/
--rw-rw-r--   0 wc        (1000) wc        (1000)      927 2023-07-18 14:57:35.000000 mamon-utils-0.0.1/mamon_utils.egg-info/PKG-INFO
--rw-rw-r--   0 wc        (1000) wc        (1000)      232 2023-07-18 14:57:35.000000 mamon-utils-0.0.1/mamon_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 wc        (1000) wc        (1000)        1 2023-07-18 14:57:35.000000 mamon-utils-0.0.1/mamon_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 wc        (1000) wc        (1000)       44 2023-07-18 14:57:35.000000 mamon-utils-0.0.1/mamon_utils.egg-info/requires.txt
--rw-rw-r--   0 wc        (1000) wc        (1000)       11 2023-07-18 14:57:35.000000 mamon-utils-0.0.1/mamon_utils.egg-info/top_level.txt
-drwxrwxr-x   0 wc        (1000) wc        (1000)        0 2023-07-18 14:57:35.789228 mamon-utils-0.0.1/mamonutils/
--rw-rw-r--   0 wc        (1000) wc        (1000)       66 2023-07-18 13:41:03.000000 mamon-utils-0.0.1/mamonutils/__init__.py
--rw-rw-r--   0 wc        (1000) wc        (1000)     1484 2023-07-18 13:39:52.000000 mamon-utils-0.0.1/mamonutils/db.py
--rw-rw-r--   0 wc        (1000) wc        (1000)       38 2023-07-18 14:57:35.789228 mamon-utils-0.0.1/setup.cfg
--rw-rw-r--   0 wc        (1000) wc        (1000)      736 2023-07-18 14:54:04.000000 mamon-utils-0.0.1/setup.py
+-rw-r--r--   0        0        0      736 2023-07-18 23:03:34.398485 mamon_utils-0.0.2/README_PYPI.md
+-rw-r--r--   0        0        0       66 2023-07-18 22:35:53.627917 mamon_utils-0.0.2/mamonutils/__init__.py
+-rw-r--r--   0        0        0     1415 2023-07-18 22:46:42.155559 mamon_utils-0.0.2/mamonutils/db.py
+-rw-r--r--   0        0        0      392 2023-07-21 19:02:08.220996 mamon_utils-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1232 1970-01-01 00:00:00.000000 mamon_utils-0.0.2/PKG-INFO
```

### Comparing `mamon-utils-0.0.1/PKG-INFO` & `mamon_utils-0.0.2/README_PYPI.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,10 @@
-Metadata-Version: 2.1
-Name: mamon-utils
-Version: 0.0.1
-Summary: Common tools and utilities
-Author: WessCoby
-Author-email: <wc@wesscoby.com>
-Description-Content-Type: text/markdown
-
-
 # Mamon Utilities
 
-A set of tools and utilities for Mamon11 Python Development
+A set of tools and utilities for Python Development
 
 ## Installation
 ```sh
 pip install mamon-utils
 ```
 
 ## Usage
@@ -41,8 +32,8 @@
 
 cursor.execute('SELECT * from clients')
 result = cursor.fetchall()
 print(result)
 
 # Disconnect
 db.disconnect()
-```
+```
```

### Comparing `mamon-utils-0.0.1/mamon_utils.egg-info/PKG-INFO` & `mamon_utils-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 Metadata-Version: 2.1
 Name: mamon-utils
-Version: 0.0.1
-Summary: Common tools and utilities
+Version: 0.0.2
+Summary: Common Mamon11 tools and utilities
 Author: WessCoby
-Author-email: <wc@wesscoby.com>
+Author-email: wc@wesscoby.com
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: psycopg2-binary (==2.9.5)
+Requires-Dist: python-dotenv (==1.0.0)
 Description-Content-Type: text/markdown
 
-
 # Mamon Utilities
 
-A set of tools and utilities for Mamon11 Python Development
+A set of tools and utilities for Python Development
 
 ## Installation
 ```sh
 pip install mamon-utils
 ```
 
 ## Usage
```

### Comparing `mamon-utils-0.0.1/mamonutils/db.py` & `mamon_utils-0.0.2/mamonutils/db.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 import os
 import psycopg2
 from psycopg2 import Error
 from typing import Optional
-from dotenv import load_dotenv
-
-# Load the .env file
-# load_dotenv()
 
 
 class Database:
     def __init__(self, dbname: str):
         self.dbname = dbname
         self.host = os.environ.get('DB_HOST')
         self.port = os.environ.get('DB_PORT')
```

