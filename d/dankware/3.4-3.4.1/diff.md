# Comparing `tmp/dankware-3.4.tar.gz` & `tmp/dankware-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dankware-3.4.tar", last modified: Thu Jun  8 11:39:02 2023, max compression
+gzip compressed data, was "dankware-3.4.1.tar", last modified: Fri Jul 21 18:04:37 2023, max compression
```

## Comparing `dankware-3.4.tar` & `dankware-3.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:39:02.130062 dankware-3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-08 11:38:49.000000 dankware-3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16297 2023-06-08 11:39:02.130062 dankware-3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-06-08 11:38:49.000000 dankware-3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:39:02.130062 dankware-3.4/dankware/
--rw-r--r--   0 runner    (1001) docker     (123)    46643 2023-06-08 11:38:49.000000 dankware-3.4/dankware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:39:02.130062 dankware-3.4/dankware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16297 2023-06-08 11:39:02.000000 dankware-3.4/dankware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-08 11:39:02.000000 dankware-3.4/dankware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:39:02.000000 dankware-3.4/dankware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 11:39:02.000000 dankware-3.4/dankware.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 11:39:02.000000 dankware-3.4/dankware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 11:39:02.130062 dankware-3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-08 11:38:49.000000 dankware-3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:04:37.863592 dankware-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-21 18:04:23.000000 dankware-3.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16479 2023-07-21 18:04:37.863592 dankware-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15540 2023-07-21 18:04:23.000000 dankware-3.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:04:37.859592 dankware-3.4.1/dankware/
+-rw-r--r--   0 runner    (1001) docker     (123)    46790 2023-07-21 18:04:23.000000 dankware-3.4.1/dankware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:04:37.863592 dankware-3.4.1/dankware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16479 2023-07-21 18:04:37.000000 dankware-3.4.1/dankware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-21 18:04:37.000000 dankware-3.4.1/dankware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 18:04:37.000000 dankware-3.4.1/dankware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 18:04:37.000000 dankware-3.4.1/dankware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 18:04:37.000000 dankware-3.4.1/dankware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 18:04:37.863592 dankware-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-21 18:04:23.000000 dankware-3.4.1/setup.py
```

### Comparing `dankware-3.4/LICENSE` & `dankware-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dankware-3.4/PKG-INFO` & `dankware-3.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dankware
-Version: 3.4
+Version: 3.4.1
 Summary: Python package with various features!
 Home-page: https://github.com/SirDank/dankware
 Author: SirDank
 Author-email: SirDankenstein@protonmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/SirDank/dankware
 Project-URL: Bug Tracker, https://github.com/SirDank/dankware/issues
@@ -438,27 +438,27 @@
 
 ---  
 
 # 🚨 Wallpapers 🚨
 
 ## ♦️ Style 1 ♦️
 
-<br><p align="center"><img width="700" alt="image" src="__wallpapers__/1.png"></p><br>
+<br><p align="center"><img width="700" alt="image" src="https://github.com/SirDank/dankware/raw/main/__wallpapers__/1.png"></p><br>
 
 ## ♦️ Style 2 ♦️
 
-<br><p align="center"><img width="700" alt="image" src="__wallpapers__/2.jpg"></p><br>
+<br><p align="center"><img width="700" alt="image" src="https://github.com/SirDank/dankware/raw/main/__wallpapers__/2.jpg"></p><br>
 
 ## ♦️ Style 3 ♦️
 
-<br><p align="center"><img width="700" alt="image" src="__wallpapers__/3.png"></p><br>
+<br><p align="center"><img width="700" alt="image" src="https://github.com/SirDank/dankware/raw/main/__wallpapers__/3.png"></p><br>
 
 ## ♦️ Style 4 ♦️
 
-<br><p align="center"><img width="700" alt="image" src="__wallpapers__/4.png"></p><br>
+<br><p align="center"><img width="700" alt="image" src="https://github.com/SirDank/dankware/raw/main/__wallpapers__/4.png"></p><br>
 
 <p>&nbsp;</p>
 
 ---  
 
 # 🚨 Stats 🚨
```

### Comparing `dankware-3.4/README.md` & `dankware-3.4.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -416,27 +416,27 @@
 
 ---  
 
 # 🚨 Wallpapers 🚨
 
 ## ♦️ Style 1 ♦️
 
-<br><p align="center"><img width="700" alt="image" src="__wallpapers__/1.png"></p><br>
+<br><p align="center"><img width="700" alt="image" src="https://github.com/SirDank/dankware/raw/main/__wallpapers__/1.png"></p><br>
 
 ## ♦️ Style 2 ♦️
 
