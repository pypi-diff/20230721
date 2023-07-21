# Comparing `tmp/easycompletion-0.2.6.tar.gz` & `tmp/easycompletion-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycompletion-0.2.6.tar", last modified: Thu Jul 20 13:29:23 2023, max compression
+gzip compressed data, was "easycompletion-0.2.7.tar", last modified: Fri Jul 21 12:25:37 2023, max compression
```

## Comparing `easycompletion-0.2.6.tar` & `easycompletion-0.2.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:29:23.053725 easycompletion-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-20 13:29:10.000000 easycompletion-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-07-20 13:29:23.053725 easycompletion-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-07-20 13:29:10.000000 easycompletion-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:29:23.049725 easycompletion-0.2.6/easycompletion/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-20 13:29:10.000000 easycompletion-0.2.6/easycompletion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-20 13:29:10.000000 easycompletion-0.2.6/easycompletion/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    14849 2023-07-20 13:29:10.000000 easycompletion-0.2.6/easycompletion/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-07-20 13:29:10.000000 easycompletion-0.2.6/easycompletion/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:29:23.053725 easycompletion-0.2.6/easycompletion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-07-20 13:29:23.000000 easycompletion-0.2.6/easycompletion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 13:29:23.000000 easycompletion-0.2.6/easycompletion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:29:23.000000 easycompletion-0.2.6/easycompletion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-20 13:29:23.000000 easycompletion-0.2.6/easycompletion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 13:29:23.000000 easycompletion-0.2.6/easycompletion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 13:29:23.053725 easycompletion-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-20 13:29:10.000000 easycompletion-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:25:37.958800 easycompletion-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-21 12:25:25.000000 easycompletion-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-07-21 12:25:37.958800 easycompletion-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-07-21 12:25:25.000000 easycompletion-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:25:37.958800 easycompletion-0.2.7/easycompletion/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-21 12:25:25.000000 easycompletion-0.2.7/easycompletion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-21 12:25:25.000000 easycompletion-0.2.7/easycompletion/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-21 12:25:25.000000 easycompletion-0.2.7/easycompletion/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16118 2023-07-21 12:25:25.000000 easycompletion-0.2.7/easycompletion/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-21 12:25:25.000000 easycompletion-0.2.7/easycompletion/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:25:37.958800 easycompletion-0.2.7/easycompletion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-07-21 12:25:37.000000 easycompletion-0.2.7/easycompletion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-21 12:25:37.000000 easycompletion-0.2.7/easycompletion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:25:37.000000 easycompletion-0.2.7/easycompletion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-21 12:25:37.000000 easycompletion-0.2.7/easycompletion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 12:25:37.000000 easycompletion-0.2.7/easycompletion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 12:25:37.958800 easycompletion-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-21 12:25:25.000000 easycompletion-0.2.7/setup.py
```

### Comparing `easycompletion-0.2.6/LICENSE` & `easycompletion-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `easycompletion-0.2.6/PKG-INFO` & `easycompletion-0.2.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,12 @@
-Metadata-Version: 2.1
-Name: easycompletion
-Version: 0.2.6
-Summary: Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
-Home-page: https://github.com/AutonomousResearchGroup/easycompletion
-Author: Moon
-Author-email: shawmakesmagic@gmail.com
-License: MIT
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # easycompletion
 
 Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 
+<img src="resources/image.jpg">
 
 # Installation
 
 ```bash
 pip install easycompletion
 ```
 
@@ -125,15 +108,15 @@
             "description": "Detailed summary of the text.",
         },
     },
     required_properties=["summary"],
 )
 ```
 
-### `openai_text_call(text, model_failure_retries=5, model=None, chunk_length=default_chunk_length, api_key=None)`
+### `openai_text_call(text, model_failure_retries=5, model=None, chunk_length=DEFAULT_CHUNK_LENGTH, api_key=None)`
 
 Sends text to the OpenAI API and returns a text response.
 
 ```python
 response = openai_text_call(
     "Hello, how are you?",
     model_failure_retries=3,
@@ -154,15 +137,15 @@
         "total_tokens": "number"
     },
     "error": "string|None",
     "finish_reason": "string"
 }
 ```
 
