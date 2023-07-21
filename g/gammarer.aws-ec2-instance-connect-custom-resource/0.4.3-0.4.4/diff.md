# Comparing `tmp/gammarer.aws-ec2-instance-connect-custom-resource-0.4.3.tar.gz` & `tmp/gammarer.aws-ec2-instance-connect-custom-resource-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-ec2-instance-connect-custom-resource-0.4.3.tar", last modified: Thu Jul 20 17:13:12 2023, max compression
+gzip compressed data, was "gammarer.aws-ec2-instance-connect-custom-resource-0.4.4.tar", last modified: Fri Jul 21 17:13:04 2023, max compression
```

## Comparing `gammarer.aws-ec2-instance-connect-custom-resource-0.4.3.tar` & `gammarer.aws-ec2-instance-connect-custom-resource-0.4.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:13:12.950274 gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-20 17:13:01.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 17:13:01.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-20 17:13:12.950274 gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-20 17:13:01.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-20 17:13:01.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 17:13:12.950274 gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-20 17:13:01.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:13:12.946274 gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:13:12.946274 gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:13:12.950274 gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/src/gammarer/aws_ec2_instance_connect_custom_resource/
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-20 17:13:01.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/src/gammarer/aws_ec2_instance_connect_custom_resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:13:12.950274 gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-20 17:13:01.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16978 2023-07-20 17:13:01.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/aws-ec2-instance-connect-custom-resource@0.4.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:13:01.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/src/gammarer/aws_ec2_instance_connect_custom_resource/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:13:12.950274 gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-20 17:13:12.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-20 17:13:12.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:13:12.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-20 17:13:12.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 17:13:12.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:13:04.380452 gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-21 17:12:48.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 17:12:48.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-21 17:13:04.380452 gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-21 17:12:48.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-21 17:12:48.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 17:13:04.380452 gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-21 17:12:48.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:13:04.380452 gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:13:04.380452 gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:13:04.380452 gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/src/gammarer/aws_ec2_instance_connect_custom_resource/
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-21 17:12:48.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/src/gammarer/aws_ec2_instance_connect_custom_resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:13:04.380452 gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-21 17:12:48.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16978 2023-07-21 17:12:48.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/aws-ec2-instance-connect-custom-resource@0.4.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 17:12:48.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/src/gammarer/aws_ec2_instance_connect_custom_resource/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:13:04.380452 gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-21 17:13:04.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-21 17:13:04.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 17:13:04.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-21 17:13:04.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 17:13:04.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/top_level.txt
```

### Comparing `gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/LICENSE` & `gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/PKG-INFO` & `gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ec2-instance-connect-custom-resource
-Version: 0.4.3
+Version: 0.4.4
 Summary: AWS EC2 instance connect custom resource
 Home-page: https://github.com/yicr/aws-ec2-instance-connect-custom-resource.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ec2-instance-connect-custom-resource.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/README.md` & `gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/setup.py` & `gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-ec2-instance-connect-custom-resource",
-    "version": "0.4.3",
+    "version": "0.4.4",
     "description": "AWS EC2 instance connect custom resource",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-ec2-instance-connect-custom-resource.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_ec2_instance_connect_custom_resource",
         "gammarer.aws_ec2_instance_connect_custom_resource._jsii"
     ],
     "package_data": {
         "gammarer.aws_ec2_instance_connect_custom_resource._jsii": [
-            "aws-ec2-instance-connect-custom-resource@0.4.3.jsii.tgz"
+            "aws-ec2-instance-connect-custom-resource@0.4.4.jsii.tgz"
         ],
         "gammarer.aws_ec2_instance_connect_custom_resource": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/src/gammarer/aws_ec2_instance_connect_custom_resource/__init__.py` & `gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/src/gammarer/aws_ec2_instance_connect_custom_resource/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/PKG-INFO` & `gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ec2-instance-connect-custom-resource
-Version: 0.4.3
+Version: 0.4.4
 Summary: AWS EC2 instance connect custom resource
 Home-page: https://github.com/yicr/aws-ec2-instance-connect-custom-resource.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ec2-instance-connect-custom-resource.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-ec2-instance-connect-custom-resource-0.4.3/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/SOURCES.txt` & `gammarer.aws-ec2-instance-connect-custom-resource-0.4.4/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/SOURCES.txt
 src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/dependency_links.txt
 src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/requires.txt
 src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/top_level.txt
 src/gammarer/aws_ec2_instance_connect_custom_resource/__init__.py
 src/gammarer/aws_ec2_instance_connect_custom_resource/py.typed
 src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/__init__.py
-src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/aws-ec2-instance-connect-custom-resource@0.4.3.jsii.tgz
+src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/aws-ec2-instance-connect-custom-resource@0.4.4.jsii.tgz
```

