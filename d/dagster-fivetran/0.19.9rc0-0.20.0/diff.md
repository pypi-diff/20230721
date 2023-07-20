# Comparing `tmp/dagster-fivetran-0.19.9rc0.tar.gz` & `tmp/dagster-fivetran-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-fivetran-0.19.9rc0.tar", last modified: Thu Jun  8 18:29:34 2023, max compression
+gzip compressed data, was "dagster-fivetran-0.20.0.tar", last modified: Thu Jul 20 22:02:02 2023, max compression
```

## Comparing `dagster-fivetran-0.19.9rc0.tar` & `dagster-fivetran-0.20.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:34.079712 dagster-fivetran-0.19.9rc0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-fivetran-0.19.9rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       68 2023-06-08 18:20:46.000000 dagster-fivetran-0.19.9rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      701 2023-06-08 18:29:34.079712 dagster-fivetran-0.19.9rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      134 2023-06-08 18:20:46.000000 dagster-fivetran-0.19.9rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:34.079712 dagster-fivetran-0.19.9rc0/dagster_fivetran/
--rw-r--r--   0 root         (0) root         (0)      854 2023-06-08 18:20:46.000000 dagster-fivetran-0.19.9rc0/dagster_fivetran/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20552 2023-06-08 18:20:46.000000 dagster-fivetran-0.19.9rc0/dagster_fivetran/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)      426 2023-06-08 18:20:46.000000 dagster-fivetran-0.19.9rc0/dagster_fivetran/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:34.079712 dagster-fivetran-0.19.9rc0/dagster_fivetran/managed/
--rw-r--r--   0 root         (0) root         (0)      212 2023-06-08 18:20:46.000000 dagster-fivetran-0.19.9rc0/dagster_fivetran/managed/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14474 2023-06-08 18:20:46.000000 dagster-fivetran-0.19.9rc0/dagster_fivetran/managed/reconciliation.py
--rw-r--r--   0 root         (0) root         (0)     3258 2023-06-08 18:20:46.000000 dagster-fivetran-0.19.9rc0/dagster_fivetran/managed/types.py
--rw-r--r--   0 root         (0) root         (0)     7139 2023-06-08 18:20:46.000000 dagster-fivetran-0.19.9rc0/dagster_fivetran/ops.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 18:20:46.000000 dagster-fivetran-0.19.9rc0/dagster_fivetran/py.typed
--rw-r--r--   0 root         (0) root         (0)    18113 2023-06-08 18:20:46.000000 dagster-fivetran-0.19.9rc0/dagster_fivetran/resources.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-06-08 18:20:46.000000 dagster-fivetran-0.19.9rc0/dagster_fivetran/types.py
--rw-r--r--   0 root         (0) root         (0)     2994 2023-06-08 18:20:46.000000 dagster-fivetran-0.19.9rc0/dagster_fivetran/utils.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-fivetran-0.19.9rc0/dagster_fivetran/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:34.079712 dagster-fivetran-0.19.9rc0/dagster_fivetran.egg-info/
--rw-r--r--   0 root         (0) root         (0)      701 2023-06-08 18:29:33.000000 dagster-fivetran-0.19.9rc0/dagster_fivetran.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      687 2023-06-08 18:29:34.000000 dagster-fivetran-0.19.9rc0/dagster_fivetran.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:29:33.000000 dagster-fivetran-0.19.9rc0/dagster_fivetran.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-08 18:29:33.000000 dagster-fivetran-0.19.9rc0/dagster_fivetran.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:29:33.000000 dagster-fivetran-0.19.9rc0/dagster_fivetran.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-08 18:29:33.000000 dagster-fivetran-0.19.9rc0/dagster_fivetran.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-08 18:29:33.000000 dagster-fivetran-0.19.9rc0/dagster_fivetran.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      163 2023-06-08 18:29:34.083713 dagster-fivetran-0.19.9rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1497 2023-06-08 18:20:46.000000 dagster-fivetran-0.19.9rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:02.666084 dagster-fivetran-0.20.0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-20 21:53:16.000000 dagster-fivetran-0.20.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       68 2023-07-20 21:53:16.000000 dagster-fivetran-0.20.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      648 2023-07-20 22:02:02.666084 dagster-fivetran-0.20.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      134 2023-07-20 21:53:16.000000 dagster-fivetran-0.20.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:02.662084 dagster-fivetran-0.20.0/dagster_fivetran/
+-rw-r--r--   0 root         (0) root         (0)      854 2023-07-20 21:53:16.000000 dagster-fivetran-0.20.0/dagster_fivetran/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20478 2023-07-20 21:53:16.000000 dagster-fivetran-0.20.0/dagster_fivetran/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)      426 2023-07-20 21:53:16.000000 dagster-fivetran-0.20.0/dagster_fivetran/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:02.662084 dagster-fivetran-0.20.0/dagster_fivetran/managed/
+-rw-r--r--   0 root         (0) root         (0)      212 2023-07-20 21:53:16.000000 dagster-fivetran-0.20.0/dagster_fivetran/managed/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14474 2023-07-20 21:53:16.000000 dagster-fivetran-0.20.0/dagster_fivetran/managed/reconciliation.py
+-rw-r--r--   0 root         (0) root         (0)     3258 2023-07-20 21:53:16.000000 dagster-fivetran-0.20.0/dagster_fivetran/managed/types.py
+-rw-r--r--   0 root         (0) root         (0)     7139 2023-07-20 21:53:16.000000 dagster-fivetran-0.20.0/dagster_fivetran/ops.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-20 21:53:16.000000 dagster-fivetran-0.20.0/dagster_fivetran/py.typed
+-rw-r--r--   0 root         (0) root         (0)    18311 2023-07-20 21:53:16.000000 dagster-fivetran-0.20.0/dagster_fivetran/resources.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-07-20 21:53:16.000000 dagster-fivetran-0.20.0/dagster_fivetran/types.py
+-rw-r--r--   0 root         (0) root         (0)     2994 2023-07-20 21:53:16.000000 dagster-fivetran-0.20.0/dagster_fivetran/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-fivetran-0.20.0/dagster_fivetran/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:02.662084 dagster-fivetran-0.20.0/dagster_fivetran.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      648 2023-07-20 22:02:02.000000 dagster-fivetran-0.20.0/dagster_fivetran.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      687 2023-07-20 22:02:02.000000 dagster-fivetran-0.20.0/dagster_fivetran.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:02:02.000000 dagster-fivetran-0.20.0/dagster_fivetran.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-20 22:02:02.000000 dagster-fivetran-0.20.0/dagster_fivetran.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:02:02.000000 dagster-fivetran-0.20.0/dagster_fivetran.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-20 22:02:02.000000 dagster-fivetran-0.20.0/dagster_fivetran.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-20 22:02:02.000000 dagster-fivetran-0.20.0/dagster_fivetran.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2023-07-20 22:02:02.666084 dagster-fivetran-0.20.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-07-20 21:53:16.000000 dagster-fivetran-0.20.0/setup.py
```

### Comparing `dagster-fivetran-0.19.9rc0/LICENSE` & `dagster-fivetran-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.19.9rc0/PKG-INFO` & `dagster-fivetran-0.20.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-fivetran
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for integrating Fivetran with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-fivetran
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
 Provides-Extra: managed