-### `openai_function_call(text, functions=None, model_failure_retries=5, function_call=None, function_failure_retries=10, chunk_length=default_chunk_length, model=None, api_key=None)`
+### `openai_function_call(text, functions=None, model_failure_retries=5, function_call=None, function_failure_retries=10, chunk_length=DEFAULT_CHUNK_LENGTH, model=None, api_key=None)`
 
 Sends text and a list of functions to the OpenAI API and returns optional text and a function call. The function call is validated against the functions array.
 
 ```python
 function = {
     'name': 'function1',
     'parameters': {'param1': 'value1'}
@@ -184,39 +167,39 @@
         "total_tokens": "number"
     },
     "finish_reason": "string",
     "error": "string|None"
 }
 ```
 
-### `trim_prompt(text, max_tokens=default_chunk_length, model=default_text_model, preserve_top=True)`
+### `trim_prompt(text, max_tokens=DEFAULT_CHUNK_LENGTH, model=DEFAULT_TEXT_MODEL, preserve_top=True)`
 
 Trim the given text to a maximum number of tokens.
 
 ```python
 trimmed_text = trim_prompt("This is a test.", 3, preserve_top=True)
 ```
 
-### `chunk_prompt(prompt, chunk_length=default_chunk_length)`
+### `chunk_prompt(prompt, chunk_length=DEFAULT_CHUNK_LENGTH)`
 
 Split the given prompt into chunks where each chunk has a maximum number of tokens.
 
 ```python
 prompt_chunks = chunk_prompt("This is a test. I am writing a function.", 4)
 ```
 
-### `count_tokens(prompt, model=default_text_model)`
+### `count_tokens(prompt, model=DEFAULT_TEXT_MODEL)`
 
 Count the number of tokens in a string.
 
 ```python
 num_tokens = count_tokens("This is a test.")
 ```
 
-### `get_tokens(prompt, model=default_text_model)`
+### `get_tokens(prompt, model=DEFAULT_TEXT_MODEL)`
 
 Returns a list of tokens in a string.
 
 ```python
 tokens = get_tokens("This is a test.")
 ```
```

### Comparing `easycompletion-0.2.6/README.md` & `easycompletion-0.2.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,29 @@
+Metadata-Version: 2.1
+Name: easycompletion
+Version: 0.2.7
+Summary: Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
+Home-page: https://github.com/AutonomousResearchGroup/easycompletion
+Author: Moon
+Author-email: shawmakesmagic@gmail.com
+License: MIT
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # easycompletion
 
 Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 
-<img src="resources/image.jpg">
 
 # Installation
 
 ```bash
 pip install easycompletion
 ```
 
@@ -108,15 +125,15 @@
             "description": "Detailed summary of the text.",
         },
     },
     required_properties=["summary"],
 )
 ```
 
-### `openai_text_call(text, model_failure_retries=5, model=None, chunk_length=default_chunk_length, api_key=None)`
+### `openai_text_call(text, model_failure_retries=5, model=None, chunk_length=DEFAULT_CHUNK_LENGTH, api_key=None)`
 
 Sends text to the OpenAI API and returns a text response.
 
 ```python
 response = openai_text_call(
     "Hello, how are you?",
     model_failure_retries=3,
@@ -137,15 +154,15 @@
         "total_tokens": "number"
     },
     "error": "string|None",
     "finish_reason": "string"
 }
 ```
 
-### `openai_function_call(text, functions=None, model_failure_retries=5, function_call=None, function_failure_retries=10, chunk_length=default_chunk_length, model=None, api_key=None)`
+### `openai_function_call(text, functions=None, model_failure_retries=5, function_call=None, function_failure_retries=10, chunk_length=DEFAULT_CHUNK_LENGTH, model=None, api_key=None)`
 
 Sends text and a list of functions to the OpenAI API and returns optional text and a function call. The function call is validated against the functions array.
 
 ```python
 function = {
     'name': 'function1',
     'parameters': {'param1': 'value1'}
@@ -167,39 +184,39 @@
         "total_tokens": "number"
     },
     "finish_reason": "string",
     "error": "string|None"
 }
 ```
 
-### `trim_prompt(text, max_tokens=default_chunk_length, model=default_text_model, preserve_top=True)`
+### `trim_prompt(text, max_tokens=DEFAULT_CHUNK_LENGTH, model=DEFAULT_TEXT_MODEL, preserve_top=True)`
 
 Trim the given text to a maximum number of tokens.
 
 ```python
 trimmed_text = trim_prompt("This is a test.", 3, preserve_top=True)
 ```
 
-### `chunk_prompt(prompt, chunk_length=default_chunk_length)`
+### `chunk_prompt(prompt, chunk_length=DEFAULT_CHUNK_LENGTH)`
 
 Split the given prompt into chunks where each chunk has a maximum number of tokens.
 
 ```python
 prompt_chunks = chunk_prompt("This is a test. I am writing a function.", 4)
 ```
 
-### `count_tokens(prompt, model=default_text_model)`
+### `count_tokens(prompt, model=DEFAULT_TEXT_MODEL)`
 
 Count the number of tokens in a string.
 
 ```python
 num_tokens = count_tokens("This is a test.")
 ```
 
-### `get_tokens(prompt, model=default_text_model)`
+### `get_tokens(prompt, model=DEFAULT_TEXT_MODEL)`
 
 Returns a list of tokens in a string.
 
 ```python
 tokens = get_tokens("This is a test.")
 ```
```

