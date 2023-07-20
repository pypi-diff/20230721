# Comparing `tmp/edgeimpulse-1.0.4.tar.gz` & `tmp/edgeimpulse-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgeimpulse-1.0.4.tar", max compression
+gzip compressed data, was "edgeimpulse-1.0.5.tar", max compression
```

## Comparing `edgeimpulse-1.0.4.tar` & `edgeimpulse-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1531 2023-05-18 14:34:09.032216 edgeimpulse-1.0.4/README.md
--rw-r--r--   0        0        0      297 2023-04-11 14:48:06.889249 edgeimpulse-1.0.4/edgeimpulse/__init__.py
--rw-r--r--   0        0        0     3017 2023-04-11 14:48:06.889354 edgeimpulse-1.0.4/edgeimpulse/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-17 15:56:20.819238 edgeimpulse-1.0.4/edgeimpulse/methods/__init__.py
--rw-r--r--   0        0        0    16925 2023-04-26 06:06:03.317877 edgeimpulse-1.0.4/edgeimpulse/methods/deploy.py
--rw-r--r--   0        0        0     7079 2023-04-24 08:52:27.286619 edgeimpulse-1.0.4/edgeimpulse/methods/profile.py
--rw-r--r--   0        0        0      313 2023-04-13 14:43:29.187994 edgeimpulse-1.0.4/edgeimpulse/model/__init__.py
--rw-r--r--   0        0        0      466 2023-04-03 13:45:58.875930 edgeimpulse-1.0.4/edgeimpulse/model/input_type.py
--rw-r--r--   0        0        0      673 2023-04-03 13:45:58.876012 edgeimpulse-1.0.4/edgeimpulse/model/model_info.py
--rw-r--r--   0        0        0      607 2023-04-03 13:45:58.876076 edgeimpulse-1.0.4/edgeimpulse/model/output_type.py
--rw-r--r--   0        0        0    15524 2023-04-24 08:52:27.286918 edgeimpulse-1.0.4/edgeimpulse/util.py
--rw-r--r--   0        0        0      803 2023-05-18 15:59:54.108649 edgeimpulse-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     2450 1970-01-01 00:00:00.000000 edgeimpulse-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1528 2023-07-20 23:35:17.959922 edgeimpulse-1.0.5/README.md
+-rw-r--r--   0        0        0      297 2023-07-20 23:35:17.959922 edgeimpulse-1.0.5/edgeimpulse/__init__.py
+-rw-r--r--   0        0        0     3017 2023-07-20 23:35:17.959922 edgeimpulse-1.0.5/edgeimpulse/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-20 23:35:17.959922 edgeimpulse-1.0.5/edgeimpulse/methods/__init__.py
+-rw-r--r--   0        0        0    17313 2023-07-20 23:35:17.959922 edgeimpulse-1.0.5/edgeimpulse/methods/deploy.py
+-rw-r--r--   0        0        0     7079 2023-07-20 23:35:17.959922 edgeimpulse-1.0.5/edgeimpulse/methods/profile.py
+-rw-r--r--   0        0        0      313 2023-07-20 23:35:17.959922 edgeimpulse-1.0.5/edgeimpulse/model/__init__.py
+-rw-r--r--   0        0        0     2144 2023-07-20 23:35:17.959922 edgeimpulse-1.0.5/edgeimpulse/model/input_type.py
+-rw-r--r--   0        0        0      673 2023-07-20 23:35:17.959922 edgeimpulse-1.0.5/edgeimpulse/model/model_info.py
+-rw-r--r--   0        0        0     2272 2023-07-20 23:35:17.959922 edgeimpulse-1.0.5/edgeimpulse/model/output_type.py
+-rw-r--r--   0        0        0    15524 2023-07-20 23:35:17.959922 edgeimpulse-1.0.5/edgeimpulse/util.py
+-rw-r--r--   0        0        0      804 2023-07-20 23:35:36.063612 edgeimpulse-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 edgeimpulse-1.0.5/PKG-INFO
```

### Comparing `edgeimpulse-1.0.4/README.md` & `edgeimpulse-1.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
     <a href="https://www.edgeimpulse.com/"><img src="https://events.edgeimpulse.com/hs-fs/hubfs/Edge%20Impulse%20Full%20Logo_RGB.png?width=1817&name=Edge%20Impulse%20Full%20Logo_RGB.png?raw=true" alt="Edge Impulse logo"/></a>
 </p>
 
 # Edge Impulse SDK
 
 The official Python SDK for Edge Impulse is designed to help machine learning practitioners build and deploy models for embedded hardware and edge AI applications.
 
