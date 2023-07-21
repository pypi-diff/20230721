# Comparing `tmp/honeyhive-0.1.8.tar.gz` & `tmp/honeyhive-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "honeyhive-0.1.8.tar", last modified: Fri Jul 21 15:43:30 2023, max compression
+gzip compressed data, was "honeyhive-0.1.9.tar", last modified: Fri Jul 21 16:15:29 2023, max compression
```

## Comparing `honeyhive-0.1.8.tar` & `honeyhive-0.1.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 15:43:30.921732 honeyhive-0.1.8/
--rw-r--r--   0 dhruvsingh   (501) staff       (20)      205 2022-12-13 17:06:38.000000 honeyhive-0.1.8/LICENSE
--rw-r--r--   0 dhruvsingh   (501) staff       (20)       40 2022-12-09 00:56:14.000000 honeyhive-0.1.8/MANIFEST.in
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     5542 2023-07-21 15:43:30.921522 honeyhive-0.1.8/PKG-INFO
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     4567 2023-03-05 07:17:37.000000 honeyhive-0.1.8/README.md
-drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 15:43:30.913181 honeyhive-0.1.8/honeyhive/
--rw-r--r--   0 dhruvsingh   (501) staff       (20)       19 2022-12-26 05:27:25.000000 honeyhive-0.1.8/honeyhive/__init__.py
-drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 15:43:30.914207 honeyhive-0.1.8/honeyhive/api/
--rw-r--r--   0 dhruvsingh   (501) staff       (20)        0 2022-12-13 17:07:45.000000 honeyhive-0.1.8/honeyhive/api/__init__.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     6681 2023-03-05 06:41:14.000000 honeyhive-0.1.8/honeyhive/api/client.py
-drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 15:43:30.917021 honeyhive-0.1.8/honeyhive/api/models/
--rw-r--r--   0 dhruvsingh   (501) staff       (20)        0 2022-12-13 17:08:09.000000 honeyhive-0.1.8/honeyhive/api/models/__init__.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     2299 2023-03-05 07:44:40.000000 honeyhive-0.1.8/honeyhive/api/models/datasets.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     1140 2022-12-18 14:25:26.000000 honeyhive-0.1.8/honeyhive/api/models/feedback.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     1899 2023-03-05 07:27:57.000000 honeyhive-0.1.8/honeyhive/api/models/fine_tuned_models.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     6087 2023-07-21 15:42:46.000000 honeyhive-0.1.8/honeyhive/api/models/generations.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     1244 2023-03-05 07:45:16.000000 honeyhive-0.1.8/honeyhive/api/models/metrics.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     4415 2023-01-10 00:49:31.000000 honeyhive-0.1.8/honeyhive/api/models/prompts.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     2638 2023-01-09 23:57:51.000000 honeyhive-0.1.8/honeyhive/api/models/tasks.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)      257 2022-12-14 20:38:37.000000 honeyhive-0.1.8/honeyhive/api/models/utils.py
-drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 15:43:30.920909 honeyhive-0.1.8/honeyhive/sdk/
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     2798 2023-03-12 05:30:52.000000 honeyhive-0.1.8/honeyhive/sdk/ChatCompletion.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     2926 2023-06-09 15:56:04.000000 honeyhive-0.1.8/honeyhive/sdk/Completion.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)        0 2022-12-31 04:55:35.000000 honeyhive-0.1.8/honeyhive/sdk/Untitled-3
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     1192 2023-03-28 00:19:47.000000 honeyhive-0.1.8/honeyhive/sdk/__init__.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     1799 2023-03-27 19:26:27.000000 honeyhive-0.1.8/honeyhive/sdk/datasets.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)      551 2023-03-05 06:42:19.000000 honeyhive-0.1.8/honeyhive/sdk/feedback.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)      711 2023-03-27 19:26:17.000000 honeyhive-0.1.8/honeyhive/sdk/fine_tuned_models.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     2947 2023-07-21 15:42:35.000000 honeyhive-0.1.8/honeyhive/sdk/generations.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)      245 2023-07-21 14:53:07.000000 honeyhive-0.1.8/honeyhive/sdk/init.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     1236 2023-03-27 19:28:28.000000 honeyhive-0.1.8/honeyhive/sdk/metrics.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     2352 2023-03-28 00:20:20.000000 honeyhive-0.1.8/honeyhive/sdk/projects.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     2415 2023-03-27 19:28:09.000000 honeyhive-0.1.8/honeyhive/sdk/prompts.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     5065 2023-03-26 17:31:47.000000 honeyhive-0.1.8/honeyhive/sdk/sdk-examples.py
-drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 15:43:30.913972 honeyhive-0.1.8/honeyhive.egg-info/
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     5542 2023-07-21 15:43:30.000000 honeyhive-0.1.8/honeyhive.egg-info/PKG-INFO
--rw-r--r--   0 dhruvsingh   (501) staff       (20)      981 2023-07-21 15:43:30.000000 honeyhive-0.1.8/honeyhive.egg-info/SOURCES.txt
--rw-r--r--   0 dhruvsingh   (501) staff       (20)        1 2023-07-21 15:43:30.000000 honeyhive-0.1.8/honeyhive.egg-info/dependency_links.txt
--rw-r--r--   0 dhruvsingh   (501) staff       (20)       54 2023-07-21 15:43:30.000000 honeyhive-0.1.8/honeyhive.egg-info/entry_points.txt
--rw-r--r--   0 dhruvsingh   (501) staff       (20)       75 2023-07-21 15:43:30.000000 honeyhive-0.1.8/honeyhive.egg-info/requires.txt
--rw-r--r--   0 dhruvsingh   (501) staff       (20)       10 2023-07-21 15:43:30.000000 honeyhive-0.1.8/honeyhive.egg-info/top_level.txt
--rw-r--r--   0 dhruvsingh   (501) staff       (20)      340 2023-03-05 06:49:29.000000 honeyhive-0.1.8/pyproject.toml
--rw-r--r--   0 dhruvsingh   (501) staff       (20)       38 2023-07-21 15:43:30.921776 honeyhive-0.1.8/setup.cfg
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     1634 2023-07-21 15:43:25.000000 honeyhive-0.1.8/setup.py
+drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 16:15:29.670129 honeyhive-0.1.9/
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)      205 2022-12-13 17:06:38.000000 honeyhive-0.1.9/LICENSE
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)       40 2022-12-09 00:56:14.000000 honeyhive-0.1.9/MANIFEST.in
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     5542 2023-07-21 16:15:29.669945 honeyhive-0.1.9/PKG-INFO
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     4567 2023-03-05 07:17:37.000000 honeyhive-0.1.9/README.md
+drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 16:15:29.665151 honeyhive-0.1.9/honeyhive/
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)       19 2022-12-26 05:27:25.000000 honeyhive-0.1.9/honeyhive/__init__.py
+drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 16:15:29.666063 honeyhive-0.1.9/honeyhive/api/
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)        0 2022-12-13 17:07:45.000000 honeyhive-0.1.9/honeyhive/api/__init__.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     6681 2023-03-05 06:41:14.000000 honeyhive-0.1.9/honeyhive/api/client.py
+drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 16:15:29.667426 honeyhive-0.1.9/honeyhive/api/models/
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)        0 2022-12-13 17:08:09.000000 honeyhive-0.1.9/honeyhive/api/models/__init__.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     2299 2023-03-05 07:44:40.000000 honeyhive-0.1.9/honeyhive/api/models/datasets.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     1140 2022-12-18 14:25:26.000000 honeyhive-0.1.9/honeyhive/api/models/feedback.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     1899 2023-03-05 07:27:57.000000 honeyhive-0.1.9/honeyhive/api/models/fine_tuned_models.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     6087 2023-07-21 15:42:46.000000 honeyhive-0.1.9/honeyhive/api/models/generations.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     1244 2023-03-05 07:45:16.000000 honeyhive-0.1.9/honeyhive/api/models/metrics.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     4415 2023-01-10 00:49:31.000000 honeyhive-0.1.9/honeyhive/api/models/prompts.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     2638 2023-01-09 23:57:51.000000 honeyhive-0.1.9/honeyhive/api/models/tasks.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)      257 2022-12-14 20:38:37.000000 honeyhive-0.1.9/honeyhive/api/models/utils.py
+drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 16:15:29.669532 honeyhive-0.1.9/honeyhive/sdk/
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     2798 2023-03-12 05:30:52.000000 honeyhive-0.1.9/honeyhive/sdk/ChatCompletion.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     2926 2023-06-09 15:56:04.000000 honeyhive-0.1.9/honeyhive/sdk/Completion.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     1225 2023-07-21 16:05:39.000000 honeyhive-0.1.9/honeyhive/sdk/__init__.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     1799 2023-03-27 19:26:27.000000 honeyhive-0.1.9/honeyhive/sdk/datasets.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)      551 2023-03-05 06:42:19.000000 honeyhive-0.1.9/honeyhive/sdk/feedback.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)      711 2023-03-27 19:26:17.000000 honeyhive-0.1.9/honeyhive/sdk/fine_tuned_models.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     2947 2023-07-21 15:42:35.000000 honeyhive-0.1.9/honeyhive/sdk/generations.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)      245 2023-07-21 14:53:07.000000 honeyhive-0.1.9/honeyhive/sdk/init.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     1236 2023-03-27 19:28:28.000000 honeyhive-0.1.9/honeyhive/sdk/metrics.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     2352 2023-03-28 00:20:20.000000 honeyhive-0.1.9/honeyhive/sdk/projects.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     2415 2023-03-27 19:28:09.000000 honeyhive-0.1.9/honeyhive/sdk/prompts.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     5065 2023-03-26 17:31:47.000000 honeyhive-0.1.9/honeyhive/sdk/sdk-examples.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)      328 2023-07-21 16:04:30.000000 honeyhive-0.1.9/honeyhive/sdk/utils.py
+drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 16:15:29.665854 honeyhive-0.1.9/honeyhive.egg-info/
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     5542 2023-07-21 16:15:29.000000 honeyhive-0.1.9/honeyhive.egg-info/PKG-INFO
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)      979 2023-07-21 16:15:29.000000 honeyhive-0.1.9/honeyhive.egg-info/SOURCES.txt
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)        1 2023-07-21 16:15:29.000000 honeyhive-0.1.9/honeyhive.egg-info/dependency_links.txt
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)       54 2023-07-21 16:15:29.000000 honeyhive-0.1.9/honeyhive.egg-info/entry_points.txt
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)       75 2023-07-21 16:15:29.000000 honeyhive-0.1.9/honeyhive.egg-info/requires.txt
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)       10 2023-07-21 16:15:29.000000 honeyhive-0.1.9/honeyhive.egg-info/top_level.txt
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)      340 2023-03-05 06:49:29.000000 honeyhive-0.1.9/pyproject.toml
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)       38 2023-07-21 16:15:29.670169 honeyhive-0.1.9/setup.cfg
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     1634 2023-07-21 16:15:16.000000 honeyhive-0.1.9/setup.py
```

### Comparing `honeyhive-0.1.8/PKG-INFO` & `honeyhive-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeyhive
-Version: 0.1.8
+Version: 0.1.9
 Summary: The HoneyHive SDK for Python
 Home-page: https://github.com/codehruv/honeyhive-sdk
 Author: HoneyHive
 Author-email: dhruv@honeyhive.ai
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.honeyhive.ai/
 Project-URL: Source, https://github.com/codehruv/honeyhive-sdk
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: honeyhive Version: 0.1.8 Summary: The HoneyHive SDK
+Metadata-Version: 2.1 Name: honeyhive Version: 0.1.9 Summary: The HoneyHive SDK
 for Python Home-page: https://github.com/codehruv/honeyhive-sdk Author:
 HoneyHive Author-email: dhruv@honeyhive.ai License: Apache License 2.0 Project-
 URL: Documentation, https://docs.honeyhive.ai/ Project-URL: Source, https://
 github.com/codehruv/honeyhive-sdk Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python Classifier:
