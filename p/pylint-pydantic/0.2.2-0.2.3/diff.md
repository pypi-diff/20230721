# Comparing `tmp/pylint_pydantic-0.2.2-py3-none-any.whl.zip` & `tmp/pylint_pydantic-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 15126 bytes, number of entries: 6
--rw-r--r--  2.0 unx     2469 b- defN 23-Jul-17 09:52 pylint_pydantic/__init__.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jul-17 09:53 pylint_pydantic-0.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1931 b- defN 23-Jul-17 09:53 pylint_pydantic-0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 09:53 pylint_pydantic-0.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jul-17 09:53 pylint_pydantic-0.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      511 b- defN 23-Jul-17 09:53 pylint_pydantic-0.2.2.dist-info/RECORD
-6 files, 40168 bytes uncompressed, 14196 bytes compressed:  64.7%
+Zip file size: 15118 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     2500 b- defN 23-Jul-21 02:24 pylint_pydantic/__init__.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jul-21 02:24 pylint_pydantic-0.2.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1931 b- defN 23-Jul-21 02:24 pylint_pydantic-0.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 02:24 pylint_pydantic-0.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-21 02:24 pylint_pydantic-0.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      511 b- defN 23-Jul-21 02:24 pylint_pydantic-0.2.3.dist-info/RECORD
+6 files, 40199 bytes uncompressed, 14188 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pylint_pydantic/__init__.py
 Comment: 
 
-Filename: pylint_pydantic-0.2.2.dist-info/LICENSE
+Filename: pylint_pydantic-0.2.3.dist-info/LICENSE
 Comment: 
 
-Filename: pylint_pydantic-0.2.2.dist-info/METADATA
+Filename: pylint_pydantic-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: pylint_pydantic-0.2.2.dist-info/WHEEL
+Filename: pylint_pydantic-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: pylint_pydantic-0.2.2.dist-info/top_level.txt
+Filename: pylint_pydantic-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pylint_pydantic-0.2.2.dist-info/RECORD
+Filename: pylint_pydantic-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pylint_pydantic/__init__.py

```diff
@@ -26,24 +26,28 @@
     if isinstance(decorator, Name):
         return decorator.name
 
     # @pydantic.validator
     if isinstance(decorator, Attribute):
         return decorator.attrname
 
-    raise ValueError("Invalid decorator name")
+    return None
 
 
 def _is_classmethod_decorator(node: FunctionDef):
 
     if not node.decorators:
         return False
 
     for decorator in node.decorators.get_children():
         decorator_name = _get_decorator_name(decorator)
+
+        if decorator_name is None:
+            return False
+
         if decorator_name in CLASSMETHOD_VALIDATOR_NAMES:
             return True
 
         if decorator_name in MODE_VALIDATOR_NAMES:
             return _mode_validator_is_classmethod(decorator)
 
     return False
```

## Comparing `pylint_pydantic-0.2.2.dist-info/LICENSE` & `pylint_pydantic-0.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pylint_pydantic-0.2.2.dist-info/METADATA` & `pylint_pydantic-0.2.3.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylint-pydantic
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Pylint plugin to help Pylint understand the Pydantic
 Home-page: https://github.com/fcfangcc/pylint-pydantic
 Author: fcfangcc
 Author-email: swjfc22@163.com
 License: GPLv3
 Keywords: pylint,pydantic
 Platform: UNKNOWN
```

