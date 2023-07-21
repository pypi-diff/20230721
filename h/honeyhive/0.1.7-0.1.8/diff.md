# Comparing `tmp/honeyhive-0.1.7.tar.gz` & `tmp/honeyhive-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "honeyhive-0.1.7.tar", last modified: Fri Jul 21 15:41:26 2023, max compression
+gzip compressed data, was "honeyhive-0.1.8.tar", last modified: Fri Jul 21 15:43:30 2023, max compression
```

## Comparing `honeyhive-0.1.7.tar` & `honeyhive-0.1.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 15:41:26.172913 honeyhive-0.1.7/
--rw-r--r--   0 dhruvsingh   (501) staff       (20)      205 2022-12-13 17:06:38.000000 honeyhive-0.1.7/LICENSE
--rw-r--r--   0 dhruvsingh   (501) staff       (20)       40 2022-12-09 00:56:14.000000 honeyhive-0.1.7/MANIFEST.in
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     5542 2023-07-21 15:41:26.172731 honeyhive-0.1.7/PKG-INFO
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     4567 2023-03-05 07:17:37.000000 honeyhive-0.1.7/README.md
-drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 15:41:26.164310 honeyhive-0.1.7/honeyhive/
--rw-r--r--   0 dhruvsingh   (501) staff       (20)       19 2022-12-26 05:27:25.000000 honeyhive-0.1.7/honeyhive/__init__.py
-drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 15:41:26.165681 honeyhive-0.1.7/honeyhive/api/
--rw-r--r--   0 dhruvsingh   (501) staff       (20)        0 2022-12-13 17:07:45.000000 honeyhive-0.1.7/honeyhive/api/__init__.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     6681 2023-03-05 06:41:14.000000 honeyhive-0.1.7/honeyhive/api/client.py
-drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 15:41:26.167873 honeyhive-0.1.7/honeyhive/api/models/
--rw-r--r--   0 dhruvsingh   (501) staff       (20)        0 2022-12-13 17:08:09.000000 honeyhive-0.1.7/honeyhive/api/models/__init__.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     2299 2023-03-05 07:44:40.000000 honeyhive-0.1.7/honeyhive/api/models/datasets.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     1140 2022-12-18 14:25:26.000000 honeyhive-0.1.7/honeyhive/api/models/feedback.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     1899 2023-03-05 07:27:57.000000 honeyhive-0.1.7/honeyhive/api/models/fine_tuned_models.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     5940 2023-07-21 15:39:24.000000 honeyhive-0.1.7/honeyhive/api/models/generations.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     1244 2023-03-05 07:45:16.000000 honeyhive-0.1.7/honeyhive/api/models/metrics.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     4415 2023-01-10 00:49:31.000000 honeyhive-0.1.7/honeyhive/api/models/prompts.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     2638 2023-01-09 23:57:51.000000 honeyhive-0.1.7/honeyhive/api/models/tasks.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)      257 2022-12-14 20:38:37.000000 honeyhive-0.1.7/honeyhive/api/models/utils.py
-drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 15:41:26.172352 honeyhive-0.1.7/honeyhive/sdk/
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     2798 2023-03-12 05:30:52.000000 honeyhive-0.1.7/honeyhive/sdk/ChatCompletion.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     2926 2023-06-09 15:56:04.000000 honeyhive-0.1.7/honeyhive/sdk/Completion.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)        0 2022-12-31 04:55:35.000000 honeyhive-0.1.7/honeyhive/sdk/Untitled-3
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     1192 2023-03-28 00:19:47.000000 honeyhive-0.1.7/honeyhive/sdk/__init__.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     1799 2023-03-27 19:26:27.000000 honeyhive-0.1.7/honeyhive/sdk/datasets.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)      551 2023-03-05 06:42:19.000000 honeyhive-0.1.7/honeyhive/sdk/feedback.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)      711 2023-03-27 19:26:17.000000 honeyhive-0.1.7/honeyhive/sdk/fine_tuned_models.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     2869 2023-07-21 15:39:27.000000 honeyhive-0.1.7/honeyhive/sdk/generations.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)      245 2023-07-21 14:53:07.000000 honeyhive-0.1.7/honeyhive/sdk/init.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     1236 2023-03-27 19:28:28.000000 honeyhive-0.1.7/honeyhive/sdk/metrics.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     2352 2023-03-28 00:20:20.000000 honeyhive-0.1.7/honeyhive/sdk/projects.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     2415 2023-03-27 19:28:09.000000 honeyhive-0.1.7/honeyhive/sdk/prompts.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     5065 2023-03-26 17:31:47.000000 honeyhive-0.1.7/honeyhive/sdk/sdk-examples.py
-drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 15:41:26.165431 honeyhive-0.1.7/honeyhive.egg-info/
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     5542 2023-07-21 15:41:26.000000 honeyhive-0.1.7/honeyhive.egg-info/PKG-INFO
--rw-r--r--   0 dhruvsingh   (501) staff       (20)      981 2023-07-21 15:41:26.000000 honeyhive-0.1.7/honeyhive.egg-info/SOURCES.txt
--rw-r--r--   0 dhruvsingh   (501) staff       (20)        1 2023-07-21 15:41:26.000000 honeyhive-0.1.7/honeyhive.egg-info/dependency_links.txt
--rw-r--r--   0 dhruvsingh   (501) staff       (20)       54 2023-07-21 15:41:26.000000 honeyhive-0.1.7/honeyhive.egg-info/entry_points.txt
--rw-r--r--   0 dhruvsingh   (501) staff       (20)       75 2023-07-21 15:41:26.000000 honeyhive-0.1.7/honeyhive.egg-info/requires.txt
--rw-r--r--   0 dhruvsingh   (501) staff       (20)       10 2023-07-21 15:41:26.000000 honeyhive-0.1.7/honeyhive.egg-info/top_level.txt
--rw-r--r--   0 dhruvsingh   (501) staff       (20)      340 2023-03-05 06:49:29.000000 honeyhive-0.1.7/pyproject.toml
--rw-r--r--   0 dhruvsingh   (501) staff       (20)       38 2023-07-21 15:41:26.172958 honeyhive-0.1.7/setup.cfg
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     1634 2023-07-21 15:41:20.000000 honeyhive-0.1.7/setup.py
+drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 15:43:30.921732 honeyhive-0.1.8/
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)      205 2022-12-13 17:06:38.000000 honeyhive-0.1.8/LICENSE
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)       40 2022-12-09 00:56:14.000000 honeyhive-0.1.8/MANIFEST.in
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     5542 2023-07-21 15:43:30.921522 honeyhive-0.1.8/PKG-INFO
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     4567 2023-03-05 07:17:37.000000 honeyhive-0.1.8/README.md
+drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 15:43:30.913181 honeyhive-0.1.8/honeyhive/
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)       19 2022-12-26 05:27:25.000000 honeyhive-0.1.8/honeyhive/__init__.py
+drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 15:43:30.914207 honeyhive-0.1.8/honeyhive/api/
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)        0 2022-12-13 17:07:45.000000 honeyhive-0.1.8/honeyhive/api/__init__.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     6681 2023-03-05 06:41:14.000000 honeyhive-0.1.8/honeyhive/api/client.py
+drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 15:43:30.917021 honeyhive-0.1.8/honeyhive/api/models/
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)        0 2022-12-13 17:08:09.000000 honeyhive-0.1.8/honeyhive/api/models/__init__.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     2299 2023-03-05 07:44:40.000000 honeyhive-0.1.8/honeyhive/api/models/datasets.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     1140 2022-12-18 14:25:26.000000 honeyhive-0.1.8/honeyhive/api/models/feedback.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     1899 2023-03-05 07:27:57.000000 honeyhive-0.1.8/honeyhive/api/models/fine_tuned_models.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     6087 2023-07-21 15:42:46.000000 honeyhive-0.1.8/honeyhive/api/models/generations.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     1244 2023-03-05 07:45:16.000000 honeyhive-0.1.8/honeyhive/api/models/metrics.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     4415 2023-01-10 00:49:31.000000 honeyhive-0.1.8/honeyhive/api/models/prompts.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     2638 2023-01-09 23:57:51.000000 honeyhive-0.1.8/honeyhive/api/models/tasks.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)      257 2022-12-14 20:38:37.000000 honeyhive-0.1.8/honeyhive/api/models/utils.py
+drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 15:43:30.920909 honeyhive-0.1.8/honeyhive/sdk/
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     2798 2023-03-12 05:30:52.000000 honeyhive-0.1.8/honeyhive/sdk/ChatCompletion.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     2926 2023-06-09 15:56:04.000000 honeyhive-0.1.8/honeyhive/sdk/Completion.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)        0 2022-12-31 04:55:35.000000 honeyhive-0.1.8/honeyhive/sdk/Untitled-3
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     1192 2023-03-28 00:19:47.000000 honeyhive-0.1.8/honeyhive/sdk/__init__.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     1799 2023-03-27 19:26:27.000000 honeyhive-0.1.8/honeyhive/sdk/datasets.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)      551 2023-03-05 06:42:19.000000 honeyhive-0.1.8/honeyhive/sdk/feedback.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)      711 2023-03-27 19:26:17.000000 honeyhive-0.1.8/honeyhive/sdk/fine_tuned_models.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     2947 2023-07-21 15:42:35.000000 honeyhive-0.1.8/honeyhive/sdk/generations.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)      245 2023-07-21 14:53:07.000000 honeyhive-0.1.8/honeyhive/sdk/init.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     1236 2023-03-27 19:28:28.000000 honeyhive-0.1.8/honeyhive/sdk/metrics.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     2352 2023-03-28 00:20:20.000000 honeyhive-0.1.8/honeyhive/sdk/projects.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     2415 2023-03-27 19:28:09.000000 honeyhive-0.1.8/honeyhive/sdk/prompts.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     5065 2023-03-26 17:31:47.000000 honeyhive-0.1.8/honeyhive/sdk/sdk-examples.py
+drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-21 15:43:30.913972 honeyhive-0.1.8/honeyhive.egg-info/
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     5542 2023-07-21 15:43:30.000000 honeyhive-0.1.8/honeyhive.egg-info/PKG-INFO
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)      981 2023-07-21 15:43:30.000000 honeyhive-0.1.8/honeyhive.egg-info/SOURCES.txt
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)        1 2023-07-21 15:43:30.000000 honeyhive-0.1.8/honeyhive.egg-info/dependency_links.txt
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)       54 2023-07-21 15:43:30.000000 honeyhive-0.1.8/honeyhive.egg-info/entry_points.txt
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)       75 2023-07-21 15:43:30.000000 honeyhive-0.1.8/honeyhive.egg-info/requires.txt
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)       10 2023-07-21 15:43:30.000000 honeyhive-0.1.8/honeyhive.egg-info/top_level.txt
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)      340 2023-03-05 06:49:29.000000 honeyhive-0.1.8/pyproject.toml
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)       38 2023-07-21 15:43:30.921776 honeyhive-0.1.8/setup.cfg
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     1634 2023-07-21 15:43:25.000000 honeyhive-0.1.8/setup.py
```

### Comparing `honeyhive-0.1.7/PKG-INFO` & `honeyhive-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeyhive
-Version: 0.1.7
+Version: 0.1.8
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
-Metadata-Version: 2.1 Name: honeyhive Version: 0.1.7 Summary: The HoneyHive SDK
+Metadata-Version: 2.1 Name: honeyhive Version: 0.1.8 Summary: The HoneyHive SDK
 for Python Home-page: https://github.com/codehruv/honeyhive-sdk Author:
 HoneyHive Author-email: dhruv@honeyhive.ai License: Apache License 2.0 Project-
 URL: Documentation, https://docs.honeyhive.ai/ Project-URL: Source, https://
 github.com/codehruv/honeyhive-sdk Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python Classifier:
