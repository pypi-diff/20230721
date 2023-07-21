# Comparing `tmp/docblock-0.0.4.tar.gz` & `tmp/docblock-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docblock-0.0.4.tar", max compression
+gzip compressed data, was "docblock-0.0.5.tar", max compression
```

## Comparing `docblock-0.0.4.tar` & `docblock-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2023-07-21 14:40:00.429071 docblock-0.0.4/LICENSE.md
--rw-r--r--   0        0        0     3041 2023-07-21 14:40:00.429071 docblock-0.0.4/README.md
--rw-r--r--   0        0        0       78 2023-07-21 14:40:00.429071 docblock-0.0.4/docblock/__init__.py
--rw-r--r--   0        0        0     1279 2023-07-21 14:40:00.429071 docblock-0.0.4/docblock/grammar.py
--rw-r--r--   0        0        0     2110 2023-07-21 14:40:00.429071 docblock-0.0.4/docblock/parse.py
--rw-r--r--   0        0        0      779 2023-07-21 14:40:00.429071 docblock-0.0.4/docblock/show_versions.py
--rw-r--r--   0        0        0      831 2023-07-21 14:40:00.429071 docblock-0.0.4/docblock/utils.py
--rw-r--r--   0        0        0     1825 2023-07-21 14:40:00.429071 docblock-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3963 1970-01-01 00:00:00.000000 docblock-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-21 14:47:01.224651 docblock-0.0.5/LICENSE.md
+-rw-r--r--   0        0        0     3041 2023-07-21 14:47:01.224651 docblock-0.0.5/README.md
+-rw-r--r--   0        0        0       78 2023-07-21 14:47:01.224651 docblock-0.0.5/docblock/__init__.py
+-rw-r--r--   0        0        0     1299 2023-07-21 14:47:01.224651 docblock-0.0.5/docblock/grammar.py
+-rw-r--r--   0        0        0     2110 2023-07-21 14:47:01.224651 docblock-0.0.5/docblock/parse.py
+-rw-r--r--   0        0        0      779 2023-07-21 14:47:01.224651 docblock-0.0.5/docblock/show_versions.py
+-rw-r--r--   0        0        0      831 2023-07-21 14:47:01.224651 docblock-0.0.5/docblock/utils.py
+-rw-r--r--   0        0        0     1825 2023-07-21 14:47:01.224651 docblock-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3963 1970-01-01 00:00:00.000000 docblock-0.0.5/PKG-INFO
```

### Comparing `docblock-0.0.4/LICENSE.md` & `docblock-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `docblock-0.0.4/README.md` & `docblock-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `docblock-0.0.4/docblock/grammar.py` & `docblock-0.0.5/docblock/grammar.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 # but seem to work well.
 NAMESPACE = pp.Keyword("namespace").suppress() + QUALIFIED_ID
 CLASS = (pp.Keyword("struct") | pp.Keyword("class")).suppress() + QUALIFIED_ID
 
 # Exclude braces: we only want the delcarations, not any implementations.
 # Assumes those are separated. Some special care is needed to match
 # "operator X" overloads.
-OPERATOR = "operator" + (pp.Word("<>!=&|*/+-~^", min=1, max=3) | "()" | "[]")
+_OP = pp.Word("<>!=&|*/+-~^", min=1, max=3) | "()" | "[]"
+OPERATOR = pp.Combine("operator" + _OP)
 FUNC_NAME = OPERATOR | QUALIFIED_ID
 FUNC = FUNC_NAME + (LPAR + ... + RPAR + ID[...] + CLOSE_STMT).suppress()
 
 # Line comment and documentation blocks.
 LINE_COMMENT = pp.dbl_slash_comment
 DOCBLOCK = pp.c_style_comment
```

### Comparing `docblock-0.0.4/docblock/parse.py` & `docblock-0.0.5/docblock/parse.py`

 * *Files identical despite different names*

### Comparing `docblock-0.0.4/docblock/show_versions.py` & `docblock-0.0.5/docblock/show_versions.py`

 * *Files identical despite different names*

### Comparing `docblock-0.0.4/docblock/utils.py` & `docblock-0.0.5/docblock/utils.py`

 * *Files identical despite different names*

### Comparing `docblock-0.0.4/pyproject.toml` & `docblock-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docblock"
-version = "0.0.4"
+version = "0.0.5"
 description = "Reads and parses documentation from header files in pure Python."
 authors = ["Niels Wouda <nielswouda@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/N-Wouda/docblock"
 include = [
     "LICENSE.md",
```

### Comparing `docblock-0.0.4/PKG-INFO` & `docblock-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docblock
-Version: 0.0.4
+Version: 0.0.5
 Summary: Reads and parses documentation from header files in pure Python.
 Home-page: https://github.com/N-Wouda/docblock
 License: MIT
 Author: Niels Wouda
 Author-email: nielswouda@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

