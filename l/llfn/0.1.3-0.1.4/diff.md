# Comparing `tmp/llfn-0.1.3.tar.gz` & `tmp/llfn-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llfn-0.1.3.tar", max compression
+gzip compressed data, was "llfn-0.1.4.tar", max compression
```

## Comparing `llfn-0.1.3.tar` & `llfn-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1101 2023-07-20 11:12:16.267041 llfn-0.1.3/LICENSE
--rw-r--r--   0        0        0    10940 2023-07-20 11:50:24.862974 llfn-0.1.3/README.md
--rw-r--r--   0        0        0       43 2023-07-20 10:49:19.230094 llfn-0.1.3/llfn/__init__.py
--rw-r--r--   0        0        0     1668 2023-07-20 16:42:16.817301 llfn-0.1.3/llfn/llfn.py
--rw-r--r--   0        0        0      345 2023-07-20 16:50:41.902629 llfn-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    11439 1970-01-01 00:00:00.000000 llfn-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1101 2023-07-20 11:12:16.267041 llfn-0.1.4/LICENSE
+-rw-r--r--   0        0        0    10940 2023-07-20 11:50:24.862974 llfn-0.1.4/README.md
+-rw-r--r--   0        0        0       43 2023-07-20 10:49:19.230094 llfn-0.1.4/llfn/__init__.py
+-rw-r--r--   0        0        0     2067 2023-07-21 02:24:05.180281 llfn-0.1.4/llfn/llfn.py
+-rw-r--r--   0        0        0      502 2023-07-21 03:11:47.391881 llfn-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    11540 1970-01-01 00:00:00.000000 llfn-0.1.4/PKG-INFO
```

### Comparing `llfn-0.1.3/LICENSE` & `llfn-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llfn-0.1.3/README.md` & `llfn-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `llfn-0.1.3/llfn/llfn.py` & `llfn-0.1.4/llfn/llfn.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import json
 from functools import update_wrapper
+from langchain.llms.base import BaseLLM
+from langchain.chat_models.base import BaseChatModel
 from langchain.schema import HumanMessage, SystemMessage
 from pydantic import BaseModel, Field
 
 
 class LLFnFunc:
     def __init__(self, app, func):
         self.app = app
@@ -26,28 +27,37 @@
             llm = self.llm
         elif self.app.llm is not None:
             llm = self.app.llm
         else:
             raise ValueError(
                 f'You must call "bind" before calling "{self.func.__name__}"'
             )
-        prompt = self.func(*args, **kwargs)
-        output = llm.predict_messages(
-            [
-                SystemMessage(
-                    content=f"""
+        user_prompt = self.func(*args, **kwargs)
+        system_prompt = f"""
 - You MUST process the user's command and produce exactly one result without any other contexts or explanations
 - Your output must be a JSON dump of a Pydantic object of schema: {self.result_type.schema()}
 - Output format is EXTREMELY important. Make sure it's a valid JSON dump of the Pydantic object
 """
-                ),
-                HumanMessage(content=prompt),
-            ]
-        )
-        return self.result_type.parse_raw(output.content).result
+        if isinstance(llm, BaseChatModel):
+            output = llm.predict_messages(
+                [
+                    SystemMessage(content=system_prompt),
+                    HumanMessage(content=user_prompt),
+                ]
+            ).content
+        elif isinstance(llm, BaseLLM):
+            output = llm(
+                f"""{system_prompt}
+
+User command: {user_prompt}""
+"""
+            )
+        else:
+            raise ValueError(f"LLM must be either a ChatModel or a BaseLLM")
+        return self.result_type.parse_raw(output).result
 
 
 class LLFn:
     def __init__(self):
         self.llm = None
 
     def bind(self, llm):
```

### Comparing `llfn-0.1.3/PKG-INFO` & `llfn-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: llfn
-Version: 0.1.3
-Summary: 
+Version: 0.1.4
+Summary: Build anything from a simple text-summarizer to complex AI agents with one common primitive: function
 Author: Sorawit Suriyakarn
 Author-email: thepsint@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

