# Comparing `tmp/dagster-wandb-0.19.9rc0.tar.gz` & `tmp/dagster-wandb-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-wandb-0.19.9rc0.tar", last modified: Thu Jun  8 18:31:09 2023, max compression
+gzip compressed data, was "dagster-wandb-0.20.0.tar", last modified: Thu Jul 20 22:04:09 2023, max compression
```

## Comparing `dagster-wandb-0.19.9rc0.tar` & `dagster-wandb-0.20.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:09.853053 dagster-wandb-0.19.9rc0/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      682 2023-06-08 18:31:09.853053 dagster-wandb-0.19.9rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:09.849053 dagster-wandb-0.19.9rc0/dagster_wandb/
--rw-r--r--   0 root         (0) root         (0)      613 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/dagster_wandb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33673 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/dagster_wandb/io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:09.849053 dagster-wandb-0.19.9rc0/dagster_wandb/launch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/dagster_wandb/launch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4425 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/dagster_wandb/launch/configs.py
--rw-r--r--   0 root         (0) root         (0)     5192 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/dagster_wandb/launch/ops.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/dagster_wandb/py.typed
--rw-r--r--   0 root         (0) root         (0)     2157 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/dagster_wandb/resources.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/dagster_wandb/types.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/dagster_wandb/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:09.849053 dagster-wandb-0.19.9rc0/dagster_wandb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      682 2023-06-08 18:31:09.000000 dagster-wandb-0.19.9rc0/dagster_wandb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      513 2023-06-08 18:31:09.000000 dagster-wandb-0.19.9rc0/dagster_wandb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:31:09.000000 dagster-wandb-0.19.9rc0/dagster_wandb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:31:09.000000 dagster-wandb-0.19.9rc0/dagster_wandb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       78 2023-06-08 18:31:09.000000 dagster-wandb-0.19.9rc0/dagster_wandb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-08 18:31:09.000000 dagster-wandb-0.19.9rc0/dagster_wandb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      160 2023-06-08 18:31:09.853053 dagster-wandb-0.19.9rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1371 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:09.195850 dagster-wandb-0.20.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      629 2023-07-20 22:04:09.195850 dagster-wandb-0.20.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      150 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:09.191850 dagster-wandb-0.20.0/dagster_wandb/
+-rw-r--r--   0 root         (0) root         (0)      613 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/dagster_wandb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34007 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/dagster_wandb/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:09.191850 dagster-wandb-0.20.0/dagster_wandb/launch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/dagster_wandb/launch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4425 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/dagster_wandb/launch/configs.py
+-rw-r--r--   0 root         (0) root         (0)     5192 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/dagster_wandb/launch/ops.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/dagster_wandb/py.typed
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/dagster_wandb/resources.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/dagster_wandb/types.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/dagster_wandb/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:09.191850 dagster-wandb-0.20.0/dagster_wandb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-07-20 22:04:09.000000 dagster-wandb-0.20.0/dagster_wandb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      513 2023-07-20 22:04:09.000000 dagster-wandb-0.20.0/dagster_wandb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:04:09.000000 dagster-wandb-0.20.0/dagster_wandb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:04:09.000000 dagster-wandb-0.20.0/dagster_wandb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       75 2023-07-20 22:04:09.000000 dagster-wandb-0.20.0/dagster_wandb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-20 22:04:09.000000 dagster-wandb-0.20.0/dagster_wandb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      160 2023-07-20 22:04:09.195850 dagster-wandb-0.20.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1319 2023-07-20 21:53:16.000000 dagster-wandb-0.20.0/setup.py
```

### Comparing `dagster-wandb-0.19.9rc0/LICENSE` & `dagster-wandb-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.19.9rc0/PKG-INFO` & `dagster-wandb-0.20.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-wandb
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for wandb Dagster components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-wandb
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
 Provides-Extra: dev
```

### Comparing `dagster-wandb-0.19.9rc0/dagster_wandb/__init__.py` & `dagster-wandb-0.20.0/dagster_wandb/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.19.9rc0/dagster_wandb/io_manager.py` & `dagster-wandb-0.20.0/dagster_wandb/io_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     Int,
     IOManager,
     MetadataValue,
     OutputContext,
     String,
     io_manager,
 )
