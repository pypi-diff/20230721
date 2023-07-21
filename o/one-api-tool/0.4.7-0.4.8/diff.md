# Comparing `tmp/one-api-tool-0.4.7.tar.gz` & `tmp/one-api-tool-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.4.7.tar", last modified: Tue Jul  4 12:04:03 2023, max compression
+gzip compressed data, was "one-api-tool-0.4.8.tar", last modified: Fri Jul 21 08:12:24 2023, max compression
```

## Comparing `one-api-tool-0.4.7.tar` & `one-api-tool-0.4.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 12:04:03.722114 one-api-tool-0.4.7/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.4.7/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     7488 2023-07-04 12:04:03.721872 one-api-tool-0.4.7/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     6932 2023-07-04 06:55:22.000000 one-api-tool-0.4.7/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 12:04:03.720510 one-api-tool-0.4.7/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     7488 2023-07-04 12:04:03.000000 one-api-tool-0.4.7/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      359 2023-07-04 12:04:03.000000 one-api-tool-0.4.7/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-04 12:04:03.000000 one-api-tool-0.4.7/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-07-04 12:04:03.000000 one-api-tool-0.4.7/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       86 2023-07-04 12:04:03.000000 one-api-tool-0.4.7/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-07-04 12:04:03.000000 one-api-tool-0.4.7/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 12:04:03.721112 one-api-tool-0.4.7/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-04 04:37:23.000000 one-api-tool-0.4.7/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 12:04:03.721489 one-api-tool-0.4.7/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.4.7/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-06-26 09:39:20.000000 one-api-tool-0.4.7/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    17841 2023-07-04 12:03:32.000000 one-api-tool-0.4.7/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3598 2023-07-04 12:02:12.000000 one-api-tool-0.4.7/oneapi/utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-04 12:04:03.722173 one-api-tool-0.4.7/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1078 2023-07-04 12:03:59.000000 one-api-tool-0.4.7/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 08:12:24.634886 one-api-tool-0.4.8/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.4.8/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     7677 2023-07-21 08:12:24.634702 one-api-tool-0.4.8/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     7121 2023-07-21 08:10:20.000000 one-api-tool-0.4.8/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 08:12:24.632772 one-api-tool-0.4.8/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     7677 2023-07-21 08:12:24.000000 one-api-tool-0.4.8/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      359 2023-07-21 08:12:24.000000 one-api-tool-0.4.8/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-21 08:12:24.000000 one-api-tool-0.4.8/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-07-21 08:12:24.000000 one-api-tool-0.4.8/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       86 2023-07-21 08:12:24.000000 one-api-tool-0.4.8/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-07-21 08:12:24.000000 one-api-tool-0.4.8/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 08:12:24.633736 one-api-tool-0.4.8/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-04 04:37:23.000000 one-api-tool-0.4.8/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 08:12:24.634274 one-api-tool-0.4.8/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.4.8/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-06-26 09:39:20.000000 one-api-tool-0.4.8/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    21439 2023-07-21 08:10:55.000000 one-api-tool-0.4.8/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3598 2023-07-04 12:02:12.000000 one-api-tool-0.4.8/oneapi/utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-21 08:12:24.634941 one-api-tool-0.4.8/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1078 2023-07-21 08:11:12.000000 one-api-tool-0.4.8/setup.py
```

### Comparing `one-api-tool-0.4.7/LICENSE` & `one-api-tool-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.4.7/PKG-INFO` & `one-api-tool-0.4.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.4.7
+Version: 0.4.8
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -71,20 +71,23 @@
 If you are using Azure APIs, you can find relevant information on the Azure resource dashboard. The API format typically follows this pattern: `https://{your_organization}.openai.azure.com/`.
 
 `api_type`: Currently supported values are "open_ai", "azure", or "claude".
 
 #### Chat example:
 ```python
 from oneapi import OneAPITool
+import asyncio
 # Two ways to initialize the OneAPITool object  
 # tool = OneAPITool.from_config(api_key, api_base, api_type)
 tool = OneAPITool.from_config_file("your_config_file.json")
 # Say hello to ChatGPT/Claude/GPT-4
 res = tool.simple_chat("Hello AI!")
 print(res)
+# Async chat to ChatGPT/Claude/GPT-4 with `stream=False`
+res = asyncio.run(tool.asimple_chat('How\'s the weather today?', model='gpt-4', stream=False))
 # Get embeddings of some sentences for further usage, e.g., clustering
 embeddings = tool.get_embeddings(["Hello AI!", "Hello world!"])
 print(len(embeddings)))
 # Count the number of tokens
 print(tool.count_tokens(["Hello AI!", "Hello world!"]))
 ```
 **Note: Currently, `get_embeddings` only support OpenAI or Microsoft Azure API.**
