# Comparing `tmp/responsecurve-0.0.7.tar.gz` & `tmp/responsecurve-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "responsecurve-0.0.7.tar", last modified: Thu Jul 20 22:41:46 2023, max compression
+gzip compressed data, was "responsecurve-0.0.8.tar", last modified: Thu Jul 20 22:58:39 2023, max compression
```

## Comparing `responsecurve-0.0.7.tar` & `responsecurve-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-20 22:41:46.534032 responsecurve-0.0.7/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1163 2023-07-20 18:34:56.000000 responsecurve-0.0.7/LICENSE
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    13733 2023-07-20 22:41:46.532809 responsecurve-0.0.7/PKG-INFO
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    13475 2023-07-20 22:41:01.000000 responsecurve-0.0.7/README.md
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-20 22:41:46.530709 responsecurve-0.0.7/responsecurve.egg-info/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    13733 2023-07-20 22:41:46.000000 responsecurve-0.0.7/responsecurve.egg-info/PKG-INFO
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      210 2023-07-20 22:41:46.000000 responsecurve-0.0.7/responsecurve.egg-info/SOURCES.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-20 22:41:46.000000 responsecurve-0.0.7/responsecurve.egg-info/dependency_links.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       43 2023-07-20 22:41:46.000000 responsecurve-0.0.7/responsecurve.egg-info/requires.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-20 22:41:46.000000 responsecurve-0.0.7/responsecurve.egg-info/top_level.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-20 22:41:46.534407 responsecurve-0.0.7/setup.cfg
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      572 2023-07-20 22:41:39.000000 responsecurve-0.0.7/setup.py
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-20 22:58:39.188336 responsecurve-0.0.8/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1163 2023-07-20 18:34:56.000000 responsecurve-0.0.8/LICENSE
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    13787 2023-07-20 22:58:39.187548 responsecurve-0.0.8/PKG-INFO
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    13475 2023-07-20 22:49:19.000000 responsecurve-0.0.8/README.md
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-20 22:58:39.186572 responsecurve-0.0.8/responsecurve.egg-info/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    13787 2023-07-20 22:58:39.000000 responsecurve-0.0.8/responsecurve.egg-info/PKG-INFO
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      210 2023-07-20 22:58:39.000000 responsecurve-0.0.8/responsecurve.egg-info/SOURCES.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-20 22:58:39.000000 responsecurve-0.0.8/responsecurve.egg-info/dependency_links.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       43 2023-07-20 22:58:39.000000 responsecurve-0.0.8/responsecurve.egg-info/requires.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-20 22:58:39.000000 responsecurve-0.0.8/responsecurve.egg-info/top_level.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-20 22:58:39.188534 responsecurve-0.0.8/setup.cfg
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      626 2023-07-20 22:58:31.000000 responsecurve-0.0.8/setup.py
```

### Comparing `responsecurve-0.0.7/LICENSE` & `responsecurve-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `responsecurve-0.0.7/PKG-INFO` & `responsecurve-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: responsecurve
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library for detecting response curves in time series data.
+Home-page: https://github.com/himanalot/ResponseCurve
 Author: Ishan Ramrakhiani
 Author-email: ishanramrakhiani@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ResponseCurve.py
```

### Comparing `responsecurve-0.0.7/README.md` & `responsecurve-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `responsecurve-0.0.7/responsecurve.egg-info/PKG-INFO` & `responsecurve-0.0.8/responsecurve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: responsecurve
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library for detecting response curves in time series data.
+Home-page: https://github.com/himanalot/ResponseCurve
 Author: Ishan Ramrakhiani
 Author-email: ishanramrakhiani@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ResponseCurve.py
```

### Comparing `responsecurve-0.0.7/setup.py` & `responsecurve-0.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='responsecurve',
-    version='0.0.7',
+    version='0.0.8',
     packages=find_packages(),
     install_requires=[
         'pandas',
         'numpy',
         'scipy',
         'matplotlib',
         'scikit-learn'
     ],
     author='Ishan Ramrakhiani',
     author_email='ishanramrakhiani@gmail.com',
     description='A library for detecting response curves in time series data.',
     long_description=long_description,
-    long_description_content_type='text/markdown'
+    long_description_content_type='text/markdown',
+    url='https://github.com/himanalot/ResponseCurve'
 )
```

