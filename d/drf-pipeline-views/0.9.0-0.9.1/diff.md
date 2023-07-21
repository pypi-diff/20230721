# Comparing `tmp/drf_pipeline_views-0.9.0.tar.gz` & `tmp/drf_pipeline_views-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_pipeline_views-0.9.0.tar", max compression
+gzip compressed data, was "drf_pipeline_views-0.9.1.tar", max compression
```

## Comparing `drf_pipeline_views-0.9.0.tar` & `drf_pipeline_views-0.9.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1069 2023-05-06 13:01:05.761154 drf_pipeline_views-0.9.0/LICENSE
--rw-r--r--   0        0        0     3754 2023-05-06 13:01:05.761154 drf_pipeline_views-0.9.0/README.md
--rw-r--r--   0        0        0      193 2023-05-06 13:01:05.761154 drf_pipeline_views-0.9.0/pipeline_views/__init__.py
--rw-r--r--   0        0        0      478 2023-05-06 13:01:05.761154 drf_pipeline_views-0.9.0/pipeline_views/exceptions.py
--rw-r--r--   0        0        0     3554 2023-05-06 13:01:05.761154 drf_pipeline_views-0.9.0/pipeline_views/meta.py
--rw-r--r--   0        0        0        0 2023-05-06 13:01:05.761154 drf_pipeline_views-0.9.0/pipeline_views/py.typed
--rw-r--r--   0        0        0     3889 2023-05-06 13:01:05.761154 drf_pipeline_views-0.9.0/pipeline_views/serializers.py
--rw-r--r--   0        0        0     1584 2023-05-06 13:01:05.761154 drf_pipeline_views-0.9.0/pipeline_views/typing.py
--rw-r--r--   0        0        0     3762 2023-05-06 13:01:05.761154 drf_pipeline_views-0.9.0/pipeline_views/utils.py
--rw-r--r--   0        0        0     6822 2023-05-06 13:01:05.761154 drf_pipeline_views-0.9.0/pipeline_views/views.py
--rw-r--r--   0        0        0     4423 2023-05-06 13:01:05.765154 drf_pipeline_views-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     5713 1970-01-01 00:00:00.000000 drf_pipeline_views-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-21 13:14:28.079141 drf_pipeline_views-0.9.1/LICENSE
+-rw-r--r--   0        0        0     3754 2023-07-21 13:14:28.079141 drf_pipeline_views-0.9.1/README.md
+-rw-r--r--   0        0        0      171 2023-07-21 13:14:28.079141 drf_pipeline_views-0.9.1/pipeline_views/__init__.py
+-rw-r--r--   0        0        0      536 2023-07-21 13:14:28.079141 drf_pipeline_views-0.9.1/pipeline_views/exceptions.py
+-rw-r--r--   0        0        0     3591 2023-07-21 13:14:28.083141 drf_pipeline_views-0.9.1/pipeline_views/meta.py
+-rw-r--r--   0        0        0        0 2023-07-21 13:14:28.083141 drf_pipeline_views-0.9.1/pipeline_views/py.typed
+-rw-r--r--   0        0        0     3901 2023-07-21 13:14:28.083141 drf_pipeline_views-0.9.1/pipeline_views/serializers.py
+-rw-r--r--   0        0        0     1563 2023-07-21 13:14:28.083141 drf_pipeline_views-0.9.1/pipeline_views/typing.py
+-rw-r--r--   0        0        0     3787 2023-07-21 13:14:28.083141 drf_pipeline_views-0.9.1/pipeline_views/utils.py
+-rw-r--r--   0        0        0     7025 2023-07-21 13:14:28.083141 drf_pipeline_views-0.9.1/pipeline_views/views.py
+-rw-r--r--   0        0        0     5613 2023-07-21 13:14:28.083141 drf_pipeline_views-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     5513 1970-01-01 00:00:00.000000 drf_pipeline_views-0.9.1/PKG-INFO
```

### Comparing `drf_pipeline_views-0.9.0/LICENSE` & `drf_pipeline_views-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_pipeline_views-0.9.0/README.md` & `drf_pipeline_views-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `drf_pipeline_views-0.9.0/pipeline_views/meta.py` & `drf_pipeline_views-0.9.1/pipeline_views/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from typing import TYPE_CHECKING
+
 from django.utils.encoding import force_str
 from rest_framework.fields import DictField, Field, SerializerMethodField
 from rest_framework.metadata import SimpleMetadata
 from rest_framework.request import Request, clone_request
 from rest_framework.serializers import (
     HiddenField,
     ListSerializer,
     ManyRelatedField,
     ReadOnlyField,
     RelatedField,
     Serializer,
 )
 
-from .typing import TYPE_CHECKING, Any, ClassVar, Union
+from .typing import Any, ClassVar, Union
 
 if TYPE_CHECKING:
     from .views import BasePipelineView
 
 
 __all__ = [
     "PipelineMetadata",
@@ -28,15 +30,15 @@
     the serializers for that method.
     """
 
     recognized_methods: ClassVar[set[str]] = {"GET", "POST", "PUT", "PATCH", "DELETE"}
     skip_fields: ClassVar[set[type[Field]]] = {ReadOnlyField, HiddenField, SerializerMethodField}
     used_attrs: ClassVar[list[str]] = ["label", "help_text", "min_length", "max_length", "min_value", "max_value"]
 
-    def determine_actions(self, request: Request, view: "BasePipelineView"):
+    def determine_actions(self, request: Request, view: "BasePipelineView") -> dict[str, Any]:
         """Return information about the fields that are accepted for methods in self.recognized_methods."""
         actions = {}
         for method in self.recognized_methods & set(view.allowed_methods):
             view.request = clone_request(request, method)
 
             input_serializer = view.get_serializer()
             output_serializer = view.get_serializer(output=True)
```

