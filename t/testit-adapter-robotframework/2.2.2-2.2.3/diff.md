# Comparing `tmp/testit-adapter-robotframework-2.2.2.tar.gz` & `tmp/testit-adapter-robotframework-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-adapter-robotframework-2.2.2.tar", last modified: Wed Jul 19 15:06:44 2023, max compression
+gzip compressed data, was "testit-adapter-robotframework-2.2.3.tar", last modified: Fri Jul 21 09:41:12 2023, max compression
```

## Comparing `testit-adapter-robotframework-2.2.2.tar` & `testit-adapter-robotframework-2.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:06:44.187054 testit-adapter-robotframework-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-07-19 15:06:44.187054 testit-adapter-robotframework-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12757 2023-07-19 15:06:32.000000 testit-adapter-robotframework-2.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 15:06:44.187054 testit-adapter-robotframework-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-19 15:06:32.000000 testit-adapter-robotframework-2.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:06:44.183054 testit-adapter-robotframework-2.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:06:44.183054 testit-adapter-robotframework-2.2.2/src/testit_adapter_robotframework/
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-07-19 15:06:32.000000 testit-adapter-robotframework-2.2.2/src/testit_adapter_robotframework/TMSLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:06:32.000000 testit-adapter-robotframework-2.2.2/src/testit_adapter_robotframework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-19 15:06:32.000000 testit-adapter-robotframework-2.2.2/src/testit_adapter_robotframework/listeners.py
--rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-07-19 15:06:32.000000 testit-adapter-robotframework-2.2.2/src/testit_adapter_robotframework/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-19 15:06:32.000000 testit-adapter-robotframework-2.2.2/src/testit_adapter_robotframework/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:06:44.183054 testit-adapter-robotframework-2.2.2/src/testit_adapter_robotframework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-07-19 15:06:44.000000 testit-adapter-robotframework-2.2.2/src/testit_adapter_robotframework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-19 15:06:44.000000 testit-adapter-robotframework-2.2.2/src/testit_adapter_robotframework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 15:06:44.000000 testit-adapter-robotframework-2.2.2/src/testit_adapter_robotframework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-19 15:06:44.000000 testit-adapter-robotframework-2.2.2/src/testit_adapter_robotframework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-19 15:06:44.000000 testit-adapter-robotframework-2.2.2/src/testit_adapter_robotframework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:41:12.439534 testit-adapter-robotframework-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-07-21 09:41:12.439534 testit-adapter-robotframework-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12757 2023-07-21 09:41:02.000000 testit-adapter-robotframework-2.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 09:41:12.439534 testit-adapter-robotframework-2.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-21 09:41:02.000000 testit-adapter-robotframework-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:41:12.435534 testit-adapter-robotframework-2.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:41:12.435534 testit-adapter-robotframework-2.2.3/src/testit_adapter_robotframework/
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-07-21 09:41:02.000000 testit-adapter-robotframework-2.2.3/src/testit_adapter_robotframework/TMSLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:41:02.000000 testit-adapter-robotframework-2.2.3/src/testit_adapter_robotframework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-21 09:41:02.000000 testit-adapter-robotframework-2.2.3/src/testit_adapter_robotframework/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-07-21 09:41:02.000000 testit-adapter-robotframework-2.2.3/src/testit_adapter_robotframework/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-21 09:41:02.000000 testit-adapter-robotframework-2.2.3/src/testit_adapter_robotframework/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:41:12.439534 testit-adapter-robotframework-2.2.3/src/testit_adapter_robotframework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-07-21 09:41:12.000000 testit-adapter-robotframework-2.2.3/src/testit_adapter_robotframework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-21 09:41:12.000000 testit-adapter-robotframework-2.2.3/src/testit_adapter_robotframework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 09:41:12.000000 testit-adapter-robotframework-2.2.3/src/testit_adapter_robotframework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-21 09:41:12.000000 testit-adapter-robotframework-2.2.3/src/testit_adapter_robotframework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-21 09:41:12.000000 testit-adapter-robotframework-2.2.3/src/testit_adapter_robotframework.egg-info/top_level.txt
```

### Comparing `testit-adapter-robotframework-2.2.2/PKG-INFO` & `testit-adapter-robotframework-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-robotframework
-Version: 2.2.2
+Version: 2.2.3
 Summary: Robot Framework adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-adapter-robotframework-2.2.2/README.md` & `testit-adapter-robotframework-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `testit-adapter-robotframework-2.2.2/setup.py` & `testit-adapter-robotframework-2.2.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-adapter-robotframework',
-    version='2.2.2',
+    version='2.2.3',
     description='Robot Framework adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -16,9 +16,9 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     py_modules=['testit_adapter_robotframework'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['attrs', 'robotframework', 'testit-python-commons==2.2.2']
+    install_requires=['attrs', 'robotframework', 'testit-python-commons==2.2.3']
 )
```

### Comparing `testit-adapter-robotframework-2.2.2/src/testit_adapter_robotframework/TMSLibrary.py` & `testit-adapter-robotframework-2.2.3/src/testit_adapter_robotframework/TMSLibrary.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-robotframework-2.2.2/src/testit_adapter_robotframework/listeners.py` & `testit-adapter-robotframework-2.2.3/src/testit_adapter_robotframework/listeners.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-robotframework-2.2.2/src/testit_adapter_robotframework/models.py` & `testit-adapter-robotframework-2.2.3/src/testit_adapter_robotframework/models.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-robotframework-2.2.2/src/testit_adapter_robotframework/utils.py` & `testit-adapter-robotframework-2.2.3/src/testit_adapter_robotframework/utils.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-robotframework-2.2.2/src/testit_adapter_robotframework.egg-info/PKG-INFO` & `testit-adapter-robotframework-2.2.3/src/testit_adapter_robotframework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-robotframework
-Version: 2.2.2
+Version: 2.2.3
 Summary: Robot Framework adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-adapter-robotframework-2.2.2/src/testit_adapter_robotframework.egg-info/SOURCES.txt` & `testit-adapter-robotframework-2.2.3/src/testit_adapter_robotframework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

