# Comparing `tmp/djgraphql-1.1.0.tar.gz` & `tmp/djgraphql-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djgraphql-1.1.0.tar", last modified: Fri Jul 21 06:15:35 2023, max compression
+gzip compressed data, was "djgraphql-1.1.1.tar", last modified: Fri Jul 21 15:31:18 2023, max compression
```

## Comparing `djgraphql-1.1.0.tar` & `djgraphql-1.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:15:35.503364 djgraphql-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 06:15:07.000000 djgraphql-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-21 06:15:07.000000 djgraphql-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 06:15:35.503364 djgraphql-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-21 06:15:07.000000 djgraphql-1.1.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    13032 2023-07-21 06:15:07.000000 djgraphql-1.1.0/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-21 06:15:07.000000 djgraphql-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:15:35.499364 djgraphql-1.1.0/djgraphql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:15:35.499364 djgraphql-1.1.0/djgraphql/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/test/test_routers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/test/test_schema_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:15:35.503364 djgraphql-1.1.0/djgraphql/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/utils/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/utils/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:15:35.499364 djgraphql-1.1.0/djgraphql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 06:15:35.000000 djgraphql-1.1.0/djgraphql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-21 06:15:35.000000 djgraphql-1.1.0/djgraphql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 06:15:35.000000 djgraphql-1.1.0/djgraphql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 06:15:35.000000 djgraphql-1.1.0/djgraphql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 06:15:35.000000 djgraphql-1.1.0/djgraphql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 06:15:07.000000 djgraphql-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 06:15:35.503364 djgraphql-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-21 06:15:07.000000 djgraphql-1.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 06:15:07.000000 djgraphql-1.1.0/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:31:18.123967 djgraphql-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 15:30:57.000000 djgraphql-1.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-21 15:30:57.000000 djgraphql-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 15:31:18.123967 djgraphql-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-21 15:30:57.000000 djgraphql-1.1.1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    13032 2023-07-21 15:30:57.000000 djgraphql-1.1.1/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-21 15:30:57.000000 djgraphql-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:31:18.119967 djgraphql-1.1.1/djgraphql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:30:57.000000 djgraphql-1.1.1/djgraphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-21 15:30:57.000000 djgraphql-1.1.1/djgraphql/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-21 15:30:57.000000 djgraphql-1.1.1/djgraphql/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-21 15:30:57.000000 djgraphql-1.1.1/djgraphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-21 15:30:57.000000 djgraphql-1.1.1/djgraphql/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:31:18.123967 djgraphql-1.1.1/djgraphql/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:30:57.000000 djgraphql-1.1.1/djgraphql/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-21 15:30:57.000000 djgraphql-1.1.1/djgraphql/test/test_routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-21 15:30:57.000000 djgraphql-1.1.1/djgraphql/test/test_schema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-21 15:30:57.000000 djgraphql-1.1.1/djgraphql/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:31:18.123967 djgraphql-1.1.1/djgraphql/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:30:57.000000 djgraphql-1.1.1/djgraphql/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-21 15:30:57.000000 djgraphql-1.1.1/djgraphql/utils/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-21 15:30:57.000000 djgraphql-1.1.1/djgraphql/utils/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:31:18.123967 djgraphql-1.1.1/djgraphql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 15:31:17.000000 djgraphql-1.1.1/djgraphql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-21 15:31:18.000000 djgraphql-1.1.1/djgraphql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:31:17.000000 djgraphql-1.1.1/djgraphql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 15:31:17.000000 djgraphql-1.1.1/djgraphql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 15:31:17.000000 djgraphql-1.1.1/djgraphql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 15:30:57.000000 djgraphql-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:31:18.123967 djgraphql-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-21 15:30:57.000000 djgraphql-1.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 15:30:57.000000 djgraphql-1.1.1/version
```

### Comparing `djgraphql-1.1.0/LICENSE.txt` & `djgraphql-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djgraphql-1.1.0/PKG-INFO` & `djgraphql-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: djgraphql
-Version: 1.1.0
+Version: 1.1.1
 Summary: A package that makes easier to use graphql with django.
 Home-page: https://shitalluitel.com.np
 Author: Shital Babu Luitel
 Author-email: ctalluitel@gmail.com
 License: file: LICENSE.txt
 Description: file: README.md
 Platform: UNKNOWN
```

### Comparing `djgraphql-1.1.0/Pipfile.lock` & `djgraphql-1.1.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `djgraphql-1.1.0/README.md` & `djgraphql-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `djgraphql-1.1.0/djgraphql/schema.py` & `djgraphql-1.1.1/djgraphql/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,11 @@
         query_resolvers = self._resolvers['query']
         mutation_resolvers = self._resolvers['mutation']
 
         schema_params = dict()
 
         schema_params['query'] = SchemaParameters('Query', *query_resolvers)  # noqa
         schema_params['mutation'] = SchemaParameters('Mutation', *mutation_resolvers)  # noqa
-
-        print(schema_params)
-
         return graphene.Schema(**schema_params)
 
 
 schema = Schema()
```

### Comparing `djgraphql-1.1.0/djgraphql/settings.py` & `djgraphql-1.1.1/djgraphql/settings.py`

 * *Files identical despite different names*

### Comparing `djgraphql-1.1.0/djgraphql/test/test_routers.py` & `djgraphql-1.1.1/djgraphql/test/test_routers.py`

 * *Files identical despite different names*

### Comparing `djgraphql-1.1.0/djgraphql/test/test_schema_generation.py` & `djgraphql-1.1.1/djgraphql/test/test_schema_generation.py`

 * *Files identical despite different names*

### Comparing `djgraphql-1.1.0/djgraphql/utils/routes.py` & `djgraphql-1.1.1/djgraphql/utils/routes.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,25 +38,28 @@
             setattr(self, f'_{method.value}_resolvers', [])
             resolvers = getattr(self, f'_{method.value}_resolvers')
 
         resolvers.append(resolver)
 
     @property
     def query(self):
+        query_resolver = self._query_resolvers or []
         return type(
             'Query',
             (
-                *self._query_resolvers,
+                *query_resolver,
                 graphene.ObjectType
             ),
             {}
         )
 
     @property
     def mutation(self):
+        mutation_resolver = self._mutation_resolvers or []
         return type(
             'Mutation',
             (
+                *mutation_resolver,
                 graphene.ObjectType,
             ),
             {}
         )
```

### Comparing `djgraphql-1.1.0/djgraphql.egg-info/PKG-INFO` & `djgraphql-1.1.1/djgraphql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: djgraphql
-Version: 1.1.0
+Version: 1.1.1
 Summary: A package that makes easier to use graphql with django.
 Home-page: https://shitalluitel.com.np
 Author: Shital Babu Luitel
 Author-email: ctalluitel@gmail.com
 License: file: LICENSE.txt
 Description: file: README.md
 Platform: UNKNOWN
```

### Comparing `djgraphql-1.1.0/djgraphql.egg-info/SOURCES.txt` & `djgraphql-1.1.1/djgraphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djgraphql-1.1.0/setup.py` & `djgraphql-1.1.1/setup.py`

 * *Files identical despite different names*

