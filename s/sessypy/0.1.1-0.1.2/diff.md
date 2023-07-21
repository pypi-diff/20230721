# Comparing `tmp/sessypy-0.1.1.tar.gz` & `tmp/sessypy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sessypy-0.1.1.tar", last modified: Tue Jul 11 17:22:42 2023, max compression
+gzip compressed data, was "sessypy-0.1.2.tar", last modified: Fri Jul 21 15:34:34 2023, max compression
```

## Comparing `sessypy-0.1.1.tar` & `sessypy-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:22:42.420795 sessypy-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-11 17:22:30.000000 sessypy-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-11 17:22:42.420795 sessypy-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-11 17:22:30.000000 sessypy-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-11 17:22:30.000000 sessypy-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-11 17:22:42.420795 sessypy-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:22:42.416794 sessypy-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:22:42.420795 sessypy-0.1.1/src/sessypy/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-11 17:22:30.000000 sessypy-0.1.1/src/sessypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-11 17:22:30.000000 sessypy-0.1.1/src/sessypy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-11 17:22:30.000000 sessypy-0.1.1/src/sessypy/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-11 17:22:30.000000 sessypy-0.1.1/src/sessypy/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-11 17:22:30.000000 sessypy-0.1.1/src/sessypy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:22:42.420795 sessypy-0.1.1/src/sessypy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-11 17:22:42.000000 sessypy-0.1.1/src/sessypy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-11 17:22:42.000000 sessypy-0.1.1/src/sessypy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:22:42.000000 sessypy-0.1.1/src/sessypy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 17:22:42.000000 sessypy-0.1.1/src/sessypy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 17:22:42.000000 sessypy-0.1.1/src/sessypy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:34:34.242035 sessypy-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-21 15:34:21.000000 sessypy-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-21 15:34:34.242035 sessypy-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-21 15:34:21.000000 sessypy-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 15:34:21.000000 sessypy-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-21 15:34:34.242035 sessypy-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:34:34.238036 sessypy-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:34:34.238036 sessypy-0.1.2/src/sessypy/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-21 15:34:21.000000 sessypy-0.1.2/src/sessypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-21 15:34:21.000000 sessypy-0.1.2/src/sessypy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-21 15:34:21.000000 sessypy-0.1.2/src/sessypy/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-07-21 15:34:21.000000 sessypy-0.1.2/src/sessypy/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-21 15:34:21.000000 sessypy-0.1.2/src/sessypy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:34:34.242035 sessypy-0.1.2/src/sessypy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-21 15:34:34.000000 sessypy-0.1.2/src/sessypy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-21 15:34:34.000000 sessypy-0.1.2/src/sessypy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:34:34.000000 sessypy-0.1.2/src/sessypy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 15:34:34.000000 sessypy-0.1.2/src/sessypy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 15:34:34.000000 sessypy-0.1.2/src/sessypy.egg-info/top_level.txt
```

### Comparing `sessypy-0.1.1/LICENSE` & `sessypy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sessypy-0.1.1/PKG-INFO` & `sessypy-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sessypy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python wrapper for Sessy REST API
 Home-page: https://github.com/PimDoos/sessypy
 Author: PimDoos
 License: GNU GPLv3
 Project-URL: Homepage, https://github.com/PimDoos/sessypy
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sessypy-0.1.1/src/sessypy/const.py` & `sessypy-0.1.2/src/sessypy/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,18 +50,21 @@
     VERSION_ERROR = "P1_VERSION_ERR"
     PARSE_ERROR = "P1_PARSE_ERR"
     OK = "P1_OK"
 
 class SessyOtaTarget(str, Enum):
     SELF = "OTA_TARGET_SELF"
     SERIAL = "OTA_TARGET_SERIAL"
+    ALL = "OTA_TARGET_ALL"  # available as of version 1.5.1
 
 class SessyOtaState(str, Enum):
     FAILED = "OTA_UPDATE_FAILED"
+    DISABLED = "OTA_DISABLED"
     INACTIVE = "OTA_INACTIVE"
     CHECKING = "OTA_CHECKING"
     CHECK_FAILED = "OTA_CHECK_FAILED"
     UP_TO_DATE = "OTA_UP_TO_DATE"
     AVAILABLE = "OTA_NEW_VERSION_AVAILABLE"
     UPDATING = "OTA_UPDATING"
+    PENDING_VERIFY = "OTA_PENDING_VERIFY"
     DONE = "OTA_DONE"
-    UNKNOWN = "unknown"
+    UNKNOWN = "unknown"
```

### Comparing `sessypy-0.1.1/src/sessypy/devices.py` & `sessypy-0.1.2/src/sessypy/devices.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from .const import SessyApiCommand, SessyOtaTarget, SessyPowerStrategy
 from .api import SessyApi
 from .util import SessyConnectionException, SessyNotSupportedException
+import logging
+
+_LOGGER = logging.getLogger(__name__)
 
 class SessyDevice():
     def __init__(self, host, username: str, password: str):
         self._serial_number = username.upper()
         self._api = SessyApi(host, username, password)
         self._host = host
     
@@ -102,16 +105,18 @@
     api = SessyApi(host, username, password)
 
     for device_profile in device_profiles:
         if serial_number[0].upper() != device_profile[2]:
             continue
         try:
             await api.get(device_profile[1])
+            _LOGGER.debug(f"Found matching profile {device_profile[0]} for {host}")
             return device_profile[0](api)
         except SessyConnectionException:
+            _LOGGER.debug(f"Skipping device profile {device_profile[0]} for {host}: Connection exception")
             pass
         except SessyNotSupportedException:
+            _LOGGER.debug(f"Skipping device profile {device_profile[0]} for {host}: Not supported")
             pass
 
     await api.close()
     return None
-
```

### Comparing `sessypy-0.1.1/src/sessypy.egg-info/PKG-INFO` & `sessypy-0.1.2/src/sessypy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sessypy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python wrapper for Sessy REST API
 Home-page: https://github.com/PimDoos/sessypy
 Author: PimDoos
 License: GNU GPLv3
 Project-URL: Homepage, https://github.com/PimDoos/sessypy
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