-<br><p align="center"><img width="700" alt="image" src="__wallpapers__/2.jpg"></p><br>
+<br><p align="center"><img width="700" alt="image" src="https://github.com/SirDank/dankware/raw/main/__wallpapers__/2.jpg"></p><br>
 
 ## ♦️ Style 3 ♦️
 
-<br><p align="center"><img width="700" alt="image" src="__wallpapers__/3.png"></p><br>
+<br><p align="center"><img width="700" alt="image" src="https://github.com/SirDank/dankware/raw/main/__wallpapers__/3.png"></p><br>
 
 ## ♦️ Style 4 ♦️
 
-<br><p align="center"><img width="700" alt="image" src="__wallpapers__/4.png"></p><br>
+<br><p align="center"><img width="700" alt="image" src="https://github.com/SirDank/dankware/raw/main/__wallpapers__/4.png"></p><br>
 
 <p>&nbsp;</p>
 
 ---  
 
 # 🚨 Stats 🚨
```

### Comparing `dankware-3.4/dankware/__init__.py` & `dankware-3.4.1/dankware/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 ###################################################################################
 
 import os
 import sys
 import time
 import random
 from datetime import datetime
-from colorama import Fore, Style
+from colorama import Fore, Style, init
+
+init(autoreset=True)
 
 # colorama colours
 reset = Style.RESET_ALL
 
 black = Fore.BLACK + Style.BRIGHT
 blue = Fore.BLUE + Style.BRIGHT
 cyan = Fore.CYAN + Style.BRIGHT
@@ -772,15 +774,18 @@
     ```python
     from concurrent.futures import ThreadPoolExecutor
     ThreadPoolExecutor().submit(splash_screen, "splash.gif", duration=3)
     ```
     """
     
     import tkinter as tk
-    from PIL import Image, ImageTk
+    try:
+        from PIL import Image, ImageTk
+    except:
+        raise ImportError("Pillow is not installed! Run 'pip install pillow' to install it!")
     
     class SplashScreen(tk.Toplevel):
 
         def __init__(self, img_path):
             super().__init__()
             self.img_path = img_path
             self.setup_window()
```

### Comparing `dankware-3.4/dankware.egg-info/PKG-INFO` & `dankware-3.4.1/dankware.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dankware
-Version: 3.4
+Version: 3.4.1
 Summary: Python package with various features!
 Home-page: https://github.com/SirDank/dankware
 Author: SirDank
 Author-email: SirDankenstein@protonmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/SirDank/dankware
 Project-URL: Bug Tracker, https://github.com/SirDank/dankware/issues
@@ -438,27 +438,27 @@
 
 ---  
 
 # 🚨 Wallpapers 🚨
 
 ## ♦️ Style 1 ♦️
 
-<br><p align="center"><img width="700" alt="image" src="__wallpapers__/1.png"></p><br>
+<br><p align="center"><img width="700" alt="image" src="https://github.com/SirDank/dankware/raw/main/__wallpapers__/1.png"></p><br>
 
 ## ♦️ Style 2 ♦️
 
-<br><p align="center"><img width="700" alt="image" src="__wallpapers__/2.jpg"></p><br>
+<br><p align="center"><img width="700" alt="image" src="https://github.com/SirDank/dankware/raw/main/__wallpapers__/2.jpg"></p><br>
 
 ## ♦️ Style 3 ♦️
 
-<br><p align="center"><img width="700" alt="image" src="__wallpapers__/3.png"></p><br>
+<br><p align="center"><img width="700" alt="image" src="https://github.com/SirDank/dankware/raw/main/__wallpapers__/3.png"></p><br>
 
 ## ♦️ Style 4 ♦️
 
-<br><p align="center"><img width="700" alt="image" src="__wallpapers__/4.png"></p><br>
+<br><p align="center"><img width="700" alt="image" src="https://github.com/SirDank/dankware/raw/main/__wallpapers__/4.png"></p><br>
 
 <p>&nbsp;</p>
 
 ---  
 
 # 🚨 Stats 🚨
```

### Comparing `dankware-3.4/setup.py` & `dankware-3.4.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
 
     license = "MIT",
     name = "dankware",
-    version = "3.4",
+    version = "3.4.1",
     author = "SirDank",
     
     author_email = "SirDankenstein@protonmail.com",
     description = "Python package with various features!",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type = "text/markdown",
     url = "https://github.com/SirDank/dankware",
@@ -46,10 +46,9 @@
 
     package_dir = {"": "."},
     packages = find_packages(where = "."),
     install_requires = [
         "rich",
         "colorama",
         "requests",
-        "pillow",
     ],
 )
```

