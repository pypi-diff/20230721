# Comparing `tmp/modelz-llm-23.6.9.tar.gz` & `tmp/modelz-llm-23.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelz-llm-23.6.9.tar", last modified: Tue Jun  6 08:54:51 2023, max compression
+gzip compressed data, was "modelz-llm-23.7.1.tar", last modified: Fri Jul 21 04:35:20 2023, max compression
```

## Comparing `modelz-llm-23.6.9.tar` & `modelz-llm-23.7.1.tar`

### file list

```diff
@@ -1,47 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.815390 modelz-llm-23.6.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.807389 modelz-llm-23.6.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.811390 modelz-llm-23.6.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/.github/workflows/docker-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/.github/workflows/gcr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/.github/workflows/python-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-06 08:54:51.811390 modelz-llm-23.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/build.envd
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.807389 modelz-llm-23.6.9/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.811390 modelz-llm-23.6.9/images/bloomz-560m/
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/images/bloomz-560m/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.811390 modelz-llm-23.6.9/images/chatglm-6b/
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/images/chatglm-6b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.811390 modelz-llm-23.6.9/images/chatglm-6b-int4/
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/images/chatglm-6b-int4/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.811390 modelz-llm-23.6.9/images/fastchat-t5-3b/
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/images/fastchat-t5-3b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.811390 modelz-llm-23.6.9/images/llama-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/images/llama-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/images/llama-7b/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.811390 modelz-llm-23.6.9/images/vicuna-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/images/vicuna-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/requirements-cpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:54:51.815390 modelz-llm-23.6.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.807389 modelz-llm-23.6.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.811390 modelz-llm-23.6.9/src/modelz_llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/src/modelz_llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-06 08:54:51.000000 modelz-llm-23.6.9/src/modelz_llm/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/src/modelz_llm/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/src/modelz_llm/falcon_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/src/modelz_llm/mosec_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-06 08:54:38.000000 modelz-llm-23.6.9/src/modelz_llm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:54:51.811390 modelz-llm-23.6.9/src/modelz_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-06 08:54:51.000000 modelz-llm-23.6.9/src/modelz_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-06 08:54:51.000000 modelz-llm-23.6.9/src/modelz_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:54:51.000000 modelz-llm-23.6.9/src/modelz_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-06 08:54:51.000000 modelz-llm-23.6.9/src/modelz_llm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-06 08:54:51.000000 modelz-llm-23.6.9/src/modelz_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 08:54:51.000000 modelz-llm-23.6.9/src/modelz_llm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.122982 modelz-llm-23.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.114982 modelz-llm-23.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.118982 modelz-llm-23.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/.github/workflows/docker-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/.github/workflows/gcr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/.github/workflows/python-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-21 04:35:20.122982 modelz-llm-23.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/build.envd
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.114982 modelz-llm-23.7.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.118982 modelz-llm-23.7.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/docs/images/deploy.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.114982 modelz-llm-23.7.1/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.118982 modelz-llm-23.7.1/images/bloomz-560m/
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/images/bloomz-560m/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.118982 modelz-llm-23.7.1/images/chatglm-6b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/images/chatglm-6b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.118982 modelz-llm-23.7.1/images/chatglm-6b-int4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/images/chatglm-6b-int4/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.118982 modelz-llm-23.7.1/images/fastchat-t5-3b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/images/fastchat-t5-3b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.118982 modelz-llm-23.7.1/images/llama-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/images/llama-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/images/llama-7b/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.118982 modelz-llm-23.7.1/images/vicuna-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/images/vicuna-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/requirements-cpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 04:35:20.122982 modelz-llm-23.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.118982 modelz-llm-23.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.122982 modelz-llm-23.7.1/src/modelz_llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/src/modelz_llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-21 04:35:19.000000 modelz-llm-23.7.1/src/modelz_llm/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/src/modelz_llm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/src/modelz_llm/emb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/src/modelz_llm/falcon_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/src/modelz_llm/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/src/modelz_llm/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/src/modelz_llm/mosec_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/src/modelz_llm/uds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/src/modelz_llm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.122982 modelz-llm-23.7.1/src/modelz_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-21 04:35:20.000000 modelz-llm-23.7.1/src/modelz_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-21 04:35:20.000000 modelz-llm-23.7.1/src/modelz_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 04:35:20.000000 modelz-llm-23.7.1/src/modelz_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-21 04:35:20.000000 modelz-llm-23.7.1/src/modelz_llm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-21 04:35:20.000000 modelz-llm-23.7.1/src/modelz_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 04:35:20.000000 modelz-llm-23.7.1/src/modelz_llm.egg-info/top_level.txt
```

### Comparing `modelz-llm-23.6.9/.github/workflows/docker-publish.yml` & `modelz-llm-23.7.1/.github/workflows/docker-publish.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.9/.github/workflows/gcr.yml` & `modelz-llm-23.7.1/.github/workflows/gcr.yml`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 jobs:
   build:
     strategy:
       matrix:
         image:
           - name: modelzai/llm-chatglm-6b-int4
             dockerfile: ./images/chatglm-6b-int4/Dockerfile
+          - name: modelzai/llm-bloomz-560m
+            dockerfile: ./images/bloomz-560m/Dockerfile
           - name: modelzai/llm-chatglm-6b
             dockerfile: ./images/chatglm-6b/Dockerfile
           - name: modelzai/llm-llama-7b
             dockerfile: ./images/llama-7b/Dockerfile
           - name: modelzai/llm-fastchat-t5-3b
             dockerfile: ./images/fastchat-t5-3b/Dockerfile
           - name: modelzai/llm-vicuna-7b
```

