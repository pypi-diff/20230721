# Comparing `tmp/maglevai-0.1.2.tar.gz` & `tmp/maglevai-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maglevai-0.1.2.tar", max compression
+gzip compressed data, was "maglevai-0.1.3.tar", max compression
```

## Comparing `maglevai-0.1.2.tar` & `maglevai-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-07-21 16:45:01.152228 maglevai-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-07-21 16:45:01.152104 maglevai-0.1.2/maglevai/__init__.py
--rw-r--r--   0        0        0     1513 2023-07-21 17:25:06.526000 maglevai-0.1.2/maglevai/main.py
--rw-r--r--   0        0        0      346 2023-07-21 17:26:31.970090 maglevai-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 maglevai-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-21 16:45:01.152228 maglevai-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 16:45:01.152105 maglevai-0.1.3/maglevai/__init__.py
+-rw-r--r--   0        0        0     1513 2023-07-21 17:25:06.526000 maglevai-0.1.3/maglevai/main.py
+-rw-r--r--   0        0        0      408 2023-07-21 17:38:25.625165 maglevai-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 maglevai-0.1.3/PKG-INFO
```

### Comparing `maglevai-0.1.2/maglevai/main.py` & `maglevai-0.1.3/maglevai/main.py`

 * *Files identical despite different names*

### Comparing `maglevai-0.1.2/PKG-INFO` & `maglevai-0.1.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: maglevai
-Version: 0.1.2
-Summary: Making AI Content Trustworthy
+Version: 0.1.3
+Summary: Making AI content safe and trustworthy
+Home-page: https://github.com/Maglev-AI/MaglevAI
 Author: Maglev AI, Inc.
 Author-email: 97685959+MaglevAIInc@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Project-URL: Repository, https://github.com/Maglev-AI/MaglevAI
 Description-Content-Type: text/markdown
```

