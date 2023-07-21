# Comparing `tmp/ydata_core-0.4.0rc6-py2.py3-none-any.whl.zip` & `tmp/ydata_core-0.4.0rc7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 4210 bytes, number of entries: 11
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-28 17:32 ydata/core/__init__.py
--rw-r--r--  2.0 unx       59 b- defN 23-Jun-28 17:32 ydata/core/connectors/__init__.py
--rw-r--r--  2.0 unx      134 b- defN 23-Jun-28 17:32 ydata/core/connectors/write_mode.py
--rw-r--r--  2.0 unx       67 b- defN 23-Jun-28 17:32 ydata/core/enum/__init__.py
--rw-r--r--  2.0 unx      664 b- defN 23-Jun-28 17:32 ydata/core/enum/string_enum.py
--rw-r--r--  2.0 unx       70 b- defN 23-Jun-28 17:32 ydata/core/error/__init__.py
--rw-r--r--  2.0 unx     1842 b- defN 23-Jun-28 17:32 ydata/core/error/fabric_error.py
--rw-r--r--  2.0 unx     1482 b- defN 23-Jun-28 17:32 ydata_core-0.4.0rc6.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-28 17:32 ydata_core-0.4.0rc6.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-28 17:32 ydata_core-0.4.0rc6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      917 b- defN 23-Jun-28 17:32 ydata_core-0.4.0rc6.dist-info/RECORD
-11 files, 5351 bytes uncompressed, 2634 bytes compressed:  50.8%
+Zip file size: 4225 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 10:32 ydata/core/__init__.py
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-29 10:32 ydata/core/connectors/__init__.py
+-rw-r--r--  2.0 unx      134 b- defN 23-Jun-29 10:32 ydata/core/connectors/write_mode.py
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-29 10:32 ydata/core/enum/__init__.py
+-rw-r--r--  2.0 unx      722 b- defN 23-Jun-29 10:32 ydata/core/enum/string_enum.py
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-29 10:32 ydata/core/error/__init__.py
+-rw-r--r--  2.0 unx     1842 b- defN 23-Jun-29 10:32 ydata/core/error/fabric_error.py
+-rw-r--r--  2.0 unx     1482 b- defN 23-Jun-29 10:32 ydata_core-0.4.0rc7.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-29 10:32 ydata_core-0.4.0rc7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-29 10:32 ydata_core-0.4.0rc7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      917 b- defN 23-Jun-29 10:32 ydata_core-0.4.0rc7.dist-info/RECORD
+11 files, 5409 bytes uncompressed, 2649 bytes compressed:  51.0%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: ydata/core/error/__init__.py
 Comment: 
 
 Filename: ydata/core/error/fabric_error.py
 Comment: 
 
-Filename: ydata_core-0.4.0rc6.dist-info/METADATA
+Filename: ydata_core-0.4.0rc7.dist-info/METADATA
 Comment: 
 
-Filename: ydata_core-0.4.0rc6.dist-info/WHEEL
+Filename: ydata_core-0.4.0rc7.dist-info/WHEEL
 Comment: 
 
-Filename: ydata_core-0.4.0rc6.dist-info/top_level.txt
+Filename: ydata_core-0.4.0rc7.dist-info/top_level.txt
 Comment: 
 
-Filename: ydata_core-0.4.0rc6.dist-info/RECORD
+Filename: ydata_core-0.4.0rc7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ydata/core/enum/string_enum.py

```diff
@@ -22,9 +22,12 @@
   @classmethod
   def _key_from_str(cls, value: str):
     if value in cls._member_map_.keys():
       return cls._member_map_[value]
 
     return None
 
+  def __hash__(self) -> int:
+    return hash(self.value)
+
   def __eq__(self, other: object) -> bool:
     return self.value == other.value
```

## Comparing `ydata_core-0.4.0rc6.dist-info/METADATA` & `ydata_core-0.4.0rc7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydata-core
-Version: 0.4.0rc6
+Version: 0.4.0rc7
 Summary: Core functionality for all python packages at YData
 Home-page: https://github.com/ydataai/python-core
 Author: YData
 Author-email: developers@ydata.ai
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

## Comparing `ydata_core-0.4.0rc6.dist-info/RECORD` & `ydata_core-0.4.0rc7.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ydata/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ydata/core/connectors/__init__.py,sha256=rsifccFDjMFl71_MOEzejh-4lOLbgHLdgtrHd8l6efw,59
 ydata/core/connectors/write_mode.py,sha256=uUZMVD6yx3GJLR7_dLJyIOHrVZO1WaSjpulZA23aN-M,134
 ydata/core/enum/__init__.py,sha256=R5LgZ-ZFiZJGW19f8ejDodDf6EZjSJ0a_LXxIyhkOdo,67
-ydata/core/enum/string_enum.py,sha256=l11UUEBKXvQYBdnuvExMHEU-PnIrIpAIoRNBb6rZpmo,664
+ydata/core/enum/string_enum.py,sha256=gwSPIzkPJoKXNEe8hAnVUGReVmLIakWkcXD4Dqg6rxY,722
 ydata/core/error/__init__.py,sha256=tA7nd8DVnbFyTexySXzNXDhmloFjPKzjJ_Wmz2IBl-Y,70
 ydata/core/error/fabric_error.py,sha256=c2AF03-suBI1G5-tWfwuu-BMn_Zk_QF2w3QvLA_qZHo,1842
-ydata_core-0.4.0rc6.dist-info/METADATA,sha256=aI31ZHdWh3GVjiJMzPWzY1Qtf5QbuUakFuJS8s82EYE,1482
-ydata_core-0.4.0rc6.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-ydata_core-0.4.0rc6.dist-info/top_level.txt,sha256=s4ySCHuzMHwZ8NeXGj2CkDdJaGLv0YzfNsi3JW3V8gQ,6
-ydata_core-0.4.0rc6.dist-info/RECORD,,
+ydata_core-0.4.0rc7.dist-info/METADATA,sha256=Sq0NHT83yswKCWzcN8dylwUENYQ_86Pq54LuVjrP1wU,1482
+ydata_core-0.4.0rc7.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+ydata_core-0.4.0rc7.dist-info/top_level.txt,sha256=s4ySCHuzMHwZ8NeXGj2CkDdJaGLv0YzfNsi3JW3V8gQ,6
+ydata_core-0.4.0rc7.dist-info/RECORD,,
```

