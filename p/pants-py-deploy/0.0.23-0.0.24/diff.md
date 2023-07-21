# Comparing `tmp/pants_py_deploy-0.0.23-py3-none-any.whl.zip` & `tmp/pants_py_deploy-0.0.24-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 11588 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-06 13:37 pants_py_deploy/__init__.py
--rw-r--r--  2.0 unx     4820 b- defN 23-Jul-06 13:37 pants_py_deploy/compose_file.py
--rw-r--r--  2.0 unx     7083 b- defN 23-Jul-06 13:37 pants_py_deploy/export_env.py
--rw-r--r--  2.0 unx     1453 b- defN 23-Jul-06 13:37 pants_py_deploy/fields.py
--rw-r--r--  2.0 unx     4812 b- defN 23-Jul-06 13:37 pants_py_deploy/models.py
--rw-r--r--  2.0 unx    10518 b- defN 23-Jul-06 13:37 pants_py_deploy/plugin.py
--rw-r--r--  2.0 unx      581 b- defN 23-Jul-06 13:37 pants_py_deploy/register.py
--rw-r--r--  2.0 unx     2179 b- defN 23-Jul-06 13:37 pants_py_deploy-0.0.23.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 13:37 pants_py_deploy-0.0.23.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-06 13:37 pants_py_deploy-0.0.23.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx       16 b- defN 23-Jul-06 13:37 pants_py_deploy-0.0.23.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1028 b- defN 23-Jul-06 13:37 pants_py_deploy-0.0.23.dist-info/RECORD
-12 files, 32583 bytes uncompressed, 9838 bytes compressed:  69.8%
+Zip file size: 11589 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 08:47 pants_py_deploy/__init__.py
+-rw-r--r--  2.0 unx     4820 b- defN 23-Jul-21 08:47 pants_py_deploy/compose_file.py
+-rw-r--r--  2.0 unx     7083 b- defN 23-Jul-21 08:47 pants_py_deploy/export_env.py
+-rw-r--r--  2.0 unx     1453 b- defN 23-Jul-21 08:47 pants_py_deploy/fields.py
+-rw-r--r--  2.0 unx     4812 b- defN 23-Jul-21 08:47 pants_py_deploy/models.py
+-rw-r--r--  2.0 unx    10518 b- defN 23-Jul-21 08:47 pants_py_deploy/plugin.py
+-rw-r--r--  2.0 unx      581 b- defN 23-Jul-21 08:47 pants_py_deploy/register.py
+-rw-r--r--  2.0 unx     2179 b- defN 23-Jul-21 08:47 pants_py_deploy-0.0.24.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 08:47 pants_py_deploy-0.0.24.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-21 08:47 pants_py_deploy-0.0.24.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-21 08:47 pants_py_deploy-0.0.24.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1028 b- defN 23-Jul-21 08:47 pants_py_deploy-0.0.24.dist-info/RECORD
+12 files, 32583 bytes uncompressed, 9839 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: pants_py_deploy/plugin.py
 Comment: 
 
 Filename: pants_py_deploy/register.py
 Comment: 
 
-Filename: pants_py_deploy-0.0.23.dist-info/METADATA
+Filename: pants_py_deploy-0.0.24.dist-info/METADATA
 Comment: 
 
-Filename: pants_py_deploy-0.0.23.dist-info/WHEEL
+Filename: pants_py_deploy-0.0.24.dist-info/WHEEL
 Comment: 
 
-Filename: pants_py_deploy-0.0.23.dist-info/namespace_packages.txt
+Filename: pants_py_deploy-0.0.24.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: pants_py_deploy-0.0.23.dist-info/top_level.txt
+Filename: pants_py_deploy-0.0.24.dist-info/top_level.txt
 Comment: 
 
-Filename: pants_py_deploy-0.0.23.dist-info/RECORD
+Filename: pants_py_deploy-0.0.24.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pants_py_deploy-0.0.23.dist-info/METADATA` & `pants_py_deploy-0.0.24.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pants-py-deploy
-Version: 0.0.23
+Version: 0.0.24
 Summary: Make it easy to maintain docker-compose files and helm-charts across projects with pants-py-deploy
 Home-page: https://github.com/EspenAlbert/py-libs
 Author: Espen Albert
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: <3.10,>=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: compose-chart-export (==0.0.23)
-Requires-Dist: docker-compose-parser (==0.0.23)
-Requires-Dist: model-lib (==0.0.23)
+Requires-Dist: compose-chart-export (==0.0.24)
+Requires-Dist: docker-compose-parser (==0.0.24)
+Requires-Dist: model-lib (==0.0.24)
 Requires-Dist: pantsbuild.pants (<2.17,>=2.16.0a0)
-Requires-Dist: zero-3rdparty (==0.0.23)
+Requires-Dist: zero-3rdparty (==0.0.24)
 
 # Pants py_deploy plugin
 - Purpose: Make it easy to maintain docker-compose files and helm-charts across projects
 - Goals
   - Support updating services.{service_name}.
     - `environment` by scanning source code
     - `ports` by scanning source code
```

## Comparing `pants_py_deploy-0.0.23.dist-info/RECORD` & `pants_py_deploy-0.0.24.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pants_py_deploy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pants_py_deploy/compose_file.py,sha256=jc1kyOuc0XsBISQCm9yNs_yuwTVfwwY1T6HuXjYdp1c,4820
 pants_py_deploy/export_env.py,sha256=z0a7Sa2Lc4_7cFf9oH7rdoHjUqHgU-e6oshAQ9bm1Yg,7083
 pants_py_deploy/fields.py,sha256=EJwG5FndUPw17-AOVaNseZDmRZuVK46u6ZFYUMrAMlo,1453
 pants_py_deploy/models.py,sha256=PJHV-PFCayRC9KxpoTMjpO0iWiaO3H6q85xE6U4hnRs,4812
 pants_py_deploy/plugin.py,sha256=pI1ng6qKkC-Jo8PLZP7A6Td9tt6vpqjuiQBuMpK0eTs,10518
 pants_py_deploy/register.py,sha256=S9bQzA268aY9NXSfW-PvRuRKPvuFT-B86A3FvNbK53E,581
-pants_py_deploy-0.0.23.dist-info/METADATA,sha256=GbrDv7RppvFnPPC4GUtx62whM2z0MWC3kVi4iCcNKUE,2179
-pants_py_deploy-0.0.23.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pants_py_deploy-0.0.23.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-pants_py_deploy-0.0.23.dist-info/top_level.txt,sha256=6ImFjHnejcc1tZDfj2IB6KwifldxnUrXnYfA5rSHSmc,16
-pants_py_deploy-0.0.23.dist-info/RECORD,,
+pants_py_deploy-0.0.24.dist-info/METADATA,sha256=JK0ZLgRBEiYTf9BdO1zUcg6UJgsGPT2_winlwhfKGSk,2179
+pants_py_deploy-0.0.24.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pants_py_deploy-0.0.24.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+pants_py_deploy-0.0.24.dist-info/top_level.txt,sha256=6ImFjHnejcc1tZDfj2IB6KwifldxnUrXnYfA5rSHSmc,16
+pants_py_deploy-0.0.24.dist-info/RECORD,,
```

