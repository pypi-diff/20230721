# Comparing `tmp/auto_schema-0.0.8.tar.gz` & `tmp/auto_schema-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_schema-0.0.8.tar", last modified: Mon Aug  2 18:02:43 2021, max compression
+gzip compressed data, was "auto_schema-0.0.9.tar", last modified: Tue Aug  3 17:37:30 2021, max compression
```

## Comparing `auto_schema-0.0.8.tar` & `auto_schema-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 ola        (501) staff       (20)        0 2021-08-02 18:02:43.393414 auto_schema-0.0.8/
--rw-r--r--   0 ola        (501) staff       (20)     1075 2021-05-18 15:03:48.000000 auto_schema-0.0.8/LICENSE
--rw-r--r--   0 ola        (501) staff       (20)       34 2021-05-18 15:03:48.000000 auto_schema-0.0.8/MANIFEST.in
--rw-r--r--   0 ola        (501) staff       (20)      991 2021-08-02 18:02:43.393303 auto_schema-0.0.8/PKG-INFO
-drwxr-xr-x   0 ola        (501) staff       (20)        0 2021-08-02 18:02:43.391431 auto_schema-0.0.8/auto_schema/
--rw-r--r--   0 ola        (501) staff       (20)        0 2020-07-28 08:47:43.000000 auto_schema-0.0.8/auto_schema/__init__.py
--rw-r--r--   0 ola        (501) staff       (20)      787 2021-08-02 17:19:33.000000 auto_schema-0.0.8/auto_schema/change_type.py
--rw-r--r--   0 ola        (501) staff       (20)      710 2021-08-02 16:02:49.000000 auto_schema-0.0.8/auto_schema/clause_text.py
-drwxr-xr-x   0 ola        (501) staff       (20)        0 2021-08-02 18:02:43.392098 auto_schema-0.0.8/auto_schema/cli/
--rw-r--r--   0 ola        (501) staff       (20)     2745 2021-08-02 17:16:57.000000 auto_schema-0.0.8/auto_schema/cli/__init__.py
--rw-r--r--   0 ola        (501) staff       (20)     3241 2021-06-01 22:21:31.000000 auto_schema-0.0.8/auto_schema/command.py
--rw-r--r--   0 ola        (501) staff       (20)    13610 2021-03-30 22:54:22.000000 auto_schema-0.0.8/auto_schema/compare.py
--rw-r--r--   0 ola        (501) staff       (20)       34 2020-07-28 08:47:43.000000 auto_schema-0.0.8/auto_schema/config.py
--rw-r--r--   0 ola        (501) staff       (20)     6973 2021-08-02 17:58:09.000000 auto_schema-0.0.8/auto_schema/diff.py
--rw-r--r--   0 ola        (501) staff       (20)     3621 2021-03-30 22:54:22.000000 auto_schema-0.0.8/auto_schema/env.py
--rw-r--r--   0 ola        (501) staff       (20)    10530 2021-08-02 17:59:04.000000 auto_schema-0.0.8/auto_schema/ops.py
--rw-r--r--   0 ola        (501) staff       (20)     4697 2021-08-02 17:59:33.000000 auto_schema-0.0.8/auto_schema/ops_impl.py
--rw-r--r--   0 ola        (501) staff       (20)     5159 2021-08-02 17:59:23.000000 auto_schema-0.0.8/auto_schema/renderers.py
--rw-r--r--   0 ola        (501) staff       (20)     8905 2021-08-02 17:17:40.000000 auto_schema-0.0.8/auto_schema/runner.py
--rw-r--r--   0 ola        (501) staff       (20)      750 2021-03-30 22:54:22.000000 auto_schema-0.0.8/auto_schema/script.py.mako
--rw-r--r--   0 ola        (501) staff       (20)      199 2021-03-30 22:54:22.000000 auto_schema-0.0.8/auto_schema/util.py
-drwxr-xr-x   0 ola        (501) staff       (20)        0 2021-08-02 18:02:43.392007 auto_schema-0.0.8/auto_schema.egg-info/
--rw-r--r--   0 ola        (501) staff       (20)      991 2021-08-02 18:02:43.000000 auto_schema-0.0.8/auto_schema.egg-info/PKG-INFO
--rw-r--r--   0 ola        (501) staff       (20)      647 2021-08-02 18:02:43.000000 auto_schema-0.0.8/auto_schema.egg-info/SOURCES.txt
--rw-r--r--   0 ola        (501) staff       (20)        1 2021-08-02 18:02:43.000000 auto_schema-0.0.8/auto_schema.egg-info/dependency_links.txt
--rw-r--r--   0 ola        (501) staff       (20)       54 2021-08-02 18:02:43.000000 auto_schema-0.0.8/auto_schema.egg-info/entry_points.txt
--rw-r--r--   0 ola        (501) staff       (20)       80 2021-08-02 18:02:43.000000 auto_schema-0.0.8/auto_schema.egg-info/requires.txt
--rw-r--r--   0 ola        (501) staff       (20)       18 2021-08-02 18:02:43.000000 auto_schema-0.0.8/auto_schema.egg-info/top_level.txt
--rw-r--r--   0 ola        (501) staff       (20)       38 2021-08-02 18:02:43.393448 auto_schema-0.0.8/setup.cfg
--rw-r--r--   0 ola        (501) staff       (20)      965 2021-08-02 18:01:09.000000 auto_schema-0.0.8/setup.py
-drwxr-xr-x   0 ola        (501) staff       (20)        0 2021-08-02 18:02:43.392789 auto_schema-0.0.8/tests/
--rw-r--r--   0 ola        (501) staff       (20)        0 2020-07-28 08:47:43.000000 auto_schema-0.0.8/tests/__init__.py
--rw-r--r--   0 ola        (501) staff       (20)    32311 2021-08-02 16:55:41.000000 auto_schema-0.0.8/tests/conftest.py
--rw-r--r--   0 ola        (501) staff       (20)    53552 2021-08-02 16:57:36.000000 auto_schema-0.0.8/tests/runner_test.py
+drwxr-xr-x   0 ola        (501) staff       (20)        0 2021-08-03 17:37:30.496360 auto_schema-0.0.9/
+-rw-r--r--   0 ola        (501) staff       (20)     1075 2021-05-18 15:03:48.000000 auto_schema-0.0.9/LICENSE
+-rw-r--r--   0 ola        (501) staff       (20)       34 2021-05-18 15:03:48.000000 auto_schema-0.0.9/MANIFEST.in
+-rw-r--r--   0 ola        (501) staff       (20)      991 2021-08-03 17:37:30.496241 auto_schema-0.0.9/PKG-INFO
+drwxr-xr-x   0 ola        (501) staff       (20)        0 2021-08-03 17:37:30.494763 auto_schema-0.0.9/auto_schema/
+-rw-r--r--   0 ola        (501) staff       (20)        0 2020-07-28 08:47:43.000000 auto_schema-0.0.9/auto_schema/__init__.py
+-rw-r--r--   0 ola        (501) staff       (20)      858 2021-08-02 19:01:00.000000 auto_schema-0.0.9/auto_schema/change_type.py
+-rw-r--r--   0 ola        (501) staff       (20)      710 2021-08-02 18:31:50.000000 auto_schema-0.0.9/auto_schema/clause_text.py
+drwxr-xr-x   0 ola        (501) staff       (20)        0 2021-08-03 17:37:30.495537 auto_schema-0.0.9/auto_schema/cli/
+-rw-r--r--   0 ola        (501) staff       (20)     2733 2021-08-03 17:36:37.000000 auto_schema-0.0.9/auto_schema/cli/__init__.py
+-rw-r--r--   0 ola        (501) staff       (20)     3241 2021-06-01 22:21:31.000000 auto_schema-0.0.9/auto_schema/command.py
+-rw-r--r--   0 ola        (501) staff       (20)    13610 2021-03-30 22:54:22.000000 auto_schema-0.0.9/auto_schema/compare.py
+-rw-r--r--   0 ola        (501) staff       (20)       34 2020-07-28 08:47:43.000000 auto_schema-0.0.9/auto_schema/config.py
+-rw-r--r--   0 ola        (501) staff       (20)     6973 2021-08-02 18:31:50.000000 auto_schema-0.0.9/auto_schema/diff.py
+-rw-r--r--   0 ola        (501) staff       (20)     3621 2021-03-30 22:54:22.000000 auto_schema-0.0.9/auto_schema/env.py
+-rw-r--r--   0 ola        (501) staff       (20)    10530 2021-08-02 18:31:50.000000 auto_schema-0.0.9/auto_schema/ops.py
+-rw-r--r--   0 ola        (501) staff       (20)     4697 2021-08-02 18:31:50.000000 auto_schema-0.0.9/auto_schema/ops_impl.py
+-rw-r--r--   0 ola        (501) staff       (20)     5159 2021-08-02 18:31:50.000000 auto_schema-0.0.9/auto_schema/renderers.py
+-rw-r--r--   0 ola        (501) staff       (20)     8905 2021-08-02 18:31:50.000000 auto_schema-0.0.9/auto_schema/runner.py
+-rw-r--r--   0 ola        (501) staff       (20)      750 2021-03-30 22:54:22.000000 auto_schema-0.0.9/auto_schema/script.py.mako
+-rw-r--r--   0 ola        (501) staff       (20)      199 2021-03-30 22:54:22.000000 auto_schema-0.0.9/auto_schema/util.py
+drwxr-xr-x   0 ola        (501) staff       (20)        0 2021-08-03 17:37:30.495439 auto_schema-0.0.9/auto_schema.egg-info/
+-rw-r--r--   0 ola        (501) staff       (20)      991 2021-08-03 17:37:30.000000 auto_schema-0.0.9/auto_schema.egg-info/PKG-INFO
+-rw-r--r--   0 ola        (501) staff       (20)      647 2021-08-03 17:37:30.000000 auto_schema-0.0.9/auto_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 ola        (501) staff       (20)        1 2021-08-03 17:37:30.000000 auto_schema-0.0.9/auto_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 ola        (501) staff       (20)       54 2021-08-03 17:37:30.000000 auto_schema-0.0.9/auto_schema.egg-info/entry_points.txt
+-rw-r--r--   0 ola        (501) staff       (20)       80 2021-08-03 17:37:30.000000 auto_schema-0.0.9/auto_schema.egg-info/requires.txt
+-rw-r--r--   0 ola        (501) staff       (20)       18 2021-08-03 17:37:30.000000 auto_schema-0.0.9/auto_schema.egg-info/top_level.txt
+-rw-r--r--   0 ola        (501) staff       (20)       38 2021-08-03 17:37:30.496394 auto_schema-0.0.9/setup.cfg
+-rw-r--r--   0 ola        (501) staff       (20)      965 2021-08-03 17:37:03.000000 auto_schema-0.0.9/setup.py
+drwxr-xr-x   0 ola        (501) staff       (20)        0 2021-08-03 17:37:30.495987 auto_schema-0.0.9/tests/
+-rw-r--r--   0 ola        (501) staff       (20)        0 2020-07-28 08:47:43.000000 auto_schema-0.0.9/tests/__init__.py
+-rw-r--r--   0 ola        (501) staff       (20)    32311 2021-08-02 18:31:50.000000 auto_schema-0.0.9/tests/conftest.py
+-rw-r--r--   0 ola        (501) staff       (20)    53552 2021-08-02 18:31:50.000000 auto_schema-0.0.9/tests/runner_test.py
```

### Comparing `auto_schema-0.0.8/LICENSE` & `auto_schema-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_schema-0.0.8/PKG-INFO` & `auto_schema-0.0.9/auto_schema.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: auto_schema
-Version: 0.0.8
+Name: auto-schema
+Version: 0.0.9
 Summary: auto schema for a db
 Home-page: https://github.com/lolopinto/ent/tree/master/python/auto_schema
 Author: Ola Okelola
 Author-email: email@email.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `auto_schema-0.0.8/auto_schema/change_type.py` & `auto_schema-0.0.9/auto_schema/change_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from enum import Enum
 
 
 # subclass of str for enum encoding
+# NOTE: these need to be in sync with golang internal/schema/change.go
 class ChangeType(str, Enum):
     ADD_TABLE = "add_table"
     DROP_TABLE = "drop_table"
     ADD_COLUMN = "add_column"
     DROP_COLUMN = "drop_column"
     CREATE_INDEX = "create_index"
     DROP_INDEX = "drop_index"
```

