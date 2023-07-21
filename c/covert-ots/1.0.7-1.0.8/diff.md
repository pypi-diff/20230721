# Comparing `tmp/covert-ots-1.0.7.tar.gz` & `tmp/covert-ots-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covert-ots-1.0.7.tar", last modified: Fri Jul 21 10:48:54 2023, max compression
+gzip compressed data, was "covert-ots-1.0.8.tar", last modified: Fri Jul 21 10:50:46 2023, max compression
```

## Comparing `covert-ots-1.0.7.tar` & `covert-ots-1.0.8.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxr-x   0 om        (1001) om        (1001)        0 2023-07-21 10:48:54.457238 covert-ots-1.0.7/
--rw-rw-r--   0 om        (1001) om        (1001)     1154 2023-07-21 10:48:54.457238 covert-ots-1.0.7/PKG-INFO
--rw-rw-r--   0 om        (1001) om        (1001)       60 2023-07-17 19:18:34.000000 covert-ots-1.0.7/constants.py
--rw-rw-r--   0 om        (1001) om        (1001)     3554 2023-07-18 05:15:15.000000 covert-ots-1.0.7/covert.py
-drwxrwxr-x   0 om        (1001) om        (1001)        0 2023-07-21 10:48:54.457238 covert-ots-1.0.7/covert_ots.egg-info/
--rw-rw-r--   0 om        (1001) om        (1001)     1154 2023-07-21 10:48:54.000000 covert-ots-1.0.7/covert_ots.egg-info/PKG-INFO
--rw-rw-r--   0 om        (1001) om        (1001)      241 2023-07-21 10:48:54.000000 covert-ots-1.0.7/covert_ots.egg-info/SOURCES.txt
--rw-rw-r--   0 om        (1001) om        (1001)        1 2023-07-21 10:48:54.000000 covert-ots-1.0.7/covert_ots.egg-info/dependency_links.txt
--rw-rw-r--   0 om        (1001) om        (1001)       39 2023-07-21 10:48:54.000000 covert-ots-1.0.7/covert_ots.egg-info/entry_points.txt
--rw-rw-r--   0 om        (1001) om        (1001)       33 2023-07-21 10:48:54.000000 covert-ots-1.0.7/covert_ots.egg-info/requires.txt
--rw-rw-r--   0 om        (1001) om        (1001)       17 2023-07-21 10:48:54.000000 covert-ots-1.0.7/covert_ots.egg-info/top_level.txt
--rw-rw-r--   0 om        (1001) om        (1001)       38 2023-07-21 10:48:54.457238 covert-ots-1.0.7/setup.cfg
--rw-rw-r--   0 om        (1001) om        (1001)      857 2023-07-21 10:48:16.000000 covert-ots-1.0.7/setup.py
+drwxrwxr-x   0 om        (1001) om        (1001)        0 2023-07-21 10:50:46.761719 covert-ots-1.0.8/
+-rw-rw-r--   0 om        (1001) om        (1001)     1154 2023-07-21 10:50:46.761719 covert-ots-1.0.8/PKG-INFO
+-rw-rw-r--   0 om        (1001) om        (1001)     3574 2023-07-21 10:50:04.000000 covert-ots-1.0.8/covert.py
+drwxrwxr-x   0 om        (1001) om        (1001)        0 2023-07-21 10:50:46.761719 covert-ots-1.0.8/covert_ots.egg-info/
+-rw-rw-r--   0 om        (1001) om        (1001)     1154 2023-07-21 10:50:46.000000 covert-ots-1.0.8/covert_ots.egg-info/PKG-INFO
+-rw-rw-r--   0 om        (1001) om        (1001)      226 2023-07-21 10:50:46.000000 covert-ots-1.0.8/covert_ots.egg-info/SOURCES.txt
+-rw-rw-r--   0 om        (1001) om        (1001)        1 2023-07-21 10:50:46.000000 covert-ots-1.0.8/covert_ots.egg-info/dependency_links.txt
+-rw-rw-r--   0 om        (1001) om        (1001)       39 2023-07-21 10:50:46.000000 covert-ots-1.0.8/covert_ots.egg-info/entry_points.txt
+-rw-rw-r--   0 om        (1001) om        (1001)       33 2023-07-21 10:50:46.000000 covert-ots-1.0.8/covert_ots.egg-info/requires.txt
+-rw-rw-r--   0 om        (1001) om        (1001)        7 2023-07-21 10:50:46.000000 covert-ots-1.0.8/covert_ots.egg-info/top_level.txt
+-rw-rw-r--   0 om        (1001) om        (1001)       38 2023-07-21 10:50:46.761719 covert-ots-1.0.8/setup.cfg
+-rw-rw-r--   0 om        (1001) om        (1001)      844 2023-07-21 10:50:43.000000 covert-ots-1.0.8/setup.py
```

### Comparing `covert-ots-1.0.7/PKG-INFO` & `covert-ots-1.0.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covert-ots
-Version: 1.0.7
+Version: 1.0.8
 Summary: A secure way to communicate your secrets
 Home-page: UNKNOWN
 Author: Om Gupta
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `covert-ots-1.0.7/covert.py` & `covert-ots-1.0.8/covert.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import typer
 from rich import print as rprint
 import os
 import sys
 import requests
 from dotenv import load_dotenv
 import json
-from constants import COVERT_SERVER_URL
 import base64
 from Crypto.Cipher import AES
 from Crypto.Hash import SHA256
 from Crypto import Random
 import inquirer 
 
 app = typer.Typer()
 load_dotenv()
 sys.path.append(os.path.realpath("."))
-
+COVERT_SERVER_URL = 'https://covert-server.as.r.appspot.com'
 
 def encrypt(key: str, source: str, encode=True):
     try:
         key = key.encode("UTF-8")
         source = source.encode("UTF-8")
         key = SHA256.new(key).digest()
         IV = Random.new().read(AES.block_size)
```

### Comparing `covert-ots-1.0.7/covert_ots.egg-info/PKG-INFO` & `covert-ots-1.0.8/covert_ots.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covert-ots
-Version: 1.0.7
+Version: 1.0.8
 Summary: A secure way to communicate your secrets
 Home-page: UNKNOWN
 Author: Om Gupta
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `covert-ots-1.0.7/setup.py` & `covert-ots-1.0.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import setuptools
 
 with open("../README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='covert-ots',
-   version='1.0.7',
+   version='1.0.8',
     author="Om Gupta",                     
     description="A secure way to communicate your secrets",
     long_description=long_description,      
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(), 
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],                         
     python_requires='>=3.6',   
-    py_modules=["covert", "constants"],
+    py_modules=["covert"],
     package_dir={'':'.'},
     install_requires=[
       'typer',
       'rich',
       'inquirer',
       'pycryptodome'
    ],
```

