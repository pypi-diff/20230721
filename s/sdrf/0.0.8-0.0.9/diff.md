# Comparing `tmp/sdrf-0.0.8.tar.gz` & `tmp/sdrf-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdrf-0.0.8.tar", last modified: Thu Jul 20 00:23:40 2023, max compression
+gzip compressed data, was "sdrf-0.0.9.tar", last modified: Fri Jul 21 12:30:25 2023, max compression
```

## Comparing `sdrf-0.0.8.tar` & `sdrf-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 00:23:40.320106 sdrf-0.0.8/
--rw-rw-rw-   0        0        0     1083 2023-07-19 21:53:19.000000 sdrf-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0     4523 2023-07-20 00:23:40.319107 sdrf-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3826 2023-07-20 00:21:03.000000 sdrf-0.0.8/README.md
--rw-rw-rw-   0        0        0      570 2023-07-20 00:21:59.000000 sdrf-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-20 00:23:40.320106 sdrf-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      589 2023-07-20 00:21:53.000000 sdrf-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 00:23:40.258880 sdrf-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-20 00:23:40.286883 sdrf-0.0.8/src/sdrf/
--rw-rw-rw-   0        0        0        0 2023-07-12 15:32:23.000000 sdrf-0.0.8/src/sdrf/__init__.py
--rw-rw-rw-   0        0        0     1957 2023-07-19 22:29:51.000000 sdrf-0.0.8/src/sdrf/api_endpoint.py
--rw-rw-rw-   0        0        0      146 2023-07-19 22:22:43.000000 sdrf-0.0.8/src/sdrf/apps.py
--rw-rw-rw-   0        0        0     4271 2023-07-20 00:06:36.000000 sdrf-0.0.8/src/sdrf/endpoint_config.py
-drwxrwxrwx   0        0        0        0 2023-07-20 00:23:40.316108 sdrf-0.0.8/src/sdrf/enums/
--rw-rw-rw-   0        0        0       98 2023-07-14 20:55:44.000000 sdrf-0.0.8/src/sdrf/enums/__init__.py
--rw-rw-rw-   0        0        0      356 2023-07-12 15:32:23.000000 sdrf-0.0.8/src/sdrf/enums/api_data_type_enum.py
--rw-rw-rw-   0        0        0      268 2023-07-12 15:32:23.000000 sdrf-0.0.8/src/sdrf/enums/parameter_type_enum.py
--rw-rw-rw-   0        0        0      903 2023-07-19 23:47:49.000000 sdrf-0.0.8/src/sdrf/swagger_config.py
--rw-rw-rw-   0        0        0      460 2023-07-20 00:02:14.000000 sdrf-0.0.8/src/sdrf/urls.py
-drwxrwxrwx   0        0        0        0 2023-07-20 00:23:40.318107 sdrf-0.0.8/src/sdrf/utils/
--rw-rw-rw-   0        0        0      246 2023-07-19 23:45:26.000000 sdrf-0.0.8/src/sdrf/utils/settings_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-20 00:23:40.307588 sdrf-0.0.8/src/sdrf.egg-info/
--rw-rw-rw-   0        0        0     4523 2023-07-20 00:23:40.000000 sdrf-0.0.8/src/sdrf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      474 2023-07-20 00:23:40.000000 sdrf-0.0.8/src/sdrf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 00:23:40.000000 sdrf-0.0.8/src/sdrf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-20 00:23:40.000000 sdrf-0.0.8/src/sdrf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-20 00:23:40.000000 sdrf-0.0.8/src/sdrf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:30:25.567203 sdrf-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-21 12:30:15.000000 sdrf-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-07-21 12:30:25.567203 sdrf-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-07-21 12:30:15.000000 sdrf-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-21 12:30:15.000000 sdrf-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 12:30:25.567203 sdrf-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-21 12:30:15.000000 sdrf-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:30:25.563203 sdrf-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:30:25.563203 sdrf-0.0.9/src/sdrf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:30:15.000000 sdrf-0.0.9/src/sdrf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-21 12:30:15.000000 sdrf-0.0.9/src/sdrf/api_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-21 12:30:15.000000 sdrf-0.0.9/src/sdrf/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-07-21 12:30:15.000000 sdrf-0.0.9/src/sdrf/endpoint_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:30:25.567203 sdrf-0.0.9/src/sdrf/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-21 12:30:15.000000 sdrf-0.0.9/src/sdrf/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-21 12:30:15.000000 sdrf-0.0.9/src/sdrf/enums/api_data_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-21 12:30:15.000000 sdrf-0.0.9/src/sdrf/enums/parameter_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-21 12:30:15.000000 sdrf-0.0.9/src/sdrf/model_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-21 12:30:15.000000 sdrf-0.0.9/src/sdrf/swagger_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-21 12:30:15.000000 sdrf-0.0.9/src/sdrf/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:30:25.567203 sdrf-0.0.9/src/sdrf/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-21 12:30:15.000000 sdrf-0.0.9/src/sdrf/utils/settings_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:30:25.567203 sdrf-0.0.9/src/sdrf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-07-21 12:30:25.000000 sdrf-0.0.9/src/sdrf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-21 12:30:25.000000 sdrf-0.0.9/src/sdrf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:30:25.000000 sdrf-0.0.9/src/sdrf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-21 12:30:25.000000 sdrf-0.0.9/src/sdrf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 12:30:25.000000 sdrf-0.0.9/src/sdrf.egg-info/top_level.txt
```

### Comparing `sdrf-0.0.8/LICENSE.txt` & `sdrf-0.0.9/LICENSE.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-MIT License
-
-Copyright (c) 2023 Hussein Anabtawi
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Hussein Anabtawi
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `sdrf-0.0.8/PKG-INFO` & `sdrf-0.0.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,118 +1,127 @@
-Metadata-Version: 2.1
-Name: sdrf
-Version: 0.0.8
-Summary: Simple rest framework is an abstraction for building rest api with well written documentations
-Home-page: https://github.com/hus201/sdrf
-Author: Hussein Anabtawi
-Author-email: Hussein Anabtawi <husainanabtawi2001@hotmail.com>
-Project-URL: Homepage, https://github.com/hus201/sdrf
-Project-URL: Bug Tracker, https://github.com/hus201/sdrf/issues
-Keywords: django,rest apis,abstraction
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# Simple Django Rest Framework
-
-Simple Django Rest Framework is django based app used to provide abstraction that combines both django rest framework with drf_yasg a swagger generator to implement good looking and  well documented apis using djang
-
-
-## Quick Start
-
-### Install
-1. assuming you already have a django project that you need to add this app to you need to start with installing the package using
-```
-pip install sdrf
-```
-2. install required apps to INSTALLED_APPS in django settings
-```python
-INSTALLED_APPS = [
-    ...
-    "rest_framework",
-    "drf_yasg",
-    'sdrf',
-]
-```
-3. add swagger docs url to your project urls
-```python
-from django.contrib import admin
-from django.urls import path,include
-
-urlpatterns = [
-    ...
-    path('',include('sdrf.urls'))
-]
-```
-4. check out if everything is okay by visting default swagger docs url at ``http://<your-project-url>/rest``
-![Empty Swagger UI example](docs/empty-swagger-ui.png)
-
-### Configure
-now you have an rest app up and running you can configure it as you want. addtionally for django rest framework configuration and drf_yasg configuration you have our sdrf configs you can make with these default values
-
-
-| config variable name | default value | description |
-| ------- | ------ | ----- |
-| REST_APP_NAME | `Weather API` | the app name used in swagger docs view |
-| REST_APP_VERSION | `v1` | the api version used in swagger docs view |
-| REST_APP_CREATOR | ``{'name': '','email': '','url': ''}`` | the contact information for communicating the rest app creator used in swagger docs view |
-| REST_APP_BASE_URL | `rest/` | the base url that the swagger docs will be viewd on and a prefix for default api endpoint |
-### Build API Endpoints
-1. assuming you have an django app that already exsist create and an API endpoint class that inheiret APIEndPoint class for example see out hello world here
-```python
-from sdrf.api_endpoint import APIEndpoint
-from sdrf.endpoint_config import APIEndpointConfig
-
-
-class HelloEndPoint(APIEndpoint):
-    def configure(self, config: APIEndpointConfig) -> APIEndpointConfig:
-        ...
-        return config
-
-    @staticmethod
-    def execute(request: Request, *args, **kwargs) -> Response:
-        name = request.query_params.get('name')
-        return HttpResponse(f'Hello {name}')
-
-```
-2. configure your api endpoint using configure method, in this method you have all sort of configuration that you can configure for your rest api even the auhentication and authorization configurations, http method, routing, and swagger view configs simplified with easy and nice looking config code
-```python
-from sdrf.api_endpoint import APIEndpoint
-from sdrf.endpoint_config import APIEndpointConfig
-
-
-class HelloEndPoint(APIEndpoint):
-    def configure(self, config: APIEndpointConfig) -> APIEndpointConfig:
-        config.name = 'Hello Rest!'
-        config.description= """
-        First Well documented API endpoint that says hello to name that you send
-        """
-        config.endpoint= 'hello'
-        config.http_method = 'GET'
-        config.set_response(200,'hello [name]')
-        config.add_parameter('name',self.DataType.STRING,self.ParameterTypes.QUERY_PARAM)
-        config.add_tag('First API')
-        return config
-
-    @staticmethod
-    def execute(request: Request, *args, **kwargs) -> Response:
-        name = request.query_params.get('name')
-        return HttpResponse(f'Hello {name}')
-
-```
-3. finally add your api endpoint to your app urls using as_url static method
-```python
-from .views import HelloEndPoint
-
-urlpatterns = [
-    HelloEndPoint.as_url()
-]
-```
-
-4. check your output and test your api in the swagger view
-
-![An example of swagger output of APIEndPoint](docs/swagger-output-example.png)
-
-
+# Simple Django Rest Framework
+
+Simple Django Rest Framework is django based app used to provide abstraction that combines both django rest framework with drf_yasg a swagger generator to implement good looking and  well documented apis using djang
+
+
+## Quick Start
+
+### Install
+1. assuming you already have a django project that you need to add this app to you need to start with installing the package using
+```
+pip install sdrf
+```
+2. install required apps to INSTALLED_APPS in django settings
+```python
+INSTALLED_APPS = [
+    ...
+    "rest_framework",
+    "drf_yasg",
+    'sdrf',
+]
+```
+3. add swagger docs url to your project urls
+```python
+from django.contrib import admin
+from django.urls import path,include
+
+urlpatterns = [
+    ...
+    path('',include('sdrf.urls'))
+]
+```
+4. check out if everything is okay by visting default swagger docs url at ``http://<your-project-url>/rest``
+![Empty Swagger UI example](https://raw.githubusercontent.com/hus201/sdrf/main/docs/empty-swagger-ui.png)
+
+### Configure
+now you have an rest app up and running you can configure it as you want. addtionally for django rest framework configuration and drf_yasg configuration you have our sdrf configs you can make with these default values
+
+
+| config variable name | default value | description |
+| ------- | ------ | ----- |
+| REST_APP_NAME | `Weather API` | the app name used in swagger docs view |
+| REST_APP_VERSION | `v1` | the api version used in swagger docs view |
+| REST_APP_CREATOR | ``{'name': '','email': '','url': ''}`` | the contact information for communicating the rest app creator used in swagger docs view |
+| REST_APP_BASE_URL | `rest/` | the base url that the swagger docs will be viewd on and a prefix for default api endpoint |
+
+## Usage
+
+### Build Single Method API Endpoints
+1. assuming you have an django app that already exsist create and an API endpoint class that inheiret APIEndPoint class for example see out hello world here
+```python
+from sdrf.api_endpoint import APIEndpoint
+from sdrf.endpoint_config import APIEndpointConfig
+
+
+class HelloEndPoint(APIEndpoint):
+    def configure(self, config: APIEndpointConfig) -> APIEndpointConfig:
+        ...
+        return config
+
+    @staticmethod
+    def execute(request: Request, *args, **kwargs) -> Response:
+        name = request.query_params.get('name')
+        return HttpResponse(f'Hello {name}')
+
+```
+2. configure your api endpoint using configure method, in this method you have all sort of configuration that you can configure for your rest api even the auhentication and authorization configurations, http method, routing, and swagger view configs simplified with easy and nice looking config code
+```python
+from sdrf.api_endpoint import APIEndpoint
+from sdrf.endpoint_config import APIEndpointConfig
+
+
+class HelloEndPoint(APIEndpoint):
+    def configure(self, config: APIEndpointConfig) -> APIEndpointConfig:
+        config.name = 'Hello Rest!'
+        config.description= """
+        First Well documented API endpoint that says hello to name that you send
+        """
+        config.endpoint= 'hello'
+        config.http_method = 'GET'
+        config.set_response(200,'hello [name]')
+        config.add_parameter('name',self.DataType.STRING,self.ParameterTypes.QUERY_PARAM)
+        config.add_tag('First API')
+        return config
+
+    @staticmethod
+    def execute(request: Request, *args, **kwargs) -> Response:
+        name = request.query_params.get('name')
+        return HttpResponse(f'Hello {name}')
+
+```
+3. finally add your api endpoint to your app urls using as_url static method
+```python
+from .views import HelloEndPoint
+
+urlpatterns = [
+    HelloEndPoint.as_url()
+]
+```
+
+4. check your output and test your api in the swagger view
+
+![An example of swagger output of APIEndPoint](https://raw.githubusercontent.com/hus201/sdrf/main/docs/swagger-output-example.png)
+
+
+### Build Model API EndPoint
+
+just like you would do in normal django rest framework and make `ViewSet` you don`t need to learn anything new to that but instead of inherting `rest_framework.viewsets.ModelViewSet` you will inherit our `ModelEndPoint`like that
+
+```python
+from .models import Person,PersonSeralizer
+from sdrf.model_endpoint import ModelEndPoint
+...
+class PersonEndPoint(ModelEndPoint):
+    queryset = Person.objects.all()
+    serializer_class = PersonSeralizer
+```
+then simply make  it as urls in `urls.py`
+```python
+from .views import PersonEndPoint
+
+urlpatterns = [
+    ...
+    PersonEndPoint.as_urls(),
+]
+
+```
+![Model EndPoint Swagger output](https://raw.githubusercontent.com/hus201/sdrf/main/docs/model-endpoint-example.png)
```

### Comparing `sdrf-0.0.8/src/sdrf/api_endpoint.py` & `sdrf-0.0.9/src/sdrf/api_endpoint.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from abc import ABC, abstractmethod
-
-from django.urls import path
-from django.utils.decorators import classonlymethod
-from rest_framework.request import Request
-from rest_framework.response import Response
-from sdrf.endpoint_config import APIEndpointConfig
-from rest_framework.decorators import api_view
-from drf_yasg.utils import swagger_auto_schema
-from sdrf.enums import ParameterType, APIParamDataType
-from rest_framework.decorators import permission_classes, authentication_classes
-
-
-class APIEndpoint(ABC):
-
-    ParameterTypes = ParameterType
-    DataType = APIParamDataType
-
-    @classonlymethod
-    @abstractmethod
-    def configure(self, config: APIEndpointConfig) -> APIEndpointConfig:
-        pass
-
-    @classonlymethod
-    def as_url(self):
-        config: APIEndpointConfig = APIEndpointConfig(name=self.__name__)
-        config = self.configure(self, config)
-        assert config.endpoint != '' or config.full_route != '', 'you need to setup either endpoint or full route'
-        authorized_function = permission_classes(config.permission_classes)(self.execute)
-        authenticated_function = authentication_classes(config.authentication_classes)(authorized_function)
-        as_view = api_view([config.http_method])(authenticated_function)
-        with_swagger = swagger_auto_schema(
-            name=config.name,
-            operation_description=config.description,
-            operation_summary=config.summary,
-            deprecated=config.deprecated,
-            method=config.http_method,
-            manual_parameters=config.parameters,
-            request_body=config.request_body,
-            responses=config.responses,
-            tags=config.tags
-        )(as_view)
-        url = path(config.get_full_route(), with_swagger, name=config.name)
-        return url
-
-    @staticmethod
-    @abstractmethod
-    def execute(request: Request, *args, **kwargs) -> Response:
-        pass
+from abc import ABC, abstractmethod
+
+from django.urls import path
+from django.utils.decorators import classonlymethod
+from rest_framework.request import Request
+from rest_framework.response import Response
+from sdrf.endpoint_config import APIEndpointConfig
+from rest_framework.decorators import api_view
+from drf_yasg.utils import swagger_auto_schema
+from sdrf.enums import ParameterType, APIParamDataType
+from rest_framework.decorators import permission_classes, authentication_classes
+
+
+class APIEndpoint(ABC):
+
+    ParameterTypes = ParameterType
+    DataType = APIParamDataType
+
+    @classonlymethod
+    @abstractmethod
+    def configure(self, config: APIEndpointConfig) -> APIEndpointConfig:
+        pass
+
+    @classonlymethod
+    def as_url(self):
+        config: APIEndpointConfig = APIEndpointConfig(name=self.__name__)
+        config = self.configure(self, config)
+        assert config.endpoint != '' or config.full_route != '', 'you need to setup either endpoint or full route'
+        authorized_function = permission_classes(config.permission_classes)(self.execute)
+        authenticated_function = authentication_classes(config.authentication_classes)(authorized_function)
+        as_view = api_view([config.http_method])(authenticated_function)
+        with_swagger = swagger_auto_schema(
+            name=config.name,
+            operation_description=config.description,
+            operation_summary=config.summary,
+            deprecated=config.deprecated,
+            method=config.http_method,
+            manual_parameters=config.parameters,
+            request_body=config.request_body,
+            responses=config.responses,
+            tags=config.tags
+        )(as_view)
+        url = path(config.get_full_route(), with_swagger, name=config.name)
+        return url
+
+    @staticmethod
+    @abstractmethod
+    def execute(request: Request, *args, **kwargs) -> Response:
+        pass
```

### Comparing `sdrf-0.0.8/src/sdrf/endpoint_config.py` & `sdrf-0.0.9/src/sdrf/endpoint_config.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-from typing import Literal, List, Union, Dict, Type
-from drf_yasg.openapi import Parameter, Schema, Response
-from sdrf.enums import ParameterType, APIParamDataType
-from rest_framework.serializers import Serializer
-from rest_framework.authentication import BaseAuthentication
-from rest_framework.permissions import IsAuthenticated, BasePermission
-from django.conf import settings
-from sdrf.utils.settings_utils import get_settings_value
-
-class APIEndpointConfig:
-    def __init__(self, name: str) -> None:
-        super().__init__()
-        self.name = name
-        self.parameters = []
-        self.tags = []
-        self.responses = {}
-        self.permission_classes = []
-        self.authentication_classes = []
-
-    name: str
-    description: str = ''
-    summary: str = ''
-    http_method: Literal['GET', 'POST', 'PUT', 'PATCH', 'DELETE'] = 'GET'
-    parameters: List[Parameter] = []
-    responses: Dict = {}
-    tags: List[str] = []
-    request_body: Schema = None
-    base_url: str = get_settings_value('REST_APP_BASE_URL','rest/')
-    rest_api_version = get_settings_value('REST_APP_VERSION','v1')
-    endpoint: str = ''
-    full_route: str = ''
-    deprecated: bool = False
-    authentication_classes: List = []
-    permission_classes: List = []
-
-    def require_authenticated_permission(self):
-        self.add_permission_class(IsAuthenticated)
-
-    def add_permission_class(self, permission_class):
-        assert issubclass(permission_class, BasePermission), 'Permission Class should be of type BasePermission'
-        self.permission_classes.append(permission_class)
-
-    def add_authentication_class(self, authentication_class):
-        assert issubclass(authentication_class, BaseAuthentication), 'Permission Class should be an instance of ' \
-                                                                     'BaseAuthentication '
-        self.authentication_classes.append(authentication_class)
-
-    def add_parameter(self,
-                      name: str,
-                      data_type: APIParamDataType = APIParamDataType.STRING,
-                      parameter_type: ParameterType = ParameterType.QUERY_PARAM,
-                      description: str = '',
-                      required: bool = True,
-                      default=None):
-        if parameter_type.value == ParameterType.BODY_PARAM.value:
-            if self.request_body is None:
-                self.request_body = Schema(type=APIParamDataType.OBJECT.value, required=[], properties={})
-            self.request_body.properties[name] = Schema(type=data_type.value)
-            if required:
-                self.request_body.required.append(name)
-
-        else:
-            param = Parameter(name=name,
-                              description=description,
-                              in_=parameter_type.value,
-                              type=data_type.value,
-                              required=required,
-                              default=default)
-            self.parameters.append(param)
-
-    def add_tag(self, tag: str):
-        tags = self.tags
-        tags.append(tag)
-        new_tags = list(set(tags))
-        self.tags = new_tags
-
-    def set_response(self, code: int, response: Union[Type[Serializer], str, Dict]):
-        if response is Type[Serializer]:
-            response = Response('', response)
-        self.responses[code] = response
-
-    def get_path_param_converter(self, param_type: str) -> str:
-        rules = {
-            APIParamDataType.STRING.value: 'str',
-            APIParamDataType.INTEGER.value: 'int'
-        }
-        return rules[param_type]
-
-    def get_full_route(self) -> str:
-        if self.full_route != '':
-            return self.full_route
-        if self.base_url.endswith('/'):
-            base_url = self.base_url[:-1]
-        else:
-            base_url = self.base_url
-        full_route = f'{base_url}/{self.rest_api_version}/{self.endpoint}'
-        path_parameters = [param for param in self.parameters if param.in_ == ParameterType.PATH_PARAM.value]
-        for param in path_parameters:
-            full_route = full_route + f'/<{self.get_path_param_converter(param.type)}:{param.name}>'
-        return full_route
+from typing import Literal, List, Union, Dict, Type
+from drf_yasg.openapi import Parameter, Schema, Response
+from sdrf.enums import ParameterType, APIParamDataType
+from rest_framework.serializers import Serializer
+from rest_framework.authentication import BaseAuthentication
+from rest_framework.permissions import IsAuthenticated, BasePermission
+from django.conf import settings
+from sdrf.utils.settings_utils import get_settings_value
+
+class APIEndpointConfig:
+    def __init__(self, name: str) -> None:
+        super().__init__()
+        self.name = name
+        self.parameters = []
+        self.tags = []
+        self.responses = {}
+        self.permission_classes = []
+        self.authentication_classes = []
+
+    name: str
+    description: str = ''
+    summary: str = ''
+    http_method: Literal['GET', 'POST', 'PUT', 'PATCH', 'DELETE'] = 'GET'
+    parameters: List[Parameter] = []
+    responses: Dict = {}
+    tags: List[str] = []
+    request_body: Schema = None
+    base_url: str = get_settings_value('REST_APP_BASE_URL','rest/')
+    rest_api_version = get_settings_value('REST_APP_VERSION','v1')
+    endpoint: str = ''
+    full_route: str = ''
+    deprecated: bool = False
+    authentication_classes: List = []
+    permission_classes: List = []
+
+    def require_authenticated_permission(self):
+        self.add_permission_class(IsAuthenticated)
+
+    def add_permission_class(self, permission_class):
+        assert issubclass(permission_class, BasePermission), 'Permission Class should be of type BasePermission'
+        self.permission_classes.append(permission_class)
+
+    def add_authentication_class(self, authentication_class):
+        assert issubclass(authentication_class, BaseAuthentication), 'Permission Class should be an instance of ' \
+                                                                     'BaseAuthentication '
+        self.authentication_classes.append(authentication_class)
+
+    def add_parameter(self,
+                      name: str,
+                      data_type: APIParamDataType = APIParamDataType.STRING,
+                      parameter_type: ParameterType = ParameterType.QUERY_PARAM,
+                      description: str = '',
+                      required: bool = True,
+                      default=None):
+        if parameter_type.value == ParameterType.BODY_PARAM.value:
+            if self.request_body is None:
+                self.request_body = Schema(type=APIParamDataType.OBJECT.value, required=[], properties={})
+            self.request_body.properties[name] = Schema(type=data_type.value)
+            if required:
+                self.request_body.required.append(name)
+
+        else:
+            param = Parameter(name=name,
+                              description=description,
+                              in_=parameter_type.value,
+                              type=data_type.value,
+                              required=required,
+                              default=default)
+            self.parameters.append(param)
+
+    def add_tag(self, tag: str):
+        tags = self.tags
+        tags.append(tag)
+        new_tags = list(set(tags))
+        self.tags = new_tags
+
+    def set_response(self, code: int, response: Union[Type[Serializer], str, Dict]):
+        if response is Type[Serializer]:
+            response = Response('', response)
+        self.responses[code] = response
+
+    def get_path_param_converter(self, param_type: str) -> str:
+        rules = {
+            APIParamDataType.STRING.value: 'str',
+            APIParamDataType.INTEGER.value: 'int'
+        }
+        return rules[param_type]
+
+    def get_full_route(self) -> str:
+        if self.full_route != '':
+            return self.full_route
+        if self.base_url.endswith('/'):
+            base_url = self.base_url[:-1]
+        else:
+            base_url = self.base_url
+        full_route = f'{base_url}/{self.rest_api_version}/{self.endpoint}'
+        path_parameters = [param for param in self.parameters if param.in_ == ParameterType.PATH_PARAM.value]
+        for param in path_parameters:
+            full_route = full_route + f'/<{self.get_path_param_converter(param.type)}:{param.name}>'
+        return full_route
```

