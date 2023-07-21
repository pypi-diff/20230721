# Comparing `tmp/compose_chart_export-0.0.23-py3-none-any.whl.zip` & `tmp/compose_chart_export-0.0.24-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 13452 bytes, number of entries: 13
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-06 13:36 compose_chart_export/__init__.py
--rw-r--r--  2.0 unx     2517 b- defN 23-Jul-06 13:36 compose_chart_export/chart_export.py
--rw-r--r--  2.0 unx    14564 b- defN 23-Jul-06 13:36 compose_chart_export/chart_file_templates.py
--rw-r--r--  2.0 unx     4974 b- defN 23-Jul-06 13:36 compose_chart_export/chart_mods.py
--rw-r--r--  2.0 unx     2285 b- defN 23-Jul-06 13:36 compose_chart_export/chart_read.py
--rw-r--r--  2.0 unx     9945 b- defN 23-Jul-06 13:36 compose_chart_export/compose_export.py
--rw-r--r--  2.0 unx     2365 b- defN 23-Jul-06 13:36 compose_chart_export/ports.py
--rw-r--r--  2.0 unx      191 b- defN 23-Jul-06 13:36 compose_chart_export/settings.py
--rw-r--r--  2.0 unx      626 b- defN 23-Jul-06 13:36 compose_chart_export-0.0.23.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 13:36 compose_chart_export-0.0.23.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-06 13:36 compose_chart_export-0.0.23.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx       21 b- defN 23-Jul-06 13:36 compose_chart_export-0.0.23.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1199 b- defN 23-Jul-06 13:36 compose_chart_export-0.0.23.dist-info/RECORD
-13 files, 38780 bytes uncompressed, 11396 bytes compressed:  70.6%
+Zip file size: 13454 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 08:46 compose_chart_export/__init__.py
+-rw-r--r--  2.0 unx     2517 b- defN 23-Jul-21 08:46 compose_chart_export/chart_export.py
+-rw-r--r--  2.0 unx    14564 b- defN 23-Jul-21 08:46 compose_chart_export/chart_file_templates.py
+-rw-r--r--  2.0 unx     4974 b- defN 23-Jul-21 08:46 compose_chart_export/chart_mods.py
+-rw-r--r--  2.0 unx     2285 b- defN 23-Jul-21 08:46 compose_chart_export/chart_read.py
+-rw-r--r--  2.0 unx     9945 b- defN 23-Jul-21 08:46 compose_chart_export/compose_export.py
+-rw-r--r--  2.0 unx     2365 b- defN 23-Jul-21 08:46 compose_chart_export/ports.py
+-rw-r--r--  2.0 unx      191 b- defN 23-Jul-21 08:46 compose_chart_export/settings.py
+-rw-r--r--  2.0 unx      626 b- defN 23-Jul-21 08:46 compose_chart_export-0.0.24.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 08:46 compose_chart_export-0.0.24.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-21 08:46 compose_chart_export-0.0.24.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-Jul-21 08:46 compose_chart_export-0.0.24.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1199 b- defN 23-Jul-21 08:46 compose_chart_export-0.0.24.dist-info/RECORD
+13 files, 38780 bytes uncompressed, 11398 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: compose_chart_export/ports.py
 Comment: 
 
 Filename: compose_chart_export/settings.py
 Comment: 
 
-Filename: compose_chart_export-0.0.23.dist-info/METADATA
+Filename: compose_chart_export-0.0.24.dist-info/METADATA
 Comment: 
 
-Filename: compose_chart_export-0.0.23.dist-info/WHEEL
+Filename: compose_chart_export-0.0.24.dist-info/WHEEL
 Comment: 
 
-Filename: compose_chart_export-0.0.23.dist-info/namespace_packages.txt
+Filename: compose_chart_export-0.0.24.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: compose_chart_export-0.0.23.dist-info/top_level.txt
+Filename: compose_chart_export-0.0.24.dist-info/top_level.txt
 Comment: 
 
-Filename: compose_chart_export-0.0.23.dist-info/RECORD
+Filename: compose_chart_export-0.0.24.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `compose_chart_export-0.0.23.dist-info/METADATA` & `compose_chart_export-0.0.24.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: compose-chart-export
-Version: 0.0.23
+Version: 0.0.24
 Summary: compose_agent_export for docker-compose -> helm chart
 Author: Espen
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
-Requires-Dist: docker-compose-parser (==0.0.23)
-Requires-Dist: model-lib (==0.0.23)
+Requires-Dist: docker-compose-parser (==0.0.24)
+Requires-Dist: model-lib (==0.0.24)
 Requires-Dist: pydantic (==1.10.2)
 Requires-Dist: semver (==2.13.0)
 Requires-Dist: typing-extensions (>=4.3.0)
-Requires-Dist: zero-3rdparty (==0.0.23)
+Requires-Dist: zero-3rdparty (==0.0.24)
 
 # Compose Chart Export
 - Uses `docker-compose.yaml` to generate a helm chart
 - Supports various customizations using labels
```

## Comparing `compose_chart_export-0.0.23.dist-info/RECORD` & `compose_chart_export-0.0.24.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 compose_chart_export/chart_export.py,sha256=lRtxzU3Ac2SfOAxZmSv9ml0KsDM4tHx5ois0BOFF9dc,2517
 compose_chart_export/chart_file_templates.py,sha256=sQMgnbhaCgppTOO5XZD72YbshNJS90INvCENukeNY3w,14564
 compose_chart_export/chart_mods.py,sha256=6eaO7tuccQWcZDc_yoi3p7aIOO2YQ4vAb2aqKZ5qBzc,4974
 compose_chart_export/chart_read.py,sha256=5A7mcFdq1lnD7fitj5-evHE9A0zJ6aAlY0KEYPmeRZo,2285
 compose_chart_export/compose_export.py,sha256=E8_y5HfKed20hKcb4GrUFP9QkoAHa6l4my3nFwr3AzI,9945
 compose_chart_export/ports.py,sha256=ubPaqe31gwDqPj8s4Bd6pZf8qB02hylpoQpYpbFkYwc,2365
 compose_chart_export/settings.py,sha256=-vo5OY1ttQUeGQwihuX2YTD-qHRgvBdMuRwP_BelWQY,191
-compose_chart_export-0.0.23.dist-info/METADATA,sha256=PGOyty8uZnWW0oAnFe5jBbRpyHZkjD4SG-9F0QYfzuw,626
-compose_chart_export-0.0.23.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-compose_chart_export-0.0.23.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-compose_chart_export-0.0.23.dist-info/top_level.txt,sha256=leubfJ1d95x8SfDGSVFPIHT8AGgj9xYF0CMorIbq3uo,21
-compose_chart_export-0.0.23.dist-info/RECORD,,
+compose_chart_export-0.0.24.dist-info/METADATA,sha256=cKZ3gVWc0A3AkCFgCAT4BulTgTr8kMExir9d2eRu9z4,626
+compose_chart_export-0.0.24.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+compose_chart_export-0.0.24.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+compose_chart_export-0.0.24.dist-info/top_level.txt,sha256=leubfJ1d95x8SfDGSVFPIHT8AGgj9xYF0CMorIbq3uo,21
+compose_chart_export-0.0.24.dist-info/RECORD,,
```

