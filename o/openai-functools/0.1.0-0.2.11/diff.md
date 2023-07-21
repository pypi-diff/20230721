# Comparing `tmp/openai_functools-0.1.0.tar.gz` & `tmp/openai_functools-0.2.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functools-0.1.0.tar", max compression
+gzip compressed data, was "openai_functools-0.2.11.tar", max compression
```

## Comparing `openai_functools-0.1.0.tar` & `openai_functools-0.2.11.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0       11 2023-07-21 12:15:45.326850 openai_functools-0.1.0/README.md
--rw-r--r--   0        0        0     2054 2023-07-21 12:15:45.326850 openai_functools-0.1.0/openai_functools/metadata_generator.py
--rw-r--r--   0        0        0      470 2023-07-21 12:15:45.326850 openai_functools-0.1.0/openai_functools/types.py
--rw-r--r--   0        0        0     2318 2023-07-21 12:15:45.326850 openai_functools-0.1.0/openai_functools/utils/openai_service.py
--rw-r--r--   0        0        0      509 2023-07-21 12:15:45.326850 openai_functools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 openai_functools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       11 2023-07-21 12:31:37.091861 openai_functools-0.2.11/README.md
+-rw-r--r--   0        0        0      169 2023-07-21 12:31:37.091861 openai_functools-0.2.11/openai_functools/__init__.py
+-rw-r--r--   0        0        0     2054 2023-07-21 12:31:37.091861 openai_functools-0.2.11/openai_functools/metadata_generator.py
+-rw-r--r--   0        0        0      470 2023-07-21 12:31:37.091861 openai_functools-0.2.11/openai_functools/types.py
+-rw-r--r--   0        0        0     2318 2023-07-21 12:31:37.091861 openai_functools-0.2.11/openai_functools/utils/openai_service.py
+-rw-r--r--   0        0        0      510 2023-07-21 12:31:59.491906 openai_functools-0.2.11/pyproject.toml
+-rw-r--r--   0        0        0      611 1970-01-01 00:00:00.000000 openai_functools-0.2.11/PKG-INFO
```

### Comparing `openai_functools-0.1.0/openai_functools/metadata_generator.py` & `openai_functools-0.2.11/openai_functools/metadata_generator.py`

 * *Files identical despite different names*

### Comparing `openai_functools-0.1.0/openai_functools/utils/openai_service.py` & `openai_functools-0.2.11/openai_functools/utils/openai_service.py`

 * *Files identical despite different names*

### Comparing `openai_functools-0.1.0/PKG-INFO` & `openai_functools-0.2.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-functools
-Version: 0.1.0
+Version: 0.2.11
 Summary: python openai functions tooling
 Author: Jakob Serlier
 Author-email: 37184788+Jakob-98@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