### Comparing `drf_pipeline_views-0.9.0/pipeline_views/serializers.py` & `drf_pipeline_views-0.9.1/pipeline_views/serializers.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         request: Optional[Request] = self.context.get("request")
         if request is None or not isinstance(request, Request):
             raise ValidationError(
                 {
                     api_settings.NON_FIELD_ERRORS_KEY: ErrorDetail(
                         string="Must include a Request object in the context of the Serializer.",
                         code="request_missing",
-                    )
-                }
+                    ),
+                },
             )
         return request
 
 
 class HeaderSerializerMixin(RequestFromContextMixin):
     take_from_headers: ClassVar[list[str]] = []
     """Headers to take values from.
@@ -49,15 +49,15 @@
         return data
 
     def to_internal_value(self, data: dict[str, Any]) -> dict[str, Any]:
         ret = super().to_internal_value(data)
         ret = self.add_headers(ret)
         return ret
 
-    def to_representation(self, instance) -> dict[str, Any]:
+    def to_representation(self, instance: Any) -> dict[str, Any]:
         ret = super().to_representation(instance)
         ret = self.add_headers(ret)
         return ret
 
 
 class CookieSerializerMixin(RequestFromContextMixin):
     take_from_cookies: ClassVar[list[str]] = []
@@ -78,15 +78,15 @@
         return data
 
     def to_internal_value(self, data: dict[str, Any]) -> dict[str, Any]:
         ret = super().to_internal_value(data)
         ret = self.add_cookies(ret)
         return ret
 
-    def to_representation(self, instance) -> dict[str, Any]:
+    def to_representation(self, instance: Any) -> dict[str, Any]:
         ret = super().to_representation(instance)
         ret = self.add_cookies(ret)
         return ret
 
 
 class HeaderAndCookieSerializer(HeaderSerializerMixin, CookieSerializerMixin, serializers.Serializer):
     """Serializer that adds the specified headers and cookies from request to the serializer data.
```

### Comparing `drf_pipeline_views-0.9.0/pipeline_views/typing.py` & `drf_pipeline_views-0.9.1/pipeline_views/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     "ClassVar",
     "Generator",
     "Iterable",
     "Literal",
     "Optional",
     "ParamSpec",
     "Protocol",
-    "TYPE_CHECKING",
     "TypeAlias",
     "TypedDict",
     "TypeGuard",
     "TypeVar",
     "Union",
 ]
```

### Comparing `drf_pipeline_views-0.9.0/pipeline_views/utils.py` & `drf_pipeline_views-0.9.1/pipeline_views/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import asyncio
 from contextlib import contextmanager
 from functools import wraps
 from itertools import chain
