# Comparing `tmp/autospark_kit-0.0.1.tar.gz` & `tmp/autospark_kit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autospark_kit-0.0.1.tar", max compression
+gzip compressed data, was "autospark_kit-0.0.2.tar", max compression
```

## Comparing `autospark_kit-0.0.1.tar` & `autospark_kit-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      758 2023-07-14 07:37:05.591277 autospark_kit-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 07:28:40.843740 autospark_kit-0.0.1/src/autospark_kit/__init__.py
--rw-r--r--   0        0        0        0 2023-07-14 07:28:40.843578 autospark_kit-0.0.1/src/autospark_kit/tools/__init__.py
--rw-r--r--   0        0        0     7485 2023-07-14 07:28:40.843683 autospark_kit-0.0.1/src/autospark_kit/tools/base_tool.py
--rw-r--r--   0        0        0      567 1970-01-01 00:00:00.000000 autospark_kit-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      758 2023-07-21 02:38:13.630331 autospark_kit-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 07:28:40.843740 autospark_kit-0.0.2/src/autospark_kit/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 07:28:40.843578 autospark_kit-0.0.2/src/autospark_kit/tools/__init__.py
+-rw-r--r--   0        0        0     6715 2023-07-21 02:37:56.030825 autospark_kit-0.0.2/src/autospark_kit/tools/base_tool.py
+-rw-r--r--   0        0        0     7485 2023-07-14 07:28:40.843683 autospark_kit-0.0.2/src/autospark_kit/tools/base_tool2.py
+-rw-r--r--   0        0        0      567 1970-01-01 00:00:00.000000 autospark_kit-0.0.2/PKG-INFO
```

### Comparing `autospark_kit-0.0.1/pyproject.toml` & `autospark_kit-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autospark_kit"
-version = "0.0.1"
+version = "0.0.2"
 description = "a iflytek autospark dev kit library ..."
 authors = ["ybyang <ybyang7@iflytek.com>", "jianjiang <jianjiang@iflytek.com>", ]
 license = "Apache License 2"
 packages = [
     { include = "autospark_kit", from = "src" }
 ]
```

### Comparing `autospark_kit-0.0.1/src/autospark_kit/tools/base_tool.py` & `autospark_kit-0.0.2/src/autospark_kit/tools/base_tool2.py`

 * *Files identical despite different names*

### Comparing `autospark_kit-0.0.1/PKG-INFO` & `autospark_kit-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autospark-kit
-Version: 0.0.1
+Version: 0.0.2
 Summary: a iflytek autospark dev kit library ...
 License: Apache License 2
 Author: ybyang
 Author-email: ybyang7@iflytek.com
 Requires-Python: >3.7
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

