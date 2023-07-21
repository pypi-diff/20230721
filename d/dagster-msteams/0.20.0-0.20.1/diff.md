# Comparing `tmp/dagster-msteams-0.20.0.tar.gz` & `tmp/dagster-msteams-0.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-msteams-0.20.0.tar", last modified: Thu Jul 20 22:03:37 2023, max compression
+gzip compressed data, was "dagster-msteams-0.20.1.tar", last modified: Fri Jul 21 15:38:07 2023, max compression
```

## Comparing `dagster-msteams-0.20.0.tar` & `dagster-msteams-0.20.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:03:37.847404 dagster-msteams-0.20.0/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       66 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      640 2023-07-20 22:03:37.847404 dagster-msteams-0.20.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:03:37.847404 dagster-msteams-0.20.0/dagster_msteams/
--rw-r--r--   0 root         (0) root         (0)      510 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/dagster_msteams/__init__.py
--rw-r--r--   0 root         (0) root         (0)      849 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/dagster_msteams/card.py
--rw-r--r--   0 root         (0) root         (0)     1389 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/dagster_msteams/client.py
--rw-r--r--   0 root         (0) root         (0)     3881 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/dagster_msteams/hooks.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/dagster_msteams/py.typed
--rw-r--r--   0 root         (0) root         (0)     3751 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/dagster_msteams/resources.py
--rw-r--r--   0 root         (0) root         (0)     5213 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/dagster_msteams/sensors.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/dagster_msteams/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:03:37.847404 dagster-msteams-0.20.0/dagster_msteams.egg-info/
--rw-r--r--   0 root         (0) root         (0)      640 2023-07-20 22:03:37.000000 dagster-msteams-0.20.0/dagster_msteams.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      491 2023-07-20 22:03:37.000000 dagster-msteams-0.20.0/dagster_msteams.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:03:37.000000 dagster-msteams-0.20.0/dagster_msteams.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:03:37.000000 dagster-msteams-0.20.0/dagster_msteams.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       30 2023-07-20 22:03:37.000000 dagster-msteams-0.20.0/dagster_msteams.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-20 22:03:37.000000 dagster-msteams-0.20.0/dagster_msteams.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2023-07-20 22:03:37.847404 dagster-msteams-0.20.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1243 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:07.151232 dagster-msteams-0.20.1/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-07-21 15:29:00.000000 dagster-msteams-0.20.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-21 15:29:00.000000 dagster-msteams-0.20.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      640 2023-07-21 15:38:07.151232 dagster-msteams-0.20.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2023-07-21 15:29:00.000000 dagster-msteams-0.20.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:07.151232 dagster-msteams-0.20.1/dagster_msteams/
+-rw-r--r--   0 root         (0) root         (0)      510 2023-07-21 15:29:00.000000 dagster-msteams-0.20.1/dagster_msteams/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      849 2023-07-21 15:29:00.000000 dagster-msteams-0.20.1/dagster_msteams/card.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-07-21 15:29:00.000000 dagster-msteams-0.20.1/dagster_msteams/client.py
+-rw-r--r--   0 root         (0) root         (0)     3881 2023-07-21 15:29:00.000000 dagster-msteams-0.20.1/dagster_msteams/hooks.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-21 15:29:00.000000 dagster-msteams-0.20.1/dagster_msteams/py.typed
+-rw-r--r--   0 root         (0) root         (0)     3751 2023-07-21 15:29:00.000000 dagster-msteams-0.20.1/dagster_msteams/resources.py
+-rw-r--r--   0 root         (0) root         (0)     5213 2023-07-21 15:29:00.000000 dagster-msteams-0.20.1/dagster_msteams/sensors.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-21 15:29:00.000000 dagster-msteams-0.20.1/dagster_msteams/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:07.151232 dagster-msteams-0.20.1/dagster_msteams.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      640 2023-07-21 15:38:07.000000 dagster-msteams-0.20.1/dagster_msteams.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      491 2023-07-21 15:38:07.000000 dagster-msteams-0.20.1/dagster_msteams.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:38:07.000000 dagster-msteams-0.20.1/dagster_msteams.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:38:07.000000 dagster-msteams-0.20.1/dagster_msteams.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-21 15:38:07.000000 dagster-msteams-0.20.1/dagster_msteams.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-21 15:38:07.000000 dagster-msteams-0.20.1/dagster_msteams.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2023-07-21 15:38:07.155232 dagster-msteams-0.20.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-07-21 15:29:00.000000 dagster-msteams-0.20.1/setup.py
```

### Comparing `dagster-msteams-0.20.0/LICENSE` & `dagster-msteams-0.20.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.20.0/PKG-INFO` & `dagster-msteams-0.20.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-msteams
-Version: 0.20.0
+Version: 0.20.1
 Summary: A Microsoft Teams client resource for posting to Microsoft Teams
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-msteams
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-msteams-0.20.0/dagster_msteams/card.py` & `dagster-msteams-0.20.1/dagster_msteams/card.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.20.0/dagster_msteams/client.py` & `dagster-msteams-0.20.1/dagster_msteams/client.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.20.0/dagster_msteams/hooks.py` & `dagster-msteams-0.20.1/dagster_msteams/hooks.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.20.0/dagster_msteams/resources.py` & `dagster-msteams-0.20.1/dagster_msteams/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.20.0/dagster_msteams/sensors.py` & `dagster-msteams-0.20.1/dagster_msteams/sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.20.0/dagster_msteams.egg-info/PKG-INFO` & `dagster-msteams-0.20.1/dagster_msteams.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-msteams
-Version: 0.20.0
+Version: 0.20.1
 Summary: A Microsoft Teams client resource for posting to Microsoft Teams
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-msteams
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-msteams-0.20.0/setup.py` & `dagster-msteams-0.20.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,12 +30,12 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_msteams_tests*"]),
     install_requires=[
-        "dagster==1.4.0",
+        "dagster==1.4.1",
         "requests>=2,<3",
     ],
     zip_safe=False,
 )
```

