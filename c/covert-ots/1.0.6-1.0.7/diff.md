# Comparing `tmp/covert-ots-1.0.6.tar.gz` & `tmp/covert-ots-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covert-ots-1.0.6.tar", last modified: Fri Jul 21 10:46:14 2023, max compression
+gzip compressed data, was "covert-ots-1.0.7.tar", last modified: Fri Jul 21 10:48:54 2023, max compression
```

## Comparing `covert-ots-1.0.6.tar` & `covert-ots-1.0.7.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 om        (1001) om        (1001)        0 2023-07-21 10:46:14.435300 covert-ots-1.0.6/
--rw-rw-r--   0 om        (1001) om        (1001)     1154 2023-07-21 10:46:14.435300 covert-ots-1.0.6/PKG-INFO
--rw-rw-r--   0 om        (1001) om        (1001)     3554 2023-07-18 05:15:15.000000 covert-ots-1.0.6/covert.py
-drwxrwxr-x   0 om        (1001) om        (1001)        0 2023-07-21 10:46:14.435300 covert-ots-1.0.6/covert_ots.egg-info/
--rw-rw-r--   0 om        (1001) om        (1001)     1154 2023-07-21 10:46:14.000000 covert-ots-1.0.6/covert_ots.egg-info/PKG-INFO
--rw-rw-r--   0 om        (1001) om        (1001)      226 2023-07-21 10:46:14.000000 covert-ots-1.0.6/covert_ots.egg-info/SOURCES.txt
--rw-rw-r--   0 om        (1001) om        (1001)        1 2023-07-21 10:46:14.000000 covert-ots-1.0.6/covert_ots.egg-info/dependency_links.txt
--rw-rw-r--   0 om        (1001) om        (1001)       39 2023-07-21 10:46:14.000000 covert-ots-1.0.6/covert_ots.egg-info/entry_points.txt
--rw-rw-r--   0 om        (1001) om        (1001)       33 2023-07-21 10:46:14.000000 covert-ots-1.0.6/covert_ots.egg-info/requires.txt
--rw-rw-r--   0 om        (1001) om        (1001)        7 2023-07-21 10:46:14.000000 covert-ots-1.0.6/covert_ots.egg-info/top_level.txt
--rw-rw-r--   0 om        (1001) om        (1001)       38 2023-07-21 10:46:14.435300 covert-ots-1.0.6/setup.cfg
--rw-rw-r--   0 om        (1001) om        (1001)      844 2023-07-21 10:46:10.000000 covert-ots-1.0.6/setup.py
+drwxrwxr-x   0 om        (1001) om        (1001)        0 2023-07-21 10:48:54.457238 covert-ots-1.0.7/
+-rw-rw-r--   0 om        (1001) om        (1001)     1154 2023-07-21 10:48:54.457238 covert-ots-1.0.7/PKG-INFO
+-rw-rw-r--   0 om        (1001) om        (1001)       60 2023-07-17 19:18:34.000000 covert-ots-1.0.7/constants.py
+-rw-rw-r--   0 om        (1001) om        (1001)     3554 2023-07-18 05:15:15.000000 covert-ots-1.0.7/covert.py
+drwxrwxr-x   0 om        (1001) om        (1001)        0 2023-07-21 10:48:54.457238 covert-ots-1.0.7/covert_ots.egg-info/
+-rw-rw-r--   0 om        (1001) om        (1001)     1154 2023-07-21 10:48:54.000000 covert-ots-1.0.7/covert_ots.egg-info/PKG-INFO
+-rw-rw-r--   0 om        (1001) om        (1001)      241 2023-07-21 10:48:54.000000 covert-ots-1.0.7/covert_ots.egg-info/SOURCES.txt
+-rw-rw-r--   0 om        (1001) om        (1001)        1 2023-07-21 10:48:54.000000 covert-ots-1.0.7/covert_ots.egg-info/dependency_links.txt
+-rw-rw-r--   0 om        (1001) om        (1001)       39 2023-07-21 10:48:54.000000 covert-ots-1.0.7/covert_ots.egg-info/entry_points.txt
+-rw-rw-r--   0 om        (1001) om        (1001)       33 2023-07-21 10:48:54.000000 covert-ots-1.0.7/covert_ots.egg-info/requires.txt
+-rw-rw-r--   0 om        (1001) om        (1001)       17 2023-07-21 10:48:54.000000 covert-ots-1.0.7/covert_ots.egg-info/top_level.txt
+-rw-rw-r--   0 om        (1001) om        (1001)       38 2023-07-21 10:48:54.457238 covert-ots-1.0.7/setup.cfg
+-rw-rw-r--   0 om        (1001) om        (1001)      857 2023-07-21 10:48:16.000000 covert-ots-1.0.7/setup.py
```

### Comparing `covert-ots-1.0.6/PKG-INFO` & `covert-ots-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covert-ots
-Version: 1.0.6
+Version: 1.0.7
 Summary: A secure way to communicate your secrets
 Home-page: UNKNOWN
 Author: Om Gupta
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `covert-ots-1.0.6/covert.py` & `covert-ots-1.0.7/covert.py`

 * *Files identical despite different names*

### Comparing `covert-ots-1.0.6/covert_ots.egg-info/PKG-INFO` & `covert-ots-1.0.7/covert_ots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covert-ots
-Version: 1.0.6
+Version: 1.0.7
 Summary: A secure way to communicate your secrets
 Home-page: UNKNOWN
 Author: Om Gupta
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `covert-ots-1.0.6/setup.py` & `covert-ots-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import setuptools
 
 with open("../README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='covert-ots',
-   version='1.0.6',
+   version='1.0.7',
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
-    py_modules=["covert"],
+    py_modules=["covert", "constants"],
     package_dir={'':'.'},
     install_requires=[
       'typer',
       'rich',
       'inquirer',
       'pycryptodome'
    ],
```

