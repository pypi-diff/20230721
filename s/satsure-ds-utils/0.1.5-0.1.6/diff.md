# Comparing `tmp/satsure-ds-utils-0.1.5.tar.gz` & `tmp/satsure-ds-utils-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsure-ds-utils-0.1.5.tar", last modified: Thu Jul  6 06:20:41 2023, max compression
+gzip compressed data, was "satsure-ds-utils-0.1.6.tar", last modified: Fri Jul 21 09:01:16 2023, max compression
```

## Comparing `satsure-ds-utils-0.1.5.tar` & `satsure-ds-utils-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 divinity  (1000) divinity  (1000)        0 2023-07-06 06:20:41.602032 satsure-ds-utils-0.1.5/
--rw-rw-r--   0 divinity  (1000) divinity  (1000)     1190 2023-07-06 06:20:41.602032 satsure-ds-utils-0.1.5/PKG-INFO
--rw-rw-r--   0 divinity  (1000) divinity  (1000)      510 2023-07-06 05:28:22.000000 satsure-ds-utils-0.1.5/README.md
-drwxrwxr-x   0 divinity  (1000) divinity  (1000)        0 2023-07-06 06:20:41.602032 satsure-ds-utils-0.1.5/satsure_ds_utils.egg-info/
--rw-rw-r--   0 divinity  (1000) divinity  (1000)     1190 2023-07-06 06:20:41.000000 satsure-ds-utils-0.1.5/satsure_ds_utils.egg-info/PKG-INFO
--rw-rw-r--   0 divinity  (1000) divinity  (1000)      217 2023-07-06 06:20:41.000000 satsure-ds-utils-0.1.5/satsure_ds_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 divinity  (1000) divinity  (1000)        1 2023-07-06 06:20:41.000000 satsure-ds-utils-0.1.5/satsure_ds_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 divinity  (1000) divinity  (1000)       51 2023-07-06 06:20:41.000000 satsure-ds-utils-0.1.5/satsure_ds_utils.egg-info/requires.txt
--rw-rw-r--   0 divinity  (1000) divinity  (1000)       17 2023-07-06 06:20:41.000000 satsure-ds-utils-0.1.5/satsure_ds_utils.egg-info/top_level.txt
--rw-rw-r--   0 divinity  (1000) divinity  (1000)       38 2023-07-06 06:20:41.602032 satsure-ds-utils-0.1.5/setup.cfg
--rw-rw-r--   0 divinity  (1000) divinity  (1000)     1207 2023-07-06 06:20:32.000000 satsure-ds-utils-0.1.5/setup.py
+drwxrwxr-x   0 divinity  (1000) divinity  (1000)        0 2023-07-21 09:01:16.277849 satsure-ds-utils-0.1.6/
+-rw-rw-r--   0 divinity  (1000) divinity  (1000)     1190 2023-07-21 09:01:16.277849 satsure-ds-utils-0.1.6/PKG-INFO
+-rw-rw-r--   0 divinity  (1000) divinity  (1000)      510 2023-07-06 05:28:22.000000 satsure-ds-utils-0.1.6/README.md
+drwxrwxr-x   0 divinity  (1000) divinity  (1000)        0 2023-07-21 09:01:16.277849 satsure-ds-utils-0.1.6/satsure_ds_utils.egg-info/
+-rw-rw-r--   0 divinity  (1000) divinity  (1000)     1190 2023-07-21 09:01:16.000000 satsure-ds-utils-0.1.6/satsure_ds_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 divinity  (1000) divinity  (1000)      217 2023-07-21 09:01:16.000000 satsure-ds-utils-0.1.6/satsure_ds_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 divinity  (1000) divinity  (1000)        1 2023-07-21 09:01:16.000000 satsure-ds-utils-0.1.6/satsure_ds_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 divinity  (1000) divinity  (1000)       51 2023-07-21 09:01:16.000000 satsure-ds-utils-0.1.6/satsure_ds_utils.egg-info/requires.txt
+-rw-rw-r--   0 divinity  (1000) divinity  (1000)       17 2023-07-21 09:01:16.000000 satsure-ds-utils-0.1.6/satsure_ds_utils.egg-info/top_level.txt
+-rw-rw-r--   0 divinity  (1000) divinity  (1000)       38 2023-07-21 09:01:16.277849 satsure-ds-utils-0.1.6/setup.cfg
+-rw-rw-r--   0 divinity  (1000) divinity  (1000)     1207 2023-07-21 08:55:09.000000 satsure-ds-utils-0.1.6/setup.py
```

### Comparing `satsure-ds-utils-0.1.5/PKG-INFO` & `satsure-ds-utils-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsure-ds-utils
-Version: 0.1.5
+Version: 0.1.6
 Summary: Common Utilities for SatSure Data Science Team.
 Home-page: https://satsure-ds-utils.readthedocs.io/
 Author: SatSure DS Team
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `satsure-ds-utils-0.1.5/satsure_ds_utils.egg-info/PKG-INFO` & `satsure-ds-utils-0.1.6/satsure_ds_utils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsure-ds-utils
-Version: 0.1.5
+Version: 0.1.6
 Summary: Common Utilities for SatSure Data Science Team.
 Home-page: https://satsure-ds-utils.readthedocs.io/
 Author: SatSure DS Team
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `satsure-ds-utils-0.1.5/setup.py` & `satsure-ds-utils-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 NAME = path.abspath(path.dirname(__file__))
 
 with open(path.join(NAME, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="satsure-ds-utils",
-    version="0.1.5",
+    version="0.1.6",
     description="Common Utilities for SatSure Data Science Team.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://satsure-ds-utils.readthedocs.io/",
     author="SatSure DS Team",
     license="MIT",
     classifiers=[
```

