# Comparing `tmp/sessypy-0.1.2.tar.gz` & `tmp/sessypy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sessypy-0.1.2.tar", last modified: Fri Jul 21 15:34:34 2023, max compression
+gzip compressed data, was "sessypy-0.1.3.tar", last modified: Fri Jul 21 18:48:48 2023, max compression
```

## Comparing `sessypy-0.1.2.tar` & `sessypy-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:34:34.242035 sessypy-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-21 15:34:21.000000 sessypy-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-21 15:34:34.242035 sessypy-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-21 15:34:21.000000 sessypy-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 15:34:21.000000 sessypy-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-21 15:34:34.242035 sessypy-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:34:34.238036 sessypy-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:34:34.238036 sessypy-0.1.2/src/sessypy/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-21 15:34:21.000000 sessypy-0.1.2/src/sessypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-21 15:34:21.000000 sessypy-0.1.2/src/sessypy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-21 15:34:21.000000 sessypy-0.1.2/src/sessypy/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-07-21 15:34:21.000000 sessypy-0.1.2/src/sessypy/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-21 15:34:21.000000 sessypy-0.1.2/src/sessypy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:34:34.242035 sessypy-0.1.2/src/sessypy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-21 15:34:34.000000 sessypy-0.1.2/src/sessypy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-21 15:34:34.000000 sessypy-0.1.2/src/sessypy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:34:34.000000 sessypy-0.1.2/src/sessypy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 15:34:34.000000 sessypy-0.1.2/src/sessypy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 15:34:34.000000 sessypy-0.1.2/src/sessypy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:48:48.610309 sessypy-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-21 18:48:35.000000 sessypy-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-21 18:48:48.610309 sessypy-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-21 18:48:35.000000 sessypy-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 18:48:35.000000 sessypy-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-21 18:48:48.610309 sessypy-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:48:48.610309 sessypy-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:48:48.610309 sessypy-0.1.3/src/sessypy/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-21 18:48:35.000000 sessypy-0.1.3/src/sessypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-21 18:48:35.000000 sessypy-0.1.3/src/sessypy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-21 18:48:35.000000 sessypy-0.1.3/src/sessypy/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-21 18:48:35.000000 sessypy-0.1.3/src/sessypy/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-21 18:48:35.000000 sessypy-0.1.3/src/sessypy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:48:48.610309 sessypy-0.1.3/src/sessypy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-21 18:48:48.000000 sessypy-0.1.3/src/sessypy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-21 18:48:48.000000 sessypy-0.1.3/src/sessypy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 18:48:48.000000 sessypy-0.1.3/src/sessypy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 18:48:48.000000 sessypy-0.1.3/src/sessypy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 18:48:48.000000 sessypy-0.1.3/src/sessypy.egg-info/top_level.txt
```

### Comparing `sessypy-0.1.2/LICENSE` & `sessypy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sessypy-0.1.2/PKG-INFO` & `sessypy-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sessypy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python wrapper for Sessy REST API
 Home-page: https://github.com/PimDoos/sessypy
 Author: PimDoos
 License: GNU GPLv3
 Project-URL: Homepage, https://github.com/PimDoos/sessypy
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sessypy-0.1.2/src/sessypy/api.py` & `sessypy-0.1.3/src/sessypy/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,25 +26,25 @@
             url = self._command_url(command)
             _LOGGER.debug(f"Sending {method} request to {url} with data {data}")
             response = await self.session.request(method, url, json = data)
             return await response.json()
         
         except ClientConnectionError as e:
             _LOGGER.debug(f"{method} request to {url} raised a connection error: {e}")
-            raise SessyConnectionException
+            raise SessyConnectionException from e
         
         except ContentTypeError as e:
             _LOGGER.debug(f"{method} request to {url} returned content of an unexpected type: {e.message}")
-            raise SessyNotSupportedException
+            raise SessyNotSupportedException from e
         
         except ClientResponseError as e:
             _LOGGER.debug(f"{method} request to {url} returned an error response code: {e.status} {e.message}")
             if e.status == 401:
-                raise SessyLoginException
+                raise SessyLoginException from e
             else:
-                raise SessyNotSupportedException
+                raise SessyNotSupportedException from e
 
     def _command_url(self, command: SessyApiCommand):
         return f"http://{self.host}/{command.value}"
 
     async def close(self):
         await self.session.close()
```

### Comparing `sessypy-0.1.2/src/sessypy/const.py` & `sessypy-0.1.3/src/sessypy/const.py`

 * *Files identical despite different names*

### Comparing `sessypy-0.1.2/src/sessypy/devices.py` & `sessypy-0.1.3/src/sessypy/devices.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,14 +109,16 @@
             continue
         try:
             await api.get(device_profile[1])
             _LOGGER.debug(f"Found matching profile {device_profile[0]} for {host}")
             return device_profile[0](api)
         except SessyConnectionException:
             _LOGGER.debug(f"Skipping device profile {device_profile[0]} for {host}: Connection exception")
-            pass
+
         except SessyNotSupportedException:
             _LOGGER.debug(f"Skipping device profile {device_profile[0]} for {host}: Not supported")
-            pass
+
 
     await api.close()
-    return None
+    
+    # Device does not match any known device profiles, so it is not supported
+    raise SessyNotSupportedException
```

### Comparing `sessypy-0.1.2/src/sessypy.egg-info/PKG-INFO` & `sessypy-0.1.3/src/sessypy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sessypy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python wrapper for Sessy REST API
 Home-page: https://github.com/PimDoos/sessypy
 Author: PimDoos
 License: GNU GPLv3
 Project-URL: Homepage, https://github.com/PimDoos/sessypy
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