### Comparing `modelz-llm-23.6.9/.github/workflows/python-check.yml` & `modelz-llm-23.7.1/.github/workflows/python-check.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.9/.github/workflows/python-publish.yml` & `modelz-llm-23.7.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.9/.gitignore` & `modelz-llm-23.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.9/PKG-INFO` & `modelz-llm-23.7.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: modelz-llm
-Version: 23.6.9
-Summary: LLM unified service
-Author-email: TensorChord <modelz@tensorchord.ai>
-Project-URL: Homepage, https://github.com/tensorchord/modelz-llm
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: gpu
-
 <div align="center">
 
 # Modelz LLM
 
 </div>
 
 <p align=center>
@@ -21,70 +9,95 @@
 <a href="https://twitter.com/TensorChord"><img src="https://img.shields.io/twitter/follow/tensorchord?style=social" alt="trackgit-views" /></a>
 </p>
 
 Modelz LLM is an inference server that facilitates the utilization of open source large language models (LLMs), such as FastChat, LLaMA, and ChatGLM, on either **local or cloud-based** environments with **OpenAI compatible API**.
 
 ## Features
 
-- **OpenAI compatible API**: Modelz LLM provides an OpenAI compatible API for LLMs, which means you can use the OpenAI python SDK to interact with the model.
+- **OpenAI compatible API**: Modelz LLM provides an OpenAI compatible API for LLMs, which means you can use the OpenAI python SDK or LangChain to interact with the model.
 - **Self-hosted**: Modelz LLM can be easily deployed on either local or cloud-based environments.
 - **Open source LLMs**: Modelz LLM supports open source LLMs, such as FastChat, LLaMA, and ChatGLM.
