# Comparing `tmp/frozenclass-0.0.8.tar.gz` & `tmp/frozenclass-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frozenclass-0.0.8.tar", last modified: Thu Apr  6 14:36:38 2023, max compression
+gzip compressed data, was "frozenclass-0.0.9.tar", last modified: Wed Apr 12 16:03:39 2023, max compression
```

## Comparing `frozenclass-0.0.8.tar` & `frozenclass-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-04-06 14:36:38.897109 frozenclass-0.0.8/
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      677 2023-04-06 12:43:56.000000 frozenclass-0.0.8/LICENSE
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)     2894 2023-04-06 14:36:38.897109 frozenclass-0.0.8/PKG-INFO
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1987 2023-04-06 12:44:06.000000 frozenclass-0.0.8/README.md
-drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-04-06 14:36:38.896109 frozenclass-0.0.8/frozenclass/
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      115 2023-04-06 12:43:56.000000 frozenclass-0.0.8/frozenclass/__init__.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)     3567 2023-04-06 12:43:59.000000 frozenclass-0.0.8/frozenclass/data_controller.py
-drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-04-06 14:36:38.897109 frozenclass-0.0.8/frozenclass.egg-info/
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)     2894 2023-04-06 14:36:38.000000 frozenclass-0.0.8/frozenclass.egg-info/PKG-INFO
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      314 2023-04-06 14:36:38.000000 frozenclass-0.0.8/frozenclass.egg-info/SOURCES.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)        1 2023-04-06 14:36:38.000000 frozenclass-0.0.8/frozenclass.egg-info/dependency_links.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)       12 2023-04-06 14:36:38.000000 frozenclass-0.0.8/frozenclass.egg-info/top_level.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      985 2023-04-06 14:36:28.000000 frozenclass-0.0.8/pyproject.toml
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)       38 2023-04-06 14:36:38.897109 frozenclass-0.0.8/setup.cfg
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1424 2023-04-06 12:44:09.000000 frozenclass-0.0.8/setup.py
-drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-04-06 14:36:38.897109 frozenclass-0.0.8/tests/
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      934 2023-04-06 14:36:05.000000 frozenclass-0.0.8/tests/test_deep_save_load.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1461 2023-04-06 12:44:11.000000 frozenclass-0.0.8/tests/test_save_bases.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1007 2023-04-06 12:44:13.000000 frozenclass-0.0.8/tests/test_save_load.py
+drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-04-12 16:03:39.546409 frozenclass-0.0.9/
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)      677 2023-04-01 20:31:35.000000 frozenclass-0.0.9/LICENSE
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)     2826 2023-04-12 16:03:39.543075 frozenclass-0.0.9/PKG-INFO
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1920 2023-04-12 16:03:09.000000 frozenclass-0.0.9/README.md
+drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-04-12 16:03:39.539742 frozenclass-0.0.9/frozenclass/
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)      151 2023-04-12 15:59:40.000000 frozenclass-0.0.9/frozenclass/__init__.py
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)     2365 2023-04-12 16:00:06.000000 frozenclass-0.0.9/frozenclass/auto_freeze.py
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)     4989 2023-04-12 15:17:00.000000 frozenclass-0.0.9/frozenclass/data_controller.py
+drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-04-12 16:03:39.543075 frozenclass-0.0.9/frozenclass.egg-info/
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)     2826 2023-04-12 16:03:39.000000 frozenclass-0.0.9/frozenclass.egg-info/PKG-INFO
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)      364 2023-04-12 16:03:39.000000 frozenclass-0.0.9/frozenclass.egg-info/SOURCES.txt
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)        1 2023-04-12 16:03:39.000000 frozenclass-0.0.9/frozenclass.egg-info/dependency_links.txt
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)       12 2023-04-12 16:03:39.000000 frozenclass-0.0.9/frozenclass.egg-info/top_level.txt
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1011 2023-04-12 16:01:58.000000 frozenclass-0.0.9/pyproject.toml
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)       38 2023-04-12 16:03:39.546409 frozenclass-0.0.9/setup.cfg
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1406 2023-04-12 16:01:49.000000 frozenclass-0.0.9/setup.py
+drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-04-12 16:03:39.543075 frozenclass-0.0.9/tests/
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)      900 2023-04-12 16:00:56.000000 frozenclass-0.0.9/tests/test_autosave.py
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)      860 2023-04-08 16:22:08.000000 frozenclass-0.0.9/tests/test_deep_save_load.py
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1461 2023-04-05 19:34:07.000000 frozenclass-0.0.9/tests/test_save_bases.py
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1007 2023-04-05 19:34:07.000000 frozenclass-0.0.9/tests/test_save_load.py
```

### Comparing `frozenclass-0.0.8/LICENSE` & `frozenclass-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `frozenclass-0.0.8/PKG-INFO` & `frozenclass-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frozenclass
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python module for convenient storage of classes in files.
 Home-page: https://github.com/GigantPro/frozenclass
 Download-URL: https://github.com/Peopl3s/club-house-api/archive/main.zip
 Author: GigantPro
 Author-email: gigantpro2000@gmail.ru
 License: The GPLv3 License (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -16,65 +16,67 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Warning: project is unstable now. At the moment, the library has just begun to be developed, so this is not the final form of the product!
+<p align="center">
+        <h1 align="center">FrozenClass</h1>
+        <h2 align="center">This library was created in order to be able to save classes with a single line, as well as load them!</h2>
+</a>
+
+
 
 <p align="center">
         <a href="https://pypi.python.org/pypi/frozenclass"><img alt="Pypi version" src="https://img.shields.io/pypi/v/frozenclass.svg"></a>
         <a href="https://pypi.python.org/pypi/frozenclass"><img alt="Python versions" src="https://img.shields.io/badge/python-3.7+ | PyPy-blue.svg"></a>
         <img alt="Size" src="https://img.shields.io/github/languages/code-size/GigantPro/frozenclass">
         <a href="https://pypi.org/project/frozenclass/"><img alt="Pypi version" src="https://img.shields.io/pypi/l/frozenclass?color=orange"></a>
 </p>
 <p align="center">
         <a href="https://github.com/GigantPro/frozenclass/actions/workflows/tests.yml"><img alt="Testing status" src="https://github.com/GigantPro/frozenclass/actions/workflows/tests.yml/badge.svg?branch=main"></a>
         <a href="https://github.com/GigantPro/frozenclass/actions/workflows/linting.yml"><img alt="Linting" src="https://github.com/GigantPro/frozenclass/actions/workflows/linting.yml/badge.svg?branch=main"></a>
 </p>
 
-# frozenclass 
-This library was created in order to be able to save classes with a single line, as well as load them!
+
 
 
 
 ## Example
 ```python 
 from frozenclass import DataController
 
 
 # Test class
 class Test:
-    pass
+    test_var = 10
 
 
 # Init controller class
 data_controller = DataController('PATH_TO_SAVE`S FOLDER')
 
 # Save class as file
-data_controller.freeze_class(Test())
+save_name = data_controller.freeze_class(Test())
 
 # Get all saves classes models
-loaded_classes = data_controller.get_all_saves_list()  # -> list[class instances]
+loaded_classes = data_controller.load_save(save_name)  # -> Test object
+
+# Get var value
+print(test_var.test_var) # -> 10
 ```
 
 ## Installation
 
 ```bash
 $ pip install frozenclass
 ```
 
 ## Installation from source
 
 ### Dependencies:
 - **poetry**
 ```bash
-$ git clone https://github.com/GigantPro/frozenclass.git; cd frozenclass
-$ poetry run build
+$ git clone https://github.com/GigantPro/frozenclass.git; cd frozenclass-main
+$ poetry run build; cd dist
 $ pip install $(ls -Art | tail -n 1)
 ```
-
-## poetry install:
-```bash
-$ curl -sSL https://install.python-poetry.org | python3 -
-```
```

### Comparing `frozenclass-0.0.8/README.md` & `frozenclass-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,60 @@
-# Warning: project is unstable now. At the moment, the library has just begun to be developed, so this is not the final form of the product!
+<p align="center">
+        <h1 align="center">FrozenClass</h1>
+        <h2 align="center">This library was created in order to be able to save classes with a single line, as well as load them!</h2>
+</a>
+
+
 
 <p align="center">
         <a href="https://pypi.python.org/pypi/frozenclass"><img alt="Pypi version" src="https://img.shields.io/pypi/v/frozenclass.svg"></a>
         <a href="https://pypi.python.org/pypi/frozenclass"><img alt="Python versions" src="https://img.shields.io/badge/python-3.7+ | PyPy-blue.svg"></a>
         <img alt="Size" src="https://img.shields.io/github/languages/code-size/GigantPro/frozenclass">
         <a href="https://pypi.org/project/frozenclass/"><img alt="Pypi version" src="https://img.shields.io/pypi/l/frozenclass?color=orange"></a>
 </p>
 <p align="center">
         <a href="https://github.com/GigantPro/frozenclass/actions/workflows/tests.yml"><img alt="Testing status" src="https://github.com/GigantPro/frozenclass/actions/workflows/tests.yml/badge.svg?branch=main"></a>
         <a href="https://github.com/GigantPro/frozenclass/actions/workflows/linting.yml"><img alt="Linting" src="https://github.com/GigantPro/frozenclass/actions/workflows/linting.yml/badge.svg?branch=main"></a>
 </p>
 
