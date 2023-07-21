# Comparing `tmp/djgraphql-1.0.7.tar.gz` & `tmp/djgraphql-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djgraphql-1.0.7.tar", last modified: Fri Jul 21 05:45:14 2023, max compression
+gzip compressed data, was "djgraphql-1.0.8.tar", last modified: Fri Jul 21 06:02:59 2023, max compression
```

## Comparing `djgraphql-1.0.7.tar` & `djgraphql-1.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:45:14.273669 djgraphql-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 05:44:51.000000 djgraphql-1.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-21 05:44:51.000000 djgraphql-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 05:45:14.273669 djgraphql-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-21 05:44:51.000000 djgraphql-1.0.7/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-07-21 05:44:51.000000 djgraphql-1.0.7/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-21 05:44:51.000000 djgraphql-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:45:14.269669 djgraphql-1.0.7/djgraphql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:44:51.000000 djgraphql-1.0.7/djgraphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-21 05:44:51.000000 djgraphql-1.0.7/djgraphql/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-21 05:44:51.000000 djgraphql-1.0.7/djgraphql/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-21 05:44:51.000000 djgraphql-1.0.7/djgraphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-21 05:44:51.000000 djgraphql-1.0.7/djgraphql/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:45:14.273669 djgraphql-1.0.7/djgraphql/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:44:51.000000 djgraphql-1.0.7/djgraphql/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-21 05:44:51.000000 djgraphql-1.0.7/djgraphql/test/test_routers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-21 05:44:51.000000 djgraphql-1.0.7/djgraphql/test/test_schema_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-21 05:44:51.000000 djgraphql-1.0.7/djgraphql/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:45:14.273669 djgraphql-1.0.7/djgraphql/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:44:51.000000 djgraphql-1.0.7/djgraphql/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-21 05:44:51.000000 djgraphql-1.0.7/djgraphql/utils/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-21 05:44:51.000000 djgraphql-1.0.7/djgraphql/utils/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:45:14.273669 djgraphql-1.0.7/djgraphql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 05:45:13.000000 djgraphql-1.0.7/djgraphql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-21 05:45:14.000000 djgraphql-1.0.7/djgraphql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 05:45:13.000000 djgraphql-1.0.7/djgraphql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 05:45:13.000000 djgraphql-1.0.7/djgraphql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 05:45:13.000000 djgraphql-1.0.7/djgraphql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 05:44:51.000000 djgraphql-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 05:45:14.273669 djgraphql-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-21 05:44:51.000000 djgraphql-1.0.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 05:44:51.000000 djgraphql-1.0.7/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:02:59.066905 djgraphql-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 06:02:41.000000 djgraphql-1.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-21 06:02:41.000000 djgraphql-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 06:02:59.066905 djgraphql-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-21 06:02:41.000000 djgraphql-1.0.8/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-07-21 06:02:41.000000 djgraphql-1.0.8/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-21 06:02:41.000000 djgraphql-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:02:59.066905 djgraphql-1.0.8/djgraphql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:02:59.066905 djgraphql-1.0.8/djgraphql/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/test/test_routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/test/test_schema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:02:59.066905 djgraphql-1.0.8/djgraphql/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/utils/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/utils/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:02:59.066905 djgraphql-1.0.8/djgraphql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 06:02:58.000000 djgraphql-1.0.8/djgraphql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-21 06:02:59.000000 djgraphql-1.0.8/djgraphql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 06:02:58.000000 djgraphql-1.0.8/djgraphql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 06:02:58.000000 djgraphql-1.0.8/djgraphql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 06:02:58.000000 djgraphql-1.0.8/djgraphql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 06:02:41.000000 djgraphql-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 06:02:59.066905 djgraphql-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-21 06:02:41.000000 djgraphql-1.0.8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 06:02:41.000000 djgraphql-1.0.8/version
```

### Comparing `djgraphql-1.0.7/LICENSE.txt` & `djgraphql-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.7/PKG-INFO` & `djgraphql-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: djgraphql
-Version: 1.0.7
+Version: 1.0.8
 Summary: A package that makes easier to use graphql with django.
 Home-page: https://shitalluitel.com.np
 Author: Shital Babu Luitel
 Author-email: ctalluitel@gmail.com
 License: file: LICENSE.txt
 Description: file: README.md
 Platform: UNKNOWN
