# Comparing `tmp/baysalt_christmas-0.1.9.0.tar.gz` & `tmp/baysalt_christmas-0.1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baysalt_christmas-0.1.9.0.tar", last modified: Thu Jul 13 06:20:22 2023, max compression
+gzip compressed data, was "baysalt_christmas-0.1.9.1.tar", last modified: Fri Jul 21 06:24:05 2023, max compression
```

## Comparing `baysalt_christmas-0.1.9.0.tar` & `baysalt_christmas-0.1.9.1.tar`

### file list

```diff
@@ -1,36 +1,41 @@
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-13 06:20:22.091675 baysalt_christmas-0.1.9.0/
--rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-07-13 03:38:11.000000 baysalt_christmas-0.1.9.0/.DS_Store
--rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.9.0/MANIFEST.in
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-13 06:20:22.091546 baysalt_christmas-0.1.9.0/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.9.0/README.md
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-13 06:20:22.087493 baysalt_christmas-0.1.9.0/baysalt_christmas.egg-info/
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-13 06:20:21.000000 baysalt_christmas-0.1.9.0/baysalt_christmas.egg-info/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)      788 2023-07-13 06:20:22.000000 baysalt_christmas-0.1.9.0/baysalt_christmas.egg-info/SOURCES.txt
--rw-r--r--   0 christmas   (501) staff       (20)        1 2023-07-13 06:20:21.000000 baysalt_christmas-0.1.9.0/baysalt_christmas.egg-info/dependency_links.txt
--rw-r--r--   0 christmas   (501) staff       (20)       30 2023-07-13 06:20:21.000000 baysalt_christmas-0.1.9.0/baysalt_christmas.egg-info/requires.txt
--rw-r--r--   0 christmas   (501) staff       (20)       10 2023-07-13 06:20:21.000000 baysalt_christmas-0.1.9.0/baysalt_christmas.egg-info/top_level.txt
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-13 06:20:22.089481 baysalt_christmas-0.1.9.0/christmas/
--rw-r--r--   0 christmas   (501) staff       (20)    22668 2023-07-13 06:19:54.000000 baysalt_christmas-0.1.9.0/christmas/Blogging.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-13 06:20:22.089911 baysalt_christmas-0.1.9.0/christmas/Pyshell/
--rw-r--r--   0 christmas   (501) staff       (20)     5957 2023-07-04 08:34:25.000000 baysalt_christmas-0.1.9.0/christmas/Pyshell/RS_File.py
--rw-r--r--   0 christmas   (501) staff       (20)      249 2023-07-03 02:25:19.000000 baysalt_christmas-0.1.9.0/christmas/Pyshell/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.9.0/christmas/S_DateTime.py
--rw-r--r--   0 christmas   (501) staff       (20)      405 2023-07-13 04:50:52.000000 baysalt_christmas-0.1.9.0/christmas/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.9.0/christmas/commonCode.py
--rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.9.0/christmas/cprintf.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-13 06:20:22.090703 baysalt_christmas-0.1.9.0/christmas/mncPy/
--rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.9.0/christmas/mncPy/.gitignore
--rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.9.0/christmas/mncPy/LICENSE
--rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.9.0/christmas/mncPy/__init__.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-13 06:20:22.091241 baysalt_christmas-0.1.9.0/christmas/mncPy/__pycache__/
--rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.9.0/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.9.0/christmas/mncPy/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.9.0/christmas/mncPy/__pycache__/compress.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.9.0/christmas/mncPy/common.py
--rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.9.0/christmas/mncPy/compress.py
--rw-r--r--   0 christmas   (501) staff       (20)     9260 2023-07-10 06:49:33.000000 baysalt_christmas-0.1.9.0/christmas/processBar.py
--rw-r--r--   0 christmas   (501) staff       (20)     3679 2023-06-12 03:11:04.000000 baysalt_christmas-0.1.9.0/christmas/read_conf.py
--rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.9.0/christmas/server_info.py
--rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.9.0/run_twine.py
--rw-r--r--   0 christmas   (501) staff       (20)       38 2023-07-13 06:20:22.091728 baysalt_christmas-0.1.9.0/setup.cfg
--rw-r--r--   0 christmas   (501) staff       (20)      796 2023-07-13 06:20:20.000000 baysalt_christmas-0.1.9.0/setup.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-21 06:24:05.959264 baysalt_christmas-0.1.9.1/
+-rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-07-13 03:38:11.000000 baysalt_christmas-0.1.9.1/.DS_Store
+-rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.9.1/MANIFEST.in
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-21 06:24:05.959129 baysalt_christmas-0.1.9.1/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.9.1/README.md
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-21 06:24:05.952976 baysalt_christmas-0.1.9.1/baysalt_christmas.egg-info/
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-21 06:24:05.000000 baysalt_christmas-0.1.9.1/baysalt_christmas.egg-info/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)      931 2023-07-21 06:24:05.000000 baysalt_christmas-0.1.9.1/baysalt_christmas.egg-info/SOURCES.txt
+-rw-r--r--   0 christmas   (501) staff       (20)        1 2023-07-21 06:24:05.000000 baysalt_christmas-0.1.9.1/baysalt_christmas.egg-info/dependency_links.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       30 2023-07-21 06:24:05.000000 baysalt_christmas-0.1.9.1/baysalt_christmas.egg-info/requires.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       10 2023-07-21 06:24:05.000000 baysalt_christmas-0.1.9.1/baysalt_christmas.egg-info/top_level.txt
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-21 06:24:05.955622 baysalt_christmas-0.1.9.1/christmas/
+-rw-r--r--   0 christmas   (501) staff       (20)    22668 2023-07-13 06:19:54.000000 baysalt_christmas-0.1.9.1/christmas/Blogging.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-21 06:24:05.956087 baysalt_christmas-0.1.9.1/christmas/Pyshell/
+-rw-r--r--   0 christmas   (501) staff       (20)     5957 2023-07-04 08:34:25.000000 baysalt_christmas-0.1.9.1/christmas/Pyshell/RS_File.py
+-rw-r--r--   0 christmas   (501) staff       (20)      249 2023-07-03 02:25:19.000000 baysalt_christmas-0.1.9.1/christmas/Pyshell/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.9.1/christmas/S_DateTime.py
+-rw-r--r--   0 christmas   (501) staff       (20)      426 2023-07-20 11:46:10.000000 baysalt_christmas-0.1.9.1/christmas/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.9.1/christmas/commonCode.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.9.1/christmas/cprintf.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-21 06:24:05.957055 baysalt_christmas-0.1.9.1/christmas/mncPy/
+-rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.9.1/christmas/mncPy/.gitignore
+-rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.9.1/christmas/mncPy/LICENSE
+-rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.9.1/christmas/mncPy/__init__.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-21 06:24:05.958026 baysalt_christmas-0.1.9.1/christmas/mncPy/__pycache__/
+-rw-r--r--   0 christmas   (501) staff       (20)      278 2023-07-20 07:12:00.000000 baysalt_christmas-0.1.9.1/christmas/mncPy/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.9.1/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.9.1/christmas/mncPy/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.9.1/christmas/mncPy/__pycache__/compress.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.9.1/christmas/mncPy/common.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.9.1/christmas/mncPy/compress.py
+-rw-r--r--   0 christmas   (501) staff       (20)     9260 2023-07-10 06:49:33.000000 baysalt_christmas-0.1.9.1/christmas/processBar.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3679 2023-06-12 03:11:04.000000 baysalt_christmas-0.1.9.1/christmas/read_conf.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.9.1/christmas/server_info.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-21 06:24:05.958757 baysalt_christmas-0.1.9.1/christmas/tools/
+-rw-r--r--   0 christmas   (501) staff       (20)      702 2023-07-20 11:46:10.000000 baysalt_christmas-0.1.9.1/christmas/tools/P_params.py
+-rw-r--r--   0 christmas   (501) staff       (20)      264 2023-07-20 11:57:28.000000 baysalt_christmas-0.1.9.1/christmas/tools/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3917 2023-07-20 11:58:23.000000 baysalt_christmas-0.1.9.1/christmas/tools/download_check.py
+-rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.9.1/run_twine.py
+-rw-r--r--   0 christmas   (501) staff       (20)       38 2023-07-21 06:24:05.959305 baysalt_christmas-0.1.9.1/setup.cfg
+-rw-r--r--   0 christmas   (501) staff       (20)      796 2023-07-21 05:26:50.000000 baysalt_christmas-0.1.9.1/setup.py
```

### Comparing `baysalt_christmas-0.1.9.0/.DS_Store` & `baysalt_christmas-0.1.9.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.9.0/PKG-INFO` & `baysalt_christmas-0.1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt_christmas
-Version: 0.1.9.0
+Version: 0.1.9.1
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.9.0/README.md` & `baysalt_christmas-0.1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.9.0/baysalt_christmas.egg-info/PKG-INFO` & `baysalt_christmas-0.1.9.1/baysalt_christmas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt-christmas
-Version: 0.1.9.0
+Version: 0.1.9.1
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.9.0/baysalt_christmas.egg-info/SOURCES.txt` & `baysalt_christmas-0.1.9.1/baysalt_christmas.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -19,10 +19,14 @@
 christmas/Pyshell/RS_File.py
 christmas/Pyshell/__init__.py
 christmas/mncPy/.gitignore
 christmas/mncPy/LICENSE
 christmas/mncPy/__init__.py
 christmas/mncPy/common.py
 christmas/mncPy/compress.py
