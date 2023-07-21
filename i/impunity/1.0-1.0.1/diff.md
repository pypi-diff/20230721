# Comparing `tmp/impunity-1.0.tar.gz` & `tmp/impunity-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impunity-1.0.tar", max compression
+gzip compressed data, was "impunity-1.0.1.tar", max compression
```

## Comparing `impunity-1.0.tar` & `impunity-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1086 2023-03-17 15:25:08.762240 impunity-1.0/license.txt
--rw-r--r--   0        0        0     1361 2023-07-20 08:46:19.598546 impunity-1.0/pyproject.toml
--rw-r--r--   0        0        0       54 2022-12-15 08:10:37.693666 impunity-1.0/src/impunity/__init__.py
--rw-r--r--   0        0        0      520 2023-04-26 09:32:15.372322 impunity-1.0/src/impunity/exception.py
--rw-r--r--   0        0        0        0 2023-03-17 15:25:08.762240 impunity-1.0/src/impunity/py.typed
--rw-r--r--   0        0        0      859 2023-06-20 08:36:00.376797 impunity-1.0/src/impunity/quantityNode.py
--rw-r--r--   0        0        0    38089 2023-07-12 12:44:39.459946 impunity-1.0/src/impunity/visitor.py
--rw-r--r--   0        0        0     9530 2023-07-12 08:34:02.847488 impunity-1.0/src/impunity/wrapper.py
--rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 impunity-1.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-03-17 15:25:08.762240 impunity-1.0.1/license.txt
+-rw-r--r--   0        0        0     1363 2023-07-21 10:47:02.546507 impunity-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       54 2022-12-15 08:10:37.693666 impunity-1.0.1/src/impunity/__init__.py
+-rw-r--r--   0        0        0      520 2023-04-26 09:32:15.372322 impunity-1.0.1/src/impunity/exception.py
+-rw-r--r--   0        0        0        0 2023-03-17 15:25:08.762240 impunity-1.0.1/src/impunity/py.typed
+-rw-r--r--   0        0        0      859 2023-06-20 08:36:00.376797 impunity-1.0.1/src/impunity/quantityNode.py
+-rw-r--r--   0        0        0    38267 2023-07-21 10:57:01.761738 impunity-1.0.1/src/impunity/visitor.py
+-rw-r--r--   0        0        0     9530 2023-07-12 08:34:02.847488 impunity-1.0.1/src/impunity/wrapper.py
+-rw-r--r--   0        0        0      662 1970-01-01 00:00:00.000000 impunity-1.0.1/PKG-INFO
```

### Comparing `impunity-1.0/license.txt` & `impunity-1.0.1/license.txt`

 * *Files identical despite different names*

### Comparing `impunity-1.0/pyproject.toml` & `impunity-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "impunity"
-version = "1.0"
+version = "1.0.1"
 description = "Static checking for consistency of physical units"
 authors = [
   "Antoine Chevrot <antoine.chevrot@gmail.com>",
   "Xavier Olive <git@xoolive.org>"
 ]
 license = "MIT"
 include = [
```

### Comparing `impunity-1.0/src/impunity/exception.py` & `impunity-1.0.1/src/impunity/exception.py`

 * *Files identical despite different names*

### Comparing `impunity-1.0/src/impunity/quantityNode.py` & `impunity-1.0.1/src/impunity/quantityNode.py`

 * *Files identical despite different names*

### Comparing `impunity-1.0/src/impunity/visitor.py` & `impunity-1.0.1/src/impunity/visitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -818,16 +818,18 @@
         Args:
             node (ast.AnnAssign): input node
 
         """
 
         value = self.get_node_unit(node.value)
 
-        if value is None:
-            pass
+        if value.node is None:
+            expected = cast(annotation_node, node.annotation)
+            expected_unit = get_annotation_unit(expected)
+            self.vars[node.target.id] = expected_unit  # type: ignore
 
         if value.node != node.value:
             new_node = ast.AnnAssign(
                 target=node.target,
                 annotation=node.annotation,
                 value=value.node,
                 simple=node.simple,
```

### Comparing `impunity-1.0/src/impunity/wrapper.py` & `impunity-1.0.1/src/impunity/wrapper.py`

 * *Files identical despite different names*

### Comparing `impunity-1.0/PKG-INFO` & `impunity-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impunity
-Version: 1.0
+Version: 1.0.1
 Summary: Static checking for consistency of physical units
 License: MIT
 Author: Antoine Chevrot
 Author-email: antoine.chevrot@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

