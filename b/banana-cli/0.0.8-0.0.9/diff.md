# Comparing `tmp/banana_cli-0.0.8.tar.gz` & `tmp/banana_cli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "banana_cli-0.0.8.tar", last modified: Wed Mar 22 17:58:40 2023, max compression
+gzip compressed data, was "banana_cli-0.0.9.tar", last modified: Fri Mar 24 06:11:57 2023, max compression
```

## Comparing `banana_cli-0.0.8.tar` & `banana_cli-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-03-22 17:58:40.043110 banana_cli-0.0.8/
--rw-r--r--   0 erik       (501) staff       (20)    10947 2023-03-01 01:18:48.000000 banana_cli-0.0.8/LICENSE
--rw-r--r--   0 erik       (501) staff       (20)     2270 2023-03-22 17:58:40.042993 banana_cli-0.0.8/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)     1635 2023-03-22 17:55:54.000000 banana_cli-0.0.8/README.md
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-03-22 17:58:40.041892 banana_cli-0.0.8/banana_cli/
--rw-r--r--   0 erik       (501) staff       (20)       20 2023-03-22 17:56:26.000000 banana_cli-0.0.8/banana_cli/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)     2002 2023-03-22 17:49:22.000000 banana_cli-0.0.8/banana_cli/cli.py
--rw-r--r--   0 erik       (501) staff       (20)     2950 2023-03-22 17:49:22.000000 banana_cli-0.0.8/banana_cli/cmd_dev.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-03-22 17:58:40.042780 banana_cli-0.0.8/banana_cli/process/
--rw-r--r--   0 erik       (501) staff       (20)        0 2023-03-22 17:56:28.000000 banana_cli-0.0.8/banana_cli/process/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)       59 2023-03-22 17:49:22.000000 banana_cli-0.0.8/banana_cli/process/run.py
--rw-r--r--   0 erik       (501) staff       (20)     3197 2023-03-22 17:49:22.000000 banana_cli-0.0.8/banana_cli/utils.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-03-22 17:58:40.042585 banana_cli-0.0.8/banana_cli.egg-info/
--rw-r--r--   0 erik       (501) staff       (20)     2270 2023-03-22 17:58:40.000000 banana_cli-0.0.8/banana_cli.egg-info/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)      372 2023-03-22 17:58:40.000000 banana_cli-0.0.8/banana_cli.egg-info/SOURCES.txt
--rw-r--r--   0 erik       (501) staff       (20)        1 2023-03-22 17:58:40.000000 banana_cli-0.0.8/banana_cli.egg-info/dependency_links.txt
--rw-r--r--   0 erik       (501) staff       (20)       42 2023-03-22 17:58:40.000000 banana_cli-0.0.8/banana_cli.egg-info/entry_points.txt
--rw-r--r--   0 erik       (501) staff       (20)       35 2023-03-22 17:58:40.000000 banana_cli-0.0.8/banana_cli.egg-info/requires.txt
--rw-r--r--   0 erik       (501) staff       (20)       15 2023-03-22 17:58:40.000000 banana_cli-0.0.8/banana_cli.egg-info/top_level.txt
--rw-r--r--   0 erik       (501) staff       (20)       38 2023-03-22 17:58:40.043144 banana_cli-0.0.8/setup.cfg
--rw-r--r--   0 erik       (501) staff       (20)     1383 2023-03-22 17:55:24.000000 banana_cli-0.0.8/setup.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-03-24 06:11:57.377371 banana_cli-0.0.9/
+-rw-r--r--   0 erik       (501) staff       (20)    10947 2023-03-01 01:18:48.000000 banana_cli-0.0.9/LICENSE
+-rw-r--r--   0 erik       (501) staff       (20)     2446 2023-03-24 06:11:57.377226 banana_cli-0.0.9/PKG-INFO
+-rw-r--r--   0 erik       (501) staff       (20)     1811 2023-03-24 06:11:09.000000 banana_cli-0.0.9/README.md
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-03-24 06:11:57.375418 banana_cli-0.0.9/banana_cli/
+-rw-r--r--   0 erik       (501) staff       (20)       20 2023-03-22 17:56:26.000000 banana_cli-0.0.9/banana_cli/__init__.py
+-rw-r--r--   0 erik       (501) staff       (20)     2002 2023-03-24 04:46:11.000000 banana_cli-0.0.9/banana_cli/cli.py
+-rw-r--r--   0 erik       (501) staff       (20)     3648 2023-03-24 05:59:25.000000 banana_cli-0.0.9/banana_cli/cmd_dev.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-03-24 06:11:57.376888 banana_cli-0.0.9/banana_cli/process/
+-rw-r--r--   0 erik       (501) staff       (20)        0 2023-03-22 17:56:28.000000 banana_cli-0.0.9/banana_cli/process/__init__.py
+-rw-r--r--   0 erik       (501) staff       (20)      659 2023-03-24 05:55:03.000000 banana_cli-0.0.9/banana_cli/process/cells.py
+-rw-r--r--   0 erik       (501) staff       (20)       59 2023-03-22 17:49:22.000000 banana_cli-0.0.9/banana_cli/process/run.py
+-rw-r--r--   0 erik       (501) staff       (20)     3210 2023-03-24 04:52:28.000000 banana_cli-0.0.9/banana_cli/utils.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-03-24 06:11:57.376139 banana_cli-0.0.9/banana_cli.egg-info/
+-rw-r--r--   0 erik       (501) staff       (20)     2446 2023-03-24 06:11:57.000000 banana_cli-0.0.9/banana_cli.egg-info/PKG-INFO
+-rw-r--r--   0 erik       (501) staff       (20)      400 2023-03-24 06:11:57.000000 banana_cli-0.0.9/banana_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 erik       (501) staff       (20)        1 2023-03-24 06:11:57.000000 banana_cli-0.0.9/banana_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 erik       (501) staff       (20)       42 2023-03-24 06:11:57.000000 banana_cli-0.0.9/banana_cli.egg-info/entry_points.txt
+-rw-r--r--   0 erik       (501) staff       (20)       35 2023-03-24 06:11:57.000000 banana_cli-0.0.9/banana_cli.egg-info/requires.txt
+-rw-r--r--   0 erik       (501) staff       (20)       15 2023-03-24 06:11:57.000000 banana_cli-0.0.9/banana_cli.egg-info/top_level.txt
+-rw-r--r--   0 erik       (501) staff       (20)       38 2023-03-24 06:11:57.377415 banana_cli-0.0.9/setup.cfg
+-rw-r--r--   0 erik       (501) staff       (20)     1383 2023-03-24 06:09:58.000000 banana_cli-0.0.9/setup.py
```

### Comparing `banana_cli-0.0.8/LICENSE` & `banana_cli-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `banana_cli-0.0.8/PKG-INFO` & `banana_cli-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banana_cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: The Banana CLI helps you build Potassium apps
 Home-page: https://www.banana.dev
 Author: Erik Dunteman
 Author-email: erik@banana.dev
 License: Apache License 2.0
 Keywords: Banana server,HTTP server,Banana,Framework
 Classifier: Development Status :: 3 - Alpha
@@ -29,27 +29,32 @@
 This is a v0 release using SemVer; it is not stable and the interface can break at any time.
 ---
 
 ## To use it
 
 1. Install the CLI with pip
 ```bash
