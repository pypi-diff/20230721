# Comparing `tmp/djgraphql-1.0.4.tar.gz` & `tmp/djgraphql-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djgraphql-1.0.4.tar", last modified: Fri Jul 21 03:15:24 2023, max compression
+gzip compressed data, was "djgraphql-1.0.5.tar", last modified: Fri Jul 21 05:15:16 2023, max compression
```

## Comparing `djgraphql-1.0.4.tar` & `djgraphql-1.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:15:24.206587 djgraphql-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 03:14:58.000000 djgraphql-1.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-21 03:14:58.000000 djgraphql-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 03:15:24.206587 djgraphql-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-21 03:14:58.000000 djgraphql-1.0.4/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-07-21 03:14:58.000000 djgraphql-1.0.4/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-21 03:14:58.000000 djgraphql-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:15:24.202587 djgraphql-1.0.4/djgraphql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:14:58.000000 djgraphql-1.0.4/djgraphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-21 03:14:58.000000 djgraphql-1.0.4/djgraphql/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-21 03:14:58.000000 djgraphql-1.0.4/djgraphql/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-21 03:14:58.000000 djgraphql-1.0.4/djgraphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-21 03:14:58.000000 djgraphql-1.0.4/djgraphql/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:15:24.202587 djgraphql-1.0.4/djgraphql/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:14:58.000000 djgraphql-1.0.4/djgraphql/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-21 03:14:58.000000 djgraphql-1.0.4/djgraphql/test/test_routers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-21 03:14:58.000000 djgraphql-1.0.4/djgraphql/test/test_schema_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-21 03:14:58.000000 djgraphql-1.0.4/djgraphql/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:15:24.202587 djgraphql-1.0.4/djgraphql/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:14:58.000000 djgraphql-1.0.4/djgraphql/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-21 03:14:58.000000 djgraphql-1.0.4/djgraphql/utils/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-21 03:14:58.000000 djgraphql-1.0.4/djgraphql/utils/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:15:24.202587 djgraphql-1.0.4/djgraphql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 03:15:23.000000 djgraphql-1.0.4/djgraphql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-21 03:15:24.000000 djgraphql-1.0.4/djgraphql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 03:15:23.000000 djgraphql-1.0.4/djgraphql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 03:15:23.000000 djgraphql-1.0.4/djgraphql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 03:15:23.000000 djgraphql-1.0.4/djgraphql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 03:14:58.000000 djgraphql-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 03:15:24.206587 djgraphql-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-21 03:14:58.000000 djgraphql-1.0.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 03:14:58.000000 djgraphql-1.0.4/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:15:16.122707 djgraphql-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 05:14:52.000000 djgraphql-1.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-21 05:14:52.000000 djgraphql-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 05:15:16.122707 djgraphql-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-21 05:14:52.000000 djgraphql-1.0.5/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-07-21 05:14:52.000000 djgraphql-1.0.5/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-21 05:14:52.000000 djgraphql-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:15:16.122707 djgraphql-1.0.5/djgraphql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:14:52.000000 djgraphql-1.0.5/djgraphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-21 05:14:52.000000 djgraphql-1.0.5/djgraphql/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-21 05:14:52.000000 djgraphql-1.0.5/djgraphql/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-21 05:14:52.000000 djgraphql-1.0.5/djgraphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-21 05:14:52.000000 djgraphql-1.0.5/djgraphql/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:15:16.122707 djgraphql-1.0.5/djgraphql/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:14:52.000000 djgraphql-1.0.5/djgraphql/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-21 05:14:52.000000 djgraphql-1.0.5/djgraphql/test/test_routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-21 05:14:52.000000 djgraphql-1.0.5/djgraphql/test/test_schema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-21 05:14:52.000000 djgraphql-1.0.5/djgraphql/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:15:16.122707 djgraphql-1.0.5/djgraphql/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:14:52.000000 djgraphql-1.0.5/djgraphql/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-21 05:14:52.000000 djgraphql-1.0.5/djgraphql/utils/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-21 05:14:52.000000 djgraphql-1.0.5/djgraphql/utils/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:15:16.122707 djgraphql-1.0.5/djgraphql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 05:15:15.000000 djgraphql-1.0.5/djgraphql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-21 05:15:16.000000 djgraphql-1.0.5/djgraphql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 05:15:15.000000 djgraphql-1.0.5/djgraphql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 05:15:15.000000 djgraphql-1.0.5/djgraphql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 05:15:15.000000 djgraphql-1.0.5/djgraphql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 05:14:52.000000 djgraphql-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 05:15:16.122707 djgraphql-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-21 05:14:52.000000 djgraphql-1.0.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 05:14:52.000000 djgraphql-1.0.5/version
```

### Comparing `djgraphql-1.0.4/LICENSE.txt` & `djgraphql-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.4/PKG-INFO` & `djgraphql-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: djgraphql
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package that makes easier to use graphql with django.
 Home-page: https://shitalluitel.com.np
 Author: Shital Babu Luitel
 Author-email: ctalluitel@gmail.com
 License: file: LICENSE.txt
 Description: file: README.md
 Platform: UNKNOWN
```

### Comparing `djgraphql-1.0.4/Pipfile.lock` & `djgraphql-1.0.5/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.4/README.md` & `djgraphql-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.4/djgraphql/settings.py` & `djgraphql-1.0.5/djgraphql/settings.py`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.4/djgraphql/test/test_routers.py` & `djgraphql-1.0.5/djgraphql/test/test_routers.py`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.4/djgraphql/test/test_schema_generation.py` & `djgraphql-1.0.5/djgraphql/test/test_schema_generation.py`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.4/djgraphql/utils/routes.py` & `djgraphql-1.0.5/djgraphql/utils/routes.py`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.4/djgraphql.egg-info/PKG-INFO` & `djgraphql-1.0.5/djgraphql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: djgraphql
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package that makes easier to use graphql with django.
 Home-page: https://shitalluitel.com.np
 Author: Shital Babu Luitel
 Author-email: ctalluitel@gmail.com
 License: file: LICENSE.txt
 Description: file: README.md
 Platform: UNKNOWN
```

### Comparing `djgraphql-1.0.4/djgraphql.egg-info/SOURCES.txt` & `djgraphql-1.0.5/djgraphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.4/setup.py` & `djgraphql-1.0.5/setup.py`

 * *Files identical despite different names*

