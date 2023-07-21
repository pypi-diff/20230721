# Comparing `tmp/nautobot_api_sandbox-0.1.2.tar.gz` & `tmp/nautobot_api_sandbox-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_api_sandbox-0.1.2.tar", max compression
+gzip compressed data, was "nautobot_api_sandbox-0.1.3.tar", max compression
```

## Comparing `nautobot_api_sandbox-0.1.2.tar` & `nautobot_api_sandbox-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1634 2023-07-20 20:47:13.069848 nautobot_api_sandbox-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-07-17 21:52:11.544627 nautobot_api_sandbox-0.1.2/nautobot_api_sandbox/__init__.py
--rwxr-xr-x   0        0        0     2429 2023-07-20 20:46:46.869843 nautobot_api_sandbox-0.1.2/nautobot_api_sandbox/click_ui.py
--rw-r--r--   0        0        0     4439 2023-07-20 20:46:46.869843 nautobot_api_sandbox-0.1.2/nautobot_api_sandbox/nauto_demo_functions.py
--rw-r--r--   0        0        0     4600 2023-07-20 20:46:46.869843 nautobot_api_sandbox-0.1.2/nautobot_api_sandbox/nautobot_api_sandbox_ui.py
--rw-r--r--   0        0        0      656 2023-07-20 20:48:28.399861 nautobot_api_sandbox-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2136 1970-01-01 00:00:00.000000 nautobot_api_sandbox-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1634 2023-07-20 20:47:13.069848 nautobot_api_sandbox-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-17 21:52:11.544627 nautobot_api_sandbox-0.1.3/nautobot_api_sandbox/__init__.py
+-rwxr-xr-x   0        0        0     2778 2023-07-21 14:11:51.046126 nautobot_api_sandbox-0.1.3/nautobot_api_sandbox/click_ui.py
+-rw-r--r--   0        0        0     4614 2023-07-21 13:52:14.735929 nautobot_api_sandbox-0.1.3/nautobot_api_sandbox/nauto_demo_functions.py
+-rw-r--r--   0        0        0     4818 2023-07-21 13:50:14.785908 nautobot_api_sandbox-0.1.3/nautobot_api_sandbox/nautobot_api_sandbox_ui.py
+-rw-r--r--   0        0        0      656 2023-07-21 14:17:19.036184 nautobot_api_sandbox-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2136 1970-01-01 00:00:00.000000 nautobot_api_sandbox-0.1.3/PKG-INFO
```

### Comparing `nautobot_api_sandbox-0.1.2/README.md` & `nautobot_api_sandbox-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nautobot_api_sandbox-0.1.2/nautobot_api_sandbox/click_ui.py` & `nautobot_api_sandbox-0.1.3/nautobot_api_sandbox/click_ui.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 import logging
 import click
 from pynautobot.core.query import RequestError
+from nautobot_api_sandbox_ui import (
+    INVALID_SITE_MSG,
+    INVALID_TENANT_MSG,
+    TOKEN_ERROR_MSG,
+    COMMAND_ARG_ERROR_MSG,
+    TENANT_CREATED_SUCCESS_MSG,
+    TENANT_EXISTS_ERROR_MSG,
+)
 from nautobot_api_sandbox.nauto_demo_functions import (
     DemoNautobotClient,
     TenantNotFoundError,
     SiteNotFoundError,
 )
 
 
@@ -12,62 +20,70 @@
 @click.pass_context
 def cli(ctx):
     api_token = click.prompt("Please enter your API token. HINT-check readme...", type=str)
     try:
         ctx.obj = DemoNautobotClient(api_token=api_token)
         ctx.obj.api.dcim.sites.all()  # Make a simple request to check if the token is valid
     except RequestError:
-        logging.error("Invalid API token. Please try again.")
+        logging.error(TOKEN_ERROR_MSG)
         ctx.exit()
 
 
 @cli.command()
 @click.pass_context
 def show_sites(ctx):
     ctx.obj.display_sites()
 
 
