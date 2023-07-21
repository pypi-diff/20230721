# Comparing `tmp/buscador-0.8.tar.gz` & `tmp/buscador-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buscador-0.8.tar", last modified: Fri Jul 21 09:38:25 2023, max compression
+gzip compressed data, was "buscador-0.9.tar", last modified: Fri Jul 21 09:45:00 2023, max compression
```

## Comparing `buscador-0.8.tar` & `buscador-0.9.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-21 09:38:25.782791 buscador-0.8/
--rw-r--r--   0 samcook    (501) staff       (20)     1068 2023-07-19 21:01:14.000000 buscador-0.8/LICENSE.txt
--rw-r--r--   0 samcook    (501) staff       (20)      739 2023-07-21 09:38:25.783177 buscador-0.8/PKG-INFO
--rw-r--r--   0 samcook    (501) staff       (20)      760 2023-07-21 08:23:09.000000 buscador-0.8/README.md
-drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-21 09:38:25.777616 buscador-0.8/buscador/
--rw-r--r--   0 samcook    (501) staff       (20)      969 2023-07-21 08:22:56.000000 buscador-0.8/buscador/JsonStuff.py
--rw-r--r--   0 samcook    (501) staff       (20)     3019 2023-07-21 08:22:56.000000 buscador-0.8/buscador/S3Stuff.py
--rw-r--r--   0 samcook    (501) staff       (20)      142 2023-07-21 09:36:00.000000 buscador-0.8/buscador/__init__.py
-drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-21 09:38:25.781799 buscador-0.8/buscador.egg-info/
--rw-r--r--   0 samcook    (501) staff       (20)      739 2023-07-21 09:38:25.000000 buscador-0.8/buscador.egg-info/PKG-INFO
--rw-r--r--   0 samcook    (501) staff       (20)      262 2023-07-21 09:38:25.000000 buscador-0.8/buscador.egg-info/SOURCES.txt
--rw-r--r--   0 samcook    (501) staff       (20)        1 2023-07-21 09:38:25.000000 buscador-0.8/buscador.egg-info/dependency_links.txt
--rw-r--r--   0 samcook    (501) staff       (20)       25 2023-07-21 09:38:25.000000 buscador-0.8/buscador.egg-info/requires.txt
--rw-r--r--   0 samcook    (501) staff       (20)        9 2023-07-21 09:38:25.000000 buscador-0.8/buscador.egg-info/top_level.txt
--rw-r--r--   0 samcook    (501) staff       (20)       79 2023-07-21 09:38:25.784105 buscador-0.8/setup.cfg
--rw-r--r--   0 samcook    (501) staff       (20)      998 2023-07-21 09:37:46.000000 buscador-0.8/setup.py
+drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-21 09:45:00.816653 buscador-0.9/
+-rw-r--r--   0 samcook    (501) staff       (20)     1068 2023-07-19 21:01:14.000000 buscador-0.9/LICENSE.txt
+-rw-r--r--   0 samcook    (501) staff       (20)      739 2023-07-21 09:45:00.816953 buscador-0.9/PKG-INFO
+-rw-r--r--   0 samcook    (501) staff       (20)      761 2023-07-21 09:44:56.000000 buscador-0.9/README.md
+drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-21 09:45:00.810772 buscador-0.9/buscador/
+-rw-r--r--   0 samcook    (501) staff       (20)      147 2023-07-21 09:42:07.000000 buscador-0.9/buscador/__init__.py
+-rw-r--r--   0 samcook    (501) staff       (20)     3621 2023-07-21 09:41:55.000000 buscador-0.9/buscador/functions.py
+drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-21 09:45:00.816129 buscador-0.9/buscador.egg-info/
+-rw-r--r--   0 samcook    (501) staff       (20)      739 2023-07-21 09:45:00.000000 buscador-0.9/buscador.egg-info/PKG-INFO
+-rw-r--r--   0 samcook    (501) staff       (20)      242 2023-07-21 09:45:00.000000 buscador-0.9/buscador.egg-info/SOURCES.txt
+-rw-r--r--   0 samcook    (501) staff       (20)        1 2023-07-21 09:45:00.000000 buscador-0.9/buscador.egg-info/dependency_links.txt
+-rw-r--r--   0 samcook    (501) staff       (20)       25 2023-07-21 09:45:00.000000 buscador-0.9/buscador.egg-info/requires.txt
+-rw-r--r--   0 samcook    (501) staff       (20)        9 2023-07-21 09:45:00.000000 buscador-0.9/buscador.egg-info/top_level.txt
+-rw-r--r--   0 samcook    (501) staff       (20)       79 2023-07-21 09:45:00.817688 buscador-0.9/setup.cfg
+-rw-r--r--   0 samcook    (501) staff       (20)      998 2023-07-21 09:44:34.000000 buscador-0.9/setup.py
```

### Comparing `buscador-0.8/LICENSE.txt` & `buscador-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buscador-0.8/PKG-INFO` & `buscador-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: buscador
-Version: 0.8
+Version: 0.9
 Summary: Just a collection of helpful tools
 Home-page: https://github.com/SamuelBCook
-Download-URL: https://github.com/SamuelBCook/buscador/archive/refs/tags/v0.8.tar.gz
+Download-URL: https://github.com/SamuelBCook/buscador/archive/refs/tags/v0.9.tar.gz
 Author: Samuel Cook
 Author-email: samcook23@hotmail.com
 License: MIT
 Keywords: tools,json,easy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `buscador-0.8/README.md` & `buscador-0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,12 +5,12 @@
 https://medium.com/@joel.barmettler/how-to-upload-your-python-package-to-pypi-65edc5fe9c56
 
 https://dillinger.io
 
 New Version*
 . Simply upload your new code to github, create a new release, then adapt the setup.py file (new download_url — according to your new release tag, new version), then run the setup.py and the twin command again (navigate to your folder first!)
 
-- python setup.py sdist
+- python3 setup.py sdist
 - twine upload dist/*
 
 or if Vs already exist 
 - twine upload --skip-existing dist/*
```

### Comparing `buscador-0.8/buscador.egg-info/PKG-INFO` & `buscador-0.9/buscador.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: buscador
-Version: 0.8
+Version: 0.9
 Summary: Just a collection of helpful tools
 Home-page: https://github.com/SamuelBCook
-Download-URL: https://github.com/SamuelBCook/buscador/archive/refs/tags/v0.8.tar.gz
+Download-URL: https://github.com/SamuelBCook/buscador/archive/refs/tags/v0.9.tar.gz
 Author: Samuel Cook
 Author-email: samcook23@hotmail.com
 License: MIT
 Keywords: tools,json,easy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `buscador-0.8/setup.py` & `buscador-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
     name="buscador",
     packages=["buscador"],
-    version="0.8",
+    version="0.9",
     license="MIT",
     description="Just a collection of helpful tools",
     author="Samuel Cook",
     author_email="samcook23@hotmail.com",
     url="https://github.com/SamuelBCook",
-    download_url="https://github.com/SamuelBCook/buscador/archive/refs/tags/v0.8.tar.gz",
+    download_url="https://github.com/SamuelBCook/buscador/archive/refs/tags/v0.9.tar.gz",
     keywords=["tools", "json", "easy"],
     install_requires=[
         "pandas",
         "boto3",
         "botocore",
         "io",
     ],
```