```

### Comparing `honeyhive-0.1.7/README.md` & `honeyhive-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.7/honeyhive/api/client.py` & `honeyhive-0.1.8/honeyhive/api/client.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.7/honeyhive/api/models/datasets.py` & `honeyhive-0.1.8/honeyhive/api/models/datasets.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.7/honeyhive/api/models/feedback.py` & `honeyhive-0.1.8/honeyhive/api/models/feedback.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.7/honeyhive/api/models/fine_tuned_models.py` & `honeyhive-0.1.8/honeyhive/api/models/fine_tuned_models.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.7/honeyhive/api/models/generations.py` & `honeyhive-0.1.8/honeyhive/api/models/generations.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,18 @@
         title="Metadata",
         description="The metadata to track for the generation"
     )
     ground_truth: Optional[str] = Field(
         title="Ground Truth",
         description="The ground truth for the generation"
     )
+    feedback: Optional[Dict[str, Any]] = Field(
+        title="Feedback",
+        description="The feedback associated with this generation"
+    )
 
 
 class Generation(BaseModel):
     generation_id: str = Field(
         title="Generation ID",
         description="The unique ID of the generation"
     )
```

### Comparing `honeyhive-0.1.7/honeyhive/api/models/metrics.py` & `honeyhive-0.1.8/honeyhive/api/models/metrics.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.7/honeyhive/api/models/prompts.py` & `honeyhive-0.1.8/honeyhive/api/models/prompts.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.7/honeyhive/api/models/tasks.py` & `honeyhive-0.1.8/honeyhive/api/models/tasks.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.7/honeyhive/sdk/ChatCompletion.py` & `honeyhive-0.1.8/honeyhive/sdk/ChatCompletion.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.7/honeyhive/sdk/Completion.py` & `honeyhive-0.1.8/honeyhive/sdk/Completion.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.7/honeyhive/sdk/__init__.py` & `honeyhive-0.1.8/honeyhive/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.7/honeyhive/sdk/datasets.py` & `honeyhive-0.1.8/honeyhive/sdk/datasets.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.7/honeyhive/sdk/feedback.py` & `honeyhive-0.1.8/honeyhive/sdk/feedback.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.7/honeyhive/sdk/fine_tuned_models.py` & `honeyhive-0.1.8/honeyhive/sdk/fine_tuned_models.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.7/honeyhive/sdk/generations.py` & `honeyhive-0.1.8/honeyhive/sdk/generations.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,16 @@
     prompt_template: Optional[str] = None,
     inputs: Optional[Dict[str, Any]] = None,
     prompt: Optional[str] = None,
     ground_truth: Optional[str] = None,
     usage: Optional[Dict[str, Any]] = None,
     latency: Optional[float] = None,
     user_properties: Optional[Dict[str, Any]] = None,