### Comparing `easycompletion-0.2.6/easycompletion/__init__.py` & `easycompletion-0.2.7/easycompletion/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,23 +9,23 @@
     trim_prompt,
     chunk_prompt,
     count_tokens,
     get_tokens,
 )
 
 from .constants import (
-    default_text_model,
-    default_chunk_length,
+    DEFAULT_TEXT_MODEL,
+    DEFAULT_CHUNK_LENGTH,
 )
 
 __all__ = [
     "openai_function_call",
     "openai_text_call",
     "compose_prompt",
     "compose_function",
     "trim_prompt",
     "chunk_prompt",
     "count_tokens",
     "get_tokens",
-    "default_text_model",
-    "default_chunk_length",
+    "DEFAULT_TEXT_MODEL",
+    "DEFAULT_CHUNK_LENGTH",
 ]
```

### Comparing `easycompletion-0.2.6/easycompletion/model.py` & `easycompletion-0.2.7/easycompletion/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,27 +7,30 @@
 
 from dotenv import load_dotenv
 
 # Load environment variables from .env file
 load_dotenv()
 
 from .constants import (
-    default_text_model,
-    long_text_model,
-    openai_api_key,
-    default_chunk_length,
+    DEFAULT_TEXT_MODEL,
+    LONG_TEXT_MODEL,
+    OPENAI_API_KEY,
+    DEFAULT_CHUNK_LENGTH,
+    DEBUG,
 )
 
+from .logger import log
+
 from .prompt import count_tokens
 
 # Set the OpenAI API key
-openai.api_key = openai_api_key
+openai.api_key = OPENAI_API_KEY
 
 
-def parse_arguments(arguments):
+def parse_arguments(arguments, debug=DEBUG):
     """
     Parses arguments that are expected to be either a JSON string, dictionary, or a list.
 
     Parameters:
         arguments (str or dict or list): Arguments in string or dictionary or list format.
 
     Returns:
@@ -35,38 +38,37 @@
 
     Usage:
         arguments = parse_arguments('{"arg1": "value1", "arg2": "value2"}')
     """
     try:
         # Handle string inputs, remove any ellipsis from the string
         if isinstance(arguments, str):
-            arguments = re.sub(r"\.\.\.|\…", "", arguments)
-            return json.loads(arguments)
-        # If input is already a dictionary or list, return as is
-        elif isinstance(arguments, dict) or isinstance(arguments, list):
-            return arguments
+            arguments = json.loads(arguments)
     # If JSON decoding fails, try using ast.literal_eval
     except json.JSONDecodeError:
         try:
-            return ast.literal_eval(arguments)
+            arguments = ast.literal_eval(arguments)
         # If ast.literal_eval fails, remove line breaks and non-ASCII characters and try JSON decoding again
         except (ValueError, SyntaxError):
             try:
+                arguments = re.sub(r"\.\.\.|\…", "", arguments)
                 arguments = re.sub(r"[\r\n]+", "", arguments)
                 arguments = re.sub(r"[^\x00-\x7F]+", "", arguments)
-                return json.loads(arguments)
+                arguments = json.loads(arguments)
             # If everything fails, try Python's eval function
             except (ValueError, SyntaxError):
                 try:
-                    return eval(arguments)
+                    arguments = eval(arguments)
                 except (ValueError, SyntaxError):
