# Comparing `tmp/warmindo-0.1.tar.gz` & `tmp/warmindo-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warmindo-0.1.tar", last modified: Fri Jul 21 19:11:36 2023, max compression
+gzip compressed data, was "warmindo-0.2.tar", last modified: Fri Jul 21 20:09:32 2023, max compression
```

## Comparing `warmindo-0.1.tar` & `warmindo-0.2.tar`

### file list

```diff
@@ -1,32 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 19:11:36.214719 warmindo-0.1/
--rw-rw-rw-   0        0        0      775 2023-07-21 19:11:36.213722 warmindo-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-21 19:11:36.015451 warmindo-0.1/config/
--rw-rw-rw-   0        0        0        0 2023-07-21 18:36:33.000000 warmindo-0.1/config/__init__.py
--rw-rw-rw-   0        0        0       64 2023-07-21 18:55:02.000000 warmindo-0.1/config/api_config.py
--rw-rw-rw-   0        0        0      134 2023-07-21 18:58:37.000000 warmindo-0.1/config/database_config.py
-drwxrwxrwx   0        0        0        0 2023-07-21 19:11:36.034469 warmindo-0.1/core/
--rw-rw-rw-   0        0        0        0 2023-07-21 18:28:25.000000 warmindo-0.1/core/__init__.py
--rw-rw-rw-   0        0        0      457 2023-07-21 18:57:46.000000 warmindo-0.1/core/app.py
--rw-rw-rw-   0        0        0       43 2023-07-21 18:59:13.000000 warmindo-0.1/core/exceptions.py
--rw-rw-rw-   0        0        0      201 2023-07-21 18:56:33.000000 warmindo-0.1/core/middleware.py
--rw-rw-rw-   0        0        0        0 2023-07-21 18:29:58.000000 warmindo-0.1/core/request_manager.py
--rw-rw-rw-   0        0        0      260 2023-07-21 18:56:10.000000 warmindo-0.1/core/response.py
--rw-rw-rw-   0        0        0        0 2023-07-21 18:28:37.000000 warmindo-0.1/core/routing.py
--rw-rw-rw-   0        0        0       42 2023-07-21 19:11:36.214719 warmindo-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1130 2023-07-21 18:44:27.000000 warmindo-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 19:11:36.150714 warmindo-0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-07-21 18:36:57.000000 warmindo-0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     1092 2023-07-21 18:58:53.000000 warmindo-0.1/tests/test_database.py
--rw-rw-rw-   0        0        0        0 2023-07-21 18:37:04.000000 warmindo-0.1/tests/test_middleware.py
--rw-rw-rw-   0        0        0        0 2023-07-21 18:37:01.000000 warmindo-0.1/tests/test_routing.py
-drwxrwxrwx   0        0        0        0 2023-07-21 19:11:36.157715 warmindo-0.1/utils/
--rw-rw-rw-   0        0        0        0 2023-07-21 18:39:01.000000 warmindo-0.1/utils/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-21 18:39:04.000000 warmindo-0.1/utils/helpers.py
--rw-rw-rw-   0        0        0      543 2023-07-21 19:02:19.000000 warmindo-0.1/utils/validators.py
-drwxrwxrwx   0        0        0        0 2023-07-21 19:11:36.211720 warmindo-0.1/warmindo.egg-info/
--rw-rw-rw-   0        0        0      775 2023-07-21 19:11:35.000000 warmindo-0.1/warmindo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2023-07-21 19:11:35.000000 warmindo-0.1/warmindo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 19:11:35.000000 warmindo-0.1/warmindo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-07-21 19:11:35.000000 warmindo-0.1/warmindo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-21 19:11:35.000000 warmindo-0.1/warmindo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-07-21 19:11:35.000000 warmindo-0.1/warmindo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 20:09:32.930189 warmindo-0.2/
+-rw-rw-rw-   0        0        0      775 2023-07-21 20:09:32.929176 warmindo-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-21 20:09:32.930189 warmindo-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2023-07-21 19:50:09.000000 warmindo-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:09:32.927190 warmindo-0.2/warmindo.egg-info/
+-rw-rw-rw-   0        0        0      775 2023-07-21 20:09:32.000000 warmindo-0.2/warmindo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-07-21 20:09:32.000000 warmindo-0.2/warmindo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 20:09:32.000000 warmindo-0.2/warmindo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-21 20:09:32.000000 warmindo-0.2/warmindo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       73 2023-07-21 20:09:32.000000 warmindo-0.2/warmindo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 20:09:32.000000 warmindo-0.2/warmindo.egg-info/top_level.txt
```

### Comparing `warmindo-0.1/PKG-INFO` & `warmindo-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warmindo
-Version: 0.1
+Version: 0.2
 Summary: Framework Warmindo berbasis Python
 Home-page: https://github.com/adhamcahyo/warmindo
 Author: adham cahyo
 Author-email: email@anda.com
 Project-URL: Source Code, https://github.com/adhamcahyo/warmindo
 Project-URL: Documentation, https://github.com/adhamcahyo/warmindo/docs
 Keywords: framework web warmindo python
```

### Comparing `warmindo-0.1/setup.py` & `warmindo-0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='warmindo',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     install_requires=[
-        'SQLAlchemy',  
-        'Flask',       
+    'SQLAlchemy',
+    'Flask',
+    'mysql-connector-python',
+    'scikit-learn',           
+    'python-telegram-bot',     
     ],
     entry_points={
         'console_scripts': [
             'runserve = warmindo.server:main'
         ]
     },
     author='adham cahyo',
```

### Comparing `warmindo-0.1/warmindo.egg-info/PKG-INFO` & `warmindo-0.2/warmindo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warmindo
-Version: 0.1
+Version: 0.2
 Summary: Framework Warmindo berbasis Python
 Home-page: https://github.com/adhamcahyo/warmindo
 Author: adham cahyo
 Author-email: email@anda.com
 Project-URL: Source Code, https://github.com/adhamcahyo/warmindo
 Project-URL: Documentation, https://github.com/adhamcahyo/warmindo/docs
 Keywords: framework web warmindo python
```

