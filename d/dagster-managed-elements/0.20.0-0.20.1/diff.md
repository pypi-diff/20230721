# Comparing `tmp/dagster-managed-elements-0.20.0.tar.gz` & `tmp/dagster-managed-elements-0.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-managed-elements-0.20.0.tar", last modified: Thu Jul 20 22:02:12 2023, max compression
+gzip compressed data, was "dagster-managed-elements-0.20.1.tar", last modified: Fri Jul 21 15:38:36 2023, max compression
```

## Comparing `dagster-managed-elements-0.20.0.tar` & `dagster-managed-elements-0.20.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:11.998216 dagster-managed-elements-0.20.0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-07-20 21:53:16.000000 dagster-managed-elements-0.20.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       76 2023-07-20 21:53:16.000000 dagster-managed-elements-0.20.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      636 2023-07-20 22:02:11.998216 dagster-managed-elements-0.20.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-20 21:53:16.000000 dagster-managed-elements-0.20.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:11.998216 dagster-managed-elements-0.20.0/dagster_managed_elements/
--rw-r--r--   0 root         (0) root         (0)      202 2023-07-20 21:53:16.000000 dagster-managed-elements-0.20.0/dagster_managed_elements/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6327 2023-07-20 21:53:16.000000 dagster-managed-elements-0.20.0/dagster_managed_elements/cli.py
--rw-r--r--   0 root         (0) root         (0)     9573 2023-07-20 21:53:16.000000 dagster-managed-elements-0.20.0/dagster_managed_elements/types.py
--rw-r--r--   0 root         (0) root         (0)     3357 2023-07-20 21:53:16.000000 dagster-managed-elements-0.20.0/dagster_managed_elements/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-managed-elements-0.20.0/dagster_managed_elements/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:11.998216 dagster-managed-elements-0.20.0/dagster_managed_elements.egg-info/
--rw-r--r--   0 root         (0) root         (0)      636 2023-07-20 22:02:11.000000 dagster-managed-elements-0.20.0/dagster_managed_elements.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      558 2023-07-20 22:02:11.000000 dagster-managed-elements-0.20.0/dagster_managed_elements.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:02:11.000000 dagster-managed-elements-0.20.0/dagster_managed_elements.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      126 2023-07-20 22:02:11.000000 dagster-managed-elements-0.20.0/dagster_managed_elements.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:02:11.000000 dagster-managed-elements-0.20.0/dagster_managed_elements.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 22:02:11.000000 dagster-managed-elements-0.20.0/dagster_managed_elements.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-20 22:02:11.000000 dagster-managed-elements-0.20.0/dagster_managed_elements.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      171 2023-07-20 22:02:12.002215 dagster-managed-elements-0.20.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1469 2023-07-20 21:53:16.000000 dagster-managed-elements-0.20.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:36.835142 dagster-managed-elements-0.20.1/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-21 15:29:00.000000 dagster-managed-elements-0.20.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       76 2023-07-21 15:29:00.000000 dagster-managed-elements-0.20.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      636 2023-07-21 15:38:36.835142 dagster-managed-elements-0.20.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-21 15:29:00.000000 dagster-managed-elements-0.20.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:36.831142 dagster-managed-elements-0.20.1/dagster_managed_elements/
+-rw-r--r--   0 root         (0) root         (0)      202 2023-07-21 15:29:00.000000 dagster-managed-elements-0.20.1/dagster_managed_elements/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6327 2023-07-21 15:29:00.000000 dagster-managed-elements-0.20.1/dagster_managed_elements/cli.py
+-rw-r--r--   0 root         (0) root         (0)     9573 2023-07-21 15:29:00.000000 dagster-managed-elements-0.20.1/dagster_managed_elements/types.py
+-rw-r--r--   0 root         (0) root         (0)     3357 2023-07-21 15:29:00.000000 dagster-managed-elements-0.20.1/dagster_managed_elements/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-21 15:29:00.000000 dagster-managed-elements-0.20.1/dagster_managed_elements/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:36.835142 dagster-managed-elements-0.20.1/dagster_managed_elements.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      636 2023-07-21 15:38:36.000000 dagster-managed-elements-0.20.1/dagster_managed_elements.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      558 2023-07-21 15:38:36.000000 dagster-managed-elements-0.20.1/dagster_managed_elements.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:38:36.000000 dagster-managed-elements-0.20.1/dagster_managed_elements.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      126 2023-07-21 15:38:36.000000 dagster-managed-elements-0.20.1/dagster_managed_elements.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:38:36.000000 dagster-managed-elements-0.20.1/dagster_managed_elements.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 15:38:36.000000 dagster-managed-elements-0.20.1/dagster_managed_elements.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-21 15:38:36.000000 dagster-managed-elements-0.20.1/dagster_managed_elements.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      171 2023-07-21 15:38:36.835142 dagster-managed-elements-0.20.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-07-21 15:29:00.000000 dagster-managed-elements-0.20.1/setup.py
```

### Comparing `dagster-managed-elements-0.20.0/LICENSE` & `dagster-managed-elements-0.20.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.20.0/PKG-INFO` & `dagster-managed-elements-0.20.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-managed-elements
-Version: 0.20.0
+Version: 0.20.1
 Summary: Package for Managed elements with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-managed-elements
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-managed-elements-0.20.0/dagster_managed_elements/cli.py` & `dagster-managed-elements-0.20.1/dagster_managed_elements/cli.py`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.20.0/dagster_managed_elements/types.py` & `dagster-managed-elements-0.20.1/dagster_managed_elements/types.py`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.20.0/dagster_managed_elements/utils.py` & `dagster-managed-elements-0.20.1/dagster_managed_elements/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.20.0/dagster_managed_elements.egg-info/PKG-INFO` & `dagster-managed-elements-0.20.1/dagster_managed_elements.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-managed-elements
-Version: 0.20.0
+Version: 0.20.1
 Summary: Package for Managed elements with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-managed-elements
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-managed-elements-0.20.0/dagster_managed_elements.egg-info/SOURCES.txt` & `dagster-managed-elements-0.20.1/dagster_managed_elements.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.20.0/setup.py` & `dagster-managed-elements-0.20.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_managed_elements_tests*"]),
-    install_requires=["dagster==1.4.0", "requests", "click_spinner"],
+    install_requires=["dagster==1.4.1", "requests", "click_spinner"],
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "dagster-managed-elements = dagster_managed_elements.cli:main",
             "dagster-me = dagster_managed_elements.cli:main",
         ]
     },
```

