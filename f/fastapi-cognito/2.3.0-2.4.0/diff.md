# Comparing `tmp/fastapi-cognito-2.3.0.tar.gz` & `tmp/fastapi-cognito-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-cognito-2.3.0.tar", last modified: Thu Dec 22 13:28:54 2022, max compression
+gzip compressed data, was "fastapi-cognito-2.4.0.tar", last modified: Fri Jul 21 14:26:34 2023, max compression
```

## Comparing `fastapi-cognito-2.3.0.tar` & `fastapi-cognito-2.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-12-22 13:28:54.134103 fastapi-cognito-2.3.0/
--rw-rw-rw-   0        0        0     1093 2022-10-09 21:24:41.000000 fastapi-cognito-2.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0     5227 2022-12-22 13:28:54.134103 fastapi-cognito-2.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4686 2022-12-22 13:23:34.000000 fastapi-cognito-2.3.0/README.md
--rw-rw-rw-   0        0        0      108 2022-10-09 21:24:41.000000 fastapi-cognito-2.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-22 13:28:54.135103 fastapi-cognito-2.3.0/setup.cfg
--rw-rw-rw-   0        0        0      995 2022-12-22 13:02:25.000000 fastapi-cognito-2.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-22 13:28:54.063383 fastapi-cognito-2.3.0/src/
-drwxrwxrwx   0        0        0        0 2022-12-22 13:28:54.119987 fastapi-cognito-2.3.0/src/fastapi_cognito/
--rw-rw-rw-   0        0        0      180 2022-10-09 21:24:41.000000 fastapi-cognito-2.3.0/src/fastapi_cognito/__init__.py
--rw-rw-rw-   0        0        0      541 2022-10-09 21:24:41.000000 fastapi-cognito-2.3.0/src/fastapi_cognito/exceptions.py
--rw-rw-rw-   0        0        0     9423 2022-12-12 12:44:32.000000 fastapi-cognito-2.3.0/src/fastapi_cognito/fastapi_cognito.py
--rw-rw-rw-   0        0        0      527 2022-12-22 13:21:36.000000 fastapi-cognito-2.3.0/src/fastapi_cognito/models.py
--rw-rw-rw-   0        0        0     1574 2022-12-12 12:44:32.000000 fastapi-cognito-2.3.0/src/fastapi_cognito/settings_parsers.py
-drwxrwxrwx   0        0        0        0 2022-12-22 13:28:54.133103 fastapi-cognito-2.3.0/src/fastapi_cognito.egg-info/
--rw-rw-rw-   0        0        0     5227 2022-12-22 13:28:54.000000 fastapi-cognito-2.3.0/src/fastapi_cognito.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2022-12-22 13:28:54.000000 fastapi-cognito-2.3.0/src/fastapi_cognito.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-22 13:28:54.000000 fastapi-cognito-2.3.0/src/fastapi_cognito.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2022-12-22 13:28:54.000000 fastapi-cognito-2.3.0/src/fastapi_cognito.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-12-22 13:28:54.000000 fastapi-cognito-2.3.0/src/fastapi_cognito.egg-info/top_level.txt
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-07-21 14:26:34.196895 fastapi-cognito-2.4.0/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1073 2023-07-21 10:49:27.000000 fastapi-cognito-2.4.0/LICENSE.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4675 2023-07-21 14:26:34.196895 fastapi-cognito-2.4.0/PKG-INFO
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4150 2023-07-21 14:24:49.000000 fastapi-cognito-2.4.0/README.md
+-rw-rw-r--   0 marko     (1000) marko     (1000)      103 2023-07-21 10:49:27.000000 fastapi-cognito-2.4.0/pyproject.toml
+-rw-rw-r--   0 marko     (1000) marko     (1000)       38 2023-07-21 14:26:34.196895 fastapi-cognito-2.4.0/setup.cfg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1036 2023-07-21 14:20:30.000000 fastapi-cognito-2.4.0/setup.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-07-21 14:26:34.196895 fastapi-cognito-2.4.0/src/
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-07-21 14:26:34.196895 fastapi-cognito-2.4.0/src/fastapi_cognito/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      176 2023-07-21 10:49:27.000000 fastapi-cognito-2.4.0/src/fastapi_cognito/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      525 2023-07-21 10:49:27.000000 fastapi-cognito-2.4.0/src/fastapi_cognito/exceptions.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     9290 2023-07-21 13:40:19.000000 fastapi-cognito-2.4.0/src/fastapi_cognito/fastapi_cognito.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      527 2023-07-21 12:40:47.000000 fastapi-cognito-2.4.0/src/fastapi_cognito/models.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1490 2023-07-21 13:40:46.000000 fastapi-cognito-2.4.0/src/fastapi_cognito/settings_parsers.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2023-07-21 14:26:34.196895 fastapi-cognito-2.4.0/src/fastapi_cognito.egg-info/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4675 2023-07-21 14:26:34.000000 fastapi-cognito-2.4.0/src/fastapi_cognito.egg-info/PKG-INFO
+-rw-rw-r--   0 marko     (1000) marko     (1000)      434 2023-07-21 14:26:34.000000 fastapi-cognito-2.4.0/src/fastapi_cognito.egg-info/SOURCES.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)        1 2023-07-21 14:26:34.000000 fastapi-cognito-2.4.0/src/fastapi_cognito.egg-info/dependency_links.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)       88 2023-07-21 14:26:34.000000 fastapi-cognito-2.4.0/src/fastapi_cognito.egg-info/requires.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)       16 2023-07-21 14:26:34.000000 fastapi-cognito-2.4.0/src/fastapi_cognito.egg-info/top_level.txt
```

### Comparing `fastapi-cognito-2.3.0/LICENSE.txt` & `fastapi-cognito-2.4.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 Marko Mirosavljev
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2021 Marko Mirosavljev
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `fastapi-cognito-2.3.0/PKG-INFO` & `fastapi-cognito-2.4.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,162 +1,152 @@
-Metadata-Version: 2.1
-Name: fastapi-cognito
-Version: 2.3.0
-Summary: Basic AWS cognito authentication package for FastAPI
-Home-page: https://github.com/markomirosavljev/fastapi-cognito
-Author: Marko Mirosavljev
-Author-email: mirosavljevm023@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: Framework :: FastAPI
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# FastAPI - Cognito
-FastAPI package that ease usage of AWS Cognito Auth.
-This package provides basic functions/tools which helps developers to use
-Cognito JWT.
-
-## Requirements
-
-* Python >=3.8
-* FastAPI 
-* AWS Cognito Service
-
-## How to install
-### Pip Command
-```
-pip install fastapi-cognito
-```
-## How to use
-This is the simple example of how to use this package:
-* Create app
-
-```python
-from fastapi import FastAPI
-
-app = FastAPI()
-```
-  
-All mandatory fields are added in CognitoSettings
-BaseSettings object. Settings can be added in different ways.
-You can provide all required settings in **.yaml** or **.json** files,
-or your global BaseSettings file. Note that userpools field is Dict,
-**FIRST** user pool in a dict will be set as default automatically if
-userpool_name is not provided in CognitoAuth object.
-All fields shown in example below, are also required in .json or .yaml file
-(with syntax matching those files.)
-
-You should also import BaseSettings from pydantic if you are going to use global BaseSettings object.
-* Provide settings that are mandatory for CognitoAuth to work. You can provide
-one or more userpools.
-  * `app_client_id` field for userpool besides string, can contain multiple string values provided within 
-    list, tuple or set
-
-```python
-from pydantic import BaseSettings
-
-class Settings(BaseSettings):
-    check_expiration = True
-    jwt_header_prefix = "Bearer"
-    jwt_header_name = "Authorization"
-    userpools = {
-        "eu": {
-            "region": "USERPOOL_REGION",
-            "userpool_id": "USERPOOL_ID",
-            "app_client_id": ["APP_CLIENT_ID_1", "APP_CLIENT_ID_2"] # Example with multiple ids
-        },
-        "us": {
-            "region": "USERPOOL_REGION",
-            "userpool_id": "USERPOOL_ID",
-            "app_client_id": "APP_CLIENT_ID"
-        },
-        ...
-    }
-
-settings = Settings()
-```
-  
-This example below shows how global BaseSettings object can be mapped to
-CognitoSettings and passed as param to CognitoAuth.
-If we were using .yaml or .json, we should call **.from_yaml(_filename_)** or
-**.from_json(_filename_)** methods on CognitoSettings object.
-
-* Instantiate CognitoAuth and pass previously created settings as settings param.
-  
-```python
-from fastapi_cognito import CognitoAuth, CognitoSettings
-
-# default userpool(eu) will be used if there is no userpool_name param provided.
-cognito_eu = CognitoAuth(settings=CognitoSettings.from_global_settings(settings))
-cognito_us = CognitoAuth(settings=CognitoSettings.from_global_settings(settings), userpool_name="us")
-```
-
-* This is a simple endpoint that is protected by Cognito, it uses FastAPI 
-dependency injection to resolve all required operations and get Cognito JWT.
-It can be used later to add more security to endpoints and to get required
-data about user which token belongs to.
-  
-```python
-from fastapi_cognito import CognitoToken
-from fastapi import Depends
-
-@app.get("/")
-def hello_world(auth: CognitoToken = Depends(cognito_eu.auth_required)):
-    return {"message": "Hello world"}
-```
-
-### Optional authentication
-
-If authentication should be optional, we can use ```cognito_eu.auth_optional```
-
-Example:
-```python
-from fastapi_cognito import CognitoToken
-from fastapi import Depends
-
-@app.get("/")
-def hello_world(auth: CognitoToken = Depends(cognito_eu.auth_optional)):
-    return {"message": "Hello world"}
-```
-
-### Custom Token Model
-
-In case your token payload contains additional values, you can provide custom
-token model instead of `CognitoToken`. If there is no custom token model
-provided, `CognitoToken` will be set as a default model.
-
-Example:
-```python
-class CustomTokenModel(CognitoToken):
-    custom_value: Optional[str]
-
-
-class Settings(BaseSettings):
-    check_expiration = True
-    jwt_header_prefix = "Bearer"
-    jwt_header_name = "Authorization"
-    userpools = {
-        "eu": {
-            "region": "USERPOOL_REGION",
-            "userpool_id": "USERPOOL_ID",
-            "app_client_id": "APP_CLIENT_ID"
-        },
-        "us": {
-            "region": "USERPOOL_REGION",
-            "userpool_id": "USERPOOL_ID",
-            "app_client_id": "APP_CLIENT_ID"
-        }
-    }
-    custom_cognito_token_model: PyObject = CustomTokenModel
-
-@app.get("/")
-def hello_world(auth: CustomTokenModel = Depends(cognito_us.auth_required)):
-    return {"message": f"Hello {auth.custom_value}"}
-```
-**NOTE: It is important to set `custom_cognito_token_model` type in BaseSettings
-to `PyObject`**. In order to have type hints, you need to set your custom model
-as type of `auth`.
-
+Metadata-Version: 2.1
+Name: fastapi-cognito
+Version: 2.4.0
+Summary: Basic AWS cognito authentication package for FastAPI
+Home-page: https://github.com/markomirosavljev/fastapi-cognito
+Author: Marko Mirosavljev
+Author-email: mirosavljevm023@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Framework :: FastAPI
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# FastAPI - Cognito
+FastAPI package that ease usage of AWS Cognito Auth.
+This package provides basic functions/tools which helps developers to use
+Cognito JWT.
+
+## Requirements
+
+* Python >=3.8
+* FastAPI 
+* AWS Cognito Service
+
+## How to install
+### Pip Command
+```
+pip install fastapi-cognito
+```
+## How to use
+This is the simple example of how to use this package:
+* Create app
+
+```python
+from fastapi import FastAPI
+
+app = FastAPI()
+```
+  
+All mandatory fields are added in CognitoSettings
+BaseSettings object. Settings can be added in different ways.
+You can provide all required settings in **.yaml** or **.json** files,
+or your global BaseSettings file. Note that userpools field is Dict,
+**FIRST** user pool in a dict will be set as default automatically if
+userpool_name is not provided in CognitoAuth object.
+All fields shown in example below, are also required in .json or .yaml file
+(with syntax matching those files.)
+
+You should also import BaseSettings from pydantic if you are going to use global BaseSettings object.
+* Provide settings that are mandatory for CognitoAuth to work. You can provide
+one or more userpools.
+  * `app_client_id` field for userpool besides string, can contain multiple string values provided within 
+    list, tuple or set
+
+```python
+from pydantic_settings import BaseSettings
+from pydantic.types import Any
+
+class Settings(BaseSettings):
+    check_expiration: bool = True
+    jwt_header_prefix: str = "Bearer"
+    jwt_header_name: str = "Authorization"
+    userpools: dict[str, dict[str, Any]] = {
+        "eu": {
+            "region": "USERPOOL_REGION",
+            "userpool_id": "USERPOOL_ID",
+            "app_client_id": ["APP_CLIENT_ID_1", "APP_CLIENT_ID_2"] # Example with multiple ids
+        },
+        "us": {
+            "region": "USERPOOL_REGION",
+            "userpool_id": "USERPOOL_ID",
+            "app_client_id": "APP_CLIENT_ID"
+        },
+        ...
+    }
+
+settings = Settings()
+```
+  
+This example below shows how global BaseSettings object can be mapped to
+CognitoSettings and passed as param to CognitoAuth.
+If we were using .yaml or .json, we should call **.from_yaml(_filename_)** or
+**.from_json(_filename_)** methods on CognitoSettings object.
+
+* Instantiate CognitoAuth and pass previously created settings as settings param.
+  
+```python
+from fastapi_cognito import CognitoAuth, CognitoSettings
+
+# default userpool(eu) will be used if there is no userpool_name param provided.
+cognito_eu = CognitoAuth(
+  settings=CognitoSettings.from_global_settings(settings)
+)
+cognito_us = CognitoAuth(
+  settings=CognitoSettings.from_global_settings(settings), userpool_name="us"
+)
+```
+
+* This is a simple endpoint that is protected by Cognito, it uses FastAPI 
+dependency injection to resolve all required operations and get Cognito JWT.
+It can be used later to add more security to endpoints and to get required
+data about user which token belongs to.
+  
+```python
+from fastapi_cognito import CognitoToken
+from fastapi import Depends
+
+@app.get("/")
+def hello_world(auth: CognitoToken = Depends(cognito_eu.auth_required)):
+    return {"message": "Hello world"}
+```
+
+### Optional authentication
+
+If authentication should be optional, we can use ```cognito_eu.auth_optional```
+
+Example:
+```python
+from fastapi_cognito import CognitoToken
+from fastapi import Depends
+
+@app.get("/")
+def hello_world(auth: CognitoToken = Depends(cognito_eu.auth_optional)):
+    return {"message": "Hello world"}
+```
+
+### Custom Token Model
+
+In case your token payload contains additional values, you can provide custom
+token model instead of `CognitoToken`. If there is no custom token model
+provided, `CognitoToken` will be set as a default model. Custom model should
+be provided to `CognitoAuth` object.
+
+Example:
+```python
+class CustomTokenModel(CognitoToken):
+    custom_value: Optional[str] = None
+
+
+cognito = CognitoAuth(
+    settings=CognitoSettings.from_global_settings(settings),
+    # Here we provide custom token model
+    custom_model=CustomTokenModel
+)
+
+@app.get("/")
+def hello_world(auth: CustomTokenModel = Depends(cognito.auth_required)):
+    return {"message": f"Hello {auth.custom_value}"}
+```
```

