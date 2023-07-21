# Comparing `tmp/dagster-datahub-0.20.0.tar.gz` & `tmp/dagster-datahub-0.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-datahub-0.20.0.tar", last modified: Thu Jul 20 22:01:03 2023, max compression
+gzip compressed data, was "dagster-datahub-0.20.1.tar", last modified: Fri Jul 21 15:37:00 2023, max compression
```

## Comparing `dagster-datahub-0.20.0.tar` & `dagster-datahub-0.20.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:01:03.197237 dagster-datahub-0.20.0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-07-20 21:53:16.000000 dagster-datahub-0.20.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      214 2023-07-20 21:53:16.000000 dagster-datahub-0.20.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      653 2023-07-20 22:01:03.197237 dagster-datahub-0.20.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2023-07-20 21:53:16.000000 dagster-datahub-0.20.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:01:03.197237 dagster-datahub-0.20.0/dagster_datahub/
--rw-r--r--   0 root         (0) root         (0)      492 2023-07-20 21:53:16.000000 dagster-datahub-0.20.0/dagster_datahub/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:16.000000 dagster-datahub-0.20.0/dagster_datahub/py.typed
--rw-r--r--   0 root         (0) root         (0)     4242 2023-07-20 21:53:16.000000 dagster-datahub-0.20.0/dagster_datahub/resources.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-datahub-0.20.0/dagster_datahub/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:01:03.197237 dagster-datahub-0.20.0/dagster_datahub.egg-info/
--rw-r--r--   0 root         (0) root         (0)      653 2023-07-20 22:01:03.000000 dagster-datahub-0.20.0/dagster_datahub.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-07-20 22:01:03.000000 dagster-datahub-0.20.0/dagster_datahub.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:01:03.000000 dagster-datahub-0.20.0/dagster_datahub.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:01:03.000000 dagster-datahub-0.20.0/dagster_datahub.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       84 2023-07-20 22:01:03.000000 dagster-datahub-0.20.0/dagster_datahub.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-20 22:01:03.000000 dagster-datahub-0.20.0/dagster_datahub.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2023-07-20 22:01:03.197237 dagster-datahub-0.20.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1424 2023-07-20 21:53:16.000000 dagster-datahub-0.20.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:37:00.503431 dagster-datahub-0.20.1/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-21 15:29:00.000000 dagster-datahub-0.20.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      214 2023-07-21 15:29:00.000000 dagster-datahub-0.20.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      653 2023-07-21 15:37:00.503431 dagster-datahub-0.20.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2023-07-21 15:29:00.000000 dagster-datahub-0.20.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:37:00.499431 dagster-datahub-0.20.1/dagster_datahub/
+-rw-r--r--   0 root         (0) root         (0)      492 2023-07-21 15:29:00.000000 dagster-datahub-0.20.1/dagster_datahub/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 15:29:00.000000 dagster-datahub-0.20.1/dagster_datahub/py.typed
+-rw-r--r--   0 root         (0) root         (0)     4242 2023-07-21 15:29:00.000000 dagster-datahub-0.20.1/dagster_datahub/resources.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-21 15:29:00.000000 dagster-datahub-0.20.1/dagster_datahub/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:37:00.499431 dagster-datahub-0.20.1/dagster_datahub.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      653 2023-07-21 15:37:00.000000 dagster-datahub-0.20.1/dagster_datahub.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-07-21 15:37:00.000000 dagster-datahub-0.20.1/dagster_datahub.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:37:00.000000 dagster-datahub-0.20.1/dagster_datahub.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:37:00.000000 dagster-datahub-0.20.1/dagster_datahub.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       84 2023-07-21 15:37:00.000000 dagster-datahub-0.20.1/dagster_datahub.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-21 15:37:00.000000 dagster-datahub-0.20.1/dagster_datahub.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2023-07-21 15:37:00.503431 dagster-datahub-0.20.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1424 2023-07-21 15:29:00.000000 dagster-datahub-0.20.1/setup.py
```

### Comparing `dagster-datahub-0.20.0/LICENSE` & `dagster-datahub-0.20.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-datahub-0.20.0/PKG-INFO` & `dagster-datahub-0.20.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-datahub
-Version: 0.20.0
+Version: 0.20.1
 Summary: Package for Datahub-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-datahub
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-datahub-0.20.0/dagster_datahub/resources.py` & `dagster-datahub-0.20.1/dagster_datahub/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-datahub-0.20.0/dagster_datahub.egg-info/PKG-INFO` & `dagster-datahub-0.20.1/dagster_datahub.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-datahub
-Version: 0.20.0
+Version: 0.20.1
 Summary: Package for Datahub-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-datahub
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-datahub-0.20.0/setup.py` & `dagster-datahub-0.20.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,14 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_datahub_tests*"]),
     include_package_data=True,
     install_requires=[
         "acryl-datahub[datahub-rest, datahub-kafka]<=0.10.2",
-        "dagster==1.4.0",
+        "dagster==1.4.1",
         "packaging",
         "requests",
     ],
     extras_require={},
     zip_safe=False,
 )
```