-                    return None
+                    arguments = None
+    log(f"Arguments:\n{str(arguments)}", log=debug)
+    return arguments
 
 
-def validate_functions(response, functions, function_call):
+def validate_functions(response, functions, function_call, debug=DEBUG):
     """
     Validates if the function returned by the OpenAI API matches the intended function call.
 
     Parameters:
         response (dict): The response from OpenAI API.
         functions (list): A list of function definitions.
         function_call (dict or str): The expected function call.
@@ -77,54 +79,60 @@
     Usage:
         isValid = validate_functions(response, functions, function_call)
     """
     response_function_call = response["choices"][0]["message"].get(
         "function_call", None
     )
     if response_function_call is None:
+        log("No function call in response", type="error", log=debug)
         return False
 
     # If function_call is not "auto" and the name does not match with the response, return False
     if (
         function_call != "auto"
         and response_function_call["name"] != function_call["name"]
     ):
+        log("Function call does not match", type="error", log=debug)
         return False
 
     # If function_call is "auto", extract the name from the response
     function_call_name = (
         function_call["name"]
         if function_call != "auto"
         else response_function_call["name"]
     )
 
     # Parse the arguments from the response
     arguments = parse_arguments(response_function_call["arguments"])
 
     # If arguments are None, return False
     if arguments is None:
+        log("Arguments are None", type="error", log=debug)
         return False
 
     # Get the function that matches the function name from the list of functions
     function = next(
         (item for item in functions if item["name"] == function_call_name), None
     )
 
     # If no matching function is found, return False
     if function is None:
+        log("No matching function found", type="error", log=debug)
         return False
 
     # Check if the function's argument keys match with the response's argument keys
-    if set(function["parameters"]["properties"].keys()) == set(arguments.keys()):
-        return True
+    if set(function["parameters"]["properties"].keys()) != set(arguments.keys()):
+        log("Argument keys do not match", type="error", log=debug)
+        return False
 
-    return False
+    log("Function call is valid", type="success", log=debug)
+    return True
 
 
-def compose_function(name, description, properties, required_properties):
+def compose_function(name, description, properties, required_properties, debug=DEBUG):
     """
     Composes a function object for OpenAI API.
 
     Parameters:
         name (str): The name of the function.
         description (str): Description of the function.
         properties (dict): Dictionary of property objects.
@@ -142,39 +150,42 @@
                     "type": "string",
                     "description": "Detailed summary of the text.",
                 },
             },
             required_properties=["summary"],
         )
     """