### Comparing `auto_schema-0.0.8/auto_schema/clause_text.py` & `auto_schema-0.0.9/auto_schema/clause_text.py`

 * *Files identical despite different names*

### Comparing `auto_schema-0.0.8/auto_schema/cli/__init__.py` & `auto_schema-0.0.9/auto_schema/cli/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             r.branches()
         elif args.show is not None:
             r.show(args.show)
         elif args.stamp is not None:
             r.stamp(args.stamp)
         elif args.edit is not None:
             r.edit(args.edit)
-        elif args.changes is not None:
+        elif args.changes:
             r.changes()
         else:
             r.run()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `auto_schema-0.0.8/auto_schema/command.py` & `auto_schema-0.0.9/auto_schema/command.py`

 * *Files identical despite different names*

### Comparing `auto_schema-0.0.8/auto_schema/compare.py` & `auto_schema-0.0.9/auto_schema/compare.py`

 * *Files identical despite different names*

### Comparing `auto_schema-0.0.8/auto_schema/diff.py` & `auto_schema-0.0.9/auto_schema/diff.py`

 * *Files identical despite different names*

### Comparing `auto_schema-0.0.8/auto_schema/env.py` & `auto_schema-0.0.9/auto_schema/env.py`

 * *Files identical despite different names*

### Comparing `auto_schema-0.0.8/auto_schema/ops.py` & `auto_schema-0.0.9/auto_schema/ops.py`

 * *Files identical despite different names*