-    metadata: Optional[Dict[str, Any]] = None
+    metadata: Optional[Dict[str, Any]] = None,
+    feedback: Optional[Dict[str, Any]] = None
 ) -> GenerationResponse:
     # log generation via honeyhive
     client = honeyhive_client()
 
     if prompt == None:
         prompt = prompt_template
         if inputs == None and prompt_template == None:
@@ -78,15 +79,16 @@
             hyperparameters=hyperparameters,
             generation=generation,
             usage=usage,
             latency=latency,
             source=source,
             user_properties=user_properties,
             metadata=metadata,
-            ground_truth=ground_truth
+            ground_truth=ground_truth,
+            feedback=feedback
         )
     )
 
     return honeyhive_response
 
 __all__ = [
     "generate",
```

### Comparing `honeyhive-0.1.7/honeyhive/sdk/metrics.py` & `honeyhive-0.1.8/honeyhive/sdk/metrics.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.7/honeyhive/sdk/projects.py` & `honeyhive-0.1.8/honeyhive/sdk/projects.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.7/honeyhive/sdk/prompts.py` & `honeyhive-0.1.8/honeyhive/sdk/prompts.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.7/honeyhive/sdk/sdk-examples.py` & `honeyhive-0.1.8/honeyhive/sdk/sdk-examples.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.7/honeyhive.egg-info/PKG-INFO` & `honeyhive-0.1.8/honeyhive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeyhive
-Version: 0.1.7
+Version: 0.1.8
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
-Metadata-Version: 2.1 Name: honeyhive Version: 0.1.7 Summary: The HoneyHive SDK
+Metadata-Version: 2.1 Name: honeyhive Version: 0.1.8 Summary: The HoneyHive SDK
 for Python Home-page: https://github.com/codehruv/honeyhive-sdk Author:
 HoneyHive Author-email: dhruv@honeyhive.ai License: Apache License 2.0 Project-
 URL: Documentation, https://docs.honeyhive.ai/ Project-URL: Source, https://
 github.com/codehruv/honeyhive-sdk Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python Classifier:
```

### Comparing `honeyhive-0.1.7/honeyhive.egg-info/SOURCES.txt` & `honeyhive-0.1.8/honeyhive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.7/setup.py` & `honeyhive-0.1.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     'console_scripts': [
         'honeyhive = honeyhive.cli:honeyhive'
     ]
 }
 
 setup(
     name='honeyhive',
-    version='0.1.7',
+    version='0.1.8',
     description='The HoneyHive SDK for Python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='HoneyHive',
     author_email="dhruv@honeyhive.ai",
     scripts=[],
     url='https://github.com/codehruv/honeyhive-sdk',
```

