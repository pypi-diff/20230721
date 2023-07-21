# Comparing `tmp/cdk-aws-lambda-powertools-layer-3.5.0.tar.gz` & `tmp/cdk-aws-lambda-powertools-layer-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-aws-lambda-powertools-layer-3.5.0.tar", last modified: Tue Apr 18 13:15:41 2023, max compression
+gzip compressed data, was "cdk-aws-lambda-powertools-layer-3.6.0.tar", last modified: Fri Jul 21 14:55:25 2023, max compression
```

## Comparing `cdk-aws-lambda-powertools-layer-3.5.0.tar` & `cdk-aws-lambda-powertools-layer-3.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:15:41.269545 cdk-aws-lambda-powertools-layer-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-18 13:15:25.000000 cdk-aws-lambda-powertools-layer-3.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 13:15:25.000000 cdk-aws-lambda-powertools-layer-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-04-18 13:15:41.269545 cdk-aws-lambda-powertools-layer-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-04-18 13:15:25.000000 cdk-aws-lambda-powertools-layer-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 13:15:25.000000 cdk-aws-lambda-powertools-layer-3.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 13:15:41.269545 cdk-aws-lambda-powertools-layer-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-18 13:15:25.000000 cdk-aws-lambda-powertools-layer-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:15:41.265545 cdk-aws-lambda-powertools-layer-3.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:15:41.269545 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer/
--rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-04-18 13:15:25.000000 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:15:41.269545 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-18 13:15:25.000000 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22909 2023-04-18 13:15:25.000000 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer/_jsii/cdk-aws-lambda-powertools-layer@3.5.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:15:25.000000 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:15:41.269545 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-04-18 13:15:41.000000 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-18 13:15:41.000000 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:15:41.000000 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-18 13:15:41.000000 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-18 13:15:41.000000 cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:55:25.775447 cdk-aws-lambda-powertools-layer-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-21 14:55:14.000000 cdk-aws-lambda-powertools-layer-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 14:55:14.000000 cdk-aws-lambda-powertools-layer-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-21 14:55:25.775447 cdk-aws-lambda-powertools-layer-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-21 14:55:14.000000 cdk-aws-lambda-powertools-layer-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-21 14:55:14.000000 cdk-aws-lambda-powertools-layer-3.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 14:55:25.775447 cdk-aws-lambda-powertools-layer-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-21 14:55:14.000000 cdk-aws-lambda-powertools-layer-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:55:25.771447 cdk-aws-lambda-powertools-layer-3.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:55:25.775447 cdk-aws-lambda-powertools-layer-3.6.0/src/cdk_aws_lambda_powertools_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-07-21 14:55:14.000000 cdk-aws-lambda-powertools-layer-3.6.0/src/cdk_aws_lambda_powertools_layer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:55:25.775447 cdk-aws-lambda-powertools-layer-3.6.0/src/cdk_aws_lambda_powertools_layer/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-21 14:55:14.000000 cdk-aws-lambda-powertools-layer-3.6.0/src/cdk_aws_lambda_powertools_layer/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23108 2023-07-21 14:55:14.000000 cdk-aws-lambda-powertools-layer-3.6.0/src/cdk_aws_lambda_powertools_layer/_jsii/cdk-aws-lambda-powertools-layer@3.6.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:55:14.000000 cdk-aws-lambda-powertools-layer-3.6.0/src/cdk_aws_lambda_powertools_layer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:55:25.775447 cdk-aws-lambda-powertools-layer-3.6.0/src/cdk_aws_lambda_powertools_layer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-21 14:55:25.000000 cdk-aws-lambda-powertools-layer-3.6.0/src/cdk_aws_lambda_powertools_layer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-21 14:55:25.000000 cdk-aws-lambda-powertools-layer-3.6.0/src/cdk_aws_lambda_powertools_layer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:55:25.000000 cdk-aws-lambda-powertools-layer-3.6.0/src/cdk_aws_lambda_powertools_layer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-21 14:55:25.000000 cdk-aws-lambda-powertools-layer-3.6.0/src/cdk_aws_lambda_powertools_layer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-21 14:55:25.000000 cdk-aws-lambda-powertools-layer-3.6.0/src/cdk_aws_lambda_powertools_layer.egg-info/top_level.txt
```

### Comparing `cdk-aws-lambda-powertools-layer-3.5.0/LICENSE` & `cdk-aws-lambda-powertools-layer-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-aws-lambda-powertools-layer-3.5.0/PKG-INFO` & `cdk-aws-lambda-powertools-layer-3.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cdk-aws-lambda-powertools-layer
-Version: 3.5.0
-Summary: A lambda layer for AWS Powertools for python and typescript
+Version: 3.6.0
+Summary: Powertools for AWS Lambda layer for python and typescript
 Home-page: https://github.com/awslabs/cdk-aws-lambda-powertools-layer.git
 Author: Amazon Web Services
 License: MIT-0
 Project-URL: Source, https://github.com/awslabs/cdk-aws-lambda-powertools-layer.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
