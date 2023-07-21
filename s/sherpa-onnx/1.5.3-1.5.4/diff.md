# Comparing `tmp/sherpa-onnx-1.5.3.tar.gz` & `tmp/sherpa-onnx-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherpa-onnx-1.5.3.tar", last modified: Sat Jul 15 04:42:37 2023, max compression
+gzip compressed data, was "sherpa-onnx-1.5.4.tar", last modified: Fri Jul 21 10:38:56 2023, max compression
```

## Comparing `sherpa-onnx-1.5.3.tar` & `sherpa-onnx-1.5.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:42:37.663394 sherpa-onnx-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-15 04:31:33.000000 sherpa-onnx-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-15 04:42:37.663394 sherpa-onnx-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-15 04:31:33.000000 sherpa-onnx-1.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 04:42:37.663394 sherpa-onnx-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-15 04:31:33.000000 sherpa-onnx-1.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:42:37.659394 sherpa-onnx-1.5.3/sherpa-onnx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:42:37.659394 sherpa-onnx-1.5.3/sherpa-onnx/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:42:37.663394 sherpa-onnx-1.5.3/sherpa-onnx/python/sherpa_onnx/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-15 04:42:37.000000 sherpa-onnx-1.5.3/sherpa-onnx/python/sherpa_onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-07-15 04:31:33.000000 sherpa-onnx-1.5.3/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-07-15 04:31:33.000000 sherpa-onnx-1.5.3/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-15 04:31:33.000000 sherpa-onnx-1.5.3/sherpa-onnx/python/sherpa_onnx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:42:37.663394 sherpa-onnx-1.5.3/sherpa_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-15 04:42:37.000000 sherpa-onnx-1.5.3/sherpa_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-15 04:42:37.000000 sherpa-onnx-1.5.3/sherpa_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 04:42:37.000000 sherpa-onnx-1.5.3/sherpa_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 04:42:37.000000 sherpa-onnx-1.5.3/sherpa_onnx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-15 04:42:37.000000 sherpa-onnx-1.5.3/sherpa_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-15 04:42:37.000000 sherpa-onnx-1.5.3/sherpa_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:56.003717 sherpa-onnx-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-21 10:28:13.000000 sherpa-onnx-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-21 10:38:56.003717 sherpa-onnx-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-21 10:28:13.000000 sherpa-onnx-1.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 10:38:56.003717 sherpa-onnx-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-21 10:28:13.000000 sherpa-onnx-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:56.003717 sherpa-onnx-1.5.4/sherpa-onnx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:56.003717 sherpa-onnx-1.5.4/sherpa-onnx/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:56.003717 sherpa-onnx-1.5.4/sherpa-onnx/python/sherpa_onnx/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-21 10:38:55.000000 sherpa-onnx-1.5.4/sherpa-onnx/python/sherpa_onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-07-21 10:28:13.000000 sherpa-onnx-1.5.4/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-07-21 10:28:13.000000 sherpa-onnx-1.5.4/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-21 10:28:13.000000 sherpa-onnx-1.5.4/sherpa-onnx/python/sherpa_onnx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:56.003717 sherpa-onnx-1.5.4/sherpa_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-21 10:38:55.000000 sherpa-onnx-1.5.4/sherpa_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-21 10:38:55.000000 sherpa-onnx-1.5.4/sherpa_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:38:55.000000 sherpa-onnx-1.5.4/sherpa_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:38:55.000000 sherpa-onnx-1.5.4/sherpa_onnx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 10:38:55.000000 sherpa-onnx-1.5.4/sherpa_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-21 10:38:55.000000 sherpa-onnx-1.5.4/sherpa_onnx.egg-info/top_level.txt
```

### Comparing `sherpa-onnx-1.5.3/LICENSE` & `sherpa-onnx-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.5.3/PKG-INFO` & `sherpa-onnx-1.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.5.3
+Version: 1.5.4
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

### Comparing `sherpa-onnx-1.5.3/setup.py` & `sherpa-onnx-1.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.5.3/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py` & `sherpa-onnx-1.5.4/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.5.3/sherpa-onnx/python/sherpa_onnx/online_recognizer.py` & `sherpa-onnx-1.5.4/sherpa-onnx/python/sherpa_onnx/online_recognizer.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.5.3/sherpa-onnx/python/sherpa_onnx/utils.py` & `sherpa-onnx-1.5.4/sherpa-onnx/python/sherpa_onnx/utils.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.5.3/sherpa_onnx.egg-info/PKG-INFO` & `sherpa-onnx-1.5.4/sherpa_onnx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.5.3
+Version: 1.5.4
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

