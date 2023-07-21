# Comparing `tmp/promptquality-0.2.1.tar.gz` & `tmp/promptquality-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptquality-0.2.1.tar", max compression
+gzip compressed data, was "promptquality-0.2.2.tar", max compression
```

## Comparing `promptquality-0.2.1.tar` & `promptquality-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    10946 2023-07-21 00:13:07.454901 promptquality-0.2.1/LICENSE
--rw-r--r--   0        0        0      157 2023-07-21 00:13:07.454901 promptquality-0.2.1/README.md
--rw-r--r--   0        0        0     1543 2023-07-21 00:13:07.454901 promptquality-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      398 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/constants/__init__.py
--rw-r--r--   0        0        0      353 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/constants/config.py
--rw-r--r--   0        0        0       80 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/constants/integrations.py
--rw-r--r--   0        0        0      172 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/constants/job.py
--rw-r--r--   0        0        0      618 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/constants/routes.py
--rw-r--r--   0        0        0      150 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/constants/run.py
--rw-r--r--   0        0        0     1840 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/get_metrics.py
--rw-r--r--   0        0        0     4588 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/helpers.py
--rw-r--r--   0        0        0      543 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/integrations.py
--rw-r--r--   0        0        0     1060 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/job_progress.py
--rw-r--r--   0        0        0      466 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/login.py
--rw-r--r--   0        0        0     1603 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/run.py
--rw-r--r--   0        0        0     1019 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/set_config.py
--rw-r--r--   0        0        0        0 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/types/__init__.py
--rw-r--r--   0        0        0     7781 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/types/config.py
--rw-r--r--   0        0        0     3619 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/types/run.py
--rw-r--r--   0        0        0      474 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/types/settings.py
--rw-r--r--   0        0        0        0 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/utils/__init__.py
--rw-r--r--   0        0        0     4460 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/utils/api_client.py
--rw-r--r--   0        0        0      838 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/utils/config.py
--rw-r--r--   0        0        0       60 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/utils/logger.py
--rw-r--r--   0        0        0    24261 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/utils/name.py
--rw-r--r--   0        0        0     1625 2023-07-21 00:13:07.458901 promptquality-0.2.1/src/promptquality/utils/request.py
--rw-r--r--   0        0        0      845 1970-01-01 00:00:00.000000 promptquality-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    10946 2023-07-21 21:05:56.084023 promptquality-0.2.2/LICENSE
+-rw-r--r--   0        0        0      157 2023-07-21 21:05:56.084023 promptquality-0.2.2/README.md
+-rw-r--r--   0        0        0     1543 2023-07-21 21:05:56.088023 promptquality-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      398 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/constants/__init__.py
+-rw-r--r--   0        0        0      353 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/constants/config.py
+-rw-r--r--   0        0        0       80 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/constants/integrations.py
+-rw-r--r--   0        0        0      172 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/constants/job.py
+-rw-r--r--   0        0        0      618 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/constants/routes.py
+-rw-r--r--   0        0        0      150 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/constants/run.py
+-rw-r--r--   0        0        0     1840 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/get_metrics.py
+-rw-r--r--   0        0        0     4588 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/helpers.py
+-rw-r--r--   0        0        0      543 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/integrations.py
+-rw-r--r--   0        0        0     1060 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/job_progress.py
+-rw-r--r--   0        0        0      466 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/login.py
+-rw-r--r--   0        0        0     1603 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/run.py
+-rw-r--r--   0        0        0     1019 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/set_config.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/types/__init__.py
+-rw-r--r--   0        0        0     7781 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/types/config.py
+-rw-r--r--   0        0        0     3619 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/types/run.py
+-rw-r--r--   0        0        0      474 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/types/settings.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/utils/__init__.py
+-rw-r--r--   0        0        0     4460 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/utils/api_client.py
+-rw-r--r--   0        0        0      838 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/utils/config.py
+-rw-r--r--   0        0        0       60 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/utils/logger.py
+-rw-r--r--   0        0        0    24261 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/utils/name.py
+-rw-r--r--   0        0        0     1625 2023-07-21 21:05:56.088023 promptquality-0.2.2/src/promptquality/utils/request.py
+-rw-r--r--   0        0        0      845 1970-01-01 00:00:00.000000 promptquality-0.2.2/PKG-INFO
```

### Comparing `promptquality-0.2.1/LICENSE` & `promptquality-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.1/pyproject.toml` & `promptquality-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "promptquality"
-version = "0.2.1"
+version = "0.2.2"
 description = "🦸 Supercharge your prompts with Galileo's Prompt Inspector!"
 authors = ["Galileo Technologies Inc. <team@rungalileo.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.12"
 requests = "^2.31.0"
```

### Comparing `promptquality-0.2.1/src/promptquality/constants/routes.py` & `promptquality-0.2.2/src/promptquality/constants/routes.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.1/src/promptquality/get_metrics.py` & `promptquality-0.2.2/src/promptquality/get_metrics.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.1/src/promptquality/helpers.py` & `promptquality-0.2.2/src/promptquality/helpers.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.1/src/promptquality/integrations.py` & `promptquality-0.2.2/src/promptquality/integrations.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.1/src/promptquality/job_progress.py` & `promptquality-0.2.2/src/promptquality/job_progress.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.1/src/promptquality/run.py` & `promptquality-0.2.2/src/promptquality/run.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.1/src/promptquality/set_config.py` & `promptquality-0.2.2/src/promptquality/set_config.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.1/src/promptquality/types/config.py` & `promptquality-0.2.2/src/promptquality/types/config.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.1/src/promptquality/types/run.py` & `promptquality-0.2.2/src/promptquality/types/run.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.1/src/promptquality/utils/api_client.py` & `promptquality-0.2.2/src/promptquality/utils/api_client.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.1/src/promptquality/utils/config.py` & `promptquality-0.2.2/src/promptquality/utils/config.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.1/src/promptquality/utils/name.py` & `promptquality-0.2.2/src/promptquality/utils/name.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.1/src/promptquality/utils/request.py` & `promptquality-0.2.2/src/promptquality/utils/request.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.1/PKG-INFO` & `promptquality-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptquality
-Version: 0.2.1
+Version: 0.2.2
 Summary: 🦸 Supercharge your prompts with Galileo's Prompt Inspector!
 Author: Galileo Technologies Inc.
 Author-email: team@rungalileo.io
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