-pip3 install banana-cli==0.0.8
+pip3 install banana-cli==0.0.9
 ```
 
 2. Create a new project directory with 
 ```bash
 banana init my-app
 cd my-app
 ```
 3. Start the dev server
 ```bash
 banana dev
 ```
 
+4. Call your API (from a separate terminal)
+```bash
+curl -X POST -H "Content-Type: application/json" -d '{"prompt": "Hello I am a [MASK] model."}' http://localhost:8000/
+``` 
+
 ## Hot-Reload Dev Server
 
 The interactive dev server works like a react, next, or nodemon server: it selectively hot reloads components when you save changes to different parts of your `app.py` file.
 
 The init() function is ran on startup and for every change to init().
 
 The handler() function is ran on every change to handler(), without needing to wait for a long init()
```

### Comparing `banana_cli-0.0.8/README.md` & `banana_cli-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,27 +11,32 @@
 This is a v0 release using SemVer; it is not stable and the interface can break at any time.
 ---
 
 ## To use it
 
 1. Install the CLI with pip
 ```bash
-pip3 install banana-cli==0.0.8
+pip3 install banana-cli==0.0.9
 ```
 
 2. Create a new project directory with 
 ```bash
 banana init my-app
 cd my-app
 ```
 3. Start the dev server
 ```bash
 banana dev
 ```
 
