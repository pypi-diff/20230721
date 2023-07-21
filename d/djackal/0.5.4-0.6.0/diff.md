# Comparing `tmp/djackal-0.5.4.tar.gz` & `tmp/djackal-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djackal-0.5.4.tar", max compression
+gzip compressed data, was "djackal-0.6.0.tar", max compression
```

## Comparing `djackal-0.5.4.tar` & `djackal-0.6.0.tar`

### file list

```diff
@@ -1,51 +1,50 @@
--rw-r--r--   0        0        0     1068 2021-04-27 09:26:04.461893 djackal-0.5.4/LICENSE
--rw-r--r--   0        0        0      484 2022-01-14 07:38:42.023715 djackal-0.5.4/README.md
--rw-r--r--   0        0        0        0 2021-04-27 10:13:03.376108 djackal-0.5.4/djackal/__init__.py
--rw-r--r--   0        0        0      118 2021-04-28 13:22:14.818993 djackal-0.5.4/djackal/apps.py
--rw-r--r--   0        0        0      541 2021-11-23 06:18:24.021837 djackal-0.5.4/djackal/erra.py
--rw-r--r--   0        0        0     2614 2022-04-16 11:25:48.492286 djackal-0.5.4/djackal/exceptions.py
--rw-r--r--   0        0        0      227 2021-02-25 12:42:37.423177 djackal-0.5.4/djackal/expressions.py
--rw-r--r--   0        0        0       34 2021-04-29 09:48:08.913022 djackal-0.5.4/djackal/fields/__init__.py
--rw-r--r--   0        0        0     2145 2023-04-12 19:08:44.501732 djackal-0.5.4/djackal/fields/json_field.py
--rw-r--r--   0        0        0     1165 2021-06-17 15:10:32.345990 djackal-0.5.4/djackal/initializer.py
--rw-r--r--   0        0        0      161 2022-06-01 07:29:57.471726 djackal-0.5.4/djackal/loaders.py
--rw-r--r--   0        0        0        0 2021-02-25 12:42:37.423177 djackal-0.5.4/djackal/management/__init__.py
--rw-r--r--   0        0        0        0 2021-02-25 12:42:37.423177 djackal-0.5.4/djackal/management/commands/__init__.py
--rw-r--r--   0        0        0      370 2021-06-17 15:10:32.349990 djackal-0.5.4/djackal/management/commands/init.py
--rw-r--r--   0        0        0       36 2023-04-12 19:08:44.501732 djackal-0.5.4/djackal/model_mixins/__init__.py
--rw-r--r--   0        0        0     1222 2023-04-12 19:08:44.501732 djackal-0.5.4/djackal/model_mixins/extra_mixin.py
--rw-r--r--   0        0        0     2243 2022-06-01 07:29:57.471726 djackal-0.5.4/djackal/pagination.py
--rw-r--r--   0        0        0     2699 2022-04-16 11:25:48.492286 djackal-0.5.4/djackal/permissions.py
--rw-r--r--   0        0        0     2785 2023-04-12 19:08:44.501732 djackal-0.5.4/djackal/query_filter.py
--rw-r--r--   0        0        0     1606 2021-06-28 06:44:58.185826 djackal-0.5.4/djackal/serializers.py
--rw-r--r--   0        0        0     2953 2023-04-12 19:08:44.501732 djackal-0.5.4/djackal/settings.py
--rw-r--r--   0        0        0     1638 2022-06-01 07:29:57.471726 djackal-0.5.4/djackal/shortcuts.py
--rw-r--r--   0        0        0        0 2021-06-17 15:10:32.349990 djackal-0.5.4/djackal/storage/__init__.py
--rw-r--r--   0        0        0      126 2021-06-17 15:10:32.349990 djackal-0.5.4/djackal/storage/apps.py
--rw-r--r--   0        0        0      404 2021-06-17 15:10:32.349990 djackal-0.5.4/djackal/storage/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2021-06-17 15:10:32.349990 djackal-0.5.4/djackal/storage/migrations/__init__.py
--rw-r--r--   0        0        0      658 2021-06-17 15:10:32.349990 djackal-0.5.4/djackal/storage/models.py
--rw-r--r--   0        0        0      760 2022-06-01 07:29:12.961130 djackal-0.5.4/djackal/tests.py
--rw-r--r--   0        0        0      751 2023-04-12 19:08:44.501732 djackal-0.5.4/djackal/utils.py
--rw-r--r--   0        0        0       79 2021-04-27 10:23:21.074040 djackal-0.5.4/djackal/views/__init__.py
--rw-r--r--   0        0        0    11206 2023-04-12 19:08:44.505732 djackal-0.5.4/djackal/views/base.py
--rw-r--r--   0        0        0     3316 2021-04-28 14:02:19.921014 djackal-0.5.4/djackal/views/generics.py
--rw-r--r--   0        0        0      379 2021-12-15 14:11:54.023043 djackal-0.5.4/djackal/views/handler.py
--rw-r--r--   0        0        0     2219 2023-04-13 16:08:31.273087 djackal-0.5.4/djackal/views/mixins.py
--rw-r--r--   0        0        0      574 2023-04-13 16:08:34.409049 djackal-0.5.4/pyproject.toml
--rw-r--r--   0        0        0        0 2021-02-25 12:42:37.427177 djackal-0.5.4/tests/__init__.py
--rw-r--r--   0        0        0        0 2021-02-25 12:42:37.427177 djackal-0.5.4/tests/model_mixins/__init__.py
--rw-r--r--   0        0        0     2360 2023-04-12 19:08:44.505732 djackal-0.5.4/tests/model_mixins/test_extra_mixin.py
--rw-r--r--   0        0        0      515 2021-04-27 10:01:21.653305 djackal-0.5.4/tests/models.py
--rw-r--r--   0        0        0      494 2022-06-01 07:29:57.471726 djackal-0.5.4/tests/settings.py
--rw-r--r--   0        0        0      770 2022-06-01 07:29:57.471726 djackal-0.5.4/tests/test_erra.py
--rw-r--r--   0        0        0     3665 2022-06-01 07:29:57.471726 djackal-0.5.4/tests/test_exceptions.py
--rw-r--r--   0        0        0      631 2021-04-29 09:49:02.876011 djackal-0.5.4/tests/test_fields.py
--rw-r--r--   0        0        0     1165 2021-06-17 15:10:32.353990 djackal-0.5.4/tests/test_initializer.py
--rw-r--r--   0        0        0      260 2022-06-01 07:29:57.471726 djackal-0.5.4/tests/test_loaders.py
--rw-r--r--   0        0        0     4139 2023-01-05 11:28:45.245418 djackal-0.5.4/tests/test_query_filter.py
--rw-r--r--   0        0        0      899 2023-04-12 19:08:44.505732 djackal-0.5.4/tests/test_settings.py
--rw-r--r--   0        0        0     2808 2022-06-01 07:29:57.471726 djackal-0.5.4/tests/test_shortcuts.py
--rw-r--r--   0        0        0     1365 2023-04-12 19:08:44.505732 djackal-0.5.4/tests/test_utils.py
--rw-r--r--   0        0        0     1342 1970-01-01 00:00:00.000000 djackal-0.5.4/setup.py
--rw-r--r--   0        0        0     1299 1970-01-01 00:00:00.000000 djackal-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2021-04-27 09:26:04.461893 djackal-0.6.0/LICENSE
+-rw-r--r--   0        0        0      484 2022-01-14 07:38:42.023715 djackal-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2021-04-27 10:13:03.376108 djackal-0.6.0/djackal/__init__.py
+-rw-r--r--   0        0        0      118 2021-04-28 13:22:14.818993 djackal-0.6.0/djackal/apps.py
+-rw-r--r--   0        0        0      541 2021-11-23 06:18:24.021837 djackal-0.6.0/djackal/erra.py
+-rw-r--r--   0        0        0     2614 2022-04-16 11:25:48.492286 djackal-0.6.0/djackal/exceptions.py
+-rw-r--r--   0        0        0      227 2021-02-25 12:42:37.423177 djackal-0.6.0/djackal/expressions.py
+-rw-r--r--   0        0        0       34 2021-04-29 09:48:08.913022 djackal-0.6.0/djackal/fields/__init__.py
+-rw-r--r--   0        0        0     2145 2023-04-12 19:08:44.501732 djackal-0.6.0/djackal/fields/json_field.py
+-rw-r--r--   0        0        0     1165 2021-06-17 15:10:32.345990 djackal-0.6.0/djackal/initializer.py
+-rw-r--r--   0        0        0      161 2022-06-01 07:29:57.471726 djackal-0.6.0/djackal/loaders.py
+-rw-r--r--   0        0        0        0 2021-02-25 12:42:37.423177 djackal-0.6.0/djackal/management/__init__.py
+-rw-r--r--   0        0        0        0 2021-02-25 12:42:37.423177 djackal-0.6.0/djackal/management/commands/__init__.py
+-rw-r--r--   0        0        0      370 2021-06-17 15:10:32.349990 djackal-0.6.0/djackal/management/commands/init.py
+-rw-r--r--   0        0        0       36 2023-04-12 19:08:44.501732 djackal-0.6.0/djackal/model_mixins/__init__.py
+-rw-r--r--   0        0        0     1222 2023-04-12 19:08:44.501732 djackal-0.6.0/djackal/model_mixins/extra_mixin.py
+-rw-r--r--   0        0        0     2243 2022-06-01 07:29:57.471726 djackal-0.6.0/djackal/pagination.py
+-rw-r--r--   0        0        0     2699 2022-04-16 11:25:48.492286 djackal-0.6.0/djackal/permissions.py
+-rw-r--r--   0        0        0     2785 2023-04-12 19:08:44.501732 djackal-0.6.0/djackal/query_filter.py
+-rw-r--r--   0        0        0     1606 2021-06-28 06:44:58.185826 djackal-0.6.0/djackal/serializers.py
+-rw-r--r--   0        0        0     2953 2023-04-12 19:08:44.501732 djackal-0.6.0/djackal/settings.py
+-rw-r--r--   0        0        0     1638 2022-06-01 07:29:57.471726 djackal-0.6.0/djackal/shortcuts.py
+-rw-r--r--   0        0        0        0 2021-06-17 15:10:32.349990 djackal-0.6.0/djackal/storage/__init__.py
+-rw-r--r--   0        0        0      126 2021-06-17 15:10:32.349990 djackal-0.6.0/djackal/storage/apps.py
+-rw-r--r--   0        0        0      404 2021-06-17 15:10:32.349990 djackal-0.6.0/djackal/storage/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2021-06-17 15:10:32.349990 djackal-0.6.0/djackal/storage/migrations/__init__.py
+-rw-r--r--   0        0        0      658 2021-06-17 15:10:32.349990 djackal-0.6.0/djackal/storage/models.py
+-rw-r--r--   0        0        0      760 2022-06-01 07:29:12.961130 djackal-0.6.0/djackal/tests.py
+-rw-r--r--   0        0        0      751 2023-04-12 19:08:44.501732 djackal-0.6.0/djackal/utils.py
+-rw-r--r--   0        0        0       79 2021-04-27 10:23:21.074040 djackal-0.6.0/djackal/views/__init__.py
+-rw-r--r--   0        0        0    11443 2023-07-21 04:30:50.038112 djackal-0.6.0/djackal/views/base.py
+-rw-r--r--   0        0        0     3316 2021-04-28 14:02:19.921014 djackal-0.6.0/djackal/views/generics.py
+-rw-r--r--   0        0        0      379 2021-12-15 14:11:54.023043 djackal-0.6.0/djackal/views/handler.py
+-rw-r--r--   0        0        0     2219 2023-04-13 16:08:31.273087 djackal-0.6.0/djackal/views/mixins.py
+-rw-r--r--   0        0        0      574 2023-07-21 04:29:00.153733 djackal-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-02-25 12:42:37.427177 djackal-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2021-02-25 12:42:37.427177 djackal-0.6.0/tests/model_mixins/__init__.py
+-rw-r--r--   0        0        0     2360 2023-04-12 19:08:44.505732 djackal-0.6.0/tests/model_mixins/test_extra_mixin.py
+-rw-r--r--   0        0        0      515 2021-04-27 10:01:21.653305 djackal-0.6.0/tests/models.py
+-rw-r--r--   0        0        0      494 2022-06-01 07:29:57.471726 djackal-0.6.0/tests/settings.py
+-rw-r--r--   0        0        0      770 2022-06-01 07:29:57.471726 djackal-0.6.0/tests/test_erra.py
+-rw-r--r--   0        0        0     3665 2022-06-01 07:29:57.471726 djackal-0.6.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0      631 2021-04-29 09:49:02.876011 djackal-0.6.0/tests/test_fields.py
+-rw-r--r--   0        0        0     1165 2021-06-17 15:10:32.353990 djackal-0.6.0/tests/test_initializer.py
+-rw-r--r--   0        0        0      260 2022-06-01 07:29:57.471726 djackal-0.6.0/tests/test_loaders.py
+-rw-r--r--   0        0        0     4139 2023-01-05 11:28:45.245418 djackal-0.6.0/tests/test_query_filter.py
+-rw-r--r--   0        0        0      899 2023-04-12 19:08:44.505732 djackal-0.6.0/tests/test_settings.py
+-rw-r--r--   0        0        0     2808 2022-06-01 07:29:57.471726 djackal-0.6.0/tests/test_shortcuts.py
+-rw-r--r--   0        0        0     1365 2023-04-12 19:08:44.505732 djackal-0.6.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1299 1970-01-01 00:00:00.000000 djackal-0.6.0/PKG-INFO
```

### Comparing `djackal-0.5.4/LICENSE` & `djackal-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/djackal/erra.py` & `djackal-0.6.0/djackal/erra.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/djackal/exceptions.py` & `djackal-0.6.0/djackal/exceptions.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/djackal/fields/json_field.py` & `djackal-0.6.0/djackal/fields/json_field.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/djackal/initializer.py` & `djackal-0.6.0/djackal/initializer.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/djackal/model_mixins/extra_mixin.py` & `djackal-0.6.0/djackal/model_mixins/extra_mixin.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/djackal/pagination.py` & `djackal-0.6.0/djackal/pagination.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/djackal/permissions.py` & `djackal-0.6.0/djackal/permissions.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/djackal/query_filter.py` & `djackal-0.6.0/djackal/query_filter.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/djackal/serializers.py` & `djackal-0.6.0/djackal/serializers.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/djackal/settings.py` & `djackal-0.6.0/djackal/settings.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/djackal/shortcuts.py` & `djackal-0.6.0/djackal/shortcuts.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/djackal/storage/models.py` & `djackal-0.6.0/djackal/storage/models.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/djackal/tests.py` & `djackal-0.6.0/djackal/tests.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/djackal/utils.py` & `djackal-0.6.0/djackal/utils.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/djackal/views/base.py` & `djackal-0.6.0/djackal/views/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from functools import cached_property
+
 from puty import purify
 from rest_framework.response import Response
 from rest_framework.views import APIView
 
 from djackal import query_filter
 from djackal.exceptions import NotFound
 from djackal.settings import djackal_settings
