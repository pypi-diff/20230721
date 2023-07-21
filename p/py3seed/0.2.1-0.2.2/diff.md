# Comparing `tmp/py3seed-0.2.1.tar.gz` & `tmp/py3seed-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3seed-0.2.1.tar", last modified: Wed Jul 19 07:50:45 2023, max compression
+gzip compressed data, was "py3seed-0.2.2.tar", last modified: Fri Jul 21 09:05:34 2023, max compression
```

## Comparing `py3seed-0.2.1.tar` & `py3seed-0.2.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:50:45.548194 py3seed-0.2.1/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.2.1/LICENSE
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-19 07:50:45.548471 py3seed-0.2.1/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.2.1/README.md
--rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.2.1/pyproject.toml
--rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-19 07:50:45.549167 py3seed-0.2.1/setup.cfg
--rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.2.1/setup.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:50:45.535984 py3seed-0.2.1/src/
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:50:45.542012 py3seed-0.2.1/src/py3seed/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.2.1/src/py3seed/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.2.1/src/py3seed/__main__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.2.1/src/py3seed/admin.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6458 2023-07-10 03:55:28.000000 py3seed-0.2.1/src/py3seed/cachesupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:50:45.545365 py3seed-0.2.1/src/py3seed/commands/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.2.1/src/py3seed/commands/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    21146 2023-07-19 07:50:14.000000 py3seed-0.2.1/src/py3seed/commands/gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.2.1/src/py3seed/error.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.2.1/src/py3seed/inflection.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.2.1/src/py3seed/log.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.2.1/src/py3seed/merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-18 01:28:13.000000 py3seed-0.2.1/src/py3seed/model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.2.1/src/py3seed/mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14673 2023-07-19 03:29:37.000000 py3seed-0.2.1/src/py3seed/utils.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.2.1/src/py3seed/websupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:50:45.544276 py3seed-0.2.1/src/py3seed.egg-info/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-19 07:50:45.000000 py3seed-0.2.1/src/py3seed.egg-info/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-19 07:50:45.000000 py3seed-0.2.1/src/py3seed.egg-info/SOURCES.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-19 07:50:45.000000 py3seed-0.2.1/src/py3seed.egg-info/dependency_links.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-19 07:50:45.000000 py3seed-0.2.1/src/py3seed.egg-info/entry_points.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-19 07:50:45.000000 py3seed-0.2.1/src/py3seed.egg-info/requires.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-19 07:50:45.000000 py3seed-0.2.1/src/py3seed.egg-info/top_level.txt
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:50:45.547804 py3seed-0.2.1/tests/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     3216 2022-12-09 02:58:18.000000 py3seed-0.2.1/tests/test_cachesupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6599 2023-07-18 07:07:02.000000 py3seed-0.2.1/tests/test_gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.2.1/tests/test_merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.2.1/tests/test_model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.2.1/tests/test_mongosupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-21 09:05:34.024086 py3seed-0.2.2/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.2.2/LICENSE
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-21 09:05:34.024207 py3seed-0.2.2/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.2.2/README.md
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.2.2/pyproject.toml
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-21 09:05:34.024801 py3seed-0.2.2/setup.cfg
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.2.2/setup.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-21 09:05:34.002187 py3seed-0.2.2/src/
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-21 09:05:34.014601 py3seed-0.2.2/src/py3seed/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.2.2/src/py3seed/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.2.2/src/py3seed/__main__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.2.2/src/py3seed/admin.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7571 2023-07-21 09:02:47.000000 py3seed-0.2.2/src/py3seed/cachesupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-21 09:05:34.018261 py3seed-0.2.2/src/py3seed/commands/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.2.2/src/py3seed/commands/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    21146 2023-07-19 07:50:14.000000 py3seed-0.2.2/src/py3seed/commands/gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.2.2/src/py3seed/error.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.2.2/src/py3seed/inflection.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.2.2/src/py3seed/log.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.2.2/src/py3seed/merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-18 01:28:13.000000 py3seed-0.2.2/src/py3seed/model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.2.2/src/py3seed/mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14673 2023-07-19 03:29:37.000000 py3seed-0.2.2/src/py3seed/utils.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.2.2/src/py3seed/websupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-21 09:05:34.017204 py3seed-0.2.2/src/py3seed.egg-info/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-21 09:05:33.000000 py3seed-0.2.2/src/py3seed.egg-info/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-21 09:05:33.000000 py3seed-0.2.2/src/py3seed.egg-info/SOURCES.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-21 09:05:33.000000 py3seed-0.2.2/src/py3seed.egg-info/dependency_links.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-21 09:05:33.000000 py3seed-0.2.2/src/py3seed.egg-info/entry_points.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-21 09:05:33.000000 py3seed-0.2.2/src/py3seed.egg-info/requires.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-21 09:05:33.000000 py3seed-0.2.2/src/py3seed.egg-info/top_level.txt
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-21 09:05:34.023473 py3seed-0.2.2/tests/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     4032 2023-07-21 09:03:11.000000 py3seed-0.2.2/tests/test_cachesupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6599 2023-07-18 07:07:02.000000 py3seed-0.2.2/tests/test_gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.2.2/tests/test_merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.2.2/tests/test_model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.2.2/tests/test_mongosupport.py
```

### Comparing `py3seed-0.2.1/LICENSE` & `py3seed-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.1/PKG-INFO` & `py3seed-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.2.1
+Version: 0.2.2
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.2.1/setup.cfg` & `py3seed-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py3seed
-version = 0.2.1
+version = 0.2.2
 author = Samuel Feng
 author_email = okosioc@gmail.com
 description = A package that bootstraps your project by simple data models definition and auto api and user interface generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/okosioc/pyseed
 project_urls =
