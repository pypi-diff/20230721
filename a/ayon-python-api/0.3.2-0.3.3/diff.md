# Comparing `tmp/ayon-python-api-0.3.2.tar.gz` & `tmp/ayon-python-api-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayon-python-api-0.3.2.tar", last modified: Wed Jul  5 12:10:01 2023, max compression
+gzip compressed data, was "ayon-python-api-0.3.3.tar", last modified: Fri Jul 21 13:39:19 2023, max compression
```

## Comparing `ayon-python-api-0.3.2.tar` & `ayon-python-api-0.3.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:10:01.621467 ayon-python-api-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-07-05 12:10:01.621467 ayon-python-api-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:10:01.621467 ayon-python-api-0.3.2/ayon_api/
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30325 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    59757 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/entity_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25639 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)    15583 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/graphql_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)   188014 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/server_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/ayon_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:10:01.621467 ayon-python-api-0.3.2/ayon_python_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-07-05 12:10:01.000000 ayon-python-api-0.3.2/ayon_python_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-05 12:10:01.000000 ayon-python-api-0.3.2/ayon_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 12:10:01.000000 ayon-python-api-0.3.2/ayon_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 12:10:01.000000 ayon-python-api-0.3.2/ayon_python_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 12:10:01.000000 ayon-python-api-0.3.2/ayon_python_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 12:10:01.621467 ayon-python-api-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-05 12:09:55.000000 ayon-python-api-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:39:19.025102 ayon-python-api-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-07-21 13:39:19.025102 ayon-python-api-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:39:19.025102 ayon-python-api-0.3.3/ayon_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30310 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59757 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/entity_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25639 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15583 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/graphql_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192441 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/server_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15078 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/ayon_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:39:19.025102 ayon-python-api-0.3.3/ayon_python_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-07-21 13:39:19.000000 ayon-python-api-0.3.3/ayon_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-21 13:39:19.000000 ayon-python-api-0.3.3/ayon_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:39:19.000000 ayon-python-api-0.3.3/ayon_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-21 13:39:19.000000 ayon-python-api-0.3.3/ayon_python_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 13:39:19.000000 ayon-python-api-0.3.3/ayon_python_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 13:39:19.025102 ayon-python-api-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-21 13:39:12.000000 ayon-python-api-0.3.3/setup.py
```

### Comparing `ayon-python-api-0.3.2/LICENSE` & `ayon-python-api-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.2/PKG-INFO` & `ayon-python-api-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayon-python-api
-Version: 0.3.2
+Version: 0.3.3
 Summary: AYON Python API
 Home-page: https://github.com/ynput/ayon-python-api
 Author: ynput.io
 Author-email: "ynput.io" <info@ynput.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ayon-python-api-0.3.2/README.md` & `ayon-python-api-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.2/ayon_api/__init__.py` & `ayon-python-api-0.3.3/ayon_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,16 @@
     create_dependency_package,
     update_dependency_package,
     delete_dependency_package,
 
     download_dependency_package,
     upload_dependency_package,
 
+    upload_addon_zip,
+
     get_bundles,
     create_bundle,
     update_bundle,
     delete_bundle,
 
     get_info,
     get_server_version,
@@ -258,14 +260,16 @@
     "create_dependency_package",
     "update_dependency_package",
     "delete_dependency_package",
 
     "download_dependency_package",
     "upload_dependency_package",
 
+    "upload_addon_zip",
+
     "get_bundles",
     "create_bundle",
     "update_bundle",
     "delete_bundle",
 
     "get_info",
     "get_server_version",
```

### Comparing `ayon-python-api-0.3.2/ayon_api/_api.py` & `ayon-python-api-0.3.3/ayon_api/_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,20 +21,37 @@
     """Extended server api which also handles storing tokens and url.
 
     Created object expect to have set environment variables
     'AYON_SERVER_URL'. Also is expecting filled 'AYON_API_KEY'
     but that can be filled afterwards with calling 'login' method.
     """
 
-    def __init__(self, site_id=None, client_version=None):
+    def __init__(
+        self,
+        site_id=None,
+        client_version=None,
+        default_settings_variant=None,
+        ssl_verify=None,
+        cert=None,
+    ):
         url = self.get_url()
         token = self.get_token()
 
