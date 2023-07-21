# Comparing `tmp/pydoclint-0.1.1.tar.gz` & `tmp/pydoclint-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoclint-0.1.1.tar", last modified: Wed Jul 19 02:27:17 2023, max compression
+gzip compressed data, was "pydoclint-0.1.2.tar", last modified: Fri Jul 21 02:42:21 2023, max compression
```

## Comparing `pydoclint-0.1.1.tar` & `pydoclint-0.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:27:17.775635 pydoclint-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-19 02:27:07.000000 pydoclint-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13276 2023-07-19 02:27:17.775635 pydoclint-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-07-19 02:27:07.000000 pydoclint-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:27:17.767635 pydoclint-0.1.1/pydoclint/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/flake8_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/parse_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:27:17.775635 pydoclint-0.1.1/pydoclint/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/astTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/internal_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/method_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/return_anno.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/return_arg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/return_yield_raise.py
--rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/unparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/violation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/walk.py
--rw-r--r--   0 runner    (1001) docker     (123)    23893 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:27:17.771635 pydoclint-0.1.1/pydoclint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13276 2023-07-19 02:27:17.000000 pydoclint-0.1.1/pydoclint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-19 02:27:17.000000 pydoclint-0.1.1/pydoclint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 02:27:17.000000 pydoclint-0.1.1/pydoclint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-19 02:27:17.000000 pydoclint-0.1.1/pydoclint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-19 02:27:17.000000 pydoclint-0.1.1/pydoclint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 02:27:17.000000 pydoclint-0.1.1/pydoclint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-19 02:27:17.775635 pydoclint-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-19 02:27:07.000000 pydoclint-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:27:17.775635 pydoclint-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-19 02:27:07.000000 pydoclint-0.1.1/tests/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    40155 2023-07-19 02:27:07.000000 pydoclint-0.1.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-19 02:27:07.000000 pydoclint-0.1.1/tests/test_parse_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:42:21.789863 pydoclint-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-21 02:42:09.000000 pydoclint-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14506 2023-07-21 02:42:21.789863 pydoclint-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14059 2023-07-21 02:42:09.000000 pydoclint-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:42:21.781863 pydoclint-0.1.2/pydoclint/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7396 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/flake8_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/parse_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:42:21.789863 pydoclint-0.1.2/pydoclint/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/astTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/internal_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/method_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/return_anno.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/return_arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/return_yield_raise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/unparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/violation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24031 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:42:21.785863 pydoclint-0.1.2/pydoclint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14506 2023-07-21 02:42:21.000000 pydoclint-0.1.2/pydoclint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-21 02:42:21.000000 pydoclint-0.1.2/pydoclint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 02:42:21.000000 pydoclint-0.1.2/pydoclint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-21 02:42:21.000000 pydoclint-0.1.2/pydoclint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-21 02:42:21.000000 pydoclint-0.1.2/pydoclint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 02:42:21.000000 pydoclint-0.1.2/pydoclint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-21 02:42:21.789863 pydoclint-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-21 02:42:09.000000 pydoclint-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:42:21.789863 pydoclint-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-21 02:42:09.000000 pydoclint-0.1.2/tests/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40645 2023-07-21 02:42:09.000000 pydoclint-0.1.2/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-21 02:42:09.000000 pydoclint-0.1.2/tests/test_parse_config.py
```

### Comparing `pydoclint-0.1.1/LICENSE` & `pydoclint-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.1/PKG-INFO` & `pydoclint-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoclint
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python docstring linter that checks arguments, returns, yields, and raises sections
 Home-page: https://github.com/jsh9/pydoclint
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
@@ -156,14 +156,20 @@
 | Code     | Explanation                                                                                                                                         |
 | -------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `DOC101` | Docstring contains fewer arguments than in function signature                                                                                       |
 | `DOC102` | Docstring contains more arguments than in function signature                                                                                        |
 | `DOC103` | Docstring arguments are different from function arguments. (Or could be other formatting issues: https://github.com/jsh9/pydoclint#notes-on-doc103) |
 | `DOC104` | Arguments are the same in the docstring and the function signature, but are in a different order.                                                   |
 | `DOC105` | Argument names match, but type hints do not match                                                                                                   |
+| `DOC106` | The option `--arg-type-hints-in-signature` is `True` but there are no argument type hints in the signature                                          |
+| `DOC107` | The option `--arg-type-hints-in-signature` is `True` but not all args in the signature have type hints                                              |
+| `DOC108` | The option `--arg-type-hints-in-signature` is `False` but there are argument type hints in the signature                                            |
+| `DOC109` | The option `--arg-type-hints-in-docstring` is `True` but there are no type hints in the docstring arg list                                          |
+| `DOC110` | The option `--arg-type-hints-in-docstring` is `True` but not all args in the docstring arg list have type hints                                     |
+| `DOC111` | The option `--arg-type-hints-in-docstring` is `False` but there are type hints in the docstring arg list                                            |
 
 #### Notes on `DOC103`:
 
 Other potential causes to `DOC103` include:
 
 - Numpy docstring style requires this style: `arg1 : int` (a space between
   `arg1` and `:`) but people sometimes write `arg1: int`. This will trigger
@@ -256,34 +262,36 @@
 
 or
 
 ```
 flake8 --style=google <FILE_OR_FOLDER>
 ```
 
-### 4.4. `--type-hints-in-docstring` and `--type-hints-in-signature`
+### 4.4. `--arg-type-hints-in-docstring` and `--arg-type-hints-in-signature`
 
-- `--type-hints-in-docstring`
+- `--arg-type-hints-in-docstring`
   - Shortform: `-thd`
   - Default: `True`
   - Meaning:
     - If `True`, there need to be type hints in the argument list of a
       docstring
     - If `False`, there cannot be any type hints in the argument list of a
       docstring
-- `--type-hints-in-signature`
+- `--arg-type-hints-in-signature`
   - Shortform: `-ths`
   - Default: `True`
   - Meaning:
-    - If `True`, there need to be type hints in the function/method signature
-    - If `False`, there cannot be any type hints in the function/method
+    - If `True`, there need to be argument type hints in the function/method
       signature
+    - If `False`, there cannot be any argument type hints in the
+      function/method signature
 
-Note: if users choose `True` for both options, the type hints in the signature
-and in the docstring need to match, otherwise there will be a style violation.
+Note: if users choose `True` for both options, the argument type hints in the
+signature and in the docstring need to match, otherwise there will be a style
+violation.
 
 ### 4.5. `--check-arg-order` (shortform: `-ao`, default: `True`)
 
 If `True`, the input argument order in the docstring needs to match that in the
 function signature.
 
 To turn this option on/off, do this:
@@ -328,7 +336,12 @@
 under `__init__()` rather than in the class docstring.
 
 ### 4.9. `--require-return-section-when-returning-none` (shortform: `-rrs`, default: `False`)
 
 If `False`, a "return" section is not necessary in the docstring if the
 function implicitly returns `None` (for example, doesn't have a return
 statement, or has `-> None` as the return annotation).
+
+### 4.10. `--check-return-types` (shortform: `-crt`, default: `True`)
+
+If True, check that the type(s) in the docstring return section and the return
+annotation in the function signature are consistent
```

### Comparing `pydoclint-0.1.1/README.md` & `pydoclint-0.1.2/pydoclint.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: pydoclint
+Version: 0.1.2
+Summary: A Python docstring linter that checks arguments, returns, yields, and raises sections
+Home-page: https://github.com/jsh9/pydoclint
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pydoclint
 
 A Python docstring linter to check whether a docstring's sections (arguments,
 returns, raises, ...) match the function signature or function implementation.
 
 It runs really fast. In fact, it is at least ~1,475 times faster than
 [darglint](https://github.com/terrencepreilly/darglint) (or its maintained fork
@@ -143,14 +156,20 @@
 | Code     | Explanation                                                                                                                                         |
 | -------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `DOC101` | Docstring contains fewer arguments than in function signature                                                                                       |
 | `DOC102` | Docstring contains more arguments than in function signature                                                                                        |
 | `DOC103` | Docstring arguments are different from function arguments. (Or could be other formatting issues: https://github.com/jsh9/pydoclint#notes-on-doc103) |
 | `DOC104` | Arguments are the same in the docstring and the function signature, but are in a different order.                                                   |
 | `DOC105` | Argument names match, but type hints do not match                                                                                                   |
+| `DOC106` | The option `--arg-type-hints-in-signature` is `True` but there are no argument type hints in the signature                                          |
+| `DOC107` | The option `--arg-type-hints-in-signature` is `True` but not all args in the signature have type hints                                              |
+| `DOC108` | The option `--arg-type-hints-in-signature` is `False` but there are argument type hints in the signature                                            |
+| `DOC109` | The option `--arg-type-hints-in-docstring` is `True` but there are no type hints in the docstring arg list                                          |
+| `DOC110` | The option `--arg-type-hints-in-docstring` is `True` but not all args in the docstring arg list have type hints                                     |
+| `DOC111` | The option `--arg-type-hints-in-docstring` is `False` but there are type hints in the docstring arg list                                            |
 
 #### Notes on `DOC103`:
 
 Other potential causes to `DOC103` include:
 
 - Numpy docstring style requires this style: `arg1 : int` (a space between
   `arg1` and `:`) but people sometimes write `arg1: int`. This will trigger
@@ -243,34 +262,36 @@
 
 or
 
 ```
 flake8 --style=google <FILE_OR_FOLDER>
 ```
 
-### 4.4. `--type-hints-in-docstring` and `--type-hints-in-signature`
+### 4.4. `--arg-type-hints-in-docstring` and `--arg-type-hints-in-signature`
 
-- `--type-hints-in-docstring`
+- `--arg-type-hints-in-docstring`
   - Shortform: `-thd`
   - Default: `True`
   - Meaning:
     - If `True`, there need to be type hints in the argument list of a
       docstring
     - If `False`, there cannot be any type hints in the argument list of a
       docstring
-- `--type-hints-in-signature`
+- `--arg-type-hints-in-signature`
   - Shortform: `-ths`
   - Default: `True`
   - Meaning:
-    - If `True`, there need to be type hints in the function/method signature
-    - If `False`, there cannot be any type hints in the function/method
+    - If `True`, there need to be argument type hints in the function/method
       signature
+    - If `False`, there cannot be any argument type hints in the
+      function/method signature
 
-Note: if users choose `True` for both options, the type hints in the signature
-and in the docstring need to match, otherwise there will be a style violation.
+Note: if users choose `True` for both options, the argument type hints in the
+signature and in the docstring need to match, otherwise there will be a style
+violation.
 
 ### 4.5. `--check-arg-order` (shortform: `-ao`, default: `True`)
 
 If `True`, the input argument order in the docstring needs to match that in the
 function signature.
 
 To turn this option on/off, do this:
@@ -315,7 +336,12 @@
 under `__init__()` rather than in the class docstring.
 
 ### 4.9. `--require-return-section-when-returning-none` (shortform: `-rrs`, default: `False`)
 
 If `False`, a "return" section is not necessary in the docstring if the
 function implicitly returns `None` (for example, doesn't have a return
 statement, or has `-> None` as the return annotation).
+
+### 4.10. `--check-return-types` (shortform: `-crt`, default: `True`)
+
+If True, check that the type(s) in the docstring return section and the return
+annotation in the function signature are consistent
```

### Comparing `pydoclint-0.1.1/pydoclint/flake8_entry.py` & `pydoclint-0.1.2/pydoclint/flake8_entry.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,22 +23,38 @@
             parse_from_config=True,
             help='Which style of docstring is your code base using',
         )
         parser.add_option(
             '-ths',
             '--type-hints-in-signature',
             action='store',
+            default='None',
+            parse_from_config=True,
+            help='(Deprecated) Please use --arg-type-hints-in-signature instead',
+        )
+        parser.add_option(
+            '-aths',
+            '--arg-type-hints-in-signature',
+            action='store',
             default='True',
             parse_from_config=True,
-            help='Whether to require type hints in function signatures',
+            help='Whether to require argument type hints in function signatures',
         )
         parser.add_option(
             '-thd',
             '--type-hints-in-docstring',
             action='store',
+            default='None',
+            parse_from_config=True,
+            help='(Deprecated) Please use --arg-type-hints-in-docstring instead',
+        )
+        parser.add_option(
+            '-athd',
+            '--arg-type-hints-in-docstring',
+            action='store',
             default='True',
             parse_from_config=True,
             help='Whether to require type hints in the argument list in docstrings',
         )
         parser.add_option(
             '-ao',
             '--check-arg-order',
@@ -98,34 +114,48 @@
             ),
         )
 
     @classmethod
     def parse_options(cls, options):  # noqa: D102
         cls.type_hints_in_signature = options.type_hints_in_signature
         cls.type_hints_in_docstring = options.type_hints_in_docstring