```

### Comparing `dagster-fivetran-0.19.9rc0/dagster_fivetran/__init__.py` & `dagster-fivetran-0.20.0/dagster_fivetran/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.19.9rc0/dagster_fivetran/asset_defs.py` & `dagster-fivetran-0.20.0/dagster_fivetran/asset_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     AssetsDefinition,
     Nothing,
     OpExecutionContext,
     Output,
     _check as check,
     multi_asset,
 )
-from dagster._annotations import experimental
 from dagster._core.definitions.cacheable_assets import (
     AssetsDefinitionCacheableData,
     CacheableAssetsDefinition,
 )
 from dagster._core.definitions.events import CoercibleToAssetKeyPrefix
 from dagster._core.definitions.metadata import MetadataUserInput
 from dagster._core.definitions.resource_definition import ResourceDefinition
@@ -130,15 +129,14 @@
                     step_key=context.get_step_execution_context().step.key,
                     output_name=output_name,
                 )
 
     return [_assets]
 
 
-@experimental
 def build_fivetran_assets(
     connector_id: str,
     destination_tables: Sequence[str],
     poll_interval: float = DEFAULT_POLL_INTERVAL,
     poll_timeout: Optional[float] = None,
     io_manager_key: Optional[str] = None,
     asset_key_prefix: Optional[Sequence[str]] = None,
@@ -411,15 +409,14 @@
 
 
 def _clean_name(name: str) -> str:
     """Cleans an input to be a valid Dagster asset name."""
     return re.sub(r"[^a-z0-9]+", "_", name.lower())
 
 
-@experimental
 def load_assets_from_fivetran_instance(
     fivetran: Union[FivetranResource, ResourceDefinition],
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     connector_to_group_fn: Optional[Callable[[str], Optional[str]]] = _clean_name,
     io_manager_key: Optional[str] = None,
     connector_to_io_manager_key_fn: Optional[Callable[[str], Optional[str]]] = None,
     connector_filter: Optional[Callable[[FivetranConnectionMetadata], bool]] = None,
```

### Comparing `dagster-fivetran-0.19.9rc0/dagster_fivetran/managed/reconciliation.py` & `dagster-fivetran-0.20.0/dagster_fivetran/managed/reconciliation.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.19.9rc0/dagster_fivetran/managed/types.py` & `dagster-fivetran-0.20.0/dagster_fivetran/managed/types.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.19.9rc0/dagster_fivetran/ops.py` & `dagster-fivetran-0.20.0/dagster_fivetran/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.19.9rc0/dagster_fivetran/resources.py` & `dagster-fivetran-0.20.0/dagster_fivetran/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     MetadataValue,
     __version__,
     _check as check,
     get_dagster_logger,
     resource,
 )
 from dagster._config.pythonic_config import ConfigurableResource
+from dagster._core.definitions.resource_definition import dagster_maintained_resource
 from dagster._utils.cached_method import cached_method
 from dateutil import parser
 from pydantic import Field
 from requests.auth import HTTPBasicAuth
 from requests.exceptions import RequestException
 
 from dagster_fivetran.types import FivetranOutput
@@ -53,14 +54,18 @@
         ),
     )
     request_retry_delay: float = Field(
         default=0.25,
         description="Time (in seconds) to wait between each request retry.",
     )
 
