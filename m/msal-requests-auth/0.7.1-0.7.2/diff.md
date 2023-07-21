# Comparing `tmp/msal_requests_auth-0.7.1.tar.gz` & `tmp/msal_requests_auth-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msal_requests_auth-0.7.1.tar", last modified: Fri Jul 14 14:46:49 2023, max compression
+gzip compressed data, was "msal_requests_auth-0.7.2.tar", last modified: Fri Jul 21 20:53:11 2023, max compression
```

## Comparing `msal_requests_auth-0.7.1.tar` & `msal_requests_auth-0.7.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:46:49.572959 msal_requests_auth-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-14 14:46:49.572959 msal_requests_auth-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:46:49.572959 msal_requests_auth-0.7.1/msal_requests_auth/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/msal_requests_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/msal_requests_auth/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:46:49.572959 msal_requests_auth-0.7.1/msal_requests_auth/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/msal_requests_auth/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/msal_requests_auth/auth/base_auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/msal_requests_auth/auth/client_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/msal_requests_auth/auth/device_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/msal_requests_auth/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/msal_requests_auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/msal_requests_auth/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:46:49.572959 msal_requests_auth-0.7.1/msal_requests_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-14 14:46:49.000000 msal_requests_auth-0.7.1/msal_requests_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-14 14:46:49.000000 msal_requests_auth-0.7.1/msal_requests_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:46:49.000000 msal_requests_auth-0.7.1/msal_requests_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:46:49.000000 msal_requests_auth-0.7.1/msal_requests_auth.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-14 14:46:49.000000 msal_requests_auth-0.7.1/msal_requests_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 14:46:49.000000 msal_requests_auth-0.7.1/msal_requests_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-14 14:46:49.572959 msal_requests_auth-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:46:49.572959 msal_requests_auth-0.7.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/test/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/test/test_client_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-07-14 14:46:32.000000 msal_requests_auth-0.7.1/test/test_devide_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:53:11.145313 msal_requests_auth-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-21 20:52:51.000000 msal_requests_auth-0.7.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-21 20:52:51.000000 msal_requests_auth-0.7.2/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-21 20:52:51.000000 msal_requests_auth-0.7.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-21 20:52:51.000000 msal_requests_auth-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-21 20:52:51.000000 msal_requests_auth-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-21 20:53:11.145313 msal_requests_auth-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-21 20:52:51.000000 msal_requests_auth-0.7.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:53:11.141313 msal_requests_auth-0.7.2/msal_requests_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-21 20:52:51.000000 msal_requests_auth-0.7.2/msal_requests_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 20:52:51.000000 msal_requests_auth-0.7.2/msal_requests_auth/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:53:11.145313 msal_requests_auth-0.7.2/msal_requests_auth/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-21 20:52:51.000000 msal_requests_auth-0.7.2/msal_requests_auth/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-21 20:52:51.000000 msal_requests_auth-0.7.2/msal_requests_auth/auth/base_auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-21 20:52:51.000000 msal_requests_auth-0.7.2/msal_requests_auth/auth/client_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-21 20:52:51.000000 msal_requests_auth-0.7.2/msal_requests_auth/auth/device_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-21 20:52:51.000000 msal_requests_auth-0.7.2/msal_requests_auth/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-21 20:52:51.000000 msal_requests_auth-0.7.2/msal_requests_auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:52:51.000000 msal_requests_auth-0.7.2/msal_requests_auth/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:53:11.145313 msal_requests_auth-0.7.2/msal_requests_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-21 20:53:11.000000 msal_requests_auth-0.7.2/msal_requests_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-21 20:53:11.000000 msal_requests_auth-0.7.2/msal_requests_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:53:11.000000 msal_requests_auth-0.7.2/msal_requests_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:53:10.000000 msal_requests_auth-0.7.2/msal_requests_auth.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-21 20:53:11.000000 msal_requests_auth-0.7.2/msal_requests_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 20:53:11.000000 msal_requests_auth-0.7.2/msal_requests_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-21 20:53:11.149313 msal_requests_auth-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 20:52:51.000000 msal_requests_auth-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:53:11.145313 msal_requests_auth-0.7.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-21 20:52:51.000000 msal_requests_auth-0.7.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-21 20:52:51.000000 msal_requests_auth-0.7.2/test/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-21 20:52:51.000000 msal_requests_auth-0.7.2/test/test_client_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-07-21 20:52:51.000000 msal_requests_auth-0.7.2/test/test_devide_code.py
```

### Comparing `msal_requests_auth-0.7.1/AUTHORS.rst` & `msal_requests_auth-0.7.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.7.1/CODE_OF_CONDUCT.rst` & `msal_requests_auth-0.7.2/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.7.1/CONTRIBUTING.rst` & `msal_requests_auth-0.7.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.7.1/LICENSE` & `msal_requests_auth-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.7.1/PKG-INFO` & `msal_requests_auth-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msal_requests_auth
-Version: 0.7.1
+Version: 0.7.2
 Summary: Authentication using python requests and MSAL
 Home-page: https://github.com/corteva/msal-requests-auth
 Download-URL: http://python.org/pypi/msal-requests-auth
 Author: msal_requests_auth Contributors
 Author-email: alansnow21@gmail.com
 License: BSD License
 Keywords: msal,requests