```

### Comparing `py3seed-0.2.1/src/py3seed/__init__.py` & `py3seed-0.2.2/src/py3seed/__init__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.1/src/py3seed/__main__.py` & `py3seed-0.2.2/src/py3seed/__main__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.1/src/py3seed/admin.py` & `py3seed-0.2.2/src/py3seed/admin.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.1/src/py3seed/cachesupport.py` & `py3seed-0.2.2/src/py3seed/cachesupport.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 
     :copyright: (c) 2021 by weiminfeng.
     :date: 2022/9/14
 """
 from py3seed import DataError, BaseModel, Pagination, inflection
 
 # {model_name:[dict]}
-# Note: Do no store model object directly, as it may cause concurrent accessing issue
+# Note: Do no store model object directly but parsed dict object, as it may cause concurrent accessing issue
 CACHES = {}
 
 
 class CacheModel(BaseModel):
     """ Model in cache. """
-    # TODO: Support __keys__ to mark the key field to be unique
-    __keys__ = []
+    # a user-friendly unique field name
+    # NOTE: this field should be reqired
+    __key__ = None
 
     # id field definition
     __id_name__ = 'id'
     __id_type__ = int
 
     # id field
     id: int = None
@@ -139,19 +140,30 @@
         records = cls.find(filter_, skip=start, limit=per_page, **kwargs)
         pagination = Pagination(page, per_page, count)
         return records, pagination
 
     @classmethod
     def delete_many(cls, filter_=None, **kwargs):
         collection = cls.get_collection(**kwargs)
-        indexes = [index for index, record in enumerate(collection) if cls.match_record(record, filter_)]
-        for index in indexes:
-            del collection[index]
+        start = 0
+        count = 0
+        while start < len(collection):
+            found = -1
+            for i, record in enumerate(collection, start):
+                if cls.match_record(record, filter_):
+                    found = i
+                    break
+            #
+            if found >= 0:
+                del collection[found]
+                count += 1
+            else:
+                start = len(collection)
         #
-        return True
+        return count
 
     #
     #
     # Instance level methods
     #
     #
 
@@ -161,26 +173,42 @@
         if errors:
             raise DataError(f'It is an illegal {self.__class__.__name__} with errors, {errors}')
         #
         collection = self.get_collection(**kwargs)
         if insert_with_id or not self.id:
             # get the max id, start from 1
             self.id = max(list(map(lambda x: x['id'], collection)) or [0]) + 1
+            # check duplicated key value
+            if self.__key__:
+                key = self.__key__
+                key_value = getattr(self, key)
+                existing = next((record for record in collection if record[key] == key_value), None)
+                if existing:
+                    raise DataError(f'Duplicate key value: {key_value}')
+            #
             collection.append(self.dict())
             return True
         else:
-            indexes = [index for index, record in enumerate(collection) if record['id'] == self.id]
-            if indexes:
-                collection[indexes[0]] = self.dict()
+            index = next((index for index, record in enumerate(collection) if record['id'] == self.id), -1)
+            if index >= 0:
+                # check duplicated key value
+                if self.__key__:
+                    key = self.__key__
+                    key_value = getattr(self, key)
+                    existing = next((record for record in collection if record['id'] != self.id and record[key] == key_value), None)
+                    if existing:
+                        raise DataError(f'Duplicate key value: {key_value}')
+                #
+                collection[index] = self.dict()
                 return True
             else:
                 return False
 
     def delete(self, **kwargs):
         """ Delete self form cache. """
         collection = self.get_collection(**kwargs)
-        indexes = [index for index, record in enumerate(collection) if record['id'] == self.id]
-        if indexes:
-            del collection[indexes[0]]
+        index = next((index for index, record in enumerate(collection) if record['id'] == self.id), -1)
+        if index >= 0:
+            del collection[index]
             return True
         else:
             return False
```

### Comparing `py3seed-0.2.1/src/py3seed/commands/gen.py` & `py3seed-0.2.2/src/py3seed/commands/gen.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.1/src/py3seed/error.py` & `py3seed-0.2.2/src/py3seed/error.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.1/src/py3seed/inflection.py` & `py3seed-0.2.2/src/py3seed/inflection.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.1/src/py3seed/log.py` & `py3seed-0.2.2/src/py3seed/log.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.1/src/py3seed/merge3.py` & `py3seed-0.2.2/src/py3seed/merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.1/src/py3seed/model.py` & `py3seed-0.2.2/src/py3seed/model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.1/src/py3seed/mongosupport.py` & `py3seed-0.2.2/src/py3seed/mongosupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.1/src/py3seed/utils.py` & `py3seed-0.2.2/src/py3seed/utils.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.1/src/py3seed/websupport.py` & `py3seed-0.2.2/src/py3seed/websupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.1/src/py3seed.egg-info/PKG-INFO` & `py3seed-0.2.2/src/py3seed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.2.1
+Version: 0.2.2
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.2.1/src/py3seed.egg-info/SOURCES.txt` & `py3seed-0.2.2/src/py3seed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.1/tests/test_cachesupport.py` & `py3seed-0.2.2/tests/test_cachesupport.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,17 @@
     :copyright: (c) 2021 by weiminfeng.
     :date: 2022/9/14
 """
 import re
 from datetime import datetime
 from typing import List
 
