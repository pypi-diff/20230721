# Comparing `tmp/nautobot_api_sandbox-0.1.4.tar.gz` & `tmp/nautobot_api_sandbox-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_api_sandbox-0.1.4.tar", max compression
+gzip compressed data, was "nautobot_api_sandbox-0.1.5.tar", max compression
```

## Comparing `nautobot_api_sandbox-0.1.4.tar` & `nautobot_api_sandbox-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1634 2023-07-21 16:44:03.837251 nautobot_api_sandbox-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-07-17 21:52:11.544627 nautobot_api_sandbox-0.1.4/nautobot_api_sandbox/__init__.py
--rwxr-xr-x   0        0        0     2777 2023-07-21 14:30:03.225891 nautobot_api_sandbox-0.1.4/nautobot_api_sandbox/click_ui.py
--rw-r--r--   0        0        0     4606 2023-07-21 14:30:03.225891 nautobot_api_sandbox-0.1.4/nautobot_api_sandbox/nauto_demo_functions.py
--rw-r--r--   0        0        0     4800 2023-07-21 14:30:03.225891 nautobot_api_sandbox-0.1.4/nautobot_api_sandbox/nautobot_api_sandbox_ui.py
--rw-r--r--   0        0        0      738 2023-07-21 16:45:28.557266 nautobot_api_sandbox-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2197 1970-01-01 00:00:00.000000 nautobot_api_sandbox-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1634 2023-07-21 16:44:03.837251 nautobot_api_sandbox-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-07-17 21:52:11.544627 nautobot_api_sandbox-0.1.5/nautobot_api_sandbox/__init__.py
+-rwxr-xr-x   0        0        0     2777 2023-07-21 14:30:03.225891 nautobot_api_sandbox-0.1.5/nautobot_api_sandbox/click_ui.py
+-rw-r--r--   0        0        0     4606 2023-07-21 14:30:03.225891 nautobot_api_sandbox-0.1.5/nautobot_api_sandbox/nauto_demo_functions.py
+-rw-r--r--   0        0        0     4800 2023-07-21 14:30:03.225891 nautobot_api_sandbox-0.1.5/nautobot_api_sandbox/nautobot_api_sandbox_ui.py
+-rw-r--r--   0        0        0      699 2023-07-21 16:48:52.857300 nautobot_api_sandbox-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2136 1970-01-01 00:00:00.000000 nautobot_api_sandbox-0.1.5/PKG-INFO
```

### Comparing `nautobot_api_sandbox-0.1.4/README.md` & `nautobot_api_sandbox-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nautobot_api_sandbox-0.1.4/nautobot_api_sandbox/click_ui.py` & `nautobot_api_sandbox-0.1.5/nautobot_api_sandbox/click_ui.py`

 * *Files identical despite different names*

### Comparing `nautobot_api_sandbox-0.1.4/nautobot_api_sandbox/nauto_demo_functions.py` & `nautobot_api_sandbox-0.1.5/nautobot_api_sandbox/nauto_demo_functions.py`

 * *Files identical despite different names*

### Comparing `nautobot_api_sandbox-0.1.4/nautobot_api_sandbox/nautobot_api_sandbox_ui.py` & `nautobot_api_sandbox-0.1.5/nautobot_api_sandbox/nautobot_api_sandbox_ui.py`

 * *Files identical despite different names*

### Comparing `nautobot_api_sandbox-0.1.4/pyproject.toml` & `nautobot_api_sandbox-0.1.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "nautobot_api_sandbox"
-version = "0.1.4"
+version = "0.1.5"
 description = "This is just a simple program to test my programing knowledge and to learn more about API and Nautobot."
 authors = ["tPayne0647"]
 readme = "README.md"
 packages = [{include = "nautobot_api_sandbox"}]
 
 [tool.poetry.scripts]
 nautobot_api_sandbox = "nautobot_api_sandbox.nautobot_api_sandbox_ui:user_interface"
 nauto_click = "nautobot_api_sandbox.click_ui:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pynautobot = "1.5.0"
-nautobot-api-sandbox-clickui = "^0.1.0"
+
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 pytest = "7.4.0"
 nautobot-api-sandbox-clickui =  "^0.1.0"
 
 [build-system]
```

### Comparing `nautobot_api_sandbox-0.1.4/PKG-INFO` & `nautobot_api_sandbox-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: nautobot-api-sandbox
-Version: 0.1.4
+Version: 0.1.5
 Summary: This is just a simple program to test my programing knowledge and to learn more about API and Nautobot.
 Author: tPayne0647
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: nautobot-api-sandbox-clickui (>=0.1.0,<0.2.0)
 Requires-Dist: pynautobot (==1.5.0)
 Description-Content-Type: text/markdown
 
 # Nautobot API Sandbox
 
 This is a simple program to test my programming knowledge and learn more about API, Nautobot, and developing in general.
```