### Comparing `fastapi-cognito-2.3.0/README.md` & `fastapi-cognito-2.4.0/src/fastapi_cognito.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,146 +1,152 @@
-# FastAPI - Cognito
-FastAPI package that ease usage of AWS Cognito Auth.
-This package provides basic functions/tools which helps developers to use
-Cognito JWT.
-
-## Requirements
-
-* Python >=3.8
-* FastAPI 
-* AWS Cognito Service
-
-## How to install
-### Pip Command
-```
-pip install fastapi-cognito
-```
-## How to use
-This is the simple example of how to use this package:
-* Create app
-
-```python
-from fastapi import FastAPI
-
-app = FastAPI()
-```
-  
-All mandatory fields are added in CognitoSettings
-BaseSettings object. Settings can be added in different ways.
-You can provide all required settings in **.yaml** or **.json** files,
-or your global BaseSettings file. Note that userpools field is Dict,
-**FIRST** user pool in a dict will be set as default automatically if
-userpool_name is not provided in CognitoAuth object.
-All fields shown in example below, are also required in .json or .yaml file
-(with syntax matching those files.)
-
-You should also import BaseSettings from pydantic if you are going to use global BaseSettings object.
-* Provide settings that are mandatory for CognitoAuth to work. You can provide
-one or more userpools.
-  * `app_client_id` field for userpool besides string, can contain multiple string values provided within 
-    list, tuple or set
-
-```python
-from pydantic import BaseSettings
-
-class Settings(BaseSettings):
-    check_expiration = True
-    jwt_header_prefix = "Bearer"
-    jwt_header_name = "Authorization"
-    userpools = {
-        "eu": {
-            "region": "USERPOOL_REGION",
-            "userpool_id": "USERPOOL_ID",
-            "app_client_id": ["APP_CLIENT_ID_1", "APP_CLIENT_ID_2"] # Example with multiple ids
-        },
-        "us": {
-            "region": "USERPOOL_REGION",
-            "userpool_id": "USERPOOL_ID",
-            "app_client_id": "APP_CLIENT_ID"
-        },
-        ...
-    }
-
-settings = Settings()
-```
-  
-This example below shows how global BaseSettings object can be mapped to
-CognitoSettings and passed as param to CognitoAuth.
-If we were using .yaml or .json, we should call **.from_yaml(_filename_)** or
-**.from_json(_filename_)** methods on CognitoSettings object.
-
-* Instantiate CognitoAuth and pass previously created settings as settings param.
-  
-```python
-from fastapi_cognito import CognitoAuth, CognitoSettings
-
-# default userpool(eu) will be used if there is no userpool_name param provided.
-cognito_eu = CognitoAuth(settings=CognitoSettings.from_global_settings(settings))
-cognito_us = CognitoAuth(settings=CognitoSettings.from_global_settings(settings), userpool_name="us")
-```
-
-* This is a simple endpoint that is protected by Cognito, it uses FastAPI 
-dependency injection to resolve all required operations and get Cognito JWT.
-It can be used later to add more security to endpoints and to get required
-data about user which token belongs to.
-  
-```python
-from fastapi_cognito import CognitoToken
-from fastapi import Depends
-
-@app.get("/")
-def hello_world(auth: CognitoToken = Depends(cognito_eu.auth_required)):
-    return {"message": "Hello world"}
-```
-
-### Optional authentication
-
-If authentication should be optional, we can use ```cognito_eu.auth_optional```
-
-Example:
-```python
-from fastapi_cognito import CognitoToken
-from fastapi import Depends
-
-@app.get("/")
-def hello_world(auth: CognitoToken = Depends(cognito_eu.auth_optional)):
-    return {"message": "Hello world"}
-```
-
-### Custom Token Model
-
-In case your token payload contains additional values, you can provide custom
-token model instead of `CognitoToken`. If there is no custom token model
-provided, `CognitoToken` will be set as a default model.
-
-Example:
-```python
-class CustomTokenModel(CognitoToken):
-    custom_value: Optional[str]
-
-
-class Settings(BaseSettings):
-    check_expiration = True
-    jwt_header_prefix = "Bearer"
-    jwt_header_name = "Authorization"
-    userpools = {
-        "eu": {
-            "region": "USERPOOL_REGION",
-            "userpool_id": "USERPOOL_ID",
-            "app_client_id": "APP_CLIENT_ID"
-        },
-        "us": {
-            "region": "USERPOOL_REGION",
-            "userpool_id": "USERPOOL_ID",
-            "app_client_id": "APP_CLIENT_ID"
-        }
-    }
-    custom_cognito_token_model: PyObject = CustomTokenModel
-
-@app.get("/")
-def hello_world(auth: CustomTokenModel = Depends(cognito_us.auth_required)):
-    return {"message": f"Hello {auth.custom_value}"}
-```
-**NOTE: It is important to set `custom_cognito_token_model` type in BaseSettings
-to `PyObject`**. In order to have type hints, you need to set your custom model
-as type of `auth`.
-
+Metadata-Version: 2.1
+Name: fastapi-cognito
+Version: 2.4.0
+Summary: Basic AWS cognito authentication package for FastAPI
+Home-page: https://github.com/markomirosavljev/fastapi-cognito
+Author: Marko Mirosavljev
+Author-email: mirosavljevm023@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Framework :: FastAPI
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# FastAPI - Cognito
+FastAPI package that ease usage of AWS Cognito Auth.
+This package provides basic functions/tools which helps developers to use
+Cognito JWT.
+
+## Requirements
+
+* Python >=3.8
+* FastAPI 
+* AWS Cognito Service
+
+## How to install
+### Pip Command
+```
+pip install fastapi-cognito
+```
+## How to use
+This is the simple example of how to use this package:
+* Create app
+
+```python
+from fastapi import FastAPI
+
+app = FastAPI()
+```
+  
+All mandatory fields are added in CognitoSettings
+BaseSettings object. Settings can be added in different ways.
+You can provide all required settings in **.yaml** or **.json** files,
+or your global BaseSettings file. Note that userpools field is Dict,
+**FIRST** user pool in a dict will be set as default automatically if
+userpool_name is not provided in CognitoAuth object.
+All fields shown in example below, are also required in .json or .yaml file
+(with syntax matching those files.)
+
+You should also import BaseSettings from pydantic if you are going to use global BaseSettings object.
+* Provide settings that are mandatory for CognitoAuth to work. You can provide
+one or more userpools.
+  * `app_client_id` field for userpool besides string, can contain multiple string values provided within 
+    list, tuple or set
+
+```python
+from pydantic_settings import BaseSettings
+from pydantic.types import Any
+
+class Settings(BaseSettings):
+    check_expiration: bool = True
+    jwt_header_prefix: str = "Bearer"
+    jwt_header_name: str = "Authorization"
+    userpools: dict[str, dict[str, Any]] = {
+        "eu": {
+            "region": "USERPOOL_REGION",
+            "userpool_id": "USERPOOL_ID",
+            "app_client_id": ["APP_CLIENT_ID_1", "APP_CLIENT_ID_2"] # Example with multiple ids
+        },
+        "us": {
+            "region": "USERPOOL_REGION",
+            "userpool_id": "USERPOOL_ID",
+            "app_client_id": "APP_CLIENT_ID"
+        },
+        ...
+    }
+
+settings = Settings()
+```
+  
+This example below shows how global BaseSettings object can be mapped to
+CognitoSettings and passed as param to CognitoAuth.
+If we were using .yaml or .json, we should call **.from_yaml(_filename_)** or
+**.from_json(_filename_)** methods on CognitoSettings object.
+
+* Instantiate CognitoAuth and pass previously created settings as settings param.
+  
+```python
+from fastapi_cognito import CognitoAuth, CognitoSettings
+
+# default userpool(eu) will be used if there is no userpool_name param provided.
+cognito_eu = CognitoAuth(
+  settings=CognitoSettings.from_global_settings(settings)
+)
+cognito_us = CognitoAuth(
+  settings=CognitoSettings.from_global_settings(settings), userpool_name="us"
+)
+```
+
+* This is a simple endpoint that is protected by Cognito, it uses FastAPI 
+dependency injection to resolve all required operations and get Cognito JWT.
+It can be used later to add more security to endpoints and to get required
+data about user which token belongs to.
+  
+```python
+from fastapi_cognito import CognitoToken
+from fastapi import Depends
+
+@app.get("/")
+def hello_world(auth: CognitoToken = Depends(cognito_eu.auth_required)):
+    return {"message": "Hello world"}
+```
+
+### Optional authentication
+
+If authentication should be optional, we can use ```cognito_eu.auth_optional```
+
+Example:
+```python
+from fastapi_cognito import CognitoToken
+from fastapi import Depends
+
+@app.get("/")
+def hello_world(auth: CognitoToken = Depends(cognito_eu.auth_optional)):
+    return {"message": "Hello world"}
+```
+
+### Custom Token Model
+
+In case your token payload contains additional values, you can provide custom
+token model instead of `CognitoToken`. If there is no custom token model
+provided, `CognitoToken` will be set as a default model. Custom model should
+be provided to `CognitoAuth` object.
+
+Example:
+```python
+class CustomTokenModel(CognitoToken):
+    custom_value: Optional[str] = None
+
+
+cognito = CognitoAuth(
+    settings=CognitoSettings.from_global_settings(settings),
+    # Here we provide custom token model
+    custom_model=CustomTokenModel
+)
+
+@app.get("/")
+def hello_world(auth: CustomTokenModel = Depends(cognito.auth_required)):
+    return {"message": f"Hello {auth.custom_value}"}
+```
```

### Comparing `fastapi-cognito-2.3.0/src/fastapi_cognito/settings_parsers.py` & `fastapi-cognito-2.4.0/src/fastapi_cognito/settings_parsers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import yaml
-import json
-from pydantic import BaseSettings, PyObject
-from typing import Dict, Optional
-
-
-class CognitoSettings(BaseSettings):
-    """
-    This class contains all mandatory fields which should get values from
-    provided config file
-    """
-    check_expiration: bool
-    jwt_header_name: str
-    jwt_header_prefix: str
-    userpools: Dict
-    custom_cognito_token_model: Optional[PyObject]
-
-    class Config:
-        extra = "ignore"
-
-    @classmethod
-    def from_global_settings(cls, global_settings: BaseSettings):
-        """
-        Parse configurations from global BaseSettings object where all
-        configurations could be provided.
-        :param global_settings: global BaseSettings object.
-        :return: mapped CognitoSettings class
-        """
-        return cls(**global_settings.dict())
-
-    @classmethod
-    def load_yaml(cls, yaml_file: str):
-        """
-        Open provided .yaml file and read configs from it.
-        :param yaml_file: file that should contain all required configurations
-        :return: mapped CognitoSettings class
-        """
-        with open(yaml_file, "r") as file:
-            return cls(**yaml.safe_load(file))
-
-    @classmethod
-    def load_json(cls, json_file: str):
-        """
-        Open provided .json file and read configs from it.
-        :param json_file: file that should contain all required configurations.
-        :return: mapped CognitoSettings class
-        """
-        with open(json_file) as file:
-            return cls(**json.load(file))
+import json
+from typing import Any
+
+import yaml
+from pydantic_settings import BaseSettings
+
+
+class CognitoSettings(BaseSettings):
+    """
+    This class contains all mandatory fields which should get values from
+    provided config file
+    """
+    check_expiration: bool
+    jwt_header_name: str
+    jwt_header_prefix: str
+    userpools: dict[str, dict[str, Any]]
+
+    class Config:
+        extra = "ignore"
+
+    @classmethod
+    def from_global_settings(cls, global_settings: BaseSettings):
+        """
+        Parse configurations from global BaseSettings object where all
+        configurations could be provided.
+        :param global_settings: global BaseSettings object.
+        :return: mapped CognitoSettings class
+        """
+        return cls(**global_settings.model_dump())
+
+    @classmethod
+    def load_yaml(cls, yaml_file: str):
+        """
+        Open provided .yaml file and read configs from it.
+        :param yaml_file: file that should contain all required configurations
+        :return: mapped CognitoSettings class
+        """
+        with open(yaml_file, "r") as file:
+            return cls(**yaml.safe_load(file))
+
+    @classmethod
+    def load_json(cls, json_file: str):
+        """
+        Open provided .json file and read configs from it.
+        :param json_file: file that should contain all required configurations.
+        :return: mapped CognitoSettings class
+        """
+        with open(json_file) as file:
+            return cls(**json.load(file))
```

