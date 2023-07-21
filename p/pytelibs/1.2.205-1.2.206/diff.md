# Comparing `tmp/pytelibs-1.2.205.tar.gz` & `tmp/pytelibs-1.2.206.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytelibs-1.2.205.tar", last modified: Fri Jul 21 12:11:40 2023, max compression
+gzip compressed data, was "pytelibs-1.2.206.tar", last modified: Fri Jul 21 15:52:15 2023, max compression
```

## Comparing `pytelibs-1.2.205.tar` & `pytelibs-1.2.206.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:11:40.754642 pytelibs-1.2.205/
--rw-r--r--   0 root         (0) root         (0)    34523 2023-07-06 17:18:01.000000 pytelibs-1.2.205/LICENSE
--rw-r--r--   0 root         (0) root         (0)      662 2023-07-21 12:11:40.754642 pytelibs-1.2.205/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-06 19:28:15.000000 pytelibs-1.2.205/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:11:40.694642 pytelibs-1.2.205/pytelibs/
--rw-r--r--   0 root         (0) root         (0)      539 2023-07-21 11:53:32.000000 pytelibs-1.2.205/pytelibs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      451 2023-07-21 12:10:57.000000 pytelibs-1.2.205/pytelibs/_globvals.py
--rw-r--r--   0 root         (0) root         (0)     1543 2023-07-21 12:09:57.000000 pytelibs-1.2.205/pytelibs/_journal.py
--rw-r--r--   0 root         (0) root         (0)      274 2023-07-21 09:24:58.000000 pytelibs-1.2.205/pytelibs/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:11:40.734642 pytelibs-1.2.205/pytelibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      662 2023-07-21 12:11:40.000000 pytelibs-1.2.205/pytelibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      270 2023-07-21 12:11:40.000000 pytelibs-1.2.205/pytelibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 12:11:40.000000 pytelibs-1.2.205/pytelibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-21 12:11:40.000000 pytelibs-1.2.205/pytelibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-21 12:11:40.000000 pytelibs-1.2.205/pytelibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 12:11:40.754642 pytelibs-1.2.205/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1053 2023-07-13 10:27:02.000000 pytelibs-1.2.205/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:52:15.852681 pytelibs-1.2.206/
+-rw-r--r--   0 root         (0) root         (0)    34523 2023-07-06 17:18:01.000000 pytelibs-1.2.206/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      662 2023-07-21 15:52:15.852681 pytelibs-1.2.206/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-06 19:28:15.000000 pytelibs-1.2.206/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:52:15.772681 pytelibs-1.2.206/pytelibs/
+-rw-r--r--   0 root         (0) root         (0)      539 2023-07-21 11:53:32.000000 pytelibs-1.2.206/pytelibs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-07-21 14:59:57.000000 pytelibs-1.2.206/pytelibs/_globvals.py
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-07-21 12:09:57.000000 pytelibs-1.2.206/pytelibs/_journal.py
+-rw-r--r--   0 root         (0) root         (0)      274 2023-07-21 14:15:10.000000 pytelibs-1.2.206/pytelibs/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:52:15.832681 pytelibs-1.2.206/pytelibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      662 2023-07-21 15:52:15.000000 pytelibs-1.2.206/pytelibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      270 2023-07-21 15:52:15.000000 pytelibs-1.2.206/pytelibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:52:15.000000 pytelibs-1.2.206/pytelibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-21 15:52:15.000000 pytelibs-1.2.206/pytelibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-21 15:52:15.000000 pytelibs-1.2.206/pytelibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 15:52:15.852681 pytelibs-1.2.206/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-07-13 10:27:02.000000 pytelibs-1.2.206/setup.py
```

### Comparing `pytelibs-1.2.205/LICENSE` & `pytelibs-1.2.206/LICENSE`

 * *Files identical despite different names*

### Comparing `pytelibs-1.2.205/PKG-INFO` & `pytelibs-1.2.206/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytelibs
-Version: 1.2.205
+Version: 1.2.206
 Summary: Client library for Pytel
 Home-page: https://github.com/kastaid/pytelibs
 Author: Unknown
 Author-email: unknownkz@outlook.co.id
 License: AGPL
 Keywords: pypi,pytelibs,python,pyrogram,telebot
 Platform: UNKNOWN
```

### Comparing `pytelibs-1.2.205/pytelibs/__init__.py` & `pytelibs-1.2.206/pytelibs/__init__.py`

 * *Files identical despite different names*

### Comparing `pytelibs-1.2.205/pytelibs/_journal.py` & `pytelibs-1.2.206/pytelibs/_journal.py`

 * *Files identical despite different names*

### Comparing `pytelibs-1.2.205/pytelibs.egg-info/PKG-INFO` & `pytelibs-1.2.206/pytelibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytelibs
-Version: 1.2.205
+Version: 1.2.206
 Summary: Client library for Pytel
 Home-page: https://github.com/kastaid/pytelibs
 Author: Unknown
 Author-email: unknownkz@outlook.co.id
 License: AGPL
 Keywords: pypi,pytelibs,python,pyrogram,telebot
 Platform: UNKNOWN
```

### Comparing `pytelibs-1.2.205/setup.py` & `pytelibs-1.2.206/setup.py`

 * *Files identical despite different names*

