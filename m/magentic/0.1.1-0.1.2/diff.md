# Comparing `tmp/magentic-0.1.1.tar.gz` & `tmp/magentic-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magentic-0.1.1.tar", max compression
+gzip compressed data, was "magentic-0.1.2.tar", max compression
```

## Comparing `magentic-0.1.1.tar` & `magentic-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1069 2023-06-18 04:31:45.568698 magentic-0.1.1/LICENSE
--rw-r--r--   0        0        0     4936 2023-07-15 16:45:38.068501 magentic-0.1.1/README.md
--rw-r--r--   0        0        0      922 2023-07-17 06:22:04.852150 magentic-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      139 2023-07-15 07:11:09.503451 magentic-0.1.1/src/magentic/__init__.py
--rw-r--r--   0        0        0     2100 2023-07-15 07:11:09.503748 magentic-0.1.1/src/magentic/chat.py
--rw-r--r--   0        0        0        0 2023-07-15 07:11:09.503836 magentic-0.1.1/src/magentic/chat_model/__init__.py
--rw-r--r--   0        0        0     1517 2023-07-16 21:00:12.901908 magentic-0.1.1/src/magentic/chat_model/base.py
--rw-r--r--   0        0        0     9687 2023-07-17 06:21:54.657860 magentic-0.1.1/src/magentic/chat_model/openai_chat_model.py
--rw-r--r--   0        0        0     1019 2023-07-15 07:11:09.512404 magentic-0.1.1/src/magentic/function_call.py
--rw-r--r--   0        0        0     1712 2023-07-15 07:11:09.513068 magentic-0.1.1/src/magentic/prompt_chain.py
--rw-r--r--   0        0        0     3271 2023-07-16 20:42:38.366497 magentic-0.1.1/src/magentic/prompt_function.py
--rw-r--r--   0        0        0       61 2023-07-15 07:11:09.514294 magentic-0.1.1/src/magentic/py.typed
--rw-r--r--   0        0        0     1584 2023-07-17 05:50:31.713612 magentic-0.1.1/src/magentic/typing.py
--rw-r--r--   0        0        0     5529 1970-01-01 00:00:00.000000 magentic-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-18 04:31:45.568698 magentic-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5156 2023-07-21 07:11:25.073401 magentic-0.1.2/README.md
+-rw-r--r--   0        0        0     1023 2023-07-21 07:35:56.486824 magentic-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      139 2023-07-15 07:11:09.503451 magentic-0.1.2/src/magentic/__init__.py
+-rw-r--r--   0        0        0     2100 2023-07-15 07:11:09.503748 magentic-0.1.2/src/magentic/chat.py
+-rw-r--r--   0        0        0        0 2023-07-15 07:11:09.503836 magentic-0.1.2/src/magentic/chat_model/__init__.py
+-rw-r--r--   0        0        0     1517 2023-07-16 21:00:12.901908 magentic-0.1.2/src/magentic/chat_model/base.py
+-rw-r--r--   0        0        0     9536 2023-07-21 05:15:28.116776 magentic-0.1.2/src/magentic/chat_model/openai_chat_model.py
+-rw-r--r--   0        0        0     1348 2023-07-21 05:14:05.054740 magentic-0.1.2/src/magentic/function_call.py
+-rw-r--r--   0        0        0     1712 2023-07-15 07:11:09.513068 magentic-0.1.2/src/magentic/prompt_chain.py
+-rw-r--r--   0        0        0     3271 2023-07-16 20:42:38.366497 magentic-0.1.2/src/magentic/prompt_function.py
+-rw-r--r--   0        0        0       61 2023-07-15 07:11:09.514294 magentic-0.1.2/src/magentic/py.typed
+-rw-r--r--   0        0        0     1584 2023-07-17 05:50:31.713612 magentic-0.1.2/src/magentic/typing.py
+-rw-r--r--   0        0        0     5749 1970-01-01 00:00:00.000000 magentic-0.1.2/PKG-INFO
```

### Comparing `magentic-0.1.1/LICENSE` & `magentic-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `magentic-0.1.1/README.md` & `magentic-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 poetry add magentic
 ```
 
 Configure your OpenAI API key by setting the `OPENAI_API_KEY` environment variable or using `openai.api_key = "sk-..."`. See the [OpenAI Python library documentation](https://github.com/openai/openai-python#usage) for more information.
 
 ## Usage
 
-The `@prompt` decorator allows you to define a template for a Large Language Model (LLM) prompt as a Python function.
+The `@prompt` decorator allows you to define a template for a Large Language Model (LLM) prompt as a Python function. When this function is called, the arguments are inserted into the template, then this prompt is sent to an LLM which generates the function output.
 
 ```python
 from magentic import prompt
 
 
-@prompt("What is a good name for a company that makes {product}?")
-def get_company_name(product: str) -> str:
-    ...  # No code required!
+@prompt('Add more "dude"ness to: {phrase}')
+def dudeify(phrase: str) -> str:
+    ...  # No function body as this is never executed
 
 
-get_company_name(product="colorful socks")
-# 'Colorful Threads'
+dudeify("Hello, how are you?")
+# "Hey, dude! What's up? How's it going, my man?"
 ```
 
 The `@prompt` decorator will respect the return type annotation of the decorated function. This can be [any type supported by pydantic](https://docs.pydantic.dev/latest/usage/types/types/) including a `pydantic` model.
 
 ```python
 from magentic import prompt
 from pydantic import BaseModel
@@ -79,15 +79,15 @@
 # FunctionCall(<function activate_oven at 0x1105a6200>, temperature=350, mode='bake')
 output()
 # 'Preheating to 350 F with mode bake'
 ```
 
 Sometimes the LLM requires making one or more function calls to generate a final answer. The `@prompt_chain` decorator will resolve `FunctionCall` objects automatically and pass the output back to the LLM to continue until the final answer is reached.
 
-In the following example the LLM first calls the `get_current_weather` function, then uses the result to formulate its final answer.
+In the following example, when `describe_weather` is called the LLM first calls the `get_current_weather` function, then uses the result of this to formulate its final answer which gets returned.
 
 ```python
 from magentic import prompt_chain
 
 
 def get_current_weather(location, unit="fahrenheit"):
     """Get the current weather in a given location"""
```

### Comparing `magentic-0.1.1/pyproject.toml` & `magentic-0.1.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 check_untyped_defs = true
 disable_error_code = ["empty-body"]
 disallow_untyped_defs = false
 strict = true
 
 [tool.poetry]
 name = "magentic"
-version = "0.1.1"
+version = "0.1.2"
 description = "Seamlessly integrate LLMs as Python functions"
 license = "MIT"
 authors = ["Jack Collins"]
 readme = "README.md"
 repository = "https://github.com/jackmpcollins/magentic"
 
 [tool.poetry.dependencies]
@@ -30,16 +30,21 @@
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 isort = "*"
 mypy = "*"
 pytest = "*"
 pytest-clarity = "*"
+pytest-cov = "*"
+
+[tool.poetry.group.examples.dependencies]
+jupyter = "*"
 
 [tool.pytest.ini_options]
+addopts = "--cov=magentic"
 markers = [
     "openai: Tests that query the OpenAI API"
 ]
 
 [tool.ruff]
 line-length = 120
```

### Comparing `magentic-0.1.1/src/magentic/chat.py` & `magentic-0.1.2/src/magentic/chat.py`

 * *Files identical despite different names*

### Comparing `magentic-0.1.1/src/magentic/chat_model/base.py` & `magentic-0.1.2/src/magentic/chat_model/base.py`

 * *Files identical despite different names*

### Comparing `magentic-0.1.1/src/magentic/chat_model/openai_chat_model.py` & `magentic-0.1.2/src/magentic/chat_model/openai_chat_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         model_schema["properties"] = model_schema.get("properties", {})
         return model_schema
 
     def parse_args(self, arguments: str) -> T:
         return self._type_adapter.validate_json(arguments)
 
     def serialize_args(self, value: T) -> str:
-        return json.dumps(value)
+        return self._type_adapter.dump_json(value).decode()
 
 
 BaseModelT = TypeVar("BaseModelT", bound=BaseModel)
 
 
 class BaseModelFunctionSchema(BaseFunctionSchema[BaseModelT], Generic[BaseModelT]):
     def __init__(self, model: type[BaseModelT]):
@@ -152,15 +152,15 @@
     @property
     def parameters(self) -> dict[str, Any]:
         schema: dict[str, Any] = self._model.model_json_schema().copy()
         schema.pop("title", None)
         return schema
 
     def parse_args(self, arguments: str) -> FunctionCall[T]:
-        args = self._model.model_validate_json(arguments).model_dump()
+        args = self._model.model_validate_json(arguments).model_dump(exclude_unset=True)
         return FunctionCall(self._func, **args)
 
     def parse_args_to_message(self, arguments: str) -> FunctionCallMessage[T]:
         return FunctionCallMessage(self.parse_args(arguments))
 
     def serialize_args(self, value: FunctionCall[T]) -> str:
         return json.dumps(value.arguments)
@@ -236,23 +236,19 @@
         functions: Iterable[Callable[..., FuncR]] | None = None,
         output_types: Iterable[type[R | str]] | None = None,
     ) -> FunctionCallMessage[FuncR] | AssistantMessage[R]:
         """Request an LLM message."""
         if output_types is None:
             output_types = [str]
 
-        function_schemas: list[
-            FunctionCallFunctionSchema[FuncR] | BaseFunctionSchema[R]
-        ] = []
-        for function in functions or []:
-            function_schemas.append(FunctionCallFunctionSchema(function))
-        for output_type in output_types:
-            if issubclass(output_type, str):
-                continue
-            function_schemas.append(function_schema_for_type(output_type))
+        function_schemas = [FunctionCallFunctionSchema(f) for f in functions or []] + [
+            function_schema_for_type(type_)
+            for type_ in output_types
+            if not issubclass(type_, str)
+        ]
 
         includes_str_output_type = any(issubclass(cls, str) for cls in output_types)
 
         # `openai.ChatCompletion.create` doesn't accept `None`
         # so only pass function args if there are functions
         function_args: dict[str, Any] = {}
         if function_schemas:
```

### Comparing `magentic-0.1.1/src/magentic/function_call.py` & `magentic-0.1.2/src/magentic/function_call.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,24 @@
         self._function = function
         self._args = args
         self._kwargs = kwargs
 
     def __call__(self) -> T:
         return self._function(*self._args, **self._kwargs)
 
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, type(self)):
+            return NotImplemented
+        return (
+            type(self) is type(other)
+            and self._function == other._function
+            and self._args == other._args
+            and self._kwargs == other._kwargs
+        )
+
     def __repr__(self) -> str:
         args_kwargs_repr = ", ".join(
             [
                 *(repr(arg) for arg in self._args),
                 *(f"{key}={value!r}" for key, value in self._kwargs.items()),
             ]
         )
