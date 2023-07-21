# Comparing `tmp/jsepp-0.1.2.tar.gz` & `tmp/jsepp-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsepp-0.1.2.tar", last modified: Sat May  6 04:55:07 2023, max compression
+gzip compressed data, was "jsepp-0.1.3.tar", last modified: Fri Jul 21 02:42:50 2023, max compression
```

## Comparing `jsepp-0.1.2.tar` & `jsepp-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 04:55:07.973894 jsepp-0.1.2/
--rw-rw-rw-   0        0        0      610 2023-05-06 04:55:07.973894 jsepp-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-04-12 02:46:41.000000 jsepp-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 04:55:07.968909 jsepp-0.1.2/jsepp/
--rw-rw-rw-   0        0        0       14 2023-04-12 06:01:14.000000 jsepp-0.1.2/jsepp/__init__.py
--rw-rw-rw-   0        0        0     3114 2023-05-06 04:46:06.000000 jsepp-0.1.2/jsepp/data.py
--rw-rw-rw-   0        0        0     2049 2023-04-17 07:54:59.000000 jsepp-0.1.2/jsepp/dbutils.py
--rw-rw-rw-   0        0        0      571 2023-05-06 04:45:51.000000 jsepp-0.1.2/jsepp/ml.py
-drwxrwxrwx   0        0        0        0 2023-05-06 04:55:07.972897 jsepp-0.1.2/jsepp.egg-info/
--rw-rw-rw-   0        0        0      610 2023-05-06 04:55:07.000000 jsepp-0.1.2/jsepp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-05-06 04:55:07.000000 jsepp-0.1.2/jsepp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 04:55:07.000000 jsepp-0.1.2/jsepp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-06 04:55:07.000000 jsepp-0.1.2/jsepp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-06 04:55:07.000000 jsepp-0.1.2/jsepp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 04:55:07.973894 jsepp-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      529 2023-05-06 04:53:47.000000 jsepp-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 02:42:50.890041 jsepp-0.1.3/
+-rw-rw-rw-   0        0        0      610 2023-07-21 02:42:50.889043 jsepp-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-04-12 02:46:41.000000 jsepp-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 02:42:50.886549 jsepp-0.1.3/jsepp/
+-rw-rw-rw-   0        0        0       14 2023-04-12 06:01:14.000000 jsepp-0.1.3/jsepp/__init__.py
+-rw-rw-rw-   0        0        0     3082 2023-05-06 06:46:53.000000 jsepp-0.1.3/jsepp/data.py
+-rw-rw-rw-   0        0        0     2473 2023-07-21 02:41:10.000000 jsepp-0.1.3/jsepp/dbutils.py
+-rw-rw-rw-   0        0        0      571 2023-05-06 04:45:51.000000 jsepp-0.1.3/jsepp/ml.py
+drwxrwxrwx   0        0        0        0 2023-07-21 02:42:50.889043 jsepp-0.1.3/jsepp.egg-info/
+-rw-rw-rw-   0        0        0      610 2023-07-21 02:42:50.000000 jsepp-0.1.3/jsepp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-07-21 02:42:50.000000 jsepp-0.1.3/jsepp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 02:42:50.000000 jsepp-0.1.3/jsepp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-07-21 02:42:50.000000 jsepp-0.1.3/jsepp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-21 02:42:50.000000 jsepp-0.1.3/jsepp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 02:42:50.890041 jsepp-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      529 2023-07-21 02:42:09.000000 jsepp-0.1.3/setup.py
```

### Comparing `jsepp-0.1.2/PKG-INFO` & `jsepp-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsepp
-Version: 0.1.2
+Version: 0.1.3
 Summary: a package for general environmental data processing
 Author: Hansen Zhao
 Author-email: zhaohs12@163.com
 
 ## JSEPP
 ### dbutils
 #### MySQLConn
```

### Comparing `jsepp-0.1.2/jsepp/data.py` & `jsepp-0.1.3/jsepp/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import datetime
 import pandas as pd
 import numpy as np
-import matplotlib.pyplot as plt
-from ml import autoreg_fill
+from .ml import autoreg_fill
 def tryfloat(x, nanflag:float = None, nanvalue=np.nan):
     if nanflag and np.abs(float(x) - nanflag) < 1E-8:
         return nanvalue
     try:
         return float(x)
     except:
         return nanvalue
```

### Comparing `jsepp-0.1.2/jsepp/dbutils.py` & `jsepp-0.1.3/jsepp/dbutils.py`

 * *Files 18% similar despite different names*

```diff
@@ -43,16 +43,21 @@
         self.conn.commit()
 
     def rollback(self):
         self.conn.rollback()
 
 
 class MongoConn(object):
-    def __init__(self, user:str, password:str, host:str, port:int, db:str):
-        self.conn = pymongo.MongoClient(f'mongodb://{urllib.parse.quote_plus(user)}:{urllib.parse.quote_plus(password)}@{host}:{port}')
+    def __init__(self, user:str, password:str, host:str, port:int, db:str, authMechanism:str='DEFAULT', authSource:str=None):
+        if authSource is None:
+            self.conn = pymongo.MongoClient('mongodb://{urllib.parse.quote_plus(user)}:{urllib.parse.quote_plus(password)}@{host}:{port}'
+                                            '/?authMechanism={authMechanism}')
+        else:
+            self.conn = pymongo.MongoClient(f'mongodb://{urllib.parse.quote_plus(user)}:{urllib.parse.quote_plus(password)}@{host}:{port}'
+                                            f'/?authMechanism={authMechanism}&authSource={authSource}')
         self.cursor = self.conn[db]
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.conn.close()
```

### Comparing `jsepp-0.1.2/jsepp/ml.py` & `jsepp-0.1.3/jsepp/ml.py`

 * *Files identical despite different names*

### Comparing `jsepp-0.1.2/jsepp.egg-info/PKG-INFO` & `jsepp-0.1.3/jsepp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsepp
-Version: 0.1.2
+Version: 0.1.3
 Summary: a package for general environmental data processing
 Author: Hansen Zhao
 Author-email: zhaohs12@163.com
 
 ## JSEPP
 ### dbutils
 #### MySQLConn
```

### Comparing `jsepp-0.1.2/setup.py` & `jsepp-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_des = f.read()
 
 setup(
     name='jsepp',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=[
         'pymysql',
         'pymongo',
         'numpy',
         'pandas',
         'openpyxl',
```

