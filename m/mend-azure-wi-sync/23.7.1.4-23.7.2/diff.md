# Comparing `tmp/mend_azure_wi_sync-23.7.1.4-py3-none-any.whl.zip` & `tmp/mend_azure_wi_sync-23.7.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 25531 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 20:10 mend_azure_wi_sync/__init__.py
--rw-r--r--  2.0 unx      136 b- defN 23-Jul-21 20:10 mend_azure_wi_sync/_version.py
--rw-r--r--  2.0 unx     2858 b- defN 23-Jul-21 20:10 mend_azure_wi_sync/azure_wi_sync.py
--rw-r--r--  2.0 unx     4732 b- defN 23-Jul-21 20:10 mend_azure_wi_sync/config.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 20:10 mend_azure_wi_sync/conftest.py
--rw-r--r--  2.0 unx    49600 b- defN 23-Jul-21 20:10 mend_azure_wi_sync/core.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-21 20:10 mend_azure_wi_sync-23.7.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx    17301 b- defN 23-Jul-21 20:10 mend_azure_wi_sync-23.7.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 20:10 mend_azure_wi_sync-23.7.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       72 b- defN 23-Jul-21 20:10 mend_azure_wi_sync-23.7.1.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-21 20:10 mend_azure_wi_sync-23.7.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1082 b- defN 23-Jul-21 20:10 mend_azure_wi_sync-23.7.1.4.dist-info/RECORD
-12 files, 87249 bytes uncompressed, 23673 bytes compressed:  72.9%
+Zip file size: 25500 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 20:14 mend_azure_wi_sync/__init__.py
+-rw-r--r--  2.0 unx      134 b- defN 23-Jul-21 20:14 mend_azure_wi_sync/_version.py
+-rw-r--r--  2.0 unx     2858 b- defN 23-Jul-21 20:14 mend_azure_wi_sync/azure_wi_sync.py
+-rw-r--r--  2.0 unx     4732 b- defN 23-Jul-21 20:14 mend_azure_wi_sync/config.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 20:14 mend_azure_wi_sync/conftest.py
+-rw-r--r--  2.0 unx    49600 b- defN 23-Jul-21 20:14 mend_azure_wi_sync/core.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-21 20:14 mend_azure_wi_sync-23.7.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    17299 b- defN 23-Jul-21 20:14 mend_azure_wi_sync-23.7.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 20:14 mend_azure_wi_sync-23.7.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       72 b- defN 23-Jul-21 20:14 mend_azure_wi_sync-23.7.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-21 20:14 mend_azure_wi_sync-23.7.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1070 b- defN 23-Jul-21 20:14 mend_azure_wi_sync-23.7.2.dist-info/RECORD
+12 files, 87233 bytes uncompressed, 23666 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: mend_azure_wi_sync/conftest.py
 Comment: 
 
 Filename: mend_azure_wi_sync/core.py
 Comment: 
 
-Filename: mend_azure_wi_sync-23.7.1.4.dist-info/LICENSE
+Filename: mend_azure_wi_sync-23.7.2.dist-info/LICENSE
 Comment: 
 
-Filename: mend_azure_wi_sync-23.7.1.4.dist-info/METADATA
+Filename: mend_azure_wi_sync-23.7.2.dist-info/METADATA
 Comment: 
 
-Filename: mend_azure_wi_sync-23.7.1.4.dist-info/WHEEL
+Filename: mend_azure_wi_sync-23.7.2.dist-info/WHEEL
 Comment: 
 
-Filename: mend_azure_wi_sync-23.7.1.4.dist-info/entry_points.txt
+Filename: mend_azure_wi_sync-23.7.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: mend_azure_wi_sync-23.7.1.4.dist-info/top_level.txt
+Filename: mend_azure_wi_sync-23.7.2.dist-info/top_level.txt
 Comment: 
 
-Filename: mend_azure_wi_sync-23.7.1.4.dist-info/RECORD
+Filename: mend_azure_wi_sync-23.7.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mend_azure_wi_sync/_version.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "23.7.1.4"
+__version__ = "23.7.2"
 __tool_name__ = "azure_wi_sync"
 __description__ = "Synchronize Mend SCA security alerts with Azure Work Items"
```

## Comparing `mend_azure_wi_sync-23.7.1.4.dist-info/LICENSE` & `mend_azure_wi_sync-23.7.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mend_azure_wi_sync-23.7.1.4.dist-info/METADATA` & `mend_azure_wi_sync-23.7.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mend-azure-wi-sync
-Version: 23.7.1.4
+Version: 23.7.2
 Summary: Synchronize Mend SCA security alerts with Azure Work Items
 Home-page: https://github.com/mend-toolkit/azure-wi-sync
 Author: Mend Professional Services
 Author-email: ps@mend.io
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

