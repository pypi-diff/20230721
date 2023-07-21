# Comparing `tmp/sonnenbatterie-0.1.1.tar.gz` & `tmp/sonnenbatterie-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sonnenbatterie-0.1.1.tar", last modified: Wed Apr  1 07:23:59 2020, max compression
+gzip compressed data, was "sonnenbatterie-0.2.0.tar", last modified: Fri Jul 21 08:57:44 2023, max compression
```

## Comparing `sonnenbatterie-0.1.1.tar` & `sonnenbatterie-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,23 @@
-drwxrwxrwx   0        0        0        0 2020-04-01 07:23:59.000000 sonnenbatterie-0.1.1/
--rw-rw-rw-   0        0        0      592 2020-04-01 07:23:59.000000 sonnenbatterie-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       25 2020-03-27 19:55:40.000000 sonnenbatterie-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2020-04-01 07:23:59.000000 sonnenbatterie-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      830 2020-04-01 07:19:51.000000 sonnenbatterie-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2020-04-01 07:23:59.000000 sonnenbatterie-0.1.1/sonnenbatterie/
--rw-rw-rw-   0        0        0       42 2020-03-27 20:25:55.000000 sonnenbatterie-0.1.1/sonnenbatterie/__init__.py
--rw-rw-rw-   0        0        0     1964 2020-04-01 07:19:28.000000 sonnenbatterie-0.1.1/sonnenbatterie/sonnenbatterie.py
-drwxrwxrwx   0        0        0        0 2020-04-01 07:23:59.000000 sonnenbatterie-0.1.1/sonnenbatterie.egg-info/
--rw-rw-rw-   0        0        0      592 2020-04-01 07:23:58.000000 sonnenbatterie-0.1.1/sonnenbatterie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2020-04-01 07:23:58.000000 sonnenbatterie-0.1.1/sonnenbatterie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-04-01 07:23:58.000000 sonnenbatterie-0.1.1/sonnenbatterie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2020-04-01 07:23:58.000000 sonnenbatterie-0.1.1/sonnenbatterie.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2020-04-01 07:23:58.000000 sonnenbatterie-0.1.1/sonnenbatterie.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 08:57:44.907661 sonnenbatterie-0.2.0/
+-rw-rw-rw-   0        0        0    35823 2023-07-21 08:41:34.000000 sonnenbatterie-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      557 2023-07-21 08:57:44.906435 sonnenbatterie-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       25 2023-07-21 08:41:34.000000 sonnenbatterie-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-21 08:57:44.907661 sonnenbatterie-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      830 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:57:44.891443 sonnenbatterie-0.2.0/sonnenbatterie/
+-rw-rw-rw-   0        0        0       42 2023-07-21 08:41:34.000000 sonnenbatterie-0.2.0/sonnenbatterie/__init__.py
+-rw-rw-rw-   0        0        0     1548 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.0/sonnenbatterie/const.py
+-rw-rw-rw-   0        0        0     6264 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.0/sonnenbatterie/sonnenbatterie.py
+-rw-rw-rw-   0        0        0     5425 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.0/sonnenbatterie/timeofuse.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:57:44.901434 sonnenbatterie-0.2.0/sonnenbatterie.egg-info/
+-rw-rw-rw-   0        0        0      557 2023-07-21 08:57:44.000000 sonnenbatterie-0.2.0/sonnenbatterie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      462 2023-07-21 08:57:44.000000 sonnenbatterie-0.2.0/sonnenbatterie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 08:57:44.000000 sonnenbatterie-0.2.0/sonnenbatterie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-21 08:57:44.000000 sonnenbatterie-0.2.0/sonnenbatterie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-21 08:57:44.000000 sonnenbatterie-0.2.0/sonnenbatterie.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 08:57:44.906435 sonnenbatterie-0.2.0/test/
+-rw-rw-rw-   0        0        0     2158 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.0/test/test_battery_reserve.py
+-rw-rw-rw-   0        0        0     1964 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.0/test/test_operating_mode.py
+-rw-rw-rw-   0        0        0      985 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.0/test/test_origional_code.py
+-rw-rw-rw-   0        0        0     1945 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.0/test/test_timeofuse.py
+-rw-rw-rw-   0        0        0     2637 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.0/test/test_timeofuse_lib.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sonnenbatterie-0.1.1/PKG-INFO` & `sonnenbatterie-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: sonnenbatterie
-Version: 0.1.1
+Version: 0.2.0
 Summary: Access Sonnenbatterie REST API
 Home-page: https://github.com/weltmeyer/python_sonnenbatterie
 Author: Jan Weltmeyer
 Author-email: author@example.com
-License: UNKNOWN
-Description: # python_sonnenbatterie
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# python_sonnenbatterie
```

### Comparing `sonnenbatterie-0.1.1/setup.py` & `sonnenbatterie-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="sonnenbatterie", # Replace with your own username
-    version="0.1.1",
+    version="0.2.0",
     author="Jan Weltmeyer",
     author_email="author@example.com",
     description="Access Sonnenbatterie REST API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/weltmeyer/python_sonnenbatterie",
     packages=["sonnenbatterie"],
```

### Comparing `sonnenbatterie-0.1.1/sonnenbatterie.egg-info/PKG-INFO` & `sonnenbatterie-0.2.0/sonnenbatterie.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: sonnenbatterie
-Version: 0.1.1
+Version: 0.2.0
 Summary: Access Sonnenbatterie REST API
 Home-page: https://github.com/weltmeyer/python_sonnenbatterie
 Author: Jan Weltmeyer
 Author-email: author@example.com
-License: UNKNOWN
-Description: # python_sonnenbatterie
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# python_sonnenbatterie
```