+from dagster._core.storage.io_manager import dagster_maintained_io_manager
 from wandb.sdk.data_types.base_types.wb_value import WBValue
 from wandb.sdk.wandb_artifacts import Artifact
 
 from .resources import WANDB_CLOUD_HOST
 from .version import __version__
 
 if sys.version_info >= (3, 8):
@@ -266,14 +267,18 @@
                             " an @op. Alternatively you can use an @asset."
                         )
                     artifact_name = parameters.get("name")
 
                 if context.has_partition_key:
                     artifact_name = f"{artifact_name}.{context.partition_key}"
 
+                # We replace the | character with - because it is not allowed in artifact names
+                # The | character is used in multi-dimensional partition keys
+                artifact_name = str(artifact_name).replace("|", "-")
+
                 # Creates an artifact to hold the obj
                 artifact = self.wandb.Artifact(
                     name=artifact_name,
                     type=artifact_type,
                     description=artifact_description,
                     metadata=artifact_metadata,
                 )
@@ -576,14 +581,15 @@
             return self._download_artifact(context)
         except WandbArtifactsIOManagerError as exception:
             raise exception
         except Exception as exception:
             raise WandbArtifactsIOManagerError() from exception
 
 
+@dagster_maintained_io_manager
 @io_manager(
     required_resource_keys={"wandb_resource", "wandb_config"},
     description="IO manager to read and write W&B Artifacts",
     config_schema={
         "run_name": Field(
             String,
             is_required=False,
@@ -723,11 +729,11 @@
         "dagster_run_id": dagster_run_id or "",
         "wandb_host": wandb_host,
         "wandb_entity": wandb_entity,
         "wandb_project": wandb_project,
         "wandb_run_name": wandb_run_name,
         "wandb_run_id": wandb_run_id,
         "wandb_run_tags": wandb_run_tags,
-        "base_dir": base_dir,  # type: ignore
+        "base_dir": base_dir,
         "cache_duration_in_minutes": cache_duration_in_minutes,
     }
     return ArtifactsIOManager(wandb_client, config)
```

### Comparing `dagster-wandb-0.19.9rc0/dagster_wandb/launch/configs.py` & `dagster-wandb-0.20.0/dagster_wandb/launch/configs.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.19.9rc0/dagster_wandb/launch/ops.py` & `dagster-wandb-0.20.0/dagster_wandb/launch/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.19.9rc0/dagster_wandb/resources.py` & `dagster-wandb-0.20.0/dagster_wandb/resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from typing import Any, Dict
 
 import wandb
 from dagster import Field, InitResourceContext, String, StringSource, resource
+from dagster._core.definitions.resource_definition import dagster_maintained_resource
 from wandb.sdk.internal.internal_api import Api
 
 WANDB_CLOUD_HOST: str = "https://api.wandb.ai"
 
 
+@dagster_maintained_resource
 @resource(
     config_schema={
         "api_key": Field(
             StringSource,
             description="W&B API key necessary to communicate with the W&B API.",
             is_required=True,
         ),
```

### Comparing `dagster-wandb-0.19.9rc0/dagster_wandb/types.py` & `dagster-wandb-0.20.0/dagster_wandb/types.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.19.9rc0/dagster_wandb.egg-info/PKG-INFO` & `dagster-wandb-0.20.0/dagster_wandb.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-wandb
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for wandb Dagster components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-wandb
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
 Provides-Extra: dev
```

### Comparing `dagster-wandb-0.19.9rc0/dagster_wandb.egg-info/SOURCES.txt` & `dagster-wandb-0.20.0/dagster_wandb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.19.9rc0/setup.py` & `dagster-wandb-0.20.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,23 +20,22 @@
     version=get_version(),
     author="Elementl",
     author_email="hello@elementl.com",
     license="Apache-2.0",
     description="Package for wandb Dagster components.",
     url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-wandb",
     classifiers=[
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_wandb_tests*"]),
     install_requires=[
-        "dagster==1.3.9rc0",
+        "dagster==1.4.0",
         "wandb>=0.13.5,<0.15.4",
     ],
     extras_require={"dev": ["cloudpickle", "joblib", "callee", "dill"]},
     zip_safe=False,
 )
```

