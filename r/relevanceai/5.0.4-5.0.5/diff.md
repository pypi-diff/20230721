# Comparing `tmp/relevanceai-5.0.4.tar.gz` & `tmp/relevanceai-5.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relevanceai-5.0.4.tar", last modified: Mon Jul 17 13:57:12 2023, max compression
+gzip compressed data, was "relevanceai-5.0.5.tar", last modified: Fri Jul 21 01:38:59 2023, max compression
```

## Comparing `relevanceai-5.0.4.tar` & `relevanceai-5.0.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 13:57:12.676001 relevanceai-5.0.4/
--rw-rw-rw-   0        0        0    11547 2023-07-17 13:38:32.000000 relevanceai-5.0.4/LICENSE
--rw-rw-rw-   0        0        0     1192 2023-07-17 13:57:12.675001 relevanceai-5.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      970 2023-07-17 13:38:32.000000 relevanceai-5.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 13:57:12.646989 relevanceai-5.0.4/relevanceai/
--rw-rw-rw-   0        0        0      279 2023-07-17 13:57:03.000000 relevanceai-5.0.4/relevanceai/__init__.py
--rw-rw-rw-   0        0        0      117 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/_request.py
--rw-rw-rw-   0        0        0     2158 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/auth.py
--rw-rw-rw-   0        0        0     6646 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/chain.py
-drwxrwxrwx   0        0        0        0 2023-07-17 13:57:12.656989 relevanceai-5.0.4/relevanceai/connect/
--rw-rw-rw-   0        0        0        0 2023-07-17 13:53:04.000000 relevanceai-5.0.4/relevanceai/connect/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 13:57:12.658989 relevanceai-5.0.4/relevanceai/connect/fastapi/
--rw-rw-rw-   0        0        0       99 2023-07-17 13:56:57.000000 relevanceai-5.0.4/relevanceai/connect/fastapi/__init__.py
--rw-rw-rw-   0        0        0     4325 2023-07-17 13:44:35.000000 relevanceai-5.0.4/relevanceai/connect/fastapi/chains.py
--rw-rw-rw-   0        0        0     3812 2023-07-17 13:50:03.000000 relevanceai-5.0.4/relevanceai/connect/fastapi/steps.py
--rw-rw-rw-   0        0        0     3401 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/datasets.py
--rw-rw-rw-   0        0        0     1046 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/env.py
-drwxrwxrwx   0        0        0        0 2023-07-17 13:57:12.660989 relevanceai-5.0.4/relevanceai/frontend/
--rw-rw-rw-   0        0        0      104 2023-07-17 13:40:02.000000 relevanceai-5.0.4/relevanceai/frontend/__init__.py
--rw-rw-rw-   0        0        0      686 2023-07-17 06:16:31.000000 relevanceai-5.0.4/relevanceai/frontend/input_components.py
--rw-rw-rw-   0        0        0     1908 2023-07-17 13:39:59.000000 relevanceai-5.0.4/relevanceai/frontend/upload_file.py
--rw-rw-rw-   0        0        0     4586 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/params.py
-drwxrwxrwx   0        0        0        0 2023-07-17 13:57:12.675001 relevanceai-5.0.4/relevanceai/steps/
--rw-rw-rw-   0        0        0      600 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/steps/__init__.py
--rw-rw-rw-   0        0        0     2671 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/steps/_base.py
--rw-rw-rw-   0        0        0     1994 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/steps/api_call.py
--rw-rw-rw-   0        0        0     1150 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/steps/execute_javascript.py
--rw-rw-rw-   0        0        0     1285 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/steps/generate_vector_embedding.py
--rw-rw-rw-   0        0        0     3751 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/steps/prompt_completion.py
--rw-rw-rw-   0        0        0     1721 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/steps/redis_vector_search.py
--rw-rw-rw-   0        0        0     1018 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/steps/run_chain.py
--rw-rw-rw-   0        0        0     2829 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/steps/run_step.py
--rw-rw-rw-   0        0        0     2120 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/steps/vector_search.py
--rw-rw-rw-   0        0        0     1728 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/steps/vectorize_and_search.py
-drwxrwxrwx   0        0        0        0 2023-07-17 13:57:12.653989 relevanceai-5.0.4/relevanceai.egg-info/
--rw-rw-rw-   0        0        0     1192 2023-07-17 13:57:12.000000 relevanceai-5.0.4/relevanceai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1003 2023-07-17 13:57:12.000000 relevanceai-5.0.4/relevanceai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 13:57:12.000000 relevanceai-5.0.4/relevanceai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 13:57:12.000000 relevanceai-5.0.4/relevanceai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-17 13:57:12.000000 relevanceai-5.0.4/relevanceai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 13:57:12.676001 relevanceai-5.0.4/setup.cfg
--rw-rw-rw-   0        0        0      572 2023-07-17 13:38:32.000000 relevanceai-5.0.4/setup.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-07-21 01:38:59.831077 relevanceai-5.0.5/
+-rw-r--r--   0 jackykoh   (502) staff       (20)    11547 2023-06-03 05:15:28.000000 relevanceai-5.0.5/LICENSE
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1165 2023-07-21 01:38:59.830916 relevanceai-5.0.5/PKG-INFO
+-rw-r--r--   0 jackykoh   (502) staff       (20)      953 2023-06-03 07:08:05.000000 relevanceai-5.0.5/README.md
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-07-21 01:38:59.826198 relevanceai-5.0.5/relevanceai/
+-rw-r--r--   0 jackykoh   (502) staff       (20)      272 2023-07-20 07:34:26.000000 relevanceai-5.0.5/relevanceai/__init__.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)      112 2023-06-03 05:16:32.000000 relevanceai-5.0.5/relevanceai/_request.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2085 2023-06-03 05:16:32.000000 relevanceai-5.0.5/relevanceai/auth.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     6447 2023-07-20 07:21:31.000000 relevanceai-5.0.5/relevanceai/chain.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-07-21 01:38:59.827183 relevanceai-5.0.5/relevanceai/connect/
+-rw-r--r--   0 jackykoh   (502) staff       (20)        0 2023-07-20 07:21:31.000000 relevanceai-5.0.5/relevanceai/connect/__init__.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-07-21 01:38:59.827612 relevanceai-5.0.5/relevanceai/connect/fastapi/
+-rw-r--r--   0 jackykoh   (502) staff       (20)       97 2023-07-20 07:21:31.000000 relevanceai-5.0.5/relevanceai/connect/fastapi/__init__.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     4201 2023-07-20 07:37:33.000000 relevanceai-5.0.5/relevanceai/connect/fastapi/chains.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     3705 2023-07-20 07:21:31.000000 relevanceai-5.0.5/relevanceai/connect/fastapi/steps.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     3288 2023-06-03 16:21:52.000000 relevanceai-5.0.5/relevanceai/datasets.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1010 2023-06-03 05:16:32.000000 relevanceai-5.0.5/relevanceai/env.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-07-21 01:38:59.828452 relevanceai-5.0.5/relevanceai/frontend/
+-rw-r--r--   0 jackykoh   (502) staff       (20)      103 2023-07-20 07:21:31.000000 relevanceai-5.0.5/relevanceai/frontend/__init__.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)      654 2023-07-20 07:21:31.000000 relevanceai-5.0.5/relevanceai/frontend/input_components.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1850 2023-07-20 07:21:31.000000 relevanceai-5.0.5/relevanceai/frontend/upload_file.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     4404 2023-06-03 05:16:32.000000 relevanceai-5.0.5/relevanceai/params.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-07-21 01:38:59.830690 relevanceai-5.0.5/relevanceai/steps/
+-rw-r--r--   0 jackykoh   (502) staff       (20)      590 2023-07-20 07:21:31.000000 relevanceai-5.0.5/relevanceai/steps/__init__.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2595 2023-07-20 07:21:31.000000 relevanceai-5.0.5/relevanceai/steps/_base.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1933 2023-06-03 06:58:35.000000 relevanceai-5.0.5/relevanceai/steps/api_call.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1121 2023-06-03 06:58:35.000000 relevanceai-5.0.5/relevanceai/steps/execute_javascript.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1246 2023-06-03 06:58:35.000000 relevanceai-5.0.5/relevanceai/steps/generate_vector_embedding.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     3676 2023-06-03 06:58:35.000000 relevanceai-5.0.5/relevanceai/steps/prompt_completion.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1670 2023-06-03 06:58:35.000000 relevanceai-5.0.5/relevanceai/steps/redis_vector_search.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)      985 2023-06-03 14:40:31.000000 relevanceai-5.0.5/relevanceai/steps/run_chain.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2750 2023-07-20 07:21:31.000000 relevanceai-5.0.5/relevanceai/steps/run_step.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2059 2023-06-03 06:58:35.000000 relevanceai-5.0.5/relevanceai/steps/vector_search.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1679 2023-06-03 06:58:35.000000 relevanceai-5.0.5/relevanceai/steps/vectorize_and_search.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-07-21 01:38:59.827025 relevanceai-5.0.5/relevanceai.egg-info/
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1165 2023-07-21 01:38:59.000000 relevanceai-5.0.5/relevanceai.egg-info/PKG-INFO
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1003 2023-07-21 01:38:59.000000 relevanceai-5.0.5/relevanceai.egg-info/SOURCES.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)        1 2023-07-21 01:38:59.000000 relevanceai-5.0.5/relevanceai.egg-info/dependency_links.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)        9 2023-07-21 01:38:59.000000 relevanceai-5.0.5/relevanceai.egg-info/requires.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)       12 2023-07-21 01:38:59.000000 relevanceai-5.0.5/relevanceai.egg-info/top_level.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)       38 2023-07-21 01:38:59.831118 relevanceai-5.0.5/setup.cfg
+-rw-r--r--   0 jackykoh   (502) staff       (20)      551 2023-06-03 05:17:49.000000 relevanceai-5.0.5/setup.py
```

### Comparing `relevanceai-5.0.4/LICENSE` & `relevanceai-5.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.4/PKG-INFO` & `relevanceai-5.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1
-Name: relevanceai
-Version: 5.0.4
-Home-page: https://relevanceai.com/
-Author: Relevance AI
-Author-email: jacky@relevanceai.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## Relevance AI - The platform for building and deploying AI chains and Agents
-[![License](https://img.shields.io/pypi/l/relevanceai)](https://img.shields.io/pypi/l/relevanceai)
-
-🔥 Use Relevance to unlock the value of LLMs:
-- ⚡ Quickly build and deploy chains in a few lines of code with fully managed deployment.
-- 🔎 Drilldown with filters and similarity search to explore and find insights.
-- 🔑 Vectors, storing and querying vectors with flexible vector similarity search, that can be combined with multiple vectors, aggregates and filters.
-- 🚀 Share chains as data apps with your team.
-
-[Sign up for a free account ->](https://chain.relevanceai.com)
-
-## 🧠 Documentation
-
-| Type      | Link |
-| ------------- | ----------- |
-| Python SDK | [Documentation](https://sdk.relevanceai.com/) |
-| Dashboard | [Documentation](https://chain.relevanceai.com/) |
-| Javascript SDK | [Documentation](https://documentation.relevanceai.com)        |
+Metadata-Version: 2.1
+Name: relevanceai
+Version: 5.0.5
+Home-page: https://relevanceai.com/
+Author: Relevance AI
+Author-email: jacky@relevanceai.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## Relevance AI - The platform for building and deploying AI chains and Agents
+[![License](https://img.shields.io/pypi/l/relevanceai)](https://img.shields.io/pypi/l/relevanceai)
+
+🔥 Use Relevance to unlock the value of LLMs:
+- ⚡ Quickly build and deploy chains in a few lines of code with fully managed deployment.
+- 🔎 Drilldown with filters and similarity search to explore and find insights.
+- 🔑 Vectors, storing and querying vectors with flexible vector similarity search, that can be combined with multiple vectors, aggregates and filters.
+- 🚀 Share chains as data apps with your team.
+
+[Sign up for a free account ->](https://chain.relevanceai.com)
+
+## 🧠 Documentation
+
+| Type      | Link |
+| ------------- | ----------- |
+| Python SDK | [Documentation](https://sdk.relevanceai.com/) |
+| Dashboard | [Documentation](https://chain.relevanceai.com/) |
+| Javascript SDK | [Documentation](https://documentation.relevanceai.com)        |
```

### Comparing `relevanceai-5.0.4/README.md` & `relevanceai-5.0.5/README.md`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-## Relevance AI - The platform for building and deploying AI chains and Agents
-[![License](https://img.shields.io/pypi/l/relevanceai)](https://img.shields.io/pypi/l/relevanceai)
-
-🔥 Use Relevance to unlock the value of LLMs:
-- ⚡ Quickly build and deploy chains in a few lines of code with fully managed deployment.
-- 🔎 Drilldown with filters and similarity search to explore and find insights.
-- 🔑 Vectors, storing and querying vectors with flexible vector similarity search, that can be combined with multiple vectors, aggregates and filters.
-- 🚀 Share chains as data apps with your team.
-
-[Sign up for a free account ->](https://chain.relevanceai.com)
-
-## 🧠 Documentation
-
-| Type      | Link |
-| ------------- | ----------- |
-| Python SDK | [Documentation](https://sdk.relevanceai.com/) |
-| Dashboard | [Documentation](https://chain.relevanceai.com/) |
+## Relevance AI - The platform for building and deploying AI chains and Agents
+[![License](https://img.shields.io/pypi/l/relevanceai)](https://img.shields.io/pypi/l/relevanceai)
+
+🔥 Use Relevance to unlock the value of LLMs:
+- ⚡ Quickly build and deploy chains in a few lines of code with fully managed deployment.
+- 🔎 Drilldown with filters and similarity search to explore and find insights.
+- 🔑 Vectors, storing and querying vectors with flexible vector similarity search, that can be combined with multiple vectors, aggregates and filters.
+- 🚀 Share chains as data apps with your team.
+
+[Sign up for a free account ->](https://chain.relevanceai.com)
+
+## 🧠 Documentation
+
+| Type      | Link |
+| ------------- | ----------- |
+| Python SDK | [Documentation](https://sdk.relevanceai.com/) |
+| Dashboard | [Documentation](https://chain.relevanceai.com/) |
 | Javascript SDK | [Documentation](https://documentation.relevanceai.com)        |
```

### Comparing `relevanceai-5.0.4/relevanceai/auth.py` & `relevanceai-5.0.5/relevanceai/auth.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-import os
-import json
-import getpass
-
-
-class Config:
-    def __init__(self):
-        self._auth = None
-        self.headers = {}
-
-    @property
-    def auth(self):
-        if not self._auth:
-            login()
-        return self._auth
-
-    def set_auth(self, auth):
-        self._auth = auth
-
-
-config = Config()
-
-
-class Auth:
-    def __init__(self, api_key: str, region: str, project: str):
-        self.api_key = api_key
-        self.region = region
-        self.project = project
-        self.headers = {"Authorization": f"{project}:{api_key}"}
-
-
-def login(
-    api_key: str = None, region: str = None, project: str = None, store: bool = True
-):
-    cred_path = os.path.expanduser("~/relevanceai.json")
-    cred_json = {}
-    try:
-        if os.path.exists(cred_path):
-            with open(cred_path, "r") as f:
-                cred_json = json.load(f)
-    except:
-        print("Error reading credentials file, please login again")
-
-    if cred_json:
-        if api_key and region and project:
-            cred_json = {"api_key": api_key, "region": region, "project": project}
-    else:
-        print(
-            "You can create and find your API key in your browser here: https://chain.relevanceai.com/login/sdk"
-        )
-        if not api_key:
-            api_key = os.getenv("RELEVANCE_API_KEY") or getpass.getpass(
-                "Paste the API key from your profile and hit enter: "
-            )
-
-        if not region:
-            region = os.getenv("RELEVANCE_REGION") or input(
-                "Paste the Region from your profile and hit enter: "
-            )
-
-        if not project:
-            project = os.getenv("RELEVANCE_PROJECT") or input(
-                "Paste the Project from your profile and hit enter: "
-            )
-
-        cred_json = {"api_key": api_key, "region": region, "project": project}
-    config.set_auth(Auth(**cred_json))
-    # TBC: make it more secure with netsrc
-    if store:
-        with open(cred_path, "w") as f:
-            json.dump(cred_json, f)
-        os.chmod(cred_path, 0o600)
-    print("Successfully logged in, welcome!")
+import os
+import json
+import getpass
+
+
+class Config:
+    def __init__(self):
+        self._auth = None
+        self.headers = {}
+
+    @property
+    def auth(self):
+        if not self._auth:
+            login()
+        return self._auth
+
+    def set_auth(self, auth):
+        self._auth = auth
+
+
+config = Config()
+
+
+class Auth:
+    def __init__(self, api_key: str, region: str, project: str):
+        self.api_key = api_key
+        self.region = region
+        self.project = project
+        self.headers = {"Authorization": f"{project}:{api_key}"}
+
+
+def login(
+    api_key: str = None, region: str = None, project: str = None, store: bool = True
+):
+    cred_path = os.path.expanduser("~/relevanceai.json")
+    cred_json = {}
+    try:
+        if os.path.exists(cred_path):
+            with open(cred_path, "r") as f:
+                cred_json = json.load(f)
+    except:
+        print("Error reading credentials file, please login again")
+
+    if cred_json:
+        if api_key and region and project:
+            cred_json = {"api_key": api_key, "region": region, "project": project}
+    else:
+        print(
+            "You can create and find your API key in your browser here: https://chain.relevanceai.com/login/sdk"
+        )
+        if not api_key:
+            api_key = os.getenv("RELEVANCE_API_KEY") or getpass.getpass(
+                "Paste the API key from your profile and hit enter: "
+            )
+
+        if not region:
+            region = os.getenv("RELEVANCE_REGION") or input(
+                "Paste the Region from your profile and hit enter: "
+            )
+
+        if not project:
+            project = os.getenv("RELEVANCE_PROJECT") or input(
+                "Paste the Project from your profile and hit enter: "
+            )
+
+        cred_json = {"api_key": api_key, "region": region, "project": project}
+    config.set_auth(Auth(**cred_json))
+    # TBC: make it more secure with netsrc
+    if store:
+        with open(cred_path, "w") as f:
+            json.dump(cred_json, f)
+        os.chmod(cred_path, 0o600)
+    print("Successfully logged in, welcome!")
```

### Comparing `relevanceai-5.0.4/relevanceai/chain.py` & `relevanceai-5.0.5/relevanceai/chain.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,199 +1,199 @@
-import json
-import requests
-from relevanceai._request import handle_response
-from relevanceai import config
-from relevanceai.auth import Auth
-from relevanceai.params import Parameters
-
-
-def create(name, description="", parameters={}, id=None, auth=None):
-    chain = Chain(
-        name=name, description=description, parameters=parameters, id=id, auth=auth
-    )
-    return chain
-
-
-def load(id, auth=None):
-    if auth is None:
-        auth = config.auth
-    response = requests.get(
-        f"https://api-{auth.region}.stack.tryrelevance.com/latest/studios/{auth.project}/{id}",
-        json={
-            "filters": [
-                {
-                    "field": "studio_id",
-                    "condition": "==",
-                    "condition_value": id,
-                    "filter_type": "exact_match",
-                },
-                {
-                    "field": "project",
-                    "condition": "==",
-                    "condition_value": auth.project,
-                    "filter_type": "exact_match",
-                },
-            ]
-        },
-    )
-    res = handle_response(response)
-    chain = Chain(name="", description="", parameters={}, id=id, auth=auth)
-    return chain
-
-
-def load_from_json(filepath_or_json):
-    if isinstance(filepath_or_json, str):
-        with open(filepath_or_json, "r") as f:
-            chain_json = json.load(f)
-    else:
-        chain_json = filepath_or_json
-    chain = Chain(
-        name=chain_json["title"],
-        description=chain_json["description"],
-        parameters=chain_json["params_schema"]["properties"],
-        id=chain_json["studio_id"],
-    )
-    chain.add(chain_json["transformations"]["steps"])
-    return chain
-
-
-class Chain:
-    def __init__(
-        self,
-        name: str,
-        description: str = "",
-        parameters={},
-        id: str = None,
-        auth: Auth = None,
-    ):
-        self.name = name
-        self.description = description
-        self._parameters = parameters
-        self.steps = []
-        # generate random id if none
-        self.random_id = False
-        if id is None:
-            import uuid
-
-            id = str(uuid.uuid4())
-            self.random_id = True
-        self.id = id
-        self.auth: Auth = config.auth if auth is None else auth
-
-    @property
-    def parameters(self):
-        return Parameters(self._parameters)
-
-    params = parameters
-
-    def add(self, steps):
-        if isinstance(steps, list):
-            self.steps.extend(steps)
-        else:
-            self.steps.append(steps)
-
-    def _transform_steps(self, steps):
-        chain_steps = [step.steps[0] for step in steps]
-        unique_ids = []
-        for step in chain_steps:
-            if step["name"] in unique_ids:
-                raise ValueError(
-                    f"Duplicate step name {step['name']}, please rename the step name with Step(step_name=step_name)."
-                )
-            unique_ids.append(step["name"])
-        return chain_steps
-
-    def _trigger_json(
-        self, values: dict = {}, return_state: bool = True, public: bool = False
-    ):
-        data = {
-            "return_state": return_state,
-            "studio_override": {
-                "public": public,
-                "transformations": {"steps": self._transform_steps(self.steps)},
-                "params_schema": {"properties": self.parameters.to_json()},
-            },
-            "params": values,
-        }
-        data["studio_id"] = self.id
-        data["studio_override"]["studio_id"] = self.id
-        return data
-
-    def run(self, parameters={}, full_response: bool = False):
-        url = f"https://api-{self.auth.region}.stack.tryrelevance.com/latest/studios/{self.auth.project}"
-        response = requests.post(
-            f"{url}/trigger",
-            json=self._trigger_json(parameters),
-            headers=self.auth.headers,
-        )
-        res = handle_response(response)
-        if isinstance(res, dict):
-            if ("errors" in res and res["errors"]) or full_response:
-                return res
-            elif "output" in res:
-                return res["output"]
-        return res
-
-    def _json(self):
-        data = {
-            "title": self.name,
-            "description": self.description,
-            "version": "latest",
-            "project": self.auth.project,
-            "public": False,
-            "params_schema": {"properties": self.parameters.to_json()},
-            "transformations": {"steps": self._transform_steps(self.steps)},
-        }
-        data["studio_id"] = self.id
-        return data
-
-    def deploy(self):
-        url = f"https://api-{self.auth.region}.stack.tryrelevance.com/latest/studios"
-        response = requests.post(
-            f"{url}/bulk_update",
-            json={"updates": [self._json()]},
-            headers=self.auth.headers,
-        )
-        res = handle_response(response)
-        print("Studio deployed successfully to id ", self.id)
-        if self.random_id:
-            print(
-                "Your studio id is randomly generated, to ensure you are updating the same chain you should specify the id on rai.create(id=id) ",
-            )
-        print("\n=============Low Code Notebook================")
-        print(
-            f"You can share/visualize your chain as an app in our low code notebook here: https://chain.relevanceai.com/notebook/{self.auth.region}/{self.auth.project}/{self.id}/app"
-        )
-        print("\n=============with Requests================")
-        print("Here is an example of how to run the chain with API: ")
-        print(
-            f"""
-import requests
-requests.post(https://api-{self.auth.region}.stack.tryrelevance.com/latest/studios/{self.id}/trigger_limited", json={{
-    "project": "{self.auth.project}",
-    "params": {{
-        YOUR PARAMS HERE
-    }}
-}})
-            """
-        )
-        print("\n=============with Python SDK================")
-        print("Here is an example of how to run the chain with Python: ")
-        print(
-            f"""
-import relevanceai as rai
-chain = rai.load("{self.id}")
-chain.run({{YOUR PARAMS HERE}})
-            """
-        )
-        return self.id
-
-    def to_json(self, filepath, return_json=False):
-        if return_json:
-            with open(filepath, "w") as f:
-                json.dump(self._json(), f)
-                print("Chain saved to ", filepath)
-        else:
-            return self._json()
-
-    def reset(self):
-        self.steps = []
+import json
+import requests
+from relevanceai._request import handle_response
+from relevanceai import config
+from relevanceai.auth import Auth
+from relevanceai.params import Parameters
+
+
+def create(name, description="", parameters={}, id=None, auth=None):
+    chain = Chain(
+        name=name, description=description, parameters=parameters, id=id, auth=auth
+    )
+    return chain
+
+
+def load(id, auth=None):
+    if auth is None:
+        auth = config.auth
+    response = requests.get(
+        f"https://api-{auth.region}.stack.tryrelevance.com/latest/studios/{auth.project}/{id}",
+        json={
+            "filters": [
+                {
+                    "field": "studio_id",
+                    "condition": "==",
+                    "condition_value": id,
+                    "filter_type": "exact_match",
+                },
+                {
+                    "field": "project",
+                    "condition": "==",
+                    "condition_value": auth.project,
+                    "filter_type": "exact_match",
+                },
+            ]
+        },
+    )
+    res = handle_response(response)
+    chain = Chain(name="", description="", parameters={}, id=id, auth=auth)
+    return chain
+
+
+def load_from_json(filepath_or_json):
+    if isinstance(filepath_or_json, str):
+        with open(filepath_or_json, "r") as f:
+            chain_json = json.load(f)
+    else:
+        chain_json = filepath_or_json
+    chain = Chain(
+        name=chain_json["title"],
+        description=chain_json["description"],
+        parameters=chain_json["params_schema"]["properties"],
+        id=chain_json["studio_id"],
+    )
+    chain.add(chain_json["transformations"]["steps"])
+    return chain
+
+
+class Chain:
+    def __init__(
+        self,
+        name: str,
+        description: str = "",
+        parameters={},
+        id: str = None,
+        auth: Auth = None,
+    ):
+        self.name = name
+        self.description = description
+        self._parameters = parameters
+        self.steps = []
+        # generate random id if none
+        self.random_id = False
+        if id is None:
+            import uuid
+
+            id = str(uuid.uuid4())
+            self.random_id = True
+        self.id = id
+        self.auth: Auth = config.auth if auth is None else auth
+
+    @property
+    def parameters(self):
+        return Parameters(self._parameters)
+
+    params = parameters
+
+    def add(self, steps):
+        if isinstance(steps, list):
+            self.steps.extend(steps)
+        else:
+            self.steps.append(steps)
+
+    def _transform_steps(self, steps):
+        chain_steps = [step.steps[0] for step in steps]
+        unique_ids = []
+        for step in chain_steps:
+            if step["name"] in unique_ids:
+                raise ValueError(
+                    f"Duplicate step name {step['name']}, please rename the step name with Step(step_name=step_name)."
+                )
+            unique_ids.append(step["name"])
+        return chain_steps
+
+    def _trigger_json(
+        self, values: dict = {}, return_state: bool = True, public: bool = False
+    ):
+        data = {
+            "return_state": return_state,
+            "studio_override": {
+                "public": public,
+                "transformations": {"steps": self._transform_steps(self.steps)},
+                "params_schema": {"properties": self.parameters.to_json()},
+            },
+            "params": values,
+        }
+        data["studio_id"] = self.id
+        data["studio_override"]["studio_id"] = self.id
+        return data
+
+    def run(self, parameters={}, full_response: bool = False):
+        url = f"https://api-{self.auth.region}.stack.tryrelevance.com/latest/studios/{self.auth.project}"
+        response = requests.post(
+            f"{url}/trigger",
+            json=self._trigger_json(parameters),
+            headers=self.auth.headers,
+        )
+        res = handle_response(response)
+        if isinstance(res, dict):
+            if ("errors" in res and res["errors"]) or full_response:
+                return res
+            elif "output" in res:
+                return res["output"]
+        return res
+
+    def _json(self):
+        data = {
+            "title": self.name,
+            "description": self.description,
+            "version": "latest",
+            "project": self.auth.project,
+            "public": False,
+            "params_schema": {"properties": self.parameters.to_json()},
+            "transformations": {"steps": self._transform_steps(self.steps)},
+        }
+        data["studio_id"] = self.id
+        return data
+
+    def deploy(self):
+        url = f"https://api-{self.auth.region}.stack.tryrelevance.com/latest/studios"
+        response = requests.post(
+            f"{url}/bulk_update",
+            json={"updates": [self._json()]},
+            headers=self.auth.headers,
+        )
+        res = handle_response(response)
+        print("Studio deployed successfully to id ", self.id)
+        if self.random_id:
+            print(
+                "Your studio id is randomly generated, to ensure you are updating the same chain you should specify the id on rai.create(id=id) ",
+            )
+        print("\n=============Low Code Notebook================")
+        print(
+            f"You can share/visualize your chain as an app in our low code notebook here: https://chain.relevanceai.com/notebook/{self.auth.region}/{self.auth.project}/{self.id}/app"
+        )
+        print("\n=============with Requests================")
+        print("Here is an example of how to run the chain with API: ")
+        print(
+            f"""
+import requests
+requests.post(https://api-{self.auth.region}.stack.tryrelevance.com/latest/studios/{self.id}/trigger_limited", json={{
+    "project": "{self.auth.project}",
+    "params": {{
+        YOUR PARAMS HERE
+    }}
+}})
+            """
+        )
+        print("\n=============with Python SDK================")
+        print("Here is an example of how to run the chain with Python: ")
+        print(
+            f"""
+import relevanceai as rai
+chain = rai.load("{self.id}")
+chain.run({{YOUR PARAMS HERE}})
+            """
+        )
+        return self.id
+
+    def to_json(self, filepath, return_json=False):
+        if return_json:
+            with open(filepath, "w") as f:
+                json.dump(self._json(), f)
+                print("Chain saved to ", filepath)
+        else:
+            return self._json()
+
+    def reset(self):
+        self.steps = []
```

### Comparing `relevanceai-5.0.4/relevanceai/connect/fastapi/chains.py` & `relevanceai-5.0.5/relevanceai/connect/fastapi/chains.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-import os
-import json
-import atexit
-import requests
-from typing import List
-from fastapi.routing import APIRoute
-from relevanceai.auth import config
-
-
-def routes_to_chains(api_routes, url, id_suffix=""):
-    chains_list = []
-    id_list = []
-    for route in api_routes:
-        if isinstance(route, APIRoute):
-            id_list.append(route.unique_id + id_suffix)
-            input_schema = {}
-            request_body = ""
-            if route.body_field:
-                input_schema = json.loads(route.body_field.type_.schema_json())
-                for k, v in input_schema["properties"].items():
-                    if v["type"] == "string":
-                        request_body += f'"{k}" : "{{{{ params.{k} }}}}",'
-                    else:
-                        request_body += f'"{k}" : {{{{ params.{k} }}}},'
-                request_body = "{ " + request_body[:-1] + " }"
-
-            output_schema = {}
-            if route.response_field:
-                output_raw_schema = json.loads(route.response_field.type_.schema_json())
-                for k, v in output_raw_schema["properties"].items():
-                    output_schema[
-                        k
-                    ] = f"{{{{ steps.api_call.output.response_body.{k} }}}}"
-
-            if url.endswith("/"):
-                full_path = url[:-1] + route.path
-            else:
-                full_path = url + route.path
-
-            chains_list.append(
-                {
-                    "public": False,
-                    "studio_id": route.unique_id + id_suffix,
-                    "params_schema": input_schema,
-                    "publicly_triggerable": False,
-                    "project": config.auth.project,
-                    "title": route.summary if route.summary else route.name,
-                    "description": route.description,
-                    "tags": {"type": "transformation"},
-                    "transformations": {
-                        "steps": [
-                            {
-                                "name": "api_call",
-                                "transformation": "api_call",
-                                "params": {
-                                    "url": full_path,
-                                    "method": "POST",
-                                    "headers": {
-                                        "Content-Type": "application/json",
-                                        # **headers
-                                    },
-                                    "body": request_body,
-                                    "response_type": "json",
-                                },
-                                "output": {
-                                    "response_body": "{{response_body}}",
-                                    "status": "{{status}}",
-                                },
-                            }
-                        ],
-                        "output": output_schema,
-                    },
-                }
-            )
-    return chains_list, id_list
-
-
-def upload_chains(chains):
-    url = f"https://api-{config.auth.region}.stack.tryrelevance.com"
-    results = requests.post(
-        f"{url}/latest/studios/bulk_update",
-        headers=config.auth.headers,
-        json={"updates": chains},
-    )
-    print("Uploaded chains: ", results.json())
-    print("Trace-id ", results.headers.get("x-trace-id"))
-
-
-def cleanup_chains(chain_id_list):
-    results = requests.post(
-        f"https://api-{config.auth.region}.stack.tryrelevance.com/latest/studios/bulk_delete",
-        headers=config.auth.headers,
-        json={"ids": chain_id_list},
-    )
-    print("Successfully deleted chains from cloud: ", results.json())
-    print("Trace-id ", results.headers.get("x-trace-id"))
-
-
-def connect_chains(api_routes, url, id_suffix="", cleanup=True, export_json=False):
-    chains, chain_id_list = routes_to_chains(api_routes, url, id_suffix=id_suffix)
-    if export_json:
-        import json
-
-        with open("chain_export.json", "w") as outfile:
-            json.dump({"export": chains}, outfile)
-    else:
-        upload_chains(chains)
-    if cleanup:
-        atexit.register(cleanup_chains, chain_id_list)
-    return chain_id_list
+import os
+import json
+import atexit
+import requests
+from typing import List
+from fastapi.routing import APIRoute
+from relevanceai.auth import config
+
+
+def routes_to_chains(api_routes, url, id_suffix=""):
+    chains_list = []
+    id_list = []
+    for route in api_routes:
+        if isinstance(route, APIRoute):
+            id_list.append(route.unique_id + id_suffix)
+            input_schema = {}
+            request_body = {}
+            if route.body_field:
+                input_schema = json.loads(route.body_field.type_.schema_json())
+                for k, v in input_schema["properties"].items():
+                    if v["type"] == "string":
+                        request_body[k] = f"{{{{ params.{k} }}}}"
+                    else:
+                        request_body[k] = f"{{{{ params.{k} }}}}"
+                # request_body = "{ " + request_body[:-1] + " }"
+
+            output_schema = {}
+            if route.response_field:
+                output_raw_schema = json.loads(route.response_field.type_.schema_json())
+                for k, v in output_raw_schema["properties"].items():
+                    output_schema[
+                        k
+                    ] = f"{{{{ steps.api_call.output.response_body.{k} }}}}"
+
+            if url.endswith("/"):
+                full_path = url[:-1] + route.path
+            else:
+                full_path = url + route.path
+
+            chains_list.append(
+                {
+                    "public": False,
+                    "studio_id": route.unique_id + id_suffix,
+                    "params_schema": input_schema,
+                    "publicly_triggerable": False,
+                    "project": config.auth.project,
+                    "title": route.summary if route.summary else route.name,
+                    "description": route.description,
+                    "tags": {"type": "transformation"},
+                    "transformations": {
+                        "steps": [
+                            {
+                                "name": "api_call",
+                                "transformation": "api_call",
+                                "params": {
+                                    "url": full_path,
+                                    "method": "POST",
+                                    "headers": {
+                                        "Content-Type": "application/json",
+                                        # **headers
+                                    },
+                                    "body": request_body,
+                                    "response_type": "json",
+                                },
+                                "output": {
+                                    "response_body": "{{response_body}}",
+                                    "status": "{{status}}",
+                                },
+                            }
+                        ],
+                        "output": output_schema,
+                    },
+                }
+            )
+    return chains_list, id_list
+
+
+def upload_chains(chains):
+    url = f"https://api-{config.auth.region}.stack.tryrelevance.com"
+    results = requests.post(
+        f"{url}/latest/studios/bulk_update",
+        headers=config.auth.headers,
+        json={"updates": chains},
+    )
+    print("Uploaded chains: ", results.json())
+    print("Trace-id ", results.headers.get("x-trace-id"))
+
+
+def cleanup_chains(chain_id_list):
+    results = requests.post(
+        f"https://api-{config.auth.region}.stack.tryrelevance.com/latest/studios/bulk_delete",
+        headers=config.auth.headers,
+        json={"ids": chain_id_list},
+    )
+    print("Successfully deleted chains from cloud: ", results.json())
+    print("Trace-id ", results.headers.get("x-trace-id"))
+
+
+def connect_chains(api_routes, url, id_suffix="", cleanup=True, export_json=False):
+    chains, chain_id_list = routes_to_chains(api_routes, url, id_suffix=id_suffix)
+    if export_json:
+        import json
+
+        with open("chain_export.json", "w") as outfile:
+            json.dump({"export": chains}, outfile)
+    else:
+        upload_chains(chains)
+    if cleanup:
+        atexit.register(cleanup_chains, chain_id_list)
+    return chain_id_list
```

### Comparing `relevanceai-5.0.4/relevanceai/env.py` & `relevanceai-5.0.5/relevanceai/env.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import requests
-from relevanceai._request import handle_response
-from relevanceai import config
-
-def set_key(key:str, value:str):
-    url = f"https://api-{config.auth.region}.stack.tryrelevance.com/latest"
-    response = requests.post(
-        f"{url}/projects/keys/set",
-        headers=config.auth.headers,
-        json={
-            "key": key,
-            "value": value,
-        }
-    )
-    res = handle_response(response)
-    return res
-
-def list_keys():
-    url = f"https://api-{config.auth.region}.stack.tryrelevance.com/latest"
-    response = requests.get(
-        f"{url}/projects/keys/list",
-        headers=config.auth.headers,
-    )
-    res = handle_response(response)
-    return res
-
-def delete_key(key:str):
-    url = f"https://api-{config.auth.region}.stack.tryrelevance.com/latest"
-    response = requests.post(
-        f"{url}/projects/keys/delete",
-        headers=config.auth.headers,
-        json={
-            "key": key,
-        }
-    )
-    res = handle_response(response)
+import requests
+from relevanceai._request import handle_response
+from relevanceai import config
+
+def set_key(key:str, value:str):
+    url = f"https://api-{config.auth.region}.stack.tryrelevance.com/latest"
+    response = requests.post(
+        f"{url}/projects/keys/set",
+        headers=config.auth.headers,
+        json={
+            "key": key,
+            "value": value,
+        }
+    )
+    res = handle_response(response)
+    return res
+
+def list_keys():
+    url = f"https://api-{config.auth.region}.stack.tryrelevance.com/latest"
+    response = requests.get(
+        f"{url}/projects/keys/list",
+        headers=config.auth.headers,
+    )
+    res = handle_response(response)
+    return res
+
+def delete_key(key:str):
+    url = f"https://api-{config.auth.region}.stack.tryrelevance.com/latest"
+    response = requests.post(
+        f"{url}/projects/keys/delete",
+        headers=config.auth.headers,
+        json={
+            "key": key,
+        }
+    )
+    res = handle_response(response)
     return res
```

### Comparing `relevanceai-5.0.4/relevanceai/params.py` & `relevanceai-5.0.5/relevanceai/params.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,182 +1,182 @@
-from typing import Any
-
-class ParamBase:
-    def __init__(self, name):
-        self.name = name
-        self.json = {name: {}}
-    
-    def to_json(self):
-        return self.json
-
-class Parameters:
-    def __init__(self, parameters):
-        self.parameters = parameters
-
-    def _check_param(self, param):
-        if isinstance(param, dict):
-            return param
-        elif isinstance(param, ParamBase):
-            return param.json
-        else:
-            raise ValueError(
-                "Parameters must be a ParamBase instances or a dictionary"
-            )
-
-    def to_json(self):
-        if isinstance(self.parameters, list):
-            dict_params = {}
-            for p in self.parameters:
-                dict_params.update(self._check_param(p))
-            return dict_params
-        elif isinstance(self.parameters, dict):
-            return self.parameters
-        else:
-            return self.parameters.json
-
-    def _format_name(self, name:str):
-        return "{{" + name + "}}"
-
-
-class StringParam(ParamBase):
-    def __init__(self, name, long: bool = False, title="Text Input", description=""):
-        super().__init__(name)
-        self.title = title
-        self.description = description
-        self.long = long
-        self.json = {
-            name: {
-                "title": title,
-                "description": description,
-                "type": "string",
-            }
-        }
-        if self.long:
-            self.json[name]["metadata"] = {"content_type": "long_text"}
-
-
-class NumberParam(ParamBase):
-    def __init__(
-        self,
-        name,
-        max: int = None,
-        min: int = None,
-        title="Number Input",
-        description="",
-    ):
-        self.name = name
-        self.title = title
-        self.description = description
-        self.max = max
-        self.min = min
-        self.json = {
-            name: {
-                "title": title,
-                "description": description,
-                "type": "number",
-            }
-        }
-        if self.max:
-            self.json[name]["max"] = max
-        if self.min:
-            self.json[name]["min"] = min
-
-
-class OptionsParam:
-    def __init__(
-        self,
-        name,
-        options,
-        title="Options",
-        description="",
-    ):
-        self.name = name
-        self.title = title
-        self.description = description
-        self.options = options
-        self.json = {
-            name: {
-                "title": title,
-                "description": description,
-                "type": "string",
-                "enum": options,
-            }
-        }
-
-
-class StringListParam(ParamBase):
-    def __init__(
-        self,
-        name,
-        title="Text List Input",
-        description="",
-    ):
-        self.name = name
-        self.title = title
-        self.description = description
-        self.json = {
-            name: {
-                "title": title,
-                "description": description,
-                "type": "array",
-                "items": {"type": "string"},
-            }
-        }
-
-
-class JsonParam:
-    def __init__(
-        self,
-        name,
-        title="JSON Input",
-        description="",
-    ):
-        self.name = name
-        self.title = title
-        self.description = description
-        self.json = {
-            name: {
-                "title": title,
-                "description": description,
-                "type": "object",
-            }
-        }
-
-
-class JsonListParam(ParamBase):
-    def __init__(
-        self,
-        name,
-        title="JSON List Input",
-        description="",
-    ):
-        self.name = name
-        self.title = title
-        self.description = description
-        self.json = {
-            name: {
-                "title": title,
-                "description": description,
-                "type": "array",
-                "items": {"type": "object"},
-            }
-        }
-
-
-class FileParam(ParamBase):
-    def __init__(
-        self,
-        name,
-        title="File Input",
-        description="",
-    ):
-        self.name = name
-        self.title = title
-        self.description = description
-        self.json = {
-            name: {
-                "title": title,
-                "description": description,
-                "type": "string",
-                "metadata": {"content_type": "file", "accepted_file_types": []},
-            }
-        }
+from typing import Any
+
+class ParamBase:
+    def __init__(self, name):
+        self.name = name
+        self.json = {name: {}}
+    
+    def to_json(self):
+        return self.json
+
+class Parameters:
+    def __init__(self, parameters):
+        self.parameters = parameters
+
+    def _check_param(self, param):
+        if isinstance(param, dict):
+            return param
+        elif isinstance(param, ParamBase):
+            return param.json
+        else:
+            raise ValueError(
+                "Parameters must be a ParamBase instances or a dictionary"
+            )
+
+    def to_json(self):
+        if isinstance(self.parameters, list):
+            dict_params = {}
+            for p in self.parameters:
+                dict_params.update(self._check_param(p))
+            return dict_params
+        elif isinstance(self.parameters, dict):
+            return self.parameters
+        else:
+            return self.parameters.json
+
+    def _format_name(self, name:str):
+        return "{{" + name + "}}"
+
+
+class StringParam(ParamBase):
+    def __init__(self, name, long: bool = False, title="Text Input", description=""):
+        super().__init__(name)
+        self.title = title
+        self.description = description
+        self.long = long
+        self.json = {
+            name: {
+                "title": title,
+                "description": description,
+                "type": "string",
+            }
+        }
+        if self.long:
+            self.json[name]["metadata"] = {"content_type": "long_text"}
+
+
+class NumberParam(ParamBase):
+    def __init__(
+        self,
+        name,
+        max: int = None,
+        min: int = None,
+        title="Number Input",
+        description="",
+    ):
+        self.name = name
+        self.title = title
+        self.description = description
+        self.max = max
+        self.min = min
+        self.json = {
+            name: {
+                "title": title,
+                "description": description,
+                "type": "number",
+            }
+        }
+        if self.max:
+            self.json[name]["max"] = max
+        if self.min:
+            self.json[name]["min"] = min
+
+
+class OptionsParam:
+    def __init__(
+        self,
+        name,
+        options,
+        title="Options",
+        description="",
+    ):
+        self.name = name
+        self.title = title
+        self.description = description
+        self.options = options
+        self.json = {
+            name: {
+                "title": title,
+                "description": description,
+                "type": "string",
+                "enum": options,
+            }
+        }
+
+
+class StringListParam(ParamBase):
+    def __init__(
+        self,
+        name,
+        title="Text List Input",
+        description="",
+    ):
+        self.name = name
+        self.title = title
+        self.description = description
+        self.json = {
+            name: {
+                "title": title,
+                "description": description,
+                "type": "array",
+                "items": {"type": "string"},
+            }
+        }
+
+
+class JsonParam:
+    def __init__(
+        self,
+        name,
+        title="JSON Input",
+        description="",
+    ):
+        self.name = name
+        self.title = title
+        self.description = description
+        self.json = {
+            name: {
+                "title": title,
+                "description": description,
+                "type": "object",
+            }
+        }
+
+
+class JsonListParam(ParamBase):
+    def __init__(
+        self,
+        name,
+        title="JSON List Input",
+        description="",
+    ):
+        self.name = name
+        self.title = title
+        self.description = description
+        self.json = {
+            name: {
+                "title": title,
+                "description": description,
+                "type": "array",
+                "items": {"type": "object"},
+            }
+        }
+
+
+class FileParam(ParamBase):
+    def __init__(
+        self,
+        name,
+        title="File Input",
+        description="",
+    ):
+        self.name = name
+        self.title = title
+        self.description = description
+        self.json = {
+            name: {
+                "title": title,
+                "description": description,
+                "type": "string",
+                "metadata": {"content_type": "file", "accepted_file_types": []},
+            }
+        }
```

### Comparing `relevanceai-5.0.4/relevanceai/steps/__init__.py` & `relevanceai-5.0.5/relevanceai/steps/__init__.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from relevanceai.steps.prompt_completion import PromptCompletion
-
-# from relevanceai.steps.redis_insert import RedisInsert
-from relevanceai.steps.vector_search import VectorSimilaritySearch
-from relevanceai.steps.redis_vector_search import RedisSearch
-from relevanceai.steps.vectorize_and_search import VectorizeAndSearchArray
-from relevanceai.steps.execute_javascript import ExecuteJavascriptCode
-from relevanceai.steps.generate_vector_embedding import GenerateVectorEmbedding
-from relevanceai.steps.run_chain import RunChain
-from relevanceai.steps.run_step import RunStep, list_all_steps
+from relevanceai.steps.prompt_completion import PromptCompletion
+
+# from relevanceai.steps.redis_insert import RedisInsert
+from relevanceai.steps.vector_search import VectorSimilaritySearch
+from relevanceai.steps.redis_vector_search import RedisSearch
+from relevanceai.steps.vectorize_and_search import VectorizeAndSearchArray
+from relevanceai.steps.execute_javascript import ExecuteJavascriptCode
+from relevanceai.steps.generate_vector_embedding import GenerateVectorEmbedding
+from relevanceai.steps.run_chain import RunChain
+from relevanceai.steps.run_step import RunStep, list_all_steps
```

### Comparing `relevanceai-5.0.4/relevanceai/steps/_base.py` & `relevanceai-5.0.5/relevanceai/steps/_base.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-import requests
-from relevanceai import config
-from relevanceai.auth import Auth
-from relevanceai._request import handle_response
-from relevanceai.params import Parameters, ParamBase
-
-
-class StepBase:
-    def __init__(
-        self, name="step", description="a step", parameters={}, id="new", auth=None
-    ):
-        self.name = name
-        self.description = description
-        if isinstance(parameters, Parameters):
-            self.parameters = parameters.to_json()
-        elif isinstance(parameters, ParamBase):
-            self.parameters = parameters.to_json()
-        else:
-            self.parameters = parameters
-        self.id = id
-        self.auth: Auth = config.auth if auth is None else auth
-
-    def _trigger_json(
-        self, values: dict = {}, return_state: bool = True, public: bool = False
-    ):
-        return {
-            "studio_id": self.id,
-            "return_state": return_state,
-            "params": values,
-            "state_override": {
-                "steps": {},
-                "params": values,
-            },
-            "studio_override": {
-                "studio_id": self.id,
-                "public": public,
-                "transformations": {"steps": self.steps},
-                "params_schema": {"properties": self.parameters},
-            },
-        }
-
-    def run(self, parameters={}, full_response: bool = False):
-        url = f"https://api-{self.auth.region}.stack.tryrelevance.com/latest/studios/{self.auth.project}"
-        response = requests.post(
-            f"{url}/trigger",
-            json=self._trigger_json(parameters),
-            headers=self.auth.headers,
-        )
-        res = handle_response(response)
-        if isinstance(res, dict):
-            if ("errors" in res and res["errors"]) or full_response:
-                return res
-            elif "output" in res:
-                return res["output"]
-        return res
-
-    def _json(self):
-        return {
-            "title": self.name,
-            "description": self.description,
-            "version": "latest",
-            "project": self.auth.project,
-            "studio_id": self.id,
-            "public": False,
-            "params_schema": {"properties": self.parameters},
-            "transformations": {"steps": self.steps},
-        }
-
-    def deploy(self):
-        url = f"https://api-{self.auth.region}.stack.tryrelevance.com/latest/studios"
-        response = requests.post(
-            f"{url}/bulk_update",
-            json={"updates": [self._json()]},
-            headers=self.auth.headers,
-        )
-        return handle_response(response)
+import requests
+from relevanceai import config
+from relevanceai.auth import Auth
+from relevanceai._request import handle_response
+from relevanceai.params import Parameters, ParamBase
+
+
+class StepBase:
+    def __init__(
+        self, name="step", description="a step", parameters={}, id="new", auth=None
+    ):
+        self.name = name
+        self.description = description
+        if isinstance(parameters, Parameters):
+            self.parameters = parameters.to_json()
+        elif isinstance(parameters, ParamBase):
+            self.parameters = parameters.to_json()
+        else:
+            self.parameters = parameters
+        self.id = id
+        self.auth: Auth = config.auth if auth is None else auth
+
+    def _trigger_json(
+        self, values: dict = {}, return_state: bool = True, public: bool = False
+    ):
+        return {
+            "studio_id": self.id,
+            "return_state": return_state,
+            "params": values,
+            "state_override": {
+                "steps": {},
+                "params": values,
+            },
+            "studio_override": {
+                "studio_id": self.id,
+                "public": public,
+                "transformations": {"steps": self.steps},
+                "params_schema": {"properties": self.parameters},
+            },
+        }
+
+    def run(self, parameters={}, full_response: bool = False):
+        url = f"https://api-{self.auth.region}.stack.tryrelevance.com/latest/studios/{self.auth.project}"
+        response = requests.post(
+            f"{url}/trigger",
+            json=self._trigger_json(parameters),
+            headers=self.auth.headers,
+        )
+        res = handle_response(response)
+        if isinstance(res, dict):
+            if ("errors" in res and res["errors"]) or full_response:
+                return res
+            elif "output" in res:
+                return res["output"]
+        return res
+
+    def _json(self):
+        return {
+            "title": self.name,
+            "description": self.description,
+            "version": "latest",
+            "project": self.auth.project,
+            "studio_id": self.id,
+            "public": False,
+            "params_schema": {"properties": self.parameters},
+            "transformations": {"steps": self.steps},
+        }
+
+    def deploy(self):
+        url = f"https://api-{self.auth.region}.stack.tryrelevance.com/latest/studios"
+        response = requests.post(
+            f"{url}/bulk_update",
+            json={"updates": [self._json()]},
+            headers=self.auth.headers,
+        )
+        return handle_response(response)
```

### Comparing `relevanceai-5.0.4/relevanceai/steps/generate_vector_embedding.py` & `relevanceai-5.0.5/relevanceai/steps/generate_vector_embedding.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-from relevanceai.steps._base import StepBase
-
-class GenerateVectorEmbedding(StepBase):
-    """Generate vector embedding
-    Generate a vector embedding from a given input with a choice of models.
-    Args:
-        input (str): The input to generate a vector embedding with.
-        model (str): The model name to use.
-    Returns:
-        vector (list): The vector embedding.
-    """
-    def __init__(
-        self,
-        input: str,
-        model: str,
-        step_name: str = "generate_vector_embedding",
-        *args,
-        **kwargs
-    ) -> None:
-        self.input = input
-        self.model = model
-        self.step_name = step_name
-        self._outputs = ["vector"]
-        self.outputs = [f"steps.{self.step_name}.output.{a}" for a in self._outputs]
-        super().__init__(*args, **kwargs)
-
-    @property
-    def steps(self):
-        return [
-            {
-                "transformation": "generate_vector_embedding",
-                "name": self.step_name,
-                "foreach": "",
-                "output": {output: f"{{{{ {output} }}}}" for output in self._outputs},
-                "params": {
-                    "input": self.input,
-                    "model": self.model
-                }
-            }
+from relevanceai.steps._base import StepBase
+
+class GenerateVectorEmbedding(StepBase):
+    """Generate vector embedding
+    Generate a vector embedding from a given input with a choice of models.
+    Args:
+        input (str): The input to generate a vector embedding with.
+        model (str): The model name to use.
+    Returns:
+        vector (list): The vector embedding.
+    """
+    def __init__(
+        self,
+        input: str,
+        model: str,
+        step_name: str = "generate_vector_embedding",
+        *args,
+        **kwargs
+    ) -> None:
+        self.input = input
+        self.model = model
+        self.step_name = step_name
+        self._outputs = ["vector"]
+        self.outputs = [f"steps.{self.step_name}.output.{a}" for a in self._outputs]
+        super().__init__(*args, **kwargs)
+
+    @property
+    def steps(self):
+        return [
+            {
+                "transformation": "generate_vector_embedding",
+                "name": self.step_name,
+                "foreach": "",
+                "output": {output: f"{{{{ {output} }}}}" for output in self._outputs},
+                "params": {
+                    "input": self.input,
+                    "model": self.model
+                }
+            }
         ]
```

### Comparing `relevanceai-5.0.4/relevanceai/steps/redis_vector_search.py` & `relevanceai-5.0.5/relevanceai/steps/vector_search.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,61 @@
-from relevanceai.steps._base import StepBase
-
-class RedisSearch(StepBase):
-    """Vector search on Redis
-    Retrieve data from Redis based on semantic similarity.
-    Args:
-        index (str): The name of the index to search.
-        query (str): The search query.
-        vector_field (str): The name of the field that contains the vector.
-        model (str): The model name to use.
-        page_size (int): The number of results to return.
-    Returns:
-        results (list): The search results.
-    """
-    def __init__(
-        self,
-        index: str,
-        query: str,
-        vector_field: str,
-        model: str,
-        page_size: int = 5,
-        step_name: str = "redis_search",
-        *args,
-        **kwargs
-    ) -> None:
-        self.index = index
-        self.query = query
-        self.vector_field = vector_field
-        self.model = model
-        self.page_size = page_size
-        self.step_name = step_name
-        self._outputs = ["results"]
-        self.outputs = [f"steps.{self.step_name}.output.{a}" for a in self._outputs]
-        super().__init__(*args, **kwargs)
-
-    @property
-    def steps(self):
-        return [
-            {
-                "transformation": "redis_search",
-                "name": self.step_name,
-                "foreach": "",
-                "output": {output: f"{{{{ {output} }}}}" for output in self._outputs},
-                "params": {
-                    "index": self.index,
-                    "query": self.query,
-                    "vector_field": self.vector_field,
-                    "model": self.model,
-                    "page_size": self.page_size
-                }
-            }
-        ]
+from relevanceai.steps._base import StepBase
+
+
+class VectorSimilaritySearch(StepBase):
+    """Vector similarity search on Relevance dataset
+    Search your dataset based on semantic similarity.
+    Args:
+        dataset_id (str): The ID of the dataset to search.
+        query (str): The query to search for.
+        vector_field (str): The name of the field that contains the vector.
+        model (str): The model name to use.
+        content_field ((Optional) str):
+        page_size ((Optional) int): The number of results to return.
+    Returns:
+        results (list): {'type': 'array', 'items': {'type': ['string', 'object']}}
+    """
+
+    def __init__(
+        self,
+        dataset_id: str,
+        query: str,
+        vector_field: str,
+        model: str,
+        content_field: str = None,
+        page_size: int = 5,
+        step_name: str = "vector_similarity_search",
+        *args,
+        **kwargs,
+    ) -> None:
+        self.dataset_id = dataset_id
+        self.query = query
+        self.vector_field = vector_field
+        self.model = model
+        self.content_field = content_field
+        self.page_size = page_size
+        self.step_name = step_name
+        self._outputs = ["results"]
+        self.outputs = [f"steps.{self.step_name}.output.{a}" for a in self._outputs]
+        super().__init__(*args, **kwargs)
+
+    @property
+    def steps(self):
+        step_params = {
+            "dataset_id": self.dataset_id,
+            "query": self.query,
+            "vector_field": self.vector_field,
+            "model": self.model,
+        }
+        if self.content_field is not None:
+            step_params["content_field"] = self.content_field
+        if self.page_size is not None:
+            step_params["page_size"] = self.page_size
+        return [
+            {
+                "transformation": "search",
+                "name": self.step_name,
+                "foreach": "",
+                "output": {output: f"{{{{ {output} }}}}" for output in self._outputs},
+                "params": step_params,
+            }
+        ]
```

### Comparing `relevanceai-5.0.4/relevanceai/steps/vector_search.py` & `relevanceai-5.0.5/relevanceai/steps/redis_vector_search.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,52 @@
-from relevanceai.steps._base import StepBase
-
-
-class VectorSimilaritySearch(StepBase):
-    """Vector similarity search on Relevance dataset
-    Search your dataset based on semantic similarity.
-    Args:
-        dataset_id (str): The ID of the dataset to search.
-        query (str): The query to search for.
-        vector_field (str): The name of the field that contains the vector.
-        model (str): The model name to use.
-        content_field ((Optional) str):
-        page_size ((Optional) int): The number of results to return.
-    Returns:
-        results (list): {'type': 'array', 'items': {'type': ['string', 'object']}}
-    """
-
-    def __init__(
-        self,
-        dataset_id: str,
-        query: str,
-        vector_field: str,
-        model: str,
-        content_field: str = None,
-        page_size: int = 5,
-        step_name: str = "vector_similarity_search",
-        *args,
-        **kwargs,
-    ) -> None:
-        self.dataset_id = dataset_id
-        self.query = query
-        self.vector_field = vector_field
-        self.model = model
-        self.content_field = content_field
-        self.page_size = page_size
-        self.step_name = step_name
-        self._outputs = ["results"]
-        self.outputs = [f"steps.{self.step_name}.output.{a}" for a in self._outputs]
-        super().__init__(*args, **kwargs)
-
-    @property
-    def steps(self):
-        step_params = {
-            "dataset_id": self.dataset_id,
-            "query": self.query,
-            "vector_field": self.vector_field,
-            "model": self.model,
-        }
-        if self.content_field is not None:
-            step_params["content_field"] = self.content_field
-        if self.page_size is not None:
-            step_params["page_size"] = self.page_size
-        return [
-            {
-                "transformation": "search",
-                "name": self.step_name,
-                "foreach": "",
-                "output": {output: f"{{{{ {output} }}}}" for output in self._outputs},
-                "params": step_params,
-            }
-        ]
+from relevanceai.steps._base import StepBase
+
+class RedisSearch(StepBase):
+    """Vector search on Redis
+    Retrieve data from Redis based on semantic similarity.
+    Args:
+        index (str): The name of the index to search.
+        query (str): The search query.
+        vector_field (str): The name of the field that contains the vector.
+        model (str): The model name to use.
+        page_size (int): The number of results to return.
+    Returns:
+        results (list): The search results.
+    """
+    def __init__(
+        self,
+        index: str,
+        query: str,
+        vector_field: str,
+        model: str,
+        page_size: int = 5,
+        step_name: str = "redis_search",
+        *args,
+        **kwargs
+    ) -> None:
+        self.index = index
+        self.query = query
+        self.vector_field = vector_field
+        self.model = model
+        self.page_size = page_size
+        self.step_name = step_name
+        self._outputs = ["results"]
+        self.outputs = [f"steps.{self.step_name}.output.{a}" for a in self._outputs]
+        super().__init__(*args, **kwargs)
+
+    @property
+    def steps(self):
+        return [
+            {
+                "transformation": "redis_search",
+                "name": self.step_name,
+                "foreach": "",
+                "output": {output: f"{{{{ {output} }}}}" for output in self._outputs},
+                "params": {
+                    "index": self.index,
+                    "query": self.query,
+                    "vector_field": self.vector_field,
+                    "model": self.model,
+                    "page_size": self.page_size
+                }
+            }
+        ]
```

### Comparing `relevanceai-5.0.4/relevanceai/steps/vectorize_and_search.py` & `relevanceai-5.0.5/relevanceai/steps/vectorize_and_search.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-from relevanceai.steps._base import StepBase
-
-class VectorizeAndSearchArray(StepBase):
-    """Vectorize and search array
-    Vectorise an array of strings and rank items by relevance to your search query.
-    Args:
-        array (list): The array of data to search. If it is an object, it will be stringified when searching.
-        query (str): The query to search for.
-        page_size (int): The number of results to return.
-        field (str): The field to search in if array includes objects.
-    Returns:
-        results (list): {'type': 'array', 'items': {}}
-    """
-    def __init__(
-        self,
-        array: list,
-        query: str,
-        page_size: int = 5,
-        field: str = None,
-        step_name: str = "vectorize_and_search_array",
-        *args,
-        **kwargs
-    ) -> None:
-        self.array = array
-        self.query = query
-        self.page_size = page_size
-        self.field = field
-        self.step_name = step_name
-        self._outputs = ["results"]
-        self.outputs = [f"steps.{self.step_name}.output.{a}" for a in self._outputs]
-        super().__init__(*args, **kwargs)
-
-    @property
-    def steps(self):
-        step_params = {
-            "array": self.array,
-            "query": self.query,
-            "page_size": self.page_size,
-        }
-        if self.field is not None:
-            step_params["field"] = self.field
-        return [
-            {
-                "transformation": "search_array",
-                "name": self.step_name,
-                "foreach": "",
-                "output": {output: f"{{{{ {output} }}}}" for output in self._outputs},
-                "params": step_params,
-            }
+from relevanceai.steps._base import StepBase
+
+class VectorizeAndSearchArray(StepBase):
+    """Vectorize and search array
+    Vectorise an array of strings and rank items by relevance to your search query.
+    Args:
+        array (list): The array of data to search. If it is an object, it will be stringified when searching.
+        query (str): The query to search for.
+        page_size (int): The number of results to return.
+        field (str): The field to search in if array includes objects.
+    Returns:
+        results (list): {'type': 'array', 'items': {}}
+    """
+    def __init__(
+        self,
+        array: list,
+        query: str,
+        page_size: int = 5,
+        field: str = None,
+        step_name: str = "vectorize_and_search_array",
+        *args,
+        **kwargs
+    ) -> None:
+        self.array = array
+        self.query = query
+        self.page_size = page_size
+        self.field = field
+        self.step_name = step_name
+        self._outputs = ["results"]
+        self.outputs = [f"steps.{self.step_name}.output.{a}" for a in self._outputs]
+        super().__init__(*args, **kwargs)
+
+    @property
+    def steps(self):
+        step_params = {
+            "array": self.array,
+            "query": self.query,
+            "page_size": self.page_size,
+        }
+        if self.field is not None:
+            step_params["field"] = self.field
+        return [
+            {
+                "transformation": "search_array",
+                "name": self.step_name,
+                "foreach": "",
+                "output": {output: f"{{{{ {output} }}}}" for output in self._outputs},
+                "params": step_params,
+            }
         ]
```

### Comparing `relevanceai-5.0.4/relevanceai.egg-info/PKG-INFO` & `relevanceai-5.0.5/relevanceai.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1
-Name: relevanceai
-Version: 5.0.4
-Home-page: https://relevanceai.com/
-Author: Relevance AI
-Author-email: jacky@relevanceai.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## Relevance AI - The platform for building and deploying AI chains and Agents
-[![License](https://img.shields.io/pypi/l/relevanceai)](https://img.shields.io/pypi/l/relevanceai)
-
-🔥 Use Relevance to unlock the value of LLMs:
-- ⚡ Quickly build and deploy chains in a few lines of code with fully managed deployment.
-- 🔎 Drilldown with filters and similarity search to explore and find insights.
-- 🔑 Vectors, storing and querying vectors with flexible vector similarity search, that can be combined with multiple vectors, aggregates and filters.
-- 🚀 Share chains as data apps with your team.
-
-[Sign up for a free account ->](https://chain.relevanceai.com)
-
-## 🧠 Documentation
-
-| Type      | Link |
-| ------------- | ----------- |
-| Python SDK | [Documentation](https://sdk.relevanceai.com/) |
-| Dashboard | [Documentation](https://chain.relevanceai.com/) |
-| Javascript SDK | [Documentation](https://documentation.relevanceai.com)        |
+Metadata-Version: 2.1
+Name: relevanceai
+Version: 5.0.5
+Home-page: https://relevanceai.com/
+Author: Relevance AI
+Author-email: jacky@relevanceai.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## Relevance AI - The platform for building and deploying AI chains and Agents
+[![License](https://img.shields.io/pypi/l/relevanceai)](https://img.shields.io/pypi/l/relevanceai)
+
+🔥 Use Relevance to unlock the value of LLMs:
+- ⚡ Quickly build and deploy chains in a few lines of code with fully managed deployment.
+- 🔎 Drilldown with filters and similarity search to explore and find insights.
+- 🔑 Vectors, storing and querying vectors with flexible vector similarity search, that can be combined with multiple vectors, aggregates and filters.
+- 🚀 Share chains as data apps with your team.
+
+[Sign up for a free account ->](https://chain.relevanceai.com)
+
+## 🧠 Documentation
+
+| Type      | Link |
+| ------------- | ----------- |
+| Python SDK | [Documentation](https://sdk.relevanceai.com/) |
+| Dashboard | [Documentation](https://chain.relevanceai.com/) |
+| Javascript SDK | [Documentation](https://documentation.relevanceai.com)        |
```

### Comparing `relevanceai-5.0.4/relevanceai.egg-info/SOURCES.txt` & `relevanceai-5.0.5/relevanceai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