-# frozenclass 
-This library was created in order to be able to save classes with a single line, as well as load them!
+
 
 
 
 ## Example
 ```python 
 from frozenclass import DataController
 
 
 # Test class
 class Test:
-    pass
+    test_var = 10
 
 
 # Init controller class
 data_controller = DataController('PATH_TO_SAVE`S FOLDER')
 
 # Save class as file
-data_controller.freeze_class(Test())
+save_name = data_controller.freeze_class(Test())
 
 # Get all saves classes models
-loaded_classes = data_controller.get_all_saves_list()  # -> list[class instances]
+loaded_classes = data_controller.load_save(save_name)  # -> Test object
+
+# Get var value
+print(test_var.test_var) # -> 10
 ```
 
 ## Installation
 
 ```bash
 $ pip install frozenclass
 ```
 
 ## Installation from source
 
 ### Dependencies:
 - **poetry**
 ```bash
-$ git clone https://github.com/GigantPro/frozenclass.git; cd frozenclass
-$ poetry run build
+$ git clone https://github.com/GigantPro/frozenclass.git; cd frozenclass-main
+$ poetry run build; cd dist
 $ pip install $(ls -Art | tail -n 1)
 ```
-
-## poetry install:
-```bash
-$ curl -sSL https://install.python-poetry.org | python3 -
-```
```

