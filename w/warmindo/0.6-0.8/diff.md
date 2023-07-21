# Comparing `tmp/warmindo-0.6.tar.gz` & `tmp/warmindo-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warmindo-0.6.tar", last modified: Fri Jul 21 21:20:41 2023, max compression
+gzip compressed data, was "warmindo-0.8.tar", last modified: Fri Jul 21 21:23:08 2023, max compression
```

## Comparing `warmindo-0.6.tar` & `warmindo-0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 21:20:41.836101 warmindo-0.6/
--rw-rw-rw-   0        0        0      835 2023-07-21 21:20:41.835100 warmindo-0.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-21 21:20:41.836101 warmindo-0.6/setup.cfg
--rw-rw-rw-   0        0        0     1297 2023-07-21 20:44:18.000000 warmindo-0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 21:20:41.832100 warmindo-0.6/warmindo.egg-info/
--rw-rw-rw-   0        0        0      835 2023-07-21 21:20:41.000000 warmindo-0.6/warmindo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-07-21 21:20:41.000000 warmindo-0.6/warmindo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 21:20:41.000000 warmindo-0.6/warmindo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-21 21:20:41.000000 warmindo-0.6/warmindo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       73 2023-07-21 21:20:41.000000 warmindo-0.6/warmindo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 21:20:41.000000 warmindo-0.6/warmindo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 21:23:08.721260 warmindo-0.8/
+-rw-rw-rw-   0        0        0      835 2023-07-21 21:23:08.720262 warmindo-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-21 21:23:08.721260 warmindo-0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1297 2023-07-21 21:22:01.000000 warmindo-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:23:08.718255 warmindo-0.8/warmindo.egg-info/
+-rw-rw-rw-   0        0        0      835 2023-07-21 21:23:08.000000 warmindo-0.8/warmindo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-07-21 21:23:08.000000 warmindo-0.8/warmindo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 21:23:08.000000 warmindo-0.8/warmindo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-21 21:23:08.000000 warmindo-0.8/warmindo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       73 2023-07-21 21:23:08.000000 warmindo-0.8/warmindo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 21:23:08.000000 warmindo-0.8/warmindo.egg-info/top_level.txt
```

### Comparing `warmindo-0.6/PKG-INFO` & `warmindo-0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warmindo
-Version: 0.6
+Version: 0.8
 Summary: Framework Warmindo berbasis Python
 Home-page: https://github.com/adhamcahyo/warmindo
 Author: adham cahyo
 Author-email: arnolisarnol@gmail.com
 Project-URL: Source Code, https://github.com/adhamcahyo/warmindo
 Project-URL: Documentation, https://github.com/adhamcahyo/warmindo/docs
 Keywords: framework web warmindo python
```

### Comparing `warmindo-0.6/setup.py` & `warmindo-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='warmindo',
-    version='0.6', 
+    version='0.8', 
     packages=find_packages(),
     install_requires=[
         'SQLAlchemy',
         'Flask',
         'mysql-connector-python',
         'scikit-learn',
         'python-telegram-bot',
```

### Comparing `warmindo-0.6/warmindo.egg-info/PKG-INFO` & `warmindo-0.8/warmindo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warmindo
-Version: 0.6
+Version: 0.8
 Summary: Framework Warmindo berbasis Python
 Home-page: https://github.com/adhamcahyo/warmindo
 Author: adham cahyo
 Author-email: arnolisarnol@gmail.com
 Project-URL: Source Code, https://github.com/adhamcahyo/warmindo
 Project-URL: Documentation, https://github.com/adhamcahyo/warmindo/docs
 Keywords: framework web warmindo python
```

