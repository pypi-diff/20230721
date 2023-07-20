# Comparing `tmp/adsbcot-6.2.0b2.tar.gz` & `tmp/adsbcot-6.2.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adsbcot-6.2.0b2.tar", last modified: Thu Jul 20 23:17:04 2023, max compression
+gzip compressed data, was "adsbcot-6.2.0b3.tar", last modified: Thu Jul 20 23:42:09 2023, max compression
```

## Comparing `adsbcot-6.2.0b2.tar` & `adsbcot-6.2.0b3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 23:17:04.283589 adsbcot-6.2.0b2/
--rw-r--r--   0 runner    (1001) docker     (122)      557 2023-07-20 23:16:54.000000 adsbcot-6.2.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-07-20 23:16:54.000000 adsbcot-6.2.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3938 2023-07-20 23:17:04.283589 adsbcot-6.2.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2454 2023-07-20 23:16:54.000000 adsbcot-6.2.0b2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 23:17:04.283589 adsbcot-6.2.0b2/adsbcot/
--rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-07-20 23:16:54.000000 adsbcot-6.2.0b2/adsbcot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16789 2023-07-20 23:16:54.000000 adsbcot-6.2.0b2/adsbcot/classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-07-20 23:16:54.000000 adsbcot-6.2.0b2/adsbcot/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-20 23:16:54.000000 adsbcot-6.2.0b2/adsbcot/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     8114 2023-07-20 23:16:54.000000 adsbcot-6.2.0b2/adsbcot/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 23:17:04.283589 adsbcot-6.2.0b2/adsbcot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3938 2023-07-20 23:17:04.000000 adsbcot-6.2.0b2/adsbcot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      338 2023-07-20 23:17:04.000000 adsbcot-6.2.0b2/adsbcot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 23:17:04.000000 adsbcot-6.2.0b2/adsbcot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-20 23:17:04.000000 adsbcot-6.2.0b2/adsbcot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      170 2023-07-20 23:17:04.000000 adsbcot-6.2.0b2/adsbcot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-20 23:17:04.000000 adsbcot-6.2.0b2/adsbcot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1662 2023-07-20 23:17:04.287589 adsbcot-6.2.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      771 2023-07-20 23:16:54.000000 adsbcot-6.2.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 23:42:09.485103 adsbcot-6.2.0b3/
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-07-20 23:41:56.000000 adsbcot-6.2.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-07-20 23:41:56.000000 adsbcot-6.2.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3938 2023-07-20 23:42:09.489103 adsbcot-6.2.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2454 2023-07-20 23:41:56.000000 adsbcot-6.2.0b3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 23:42:09.485103 adsbcot-6.2.0b3/adsbcot/
+-rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-07-20 23:41:56.000000 adsbcot-6.2.0b3/adsbcot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 23:42:09.485103 adsbcot-6.2.0b3/adsbcot/adsbcot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3938 2023-07-20 23:42:09.000000 adsbcot-6.2.0b3/adsbcot/adsbcot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-20 23:42:09.000000 adsbcot-6.2.0b3/adsbcot/adsbcot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 23:42:09.000000 adsbcot-6.2.0b3/adsbcot/adsbcot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-20 23:42:09.000000 adsbcot-6.2.0b3/adsbcot/adsbcot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-07-20 23:42:09.000000 adsbcot-6.2.0b3/adsbcot/adsbcot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-20 23:42:09.000000 adsbcot-6.2.0b3/adsbcot/adsbcot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    16789 2023-07-20 23:41:56.000000 adsbcot-6.2.0b3/adsbcot/classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-07-20 23:41:56.000000 adsbcot-6.2.0b3/adsbcot/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-20 23:41:56.000000 adsbcot-6.2.0b3/adsbcot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8114 2023-07-20 23:41:56.000000 adsbcot-6.2.0b3/adsbcot/functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-20 23:42:09.489103 adsbcot-6.2.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      771 2023-07-20 23:41:56.000000 adsbcot-6.2.0b3/setup.py
```

### Comparing `adsbcot-6.2.0b2/LICENSE` & `adsbcot-6.2.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `adsbcot-6.2.0b2/PKG-INFO` & `adsbcot-6.2.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adsbcot
-Version: 6.2.0b2
+Version: 6.2.0b3
 Summary: ADSBCOT: ADS-B to TAK Gateway
 Home-page: https://github.com/snstac/adsbcot
 Maintainer: Greg Albrecht <oss@undef.net>
 Maintainer-email: oss@undef.net
 License: Apache 2.0
 Project-URL: CI: GitHub Actions, https://github.com/snstac/adsbcot/actions
 Project-URL: GitHub: issues, https://github.com/snstac/adsbcot/issues
```

### Comparing `adsbcot-6.2.0b2/README.rst` & `adsbcot-6.2.0b3/README.rst`

 * *Files identical despite different names*

### Comparing `adsbcot-6.2.0b2/adsbcot/__init__.py` & `adsbcot-6.2.0b3/adsbcot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 """ADS-B to TAK Gateway.
 
 :author: Greg Albrecht <gba@snstac.com>
 :source: <https://github.com/snstac/adsbcot>
 """
 
-__version__ = "6.2.0-beta2"
+__version__ = "6.2.0-beta3"
 __author__ = "Greg Albrecht <gba@snstac.com>"
 __copyright__ = "Copyright 2023 Sensors & Signals LLC"
 __license__ = "Apache License, Version 2.0"
 
 # Python 3.6 test/build work-around:
 try:
     from .constants import (  # NOQA
```

### Comparing `adsbcot-6.2.0b2/adsbcot/classes.py` & `adsbcot-6.2.0b3/adsbcot/classes.py`

 * *Files identical despite different names*

### Comparing `adsbcot-6.2.0b2/adsbcot/commands.py` & `adsbcot-6.2.0b3/adsbcot/commands.py`

 * *Files identical despite different names*

### Comparing `adsbcot-6.2.0b2/adsbcot/constants.py` & `adsbcot-6.2.0b3/adsbcot/constants.py`

 * *Files identical despite different names*

### Comparing `adsbcot-6.2.0b2/adsbcot/functions.py` & `adsbcot-6.2.0b3/adsbcot/functions.py`

 * *Files identical despite different names*

### Comparing `adsbcot-6.2.0b2/adsbcot.egg-info/PKG-INFO` & `adsbcot-6.2.0b3/adsbcot/adsbcot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adsbcot
-Version: 6.2.0b2
+Version: 6.2.0b3
 Summary: ADSBCOT: ADS-B to TAK Gateway
 Home-page: https://github.com/snstac/adsbcot
 Maintainer: Greg Albrecht <oss@undef.net>
 Maintainer-email: oss@undef.net
 License: Apache 2.0
 Project-URL: CI: GitHub Actions, https://github.com/snstac/adsbcot/actions
 Project-URL: GitHub: issues, https://github.com/snstac/adsbcot/issues
```

### Comparing `adsbcot-6.2.0b2/setup.cfg` & `adsbcot-6.2.0b3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 	Aircraft
 
 [options.entry_points]
 console_scripts = 
 	adsbcot = adsbcot.commands:main
 
 [options]
+package_dir = 
+	= adsbcot
 python_requires = >=3.6, <4
 install_requires = 
 	aircot >= 1.2.0
 	pytak >= 5.4.0
 	aiohttp < 4.0.0
 	asyncinotify
```

### Comparing `adsbcot-6.2.0b2/setup.py` & `adsbcot-6.2.0b3/setup.py`

 * *Files identical despite different names*

