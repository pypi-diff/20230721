# Comparing `tmp/panther-1.7.8.tar.gz` & `tmp/panther-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panther-1.7.8.tar", last modified: Fri Jun 30 10:50:52 2023, max compression
+gzip compressed data, was "panther-1.7.9.tar", last modified: Tue Jul  4 19:40:00 2023, max compression
```

## Comparing `panther-1.7.8.tar` & `panther-1.7.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:50:52.585147 panther-1.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-30 10:50:35.000000 panther-1.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-06-30 10:50:52.585147 panther-1.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-06-30 10:50:35.000000 panther-1.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:50:52.581146 panther-1.7.8/panther/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 10:50:35.000000 panther-1.7.8/panther/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-30 10:50:35.000000 panther-1.7.8/panther/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-06-30 10:50:35.000000 panther-1.7.8/panther/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-30 10:50:35.000000 panther-1.7.8/panther/authentications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-30 10:50:35.000000 panther-1.7.8/panther/caching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:50:52.581146 panther-1.7.8/panther/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:50:35.000000 panther-1.7.8/panther/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-30 10:50:35.000000 panther-1.7.8/panther/cli/create_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-30 10:50:35.000000 panther-1.7.8/panther/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-30 10:50:35.000000 panther-1.7.8/panther/cli/monitor_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-30 10:50:35.000000 panther-1.7.8/panther/cli/run_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-30 10:50:35.000000 panther-1.7.8/panther/cli/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-06-30 10:50:35.000000 panther-1.7.8/panther/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-30 10:50:35.000000 panther-1.7.8/panther/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:50:52.581146 panther-1.7.8/panther/db/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-30 10:50:35.000000 panther-1.7.8/panther/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-30 10:50:35.000000 panther-1.7.8/panther/db/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-30 10:50:35.000000 panther-1.7.8/panther/db/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:50:52.581146 panther-1.7.8/panther/db/queries/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 10:50:35.000000 panther-1.7.8/panther/db/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-30 10:50:35.000000 panther-1.7.8/panther/db/queries/mongodb_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-30 10:50:35.000000 panther-1.7.8/panther/db/queries/pantherdb_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-06-30 10:50:35.000000 panther-1.7.8/panther/db/queries/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-30 10:50:35.000000 panther-1.7.8/panther/db/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-30 10:50:35.000000 panther-1.7.8/panther/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-30 10:50:35.000000 panther-1.7.8/panther/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-06-30 10:50:35.000000 panther-1.7.8/panther/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:50:52.585147 panther-1.7.8/panther/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-30 10:50:35.000000 panther-1.7.8/panther/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-30 10:50:35.000000 panther-1.7.8/panther/middlewares/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-30 10:50:35.000000 panther-1.7.8/panther/middlewares/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-30 10:50:35.000000 panther-1.7.8/panther/middlewares/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-30 10:50:35.000000 panther-1.7.8/panther/middlewares/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:50:52.585147 panther-1.7.8/panther/panel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:50:35.000000 panther-1.7.8/panther/panel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-30 10:50:35.000000 panther-1.7.8/panther/panel/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-30 10:50:35.000000 panther-1.7.8/panther/panel/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-30 10:50:35.000000 panther-1.7.8/panther/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-30 10:50:35.000000 panther-1.7.8/panther/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-30 10:50:35.000000 panther-1.7.8/panther/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-06-30 10:50:35.000000 panther-1.7.8/panther/routings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-30 10:50:35.000000 panther-1.7.8/panther/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-30 10:50:35.000000 panther-1.7.8/panther/throttling.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-30 10:50:35.000000 panther-1.7.8/panther/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:50:52.581146 panther-1.7.8/panther.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-06-30 10:50:52.000000 panther-1.7.8/panther.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-30 10:50:52.000000 panther-1.7.8/panther.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:50:52.000000 panther-1.7.8/panther.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-30 10:50:52.000000 panther-1.7.8/panther.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-30 10:50:52.000000 panther-1.7.8/panther.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 10:50:52.000000 panther-1.7.8/panther.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-30 10:50:35.000000 panther-1.7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 10:50:52.585147 panther-1.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-30 10:50:35.000000 panther-1.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:40:00.239499 panther-1.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-04 19:39:46.000000 panther-1.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-04 19:40:00.239499 panther-1.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-07-04 19:39:46.000000 panther-1.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:40:00.235499 panther-1.7.9/panther/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-04 19:39:46.000000 panther-1.7.9/panther/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-04 19:39:46.000000 panther-1.7.9/panther/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-07-04 19:39:46.000000 panther-1.7.9/panther/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-04 19:39:46.000000 panther-1.7.9/panther/authentications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-04 19:39:46.000000 panther-1.7.9/panther/caching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:40:00.235499 panther-1.7.9/panther/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 19:39:46.000000 panther-1.7.9/panther/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-04 19:39:46.000000 panther-1.7.9/panther/cli/create_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-04 19:39:46.000000 panther-1.7.9/panther/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-04 19:39:46.000000 panther-1.7.9/panther/cli/monitor_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-04 19:39:46.000000 panther-1.7.9/panther/cli/run_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-04 19:39:46.000000 panther-1.7.9/panther/cli/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-07-04 19:39:46.000000 panther-1.7.9/panther/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-04 19:39:46.000000 panther-1.7.9/panther/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:40:00.239499 panther-1.7.9/panther/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-04 19:39:46.000000 panther-1.7.9/panther/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-04 19:39:46.000000 panther-1.7.9/panther/db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-04 19:39:46.000000 panther-1.7.9/panther/db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:40:00.239499 panther-1.7.9/panther/db/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-04 19:39:46.000000 panther-1.7.9/panther/db/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-04 19:39:46.000000 panther-1.7.9/panther/db/queries/mongodb_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-04 19:39:46.000000 panther-1.7.9/panther/db/queries/pantherdb_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-07-04 19:39:46.000000 panther-1.7.9/panther/db/queries/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-04 19:39:46.000000 panther-1.7.9/panther/db/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-04 19:39:46.000000 panther-1.7.9/panther/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-04 19:39:46.000000 panther-1.7.9/panther/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-07-04 19:39:46.000000 panther-1.7.9/panther/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:40:00.239499 panther-1.7.9/panther/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-04 19:39:46.000000 panther-1.7.9/panther/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-04 19:39:46.000000 panther-1.7.9/panther/middlewares/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-04 19:39:46.000000 panther-1.7.9/panther/middlewares/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-04 19:39:46.000000 panther-1.7.9/panther/middlewares/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-04 19:39:46.000000 panther-1.7.9/panther/middlewares/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:40:00.239499 panther-1.7.9/panther/panel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 19:39:46.000000 panther-1.7.9/panther/panel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-04 19:39:46.000000 panther-1.7.9/panther/panel/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-04 19:39:46.000000 panther-1.7.9/panther/panel/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-04 19:39:46.000000 panther-1.7.9/panther/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-04 19:39:46.000000 panther-1.7.9/panther/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-04 19:39:46.000000 panther-1.7.9/panther/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-07-04 19:39:46.000000 panther-1.7.9/panther/routings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-04 19:39:46.000000 panther-1.7.9/panther/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-04 19:39:46.000000 panther-1.7.9/panther/throttling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-04 19:39:46.000000 panther-1.7.9/panther/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:40:00.235499 panther-1.7.9/panther.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-04 19:40:00.000000 panther-1.7.9/panther.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-04 19:40:00.000000 panther-1.7.9/panther.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 19:40:00.000000 panther-1.7.9/panther.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-04 19:40:00.000000 panther-1.7.9/panther.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-04 19:40:00.000000 panther-1.7.9/panther.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 19:40:00.000000 panther-1.7.9/panther.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-04 19:39:46.000000 panther-1.7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 19:40:00.239499 panther-1.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-04 19:39:46.000000 panther-1.7.9/setup.py
```

### Comparing `panther-1.7.8/LICENSE` & `panther-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/PKG-INFO` & `panther-1.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panther
-Version: 1.7.8
+Version: 1.7.9
 Summary: Fast &  Friendly, Web Framework For Building Async APIs
 Home-page: https://github.com/alirn76/panther
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `panther-1.7.8/README.md` & `panther-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/panther/_utils.py` & `panther-1.7.9/panther/_utils.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/panther/app.py` & `panther-1.7.9/panther/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
             return data
 
         return self.serialize_with_output_model(data)
 
     def serialize_with_output_model(self, data: any):
         # Dict
         if isinstance(data, dict):
-            return self.output_model(**data).dict()
+            return self.output_model(**data).model_dump()
 
         # Iterable
         elif isinstance(data, IterableDataTypes):
             return [self.serialize_with_output_model(d) for d in data]
 
         # Str | Bool
         raise TypeError('Type of Response data is not match with output_model. '
```

