# Comparing `tmp/openai_functools-0.2.25.tar.gz` & `tmp/openai_functools-0.2.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functools-0.2.25.tar", max compression
+gzip compressed data, was "openai_functools-0.2.26.tar", max compression
```

## Comparing `openai_functools-0.2.25.tar` & `openai_functools-0.2.26.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-07-21 13:46:08.700179 openai_functools-0.2.25/LICENSE
--rw-r--r--   0        0        0     1766 2023-07-21 13:46:08.700179 openai_functools-0.2.25/README.md
--rw-r--r--   0        0        0      195 2023-07-21 13:46:08.704179 openai_functools-0.2.25/openai_functools/__init__.py
--rw-r--r--   0        0        0     1755 2023-07-21 13:46:08.704179 openai_functools-0.2.25/openai_functools/metadata_generator.py
--rw-r--r--   0        0        0      470 2023-07-21 13:46:08.704179 openai_functools-0.2.25/openai_functools/types.py
--rw-r--r--   0        0        0     2318 2023-07-21 13:46:08.704179 openai_functools-0.2.25/openai_functools/utils/openai_service.py
--rw-r--r--   0        0        0      537 2023-07-21 13:46:31.896596 openai_functools-0.2.25/pyproject.toml
--rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 openai_functools-0.2.25/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-21 13:46:42.512278 openai_functools-0.2.26/LICENSE
+-rw-r--r--   0        0        0     1766 2023-07-21 13:46:42.512278 openai_functools-0.2.26/README.md
+-rw-r--r--   0        0        0      195 2023-07-21 13:46:42.512278 openai_functools-0.2.26/openai_functools/__init__.py
+-rw-r--r--   0        0        0     1755 2023-07-21 13:46:42.512278 openai_functools-0.2.26/openai_functools/metadata_generator.py
+-rw-r--r--   0        0        0      470 2023-07-21 13:46:42.512278 openai_functools-0.2.26/openai_functools/types.py
+-rw-r--r--   0        0        0     2318 2023-07-21 13:46:42.512278 openai_functools-0.2.26/openai_functools/utils/openai_service.py
+-rw-r--r--   0        0        0      537 2023-07-21 13:47:08.758196 openai_functools-0.2.26/pyproject.toml
+-rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 openai_functools-0.2.26/PKG-INFO
```

### Comparing `openai_functools-0.2.25/LICENSE` & `openai_functools-0.2.26/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_functools-0.2.25/README.md` & `openai_functools-0.2.26/README.md`

 * *Files identical despite different names*

### Comparing `openai_functools-0.2.25/openai_functools/metadata_generator.py` & `openai_functools-0.2.26/openai_functools/metadata_generator.py`

 * *Files identical despite different names*

### Comparing `openai_functools-0.2.25/openai_functools/utils/openai_service.py` & `openai_functools-0.2.26/openai_functools/utils/openai_service.py`

 * *Files identical despite different names*

### Comparing `openai_functools-0.2.25/pyproject.toml` & `openai_functools-0.2.26/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai_functools"
-version = "0.2.25"
+version = "0.2.26"
 description = "python openai functions tooling"
 authors = ["Jakob Serlier <37184788+Jakob-98@users.noreply.github.com>", "Marc van Duyn <codingkitties@gmail.com>"]
 readme = "README.md"
 packages = [{include = "openai_functools"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `openai_functools-0.2.25/PKG-INFO` & `openai_functools-0.2.26/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-functools
-Version: 0.2.25
+Version: 0.2.26
 Summary: python openai functions tooling
 Author: Jakob Serlier
 Author-email: 37184788+Jakob-98@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