### Comparing `auto_schema-0.0.8/auto_schema/ops_impl.py` & `auto_schema-0.0.9/auto_schema/ops_impl.py`

 * *Files identical despite different names*

### Comparing `auto_schema-0.0.8/auto_schema/renderers.py` & `auto_schema-0.0.9/auto_schema/renderers.py`

 * *Files identical despite different names*

### Comparing `auto_schema-0.0.8/auto_schema/runner.py` & `auto_schema-0.0.9/auto_schema/runner.py`

 * *Files identical despite different names*

### Comparing `auto_schema-0.0.8/auto_schema/script.py.mako` & `auto_schema-0.0.9/auto_schema/script.py.mako`

 * *Files identical despite different names*

### Comparing `auto_schema-0.0.8/auto_schema.egg-info/PKG-INFO` & `auto_schema-0.0.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: auto-schema
-Version: 0.0.8
+Name: auto_schema
+Version: 0.0.9
 Summary: auto schema for a db
 Home-page: https://github.com/lolopinto/ent/tree/master/python/auto_schema
 Author: Ola Okelola
 Author-email: email@email.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `auto_schema-0.0.8/auto_schema.egg-info/SOURCES.txt` & `auto_schema-0.0.9/auto_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto_schema-0.0.8/setup.py` & `auto_schema-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="auto_schema",  # auto_schema_test to test
-    version="0.0.8",  # 0.0.5 was last test version
+    version="0.0.9",  # 0.0.5 was last test version
     author="Ola Okelola",
     author_email="email@email.com",
     description="auto schema for a db",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lolopinto/ent/tree/master/python/auto_schema",
     packages=setuptools.find_packages(),
```

### Comparing `auto_schema-0.0.8/tests/conftest.py` & `auto_schema-0.0.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `auto_schema-0.0.8/tests/runner_test.py` & `auto_schema-0.0.9/tests/runner_test.py`

 * *Files identical despite different names*

