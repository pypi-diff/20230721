# Comparing `tmp/djgraphql-1.0.1.tar.gz` & `tmp/djgraphql-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djgraphql-1.0.1.tar", last modified: Thu Jul 20 14:16:16 2023, max compression
+gzip compressed data, was "djgraphql-1.0.2.tar", last modified: Fri Jul 21 01:12:59 2023, max compression
```

## Comparing `djgraphql-1.0.1.tar` & `djgraphql-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:16:16.387680 djgraphql-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-20 14:15:51.000000 djgraphql-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-20 14:15:51.000000 djgraphql-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-20 14:16:16.387680 djgraphql-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-20 14:15:51.000000 djgraphql-1.0.1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-20 14:15:51.000000 djgraphql-1.0.1/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-20 14:15:51.000000 djgraphql-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:16:16.387680 djgraphql-1.0.1/djgraphql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:15:51.000000 djgraphql-1.0.1/djgraphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-20 14:15:51.000000 djgraphql-1.0.1/djgraphql/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-20 14:15:51.000000 djgraphql-1.0.1/djgraphql/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-20 14:15:51.000000 djgraphql-1.0.1/djgraphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-20 14:15:51.000000 djgraphql-1.0.1/djgraphql/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:16:16.387680 djgraphql-1.0.1/djgraphql/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:15:51.000000 djgraphql-1.0.1/djgraphql/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-20 14:15:51.000000 djgraphql-1.0.1/djgraphql/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:16:16.387680 djgraphql-1.0.1/djgraphql/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:15:51.000000 djgraphql-1.0.1/djgraphql/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-20 14:15:51.000000 djgraphql-1.0.1/djgraphql/utils/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-20 14:15:51.000000 djgraphql-1.0.1/djgraphql/utils/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:16:16.387680 djgraphql-1.0.1/djgraphql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-20 14:16:16.000000 djgraphql-1.0.1/djgraphql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-20 14:16:16.000000 djgraphql-1.0.1/djgraphql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:16:16.000000 djgraphql-1.0.1/djgraphql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 14:16:16.000000 djgraphql-1.0.1/djgraphql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 14:16:16.000000 djgraphql-1.0.1/djgraphql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-20 14:15:51.000000 djgraphql-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:16:16.387680 djgraphql-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-20 14:15:51.000000 djgraphql-1.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 14:15:51.000000 djgraphql-1.0.1/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:12:59.872817 djgraphql-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 01:12:38.000000 djgraphql-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-21 01:12:38.000000 djgraphql-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 01:12:59.872817 djgraphql-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-21 01:12:38.000000 djgraphql-1.0.2/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-21 01:12:38.000000 djgraphql-1.0.2/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-21 01:12:38.000000 djgraphql-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:12:59.868817 djgraphql-1.0.2/djgraphql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:12:38.000000 djgraphql-1.0.2/djgraphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-21 01:12:38.000000 djgraphql-1.0.2/djgraphql/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-21 01:12:38.000000 djgraphql-1.0.2/djgraphql/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-21 01:12:38.000000 djgraphql-1.0.2/djgraphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-21 01:12:38.000000 djgraphql-1.0.2/djgraphql/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:12:59.868817 djgraphql-1.0.2/djgraphql/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:12:38.000000 djgraphql-1.0.2/djgraphql/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-21 01:12:38.000000 djgraphql-1.0.2/djgraphql/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:12:59.872817 djgraphql-1.0.2/djgraphql/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:12:38.000000 djgraphql-1.0.2/djgraphql/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-21 01:12:38.000000 djgraphql-1.0.2/djgraphql/utils/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-21 01:12:38.000000 djgraphql-1.0.2/djgraphql/utils/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:12:59.868817 djgraphql-1.0.2/djgraphql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 01:12:59.000000 djgraphql-1.0.2/djgraphql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-21 01:12:59.000000 djgraphql-1.0.2/djgraphql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:12:59.000000 djgraphql-1.0.2/djgraphql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 01:12:59.000000 djgraphql-1.0.2/djgraphql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 01:12:59.000000 djgraphql-1.0.2/djgraphql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 01:12:38.000000 djgraphql-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:12:59.872817 djgraphql-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-21 01:12:38.000000 djgraphql-1.0.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 01:12:38.000000 djgraphql-1.0.2/version
```

### Comparing `djgraphql-1.0.1/LICENSE.txt` & `djgraphql-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.1/PKG-INFO` & `djgraphql-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: djgraphql
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package that makes easier to use graphql with django.
 Home-page: https://shitalluitel.com.np
 Author: Shital Babu Luitel
 Author-email: ctalluitel@gmail.com
 License: file: LICENSE.txt
 Description: file: README.md
 Platform: UNKNOWN
```

### Comparing `djgraphql-1.0.1/Pipfile.lock` & `djgraphql-1.0.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.1/README.md` & `djgraphql-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.1/djgraphql/schema.py` & `djgraphql-1.0.2/djgraphql/schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import defaultdict
 
 import graphene
 from graphene_django.debug import DjangoDebug
 
-from djql.utils.routes import DefaultRouter
+from djgraphql.utils.routes import DefaultRouter
 
 __all__ = [
     'schema',
 ]
 
 
 class SchemaParameters:
```

### Comparing `djgraphql-1.0.1/djgraphql/settings.py` & `djgraphql-1.0.2/djgraphql/settings.py`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.1/djgraphql/utils/routes.py` & `djgraphql-1.0.2/djgraphql/utils/routes.py`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.1/djgraphql.egg-info/PKG-INFO` & `djgraphql-1.0.2/djgraphql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: djgraphql
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package that makes easier to use graphql with django.
 Home-page: https://shitalluitel.com.np
 Author: Shital Babu Luitel
 Author-email: ctalluitel@gmail.com
 License: file: LICENSE.txt
 Description: file: README.md
 Platform: UNKNOWN
```

### Comparing `djgraphql-1.0.1/setup.py` & `djgraphql-1.0.2/setup.py`

 * *Files identical despite different names*