-    return {
+    function = {
         "name": name,
         "description": description,
         "parameters": {
             "type": "object",
             "properties": properties,
             "required": required_properties,
         },
     }
+    log(f"Function:\n{str(function)}", type="info", log=debug)
+    return function
 
 
 def openai_text_call(
     text,
     model_failure_retries=5,
     model=None,
-    chunk_length=default_chunk_length,
+    chunk_length=DEFAULT_CHUNK_LENGTH,
     api_key=None,
+    debug=DEBUG,
 ):
     """
     Function for sending text to the OpenAI API and returning a text response.
 
     Parameters:
         text (str): Text to send to the model.
         model_failure_retries (int, optional): Number of retries if the request fails. Default is 5.
-        model (str, optional): The model to use. Default is the default_text_model defined in constants.py.
+        model (str, optional): The model to use. Default is the DEFAULT_TEXT_MODEL defined in constants.py.
         chunk_length (int, optional): Maximum length of text chunk to process. Default is defined in constants.py.
         api_key (str, optional): OpenAI API key. If not provided, it uses the one defined in constants.py.
 
     Returns:
         str: The response content from the model.
 
     Example:
@@ -183,22 +194,22 @@
 
     # Override the API key if provided as parameter
     if api_key is not None:
         openai.api_key = api_key
 
     # Use the default model if no model is specified
     if model == None:
-        model = default_text_model
+        model = DEFAULT_TEXT_MODEL
 
     # Count tokens in the input text
     total_tokens = count_tokens(text, model=model)
 
     # If text is longer than chunk_length and model is not for long texts, switch to the long text model
     if total_tokens > chunk_length and "16k" not in model:
-        model = long_text_model
+        model = LONG_TEXT_MODEL
         if not os.environ.get("SUPPRESS_WARNINGS"):
             print(
                 "Warning: Message is long. Using 16k model (to hide this message, set SUPPRESS_WARNINGS=1)"
             )
 
     # If text is too long even for long text model, return None
     if total_tokens > (16384 - chunk_length):
@@ -209,26 +220,25 @@
             "finish_reason": None,
             "error": "Message too long",
         }
 
     # Prepare messages for the API call
     messages = [{"role": "user", "content": text}]
 
-    # Try making a request to the OpenAI API
-    def try_request():
-        try:
-            return openai.ChatCompletion.create(model=model, messages=messages)
-        except Exception as e:
-            return None
+    log(f"Prompt:\n{text}", type="prompt", log=debug)
 
     # Try to make a request for a specified number of times
     response = None
     for i in range(model_failure_retries):
-        response = try_request()
-        if response:
+        try:
+            response = openai.ChatCompletion.create(model=model, messages=messages)
+        except Exception as e:
+            log(f"OpenAI Error: {e}", type="error", log=debug)
+            continue
+        if response is not None:
             break
         # wait 1 second
         time.sleep(1)
 
     # If response is not valid, print an error message and return None
     if (
         response is None
@@ -257,31 +267,32 @@
 
 def openai_function_call(
     text,
     functions=None,
     model_failure_retries=5,
     function_call=None,
     function_failure_retries=10,
-    chunk_length=default_chunk_length,
+    chunk_length=DEFAULT_CHUNK_LENGTH,
     model=None,
     api_key=None,
+    debug=DEBUG,
 ):
     """
     Send text and a list of functions to the OpenAI API and return optional text and a function call.
     The function call is validated against the functions array.
     The input text is sent to the chat model and is treated as a user message.
 
     Args:
         text (str): Text that will be sent as the user message to the model.
         functions (list[dict] | dict | None): List of functions or a single function dictionary to be sent to the model.
         model_failure_retries (int): Number of times to retry the request if it fails (default is 5).
         function_call (str | dict | None): 'auto' to let the model decide, or a function name or a dictionary containing the function name (default is "auto").
         function_failure_retries (int): Number of times to retry the request if the function call is invalid (default is 10).
         chunk_length (int): The length of each chunk to be processed.
-        model (str | None): The model to use (default is the default_text_model, i.e. gpt-3.5-turbo).
+        model (str | None): The model to use (default is the DEFAULT_TEXT_MODEL, i.e. gpt-3.5-turbo).
         api_key (str | None): If you'd like to pass in a key to override the environment variable OPENAI_API_KEY.
 
     Returns:
         dict: On most errors, returns a dictionary with an "error" key. On success, returns a dictionary containing
         "text" (response from the model), "function_name" (name of the function called), "arguments" (arguments for the function), "error" (None).
 
     Example:
@@ -315,52 +326,61 @@
     # Set the function call to the name of the function if only one function is provided
     # If there are multiple functions, use "auto"
     if function_call is None:
         function_call = functions[0]["name"] if len(functions) == 1 else "auto"
 
     # Make sure text is provided
     if text is None:
+        log("Text is required", type="error", log=debug)
         return {"error": "text is required"}
 
     # Check if the function call is valid
     if function_call != "auto":
         if isinstance(function_call, str):
             function_call = {"name": function_call}
         elif "name" not in function_call:
+            log("function_call must have a name property", type="error", log=debug)
             return {
                 "error": "function_call had an invalid name. Should be a string of the function name or an object with a name property"
             }
 
     # Use the default text model if no model is specified
     if model is None:
-        model = default_text_model
+        model = DEFAULT_TEXT_MODEL
 
     # Count the number of tokens in the message
     message_tokens = count_tokens(text, model=model)
     total_tokens = message_tokens
 
-    if functions is None:
-        function_call_tokens = count_tokens(functions, model=model)
-        total_tokens += function_call_tokens + 3  # Additional tokens for the user
+    function_call_tokens = count_tokens(functions, model=model)
+    total_tokens += function_call_tokens + 3  # Additional tokens for the user
+
+    log(
+        f"Message tokens: {str(message_tokens)}"
+        + f"\nFunction call tokens: {str(function_call_tokens)}"
+        + f"\nTotal tokens: {str(total_tokens)}",
+        type="info",
+        log=debug,
+    )
 
     # Switch to a larger model if the message is too long for the default model
     if total_tokens > chunk_length and "16k" not in model:
-        model = long_text_model
-        if not os.environ.get("SUPPRESS_WARNINGS"):
-            print(
-                "Warning: Message is long. Using 16k model (to hide this message, set SUPPRESS_WARNINGS=1)"
-            )
+        model = LONG_TEXT_MODEL
+        log("Warning: Message is long. Using 16k model", type="warning", log=debug)
 
     # Check if the total number of tokens exceeds the maximum allowable tokens for the model
     if total_tokens > (16384 - chunk_length):
+        log("Error: Message too long", type="error", log=debug)
         return {"error": "Message too long"}
 
     # Prepare the messages to be sent to the API
     messages = [{"role": "user", "content": text}]
 
+    log(f"Prompt:\n{text}\n\nFunctions:\n{json.dumps(functions, indent=4)}", type="prompt", log=debug)
+
     # Define a nested function to handle API request and exceptions
     def try_request():
         """Attempts to create a chat completion with OpenAI's API and handles any exceptions that may occur."""
         try:
             # If there are function(s) to call
             if functions:
                 response = openai.ChatCompletion.create(
@@ -370,15 +390,15 @@
                     function_call=function_call,
                 )
             else:
                 # If there are no function(s) to call
                 response = openai.ChatCompletion.create(model=model, messages=messages)
             return response
         except Exception as e:
-            print(f"OpenAI Error: {e}")
+            log(f"OpenAI Error: {e}", type="error", log=debug)
             return None
 
     # Retry function call and model calls according to the specified retry counts
     response = None
     for _ in range(function_failure_retries):
         for _ in range(model_failure_retries):
             response = try_request()
@@ -403,18 +423,21 @@
     usage = response["usage"]
 
     text = response_data["content"]
     function_call_response = response_data.get("function_call", None)
 
     # If no function call in response, return an error
     if function_call_response is None:
+        log("No function call in response", type="error", log=debug)
         return {"error": "No function call in response"}
-
+    function_name = function_call_response["name"]
+    arguments = parse_arguments(function_call_response["arguments"])
+    log(f"Response\n\nFunction Name: {function_name}\n\nArguments:\n{arguments}\n\nText:\n{text}\n\nFinish Reason: {finish_reason}\n\nUsage:\n{usage}", type="response", log=debug)
     # Return the final result with the text response, function name, arguments and no error
     return {
         "text": text,
-        "function_name": function_call_response["name"],
-        "arguments": parse_arguments(function_call_response["arguments"]),
+        "function_name": function_name,
+        "arguments": arguments,
         "usage": usage,
         "finish_reason": finish_reason,
         "error": None,
     }
```

### Comparing `easycompletion-0.2.6/easycompletion/prompt.py` & `easycompletion-0.2.7/easycompletion/prompt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import re
 import tiktoken
-import sys
-
-from .constants import (
-    default_text_model,
-    default_chunk_length,
-)
 
+from .constants import DEFAULT_TEXT_MODEL, DEFAULT_CHUNK_LENGTH, DEBUG
+from .logger import log
 
 def trim_prompt(
-    text, max_tokens=default_chunk_length, model=default_text_model, preserve_top=True
+    text,
+    max_tokens=DEFAULT_CHUNK_LENGTH,
+    model=DEFAULT_TEXT_MODEL,
+    preserve_top=True,
+    debug=DEBUG,
 ):
     """
     Trim the given text to a maximum number of tokens.
 
     Args:
         text: Input text which needs to be trimmed.
         max_tokens: Maximum number of tokens allowed in the trimmed text.
@@ -30,23 +30,25 @@
         Output: "This is"
     """
     # Encoding the text into tokens.
     encoding = tiktoken.encoding_for_model(model)
     tokens = encoding.encode(text)
     if len(tokens) <= max_tokens:
         return text  # If text is already within limit, return as is.
+    
+    log(f"Trimming prompt, token len is {str(len(tokens))}", type="warning", log=debug)
 
     # If 'preserve_top' is True, keep the first 'max_tokens' tokens.
     # Otherwise, keep the last 'max_tokens' tokens.
     return encoding.decode(
         tokens[:max_tokens] if preserve_top else tokens[-max_tokens:]
     )
 
 
-def chunk_prompt(prompt, chunk_length=default_chunk_length):
+def chunk_prompt(prompt, chunk_length=DEFAULT_CHUNK_LENGTH, debug=DEBUG):
     """
     Split the given prompt into chunks where each chunk has a maximum number of tokens.
 
     Args:
         prompt: Input text that needs to be split.
         chunk_length: Maximum number of tokens allowed per chunk.
                       Default value is taken from the constants.
@@ -54,14 +56,17 @@
     Returns:
         A list of string chunks where each chunk is within the specified token limit.
 
     Example:
         chunk_prompt("This is a test. I am writing a function.", 4)
         Output: ['This is', 'a test.', 'I am', 'writing a', 'function.']
     """
+    if count_tokens(prompt) <= chunk_length:
+        return [prompt]
+
     # Splitting the prompt into sentences using regular expressions.
     sentences = re.split(r"(?<=[.!?])\s+", prompt)
     current_chunk = ""
     prompt_chunks = []
 
     # For each sentence in the input text.
     for sentence in sentences:
@@ -74,18 +79,20 @@
             prompt_chunks.append(current_chunk.strip())
             current_chunk = sentence + " "
 
     # If there's any sentence left after looping through all sentences, add it to the list.
     if current_chunk:
         prompt_chunks.append(current_chunk.strip())
 
+    log(f"Chunked prompt into {str(len(prompt_chunks))} chunks", type="warning", log=debug)
+
     return prompt_chunks
 
 
-def count_tokens(prompt: str, model=default_text_model) -> int:
+def count_tokens(prompt: str, model=DEFAULT_TEXT_MODEL) -> int:
     """
     Count the number of tokens in a string.
 
     Args:
         prompt: The string to be tokenized.
         model: The model to use for tokenization.
 
@@ -94,21 +101,23 @@
 
     Example:
         count_tokens("This is a test.")
         Output: 5
     """
     if not isinstance(prompt, str):
         prompt = str(prompt)
+        
     encoding = tiktoken.encoding_for_model(model)
-    return len(
+    length = len(
         encoding.encode(prompt)
     )  # Encoding the text into tokens and counting the number of tokens.
+    return length
 
 
-def get_tokens(prompt: str, model=default_text_model) -> list:
+def get_tokens(prompt: str, model=DEFAULT_TEXT_MODEL) -> list:
     """
     Returns a list of tokens in a string.
 
     Args:
         prompt: The string to be tokenized.
         model: The model to use for tokenization.
 
@@ -121,15 +130,15 @@
     """
     encoding = tiktoken.encoding_for_model(model)
     return encoding.encode(
         prompt
     )  # Encoding the text into tokens and returning the list of tokens.
 
 
-def compose_prompt(prompt_template, parameters):
+def compose_prompt(prompt_template, parameters, debug=DEBUG):
     """
     Composes a prompt using a template and parameters.
     Parameter keys are enclosed in double curly brackets and replaced with parameter values.
 
     Args:
         prompt_template: A template string that contains placeholders for the parameters.
         parameters: A dictionary containing key-value pairs to replace the placeholders.
@@ -141,30 +150,32 @@
         compose_prompt("Hello {{name}}!", {"name": "John"})
         Output: "Hello John!"
     """
     prompt = prompt_template  # Initial prompt template.
 
     # Replacing placeholders in the template with the actual values from the parameters.
     for key, value in parameters.items():
-            # check if "{{" + key + "}}" is in prompt
-            # if not, continue
-            if "{{" + key + "}}" not in prompt:
-                continue
-            try:
-                if isinstance(value, str):
-                    prompt = prompt.replace("{{" + key + "}}", value)
-                elif isinstance(value, int):
-                    prompt = prompt.replace("{{" + key + "}}", str(value))
-                elif isinstance(value, dict):
-                    for k, v in value.items():
-                        prompt = prompt.replace("{{" + key + "}}", k + "::" + v)
-                elif isinstance(value, list):
-                    for item in value:
-                        prompt = prompt.replace("{{" + key + "}}", item + "\n")
-                elif value is None:
-                    prompt = prompt.replace("{{" + key + "}}", "None")
-                else:
-                    raise Exception(f"ERROR PARSING:\n{key}\n{value}")
-            except:
+        # check if "{{" + key + "}}" is in prompt
+        # if not, continue
+        if "{{" + key + "}}" not in prompt:
+            continue
+        try:
+            if isinstance(value, str):
+                prompt = prompt.replace("{{" + key + "}}", value)
+            elif isinstance(value, int):
+                prompt = prompt.replace("{{" + key + "}}", str(value))
+            elif isinstance(value, dict):
+                for k, v in value.items():
+                    prompt = prompt.replace("{{" + key + "}}", k + "::" + v)
+            elif isinstance(value, list):
+                for item in value:
+                    prompt = prompt.replace("{{" + key + "}}", item + "\n")
+            elif value is None:
+                prompt = prompt.replace("{{" + key + "}}", "None")
+            else:
                 raise Exception(f"ERROR PARSING:\n{key}\n{value}")
+        except:
+            raise Exception(f"ERROR PARSING:\n{key}\n{value}")
+
+    log(f"Composed prompt:\n{prompt}", log=debug)
 
     return prompt
```

### Comparing `easycompletion-0.2.6/easycompletion.egg-info/PKG-INFO` & `easycompletion-0.2.7/easycompletion.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.2.6
+Version: 0.2.7
 Summary: Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/AutonomousResearchGroup/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
@@ -125,15 +125,15 @@
             "description": "Detailed summary of the text.",
         },
     },
     required_properties=["summary"],
 )
 ```
 
-### `openai_text_call(text, model_failure_retries=5, model=None, chunk_length=default_chunk_length, api_key=None)`
+### `openai_text_call(text, model_failure_retries=5, model=None, chunk_length=DEFAULT_CHUNK_LENGTH, api_key=None)`
 
 Sends text to the OpenAI API and returns a text response.
 
 ```python
 response = openai_text_call(
     "Hello, how are you?",
     model_failure_retries=3,
@@ -154,15 +154,15 @@
         "total_tokens": "number"
     },
     "error": "string|None",
     "finish_reason": "string"
 }
 ```
 
-### `openai_function_call(text, functions=None, model_failure_retries=5, function_call=None, function_failure_retries=10, chunk_length=default_chunk_length, model=None, api_key=None)`
+### `openai_function_call(text, functions=None, model_failure_retries=5, function_call=None, function_failure_retries=10, chunk_length=DEFAULT_CHUNK_LENGTH, model=None, api_key=None)`
 
 Sends text and a list of functions to the OpenAI API and returns optional text and a function call. The function call is validated against the functions array.
 
 ```python
 function = {
     'name': 'function1',
     'parameters': {'param1': 'value1'}
@@ -184,39 +184,39 @@
         "total_tokens": "number"
     },
     "finish_reason": "string",
     "error": "string|None"
 }
 ```
 
-### `trim_prompt(text, max_tokens=default_chunk_length, model=default_text_model, preserve_top=True)`
+### `trim_prompt(text, max_tokens=DEFAULT_CHUNK_LENGTH, model=DEFAULT_TEXT_MODEL, preserve_top=True)`
 
 Trim the given text to a maximum number of tokens.
 
 ```python
 trimmed_text = trim_prompt("This is a test.", 3, preserve_top=True)
 ```
 
-### `chunk_prompt(prompt, chunk_length=default_chunk_length)`
+### `chunk_prompt(prompt, chunk_length=DEFAULT_CHUNK_LENGTH)`
 
 Split the given prompt into chunks where each chunk has a maximum number of tokens.
 
 ```python
 prompt_chunks = chunk_prompt("This is a test. I am writing a function.", 4)
 ```
 
-### `count_tokens(prompt, model=default_text_model)`
+### `count_tokens(prompt, model=DEFAULT_TEXT_MODEL)`
 
 Count the number of tokens in a string.
 
 ```python
 num_tokens = count_tokens("This is a test.")
 ```
 
-### `get_tokens(prompt, model=default_text_model)`
+### `get_tokens(prompt, model=DEFAULT_TEXT_MODEL)`
 
 Returns a list of tokens in a string.
 
 ```python
 tokens = get_tokens("This is a test.")
 ```
```

### Comparing `easycompletion-0.2.6/setup.py` & `easycompletion-0.2.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,24 +8,24 @@
     long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
     long_description = "\n".join(long_description)
 
 
 setup(
     name="easycompletion",
-    version='0.2.6',
+    version='0.2.7',
     description="Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/easycompletion",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
     packages=["easycompletion"],
-    install_requires=["openai", "tiktoken", "python-dotenv"],
+    install_requires=["openai", "tiktoken", "python-dotenv", "rich"],
     readme="README.md",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3",
```

