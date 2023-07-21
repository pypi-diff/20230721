# Comparing `tmp/alephvault-http-mongodb-storage-0.0.8.tar.gz` & `tmp/alephvault-http-mongodb-storage-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alephvault-http-mongodb-storage-0.0.8.tar", last modified: Mon Jun 27 16:27:59 2022, max compression
+gzip compressed data, was "alephvault-http-mongodb-storage-0.0.9.tar", last modified: Wed Feb  8 00:34:44 2023, max compression
```

## Comparing `alephvault-http-mongodb-storage-0.0.8.tar` & `alephvault-http-mongodb-storage-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2022-06-27 16:27:59.040903 alephvault-http-mongodb-storage-0.0.8/
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     1067 2022-04-13 22:54:57.000000 alephvault-http-mongodb-storage-0.0.8/LICENSE
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      329 2022-06-27 16:27:59.040903 alephvault-http-mongodb-storage-0.0.8/PKG-INFO
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      101 2022-04-24 04:11:09.000000 alephvault-http-mongodb-storage-0.0.8/README.md
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2022-06-27 16:27:59.036903 alephvault-http-mongodb-storage-0.0.8/alephvault/
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2022-06-27 16:27:59.040903 alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        0 2022-04-14 15:54:19.000000 alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/__init__.py
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2022-06-27 16:27:59.040903 alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/core/
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        0 2022-04-22 01:53:21.000000 alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/core/__init__.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      206 2022-04-23 03:46:21.000000 alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/core/converters.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      154 2022-04-22 01:57:49.000000 alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/core/formats.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      840 2022-04-22 01:57:49.000000 alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/core/json.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     1359 2022-04-26 21:30:35.000000 alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/core/responses.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     2886 2022-04-22 02:00:03.000000 alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/core/validation.py
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2022-06-27 16:27:59.040903 alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/engine/
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        0 2022-04-17 23:26:28.000000 alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/engine/__init__.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     4470 2022-04-20 22:21:30.000000 alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/engine/path.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     7067 2022-06-27 16:19:29.000000 alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/engine/schemas.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)    30521 2022-06-27 16:21:14.000000 alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/flask_app.py
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2022-06-27 16:27:59.040903 alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/types/
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        0 2022-04-21 22:49:44.000000 alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/types/__init__.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     1158 2022-04-22 21:52:32.000000 alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/types/cursor.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     4698 2022-04-22 01:30:33.000000 alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/types/method_handlers.py
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2022-06-27 16:27:59.040903 alephvault-http-mongodb-storage-0.0.8/alephvault_http_mongodb_storage.egg-info/
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      329 2022-06-27 16:27:58.000000 alephvault-http-mongodb-storage-0.0.8/alephvault_http_mongodb_storage.egg-info/PKG-INFO
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      925 2022-06-27 16:27:59.000000 alephvault-http-mongodb-storage-0.0.8/alephvault_http_mongodb_storage.egg-info/SOURCES.txt
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        1 2022-06-27 16:27:58.000000 alephvault-http-mongodb-storage-0.0.8/alephvault_http_mongodb_storage.egg-info/dependency_links.txt
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      164 2022-06-27 16:27:58.000000 alephvault-http-mongodb-storage-0.0.8/alephvault_http_mongodb_storage.egg-info/requires.txt
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)       35 2022-06-27 16:27:58.000000 alephvault-http-mongodb-storage-0.0.8/alephvault_http_mongodb_storage.egg-info/top_level.txt
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2022-06-27 16:27:59.040903 alephvault-http-mongodb-storage-0.0.8/sample/
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        0 2022-04-23 02:33:10.000000 alephvault-http-mongodb-storage-0.0.8/sample/__init__.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     8966 2022-06-27 16:22:38.000000 alephvault-http-mongodb-storage-0.0.8/sample/universe_and_accounts.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)       38 2022-06-27 16:27:59.040903 alephvault-http-mongodb-storage-0.0.8/setup.cfg
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      731 2022-06-27 16:13:36.000000 alephvault-http-mongodb-storage-0.0.8/setup.py
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-02-08 00:34:44.949910 alephvault-http-mongodb-storage-0.0.9/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     1067 2022-04-13 22:54:57.000000 alephvault-http-mongodb-storage-0.0.9/LICENSE
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      329 2023-02-08 00:34:44.945910 alephvault-http-mongodb-storage-0.0.9/PKG-INFO
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      101 2022-04-24 04:11:09.000000 alephvault-http-mongodb-storage-0.0.9/README.md
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-02-08 00:34:44.941910 alephvault-http-mongodb-storage-0.0.9/alephvault/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-02-08 00:34:44.945910 alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        0 2022-04-14 15:54:19.000000 alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/__init__.py
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-02-08 00:34:44.945910 alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/core/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        0 2022-04-22 01:53:21.000000 alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/core/__init__.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      206 2022-04-23 03:46:21.000000 alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/core/converters.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      154 2022-04-22 01:57:49.000000 alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/core/formats.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      840 2022-04-22 01:57:49.000000 alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/core/json.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     1359 2022-04-26 21:30:35.000000 alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/core/responses.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     2886 2022-04-22 02:00:03.000000 alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/core/validation.py
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-02-08 00:34:44.945910 alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/engine/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        0 2022-04-17 23:26:28.000000 alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/engine/__init__.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     4470 2022-04-20 22:21:30.000000 alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/engine/path.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     7067 2022-06-27 16:19:29.000000 alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/engine/schemas.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)    30916 2023-02-08 00:33:59.000000 alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/flask_app.py
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-02-08 00:34:44.945910 alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/types/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        0 2022-04-21 22:49:44.000000 alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/types/__init__.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     1158 2022-04-22 21:52:32.000000 alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/types/cursor.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     4698 2022-04-22 01:30:33.000000 alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/types/method_handlers.py
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-02-08 00:34:44.945910 alephvault-http-mongodb-storage-0.0.9/alephvault_http_mongodb_storage.egg-info/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      329 2023-02-08 00:34:44.000000 alephvault-http-mongodb-storage-0.0.9/alephvault_http_mongodb_storage.egg-info/PKG-INFO
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      925 2023-02-08 00:34:44.000000 alephvault-http-mongodb-storage-0.0.9/alephvault_http_mongodb_storage.egg-info/SOURCES.txt
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        1 2023-02-08 00:34:44.000000 alephvault-http-mongodb-storage-0.0.9/alephvault_http_mongodb_storage.egg-info/dependency_links.txt
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      164 2023-02-08 00:34:44.000000 alephvault-http-mongodb-storage-0.0.9/alephvault_http_mongodb_storage.egg-info/requires.txt
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)       35 2023-02-08 00:34:44.000000 alephvault-http-mongodb-storage-0.0.9/alephvault_http_mongodb_storage.egg-info/top_level.txt
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-02-08 00:34:44.945910 alephvault-http-mongodb-storage-0.0.9/sample/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        0 2022-04-23 02:33:10.000000 alephvault-http-mongodb-storage-0.0.9/sample/__init__.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     8966 2022-06-27 16:22:38.000000 alephvault-http-mongodb-storage-0.0.9/sample/universe_and_accounts.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)       38 2023-02-08 00:34:44.949910 alephvault-http-mongodb-storage-0.0.9/setup.cfg
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      731 2023-02-08 00:30:26.000000 alephvault-http-mongodb-storage-0.0.9/setup.py
```

### Comparing `alephvault-http-mongodb-storage-0.0.8/LICENSE` & `alephvault-http-mongodb-storage-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/core/json.py` & `alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/core/json.py`

 * *Files identical despite different names*

### Comparing `alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/core/responses.py` & `alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/core/responses.py`

 * *Files identical despite different names*

### Comparing `alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/core/validation.py` & `alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/core/validation.py`

 * *Files identical despite different names*

### Comparing `alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/engine/path.py` & `alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/engine/path.py`

 * *Files identical despite different names*

### Comparing `alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/engine/schemas.py` & `alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/engine/schemas.py`

 * *Files identical despite different names*

### Comparing `alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/flask_app.py` & `alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/flask_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -367,15 +367,18 @@
             :return: Flask-compatible responses.
             """
 
             if not self._expect_verb(resource_definition, "create"):
                 return method_not_allowed()
 
             # Require the body to be json, and validate it.
-            if not request.is_json or not isinstance(request.json, dict):
+            try:
+                if not request.is_json or not isinstance(request.json, dict):
+                    raise Exception()
+            except:
                 return format_unexpected()
             validator = self._resource_validators[resource]
             request.json.pop('_id', None)
             self._logger.debug(f"POST /{resource} (type={resource_definition['type']}) "
                                f"with body: {request.json}")
             if validator.validate(request.json):
                 # Its "type" will be "list" or "simple".
@@ -436,15 +439,18 @@
             the incoming json body.
             :return: Flask-compatible responses.
             """
 
             if not self._expect_verb(resource_definition, "replace"):
                 return method_not_allowed()
 
