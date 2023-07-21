# Comparing `tmp/gasearch-0.0.4.tar.gz` & `tmp/gasearch-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gasearch-0.0.4.tar", last modified: Sun Jul 16 12:13:12 2023, max compression
+gzip compressed data, was "gasearch-0.0.5.tar", last modified: Fri Jul 21 14:40:24 2023, max compression
```

## Comparing `gasearch-0.0.4.tar` & `gasearch-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 jpodivin  (1000) jpodivin  (1000)        0 2023-07-16 12:13:12.824277 gasearch-0.0.4/
--rw-rw-r--   0 jpodivin  (1000) jpodivin  (1000)     1523 2023-07-01 12:25:02.000000 gasearch-0.0.4/LICENSE
--rw-rw-r--   0 jpodivin  (1000) jpodivin  (1000)       25 2023-06-24 10:23:12.000000 gasearch-0.0.4/MANIFEST.in
--rw-rw-r--   0 jpodivin  (1000) jpodivin  (1000)     2600 2023-07-16 12:13:12.824277 gasearch-0.0.4/PKG-INFO
--rw-rw-r--   0 jpodivin  (1000) jpodivin  (1000)     1447 2023-07-16 11:39:44.000000 gasearch-0.0.4/README.rst
-drwxrwxr-x   0 jpodivin  (1000) jpodivin  (1000)        0 2023-07-16 12:13:12.824277 gasearch-0.0.4/gasearch.egg-info/
--rw-rw-r--   0 jpodivin  (1000) jpodivin  (1000)     2600 2023-07-16 12:13:12.000000 gasearch-0.0.4/gasearch.egg-info/PKG-INFO
--rw-rw-r--   0 jpodivin  (1000) jpodivin  (1000)      448 2023-07-16 12:13:12.000000 gasearch-0.0.4/gasearch.egg-info/SOURCES.txt
--rw-rw-r--   0 jpodivin  (1000) jpodivin  (1000)        1 2023-07-16 12:13:12.000000 gasearch-0.0.4/gasearch.egg-info/dependency_links.txt
--rw-rw-r--   0 jpodivin  (1000) jpodivin  (1000)        1 2023-07-16 12:13:12.000000 gasearch-0.0.4/gasearch.egg-info/not-zip-safe
--rw-rw-r--   0 jpodivin  (1000) jpodivin  (1000)      119 2023-07-16 12:13:12.000000 gasearch-0.0.4/gasearch.egg-info/requires.txt
--rw-rw-r--   0 jpodivin  (1000) jpodivin  (1000)       16 2023-07-16 12:13:12.000000 gasearch-0.0.4/gasearch.egg-info/top_level.txt
-drwxrwxr-x   0 jpodivin  (1000) jpodivin  (1000)        0 2023-07-16 12:13:12.824277 gasearch-0.0.4/geneticsearchcv/
--rw-rw-r--   0 jpodivin  (1000) jpodivin  (1000)      137 2023-07-08 14:26:22.000000 gasearch-0.0.4/geneticsearchcv/__init__.py
--rw-rw-r--   0 jpodivin  (1000) jpodivin  (1000)    18206 2023-07-08 14:26:22.000000 gasearch-0.0.4/geneticsearchcv/_search.py
--rw-rw-r--   0 jpodivin  (1000) jpodivin  (1000)       22 2023-07-16 11:52:27.000000 gasearch-0.0.4/geneticsearchcv/_version.py
-drwxrwxr-x   0 jpodivin  (1000) jpodivin  (1000)        0 2023-07-16 12:13:12.824277 gasearch-0.0.4/geneticsearchcv/tests/
--rw-rw-r--   0 jpodivin  (1000) jpodivin  (1000)        0 2023-07-02 14:11:31.000000 gasearch-0.0.4/geneticsearchcv/tests/__init__.py
--rw-rw-r--   0 jpodivin  (1000) jpodivin  (1000)     1440 2023-07-08 14:26:22.000000 gasearch-0.0.4/geneticsearchcv/tests/test_common.py
--rw-rw-r--   0 jpodivin  (1000) jpodivin  (1000)      646 2023-07-08 14:26:22.000000 gasearch-0.0.4/geneticsearchcv/tests/test_mutator.py
--rw-rw-r--   0 jpodivin  (1000) jpodivin  (1000)       69 2023-07-08 15:08:15.000000 gasearch-0.0.4/requirements.txt
--rw-rw-r--   0 jpodivin  (1000) jpodivin  (1000)      186 2023-07-16 12:13:12.824277 gasearch-0.0.4/setup.cfg
--rw-rw-r--   0 jpodivin  (1000) jpodivin  (1000)     2282 2023-07-16 12:13:00.000000 gasearch-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:40:24.487015 gasearch-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-21 14:40:14.000000 gasearch-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-21 14:40:14.000000 gasearch-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-21 14:40:24.487015 gasearch-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-21 14:40:14.000000 gasearch-0.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:40:24.487015 gasearch-0.0.5/gasearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-21 14:40:24.000000 gasearch-0.0.5/gasearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-21 14:40:24.000000 gasearch-0.0.5/gasearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:40:24.000000 gasearch-0.0.5/gasearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:40:24.000000 gasearch-0.0.5/gasearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-21 14:40:24.000000 gasearch-0.0.5/gasearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 14:40:24.000000 gasearch-0.0.5/gasearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:40:24.487015 gasearch-0.0.5/geneticsearchcv/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-21 14:40:14.000000 gasearch-0.0.5/geneticsearchcv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-07-21 14:40:14.000000 gasearch-0.0.5/geneticsearchcv/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 14:40:14.000000 gasearch-0.0.5/geneticsearchcv/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:40:24.487015 gasearch-0.0.5/geneticsearchcv/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 14:40:14.000000 gasearch-0.0.5/geneticsearchcv/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-21 14:40:14.000000 gasearch-0.0.5/geneticsearchcv/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-21 14:40:14.000000 gasearch-0.0.5/geneticsearchcv/tests/test_mutator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-21 14:40:14.000000 gasearch-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-21 14:40:24.487015 gasearch-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-21 14:40:14.000000 gasearch-0.0.5/setup.py
```

### Comparing `gasearch-0.0.4/LICENSE` & `gasearch-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gasearch-0.0.4/PKG-INFO` & `gasearch-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gasearch
-Version: 0.0.4
+Version: 0.0.5
 Summary: Genetic algorithm based hyperparameter optimalization.
 Home-page: https://github.com/jpodivin/geneticsearchcv
 Download-URL: https://github.com/jpodivin/geneticsearchcv
 Maintainer: Jiri Podivin
 Maintainer-email: jpodivin@logosgen.net
 License: new BSD
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gasearch-0.0.4/README.rst` & `gasearch-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `gasearch-0.0.4/gasearch.egg-info/PKG-INFO` & `gasearch-0.0.5/gasearch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gasearch
-Version: 0.0.4
+Version: 0.0.5
 Summary: Genetic algorithm based hyperparameter optimalization.
 Home-page: https://github.com/jpodivin/geneticsearchcv
 Download-URL: https://github.com/jpodivin/geneticsearchcv
 Maintainer: Jiri Podivin
 Maintainer-email: jpodivin@logosgen.net
 License: new BSD
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gasearch-0.0.4/geneticsearchcv/_search.py` & `gasearch-0.0.5/geneticsearchcv/_search.py`

 * *Files identical despite different names*

### Comparing `gasearch-0.0.4/geneticsearchcv/tests/test_common.py` & `gasearch-0.0.5/geneticsearchcv/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `gasearch-0.0.4/geneticsearchcv/tests/test_mutator.py` & `gasearch-0.0.5/geneticsearchcv/tests/test_mutator.py`

 * *Files identical despite different names*

### Comparing `gasearch-0.0.4/setup.py` & `gasearch-0.0.5/setup.py`

 * *Files identical despite different names*