-from py3seed import CacheModel, RelationField
+import pytest
+
+from py3seed import CacheModel, RelationField, DataError
 
 
 class CTeam(CacheModel):
     """ Cache team definition"""
     name: str
     update_time: datetime = None
     create_time: datetime = datetime.now
@@ -27,14 +29,16 @@
     name: str
     email: str
     phone: str = None
     team: CTeam = RelationField(back_field_name='members', back_field_is_list=True, back_field_order=[('team_join_time', -1)])
     team_join_time: datetime = None
     update_time: datetime = None
     create_time: datetime = datetime.now
+    #
+    __key__ = 'email'
 
 
 class CProject(CacheModel):
     """ Cache project defintion. """
     name: str
     members: List[CUser] = RelationField(required=False, back_field_name='projects', back_field_is_list=True, back_field_order=[('create_time', -1)])
     update_time: datetime = None
@@ -48,17 +52,15 @@
     assert cuser_schema['relations'] == ['CTeam', 'CProject']
     assert cuser_schema['id_name'] == 'id'
     assert cuser_schema['id_type'] == 'int'
     cproject_schema = CProject.schema()
     assert cproject_schema['relations'] == ['CUser']
 
     # Init
-    assert CUser.delete_many()
     assert CUser.count() == 0
-    assert CTeam.delete_many()
     assert CTeam.count() == 0
 
     # C
     team1 = CTeam(name='team1')
     team1.save()
     user1 = CUser(name='user1', email='user1@dev', phone='13800138000', team=team1, team_join_time=datetime.now())
     user1.save()
@@ -71,14 +73,20 @@
     # Q
     assert len(CUser.find({'name': {'$regex': re.compile('^u')}})) == 1
     assert len(CUser.find({'phone': {'$regex': re.compile('^138')}})) == 1
 
     # U
     user2 = CUser(name='user3', email='user2@dev', team=team1, team_join_time=datetime.now())
     user2.save()
+    user2.email = 'user1@dev'
+    with pytest.raises(DataError) as exc_info:
+        user2.save()
+    assert 'Duplicate key' in str(exc_info.value)
+    user2.email = 'user2@dev'
+    #
     user2.name = 'user2'
     user2.save()
     assert user2.id == 2
     assert len(team1.members) == 2
 
     # Q
     assert CUser.find_by_ids([1, 2])[1].name == user2.name
@@ -100,16 +108,32 @@
     })
     user3.save()
     assert user3.id == 2
     assert CUser.find_one(2).name == 'user3'
 
     # relation many to one
     del team1.members
-    assert list(map(lambda x:x.id, team1.members)) == [user3.id, user1.id]  # sort DESCENDING
+    assert list(map(lambda x: x.id, team1.members)) == [user3.id, user1.id]  # sort DESCENDING
 
     # relation many-to-many
     project1 = CProject(name='project1', members=[user1, user2])
     project1.save()
     assert project1.members_ids == [user1.id, user2.id]
     project2 = CProject(name='project2', members=[user2])
     project2.save()
     assert len(user2.projects) == 2
+
+    # DM
+    user11 = CUser(name='user11', email='user11@dev', team=team1, team_join_time=datetime.now())
+    user11.save()
+    user4 = CUser(name='user4', email='user4@dev', team=team1, team_join_time=datetime.now())
+    user4.save()
+    user5 = CUser(name='user5', email='user5@dev', team=team1, team_join_time=datetime.now())
+    user5.save()
+    # delete 2
+    assert CUser.delete_many({'name': {'$regex': re.compile('^user1')}}) == 2
+    # delete first
+    assert CUser.delete_many({'name': 'user3'}) == 1
+    # delete last
+    assert CUser.delete_many({'name': 'user5'}) == 1
+    # only remains user 4
+    assert CUser.count() == 1
```

### Comparing `py3seed-0.2.1/tests/test_gen.py` & `py3seed-0.2.2/tests/test_gen.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.1/tests/test_merge3.py` & `py3seed-0.2.2/tests/test_merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.1/tests/test_model.py` & `py3seed-0.2.2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.1/tests/test_mongosupport.py` & `py3seed-0.2.2/tests/test_mongosupport.py`

 * *Files identical despite different names*

