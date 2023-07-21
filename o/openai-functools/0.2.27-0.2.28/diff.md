# Comparing `tmp/openai_functools-0.2.27.tar.gz` & `tmp/openai_functools-0.2.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functools-0.2.27.tar", max compression
+gzip compressed data, was "openai_functools-0.2.28.tar", max compression
```

## Comparing `openai_functools-0.2.27.tar` & `openai_functools-0.2.28.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-07-21 13:58:48.194653 openai_functools-0.2.27/LICENSE
--rw-r--r--   0        0        0     1766 2023-07-21 13:58:48.194653 openai_functools-0.2.27/README.md
--rw-r--r--   0        0        0      195 2023-07-21 13:58:48.194653 openai_functools-0.2.27/openai_functools/__init__.py
--rw-r--r--   0        0        0     1755 2023-07-21 13:58:48.194653 openai_functools-0.2.27/openai_functools/metadata_generator.py
--rw-r--r--   0        0        0      470 2023-07-21 13:58:48.194653 openai_functools-0.2.27/openai_functools/types.py
--rw-r--r--   0        0        0     2318 2023-07-21 13:58:48.194653 openai_functools-0.2.27/openai_functools/utils/openai_service.py
--rw-r--r--   0        0        0      537 2023-07-21 13:59:09.551009 openai_functools-0.2.27/pyproject.toml
--rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 openai_functools-0.2.27/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-21 13:59:03.278084 openai_functools-0.2.28/LICENSE
+-rw-r--r--   0        0        0     1766 2023-07-21 13:59:03.278084 openai_functools-0.2.28/README.md
+-rw-r--r--   0        0        0      195 2023-07-21 13:59:03.278084 openai_functools-0.2.28/openai_functools/__init__.py
+-rw-r--r--   0        0        0     1755 2023-07-21 13:59:03.278084 openai_functools-0.2.28/openai_functools/metadata_generator.py
+-rw-r--r--   0        0        0      470 2023-07-21 13:59:03.278084 openai_functools-0.2.28/openai_functools/types.py
+-rw-r--r--   0        0        0     2318 2023-07-21 13:59:03.278084 openai_functools-0.2.28/openai_functools/utils/openai_service.py
+-rw-r--r--   0        0        0      537 2023-07-21 13:59:24.782831 openai_functools-0.2.28/pyproject.toml
+-rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 openai_functools-0.2.28/PKG-INFO
```

### Comparing `openai_functools-0.2.27/LICENSE` & `openai_functools-0.2.28/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_functools-0.2.27/README.md` & `openai_functools-0.2.28/README.md`

 * *Files identical despite different names*

### Comparing `openai_functools-0.2.27/openai_functools/metadata_generator.py` & `openai_functools-0.2.28/openai_functools/metadata_generator.py`

 * *Files identical despite different names*

### Comparing `openai_functools-0.2.27/openai_functools/utils/openai_service.py` & `openai_functools-0.2.28/openai_functools/utils/openai_service.py`

 * *Files identical despite different names*

### Comparing `openai_functools-0.2.27/pyproject.toml` & `openai_functools-0.2.28/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai_functools"
-version = "0.2.27"
+version = "0.2.28"
 description = "python openai functions tooling"
 authors = ["Jakob Serlier <37184788+Jakob-98@users.noreply.github.com>", "Marc van Duyn <codingkitties@gmail.com>"]
 readme = "README.md"
 packages = [{include = "openai_functools"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `openai_functools-0.2.27/PKG-INFO` & `openai_functools-0.2.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-functools
-Version: 0.2.27
+Version: 0.2.28
 Summary: python openai functions tooling
 Author: Jakob Serlier
 Author-email: 37184788+Jakob-98@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