+from typing import TYPE_CHECKING
 
 from django.conf import settings
 from django.utils.translation import get_language as current_language
 from django.utils.translation import override
 from rest_framework.request import Request
 from rest_framework.response import Response
 from rest_framework.serializers import BaseSerializer
 
 try:
     from pydantic import BaseModel
 except ImportError:
     BaseModel = None
 
 from .typing import (
-    TYPE_CHECKING,
     Any,
     Callable,
     DataDict,
     Generator,
     GenericView,
     HTTPMethod,
     LogicCallable,
@@ -55,15 +55,15 @@
     """Sentinel value."""
 
 
 def is_serializer_class(obj: Any) -> TypeGuard[BaseSerializer]:
     return isinstance(obj, type) and issubclass(obj, BaseSerializer)
 
 
-def is_pydantic_model(obj: Any):
+def is_pydantic_model(obj: Any) -> bool:
     if BaseModel is None:  # pragma: no cover
         return False
 
     return isinstance(obj, type) and issubclass(obj, BaseModel)
 
 
 def get_language(request: Request) -> str:
@@ -92,45 +92,46 @@
             request = None
             for arg in chain(args, kwargs.values()):
                 if isinstance(arg, Request):
                     request = arg
                     break
 
             if request is None:
-                raise ValueError("No Request-object in function parameters.")
+                msg = "No Request-object in function parameters."
+                raise ValueError(msg)
 
             with override(get_language(request)):
-                return item(*args, **kwargs)  # type: ignore
+                return item(*args, **kwargs)
 
         return decorator
 
     @contextmanager
     def context_manager(request: Request) -> Generator[Any, Any, None]:
         with override(get_language(request)):
             yield
 
     return context_manager(item)
 
 
 async def run_parallel(step: tuple[Union[LogicCallable, SerializerType], ...], data: DataDict) -> tuple[DataDict, ...]:
-    return await asyncio.gather(*(task(**data) for task in step))  # noqa
+    return await asyncio.gather(*(task(**data) for task in step))
 
 
 def get_view_method(method: HTTPMethod) -> GenericView:
     source = "query_params" if method == "GET" else "data"
 
     def inner(
         self: "BasePipelineView",
         request: Request,
-        *args: Any,
+        *args: Any,  # noqa: ARG001
         **kwargs: Any,
     ) -> Response:
         kwargs.update(
             {
                 key: value
                 for key, value in getattr(request, source, {}).items()
                 if key not in getattr(self, f"ignored_{method.lower()}_params", set())
-            }
+            },
         )
         return self.process_request(data=kwargs)
 
-    return inner  # type: ignore
+    return inner
```

### Comparing `drf_pipeline_views-0.9.0/pipeline_views/views.py` & `drf_pipeline_views-0.9.1/pipeline_views/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 
 from asgiref.sync import async_to_sync
-from openapi_schema.schema import APISchema
+from openapi_schema import OpenAPISchema
 from rest_framework import status
 from rest_framework.response import Response
 from rest_framework.serializers import Serializer
 from rest_framework.views import APIView
 from serializer_inference import serializer_from_callable
 
 from .exceptions import NextLogicBlock
@@ -29,24 +29,24 @@
 ]
 
 
 class BasePipelineView(APIView):
     pipelines: ClassVar[PipelinesDict] = {}
     """Dictionary describing the HTTP method pipelines."""
 
-    schema = APISchema()
+    schema = OpenAPISchema()
     metadata_class = PipelineMetadata
 
     ignored_get_params: ClassVar[set[str]] = {"lang", "format"}
     ignored_post_params: ClassVar[set[str]] = {"csrfmiddlewaretoken", "lang", "format"}
     ignored_put_params: ClassVar[set[str]] = {"lang", "format"}
     ignored_patch_params: ClassVar[set[str]] = {"lang", "format"}
     ignored_delete_params: ClassVar[set[str]] = {"lang", "format"}
 
-    def __new__(cls, *args, **kwargs):
+    def __new__(cls, *args: Any, **kwargs: Any) -> "BasePipelineView":  # noqa: ARG003,
         for key in cls.pipelines:
             if not hasattr(cls, key.lower()):
                 setattr(cls, key.lower(), get_view_method(key))
 
         return super().__new__(cls)
 
     def process_request(self, data: DataDict) -> Response:
@@ -59,64 +59,67 @@
         if data:
             return Response(data=data, status=status.HTTP_200_OK)
         return Response(status=status.HTTP_204_NO_CONTENT)
 
     def get_pipeline_for_current_request_method(self) -> PipelineLogic:
         """Get pipeline for the current HTTP method."""
         try:
-            return self.pipelines[self.request.method]  # type: ignore
+            return self.pipelines[self.request.method]
         except KeyError as missing_method:
-            raise KeyError(f"Pipeline not configured for HTTP method '{self.request.method}'") from missing_method
+            msg = f"Pipeline not configured for HTTP method '{self.request.method}'"
+            raise KeyError(msg) from missing_method
 