-            if not request.is_json or not isinstance(request.json, dict):
+            try:
+                if not request.is_json or not isinstance(request.json, dict):
+                    raise Exception()
+            except:
                 return format_unexpected()
             # Process a "simple" resource.
             element = collection.find_one(filter=filter)
             if element:
                 validator = self._resource_validators[resource]
                 request.json.pop('_id', None)
                 self._logger.debug(f"PUT /{resource} (type=simple) "
@@ -474,15 +480,18 @@
             the incoming json body.
             :return: Flask-compatible responses.
             """
 
             if not self._expect_verb(resource_definition, "update"):
                 return method_not_allowed()
 
-            if not request.is_json or not isinstance(request.json, dict):
+            try:
+                if not request.is_json or not isinstance(request.json, dict):
+                    raise Exception()
+            except:
                 return format_unexpected()
             element = collection.find_one(filter=filter)
             if element:
                 _id = element["_id"]
                 self._logger.debug(f"PATCH /{resource} (type=simple) "
                                    f"with body: {request.json}")
                 element = _update_document(element, request.json)
@@ -564,15 +573,18 @@
             incoming json body.
             :return: Flask-compatible responses.
             """
 
             if not self._expect_verb(resource_definition, "replace"):
                 return method_not_allowed()
 
-            if not request.is_json or not isinstance(request.json, dict):
+            try:
+                if not request.is_json or not isinstance(request.json, dict):
+                    raise Exception()
+            except:
                 return format_unexpected()
             filter = {**filter, "_id": ObjectId(object_id)}
             element = collection.find_one(filter=filter)
             if element:
                 validator = self._resource_validators[resource]
                 request.json.pop('_id', None)
                 self._logger.debug(f"PUT /{resource} (type=list) "
@@ -602,15 +614,18 @@
             incoming json body.
             :return: Flask-compatible responses.
             """
 
             if not self._expect_verb(resource_definition, "update"):
                 return method_not_allowed()
 
-            if not request.is_json or not isinstance(request.json, dict):
+            try:
+                if not request.is_json or not isinstance(request.json, dict):
+                    raise Exception()
+            except:
                 return format_unexpected()
             filter = {**filter, "_id": ObjectId(object_id)}
             element = collection.find_one(filter=filter)
             if element:
                 element = _update_document(element, request.json)
                 validator = self._resource_validators[resource]
                 self._logger.debug(f"PUT /{resource} (type=list) "
```

### Comparing `alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/types/cursor.py` & `alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/types/cursor.py`

 * *Files identical despite different names*

### Comparing `alephvault-http-mongodb-storage-0.0.8/alephvault/http_storage/types/method_handlers.py` & `alephvault-http-mongodb-storage-0.0.9/alephvault/http_storage/types/method_handlers.py`

 * *Files identical despite different names*

### Comparing `alephvault-http-mongodb-storage-0.0.8/alephvault_http_mongodb_storage.egg-info/SOURCES.txt` & `alephvault-http-mongodb-storage-0.0.9/alephvault_http_mongodb_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alephvault-http-mongodb-storage-0.0.8/sample/universe_and_accounts.py` & `alephvault-http-mongodb-storage-0.0.9/sample/universe_and_accounts.py`

 * *Files identical despite different names*

### Comparing `alephvault-http-mongodb-storage-0.0.8/setup.py` & `alephvault-http-mongodb-storage-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='alephvault-http-mongodb-storage',
-    version='0.0.8',
+    version='0.0.9',
     packages=find_namespace_packages(),
     url='https://github.com/AlephVault/http-mongodb-storage',
     license='MIT',
     author='luismasuelli',
     author_email='luismasuelli@hotmail.com',
     description='A lightweight server to work as a simple storage for games, done with MongoDB and Flask',
     install_requires=[
```

