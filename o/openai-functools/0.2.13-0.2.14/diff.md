# Comparing `tmp/openai_functools-0.2.13.tar.gz` & `tmp/openai_functools-0.2.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functools-0.2.13.tar", max compression
+gzip compressed data, was "openai_functools-0.2.14.tar", max compression
```

## Comparing `openai_functools-0.2.13.tar` & `openai_functools-0.2.14.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-07-21 12:37:12.157626 openai_functools-0.2.13/LICENSE
--rw-r--r--   0        0        0     1653 2023-07-21 12:37:12.157626 openai_functools-0.2.13/README.md
--rw-r--r--   0        0        0      169 2023-07-21 12:37:12.157626 openai_functools-0.2.13/openai_functools/__init__.py
--rw-r--r--   0        0        0     2054 2023-07-21 12:37:12.157626 openai_functools-0.2.13/openai_functools/metadata_generator.py
--rw-r--r--   0        0        0      470 2023-07-21 12:37:12.157626 openai_functools-0.2.13/openai_functools/types.py
--rw-r--r--   0        0        0     2318 2023-07-21 12:37:12.157626 openai_functools-0.2.13/openai_functools/utils/openai_service.py
--rw-r--r--   0        0        0      510 2023-07-21 12:37:40.301770 openai_functools-0.2.13/pyproject.toml
--rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 openai_functools-0.2.13/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-21 12:43:17.417484 openai_functools-0.2.14/LICENSE
+-rw-r--r--   0        0        0     1653 2023-07-21 12:43:17.417484 openai_functools-0.2.14/README.md
+-rw-r--r--   0        0        0      169 2023-07-21 12:43:17.417484 openai_functools-0.2.14/openai_functools/__init__.py
+-rw-r--r--   0        0        0     2054 2023-07-21 12:43:17.417484 openai_functools-0.2.14/openai_functools/metadata_generator.py
+-rw-r--r--   0        0        0      470 2023-07-21 12:43:17.417484 openai_functools-0.2.14/openai_functools/types.py
+-rw-r--r--   0        0        0     2318 2023-07-21 12:43:17.417484 openai_functools-0.2.14/openai_functools/utils/openai_service.py
+-rw-r--r--   0        0        0      510 2023-07-21 12:43:38.081357 openai_functools-0.2.14/pyproject.toml
+-rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 openai_functools-0.2.14/PKG-INFO
```

### Comparing `openai_functools-0.2.13/LICENSE` & `openai_functools-0.2.14/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_functools-0.2.13/README.md` & `openai_functools-0.2.14/README.md`

 * *Files identical despite different names*

### Comparing `openai_functools-0.2.13/openai_functools/metadata_generator.py` & `openai_functools-0.2.14/openai_functools/metadata_generator.py`

 * *Files identical despite different names*

### Comparing `openai_functools-0.2.13/openai_functools/utils/openai_service.py` & `openai_functools-0.2.14/openai_functools/utils/openai_service.py`

 * *Files identical despite different names*

### Comparing `openai_functools-0.2.13/PKG-INFO` & `openai_functools-0.2.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-functools
-Version: 0.2.13
+Version: 0.2.14
 Summary: python openai functions tooling
 Author: Jakob Serlier
 Author-email: 37184788+Jakob-98@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

