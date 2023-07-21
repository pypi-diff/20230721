# Comparing `tmp/nautobot_api_sandbox-0.1.5.tar.gz` & `tmp/nautobot_api_sandbox-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_api_sandbox-0.1.5.tar", max compression
+gzip compressed data, was "nautobot_api_sandbox-0.1.6.tar", max compression
```

## Comparing `nautobot_api_sandbox-0.1.5.tar` & `nautobot_api_sandbox-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1634 2023-07-21 16:44:03.837251 nautobot_api_sandbox-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-07-17 21:52:11.544627 nautobot_api_sandbox-0.1.5/nautobot_api_sandbox/__init__.py
--rwxr-xr-x   0        0        0     2777 2023-07-21 14:30:03.225891 nautobot_api_sandbox-0.1.5/nautobot_api_sandbox/click_ui.py
--rw-r--r--   0        0        0     4606 2023-07-21 14:30:03.225891 nautobot_api_sandbox-0.1.5/nautobot_api_sandbox/nauto_demo_functions.py
--rw-r--r--   0        0        0     4800 2023-07-21 14:30:03.225891 nautobot_api_sandbox-0.1.5/nautobot_api_sandbox/nautobot_api_sandbox_ui.py
--rw-r--r--   0        0        0      699 2023-07-21 16:48:52.857300 nautobot_api_sandbox-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2136 1970-01-01 00:00:00.000000 nautobot_api_sandbox-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     2350 2023-07-21 18:30:43.588331 nautobot_api_sandbox-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-17 21:52:11.544627 nautobot_api_sandbox-0.1.6/nautobot_api_sandbox/__init__.py
+-rwxr-xr-x   0        0        0     2745 2023-07-21 18:33:44.958363 nautobot_api_sandbox-0.1.6/nautobot_api_sandbox/click_ui.py
+-rw-r--r--   0        0        0     4737 2023-07-21 18:34:04.318366 nautobot_api_sandbox-0.1.6/nautobot_api_sandbox/nauto_demo_functions.py
+-rw-r--r--   0        0        0     4800 2023-07-21 18:29:40.698320 nautobot_api_sandbox-0.1.6/nautobot_api_sandbox/nautobot_api_sandbox_ui.py
+-rw-r--r--   0        0        0      658 2023-07-21 18:37:27.058399 nautobot_api_sandbox-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2852 1970-01-01 00:00:00.000000 nautobot_api_sandbox-0.1.6/PKG-INFO
```

### Comparing `nautobot_api_sandbox-0.1.5/nautobot_api_sandbox/click_ui.py` & `nautobot_api_sandbox-0.1.6/nautobot_api_sandbox/click_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,8 +97,8 @@
             logging.info("Tenant ID: %s\nTenant Name: %s", tenant.id, tenant.name)
     except TenantNotFoundError:
         logging.error(INVALID_TENANT_MSG, tenant_name)
 
 
 if __name__ == "__main__":
     logging.basicConfig(level=logging.INFO)
-    cli(obj={})  # Pass an empty context object
+    cli(obj={})
```

### Comparing `nautobot_api_sandbox-0.1.5/nautobot_api_sandbox/nauto_demo_functions.py` & `nautobot_api_sandbox-0.1.6/nautobot_api_sandbox/nauto_demo_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     """Exception raised when a site is not found."""
 
 
 class DemoNautobotClient:
     """A client for interacting with Nautobot."""
 
     DELETE_TENANT_DEPENDENT_OBJECTS_MSG = "Failed to delete tenant '%s'. It has dependent objects."
+    TENANT_NOT_FOUND_ERROR_MSG = "Tenant '%s' not found."
+    DELETE_TENANT_ERROR_MSG = "Failed to delete tenant '%s'. Error: %s."
 
     def __init__(self, api_token, api=None):
         """Initialize the client with an API token and an optional pynautobot API object."""
         if api is None:
             self.api = pynautobot.api("https://demo.nautobot.com", token=api_token)
         else:
             self.api = api
```

### Comparing `nautobot_api_sandbox-0.1.5/nautobot_api_sandbox/nautobot_api_sandbox_ui.py` & `nautobot_api_sandbox-0.1.6/nautobot_api_sandbox/nautobot_api_sandbox_ui.py`

 * *Files identical despite different names*

### Comparing `nautobot_api_sandbox-0.1.5/pyproject.toml` & `nautobot_api_sandbox-0.1.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot_api_sandbox"
-version = "0.1.5"
+version = "0.1.6"
 description = "This is just a simple program to test my programing knowledge and to learn more about API and Nautobot."
 authors = ["tPayne0647"]
 readme = "README.md"
 packages = [{include = "nautobot_api_sandbox"}]
 
 [tool.poetry.scripts]
 nautobot_api_sandbox = "nautobot_api_sandbox.nautobot_api_sandbox_ui:user_interface"
@@ -14,12 +14,11 @@
 python = "^3.9"
 pynautobot = "1.5.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 pytest = "7.4.0"
-nautobot-api-sandbox-clickui =  "^0.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

