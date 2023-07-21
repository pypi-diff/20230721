# Comparing `tmp/nautobot_api_sandbox-0.1.3.tar.gz` & `tmp/nautobot_api_sandbox-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_api_sandbox-0.1.3.tar", max compression
+gzip compressed data, was "nautobot_api_sandbox-0.1.4.tar", max compression
```

## Comparing `nautobot_api_sandbox-0.1.3.tar` & `nautobot_api_sandbox-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1634 2023-07-20 20:47:13.069848 nautobot_api_sandbox-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-07-17 21:52:11.544627 nautobot_api_sandbox-0.1.3/nautobot_api_sandbox/__init__.py
--rwxr-xr-x   0        0        0     2778 2023-07-21 14:11:51.046126 nautobot_api_sandbox-0.1.3/nautobot_api_sandbox/click_ui.py
--rw-r--r--   0        0        0     4614 2023-07-21 13:52:14.735929 nautobot_api_sandbox-0.1.3/nautobot_api_sandbox/nauto_demo_functions.py
--rw-r--r--   0        0        0     4818 2023-07-21 13:50:14.785908 nautobot_api_sandbox-0.1.3/nautobot_api_sandbox/nautobot_api_sandbox_ui.py
--rw-r--r--   0        0        0      656 2023-07-21 14:17:19.036184 nautobot_api_sandbox-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2136 1970-01-01 00:00:00.000000 nautobot_api_sandbox-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1634 2023-07-21 16:44:03.837251 nautobot_api_sandbox-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-17 21:52:11.544627 nautobot_api_sandbox-0.1.4/nautobot_api_sandbox/__init__.py
+-rwxr-xr-x   0        0        0     2777 2023-07-21 14:30:03.225891 nautobot_api_sandbox-0.1.4/nautobot_api_sandbox/click_ui.py
+-rw-r--r--   0        0        0     4606 2023-07-21 14:30:03.225891 nautobot_api_sandbox-0.1.4/nautobot_api_sandbox/nauto_demo_functions.py
+-rw-r--r--   0        0        0     4800 2023-07-21 14:30:03.225891 nautobot_api_sandbox-0.1.4/nautobot_api_sandbox/nautobot_api_sandbox_ui.py
+-rw-r--r--   0        0        0      738 2023-07-21 16:45:28.557266 nautobot_api_sandbox-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2197 1970-01-01 00:00:00.000000 nautobot_api_sandbox-0.1.4/PKG-INFO
```

### Comparing `nautobot_api_sandbox-0.1.3/README.md` & `nautobot_api_sandbox-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nautobot_api_sandbox-0.1.3/nautobot_api_sandbox/click_ui.py` & `nautobot_api_sandbox-0.1.4/nautobot_api_sandbox/click_ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,17 +46,16 @@
         site_name = site_name.title()
 
     try:
         ctx.obj.display_devices(site_name)
     except SiteNotFoundError:
         logging.error(INVALID_SITE_MSG, site_name)
 
-cli.add_command(show_devices)
-
 
+cli.add_command(show_devices)
 
 
 @cli.command()
 @click.argument("tenant_name")
 @click.pass_context
 def create_tenant(ctx, tenant_name):
     tenant = ctx.obj.create_tenant(tenant_name)
```

### Comparing `nautobot_api_sandbox-0.1.3/nautobot_api_sandbox/nauto_demo_functions.py` & `nautobot_api_sandbox-0.1.4/nautobot_api_sandbox/nauto_demo_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class SiteNotFoundError(Exception):
     """Exception raised when a site is not found."""
 
 
 class DemoNautobotClient:
     """A client for interacting with Nautobot."""
-    
+
     DELETE_TENANT_DEPENDENT_OBJECTS_MSG = "Failed to delete tenant '%s'. It has dependent objects."
 
     def __init__(self, api_token, api=None):
         """Initialize the client with an API token and an optional pynautobot API object."""
         if api is None:
             self.api = pynautobot.api("https://demo.nautobot.com", token=api_token)
         else:
@@ -94,21 +94,19 @@
         tenant = self.get_tenant(name)
         if tenant is None:
             return False, self.TENANT_NOT_FOUND_ERROR_MSG % name
         try:
             tenant.delete()
             return True, "Tenant '%s' deleted successfully!" % name
         except pynautobot.core.query.RequestError as request_error:
-            if request_error.req.status_code == 409:  
+            if request_error.req.status_code == 409:
                 return False, self.DELETE_TENANT_DEPENDENT_OBJECTS_MSG % name
             else:
                 return False, self.DELETE_TENANT_ERROR_MSG % (name, str(request_error))
 
-
-
     def get_tenants(self):
         """Return a list of all tenants."""
         return self.api.tenancy.tenants.all()
 
     def display_tenants(self):
         """Display the names of all tenants."""
         tenants = self.get_tenants()
```

### Comparing `nautobot_api_sandbox-0.1.3/nautobot_api_sandbox/nautobot_api_sandbox_ui.py` & `nautobot_api_sandbox-0.1.4/nautobot_api_sandbox/nautobot_api_sandbox_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     # Commands that need an argument
     commands_with_arg = ["show_devices", "create_tenant", "delete_tenant", "get_tenant"]
 
     while True:
         command_input = input("Enter a command: ").split()
         command = command_input[0].lower()  # Convert command to lowercase
         arg = " ".join(command_input[1:])  # Join all items after the command with a space
-        
+
         if command == "exit":
             break
 
         if command == "create_tenant" or command == "delete_tenant" or command == "get_tenant":
             tenant_name = arg  # Store the tenant name without modifying capitalization
         else:
             # Process the argument based on its length
@@ -106,14 +106,12 @@
         elif command == "get_tenant":
             try:
                 nautobot_client.display_tenant(arg)
             except TenantNotFoundError:
                 logger.error(INVALID_TENANT_MSG, arg)
         elif command == "help":
             logger.info(WELCOME_MSG)
-        
-
 
 
 if __name__ == "__main__":
     logging.basicConfig(level=logging.INFO)
     user_interface()
```

### Comparing `nautobot_api_sandbox-0.1.3/pyproject.toml` & `nautobot_api_sandbox-0.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [tool.poetry]
 name = "nautobot_api_sandbox"
-version = "0.1.3"
+version = "0.1.4"
 description = "This is just a simple program to test my programing knowledge and to learn more about API and Nautobot."
 authors = ["tPayne0647"]
 readme = "README.md"
 packages = [{include = "nautobot_api_sandbox"}]
 
 [tool.poetry.scripts]
 nautobot_api_sandbox = "nautobot_api_sandbox.nautobot_api_sandbox_ui:user_interface"
 nauto_click = "nautobot_api_sandbox.click_ui:main"
+
 [tool.poetry.dependencies]
 python = "^3.9"
 pynautobot = "1.5.0"
+nautobot-api-sandbox-clickui = "^0.1.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 pytest = "7.4.0"
+nautobot-api-sandbox-clickui =  "^0.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nautobot_api_sandbox-0.1.3/PKG-INFO` & `nautobot_api_sandbox-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: nautobot-api-sandbox
-Version: 0.1.3
+Version: 0.1.4
 Summary: This is just a simple program to test my programing knowledge and to learn more about API and Nautobot.
 Author: tPayne0647
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: nautobot-api-sandbox-clickui (>=0.1.0,<0.2.0)
 Requires-Dist: pynautobot (==1.5.0)
 Description-Content-Type: text/markdown
 
 # Nautobot API Sandbox
 
 This is a simple program to test my programming knowledge and learn more about API, Nautobot, and developing in general.
```

