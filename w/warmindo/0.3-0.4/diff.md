# Comparing `tmp/warmindo-0.3.tar.gz` & `tmp/warmindo-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warmindo-0.3.tar", last modified: Fri Jul 21 20:18:41 2023, max compression
+gzip compressed data, was "warmindo-0.4.tar", last modified: Fri Jul 21 20:27:55 2023, max compression
```

## Comparing `warmindo-0.3.tar` & `warmindo-0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 20:18:41.686474 warmindo-0.3/
--rw-rw-rw-   0        0        0      783 2023-07-21 20:18:41.685474 warmindo-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-21 20:18:41.686474 warmindo-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1203 2023-07-21 20:18:32.000000 warmindo-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 20:18:41.683483 warmindo-0.3/warmindo.egg-info/
--rw-rw-rw-   0        0        0      783 2023-07-21 20:18:41.000000 warmindo-0.3/warmindo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-07-21 20:18:41.000000 warmindo-0.3/warmindo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 20:18:41.000000 warmindo-0.3/warmindo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-21 20:18:41.000000 warmindo-0.3/warmindo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       73 2023-07-21 20:18:41.000000 warmindo-0.3/warmindo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 20:18:41.000000 warmindo-0.3/warmindo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 20:27:55.954700 warmindo-0.4/
+-rw-rw-rw-   0        0        0      783 2023-07-21 20:27:55.953695 warmindo-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-21 20:27:55.954700 warmindo-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1270 2023-07-21 20:26:58.000000 warmindo-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:27:55.950693 warmindo-0.4/warmindo.egg-info/
+-rw-rw-rw-   0        0        0      783 2023-07-21 20:27:55.000000 warmindo-0.4/warmindo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-07-21 20:27:55.000000 warmindo-0.4/warmindo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 20:27:55.000000 warmindo-0.4/warmindo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-21 20:27:55.000000 warmindo-0.4/warmindo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       73 2023-07-21 20:27:55.000000 warmindo-0.4/warmindo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 20:27:55.000000 warmindo-0.4/warmindo.egg-info/top_level.txt
```

### Comparing `warmindo-0.3/PKG-INFO` & `warmindo-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warmindo
-Version: 0.3
+Version: 0.4
 Summary: Framework Warmindo berbasis Python
 Home-page: https://github.com/adhamcahyo/warmindo
 Author: adham cahyo
 Author-email: arnolisarnol@gmail.com
 Project-URL: Source Code, https://github.com/adhamcahyo/warmindo
 Project-URL: Documentation, https://github.com/adhamcahyo/warmindo/docs
 Keywords: framework web warmindo python
```

### Comparing `warmindo-0.3/setup.py` & `warmindo-0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='warmindo',
-    version='0.3',
+    version='0.4',  # Perbarui nomor versi menjadi 0.4 atau versi yang lebih baru
     packages=find_packages(),
     install_requires=[
-    'SQLAlchemy',
-    'Flask',
-    'mysql-connector-python',
-    'scikit-learn',           
-    'python-telegram-bot',     
+        'SQLAlchemy',
+        'Flask',
+        'mysql-connector-python',
+        'scikit-learn',
+        'python-telegram-bot',
     ],
     entry_points={
         'console_scripts': [
             'warmindo=gas:main'
         ]
     },
     author='adham cahyo',
```

### Comparing `warmindo-0.3/warmindo.egg-info/PKG-INFO` & `warmindo-0.4/warmindo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warmindo
-Version: 0.3
+Version: 0.4
 Summary: Framework Warmindo berbasis Python
 Home-page: https://github.com/adhamcahyo/warmindo
 Author: adham cahyo
 Author-email: arnolisarnol@gmail.com
 Project-URL: Source Code, https://github.com/adhamcahyo/warmindo
 Project-URL: Documentation, https://github.com/adhamcahyo/warmindo/docs
 Keywords: framework web warmindo python
```

