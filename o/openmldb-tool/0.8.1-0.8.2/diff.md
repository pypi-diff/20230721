# Comparing `tmp/openmldb_tool-0.8.1-py3-none-any.whl.zip` & `tmp/openmldb_tool-0.8.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
 Zip file size: 25497 bytes, number of entries: 16
--rw-r--r--  2.0 unx      571 b- defN 23-Jun-15 09:19 diagnostic_tool/__init__.py
--rw-r--r--  2.0 unx     9672 b- defN 23-Jun-15 09:19 diagnostic_tool/collector.py
--rw-r--r--  2.0 unx    11416 b- defN 23-Jun-15 09:19 diagnostic_tool/conf_validator.py
--rw-r--r--  2.0 unx     2027 b- defN 23-Jun-15 09:19 diagnostic_tool/connector.py
--rw-r--r--  2.0 unx    12128 b- defN 23-Jun-16 09:47 diagnostic_tool/diagnose.py
--rw-r--r--  2.0 unx     9205 b- defN 23-Jun-15 09:19 diagnostic_tool/dist_conf.py
--rw-r--r--  2.0 unx     4958 b- defN 23-Jun-15 09:19 diagnostic_tool/log_analyzer.py
--rw-r--r--  2.0 unx     2657 b- defN 23-Jun-16 09:47 diagnostic_tool/parser.py
--rw-r--r--  2.0 unx     7914 b- defN 23-Jun-15 09:19 diagnostic_tool/server_checker.py
--rw-r--r--  2.0 unx     5153 b- defN 23-Jun-16 09:47 diagnostic_tool/table_checker.py
--rw-r--r--  2.0 unx     3042 b- defN 23-Jun-15 09:19 diagnostic_tool/util.py
--rw-r--r--  2.0 unx      491 b- defN 23-Jun-29 08:20 openmldb_tool-0.8.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 08:20 openmldb_tool-0.8.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       64 b- defN 23-Jun-29 08:20 openmldb_tool-0.8.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-29 08:20 openmldb_tool-0.8.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1365 b- defN 23-Jun-29 08:20 openmldb_tool-0.8.1.dist-info/RECORD
+-rw-r--r--  2.0 unx      571 b- defN 23-Apr-13 06:22 diagnostic_tool/__init__.py
+-rw-r--r--  2.0 unx     9672 b- defN 23-Apr-13 06:22 diagnostic_tool/collector.py
+-rw-r--r--  2.0 unx    11416 b- defN 23-Apr-13 06:22 diagnostic_tool/conf_validator.py
+-rw-r--r--  2.0 unx     2027 b- defN 23-Apr-13 06:22 diagnostic_tool/connector.py
+-rw-r--r--  2.0 unx    12128 b- defN 23-Jul-21 00:50 diagnostic_tool/diagnose.py
+-rw-r--r--  2.0 unx     9205 b- defN 23-Apr-13 06:22 diagnostic_tool/dist_conf.py
+-rw-r--r--  2.0 unx     4958 b- defN 23-Apr-13 06:22 diagnostic_tool/log_analyzer.py
+-rw-r--r--  2.0 unx     2657 b- defN 23-Jul-21 00:50 diagnostic_tool/parser.py
+-rw-r--r--  2.0 unx     7914 b- defN 23-Jul-21 00:50 diagnostic_tool/server_checker.py
+-rw-r--r--  2.0 unx     5153 b- defN 23-Jul-21 00:50 diagnostic_tool/table_checker.py
+-rw-r--r--  2.0 unx     3042 b- defN 23-Apr-13 06:22 diagnostic_tool/util.py
+-rw-r--r--  2.0 unx      491 b- defN 23-Jul-21 01:01 openmldb_tool-0.8.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 01:01 openmldb_tool-0.8.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       64 b- defN 23-Jul-21 01:01 openmldb_tool-0.8.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-21 01:01 openmldb_tool-0.8.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1365 b- defN 23-Jul-21 01:01 openmldb_tool-0.8.2.dist-info/RECORD
 16 files, 70771 bytes uncompressed, 23233 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: diagnostic_tool/table_checker.py
 Comment: 
 
 Filename: diagnostic_tool/util.py
 Comment: 
 