-@cli.command()
+@click.command()
 @click.argument("site_name")
 @click.pass_context
 def show_devices(ctx, site_name):
+    # Capitalize if the site_name is less than 5 characters
+    if len(site_name) <= 5:
+        site_name = site_name.upper()
+    # Convert to title case if the site_name is more than one word
+    elif " " in site_name:
+        site_name = site_name.title()
+
     try:
         ctx.obj.display_devices(site_name)
     except SiteNotFoundError:
-        logging.error("Site %s not found. Please enter a valid site name.", site_name)
+        logging.error(INVALID_SITE_MSG, site_name)
+
+cli.add_command(show_devices)
+
+
 
 
 @cli.command()
 @click.argument("tenant_name")
 @click.pass_context
 def create_tenant(ctx, tenant_name):
     tenant = ctx.obj.create_tenant(tenant_name)
     if tenant is None:
-        logging.error("A tenant with the name '%s' already exists.", tenant_name)
+        logging.error(TENANT_EXISTS_ERROR_MSG, tenant_name)
     else:
-        logging.info("Tenant '%s' created successfully.", tenant_name)
+        logging.info(TENANT_CREATED_SUCCESS_MSG, tenant_name)
 
 
-@click.command()
+@cli.command()
 @click.argument("tenant_name")
 @click.pass_context
 def delete_tenant(ctx, tenant_name):
     try:
         result = ctx.obj.delete_tenant(tenant_name)
         if result is not None:  # if result is None, it means an error has occurred
             success, message = result
             if success:
                 logging.info(message)
             else:
                 logging.error(message)
     except TenantNotFoundError as e:
-        logging.error(str(e))
-
-
-cli.add_command(delete_tenant)
+        logging.error(INVALID_TENANT_MSG, tenant_name)
 
 
 @cli.command()
 @click.pass_context
 def show_tenants(ctx):
     ctx.obj.display_tenants()
 
@@ -77,13 +93,13 @@
 @click.pass_context
 def get_tenant(ctx, tenant_name):
     try:
         tenant = ctx.obj.get_tenant(tenant_name)
         if tenant is not None:
             logging.info("Tenant ID: %s\nTenant Name: %s", tenant.id, tenant.name)
     except TenantNotFoundError:
-        logging.error("Tenant '%s' not found. Please enter a valid tenant name.", tenant_name)
+        logging.error(INVALID_TENANT_MSG, tenant_name)
 
 
 if __name__ == "__main__":
     logging.basicConfig(level=logging.INFO)
     cli(obj={})  # Pass an empty context object
```

### Comparing `nautobot_api_sandbox-0.1.2/nautobot_api_sandbox/nauto_demo_functions.py` & `nautobot_api_sandbox-0.1.3/nautobot_api_sandbox/nauto_demo_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 class SiteNotFoundError(Exception):
     """Exception raised when a site is not found."""
 
 
 class DemoNautobotClient:
     """A client for interacting with Nautobot."""
+    
+    DELETE_TENANT_DEPENDENT_OBJECTS_MSG = "Failed to delete tenant '%s'. It has dependent objects."
 
     def __init__(self, api_token, api=None):
         """Initialize the client with an API token and an optional pynautobot API object."""
         if api is None:
             self.api = pynautobot.api("https://demo.nautobot.com", token=api_token)
         else:
             self.api = api
@@ -35,23 +37,20 @@
     def display_sites(self):
         """Display the names of all sites."""
         sites = self.get_sites()
         self.logger.info("\nTotal sites: %s\n \n%s", len(sites), [site.name for site in sites])
 
     def get_devices(self, selected_site_name):
         """Return a list of all devices at the specified site, or raise SiteNotFoundError if the site does not exist."""