+        cls.arg_type_hints_in_signature = options.arg_type_hints_in_signature
+        cls.arg_type_hints_in_docstring = options.arg_type_hints_in_docstring
         cls.check_arg_order = options.check_arg_order
         cls.skip_checking_short_docstrings = (
             options.skip_checking_short_docstrings
         )
         cls.skip_checking_raises = options.skip_checking_raises
         cls.allow_init_docstring = options.allow_init_docstring
         cls.require_return_section_when_returning_none = (
             options.require_return_section_when_returning_none
         )
         cls.style = options.style
 
     def run(self) -> Generator[Tuple[int, int, str, Any], None, None]:
         """Run the linter and yield the violation information"""
-        typeHintsInSignature = self._bool(
-            '--type-hints-in-signature',
-            self.type_hints_in_signature,
-        )
-        typeHintsInDocstring = self._bool(
-            '--type-hints-in-docstring',
-            self.type_hints_in_docstring,
+        if self.type_hints_in_docstring != 'None':  # user supplies this option
+            raise ValueError(
+                'The option `--type-hints-in-docstring` has been renamed;'
+                ' please use `--arg-type-hints-in-docstring` instead'
+            )
+
+        if self.type_hints_in_signature != 'None':  # user supplies this option
+            raise ValueError(
+                'The option `--type-hints-in-signature` has been renamed;'
+                ' please use `--arg-type-hints-in-signature` instead'
+            )
+
+        argTypeHintsInSignature = self._bool(
+            '--arg-type-hints-in-signature',
+            self.arg_type_hints_in_signature,
+        )
+        argTypeHintsInDocstring = self._bool(
+            '--arg-type-hints-in-docstring',
+            self.arg_type_hints_in_docstring,
         )
         checkArgOrder = self._bool('--check-arg-order', self.check_arg_order)
         skipCheckingShortDocstrings = self._bool(
             '--skip-checking-short-docstrings',
             self.skip_checking_short_docstrings,
         )
         skipCheckingRaises = self._bool(
@@ -143,16 +173,16 @@
 
         if self.style not in {'numpy', 'google', 'sphinx'}:
             raise ValueError(
                 'Invalid value for "--style": must be "numpy", "google", or "sphinx"'
             )
 
         v = Visitor(
-            typeHintsInSignature=typeHintsInSignature,
-            typeHintsInDocstring=typeHintsInDocstring,
+            argTypeHintsInSignature=argTypeHintsInSignature,
+            argTypeHintsInDocstring=argTypeHintsInDocstring,
             checkArgOrder=checkArgOrder,
             skipCheckingShortDocstrings=skipCheckingShortDocstrings,
             skipCheckingRaises=skipCheckingRaises,
             allowInitDocstring=allowInitDocstring,
             requireReturnSectionWhenReturningNone=requireReturnSectionWhenReturningNone,
             style=self.style,
         )
```

### Comparing `pydoclint-0.1.1/pydoclint/main.py` & `pydoclint-0.1.2/pydoclint/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -68,22 +68,36 @@
     default='numpy',
     callback=validateStyleValue,
     help='',
 )
 @click.option(
     '-ths',
     '--type-hints-in-signature',
+    show_default=True,
+    default='None',
+    help='(Deprecated) Please use --arg-type-hints-in-signature instead',
+)
+@click.option(
+    '-aths',
+    '--arg-type-hints-in-signature',
     type=bool,
     show_default=True,
     default=True,
-    help='Whether to require type hints in function signatures',
+    help='Whether to require argument type hints in function signatures',
 )
 @click.option(
     '-thd',
     '--type-hints-in-docstring',
+    show_default=True,
+    default='None',
+    help='(Deprecated) Please use --arg-type-hints-in-docstring instead',
+)
+@click.option(
+    '-athd',
+    '--arg-type-hints-in-docstring',
     type=bool,
     show_default=True,
     default=True,
     help='Whether to require type hints in the argument list in docstrings',
 )
 @click.option(
     '-ao',
@@ -175,27 +189,57 @@
 def main(  # noqa: C901
         ctx: click.Context,
         quiet: bool,
         exclude: str,
         style: str,
         src: Optional[str],
         paths: Tuple[str, ...],
-        type_hints_in_signature: bool,
-        type_hints_in_docstring: bool,
+        type_hints_in_signature: str,
+        type_hints_in_docstring: str,
+        arg_type_hints_in_signature: bool,
+        arg_type_hints_in_docstring: bool,
         check_arg_order: bool,
         skip_checking_short_docstrings: bool,
         skip_checking_raises: bool,
         allow_init_docstring: bool,
         check_return_types: bool,
         require_return_section_when_returning_none: bool,
         config: Optional[str],  # don't remove it b/c it's required by `click`
 ) -> None:
     """Command-line entry point of pydoclint"""
     ctx.ensure_object(dict)
 
+    if type_hints_in_docstring != 'None':  # it means users supply this option
+        click.echo(
+            click.style(
+                ''.join([
+                    'The option `--type-hints-in-docstring` has been renamed;',
+                    ' please use `--arg-type-hints-in-docstring` instead',
+                ]),
+                fg='red',
+                bold=True,
+            ),
+            err=echoAsError,
+        )
+        ctx.exit(1)
+
+    if type_hints_in_signature != 'None':  # it means users supply this option
+        click.echo(
+            click.style(
+                ''.join([
+                    'The option `--type-hints-in-signature` has been renamed;',
+                    ' please use `--arg-type-hints-in-signature` instead',
+                ]),
+                fg='red',
+                bold=True,
+            ),
+            err=echoAsError,
+        )
+        ctx.exit(1)
+
     if paths and src is not None:
         click.echo(
             main.get_usage(ctx)
             + "\n\n'paths' and 'src' cannot be passed simultaneously.",
             err=echoAsError,
         )
         ctx.exit(1)
@@ -208,16 +252,16 @@
         ctx.exit(1)
 
     violationsInAllFiles: Dict[str, List[Violation]] = _checkPaths(
         quiet=quiet,
         exclude=exclude,
         style=style,
         paths=paths,
-        typeHintsInSignature=type_hints_in_signature,
-        typeHintsInDocstring=type_hints_in_docstring,
+        argTypeHintsInSignature=arg_type_hints_in_signature,
+        argTypeHintsInDocstring=arg_type_hints_in_docstring,
         checkArgOrder=check_arg_order,
         skipCheckingShortDocstrings=skip_checking_short_docstrings,
         skipCheckingRaises=skip_checking_raises,
         allowInitDocstring=allow_init_docstring,
         checkReturnTypes=check_return_types,
         requireReturnSectionWhenReturningNone=require_return_section_when_returning_none,
     )
@@ -264,16 +308,16 @@
 
         ctx.exit(0)
 
 
 def _checkPaths(
         paths: Tuple[str, ...],
         style: str = 'numpy',
-        typeHintsInSignature: bool = True,
-        typeHintsInDocstring: bool = True,
+        argTypeHintsInSignature: bool = True,
+        argTypeHintsInDocstring: bool = True,
         checkArgOrder: bool = True,
         skipCheckingShortDocstrings: bool = True,
         skipCheckingRaises: bool = False,
         allowInitDocstring: bool = False,
         checkReturnTypes: bool = True,
         requireReturnSectionWhenReturningNone: bool = False,
         quiet: bool = False,
@@ -306,16 +350,16 @@
             click.echo(
                 click.style(filename, fg='cyan', bold=True), err=echoAsError
             )
 
         violationsInThisFile: List[Violation] = _checkFile(
             filename,
             style=style,
-            typeHintsInSignature=typeHintsInSignature,
-            typeHintsInDocstring=typeHintsInDocstring,
+            argTypeHintsInSignature=argTypeHintsInSignature,
+            argTypeHintsInDocstring=argTypeHintsInDocstring,
             checkArgOrder=checkArgOrder,
             skipCheckingShortDocstrings=skipCheckingShortDocstrings,
             skipCheckingRaises=skipCheckingRaises,
             allowInitDocstring=allowInitDocstring,
             checkReturnTypes=checkReturnTypes,
             requireReturnSectionWhenReturningNone=requireReturnSectionWhenReturningNone,
         )
@@ -323,31 +367,31 @@
 
     return allViolations
 
 
 def _checkFile(
         filename: Path,
         style: str = 'numpy',
-        typeHintsInSignature: bool = True,
-        typeHintsInDocstring: bool = True,
+        argTypeHintsInSignature: bool = True,
+        argTypeHintsInDocstring: bool = True,
         checkArgOrder: bool = True,
         skipCheckingShortDocstrings: bool = True,
         skipCheckingRaises: bool = False,
         allowInitDocstring: bool = False,
         checkReturnTypes: bool = True,
         requireReturnSectionWhenReturningNone: bool = False,
 ) -> List[Violation]:
     with open(filename, encoding='utf8') as fp:
         src: str = ''.join(fp.readlines())
 
     tree: ast.Module = ast.parse(src)
     visitor = Visitor(
         style=style,
-        typeHintsInSignature=typeHintsInSignature,
-        typeHintsInDocstring=typeHintsInDocstring,
+        argTypeHintsInSignature=argTypeHintsInSignature,
+        argTypeHintsInDocstring=argTypeHintsInDocstring,
         checkArgOrder=checkArgOrder,
         skipCheckingShortDocstrings=skipCheckingShortDocstrings,
         skipCheckingRaises=skipCheckingRaises,
         allowInitDocstring=allowInitDocstring,
         checkReturnTypes=checkReturnTypes,
         requireReturnSectionWhenReturningNone=requireReturnSectionWhenReturningNone,
     )
```

### Comparing `pydoclint-0.1.1/pydoclint/parse_config.py` & `pydoclint-0.1.2/pydoclint/parse_config.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.1/pydoclint/utils/annotation.py` & `pydoclint-0.1.2/pydoclint/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.1/pydoclint/utils/arg.py` & `pydoclint-0.1.2/pydoclint/utils/arg.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.1/pydoclint/utils/astTypes.py` & `pydoclint-0.1.2/pydoclint/utils/astTypes.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.1/pydoclint/utils/doc.py` & `pydoclint-0.1.2/pydoclint/utils/doc.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.1/pydoclint/utils/generic.py` & `pydoclint-0.1.2/pydoclint/utils/generic.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.1/pydoclint/utils/return_anno.py` & `pydoclint-0.1.2/pydoclint/utils/return_anno.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.1/pydoclint/utils/return_yield_raise.py` & `pydoclint-0.1.2/pydoclint/utils/return_yield_raise.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.1/pydoclint/utils/unparser.py` & `pydoclint-0.1.2/pydoclint/utils/unparser.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.1/pydoclint/utils/violation.py` & `pydoclint-0.1.2/pydoclint/utils/violation.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,20 +11,20 @@
     102: 'Docstring contains more arguments than in function signature.',
     103: (  # noqa: PAR001
         'Docstring arguments are different from function arguments.'
         ' (Or could be other formatting issues: https://github.com/jsh9/pydoclint#notes-on-doc103 ).'
     ),
     104: 'Arguments are the same in the docstring and the function signature, but are in a different order.',
     105: 'Argument names match, but type hints do not match',
-    106: 'The option `--type-hints-in-signature` is `True` but there are no type hints in the signature',
-    107: 'The option `--type-hints-in-signature` is `True` but not all args in the signature have type hints',
-    108: 'The option `--type-hints-in-signature` is `False` but there are type hints in the signature',
-    109: 'The option `--type-hints-in-docstring` is `True` but there are no type hints in the docstring arg list',
-    110: 'The option `--type-hints-in-docstring` is `True` but not all args in the docstring arg list have type hints',
-    111: 'The option `--type-hints-in-docstring` is `False` but there are type hints in the docstring arg list',
+    106: 'The option `--arg-type-hints-in-signature` is `True` but there are no argument type hints in the signature',
+    107: 'The option `--arg-type-hints-in-signature` is `True` but not all args in the signature have type hints',
+    108: 'The option `--arg-type-hints-in-signature` is `False` but there are argument type hints in the signature',
+    109: 'The option `--arg-type-hints-in-docstring` is `True` but there are no type hints in the docstring arg list',
+    110: 'The option `--arg-type-hints-in-docstring` is `True` but not all args in the docstring arg list have type hints',
+    111: 'The option `--arg-type-hints-in-docstring` is `False` but there are type hints in the docstring arg list',
 
     201: 'does not have a return section in docstring',
     202: 'has a return section in docstring, but there are no return statements or annotations',
     203: 'return type(s) in docstring not consistent with the return annotation.',
 
     301: '__init__() should not have a docstring; please combine it with the docstring of the class',
     302: 'The class docstring does not need a "Returns" section, because __init__() cannot return anything',
```

### Comparing `pydoclint-0.1.1/pydoclint/utils/walk.py` & `pydoclint-0.1.2/pydoclint/utils/walk.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.1/pydoclint/visitor.py` & `pydoclint-0.1.2/pydoclint/visitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,26 +32,26 @@
 
 class Visitor(ast.NodeVisitor):
     """A class to recursively visit all the nodes in a parsed module"""
 
     def __init__(
             self,
             style: str = 'numpy',
-            typeHintsInSignature: bool = True,
-            typeHintsInDocstring: bool = True,
+            argTypeHintsInSignature: bool = True,
+            argTypeHintsInDocstring: bool = True,
             checkArgOrder: bool = True,
             skipCheckingShortDocstrings: bool = True,
             skipCheckingRaises: bool = False,
             allowInitDocstring: bool = False,
             checkReturnTypes: bool = True,
             requireReturnSectionWhenReturningNone: bool = False,
     ) -> None:
         self.style: str = style
-        self.typeHintsInSignature: bool = typeHintsInSignature
-        self.typeHintsInDocstring: bool = typeHintsInDocstring
+        self.argTypeHintsInSignature: bool = argTypeHintsInSignature
+        self.argTypeHintsInDocstring: bool = argTypeHintsInDocstring
         self.checkArgOrder: bool = checkArgOrder
         self.skipCheckingShortDocstrings: bool = skipCheckingShortDocstrings
         self.skipCheckingRaises: bool = skipCheckingRaises
         self.allowInitDocstring: bool = allowInitDocstring
         self.checkReturnTypes: bool = checkReturnTypes
         self.requireReturnSectionWhenReturningNone: bool = (
             requireReturnSectionWhenReturningNone
@@ -342,30 +342,33 @@
         violations: List[Violation] = []
         if docArgs.length < funcArgs.length:
             violations.append(v101)
 
         if docArgs.length > funcArgs.length:
             violations.append(v102)
 
-        if self.typeHintsInSignature and funcArgs.noTypeHints():
+        if self.argTypeHintsInSignature and funcArgs.noTypeHints():
             violations.append(v106)
 
-        if self.typeHintsInSignature and not funcArgs.hasTypeHintInAllArgs():
+        if (
+            self.argTypeHintsInSignature
+            and not funcArgs.hasTypeHintInAllArgs()
+        ):
             violations.append(v107)
 
-        if not self.typeHintsInSignature and funcArgs.hasTypeHintInAnyArg():
+        if not self.argTypeHintsInSignature and funcArgs.hasTypeHintInAnyArg():
             violations.append(v108)
 
-        if self.typeHintsInDocstring and docArgs.noTypeHints():
+        if self.argTypeHintsInDocstring and docArgs.noTypeHints():
             violations.append(v109)
 
-        if self.typeHintsInDocstring and not docArgs.hasTypeHintInAllArgs():
+        if self.argTypeHintsInDocstring and not docArgs.hasTypeHintInAllArgs():
             violations.append(v110)
 
-        if not self.typeHintsInDocstring and docArgs.hasTypeHintInAnyArg():
+        if not self.argTypeHintsInDocstring and docArgs.hasTypeHintInAnyArg():
             violations.append(v111)
 
         if not docArgs.equals(
             funcArgs,
             checkTypeHint=True,
             orderMatters=self.checkArgOrder,
         ):
@@ -376,15 +379,18 @@
             ):
                 violations.append(v104)
             elif docArgs.equals(
                 funcArgs,
                 checkTypeHint=False,
                 orderMatters=self.checkArgOrder,
             ):
-                if self.typeHintsInSignature and self.typeHintsInDocstring:
+                if (
+                    self.argTypeHintsInSignature
+                    and self.argTypeHintsInDocstring
+                ):
                     violations.append(v105)
             elif docArgs.equals(
                 funcArgs,
                 checkTypeHint=False,
                 orderMatters=False,
             ):
                 violations.append(v104)
```

### Comparing `pydoclint-0.1.1/pydoclint.egg-info/PKG-INFO` & `pydoclint-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: pydoclint
-Version: 0.1.1
-Summary: A Python docstring linter that checks arguments, returns, yields, and raises sections
-Home-page: https://github.com/jsh9/pydoclint
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pydoclint
 
 A Python docstring linter to check whether a docstring's sections (arguments,
 returns, raises, ...) match the function signature or function implementation.
 
 It runs really fast. In fact, it is at least ~1,475 times faster than
 [darglint](https://github.com/terrencepreilly/darglint) (or its maintained fork
@@ -156,14 +143,20 @@
 | Code     | Explanation                                                                                                                                         |
 | -------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `DOC101` | Docstring contains fewer arguments than in function signature                                                                                       |
 | `DOC102` | Docstring contains more arguments than in function signature                                                                                        |
 | `DOC103` | Docstring arguments are different from function arguments. (Or could be other formatting issues: https://github.com/jsh9/pydoclint#notes-on-doc103) |
 | `DOC104` | Arguments are the same in the docstring and the function signature, but are in a different order.                                                   |
 | `DOC105` | Argument names match, but type hints do not match                                                                                                   |
+| `DOC106` | The option `--arg-type-hints-in-signature` is `True` but there are no argument type hints in the signature                                          |
+| `DOC107` | The option `--arg-type-hints-in-signature` is `True` but not all args in the signature have type hints                                              |
+| `DOC108` | The option `--arg-type-hints-in-signature` is `False` but there are argument type hints in the signature                                            |
+| `DOC109` | The option `--arg-type-hints-in-docstring` is `True` but there are no type hints in the docstring arg list                                          |
+| `DOC110` | The option `--arg-type-hints-in-docstring` is `True` but not all args in the docstring arg list have type hints                                     |
+| `DOC111` | The option `--arg-type-hints-in-docstring` is `False` but there are type hints in the docstring arg list                                            |
 
 #### Notes on `DOC103`:
 
 Other potential causes to `DOC103` include:
 
 - Numpy docstring style requires this style: `arg1 : int` (a space between
   `arg1` and `:`) but people sometimes write `arg1: int`. This will trigger
@@ -256,34 +249,36 @@
 
 or
 
 ```
 flake8 --style=google <FILE_OR_FOLDER>
 ```
 
-### 4.4. `--type-hints-in-docstring` and `--type-hints-in-signature`
+### 4.4. `--arg-type-hints-in-docstring` and `--arg-type-hints-in-signature`
 
-- `--type-hints-in-docstring`
+- `--arg-type-hints-in-docstring`
   - Shortform: `-thd`
   - Default: `True`
   - Meaning:
     - If `True`, there need to be type hints in the argument list of a
       docstring
     - If `False`, there cannot be any type hints in the argument list of a
       docstring
-- `--type-hints-in-signature`
+- `--arg-type-hints-in-signature`
   - Shortform: `-ths`
   - Default: `True`
   - Meaning:
-    - If `True`, there need to be type hints in the function/method signature
-    - If `False`, there cannot be any type hints in the function/method
+    - If `True`, there need to be argument type hints in the function/method
       signature
+    - If `False`, there cannot be any argument type hints in the
+      function/method signature
 
-Note: if users choose `True` for both options, the type hints in the signature
-and in the docstring need to match, otherwise there will be a style violation.
+Note: if users choose `True` for both options, the argument type hints in the
+signature and in the docstring need to match, otherwise there will be a style
+violation.
 
 ### 4.5. `--check-arg-order` (shortform: `-ao`, default: `True`)
 
 If `True`, the input argument order in the docstring needs to match that in the
 function signature.
 
 To turn this option on/off, do this:
@@ -328,7 +323,12 @@
 under `__init__()` rather than in the class docstring.
 
 ### 4.9. `--require-return-section-when-returning-none` (shortform: `-rrs`, default: `False`)
 
 If `False`, a "return" section is not necessary in the docstring if the
 function implicitly returns `None` (for example, doesn't have a return
 statement, or has `-> None` as the return annotation).
+
+### 4.10. `--check-return-types` (shortform: `-crt`, default: `True`)
+
+If True, check that the type(s) in the docstring return section and the return
+annotation in the function signature are consistent
```

### Comparing `pydoclint-0.1.1/pydoclint.egg-info/SOURCES.txt` & `pydoclint-0.1.2/pydoclint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.1/setup.cfg` & `pydoclint-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pydoclint
-version = 0.1.1
+version = 0.1.2
 description = A Python docstring linter that checks arguments, returns, yields, and raises sections
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jsh9/pydoclint
 license = MIT
 license_file = LICENSE
 classifiers =
```

### Comparing `pydoclint-0.1.1/tests/test_generic.py` & `pydoclint-0.1.2/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.1/tests/test_main.py` & `pydoclint-0.1.2/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 THIS_DIR = Path(__file__).parent
 DATA_DIR = THIS_DIR / 'data'
 
 
 expectedViolations_True = [
     'DOC101: Method `MyClass.func1_3`: Docstring contains fewer arguments than in '
     'function signature. ',
-    'DOC109: Method `MyClass.func1_3`: The option `--type-hints-in-docstring` is `True` '
+    'DOC109: Method `MyClass.func1_3`: The option `--arg-type-hints-in-docstring` is `True` '
     'but there are no type hints in the docstring arg list ',
     'DOC103: Method `MyClass.func1_3`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
     'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in '
     'the docstring: [arg1: str, arg2: list[int]].',
     'DOC102: Method `MyClass.func1_6`: Docstring contains more arguments than in '
     'function signature. ',
-    'DOC106: Method `MyClass.func1_6`: The option `--type-hints-in-signature` is `True` '
-    'but there are no type hints in the signature ',
+    'DOC106: Method `MyClass.func1_6`: The option `--arg-type-hints-in-signature` is `True` '
+    'but there are no argument type hints in the signature ',
     'DOC103: Method `MyClass.func1_6`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
     'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the docstring but not in the '
     'function signature: [arg1: int].',
     'DOC101: Method `MyClass.func2`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func2`: Docstring arguments are different from '
@@ -44,35 +44,35 @@
     'the function signature, but are in a different order. ',
     'DOC105: Method `MyClass.func5`: Argument names match, but type hints do not match ',
     'DOC104: Method `MyClass.func6`: Arguments are the same in the docstring and '
     'the function signature, but are in a different order. ',
     'DOC105: Method `MyClass.func6`: Argument names match, but type hints do not match ',
     'DOC101: Function `func72`: Docstring contains fewer arguments than in '
     'function signature. ',
-    'DOC109: Function `func72`: The option `--type-hints-in-docstring` is `True` '
+    'DOC109: Function `func72`: The option `--arg-type-hints-in-docstring` is `True` '
     'but there are no type hints in the docstring arg list ',
     'DOC103: Function `func72`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
     'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
     'docstring: [arg3: list, arg4: tuple, arg5: dict].',
 ]
 
 expectedViolations_False = [
     'DOC101: Method `MyClass.func1_3`: Docstring contains fewer arguments than in '
     'function signature. ',
-    'DOC109: Method `MyClass.func1_3`: The option `--type-hints-in-docstring` is `True` '
+    'DOC109: Method `MyClass.func1_3`: The option `--arg-type-hints-in-docstring` is `True` '
     'but there are no type hints in the docstring arg list ',
     'DOC103: Method `MyClass.func1_3`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
     'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in '
     'the docstring: [arg1: str, arg2: list[int]].',
     'DOC102: Method `MyClass.func1_6`: Docstring contains more arguments than in '
     'function signature. ',
-    'DOC106: Method `MyClass.func1_6`: The option `--type-hints-in-signature` is `True` '
-    'but there are no type hints in the signature ',
+    'DOC106: Method `MyClass.func1_6`: The option `--arg-type-hints-in-signature` is `True` '
+    'but there are no argument type hints in the signature ',
     'DOC103: Method `MyClass.func1_6`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
     'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the docstring but not in the '
     'function signature: [arg1: int].',
     'DOC101: Method `MyClass.func2`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func2`: Docstring arguments are different from '
@@ -87,15 +87,15 @@
     'function signature: [arg3: Optional[Union[float, int, str]]].',
     'DOC105: Method `MyClass.func5`: Argument names match, but type hints do not '
     'match ',
     'DOC105: Method `MyClass.func6`: Argument names match, but type hints do not '
     'match ',
     'DOC101: Function `func72`: Docstring contains fewer arguments than in '
     'function signature. ',
-    'DOC109: Function `func72`: The option `--type-hints-in-docstring` is `True` '
+    'DOC109: Function `func72`: The option `--arg-type-hints-in-docstring` is `True` '
     'but there are no type hints in the docstring arg list ',
     'DOC103: Function `func72`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
     'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
     'docstring: [arg3: list, arg4: tuple, arg5: dict].',
 ]
 
@@ -252,63 +252,63 @@
             'Method `MyClass.', 'Function `'
         )
 
 
 expected_skipCheckingShortDocstrings_True = [
     'DOC101: Function `func3`: Docstring contains fewer arguments than in '
     'function signature. ',
-    'DOC106: Function `func3`: The option `--type-hints-in-signature` is `True` '
-    'but there are no type hints in the signature ',
-    'DOC107: Function `func3`: The option `--type-hints-in-signature` is `True` '
+    'DOC106: Function `func3`: The option `--arg-type-hints-in-signature` is `True` '
+    'but there are no argument type hints in the signature ',
+    'DOC107: Function `func3`: The option `--arg-type-hints-in-signature` is `True` '
     'but not all args in the signature have type hints ',
     'DOC103: Function `func3`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
     'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
     'docstring: [arg1: , arg2: , arg3: ]. Arguments in the docstring but not in '
     'the function signature: [var1: int, var2: str].',
 ]
 
 expected_skipCheckingShortDocstrings_False = [
     'DOC101: Function `func1`: Docstring contains fewer arguments than in '
     'function signature. ',
-    'DOC106: Function `func1`: The option `--type-hints-in-signature` is `True` '
-    'but there are no type hints in the signature ',
-    'DOC107: Function `func1`: The option `--type-hints-in-signature` is `True` '
+    'DOC106: Function `func1`: The option `--arg-type-hints-in-signature` is `True` '
+    'but there are no argument type hints in the signature ',
+    'DOC107: Function `func1`: The option `--arg-type-hints-in-signature` is `True` '
     'but not all args in the signature have type hints ',
-    'DOC109: Function `func1`: The option `--type-hints-in-docstring` is `True` '
+    'DOC109: Function `func1`: The option `--arg-type-hints-in-docstring` is `True` '
     'but there are no type hints in the docstring arg list ',
     'DOC103: Function `func1`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
     'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the '
     'function signature but not in the docstring: [arg1: , arg2: , arg3: ].',
     'DOC201: Function `func1` does not have a return section in docstring ',
     'DOC203: Function `func1` return type(s) in docstring not consistent with the '
     'return annotation. Return annotation has 1 type(s); docstring return section '
     'has 0 type(s).',
     'DOC101: Function `func2`: Docstring contains fewer arguments than in '
     'function signature. ',
-    'DOC106: Function `func2`: The option `--type-hints-in-signature` is `True` '
-    'but there are no type hints in the signature ',
-    'DOC107: Function `func2`: The option `--type-hints-in-signature` is `True` '
+    'DOC106: Function `func2`: The option `--arg-type-hints-in-signature` is `True` '
+    'but there are no argument type hints in the signature ',
+    'DOC107: Function `func2`: The option `--arg-type-hints-in-signature` is `True` '
     'but not all args in the signature have type hints ',
-    'DOC109: Function `func2`: The option `--type-hints-in-docstring` is `True` '
+    'DOC109: Function `func2`: The option `--arg-type-hints-in-docstring` is `True` '
     'but there are no type hints in the docstring arg list ',
     'DOC103: Function `func2`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
     'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the '
     'function signature but not in the docstring: [arg1: , arg2: , arg3: ].',
     'DOC201: Function `func2` does not have a return section in docstring ',
     'DOC203: Function `func2` return type(s) in docstring not consistent with the '
     'return annotation. Return annotation has 1 type(s); docstring return section '
     'has 0 type(s).',
     'DOC101: Function `func3`: Docstring contains fewer arguments than in '
     'function signature. ',
-    'DOC106: Function `func3`: The option `--type-hints-in-signature` is `True` '
-    'but there are no type hints in the signature ',
-    'DOC107: Function `func3`: The option `--type-hints-in-signature` is `True` '
+    'DOC106: Function `func3`: The option `--arg-type-hints-in-signature` is `True` '
+    'but there are no argument type hints in the signature ',
+    'DOC107: Function `func3`: The option `--arg-type-hints-in-signature` is `True` '
     'but not all args in the signature have type hints ',
     'DOC103: Function `func3`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
     'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the '
     'function signature but not in the docstring: [arg1: , arg2: , arg3: ]. '
     'Arguments in the docstring but not in the function signature: [var1: int, '
     'var2: str].',
@@ -455,16 +455,16 @@
         [False, True],
     ),
 )
 def testRaises(style: str, skipRaisesCheck: bool) -> None:
     violations = _checkFile(
         filename=DATA_DIR / f'{style}/raises/cases.py',
         skipCheckingRaises=skipRaisesCheck,
-        typeHintsInSignature=False,
-        typeHintsInDocstring=False,
+        argTypeHintsInSignature=False,
+        argTypeHintsInDocstring=False,
         checkReturnTypes=False,
         style=style,
     )
     expected0 = [
         'DOC501: Method `B.func1` has "raise" statements, but the docstring does not '
         'have a "Raises" section ',
         'DOC502: Method `B.func5` has a "Raises" section in the docstring, but there '
@@ -484,22 +484,22 @@
 @pytest.mark.parametrize('style', ['numpy', 'google', 'sphinx'])
 def testStarsInArgumentList(style: str) -> None:
     violations = _checkFile(
         filename=DATA_DIR / f'{style}/star_args/cases.py',
         style=style,
     )
     expected = [
-        'DOC110: Function `func2`: The option `--type-hints-in-docstring` is `True` '
+        'DOC110: Function `func2`: The option `--arg-type-hints-in-docstring` is `True` '
         'but not all args in the docstring arg list have type hints ',
         'DOC103: Function `func2`: Docstring arguments are different from function '
         'arguments. (Or could be other formatting issues: '
         'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
         'docstring: [**kwargs: ]. Arguments in the docstring but not in the function '
         'signature: [kwargs: ].',
-        'DOC110: Function `func4`: The option `--type-hints-in-docstring` is `True` '
+        'DOC110: Function `func4`: The option `--arg-type-hints-in-docstring` is `True` '
         'but not all args in the docstring arg list have type hints ',
         'DOC103: Function `func4`: Docstring arguments are different from function '
         'arguments. (Or could be other formatting issues: '
         'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
         'docstring: [*args: ]. Arguments in the docstring but not in the function '
         'signature: [args: ].',
         'DOC101: Function `func6`: Docstring contains fewer arguments than in '
@@ -519,16 +519,16 @@
     assert list(map(str, violations)) == expected
 
 
 @pytest.mark.parametrize('style', ['numpy', 'google', 'sphinx'])
 def testStarsInArgumentList2(style: str) -> None:
     violations = _checkFile(
         filename=DATA_DIR / f'{style}/star_args/cases2.py',
-        typeHintsInSignature=True,
-        typeHintsInDocstring=False,
+        argTypeHintsInSignature=True,
+        argTypeHintsInDocstring=False,
         allowInitDocstring=True,
         style=style,
     )
     expected = []
     assert list(map(str, violations)) == expected
 
 
@@ -552,16 +552,16 @@
     expected = []  # not sure how to craft docstrings with parsing errors yet
     assert list(map(str, violations)) == expected
 
 
 def testParsingErrors_numpy() -> None:
     violations = _checkFile(
         filename=DATA_DIR / 'numpy/parsing_errors/cases.py',
-        typeHintsInDocstring=False,
-        typeHintsInSignature=False,
+        argTypeHintsInDocstring=False,
+        argTypeHintsInSignature=False,
         style='numpy',
     )
     expected = [
         'DOC001: Function/method `__init__`: Potential formatting errors in '
         'docstring. Error message: The section Parameters appears twice in  Some '
         'class  Parameters ----------     arg1     arg2  Parameters ----------     '
         'arg3     arg4'
@@ -652,141 +652,143 @@
             'section in docstring ',
         ]
 
     assert list(map(str, violations)) == expected
 
 
 @pytest.mark.parametrize(
-    'style, typeHintsInDocstring, typeHintsInSignature',
+    'style, argTypeHintsInDocstring, argTypeHintsInSignature',
     itertools.product(
         ['numpy', 'google', 'sphinx'],
         [False, True],
         [False, True],
     ),
 )
 def testTypeHintChecking(
         style: str,
-        typeHintsInDocstring: bool,
-        typeHintsInSignature: bool,
+        argTypeHintsInDocstring: bool,
+        argTypeHintsInSignature: bool,
 ) -> None:
     violations = _checkFile(
         filename=DATA_DIR / f'{style}/type_hints/cases.py',
         style=style,
-        typeHintsInDocstring=typeHintsInDocstring,
-        typeHintsInSignature=typeHintsInSignature,
+        argTypeHintsInDocstring=argTypeHintsInDocstring,
+        argTypeHintsInSignature=argTypeHintsInSignature,
     )
 
     expected_lookup = {
         (False, False): [
-            'DOC108: Method `MyClass.func2`: The option `--type-hints-in-signature` is '
-            '`False` but there are type hints in the signature ',
-            'DOC111: Method `MyClass.func3`: The option `--type-hints-in-docstring` is '
+            'DOC108: Method `MyClass.func2`: The option `--arg-type-hints-in-signature` is '
+            '`False` but there are argument type hints in the signature ',
+            'DOC111: Method `MyClass.func3`: The option `--arg-type-hints-in-docstring` is '
             '`False` but there are type hints in the docstring arg list ',
-            'DOC108: Method `MyClass.func4`: The option `--type-hints-in-signature` is '
-            '`False` but there are type hints in the signature ',
-            'DOC111: Method `MyClass.func4`: The option `--type-hints-in-docstring` is '
+            'DOC108: Method `MyClass.func4`: The option `--arg-type-hints-in-signature` is '
+            '`False` but there are argument type hints in the signature ',
+            'DOC111: Method `MyClass.func4`: The option `--arg-type-hints-in-docstring` is '
             '`False` but there are type hints in the docstring arg list ',
-            'DOC108: Method `MyClass.func5`: The option `--type-hints-in-signature` is '
-            '`False` but there are type hints in the signature ',
-            'DOC111: Method `MyClass.func5`: The option `--type-hints-in-docstring` is '
+            'DOC108: Method `MyClass.func5`: The option `--arg-type-hints-in-signature` is '
+            '`False` but there are argument type hints in the signature ',
+            'DOC111: Method `MyClass.func5`: The option `--arg-type-hints-in-docstring` is '
             '`False` but there are type hints in the docstring arg list ',
-            'DOC108: Method `MyClass.func6`: The option `--type-hints-in-signature` is '
-            '`False` but there are type hints in the signature ',
-            'DOC111: Method `MyClass.func6`: The option `--type-hints-in-docstring` is '
+            'DOC108: Method `MyClass.func6`: The option `--arg-type-hints-in-signature` is '
+            '`False` but there are argument type hints in the signature ',
+            'DOC111: Method `MyClass.func6`: The option `--arg-type-hints-in-docstring` is '
             '`False` but there are type hints in the docstring arg list ',
-            'DOC108: Method `MyClass.func7`: The option `--type-hints-in-signature` is '
-            '`False` but there are type hints in the signature ',
-            'DOC111: Method `MyClass.func7`: The option `--type-hints-in-docstring` is '
+            'DOC108: Method `MyClass.func7`: The option `--arg-type-hints-in-signature` is '
+            '`False` but there are argument type hints in the signature ',
+            'DOC111: Method `MyClass.func7`: The option `--arg-type-hints-in-docstring` is '
             '`False` but there are type hints in the docstring arg list ',
         ],
         (False, True): [
-            'DOC106: Method `MyClass.func1`: The option `--type-hints-in-signature` is '
-            '`True` but there are no type hints in the signature ',
-            'DOC107: Method `MyClass.func1`: The option `--type-hints-in-signature` is '
+            'DOC106: Method `MyClass.func1`: The option `--arg-type-hints-in-signature` is '
+            '`True` but there are no argument type hints in the signature ',
+            'DOC107: Method `MyClass.func1`: The option `--arg-type-hints-in-signature` is '
             '`True` but not all args in the signature have type hints ',
-            'DOC106: Method `MyClass.func3`: The option `--type-hints-in-signature` is '
-            '`True` but there are no type hints in the signature ',
-            'DOC107: Method `MyClass.func3`: The option `--type-hints-in-signature` is '
+            'DOC106: Method `MyClass.func3`: The option `--arg-type-hints-in-signature` is '
+            '`True` but there are no argument type hints in the signature ',
+            'DOC107: Method `MyClass.func3`: The option `--arg-type-hints-in-signature` is '
             '`True` but not all args in the signature have type hints ',
-            'DOC111: Method `MyClass.func3`: The option `--type-hints-in-docstring` is '
+            'DOC111: Method `MyClass.func3`: The option `--arg-type-hints-in-docstring` is '
             '`False` but there are type hints in the docstring arg list ',
-            'DOC111: Method `MyClass.func4`: The option `--type-hints-in-docstring` is '
+            'DOC111: Method `MyClass.func4`: The option `--arg-type-hints-in-docstring` is '
             '`False` but there are type hints in the docstring arg list ',
-            'DOC107: Method `MyClass.func5`: The option `--type-hints-in-signature` is '
+            'DOC107: Method `MyClass.func5`: The option `--arg-type-hints-in-signature` is '
             '`True` but not all args in the signature have type hints ',
-            'DOC111: Method `MyClass.func5`: The option `--type-hints-in-docstring` is '
+            'DOC111: Method `MyClass.func5`: The option `--arg-type-hints-in-docstring` is '
             '`False` but there are type hints in the docstring arg list ',
-            'DOC111: Method `MyClass.func6`: The option `--type-hints-in-docstring` is '
+            'DOC111: Method `MyClass.func6`: The option `--arg-type-hints-in-docstring` is '
             '`False` but there are type hints in the docstring arg list ',
-            'DOC107: Method `MyClass.func7`: The option `--type-hints-in-signature` is '
+            'DOC107: Method `MyClass.func7`: The option `--arg-type-hints-in-signature` is '
             '`True` but not all args in the signature have type hints ',
-            'DOC111: Method `MyClass.func7`: The option `--type-hints-in-docstring` is '
+            'DOC111: Method `MyClass.func7`: The option `--arg-type-hints-in-docstring` is '
             '`False` but there are type hints in the docstring arg list ',
         ],
         (True, False): [
-            'DOC109: Method `MyClass.func1`: The option `--type-hints-in-docstring` is '
+            'DOC109: Method `MyClass.func1`: The option `--arg-type-hints-in-docstring` is '
             '`True` but there are no type hints in the docstring arg list ',
-            'DOC110: Method `MyClass.func1`: The option `--type-hints-in-docstring` is '
+            'DOC110: Method `MyClass.func1`: The option `--arg-type-hints-in-docstring` is '
             '`True` but not all args in the docstring arg list have type hints ',
-            'DOC108: Method `MyClass.func2`: The option `--type-hints-in-signature` is '
-            '`False` but there are type hints in the signature ',
-            'DOC109: Method `MyClass.func2`: The option `--type-hints-in-docstring` is '
+            'DOC108: Method `MyClass.func2`: The option `--arg-type-hints-in-signature` is '
+            '`False` but there are argument type hints in the signature ',
+            'DOC109: Method `MyClass.func2`: The option `--arg-type-hints-in-docstring` is '
             '`True` but there are no type hints in the docstring arg list ',
-            'DOC110: Method `MyClass.func2`: The option `--type-hints-in-docstring` is '
+            'DOC110: Method `MyClass.func2`: The option `--arg-type-hints-in-docstring` is '
             '`True` but not all args in the docstring arg list have type hints ',
-            'DOC108: Method `MyClass.func4`: The option `--type-hints-in-signature` is '
-            '`False` but there are type hints in the signature ',
-            'DOC108: Method `MyClass.func5`: The option `--type-hints-in-signature` is '
-            '`False` but there are type hints in the signature ',
-            'DOC110: Method `MyClass.func5`: The option `--type-hints-in-docstring` is '
+            'DOC108: Method `MyClass.func4`: The option `--arg-type-hints-in-signature` is '
+            '`False` but there are argument type hints in the signature ',
+            'DOC108: Method `MyClass.func5`: The option `--arg-type-hints-in-signature` is '
+            '`False` but there are argument type hints in the signature ',
+            'DOC110: Method `MyClass.func5`: The option `--arg-type-hints-in-docstring` is '
             '`True` but not all args in the docstring arg list have type hints ',
-            'DOC108: Method `MyClass.func6`: The option `--type-hints-in-signature` is '
-            '`False` but there are type hints in the signature ',
-            'DOC108: Method `MyClass.func7`: The option `--type-hints-in-signature` is '
-            '`False` but there are type hints in the signature ',
-            'DOC110: Method `MyClass.func7`: The option `--type-hints-in-docstring` is '
+            'DOC108: Method `MyClass.func6`: The option `--arg-type-hints-in-signature` is '
+            '`False` but there are argument type hints in the signature ',
+            'DOC108: Method `MyClass.func7`: The option `--arg-type-hints-in-signature` is '
+            '`False` but there are argument type hints in the signature ',
+            'DOC110: Method `MyClass.func7`: The option `--arg-type-hints-in-docstring` is '
             '`True` but not all args in the docstring arg list have type hints ',
         ],
         (True, True): [
-            'DOC106: Method `MyClass.func1`: The option `--type-hints-in-signature` is '
-            '`True` but there are no type hints in the signature ',
-            'DOC107: Method `MyClass.func1`: The option `--type-hints-in-signature` is '
+            'DOC106: Method `MyClass.func1`: The option `--arg-type-hints-in-signature` is '
+            '`True` but there are no argument type hints in the signature ',
+            'DOC107: Method `MyClass.func1`: The option `--arg-type-hints-in-signature` is '
             '`True` but not all args in the signature have type hints ',
-            'DOC109: Method `MyClass.func1`: The option `--type-hints-in-docstring` is '
+            'DOC109: Method `MyClass.func1`: The option `--arg-type-hints-in-docstring` is '
             '`True` but there are no type hints in the docstring arg list ',
-            'DOC110: Method `MyClass.func1`: The option `--type-hints-in-docstring` is '
+            'DOC110: Method `MyClass.func1`: The option `--arg-type-hints-in-docstring` is '
             '`True` but not all args in the docstring arg list have type hints ',
-            'DOC109: Method `MyClass.func2`: The option `--type-hints-in-docstring` is '
+            'DOC109: Method `MyClass.func2`: The option `--arg-type-hints-in-docstring` is '
             '`True` but there are no type hints in the docstring arg list ',
-            'DOC110: Method `MyClass.func2`: The option `--type-hints-in-docstring` is '
+            'DOC110: Method `MyClass.func2`: The option `--arg-type-hints-in-docstring` is '
             '`True` but not all args in the docstring arg list have type hints ',
             'DOC105: Method `MyClass.func2`: Argument names match, but type hints do not '
             'match ',
-            'DOC106: Method `MyClass.func3`: The option `--type-hints-in-signature` is '
-            '`True` but there are no type hints in the signature ',
-            'DOC107: Method `MyClass.func3`: The option `--type-hints-in-signature` is '
+            'DOC106: Method `MyClass.func3`: The option `--arg-type-hints-in-signature` is '
+            '`True` but there are no argument type hints in the signature ',
+            'DOC107: Method `MyClass.func3`: The option `--arg-type-hints-in-signature` is '
             '`True` but not all args in the signature have type hints ',
             'DOC105: Method `MyClass.func3`: Argument names match, but type hints do not '
             'match ',
-            'DOC107: Method `MyClass.func5`: The option `--type-hints-in-signature` is '
+            'DOC107: Method `MyClass.func5`: The option `--arg-type-hints-in-signature` is '
             '`True` but not all args in the signature have type hints ',
-            'DOC110: Method `MyClass.func5`: The option `--type-hints-in-docstring` is '
+            'DOC110: Method `MyClass.func5`: The option `--arg-type-hints-in-docstring` is '
             '`True` but not all args in the docstring arg list have type hints ',
             'DOC105: Method `MyClass.func5`: Argument names match, but type hints do not '
             'match ',
             'DOC105: Method `MyClass.func6`: Argument names match, but type hints do not '
             'match ',
-            'DOC107: Method `MyClass.func7`: The option `--type-hints-in-signature` is '
+            'DOC107: Method `MyClass.func7`: The option `--arg-type-hints-in-signature` is '
             '`True` but not all args in the signature have type hints ',
-            'DOC110: Method `MyClass.func7`: The option `--type-hints-in-docstring` is '
+            'DOC110: Method `MyClass.func7`: The option `--arg-type-hints-in-docstring` is '
             '`True` but not all args in the docstring arg list have type hints ',
         ],
     }
 
-    expected = expected_lookup[(typeHintsInDocstring, typeHintsInSignature)]
+    expected = expected_lookup[
+        (argTypeHintsInDocstring, argTypeHintsInSignature)
+    ]
     assert list(map(str, violations)) == expected
 
 
 def testNonAscii() -> None:
     """Don't crash on non ASCII arguments."""
     violations = _checkFile(
         filename=DATA_DIR / 'common/non_ascii/non_ascii.py',
```

### Comparing `pydoclint-0.1.1/tests/test_parse_config.py` & `pydoclint-0.1.2/tests/test_parse_config.py`

 * *Files identical despite different names*

