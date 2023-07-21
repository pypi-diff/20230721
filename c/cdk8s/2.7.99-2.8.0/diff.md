# Comparing `tmp/cdk8s-2.7.99.tar.gz` & `tmp/cdk8s-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-2.7.99.tar", last modified: Mon Jul 10 00:24:32 2023, max compression
+gzip compressed data, was "cdk8s-2.8.0.tar", last modified: Fri Jul 21 00:28:02 2023, max compression
```

## Comparing `cdk8s-2.7.99.tar` & `cdk8s-2.8.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:24:32.510015 cdk8s-2.7.99/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-10 00:24:20.000000 cdk8s-2.7.99/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 00:24:20.000000 cdk8s-2.7.99/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 00:24:20.000000 cdk8s-2.7.99/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-10 00:24:32.510015 cdk8s-2.7.99/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-10 00:24:20.000000 cdk8s-2.7.99/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-10 00:24:20.000000 cdk8s-2.7.99/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 00:24:32.510015 cdk8s-2.7.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-10 00:24:20.000000 cdk8s-2.7.99/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:24:32.510015 cdk8s-2.7.99/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:24:32.510015 cdk8s-2.7.99/src/cdk8s/
--rw-r--r--   0 runner    (1001) docker     (123)   138472 2023-07-10 00:24:20.000000 cdk8s-2.7.99/src/cdk8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:24:32.510015 cdk8s-2.7.99/src/cdk8s/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-10 00:24:20.000000 cdk8s-2.7.99/src/cdk8s/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   298142 2023-07-10 00:24:20.000000 cdk8s-2.7.99/src/cdk8s/_jsii/cdk8s@2.7.99.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 00:24:20.000000 cdk8s-2.7.99/src/cdk8s/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 00:24:32.510015 cdk8s-2.7.99/src/cdk8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-10 00:24:32.000000 cdk8s-2.7.99/src/cdk8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-10 00:24:32.000000 cdk8s-2.7.99/src/cdk8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 00:24:32.000000 cdk8s-2.7.99/src/cdk8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-10 00:24:32.000000 cdk8s-2.7.99/src/cdk8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 00:24:32.000000 cdk8s-2.7.99/src/cdk8s.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:28:02.854897 cdk8s-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-21 00:27:51.000000 cdk8s-2.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 00:27:51.000000 cdk8s-2.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-21 00:27:51.000000 cdk8s-2.8.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-21 00:28:02.854897 cdk8s-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-21 00:27:51.000000 cdk8s-2.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-21 00:27:51.000000 cdk8s-2.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 00:28:02.854897 cdk8s-2.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-21 00:27:51.000000 cdk8s-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:28:02.854897 cdk8s-2.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:28:02.854897 cdk8s-2.8.0/src/cdk8s/
+-rw-r--r--   0 runner    (1001) docker     (123)   138473 2023-07-21 00:27:51.000000 cdk8s-2.8.0/src/cdk8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:28:02.854897 cdk8s-2.8.0/src/cdk8s/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-21 00:27:51.000000 cdk8s-2.8.0/src/cdk8s/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   299476 2023-07-21 00:27:51.000000 cdk8s-2.8.0/src/cdk8s/_jsii/cdk8s@2.8.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 00:27:51.000000 cdk8s-2.8.0/src/cdk8s/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:28:02.854897 cdk8s-2.8.0/src/cdk8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-21 00:28:02.000000 cdk8s-2.8.0/src/cdk8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-21 00:28:02.000000 cdk8s-2.8.0/src/cdk8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 00:28:02.000000 cdk8s-2.8.0/src/cdk8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-21 00:28:02.000000 cdk8s-2.8.0/src/cdk8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 00:28:02.000000 cdk8s-2.8.0/src/cdk8s.egg-info/top_level.txt
```

### Comparing `cdk8s-2.7.99/LICENSE` & `cdk8s-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-2.7.99/PKG-INFO` & `cdk8s-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s
-Version: 2.7.99
+Version: 2.8.0
 Summary: This is the core library of Cloud Development Kit (CDK) for Kubernetes (cdk8s). cdk8s apps synthesize into standard Kubernetes manifests which can be applied to any Kubernetes cluster.
 Home-page: https://github.com/cdk8s-team/cdk8s-core.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-core.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-2.7.99/README.md` & `cdk8s-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-2.7.99/setup.py` & `cdk8s-2.8.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s",
-    "version": "2.7.99",
+    "version": "2.8.0",
     "description": "This is the core library of Cloud Development Kit (CDK) for Kubernetes (cdk8s). cdk8s apps synthesize into standard Kubernetes manifests which can be applied to any Kubernetes cluster.",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-core.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "cdk8s",
         "cdk8s._jsii"
     ],
     "package_data": {
         "cdk8s._jsii": [
-            "cdk8s@2.7.99.jsii.tgz"
+            "cdk8s@2.8.0.jsii.tgz"
         ],
         "cdk8s": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.81.0, <2.0.0",
+        "jsii>=1.85.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk8s-2.7.99/src/cdk8s/__init__.py` & `cdk8s-2.8.0/src/cdk8s/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1177,15 +1177,15 @@
             type_hints = typing.get_type_hints(_typecheckingstub__00e42df9fe8e54748af3dd0e25616d4ea57a51e241dfc6972407f4bce78ced02)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         jsii.create(self.__class__, self, [node])
 
     @jsii.member(jsii_name="topology")
     def topology(self) -> typing.List[_constructs_77d1e7e8.IConstruct]:
         '''
-        :see: Vertex.topology()
+        :see: Vertex.topology ()
         '''
         return typing.cast(typing.List[_constructs_77d1e7e8.IConstruct], jsii.invoke(self, "topology", []))
 
     @builtins.property
     @jsii.member(jsii_name="root")
     def root(self) -> "DependencyVertex":
         '''Returns the root of the graph.
```

### Comparing `cdk8s-2.7.99/src/cdk8s.egg-info/PKG-INFO` & `cdk8s-2.8.0/src/cdk8s.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s
-Version: 2.7.99
+Version: 2.8.0
 Summary: This is the core library of Cloud Development Kit (CDK) for Kubernetes (cdk8s). cdk8s apps synthesize into standard Kubernetes manifests which can be applied to any Kubernetes cluster.
 Home-page: https://github.com/cdk8s-team/cdk8s-core.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-core.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