@@ -18,19 +18,19 @@
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# AWS Lambda powertools layer
+# Powertools for AWS Lambda Layer
 
 ## Why this project exists
 
-This is a custom construct that will create AWS Lambda Layer with AWS Powertools for Python or NodeJS library. There are different
+This is a custom construct that will create AWS Lambda Layer with Powertools for AWS Lambda for Python or NodeJS library. There are different
 ways how to create a layer and when working with CDK you need to install the library, create a zip file and wire it
 correctly. With this construct you don't have to care about packaging and dependency management. Create a construct
 and add it to your function. The construct is an extension of the
 existing [`LayerVersion`](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_lambda.LayerVersion.html) construct
 from the CDK library, so you have access to all fields and methods.
 
 > ⚠️ **This construct uses docker to build and bundle the dependencies!**
@@ -69,15 +69,15 @@
 pip install cdk-aws-lambda-powertools-layer
 ```
 
 ## Usage
 
 ### Python
 
-A single line will create a layer with powertools for python. For NodeJS you need to specifically set the `runtimeFamily: Runtime.NODEJS` property.
+A single line will create a layer with Powertools for AWS Lambda (Python). For NodeJS you need to specifically set the `runtimeFamily: Runtime.NODEJS` property.
 
 ```python
 from cdk_aws_lambda_powertools_layer import LambdaPowertoolsLayer
 
 powertoolsLayer = LambdaPowertoolsLayer(self, 'PowertoolsLayer')
 ```
```

### Comparing `cdk-aws-lambda-powertools-layer-3.5.0/README.md` & `cdk-aws-lambda-powertools-layer-3.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# AWS Lambda powertools layer
+# Powertools for AWS Lambda Layer
 
 ## Why this project exists
 
-This is a custom construct that will create AWS Lambda Layer with AWS Powertools for Python or NodeJS library. There are different
+This is a custom construct that will create AWS Lambda Layer with Powertools for AWS Lambda for Python or NodeJS library. There are different
 ways how to create a layer and when working with CDK you need to install the library, create a zip file and wire it
 correctly. With this construct you don't have to care about packaging and dependency management. Create a construct
 and add it to your function. The construct is an extension of the
 existing [`LayerVersion`](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_lambda.LayerVersion.html) construct
 from the CDK library, so you have access to all fields and methods.
 
 > ⚠️ **This construct uses docker to build and bundle the dependencies!**
@@ -45,15 +45,15 @@
 pip install cdk-aws-lambda-powertools-layer
 ```
 
 ## Usage
 
 ### Python
 
-A single line will create a layer with powertools for python. For NodeJS you need to specifically set the `runtimeFamily: Runtime.NODEJS` property.
+A single line will create a layer with Powertools for AWS Lambda (Python). For NodeJS you need to specifically set the `runtimeFamily: Runtime.NODEJS` property.
 
 ```python
 from cdk_aws_lambda_powertools_layer import LambdaPowertoolsLayer
 
 powertoolsLayer = LambdaPowertoolsLayer(self, 'PowertoolsLayer')
 ```
```

