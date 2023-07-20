# Comparing `tmp/imagevaluec01-0.0.1.tar.gz` & `tmp/imagevaluec01-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imagevaluec01-0.0.1.tar", last modified: Thu Jul 20 21:39:02 2023, max compression
+gzip compressed data, was "imagevaluec01-0.0.2.tar", last modified: Thu Jul 20 22:00:58 2023, max compression
```

## Comparing `imagevaluec01-0.0.1.tar` & `imagevaluec01-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 21:39:02.852617 imagevaluec01-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-07-20 20:17:27.000000 imagevaluec01-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      626 2023-07-20 21:39:02.852617 imagevaluec01-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-07-20 20:16:36.000000 imagevaluec01-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 21:39:02.812259 imagevaluec01-0.0.1/imagevaluec01/
--rw-rw-rw-   0        0        0       38 2023-07-20 21:37:24.000000 imagevaluec01-0.0.1/imagevaluec01/__init__.py
--rw-rw-rw-   0        0        0     3683 2023-07-20 21:19:00.000000 imagevaluec01-0.0.1/imagevaluec01/imagevaluec01.py
-drwxrwxrwx   0        0        0        0 2023-07-20 21:39:02.850564 imagevaluec01-0.0.1/imagevaluec01.egg-info/
--rw-rw-rw-   0        0        0      626 2023-07-20 21:39:02.000000 imagevaluec01-0.0.1/imagevaluec01.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-07-20 21:39:02.000000 imagevaluec01-0.0.1/imagevaluec01.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 21:39:02.000000 imagevaluec01-0.0.1/imagevaluec01.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-20 21:39:02.000000 imagevaluec01-0.0.1/imagevaluec01.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 21:39:02.852617 imagevaluec01-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      930 2023-07-20 21:38:28.000000 imagevaluec01-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 22:00:58.149295 imagevaluec01-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-07-20 20:17:27.000000 imagevaluec01-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      626 2023-07-20 22:00:58.149295 imagevaluec01-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-07-20 20:16:36.000000 imagevaluec01-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 22:00:58.118093 imagevaluec01-0.0.2/imagevaluec01/
+-rw-rw-rw-   0        0        0        2 2023-07-20 22:00:49.000000 imagevaluec01-0.0.2/imagevaluec01/__init__.py
+-rw-rw-rw-   0        0        0     3683 2023-07-20 21:19:00.000000 imagevaluec01-0.0.2/imagevaluec01/imagevaluec01.py
+drwxrwxrwx   0        0        0        0 2023-07-20 22:00:58.133674 imagevaluec01-0.0.2/imagevaluec01.egg-info/
+-rw-rw-rw-   0        0        0      626 2023-07-20 22:00:58.000000 imagevaluec01-0.0.2/imagevaluec01.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-07-20 22:00:58.000000 imagevaluec01-0.0.2/imagevaluec01.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 22:00:58.000000 imagevaluec01-0.0.2/imagevaluec01.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-20 22:00:58.000000 imagevaluec01-0.0.2/imagevaluec01.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 22:00:58.149295 imagevaluec01-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      930 2023-07-20 21:58:35.000000 imagevaluec01-0.0.2/setup.py
```

### Comparing `imagevaluec01-0.0.1/LICENSE.txt` & `imagevaluec01-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `imagevaluec01-0.0.1/PKG-INFO` & `imagevaluec01-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imagevaluec01
-Version: 0.0.1
+Version: 0.0.2
 Summary: My first Python package
 Home-page: UNKNOWN
 Author: Kelvin Leong
 Author-email: <k.leong@chester.ac.uk>
 License: UNKNOWN
 Keywords: python,first package
 Platform: UNKNOWN
```

### Comparing `imagevaluec01-0.0.1/imagevaluec01/imagevaluec01.py` & `imagevaluec01-0.0.2/imagevaluec01/imagevaluec01.py`

 * *Files identical despite different names*

### Comparing `imagevaluec01-0.0.1/imagevaluec01.egg-info/PKG-INFO` & `imagevaluec01-0.0.2/imagevaluec01.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imagevaluec01
-Version: 0.0.1
+Version: 0.0.2
 Summary: My first Python package
 Home-page: UNKNOWN
 Author: Kelvin Leong
 Author-email: <k.leong@chester.ac.uk>
 License: UNKNOWN
 Keywords: python,first package
 Platform: UNKNOWN
```

### Comparing `imagevaluec01-0.0.1/setup.py` & `imagevaluec01-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = 'My first Python package'
 LONG_DESCRIPTION = 'My first Python package with a slightly longer description'
 
 
 setup(
         name="imagevaluec01", 
         version=VERSION,
```