-    def run_logic(self, logic: PipelineLogic, data: DataDict) -> DataReturn:  # noqa: C901
+    def run_logic(self, logic: PipelineLogic, data: DataDict) -> DataReturn:  # noqa: C901,PLR0912
         """Run pipeline logic recursively."""
         if callable(logic):
             if asyncio.iscoroutinefunction(logic):
                 logic = async_to_sync(logic)
 
             return logic(**data)
 
         try:
             for step in logic:
                 # Conditional logic path
                 if isinstance(data, tuple):
                     key, data = data
                     try:
-                        step = step[key]
+                        step = step[key]  # noqa: PLW2901
                     except (KeyError, TypeError) as error:
-                        raise TypeError(f"Next logic step doesn't have a conditional logic path '{key}'.") from error
+                        msg = f"Next logic step doesn't have a conditional logic path '{key}'."
+                        raise TypeError(msg) from error
 
                 # Serializer
                 if is_serializer_class(step):
                     data = self.run_serializer(serializer_class=step, data=data)
 
                 # Pydantic Model
                 elif is_pydantic_model(step):
                     data = self.run_model(model_class=step, data=data)
 
                 # Parallel block
                 elif isinstance(step, tuple):
                     old_kwargs: Optional[DataDict] = None
                     if ... in step:
-                        step = tuple(task for task in step if task is not ...)
+                        step = tuple(task for task in step if task is not ...)  # noqa: PLW2901
                         old_kwargs = data
 
                     results: tuple[DataDict, ...] = async_to_sync(run_parallel)(step, data)
                     data = {key: value for result in results for key, value in result.items()}
 
                     if old_kwargs is not None:
                         old_kwargs.update(data)
                         data = old_kwargs
 
                 # Logic block or callable
                 elif isinstance(step, list) or callable(step):
                     data = self.run_logic(logic=step, data=data if data is not None else {})
 
                 else:
-                    raise TypeError("Only Serializers, Pydantic Models, and callables are supported in the pipeline.")
+                    msg = "Only Serializers, Pydantic Models, and callables are supported in the pipeline."
+                    raise TypeError(msg)
 
         except NextLogicBlock as premature_return:
             return premature_return.output
 
         return data
 
     def run_serializer(self, serializer_class: SerializerType, data: DataDict) -> DataDict:
@@ -139,15 +142,15 @@
         serializer_class: SerializerType = kwargs.pop("serializer_class")
         kwargs.setdefault("context", self.get_serializer_context())
         kwargs.setdefault("many", getattr(serializer_class, "many", False))
         if kwargs.get("data", Sentinel) is None:
             kwargs["data"] = [] if kwargs["many"] else {}
         return serializer_class(*args, **kwargs)
 
-    def get_serializer_class(self, output: bool = False) -> SerializerType:
+    def get_serializer_class(self, output: bool = False) -> SerializerType:  # noqa: FBT001,FBT002
         """Get the first step in the current HTTP method's pipeline.
         If it's a Serializer, return it. Otherwise, try to infer a serializer from the
         logic callable's parameters.
         """
         step = self.get_pipeline_for_current_request_method()
 
         while isinstance(step, Iterable):
@@ -165,12 +168,13 @@
 
         if is_pydantic_model(step):  # pragma: no cover
             return serializer_from_callable(step)
 
         if callable(step):
             return serializer_from_callable(step, output=output)
 
-        raise TypeError("Only Serializers and callables are supported in the pipeline.")
+        msg = "Only Serializers and callables are supported in the pipeline."
+        raise TypeError(msg)
 
     def get_serializer_context(self) -> ViewContext:
         """Return serializer context, mainly for browsable api."""
         return {"request": self.request, "format": self.format_kwarg, "view": self}
```

### Comparing `drf_pipeline_views-0.9.0/PKG-INFO` & `drf_pipeline_views-0.9.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-pipeline-views
-Version: 0.9.0
+Version: 0.9.1
 Summary: Django REST framework views using the pipeline pattern.
 Home-page: https://github.com/MrThearMan/drf-pipeline-views
 License: MIT
 Keywords: django,djangorestframework,drf,pipeline,views
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.9,<4
@@ -18,19 +18,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: pydantic
 Provides-Extra: uritemplate
 Provides-Extra: uvloop
 Requires-Dist: Django (>=3.2)
 Requires-Dist: PyYAML (>=6.0)
 Requires-Dist: asgiref (>=3.5.0)
 Requires-Dist: djangorestframework (>=3.12.0)
```