- * Profile your model to estimate RAM, ROM, and inference speed
- * Convert your model to C++ to deploy on edge hardware
- * Interact with Edge Impulse projects to collect data, train models, and deploy them to edge devices
+- Profile your model to estimate RAM, ROM, and inference speed
+- Convert your model to C++ to deploy on edge hardware
+- Interact with Edge Impulse projects to collect data, train models, and deploy them to edge devices
 
 [Sign up for a free account →](https://studio.edgeimpulse.com/signup)
 
 ## Getting Started
 
 Install the Edge Impulse Python SDK:
 
@@ -33,10 +33,10 @@
 result.summary()
 ```
 
 To learn about the full functionality, see the resources below.
 
 ## Resources
 
-* [Overview and getting started](https://docs.edgeimpulse.com/docs/edge-impulse-python-sdk/overview)
-* [Tutorial demonstrating how to profile and deploy a model](https://docs.edgeimpulse.com/docs/edge-impulse-python-sdk/01-python-sdk-with-tf-keras)
-* [Reference guide](https://docs.edgeimpulse.com/reference/python-sdk/edgeimpulse)
+- [Overview and getting started](https://docs.edgeimpulse.com/docs/edge-impulse-python-sdk/overview)
+- [Tutorial demonstrating how to profile and deploy a model](https://docs.edgeimpulse.com/docs/edge-impulse-python-sdk/01-python-sdk-with-tf-keras)
+- [Reference guide](https://docs.edgeimpulse.com/reference/python-sdk/edgeimpulse)
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
                               [Edge_Impulse_logo]
 # Edge Impulse SDK The official Python SDK for Edge Impulse is designed to help
 machine learning practitioners build and deploy models for embedded hardware
-and edge AI applications. * Profile your model to estimate RAM, ROM, and
-inference speed * Convert your model to C++ to deploy on edge hardware *
+and edge AI applications. - Profile your model to estimate RAM, ROM, and
+inference speed - Convert your model to C++ to deploy on edge hardware -
 Interact with Edge Impulse projects to collect data, train models, and deploy
 them to edge devices [Sign up for a free account â](https://
 studio.edgeimpulse.com/signup) ## Getting Started Install the Edge Impulse
 Python SDK: ```sh pip install edgeimpulse ``` Estimate RAM, ROM, and inference
 speed for a variety of hardware platforms: ```python import edgeimpulse as ei #
 Change to an API key from your Edge Impulse project ei.API_KEY = "your-api-key"
 # Print inference estimates result = ei.model.profile(model="path/to/model")
 result.summary() ``` To learn about the full functionality, see the resources
-below. ## Resources * [Overview and getting started](https://
-docs.edgeimpulse.com/docs/edge-impulse-python-sdk/overview) * [Tutorial
+below. ## Resources - [Overview and getting started](https://
+docs.edgeimpulse.com/docs/edge-impulse-python-sdk/overview) - [Tutorial
 demonstrating how to profile and deploy a model](https://docs.edgeimpulse.com/
-docs/edge-impulse-python-sdk/01-python-sdk-with-tf-keras) * [Reference guide]
+docs/edge-impulse-python-sdk/01-python-sdk-with-tf-keras) - [Reference guide]
 (https://docs.edgeimpulse.com/reference/python-sdk/edgeimpulse)
```

### Comparing `edgeimpulse-1.0.4/edgeimpulse/exceptions.py` & `edgeimpulse-1.0.5/edgeimpulse/exceptions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse-1.0.4/edgeimpulse/methods/deploy.py` & `edgeimpulse-1.0.5/edgeimpulse/methods/deploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-import logging, re, os, tempfile
+import logging, re, os, tempfile, io
 from pathlib import Path
 
 from typing import Union, Optional, Any, List
 
 import edgeimpulse
 import pydantic
 
 from edgeimpulse.model.output_type import (
     Classification,
     Regression,
     ObjectDetection,
 )
 from edgeimpulse.model.input_type import (
+    ImageInput,
     AudioInput,
     TimeSeriesInput,
     OtherInput,
 )
 from edgeimpulse.exceptions import (
     InvalidTargetException,
     InvalidEngineException,
@@ -43,22 +44,22 @@
 from edgeimpulse_api.models.keras_model_type_enum import KerasModelTypeEnum
 from edgeimpulse_api.models.pretrained_model_tensor import PretrainedModelTensor
 
 
 def deploy(
     model: Union[Path, str, bytes, Any],
     model_output_type: Union[Classification, Regression, ObjectDetection],
-    model_input_type: Optional[Union[AudioInput, TimeSeriesInput, OtherInput]] = None,
+    model_input_type: Optional[Union[ImageInput, AudioInput, TimeSeriesInput, OtherInput]] = None,
     representative_data_for_quantization: Optional[Union[Path, str, bytes, Any]] = None,
     deploy_model_type: Optional[str] = None,
     engine: str = "tflite",
     deploy_target: str = "zip",
     output_directory: Optional[str] = None,
     api_key: Optional[str] = None,
-) -> bytes:
+) -> io.BytesIO:
     """Transforms a machine learning model into a library for an edge device
 
     Transforms a trained model into a library, package, or firmware ready to deploy on an embedded device. Can optionally
     apply post-training quantization if a representative data sample is uploaded.
 
     Supported model formats:
     * [Keras Model instance](https://www.tensorflow.org/api_docs/python/tf/keras/Model)
@@ -72,32 +73,32 @@
     * Must be representative of the range (maximum and minimum) of values in your training data.
 
     Args:
         model (Union[Path, str, bytes, Any]): A machine learning model, or similarly represented computational graph.
             Can be `Path` or `str` denoting file path, Python `bytes` containing a model, or a Keras model instance.
         model_output_type (Union[Classification, Regression, ObjectDetection]): Describe your model's type:
             Classification, Regression, or ObjectDetection. The types are available in the module `edgeimpulse.model.output_type`.
-        model_input_type (Union[AudioInput, TimeSeriesInput, OtherInput], optional): Determines any input preprocessing
+        model_input_type (Union[ImageInput, AudioInput, TimeSeriesInput, OtherInput], optional): Determines any input preprocessing
             (windowing, downsampling) that should be performed by the resulting library. The types are available
             in `edgeimpulse.model.input_type`. The default is no preprocessing.
         representative_data_for_quantization: A numpy representative input dataset. Accepts either an in memory numpy
             array or the Path/str filename of a np.save .npy file.
         deploy_model_type (str, optional): Use `int8` to receive an 8-bit quantized model, `float32` for
             non-quantized. Defaults to None, in which case it will become `int8` if representative_data_for_quantization if provided and `float32` otherwise. For other values see `edgeimpulse.model.list_model_types()`.
         engine (str, optional): Inference engine. Either `tflite` (for TensorFlow Lite for Microcontrollers)
             or `tflite-eon` (for EON Compiler) to output a portable C++ library. For all engines, call `edgeimpulse.deploy.list_engines()`. Defaults to `tflite`.
         deploy_target (str, optional): Target to deploy to, defaulting to a portable C++ library suitable for
             most devices. See `edgeimpulse.model.list_deployment_targets()` for a list.
         output_directory (str, optional): Directory to write deployment artifact to. File name may vary depending
             on deployment type. Defaults to None in which case model will not be written to file.
         api_key (str, optional): The API key for an Edge Impulse project. This can also be set via the module-level
             variable `edgeimpulse.API_KEY`, or the env var `EI_API_KEY`.
-    
+
     Returns:
-        bytes: Binary representation of deployment output.
+        BytesIO: A stream containing a binary representation of the deployment output.
 
     Raises:
         InvalidAuthTypeException: Incorrect authentication type was provided.
         InvalidDeployParameterException: Unacceptable parameter given to deploy function.
         InvalidEngineException: Unacceptable engine for this target.
         InvalidTargetException: Unacceptable deploy_target for this project.
         FileNotFoundError: Model file could not be loaded.
@@ -121,15 +122,21 @@
                             model_output_type=ei.model.output_type.Regression())
 
             # Quantize a model to int8 during deployment by passing a numpy array of data
             ei.model.deploy(model=keras_model,
                             representative_data_for_quantization=x_test,
                             model_output_type=ei.model.output_type.Classification(),
                             output_directory=".")
-    
+
+            # The function returns a BytesIO which can be written as desired
+            output = ei.model.deploy(model=keras_model,
+                                     model_output_type=ei.model.output_type.Classification())
+            with open('destination.zip', 'wb') as f:
+                f.write(output.read())
+
     """
 
     if model_input_type is None:
         model_input_type = OtherInput()
 
     if deploy_model_type is not None and deploy_model_type not in list_model_types():
         raise InvalidDeployParameterException(
@@ -260,48 +267,48 @@
             logging.info(f"Writing out to {output_path}")
             with open(output_path, "wb") as f:
                 f.write(response.data)
         except Exception as e:
             logging.debug(f"Exception saving output to '{output_path}' [{str(e)}]")
             raise e
 
-    return response.data
+    return io.BytesIO(response.data)
 
 
 def list_deployment_targets(api_key: Optional[str] = None) -> "List[str]":
     """Lists suitable deployment targets for the project associated with configured or provided api key.
 
     Args:
-        api_key (str, optional): The API key for an Edge Impulse project. 
+        api_key (str, optional): The API key for an Edge Impulse project.
             This can also be set via the module-level variable `edgeimpulse.API_KEY`, or the env var `EI_API_KEY`.
 
     Returns:
         List[str]: List of deploy targets for project
-    
+
     """
     client = configure_generic_client(
         key=api_key if api_key else edgeimpulse.API_KEY,
         host=edgeimpulse.API_ENDPOINT,
     )
     return get_project_deploy_targets(client)
 
 
 def list_engines() -> "List[str]":
     """Lists all the engines that can be passed to `deploy()`'s `engine` parameter.
 
     Returns:
         List[str]: List of engines
-    
+
     """
     return [e.value for e in DeploymentTargetEngine]
 
 
 def list_model_types() -> "List[str]":
     """Lists all the model types that can passed to `deploy()`'s `deploy_model_type` parameter.
-    
+
     Returns:
         List[str]: List of model types
 
     """
     return [t.value for t in KerasModelTypeEnum]
```

### Comparing `edgeimpulse-1.0.4/edgeimpulse/methods/profile.py` & `edgeimpulse-1.0.5/edgeimpulse/methods/profile.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse-1.0.4/edgeimpulse/model/model_info.py` & `edgeimpulse-1.0.5/edgeimpulse/model/model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse-1.0.4/edgeimpulse/util.py` & `edgeimpulse-1.0.5/edgeimpulse/util.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse-1.0.4/pyproject.toml` & `edgeimpulse-1.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "edgeimpulse"
-version = "1.0.4"
+version = "1.0.5"
 description = "Python SDK for Edge Impulse."
 authors = ["EdgeImpulse Inc. <hello@edgeimpulse.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://edgeimpulse.com"
 documentation = "https://docs.edgeimpulse.com/docs/edge-impulse-python-sdk/overview"
 classifiers = [
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Embedded Systems"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-edgeimpulse-api = "^1.23.6"
+edgeimpulse-api = "^1.25.31"
 
 [tool.poetry.dev-dependencies]
 sphinx = "5.3.0"
 sphinx-markdown-builder = "0.5.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `edgeimpulse-1.0.4/PKG-INFO` & `edgeimpulse-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgeimpulse
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python SDK for Edge Impulse.
 Home-page: https://edgeimpulse.com
 License: Apache-2.0
 Author: EdgeImpulse Inc.
 Author-email: hello@edgeimpulse.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,29 +12,29 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Embedded Systems
-Requires-Dist: edgeimpulse-api (>=1.23.6,<2.0.0)
+Requires-Dist: edgeimpulse-api (>=1.25.31,<2.0.0)
 Project-URL: Documentation, https://docs.edgeimpulse.com/docs/edge-impulse-python-sdk/overview
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a href="https://www.edgeimpulse.com/"><img src="https://events.edgeimpulse.com/hs-fs/hubfs/Edge%20Impulse%20Full%20Logo_RGB.png?width=1817&name=Edge%20Impulse%20Full%20Logo_RGB.png?raw=true" alt="Edge Impulse logo"/></a>
 </p>
 
 # Edge Impulse SDK
 
 The official Python SDK for Edge Impulse is designed to help machine learning practitioners build and deploy models for embedded hardware and edge AI applications.
 
- * Profile your model to estimate RAM, ROM, and inference speed
- * Convert your model to C++ to deploy on edge hardware
- * Interact with Edge Impulse projects to collect data, train models, and deploy them to edge devices
+- Profile your model to estimate RAM, ROM, and inference speed
+- Convert your model to C++ to deploy on edge hardware
+- Interact with Edge Impulse projects to collect data, train models, and deploy them to edge devices
 
 [Sign up for a free account →](https://studio.edgeimpulse.com/signup)
 
 ## Getting Started
 
 Install the Edge Impulse Python SDK:
 
@@ -55,11 +55,11 @@
 result.summary()
 ```
 
 To learn about the full functionality, see the resources below.
 
 ## Resources
 
-* [Overview and getting started](https://docs.edgeimpulse.com/docs/edge-impulse-python-sdk/overview)
-* [Tutorial demonstrating how to profile and deploy a model](https://docs.edgeimpulse.com/docs/edge-impulse-python-sdk/01-python-sdk-with-tf-keras)
-* [Reference guide](https://docs.edgeimpulse.com/reference/python-sdk/edgeimpulse)
+- [Overview and getting started](https://docs.edgeimpulse.com/docs/edge-impulse-python-sdk/overview)
+- [Tutorial demonstrating how to profile and deploy a model](https://docs.edgeimpulse.com/docs/edge-impulse-python-sdk/01-python-sdk-with-tf-keras)
+- [Reference guide](https://docs.edgeimpulse.com/reference/python-sdk/edgeimpulse)
```

#### html2text {}

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1 Name: edgeimpulse Version: 1.0.4 Summary: Python SDK for
+Metadata-Version: 2.1 Name: edgeimpulse Version: 1.0.5 Summary: Python SDK for
 Edge Impulse. Home-page: https://edgeimpulse.com License: Apache-2.0 Author:
 EdgeImpulse Inc. Author-email: hello@edgeimpulse.com Requires-Python:
 >=3.7,<4.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Embedded Systems Requires-Dist:
-edgeimpulse-api (>=1.23.6,<2.0.0) Project-URL: Documentation, https://
+edgeimpulse-api (>=1.25.31,<2.0.0) Project-URL: Documentation, https://
 docs.edgeimpulse.com/docs/edge-impulse-python-sdk/overview Description-Content-
 Type: text/markdown
                               [Edge_Impulse_logo]
 # Edge Impulse SDK The official Python SDK for Edge Impulse is designed to help
 machine learning practitioners build and deploy models for embedded hardware
-and edge AI applications. * Profile your model to estimate RAM, ROM, and
-inference speed * Convert your model to C++ to deploy on edge hardware *
+and edge AI applications. - Profile your model to estimate RAM, ROM, and
+inference speed - Convert your model to C++ to deploy on edge hardware -
 Interact with Edge Impulse projects to collect data, train models, and deploy
 them to edge devices [Sign up for a free account â](https://
 studio.edgeimpulse.com/signup) ## Getting Started Install the Edge Impulse
 Python SDK: ```sh pip install edgeimpulse ``` Estimate RAM, ROM, and inference
 speed for a variety of hardware platforms: ```python import edgeimpulse as ei #
 Change to an API key from your Edge Impulse project ei.API_KEY = "your-api-key"
 # Print inference estimates result = ei.model.profile(model="path/to/model")
 result.summary() ``` To learn about the full functionality, see the resources
-below. ## Resources * [Overview and getting started](https://
-docs.edgeimpulse.com/docs/edge-impulse-python-sdk/overview) * [Tutorial
+below. ## Resources - [Overview and getting started](https://
+docs.edgeimpulse.com/docs/edge-impulse-python-sdk/overview) - [Tutorial
 demonstrating how to profile and deploy a model](https://docs.edgeimpulse.com/
-docs/edge-impulse-python-sdk/01-python-sdk-with-tf-keras) * [Reference guide]
+docs/edge-impulse-python-sdk/01-python-sdk-with-tf-keras) - [Reference guide]
 (https://docs.edgeimpulse.com/reference/python-sdk/edgeimpulse)
```

