# Comparing `tmp/adsbcot-6.2.0b3.tar.gz` & `tmp/adsbcot-6.2.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adsbcot-6.2.0b3.tar", last modified: Thu Jul 20 23:42:09 2023, max compression
+gzip compressed data, was "adsbcot-6.2.0b4.tar", last modified: Thu Jul 20 23:49:10 2023, max compression
```

## Comparing `adsbcot-6.2.0b3.tar` & `adsbcot-6.2.0b4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 23:42:09.485103 adsbcot-6.2.0b3/
--rw-r--r--   0 runner    (1001) docker     (122)      557 2023-07-20 23:41:56.000000 adsbcot-6.2.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-07-20 23:41:56.000000 adsbcot-6.2.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3938 2023-07-20 23:42:09.489103 adsbcot-6.2.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2454 2023-07-20 23:41:56.000000 adsbcot-6.2.0b3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 23:42:09.485103 adsbcot-6.2.0b3/adsbcot/
--rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-07-20 23:41:56.000000 adsbcot-6.2.0b3/adsbcot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 23:42:09.485103 adsbcot-6.2.0b3/adsbcot/adsbcot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3938 2023-07-20 23:42:09.000000 adsbcot-6.2.0b3/adsbcot/adsbcot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-20 23:42:09.000000 adsbcot-6.2.0b3/adsbcot/adsbcot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 23:42:09.000000 adsbcot-6.2.0b3/adsbcot/adsbcot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-20 23:42:09.000000 adsbcot-6.2.0b3/adsbcot/adsbcot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      170 2023-07-20 23:42:09.000000 adsbcot-6.2.0b3/adsbcot/adsbcot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-20 23:42:09.000000 adsbcot-6.2.0b3/adsbcot/adsbcot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    16789 2023-07-20 23:41:56.000000 adsbcot-6.2.0b3/adsbcot/classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-07-20 23:41:56.000000 adsbcot-6.2.0b3/adsbcot/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-20 23:41:56.000000 adsbcot-6.2.0b3/adsbcot/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     8114 2023-07-20 23:41:56.000000 adsbcot-6.2.0b3/adsbcot/functions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-20 23:42:09.489103 adsbcot-6.2.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      771 2023-07-20 23:41:56.000000 adsbcot-6.2.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 23:49:10.694326 adsbcot-6.2.0b4/
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-07-20 23:48:58.000000 adsbcot-6.2.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-07-20 23:48:58.000000 adsbcot-6.2.0b4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3938 2023-07-20 23:49:10.694326 adsbcot-6.2.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2454 2023-07-20 23:48:58.000000 adsbcot-6.2.0b4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 23:49:10.694326 adsbcot-6.2.0b4/adsbcot/
+-rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-07-20 23:48:58.000000 adsbcot-6.2.0b4/adsbcot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16789 2023-07-20 23:48:58.000000 adsbcot-6.2.0b4/adsbcot/classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-07-20 23:48:58.000000 adsbcot-6.2.0b4/adsbcot/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-20 23:48:58.000000 adsbcot-6.2.0b4/adsbcot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8114 2023-07-20 23:48:58.000000 adsbcot-6.2.0b4/adsbcot/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 23:49:10.694326 adsbcot-6.2.0b4/adsbcot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3938 2023-07-20 23:49:10.000000 adsbcot-6.2.0b4/adsbcot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      338 2023-07-20 23:49:10.000000 adsbcot-6.2.0b4/adsbcot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 23:49:10.000000 adsbcot-6.2.0b4/adsbcot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-20 23:49:10.000000 adsbcot-6.2.0b4/adsbcot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-07-20 23:49:10.000000 adsbcot-6.2.0b4/adsbcot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-20 23:49:10.000000 adsbcot-6.2.0b4/adsbcot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1696 2023-07-20 23:49:10.694326 adsbcot-6.2.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      771 2023-07-20 23:48:58.000000 adsbcot-6.2.0b4/setup.py
```

### Comparing `adsbcot-6.2.0b3/LICENSE` & `adsbcot-6.2.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `adsbcot-6.2.0b3/PKG-INFO` & `adsbcot-6.2.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adsbcot
-Version: 6.2.0b3
+Version: 6.2.0b4
 Summary: ADSBCOT: ADS-B to TAK Gateway
 Home-page: https://github.com/snstac/adsbcot
 Maintainer: Greg Albrecht <oss@undef.net>
 Maintainer-email: oss@undef.net
 License: Apache 2.0
 Project-URL: CI: GitHub Actions, https://github.com/snstac/adsbcot/actions
 Project-URL: GitHub: issues, https://github.com/snstac/adsbcot/issues
```

### Comparing `adsbcot-6.2.0b3/README.rst` & `adsbcot-6.2.0b4/README.rst`

 * *Files identical despite different names*

### Comparing `adsbcot-6.2.0b3/adsbcot/__init__.py` & `adsbcot-6.2.0b4/adsbcot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 """ADS-B to TAK Gateway.
 
 :author: Greg Albrecht <gba@snstac.com>
 :source: <https://github.com/snstac/adsbcot>
 """
 
-__version__ = "6.2.0-beta3"
+__version__ = "6.2.0-beta4"
 __author__ = "Greg Albrecht <gba@snstac.com>"
 __copyright__ = "Copyright 2023 Sensors & Signals LLC"
 __license__ = "Apache License, Version 2.0"
 
 # Python 3.6 test/build work-around:
 try:
     from .constants import (  # NOQA
```

### Comparing `adsbcot-6.2.0b3/adsbcot/adsbcot.egg-info/PKG-INFO` & `adsbcot-6.2.0b4/adsbcot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adsbcot
-Version: 6.2.0b3
+Version: 6.2.0b4
 Summary: ADSBCOT: ADS-B to TAK Gateway
 Home-page: https://github.com/snstac/adsbcot
 Maintainer: Greg Albrecht <oss@undef.net>
 Maintainer-email: oss@undef.net
 License: Apache 2.0
 Project-URL: CI: GitHub Actions, https://github.com/snstac/adsbcot/actions
 Project-URL: GitHub: issues, https://github.com/snstac/adsbcot/issues
```

### Comparing `adsbcot-6.2.0b3/adsbcot/classes.py` & `adsbcot-6.2.0b4/adsbcot/classes.py`

 * *Files identical despite different names*

### Comparing `adsbcot-6.2.0b3/adsbcot/commands.py` & `adsbcot-6.2.0b4/adsbcot/commands.py`

 * *Files identical despite different names*

### Comparing `adsbcot-6.2.0b3/adsbcot/constants.py` & `adsbcot-6.2.0b4/adsbcot/constants.py`

 * *Files identical despite different names*

### Comparing `adsbcot-6.2.0b3/adsbcot/functions.py` & `adsbcot-6.2.0b4/adsbcot/functions.py`

 * *Files identical despite different names*

### Comparing `adsbcot-6.2.0b3/setup.cfg` & `adsbcot-6.2.0b4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 [options.entry_points]
 console_scripts = 
 	adsbcot = adsbcot.commands:main
 
 [options]
 package_dir = 
-	= adsbcot
+	adsbcot = adsbcot
 python_requires = >=3.6, <4
 install_requires = 
 	aircot >= 1.2.0
 	pytak >= 5.4.0
 	aiohttp < 4.0.0
 	asyncinotify
```

### Comparing `adsbcot-6.2.0b3/setup.py` & `adsbcot-6.2.0b4/setup.py`

 * *Files identical despite different names*

