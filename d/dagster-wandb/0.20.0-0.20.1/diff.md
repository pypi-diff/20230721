# Comparing `tmp/dagster-wandb-0.20.0.tar.gz` & `tmp/dagster-wandb-0.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-wandb-0.20.0.tar", last modified: Thu Jul 20 22:04:09 2023, max compression
+gzip compressed data, was "dagster-wandb-0.20.1.tar", last modified: Fri Jul 21 15:38:40 2023, max compression
```

## Comparing `dagster-wandb-0.20.0.tar` & `dagster-wandb-0.20.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:09.195850 dagster-wandb-0.20.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      629 2023-07-20 22:04:09.195850 dagster-wandb-0.20.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      150 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:09.191850 dagster-wandb-0.20.0/dagster_wandb/
--rw-r--r--   0 root         (0) root         (0)      613 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/dagster_wandb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34007 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/dagster_wandb/io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:09.191850 dagster-wandb-0.20.0/dagster_wandb/launch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/dagster_wandb/launch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4425 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/dagster_wandb/launch/configs.py
--rw-r--r--   0 root         (0) root         (0)     5192 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/dagster_wandb/launch/ops.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/dagster_wandb/py.typed
--rw-r--r--   0 root         (0) root         (0)     2272 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/dagster_wandb/resources.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/dagster_wandb/types.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/dagster_wandb/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:09.191850 dagster-wandb-0.20.0/dagster_wandb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      629 2023-07-20 22:04:09.000000 dagster-wandb-0.20.0/dagster_wandb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      513 2023-07-20 22:04:09.000000 dagster-wandb-0.20.0/dagster_wandb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:04:09.000000 dagster-wandb-0.20.0/dagster_wandb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:04:09.000000 dagster-wandb-0.20.0/dagster_wandb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       75 2023-07-20 22:04:09.000000 dagster-wandb-0.20.0/dagster_wandb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-20 22:04:09.000000 dagster-wandb-0.20.0/dagster_wandb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      160 2023-07-20 22:04:09.195850 dagster-wandb-0.20.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1319 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:40.355131 dagster-wandb-0.20.1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-21 15:29:00.000000 dagster-wandb-0.20.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-21 15:29:00.000000 dagster-wandb-0.20.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      629 2023-07-21 15:38:40.355131 dagster-wandb-0.20.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      150 2023-07-21 15:29:00.000000 dagster-wandb-0.20.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:40.351131 dagster-wandb-0.20.1/dagster_wandb/
+-rw-r--r--   0 root         (0) root         (0)      613 2023-07-21 15:29:00.000000 dagster-wandb-0.20.1/dagster_wandb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34007 2023-07-21 15:29:00.000000 dagster-wandb-0.20.1/dagster_wandb/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:40.355131 dagster-wandb-0.20.1/dagster_wandb/launch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 15:29:00.000000 dagster-wandb-0.20.1/dagster_wandb/launch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4425 2023-07-21 15:29:00.000000 dagster-wandb-0.20.1/dagster_wandb/launch/configs.py
+-rw-r--r--   0 root         (0) root         (0)     5192 2023-07-21 15:29:00.000000 dagster-wandb-0.20.1/dagster_wandb/launch/ops.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-21 15:29:00.000000 dagster-wandb-0.20.1/dagster_wandb/py.typed
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-07-21 15:29:00.000000 dagster-wandb-0.20.1/dagster_wandb/resources.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-21 15:29:00.000000 dagster-wandb-0.20.1/dagster_wandb/types.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-21 15:29:00.000000 dagster-wandb-0.20.1/dagster_wandb/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:40.355131 dagster-wandb-0.20.1/dagster_wandb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-07-21 15:38:40.000000 dagster-wandb-0.20.1/dagster_wandb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      513 2023-07-21 15:38:40.000000 dagster-wandb-0.20.1/dagster_wandb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:38:40.000000 dagster-wandb-0.20.1/dagster_wandb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:38:40.000000 dagster-wandb-0.20.1/dagster_wandb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       75 2023-07-21 15:38:40.000000 dagster-wandb-0.20.1/dagster_wandb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-21 15:38:40.000000 dagster-wandb-0.20.1/dagster_wandb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      160 2023-07-21 15:38:40.355131 dagster-wandb-0.20.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1319 2023-07-21 15:29:00.000000 dagster-wandb-0.20.1/setup.py
```

### Comparing `dagster-wandb-0.20.0/LICENSE` & `dagster-wandb-0.20.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.20.0/PKG-INFO` & `dagster-wandb-0.20.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-wandb
-Version: 0.20.0
+Version: 0.20.1
 Summary: Package for wandb Dagster components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-wandb
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-wandb-0.20.0/dagster_wandb/__init__.py` & `dagster-wandb-0.20.1/dagster_wandb/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.20.0/dagster_wandb/io_manager.py` & `dagster-wandb-0.20.1/dagster_wandb/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.20.0/dagster_wandb/launch/configs.py` & `dagster-wandb-0.20.1/dagster_wandb/launch/configs.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.20.0/dagster_wandb/launch/ops.py` & `dagster-wandb-0.20.1/dagster_wandb/launch/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.20.0/dagster_wandb/resources.py` & `dagster-wandb-0.20.1/dagster_wandb/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.20.0/dagster_wandb/types.py` & `dagster-wandb-0.20.1/dagster_wandb/types.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.20.0/dagster_wandb.egg-info/PKG-INFO` & `dagster-wandb-0.20.1/dagster_wandb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-wandb
-Version: 0.20.0
+Version: 0.20.1
 Summary: Package for wandb Dagster components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-wandb
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-wandb-0.20.0/dagster_wandb.egg-info/SOURCES.txt` & `dagster-wandb-0.20.1/dagster_wandb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.20.0/setup.py` & `dagster-wandb-0.20.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,13 +29,13 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_wandb_tests*"]),
     install_requires=[
-        "dagster==1.4.0",
+        "dagster==1.4.1",
         "wandb>=0.13.5,<0.15.4",
     ],
     extras_require={"dev": ["cloudpickle", "joblib", "callee", "dill"]},
     zip_safe=False,
 )
```