```

### Comparing `msal_requests_auth-0.7.1/README.rst` & `msal_requests_auth-0.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.7.1/msal_requests_auth/auth/base_auth_client.py` & `msal_requests_auth-0.7.2/msal_requests_auth/auth/base_auth_client.py`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.7.1/msal_requests_auth/auth/client_credential.py` & `msal_requests_auth-0.7.2/msal_requests_auth/auth/client_credential.py`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.7.1/msal_requests_auth/auth/device_code.py` & `msal_requests_auth-0.7.2/msal_requests_auth/auth/device_code.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Module for handling the Device Code flow with MSAL and credential refresh.
 """
 import os
+import warnings
 import webbrowser
 from typing import Dict, List, Optional
 
 import pyperclip
 from msal import PublicClientApplication
 
 from .base_auth_client import BaseMSALRefreshAuth
@@ -63,10 +64,19 @@
         # "No suitable token exists in cache. Get a new one from AAD
         flow = self.client.initiate_device_flow(
             scopes=self.scopes,
         )
         print(flow["message"])
         if not self._headless:
             # copy code to clipboard
-            pyperclip.copy(flow["user_code"])
-            webbrowser.open(flow["verification_uri"])
+            try:
+                pyperclip.copy(flow["user_code"])
+                webbrowser.open(flow["verification_uri"])
+            except Exception as error:  # pylint: disable=broad-exception-caught
+                warnings.warn(
+                    "Error encountered while copying code to clipboard "
+                    f"and opening a webbrowser ({error})."
+                    "To hide this message, set headless=True "
+                    "or set the MSAL_REQUESTS_AUTH_HEADLESS "
+                    "environment variable to 'true'."
+                )
         return self.client.acquire_token_by_device_flow(flow)
```

### Comparing `msal_requests_auth-0.7.1/msal_requests_auth/cache.py` & `msal_requests_auth-0.7.2/msal_requests_auth/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,14 @@
     @abstractmethod
     def write_cache(self) -> None:
         """
         Write cache if needed.
         """
         raise NotImplementedError
 
-    def __del__(self):
-        self.write_cache()
-
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.write_cache()
```

### Comparing `msal_requests_auth-0.7.1/msal_requests_auth.egg-info/PKG-INFO` & `msal_requests_auth-0.7.2/msal_requests_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msal-requests-auth
-Version: 0.7.1
+Version: 0.7.2
 Summary: Authentication using python requests and MSAL
 Home-page: https://github.com/corteva/msal-requests-auth
 Download-URL: http://python.org/pypi/msal-requests-auth
 Author: msal_requests_auth Contributors
 Author-email: alansnow21@gmail.com
 License: BSD License
 Keywords: msal,requests
```

### Comparing `msal_requests_auth-0.7.1/msal_requests_auth.egg-info/SOURCES.txt` & `msal_requests_auth-0.7.2/msal_requests_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.7.1/setup.cfg` & `msal_requests_auth-0.7.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.7.1/test/test_cache.py` & `msal_requests_auth-0.7.2/test/test_cache.py`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.7.1/test/test_client_credential.py` & `msal_requests_auth-0.7.2/test/test_client_credential.py`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.7.1/test/test_devide_code.py` & `msal_requests_auth-0.7.2/test/test_devide_code.py`

 * *Files 8% similar despite different names*

```diff
@@ -164,7 +164,49 @@
     )
     pca_mock.initiate_device_flow.assert_not_called()
     pca_mock.acquire_token_by_device_flow.assert_not_called()
 
     assert returned_request.headers == {"Authorization": "Bearer TEST TOKEN"}
     webbrowser_patch.open.assert_not_called()
     pyperclip_patch.copy.assert_not_called()
+
+
+@patch.dict(os.environ, {}, clear=True)
+@patch("msal.PublicClientApplication", autospec=True)
+@patch("msal_requests_auth.auth.device_code.webbrowser")
+@patch("msal_requests_auth.auth.device_code.pyperclip")
+def test_device_code_auth__pyperclip_error(pyperclip_patch, webbrowser_patch, pca_mock):
+    pyperclip_patch.copy.side_effect = AttributeError
+    pca_mock.get_accounts.return_value = None
+    pca_mock.initiate_device_flow.return_value = {
+        "message": "TEST MESSAGE",
+        "verification_uri": "TEST URL",
+        "user_code": "TEST CODE",
+    }
+    pca_mock.acquire_token_by_device_flow.return_value = {
+        "token_type": "Bearer",
+        "access_token": "TEST TOKEN",
+    }
+    request_mock = MagicMock()
+    request_mock.headers = {}
+    with pytest.warns(
+        UserWarning,
+        match="Error encountered while copying code to clipboard and opening a webbrowser.",
+    ):
+        returned_request = DeviceCodeAuth(client=pca_mock, scopes=["TEST SCOPE"])(
+            request_mock
+        )
+
+    pca_mock.acquire_token_silent.assert_not_called()
+    pca_mock.initiate_device_flow.assert_called_with(scopes=["TEST SCOPE"])
+    pca_mock.acquire_token_by_device_flow.assert_called_with(
+        {
+            "message": "TEST MESSAGE",
+            "verification_uri": "TEST URL",
+            "user_code": "TEST CODE",
+        }
+    )
+
+    assert returned_request.headers == {"Authorization": "Bearer TEST TOKEN"}
+
+    pyperclip_patch.copy.assert_called_with("TEST CODE")
+    webbrowser_patch.open.assert_not_called()
```