-Filename: openmldb_tool-0.8.1.dist-info/METADATA
+Filename: openmldb_tool-0.8.2.dist-info/METADATA
 Comment: 
 
-Filename: openmldb_tool-0.8.1.dist-info/WHEEL
+Filename: openmldb_tool-0.8.2.dist-info/WHEEL
 Comment: 
 
-Filename: openmldb_tool-0.8.1.dist-info/entry_points.txt
+Filename: openmldb_tool-0.8.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: openmldb_tool-0.8.1.dist-info/top_level.txt
+Filename: openmldb_tool-0.8.2.dist-info/top_level.txt
 Comment: 
 
-Filename: openmldb_tool-0.8.1.dist-info/RECORD
+Filename: openmldb_tool-0.8.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `openmldb_tool-0.8.1.dist-info/RECORD` & `openmldb_tool-0.8.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -5,12 +5,12 @@
 diagnostic_tool/diagnose.py,sha256=ERCACWEeCdCiIF9ulfJUTZEe3i7cLwMJAFr-kF-tLvk,12128
 diagnostic_tool/dist_conf.py,sha256=57NQjOZAJBp2zzTCP7nWMNBfnOOeEqOhrKNLKB2T3Kc,9205
 diagnostic_tool/log_analyzer.py,sha256=9-RT1oqUeAZGxey743_gZKBWO_8cROFerNyy_VRcADM,4958
 diagnostic_tool/parser.py,sha256=kW7tYXXrt7eln0W6Kkg-irNgJj6W0k4II3uO5uEFWBk,2657
 diagnostic_tool/server_checker.py,sha256=QpPiPHEqa_Bx3-NUa_bEyxFKJVuHXVj0J9NnETy5L1Q,7914
 diagnostic_tool/table_checker.py,sha256=E99BizQfwfKtVh5mF7WyULuv8jnOy4sgV_xD4bDQShU,5153
 diagnostic_tool/util.py,sha256=rj21SHz8vhLoWGTakmd7grlqym0AWRpDShaoqA83XJ4,3042
-openmldb_tool-0.8.1.dist-info/METADATA,sha256=Wo3D84SEQ-ausPHCsSQMXt6FW2P8EUirmD6oHCIAaDA,491
-openmldb_tool-0.8.1.dist-info/WHEEL,sha256=p46_5Uhzqz6AzeSosiOnxK-zmFja1i22CrQCjmYe8ec,92
-openmldb_tool-0.8.1.dist-info/entry_points.txt,sha256=aUVKKZotgPl1Tb82p74g-W1ARley8qP0CXvjXL3jmNg,64
-openmldb_tool-0.8.1.dist-info/top_level.txt,sha256=l3w2A2Oy57wqrgi95wfEAxdmJsz7Umeoxf5WMObkJb4,16
-openmldb_tool-0.8.1.dist-info/RECORD,,
+openmldb_tool-0.8.2.dist-info/METADATA,sha256=GEbmwi_FN5fXSk41XV9toevj8ORwsiwfRI1oRZ93ZDc,491
+openmldb_tool-0.8.2.dist-info/WHEEL,sha256=p46_5Uhzqz6AzeSosiOnxK-zmFja1i22CrQCjmYe8ec,92
+openmldb_tool-0.8.2.dist-info/entry_points.txt,sha256=aUVKKZotgPl1Tb82p74g-W1ARley8qP0CXvjXL3jmNg,64
+openmldb_tool-0.8.2.dist-info/top_level.txt,sha256=l3w2A2Oy57wqrgi95wfEAxdmJsz7Umeoxf5WMObkJb4,16
+openmldb_tool-0.8.2.dist-info/RECORD,,
```