+4. Call your API (from a separate terminal)
+```bash
+curl -X POST -H "Content-Type: application/json" -d '{"prompt": "Hello I am a [MASK] model."}' http://localhost:8000/
+``` 
+
 ## Hot-Reload Dev Server
 
 The interactive dev server works like a react, next, or nodemon server: it selectively hot reloads components when you save changes to different parts of your `app.py` file.
 
 The init() function is ran on startup and for every change to init().
 
 The handler() function is ran on every change to handler(), without needing to wait for a long init()
```

### Comparing `banana_cli-0.0.8/banana_cli/cli.py` & `banana_cli-0.0.9/banana_cli/cli.py`

 * *Files identical despite different names*

### Comparing `banana_cli-0.0.8/banana_cli/utils.py` & `banana_cli-0.0.9/banana_cli/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import venv
 import shutil
 import subprocess
 import sys
+import click
 
 # Uses git to clone the potassium boilerplate from /boilerplate/potassium in this git repo
 def download_boilerplate(target_dir):
     from git import Repo
     # git clone to tmp dir
     temp_dir = os.path.join(target_dir, "tmp")
     Repo.clone_from("https://github.com/bananaml/banana-cli.git", temp_dir)
```

### Comparing `banana_cli-0.0.8/banana_cli.egg-info/PKG-INFO` & `banana_cli-0.0.9/banana_cli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banana-cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: The Banana CLI helps you build Potassium apps
 Home-page: https://www.banana.dev
 Author: Erik Dunteman
 Author-email: erik@banana.dev
 License: Apache License 2.0
 Keywords: Banana server,HTTP server,Banana,Framework
 Classifier: Development Status :: 3 - Alpha
@@ -29,27 +29,32 @@
 This is a v0 release using SemVer; it is not stable and the interface can break at any time.
 ---
 
 ## To use it
 
 1. Install the CLI with pip
 ```bash
-pip3 install banana-cli==0.0.8
+pip3 install banana-cli==0.0.9
 ```
 
 2. Create a new project directory with 
 ```bash
 banana init my-app
 cd my-app
 ```
 3. Start the dev server
 ```bash
 banana dev
 ```
 
+4. Call your API (from a separate terminal)
+```bash
+curl -X POST -H "Content-Type: application/json" -d '{"prompt": "Hello I am a [MASK] model."}' http://localhost:8000/
+``` 
+
 ## Hot-Reload Dev Server
 
 The interactive dev server works like a react, next, or nodemon server: it selectively hot reloads components when you save changes to different parts of your `app.py` file.
 
 The init() function is ran on startup and for every change to init().
 
 The handler() function is ran on every change to handler(), without needing to wait for a long init()
```

### Comparing `banana_cli-0.0.8/setup.py` & `banana_cli-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='banana_cli',
     packages=['banana_cli', 'banana_cli.process'],
     py_modules=["cli"],
-    version='0.0.8',
+    version='0.0.9',
     license='Apache License 2.0',
     # Give a short description about your library
     description='The Banana CLI helps you build Potassium apps',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Erik Dunteman',
     author_email='erik@banana.dev',
```

