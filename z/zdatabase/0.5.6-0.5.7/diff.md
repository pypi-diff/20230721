# Comparing `tmp/zdatabase-0.5.6.tar.gz` & `tmp/zdatabase-0.5.7.tar.gz`

## Comparing `zdatabase-0.5.6.tar` & `zdatabase-0.5.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 zdatabase-0.5.6/src/zdatabase/__init__.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 zdatabase-0.5.6/src/zdatabase/model.py
--rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 zdatabase-0.5.6/src/zdatabase/utility.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 zdatabase-0.5.6/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zdatabase-0.5.6/LICENSE
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zdatabase-0.5.6/README.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 zdatabase-0.5.6/pyproject.toml
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 zdatabase-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 zdatabase-0.5.7/src/zdatabase/__init__.py
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 zdatabase-0.5.7/src/zdatabase/model.py
+-rw-r--r--   0        0        0     4802 2020-02-02 00:00:00.000000 zdatabase-0.5.7/src/zdatabase/utility.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 zdatabase-0.5.7/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zdatabase-0.5.7/LICENSE
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zdatabase-0.5.7/README.md
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 zdatabase-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 zdatabase-0.5.7/PKG-INFO
```

### Comparing `zdatabase-0.5.6/src/zdatabase/__init__.py` & `zdatabase-0.5.7/src/zdatabase/__init__.py`

 * *Files identical despite different names*

### Comparing `zdatabase-0.5.6/src/zdatabase/model.py` & `zdatabase-0.5.7/src/zdatabase/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,19 +20,16 @@
                 dict_.pop(key)
         return dict_
 
     @classmethod
     def keys(cls):
         return cls.__table__.columns.keys()
 
-    def get(self, key):
-        return self.__getattribute__(key)
-
     def raw_json(self):
-        return {key: self.get(key) for key in self.keys()}
+        return {key: self.__getattribute__(key) for key in self.keys()}
 
     def to_json(self):
         return self.to_json_()
 
     @property
     def key_map(self):
         return {}
@@ -40,15 +37,15 @@
     @property
     def key_derive_map(self):
         return {}
 
     def to_json_(self):  # 新方法，待替换
         tmp = {}
         for k in self.keys():
-            v = self.get(k)
+            v = self.__getattribute__(k)
             tmp[k] = v
             for key, func in self.key_map.items():
                 if k == key:
                     tmp[k] = func(v)
             for key, map in self.key_derive_map.items():
                 if k == key:
                     if isinstance(map, list):
