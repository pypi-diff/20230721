# Comparing `tmp/cumulus_message_adapter_python-2.1.1.tar.gz` & `tmp/cumulus_message_adapter_python-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumulus_message_adapter_python-2.1.1.tar", last modified: Tue Jul 18 19:15:48 2023, max compression
+gzip compressed data, was "cumulus_message_adapter_python-2.2.0.tar", last modified: Fri Jul 21 18:57:46 2023, max compression
```

## Comparing `cumulus_message_adapter_python-2.1.1.tar` & `cumulus_message_adapter_python-2.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-18 19:15:48.208299 cumulus_message_adapter_python-2.1.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9768 2023-07-18 19:15:31.000000 cumulus_message_adapter_python-2.1.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2023-07-18 19:15:31.000000 cumulus_message_adapter_python-2.1.1/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8105 2023-07-18 19:15:48.208299 cumulus_message_adapter_python-2.1.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7494 2023-07-18 19:15:31.000000 cumulus_message_adapter_python-2.1.1/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13875 2023-07-18 19:15:31.000000 cumulus_message_adapter_python-2.1.1/cumulus_logger.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-18 19:15:48.208299 cumulus_message_adapter_python-2.1.1/cumulus_message_adapter_python.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8105 2023-07-18 19:15:48.000000 cumulus_message_adapter_python-2.1.1/cumulus_message_adapter_python.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      430 2023-07-18 19:15:48.000000 cumulus_message_adapter_python-2.1.1/cumulus_message_adapter_python.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-18 19:15:48.000000 cumulus_message_adapter_python-2.1.1/cumulus_message_adapter_python.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       31 2023-07-18 19:15:48.000000 cumulus_message_adapter_python-2.1.1/cumulus_message_adapter_python.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       32 2023-07-18 19:15:48.000000 cumulus_message_adapter_python-2.1.1/cumulus_message_adapter_python.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       31 2023-07-18 19:15:31.000000 cumulus_message_adapter_python-2.1.1/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3235 2023-07-18 19:15:31.000000 cumulus_message_adapter_python-2.1.1/run_cumulus_task.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-18 19:15:48.208299 cumulus_message_adapter_python-2.1.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2419 2023-07-18 19:15:31.000000 cumulus_message_adapter_python-2.1.1/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-18 19:15:48.208299 cumulus_message_adapter_python-2.1.1/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2859 2023-07-18 19:15:31.000000 cumulus_message_adapter_python-2.1.1/tests/test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1864 2023-07-18 19:15:31.000000 cumulus_message_adapter_python-2.1.1/tests/test_env_var.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6668 2023-07-18 19:15:31.000000 cumulus_message_adapter_python-2.1.1/tests/test_logger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       23 2023-07-18 19:15:31.000000 cumulus_message_adapter_python-2.1.1/version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 18:57:46.586699 cumulus_message_adapter_python-2.2.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9768 2023-07-21 18:57:34.000000 cumulus_message_adapter_python-2.2.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2023-07-21 18:57:34.000000 cumulus_message_adapter_python-2.2.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8105 2023-07-21 18:57:46.586699 cumulus_message_adapter_python-2.2.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7494 2023-07-21 18:57:34.000000 cumulus_message_adapter_python-2.2.0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13875 2023-07-21 18:57:34.000000 cumulus_message_adapter_python-2.2.0/cumulus_logger.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 18:57:46.586699 cumulus_message_adapter_python-2.2.0/cumulus_message_adapter_python.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8105 2023-07-21 18:57:46.000000 cumulus_message_adapter_python-2.2.0/cumulus_message_adapter_python.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      430 2023-07-21 18:57:46.000000 cumulus_message_adapter_python-2.2.0/cumulus_message_adapter_python.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-21 18:57:46.000000 cumulus_message_adapter_python-2.2.0/cumulus_message_adapter_python.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       31 2023-07-21 18:57:46.000000 cumulus_message_adapter_python-2.2.0/cumulus_message_adapter_python.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       32 2023-07-21 18:57:46.000000 cumulus_message_adapter_python-2.2.0/cumulus_message_adapter_python.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       31 2023-07-21 18:57:34.000000 cumulus_message_adapter_python-2.2.0/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3235 2023-07-21 18:57:34.000000 cumulus_message_adapter_python-2.2.0/run_cumulus_task.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-21 18:57:46.586699 cumulus_message_adapter_python-2.2.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2419 2023-07-21 18:57:34.000000 cumulus_message_adapter_python-2.2.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 18:57:46.586699 cumulus_message_adapter_python-2.2.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2859 2023-07-21 18:57:34.000000 cumulus_message_adapter_python-2.2.0/tests/test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1864 2023-07-21 18:57:34.000000 cumulus_message_adapter_python-2.2.0/tests/test_env_var.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6668 2023-07-21 18:57:34.000000 cumulus_message_adapter_python-2.2.0/tests/test_logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       23 2023-07-21 18:57:34.000000 cumulus_message_adapter_python-2.2.0/version.py
```

### Comparing `cumulus_message_adapter_python-2.1.1/LICENSE` & `cumulus_message_adapter_python-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cumulus_message_adapter_python-2.1.1/PKG-INFO` & `cumulus_message_adapter_python-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumulus_message_adapter_python
-Version: 2.1.1
+Version: 2.2.0
 Summary: A handler library for cumulus tasks written in python
 Home-page: https://github.com/cumulus-nasa/cumulus-message-adapter-python
 Author: Cumulus Authors
 Author-email: info@developmentseed.org
 Keywords: nasa cumulus
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `cumulus_message_adapter_python-2.1.1/README.md` & `cumulus_message_adapter_python-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_message_adapter_python-2.1.1/cumulus_logger.py` & `cumulus_message_adapter_python-2.2.0/cumulus_logger.py`

 * *Files identical despite different names*

### Comparing `cumulus_message_adapter_python-2.1.1/cumulus_message_adapter_python.egg-info/PKG-INFO` & `cumulus_message_adapter_python-2.2.0/cumulus_message_adapter_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumulus-message-adapter-python
-Version: 2.1.1
+Version: 2.2.0
 Summary: A handler library for cumulus tasks written in python
 Home-page: https://github.com/cumulus-nasa/cumulus-message-adapter-python
 Author: Cumulus Authors
 Author-email: info@developmentseed.org
 Keywords: nasa cumulus
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `cumulus_message_adapter_python-2.1.1/run_cumulus_task.py` & `cumulus_message_adapter_python-2.2.0/run_cumulus_task.py`

 * *Files identical despite different names*

### Comparing `cumulus_message_adapter_python-2.1.1/setup.py` & `cumulus_message_adapter_python-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `cumulus_message_adapter_python-2.1.1/tests/test.py` & `cumulus_message_adapter_python-2.2.0/tests/test.py`

 * *Files identical despite different names*

### Comparing `cumulus_message_adapter_python-2.1.1/tests/test_env_var.py` & `cumulus_message_adapter_python-2.2.0/tests/test_env_var.py`

 * *Files identical despite different names*

### Comparing `cumulus_message_adapter_python-2.1.1/tests/test_logger.py` & `cumulus_message_adapter_python-2.2.0/tests/test_logger.py`

 * *Files identical despite different names*