-- **Cloud native**: We provide docker images for different LLMs, which can be easily deployed on Kubernetes, or other cloud-based environments (e.g. [Modelz](https://docs.modelz.ai))
+- **Cloud native**: We provide docker images for different LLMs, which can be easily deployed on Kubernetes, or other cloud-based environments (e.g. [Modelz](https://modelz.ai))
 
 ## Quick Start
 
 ### Install
 
 ```bash
-pip install modelz-llm[gpu]
+pip install modelz-llm
 # or install from source
 pip install git+https://github.com/tensorchord/modelz-llm.git[gpu]
 ```
 
 ### Run the self-hosted API server
 
 Please first start the self-hosted API server by following the instructions:
 
 ```bash
-modelz-llm -m "THUDM/chatglm-6b-int4"
+modelz-llm -m bigscience/bloomz-560m --device cpu
 ```
 
 Currently, we support the following models:
 
-| Model Name | Huggingface Model | Docker Image |
-| ---------- | ----------- | ---------------- |
-|FastChat T5 | `lmsys/fastchat-t5-3b-v1.0` | [modelzai/llm-fastchat-t5-3b](https://hub.docker.com/repository/docker/modelzai/llm-fastchat-t5-3b/general)
-| Vicuna 7B Delta V1.1  | `lmsys/vicuna-7b-delta-v1.1` | [modelzai/llm-vicuna-7b](https://hub.docker.com/repository/docker/modelzai/llm-vicuna-7b/general) |
-| LLaMA 7B    | `decapoda-research/llama-7b-hf` | [modelzai/llm-llama-7b](https://hub.docker.com/repository/docker/modelzai/llm-llama-7b/general) |
-| ChatGLM 6B INT4    | `THUDM/chatglm-6b-int4` | [modelzai/llm-chatglm-6b-int4](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b-int4/general) |
-| ChatGLM 6B  | `THUDM/chatglm-6b` | [modelzai/llm-chatglm-6b](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b/general) |
-| Bloomz 560M | `bigscience/bloomz-560m` | |
-| Bloomz 1.7B | `bigscience/bloomz-1b7` | |
-| Bloomz 3B | `bigscience/bloomz-3b` | |
-| Bloomz 7.1B | `bigscience/bloomz-7b1` | |
+| Model Name | Huggingface Model | Docker Image | Recommended GPU
+| ---------- | ----------- | ---------------- | -- |
+| FastChat T5 | `lmsys/fastchat-t5-3b-v1.0` | [modelzai/llm-fastchat-t5-3b](https://hub.docker.com/repository/docker/modelzai/llm-fastchat-t5-3b/general) | Nvidia L4(24GB) |
+| Vicuna 7B Delta V1.1  | `lmsys/vicuna-7b-delta-v1.1` | [modelzai/llm-vicuna-7b](https://hub.docker.com/repository/docker/modelzai/llm-vicuna-7b/general) | Nvidia A100(40GB) |
+| LLaMA 7B    | `decapoda-research/llama-7b-hf` | [modelzai/llm-llama-7b](https://hub.docker.com/repository/docker/modelzai/llm-llama-7b/general) | Nvidia A100(40GB) |
+| ChatGLM 6B INT4    | `THUDM/chatglm-6b-int4` | [modelzai/llm-chatglm-6b-int4](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b-int4/general) | Nvidia T4(16GB) |
+| ChatGLM 6B  | `THUDM/chatglm-6b` | [modelzai/llm-chatglm-6b](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b/general) | Nvidia L4(24GB) |
+| Bloomz 560M | `bigscience/bloomz-560m` | [modelzai/llm-bloomz-560m](https://hub.docker.com/repository/docker/modelzai/llm-bloomz-560m/general) | CPU |
+| Bloomz 1.7B | `bigscience/bloomz-1b7` | | CPU |
+| Bloomz 3B | `bigscience/bloomz-3b` |  | Nvidia L4(24GB) |
+| Bloomz 7.1B | `bigscience/bloomz-7b1` | | Nvidia A100(40GB) |
 
 ### Use OpenAI python SDK
 
 Then you can use the OpenAI python SDK to interact with the model:
 
 ```python
 import openai
 openai.api_base="http://localhost:8000"
 openai.api_key="any"
 
 # create a chat completion
 chat_completion = openai.ChatCompletion.create(model="any", messages=[{"role": "user", "content": "Hello world"}])
 ```
 
-## Supported APIs
+### Integrate with Langchain
+
+You could also integrate modelz-llm with langchain:
+
+```python
+import openai
+openai.api_base="http://localhost:8000"
+openai.api_key="any"
+
+from langchain.llms import OpenAI
+
+llm = OpenAI()
 
-```py
-    app.add_route("/", Ping())
-    app.add_route("/completions", completion)
-    app.add_route("/chat/completions", chat_completion)
-    app.add_route("/embeddings", embeddings)
-    app.add_route("/engines/{engine}/embeddings", embeddings)
-    app.add_route("/v1/completions", completion)
-    app.add_route("/v1/chat/completions", chat_completion)
-    app.add_route("/v1/embeddings", embeddings)
-    app.add_route("/v1/engines/{engine}/embeddings", embeddings)
+llm.generate(prompts=["Could you please recommend some movies?"])
 ```
+
+## Deploy on Modelz
+
+You could also deploy the modelz-llm directly on [Modelz](https://docs.modelz.ai):
+
+[![](./docs/images/deploy.svg)](https://cloud.modelz.ai/deployment/template?templateId=5e884bb3-6c32-468e-bc62-95cee55c17d4)
+
+## Supported APIs
+
+Modelz LLM supports the following APIs for interacting with open source large language models:
+
+- `/completions`
+- `/chat/completions`
+- `/embeddings`
+- `/engines/<any>/embeddings`
+- `/v1/completions`
+- `/v1/chat/completions`
+- `/v1/embeddings`
+
+## Acknowledgements
+
+- [FastChat](https://github.com/lm-sys/FastChat) for the prompt generation logic.
+- [Mosec](https://github.com/mosecorg/mosec) for the inference engine.
```

#### html2text {}

```diff
@@ -1,47 +1,52 @@
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.9 Summary: LLM unified
-service Author-email: TensorChord
-tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
-llm Classifier: Intended Audience :: Developers Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
-Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
 Modelz LLM is an inference server that facilitates the utilization of open
 source large language models (LLMs), such as FastChat, LLaMA, and ChatGLM, on
 either **local or cloud-based** environments with **OpenAI compatible API**. ##
 Features - **OpenAI compatible API**: Modelz LLM provides an OpenAI compatible
-API for LLMs, which means you can use the OpenAI python SDK to interact with
-the model. - **Self-hosted**: Modelz LLM can be easily deployed on either local
-or cloud-based environments. - **Open source LLMs**: Modelz LLM supports open
-source LLMs, such as FastChat, LLaMA, and ChatGLM. - **Cloud native**: We
-provide docker images for different LLMs, which can be easily deployed on
-Kubernetes, or other cloud-based environments (e.g. [Modelz](https://
-docs.modelz.ai)) ## Quick Start ### Install ```bash pip install modelz-llm[gpu]
-# or install from source pip install git+https://github.com/tensorchord/modelz-
+API for LLMs, which means you can use the OpenAI python SDK or LangChain to
+interact with the model. - **Self-hosted**: Modelz LLM can be easily deployed
+on either local or cloud-based environments. - **Open source LLMs**: Modelz LLM
+supports open source LLMs, such as FastChat, LLaMA, and ChatGLM. - **Cloud
+native**: We provide docker images for different LLMs, which can be easily
+deployed on Kubernetes, or other cloud-based environments (e.g. [Modelz](https:
+//modelz.ai)) ## Quick Start ### Install ```bash pip install modelz-llm # or
+install from source pip install git+https://github.com/tensorchord/modelz-
 llm.git[gpu] ``` ### Run the self-hosted API server Please first start the
 self-hosted API server by following the instructions: ```bash modelz-llm -
-m "THUDM/chatglm-6b-int4" ``` Currently, we support the following models: |
-Model Name | Huggingface Model | Docker Image | | ---------- | ----------- | --
--------------- | |FastChat T5 | `lmsys/fastchat-t5-3b-v1.0` | [modelzai/llm-
-fastchat-t5-3b](https://hub.docker.com/repository/docker/modelzai/llm-fastchat-
-t5-3b/general) | Vicuna 7B Delta V1.1 | `lmsys/vicuna-7b-delta-v1.1` |
-[modelzai/llm-vicuna-7b](https://hub.docker.com/repository/docker/modelzai/llm-
-vicuna-7b/general) | | LLaMA 7B | `decapoda-research/llama-7b-hf` | [modelzai/
+m bigscience/bloomz-560m --device cpu ``` Currently, we support the following
+models: | Model Name | Huggingface Model | Docker Image | Recommended GPU | ---
+------- | ----------- | ---------------- | -- | | FastChat T5 | `lmsys/
+fastchat-t5-3b-v1.0` | [modelzai/llm-fastchat-t5-3b](https://hub.docker.com/
+repository/docker/modelzai/llm-fastchat-t5-3b/general) | Nvidia L4(24GB) | |
+Vicuna 7B Delta V1.1 | `lmsys/vicuna-7b-delta-v1.1` | [modelzai/llm-vicuna-7b]
+(https://hub.docker.com/repository/docker/modelzai/llm-vicuna-7b/general) |
+Nvidia A100(40GB) | | LLaMA 7B | `decapoda-research/llama-7b-hf` | [modelzai/
 llm-llama-7b](https://hub.docker.com/repository/docker/modelzai/llm-llama-7b/
-general) | | ChatGLM 6B INT4 | `THUDM/chatglm-6b-int4` | [modelzai/llm-chatglm-
-6b-int4](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b-int4/
-general) | | ChatGLM 6B | `THUDM/chatglm-6b` | [modelzai/llm-chatglm-6b](https:
-//hub.docker.com/repository/docker/modelzai/llm-chatglm-6b/general) | | Bloomz
-560M | `bigscience/bloomz-560m` | | | Bloomz 1.7B | `bigscience/bloomz-1b7` | |
-| Bloomz 3B | `bigscience/bloomz-3b` | | | Bloomz 7.1B | `bigscience/bloomz-
-7b1` | | ### Use OpenAI python SDK Then you can use the OpenAI python SDK to
-interact with the model: ```python import openai openai.api_base="http://
-localhost:8000" openai.api_key="any" # create a chat completion chat_completion
-= openai.ChatCompletion.create(model="any", messages=[{"role": "user",
-"content": "Hello world"}]) ``` ## Supported APIs ```py app.add_route("/", Ping
-()) app.add_route("/completions", completion) app.add_route("/chat/
-completions", chat_completion) app.add_route("/embeddings", embeddings)
-app.add_route("/engines/{engine}/embeddings", embeddings) app.add_route("/v1/
-completions", completion) app.add_route("/v1/chat/completions",
-chat_completion) app.add_route("/v1/embeddings", embeddings) app.add_route("/
-v1/engines/{engine}/embeddings", embeddings) ```
+general) | Nvidia A100(40GB) | | ChatGLM 6B INT4 | `THUDM/chatglm-6b-int4` |
+[modelzai/llm-chatglm-6b-int4](https://hub.docker.com/repository/docker/
+modelzai/llm-chatglm-6b-int4/general) | Nvidia T4(16GB) | | ChatGLM 6B |
+`THUDM/chatglm-6b` | [modelzai/llm-chatglm-6b](https://hub.docker.com/
+repository/docker/modelzai/llm-chatglm-6b/general) | Nvidia L4(24GB) | | Bloomz
+560M | `bigscience/bloomz-560m` | [modelzai/llm-bloomz-560m](https://
+hub.docker.com/repository/docker/modelzai/llm-bloomz-560m/general) | CPU | |
+Bloomz 1.7B | `bigscience/bloomz-1b7` | | CPU | | Bloomz 3B | `bigscience/
+bloomz-3b` | | Nvidia L4(24GB) | | Bloomz 7.1B | `bigscience/bloomz-7b1` | |
+Nvidia A100(40GB) | ### Use OpenAI python SDK Then you can use the OpenAI
+python SDK to interact with the model: ```python import openai
+openai.api_base="http://localhost:8000" openai.api_key="any" # create a chat
+completion chat_completion = openai.ChatCompletion.create(model="any",
+messages=[{"role": "user", "content": "Hello world"}]) ``` ### Integrate with
+Langchain You could also integrate modelz-llm with langchain: ```python import
+openai openai.api_base="http://localhost:8000" openai.api_key="any" from
+langchain.llms import OpenAI llm = OpenAI() llm.generate(prompts=["Could you
+please recommend some movies?"]) ``` ## Deploy on Modelz You could also deploy
+the modelz-llm directly on [Modelz](https://docs.modelz.ai): [![](./docs/
+images/deploy.svg)](https://cloud.modelz.ai/deployment/
+template?templateId=5e884bb3-6c32-468e-bc62-95cee55c17d4) ## Supported APIs
+Modelz LLM supports the following APIs for interacting with open source large
+language models: - `/completions` - `/chat/completions` - `/embeddings` - `/
+engines//embeddings` - `/v1/completions` - `/v1/chat/completions` - `/v1/
+embeddings` ## Acknowledgements - [FastChat](https://github.com/lm-sys/
+FastChat) for the prompt generation logic. - [Mosec](https://github.com/
+mosecorg/mosec) for the inference engine.
```

### Comparing `modelz-llm-23.6.9/build.envd` & `modelz-llm-23.7.1/build.envd`

 * *Files 9% similar despite different names*

```diff
@@ -10,21 +10,23 @@
     else:
         install.python_packages(requirements="requirements-cpu.txt")
 
 
 def build():
     base(dev=True)
     basic()
-    runtime.expose(envd_port=8000, host_port=8000, service="service")
+    shell("zsh")
+    runtime.expose(envd_port=8800, host_port=8800, service="service")
 
 
 def cpu():
     base(dev=True)
     basic(gpu=False)
-    runtime.expose(envd_port=8000, host_port=8000, service="service")
+    shell("zsh")
+    runtime.expose(envd_port=8800, host_port=8800, service="service")
 
 
 def serving():
     basic()
     io.copy("main.py", "/")
     run(["python main.py --dry-run"])
     config.entrypoint(["python", "main.py", "--timeout", "30000"])
```

### Comparing `modelz-llm-23.6.9/images/bloomz-560m/Dockerfile` & `modelz-llm-23.7.1/images/bloomz-560m/Dockerfile`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-ARG base=nvidia/cuda:11.6.2-cudnn8-runtime-ubuntu20.04
+ARG base=ubuntu:20.04
 
 FROM ${base}
 
 ENV DEBIAN_FRONTEND=noninteractive LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
 ENV PATH /opt/conda/bin:$PATH
 
 ARG MOSEC_PORT=8080
@@ -42,32 +42,30 @@
     ln -s /opt/conda/etc/profile.d/conda.sh /etc/profile.d/conda.sh && \
     echo ". /opt/conda/etc/profile.d/conda.sh" >> ~/.bashrc && \
     echo "conda activate base" >> ~/.bashrc && \
     find /opt/conda/ -follow -type f -name '*.a' -delete && \
     find /opt/conda/ -follow -type f -name '*.js.map' -delete && \
     /opt/conda/bin/conda clean -afy
 
-RUN conda create -n envd python=3.9
-
-ENV ENVD_PREFIX=/opt/conda/envs/envd/bin
+ENV ENVD_PREFIX=/opt/conda/bin
 
 RUN update-alternatives --install /usr/bin/python python ${ENVD_PREFIX}/python 1 && \
     update-alternatives --install /usr/bin/python3 python3 ${ENVD_PREFIX}/python3 1 && \
     update-alternatives --install /usr/bin/pip pip ${ENVD_PREFIX}/pip 1 && \
     update-alternatives --install /usr/bin/pip3 pip3 ${ENVD_PREFIX}/pip3 1
 
 COPY requirements.txt /
 
 RUN pip install -r requirements.txt
 
 RUN mkdir -p /workspace
 
 COPY . workspace/
 WORKDIR /workspace
-RUN pip install -e .[gpu]
+RUN pip install -e .
 
 RUN modelz-llm --dry-run --model bigscience/bloomz-560m
 
 # disable huggingface update check (could be very slow)
 ENV HF_HUB_OFFLINE=true
 
 ENTRYPOINT [ "modelz-llm" ]
```

### Comparing `modelz-llm-23.6.9/images/chatglm-6b/Dockerfile` & `modelz-llm-23.7.1/images/chatglm-6b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.9/images/chatglm-6b-int4/Dockerfile` & `modelz-llm-23.7.1/images/chatglm-6b-int4/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.9/images/fastchat-t5-3b/Dockerfile` & `modelz-llm-23.7.1/images/fastchat-t5-3b/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 ENV ENVD_PREFIX=/opt/conda/envs/envd/bin
 
 RUN update-alternatives --install /usr/bin/python python ${ENVD_PREFIX}/python 1 && \
     update-alternatives --install /usr/bin/python3 python3 ${ENVD_PREFIX}/python3 1 && \
     update-alternatives --install /usr/bin/pip pip ${ENVD_PREFIX}/pip 1 && \
     update-alternatives --install /usr/bin/pip3 pip3 ${ENVD_PREFIX}/pip3 1
 
-COPY /requirements.txt /
+COPY requirements.txt /
 
 RUN pip install -r requirements.txt
 
 RUN mkdir -p /workspace
 
 COPY . workspace/
 WORKDIR /workspace
```

### Comparing `modelz-llm-23.6.9/images/llama-7b/Dockerfile` & `modelz-llm-23.7.1/images/llama-7b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.9/images/vicuna-7b/Dockerfile` & `modelz-llm-23.7.1/images/vicuna-7b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.9/pyproject.toml` & `modelz-llm-23.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.9/src/modelz_llm/cli.py` & `modelz-llm-23.7.1/src/modelz_llm/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -60,8 +60,14 @@
     print(args)
 
     app = build_falcon_app(args)
     if args.dry_run:
         print("Dry run, exiting...")
         return
 
-    uvicorn.run(app, host="0.0.0.0", port=args.port, workers=args.worker)
+    uvicorn.run(
+        app,
+        host="0.0.0.0",
+        port=args.port,
+        workers=args.worker,
+        access_log=False,
+    )
```

### Comparing `modelz-llm-23.6.9/src/modelz_llm/mosec_service.py` & `modelz-llm-23.7.1/src/modelz_llm/mosec_service.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.9/src/modelz_llm/utils.py` & `modelz-llm-23.7.1/src/modelz_llm/utils.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.9/src/modelz_llm.egg-info/PKG-INFO` & `modelz-llm-23.7.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.6.9
+Version: 23.7.1
 Summary: LLM unified service
 Author-email: TensorChord <modelz@tensorchord.ai>
 Project-URL: Homepage, https://github.com/tensorchord/modelz-llm
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -21,70 +21,95 @@
 <a href="https://twitter.com/TensorChord"><img src="https://img.shields.io/twitter/follow/tensorchord?style=social" alt="trackgit-views" /></a>
 </p>
 
 Modelz LLM is an inference server that facilitates the utilization of open source large language models (LLMs), such as FastChat, LLaMA, and ChatGLM, on either **local or cloud-based** environments with **OpenAI compatible API**.
 
 ## Features
 
-- **OpenAI compatible API**: Modelz LLM provides an OpenAI compatible API for LLMs, which means you can use the OpenAI python SDK to interact with the model.
+- **OpenAI compatible API**: Modelz LLM provides an OpenAI compatible API for LLMs, which means you can use the OpenAI python SDK or LangChain to interact with the model.
 - **Self-hosted**: Modelz LLM can be easily deployed on either local or cloud-based environments.
 - **Open source LLMs**: Modelz LLM supports open source LLMs, such as FastChat, LLaMA, and ChatGLM.
-- **Cloud native**: We provide docker images for different LLMs, which can be easily deployed on Kubernetes, or other cloud-based environments (e.g. [Modelz](https://docs.modelz.ai))
+- **Cloud native**: We provide docker images for different LLMs, which can be easily deployed on Kubernetes, or other cloud-based environments (e.g. [Modelz](https://modelz.ai))
 
 ## Quick Start
 
 ### Install
 
 ```bash
-pip install modelz-llm[gpu]
+pip install modelz-llm
 # or install from source
 pip install git+https://github.com/tensorchord/modelz-llm.git[gpu]
 ```
 
 ### Run the self-hosted API server
 
 Please first start the self-hosted API server by following the instructions:
 
 ```bash
-modelz-llm -m "THUDM/chatglm-6b-int4"
+modelz-llm -m bigscience/bloomz-560m --device cpu
 ```
 
 Currently, we support the following models:
 
-| Model Name | Huggingface Model | Docker Image |
-| ---------- | ----------- | ---------------- |
-|FastChat T5 | `lmsys/fastchat-t5-3b-v1.0` | [modelzai/llm-fastchat-t5-3b](https://hub.docker.com/repository/docker/modelzai/llm-fastchat-t5-3b/general)
-| Vicuna 7B Delta V1.1  | `lmsys/vicuna-7b-delta-v1.1` | [modelzai/llm-vicuna-7b](https://hub.docker.com/repository/docker/modelzai/llm-vicuna-7b/general) |
-| LLaMA 7B    | `decapoda-research/llama-7b-hf` | [modelzai/llm-llama-7b](https://hub.docker.com/repository/docker/modelzai/llm-llama-7b/general) |
-| ChatGLM 6B INT4    | `THUDM/chatglm-6b-int4` | [modelzai/llm-chatglm-6b-int4](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b-int4/general) |
-| ChatGLM 6B  | `THUDM/chatglm-6b` | [modelzai/llm-chatglm-6b](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b/general) |
-| Bloomz 560M | `bigscience/bloomz-560m` | |
-| Bloomz 1.7B | `bigscience/bloomz-1b7` | |
-| Bloomz 3B | `bigscience/bloomz-3b` | |
-| Bloomz 7.1B | `bigscience/bloomz-7b1` | |
+| Model Name | Huggingface Model | Docker Image | Recommended GPU
+| ---------- | ----------- | ---------------- | -- |
+| FastChat T5 | `lmsys/fastchat-t5-3b-v1.0` | [modelzai/llm-fastchat-t5-3b](https://hub.docker.com/repository/docker/modelzai/llm-fastchat-t5-3b/general) | Nvidia L4(24GB) |
+| Vicuna 7B Delta V1.1  | `lmsys/vicuna-7b-delta-v1.1` | [modelzai/llm-vicuna-7b](https://hub.docker.com/repository/docker/modelzai/llm-vicuna-7b/general) | Nvidia A100(40GB) |
+| LLaMA 7B    | `decapoda-research/llama-7b-hf` | [modelzai/llm-llama-7b](https://hub.docker.com/repository/docker/modelzai/llm-llama-7b/general) | Nvidia A100(40GB) |
+| ChatGLM 6B INT4    | `THUDM/chatglm-6b-int4` | [modelzai/llm-chatglm-6b-int4](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b-int4/general) | Nvidia T4(16GB) |
+| ChatGLM 6B  | `THUDM/chatglm-6b` | [modelzai/llm-chatglm-6b](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b/general) | Nvidia L4(24GB) |
+| Bloomz 560M | `bigscience/bloomz-560m` | [modelzai/llm-bloomz-560m](https://hub.docker.com/repository/docker/modelzai/llm-bloomz-560m/general) | CPU |
+| Bloomz 1.7B | `bigscience/bloomz-1b7` | | CPU |
+| Bloomz 3B | `bigscience/bloomz-3b` |  | Nvidia L4(24GB) |
+| Bloomz 7.1B | `bigscience/bloomz-7b1` | | Nvidia A100(40GB) |
 
 ### Use OpenAI python SDK
 
 Then you can use the OpenAI python SDK to interact with the model:
 
 ```python
 import openai
 openai.api_base="http://localhost:8000"
 openai.api_key="any"
 
 # create a chat completion
 chat_completion = openai.ChatCompletion.create(model="any", messages=[{"role": "user", "content": "Hello world"}])
 ```
 
-## Supported APIs
+### Integrate with Langchain
+
+You could also integrate modelz-llm with langchain:
+
+```python
+import openai
+openai.api_base="http://localhost:8000"
+openai.api_key="any"
+
+from langchain.llms import OpenAI
+
+llm = OpenAI()
 
-```py
-    app.add_route("/", Ping())
-    app.add_route("/completions", completion)
-    app.add_route("/chat/completions", chat_completion)
-    app.add_route("/embeddings", embeddings)
-    app.add_route("/engines/{engine}/embeddings", embeddings)
-    app.add_route("/v1/completions", completion)
-    app.add_route("/v1/chat/completions", chat_completion)
-    app.add_route("/v1/embeddings", embeddings)
-    app.add_route("/v1/engines/{engine}/embeddings", embeddings)
+llm.generate(prompts=["Could you please recommend some movies?"])
 ```
+
+## Deploy on Modelz
+
+You could also deploy the modelz-llm directly on [Modelz](https://docs.modelz.ai):
+
+[![](./docs/images/deploy.svg)](https://cloud.modelz.ai/deployment/template?templateId=5e884bb3-6c32-468e-bc62-95cee55c17d4)
+
+## Supported APIs
+
+Modelz LLM supports the following APIs for interacting with open source large language models:
+
+- `/completions`
+- `/chat/completions`
+- `/embeddings`
+- `/engines/<any>/embeddings`
+- `/v1/completions`
+- `/v1/chat/completions`
+- `/v1/embeddings`
+
+## Acknowledgements
+
+- [FastChat](https://github.com/lm-sys/FastChat) for the prompt generation logic.
+- [Mosec](https://github.com/mosecorg/mosec) for the inference engine.
```

#### html2text {}

```diff
@@ -1,47 +1,58 @@
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.9 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.7.1 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
 Modelz LLM is an inference server that facilitates the utilization of open
 source large language models (LLMs), such as FastChat, LLaMA, and ChatGLM, on
 either **local or cloud-based** environments with **OpenAI compatible API**. ##
 Features - **OpenAI compatible API**: Modelz LLM provides an OpenAI compatible
-API for LLMs, which means you can use the OpenAI python SDK to interact with
-the model. - **Self-hosted**: Modelz LLM can be easily deployed on either local
-or cloud-based environments. - **Open source LLMs**: Modelz LLM supports open
-source LLMs, such as FastChat, LLaMA, and ChatGLM. - **Cloud native**: We
-provide docker images for different LLMs, which can be easily deployed on
-Kubernetes, or other cloud-based environments (e.g. [Modelz](https://
-docs.modelz.ai)) ## Quick Start ### Install ```bash pip install modelz-llm[gpu]
-# or install from source pip install git+https://github.com/tensorchord/modelz-
+API for LLMs, which means you can use the OpenAI python SDK or LangChain to
+interact with the model. - **Self-hosted**: Modelz LLM can be easily deployed
+on either local or cloud-based environments. - **Open source LLMs**: Modelz LLM
+supports open source LLMs, such as FastChat, LLaMA, and ChatGLM. - **Cloud
+native**: We provide docker images for different LLMs, which can be easily
+deployed on Kubernetes, or other cloud-based environments (e.g. [Modelz](https:
+//modelz.ai)) ## Quick Start ### Install ```bash pip install modelz-llm # or
+install from source pip install git+https://github.com/tensorchord/modelz-
 llm.git[gpu] ``` ### Run the self-hosted API server Please first start the
 self-hosted API server by following the instructions: ```bash modelz-llm -
-m "THUDM/chatglm-6b-int4" ``` Currently, we support the following models: |
-Model Name | Huggingface Model | Docker Image | | ---------- | ----------- | --
--------------- | |FastChat T5 | `lmsys/fastchat-t5-3b-v1.0` | [modelzai/llm-
-fastchat-t5-3b](https://hub.docker.com/repository/docker/modelzai/llm-fastchat-
-t5-3b/general) | Vicuna 7B Delta V1.1 | `lmsys/vicuna-7b-delta-v1.1` |
-[modelzai/llm-vicuna-7b](https://hub.docker.com/repository/docker/modelzai/llm-
-vicuna-7b/general) | | LLaMA 7B | `decapoda-research/llama-7b-hf` | [modelzai/
+m bigscience/bloomz-560m --device cpu ``` Currently, we support the following
+models: | Model Name | Huggingface Model | Docker Image | Recommended GPU | ---
+------- | ----------- | ---------------- | -- | | FastChat T5 | `lmsys/
+fastchat-t5-3b-v1.0` | [modelzai/llm-fastchat-t5-3b](https://hub.docker.com/
+repository/docker/modelzai/llm-fastchat-t5-3b/general) | Nvidia L4(24GB) | |
+Vicuna 7B Delta V1.1 | `lmsys/vicuna-7b-delta-v1.1` | [modelzai/llm-vicuna-7b]
+(https://hub.docker.com/repository/docker/modelzai/llm-vicuna-7b/general) |
+Nvidia A100(40GB) | | LLaMA 7B | `decapoda-research/llama-7b-hf` | [modelzai/
 llm-llama-7b](https://hub.docker.com/repository/docker/modelzai/llm-llama-7b/
-general) | | ChatGLM 6B INT4 | `THUDM/chatglm-6b-int4` | [modelzai/llm-chatglm-
-6b-int4](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b-int4/
-general) | | ChatGLM 6B | `THUDM/chatglm-6b` | [modelzai/llm-chatglm-6b](https:
-//hub.docker.com/repository/docker/modelzai/llm-chatglm-6b/general) | | Bloomz
-560M | `bigscience/bloomz-560m` | | | Bloomz 1.7B | `bigscience/bloomz-1b7` | |
-| Bloomz 3B | `bigscience/bloomz-3b` | | | Bloomz 7.1B | `bigscience/bloomz-
-7b1` | | ### Use OpenAI python SDK Then you can use the OpenAI python SDK to
-interact with the model: ```python import openai openai.api_base="http://
-localhost:8000" openai.api_key="any" # create a chat completion chat_completion
-= openai.ChatCompletion.create(model="any", messages=[{"role": "user",
-"content": "Hello world"}]) ``` ## Supported APIs ```py app.add_route("/", Ping
-()) app.add_route("/completions", completion) app.add_route("/chat/
-completions", chat_completion) app.add_route("/embeddings", embeddings)
-app.add_route("/engines/{engine}/embeddings", embeddings) app.add_route("/v1/
-completions", completion) app.add_route("/v1/chat/completions",
-chat_completion) app.add_route("/v1/embeddings", embeddings) app.add_route("/
-v1/engines/{engine}/embeddings", embeddings) ```
+general) | Nvidia A100(40GB) | | ChatGLM 6B INT4 | `THUDM/chatglm-6b-int4` |
+[modelzai/llm-chatglm-6b-int4](https://hub.docker.com/repository/docker/
+modelzai/llm-chatglm-6b-int4/general) | Nvidia T4(16GB) | | ChatGLM 6B |
+`THUDM/chatglm-6b` | [modelzai/llm-chatglm-6b](https://hub.docker.com/
+repository/docker/modelzai/llm-chatglm-6b/general) | Nvidia L4(24GB) | | Bloomz
+560M | `bigscience/bloomz-560m` | [modelzai/llm-bloomz-560m](https://
+hub.docker.com/repository/docker/modelzai/llm-bloomz-560m/general) | CPU | |
+Bloomz 1.7B | `bigscience/bloomz-1b7` | | CPU | | Bloomz 3B | `bigscience/
+bloomz-3b` | | Nvidia L4(24GB) | | Bloomz 7.1B | `bigscience/bloomz-7b1` | |
+Nvidia A100(40GB) | ### Use OpenAI python SDK Then you can use the OpenAI
+python SDK to interact with the model: ```python import openai
+openai.api_base="http://localhost:8000" openai.api_key="any" # create a chat
+completion chat_completion = openai.ChatCompletion.create(model="any",
+messages=[{"role": "user", "content": "Hello world"}]) ``` ### Integrate with
+Langchain You could also integrate modelz-llm with langchain: ```python import
+openai openai.api_base="http://localhost:8000" openai.api_key="any" from
+langchain.llms import OpenAI llm = OpenAI() llm.generate(prompts=["Could you
+please recommend some movies?"]) ``` ## Deploy on Modelz You could also deploy
+the modelz-llm directly on [Modelz](https://docs.modelz.ai): [![](./docs/
+images/deploy.svg)](https://cloud.modelz.ai/deployment/
+template?templateId=5e884bb3-6c32-468e-bc62-95cee55c17d4) ## Supported APIs
+Modelz LLM supports the following APIs for interacting with open source large
+language models: - `/completions` - `/chat/completions` - `/embeddings` - `/
+engines//embeddings` - `/v1/completions` - `/v1/chat/completions` - `/v1/
+embeddings` ## Acknowledgements - [FastChat](https://github.com/lm-sys/
+FastChat) for the prompt generation logic. - [Mosec](https://github.com/
+mosecorg/mosec) for the inference engine.
```

### Comparing `modelz-llm-23.6.9/src/modelz_llm.egg-info/SOURCES.txt` & `modelz-llm-23.7.1/src/modelz_llm.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,26 +7,31 @@
 pyproject.toml
 requirements-cpu.txt
 requirements.txt
 .github/workflows/docker-publish.yml
 .github/workflows/gcr.yml
 .github/workflows/python-check.yml
 .github/workflows/python-publish.yml
+docs/images/deploy.svg
 images/bloomz-560m/Dockerfile
 images/chatglm-6b/Dockerfile
 images/chatglm-6b-int4/Dockerfile
 images/fastchat-t5-3b/Dockerfile
 images/llama-7b/Dockerfile
 images/llama-7b/requirements.txt
 images/vicuna-7b/Dockerfile
 src/modelz_llm/__init__.py
 src/modelz_llm/_version.py
 src/modelz_llm/cli.py
+src/modelz_llm/emb.py
 src/modelz_llm/falcon_service.py
+src/modelz_llm/log.py
+src/modelz_llm/model.py
 src/modelz_llm/mosec_service.py
+src/modelz_llm/uds.py
 src/modelz_llm/utils.py
 src/modelz_llm.egg-info/PKG-INFO
 src/modelz_llm.egg-info/SOURCES.txt
 src/modelz_llm.egg-info/dependency_links.txt
 src/modelz_llm.egg-info/entry_points.txt
 src/modelz_llm.egg-info/requires.txt
 src/modelz_llm.egg-info/top_level.txt
```