```

### Comparing `magentic-0.1.1/src/magentic/prompt_chain.py` & `magentic-0.1.2/src/magentic/prompt_chain.py`

 * *Files identical despite different names*

### Comparing `magentic-0.1.1/src/magentic/prompt_function.py` & `magentic-0.1.2/src/magentic/prompt_function.py`

 * *Files identical despite different names*

### Comparing `magentic-0.1.1/src/magentic/typing.py` & `magentic-0.1.2/src/magentic/typing.py`

 * *Files identical despite different names*

### Comparing `magentic-0.1.1/PKG-INFO` & `magentic-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magentic
-Version: 0.1.1
+Version: 0.1.2
 Summary: Seamlessly integrate LLMs as Python functions
 Home-page: https://github.com/jackmpcollins/magentic
 License: MIT
 Author: Jack Collins
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -29,27 +29,27 @@
 poetry add magentic
 ```
 
 Configure your OpenAI API key by setting the `OPENAI_API_KEY` environment variable or using `openai.api_key = "sk-..."`. See the [OpenAI Python library documentation](https://github.com/openai/openai-python#usage) for more information.
 
 ## Usage
 
-The `@prompt` decorator allows you to define a template for a Large Language Model (LLM) prompt as a Python function.
+The `@prompt` decorator allows you to define a template for a Large Language Model (LLM) prompt as a Python function. When this function is called, the arguments are inserted into the template, then this prompt is sent to an LLM which generates the function output.
 
 ```python
 from magentic import prompt
 
 