```

### Comparing `djgraphql-1.0.7/Pipfile.lock` & `djgraphql-1.0.8/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.7/README.md` & `djgraphql-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.7/djgraphql/schema.py` & `djgraphql-1.0.8/djgraphql/schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from collections import defaultdict
 
 import graphene
+from graphene_django.debug import DjangoDebug
 
 from djgraphql.utils.routes import DefaultRouter
 
 # from graphene_django.debug import DjangoDebug
 
 __all__ = [
     'schema',
 ]
 
 
 class SchemaParameters:
-    # debug = graphene.Field(DjangoDebug, name='_debug')
+    debug = graphene.Field(DjangoDebug, name='_debug')
 
     def __new__(cls, name, *args, **kwargs):
         klass = type(
             name,
             (
                 *args,
                 graphene.ObjectType
             ),
             {
-                # 'debug': cls.debug
+                'debug': cls.debug
             }
         )
         return klass
 
 
 class SchemaMeta(type):
     _instance = {}
@@ -38,26 +39,20 @@
         return cls._instance[cls]
 
 
 class Schema(metaclass=SchemaMeta):
     _resolvers = defaultdict(list)
 
     def register(self, resolver: DefaultRouter):
-        queries = resolver.query
-        if queries:
-            self._resolvers['query'].append(*queries)
-
-        mutations = resolver.mutation
-
-        if mutations:
-            self._resolvers['mutation'].append(*mutations)
+        self._resolvers['query'].append(resolver.query)
+        self._resolvers['mutation'].append(resolver.mutation)
 
     def generate(self):
-        query_resolvers = self._resolvers['query'] or []
-        mutation_resolvers = self._resolvers['mutation'] or []
+        query_resolvers = self._resolvers['query']
+        mutation_resolvers = self._resolvers['mutation']
 
         schema_params = dict()
 
         schema_params['query'] = SchemaParameters('Query', *query_resolvers)  # noqa
         schema_params['mutation'] = SchemaParameters('Mutation', *mutation_resolvers)  # noqa
 
         print(schema_params)
```

### Comparing `djgraphql-1.0.7/djgraphql/settings.py` & `djgraphql-1.0.8/djgraphql/settings.py`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.7/djgraphql/test/test_routers.py` & `djgraphql-1.0.8/djgraphql/test/test_routers.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
         # 1. Register query resolvers
         query = ResolverGenerator('QueryResolver')
         router.register(
             resolver=query,
             method=MethodType.QUERY
         )
-        assert router.query == [query]
+        assert router.query ==
 
         # 2. Register mutation resolvers
         mutation = ResolverGenerator('MutationResolver')
         router.register(
             resolver=mutation,
             method=MethodType.MUTATION
         )
```

### Comparing `djgraphql-1.0.7/djgraphql/test/test_schema_generation.py` & `djgraphql-1.0.8/djgraphql/test/test_schema_generation.py`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.7/djgraphql/utils/routes.py` & `djgraphql-1.0.8/djgraphql/utils/routes.py`

 * *Files 20% similar despite different names*

```diff
@@ -38,12 +38,25 @@
             setattr(self, f'_{method.value}_resolvers', [])
             resolvers = getattr(self, f'_{method.value}_resolvers')
 
         resolvers.append(resolver)
 
     @property
     def query(self):
-        return self._query_resolvers
+        return type(
+            'Query',
+            (
+                *self._query_resolvers,
+                graphene.ObjectType
+            ),
+            {}
+        )
 
     @property
     def mutation(self):
-        return self._mutation_resolvers
+        return type(
+            'Mutation',
+            (
+                graphene.ObjectType,
+            ),
+            {}
+        )
```

### Comparing `djgraphql-1.0.7/djgraphql.egg-info/PKG-INFO` & `djgraphql-1.0.8/djgraphql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: djgraphql
-Version: 1.0.7
+Version: 1.0.8
 Summary: A package that makes easier to use graphql with django.
 Home-page: https://shitalluitel.com.np
 Author: Shital Babu Luitel
 Author-email: ctalluitel@gmail.com
 License: file: LICENSE.txt
 Description: file: README.md
 Platform: UNKNOWN
```

### Comparing `djgraphql-1.0.7/djgraphql.egg-info/SOURCES.txt` & `djgraphql-1.0.8/djgraphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.7/setup.py` & `djgraphql-1.0.8/setup.py`

 * *Files identical despite different names*

