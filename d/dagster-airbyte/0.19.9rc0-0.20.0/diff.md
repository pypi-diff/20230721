# Comparing `tmp/dagster-airbyte-0.19.9rc0.tar.gz` & `tmp/dagster-airbyte-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-airbyte-0.19.9rc0.tar", last modified: Thu Jun  8 18:29:15 2023, max compression
+gzip compressed data, was "dagster-airbyte-0.20.0.tar", last modified: Thu Jul 20 22:01:06 2023, max compression
```

## Comparing `dagster-airbyte-0.19.9rc0.tar` & `dagster-airbyte-0.20.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:15.419452 dagster-airbyte-0.19.9rc0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-airbyte-0.19.9rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-08 18:20:46.000000 dagster-airbyte-0.19.9rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      719 2023-06-08 18:29:15.419452 dagster-airbyte-0.19.9rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2023-06-08 18:20:46.000000 dagster-airbyte-0.19.9rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:15.415452 dagster-airbyte-0.19.9rc0/dagster_airbyte/
--rw-r--r--   0 root         (0) root         (0)     1215 2023-06-08 18:20:46.000000 dagster-airbyte-0.19.9rc0/dagster_airbyte/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43942 2023-06-08 18:20:46.000000 dagster-airbyte-0.19.9rc0/dagster_airbyte/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)      425 2023-06-08 18:20:46.000000 dagster-airbyte-0.19.9rc0/dagster_airbyte/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:15.419452 dagster-airbyte-0.19.9rc0/dagster_airbyte/managed/
--rw-r--r--   0 root         (0) root         (0)      423 2023-06-08 18:20:46.000000 dagster-airbyte-0.19.9rc0/dagster_airbyte/managed/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:15.419452 dagster-airbyte-0.19.9rc0/dagster_airbyte/managed/generated/
--rw-r--r--   0 root         (0) root         (0)       76 2023-06-08 18:20:46.000000 dagster-airbyte-0.19.9rc0/dagster_airbyte/managed/generated/__init__.py
--rw-r--r--   0 root         (0) root         (0)   119751 2023-06-08 18:20:46.000000 dagster-airbyte-0.19.9rc0/dagster_airbyte/managed/generated/destinations.py
--rw-r--r--   0 root         (0) root         (0)   282784 2023-06-08 18:20:46.000000 dagster-airbyte-0.19.9rc0/dagster_airbyte/managed/generated/sources.py
--rw-r--r--   0 root         (0) root         (0)    33757 2023-06-08 18:20:46.000000 dagster-airbyte-0.19.9rc0/dagster_airbyte/managed/reconciliation.py
--rw-r--r--   0 root         (0) root         (0)    14161 2023-06-08 18:20:46.000000 dagster-airbyte-0.19.9rc0/dagster_airbyte/managed/types.py
--rw-r--r--   0 root         (0) root         (0)     4128 2023-06-08 18:20:46.000000 dagster-airbyte-0.19.9rc0/dagster_airbyte/ops.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 18:20:46.000000 dagster-airbyte-0.19.9rc0/dagster_airbyte/py.typed
--rw-r--r--   0 root         (0) root         (0)    26443 2023-06-08 18:20:46.000000 dagster-airbyte-0.19.9rc0/dagster_airbyte/resources.py
--rw-r--r--   0 root         (0) root         (0)     1434 2023-06-08 18:20:46.000000 dagster-airbyte-0.19.9rc0/dagster_airbyte/types.py
--rw-r--r--   0 root         (0) root         (0)     2633 2023-06-08 18:20:46.000000 dagster-airbyte-0.19.9rc0/dagster_airbyte/utils.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-airbyte-0.19.9rc0/dagster_airbyte/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:15.419452 dagster-airbyte-0.19.9rc0/dagster_airbyte.egg-info/
--rw-r--r--   0 root         (0) root         (0)      719 2023-06-08 18:29:15.000000 dagster-airbyte-0.19.9rc0/dagster_airbyte.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      809 2023-06-08 18:29:15.000000 dagster-airbyte-0.19.9rc0/dagster_airbyte.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:29:15.000000 dagster-airbyte-0.19.9rc0/dagster_airbyte.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-06-08 18:29:15.000000 dagster-airbyte-0.19.9rc0/dagster_airbyte.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:29:15.000000 dagster-airbyte-0.19.9rc0/dagster_airbyte.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       96 2023-06-08 18:29:15.000000 dagster-airbyte-0.19.9rc0/dagster_airbyte.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-08 18:29:15.000000 dagster-airbyte-0.19.9rc0/dagster_airbyte.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2023-06-08 18:29:15.423452 dagster-airbyte-0.19.9rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1599 2023-06-08 18:20:46.000000 dagster-airbyte-0.19.9rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:01:06.953291 dagster-airbyte-0.20.0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-20 21:53:16.000000 dagster-airbyte-0.20.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       67 2023-07-20 21:53:16.000000 dagster-airbyte-0.20.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      666 2023-07-20 22:01:06.953291 dagster-airbyte-0.20.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2023-07-20 21:53:16.000000 dagster-airbyte-0.20.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:01:06.941291 dagster-airbyte-0.20.0/dagster_airbyte/
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-07-20 21:53:16.000000 dagster-airbyte-0.20.0/dagster_airbyte/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44583 2023-07-20 21:53:16.000000 dagster-airbyte-0.20.0/dagster_airbyte/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)      425 2023-07-20 21:53:16.000000 dagster-airbyte-0.20.0/dagster_airbyte/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:01:06.941291 dagster-airbyte-0.20.0/dagster_airbyte/managed/
+-rw-r--r--   0 root         (0) root         (0)      423 2023-07-20 21:53:16.000000 dagster-airbyte-0.20.0/dagster_airbyte/managed/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:01:06.945291 dagster-airbyte-0.20.0/dagster_airbyte/managed/generated/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-07-20 21:53:16.000000 dagster-airbyte-0.20.0/dagster_airbyte/managed/generated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   119751 2023-07-20 21:53:16.000000 dagster-airbyte-0.20.0/dagster_airbyte/managed/generated/destinations.py
+-rw-r--r--   0 root         (0) root         (0)   282784 2023-07-20 21:53:16.000000 dagster-airbyte-0.20.0/dagster_airbyte/managed/generated/sources.py
+-rw-r--r--   0 root         (0) root         (0)    33752 2023-07-20 21:53:16.000000 dagster-airbyte-0.20.0/dagster_airbyte/managed/reconciliation.py
+-rw-r--r--   0 root         (0) root         (0)    14161 2023-07-20 21:53:16.000000 dagster-airbyte-0.20.0/dagster_airbyte/managed/types.py
+-rw-r--r--   0 root         (0) root         (0)     4128 2023-07-20 21:53:16.000000 dagster-airbyte-0.20.0/dagster_airbyte/ops.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-20 21:53:16.000000 dagster-airbyte-0.20.0/dagster_airbyte/py.typed
+-rw-r--r--   0 root         (0) root         (0)    26670 2023-07-20 21:53:16.000000 dagster-airbyte-0.20.0/dagster_airbyte/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1434 2023-07-20 21:53:16.000000 dagster-airbyte-0.20.0/dagster_airbyte/types.py
+-rw-r--r--   0 root         (0) root         (0)     2633 2023-07-20 21:53:16.000000 dagster-airbyte-0.20.0/dagster_airbyte/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-airbyte-0.20.0/dagster_airbyte/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:01:06.941291 dagster-airbyte-0.20.0/dagster_airbyte.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      666 2023-07-20 22:01:06.000000 dagster-airbyte-0.20.0/dagster_airbyte.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      809 2023-07-20 22:01:06.000000 dagster-airbyte-0.20.0/dagster_airbyte.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:01:06.000000 dagster-airbyte-0.20.0/dagster_airbyte.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-07-20 22:01:06.000000 dagster-airbyte-0.20.0/dagster_airbyte.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:01:06.000000 dagster-airbyte-0.20.0/dagster_airbyte.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-20 22:01:06.000000 dagster-airbyte-0.20.0/dagster_airbyte.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-20 22:01:06.000000 dagster-airbyte-0.20.0/dagster_airbyte.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2023-07-20 22:01:06.953291 dagster-airbyte-0.20.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-07-20 21:53:16.000000 dagster-airbyte-0.20.0/setup.py
```

### Comparing `dagster-airbyte-0.19.9rc0/LICENSE` & `dagster-airbyte-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.19.9rc0/PKG-INFO` & `dagster-airbyte-0.20.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-airbyte
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for integrating Airbyte with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte
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
 Provides-Extra: test
