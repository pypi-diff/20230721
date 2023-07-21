# Comparing `tmp/docblock-0.0.3.tar.gz` & `tmp/docblock-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docblock-0.0.3.tar", max compression
+gzip compressed data, was "docblock-0.0.4.tar", max compression
```

## Comparing `docblock-0.0.3.tar` & `docblock-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2023-07-20 17:26:25.195425 docblock-0.0.3/LICENSE.md
--rw-r--r--   0        0        0     3041 2023-07-20 17:26:25.195425 docblock-0.0.3/README.md
--rw-r--r--   0        0        0       78 2023-07-20 17:26:25.199426 docblock-0.0.3/docblock/__init__.py
--rw-r--r--   0        0        0     1110 2023-07-20 17:26:25.199426 docblock-0.0.3/docblock/grammar.py
--rw-r--r--   0        0        0     2110 2023-07-20 17:26:25.199426 docblock-0.0.3/docblock/parse.py
--rw-r--r--   0        0        0      779 2023-07-20 17:26:25.199426 docblock-0.0.3/docblock/show_versions.py
--rw-r--r--   0        0        0      832 2023-07-20 17:26:25.199426 docblock-0.0.3/docblock/utils.py
--rw-r--r--   0        0        0     1825 2023-07-20 17:26:25.199426 docblock-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3963 1970-01-01 00:00:00.000000 docblock-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-21 14:40:00.429071 docblock-0.0.4/LICENSE.md
+-rw-r--r--   0        0        0     3041 2023-07-21 14:40:00.429071 docblock-0.0.4/README.md
+-rw-r--r--   0        0        0       78 2023-07-21 14:40:00.429071 docblock-0.0.4/docblock/__init__.py
+-rw-r--r--   0        0        0     1279 2023-07-21 14:40:00.429071 docblock-0.0.4/docblock/grammar.py
+-rw-r--r--   0        0        0     2110 2023-07-21 14:40:00.429071 docblock-0.0.4/docblock/parse.py
+-rw-r--r--   0        0        0      779 2023-07-21 14:40:00.429071 docblock-0.0.4/docblock/show_versions.py
+-rw-r--r--   0        0        0      831 2023-07-21 14:40:00.429071 docblock-0.0.4/docblock/utils.py
+-rw-r--r--   0        0        0     1825 2023-07-21 14:40:00.429071 docblock-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3963 1970-01-01 00:00:00.000000 docblock-0.0.4/PKG-INFO
```

### Comparing `docblock-0.0.3/LICENSE.md` & `docblock-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `docblock-0.0.3/README.md` & `docblock-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `docblock-0.0.3/docblock/grammar.py` & `docblock-0.0.4/docblock/grammar.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import pyparsing as pp
 
 # Names in C++ can either be standalone, or fully qualified parts of a
 # namespace. In the latter case the name consists of multiple parts separated
 # by "::".
 ID = pp.Word(pp.identbodychars)
-QUALIFIED_ID = pp.Combine(pp.OneOrMore(pp.Optional(ID + "::") + ID))
+QUALIFIED_ID = pp.Combine(pp.OneOrMore(pp.Optional("::") + ID))
 
 LPAR, RPAR = pp.Literal("("), pp.Literal(")")
 LBRACE, RBRACE = pp.Literal("{"), pp.Literal("}")
 CLOSE_STMT = pp.Literal(";")
 
 # Namespace, class (struct) and function definitions. These are fairly crude
 # but seem to work well.
 NAMESPACE = pp.Keyword("namespace").suppress() + QUALIFIED_ID
 CLASS = (pp.Keyword("struct") | pp.Keyword("class")).suppress() + QUALIFIED_ID
 
 # Exclude braces: we only want the delcarations, not any implementations.
-# Assumes those are separated.
-FUNC = QUALIFIED_ID + (LPAR + ... + RPAR + ID[...] + CLOSE_STMT).suppress()
+# Assumes those are separated. Some special care is needed to match
+# "operator X" overloads.
+OPERATOR = "operator" + (pp.Word("<>!=&|*/+-~^", min=1, max=3) | "()" | "[]")
+FUNC_NAME = OPERATOR | QUALIFIED_ID
+FUNC = FUNC_NAME + (LPAR + ... + RPAR + ID[...] + CLOSE_STMT).suppress()
 
 # Line comment and documentation blocks.
 LINE_COMMENT = pp.dbl_slash_comment
 DOCBLOCK = pp.c_style_comment
 
 # Complete syntax we match on, ignoring (end-of-)line comments.
 _ITEMS = NAMESPACE | CLASS | FUNC | LBRACE | RBRACE | DOCBLOCK
```

### Comparing `docblock-0.0.3/docblock/parse.py` & `docblock-0.0.4/docblock/parse.py`

 * *Files identical despite different names*

### Comparing `docblock-0.0.3/docblock/show_versions.py` & `docblock-0.0.4/docblock/show_versions.py`

 * *Files identical despite different names*

### Comparing `docblock-0.0.3/docblock/utils.py` & `docblock-0.0.4/docblock/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 def strip_doc(doc: str) -> str:
     """
     Strips a C-style documentation block of the opening and closing tags, and
     any continuation in multiline blocks. For example,
     ```
     /**
-     *  Test
+     * Test
      */
     ```
     is stripped to ``Test``.
 
     Parameters
     ----------
     doc
```

### Comparing `docblock-0.0.3/pyproject.toml` & `docblock-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docblock"
-version = "0.0.3"
+version = "0.0.4"
 description = "Reads and parses documentation from header files in pure Python."
 authors = ["Niels Wouda <nielswouda@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/N-Wouda/docblock"
 include = [
     "LICENSE.md",
```

### Comparing `docblock-0.0.3/PKG-INFO` & `docblock-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docblock
-Version: 0.0.3
+Version: 0.0.4
 Summary: Reads and parses documentation from header files in pure Python.
 Home-page: https://github.com/N-Wouda/docblock
 License: MIT
 Author: Niels Wouda
 Author-email: nielswouda@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

