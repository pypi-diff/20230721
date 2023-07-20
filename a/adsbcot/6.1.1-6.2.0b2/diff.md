# Comparing `tmp/adsbcot-6.1.1.tar.gz` & `tmp/adsbcot-6.2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adsbcot-6.1.1.tar", last modified: Thu Jul 20 22:43:21 2023, max compression
+gzip compressed data, was "adsbcot-6.2.0b2.tar", last modified: Thu Jul 20 23:17:04 2023, max compression
```

## Comparing `adsbcot-6.1.1.tar` & `adsbcot-6.2.0b2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 22:43:21.048890 adsbcot-6.1.1/
--rw-r--r--   0 runner    (1001) docker     (122)      557 2023-07-20 22:43:10.000000 adsbcot-6.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-07-20 22:43:10.000000 adsbcot-6.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3936 2023-07-20 22:43:21.048890 adsbcot-6.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2454 2023-07-20 22:43:10.000000 adsbcot-6.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 22:43:21.048890 adsbcot-6.1.1/adsbcot/
--rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-07-20 22:43:10.000000 adsbcot-6.1.1/adsbcot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16789 2023-07-20 22:43:10.000000 adsbcot-6.1.1/adsbcot/classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-07-20 22:43:10.000000 adsbcot-6.1.1/adsbcot/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-20 22:43:10.000000 adsbcot-6.1.1/adsbcot/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     8114 2023-07-20 22:43:10.000000 adsbcot-6.1.1/adsbcot/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 22:43:21.048890 adsbcot-6.1.1/adsbcot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3936 2023-07-20 22:43:20.000000 adsbcot-6.1.1/adsbcot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      338 2023-07-20 22:43:21.000000 adsbcot-6.1.1/adsbcot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 22:43:20.000000 adsbcot-6.1.1/adsbcot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-20 22:43:20.000000 adsbcot-6.1.1/adsbcot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      170 2023-07-20 22:43:20.000000 adsbcot-6.1.1/adsbcot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-20 22:43:20.000000 adsbcot-6.1.1/adsbcot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1662 2023-07-20 22:43:21.048890 adsbcot-6.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      771 2023-07-20 22:43:10.000000 adsbcot-6.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 23:17:04.283589 adsbcot-6.2.0b2/
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-07-20 23:16:54.000000 adsbcot-6.2.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-07-20 23:16:54.000000 adsbcot-6.2.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3938 2023-07-20 23:17:04.283589 adsbcot-6.2.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2454 2023-07-20 23:16:54.000000 adsbcot-6.2.0b2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 23:17:04.283589 adsbcot-6.2.0b2/adsbcot/
+-rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-07-20 23:16:54.000000 adsbcot-6.2.0b2/adsbcot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16789 2023-07-20 23:16:54.000000 adsbcot-6.2.0b2/adsbcot/classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-07-20 23:16:54.000000 adsbcot-6.2.0b2/adsbcot/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-20 23:16:54.000000 adsbcot-6.2.0b2/adsbcot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8114 2023-07-20 23:16:54.000000 adsbcot-6.2.0b2/adsbcot/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 23:17:04.283589 adsbcot-6.2.0b2/adsbcot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3938 2023-07-20 23:17:04.000000 adsbcot-6.2.0b2/adsbcot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      338 2023-07-20 23:17:04.000000 adsbcot-6.2.0b2/adsbcot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 23:17:04.000000 adsbcot-6.2.0b2/adsbcot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-20 23:17:04.000000 adsbcot-6.2.0b2/adsbcot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-07-20 23:17:04.000000 adsbcot-6.2.0b2/adsbcot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-20 23:17:04.000000 adsbcot-6.2.0b2/adsbcot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1662 2023-07-20 23:17:04.287589 adsbcot-6.2.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      771 2023-07-20 23:16:54.000000 adsbcot-6.2.0b2/setup.py
```

### Comparing `adsbcot-6.1.1/LICENSE` & `adsbcot-6.2.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `adsbcot-6.1.1/PKG-INFO` & `adsbcot-6.2.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adsbcot
-Version: 6.1.1
+Version: 6.2.0b2
 Summary: ADSBCOT: ADS-B to TAK Gateway
 Home-page: https://github.com/snstac/adsbcot
 Maintainer: Greg Albrecht <oss@undef.net>
 Maintainer-email: oss@undef.net
 License: Apache 2.0
 Project-URL: CI: GitHub Actions, https://github.com/snstac/adsbcot/actions
 Project-URL: GitHub: issues, https://github.com/snstac/adsbcot/issues
```

### Comparing `adsbcot-6.1.1/README.rst` & `adsbcot-6.2.0b2/README.rst`

 * *Files identical despite different names*

### Comparing `adsbcot-6.1.1/adsbcot/__init__.py` & `adsbcot-6.2.0b2/adsbcot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 """ADS-B to TAK Gateway.
 
 :author: Greg Albrecht <gba@snstac.com>
 :source: <https://github.com/snstac/adsbcot>
 """
 
-__version__ = "6.1.1"
+__version__ = "6.2.0-beta2"
 __author__ = "Greg Albrecht <gba@snstac.com>"
 __copyright__ = "Copyright 2023 Sensors & Signals LLC"
 __license__ = "Apache License, Version 2.0"
 
 # Python 3.6 test/build work-around:
 try:
     from .constants import (  # NOQA
```

### Comparing `adsbcot-6.1.1/adsbcot/classes.py` & `adsbcot-6.2.0b2/adsbcot/classes.py`

 * *Files identical despite different names*

### Comparing `adsbcot-6.1.1/adsbcot/commands.py` & `adsbcot-6.2.0b2/adsbcot/commands.py`

 * *Files identical despite different names*

### Comparing `adsbcot-6.1.1/adsbcot/constants.py` & `adsbcot-6.2.0b2/adsbcot/constants.py`

 * *Files identical despite different names*

### Comparing `adsbcot-6.1.1/adsbcot/functions.py` & `adsbcot-6.2.0b2/adsbcot/functions.py`

 * *Files identical despite different names*

### Comparing `adsbcot-6.1.1/adsbcot.egg-info/PKG-INFO` & `adsbcot-6.2.0b2/adsbcot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adsbcot
-Version: 6.1.1
+Version: 6.2.0b2
 Summary: ADSBCOT: ADS-B to TAK Gateway
 Home-page: https://github.com/snstac/adsbcot
 Maintainer: Greg Albrecht <oss@undef.net>
 Maintainer-email: oss@undef.net
 License: Apache 2.0
 Project-URL: CI: GitHub Actions, https://github.com/snstac/adsbcot/actions
 Project-URL: GitHub: issues, https://github.com/snstac/adsbcot/issues
```

### Comparing `adsbcot-6.1.1/setup.cfg` & `adsbcot-6.2.0b2/setup.cfg`

 * *Files identical despite different names*

### Comparing `adsbcot-6.1.1/setup.py` & `adsbcot-6.2.0b2/setup.py`

 * *Files identical despite different names*

