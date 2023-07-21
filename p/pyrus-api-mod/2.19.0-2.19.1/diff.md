# Comparing `tmp/pyrus-api-mod-2.19.0.tar.gz` & `tmp/pyrus-api-mod-2.19.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrus-api-mod-2.19.0.tar", last modified: Fri Jul 21 13:41:15 2023, max compression
+gzip compressed data, was "pyrus-api-mod-2.19.1.tar", last modified: Fri Jul 21 13:55:20 2023, max compression
```

## Comparing `pyrus-api-mod-2.19.0.tar` & `pyrus-api-mod-2.19.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:41:15.730888 pyrus-api-mod-2.19.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-21 13:41:02.000000 pyrus-api-mod-2.19.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-07-21 13:41:15.730888 pyrus-api-mod-2.19.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-07-21 13:41:02.000000 pyrus-api-mod-2.19.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:41:15.726888 pyrus-api-mod-2.19.0/pyrus/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-21 13:41:02.000000 pyrus-api-mod-2.19.0/pyrus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25449 2023-07-21 13:41:02.000000 pyrus-api-mod-2.19.0/pyrus/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:41:15.726888 pyrus-api-mod-2.19.0/pyrus/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:41:02.000000 pyrus-api-mod-2.19.0/pyrus/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-21 13:41:02.000000 pyrus-api-mod-2.19.0/pyrus/models/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-21 13:41:02.000000 pyrus-api-mod-2.19.0/pyrus/models/customhandlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    46790 2023-07-21 13:41:02.000000 pyrus-api-mod-2.19.0/pyrus/models/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)    40781 2023-07-21 13:41:02.000000 pyrus-api-mod-2.19.0/pyrus/models/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    18381 2023-07-21 13:41:02.000000 pyrus-api-mod-2.19.0/pyrus/models/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:41:15.730888 pyrus-api-mod-2.19.0/pyrus_api_mod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-07-21 13:41:15.000000 pyrus-api-mod-2.19.0/pyrus_api_mod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-21 13:41:15.000000 pyrus-api-mod-2.19.0/pyrus_api_mod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:41:15.000000 pyrus-api-mod-2.19.0/pyrus_api_mod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-21 13:41:15.000000 pyrus-api-mod-2.19.0/pyrus_api_mod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 13:41:15.000000 pyrus-api-mod-2.19.0/pyrus_api_mod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:41:15.000000 pyrus-api-mod-2.19.0/pyrus_api_mod.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 13:41:15.730888 pyrus-api-mod-2.19.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-21 13:41:02.000000 pyrus-api-mod-2.19.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:55:20.205501 pyrus-api-mod-2.19.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-21 13:55:08.000000 pyrus-api-mod-2.19.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-21 13:55:20.205501 pyrus-api-mod-2.19.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-21 13:55:08.000000 pyrus-api-mod-2.19.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:55:20.205501 pyrus-api-mod-2.19.1/pyrus/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-21 13:55:08.000000 pyrus-api-mod-2.19.1/pyrus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25449 2023-07-21 13:55:08.000000 pyrus-api-mod-2.19.1/pyrus/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:55:20.205501 pyrus-api-mod-2.19.1/pyrus/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:55:08.000000 pyrus-api-mod-2.19.1/pyrus/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-21 13:55:08.000000 pyrus-api-mod-2.19.1/pyrus/models/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-21 13:55:08.000000 pyrus-api-mod-2.19.1/pyrus/models/customhandlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46790 2023-07-21 13:55:08.000000 pyrus-api-mod-2.19.1/pyrus/models/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40781 2023-07-21 13:55:08.000000 pyrus-api-mod-2.19.1/pyrus/models/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18381 2023-07-21 13:55:08.000000 pyrus-api-mod-2.19.1/pyrus/models/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:55:20.205501 pyrus-api-mod-2.19.1/pyrus_api_mod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-21 13:55:20.000000 pyrus-api-mod-2.19.1/pyrus_api_mod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-21 13:55:20.000000 pyrus-api-mod-2.19.1/pyrus_api_mod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:55:20.000000 pyrus-api-mod-2.19.1/pyrus_api_mod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-21 13:55:20.000000 pyrus-api-mod-2.19.1/pyrus_api_mod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 13:55:20.000000 pyrus-api-mod-2.19.1/pyrus_api_mod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:55:20.000000 pyrus-api-mod-2.19.1/pyrus_api_mod.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 13:55:20.205501 pyrus-api-mod-2.19.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-21 13:55:08.000000 pyrus-api-mod-2.19.1/setup.py
```

### Comparing `pyrus-api-mod-2.19.0/LICENSE.txt` & `pyrus-api-mod-2.19.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyrus-api-mod-2.19.0/PKG-INFO` & `pyrus-api-mod-2.19.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 Metadata-Version: 2.1
 Name: pyrus-api-mod
