# Comparing `tmp/kr8_protobuf-1.0.8.tar.gz` & `tmp/kr8_protobuf-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kr8_protobuf-1.0.8.tar", last modified: Mon Jul 17 18:04:19 2023, max compression
+gzip compressed data, was "dist/kr8_protobuf-1.0.9.tar", last modified: Thu Jul 20 20:58:44 2023, max compression
```

## Comparing `kr8_protobuf-1.0.8.tar` & `kr8_protobuf-1.0.9.tar`

### file list

```diff
@@ -1,12 +1,9 @@
-drwxr-xr-x   0 raeth      (501) staff       (20)        0 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/
--rw-r--r--   0 raeth      (501) staff       (20)      739 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/PKG-INFO
-drwxr-xr-x   0 raeth      (501) staff       (20)        0 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/kr8_protobuf/
--rw-r--r--   0 raeth      (501) staff       (20)     1643 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/kr8_protobuf/analyzer_pb2.py
--rw-r--r--   0 raeth      (501) staff       (20)     3916 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/kr8_protobuf/analyzer_pb2_grpc.py
--rw-r--r--   0 raeth      (501) staff       (20)     2142 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/kr8_protobuf/authentication_pb2.py
--rw-r--r--   0 raeth      (501) staff       (20)     5733 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/kr8_protobuf/authentication_pb2_grpc.py
--rw-r--r--   0 raeth      (501) staff       (20)     1170 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/kr8_protobuf/common_pb2.py
--rw-r--r--   0 raeth      (501) staff       (20)      159 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/kr8_protobuf/common_pb2_grpc.py
--rw-r--r--   0 raeth      (501) staff       (20)     1864 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/kr8_protobuf/user_pb2.py
--rw-r--r--   0 raeth      (501) staff       (20)     2486 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/kr8_protobuf/user_pb2_grpc.py
--rw-r--r--   0 raeth      (501) staff       (20)     1664 2023-07-17 18:04:19.000000 kr8_protobuf-1.0.8/setup.py
+drwxr-xr-x   0 raeth      (501) staff       (20)        0 2023-07-20 20:58:44.000000 kr8_protobuf-1.0.9/
+-rw-r--r--   0 raeth      (501) staff       (20)      739 2023-07-20 20:58:44.000000 kr8_protobuf-1.0.9/PKG-INFO
+drwxr-xr-x   0 raeth      (501) staff       (20)        0 2023-07-20 20:58:44.000000 kr8_protobuf-1.0.9/kr8_protobuf/
+drwxr-xr-x   0 raeth      (501) staff       (20)        0 2023-07-20 20:58:44.000000 kr8_protobuf-1.0.9/kr8_protobuf/kr8_protobuf/
+-rw-r--r--   0 raeth      (501) staff       (20)      945 2023-07-20 20:58:44.000000 kr8_protobuf-1.0.9/kr8_protobuf/kr8_protobuf/analyzer_pb2.pyi
+-rw-r--r--   0 raeth      (501) staff       (20)     1451 2023-07-20 20:58:44.000000 kr8_protobuf-1.0.9/kr8_protobuf/kr8_protobuf/authentication_pb2.pyi
+-rw-r--r--   0 raeth      (501) staff       (20)      637 2023-07-20 20:58:44.000000 kr8_protobuf-1.0.9/kr8_protobuf/kr8_protobuf/common_pb2.pyi
+-rw-r--r--   0 raeth      (501) staff       (20)     1486 2023-07-20 20:58:44.000000 kr8_protobuf-1.0.9/kr8_protobuf/kr8_protobuf/user_pb2.pyi
+-rw-r--r--   0 raeth      (501) staff       (20)     1730 2023-07-20 20:58:44.000000 kr8_protobuf-1.0.9/setup.py
```

### Comparing `kr8_protobuf-1.0.8/PKG-INFO` & `kr8_protobuf-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kr8_protobuf
-Version: 1.0.8
+Version: 1.0.9
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://github.com/user/reponame
 Author: YOUR NAME
 Author-email: your.email@domain.com
 License: MIT
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Description: UNKNOWN
```

### Comparing `kr8_protobuf-1.0.8/setup.py` & `kr8_protobuf-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'kr8_protobuf',         # How you named your package folder (MyLib)
   packages = ['kr8_protobuf'],   # Chose the same as "name"
-  version = '1.0.8',      # Start with a small number and increase it with every change you make
+  version = '1.0.9',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'TYPE YOUR DESCRIPTION HERE',   # Give a short description about your library
   author = 'YOUR NAME',                   # Type in your name
   author_email = 'your.email@domain.com',      # Type in your E-Mail
   url = 'https://github.com/user/reponame',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
@@ -21,8 +21,9 @@
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
     'Programming Language :: Python :: 3.4',
     'Programming Language :: Python :: 3.5',
     'Programming Language :: Python :: 3.6',
   ],
+  package_data={"kr8_protobuf":["py.typed", "*.pyi", "**/*.pyi"]}
 )
```