-        try:
-            # First, get the site by name
-            site = self.api.dcim.sites.get(name=selected_site_name)
-            if site is None:
-                raise SiteNotFoundError("Site '%s' not found." % selected_site_name)
-            # Then, get the devices for the site using the slug
-            devices = self.api.dcim.devices.filter(site=site.slug)
-        except RequestError as request_error:
-            raise request_error
+        # First, get the site by name
+        site = self.api.dcim.sites.get(name=selected_site_name)
+        if site is None:
+            raise SiteNotFoundError("Site '%s' not found." % selected_site_name)
+        # Then, get the devices for the site using the slug
+        devices = self.api.dcim.devices.filter(site=site.slug)
         return devices
 
     def display_devices(self, selected_site):
         """Display the names of all devices at the specified site."""
         try:
             devices = self.get_devices(selected_site)
             self.logger.info(
@@ -82,28 +81,33 @@
             raise TenantNotFoundError("Tenant with name '%s' not found." % name)
         return tenant
 
     def display_tenant(self, name):
         """Display the ID and name of the tenant with the specified name."""
         try:
             tenant = self.get_tenant(name)
-            self.logger.info("Tenant ID: %s\nTenant Name: %s", tenant.id, tenant.name)
+            self.logger.info("\nTenant ID: %s\nTenant Name: %s", tenant.id, tenant.name)
         except TenantNotFoundError:
             self.logger.error("Tenant '%s' not found. Please enter a valid tenant name.", name)
 
     def delete_tenant(self, name):
         """Delete the tenant with the specified name."""
+        tenant = self.get_tenant(name)
+        if tenant is None:
+            return False, self.TENANT_NOT_FOUND_ERROR_MSG % name
         try:
-            tenant = self.get_tenant(name)
             tenant.delete()
             return True, "Tenant '%s' deleted successfully!" % name
-        except TenantNotFoundError:
-            raise
         except pynautobot.core.query.RequestError as request_error:
-            return False, "Failed to delete tenant '%s'. Error: %s" % (name, request_error)
+            if request_error.req.status_code == 409:  
+                return False, self.DELETE_TENANT_DEPENDENT_OBJECTS_MSG % name
+            else:
+                return False, self.DELETE_TENANT_ERROR_MSG % (name, str(request_error))
+
+
 
     def get_tenants(self):
         """Return a list of all tenants."""
         return self.api.tenancy.tenants.all()
 
     def display_tenants(self):
         """Display the names of all tenants."""
```

### Comparing `nautobot_api_sandbox-0.1.2/nautobot_api_sandbox/nautobot_api_sandbox_ui.py` & `nautobot_api_sandbox-0.1.3/nautobot_api_sandbox/nautobot_api_sandbox_ui.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,92 +18,102 @@
 get_tenant [TENANT NAME]...............Get specified tenant
 delete_tenant [TENANT NAME]............Delete specified tenant
 show_tenants...........................Get count and list all tenant names
 help...................................Reprint this window
 ********************************************************************************
 """
 
+INVALID_SITE_MSG = "Site %s not found. Please enter a valid site name."
+INVALID_TENANT_MSG = "Tenant '%s' not found. Please enter a valid tenant name."
+TOKEN_ERROR_MSG = "Invalid API token. Please try again."
+COMMAND_ARG_ERROR_MSG = "The %s command requires an argument."
+TENANT_EXISTS_ERROR_MSG = "A tenant with the name '%s' already exists."
+TENANT_CREATED_SUCCESS_MSG = "Tenant '%s' created successfully."
+
 
 def user_interface():
     # Set up logging
     logger = logging.getLogger(__name__)
     logger.addHandler(logging.StreamHandler())  # Outputs log messages to the console
     logger.setLevel(logging.INFO)  # Set the desired log level
+    logger.propagate = False  # Prevents the logger from passing messages to the root logger
 
     # Ask for API token
     while True:
         api_token = input(
             "Please enter your API token. HINT-check readme...(or type 'exit' to quit): "
         )
         if api_token.lower() == "exit":
             return
         try:
             nautobot_client = DemoNautobotClient(api_token=api_token)
             nautobot_client.api.dcim.sites.all()  # Make a simple request to check if the token is valid
             break
         except RequestError:
-            logger.error("Invalid API token. Please try again.")
+            logger.error(TOKEN_ERROR_MSG)
 
     logger.info(WELCOME_MSG)  # Use logger.info instead of print
 
     # Commands that need an argument
     commands_with_arg = ["show_devices", "create_tenant", "delete_tenant", "get_tenant"]
 
     while True:
         command_input = input("Enter a command: ").split()
         command = command_input[0].lower()  # Convert command to lowercase
         arg = " ".join(command_input[1:])  # Join all items after the command with a space
+        
+        if command == "exit":
+            break
 
         if command == "create_tenant" or command == "delete_tenant" or command == "get_tenant":
             tenant_name = arg  # Store the tenant name without modifying capitalization
         else:
             # Process the argument based on its length
             if len(arg) <= 5:
                 arg = arg.upper()  # Convert to uppercase if length is 5 or less
             else:
                 arg = arg.title()  # Convert to title case if more than one word
 
         # Check if the command needs an argument and if it was provided
         if command in commands_with_arg and not arg:
-            logger.error("The %s command requires an argument.", command)
+            logger.error(COMMAND_ARG_ERROR_MSG, command)
             continue
 
         if command == "show_sites":
             nautobot_client.display_sites()
         elif command == "show_devices":
             try:
                 nautobot_client.display_devices(arg)
             except SiteNotFoundError:
-                logger.error("Site %s not found. Please enter a valid site name.", arg)
+                logger.error(INVALID_SITE_MSG, arg)
         elif command == "create_tenant":
             tenant = nautobot_client.create_tenant(tenant_name)
             if tenant is None:
-                logger.error("A tenant with the name '%s' already exists.", tenant_name)
+                logger.error(TENANT_EXISTS_ERROR_MSG, tenant_name)
             else:
-                logger.info("Tenant '%s' created successfully.", tenant_name)
+                logger.info(TENANT_CREATED_SUCCESS_MSG, tenant_name)
         elif command == "delete_tenant":
             try:
                 success, message = nautobot_client.delete_tenant(arg)
                 if success:
                     logger.info(message)
                 else:
                     logger.error(message)
-            except TenantNotFoundError as e:
-                logger.error(str(e))
+            except TenantNotFoundError:
+                logger.error("Tenant with name '%s' not found.", arg)
+
         elif command == "show_tenants":
             nautobot_client.display_tenants()
         elif command == "get_tenant":
             try:
-                nautobot_client.display_tenant(arg)  # Use the display_tenant method
+                nautobot_client.display_tenant(arg)
             except TenantNotFoundError:
-                logger.error("Tenant '%s' not found. Please enter a valid tenant name.", arg)
+                logger.error(INVALID_TENANT_MSG, arg)
         elif command == "help":
-            logger.info(WELCOME_MSG)  # Use logger.info instead of print
-        elif command == "exit":
-            break
-        else:
-            logger.error("Unrecognized command. Type 'help' to see the list of available commands.")
+            logger.info(WELCOME_MSG)
+        
+
 
 
 if __name__ == "__main__":
     logging.basicConfig(level=logging.INFO)
     user_interface()
```

### Comparing `nautobot_api_sandbox-0.1.2/pyproject.toml` & `nautobot_api_sandbox-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot_api_sandbox"
-version = "0.1.2"
+version = "0.1.3"
 description = "This is just a simple program to test my programing knowledge and to learn more about API and Nautobot."
 authors = ["tPayne0647"]
 readme = "README.md"
 packages = [{include = "nautobot_api_sandbox"}]
 
 [tool.poetry.scripts]
 nautobot_api_sandbox = "nautobot_api_sandbox.nautobot_api_sandbox_ui:user_interface"
```

### Comparing `nautobot_api_sandbox-0.1.2/PKG-INFO` & `nautobot_api_sandbox-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautobot-api-sandbox
-Version: 0.1.2
+Version: 0.1.3
 Summary: This is just a simple program to test my programing knowledge and to learn more about API and Nautobot.
 Author: tPayne0647
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