-Version: 2.19.0
+Version: 2.19.1
 Summary: Python Pyrus API client
 Home-page: https://pyrus.com/en/help/api
 Author: tailgrabik
 Author-email: tailgrabik@gmail.com
 License: MIT License
 Project-URL: GitHub Project, https://github.com/tailgrabik/pyrusapi-python
 Keywords: pyrus api
 Requires-Python: >=3.4
 License-File: LICENSE.txt
 
 ==============================
-pyrus-api
+pyrus-api-mod
 ==============================
 A python 3 client for the Pyrus API.
 
+Support custom URL for API and http proxy-server
+
 The full documentation for API can be found here_.
 
 .. _here: https://pyrus.com/en/help/api/
 
 -----------------
 Installation
 -----------------
 
 To get the latest version:
   - pip_ (preffrered)
-      $ pip install --upgrade pyrus-api
+      $ pip install --upgrade pyrus-api-mod
   - Setuptools_: Use the easy_install tool included in the setuptools package:
-      $ easy_install --upgrade pyrus-api
+      $ easy_install --upgrade pyrus-api-mod
   - Manual installation: `Download the latest version of pyrus-api client`_, unpack the code, and run 
       $ python setup.py install
 
 .. _pip: https://pypi.python.org/pypi/pip
 .. _Setuptools: https://pypi.python.org/pypi/setuptools
-.. _`Download the latest version of pyrus-api client`: https://pypi.python.org/pypi/pyrus-api/
+.. _`Download the latest version of pyrus-api client`: https://pypi.python.org/pypi/pyrus-api-mod/
 
 -----------------
 Usage
 -----------------
 To start with the module:
     
     >>>  from pyrus import client
     >>>  import pyrus.models
-    >>>  pyrus_client = client.PyrusAPI(login='login@pyrus.com', security_key='sadf2R5Wrdkn..')
+    >>>  pyrus_client = client.PyrusAPI(login='login@example.com', security_key='sadf2R5Wrdkn..',proxy='http://proxy:3128',api_addr='api.pyrus.com')
 
 -----------------
 Examples
 -----------------
 Authenticate:
     
     >>> pyrus_client.auth()
```

### Comparing `pyrus-api-mod-2.19.0/README.rst` & `pyrus-api-mod-2.19.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 ==============================
-pyrus-api
+pyrus-api-mod
 ==============================
 A python 3 client for the Pyrus API.
 
+Support custom URL for API and http proxy-server
+
 The full documentation for API can be found here_.
 
 .. _here: https://pyrus.com/en/help/api/
 
 -----------------
 Installation
 -----------------
 
 To get the latest version:
   - pip_ (preffrered)
-      $ pip install --upgrade pyrus-api
+      $ pip install --upgrade pyrus-api-mod
   - Setuptools_: Use the easy_install tool included in the setuptools package:
-      $ easy_install --upgrade pyrus-api
+      $ easy_install --upgrade pyrus-api-mod
   - Manual installation: `Download the latest version of pyrus-api client`_, unpack the code, and run 
       $ python setup.py install
 
 .. _pip: https://pypi.python.org/pypi/pip
 .. _Setuptools: https://pypi.python.org/pypi/setuptools
-.. _`Download the latest version of pyrus-api client`: https://pypi.python.org/pypi/pyrus-api/
+.. _`Download the latest version of pyrus-api client`: https://pypi.python.org/pypi/pyrus-api-mod/
 
 -----------------
 Usage
 -----------------
 To start with the module:
     
     >>>  from pyrus import client
     >>>  import pyrus.models