+    @classmethod
+    def _is_dagster_maintained(cls) -> bool:
+        return True
+
     @property
     def _auth(self) -> HTTPBasicAuth:
         return HTTPBasicAuth(self.api_key, self.api_secret)
 
     @property
     @cached_method
     def _log(self) -> logging.Logger:
@@ -387,14 +392,15 @@
             init_last_sync_timestamp,
             poll_interval=poll_interval,
             poll_timeout=poll_timeout,
         )
         return FivetranOutput(connector_details=final_details, schema_config=schema_config)
 
 
+@dagster_maintained_resource
 @resource(config_schema=FivetranResource.to_config_schema())
 def fivetran_resource(context: InitResourceContext) -> FivetranResource:
     """This resource allows users to programatically interface with the Fivetran REST API to launch
     syncs and monitor their progress. This currently implements only a subset of the functionality
     exposed by the API.
 
     For a complete set of documentation on the Fivetran REST API, including expected response JSON
```

### Comparing `dagster-fivetran-0.19.9rc0/dagster_fivetran/types.py` & `dagster-fivetran-0.20.0/dagster_fivetran/types.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.19.9rc0/dagster_fivetran/utils.py` & `dagster-fivetran-0.20.0/dagster_fivetran/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.19.9rc0/dagster_fivetran.egg-info/PKG-INFO` & `dagster-fivetran-0.20.0/dagster_fivetran.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-fivetran
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for integrating Fivetran with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-fivetran
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
 Provides-Extra: managed
```

### Comparing `dagster-fivetran-0.19.9rc0/dagster_fivetran.egg-info/SOURCES.txt` & `dagster-fivetran-0.20.0/dagster_fivetran.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.19.9rc0/setup.py` & `dagster-fivetran-0.20.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,29 +20,28 @@
     version=ver,
     author="Elementl",
     author_email="hello@elementl.com",
     license="Apache-2.0",
     description="Package for integrating Fivetran with Dagster.",
     url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-fivetran",
     classifiers=[
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_fivetran_tests*"]),
-    install_requires=["dagster==1.3.9rc0"],
+    install_requires=["dagster==1.4.0"],
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "dagster-fivetran = dagster_fivetran.cli:main",
         ]
     },
     extras_require={
         "managed": [
-            "dagster-managed-elements==0.19.9rc0",
+            "dagster-managed-elements==0.20.0",
         ],
     },
 )
```

