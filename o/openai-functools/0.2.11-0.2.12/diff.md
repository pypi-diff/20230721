# Comparing `tmp/openai_functools-0.2.11.tar.gz` & `tmp/openai_functools-0.2.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functools-0.2.11.tar", max compression
+gzip compressed data, was "openai_functools-0.2.12.tar", max compression
```

## Comparing `openai_functools-0.2.11.tar` & `openai_functools-0.2.12.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       11 2023-07-21 12:31:37.091861 openai_functools-0.2.11/README.md
--rw-r--r--   0        0        0      169 2023-07-21 12:31:37.091861 openai_functools-0.2.11/openai_functools/__init__.py
--rw-r--r--   0        0        0     2054 2023-07-21 12:31:37.091861 openai_functools-0.2.11/openai_functools/metadata_generator.py
--rw-r--r--   0        0        0      470 2023-07-21 12:31:37.091861 openai_functools-0.2.11/openai_functools/types.py
--rw-r--r--   0        0        0     2318 2023-07-21 12:31:37.091861 openai_functools-0.2.11/openai_functools/utils/openai_service.py
--rw-r--r--   0        0        0      510 2023-07-21 12:31:59.491906 openai_functools-0.2.11/pyproject.toml
--rw-r--r--   0        0        0      611 1970-01-01 00:00:00.000000 openai_functools-0.2.11/PKG-INFO
+-rw-r--r--   0        0        0     1653 2023-07-21 12:36:03.232874 openai_functools-0.2.12/README.md
+-rw-r--r--   0        0        0      169 2023-07-21 12:36:03.232874 openai_functools-0.2.12/openai_functools/__init__.py
+-rw-r--r--   0        0        0     2054 2023-07-21 12:36:03.232874 openai_functools-0.2.12/openai_functools/metadata_generator.py
+-rw-r--r--   0        0        0      470 2023-07-21 12:36:03.232874 openai_functools-0.2.12/openai_functools/types.py
+-rw-r--r--   0        0        0     2318 2023-07-21 12:36:03.232874 openai_functools-0.2.12/openai_functools/utils/openai_service.py
+-rw-r--r--   0        0        0      510 2023-07-21 12:36:25.761042 openai_functools-0.2.12/pyproject.toml
+-rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 openai_functools-0.2.12/PKG-INFO
```

### Comparing `openai_functools-0.2.11/openai_functools/metadata_generator.py` & `openai_functools-0.2.12/openai_functools/metadata_generator.py`

 * *Files identical despite different names*

### Comparing `openai_functools-0.2.11/openai_functools/utils/openai_service.py` & `openai_functools-0.2.12/openai_functools/utils/openai_service.py`

 * *Files identical despite different names*

