# Comparing `tmp/pytelibs-1.2.204.tar.gz` & `tmp/pytelibs-1.2.205.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytelibs-1.2.204.tar", last modified: Thu Jul 20 10:42:02 2023, max compression
+gzip compressed data, was "pytelibs-1.2.205.tar", last modified: Fri Jul 21 12:11:40 2023, max compression
```

## Comparing `pytelibs-1.2.204.tar` & `pytelibs-1.2.205.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 10:42:02.692506 pytelibs-1.2.204/
--rw-r--r--   0 root         (0) root         (0)    34523 2023-07-06 17:18:01.000000 pytelibs-1.2.204/LICENSE
--rw-r--r--   0 root         (0) root         (0)      662 2023-07-20 10:42:02.692506 pytelibs-1.2.204/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-06 19:28:15.000000 pytelibs-1.2.204/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 10:42:02.622506 pytelibs-1.2.204/pytelibs/
--rw-r--r--   0 root         (0) root         (0)      477 2023-07-20 09:55:37.000000 pytelibs-1.2.204/pytelibs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-07-20 09:54:50.000000 pytelibs-1.2.204/pytelibs/_journal.py
--rw-r--r--   0 root         (0) root         (0)      274 2023-07-20 10:40:51.000000 pytelibs-1.2.204/pytelibs/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 10:42:02.672506 pytelibs-1.2.204/pytelibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      662 2023-07-20 10:42:01.000000 pytelibs-1.2.204/pytelibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      248 2023-07-20 10:42:01.000000 pytelibs-1.2.204/pytelibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 10:42:01.000000 pytelibs-1.2.204/pytelibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-20 10:42:01.000000 pytelibs-1.2.204/pytelibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-20 10:42:01.000000 pytelibs-1.2.204/pytelibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 10:42:02.692506 pytelibs-1.2.204/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1053 2023-07-13 10:27:02.000000 pytelibs-1.2.204/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:11:40.754642 pytelibs-1.2.205/
+-rw-r--r--   0 root         (0) root         (0)    34523 2023-07-06 17:18:01.000000 pytelibs-1.2.205/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      662 2023-07-21 12:11:40.754642 pytelibs-1.2.205/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-06 19:28:15.000000 pytelibs-1.2.205/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:11:40.694642 pytelibs-1.2.205/pytelibs/
+-rw-r--r--   0 root         (0) root         (0)      539 2023-07-21 11:53:32.000000 pytelibs-1.2.205/pytelibs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      451 2023-07-21 12:10:57.000000 pytelibs-1.2.205/pytelibs/_globvals.py
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-07-21 12:09:57.000000 pytelibs-1.2.205/pytelibs/_journal.py
+-rw-r--r--   0 root         (0) root         (0)      274 2023-07-21 09:24:58.000000 pytelibs-1.2.205/pytelibs/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:11:40.734642 pytelibs-1.2.205/pytelibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      662 2023-07-21 12:11:40.000000 pytelibs-1.2.205/pytelibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      270 2023-07-21 12:11:40.000000 pytelibs-1.2.205/pytelibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 12:11:40.000000 pytelibs-1.2.205/pytelibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-21 12:11:40.000000 pytelibs-1.2.205/pytelibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-21 12:11:40.000000 pytelibs-1.2.205/pytelibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 12:11:40.754642 pytelibs-1.2.205/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-07-13 10:27:02.000000 pytelibs-1.2.205/setup.py
```

### Comparing `pytelibs-1.2.204/LICENSE` & `pytelibs-1.2.205/LICENSE`

 * *Files identical despite different names*

### Comparing `pytelibs-1.2.204/PKG-INFO` & `pytelibs-1.2.205/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytelibs
-Version: 1.2.204
+Version: 1.2.205
 Summary: Client library for Pytel
 Home-page: https://github.com/kastaid/pytelibs
 Author: Unknown
 Author-email: unknownkz@outlook.co.id
 License: AGPL
 Keywords: pypi,pytelibs,python,pyrogram,telebot
 Platform: UNKNOWN
```

### Comparing `pytelibs-1.2.204/pytelibs/_journal.py` & `pytelibs-1.2.205/pytelibs/_journal.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # pytel < https://t.me/kastaid >
 # Copyright (C) 2023-present kastaid
 #
 # This file is a part of < https://github.com/kastaid/pytel/ >
 # Please read the GNU Affero General Public License in
 # < https://github.com/kastaid/pytel/blob/main/LICENSE/ >.
 
-from typing import Set
 from base64 import b64decode
 
 
 _c, _g, _l, _d, gsc, gse, _i, cpytl = (
     b64decode("a2FzdGFpZA==").decode(
         "utf-8"
     ),
@@ -57,10 +56,7 @@
 )
 _kastaot = (
     -1001699144606,
 )
 _chpytel = (
     -1001901158945,
 )
-
-_DELAY_MSG: Set[int] = set()
-_SCHEDULE_MSG: Set[int] = set()
```

### Comparing `pytelibs-1.2.204/pytelibs.egg-info/PKG-INFO` & `pytelibs-1.2.205/pytelibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytelibs
-Version: 1.2.204
+Version: 1.2.205
 Summary: Client library for Pytel
 Home-page: https://github.com/kastaid/pytelibs
 Author: Unknown
 Author-email: unknownkz@outlook.co.id
 License: AGPL
 Keywords: pypi,pytelibs,python,pyrogram,telebot
 Platform: UNKNOWN
```

### Comparing `pytelibs-1.2.204/setup.py` & `pytelibs-1.2.205/setup.py`

 * *Files identical despite different names*

