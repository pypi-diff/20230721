# Comparing `tmp/pytest_dogu_sdk-1.0.0.tar.gz` & `tmp/pytest_dogu_sdk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_dogu_sdk-1.0.0.tar", max compression
+gzip compressed data, was "pytest_dogu_sdk-1.0.1.tar", max compression
```

## Comparing `pytest_dogu_sdk-1.0.0.tar` & `pytest_dogu_sdk-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      899 2023-07-21 04:07:57.198859 pytest_dogu_sdk-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1690 2023-07-20 16:33:36.015474 pytest_dogu_sdk-1.0.0/README.md
--rw-r--r--   0        0        0     1031 2023-07-21 04:07:57.199858 pytest_dogu_sdk-1.0.0/src/pytest_dogu_sdk/__init__.py
--rw-r--r--   0        0        0     3258 2023-07-21 04:07:57.199858 pytest_dogu_sdk-1.0.0/src/pytest_dogu_sdk/common.py
--rw-r--r--   0        0        0     1885 2023-07-20 16:33:36.020475 pytest_dogu_sdk-1.0.0/src/pytest_dogu_sdk/dogu.config.schema.json
--rw-r--r--   0        0        0     3163 2023-07-20 16:33:36.021473 pytest_dogu_sdk-1.0.0/src/pytest_dogu_sdk/dogu_config.py
--rw-r--r--   0        0        0       89 2023-07-21 04:07:57.200858 pytest_dogu_sdk-1.0.0/src/pytest_dogu_sdk/dogu_hooks.py
--rw-r--r--   0        0        0     2721 2023-07-21 04:07:57.265860 pytest_dogu_sdk-1.0.0/src/pytest_dogu_sdk/dogu_sdk.py
--rw-r--r--   0        0        0     2832 2023-07-20 16:33:36.023474 pytest_dogu_sdk-1.0.0/src/pytest_dogu_sdk/remote_dest_report_client.py
--rw-r--r--   0        0        0     9664 2023-07-21 04:07:57.201858 pytest_dogu_sdk-1.0.0/src/pytest_dogu_sdk/remote_dest_reporter.py
--rw-r--r--   0        0        0     3037 2023-07-20 16:33:36.024474 pytest_dogu_sdk-1.0.0/src/pytest_dogu_sdk/routine_dest_report_client.py
--rw-r--r--   0        0        0     9774 2023-07-20 16:33:36.024474 pytest_dogu_sdk-1.0.0/src/pytest_dogu_sdk/routine_dest_reporter.py
--rw-r--r--   0        0        0     2218 1970-01-01 00:00:00.000000 pytest_dogu_sdk-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      899 2023-07-21 05:40:53.100944 pytest_dogu_sdk-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1690 2023-07-20 16:33:36.015474 pytest_dogu_sdk-1.0.1/README.md
+-rw-r--r--   0        0        0     1031 2023-07-21 04:07:57.199858 pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/__init__.py
+-rw-r--r--   0        0        0     3258 2023-07-21 04:07:57.199858 pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/common.py
+-rw-r--r--   0        0        0     1885 2023-07-20 16:33:36.020475 pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/dogu.config.schema.json
+-rw-r--r--   0        0        0     3163 2023-07-20 16:33:36.021473 pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/dogu_config.py
+-rw-r--r--   0        0        0       89 2023-07-21 04:07:57.200858 pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/dogu_hooks.py
+-rw-r--r--   0        0        0     2721 2023-07-21 04:07:57.265860 pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/dogu_sdk.py
+-rw-r--r--   0        0        0     2832 2023-07-20 16:33:36.023474 pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/remote_dest_report_client.py
+-rw-r--r--   0        0        0     9664 2023-07-21 04:07:57.201858 pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/remote_dest_reporter.py
+-rw-r--r--   0        0        0     3037 2023-07-20 16:33:36.024474 pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/routine_dest_report_client.py
+-rw-r--r--   0        0        0     9774 2023-07-20 16:33:36.024474 pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/routine_dest_reporter.py
+-rw-r--r--   0        0        0     2218 1970-01-01 00:00:00.000000 pytest_dogu_sdk-1.0.1/PKG-INFO
```

### Comparing `pytest_dogu_sdk-1.0.0/pyproject.toml` & `pytest_dogu_sdk-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-dogu-sdk"
-version = "1.0.0"
+version = "1.0.1"
 description = "pytest plugin for the Dogu"
 readme = "README.md"
 packages = [{include = "pytest_dogu_sdk", from = "src"}]
 authors = ["Dogu Technologies"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `pytest_dogu_sdk-1.0.0/README.md` & `pytest_dogu_sdk-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.0/src/pytest_dogu_sdk/__init__.py` & `pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.0/src/pytest_dogu_sdk/common.py` & `pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/common.py`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.0/src/pytest_dogu_sdk/dogu.config.schema.json` & `pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/dogu.config.schema.json`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.0/src/pytest_dogu_sdk/dogu_config.py` & `pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/dogu_config.py`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.0/src/pytest_dogu_sdk/dogu_sdk.py` & `pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/dogu_sdk.py`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.0/src/pytest_dogu_sdk/remote_dest_report_client.py` & `pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/remote_dest_report_client.py`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.0/src/pytest_dogu_sdk/remote_dest_reporter.py` & `pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/remote_dest_reporter.py`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.0/src/pytest_dogu_sdk/routine_dest_report_client.py` & `pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/routine_dest_report_client.py`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.0/src/pytest_dogu_sdk/routine_dest_reporter.py` & `pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/routine_dest_reporter.py`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.0/PKG-INFO` & `pytest_dogu_sdk-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-dogu-sdk
-Version: 1.0.0
+Version: 1.0.1
 Summary: pytest plugin for the Dogu
 Author: Dogu Technologies
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

