# Comparing `tmp/goldretriever-0.1.3.tar.gz` & `tmp/goldretriever-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goldretriever-0.1.3.tar", max compression
+gzip compressed data, was "goldretriever-0.1.4.tar", max compression
```

## Comparing `goldretriever-0.1.3.tar` & `goldretriever-0.1.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1063 2023-07-13 10:07:22.962369 goldretriever-0.1.3/LICENSE
--rw-r--r--   0        0        0     4730 2023-07-13 10:07:22.962369 goldretriever-0.1.3/README.md
--rw-r--r--   0        0        0      758 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/.well-known/ai-plugin.json
--rw-r--r--   0        0        0      760 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/.well-known/default-ai-plugin.json
--rw-r--r--   0        0        0      836 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/.well-known/logo.png
--rw-r--r--   0        0        0     4737 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/.well-known/openapi.yaml
--rw-r--r--   0        0        0        0 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/__init__.py
--rw-r--r--   0        0        0       98 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/config.yml
--rw-r--r--   0        0        0        0 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/datastore/__init__.py
--rw-r--r--   0        0        0     3046 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/datastore/datastore.py
--rw-r--r--   0        0        0      143 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/datastore/executor/Dockerfile
--rw-r--r--   0        0        0        0 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/datastore/executor/__init__.py
--rw-r--r--   0        0        0      161 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/datastore/executor/config.yml
--rw-r--r--   0        0        0     3193 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/datastore/executor/docarray_v1.py
--rw-r--r--   0        0        0     1220 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/datastore/factory.py
--rw-r--r--   0        0        0      796 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/flow.yml
--rw-r--r--   0        0        0    11289 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/gateway.py
--rw-r--r--   0        0        0        0 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/models/__init__.py
--rw-r--r--   0        0        0      634 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/models/api.py
--rw-r--r--   0        0        0     1460 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/models/models.py
--rw-r--r--   0        0        0    10199 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/retriever.py
--rw-r--r--   0        0        0        0 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/__init__.py
--rw-r--r--   0        0        0     3016 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_json/README.md
--rw-r--r--   0        0        0        0 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_json/__init__.py
--rw-r--r--   0        0        0      630 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_json/example.json
--rw-r--r--   0        0        0     5356 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_json/process_json.py
--rw-r--r--   0        0        0     3091 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_jsonl/README.md
--rw-r--r--   0        0        0        0 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_jsonl/__init__.py
--rw-r--r--   0        0        0      879 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_jsonl/example.jsonl
--rw-r--r--   0        0        0     5253 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_jsonl/process_jsonl.py
--rw-r--r--   0        0        0     2699 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_zip/README.md
--rw-r--r--   0        0        0        0 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_zip/__init__.py
--rw-r--r--   0        0        0    53296 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_zip/example.zip
--rw-r--r--   0        0        0     5668 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/scripts/process_zip/process_zip.py
--rw-r--r--   0        0        0        0 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/services/__init__.py
--rw-r--r--   0        0        0     7609 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/services/chunks.py
--rw-r--r--   0        0        0      793 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/services/date.py
--rw-r--r--   0        0        0     1201 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/services/extract_metadata.py
--rw-r--r--   0        0        0     3674 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/services/file.py
--rw-r--r--   0        0        0     1879 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/services/openai.py
--rw-r--r--   0        0        0     1350 2023-07-13 10:07:22.966369 goldretriever-0.1.3/goldretriever/services/pii_detection.py
--rw-r--r--   0        0        0      956 2023-07-13 10:07:22.970368 goldretriever-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6076 1970-01-01 00:00:00.000000 goldretriever-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-21 10:38:31.217250 goldretriever-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4730 2023-07-21 10:38:31.217250 goldretriever-0.1.4/README.md
+-rw-r--r--   0        0        0      758 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/.well-known/ai-plugin.json
+-rw-r--r--   0        0        0      760 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/.well-known/default-ai-plugin.json
+-rw-r--r--   0        0        0      836 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/.well-known/logo.png
+-rw-r--r--   0        0        0     4737 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/.well-known/openapi.yaml
+-rw-r--r--   0        0        0        0 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/__init__.py
+-rw-r--r--   0        0        0       98 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/config.yml
+-rw-r--r--   0        0        0        0 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/datastore/__init__.py
+-rw-r--r--   0        0        0     3046 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/datastore/datastore.py
+-rw-r--r--   0        0        0      143 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/datastore/executor/Dockerfile
+-rw-r--r--   0        0        0        0 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/datastore/executor/__init__.py
+-rw-r--r--   0        0        0      161 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/datastore/executor/config.yml
+-rw-r--r--   0        0        0     3193 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/datastore/executor/docarray_v1.py
+-rw-r--r--   0        0        0     1220 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/datastore/factory.py
+-rw-r--r--   0        0        0      832 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/flow.yml
+-rw-r--r--   0        0        0    11289 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/gateway.py
+-rw-r--r--   0        0        0        0 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/models/__init__.py
+-rw-r--r--   0        0        0      634 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/models/api.py
+-rw-r--r--   0        0        0     1460 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/models/models.py
+-rw-r--r--   0        0        0    10199 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/retriever.py
+-rw-r--r--   0        0        0        0 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/scripts/__init__.py
+-rw-r--r--   0        0        0     3016 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/scripts/process_json/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/scripts/process_json/__init__.py
+-rw-r--r--   0        0        0      630 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/scripts/process_json/example.json
+-rw-r--r--   0        0        0     5356 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/scripts/process_json/process_json.py
+-rw-r--r--   0        0        0     3091 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/scripts/process_jsonl/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/scripts/process_jsonl/__init__.py
+-rw-r--r--   0        0        0      879 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/scripts/process_jsonl/example.jsonl
+-rw-r--r--   0        0        0     5253 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/scripts/process_jsonl/process_jsonl.py
+-rw-r--r--   0        0        0     2699 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/scripts/process_zip/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/scripts/process_zip/__init__.py
+-rw-r--r--   0        0        0    53296 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/scripts/process_zip/example.zip
+-rw-r--r--   0        0        0     5668 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/scripts/process_zip/process_zip.py
+-rw-r--r--   0        0        0        0 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/services/__init__.py
+-rw-r--r--   0        0        0     7609 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/services/chunks.py
+-rw-r--r--   0        0        0      793 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/services/date.py
+-rw-r--r--   0        0        0     1201 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/services/extract_metadata.py
+-rw-r--r--   0        0        0     3674 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/services/file.py
+-rw-r--r--   0        0        0     1879 2023-07-21 10:38:31.217250 goldretriever-0.1.4/goldretriever/services/openai.py
+-rw-r--r--   0        0        0     1350 2023-07-21 10:38:31.221250 goldretriever-0.1.4/goldretriever/services/pii_detection.py
+-rw-r--r--   0        0        0      956 2023-07-21 10:38:31.221250 goldretriever-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6076 1970-01-01 00:00:00.000000 goldretriever-0.1.4/PKG-INFO
```

### Comparing `goldretriever-0.1.3/LICENSE` & `goldretriever-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/README.md` & `goldretriever-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/.well-known/ai-plugin.json` & `goldretriever-0.1.4/goldretriever/.well-known/ai-plugin.json`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/.well-known/default-ai-plugin.json` & `goldretriever-0.1.4/goldretriever/.well-known/default-ai-plugin.json`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/.well-known/logo.png` & `goldretriever-0.1.4/goldretriever/.well-known/logo.png`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/.well-known/openapi.yaml` & `goldretriever-0.1.4/goldretriever/.well-known/openapi.yaml`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/datastore/datastore.py` & `goldretriever-0.1.4/goldretriever/datastore/datastore.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/datastore/executor/docarray_v1.py` & `goldretriever-0.1.4/goldretriever/datastore/executor/docarray_v1.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/datastore/factory.py` & `goldretriever-0.1.4/goldretriever/datastore/factory.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/flow.yml` & `goldretriever-0.1.4/goldretriever/flow.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 jtype: Flow
 version: '1'
 jcloud:
   docarray: 0.21.0
   name: retrieval-plugin
