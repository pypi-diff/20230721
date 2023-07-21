# Comparing `tmp/computex_cli-0.1.6.tar.gz` & `tmp/computex_cli-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computex_cli-0.1.6.tar", max compression
+gzip compressed data, was "computex_cli-0.1.7.tar", max compression
```

## Comparing `computex_cli-0.1.6.tar` & `computex_cli-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1233 2023-07-21 20:12:11.066659 computex_cli-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-07-21 20:12:11.066659 computex_cli-0.1.6/cxcli/__init__.py
--rw-r--r--   0        0        0     8944 2023-07-21 20:12:11.066659 computex_cli-0.1.6/cxcli/cli.py
--rw-r--r--   0        0        0      911 2023-07-21 20:12:11.066659 computex_cli-0.1.6/cxcli/config.py
--rw-r--r--   0        0        0      161 2023-07-21 20:12:11.066659 computex_cli-0.1.6/cxcli/exc.py
--rw-r--r--   0        0        0        0 2023-07-21 20:12:11.066659 computex_cli-0.1.6/cxcli/services/__init__.py
--rw-r--r--   0        0        0      950 2023-07-21 20:12:11.066659 computex_cli-0.1.6/cxcli/services/auth.py
--rw-r--r--   0        0        0     3065 2023-07-21 20:12:11.066659 computex_cli-0.1.6/cxcli/services/deployments.py
--rw-r--r--   0        0        0     1912 2023-07-21 20:12:11.066659 computex_cli-0.1.6/cxcli/services/service.py
--rw-r--r--   0        0        0     1236 2023-07-21 20:12:11.066659 computex_cli-0.1.6/cxcli/services/users.py
--rw-r--r--   0        0        0      744 2023-07-21 20:12:11.070659 computex_cli-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1974 1970-01-01 00:00:00.000000 computex_cli-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1233 2023-07-21 20:22:34.791518 computex_cli-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 20:22:34.791518 computex_cli-0.1.7/cxcli/__init__.py
+-rw-r--r--   0        0        0     8944 2023-07-21 20:22:34.791518 computex_cli-0.1.7/cxcli/cli.py
+-rw-r--r--   0        0        0      911 2023-07-21 20:22:34.791518 computex_cli-0.1.7/cxcli/config.py
+-rw-r--r--   0        0        0      161 2023-07-21 20:22:34.791518 computex_cli-0.1.7/cxcli/exc.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:22:34.791518 computex_cli-0.1.7/cxcli/services/__init__.py
+-rw-r--r--   0        0        0      950 2023-07-21 20:22:34.791518 computex_cli-0.1.7/cxcli/services/auth.py
+-rw-r--r--   0        0        0     3065 2023-07-21 20:22:34.791518 computex_cli-0.1.7/cxcli/services/deployments.py
+-rw-r--r--   0        0        0     1912 2023-07-21 20:22:34.791518 computex_cli-0.1.7/cxcli/services/service.py
+-rw-r--r--   0        0        0     1236 2023-07-21 20:22:34.791518 computex_cli-0.1.7/cxcli/services/users.py
+-rw-r--r--   0        0        0      773 2023-07-21 20:22:34.791518 computex_cli-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1974 1970-01-01 00:00:00.000000 computex_cli-0.1.7/PKG-INFO
```

### Comparing `computex_cli-0.1.6/README.md` & `computex_cli-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.6/cxcli/cli.py` & `computex_cli-0.1.7/cxcli/cli.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.6/cxcli/config.py` & `computex_cli-0.1.7/cxcli/config.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.6/cxcli/services/auth.py` & `computex_cli-0.1.7/cxcli/services/auth.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.6/cxcli/services/deployments.py` & `computex_cli-0.1.7/cxcli/services/deployments.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.6/cxcli/services/service.py` & `computex_cli-0.1.7/cxcli/services/service.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.6/cxcli/services/users.py` & `computex_cli-0.1.7/cxcli/services/users.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.6/pyproject.toml` & `computex_cli-0.1.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "computex-cli"
-version = "0.1.6"
+version = "0.1.7"
 description = "ComputeX CLI tool"
 authors = ["Abate De Mey <abate@computex.ai>"]
 readme = "README.md"
 packages = [{include = "cxcli"}]
+include = ["pyproject.toml"]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 click = "^8.1.3"
 requests = "^2.31.0"
 pydantic = "^1.10.9"
 python-dotenv = "^1.0.0"
```

### Comparing `computex_cli-0.1.6/PKG-INFO` & `computex_cli-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computex-cli
-Version: 0.1.6
+Version: 0.1.7
 Summary: ComputeX CLI tool
 Author: Abate De Mey
 Author-email: abate@computex.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

