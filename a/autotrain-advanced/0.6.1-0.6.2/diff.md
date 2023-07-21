# Comparing `tmp/autotrain-advanced-0.6.1.tar.gz` & `tmp/autotrain-advanced-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotrain-advanced-0.6.1.tar", last modified: Thu Jul 20 12:00:38 2023, max compression
+gzip compressed data, was "autotrain-advanced-0.6.2.tar", last modified: Fri Jul 21 11:05:10 2023, max compression
```

## Comparing `autotrain-advanced-0.6.1.tar` & `autotrain-advanced-0.6.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-20 12:00:38.982289 autotrain-advanced-0.6.1/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.1/LICENSE
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-20 12:00:38.982289 autotrain-advanced-0.6.1/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.6.1/README.md
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      354 2023-07-20 12:00:38.982289 autotrain-advanced-0.6.1/setup.cfg
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2130 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.1/setup.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-20 12:00:38.982289 autotrain-advanced-0.6.1/src/
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-20 12:00:38.982289 autotrain-advanced-0.6.1/src/autotrain/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      816 2023-07-20 12:00:33.000000 autotrain-advanced-0.6.1/src/autotrain/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    38466 2023-07-17 12:32:57.000000 autotrain-advanced-0.6.1/src/autotrain/app.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-20 12:00:38.982289 autotrain-advanced-0.6.1/src/autotrain/cli/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-02-01 13:00:34.000000 autotrain-advanced-0.6.1/src/autotrain/cli/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1033 2023-07-19 10:07:30.000000 autotrain-advanced-0.6.1/src/autotrain/cli/autotrain.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1268 2023-06-21 11:15:59.000000 autotrain-advanced-0.6.1/src/autotrain/cli/run_app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-07-13 15:03:01.000000 autotrain-advanced-0.6.1/src/autotrain/cli/run_dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14842 2023-07-20 12:00:11.000000 autotrain-advanced-0.6.1/src/autotrain/cli/run_llm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2178 2023-07-19 10:23:02.000000 autotrain-advanced-0.6.1/src/autotrain/cli/run_setup.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-04-29 09:05:02.000000 autotrain-advanced-0.6.1/src/autotrain/config.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12419 2023-07-19 10:21:07.000000 autotrain-advanced-0.6.1/src/autotrain/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1483 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.1/src/autotrain/help.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-20 12:00:38.982289 autotrain-advanced-0.6.1/src/autotrain/infer/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-07-20 09:08:58.000000 autotrain-advanced-0.6.1/src/autotrain/infer/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1885 2023-07-20 12:00:25.000000 autotrain-advanced-0.6.1/src/autotrain/infer/text_generation.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      197 2023-04-14 11:28:41.000000 autotrain-advanced-0.6.1/src/autotrain/languages.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17211 2023-07-19 09:53:41.000000 autotrain-advanced-0.6.1/src/autotrain/params.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-20 12:00:38.982289 autotrain-advanced-0.6.1/src/autotrain/preprocessor/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.6.1/src/autotrain/preprocessor/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1741 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.1/src/autotrain/preprocessor/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3991 2023-04-29 09:05:23.000000 autotrain-advanced-0.6.1/src/autotrain/preprocessor/tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9231 2023-04-29 09:05:46.000000 autotrain-advanced-0.6.1/src/autotrain/preprocessor/text.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6549 2023-05-31 09:41:05.000000 autotrain-advanced-0.6.1/src/autotrain/preprocessor/vision.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8164 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.1/src/autotrain/project.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.1/src/autotrain/splits.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2779 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.1/src/autotrain/tasks.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-20 12:00:38.982289 autotrain-advanced-0.6.1/src/autotrain/trainers/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.1/src/autotrain/trainers/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1305 2023-07-05 07:53:30.000000 autotrain-advanced-0.6.1/src/autotrain/trainers/callbacks.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10663 2023-07-20 12:00:11.000000 autotrain-advanced-0.6.1/src/autotrain/trainers/clm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    34306 2023-07-18 10:31:20.000000 autotrain-advanced-0.6.1/src/autotrain/trainers/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10026 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.1/src/autotrain/trainers/image_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14726 2023-06-22 02:39:49.000000 autotrain-advanced-0.6.1/src/autotrain/trainers/lm_trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9119 2023-06-20 09:52:02.000000 autotrain-advanced-0.6.1/src/autotrain/trainers/text_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5756 2023-07-19 09:53:41.000000 autotrain-advanced-0.6.1/src/autotrain/trainers/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8221 2023-07-19 10:14:57.000000 autotrain-advanced-0.6.1/src/autotrain/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-20 12:00:38.982289 autotrain-advanced-0.6.1/src/autotrain_advanced.egg-info/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-20 12:00:38.000000 autotrain-advanced-0.6.1/src/autotrain_advanced.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1325 2023-07-20 12:00:38.000000 autotrain-advanced-0.6.1/src/autotrain_advanced.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-07-20 12:00:38.000000 autotrain-advanced-0.6.1/src/autotrain_advanced.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-07-20 12:00:38.000000 autotrain-advanced-0.6.1/src/autotrain_advanced.egg-info/entry_points.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2097 2023-07-20 12:00:38.000000 autotrain-advanced-0.6.1/src/autotrain_advanced.egg-info/requires.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-07-20 12:00:38.000000 autotrain-advanced-0.6.1/src/autotrain_advanced.egg-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-21 11:05:10.448928 autotrain-advanced-0.6.2/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.2/LICENSE
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-21 11:05:10.448928 autotrain-advanced-0.6.2/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.6.2/README.md
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      354 2023-07-21 11:05:10.448928 autotrain-advanced-0.6.2/setup.cfg
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2130 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.2/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-21 11:05:10.444928 autotrain-advanced-0.6.2/src/
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-21 11:05:10.444928 autotrain-advanced-0.6.2/src/autotrain/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      816 2023-07-21 11:05:06.000000 autotrain-advanced-0.6.2/src/autotrain/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    38466 2023-07-17 12:32:57.000000 autotrain-advanced-0.6.2/src/autotrain/app.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-21 11:05:10.444928 autotrain-advanced-0.6.2/src/autotrain/cli/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-02-01 13:00:34.000000 autotrain-advanced-0.6.2/src/autotrain/cli/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1033 2023-07-19 10:07:30.000000 autotrain-advanced-0.6.2/src/autotrain/cli/autotrain.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1268 2023-06-21 11:15:59.000000 autotrain-advanced-0.6.2/src/autotrain/cli/run_app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-07-13 15:03:01.000000 autotrain-advanced-0.6.2/src/autotrain/cli/run_dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14842 2023-07-20 12:00:11.000000 autotrain-advanced-0.6.2/src/autotrain/cli/run_llm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2178 2023-07-19 10:23:02.000000 autotrain-advanced-0.6.2/src/autotrain/cli/run_setup.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-04-29 09:05:02.000000 autotrain-advanced-0.6.2/src/autotrain/config.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12419 2023-07-19 10:21:07.000000 autotrain-advanced-0.6.2/src/autotrain/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1483 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.2/src/autotrain/help.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-21 11:05:10.444928 autotrain-advanced-0.6.2/src/autotrain/infer/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-07-20 09:08:58.000000 autotrain-advanced-0.6.2/src/autotrain/infer/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1885 2023-07-20 12:00:25.000000 autotrain-advanced-0.6.2/src/autotrain/infer/text_generation.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      197 2023-04-14 11:28:41.000000 autotrain-advanced-0.6.2/src/autotrain/languages.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17211 2023-07-19 09:53:41.000000 autotrain-advanced-0.6.2/src/autotrain/params.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-21 11:05:10.448928 autotrain-advanced-0.6.2/src/autotrain/preprocessor/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.6.2/src/autotrain/preprocessor/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1741 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.2/src/autotrain/preprocessor/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3991 2023-04-29 09:05:23.000000 autotrain-advanced-0.6.2/src/autotrain/preprocessor/tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9231 2023-04-29 09:05:46.000000 autotrain-advanced-0.6.2/src/autotrain/preprocessor/text.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6549 2023-05-31 09:41:05.000000 autotrain-advanced-0.6.2/src/autotrain/preprocessor/vision.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8164 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.2/src/autotrain/project.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.2/src/autotrain/splits.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2779 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.2/src/autotrain/tasks.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-21 11:05:10.448928 autotrain-advanced-0.6.2/src/autotrain/trainers/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.2/src/autotrain/trainers/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1305 2023-07-05 07:53:30.000000 autotrain-advanced-0.6.2/src/autotrain/trainers/callbacks.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10768 2023-07-21 11:04:59.000000 autotrain-advanced-0.6.2/src/autotrain/trainers/clm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    34306 2023-07-18 10:31:20.000000 autotrain-advanced-0.6.2/src/autotrain/trainers/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10026 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.2/src/autotrain/trainers/image_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14726 2023-06-22 02:39:49.000000 autotrain-advanced-0.6.2/src/autotrain/trainers/lm_trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9119 2023-06-20 09:52:02.000000 autotrain-advanced-0.6.2/src/autotrain/trainers/text_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5756 2023-07-19 09:53:41.000000 autotrain-advanced-0.6.2/src/autotrain/trainers/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8221 2023-07-19 10:14:57.000000 autotrain-advanced-0.6.2/src/autotrain/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-21 11:05:10.448928 autotrain-advanced-0.6.2/src/autotrain_advanced.egg-info/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-21 11:05:10.000000 autotrain-advanced-0.6.2/src/autotrain_advanced.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1325 2023-07-21 11:05:10.000000 autotrain-advanced-0.6.2/src/autotrain_advanced.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-07-21 11:05:10.000000 autotrain-advanced-0.6.2/src/autotrain_advanced.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-07-21 11:05:10.000000 autotrain-advanced-0.6.2/src/autotrain_advanced.egg-info/entry_points.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2097 2023-07-21 11:05:10.000000 autotrain-advanced-0.6.2/src/autotrain_advanced.egg-info/requires.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-07-21 11:05:10.000000 autotrain-advanced-0.6.2/src/autotrain_advanced.egg-info/top_level.txt
```

### Comparing `autotrain-advanced-0.6.1/LICENSE` & `autotrain-advanced-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/PKG-INFO` & `autotrain-advanced-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.6.1
+Version: 0.6.2
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.6.1/setup.py` & `autotrain-advanced-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain/__init__.py` & `autotrain-advanced-0.6.2/src/autotrain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 # pylint: enable=line-too-long
 import os
 
 
 # ignore bnb warnings
 os.environ["BITSANDBYTES_NOWELCOME"] = "1"
 os.environ["HF_HUB_DISABLE_PROGRESS_BARS"] = "1"