```

### Comparing `dagster-airbyte-0.19.9rc0/dagster_airbyte/__init__.py` & `dagster-airbyte-0.20.0/dagster_airbyte/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.19.9rc0/dagster_airbyte/asset_defs.py` & `dagster-airbyte-0.20.0/dagster_airbyte/asset_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,26 +26,26 @@
     AssetKey,
     AssetOut,
     AutoMaterializePolicy,
     FreshnessPolicy,
     Nothing,
     Output,
     ResourceDefinition,
+    SourceAsset,
     _check as check,
 )
-from dagster._annotations import experimental
 from dagster._core.definitions import AssetsDefinition, multi_asset
 from dagster._core.definitions.cacheable_assets import (
     AssetsDefinitionCacheableData,
     CacheableAssetsDefinition,
 )
-from dagster._core.definitions.events import CoercibleToAssetKeyPrefix
+from dagster._core.definitions.events import CoercibleToAssetKey, CoercibleToAssetKeyPrefix
 from dagster._core.definitions.metadata import MetadataValue, TableSchemaMetadataValue
 from dagster._core.definitions.metadata.table import TableSchema
-from dagster._core.errors import DagsterInvalidInvocationError
+from dagster._core.errors import DagsterInvalidDefinitionError, DagsterInvalidInvocationError
 from dagster._core.execution.context.init import build_init_resource_context
 from dagster._utils.merger import merge_dicts
 
 from dagster_airbyte.resources import AirbyteCloudResource, AirbyteResource, BaseAirbyteResource
 from dagster_airbyte.types import AirbyteTableMetadata
 from dagster_airbyte.utils import (
     generate_materializations,
@@ -146,15 +146,15 @@
     group_name = cast(Optional[str], metadata["group_name"])
     destination_tables = cast(List[str], metadata["destination_tables"])
     normalization_tables = cast(Mapping[str, List[str]], metadata["normalization_tables"])
     io_manager_key = cast(Optional[str], metadata["io_manager_key"])
 
     @multi_asset(
         name=f"airbyte_sync_{connection_id[:5]}",
-        non_argument_deps=set((assets_defn_meta.keys_by_input_name or {}).values()),
+        deps=list((assets_defn_meta.keys_by_input_name or {}).values()),
         outs={
             k: AssetOut(
                 key=v,
                 metadata={
                     k: cast(TableSchemaMetadataValue, v)
                     for k, v in assets_defn_meta.metadata_by_output_name.get(k, {}).items()
                 }
@@ -197,20 +197,21 @@
                         )
             else:
                 yield materialization
 
     return _assets
 
 
-@experimental
 def build_airbyte_assets(
     connection_id: str,
     destination_tables: Sequence[str],
     asset_key_prefix: Optional[Sequence[str]] = None,
+    group_name: Optional[str] = None,
     normalization_tables: Optional[Mapping[str, Set[str]]] = None,
+    deps: Optional[Sequence[Union[CoercibleToAssetKey, AssetsDefinition, SourceAsset]]] = None,
     upstream_assets: Optional[Set[AssetKey]] = None,
     schema_by_table_name: Optional[Mapping[str, TableSchema]] = None,
     freshness_policy: Optional[FreshnessPolicy] = None,
 ) -> Sequence[AssetsDefinition]:
     """Builds a set of assets representing the tables created by an Airbyte sync operation.
 
     Args:
@@ -220,17 +221,25 @@
             in the Dagster asset graph for this sync. This will generally map to the name of the
             stream in Airbyte, unless a stream prefix has been specified in Airbyte.
         normalization_tables (Optional[Mapping[str, List[str]]]): If you are using Airbyte's
             normalization feature, you may specify a mapping of destination table to a list of
             derived tables that will be created by the normalization process.
         asset_key_prefix (Optional[List[str]]): A prefix for the asset keys inside this asset.
             If left blank, assets will have a key of `AssetKey([table_name])`.
-        upstream_assets (Optional[Set[AssetKey]]): A list of assets to add as sources.
+        deps (Optional[Sequence[Union[AssetsDefinition, SourceAsset, str, AssetKey]]]):
+            A list of assets to add as sources.
+        upstream_assets (Optional[Set[AssetKey]]): Deprecated, use deps instead. A list of assets to add as sources.
         freshness_policy (Optional[FreshnessPolicy]): A freshness policy to apply to the assets
     """
+    if upstream_assets is not None and deps is not None:
+        raise DagsterInvalidDefinitionError(
+            "Cannot specify both deps and upstream_assets to build_airbyte_assets. Use only deps"
+            " instead."
+        )
+
     asset_key_prefix = check.opt_sequence_param(asset_key_prefix, "asset_key_prefix", of_type=str)
 
     # Generate a list of outputs, the set of destination tables plus any affiliated
     # normalization tables
     tables = chain.from_iterable(
         chain([destination_tables], normalization_tables.values() if normalization_tables else [])
     )
@@ -250,24 +259,29 @@
     # If normalization tables are specified, we need to add a dependency from the destination table
     # to the affilitated normalization table
     if normalization_tables:
         for base_table, derived_tables in normalization_tables.items():
             for derived_table in derived_tables:
                 internal_deps[derived_table] = {AssetKey([*asset_key_prefix, base_table])}
 
+    upstream_deps = deps
+    if upstream_assets is not None:
+        upstream_deps = list(upstream_assets)
+
     # All non-normalization tables depend on any user-provided upstream assets
     for table in destination_tables:
-        internal_deps[table] = upstream_assets or set()
+        internal_deps[table] = set(upstream_deps) if upstream_deps else set()
 
     @multi_asset(
         name=f"airbyte_sync_{connection_id[:5]}",
-        non_argument_deps=upstream_assets or set(),
+        deps=upstream_deps,
         outs=outputs,
         internal_asset_deps=internal_deps,
         compute_kind="airbyte",
+        group_name=group_name,
     )
     def _assets(context, airbyte: BaseAirbyteResource):
         ab_output = airbyte.sync_and_poll(connection_id=connection_id)
 
         # No connection details (e.g. using Airbyte Cloud) means we just assume
         # that the outputs were produced
         if len(ab_output.connection_details) == 0:
@@ -736,15 +750,14 @@
                 state = yaml.safe_load(f.read())
                 connection_id = state.get("resource_id")
 
             output_connections.append((connection_id, connection))
         return output_connections
 
 
-@experimental
 def load_assets_from_airbyte_instance(
     airbyte: Union[AirbyteResource, ResourceDefinition],
     workspace_id: Optional[str] = None,
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     create_assets_for_normalization_tables: bool = True,
     connection_to_group_fn: Optional[Callable[[str], Optional[str]]] = _clean_name,
     io_manager_key: Optional[str] = None,
@@ -852,15 +865,14 @@
         connection_filter=connection_filter,
         connection_to_asset_key_fn=connection_to_asset_key_fn,
         connection_to_freshness_policy_fn=connection_to_freshness_policy_fn,
         connection_to_auto_materialize_policy_fn=connection_to_auto_materialize_policy_fn,
     )
 
 
-@experimental
 def load_assets_from_airbyte_project(
     project_dir: str,
     workspace_id: Optional[str] = None,
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     create_assets_for_normalization_tables: bool = True,
     connection_to_group_fn: Optional[Callable[[str], Optional[str]]] = _clean_name,
     io_manager_key: Optional[str] = None,
```

### Comparing `dagster-airbyte-0.19.9rc0/dagster_airbyte/managed/generated/destinations.py` & `dagster-airbyte-0.20.0/dagster_airbyte/managed/generated/destinations.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.19.9rc0/dagster_airbyte/managed/generated/sources.py` & `dagster-airbyte-0.20.0/dagster_airbyte/managed/generated/sources.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.19.9rc0/dagster_airbyte/managed/reconciliation.py` & `dagster-airbyte-0.20.0/dagster_airbyte/managed/reconciliation.py`

 * *Files 0% similar despite different names*

```diff
@@ -728,15 +728,15 @@
         if isinstance(diff, ManagedElementDiff) and not diff.is_empty():
             raise ValueError(
                 "Airbyte connections are not in sync with provided configuration, diff:\n{}".format(
                     str(diff)
                 )
             )
         elif isinstance(diff, ManagedElementError):
-            raise ValueError(f"Error checking Airbyte connections: {str(diff)}")
+            raise ValueError(f"Error checking Airbyte connections: {diff}")
 
         return super()._get_connections()
 
 
 @experimental
 def load_assets_from_connections(
     airbyte: Union[AirbyteResource, ResourceDefinition],
```

### Comparing `dagster-airbyte-0.19.9rc0/dagster_airbyte/managed/types.py` & `dagster-airbyte-0.20.0/dagster_airbyte/managed/types.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.19.9rc0/dagster_airbyte/ops.py` & `dagster-airbyte-0.20.0/dagster_airbyte/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.19.9rc0/dagster_airbyte/resources.py` & `dagster-airbyte-0.20.0/dagster_airbyte/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     ConfigurableResource,
     Failure,
     _check as check,
     get_dagster_logger,
     resource,
 )
 from dagster._config.pythonic_config import infer_schema_from_config_class
+from dagster._core.definitions.resource_definition import dagster_maintained_resource
 from dagster._utils.cached_method import cached_method
 from dagster._utils.merger import deep_merge_dicts
 from pydantic import Field
 from requests.exceptions import RequestException
 
 from dagster_airbyte.types import AirbyteOutput
 
@@ -65,14 +66,18 @@
             "Whether to cancel a sync in Airbyte if the Dagster runner is terminated. This may"
             " be useful to disable if using Airbyte sources that cannot be cancelled and"
             " resumed easily, or if your Dagster deployment may experience runner interruptions"
             " that do not impact your Airbyte deployment."
         ),
     )
 
+    @classmethod
+    def _is_dagster_maintained(cls) -> bool:
+        return True
+
     @property
     @cached_method
     def _log(self) -> logging.Logger:
         return get_dagster_logger()
 
     @property
     @abstractmethod
@@ -656,14 +661,15 @@
                 and self.cancel_sync_on_run_termination
             ):
                 self.cancel_job(job_id)
 
         return AirbyteOutput(job_details=job_details, connection_details=connection_details)
 
 
+@dagster_maintained_resource
 @resource(config_schema=AirbyteResource.to_config_schema())
 def airbyte_resource(context) -> AirbyteResource:
     """This resource allows users to programatically interface with the Airbyte REST API to launch
     syncs and monitor their progress. This currently implements only a subset of the functionality
     exposed by the API.
 
     For a complete set of documentation on the Airbyte REST API, including expected response JSON
@@ -693,14 +699,15 @@
         def my_airbyte_job():
             ...
 
     """
     return AirbyteResource.from_resource_context(context)
 
 
+@dagster_maintained_resource
 @resource(config_schema=infer_schema_from_config_class(AirbyteCloudResource))
 def airbyte_cloud_resource(context) -> AirbyteCloudResource:
     """This resource allows users to programatically interface with the Airbyte Cloud REST API to launch
     syncs and monitor their progress. Currently, this resource may only be used with the more basic
     `dagster-airbyte` APIs, including the ops and assets.
 
     """
```

### Comparing `dagster-airbyte-0.19.9rc0/dagster_airbyte/types.py` & `dagster-airbyte-0.20.0/dagster_airbyte/types.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.19.9rc0/dagster_airbyte/utils.py` & `dagster-airbyte-0.20.0/dagster_airbyte/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.19.9rc0/dagster_airbyte.egg-info/PKG-INFO` & `dagster-airbyte-0.20.0/dagster_airbyte.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-airbyte
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for integrating Airbyte with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte
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
 Provides-Extra: test
```

### Comparing `dagster-airbyte-0.19.9rc0/dagster_airbyte.egg-info/SOURCES.txt` & `dagster-airbyte-0.20.0/dagster_airbyte.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.19.9rc0/setup.py` & `dagster-airbyte-0.20.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,35 +22,34 @@
     author_email="hello@elementl.com",
     license="Apache-2.0",
     description="Package for integrating Airbyte with Dagster.",
     url=(
         "https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte"
     ),
     classifiers=[
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_airbyte_tests*"]),
     install_requires=[
-        "dagster==1.3.9rc0",
+        "dagster==1.4.0",
         "requests",
     ],
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "dagster-airbyte = dagster_airbyte.cli:main",
         ]
     },
     extras_require={
         "test": [
             "requests-mock",
         ],
         "managed": [
-            "dagster-managed-elements==0.19.9rc0",
+            "dagster-managed-elements==0.20.0",
         ],
     },
 )
```

