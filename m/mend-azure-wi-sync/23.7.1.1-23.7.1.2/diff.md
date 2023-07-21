# Comparing `tmp/mend_azure_wi_sync-23.7.1.1-py3-none-any.whl.zip` & `tmp/mend_azure_wi_sync-23.7.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 25531 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 19:46 mend_azure_wi_sync/__init__.py
--rw-r--r--  2.0 unx      136 b- defN 23-Jul-21 19:46 mend_azure_wi_sync/_version.py
--rw-r--r--  2.0 unx     2858 b- defN 23-Jul-21 19:46 mend_azure_wi_sync/azure_wi_sync.py
--rw-r--r--  2.0 unx     4732 b- defN 23-Jul-21 19:46 mend_azure_wi_sync/config.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 19:46 mend_azure_wi_sync/conftest.py
--rw-r--r--  2.0 unx    49600 b- defN 23-Jul-21 19:46 mend_azure_wi_sync/core.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-21 19:47 mend_azure_wi_sync-23.7.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    17301 b- defN 23-Jul-21 19:47 mend_azure_wi_sync-23.7.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 19:47 mend_azure_wi_sync-23.7.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       72 b- defN 23-Jul-21 19:47 mend_azure_wi_sync-23.7.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-21 19:47 mend_azure_wi_sync-23.7.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1082 b- defN 23-Jul-21 19:47 mend_azure_wi_sync-23.7.1.1.dist-info/RECORD
-12 files, 87249 bytes uncompressed, 23673 bytes compressed:  72.9%
+Zip file size: 25530 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 20:00 mend_azure_wi_sync/__init__.py
+-rw-r--r--  2.0 unx      136 b- defN 23-Jul-21 20:00 mend_azure_wi_sync/_version.py
+-rw-r--r--  2.0 unx     2858 b- defN 23-Jul-21 20:00 mend_azure_wi_sync/azure_wi_sync.py
+-rw-r--r--  2.0 unx     4732 b- defN 23-Jul-21 20:00 mend_azure_wi_sync/config.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 20:00 mend_azure_wi_sync/conftest.py
+-rw-r--r--  2.0 unx    49600 b- defN 23-Jul-21 20:00 mend_azure_wi_sync/core.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-21 20:00 mend_azure_wi_sync-23.7.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    17301 b- defN 23-Jul-21 20:00 mend_azure_wi_sync-23.7.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 20:00 mend_azure_wi_sync-23.7.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       72 b- defN 23-Jul-21 20:00 mend_azure_wi_sync-23.7.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-21 20:00 mend_azure_wi_sync-23.7.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1082 b- defN 23-Jul-21 20:00 mend_azure_wi_sync-23.7.1.2.dist-info/RECORD
+12 files, 87249 bytes uncompressed, 23672 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: mend_azure_wi_sync/conftest.py
 Comment: 
 
 Filename: mend_azure_wi_sync/core.py
 Comment: 
 
-Filename: mend_azure_wi_sync-23.7.1.1.dist-info/LICENSE
+Filename: mend_azure_wi_sync-23.7.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: mend_azure_wi_sync-23.7.1.1.dist-info/METADATA
+Filename: mend_azure_wi_sync-23.7.1.2.dist-info/METADATA
 Comment: 
 
-Filename: mend_azure_wi_sync-23.7.1.1.dist-info/WHEEL
+Filename: mend_azure_wi_sync-23.7.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: mend_azure_wi_sync-23.7.1.1.dist-info/entry_points.txt
+Filename: mend_azure_wi_sync-23.7.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: mend_azure_wi_sync-23.7.1.1.dist-info/top_level.txt
+Filename: mend_azure_wi_sync-23.7.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: mend_azure_wi_sync-23.7.1.1.dist-info/RECORD
+Filename: mend_azure_wi_sync-23.7.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mend_azure_wi_sync/_version.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "23.7.1.1"
+__version__ = "23.7.1.2"
 __tool_name__ = "azure_wi_sync"
 __description__ = "Synchronize Mend SCA security alerts with Azure Work Items"
```

## Comparing `mend_azure_wi_sync-23.7.1.1.dist-info/LICENSE` & `mend_azure_wi_sync-23.7.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mend_azure_wi_sync-23.7.1.1.dist-info/METADATA` & `mend_azure_wi_sync-23.7.1.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mend-azure-wi-sync
-Version: 23.7.1.1
+Version: 23.7.1.2
 Summary: Synchronize Mend SCA security alerts with Azure Work Items
 Home-page: https://github.com/mend-toolkit/azure-wi-sync
 Author: Mend Professional Services
 Author-email: ps@mend.io
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `mend_azure_wi_sync-23.7.1.1.dist-info/RECORD` & `mend_azure_wi_sync-23.7.1.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 mend_azure_wi_sync/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mend_azure_wi_sync/_version.py,sha256=jplYyyleV9dkgh9g_zq6stf1BL_JApZXvT2_UwDZzDQ,136
+mend_azure_wi_sync/_version.py,sha256=mN3U3VFuLvnEi-eFyaZ81ODtqf7xMT9CA2-PTcGIy4M,136
 mend_azure_wi_sync/azure_wi_sync.py,sha256=gcxMu-1K_CYYrwRxFfUY-KXZ9ZHbv_Vo-xgX5GvOkEk,2858
 mend_azure_wi_sync/config.py,sha256=X56-0laXYxYMIDGJnTxqx9P0-CsAkMwVybhstFm6Y_g,4732
 mend_azure_wi_sync/conftest.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mend_azure_wi_sync/core.py,sha256=fPm2shfNkHGF3kc1VSWF3QoBtY9xOA9elqnI4BdjoyU,49600
-mend_azure_wi_sync-23.7.1.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mend_azure_wi_sync-23.7.1.1.dist-info/METADATA,sha256=THLEmcA2EEfAhO4mlx1Br9ZLD_-Bli70ysN4I3jK96I,17301
-mend_azure_wi_sync-23.7.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mend_azure_wi_sync-23.7.1.1.dist-info/entry_points.txt,sha256=txwI8MUUTLnmQQFCvAsVU3zJd-1VFkUlZi3fE6_c-WU,72
-mend_azure_wi_sync-23.7.1.1.dist-info/top_level.txt,sha256=TxzyE6DFEl2rNqUsHfd-wI-447X1ac926-EwaipUJvg,19
-mend_azure_wi_sync-23.7.1.1.dist-info/RECORD,,
+mend_azure_wi_sync-23.7.1.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mend_azure_wi_sync-23.7.1.2.dist-info/METADATA,sha256=6naUr9EKhzxKEq1_W4U8K6wZLJL5BJwGOsGDBFVf5f4,17301
+mend_azure_wi_sync-23.7.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mend_azure_wi_sync-23.7.1.2.dist-info/entry_points.txt,sha256=txwI8MUUTLnmQQFCvAsVU3zJd-1VFkUlZi3fE6_c-WU,72
+mend_azure_wi_sync-23.7.1.2.dist-info/top_level.txt,sha256=TxzyE6DFEl2rNqUsHfd-wI-447X1ac926-EwaipUJvg,19
+mend_azure_wi_sync-23.7.1.2.dist-info/RECORD,,
```