-@prompt("What is a good name for a company that makes {product}?")
-def get_company_name(product: str) -> str:
-    ...  # No code required!
+@prompt('Add more "dude"ness to: {phrase}')
+def dudeify(phrase: str) -> str:
+    ...  # No function body as this is never executed
 
 
-get_company_name(product="colorful socks")
-# 'Colorful Threads'
+dudeify("Hello, how are you?")
+# "Hey, dude! What's up? How's it going, my man?"
 ```
 
 The `@prompt` decorator will respect the return type annotation of the decorated function. This can be [any type supported by pydantic](https://docs.pydantic.dev/latest/usage/types/types/) including a `pydantic` model.
 
 ```python
 from magentic import prompt
 from pydantic import BaseModel
@@ -96,15 +96,15 @@
 # FunctionCall(<function activate_oven at 0x1105a6200>, temperature=350, mode='bake')
 output()
 # 'Preheating to 350 F with mode bake'
 ```
 
 Sometimes the LLM requires making one or more function calls to generate a final answer. The `@prompt_chain` decorator will resolve `FunctionCall` objects automatically and pass the output back to the LLM to continue until the final answer is reached.
 
-In the following example the LLM first calls the `get_current_weather` function, then uses the result to formulate its final answer.
+In the following example, when `describe_weather` is called the LLM first calls the `get_current_weather` function, then uses the result of this to formulate its final answer which gets returned.
 
 ```python
 from magentic import prompt_chain
 
 
 def get_current_weather(location, unit="fahrenheit"):
     """Get the current weather in a given location"""
```

