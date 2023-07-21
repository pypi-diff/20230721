# Comparing `tmp/antigranular-0.2.4.tar.gz` & `tmp/antigranular-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antigranular-0.2.4.tar", max compression
+gzip compressed data, was "antigranular-0.2.5.tar", max compression
```

## Comparing `antigranular-0.2.4.tar` & `antigranular-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      548 2023-07-19 22:04:49.517587 antigranular-0.2.4/antigranular/__init__.py
--rw-r--r--   0        0        0    11769 2023-07-19 22:09:15.601536 antigranular-0.2.4/antigranular/client.py
--rw-r--r--   0        0        0      907 2023-07-19 22:04:49.526049 antigranular-0.2.4/antigranular/config/config.py
--rw-r--r--   0        0        0     3025 2023-07-19 22:04:49.534071 antigranular-0.2.4/antigranular/enclave_client/mock_client.py
--rw-r--r--   0        0        0      802 2023-07-19 22:09:15.601536 antigranular-0.2.4/antigranular/enclave_client/oblv_client.py
--rw-r--r--   0        0        0     1053 2023-07-19 22:04:49.542507 antigranular-0.2.4/antigranular/magics/errors.py
--rw-r--r--   0        0        0     6659 2023-07-19 22:04:49.553085 antigranular-0.2.4/antigranular/magics/magics.py
--rw-r--r--   0        0        0        0 2023-07-19 22:04:49.553085 antigranular-0.2.4/antigranular/models/__init__.py
--rw-r--r--   0        0        0      661 2023-07-19 22:04:49.558996 antigranular-0.2.4/antigranular/models/models.py
--rw-r--r--   0        0        0      149 2023-07-19 22:04:49.567029 antigranular-0.2.4/antigranular/utils/error_print.py
--rw-r--r--   0        0        0    11558 2023-07-19 22:04:49.493587 antigranular-0.2.4/LICENSE
--rw-r--r--   0        0        0      759 2023-07-19 22:18:41.342555 antigranular-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     4252 2023-07-19 22:09:25.273745 antigranular-0.2.4/README.md
--rw-r--r--   0        0        0     5073 1970-01-01 00:00:00.000000 antigranular-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      548 2023-07-21 08:47:55.609083 antigranular-0.2.5/antigranular/__init__.py
+-rw-r--r--   0        0        0    11997 2023-07-21 08:48:08.808429 antigranular-0.2.5/antigranular/client.py
+-rw-r--r--   0        0        0      907 2023-07-21 08:47:55.624630 antigranular-0.2.5/antigranular/config/config.py
+-rw-r--r--   0        0        0     3025 2023-07-21 08:47:55.624630 antigranular-0.2.5/antigranular/enclave_client/mock_client.py
+-rw-r--r--   0        0        0      802 2023-07-21 08:48:08.816432 antigranular-0.2.5/antigranular/enclave_client/oblv_client.py
+-rw-r--r--   0        0        0     1053 2023-07-21 08:47:55.624630 antigranular-0.2.5/antigranular/magics/errors.py
+-rw-r--r--   0        0        0     6781 2023-07-21 08:48:08.816432 antigranular-0.2.5/antigranular/magics/magics.py
+-rw-r--r--   0        0        0        0 2023-07-21 08:47:55.624630 antigranular-0.2.5/antigranular/models/__init__.py
+-rw-r--r--   0        0        0      661 2023-07-21 08:47:55.624630 antigranular-0.2.5/antigranular/models/models.py
+-rw-r--r--   0        0        0      149 2023-07-21 08:47:55.640185 antigranular-0.2.5/antigranular/utils/error_print.py
+-rw-r--r--   0        0        0      304 2023-07-21 08:48:08.816432 antigranular-0.2.5/antigranular/utils/print_request_id.py
+-rw-r--r--   0        0        0    11558 2023-07-21 08:47:55.593316 antigranular-0.2.5/LICENSE
+-rw-r--r--   0        0        0      759 2023-07-21 08:49:12.248263 antigranular-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     4252 2023-07-21 08:48:08.808429 antigranular-0.2.5/README.md
+-rw-r--r--   0        0        0     5073 1970-01-01 00:00:00.000000 antigranular-0.2.5/PKG-INFO
```

### Comparing `antigranular-0.2.4/antigranular/__init__.py` & `antigranular-0.2.5/antigranular/__init__.py`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.4/antigranular/client.py` & `antigranular-0.2.5/antigranular/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from typing import Union
 import warnings
 import pandas as pd
 from .magics.magics import AGMagic
 from .enclave_client.oblv_client import get_oblv_client, oblv_client
 from .config import config
 from .models.models import AGServerInfo
-
+from .utils.print_request_id import print_request_id
 
 def login(
     user_id: str,
     user_secret: str,
     competition: str = None,
     dataset: str = None,
 ):
@@ -75,15 +75,15 @@
             warnings.warn(f"Error while validating server info: {str(err)}")
 
         self.oblv_enclave = get_oblv_client(ag_client_id, ag_client_secret)
         self.headers = {}
 
         # Create an AG session
         self.connect(competition=competition, dataset=dataset)
-        print(f"Connected to Antigranular server session id: {str(self.session_id)}")
+        print(f"Connected to Antigranular server session id: {str(self.session_id)}, the session will time out if idle for 60 minutes")
 
         try:
             res = AGMagic.load_ag_magic()
         except Exception as ex:
             print(
                 "Error loading %%ag magic functions, you might not be able to use cell magics as intended: ",
                 str(ex),
@@ -153,15 +153,15 @@
                     json={"session_type": "dataset", "type_identifier": dataset},
                 )
         except Exception as err:
             raise ConnectionError(f"Error calling /start-session: {str(err)}")
         else:
             if res.status_code != 200:
                 raise requests.exceptions.HTTPError(
-                    f"Error while starting a new session in enclave status code: {res.status_code} message: {res.text}"
+                    print_request_id(f"Error while starting a new session in enclave status code: {res.status_code} message: {res.text}", res)
                 )
             self.session_id = json.loads(res.text)["session_id"]
 
 
     def interrupt_kernel(self) -> dict:
         """
         Interrupt the current session.
@@ -181,15 +181,15 @@
                 json={"session_id": self.session_id},
             )
         except Exception as e:
             raise ConnectionError(f"Error calling /terminate-session: {str(e)}")
         else:
             if res.status_code != 200:
                 raise requests.exceptions.HTTPError(
-                    f"Error while fetching the terminate-session, HTTP status code: {res.status_code}, message: {res.text}"
+                    print_request_id(f"Error while fetching the terminate-session, HTTP status code: {res.status_code}, message: {res.text}", res)
                 )
             return json.loads(res.text)
 
     def terminate_session(self) -> dict:
         """
         Terminate the current session.
 
@@ -208,15 +208,15 @@
                 json={"session_id": self.session_id},
             )
         except Exception as e:
             raise ConnectionError(f"Error calling /terminate-session: {str(e)}")
         else:
             if res.status_code != 200:
                 raise requests.exceptions.HTTPError(
-                    f"Error while fetching the terminate-session, HTTP status code: {res.status_code}, message: {res.text}"
+                    print_request_id(f"Error while fetching the terminate-session, HTTP status code: {res.status_code}, message: {res.text}", res)
                 )
             return json.loads(res.text)
 
     def privacy_odometer(self) -> dict:
         """
         Get the privacy odometer.
 
@@ -235,15 +235,15 @@
                 headers=self.headers,
             )
         except Exception as e:
             raise ConnectionError(f"Error calling /privacy_odometer: {str(e)}")
         else:
             if res.status_code != 200:
                 raise requests.exceptions.HTTPError(
-                    f"Error while fetching the privacy odometer, HTTP status code: {res.status_code}, message: {res.text}"
+                    print_request_id(f"Error while fetching the privacy odometer, HTTP status code: {res.status_code}, message: {res.text}", res)
                 )
             return json.loads(res.text)
 
     def submit_predictions(self, data) -> dict:
         """
         Submit predictions to the AG server.
 
@@ -261,17 +261,17 @@
                 headers=self.headers,
             )
         except Exception as e:
             raise ConnectionError(f"Error calling /submit_predictions: {str(e)}")
         else:
             if res.status_code != 200:
                 if res.status_code == 500:
-                    return json.loads(res.text)
+                    return print_request_id(res.text, res)
                 raise requests.exceptions.HTTPError(
-                    f"Error: {res.text}"
+                    print_request_id(f"Error: {res.text}", res)
                 )
             return json.loads(res.text)
 
     # Use Oblv Client enclave to make HTTP requests
     def _exec(self, method, endpoint, data="", json={}, params={}, headers={}):
         """
         Execute an HTTP request using the Oblv Client enclave.
```