-        super(GlobalServerAPI, self).__init__(url, token, site_id, client_version)
-
+        super(GlobalServerAPI, self).__init__(
+            url,
+            token,
+            site_id,
+            client_version,
+            default_settings_variant,
+            ssl_verify,
+            cert,
+            # We want to make sure that server and api key validation
+            #   happens all the time in 'GlobalServerAPI'.
+            create_session=False,
+        )
         self.validate_server_availability()
         self.create_session()
 
     def login(self, username, password):
         """Login to the server or change user.
 
         If user is the same as current user and token is available the
@@ -125,63 +142,37 @@
 
     token = None
     server_url = None
     addon_name = None
     addon_version = None
     service_name = None
 
-    @staticmethod
-    def get_value_from_envs(env_keys, value=None):
-        if value:
-            return value
-
-        for env_key in env_keys:
-            value = os.environ.get(env_key)
-            if value:
-                break
-        return value
-
     @classmethod
     def init_service(
         cls,
         token=None,
         server_url=None,
         addon_name=None,
         addon_version=None,
         service_name=None,
         connect=True
     ):
-        token = cls.get_value_from_envs(
-            ("AY_API_KEY", "AYON_API_KEY"),
-            token
-        )
-        server_url = cls.get_value_from_envs(
-            ("AY_SERVER_URL", "AYON_SERVER_URL"),
-            server_url
-        )
+        token = token or os.environ.get("AYON_API_KEY")
+        server_url = server_url or os.environ.get("AYON_SERVER_URL")
         if not server_url:
             raise FailedServiceInit("URL to server is not set")
 
         if not token:
             raise FailedServiceInit(
                 "Token to server {} is not set".format(server_url)
             )
 
-        addon_name = cls.get_value_from_envs(
-            ("AY_ADDON_NAME", "AYON_ADDON_NAME"),
-            addon_name
-        )
-        addon_version = cls.get_value_from_envs(
-            ("AY_ADDON_VERSION", "AYON_ADDON_VERSION"),
-            addon_version
-        )
-        service_name = cls.get_value_from_envs(
-            ("AY_SERVICE_NAME", "AYON_SERVICE_NAME"),
-            service_name
-        )
+        addon_name = addon_name or os.environ.get("AYON_ADDON_NAME")
+        addon_version = addon_version or os.environ.get("AYON_ADDON_VERSION")
+        service_name = service_name or os.environ.get("AYON_SERVICE_NAME")
 
         cls.token = token
         cls.server_url = server_url
         cls.addon_name = addon_name
         cls.addon_version = addon_version
         cls.service_name = service_name or socket.gethostname()
 
@@ -614,14 +605,19 @@
 
 
 def delete_dependency_package(*args, **kwargs):
     con = get_server_api_connection()
     return con.delete_dependency_package(*args, **kwargs)
 
 
+def upload_addon_zip(*args, **kwargs):
+    con = get_server_api_connection()
+    return con.upload_addon_zip(*args, **kwargs)
+
+
 def get_project_anatomy_presets(*args, **kwargs):
     con = get_server_api_connection()
     return con.get_project_anatomy_presets(*args, **kwargs)
 
 
 def get_bundles(*args, **kwargs):
     con = get_server_api_connection()
```

### Comparing `ayon-python-api-0.3.2/ayon_api/constants.py` & `ayon-python-api-0.3.3/ayon_api/constants.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.2/ayon_api/entity_hub.py` & `ayon-python-api-0.3.3/ayon_api/entity_hub.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.2/ayon_api/events.py` & `ayon-python-api-0.3.3/ayon_api/events.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.2/ayon_api/exceptions.py` & `ayon-python-api-0.3.3/ayon_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.2/ayon_api/graphql.py` & `ayon-python-api-0.3.3/ayon_api/graphql.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.2/ayon_api/graphql_queries.py` & `ayon-python-api-0.3.3/ayon_api/graphql_queries.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.2/ayon_api/operations.py` & `ayon-python-api-0.3.3/ayon_api/operations.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.2/ayon_api/server_api.py` & `ayon-python-api-0.3.3/ayon_api/server_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import re
 import io
 import json
 import logging
 import collections
-import datetime
 import platform
 import copy
 import uuid
 from contextlib import contextmanager
 try:
     from http import HTTPStatus
 except ImportError:
@@ -321,25 +320,28 @@
             Settings variant used by default if a method for settings won't
             get any (by default is 'production').
         ssl_verify (Union[bool, str, None]): Verify SSL certificate
             Looks for env variable value 'AYON_CA_FILE' by default. If not
             available then 'True' is used.
         cert (Optional[str]): Path to certificate file. Looks for env
             variable value 'AYON_CERT_FILE' by default.
+        create_session (Optional[bool]): Create session for connection if
+            token is available. Default is True.
     """
 
     def __init__(
         self,
         base_url,
         token=None,
         site_id=None,
         client_version=None,
         default_settings_variant=None,
         ssl_verify=None,
         cert=None,
+        create_session=True,
     ):
         if not base_url:
             raise ValueError("Invalid server URL {}".format(str(base_url)))
 
         base_url = base_url.rstrip("/")
         self._base_url = base_url
         self._rest_url = "{}/api".format(base_url)
