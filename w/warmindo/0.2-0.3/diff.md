# Comparing `tmp/warmindo-0.2.tar.gz` & `tmp/warmindo-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warmindo-0.2.tar", last modified: Fri Jul 21 20:09:32 2023, max compression
+gzip compressed data, was "warmindo-0.3.tar", last modified: Fri Jul 21 20:18:41 2023, max compression
```

## Comparing `warmindo-0.2.tar` & `warmindo-0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 20:09:32.930189 warmindo-0.2/
--rw-rw-rw-   0        0        0      775 2023-07-21 20:09:32.929176 warmindo-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-21 20:09:32.930189 warmindo-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1209 2023-07-21 19:50:09.000000 warmindo-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 20:09:32.927190 warmindo-0.2/warmindo.egg-info/
--rw-rw-rw-   0        0        0      775 2023-07-21 20:09:32.000000 warmindo-0.2/warmindo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-07-21 20:09:32.000000 warmindo-0.2/warmindo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 20:09:32.000000 warmindo-0.2/warmindo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-07-21 20:09:32.000000 warmindo-0.2/warmindo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       73 2023-07-21 20:09:32.000000 warmindo-0.2/warmindo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 20:09:32.000000 warmindo-0.2/warmindo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 20:18:41.686474 warmindo-0.3/
+-rw-rw-rw-   0        0        0      783 2023-07-21 20:18:41.685474 warmindo-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-21 20:18:41.686474 warmindo-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1203 2023-07-21 20:18:32.000000 warmindo-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:18:41.683483 warmindo-0.3/warmindo.egg-info/
+-rw-rw-rw-   0        0        0      783 2023-07-21 20:18:41.000000 warmindo-0.3/warmindo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-07-21 20:18:41.000000 warmindo-0.3/warmindo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 20:18:41.000000 warmindo-0.3/warmindo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-21 20:18:41.000000 warmindo-0.3/warmindo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       73 2023-07-21 20:18:41.000000 warmindo-0.3/warmindo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 20:18:41.000000 warmindo-0.3/warmindo.egg-info/top_level.txt
```

### Comparing `warmindo-0.2/PKG-INFO` & `warmindo-0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: warmindo
-Version: 0.2
+Version: 0.3
 Summary: Framework Warmindo berbasis Python
 Home-page: https://github.com/adhamcahyo/warmindo
 Author: adham cahyo
-Author-email: email@anda.com
+Author-email: arnolisarnol@gmail.com
 Project-URL: Source Code, https://github.com/adhamcahyo/warmindo
 Project-URL: Documentation, https://github.com/adhamcahyo/warmindo/docs
 Keywords: framework web warmindo python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `warmindo-0.2/setup.py` & `warmindo-0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
     name='warmindo',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     install_requires=[
     'SQLAlchemy',
     'Flask',
     'mysql-connector-python',
     'scikit-learn',           
     'python-telegram-bot',     
     ],
     entry_points={
         'console_scripts': [
-            'runserve = warmindo.server:main'
+            'warmindo=gas:main'
         ]
     },
     author='adham cahyo',
-    author_email='email@anda.com',
+    author_email='arnolisarnol@gmail.com',
     description='Framework Warmindo berbasis Python',
     url='https://github.com/adhamcahyo/warmindo',  
     project_urls={
         'Source Code': 'https://github.com/adhamcahyo/warmindo',
         'Documentation': 'https://github.com/adhamcahyo/warmindo/docs',  
     },
     classifiers=[
```

### Comparing `warmindo-0.2/warmindo.egg-info/PKG-INFO` & `warmindo-0.3/warmindo.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: warmindo
-Version: 0.2
+Version: 0.3
 Summary: Framework Warmindo berbasis Python
 Home-page: https://github.com/adhamcahyo/warmindo
 Author: adham cahyo
-Author-email: email@anda.com
+Author-email: arnolisarnol@gmail.com
 Project-URL: Source Code, https://github.com/adhamcahyo/warmindo
 Project-URL: Documentation, https://github.com/adhamcahyo/warmindo/docs
 Keywords: framework web warmindo python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

