# Comparing `tmp/finterion-0.2.tar.gz` & `tmp/finterion-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finterion-0.2.tar", last modified: Tue Jul 18 18:22:39 2023, max compression
+gzip compressed data, was "finterion-0.3.tar", last modified: Fri Jul 21 21:02:32 2023, max compression
```

## Comparing `finterion-0.2.tar` & `finterion-0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:22:39.493156 finterion-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-18 18:22:27.000000 finterion-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-18 18:22:39.493156 finterion-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-18 18:22:27.000000 finterion-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:22:39.493156 finterion-0.2/finterion/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-18 18:22:27.000000 finterion-0.2/finterion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:22:39.493156 finterion-0.2/finterion/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:22:27.000000 finterion-0.2/finterion/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-18 18:22:27.000000 finterion-0.2/finterion/configuration/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-18 18:22:27.000000 finterion-0.2/finterion/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-18 18:22:27.000000 finterion-0.2/finterion/finterion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:22:39.493156 finterion-0.2/finterion/models/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-18 18:22:27.000000 finterion-0.2/finterion/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-18 18:22:27.000000 finterion-0.2/finterion/models/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-18 18:22:27.000000 finterion-0.2/finterion/models/algorithm_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-18 18:22:27.000000 finterion-0.2/finterion/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-18 18:22:27.000000 finterion-0.2/finterion/models/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-18 18:22:27.000000 finterion-0.2/finterion/models/order_side.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-18 18:22:27.000000 finterion-0.2/finterion/models/order_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-18 18:22:27.000000 finterion-0.2/finterion/models/order_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-18 18:22:27.000000 finterion-0.2/finterion/models/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-18 18:22:27.000000 finterion-0.2/finterion/models/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-18 18:22:27.000000 finterion-0.2/finterion/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:22:39.493156 finterion-0.2/finterion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-18 18:22:39.000000 finterion-0.2/finterion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-18 18:22:39.000000 finterion-0.2/finterion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:22:39.000000 finterion-0.2/finterion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-18 18:22:39.000000 finterion-0.2/finterion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 18:22:39.000000 finterion-0.2/finterion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:22:39.493156 finterion-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-18 18:22:27.000000 finterion-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:02:32.631711 finterion-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-21 21:02:24.000000 finterion-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-21 21:02:32.631711 finterion-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-21 21:02:24.000000 finterion-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:02:32.627711 finterion-0.3/finterion/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-21 21:02:24.000000 finterion-0.3/finterion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:02:32.627711 finterion-0.3/finterion/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 21:02:24.000000 finterion-0.3/finterion/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-21 21:02:24.000000 finterion-0.3/finterion/configuration/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-21 21:02:24.000000 finterion-0.3/finterion/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-21 21:02:24.000000 finterion-0.3/finterion/finterion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:02:32.631711 finterion-0.3/finterion/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-21 21:02:24.000000 finterion-0.3/finterion/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-21 21:02:24.000000 finterion-0.3/finterion/models/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-21 21:02:24.000000 finterion-0.3/finterion/models/algorithm_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-21 21:02:24.000000 finterion-0.3/finterion/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-21 21:02:24.000000 finterion-0.3/finterion/models/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-21 21:02:24.000000 finterion-0.3/finterion/models/order_side.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-21 21:02:24.000000 finterion-0.3/finterion/models/order_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-21 21:02:24.000000 finterion-0.3/finterion/models/order_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-21 21:02:24.000000 finterion-0.3/finterion/models/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-21 21:02:24.000000 finterion-0.3/finterion/models/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-21 21:02:24.000000 finterion-0.3/finterion/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:02:32.627711 finterion-0.3/finterion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-21 21:02:32.000000 finterion-0.3/finterion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-21 21:02:32.000000 finterion-0.3/finterion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 21:02:32.000000 finterion-0.3/finterion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 21:02:32.000000 finterion-0.3/finterion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 21:02:32.000000 finterion-0.3/finterion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 21:02:32.631711 finterion-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-21 21:02:24.000000 finterion-0.3/setup.py
```

### Comparing `finterion-0.2/LICENSE` & `finterion-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `finterion-0.2/PKG-INFO` & `finterion-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finterion
-Version: 0.2
+Version: 0.3
 Summary: Official python client for Finterion
 Home-page: https://github.com/finterion/finterion-python-client.git
 Author: Finterion
 License: Apache License 2.0
 Keywords: Finterion,finterion,investing-algorithm,INVESTING,BOT,ALGORITHM,FRAMEWORK,investing-bots,trading-bots
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `finterion-0.2/README.md` & `finterion-0.3/README.md`

 * *Files identical despite different names*

### Comparing `finterion-0.2/finterion/finterion.py` & `finterion-0.3/finterion/finterion.py`

 * *Files identical despite different names*

### Comparing `finterion-0.2/finterion/models/algorithm.py` & `finterion-0.3/finterion/models/algorithm.py`

 * *Files identical despite different names*

### Comparing `finterion-0.2/finterion/models/algorithm_profile.py` & `finterion-0.3/finterion/models/algorithm_profile.py`

 * *Files identical despite different names*

### Comparing `finterion-0.2/finterion/models/order.py` & `finterion-0.3/finterion/models/order.py`

 * *Files identical despite different names*

### Comparing `finterion-0.2/finterion/models/order_side.py` & `finterion-0.3/finterion/models/order_side.py`

 * *Files identical despite different names*

### Comparing `finterion-0.2/finterion/models/order_status.py` & `finterion-0.3/finterion/models/order_status.py`

 * *Files identical despite different names*

### Comparing `finterion-0.2/finterion/models/order_type.py` & `finterion-0.3/finterion/models/order_type.py`

 * *Files identical despite different names*

### Comparing `finterion-0.2/finterion/models/portfolio.py` & `finterion-0.3/finterion/models/portfolio.py`

 * *Files identical despite different names*

### Comparing `finterion-0.2/finterion/models/position.py` & `finterion-0.3/finterion/models/position.py`

 * *Files identical despite different names*

### Comparing `finterion-0.2/finterion/services.py` & `finterion-0.3/finterion/services.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,21 @@
     if response.status_code == 200 \
             or response.status_code == 201 \
             or response.status_code == 204:
         return response.json()
     if response.status_code == 401:
         raise ClientException("Unauthorized, check your API key")
     elif response.status_code == 400:
-        raise ClientException(response.json()["message"])
+
+        data = response.json()
+
+        if "message" in data:
+            raise ClientException(data["message"])
+
+        raise ClientException("Something went wrong")
     else:
         raise ClientException("Error connecting to finterion platform")
 
 
 def ping(api_key, url=constants.PING_ENDPOINT):
     response = requests.get(url, headers={"XApiKey": api_key})
     return handle_response(response)
```

### Comparing `finterion-0.2/finterion.egg-info/PKG-INFO` & `finterion-0.3/finterion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finterion
-Version: 0.2
+Version: 0.3
 Summary: Official python client for Finterion
 Home-page: https://github.com/finterion/finterion-python-client.git
 Author: Finterion
 License: Apache License 2.0
 Keywords: Finterion,finterion,investing-algorithm,INVESTING,BOT,ALGORITHM,FRAMEWORK,investing-bots,trading-bots
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `finterion-0.2/finterion.egg-info/SOURCES.txt` & `finterion-0.3/finterion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finterion-0.2/setup.py` & `finterion-0.3/setup.py`

 * *Files identical despite different names*

