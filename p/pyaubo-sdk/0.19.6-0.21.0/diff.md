# Comparing `tmp/pyaubo_sdk-0.19.6-cp39-cp39-win_amd64.whl.zip` & `tmp/pyaubo_sdk-0.21.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 584467 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat  1838592 b- defN 23-Mar-16 08:44 pyaubo_sdk.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      381 b- defN 23-Mar-16 08:44 pyaubo_sdk.cp39-win_amd64.pyd.manifest
--rw-rw-rw-  2.0 fat     2459 b- defN 23-Mar-16 08:44 pyaubo_sdk-0.19.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Mar-16 08:44 pyaubo_sdk-0.19.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Mar-16 08:44 pyaubo_sdk-0.19.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      497 b- defN 23-Mar-16 08:44 pyaubo_sdk-0.19.6.dist-info/RECORD
-6 files, 1842030 bytes uncompressed, 583567 bytes compressed:  68.3%
+Zip file size: 625238 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat  1956352 b- defN 23-Jul-21 07:58 pyaubo_sdk.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      381 b- defN 23-Jul-21 07:58 pyaubo_sdk.cp39-win_amd64.pyd.manifest
+-rw-rw-rw-  2.0 fat     2424 b- defN 23-Jul-21 07:59 pyaubo_sdk-0.21.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-21 07:59 pyaubo_sdk-0.21.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jul-21 07:59 pyaubo_sdk-0.21.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      497 b- defN 23-Jul-21 07:59 pyaubo_sdk-0.21.0.dist-info/RECORD
+6 files, 1959755 bytes uncompressed, 624338 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pyaubo_sdk.cp39-win_amd64.pyd
 Comment: 
 
 Filename: pyaubo_sdk.cp39-win_amd64.pyd.manifest
 Comment: 
 
-Filename: pyaubo_sdk-0.19.6.dist-info/METADATA
+Filename: pyaubo_sdk-0.21.0.dist-info/METADATA
 Comment: 
 
-Filename: pyaubo_sdk-0.19.6.dist-info/WHEEL
+Filename: pyaubo_sdk-0.21.0.dist-info/WHEEL
 Comment: 
 
-Filename: pyaubo_sdk-0.19.6.dist-info/top_level.txt
+Filename: pyaubo_sdk-0.21.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pyaubo_sdk-0.19.6.dist-info/RECORD
+Filename: pyaubo_sdk-0.21.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyaubo_sdk-0.19.6.dist-info/METADATA` & `pyaubo_sdk-0.21.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: pyaubo-sdk
-Version: 0.19.6
+Version: 0.21.0
 Summary: A Python interface for controlling aubo robot 
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6, <=3.11
 Description-Content-Type: text/markdown
-Provides-Extra: cmake
-Requires-Dist: Cmake-version (>=3.16) ; extra == 'cmake'
-Provides-Extra: g_
-Requires-Dist: version (>=7.x.x) ; extra == 'g_'
 
 <div align="center">
   <h1 align="center">aubo_sdk</h1>
   <h3 align="center">
     ARCS controller software secondary development interface
   </h3>
 </div>
@@ -54,18 +50,18 @@
 If you only want to the use the Python interface, you can install pyaubo_sdk through pip:
 
 ```bash
 pip3 install pyaubo_sdk
 ```
 
 ### Prebuilt python wheels support matrix: ###
-|                | Python3.7 | Python3.8 | Python3.9 | Python3.10 |
-| :------------: | :-------: | :-------: | :-------: | :--------: |
-|   linux x64    |     ✅     |     ✅     |     ✅     |     ✅      |
-| windows 64 bit |           |           |     ✅     |     ✅      |
+|                | Python3.6 | Python3.7 | Python3.8 | Python3.9 | Python3.10 | Python3.11 |
+| :------------: | :-------: | :-------: | :-------: | :-------: | :--------: | :--------: |
+|   linux x64    |     ✅     |     ✅     |     ✅     |     ✅     |     ✅      |     ✅      |
+| windows 64 bit |     ✅     |     ✅     |     ✅     |     ✅     |     ✅      |     ✅      |
 
 ### Dependencies ###
 *  If you're running Linux , you may need to install gcc-7/g++-7
 *  If you're running windows , you may need to install visual studio 2019 or later
 
 ### Compatible Operating Systems ###
 Currently tested on:
```