-    >>>  pyrus_client = client.PyrusAPI(login='login@pyrus.com', security_key='sadf2R5Wrdkn..')
+    >>>  pyrus_client = client.PyrusAPI(login='login@example.com', security_key='sadf2R5Wrdkn..',proxy='http://proxy:3128',api_addr='api.pyrus.com')
 
 -----------------
 Examples
 -----------------
 Authenticate:
     
     >>> pyrus_client.auth()
```

### Comparing `pyrus-api-mod-2.19.0/pyrus/client.py` & `pyrus-api-mod-2.19.1/pyrus/client.py`

 * *Files identical despite different names*

### Comparing `pyrus-api-mod-2.19.0/pyrus/models/customhandlers.py` & `pyrus-api-mod-2.19.1/pyrus/models/customhandlers.py`

 * *Files identical despite different names*

### Comparing `pyrus-api-mod-2.19.0/pyrus/models/entities.py` & `pyrus-api-mod-2.19.1/pyrus/models/entities.py`

 * *Files identical despite different names*

### Comparing `pyrus-api-mod-2.19.0/pyrus/models/requests.py` & `pyrus-api-mod-2.19.1/pyrus/models/requests.py`

 * *Files identical despite different names*

### Comparing `pyrus-api-mod-2.19.0/pyrus/models/responses.py` & `pyrus-api-mod-2.19.1/pyrus/models/responses.py`

 * *Files identical despite different names*

### Comparing `pyrus-api-mod-2.19.0/pyrus_api_mod.egg-info/PKG-INFO` & `pyrus-api-mod-2.19.1/pyrus_api_mod.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 Metadata-Version: 2.1
 Name: pyrus-api-mod
-Version: 2.19.0
+Version: 2.19.1
 Summary: Python Pyrus API client
 Home-page: https://pyrus.com/en/help/api
 Author: tailgrabik
 Author-email: tailgrabik@gmail.com
 License: MIT License
 Project-URL: GitHub Project, https://github.com/tailgrabik/pyrusapi-python
 Keywords: pyrus api
 Requires-Python: >=3.4
 License-File: LICENSE.txt
 
 ==============================
-pyrus-api
+pyrus-api-mod
 ==============================
 A python 3 client for the Pyrus API.
 
+Support custom URL for API and http proxy-server
+
 The full documentation for API can be found here_.
 
 .. _here: https://pyrus.com/en/help/api/
 
 -----------------
 Installation
 -----------------
 
 To get the latest version:
   - pip_ (preffrered)
-      $ pip install --upgrade pyrus-api
+      $ pip install --upgrade pyrus-api-mod
   - Setuptools_: Use the easy_install tool included in the setuptools package:
-      $ easy_install --upgrade pyrus-api
+      $ easy_install --upgrade pyrus-api-mod
   - Manual installation: `Download the latest version of pyrus-api client`_, unpack the code, and run 
       $ python setup.py install
 
 .. _pip: https://pypi.python.org/pypi/pip
 .. _Setuptools: https://pypi.python.org/pypi/setuptools
-.. _`Download the latest version of pyrus-api client`: https://pypi.python.org/pypi/pyrus-api/
+.. _`Download the latest version of pyrus-api client`: https://pypi.python.org/pypi/pyrus-api-mod/
 
 -----------------
 Usage
 -----------------
 To start with the module:
     
     >>>  from pyrus import client
     >>>  import pyrus.models
-    >>>  pyrus_client = client.PyrusAPI(login='login@pyrus.com', security_key='sadf2R5Wrdkn..')
+    >>>  pyrus_client = client.PyrusAPI(login='login@example.com', security_key='sadf2R5Wrdkn..',proxy='http://proxy:3128',api_addr='api.pyrus.com')
 
 -----------------
 Examples
 -----------------
 Authenticate:
     
     >>> pyrus_client.auth()
```

### Comparing `pyrus-api-mod-2.19.0/setup.py` & `pyrus-api-mod-2.19.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from setuptools import setup, find_packages
 
 setup(name="pyrus-api-mod",
-      version="2.19.0",
+      version="2.19.1",
       python_requires='>=3.4',
       description="Python Pyrus API client",
       author="tailgrabik",
       long_description=open('README.rst', 'r').read(),
       author_email="tailgrabik@gmail.com",
       url="https://pyrus.com/en/help/api",
       project_urls={
```

