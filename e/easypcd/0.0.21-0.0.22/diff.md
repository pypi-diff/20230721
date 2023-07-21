# Comparing `tmp/easypcd-0.0.21-py3-none-any.whl.zip` & `tmp/easypcd-0.0.22-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1724 bytes, number of entries: 4
--rw-rw-rw-  2.0 fat     1275 b- defN 23-Jul-21 09:09 easypcd-0.0.21.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jul-21 09:09 easypcd-0.0.21.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jul-21 09:09 easypcd-0.0.21.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      301 b- defN 23-Jul-21 09:09 easypcd-0.0.21.dist-info/RECORD
-4 files, 1674 bytes uncompressed, 1134 bytes compressed:  32.3%
+Zip file size: 1727 bytes, number of entries: 4
+-rw-rw-rw-  2.0 fat     1275 b- defN 23-Jul-21 09:12 easypcd-0.0.22.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jul-21 09:12 easypcd-0.0.22.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jul-21 09:12 easypcd-0.0.22.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      301 b- defN 23-Jul-21 09:12 easypcd-0.0.22.dist-info/RECORD
+4 files, 1674 bytes uncompressed, 1137 bytes compressed:  32.1%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: easypcd-0.0.21.dist-info/METADATA
+Filename: easypcd-0.0.22.dist-info/METADATA
 Comment: 
 
-Filename: easypcd-0.0.21.dist-info/WHEEL
+Filename: easypcd-0.0.22.dist-info/WHEEL
 Comment: 
 
-Filename: easypcd-0.0.21.dist-info/top_level.txt
+Filename: easypcd-0.0.22.dist-info/top_level.txt
 Comment: 
 
-Filename: easypcd-0.0.21.dist-info/RECORD
+Filename: easypcd-0.0.22.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `easypcd-0.0.21.dist-info/METADATA` & `easypcd-0.0.22.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easypcd
-Version: 0.0.21
+Version: 0.0.22
 Summary: a package for pcd
 Home-page: https://blog.csdn.net/qq_18566467?spm=1010.2135.3001.5343
 Author: GentleWang
 Author-email: 189030005@stu.just.edu.cn
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Requires-Dist: numpy
 Requires-Dist: opencv-python
 
 ### Easypcd使你更专注与代码本身，而不需要因为pcd格式所带来的烦恼。  
 
 #### 1、调用easypcd
 
-`From easypcd import easypcd`  
+`from easypcd import easypcd`  
 `ep = easypcd()`
 
 **2、 读取pcd文件**  
 `pcd = ep.read_pcd("point.pcd")# 读取pcd文件  `  
 `print(“point indormation:”, pcd)# 打印所有信息  `  
 `print(“point:”, pcd.point)# 打印点云  `
```