@@ -363,14 +365,15 @@
             cert = os.environ.get("AYON_CERT_FILE")
 
         self._ssl_verify = ssl_verify
         self._cert = cert
 
         self._access_token_is_service = None
         self._token_is_valid = None
+        self._token_validation_started = False
         self._server_available = None
         self._server_version = None
         self._server_version_tuple = None
 
         self._session = None
 
         self._base_functions_mapping = {
@@ -385,14 +388,19 @@
         # Attributes cache
         self._attributes_schema = None
         self._entity_type_attributes_cache = {}
 
         self._as_user_stack = _AsUserStack()
         self._thumbnail_cache = ThumbnailCache(True)
 
+        # Create session
+        if self._access_token and create_session:
+            self.validate_server_availability()
+            self.create_session()
+
     @property
     def log(self):
         if self._log is None:
             self._log = logging.getLogger(self.__class__.__name__)
         return self._log
 
     def get_base_url(self):
@@ -648,37 +656,58 @@
         if not self.is_server_available:
             raise ServerNotReached("Server \"{}\" can't be reached".format(
                 self._base_url
             ))
 
     def validate_token(self):
         try:
+            self._token_validation_started = True
             # TODO add other possible validations
             # - existence of 'user' key in info
             # - validate that 'site_id' is in 'sites' in info
             self.get_info()
             self.get_user()
             self._token_is_valid = True
 
         except UnauthorizedError:
             self._token_is_valid = False
+
+        finally:
+            self._token_validation_started = False
         return self._token_is_valid
 
     def set_token(self, token):
         self.reset_token()
         self._access_token = token
         self.get_user()
 
     def reset_token(self):
         self._access_token = None
         self._token_is_valid = None
         self.close_session()
 
-    def create_session(self):
+    def create_session(self, ignore_existing=True, force=False):
+        """Create a connection session.
+
+        Session helps to keep connection with server without
+            need to reconnect on each call.
+
+        Args:
+            ignore_existing (bool): If session already exists,
+                ignore creation.
+            force (bool): If session already exists, close it and
+                create new.
+        """
+
+        if force and self._session is not None:
+            self.close_session()
+
         if self._session is not None:
+            if ignore_existing:
+                return
             raise ValueError("Session is already created.")
 
         self._as_user_stack.clear()
         # Validate token before session creation
         self.validate_token()
 
         session = requests.Session()
@@ -837,25 +866,38 @@
                 if username:
                     headers["X-as-user"] = username
             else:
                 headers["Authorization"] = "Bearer {}".format(
                     self._access_token)
         return headers
 
-    def login(self, username, password):
+    def login(self, username, password, create_session=True):
+        """Login to server.
+
+        Args:
+            username (str): Username.
+            password (str): Password.
+            create_session (Optional[bool]): Create session after login.
+                Default: True.
+
+        Raises:
+            AuthenticationError: Login failed.
+        """
+
         if self.has_valid_token:
             try:
                 user_info = self.get_user()
             except UnauthorizedError:
                 user_info = {}
 
             current_username = user_info.get("name")
             if current_username == username:
                 self.close_session()
-                self.create_session()
+                if create_session:
+                    self.create_session()
                 return
 
         self.reset_token()
 
         self.validate_server_availability()
 
         response = self.post(
@@ -871,27 +913,38 @@
 
             raise AuthenticationError("Login failed {}".format(details))
 
         self._access_token = response["token"]
 
         if not self.has_valid_token:
             raise AuthenticationError("Invalid credentials")
-        self.create_session()
+
+        if create_session:
+            self.create_session()
 
     def logout(self, soft=False):
         if self._access_token:
             if not soft:
                 self._logout()
             self.reset_token()
 
     def _logout(self):
         logout_from_server(self._base_url, self._access_token)
 
     def _do_rest_request(self, function, url, **kwargs):
         if self._session is None:
+            # Validate token if was not yet validated
+            #    - ignore validation if we're in middle of
+            #       validation
+            if (
+                self._token_is_valid is None
+                and not self._token_validation_started
+            ):
+                self.validate_token()
+
             if "headers" not in kwargs:
                 kwargs["headers"] = self.get_headers()
 
             if isinstance(function, RequestType):
                 function = self._base_functions_mapping[function]
 
         elif isinstance(function, RequestType):
@@ -1324,14 +1377,15 @@
             stream.seek(0, io.SEEK_END)
             size = stream.tell()
             stream.seek(0)
             progress.set_content_size(size)
             response = post_func(url, data=stream, **kwargs)
         response.raise_for_status()
         progress.set_transferred_size(size)
+        return response
 
     def upload_file(
         self, endpoint, filepath, progress=None, request_type=None
     ):
         """Upload file to server.
 
         Todos:
@@ -1340,14 +1394,17 @@
         Args:
             endpoint (str): Endpoint or url where file will be uploaded.
             filepath (str): Source filepath.
             progress (Optional[TransferProgress]): Object that gives ability
                 to track upload progress.
             request_type (Optional[RequestType]): Type of request that will
                 be used to upload file.
+
+        Returns:
+            requests.Response: Response object.
         """
 
         if endpoint.startswith(self._base_url):
             url = endpoint
         else:
             endpoint = endpoint.lstrip("/").rstrip("/")
             url = "{}/{}".format(self._rest_url, endpoint)
@@ -1358,15 +1415,15 @@
             progress = TransferProgress()
 
         progress.set_source_url(filepath)
         progress.set_destination_url(url)
         progress.set_started()
 
         try:
-            self._upload_file(url, filepath, progress, request_type)
+            return self._upload_file(url, filepath, progress, request_type)
 
         except Exception as exc:
             progress.set_failed(str(exc))
             raise
 
         finally:
             progress.set_transfer_done()
@@ -1636,15 +1693,15 @@
             >>> api.get_addon_url(
             ...     "example", "1.0.0", "private", "my.zip")
             'https://your.url.com/addons/example/1.0.0/private/my.zip'
 
         Args:
             addon_name (str): Name of addon.
             addon_version (str): Version of addon.
-            subpaths (tuple[str]): Any amount of subpaths that are added to
+            *subpaths (str): Any amount of subpaths that are added to
                 addon url.
 
         Returns:
             str: Final url.
         """
 
         ending = ""
@@ -1844,17 +1901,20 @@
         """Upload installer file to server.
 
         Args:
             src_filepath (str): Source filepath.
             dst_filename (str): Destination filename.
             progress (Optional[TransferProgress]): Object that gives ability
                 to track download progress.
+
+        Returns:
+            requests.Response: Response object.
         """
 
-        self.upload_file(
+        return self.upload_file(
             "desktop/installers/{}".format(dst_filename),
             src_filepath,
             progress=progress
         )
 
     def get_dependencies_info(self):
         """Information about dependency packages on server.
@@ -2158,14 +2218,41 @@
 
         Returns:
             str: Dependency package name with timestamp and platform.
         """
 
         return create_dependency_package_basename(platform_name)
 
+    def upload_addon_zip(self, src_filepath, progress=None):
+        """Upload addon zip file to server.
+
+        File is validated on server. If it is valid, it is installed. It will
+            create an event job which can be tracked (tracking part is not
+            implemented yet).
+
+        Example output:
+            {'eventId': 'a1bfbdee27c611eea7580242ac120003'}
+
+        Args:
+            src_filepath (str): Path to a zip file.
+            progress (Optional[TransferProgress]): Object to keep track about
+                upload state.
+
+        Returns:
+            dict[str, Any]: Response data from server.
+        """
+
+        response = self.upload_file(
+            "addons/install",
+            src_filepath,
+            progress=progress,
+            request_type=RequestTypes.post,
+        )
+        return response.json()
+
     def _get_bundles_route(self):
         major, minor, patch, _, _ = self.server_version_tuple
         # Backwards compatibility for AYON server 0.3.0
         # - first version where bundles were available
         if major == 0 and minor == 3 and patch == 0:
             return "desktop/bundles"
         return "bundles"
@@ -3047,14 +3134,73 @@
         project = parsed_data["project"]
         if project is not None:
             project["name"] = project_name
             if own_attributes:
                 fill_own_attribs(project)
         return project
 
+    def get_folders_hierarchy(
+        self,
+        project_name,
+        search_string=None,
+        folder_types=None
+    ):
+        """Get project hierarchy.
+
+        All folders in project in hierarchy data structure.
+
+        Example output:
+            {
+                "hierarchy": [
+                    {
+                        "id": "...",
+                        "name": "...",
+                        "label": "...",
+                        "status": "...",
+                        "folderType": "...",
+                        "hasTasks": False,
+                        "taskNames": [],
+                        "parents": [],
+                        "parentId": None,
+                        "children": [...children folders...]
+                    },
+                    ...
+                ]
+            }
+
+        Args:
+            project_name (str): Project where to look for folders.
+            search_string (Optional[str]): Search string to filter folders.
+            folder_types (Optional[Iterable[str]]): Folder types to filter.
+
+        Returns:
+            dict[str, Any]: Response data from server.
+        """
+
+        if folder_types:
+            folder_types = ",".join(folder_types)
+
+        query_fields = [
+            "{}={}".format(key, value)
+            for key, value in (
+                ("search", search_string),
+                ("types", folder_types),
+            )
+            if value
+        ]
+        query = ""
+        if query_fields:
+            query = "?{}".format(",".join(query_fields))
+
+        response = self.get(
+            "projects/{}/hierarchy{}".format(project_name, query)
+        )
+        response.raise_for_status()
+        return response.data
+
     def get_folders(
         self,
         project_name,
         folder_ids=None,
         folder_paths=None,
         folder_names=None,
         parent_ids=None,
@@ -3618,15 +3764,14 @@
             for product in products:
                 filtered_product = self._filter_product(
                     project_name, product, active, own_attributes, use_rest
                 )
                 if filtered_product is not None:
                     yield filtered_product
 
-
     def get_product_by_id(
         self,
         project_name,
         product_id,
         fields=None,
         own_attributes=False
     ):
```

### Comparing `ayon-python-api-0.3.2/ayon_api/thumbnails.py` & `ayon-python-api-0.3.3/ayon_api/thumbnails.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.2/ayon_python_api.egg-info/PKG-INFO` & `ayon-python-api-0.3.3/ayon_python_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayon-python-api
-Version: 0.3.2
+Version: 0.3.3
 Summary: AYON Python API
 Home-page: https://github.com/ynput/ayon-python-api
 Author: ynput.io
 Author-email: "ynput.io" <info@ynput.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ayon-python-api-0.3.2/ayon_python_api.egg-info/SOURCES.txt` & `ayon-python-api-0.3.3/ayon_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.2/pyproject.toml` & `ayon-python-api-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ayon-python-api"
-version = "0.3.2"
+version = "0.3.3"
 description = "AYON Python API"
 license = {file = "LICENSE"}
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [
     {name = "ynput.io", email = "info@ynput.io"}
 ]
 keywords = ["AYON", "ynput", "OpenPype", "vfx"]
```

### Comparing `ayon-python-api-0.3.2/setup.py` & `ayon-python-api-0.3.3/setup.py`

 * *Files identical despite different names*

