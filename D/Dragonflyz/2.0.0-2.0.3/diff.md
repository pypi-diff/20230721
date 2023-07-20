# Comparing `tmp/Dragonflyz-2.0.0-py3-none-any.whl.zip` & `tmp/Dragonflyz-2.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 10630 bytes, number of entries: 10
+Zip file size: 10738 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx      235 b- defN 23-Jul-20 22:53 Dragonflyz/__init__.py
--rw-rw-r--  2.0 unx     2106 b- defN 23-Feb-08 04:36 Dragonflyz/energy.py
+-rw-rw-r--  2.0 unx     2370 b- defN 23-Jul-20 23:09 Dragonflyz/energy.py
 -rw-rw-r--  2.0 unx     5542 b- defN 23-Feb-08 04:36 Dragonflyz/gantt.py
 -rw-rw-r--  2.0 unx     4209 b- defN 23-Jul-20 22:14 Dragonflyz/sensor_info.py
 -rw-rw-r--  2.0 unx     3488 b- defN 23-Jul-20 22:37 Dragonflyz/system_utils.py
--rwxr-xr-x  2.0 unx     1070 b- defN 23-Jul-20 23:02 Dragonflyz-2.0.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     6846 b- defN 23-Jul-20 23:02 Dragonflyz-2.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-20 23:02 Dragonflyz-2.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Jul-20 23:02 Dragonflyz-2.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      797 b- defN 23-Jul-20 23:02 Dragonflyz-2.0.0.dist-info/RECORD
-10 files, 24396 bytes uncompressed, 9276 bytes compressed:  62.0%
+-rwxr-xr-x  2.0 unx     1070 b- defN 23-Jul-20 23:13 Dragonflyz-2.0.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     6814 b- defN 23-Jul-20 23:13 Dragonflyz-2.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-20 23:13 Dragonflyz-2.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jul-20 23:13 Dragonflyz-2.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      797 b- defN 23-Jul-20 23:13 Dragonflyz-2.0.3.dist-info/RECORD
+10 files, 24628 bytes uncompressed, 9384 bytes compressed:  61.9%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: Dragonflyz/sensor_info.py
 Comment: 
 
 Filename: Dragonflyz/system_utils.py
 Comment: 
 
-Filename: Dragonflyz-2.0.0.dist-info/LICENSE
+Filename: Dragonflyz-2.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: Dragonflyz-2.0.0.dist-info/METADATA
+Filename: Dragonflyz-2.0.3.dist-info/METADATA
 Comment: 
 
-Filename: Dragonflyz-2.0.0.dist-info/WHEEL
+Filename: Dragonflyz-2.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: Dragonflyz-2.0.0.dist-info/top_level.txt
+Filename: Dragonflyz-2.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: Dragonflyz-2.0.0.dist-info/RECORD
+Filename: Dragonflyz-2.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Dragonflyz/energy.py

```diff
@@ -1,13 +1,22 @@
 import os
 import time
 import functools
-from PenguinServices import verifyFolder, openFile
+# from PenguinServices import verifyFolder, openFile
 import panel as pn
 
+def verifyFoler(path):
+    return path if path[-1] == "\" else path + "\"
+    
+def openFile(path, splitLines: bool = True):
+    with open(path) as reader:
+        data = reader.read().strip()
+        
+    return data if not splitLines else data.split('\n')
+    
 class EnergyTracer:
     def __init__(self, intervalSecs = 0.5):
         self.vals = {} # first ones in lists are baseline
         self.intervalSecs = intervalSecs
         
         self.setup()
```

## Comparing `Dragonflyz-2.0.0.dist-info/LICENSE` & `Dragonflyz-2.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Dragonflyz-2.0.0.dist-info/METADATA` & `Dragonflyz-2.0.3.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: Dragonflyz
-Version: 2.0.0
+Version: 2.0.3
 Summary: Package for Code Analysis across your scripts
 Home-page: https://github.com/jacob-h-barrow/Dragonflyz
 Author: Jacob H Barrow
 Author-email: jacob.h.barrow@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Penguin-Services
 Requires-Dist: dataclasses
 Requires-Dist: matplotlib
 Requires-Dist: panel
 
 # Dragonflyz
 [![Test Coverage](https://img.shields.io/badge/Test%20Coverage-100%25-success)](https://github.com/jacob-h-barrow/Penguin-Services)
 [![Security](https://img.shields.io/badge/Secure-True-informational)](https://github.com/jacob-h-barrow/Penguin-Services)
```

## Comparing `Dragonflyz-2.0.0.dist-info/RECORD` & `Dragonflyz-2.0.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Dragonflyz/__init__.py,sha256=ZmWoOdP0bJNTgAtUClKNVAAxgQwccQeLaNvgMzuY8xk,235
-Dragonflyz/energy.py,sha256=BQUiyXl5VtW0MoAVr2pQWyC_NBccXjDcO6LG_5TkBCE,2106
+Dragonflyz/energy.py,sha256=ECJFT0iApxCOznOAbD2lLTq0pk1SJlRvjt24dK65AnY,2370
 Dragonflyz/gantt.py,sha256=XnE0Sb32bJq2cswVXF70UpwF8RM6kHAF7bvCI69Tn2c,5542
 Dragonflyz/sensor_info.py,sha256=X_Y5L28a9I5LBcebKuVUxaR4kHINdw-2M0-jdCdsRAw,4209
 Dragonflyz/system_utils.py,sha256=ouV17Mf_6KcsEOkJia7UcsaL0Fv47WSeCDNMrQ_FCFI,3488
-Dragonflyz-2.0.0.dist-info/LICENSE,sha256=uBr-ac1MfmxnzaovoKntc1ElNSIBVYTy5ogR3PpKzT0,1070
-Dragonflyz-2.0.0.dist-info/METADATA,sha256=HtztM4UxptzVwMJd9cfE9k9IZM9Uw9TatfMcvI9cfCM,6846
-Dragonflyz-2.0.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-Dragonflyz-2.0.0.dist-info/top_level.txt,sha256=FDh7V_aqZtp9C6RiqpGjDB0ssZMoaSFnvLmnlmqhnss,11
-Dragonflyz-2.0.0.dist-info/RECORD,,
+Dragonflyz-2.0.3.dist-info/LICENSE,sha256=uBr-ac1MfmxnzaovoKntc1ElNSIBVYTy5ogR3PpKzT0,1070
+Dragonflyz-2.0.3.dist-info/METADATA,sha256=78rxtxZYe3gYqXgIZ4xf_-ACTi9ybJarTML1f9pnWtM,6814
+Dragonflyz-2.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+Dragonflyz-2.0.3.dist-info/top_level.txt,sha256=FDh7V_aqZtp9C6RiqpGjDB0ssZMoaSFnvLmnlmqhnss,11
+Dragonflyz-2.0.3.dist-info/RECORD,,
```

