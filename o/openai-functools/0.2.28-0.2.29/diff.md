# Comparing `tmp/openai_functools-0.2.28.tar.gz` & `tmp/openai_functools-0.2.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functools-0.2.28.tar", max compression
+gzip compressed data, was "openai_functools-0.2.29.tar", max compression
```

## Comparing `openai_functools-0.2.28.tar` & `openai_functools-0.2.29.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-07-21 13:59:03.278084 openai_functools-0.2.28/LICENSE
--rw-r--r--   0        0        0     1766 2023-07-21 13:59:03.278084 openai_functools-0.2.28/README.md
--rw-r--r--   0        0        0      195 2023-07-21 13:59:03.278084 openai_functools-0.2.28/openai_functools/__init__.py
--rw-r--r--   0        0        0     1755 2023-07-21 13:59:03.278084 openai_functools-0.2.28/openai_functools/metadata_generator.py
--rw-r--r--   0        0        0      470 2023-07-21 13:59:03.278084 openai_functools-0.2.28/openai_functools/types.py
--rw-r--r--   0        0        0     2318 2023-07-21 13:59:03.278084 openai_functools-0.2.28/openai_functools/utils/openai_service.py
--rw-r--r--   0        0        0      537 2023-07-21 13:59:24.782831 openai_functools-0.2.28/pyproject.toml
--rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 openai_functools-0.2.28/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-21 14:00:46.605824 openai_functools-0.2.29/LICENSE
+-rw-r--r--   0        0        0     3868 2023-07-21 14:00:46.609824 openai_functools-0.2.29/README.md
+-rw-r--r--   0        0        0      195 2023-07-21 14:00:46.609824 openai_functools-0.2.29/openai_functools/__init__.py
+-rw-r--r--   0        0        0     1755 2023-07-21 14:00:46.609824 openai_functools-0.2.29/openai_functools/metadata_generator.py
+-rw-r--r--   0        0        0      470 2023-07-21 14:00:46.609824 openai_functools-0.2.29/openai_functools/types.py
+-rw-r--r--   0        0        0     2318 2023-07-21 14:00:46.609824 openai_functools-0.2.29/openai_functools/utils/openai_service.py
+-rw-r--r--   0        0        0      537 2023-07-21 14:01:13.710109 openai_functools-0.2.29/pyproject.toml
+-rw-r--r--   0        0        0     4515 1970-01-01 00:00:00.000000 openai_functools-0.2.29/PKG-INFO
```

### Comparing `openai_functools-0.2.28/LICENSE` & `openai_functools-0.2.29/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_functools-0.2.28/openai_functools/metadata_generator.py` & `openai_functools-0.2.29/openai_functools/metadata_generator.py`

 * *Files identical despite different names*

### Comparing `openai_functools-0.2.28/openai_functools/utils/openai_service.py` & `openai_functools-0.2.29/openai_functools/utils/openai_service.py`

 * *Files identical despite different names*

### Comparing `openai_functools-0.2.28/pyproject.toml` & `openai_functools-0.2.29/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai_functools"
-version = "0.2.28"
+version = "0.2.29"
 description = "python openai functions tooling"
 authors = ["Jakob Serlier <37184788+Jakob-98@users.noreply.github.com>", "Marc van Duyn <codingkitties@gmail.com>"]
 readme = "README.md"
 packages = [{include = "openai_functools"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

