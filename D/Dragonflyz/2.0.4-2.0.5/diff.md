# Comparing `tmp/Dragonflyz-2.0.4-py3-none-any.whl.zip` & `tmp/Dragonflyz-2.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 10739 bytes, number of entries: 10
--rw-rw-r--  2.0 unx      235 b- defN 23-Jul-20 22:53 Dragonflyz/__init__.py
+Zip file size: 11841 bytes, number of entries: 11
+-rw-rw-r--  2.0 unx      310 b- defN 23-Jul-21 15:47 Dragonflyz/__init__.py
+-rw-rw-r--  2.0 unx     2163 b- defN 23-Jul-21 15:46 Dragonflyz/disk_monitor.py
 -rw-rw-r--  2.0 unx     2370 b- defN 23-Jul-20 23:17 Dragonflyz/energy.py
 -rw-rw-r--  2.0 unx     5542 b- defN 23-Feb-08 04:36 Dragonflyz/gantt.py
 -rw-rw-r--  2.0 unx     4209 b- defN 23-Jul-20 22:14 Dragonflyz/sensor_info.py
 -rw-rw-r--  2.0 unx     3488 b- defN 23-Jul-20 22:37 Dragonflyz/system_utils.py
--rwxr-xr-x  2.0 unx     1070 b- defN 23-Jul-20 23:17 Dragonflyz-2.0.4.dist-info/LICENSE
--rw-rw-r--  2.0 unx     6814 b- defN 23-Jul-20 23:17 Dragonflyz-2.0.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-20 23:17 Dragonflyz-2.0.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Jul-20 23:17 Dragonflyz-2.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      797 b- defN 23-Jul-20 23:17 Dragonflyz-2.0.4.dist-info/RECORD
-10 files, 24628 bytes uncompressed, 9385 bytes compressed:  61.9%
+-rwxr-xr-x  2.0 unx     1070 b- defN 23-Jul-21 15:50 Dragonflyz-2.0.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     6988 b- defN 23-Jul-21 15:50 Dragonflyz-2.0.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-21 15:50 Dragonflyz-2.0.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jul-21 15:50 Dragonflyz-2.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      880 b- defN 23-Jul-21 15:50 Dragonflyz-2.0.5.dist-info/RECORD
+11 files, 27123 bytes uncompressed, 10359 bytes compressed:  61.8%
```

## zipnote {}

```diff
@@ -1,31 +1,34 @@
 Filename: Dragonflyz/__init__.py
 Comment: 
 
+Filename: Dragonflyz/disk_monitor.py
+Comment: 
+
 Filename: Dragonflyz/energy.py
 Comment: 
 
 Filename: Dragonflyz/gantt.py
 Comment: 
 
 Filename: Dragonflyz/sensor_info.py
 Comment: 
 
 Filename: Dragonflyz/system_utils.py
 Comment: 
 
-Filename: Dragonflyz-2.0.4.dist-info/LICENSE
+Filename: Dragonflyz-2.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: Dragonflyz-2.0.4.dist-info/METADATA
+Filename: Dragonflyz-2.0.5.dist-info/METADATA
 Comment: 
 
-Filename: Dragonflyz-2.0.4.dist-info/WHEEL
+Filename: Dragonflyz-2.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: Dragonflyz-2.0.4.dist-info/top_level.txt
+Filename: Dragonflyz-2.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: Dragonflyz-2.0.4.dist-info/RECORD
+Filename: Dragonflyz-2.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Dragonflyz/__init__.py

```diff
@@ -1,4 +1,5 @@
 from .gantt import sprint_gantt, project_gantt, map_job_ids, Date_Range_Generator
 from .energy import EnergyConsumed, totalEnergy 
 from .sensor_info import sensor_info, print_devices
 from .system_utils import MemoryHandler, CpuHandler
+from .disk_monitor import standardize_disk, check_disks, get_database_size
```