-__version__ = "0.6.1"
+__version__ = "0.6.2"
```

### Comparing `autotrain-advanced-0.6.1/src/autotrain/app.py` & `autotrain-advanced-0.6.2/src/autotrain/app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain/cli/autotrain.py` & `autotrain-advanced-0.6.2/src/autotrain/cli/autotrain.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain/cli/run_app.py` & `autotrain-advanced-0.6.2/src/autotrain/cli/run_app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain/cli/run_llm.py` & `autotrain-advanced-0.6.2/src/autotrain/cli/run_llm.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain/cli/run_setup.py` & `autotrain-advanced-0.6.2/src/autotrain/cli/run_setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain/dataset.py` & `autotrain-advanced-0.6.2/src/autotrain/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain/help.py` & `autotrain-advanced-0.6.2/src/autotrain/help.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain/infer/text_generation.py` & `autotrain-advanced-0.6.2/src/autotrain/infer/text_generation.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain/params.py` & `autotrain-advanced-0.6.2/src/autotrain/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain/preprocessor/dreambooth.py` & `autotrain-advanced-0.6.2/src/autotrain/preprocessor/dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain/preprocessor/tabular.py` & `autotrain-advanced-0.6.2/src/autotrain/preprocessor/tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain/preprocessor/text.py` & `autotrain-advanced-0.6.2/src/autotrain/preprocessor/text.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain/preprocessor/vision.py` & `autotrain-advanced-0.6.2/src/autotrain/preprocessor/vision.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain/project.py` & `autotrain-advanced-0.6.2/src/autotrain/project.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain/tasks.py` & `autotrain-advanced-0.6.2/src/autotrain/tasks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain/trainers/callbacks.py` & `autotrain-advanced-0.6.2/src/autotrain/trainers/callbacks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain/trainers/clm.py` & `autotrain-advanced-0.6.2/src/autotrain/trainers/clm.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 from autotrain.trainers.callbacks import LoadBestPeftModelCallback, SavePeftModelCallback
 
 
 def train(config):
     if isinstance(config, dict):
         config = utils.LLMTrainingParams(**config)
 
