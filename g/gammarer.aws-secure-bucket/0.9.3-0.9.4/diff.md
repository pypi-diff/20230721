# Comparing `tmp/gammarer.aws-secure-bucket-0.9.3.tar.gz` & `tmp/gammarer.aws-secure-bucket-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-secure-bucket-0.9.3.tar", last modified: Thu Jul 20 17:24:13 2023, max compression
+gzip compressed data, was "gammarer.aws-secure-bucket-0.9.4.tar", last modified: Fri Jul 21 17:23:47 2023, max compression
```

## Comparing `gammarer.aws-secure-bucket-0.9.3.tar` & `gammarer.aws-secure-bucket-0.9.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:13.871467 gammarer.aws-secure-bucket-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-20 17:23:58.000000 gammarer.aws-secure-bucket-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 17:23:58.000000 gammarer.aws-secure-bucket-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-20 17:24:13.871467 gammarer.aws-secure-bucket-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-20 17:23:58.000000 gammarer.aws-secure-bucket-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-20 17:23:58.000000 gammarer.aws-secure-bucket-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 17:24:13.871467 gammarer.aws-secure-bucket-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-20 17:23:58.000000 gammarer.aws-secure-bucket-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:13.867467 gammarer.aws-secure-bucket-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:13.867467 gammarer.aws-secure-bucket-0.9.3/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:13.867467 gammarer.aws-secure-bucket-0.9.3/src/gammarer/aws_secure_bucket/
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-07-20 17:23:58.000000 gammarer.aws-secure-bucket-0.9.3/src/gammarer/aws_secure_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:13.867467 gammarer.aws-secure-bucket-0.9.3/src/gammarer/aws_secure_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-20 17:23:58.000000 gammarer.aws-secure-bucket-0.9.3/src/gammarer/aws_secure_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30734 2023-07-20 17:23:58.000000 gammarer.aws-secure-bucket-0.9.3/src/gammarer/aws_secure_bucket/_jsii/aws-secure-bucket@0.9.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:23:58.000000 gammarer.aws-secure-bucket-0.9.3/src/gammarer/aws_secure_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:13.867467 gammarer.aws-secure-bucket-0.9.3/src/gammarer.aws_secure_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-20 17:24:13.000000 gammarer.aws-secure-bucket-0.9.3/src/gammarer.aws_secure_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-20 17:24:13.000000 gammarer.aws-secure-bucket-0.9.3/src/gammarer.aws_secure_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:24:13.000000 gammarer.aws-secure-bucket-0.9.3/src/gammarer.aws_secure_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-20 17:24:13.000000 gammarer.aws-secure-bucket-0.9.3/src/gammarer.aws_secure_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 17:24:13.000000 gammarer.aws-secure-bucket-0.9.3/src/gammarer.aws_secure_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:23:47.127654 gammarer.aws-secure-bucket-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-21 17:23:32.000000 gammarer.aws-secure-bucket-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 17:23:32.000000 gammarer.aws-secure-bucket-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-21 17:23:47.127654 gammarer.aws-secure-bucket-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-21 17:23:32.000000 gammarer.aws-secure-bucket-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-21 17:23:32.000000 gammarer.aws-secure-bucket-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 17:23:47.127654 gammarer.aws-secure-bucket-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-21 17:23:32.000000 gammarer.aws-secure-bucket-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:23:47.127654 gammarer.aws-secure-bucket-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:23:47.127654 gammarer.aws-secure-bucket-0.9.4/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:23:47.127654 gammarer.aws-secure-bucket-0.9.4/src/gammarer/aws_secure_bucket/
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-07-21 17:23:32.000000 gammarer.aws-secure-bucket-0.9.4/src/gammarer/aws_secure_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:23:47.127654 gammarer.aws-secure-bucket-0.9.4/src/gammarer/aws_secure_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-21 17:23:32.000000 gammarer.aws-secure-bucket-0.9.4/src/gammarer/aws_secure_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30735 2023-07-21 17:23:32.000000 gammarer.aws-secure-bucket-0.9.4/src/gammarer/aws_secure_bucket/_jsii/aws-secure-bucket@0.9.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 17:23:32.000000 gammarer.aws-secure-bucket-0.9.4/src/gammarer/aws_secure_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:23:47.127654 gammarer.aws-secure-bucket-0.9.4/src/gammarer.aws_secure_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-21 17:23:47.000000 gammarer.aws-secure-bucket-0.9.4/src/gammarer.aws_secure_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-21 17:23:47.000000 gammarer.aws-secure-bucket-0.9.4/src/gammarer.aws_secure_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 17:23:47.000000 gammarer.aws-secure-bucket-0.9.4/src/gammarer.aws_secure_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-21 17:23:47.000000 gammarer.aws-secure-bucket-0.9.4/src/gammarer.aws_secure_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 17:23:47.000000 gammarer.aws-secure-bucket-0.9.4/src/gammarer.aws_secure_bucket.egg-info/top_level.txt
```

### Comparing `gammarer.aws-secure-bucket-0.9.3/LICENSE` & `gammarer.aws-secure-bucket-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-bucket-0.9.3/PKG-INFO` & `gammarer.aws-secure-bucket-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-bucket
-Version: 0.9.3
+Version: 0.9.4
 Summary: This is a Simple S3 Secure Bucket.
 Home-page: https://github.com/yicr/aws-secure-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-bucket-0.9.3/README.md` & `gammarer.aws-secure-bucket-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-bucket-0.9.3/setup.py` & `gammarer.aws-secure-bucket-0.9.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-secure-bucket",
-    "version": "0.9.3",
+    "version": "0.9.4",
     "description": "This is a Simple S3 Secure Bucket.",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-secure-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_secure_bucket",
         "gammarer.aws_secure_bucket._jsii"
     ],
     "package_data": {
         "gammarer.aws_secure_bucket._jsii": [
-            "aws-secure-bucket@0.9.3.jsii.tgz"
+            "aws-secure-bucket@0.9.4.jsii.tgz"
         ],
         "gammarer.aws_secure_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `gammarer.aws-secure-bucket-0.9.3/src/gammarer/aws_secure_bucket/__init__.py` & `gammarer.aws-secure-bucket-0.9.4/src/gammarer/aws_secure_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-bucket-0.9.3/src/gammarer.aws_secure_bucket.egg-info/PKG-INFO` & `gammarer.aws-secure-bucket-0.9.4/src/gammarer.aws_secure_bucket.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-bucket
-Version: 0.9.3
+Version: 0.9.4
 Summary: This is a Simple S3 Secure Bucket.
 Home-page: https://github.com/yicr/aws-secure-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-bucket-0.9.3/src/gammarer.aws_secure_bucket.egg-info/SOURCES.txt` & `gammarer.aws-secure-bucket-0.9.4/src/gammarer.aws_secure_bucket.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_secure_bucket.egg-info/SOURCES.txt
 src/gammarer.aws_secure_bucket.egg-info/dependency_links.txt
 src/gammarer.aws_secure_bucket.egg-info/requires.txt
 src/gammarer.aws_secure_bucket.egg-info/top_level.txt
 src/gammarer/aws_secure_bucket/__init__.py
 src/gammarer/aws_secure_bucket/py.typed
 src/gammarer/aws_secure_bucket/_jsii/__init__.py
-src/gammarer/aws_secure_bucket/_jsii/aws-secure-bucket@0.9.3.jsii.tgz
+src/gammarer/aws_secure_bucket/_jsii/aws-secure-bucket@0.9.4.jsii.tgz
```