+  labels:
+    app: retrieval-plugin
 gateway:
   protocol: [http]
   uses: jinaai+docker://auth0-unified-b06aa99c0fdac54c/GptRetrievalGateway:latest
   port:
     - 12345
   port_monitoring: 51036
   uses_with:
```

### Comparing `goldretriever-0.1.3/goldretriever/gateway.py` & `goldretriever-0.1.4/goldretriever/gateway.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/models/api.py` & `goldretriever-0.1.4/goldretriever/models/api.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/models/models.py` & `goldretriever-0.1.4/goldretriever/models/models.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/retriever.py` & `goldretriever-0.1.4/goldretriever/retriever.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/scripts/process_json/README.md` & `goldretriever-0.1.4/goldretriever/scripts/process_json/README.md`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/scripts/process_json/example.json` & `goldretriever-0.1.4/goldretriever/scripts/process_json/example.json`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/scripts/process_json/process_json.py` & `goldretriever-0.1.4/goldretriever/scripts/process_json/process_json.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/scripts/process_jsonl/README.md` & `goldretriever-0.1.4/goldretriever/scripts/process_jsonl/README.md`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/scripts/process_jsonl/example.jsonl` & `goldretriever-0.1.4/goldretriever/scripts/process_jsonl/example.jsonl`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/scripts/process_jsonl/process_jsonl.py` & `goldretriever-0.1.4/goldretriever/scripts/process_jsonl/process_jsonl.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/scripts/process_zip/README.md` & `goldretriever-0.1.4/goldretriever/scripts/process_zip/README.md`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/scripts/process_zip/example.zip` & `goldretriever-0.1.4/goldretriever/scripts/process_zip/example.zip`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/scripts/process_zip/process_zip.py` & `goldretriever-0.1.4/goldretriever/scripts/process_zip/process_zip.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/services/chunks.py` & `goldretriever-0.1.4/goldretriever/services/chunks.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/services/date.py` & `goldretriever-0.1.4/goldretriever/services/date.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/services/extract_metadata.py` & `goldretriever-0.1.4/goldretriever/services/extract_metadata.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/services/file.py` & `goldretriever-0.1.4/goldretriever/services/file.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/services/openai.py` & `goldretriever-0.1.4/goldretriever/services/openai.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/goldretriever/services/pii_detection.py` & `goldretriever-0.1.4/goldretriever/services/pii_detection.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.3/pyproject.toml` & `goldretriever-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "goldretriever"
-version = "0.1.3"
+version = "0.1.4"
 description = "Create and host retrieval plugins for ChatGPT in one click"
 authors = ["Jina AI <hello@jina.ai>"]
 readme = "README.md"
 include = ["goldretriever/**/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `goldretriever-0.1.3/PKG-INFO` & `goldretriever-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goldretriever
-Version: 0.1.3
+Version: 0.1.4
 Summary: Create and host retrieval plugins for ChatGPT in one click
 Author: Jina AI
 Author-email: hello@jina.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