```

### Comparing `honeyhive-0.1.8/README.md` & `honeyhive-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.8/honeyhive/api/client.py` & `honeyhive-0.1.9/honeyhive/api/client.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.8/honeyhive/api/models/datasets.py` & `honeyhive-0.1.9/honeyhive/api/models/datasets.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.8/honeyhive/api/models/feedback.py` & `honeyhive-0.1.9/honeyhive/api/models/feedback.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.8/honeyhive/api/models/fine_tuned_models.py` & `honeyhive-0.1.9/honeyhive/api/models/fine_tuned_models.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.8/honeyhive/api/models/generations.py` & `honeyhive-0.1.9/honeyhive/api/models/generations.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.8/honeyhive/api/models/metrics.py` & `honeyhive-0.1.9/honeyhive/api/models/metrics.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.8/honeyhive/api/models/prompts.py` & `honeyhive-0.1.9/honeyhive/api/models/prompts.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.8/honeyhive/api/models/tasks.py` & `honeyhive-0.1.9/honeyhive/api/models/tasks.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.8/honeyhive/sdk/ChatCompletion.py` & `honeyhive-0.1.9/honeyhive/sdk/ChatCompletion.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.8/honeyhive/sdk/Completion.py` & `honeyhive-0.1.9/honeyhive/sdk/Completion.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.8/honeyhive/sdk/__init__.py` & `honeyhive-0.1.9/honeyhive/sdk/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .metrics import *
 from .prompts import *
 from .projects import *
 from .fine_tuned_models import *
 from .generations import *
 from .Completion import *
 from .feedback import *