+christmas/mncPy/__pycache__/__init__.cpython-311.pyc
 christmas/mncPy/__pycache__/__init__.cpython-39.pyc
 christmas/mncPy/__pycache__/common.cpython-39.pyc
-christmas/mncPy/__pycache__/compress.cpython-39.pyc
+christmas/mncPy/__pycache__/compress.cpython-39.pyc
+christmas/tools/P_params.py
+christmas/tools/__init__.py
+christmas/tools/download_check.py
```

### Comparing `baysalt_christmas-0.1.9.0/christmas/Blogging.py` & `baysalt_christmas-0.1.9.1/christmas/Blogging.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.9.0/christmas/Pyshell/RS_File.py` & `baysalt_christmas-0.1.9.1/christmas/Pyshell/RS_File.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.9.0/christmas/S_DateTime.py` & `baysalt_christmas-0.1.9.1/christmas/S_DateTime.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.9.0/christmas/commonCode.py` & `baysalt_christmas-0.1.9.1/christmas/commonCode.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.9.0/christmas/cprintf.py` & `baysalt_christmas-0.1.9.1/christmas/cprintf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.9.0/christmas/mncPy/.gitignore` & `baysalt_christmas-0.1.9.1/christmas/mncPy/.gitignore`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.9.0/christmas/mncPy/LICENSE` & `baysalt_christmas-0.1.9.1/christmas/mncPy/LICENSE`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.9.0/christmas/mncPy/__pycache__/common.cpython-39.pyc` & `baysalt_christmas-0.1.9.1/christmas/mncPy/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.9.0/christmas/mncPy/__pycache__/compress.cpython-39.pyc` & `baysalt_christmas-0.1.9.1/christmas/mncPy/__pycache__/compress.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.9.0/christmas/mncPy/common.py` & `baysalt_christmas-0.1.9.1/christmas/mncPy/common.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.9.0/christmas/mncPy/compress.py` & `baysalt_christmas-0.1.9.1/christmas/mncPy/compress.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.9.0/christmas/processBar.py` & `baysalt_christmas-0.1.9.1/christmas/processBar.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.9.0/christmas/read_conf.py` & `baysalt_christmas-0.1.9.1/christmas/read_conf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.9.0/christmas/server_info.py` & `baysalt_christmas-0.1.9.1/christmas/server_info.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.9.0/setup.py` & `baysalt_christmas-0.1.9.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="baysalt_christmas",
-    version="0.1.9.0",
+    version="0.1.9.1",
     author="Christmas",
     author_email="273519355@qq.com",
     description="Some simple tools for Christmas",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

