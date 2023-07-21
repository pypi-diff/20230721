# Comparing `tmp/dynamicadaptor-0.4.4.tar.gz` & `tmp/dynamicadaptor-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamicadaptor-0.4.4.tar", max compression
+gzip compressed data, was "dynamicadaptor-0.4.5.tar", max compression
```

## Comparing `dynamicadaptor-0.4.4.tar` & `dynamicadaptor-0.4.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    18431 2023-07-20 14:02:02.782185 dynamicadaptor-0.4.4/LICENSE
--rw-r--r--   0        0        0    10010 2023-07-20 14:02:02.782185 dynamicadaptor-0.4.4/README.md
--rw-r--r--   0        0        0     2136 2023-07-20 14:02:02.782185 dynamicadaptor-0.4.4/dynamicadaptor/AddonCard.py
--rw-r--r--   0        0        0      926 2023-07-20 14:02:02.782185 dynamicadaptor-0.4.4/dynamicadaptor/Content.py
--rw-r--r--   0        0        0    20217 2023-07-20 14:02:02.782185 dynamicadaptor-0.4.4/dynamicadaptor/DynamicConversion.py
--rw-r--r--   0        0        0      575 2023-07-20 14:02:02.782185 dynamicadaptor-0.4.4/dynamicadaptor/Header.py
--rw-r--r--   0        0        0     3849 2023-07-20 14:02:02.782185 dynamicadaptor-0.4.4/dynamicadaptor/Majors.py
--rw-r--r--   0        0        0      410 2023-07-20 14:02:02.782185 dynamicadaptor-0.4.4/dynamicadaptor/Message.py
--rw-r--r--   0        0        0      323 2023-07-20 14:02:02.782185 dynamicadaptor-0.4.4/dynamicadaptor/Repost.py
--rw-r--r--   0        0        0       10 2023-07-20 14:02:02.782185 dynamicadaptor-0.4.4/dynamicadaptor/__init__.py
--rw-r--r--   0        0        0      500 2023-07-20 14:02:02.782185 dynamicadaptor-0.4.4/pyproject.toml
--rw-r--r--   0        0        0    10528 1970-01-01 00:00:00.000000 dynamicadaptor-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    18431 2023-07-21 05:22:05.646198 dynamicadaptor-0.4.5/LICENSE
+-rw-r--r--   0        0        0    10010 2023-07-21 05:22:05.646198 dynamicadaptor-0.4.5/README.md
+-rw-r--r--   0        0        0     2136 2023-07-21 05:22:05.646198 dynamicadaptor-0.4.5/dynamicadaptor/AddonCard.py
+-rw-r--r--   0        0        0      926 2023-07-21 05:22:05.646198 dynamicadaptor-0.4.5/dynamicadaptor/Content.py
+-rw-r--r--   0        0        0    20217 2023-07-21 05:22:05.646198 dynamicadaptor-0.4.5/dynamicadaptor/DynamicConversion.py
+-rw-r--r--   0        0        0      575 2023-07-21 05:22:05.646198 dynamicadaptor-0.4.5/dynamicadaptor/Header.py
+-rw-r--r--   0        0        0     3882 2023-07-21 05:22:05.646198 dynamicadaptor-0.4.5/dynamicadaptor/Majors.py
+-rw-r--r--   0        0        0      410 2023-07-21 05:22:05.646198 dynamicadaptor-0.4.5/dynamicadaptor/Message.py
+-rw-r--r--   0        0        0      323 2023-07-21 05:22:05.646198 dynamicadaptor-0.4.5/dynamicadaptor/Repost.py
+-rw-r--r--   0        0        0       10 2023-07-21 05:22:05.646198 dynamicadaptor-0.4.5/dynamicadaptor/__init__.py
+-rw-r--r--   0        0        0      500 2023-07-21 05:22:05.646198 dynamicadaptor-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0    10528 1970-01-01 00:00:00.000000 dynamicadaptor-0.4.5/PKG-INFO
```

### Comparing `dynamicadaptor-0.4.4/LICENSE` & `dynamicadaptor-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.4/README.md` & `dynamicadaptor-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.4/dynamicadaptor/AddonCard.py` & `dynamicadaptor-0.4.5/dynamicadaptor/AddonCard.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.4/dynamicadaptor/Content.py` & `dynamicadaptor-0.4.5/dynamicadaptor/Content.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.4/dynamicadaptor/DynamicConversion.py` & `dynamicadaptor-0.4.5/dynamicadaptor/DynamicConversion.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.4/dynamicadaptor/Header.py` & `dynamicadaptor-0.4.5/dynamicadaptor/Header.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.4/dynamicadaptor/Majors.py` & `dynamicadaptor-0.4.5/dynamicadaptor/Majors.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from pydantic import BaseModel, Json
 
 
 # 图片
 class DrawItem(BaseModel):
     height: int
     width: int
-    url: str
+    src: Optional[str]
+    url:Optional[str]
 
 
 class Draw(BaseModel):
     items: List[DrawItem]
 
 
 # 视频
```

### Comparing `dynamicadaptor-0.4.4/PKG-INFO` & `dynamicadaptor-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicadaptor
-Version: 0.4.4
+Version: 0.4.5
 Summary: 
 Author: DMC
 Author-email: lzxder@outlook.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