```

### Comparing `zdatabase-0.5.6/src/zdatabase/utility.py` & `zdatabase-0.5.7/src/zdatabase/utility.py`

 * *Files 15% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         flts = []
         start_date = params.get('start_date')
         end_date = params.get('end_date')
         flts += [getattr(cls, attr_name) >= start_date] if start_date else []
         flts += [getattr(cls, attr_name) <= end_date] if end_date else []
         return flts
 
+
     @staticmethod
     def all(cls, query, method='to_json'):
         """返回全部记录
         """
         items = query.all()
         return [getattr(item, method)() for item in items]
 
@@ -78,109 +79,94 @@
         return rst
 
 
 class MapperUtility:
     @staticmethod
     def jsonlize(items):
         return [item.to_json() for item in items]
-
-    @classmethod
-    def make_flts(cls, **kwargs):
-        return [getattr(cls, k) == v for k, v in kwargs.items()]
-
-    @classmethod
-    def make_query(cls, **kwargs):
-        flts = cls.make_flts(**kwargs)
-        return cls.filter(*flts)
-
+    
     @classmethod
     def add_(cls, data):
         obj = cls.new(data)
         obj.add_one()
         return obj
-
+    
     @classmethod
-    def add(cls, data):
-        validate(instance=data, schema=cls.__schema__)
+    def add(cls, data, sync=True):
+        if hasattr(cls, 'schema'):
+            validate(instance=data, schema=cls.schema)
         obj = cls.add_(data)
-        cls.commit()
+        if sync:
+            cls.commit()
         return obj
 
     @classmethod
-    def add_list_(cls, items):
-        for item in items:
-            cls.add_(item)
-        cls.commit()
-
-    @classmethod
-    def save_(cls, primary_key, data):
-        validate(instance=data, schema=cls.__schema__)
-        obj = cls.get_(primary_key)
+    def save(cls, primary_key, data):
+        if hasattr(cls, 'schema'):
+            validate(instance=data, schema=cls.schema)
+        obj = cls.get(primary_key)
         if obj:
             obj.update(data)
         else:
             cls.add_(data)
         cls.commit()
 
     @classmethod
-    def update_(cls, primary_key, data):
-        obj = cls.get_(primary_key)
+    def update(cls, primary_key, data):
+        obj = cls.get(primary_key)
         obj.update(data)
         cls.commit()
 
     @classmethod
-    def get_(cls, primary_key):
+    def get(cls, primary_key):
         return cls.query.get(primary_key)
+    
+    @classmethod
+    def delete(cls, **kwargs):
+        cls.make_query(**kwargs).delete(synchronize_session=False)
 
     @classmethod
-    def get_json(cls, primary_key):
-        obj = cls.get_(primary_key)
-        return obj.to_json() if obj else {}
+    def make_flts(cls, **kwargs):
+        return [getattr(cls, k) == v for k, v in kwargs.items()]
 
     @classmethod
-    def get_list_(cls, **kwargs):
+    def make_query(cls, **kwargs):
+        flts = cls.make_flts(**kwargs)
+        return cls.filter(*flts)
+    
+    @classmethod
+    def get_list(cls, **kwargs):
         return cls.make_query(**kwargs).all()
+    
+    @classmethod
+    def get_json(cls, primary_key):
+        obj = cls.get(primary_key)
+        return obj.to_json() if obj else {}
 
     @classmethod
-    def get_list(cls, **kwargs):
-        if 'page_num' in kwargs:
+    def get_jsons(cls, page_num=None, page_size=None, **kwargs):
+        if page_num or page_size :
             pagination = {
-                'page_size': kwargs.pop('page_size', 20),
-                'page_num': kwargs.pop('page_num', 1)
+                'page_num': page_num if page_num else 1,
+                'page_size': page_size if page_size else 20
             }
             query = cls.make_query(**kwargs)
             return cls.paginate(query, pagination)
         else:
-            items = cls.get_list_(**kwargs)
+            items = cls.get_list(**kwargs)
             return cls.jsonlize(items)
 
     @classmethod
-    def get_all_(cls):
-        return cls.filter().all()
-
-    @classmethod
-    def get_all(cls):
-        items = cls.get_all_()
-        return cls.jsonlize(items)
-
-    @classmethod
-    def get_attrs_(cls, attr_names, **kwargs):
+    def get_attrs(cls, attr_names, **kwargs):
         flts = cls.make_flts(**kwargs)
         attrs = [getattr(cls, attr_name) for attr_name in attr_names]
         return cls.query_(*attrs).filter(*flts).all()
 
     @classmethod
-    def get_map_(cls, attr_names):
+    def get_map(cls, attr_names):
         rst_map = {}
-        for item in cls.get_attrs_(attr_names):
+        for item in cls.get_attrs(attr_names):
             a, b = item
             rst_map[a] = b
         return rst_map
 
-    @classmethod
-    def delete_list_(cls, **kwargs):
-        cls.make_query(**kwargs).delete(synchronize_session=False)
 
-    @classmethod
-    def delete_list(cls, **kwargs):
-        cls.make_query(**kwargs).delete(synchronize_session=False)
-        cls.commit()
```

### Comparing `zdatabase-0.5.6/LICENSE` & `zdatabase-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `zdatabase-0.5.6/pyproject.toml` & `zdatabase-0.5.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zdatabase"
-version = "0.5.6"
+version = "0.5.7"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen database library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `zdatabase-0.5.6/PKG-INFO` & `zdatabase-0.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zdatabase
-Version: 0.5.6
+Version: 0.5.7
 Summary: zen database library
 Project-URL: Homepage, https://github.com/inspirare6/zdatabase
 Project-URL: Bug Tracker, https://github.com/inspirare6/zdatabase/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

