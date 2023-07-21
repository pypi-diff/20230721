# Comparing `tmp/idelium-1.0.1.tar.gz` & `tmp/idelium-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idelium-1.0.1.tar", last modified: Wed Jul  5 12:54:57 2023, max compression
+gzip compressed data, was "idelium-1.0.3.tar", last modified: Fri Jul 21 15:16:57 2023, max compression
```

## Comparing `idelium-1.0.1.tar` & `idelium-1.0.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-07-05 12:54:57.403307 idelium-1.0.1/
--rw-rw-r--   0 idelfuschini   (501) staff       (20)      541 2021-11-05 11:16:26.000000 idelium-1.0.1/LICENSE.txt
--rw-r--r--   0 idelfuschini   (501) staff       (20)      218 2023-07-03 14:50:05.000000 idelium-1.0.1/MANIFEST.in
--rw-r--r--   0 idelfuschini   (501) staff       (20)     3848 2023-07-05 12:54:57.403448 idelium-1.0.1/PKG-INFO
--rw-rw-r--   0 idelfuschini   (501) staff       (20)     2544 2023-07-05 07:53:28.000000 idelium-1.0.1/README.md
--rw-r--r--   0 idelfuschini   (501) staff       (20)     2033 2023-06-30 13:38:23.000000 idelium-1.0.1/pyproject.toml
--rw-rw-rw-   0 idelfuschini   (501) staff       (20)     1281 2023-07-05 12:54:57.404729 idelium-1.0.1/setup.cfg
--rw-rw-r--   0 idelfuschini   (501) staff       (20)     4596 2023-07-05 12:52:31.000000 idelium-1.0.1/setup.py
-drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-07-05 12:54:57.390253 idelium-1.0.1/src/
-drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-07-05 12:54:57.392973 idelium-1.0.1/src/idelium/
--rw-r--r--   0 idelfuschini   (501) staff       (20)      361 2023-07-05 07:52:27.000000 idelium-1.0.1/src/idelium/__init__.py
-drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-07-05 12:54:57.396902 idelium-1.0.1/src/idelium/_internal/
--rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2023-07-03 13:43:10.000000 idelium-1.0.1/src/idelium/_internal/__init__.py
-drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-07-05 12:54:57.397803 idelium-1.0.1/src/idelium/_internal/bdd/
--rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2022-02-21 11:18:20.000000 idelium-1.0.1/src/idelium/_internal/bdd/__init__.py
--rw-r--r--   0 idelfuschini   (501) staff       (20)      193 2022-02-21 18:55:48.000000 idelium-1.0.1/src/idelium/_internal/bdd/bdd.py
--rw-r--r--   0 idelfuschini   (501) staff       (20)      273 2022-02-21 18:29:38.000000 idelium-1.0.1/src/idelium/_internal/bdd/webservice.py
-drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-07-05 12:54:57.399784 idelium-1.0.1/src/idelium/_internal/commons/
--rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2021-08-13 11:45:16.000000 idelium-1.0.1/src/idelium/_internal/commons/__init__.py
--rw-rw-r--   0 idelfuschini   (501) staff       (20)    13873 2021-12-02 13:19:23.000000 idelium-1.0.1/src/idelium/_internal/commons/androideventkey.py
--rw-rw-r--   0 idelfuschini   (501) staff       (20)      822 2021-12-02 13:22:25.000000 idelium-1.0.1/src/idelium/_internal/commons/ideliumprinter.py
--rw-rw-r--   0 idelfuschini   (501) staff       (20)      494 2021-12-02 14:11:51.000000 idelium-1.0.1/src/idelium/_internal/commons/proxy.py
--rw-rw-r--   0 idelfuschini   (501) staff       (20)      152 2021-12-02 14:15:27.000000 idelium-1.0.1/src/idelium/_internal/commons/resultenum.py
--rw-r--r--   0 idelfuschini   (501) staff       (20)      794 2021-12-02 16:50:19.000000 idelium-1.0.1/src/idelium/_internal/commons/seleniumby.py
--rw-r--r--   0 idelfuschini   (501) staff       (20)     2798 2021-12-02 16:45:25.000000 idelium-1.0.1/src/idelium/_internal/commons/seleniumkeyevent.py
-drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-07-05 12:54:57.399981 idelium-1.0.1/src/idelium/_internal/extra/
--rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2021-08-13 11:45:16.000000 idelium-1.0.1/src/idelium/_internal/extra/__init__.py
--rw-r--r--   0 idelfuschini   (501) staff       (20)     9027 2023-07-05 07:54:25.000000 idelium-1.0.1/src/idelium/_internal/ideliumclib.py
--rw-rw-r--   0 idelfuschini   (501) staff       (20)     6384 2023-07-03 16:48:58.000000 idelium-1.0.1/src/idelium/_internal/ideliummanager.py
--rw-r--r--   0 idelfuschini   (501) staff       (20)     3054 2022-01-17 18:40:07.000000 idelium-1.0.1/src/idelium/_internal/ideliumserver.py
--rw-rw-r--   0 idelfuschini   (501) staff       (20)    15846 2022-08-05 10:35:26.000000 idelium-1.0.1/src/idelium/_internal/ideliumws.py
--rw-rw-r--   0 idelfuschini   (501) staff       (20)     2559 2023-07-05 12:54:46.000000 idelium-1.0.1/src/idelium/_internal/main.py
-drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-07-05 12:54:57.400678 idelium-1.0.1/src/idelium/_internal/thirdparties/
--rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2021-08-13 11:45:16.000000 idelium-1.0.1/src/idelium/_internal/thirdparties/__init__.py
--rw-r--r--   0 idelfuschini   (501) staff       (20)     2600 2023-07-03 16:48:58.000000 idelium-1.0.1/src/idelium/_internal/thirdparties/ideliumpostman.py
--rw-rw-r--   0 idelfuschini   (501) staff       (20)    19193 2023-07-03 16:48:58.000000 idelium-1.0.1/src/idelium/_internal/thirdparties/ideliumzephyr.py
-drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-07-05 12:54:57.401547 idelium-1.0.1/src/idelium/_internal/thirdparties/postpy2/
--rw-r--r--   0 idelfuschini   (501) staff       (20)        0 2022-05-23 20:39:45.000000 idelium-1.0.1/src/idelium/_internal/thirdparties/postpy2/__init__.py
--rw-r--r--   0 idelfuschini   (501) staff       (20)     6996 2022-08-26 14:29:29.000000 idelium-1.0.1/src/idelium/_internal/thirdparties/postpy2/core.py
--rw-r--r--   0 idelfuschini   (501) staff       (20)     2846 2022-05-23 20:39:45.000000 idelium-1.0.1/src/idelium/_internal/thirdparties/postpy2/extractors.py
-drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-07-05 12:54:57.402793 idelium-1.0.1/src/idelium/_internal/wrappers/
--rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2021-08-13 11:45:16.000000 idelium-1.0.1/src/idelium/_internal/wrappers/__init__.py
--rw-rw-r--   0 idelfuschini   (501) staff       (20)    29783 2023-07-03 16:48:58.000000 idelium-1.0.1/src/idelium/_internal/wrappers/ideliumappium.py
--rw-rw-r--   0 idelfuschini   (501) staff       (20)    17796 2023-07-05 10:30:22.000000 idelium-1.0.1/src/idelium/_internal/wrappers/ideliumselenium.py
--rw-rw-rw-   0 idelfuschini   (501) staff       (20)      294 2023-07-03 13:37:10.000000 idelium-1.0.1/src/idelium/py.typed
-drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-07-05 12:54:57.395082 idelium-1.0.1/src/idelium.egg-info/
--rw-r--r--   0 idelfuschini   (501) staff       (20)     3848 2023-07-05 12:54:57.000000 idelium-1.0.1/src/idelium.egg-info/PKG-INFO
--rw-r--r--   0 idelfuschini   (501) staff       (20)     1496 2023-07-05 12:54:57.000000 idelium-1.0.1/src/idelium.egg-info/SOURCES.txt
--rw-r--r--   0 idelfuschini   (501) staff       (20)        1 2023-07-05 12:54:57.000000 idelium-1.0.1/src/idelium.egg-info/dependency_links.txt
--rw-r--r--   0 idelfuschini   (501) staff       (20)       56 2023-07-05 12:54:57.000000 idelium-1.0.1/src/idelium.egg-info/entry_points.txt
--rw-r--r--   0 idelfuschini   (501) staff       (20)        1 2023-07-03 14:35:54.000000 idelium-1.0.1/src/idelium.egg-info/not-zip-safe
--rw-r--r--   0 idelfuschini   (501) staff       (20)      111 2023-07-05 12:54:57.000000 idelium-1.0.1/src/idelium.egg-info/requires.txt
--rw-r--r--   0 idelfuschini   (501) staff       (20)        8 2023-07-05 12:54:57.000000 idelium-1.0.1/src/idelium.egg-info/top_level.txt
+drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-07-21 15:16:57.927467 idelium-1.0.3/
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)      541 2021-11-05 11:16:26.000000 idelium-1.0.3/LICENSE.txt
+-rw-r--r--   0 idelfuschini   (501) staff       (20)      218 2023-07-03 14:50:05.000000 idelium-1.0.3/MANIFEST.in
+-rw-r--r--   0 idelfuschini   (501) staff       (20)     3648 2023-07-21 15:16:57.927584 idelium-1.0.3/PKG-INFO
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)     2344 2023-07-20 16:52:00.000000 idelium-1.0.3/README.md
+-rw-r--r--   0 idelfuschini   (501) staff       (20)     2033 2023-06-30 13:38:23.000000 idelium-1.0.3/pyproject.toml
+-rw-rw-rw-   0 idelfuschini   (501) staff       (20)     1281 2023-07-21 15:16:57.928670 idelium-1.0.3/setup.cfg
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)     4455 2023-07-05 13:06:58.000000 idelium-1.0.3/setup.py
+drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-07-21 15:16:57.912196 idelium-1.0.3/src/
+drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-07-21 15:16:57.915325 idelium-1.0.3/src/idelium/
+-rw-r--r--   0 idelfuschini   (501) staff       (20)      361 2023-07-05 07:52:27.000000 idelium-1.0.3/src/idelium/__init__.py
+drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-07-21 15:16:57.919387 idelium-1.0.3/src/idelium/_internal/
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2023-07-03 13:43:10.000000 idelium-1.0.3/src/idelium/_internal/__init__.py
+drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-07-21 15:16:57.919987 idelium-1.0.3/src/idelium/_internal/bdd/
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2022-02-21 11:18:20.000000 idelium-1.0.3/src/idelium/_internal/bdd/__init__.py
+-rw-r--r--   0 idelfuschini   (501) staff       (20)      193 2022-02-21 18:55:48.000000 idelium-1.0.3/src/idelium/_internal/bdd/bdd.py
+-rw-r--r--   0 idelfuschini   (501) staff       (20)      273 2022-02-21 18:29:38.000000 idelium-1.0.3/src/idelium/_internal/bdd/webservice.py
+drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-07-21 15:16:57.922109 idelium-1.0.3/src/idelium/_internal/commons/
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2021-08-13 11:45:16.000000 idelium-1.0.3/src/idelium/_internal/commons/__init__.py
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)    13873 2021-12-02 13:19:23.000000 idelium-1.0.3/src/idelium/_internal/commons/androideventkey.py
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)      822 2021-12-02 13:22:25.000000 idelium-1.0.3/src/idelium/_internal/commons/ideliumprinter.py
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)      494 2021-12-02 14:11:51.000000 idelium-1.0.3/src/idelium/_internal/commons/proxy.py
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)      152 2021-12-02 14:15:27.000000 idelium-1.0.3/src/idelium/_internal/commons/resultenum.py
+-rw-r--r--   0 idelfuschini   (501) staff       (20)      794 2021-12-02 16:50:19.000000 idelium-1.0.3/src/idelium/_internal/commons/seleniumby.py
+-rw-r--r--   0 idelfuschini   (501) staff       (20)     2798 2021-12-02 16:45:25.000000 idelium-1.0.3/src/idelium/_internal/commons/seleniumkeyevent.py
+drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-07-21 15:16:57.922320 idelium-1.0.3/src/idelium/_internal/extra/
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2021-08-13 11:45:16.000000 idelium-1.0.3/src/idelium/_internal/extra/__init__.py
+-rw-r--r--   0 idelfuschini   (501) staff       (20)     9027 2023-07-05 07:54:25.000000 idelium-1.0.3/src/idelium/_internal/ideliumclib.py
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)     6437 2023-07-21 14:04:58.000000 idelium-1.0.3/src/idelium/_internal/ideliummanager.py
+-rw-r--r--   0 idelfuschini   (501) staff       (20)     3054 2022-01-17 18:40:07.000000 idelium-1.0.3/src/idelium/_internal/ideliumserver.py
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)    15865 2023-07-21 14:34:45.000000 idelium-1.0.3/src/idelium/_internal/ideliumws.py
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)     2558 2023-07-21 15:16:50.000000 idelium-1.0.3/src/idelium/_internal/main.py
+drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-07-21 15:16:57.922874 idelium-1.0.3/src/idelium/_internal/thirdparties/
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2021-08-13 11:45:16.000000 idelium-1.0.3/src/idelium/_internal/thirdparties/__init__.py
+-rw-r--r--   0 idelfuschini   (501) staff       (20)     2600 2023-07-03 16:48:58.000000 idelium-1.0.3/src/idelium/_internal/thirdparties/ideliumpostman.py
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)    19193 2023-07-03 16:48:58.000000 idelium-1.0.3/src/idelium/_internal/thirdparties/ideliumzephyr.py
+drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-07-21 15:16:57.926177 idelium-1.0.3/src/idelium/_internal/thirdparties/postpy2/
+-rw-r--r--   0 idelfuschini   (501) staff       (20)        0 2022-05-23 20:39:45.000000 idelium-1.0.3/src/idelium/_internal/thirdparties/postpy2/__init__.py
+-rw-r--r--   0 idelfuschini   (501) staff       (20)     6996 2022-08-26 14:29:29.000000 idelium-1.0.3/src/idelium/_internal/thirdparties/postpy2/core.py
+-rw-r--r--   0 idelfuschini   (501) staff       (20)     2846 2022-05-23 20:39:45.000000 idelium-1.0.3/src/idelium/_internal/thirdparties/postpy2/extractors.py
+drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-07-21 15:16:57.927093 idelium-1.0.3/src/idelium/_internal/wrappers/
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2021-08-13 11:45:16.000000 idelium-1.0.3/src/idelium/_internal/wrappers/__init__.py
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)    29783 2023-07-03 16:48:58.000000 idelium-1.0.3/src/idelium/_internal/wrappers/ideliumappium.py
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)    17796 2023-07-05 10:30:22.000000 idelium-1.0.3/src/idelium/_internal/wrappers/ideliumselenium.py
+-rw-rw-rw-   0 idelfuschini   (501) staff       (20)      294 2023-07-03 13:37:10.000000 idelium-1.0.3/src/idelium/py.typed
+drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-07-21 15:16:57.916848 idelium-1.0.3/src/idelium.egg-info/
+-rw-r--r--   0 idelfuschini   (501) staff       (20)     3648 2023-07-21 15:16:57.000000 idelium-1.0.3/src/idelium.egg-info/PKG-INFO
+-rw-r--r--   0 idelfuschini   (501) staff       (20)     1496 2023-07-21 15:16:57.000000 idelium-1.0.3/src/idelium.egg-info/SOURCES.txt
+-rw-r--r--   0 idelfuschini   (501) staff       (20)        1 2023-07-21 15:16:57.000000 idelium-1.0.3/src/idelium.egg-info/dependency_links.txt
+-rw-r--r--   0 idelfuschini   (501) staff       (20)       56 2023-07-21 15:16:57.000000 idelium-1.0.3/src/idelium.egg-info/entry_points.txt
+-rw-r--r--   0 idelfuschini   (501) staff       (20)        1 2023-07-03 14:35:54.000000 idelium-1.0.3/src/idelium.egg-info/not-zip-safe
+-rw-r--r--   0 idelfuschini   (501) staff       (20)      111 2023-07-21 15:16:57.000000 idelium-1.0.3/src/idelium.egg-info/requires.txt
+-rw-r--r--   0 idelfuschini   (501) staff       (20)        8 2023-07-21 15:16:57.000000 idelium-1.0.3/src/idelium.egg-info/top_level.txt
```

### Comparing `idelium-1.0.1/LICENSE.txt` & `idelium-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `idelium-1.0.1/PKG-INFO` & `idelium-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idelium
-Version: 1.0.1
+Version: 1.0.3
 Summary: Command line Test Automation Tool
 Home-page: https://idelium.io/
 Author: Idel Fuschini
 Author-email: idel.fuschini@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/idelium/idelium-cli/issues
 Project-URL: Project, https://idelium.io
@@ -30,49 +30,32 @@
 Provides-Extra: test
 License-File: LICENSE.txt
 
 ![Idelium](https://idelium.io/assets/images/idelium.png)
 
 # Idelium-CLI
 
-This is Idelium Command Line is the tool for test automation integrated with Idelium Web.
+This is Idelium Command Line is the tool for test automation integrated with [Idelium AS](https://github.com/idelium/idelium-docker).
 
 Idelium-CLI can be used through a continues integration software, such as Jenkins, GitLabs, Bamboo etc.
 
 For more info: https://idelium.io
 
 [![Introducing Idelium](https://img.youtube.com/vi/nGe3c_CU0NQ/0.jpg)](https://youtu.be/nGe3c_CU0NQ)
 
-## Requirement
+## Prerequisite
 
 Python 3.8.X
 
-## Install Libraries
+## Installing
 
+If you have pip on your system, you can simply install or upgrade the Python bindings:
 
 ```
