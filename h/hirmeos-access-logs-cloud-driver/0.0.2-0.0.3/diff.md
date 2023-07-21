# Comparing `tmp/hirmeos_access_logs_cloud_driver-0.0.2-py3-none-any.whl.zip` & `tmp/hirmeos_access_logs_cloud_driver-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1867 bytes, number of entries: 4
--rw-rw-r--  2.0 unx     1287 b- defN 23-Jul-12 08:07 hirmeos_access_logs_cloud_driver-0.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-12 08:07 hirmeos_access_logs_cloud_driver-0.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       25 b- defN 23-Jul-12 08:07 hirmeos_access_logs_cloud_driver-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      398 b- defN 23-Jul-12 08:07 hirmeos_access_logs_cloud_driver-0.0.2.dist-info/RECORD
-4 files, 1802 bytes uncompressed, 1085 bytes compressed:  39.8%
+Zip file size: 1887 bytes, number of entries: 4
+-rw-rw-r--  2.0 unx     1333 b- defN 23-Jul-21 16:26 hirmeos_access_logs_cloud_driver-0.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-21 16:26 hirmeos_access_logs_cloud_driver-0.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       25 b- defN 23-Jul-21 16:26 hirmeos_access_logs_cloud_driver-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      398 b- defN 23-Jul-21 16:26 hirmeos_access_logs_cloud_driver-0.0.3.dist-info/RECORD
+4 files, 1848 bytes uncompressed, 1105 bytes compressed:  40.2%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: hirmeos_access_logs_cloud_driver-0.0.2.dist-info/METADATA
+Filename: hirmeos_access_logs_cloud_driver-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: hirmeos_access_logs_cloud_driver-0.0.2.dist-info/WHEEL
+Filename: hirmeos_access_logs_cloud_driver-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: hirmeos_access_logs_cloud_driver-0.0.2.dist-info/top_level.txt
+Filename: hirmeos_access_logs_cloud_driver-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: hirmeos_access_logs_cloud_driver-0.0.2.dist-info/RECORD
+Filename: hirmeos_access_logs_cloud_driver-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `hirmeos_access_logs_cloud_driver-0.0.2.dist-info/METADATA` & `hirmeos_access_logs_cloud_driver-0.0.3.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hirmeos-access-logs-cloud-driver
-Version: 0.0.2
-Summary: Functions required by the access-logs-cloud-driver
+Version: 0.0.3
+Summary: Functions required by the access-logs-local-driver
 Home-page: https://github.com/hirmeos/access_logs_driver
 Author: Cristian Garcia
 Author-email: cristian.garcia@ubiquitypress.com
 Description-Content-Type: text/markdown
 Requires-Dist: hirmeos-clients (>=0.1.6)
 Requires-Dist: httplib2 (==0.12.1)
 
@@ -29,7 +29,8 @@
 [0.0.2] - 2023-07-11
 
 Added:
     * Unittests
 
 Changed:
     * Moved the files out of the package and get the file's data as parameters and return the filtered data.
+    * renamed the plugin to access-logs-local
```

