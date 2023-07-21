# Comparing `tmp/gammarer.aws-frontend-web-app-deploy-stack-0.5.2.tar.gz` & `tmp/gammarer.aws-frontend-web-app-deploy-stack-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-frontend-web-app-deploy-stack-0.5.2.tar", last modified: Thu Jul 20 19:14:05 2023, max compression
+gzip compressed data, was "gammarer.aws-frontend-web-app-deploy-stack-0.5.3.tar", last modified: Fri Jul 21 19:14:00 2023, max compression
```

## Comparing `gammarer.aws-frontend-web-app-deploy-stack-0.5.2.tar` & `gammarer.aws-frontend-web-app-deploy-stack-0.5.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:14:05.826490 gammarer.aws-frontend-web-app-deploy-stack-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-20 19:13:53.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 19:13:53.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-20 19:14:05.826490 gammarer.aws-frontend-web-app-deploy-stack-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-20 19:13:53.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-20 19:13:53.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:14:05.826490 gammarer.aws-frontend-web-app-deploy-stack-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-20 19:13:53.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:14:05.826490 gammarer.aws-frontend-web-app-deploy-stack-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:14:05.826490 gammarer.aws-frontend-web-app-deploy-stack-0.5.2/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:14:05.826490 gammarer.aws-frontend-web-app-deploy-stack-0.5.2/src/gammarer/aws_frontend_web_app_deploy_stack/
--rw-r--r--   0 runner    (1001) docker     (123)    26250 2023-07-20 19:13:53.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.2/src/gammarer/aws_frontend_web_app_deploy_stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:14:05.826490 gammarer.aws-frontend-web-app-deploy-stack-0.5.2/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-20 19:13:53.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.2/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36450 2023-07-20 19:13:53.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.2/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@0.5.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:13:53.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.2/src/gammarer/aws_frontend_web_app_deploy_stack/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:14:05.826490 gammarer.aws-frontend-web-app-deploy-stack-0.5.2/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-20 19:14:05.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.2/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-20 19:14:05.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.2/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:14:05.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.2/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-20 19:14:05.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.2/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 19:14:05.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.2/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:14:00.245340 gammarer.aws-frontend-web-app-deploy-stack-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-21 19:13:45.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 19:13:45.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-21 19:14:00.245340 gammarer.aws-frontend-web-app-deploy-stack-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-21 19:13:45.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-21 19:13:45.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 19:14:00.245340 gammarer.aws-frontend-web-app-deploy-stack-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-21 19:13:45.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:14:00.241340 gammarer.aws-frontend-web-app-deploy-stack-0.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:14:00.241340 gammarer.aws-frontend-web-app-deploy-stack-0.5.3/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:14:00.245340 gammarer.aws-frontend-web-app-deploy-stack-0.5.3/src/gammarer/aws_frontend_web_app_deploy_stack/
+-rw-r--r--   0 runner    (1001) docker     (123)    26250 2023-07-21 19:13:45.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.3/src/gammarer/aws_frontend_web_app_deploy_stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:14:00.245340 gammarer.aws-frontend-web-app-deploy-stack-0.5.3/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-21 19:13:45.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.3/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36454 2023-07-21 19:13:45.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.3/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@0.5.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 19:13:45.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.3/src/gammarer/aws_frontend_web_app_deploy_stack/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:14:00.245340 gammarer.aws-frontend-web-app-deploy-stack-0.5.3/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-21 19:14:00.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.3/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-21 19:14:00.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.3/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 19:14:00.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.3/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-21 19:14:00.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.3/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 19:14:00.000000 gammarer.aws-frontend-web-app-deploy-stack-0.5.3/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/top_level.txt
```

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-0.5.2/LICENSE` & `gammarer.aws-frontend-web-app-deploy-stack-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-0.5.2/PKG-INFO` & `gammarer.aws-frontend-web-app-deploy-stack-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-frontend-web-app-deploy-stack
-Version: 0.5.2
+Version: 0.5.3
 Summary: This is an AWS CDK Construct to make deploying a Frontend Web App (SPA) deploy to S3 behind CloudFront.
 Home-page: https://github.com/yicr/aws-frontend-web-app-deploy-stack.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-frontend-web-app-deploy-stack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-0.5.2/README.md` & `gammarer.aws-frontend-web-app-deploy-stack-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-0.5.2/setup.py` & `gammarer.aws-frontend-web-app-deploy-stack-0.5.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-frontend-web-app-deploy-stack",
-    "version": "0.5.2",
+    "version": "0.5.3",
     "description": "This is an AWS CDK Construct to make deploying a Frontend Web App (SPA) deploy to S3 behind CloudFront.",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-frontend-web-app-deploy-stack.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,27 +22,27 @@
     },
     "packages": [
         "gammarer.aws_frontend_web_app_deploy_stack",
         "gammarer.aws_frontend_web_app_deploy_stack._jsii"
     ],
     "package_data": {
         "gammarer.aws_frontend_web_app_deploy_stack._jsii": [
-            "aws-frontend-web-app-deploy-stack@0.5.2.jsii.tgz"
+            "aws-frontend-web-app-deploy-stack@0.5.3.jsii.tgz"
         ],
         "gammarer.aws_frontend_web_app_deploy_stack": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.62.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "gammarer.aws-secure-bucket>=0.9.3, <0.10.0",
-        "gammarer.aws-secure-cloudfront-origin-bucket>=0.6.2, <0.7.0",
-        "gammarer.aws-secure-frontend-web-app-cloudfront-distribution>=0.6.2, <0.7.0",
+        "gammarer.aws-secure-bucket>=0.9.4, <0.10.0",
+        "gammarer.aws-secure-cloudfront-origin-bucket>=0.6.3, <0.7.0",
+        "gammarer.aws-secure-frontend-web-app-cloudfront-distribution>=0.6.3, <0.7.0",
         "jsii>=1.85.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-0.5.2/src/gammarer/aws_frontend_web_app_deploy_stack/__init__.py` & `gammarer.aws-frontend-web-app-deploy-stack-0.5.3/src/gammarer/aws_frontend_web_app_deploy_stack/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-0.5.2/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/__init__.py` & `gammarer.aws-frontend-web-app-deploy-stack-0.5.3/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 import constructs._jsii
 import gammarer.aws_secure_bucket._jsii
 import gammarer.aws_secure_cloudfront_origin_bucket._jsii
 import gammarer.aws_secure_frontend_web_app_cloudfront_distribution._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarer/aws-frontend-web-app-deploy-stack",
-    "0.5.2",
+    "0.5.3",
     __name__[0:-6],
-    "aws-frontend-web-app-deploy-stack@0.5.2.jsii.tgz",
+    "aws-frontend-web-app-deploy-stack@0.5.3.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-0.5.2/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO` & `gammarer.aws-frontend-web-app-deploy-stack-0.5.3/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-frontend-web-app-deploy-stack
-Version: 0.5.2
+Version: 0.5.3
 Summary: This is an AWS CDK Construct to make deploying a Frontend Web App (SPA) deploy to S3 behind CloudFront.
 Home-page: https://github.com/yicr/aws-frontend-web-app-deploy-stack.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-frontend-web-app-deploy-stack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-0.5.2/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt` & `gammarer.aws-frontend-web-app-deploy-stack-0.5.3/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt
 src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/dependency_links.txt
 src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/requires.txt
 src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/top_level.txt
 src/gammarer/aws_frontend_web_app_deploy_stack/__init__.py
 src/gammarer/aws_frontend_web_app_deploy_stack/py.typed
 src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/__init__.py
-src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@0.5.2.jsii.tgz
+src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@0.5.3.jsii.tgz
```