-pip install selenium
-pip install libmagic
-pip install Appium-Python-Client
-pip install webdriver-manager
-pip install Pillow
-$ pip install Postpy2
-pip install git+https://github.com/behave/behave
-```
-On windows:
-```
-pip install Pillow
-```
-
-
-## Download idelium-cli
-
-```
-git clone https://github.com/idelium/idelium-cli.git
-cd idelium-cli
+pip install
 ```
 
 ## Run the script
 
 idelium-cli can be used in two ways:
 
 To directly launch a test cycle, useful for those who want to integrate integration tests with jenkins, bamboo or similar:
```

### Comparing `idelium-1.0.1/README.md` & `idelium-1.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,29 @@
 ![Idelium](https://idelium.io/assets/images/idelium.png)
 
 # Idelium-CLI
 
-This is Idelium Command Line is the tool for test automation integrated with Idelium Web.
+This is Idelium Command Line is the tool for test automation integrated with [Idelium AS](https://github.com/idelium/idelium-docker).
 
 Idelium-CLI can be used through a continues integration software, such as Jenkins, GitLabs, Bamboo etc.
 
 For more info: https://idelium.io
 
 [![Introducing Idelium](https://img.youtube.com/vi/nGe3c_CU0NQ/0.jpg)](https://youtu.be/nGe3c_CU0NQ)
 
-## Requirement
+## Prerequisite
 
 Python 3.8.X
 
-## Install Libraries
+## Installing
 
+If you have pip on your system, you can simply install or upgrade the Python bindings:
 
 ```
-pip install selenium
-pip install libmagic
-pip install Appium-Python-Client
-pip install webdriver-manager
-pip install Pillow
-$ pip install Postpy2
-pip install git+https://github.com/behave/behave
-```
-On windows:
-```
-pip install Pillow
-```
-
-
-## Download idelium-cli
-
-```
-git clone https://github.com/idelium/idelium-cli.git
-cd idelium-cli
+pip install
 ```
 
 ## Run the script
 
 idelium-cli can be used in two ways:
 
 To directly launch a test cycle, useful for those who want to integrate integration tests with jenkins, bamboo or similar:
```

### Comparing `idelium-1.0.1/pyproject.toml` & `idelium-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `idelium-1.0.1/setup.cfg` & `idelium-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `idelium-1.0.1/setup.py` & `idelium-1.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 
 
 this_dir = abspath(dirname(__file__))
 with open(join(this_dir, 'README.md'), encoding='utf-8') as file:
     long_description = file.read()
 def read(rel_path: str) -> str:
     here = os.path.abspath(os.path.dirname(__file__))
-    # intentionally *not* adding an encoding option to open, See:
-    #   https://github.com/pypa/virtualenv/issues/201#issuecomment-3145690
     with open(os.path.join(here, rel_path)) as fp:
         return fp.read()
 
 
 def get_version(rel_path: str) -> str:
     for line in read(rel_path).splitlines():
         if line.startswith("IDELIUM_VERSION"):
```

### Comparing `idelium-1.0.1/src/idelium/_internal/commons/androideventkey.py` & `idelium-1.0.3/src/idelium/_internal/commons/androideventkey.py`

 * *Files identical despite different names*

### Comparing `idelium-1.0.1/src/idelium/_internal/commons/ideliumprinter.py` & `idelium-1.0.3/src/idelium/_internal/commons/ideliumprinter.py`

 * *Files identical despite different names*

### Comparing `idelium-1.0.1/src/idelium/_internal/commons/seleniumby.py` & `idelium-1.0.3/src/idelium/_internal/commons/seleniumby.py`

 * *Files identical despite different names*

### Comparing `idelium-1.0.1/src/idelium/_internal/commons/seleniumkeyevent.py` & `idelium-1.0.3/src/idelium/_internal/commons/seleniumkeyevent.py`

 * *Files identical despite different names*

### Comparing `idelium-1.0.1/src/idelium/_internal/ideliumclib.py` & `idelium-1.0.3/src/idelium/_internal/ideliumclib.py`

 * *Files identical despite different names*

### Comparing `idelium-1.0.1/src/idelium/_internal/ideliummanager.py` & `idelium-1.0.3/src/idelium/_internal/ideliummanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         ''' Execute single step '''
         status = "1"
         step_failed = ""
         wrapper = config["wrapper"]
         printer = config["printer"]
         typeOfStep='seleniumOrAppium'
         postman_data=None
+        print (config["json_step"]["steps"])        
         for object_step in config["json_step"]["steps"]:
             if status == "1":
                 if object_step['stepType'] == 'postman_collection':
                     #postman=PostmanCollection()
                     #postman_data=postman.start_postman_test(object_step['collection'])
                     typeOfStep='postman'
                 else:
```

### Comparing `idelium-1.0.1/src/idelium/_internal/ideliumserver.py` & `idelium-1.0.3/src/idelium/_internal/ideliumserver.py`

 * *Files identical despite different names*

### Comparing `idelium-1.0.1/src/idelium/_internal/ideliumws.py` & `idelium-1.0.3/src/idelium/_internal/ideliumws.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,14 @@
         return Connection.start("PUT", url, payload, config["ideliumKey"],
                                 config["is_debug"])
 
     @staticmethod
     def create_step(config, id_test, id_step, name, status, data, typeofstep):
         ''' create step '''
         url = config["api_idelium"] + "step"
-        print (data)
         payload = {
             "testCycleId": config['idCycle'],
             "testId": id_test,
             "stepId": id_step,
             "name": name,
             "status": int(status),
             "data": json.dumps(data),
@@ -310,17 +309,18 @@
                     driver = object_return["driver"]
                     postman_data=object_return["postman_data"]
                     typeofstep=object_return["type"]
                     step_failed = object_return["step_failed"]
                     config["status"] = status
                     config["step_failed"] = step_failed
                     id_step = None
+                    #test["name"],
                     if config["test"] is False:
                         id_step = self.create_step(config, id_test, test["id"],
-                                                 test["name"],
+                                                 json_step["name"],
                                                  status,
                                                  postman_data,
                                                  typeofstep
                                                  )['idStep']
                     if status in ('2','5') and object_return['type']=='seleniumOrAppium':
                         path = "screenshots/"
                         file_name = str(id_test) + ".png"
```

### Comparing `idelium-1.0.1/src/idelium/_internal/main.py` & `idelium-1.0.3/src/idelium/_internal/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from idelium._internal.commons.ideliumprinter import InitPrinter
 
 
 idelium=StartManager()
 printer=InitPrinter()
 ideliumws=IdeliumWs()
 idelium_cl_lib=InitIdelium()
-IDELIUM_VERSION='1.0.1'
+IDELIUM_VERSION='1.0.3'
 
 def main(args: Optional[List[str]] = None) -> int:
     printer.print_important_text("Idelium Command Line " + IDELIUM_VERSION)
     printer.print_important_text ("Selenium version:" + idelium_cl_lib.get_selenium_version())
     if args is None:
         args = sys.argv
     define_parameters= idelium_cl_lib.define_parameters(args,ideliumws,printer)
@@ -54,8 +54,7 @@
         sslctx.check_hostname = False
         sslctx.load_cert_chain(certfile='cert/cert.pem', keyfile="cert/key.pem")
         httpd = HTTPServer(server_address, IdeliumServer)
         httpd.socket = sslctx.wrap_socket(httpd.socket, server_side=True)
         printer.success('Server start on port:' +
             str(cl_params['ideliumServerPort']))
         httpd.serve_forever()
-
```

### Comparing `idelium-1.0.1/src/idelium/_internal/thirdparties/ideliumpostman.py` & `idelium-1.0.3/src/idelium/_internal/thirdparties/ideliumpostman.py`

 * *Files identical despite different names*

### Comparing `idelium-1.0.1/src/idelium/_internal/thirdparties/ideliumzephyr.py` & `idelium-1.0.3/src/idelium/_internal/thirdparties/ideliumzephyr.py`

 * *Files identical despite different names*

### Comparing `idelium-1.0.1/src/idelium/_internal/thirdparties/postpy2/core.py` & `idelium-1.0.3/src/idelium/_internal/thirdparties/postpy2/core.py`

 * *Files identical despite different names*

### Comparing `idelium-1.0.1/src/idelium/_internal/thirdparties/postpy2/extractors.py` & `idelium-1.0.3/src/idelium/_internal/thirdparties/postpy2/extractors.py`

 * *Files identical despite different names*

### Comparing `idelium-1.0.1/src/idelium/_internal/wrappers/ideliumappium.py` & `idelium-1.0.3/src/idelium/_internal/wrappers/ideliumappium.py`

 * *Files identical despite different names*

### Comparing `idelium-1.0.1/src/idelium/_internal/wrappers/ideliumselenium.py` & `idelium-1.0.3/src/idelium/_internal/wrappers/ideliumselenium.py`

 * *Files identical despite different names*

### Comparing `idelium-1.0.1/src/idelium.egg-info/PKG-INFO` & `idelium-1.0.3/src/idelium.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idelium
-Version: 1.0.1
+Version: 1.0.3
 Summary: Command line Test Automation Tool
 Home-page: https://idelium.io/
 Author: Idel Fuschini
 Author-email: idel.fuschini@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/idelium/idelium-cli/issues
 Project-URL: Project, https://idelium.io
@@ -30,49 +30,32 @@
 Provides-Extra: test
 License-File: LICENSE.txt
 
 ![Idelium](https://idelium.io/assets/images/idelium.png)
 
 # Idelium-CLI
 
-This is Idelium Command Line is the tool for test automation integrated with Idelium Web.
+This is Idelium Command Line is the tool for test automation integrated with [Idelium AS](https://github.com/idelium/idelium-docker).
 
 Idelium-CLI can be used through a continues integration software, such as Jenkins, GitLabs, Bamboo etc.
 
 For more info: https://idelium.io
 
 [![Introducing Idelium](https://img.youtube.com/vi/nGe3c_CU0NQ/0.jpg)](https://youtu.be/nGe3c_CU0NQ)
 
-## Requirement
+## Prerequisite
 
 Python 3.8.X
 
-## Install Libraries
+## Installing
 
+If you have pip on your system, you can simply install or upgrade the Python bindings:
 
 ```
-pip install selenium
-pip install libmagic
-pip install Appium-Python-Client
-pip install webdriver-manager
-pip install Pillow
-$ pip install Postpy2
-pip install git+https://github.com/behave/behave
-```
-On windows:
-```
-pip install Pillow
-```
-
-
-## Download idelium-cli
-
-```
-git clone https://github.com/idelium/idelium-cli.git
-cd idelium-cli
+pip install
 ```
 
 ## Run the script
 
 idelium-cli can be used in two ways:
 
 To directly launch a test cycle, useful for those who want to integrate integration tests with jenkins, bamboo or similar:
```

### Comparing `idelium-1.0.1/src/idelium.egg-info/SOURCES.txt` & `idelium-1.0.3/src/idelium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