### Comparing `frozenclass-0.0.8/frozenclass.egg-info/PKG-INFO` & `frozenclass-0.0.9/frozenclass.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frozenclass
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python module for convenient storage of classes in files.
 Home-page: https://github.com/GigantPro/frozenclass
 Download-URL: https://github.com/Peopl3s/club-house-api/archive/main.zip
 Author: GigantPro
 Author-email: gigantpro2000@gmail.ru
 License: The GPLv3 License (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -16,65 +16,67 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Warning: project is unstable now. At the moment, the library has just begun to be developed, so this is not the final form of the product!
+<p align="center">
+        <h1 align="center">FrozenClass</h1>
+        <h2 align="center">This library was created in order to be able to save classes with a single line, as well as load them!</h2>
+</a>
+
+
 
 <p align="center">
         <a href="https://pypi.python.org/pypi/frozenclass"><img alt="Pypi version" src="https://img.shields.io/pypi/v/frozenclass.svg"></a>
         <a href="https://pypi.python.org/pypi/frozenclass"><img alt="Python versions" src="https://img.shields.io/badge/python-3.7+ | PyPy-blue.svg"></a>
         <img alt="Size" src="https://img.shields.io/github/languages/code-size/GigantPro/frozenclass">
         <a href="https://pypi.org/project/frozenclass/"><img alt="Pypi version" src="https://img.shields.io/pypi/l/frozenclass?color=orange"></a>
 </p>
 <p align="center">
         <a href="https://github.com/GigantPro/frozenclass/actions/workflows/tests.yml"><img alt="Testing status" src="https://github.com/GigantPro/frozenclass/actions/workflows/tests.yml/badge.svg?branch=main"></a>
         <a href="https://github.com/GigantPro/frozenclass/actions/workflows/linting.yml"><img alt="Linting" src="https://github.com/GigantPro/frozenclass/actions/workflows/linting.yml/badge.svg?branch=main"></a>
 </p>
 
-# frozenclass 
-This library was created in order to be able to save classes with a single line, as well as load them!
+
 
 
 
 ## Example
 ```python 
 from frozenclass import DataController
 
 
 # Test class
 class Test:
-    pass
+    test_var = 10
 
 
 # Init controller class
 data_controller = DataController('PATH_TO_SAVE`S FOLDER')
 
 # Save class as file
-data_controller.freeze_class(Test())
+save_name = data_controller.freeze_class(Test())
 
 # Get all saves classes models
-loaded_classes = data_controller.get_all_saves_list()  # -> list[class instances]
+loaded_classes = data_controller.load_save(save_name)  # -> Test object
+
+# Get var value
+print(test_var.test_var) # -> 10
 ```
 
 ## Installation
 
 ```bash
 $ pip install frozenclass
 ```
 
 ## Installation from source
 
 ### Dependencies:
 - **poetry**
 ```bash
-$ git clone https://github.com/GigantPro/frozenclass.git; cd frozenclass
-$ poetry run build
+$ git clone https://github.com/GigantPro/frozenclass.git; cd frozenclass-main
+$ poetry run build; cd dist
 $ pip install $(ls -Art | tail -n 1)
 ```
-
-## poetry install:
-```bash
-$ curl -sSL https://install.python-poetry.org | python3 -
-```
```

### Comparing `frozenclass-0.0.8/pyproject.toml` & `frozenclass-0.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "frozenclass"
-version = "0.0.8"
+version = "0.0.9"
 description = "Python module for convenient storage of classes in files."
 authors = ["GigantPro <gigantpro2000@gmail.com>"]
 license = "The GPLv3 License (GPLv3)"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
@@ -43,9 +43,11 @@
     "W0622",
     "W0105",
     "C0207",
     "C2801",
     "C0206",
     "C0200",
     "E0401",
-    "W1401"
+    "W1401",
+    "W0212",
+    "C0103"
 ]
```

### Comparing `frozenclass-0.0.8/setup.py` & `frozenclass-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 from io import open
 from setuptools import setup
 
 """
 :authors: GigantPro
-:license: The GPLv3 License (GPLv3), see LICENSE file
+:license: The GPLv3 License (GPLv3)
 :copyright: (c) 2023 Xiver organization
 """
 
 with open("pyproject.toml", encoding="utf-8") as file:
     VERSION = file.read().split("=")[2].split('"')[1]
 
 with open("README.md", encoding="utf-8") as f:
```

### Comparing `frozenclass-0.0.8/tests/test_deep_save_load.py` & `frozenclass-0.0.9/tests/test_deep_save_load.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-from random import choice
-from string import ascii_letters
-import pytest
-
 from frozenclass import DataController
 
 
 class PublicClassA:
     third = '123'
```

### Comparing `frozenclass-0.0.8/tests/test_save_bases.py` & `frozenclass-0.0.9/tests/test_save_bases.py`

 * *Files identical despite different names*

### Comparing `frozenclass-0.0.8/tests/test_save_load.py` & `frozenclass-0.0.9/tests/test_save_load.py`

 * *Files identical despite different names*

