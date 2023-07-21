# Comparing `tmp/dagit-1.4.0.tar.gz` & `tmp/dagit-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagit-1.4.0.tar", last modified: Thu Jul 20 21:54:00 2023, max compression
+gzip compressed data, was "dagit-1.4.1.tar", last modified: Fri Jul 21 15:29:28 2023, max compression
```

## Comparing `dagit-1.4.0.tar` & `dagit-1.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:54:00.583123 dagit-1.4.0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-07-20 21:53:15.000000 dagit-1.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       58 2023-07-20 21:53:15.000000 dagit-1.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      828 2023-07-20 21:54:00.583123 dagit-1.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      210 2023-07-20 21:53:15.000000 dagit-1.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:54:00.583123 dagit-1.4.0/dagit/
--rw-r--r--   0 root         (0) root         (0)      148 2023-07-20 21:53:15.000000 dagit-1.4.0/dagit/__init__.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-20 21:53:15.000000 dagit-1.4.0/dagit/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 21:54:00.583123 dagit-1.4.0/dagit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      828 2023-07-20 21:54:00.000000 dagit-1.4.0/dagit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      260 2023-07-20 21:54:00.000000 dagit-1.4.0/dagit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 21:54:00.000000 dagit-1.4.0/dagit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       96 2023-07-20 21:54:00.000000 dagit-1.4.0/dagit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      111 2023-07-20 21:54:00.000000 dagit-1.4.0/dagit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-07-20 21:54:00.000000 dagit-1.4.0/dagit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      153 2023-07-20 21:54:00.583123 dagit-1.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1727 2023-07-20 21:53:15.000000 dagit-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:29:28.096771 dagit-1.4.1/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-21 15:29:00.000000 dagit-1.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       58 2023-07-21 15:29:00.000000 dagit-1.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      828 2023-07-21 15:29:28.096771 dagit-1.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      210 2023-07-21 15:29:00.000000 dagit-1.4.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:29:28.092771 dagit-1.4.1/dagit/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-21 15:29:00.000000 dagit-1.4.1/dagit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 15:29:00.000000 dagit-1.4.1/dagit/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:29:28.096771 dagit-1.4.1/dagit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      828 2023-07-21 15:29:28.000000 dagit-1.4.1/dagit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      260 2023-07-21 15:29:28.000000 dagit-1.4.1/dagit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:29:28.000000 dagit-1.4.1/dagit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2023-07-21 15:29:28.000000 dagit-1.4.1/dagit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      111 2023-07-21 15:29:28.000000 dagit-1.4.1/dagit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-21 15:29:28.000000 dagit-1.4.1/dagit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      153 2023-07-21 15:29:28.096771 dagit-1.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-07-21 15:29:00.000000 dagit-1.4.1/setup.py
```

### Comparing `dagit-1.4.0/LICENSE` & `dagit-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagit-1.4.0/PKG-INFO` & `dagit-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagit
-Version: 1.4.0
+Version: 1.4.1
 Summary: Web UI for dagster.
 Home-page: https://github.com/dagster-io/dagster
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagit-1.4.0/dagit.egg-info/PKG-INFO` & `dagit-1.4.1/dagit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagit
-Version: 1.4.0
+Version: 1.4.1
 Summary: Web UI for dagster.
 Home-page: https://github.com/dagster-io/dagster
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagit-1.4.0/setup.py` & `dagit-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagit_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster-webserver==1.4.0",
+        "dagster-webserver==1.4.1",
     ],
     extras_require={
         "notebook": [f"dagster-webserver[notebook]{pin}"],  # notebooks support
         "test": [f"dagster-webserver[test]{pin}"],  # TestClient deps in full
     },
     entry_points={
         "console_scripts": [
```