@@ -219,10 +222,11 @@
 
 `--max_new_tokens` integer ${\color{grey}\text{Optional}}$ Defaults to 2048 <br>
 The maximum number of tokens to generate in the chat completion.
 The total length of input tokens and generated tokens is limited by the model's context length.
 
 ## ToDo
 - [ ] Batch requests.
-- [ ] OpenAI function_call.
+- [x] OpenAI function_call.
 - [x] Token number counting.
+- [x] Async requests.
 - [ ] Custom token budget.
```

### Comparing `one-api-tool-0.4.7/README.md` & `one-api-tool-0.4.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,20 +59,23 @@
 If you are using Azure APIs, you can find relevant information on the Azure resource dashboard. The API format typically follows this pattern: `https://{your_organization}.openai.azure.com/`.
 
 `api_type`: Currently supported values are "open_ai", "azure", or "claude".
 
 #### Chat example:
 ```python
 from oneapi import OneAPITool
+import asyncio
 # Two ways to initialize the OneAPITool object  
 # tool = OneAPITool.from_config(api_key, api_base, api_type)
 tool = OneAPITool.from_config_file("your_config_file.json")
 # Say hello to ChatGPT/Claude/GPT-4
 res = tool.simple_chat("Hello AI!")
 print(res)
+# Async chat to ChatGPT/Claude/GPT-4 with `stream=False`
+res = asyncio.run(tool.asimple_chat('How\'s the weather today?', model='gpt-4', stream=False))
 # Get embeddings of some sentences for further usage, e.g., clustering
 embeddings = tool.get_embeddings(["Hello AI!", "Hello world!"])
 print(len(embeddings)))
 # Count the number of tokens
 print(tool.count_tokens(["Hello AI!", "Hello world!"]))
 ```
 **Note: Currently, `get_embeddings` only support OpenAI or Microsoft Azure API.**
@@ -207,10 +210,11 @@
 
 `--max_new_tokens` integer ${\color{grey}\text{Optional}}$ Defaults to 2048 <br>
 The maximum number of tokens to generate in the chat completion.
 The total length of input tokens and generated tokens is limited by the model's context length.
 
 ## ToDo
 - [ ] Batch requests.
-- [ ] OpenAI function_call.
+- [x] OpenAI function_call.
 - [x] Token number counting.
+- [x] Async requests.
 - [ ] Custom token budget.
```

### Comparing `one-api-tool-0.4.7/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.4.8/one_api_tool.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.4.7
+Version: 0.4.8
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -71,20 +71,23 @@
 If you are using Azure APIs, you can find relevant information on the Azure resource dashboard. The API format typically follows this pattern: `https://{your_organization}.openai.azure.com/`.
 
 `api_type`: Currently supported values are "open_ai", "azure", or "claude".
 
 #### Chat example:
 ```python
 from oneapi import OneAPITool
+import asyncio
 # Two ways to initialize the OneAPITool object  
 # tool = OneAPITool.from_config(api_key, api_base, api_type)
 tool = OneAPITool.from_config_file("your_config_file.json")
 # Say hello to ChatGPT/Claude/GPT-4
 res = tool.simple_chat("Hello AI!")
 print(res)
+# Async chat to ChatGPT/Claude/GPT-4 with `stream=False`
+res = asyncio.run(tool.asimple_chat('How\'s the weather today?', model='gpt-4', stream=False))
 # Get embeddings of some sentences for further usage, e.g., clustering
 embeddings = tool.get_embeddings(["Hello AI!", "Hello world!"])
 print(len(embeddings)))
 # Count the number of tokens
 print(tool.count_tokens(["Hello AI!", "Hello world!"]))
 ```
 **Note: Currently, `get_embeddings` only support OpenAI or Microsoft Azure API.**
@@ -219,10 +222,11 @@
 
 `--max_new_tokens` integer ${\color{grey}\text{Optional}}$ Defaults to 2048 <br>
 The maximum number of tokens to generate in the chat completion.
 The total length of input tokens and generated tokens is limited by the model's context length.
 
 ## ToDo
 - [ ] Batch requests.
-- [ ] OpenAI function_call.
+- [x] OpenAI function_call.
 - [x] Token number counting.
+- [x] Async requests.
 - [ ] Custom token budget.
```

### Comparing `one-api-tool-0.4.7/oneapi/commands/one_api_requst.py` & `one-api-tool-0.4.8/oneapi/commands/one_api_requst.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.4.7/oneapi/one_api.py` & `one-api-tool-0.4.8/oneapi/one_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -155,15 +155,43 @@
         else:
             response_message = completion.choices[0].message
             if is_function_call:
                 if response_message.get("function_call") is not None:
                     return response_message
             return response_message.get("content", "")
 