+    # TODO: remove when SFT is fixed
+    if config.trainer == "sft":
+        config.trainer = "default"
+
     # check if config.train_split.csv exists in config.data_path
     if config.train_split is not None:
         train_path = f"{config.data_path}/{config.train_split}.csv"
         if os.path.exists(train_path):
             logger.info("loading dataset from csv")
             train_data = pd.read_csv(train_path)
             train_data = Dataset.from_pandas(train_data)
```

### Comparing `autotrain-advanced-0.6.1/src/autotrain/trainers/dreambooth.py` & `autotrain-advanced-0.6.2/src/autotrain/trainers/dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain/trainers/image_classification.py` & `autotrain-advanced-0.6.2/src/autotrain/trainers/image_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain/trainers/lm_trainer.py` & `autotrain-advanced-0.6.2/src/autotrain/trainers/lm_trainer.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain/trainers/text_classification.py` & `autotrain-advanced-0.6.2/src/autotrain/trainers/text_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain/trainers/utils.py` & `autotrain-advanced-0.6.2/src/autotrain/trainers/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain/utils.py` & `autotrain-advanced-0.6.2/src/autotrain/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain_advanced.egg-info/PKG-INFO` & `autotrain-advanced-0.6.2/src/autotrain_advanced.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.6.1
+Version: 0.6.2
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.6.1/src/autotrain_advanced.egg-info/SOURCES.txt` & `autotrain-advanced-0.6.2/src/autotrain_advanced.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.1/src/autotrain_advanced.egg-info/requires.txt` & `autotrain-advanced-0.6.2/src/autotrain_advanced.egg-info/requires.txt`

 * *Files identical despite different names*

