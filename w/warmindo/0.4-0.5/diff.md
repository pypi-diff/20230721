# Comparing `tmp/warmindo-0.4.tar.gz` & `tmp/warmindo-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warmindo-0.4.tar", last modified: Fri Jul 21 20:27:55 2023, max compression
+gzip compressed data, was "warmindo-0.5.tar", last modified: Fri Jul 21 20:35:31 2023, max compression
```

## Comparing `warmindo-0.4.tar` & `warmindo-0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 20:27:55.954700 warmindo-0.4/
--rw-rw-rw-   0        0        0      783 2023-07-21 20:27:55.953695 warmindo-0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-21 20:27:55.954700 warmindo-0.4/setup.cfg
--rw-rw-rw-   0        0        0     1270 2023-07-21 20:26:58.000000 warmindo-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 20:27:55.950693 warmindo-0.4/warmindo.egg-info/
--rw-rw-rw-   0        0        0      783 2023-07-21 20:27:55.000000 warmindo-0.4/warmindo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-07-21 20:27:55.000000 warmindo-0.4/warmindo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 20:27:55.000000 warmindo-0.4/warmindo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-21 20:27:55.000000 warmindo-0.4/warmindo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       73 2023-07-21 20:27:55.000000 warmindo-0.4/warmindo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 20:27:55.000000 warmindo-0.4/warmindo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 20:35:31.143073 warmindo-0.5/
+-rw-rw-rw-   0        0        0      835 2023-07-21 20:35:31.142076 warmindo-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-21 20:35:31.143073 warmindo-0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1297 2023-07-21 20:33:21.000000 warmindo-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:35:31.141075 warmindo-0.5/warmindo.egg-info/
+-rw-rw-rw-   0        0        0      835 2023-07-21 20:35:31.000000 warmindo-0.5/warmindo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-07-21 20:35:31.000000 warmindo-0.5/warmindo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 20:35:31.000000 warmindo-0.5/warmindo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-21 20:35:31.000000 warmindo-0.5/warmindo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       73 2023-07-21 20:35:31.000000 warmindo-0.5/warmindo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 20:35:31.000000 warmindo-0.5/warmindo.egg-info/top_level.txt
```

### Comparing `warmindo-0.4/PKG-INFO` & `warmindo-0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warmindo
-Version: 0.4
+Version: 0.5
 Summary: Framework Warmindo berbasis Python
 Home-page: https://github.com/adhamcahyo/warmindo
 Author: adham cahyo
 Author-email: arnolisarnol@gmail.com
 Project-URL: Source Code, https://github.com/adhamcahyo/warmindo
 Project-URL: Documentation, https://github.com/adhamcahyo/warmindo/docs
 Keywords: framework web warmindo python
@@ -12,7 +12,8 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
```

### Comparing `warmindo-0.4/setup.py` & `warmindo-0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='warmindo',
-    version='0.4',  # Perbarui nomor versi menjadi 0.4 atau versi yang lebih baru
+    version='0.5', 
     packages=find_packages(),
     install_requires=[
         'SQLAlchemy',
         'Flask',
         'mysql-connector-python',
         'scikit-learn',
         'python-telegram-bot',
@@ -29,10 +29,12 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        # SUPPORT PYTHON 3.11 su311
+        'Programming Language :: Python :: 3.11', 
     ],
     keywords='framework web warmindo python',
 )
```

### Comparing `warmindo-0.4/warmindo.egg-info/PKG-INFO` & `warmindo-0.5/warmindo.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warmindo
-Version: 0.4
+Version: 0.5
 Summary: Framework Warmindo berbasis Python
 Home-page: https://github.com/adhamcahyo/warmindo
 Author: adham cahyo
 Author-email: arnolisarnol@gmail.com
 Project-URL: Source Code, https://github.com/adhamcahyo/warmindo
 Project-URL: Documentation, https://github.com/adhamcahyo/warmindo/docs
 Keywords: framework web warmindo python
@@ -12,7 +12,8 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
```