-
+    async def asimple_chat(self, args: OpenAIDecodingArguments):
+        data = args.dict()
+        is_function_call = data.get("functions", None) is not None
+        if is_function_call:
+            data["stream"] = False  
+        else:
+            if isinstance(args, OpenAIDecodingArguments):
+                data.pop("functions")
+                data.pop("function_call")
+        completion = await openai.ChatCompletion.acreate(**data)
+        if data.get("stream", False):
+            # create variables to collect the stream of chunks
+            collected_chunks = []
+            collected_messages = []
+            # iterate through the stream of events
+            async for chunk in completion:
+                collected_chunks.append(chunk)  # save the event response
+                chunk_choice = chunk["choices"][0]
+                chunk_message = chunk_choice["delta"]  # extract the message
+                finish_reason = chunk_choice["finish_reason"]
+                collected_messages.append(chunk_message)  # save the message
+            full_reply_content = "".join([m.get("content", "") for m in collected_messages])
+            return full_reply_content
+        else:
+            response_message = completion.choices[0].message
+            if is_function_call:
+                if response_message.get("function_call") is not None:
+                    return response_message
+            return response_message.get("content", "")
          
 
 
     def get_embeddings(self, texts: List[str], engine="text-embedding-ada-002") -> List[List[float]]:
         assert len(texts) <= 2048, "The batch size should not be larger than 2048."
         # replace newlines, which can negatively affect performance.
         texts = [text.replace("\n", " ") for text in texts]
@@ -203,15 +231,15 @@
     https://github.com/anthropics/anthropic-sdk-python/blob/main/examples/basic_stream.py
     https://console.anthropic.com/docs/api/reference
     """
     def __init__(self,method : AbstrctMethod) -> None:
         self.method = method
         self.client = anthropic.Client(method.api_key)
     
-    async def simple_chat(self, args: ClaudeDecodingArguments):
+    async def asimple_chat(self, args: ClaudeDecodingArguments):
         if args.stream:
             resp = await self.client.acompletion_stream(**args.dict())
             async for data in resp:
                 if data["stop_reason"] == "stop_sequence" or data["stop_reason"] == "max_tokens":
                     return data["completion"]
         else:
             resp = await self.client.acompletion(**args.dict())
@@ -290,14 +318,43 @@
             args = ClaudeDecodingArguments(prompt=f"{anthropic.HUMAN_PROMPT} {prompt}{anthropic.AI_PROMPT}", model=model if model else "claude-v1.3-100k", temperature=temperature, max_tokens_to_sample=max_new_tokens, stream=stream, **kwargs)
         else:
             raise AssertionError(f"Not supported api type: {type(self.tool)}")
 
         response = self.tool.simple_chat(args)
         return response
 
+    async def asimple_chat(self, prompt: str|list|dict, system:str="", functions:List[Callable]=None, function_call:Optional[str|dict]=None, model:str="", temperature:int=1, max_new_tokens:int=2048, stream:bool=True, **kwargs):
+        if isinstance(self.tool, OpenAITool):
+            msgs = [] if not system else [dict(role="system", content=system)]
+            if isinstance(prompt, str):
+                msgs.append(dict(role="user", content=prompt))
+            elif isinstance(prompt, list):
+                msgs.extend(prompt)
+            elif isinstance(prompt, dict):
+                msgs.append(prompt)
+            else:
+                raise AssertionError(f"Prompt must be a string, list of strings, or ChatGPTMessage. Got {type(prompt)} instead.")
+            if isinstance(self.tool.method, AzureMethod):
+                args = AzureDecodingArguments(messages=msgs, engine=model if model else "gpt-35-turbo", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
+            elif isinstance(self.tool.method, OpenAIMethod):
+                if functions is not None and isinstance(functions, list):
+                    functions = [generate_function_description(func) for func in functions]
+                if function_call is None and functions is not None:
+                    function_call = "auto"
+                if function_call is not None and functions is None:
+                    function_call = None
+                args = OpenAIDecodingArguments(messages=msgs, functions=functions, function_call=function_call, model=model if model else "gpt-3.5-turbo-0613", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
+        elif isinstance(self.tool, ClaudeAITool):
+            args = ClaudeDecodingArguments(prompt=f"{anthropic.HUMAN_PROMPT} {prompt}{anthropic.AI_PROMPT}", model=model if model else "claude-2", temperature=temperature, max_tokens_to_sample=max_new_tokens, stream=stream, **kwargs)
+        else:
+            raise AssertionError(f"Not supported api type: {type(self.tool)}")
+
+        response = await self.tool.asimple_chat(args)
+        return response
+
     def function_chat(self, prompt: str|list|dict, system:str="", functions:List[Callable]=None, function_call:Optional[str|dict]=None, model:str="", temperature:int=1, max_new_tokens:int=2048, stream:bool=True, **kwargs):
         """A full chain of function calling.
         Step1: Call the model with functions and user prompt.
         Step2: Use the model response to call your API.
         Step3: Send the API response back to the model to summarize.
 
         Args:
```

### Comparing `one-api-tool-0.4.7/oneapi/utils.py` & `one-api-tool-0.4.8/oneapi/utils.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.4.7/setup.py` & `one-api-tool-0.4.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.4.7",
+    version="0.4.8",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
```