### Comparing `antigranular-0.2.4/antigranular/config/config.py` & `antigranular-0.2.5/antigranular/config/config.py`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.4/antigranular/enclave_client/mock_client.py` & `antigranular-0.2.5/antigranular/enclave_client/mock_client.py`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.4/antigranular/enclave_client/oblv_client.py` & `antigranular-0.2.5/antigranular/enclave_client/oblv_client.py`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.4/antigranular/magics/errors.py` & `antigranular-0.2.5/antigranular/magics/errors.py`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.4/antigranular/magics/magics.py` & `antigranular-0.2.5/antigranular/magics/magics.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from requests import HTTPError
 
 from ..enclave_client.mock_client import MockEnclaveClient
 from ..enclave_client.oblv_client import oblv_client
 from ..utils.error_print import eprint
 from .errors import AGRuntimeError, AGTimeOutError
 from ..config import config
-
+from ..utils.print_request_id import print_request_id
 
 @magics_class
 class AGMagic(Magics):
     """
     Provides %%ag cell magic and private python code execution on Antigranular server
     """
 
@@ -80,15 +80,15 @@
                 json={"session_id": self.session_id, "code": code},
             )
         except Exception as err:
             raise ConnectionError(f"Error calling /execute: {str(err)}")
         else:
             if res.status_code != 200:
                 raise HTTPError(
-                    f"Error while requesting AG server to execute the code, HTTP status code: {res.status_code}, message: {res.text}"
+                    print_request_id(f"Error while requesting AG server to execute the code, HTTP status code: {res.status_code}, message: {res.text}", res)
                 )
             self.get_output()
 
     def interrupt_kernel(self) -> dict:
         try:
             res = self.ag_server.post(
                 f"{self.ag_server.url}:{self.ag_server.port}/sessions/interrupt-kernel",
@@ -97,15 +97,15 @@
         except Exception as err:
             raise ConnectionError(
                 f"Error calling /sessions/interrupt-kernel: {str(err)}"
             )
         else:
             if res.status_code != 200:
                 raise HTTPError(
-                    f"Error while requesting AG server to interrupt the kernel, HTTP status code: {res.status_code}, message: {res.text}"
+                    print_request_id(f"Error while requesting AG server to interrupt the kernel, HTTP status code: {res.status_code}, message: {res.text}", res)
                 )
             return json.loads(res.text)
 
     def get_output(self):
         """
         Retrieves the code execution output from the Antigranular server.
         """
@@ -122,15 +122,15 @@
                 )
             except Exception as err:
                 raise ConnectionError(
                     f"Error during code execution on AG Server: {str(err)}"
                 )
             if res.status_code != 200:
                 raise HTTPError(
-                    f"Error while requesting AG server for output, HTTP status code: {res.status_code}, message: {res.text}"
+                    print_request_id(f"Error while requesting AG server for output, HTTP status code: {res.status_code}, message: {res.text}", res)
                 )
             kernel_messages = json.loads(res.text)["output_list"]
             for message in kernel_messages:
                 if message["msg_type"] == "status":
                     if message["content"]["execution_state"] == "idle":
                         return
                 elif message["msg_type"] == "stream":
```

### Comparing `antigranular-0.2.4/antigranular/models/models.py` & `antigranular-0.2.5/antigranular/models/models.py`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.4/LICENSE` & `antigranular-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.4/pyproject.toml` & `antigranular-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "antigranular"
-version = "0.2.4"
+version = "0.2.5"
 description = "Antigranular is a community-driven, open-source platform that merges confidential computing and differential privacy. This creates a secure environment for handling and unlocking the full potential of unseen data.."
 authors = ["Oblivious Software <support@oblivious.ai>"]
 readme = "README.md"
 packages = [{include = "antigranular"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `antigranular-0.2.4/README.md` & `antigranular-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.4/PKG-INFO` & `antigranular-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antigranular
-Version: 0.2.4
+Version: 0.2.5
 Summary: Antigranular is a community-driven, open-source platform that merges confidential computing and differential privacy. This creates a secure environment for handling and unlocking the full potential of unseen data..
 Author: Oblivious Software
 Author-email: support@oblivious.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