### Comparing `cdk-aws-lambda-powertools-layer-3.5.0/setup.py` & `cdk-aws-lambda-powertools-layer-3.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-aws-lambda-powertools-layer",
-    "version": "3.5.0",
-    "description": "A lambda layer for AWS Powertools for python and typescript",
+    "version": "3.6.0",
+    "description": "Powertools for AWS Lambda layer for python and typescript",
     "license": "MIT-0",
     "url": "https://github.com/awslabs/cdk-aws-lambda-powertools-layer.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
     },
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_aws_lambda_powertools_layer",
         "cdk_aws_lambda_powertools_layer._jsii"
     ],
     "package_data": {
         "cdk_aws_lambda_powertools_layer._jsii": [
-            "cdk-aws-lambda-powertools-layer@3.5.0.jsii.tgz"
+            "cdk-aws-lambda-powertools-layer@3.6.0.jsii.tgz"
         ],
         "cdk_aws_lambda_powertools_layer": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.75.0, <3.0.0",
+        "aws-cdk-lib>=2.88.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.80.0, <2.0.0",
+        "jsii>=1.85.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer/__init__.py` & `cdk-aws-lambda-powertools-layer-3.6.0/src/cdk_aws_lambda_powertools_layer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
-# AWS Lambda powertools layer
+# Powertools for AWS Lambda Layer
 
 ## Why this project exists
 
-This is a custom construct that will create AWS Lambda Layer with AWS Powertools for Python or NodeJS library. There are different
+This is a custom construct that will create AWS Lambda Layer with Powertools for AWS Lambda for Python or NodeJS library. There are different
 ways how to create a layer and when working with CDK you need to install the library, create a zip file and wire it
 correctly. With this construct you don't have to care about packaging and dependency management. Create a construct
 and add it to your function. The construct is an extension of the
 existing [`LayerVersion`](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_lambda.LayerVersion.html) construct
 from the CDK library, so you have access to all fields and methods.
 
 > ⚠️ **This construct uses docker to build and bundle the dependencies!**
@@ -46,15 +46,15 @@
 pip install cdk-aws-lambda-powertools-layer
 ```
 
 ## Usage
 
 ### Python
 
-A single line will create a layer with powertools for python. For NodeJS you need to specifically set the `runtimeFamily: Runtime.NODEJS` property.
+A single line will create a layer with Powertools for AWS Lambda (Python). For NodeJS you need to specifically set the `runtimeFamily: Runtime.NODEJS` property.
 
 ```python
 from cdk_aws_lambda_powertools_layer import LambdaPowertoolsLayer
 
 powertoolsLayer = LambdaPowertoolsLayer(self, 'PowertoolsLayer')
 ```
 
@@ -155,15 +155,15 @@
 
 
 class LambdaPowertoolsLayer(
     _aws_cdk_aws_lambda_ceddda9d.LayerVersion,
     metaclass=jsii.JSIIMeta,
     jsii_type="cdk-aws-lambda-powertools-layer.LambdaPowertoolsLayer",
 ):
-    '''Defines a new Lambda Layer with Powertools for python library.'''
+    '''Defines a new Lambda Layer with Powertools for AWS Lambda (Python) library.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         compatible_architectures: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.Architecture]] = None,
@@ -175,15 +175,15 @@
         '''
         :param scope: -
         :param id: -
         :param compatible_architectures: The compatible architectures for the layer.
         :param include_extras: A flag for the extras dependencies (pydantic, aws-xray-sdk, etc.) This will increase the size of the layer significantly. If you don't use parsing, ignore it.
         :param layer_version_name: the name of the layer, will be randomised if empty.
         :param runtime_family: the runtime of the layer.
-        :param version: The powertools package version from pypi repository.
+        :param version: The Powertools for AWS Lambda package version from pypi repository.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d52989f8cfc13e7d6247276ec304b50ed3fbc22151b0a48e8e5aa9349cf367ef)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = PowertoolsLayerProps(
             compatible_architectures=compatible_architectures,
@@ -239,21 +239,21 @@
         *,
         compatible_architectures: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.Architecture]] = None,
         include_extras: typing.Optional[builtins.bool] = None,
         layer_version_name: typing.Optional[builtins.str] = None,
         runtime_family: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeFamily] = None,
         version: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Properties for Powertools layer for python.
+        '''Properties for Powertools for AWS Lambda (Python) Layer.
 
         :param compatible_architectures: The compatible architectures for the layer.
         :param include_extras: A flag for the extras dependencies (pydantic, aws-xray-sdk, etc.) This will increase the size of the layer significantly. If you don't use parsing, ignore it.
         :param layer_version_name: the name of the layer, will be randomised if empty.
         :param runtime_family: the runtime of the layer.
-        :param version: The powertools package version from pypi repository.
+        :param version: The Powertools for AWS Lambda package version from pypi repository.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__fccfc4c316e2527e42747269f47e940b83a85392bfaf4b6b9b041944ee2fcf4c)
             check_type(argname="argument compatible_architectures", value=compatible_architectures, expected_type=type_hints["compatible_architectures"])
             check_type(argname="argument include_extras", value=include_extras, expected_type=type_hints["include_extras"])
             check_type(argname="argument layer_version_name", value=layer_version_name, expected_type=type_hints["layer_version_name"])
             check_type(argname="argument runtime_family", value=runtime_family, expected_type=type_hints["runtime_family"])
@@ -296,15 +296,15 @@
     ) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeFamily]:
         '''the runtime of the layer.'''
         result = self._values.get("runtime_family")
         return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeFamily], result)
 
     @builtins.property
     def version(self) -> typing.Optional[builtins.str]:
-        '''The powertools package version from pypi repository.'''
+        '''The Powertools for AWS Lambda package version from pypi repository.'''
         result = self._values.get("version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer.egg-info/PKG-INFO` & `cdk-aws-lambda-powertools-layer-3.6.0/src/cdk_aws_lambda_powertools_layer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cdk-aws-lambda-powertools-layer
-Version: 3.5.0
-Summary: A lambda layer for AWS Powertools for python and typescript
+Version: 3.6.0
+Summary: Powertools for AWS Lambda layer for python and typescript
 Home-page: https://github.com/awslabs/cdk-aws-lambda-powertools-layer.git
 Author: Amazon Web Services
 License: MIT-0
 Project-URL: Source, https://github.com/awslabs/cdk-aws-lambda-powertools-layer.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
@@ -18,19 +18,19 @@
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# AWS Lambda powertools layer
+# Powertools for AWS Lambda Layer
 
 ## Why this project exists
 
-This is a custom construct that will create AWS Lambda Layer with AWS Powertools for Python or NodeJS library. There are different
+This is a custom construct that will create AWS Lambda Layer with Powertools for AWS Lambda for Python or NodeJS library. There are different
 ways how to create a layer and when working with CDK you need to install the library, create a zip file and wire it
 correctly. With this construct you don't have to care about packaging and dependency management. Create a construct
 and add it to your function. The construct is an extension of the
 existing [`LayerVersion`](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_lambda.LayerVersion.html) construct
 from the CDK library, so you have access to all fields and methods.
 
 > ⚠️ **This construct uses docker to build and bundle the dependencies!**
@@ -69,15 +69,15 @@
 pip install cdk-aws-lambda-powertools-layer
 ```
 
 ## Usage
 
 ### Python
 
-A single line will create a layer with powertools for python. For NodeJS you need to specifically set the `runtimeFamily: Runtime.NODEJS` property.
+A single line will create a layer with Powertools for AWS Lambda (Python). For NodeJS you need to specifically set the `runtimeFamily: Runtime.NODEJS` property.
 
 ```python
 from cdk_aws_lambda_powertools_layer import LambdaPowertoolsLayer
 
 powertoolsLayer = LambdaPowertoolsLayer(self, 'PowertoolsLayer')
 ```
```

### Comparing `cdk-aws-lambda-powertools-layer-3.5.0/src/cdk_aws_lambda_powertools_layer.egg-info/SOURCES.txt` & `cdk-aws-lambda-powertools-layer-3.6.0/src/cdk_aws_lambda_powertools_layer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_aws_lambda_powertools_layer/py.typed
 src/cdk_aws_lambda_powertools_layer.egg-info/PKG-INFO
 src/cdk_aws_lambda_powertools_layer.egg-info/SOURCES.txt
 src/cdk_aws_lambda_powertools_layer.egg-info/dependency_links.txt
 src/cdk_aws_lambda_powertools_layer.egg-info/requires.txt
 src/cdk_aws_lambda_powertools_layer.egg-info/top_level.txt
 src/cdk_aws_lambda_powertools_layer/_jsii/__init__.py
-src/cdk_aws_lambda_powertools_layer/_jsii/cdk-aws-lambda-powertools-layer@3.5.0.jsii.tgz
+src/cdk_aws_lambda_powertools_layer/_jsii/cdk-aws-lambda-powertools-layer@3.6.0.jsii.tgz
```

