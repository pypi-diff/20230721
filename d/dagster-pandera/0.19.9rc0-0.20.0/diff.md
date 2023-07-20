# Comparing `tmp/dagster-pandera-0.19.9rc0.tar.gz` & `tmp/dagster-pandera-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-pandera-0.19.9rc0.tar", last modified: Thu Jun  8 18:31:06 2023, max compression
+gzip compressed data, was "dagster-pandera-0.20.0.tar", last modified: Thu Jul 20 22:01:49 2023, max compression
```

## Comparing `dagster-pandera-0.19.9rc0.tar` & `dagster-pandera-0.20.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:06.229002 dagster-pandera-0.19.9rc0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-pandera-0.19.9rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-08 18:20:46.000000 dagster-pandera-0.19.9rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      639 2023-06-08 18:31:06.229002 dagster-pandera-0.19.9rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2023-06-08 18:20:46.000000 dagster-pandera-0.19.9rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:06.229002 dagster-pandera-0.19.9rc0/dagster_pandera/
--rw-r--r--   0 root         (0) root         (0)     9258 2023-06-08 18:20:46.000000 dagster-pandera-0.19.9rc0/dagster_pandera/__init__.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 18:20:46.000000 dagster-pandera-0.19.9rc0/dagster_pandera/py.typed
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-pandera-0.19.9rc0/dagster_pandera/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:06.229002 dagster-pandera-0.19.9rc0/dagster_pandera.egg-info/
--rw-r--r--   0 root         (0) root         (0)      639 2023-06-08 18:31:06.000000 dagster-pandera-0.19.9rc0/dagster_pandera.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      322 2023-06-08 18:31:06.000000 dagster-pandera-0.19.9rc0/dagster_pandera.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:31:06.000000 dagster-pandera-0.19.9rc0/dagster_pandera.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-06-08 18:31:06.000000 dagster-pandera-0.19.9rc0/dagster_pandera.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-08 18:31:06.000000 dagster-pandera-0.19.9rc0/dagster_pandera.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-08 18:31:06.229002 dagster-pandera-0.19.9rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1319 2023-06-08 18:20:46.000000 dagster-pandera-0.19.9rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:01:49.305895 dagster-pandera-0.20.0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-20 21:53:16.000000 dagster-pandera-0.20.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       67 2023-07-20 21:53:16.000000 dagster-pandera-0.20.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      586 2023-07-20 22:01:49.305895 dagster-pandera-0.20.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2023-07-20 21:53:16.000000 dagster-pandera-0.20.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:01:49.305895 dagster-pandera-0.20.0/dagster_pandera/
+-rw-r--r--   0 root         (0) root         (0)     9258 2023-07-20 21:53:16.000000 dagster-pandera-0.20.0/dagster_pandera/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-20 21:53:16.000000 dagster-pandera-0.20.0/dagster_pandera/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-pandera-0.20.0/dagster_pandera/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:01:49.305895 dagster-pandera-0.20.0/dagster_pandera.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      586 2023-07-20 22:01:49.000000 dagster-pandera-0.20.0/dagster_pandera.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-20 22:01:49.000000 dagster-pandera-0.20.0/dagster_pandera.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:01:49.000000 dagster-pandera-0.20.0/dagster_pandera.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-20 22:01:49.000000 dagster-pandera-0.20.0/dagster_pandera.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-20 22:01:49.000000 dagster-pandera-0.20.0/dagster_pandera.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2023-07-20 22:01:49.309895 dagster-pandera-0.20.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1267 2023-07-20 21:53:16.000000 dagster-pandera-0.20.0/setup.py
```

### Comparing `dagster-pandera-0.19.9rc0/LICENSE` & `dagster-pandera-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-pandera-0.19.9rc0/PKG-INFO` & `dagster-pandera-0.20.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-pandera
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Integration layer for dagster and pandera.
 Home-page: https://github.com/dagster-io/dagster
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Provides-Extra: test
```

### Comparing `dagster-pandera-0.19.9rc0/dagster_pandera/__init__.py` & `dagster-pandera-0.20.0/dagster_pandera/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-pandera-0.19.9rc0/dagster_pandera.egg-info/PKG-INFO` & `dagster-pandera-0.20.0/dagster_pandera.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-pandera
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Integration layer for dagster and pandera.
 Home-page: https://github.com/dagster-io/dagster
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Provides-Extra: test
```

### Comparing `dagster-pandera-0.19.9rc0/setup.py` & `dagster-pandera-0.20.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,24 +20,23 @@
     version=ver,
     author="Elementl",
     author_email="hello@elementl.com",
     license="Apache-2.0",
     description="Integration layer for dagster and pandera.",
     url="https://github.com/dagster-io/dagster",
     classifiers=[
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_pandera_tests*"]),
     include_package_data=True,
-    install_requires=["dagster==1.3.9rc0", "pandas", "pandera>=0.14.2"],
+    install_requires=["dagster==1.4.0", "pandas", "pandera>=0.14.2"],
     extras_require={
         "test": [
             "pytest",
         ],
     },
 )
```

