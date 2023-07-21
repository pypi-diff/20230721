# Comparing `tmp/lest-0.4.1.tar.gz` & `tmp/lest-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lest-0.4.1.tar", last modified: Wed Jul  5 07:01:31 2023, max compression
+gzip compressed data, was "lest-0.5.0.tar", last modified: Fri Jul 21 13:27:50 2023, max compression
```

## Comparing `lest-0.4.1.tar` & `lest-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 07:01:31.253683 lest-0.4.1/
--rw-rw-rw-   0        0        0     1084 2023-04-04 11:05:14.000000 lest-0.4.1/LICENSE
--rw-rw-rw-   0        0        0     1238 2023-07-05 07:01:31.252682 lest-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0      735 2023-06-26 08:38:11.000000 lest-0.4.1/README.md
--rw-rw-rw-   0        0        0      493 2023-07-05 06:59:57.000000 lest-0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-05 07:01:31.253683 lest-0.4.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-05 07:01:31.220195 lest-0.4.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-05 07:01:31.242310 lest-0.4.1/src/lest/
--rw-rw-rw-   0        0        0      446 2023-06-22 08:44:53.000000 lest-0.4.1/src/lest/__init__.py
--rw-rw-rw-   0        0        0      911 2023-04-12 07:13:46.000000 lest-0.4.1/src/lest/assertions.py
--rw-rw-rw-   0        0        0      312 2023-04-03 11:04:41.000000 lest-0.4.1/src/lest/registerer.py
--rw-rw-rw-   0        0        0     2313 2023-07-05 06:48:27.000000 lest-0.4.1/src/lest/runner.py
--rw-rw-rw-   0        0        0      205 2023-06-22 08:40:08.000000 lest-0.4.1/src/lest/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 07:01:31.250679 lest-0.4.1/src/lest.egg-info/
--rw-rw-rw-   0        0        0     1238 2023-07-05 07:01:31.000000 lest-0.4.1/src/lest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-07-05 07:01:31.000000 lest-0.4.1/src/lest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 07:01:31.000000 lest-0.4.1/src/lest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-05 07:01:31.000000 lest-0.4.1/src/lest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 13:27:50.545940 lest-0.5.0/
+-rw-rw-rw-   0        0        0     1084 2023-04-04 11:05:14.000000 lest-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     1570 2023-07-21 13:27:50.544939 lest-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      735 2023-06-26 08:38:11.000000 lest-0.5.0/README.md
+-rw-rw-rw-   0        0        0      832 2023-07-21 13:27:06.000000 lest-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-21 13:27:50.545940 lest-0.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-21 13:27:50.452960 lest-0.5.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-21 13:27:50.520933 lest-0.5.0/src/lest/
+-rw-rw-rw-   0        0        0      446 2023-06-22 08:44:53.000000 lest-0.5.0/src/lest/__init__.py
+-rw-rw-rw-   0        0        0     1105 2023-07-21 13:10:26.000000 lest-0.5.0/src/lest/assertions.py
+-rw-rw-rw-   0        0        0      312 2023-04-03 11:04:41.000000 lest-0.5.0/src/lest/registerer.py
+-rw-rw-rw-   0        0        0     2313 2023-07-05 06:48:27.000000 lest-0.5.0/src/lest/runner.py
+-rw-rw-rw-   0        0        0      205 2023-06-22 08:40:08.000000 lest-0.5.0/src/lest/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 13:27:50.542939 lest-0.5.0/src/lest.egg-info/
+-rw-rw-rw-   0        0        0     1570 2023-07-21 13:27:50.000000 lest-0.5.0/src/lest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-07-21 13:27:50.000000 lest-0.5.0/src/lest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 13:27:50.000000 lest-0.5.0/src/lest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-21 13:27:50.000000 lest-0.5.0/src/lest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-21 13:27:50.000000 lest-0.5.0/src/lest.egg-info/top_level.txt
```

### Comparing `lest-0.4.1/LICENSE` & `lest-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lest-0.4.1/PKG-INFO` & `lest-0.5.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 Metadata-Version: 2.1
 Name: lest
-Version: 0.4.1
+Version: 0.5.0
 Summary: Light Python library for testing.
 Author-email: wchistow <wchistow@yandex.ru>
 Project-URL: Homepage, https://github.com/wchistow/lest
 Project-URL: Bug Tracker, https://github.com/wchistow/lest/issues
+Project-URL: Repository, https://github.com/wchistow/lest.git
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Lest
```

### Comparing `lest-0.4.1/README.md` & `lest-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `lest-0.4.1/src/lest/runner.py` & `lest-0.5.0/src/lest/runner.py`

 * *Files identical despite different names*

### Comparing `lest-0.4.1/src/lest.egg-info/PKG-INFO` & `lest-0.5.0/src/lest.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 Metadata-Version: 2.1
 Name: lest
-Version: 0.4.1
+Version: 0.5.0
 Summary: Light Python library for testing.
 Author-email: wchistow <wchistow@yandex.ru>
 Project-URL: Homepage, https://github.com/wchistow/lest
 Project-URL: Bug Tracker, https://github.com/wchistow/lest/issues
+Project-URL: Repository, https://github.com/wchistow/lest.git
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Lest
```

