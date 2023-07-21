# Comparing `tmp/cdk-lambda-bash-2.0.98.tar.gz` & `tmp/cdk-lambda-bash-2.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-lambda-bash-2.0.98.tar", last modified: Sat Jul 23 00:18:26 2022, max compression
+gzip compressed data, was "cdk-lambda-bash-2.0.99.tar", last modified: Sun Jul 24 00:18:10 2022, max compression
```

## Comparing `cdk-lambda-bash-2.0.98.tar` & `cdk-lambda-bash-2.0.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 00:18:26.078549 cdk-lambda-bash-2.0.98/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-07-23 00:18:12.000000 cdk-lambda-bash-2.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-07-23 00:18:12.000000 cdk-lambda-bash-2.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6035 2022-07-23 00:18:26.078549 cdk-lambda-bash-2.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5141 2022-07-23 00:18:12.000000 cdk-lambda-bash-2.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-07-23 00:18:12.000000 cdk-lambda-bash-2.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-23 00:18:26.078549 cdk-lambda-bash-2.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-07-23 00:18:12.000000 cdk-lambda-bash-2.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 00:18:26.078549 cdk-lambda-bash-2.0.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 00:18:26.078549 cdk-lambda-bash-2.0.98/src/cdk_lambda_bash/
--rw-r--r--   0 runner    (1001) docker     (121)    12418 2022-07-23 00:18:12.000000 cdk-lambda-bash-2.0.98/src/cdk_lambda_bash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 00:18:26.078549 cdk-lambda-bash-2.0.98/src/cdk_lambda_bash/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-07-23 00:18:12.000000 cdk-lambda-bash-2.0.98/src/cdk_lambda_bash/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26879 2022-07-23 00:18:12.000000 cdk-lambda-bash-2.0.98/src/cdk_lambda_bash/_jsii/cdk-lambda-bash@2.0.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-23 00:18:12.000000 cdk-lambda-bash-2.0.98/src/cdk_lambda_bash/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 00:18:26.078549 cdk-lambda-bash-2.0.98/src/cdk_lambda_bash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6035 2022-07-23 00:18:25.000000 cdk-lambda-bash-2.0.98/src/cdk_lambda_bash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-07-23 00:18:26.000000 cdk-lambda-bash-2.0.98/src/cdk_lambda_bash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-23 00:18:25.000000 cdk-lambda-bash-2.0.98/src/cdk_lambda_bash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-07-23 00:18:25.000000 cdk-lambda-bash-2.0.98/src/cdk_lambda_bash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-07-23 00:18:25.000000 cdk-lambda-bash-2.0.98/src/cdk_lambda_bash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 00:18:10.735690 cdk-lambda-bash-2.0.99/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-07-24 00:17:58.000000 cdk-lambda-bash-2.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-07-24 00:17:58.000000 cdk-lambda-bash-2.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6035 2022-07-24 00:18:10.735690 cdk-lambda-bash-2.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5141 2022-07-24 00:17:58.000000 cdk-lambda-bash-2.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-07-24 00:17:58.000000 cdk-lambda-bash-2.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-24 00:18:10.735690 cdk-lambda-bash-2.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-07-24 00:17:58.000000 cdk-lambda-bash-2.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 00:18:10.735690 cdk-lambda-bash-2.0.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 00:18:10.735690 cdk-lambda-bash-2.0.99/src/cdk_lambda_bash/
+-rw-r--r--   0 runner    (1001) docker     (121)    12418 2022-07-24 00:17:58.000000 cdk-lambda-bash-2.0.99/src/cdk_lambda_bash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 00:18:10.735690 cdk-lambda-bash-2.0.99/src/cdk_lambda_bash/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      365 2022-07-24 00:17:58.000000 cdk-lambda-bash-2.0.99/src/cdk_lambda_bash/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26881 2022-07-24 00:17:58.000000 cdk-lambda-bash-2.0.99/src/cdk_lambda_bash/_jsii/cdk-lambda-bash@2.0.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-24 00:17:58.000000 cdk-lambda-bash-2.0.99/src/cdk_lambda_bash/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 00:18:10.735690 cdk-lambda-bash-2.0.99/src/cdk_lambda_bash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6035 2022-07-24 00:18:10.000000 cdk-lambda-bash-2.0.99/src/cdk_lambda_bash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2022-07-24 00:18:10.000000 cdk-lambda-bash-2.0.99/src/cdk_lambda_bash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-24 00:18:10.000000 cdk-lambda-bash-2.0.99/src/cdk_lambda_bash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-07-24 00:18:10.000000 cdk-lambda-bash-2.0.99/src/cdk_lambda_bash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-07-24 00:18:10.000000 cdk-lambda-bash-2.0.99/src/cdk_lambda_bash.egg-info/top_level.txt
```

### Comparing `cdk-lambda-bash-2.0.98/LICENSE` & `cdk-lambda-bash-2.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-lambda-bash-2.0.98/PKG-INFO` & `cdk-lambda-bash-2.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-lambda-bash
-Version: 2.0.98
+Version: 2.0.99
 Summary: Deploy Bash Lambda Functions with AWS CDK
 Home-page: https://github.com/pahud/cdk-lambda-bash.git
 Author: Pahud Hsieh
 License: Apache-2.0
 Project-URL: Source, https://github.com/pahud/cdk-lambda-bash.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk-lambda-bash-2.0.98/README.md` & `cdk-lambda-bash-2.0.99/README.md`

 * *Files identical despite different names*

### Comparing `cdk-lambda-bash-2.0.98/setup.py` & `cdk-lambda-bash-2.0.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-lambda-bash",
-    "version": "2.0.98",
+    "version": "2.0.99",
     "description": "Deploy Bash Lambda Functions with AWS CDK",
     "license": "Apache-2.0",
     "url": "https://github.com/pahud/cdk-lambda-bash.git",
     "long_description_content_type": "text/markdown",
     "author": "Pahud Hsieh",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_lambda_bash",
         "cdk_lambda_bash._jsii"
     ],
     "package_data": {
         "cdk_lambda_bash._jsii": [
-            "cdk-lambda-bash@2.0.98.jsii.tgz"
+            "cdk-lambda-bash@2.0.99.jsii.tgz"
         ],
         "cdk_lambda_bash": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-lambda-bash-2.0.98/src/cdk_lambda_bash/__init__.py` & `cdk-lambda-bash-2.0.99/src/cdk_lambda_bash/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-lambda-bash-2.0.98/src/cdk_lambda_bash.egg-info/PKG-INFO` & `cdk-lambda-bash-2.0.99/src/cdk_lambda_bash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-lambda-bash
-Version: 2.0.98
+Version: 2.0.99
 Summary: Deploy Bash Lambda Functions with AWS CDK
 Home-page: https://github.com/pahud/cdk-lambda-bash.git
 Author: Pahud Hsieh
 License: Apache-2.0
 Project-URL: Source, https://github.com/pahud/cdk-lambda-bash.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

