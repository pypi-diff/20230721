# Comparing `tmp/tinyimagenet-0.5.tar.gz` & `tmp/tinyimagenet-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyimagenet-0.5.tar", last modified: Tue Jul 11 15:27:28 2023, max compression
+gzip compressed data, was "tinyimagenet-0.6.tar", last modified: Fri Jul 21 02:54:51 2023, max compression
```

## Comparing `tinyimagenet-0.5.tar` & `tinyimagenet-0.6.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 facundoq  (1000) facundoq  (1000)        0 2023-07-11 15:27:28.845934 tinyimagenet-0.5/
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1072 2023-07-11 14:47:13.000000 tinyimagenet-0.5/LICENSE
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1665 2023-07-11 15:27:28.841934 tinyimagenet-0.5/PKG-INFO
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)      789 2023-07-11 15:17:51.000000 tinyimagenet-0.5/README.md
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       38 2023-07-11 15:27:28.845934 tinyimagenet-0.5/setup.cfg
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     2943 2023-07-11 15:27:16.000000 tinyimagenet-0.5/setup.py
-drwxrwxr-x   0 facundoq  (1000) facundoq  (1000)        0 2023-07-11 15:27:28.841934 tinyimagenet-0.5/tinyimagenet.egg-info/
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1665 2023-07-11 15:27:28.000000 tinyimagenet-0.5/tinyimagenet.egg-info/PKG-INFO
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)      252 2023-07-11 15:27:28.000000 tinyimagenet-0.5/tinyimagenet.egg-info/SOURCES.txt
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)        1 2023-07-11 15:27:28.000000 tinyimagenet-0.5/tinyimagenet.egg-info/dependency_links.txt
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       12 2023-07-11 15:27:28.000000 tinyimagenet-0.5/tinyimagenet.egg-info/requires.txt
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       13 2023-07-11 15:27:28.000000 tinyimagenet-0.5/tinyimagenet.egg-info/top_level.txt
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)        1 2023-07-11 15:16:03.000000 tinyimagenet-0.5/tinyimagenet.egg-info/zip-safe
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     6235 2023-07-11 15:24:55.000000 tinyimagenet-0.5/tinyimagenet.py
+drwxrwxr-x   0 facundoq  (1000) facundoq  (1000)        0 2023-07-21 02:54:51.549855 tinyimagenet-0.6/
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1072 2023-07-11 14:47:13.000000 tinyimagenet-0.6/LICENSE
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1665 2023-07-21 02:54:51.549855 tinyimagenet-0.6/PKG-INFO
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)      789 2023-07-11 15:17:51.000000 tinyimagenet-0.6/README.md
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)    13085 2023-07-11 15:24:08.000000 tinyimagenet-0.6/imagenet1k.py
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       38 2023-07-21 02:54:51.549855 tinyimagenet-0.6/setup.cfg
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     2964 2023-07-21 02:54:24.000000 tinyimagenet-0.6/setup.py
+drwxrwxr-x   0 facundoq  (1000) facundoq  (1000)        0 2023-07-21 02:54:51.549855 tinyimagenet-0.6/tinyimagenet.egg-info/
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1665 2023-07-21 02:54:51.000000 tinyimagenet-0.6/tinyimagenet.egg-info/PKG-INFO
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)      266 2023-07-21 02:54:51.000000 tinyimagenet-0.6/tinyimagenet.egg-info/SOURCES.txt
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)        1 2023-07-21 02:54:51.000000 tinyimagenet-0.6/tinyimagenet.egg-info/dependency_links.txt
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       12 2023-07-21 02:54:51.000000 tinyimagenet-0.6/tinyimagenet.egg-info/requires.txt
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       24 2023-07-21 02:54:51.000000 tinyimagenet-0.6/tinyimagenet.egg-info/top_level.txt
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)        1 2023-07-11 15:16:03.000000 tinyimagenet-0.6/tinyimagenet.egg-info/zip-safe
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     6235 2023-07-11 15:24:55.000000 tinyimagenet-0.6/tinyimagenet.py
```

### Comparing `tinyimagenet-0.5/LICENSE` & `tinyimagenet-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyimagenet-0.5/PKG-INFO` & `tinyimagenet-0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyimagenet
-Version: 0.5
+Version: 0.6
 Summary: Dataset class for PyTorch and the TinyImageNet dataset, with automated download and extraction.
 Home-page: https://github.com/facundoq/tinyimagenet
 Author: Facundo Manuel Quiroga
 Author-email: facundoq@gmail.com
 Project-URL: Bug Tracker, https://github.com/facundoq/tinyimagenet/issues
 Project-URL: Documentation, https://github.com/facundoq/tinyimagenet
 Project-URL: Source Code, https://github.com/facundoq/tinyimagenet
```

### Comparing `tinyimagenet-0.5/README.md` & `tinyimagenet-0.6/README.md`

 * *Files identical despite different names*

### Comparing `tinyimagenet-0.5/setup.py` & `tinyimagenet-0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 url="https://github.com/facundoq/tinyimagenet"
-VERSION="0.5"
+VERSION="0.6"
 
 class UploadCommand(Command):
     """Support setup.py upload."""
 
     description = 'Build and publish the package.'
     user_options = []
 
@@ -61,19 +61,19 @@
 
     # Project uses reStructuredText, so ensure that the docutils get
     # installed or upgraded on the target machine
     install_requires=[
         "torchvision",
 
     ],
-    py_modules=['tinyimagenet'],
+    py_modules=['tinyimagenet',"imagenet1k"],
 
     package_data={
         # If any package contains *.txt or *.rst files, include them:
-        "": ["*.txt", "*.rst"],
+        "": ["*.txt", "*.rst","*.csv"],
         # And include any *.msg files found in the "hello" package, too:
         "hello": ["*.msg"],
     },
     zip_safe=True,
     # metadata to display on PyPI
     author="Facundo Manuel Quiroga",
     author_email="facundoq@gmail.com",
```

### Comparing `tinyimagenet-0.5/tinyimagenet.egg-info/PKG-INFO` & `tinyimagenet-0.6/tinyimagenet.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyimagenet
-Version: 0.5
+Version: 0.6
 Summary: Dataset class for PyTorch and the TinyImageNet dataset, with automated download and extraction.
 Home-page: https://github.com/facundoq/tinyimagenet
 Author: Facundo Manuel Quiroga
 Author-email: facundoq@gmail.com
 Project-URL: Bug Tracker, https://github.com/facundoq/tinyimagenet/issues
 Project-URL: Documentation, https://github.com/facundoq/tinyimagenet
 Project-URL: Source Code, https://github.com/facundoq/tinyimagenet
```

### Comparing `tinyimagenet-0.5/tinyimagenet.py` & `tinyimagenet-0.6/tinyimagenet.py`

 * *Files identical despite different names*