+from .utils import *
 
 import os 
 from typing import Optional
 
 api_key = os.environ.get("HONEYHIVE_API_KEY")
 # Path of a file with an API key, whose contents can change. Supercedes
 # `api_key` if set.  The main use case is volume-mounted Kubernetes secrets,
@@ -29,15 +30,16 @@
     "prompts",
     "projects",
     "fine_tuned_models",
     "Completion",
     "ChatCompletion",
     "generations",
     "feedback",
+    "utils",
     "api_key",
     "api_key_path",
     "organization",
     "api_base",
     "openai_api_key",
     "cohere_api_key",
-    "huggingface_api_key",
+    "huggingface_api_key"
 ]
```

### Comparing `honeyhive-0.1.8/honeyhive/sdk/datasets.py` & `honeyhive-0.1.9/honeyhive/sdk/datasets.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.8/honeyhive/sdk/feedback.py` & `honeyhive-0.1.9/honeyhive/sdk/feedback.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.8/honeyhive/sdk/fine_tuned_models.py` & `honeyhive-0.1.9/honeyhive/sdk/fine_tuned_models.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.8/honeyhive/sdk/generations.py` & `honeyhive-0.1.9/honeyhive/sdk/generations.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.8/honeyhive/sdk/metrics.py` & `honeyhive-0.1.9/honeyhive/sdk/metrics.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.8/honeyhive/sdk/projects.py` & `honeyhive-0.1.9/honeyhive/sdk/projects.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.8/honeyhive/sdk/prompts.py` & `honeyhive-0.1.9/honeyhive/sdk/prompts.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.8/honeyhive/sdk/sdk-examples.py` & `honeyhive-0.1.9/honeyhive/sdk/sdk-examples.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.8/honeyhive.egg-info/PKG-INFO` & `honeyhive-0.1.9/honeyhive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeyhive
-Version: 0.1.8
+Version: 0.1.9
 Summary: The HoneyHive SDK for Python
 Home-page: https://github.com/codehruv/honeyhive-sdk
 Author: HoneyHive
 Author-email: dhruv@honeyhive.ai
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.honeyhive.ai/
 Project-URL: Source, https://github.com/codehruv/honeyhive-sdk
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: honeyhive Version: 0.1.8 Summary: The HoneyHive SDK
+Metadata-Version: 2.1 Name: honeyhive Version: 0.1.9 Summary: The HoneyHive SDK
 for Python Home-page: https://github.com/codehruv/honeyhive-sdk Author:
 HoneyHive Author-email: dhruv@honeyhive.ai License: Apache License 2.0 Project-
 URL: Documentation, https://docs.honeyhive.ai/ Project-URL: Source, https://
 github.com/codehruv/honeyhive-sdk Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python Classifier:
```

### Comparing `honeyhive-0.1.8/honeyhive.egg-info/SOURCES.txt` & `honeyhive-0.1.9/honeyhive.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 honeyhive/api/models/generations.py
 honeyhive/api/models/metrics.py
 honeyhive/api/models/prompts.py
 honeyhive/api/models/tasks.py
 honeyhive/api/models/utils.py
 honeyhive/sdk/ChatCompletion.py
 honeyhive/sdk/Completion.py
-honeyhive/sdk/Untitled-3
 honeyhive/sdk/__init__.py
 honeyhive/sdk/datasets.py
 honeyhive/sdk/feedback.py
 honeyhive/sdk/fine_tuned_models.py
 honeyhive/sdk/generations.py
 honeyhive/sdk/init.py
 honeyhive/sdk/metrics.py
 honeyhive/sdk/projects.py
 honeyhive/sdk/prompts.py
-honeyhive/sdk/sdk-examples.py
+honeyhive/sdk/sdk-examples.py
+honeyhive/sdk/utils.py
```

### Comparing `honeyhive-0.1.8/setup.py` & `honeyhive-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     'console_scripts': [
         'honeyhive = honeyhive.cli:honeyhive'
     ]
 }
 
 setup(
     name='honeyhive',
-    version='0.1.8',
+    version='0.1.9',
     description='The HoneyHive SDK for Python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='HoneyHive',
     author_email="dhruv@honeyhive.ai",
     scripts=[],
     url='https://github.com/codehruv/honeyhive-sdk',
```

