# Comparing `tmp/openai_functools-0.2.19.tar.gz` & `tmp/openai_functools-0.2.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functools-0.2.19.tar", max compression
+gzip compressed data, was "openai_functools-0.2.20.tar", max compression
```

## Comparing `openai_functools-0.2.19.tar` & `openai_functools-0.2.20.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-07-21 13:27:26.718562 openai_functools-0.2.19/LICENSE
--rw-r--r--   0        0        0     1653 2023-07-21 13:27:26.718562 openai_functools-0.2.19/README.md
--rw-r--r--   0        0        0      169 2023-07-21 13:27:26.718562 openai_functools-0.2.19/openai_functools/__init__.py
--rw-r--r--   0        0        0     2054 2023-07-21 13:27:26.718562 openai_functools-0.2.19/openai_functools/metadata_generator.py
--rw-r--r--   0        0        0      470 2023-07-21 13:27:26.718562 openai_functools-0.2.19/openai_functools/types.py
--rw-r--r--   0        0        0     2318 2023-07-21 13:27:26.718562 openai_functools-0.2.19/openai_functools/utils/openai_service.py
--rw-r--r--   0        0        0      510 2023-07-21 13:27:55.490841 openai_functools-0.2.19/pyproject.toml
--rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 openai_functools-0.2.19/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-21 13:27:42.766337 openai_functools-0.2.20/LICENSE
+-rw-r--r--   0        0        0     1653 2023-07-21 13:27:42.766337 openai_functools-0.2.20/README.md
+-rw-r--r--   0        0        0      169 2023-07-21 13:27:42.766337 openai_functools-0.2.20/openai_functools/__init__.py
+-rw-r--r--   0        0        0     2054 2023-07-21 13:27:42.766337 openai_functools-0.2.20/openai_functools/metadata_generator.py
+-rw-r--r--   0        0        0      470 2023-07-21 13:27:42.766337 openai_functools-0.2.20/openai_functools/types.py
+-rw-r--r--   0        0        0     2318 2023-07-21 13:27:42.766337 openai_functools-0.2.20/openai_functools/utils/openai_service.py
+-rw-r--r--   0        0        0      510 2023-07-21 13:28:07.942602 openai_functools-0.2.20/pyproject.toml
+-rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 openai_functools-0.2.20/PKG-INFO
```

### Comparing `openai_functools-0.2.19/LICENSE` & `openai_functools-0.2.20/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_functools-0.2.19/README.md` & `openai_functools-0.2.20/README.md`

 * *Files identical despite different names*

### Comparing `openai_functools-0.2.19/openai_functools/metadata_generator.py` & `openai_functools-0.2.20/openai_functools/metadata_generator.py`

 * *Files identical despite different names*

### Comparing `openai_functools-0.2.19/openai_functools/utils/openai_service.py` & `openai_functools-0.2.20/openai_functools/utils/openai_service.py`

 * *Files identical despite different names*

### Comparing `openai_functools-0.2.19/PKG-INFO` & `openai_functools-0.2.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-functools
-Version: 0.2.19
+Version: 0.2.20
 Summary: python openai functions tooling
 Author: Jakob Serlier
 Author-email: 37184788+Jakob-98@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

