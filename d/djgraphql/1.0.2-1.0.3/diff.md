# Comparing `tmp/djgraphql-1.0.2.tar.gz` & `tmp/djgraphql-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djgraphql-1.0.2.tar", last modified: Fri Jul 21 01:12:59 2023, max compression
+gzip compressed data, was "djgraphql-1.0.3.tar", last modified: Fri Jul 21 01:30:21 2023, max compression
```

## Comparing `djgraphql-1.0.2.tar` & `djgraphql-1.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:12:59.872817 djgraphql-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 01:12:38.000000 djgraphql-1.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-21 01:12:38.000000 djgraphql-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 01:12:59.872817 djgraphql-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-21 01:12:38.000000 djgraphql-1.0.2/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-21 01:12:38.000000 djgraphql-1.0.2/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-21 01:12:38.000000 djgraphql-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:12:59.868817 djgraphql-1.0.2/djgraphql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:12:38.000000 djgraphql-1.0.2/djgraphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-21 01:12:38.000000 djgraphql-1.0.2/djgraphql/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-21 01:12:38.000000 djgraphql-1.0.2/djgraphql/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-21 01:12:38.000000 djgraphql-1.0.2/djgraphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-21 01:12:38.000000 djgraphql-1.0.2/djgraphql/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:12:59.868817 djgraphql-1.0.2/djgraphql/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:12:38.000000 djgraphql-1.0.2/djgraphql/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-21 01:12:38.000000 djgraphql-1.0.2/djgraphql/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:12:59.872817 djgraphql-1.0.2/djgraphql/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:12:38.000000 djgraphql-1.0.2/djgraphql/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-21 01:12:38.000000 djgraphql-1.0.2/djgraphql/utils/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-21 01:12:38.000000 djgraphql-1.0.2/djgraphql/utils/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:12:59.868817 djgraphql-1.0.2/djgraphql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 01:12:59.000000 djgraphql-1.0.2/djgraphql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-21 01:12:59.000000 djgraphql-1.0.2/djgraphql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:12:59.000000 djgraphql-1.0.2/djgraphql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 01:12:59.000000 djgraphql-1.0.2/djgraphql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 01:12:59.000000 djgraphql-1.0.2/djgraphql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 01:12:38.000000 djgraphql-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:12:59.872817 djgraphql-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-21 01:12:38.000000 djgraphql-1.0.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 01:12:38.000000 djgraphql-1.0.2/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:30:21.817476 djgraphql-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 01:30:01.000000 djgraphql-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-21 01:30:01.000000 djgraphql-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 01:30:21.817476 djgraphql-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-21 01:30:01.000000 djgraphql-1.0.3/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-21 01:30:01.000000 djgraphql-1.0.3/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-21 01:30:01.000000 djgraphql-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:30:21.817476 djgraphql-1.0.3/djgraphql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:30:01.000000 djgraphql-1.0.3/djgraphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-21 01:30:01.000000 djgraphql-1.0.3/djgraphql/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-21 01:30:01.000000 djgraphql-1.0.3/djgraphql/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-21 01:30:01.000000 djgraphql-1.0.3/djgraphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-21 01:30:01.000000 djgraphql-1.0.3/djgraphql/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:30:21.817476 djgraphql-1.0.3/djgraphql/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:30:01.000000 djgraphql-1.0.3/djgraphql/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-21 01:30:01.000000 djgraphql-1.0.3/djgraphql/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:30:21.817476 djgraphql-1.0.3/djgraphql/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:30:01.000000 djgraphql-1.0.3/djgraphql/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-21 01:30:01.000000 djgraphql-1.0.3/djgraphql/utils/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-21 01:30:01.000000 djgraphql-1.0.3/djgraphql/utils/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:30:21.817476 djgraphql-1.0.3/djgraphql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 01:30:21.000000 djgraphql-1.0.3/djgraphql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-21 01:30:21.000000 djgraphql-1.0.3/djgraphql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:30:21.000000 djgraphql-1.0.3/djgraphql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 01:30:21.000000 djgraphql-1.0.3/djgraphql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 01:30:21.000000 djgraphql-1.0.3/djgraphql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 01:30:01.000000 djgraphql-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:30:21.817476 djgraphql-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-21 01:30:01.000000 djgraphql-1.0.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 01:30:01.000000 djgraphql-1.0.3/version
```

### Comparing `djgraphql-1.0.2/LICENSE.txt` & `djgraphql-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.2/PKG-INFO` & `djgraphql-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: djgraphql
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package that makes easier to use graphql with django.
 Home-page: https://shitalluitel.com.np
 Author: Shital Babu Luitel
 Author-email: ctalluitel@gmail.com
 License: file: LICENSE.txt
 Description: file: README.md
 Platform: UNKNOWN
```

### Comparing `djgraphql-1.0.2/Pipfile.lock` & `djgraphql-1.0.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.2/README.md` & `djgraphql-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.2/djgraphql/schema.py` & `djgraphql-1.0.3/djgraphql/schema.py`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.2/djgraphql/settings.py` & `djgraphql-1.0.3/djgraphql/settings.py`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.2/djgraphql/utils/routes.py` & `djgraphql-1.0.3/djgraphql/utils/routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
 import graphene
 
-from resolver import Resolver
+from djgraphql.utils.resolver import Resolver
 
 __all__ = [
     'MethodType',
     'Query',
     'Mutation',
     'DefaultRouter'
 ]
```

### Comparing `djgraphql-1.0.2/djgraphql.egg-info/PKG-INFO` & `djgraphql-1.0.3/djgraphql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: djgraphql
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package that makes easier to use graphql with django.
 Home-page: https://shitalluitel.com.np
 Author: Shital Babu Luitel
 Author-email: ctalluitel@gmail.com
 License: file: LICENSE.txt
 Description: file: README.md
 Platform: UNKNOWN
```

### Comparing `djgraphql-1.0.2/setup.py` & `djgraphql-1.0.3/setup.py`

 * *Files identical despite different names*