@@ -143,23 +145,31 @@
     data_schema = None
     query_params_schema = None
 
     def get_purified_data(self, key=None, many=False):
         schema = self.get_data_schema(key)
         return purify(self.request.data, schema, many=many)
 
+    @cached_property
+    def purified_data(self):
+        return self.get_purified_data()
+
     def get_data_schema(self, key=None):
         if key in self.data_schema:
             return self.data_schema[key]
         return self.data_schema
 
     def get_purified_query_params(self, key=None, many=False):
         schema = self.get_query_params_schema(key)
         return purify(self.get_query_params_dict(), schema, many=many)
 
+    @cached_property
+    def purified_query_params(self):
+        return self.get_purified_query_params()
+
     def get_query_params_schema(self, key=None):
         if key in self.query_params_schema:
             return self.query_params_schema[key]
         return self.query_params_schema
 
 
 class BaseDjackalAPIView(APIView):
```

### Comparing `djackal-0.5.4/djackal/views/generics.py` & `djackal-0.6.0/djackal/views/generics.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/djackal/views/mixins.py` & `djackal-0.6.0/djackal/views/mixins.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/pyproject.toml` & `djackal-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "djackal"
-version = "0.5.4"
+version = "0.6.0"
 description = "extension of Django REST Framework"
 authors = ["jrog <jrog612@gmail.com>"]
 license = "MIT"
 readme = 'README.md'
 repository = 'https://github.com/jrog612/djackal'
 homepage = 'https://github.com/jrog612/djackal'
 packages = [
```

### Comparing `djackal-0.5.4/tests/model_mixins/test_extra_mixin.py` & `djackal-0.6.0/tests/model_mixins/test_extra_mixin.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/tests/models.py` & `djackal-0.6.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/tests/test_erra.py` & `djackal-0.6.0/tests/test_erra.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/tests/test_exceptions.py` & `djackal-0.6.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/tests/test_fields.py` & `djackal-0.6.0/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/tests/test_initializer.py` & `djackal-0.6.0/tests/test_initializer.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/tests/test_query_filter.py` & `djackal-0.6.0/tests/test_query_filter.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/tests/test_settings.py` & `djackal-0.6.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/tests/test_shortcuts.py` & `djackal-0.6.0/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/tests/test_utils.py` & `djackal-0.6.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.4/PKG-INFO` & `djackal-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djackal
-Version: 0.5.4
+Version: 0.6.0
 Summary: extension of Django REST Framework
 Home-page: https://github.com/jrog612/djackal
 License: MIT
 Author: jrog
 Author-email: jrog612@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