### Comparing `panther-1.7.8/panther/authentications.py` & `panther-1.7.9/panther/authentications.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/panther/caching.py` & `panther-1.7.9/panther/caching.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/panther/cli/create_command.py` & `panther-1.7.9/panther/cli/create_command.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/panther/cli/main.py` & `panther-1.7.9/panther/cli/main.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/panther/cli/monitor_command.py` & `panther-1.7.9/panther/cli/monitor_command.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/panther/cli/run_command.py` & `panther-1.7.9/panther/cli/run_command.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/panther/cli/template.py` & `panther-1.7.9/panther/cli/template.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/panther/cli/utils.py` & `panther-1.7.9/panther/cli/utils.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/panther/configs.py` & `panther-1.7.9/panther/configs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from typing import TypedDict
 from datetime import timedelta
 from dataclasses import dataclass
-from pydantic.main import ModelMetaclass
+from pydantic._internal._model_construction import ModelMetaclass
 
 from panther.throttling import Throttling
 
 
 @dataclass(frozen=True)
 class JWTConfig:
     key: str
```

### Comparing `panther-1.7.8/panther/db/connection.py` & `panther-1.7.9/panther/db/connection.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/panther/db/models.py` & `panther-1.7.9/panther/db/models.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/panther/db/queries/mongodb_queries.py` & `panther-1.7.9/panther/db/queries/mongodb_queries.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/panther/db/queries/pantherdb_queries.py` & `panther-1.7.9/panther/db/queries/pantherdb_queries.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/panther/db/queries/queries.py` & `panther-1.7.9/panther/db/queries/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     # # # # # Find # # # # #
     @classmethod
     @log_query
     def find_one(cls, _data: dict = None, /, **kwargs) -> Self | None:
         """
         example:
             >>> from example.app.models import User
-            >>> User.find(id=1)
+            >>> User.find_one(id=1)
         """
         return super().find_one(_data, **kwargs)
 
     @classmethod
     @log_query
     def find(cls, _data: dict = None, /, **kwargs) -> list[Self]:
         """
```

### Comparing `panther-1.7.8/panther/db/utils.py` & `panther-1.7.9/panther/db/utils.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/panther/exceptions.py` & `panther-1.7.9/panther/exceptions.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/panther/logger.py` & `panther-1.7.9/panther/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,30 +16,30 @@
 
     LOGGER_NAME: str = 'panther-logger'
     DEFAULT_LOG_FORMAT: str = '%(levelprefix)s | %(asctime)s | %(message)s'
     FILE_LOG_FORMAT: str = '%(asctime)s | %(message)s'
     LOG_LEVEL: str = 'DEBUG'
     MAX_FILE_SIZE: int = 1024 * 1024 * 100  # 100 MB
 
-    version = 1
-    disable_existing_loggers = False
+    version: int = 1
+    disable_existing_loggers: bool = False
 
-    formatters = {
+    formatters: dict = {
         'default': {
             '()': 'uvicorn.logging.DefaultFormatter',
             'fmt': DEFAULT_LOG_FORMAT,
             'datefmt': '%Y-%m-%d %H:%M:%S',
         },
         'file_formatter': {
             '()': 'uvicorn.logging.DefaultFormatter',
             'fmt': FILE_LOG_FORMAT,
             'datefmt': '%Y-%m-%d %H:%M:%S',
         },
     }
-    handlers = {
+    handlers: dict = {
         'monitoring_file': {
             'formatter': 'file_formatter',
             'filename': LOGS_DIR / 'monitoring.log',
             'class': 'logging.handlers.RotatingFileHandler',
             'maxBytes': MAX_FILE_SIZE,  # 100 MB,
             'backupCount': 3,
         },
@@ -59,15 +59,15 @@
         },
         'default': {
             'formatter': 'default',
             'class': 'logging.StreamHandler',
             'stream': 'ext://sys.stderr',
         },
     }
-    loggers = {
+    loggers: dict = {
         'panther': {
             'handlers': ['default', 'file'],
             'level': LOG_LEVEL,
         },
         'monitoring': {
             'handlers': ['monitoring_file'],
             'level': LOG_LEVEL,
@@ -75,11 +75,11 @@
         'query': {
             'handlers': ['default', 'query_file'],
             'level': LOG_LEVEL,
         },
     }
 
 
-dictConfig(LogConfig().dict())
+dictConfig(LogConfig().model_dump())
 logger = logging.getLogger('panther')
 query_logger = logging.getLogger('query')
 monitoring_logger = logging.getLogger('monitoring')
```

### Comparing `panther-1.7.8/panther/main.py` & `panther-1.7.9/panther/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import ast
 import asyncio
 from pathlib import Path
 from runpy import run_path
-from pydantic.main import ModelMetaclass
+from pydantic._internal._model_construction import ModelMetaclass
 
 from panther import status
 from panther.request import Request
 from panther.response import Response
 from panther.exceptions import APIException
 from panther.configs import JWTConfig, config
 from panther.middlewares.base import BaseMiddleware
```

### Comparing `panther-1.7.8/panther/middlewares/monitoring.py` & `panther-1.7.9/panther/middlewares/monitoring.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/panther/middlewares/redis.py` & `panther-1.7.9/panther/middlewares/redis.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/panther/panel/apis.py` & `panther-1.7.9/panther/panel/apis.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/panther/request.py` & `panther-1.7.9/panther/request.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/panther/response.py` & `panther-1.7.9/panther/response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import orjson as json
 from types import NoneType
-from pydantic.main import BaseModel as PydanticBaseModel
+from pydantic import BaseModel as PydanticBaseModel
 
 ResponseDataTypes = int | dict | list | tuple | set | str | bool | NoneType
 IterableDataTypes = list | tuple | set
 
 
 class Response:
     def __init__(self, data: ResponseDataTypes = None, status_code: int = 200):
@@ -39,14 +39,14 @@
 
     @classmethod
     def clean_data_type(cls, data: any):
         """
         Make sure the response data is only ResponseDataTypes or Iterable of ResponseDataTypes
         """
         if issubclass(type(data), PydanticBaseModel):
-            return data.dict()
+            return data.model_dump()
 
         elif isinstance(data, IterableDataTypes):
             return [cls.clean_data_type(d) for d in data]
 
         else:
             return data
```

### Comparing `panther-1.7.8/panther/routings.py` & `panther-1.7.9/panther/routings.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/panther/status.py` & `panther-1.7.9/panther/status.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/panther/utils.py` & `panther-1.7.9/panther/utils.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/panther.egg-info/PKG-INFO` & `panther-1.7.9/panther.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panther
-Version: 1.7.8
+Version: 1.7.9
 Summary: Fast &  Friendly, Web Framework For Building Async APIs
 Home-page: https://github.com/alirn76/panther
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `panther-1.7.8/panther.egg-info/SOURCES.txt` & `panther-1.7.9/panther.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panther-1.7.8/setup.py` & `panther-1.7.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,21 +38,21 @@
     entry_points={
         'console_scripts': ['panther=panther.cli.main:start'],
     },
     package_data={
         'panther': ['cli/*'],
     },
     install_requires=[
-        'bpython>=0.24',
-        'bson>=0.5.10',
-        'httptools>=0.5.0',
-        'pantherdb>=1.2.3',
-        'pydantic>=1.10.7',
-        'redis>=4.5.3',
-        'rich>=13.3.2',
-        'uvicorn>=0.21.1',
-        'uvloop>=0.17.0',
-        'watchfiles>=0.18.1',
-        'python-jose==3.3.0',
+        'bpython~=0.24',
+        'bson~=0.5',
+        'httptools~=0.5',
+        'pantherdb~=1.2',
+        'pydantic~=2.0',
+        'redis~=4.5',
+        'rich~=13.3',
+        'uvicorn~=0.21',
+        'uvloop~=0.17',
+        'watchfiles~=0.18',
+        'python-jose~=3.3',
     ],
     extras_require=EXTRAS_REQUIRE,
 )
```