## Comparing `Dragonflyz-2.0.4.dist-info/LICENSE` & `Dragonflyz-2.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Dragonflyz-2.0.4.dist-info/METADATA` & `Dragonflyz-2.0.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dragonflyz
-Version: 2.0.4
+Version: 2.0.5
 Summary: Package for Code Analysis across your scripts
 Home-page: https://github.com/jacob-h-barrow/Dragonflyz
 Author: Jacob H Barrow
 Author-email: jacob.h.barrow@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -131,14 +131,20 @@
 >>> def decoratedFun2():
 >>> 	pass
 >>> # Experimental
 >>> print(totalEnergy(decoratedFun2()))
 ```
 ### Used in Profile-Aware -> Online GUI
 ``` python
+>>> from Dragonflyz import check_disks, get_database_size
+>>> from pathlib import Path
+>>> check_disks()
+>>> get_database_size(Path("DATABASE LOCATION HERE"))
+```
+``` python
 >>> from Dragonflyz import sensor_info, print_devices
 >>> print_devices(sensor_info())
 ```
 ### Used in Profile-Aware -> Online GUI
 #### CpuHandler won't work with PowerEdge devices -> commercial product coming soon
 ``` python
 >>> from Dragonflyz import MemoryHandler, CpuHandler
```

## Comparing `Dragonflyz-2.0.4.dist-info/RECORD` & `Dragonflyz-2.0.5.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-Dragonflyz/__init__.py,sha256=ZmWoOdP0bJNTgAtUClKNVAAxgQwccQeLaNvgMzuY8xk,235
+Dragonflyz/__init__.py,sha256=9vdHKuPSVeuRevR_3uF4X7UgCNWvOUQkbWuzQk3P6JA,310
+Dragonflyz/disk_monitor.py,sha256=3dYwBxxKgcoFyuhhltAlOlB3YjmnYZVDPpGAzxw0oL0,2163
 Dragonflyz/energy.py,sha256=SgriDIyOw2hM_m25E_6-ZYxVMInIuCGyjn-rp9Ba_Ac,2370
 Dragonflyz/gantt.py,sha256=XnE0Sb32bJq2cswVXF70UpwF8RM6kHAF7bvCI69Tn2c,5542
 Dragonflyz/sensor_info.py,sha256=X_Y5L28a9I5LBcebKuVUxaR4kHINdw-2M0-jdCdsRAw,4209
 Dragonflyz/system_utils.py,sha256=ouV17Mf_6KcsEOkJia7UcsaL0Fv47WSeCDNMrQ_FCFI,3488
-Dragonflyz-2.0.4.dist-info/LICENSE,sha256=uBr-ac1MfmxnzaovoKntc1ElNSIBVYTy5ogR3PpKzT0,1070
-Dragonflyz-2.0.4.dist-info/METADATA,sha256=ZBVmnUW8OuK9LXq22gFPkIgIA9JxsRk9ylzkOzZBiV0,6814
-Dragonflyz-2.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-Dragonflyz-2.0.4.dist-info/top_level.txt,sha256=FDh7V_aqZtp9C6RiqpGjDB0ssZMoaSFnvLmnlmqhnss,11
-Dragonflyz-2.0.4.dist-info/RECORD,,
+Dragonflyz-2.0.5.dist-info/LICENSE,sha256=uBr-ac1MfmxnzaovoKntc1ElNSIBVYTy5ogR3PpKzT0,1070
+Dragonflyz-2.0.5.dist-info/METADATA,sha256=TeB8pBINzQfh6NjgzgIYXNg8mnOyWx2whcl-ybTe0ww,6988
+Dragonflyz-2.0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+Dragonflyz-2.0.5.dist-info/top_level.txt,sha256=FDh7V_aqZtp9C6RiqpGjDB0ssZMoaSFnvLmnlmqhnss,11
+Dragonflyz-2.0.5.dist-info/RECORD,,
```

