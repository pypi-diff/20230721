# Comparing `tmp/forestadmin_agent_toolkit-0.1.0b9.tar.gz` & `tmp/forestadmin_agent_toolkit-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_agent_toolkit-0.1.0b9.tar", max compression
+gzip compressed data, was "forestadmin_agent_toolkit-1.0.0b1.tar", max compression
```

## Comparing `forestadmin_agent_toolkit-0.1.0b9.tar` & `forestadmin_agent_toolkit-1.0.0b1.tar`

### file list

```diff
@@ -1,45 +1,47 @@
--rw-r--r--   0        0        0        0 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/README.md
--rw-r--r--   0        0        0      190 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/__init__.py
--rw-r--r--   0        0        0     3917 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/agent.py
--rw-r--r--   0        0        0       57 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/exceptions.py
--rw-r--r--   0        0        0      564 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/options.py
--rw-r--r--   0        0        0        0 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/__init__.py
--rw-r--r--   0        0        0        0 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/actions/__init__.py
--rw-r--r--   0        0        0     2249 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/actions/requests.py
--rw-r--r--   0        0        0     5919 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/actions/resources.py
--rw-r--r--   0        0        0      427 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/base.py
--rw-r--r--   0        0        0      891 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/__init__.py
--rw-r--r--   0        0        0    13948 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/crud.py
--rw-r--r--   0        0        0    16998 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/crud_related.py
--rw-r--r--   0        0        0     2838 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/decorators.py
--rw-r--r--   0        0        0      148 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/exceptions.py
--rw-r--r--   0        0        0     9841 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/filter.py
--rw-r--r--   0        0        0     5466 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/requests.py
--rw-r--r--   0        0        0     9227 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/stats.py
--rw-r--r--   0        0        0        0 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/security/__init__.py
--rw-r--r--   0        0        0      144 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/security/exceptions.py
--rw-r--r--   0        0        0     3928 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/security/resources.py
--rw-r--r--   0        0        0        0 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/services/__init__.py
--rw-r--r--   0        0        0     8382 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/services/permissions/__init__.py
--rw-r--r--   0        0        0      264 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/services/permissions/options.py
--rw-r--r--   0        0        0     1660 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/services/serializers/__init__.py
--rw-r--r--   0        0        0     9301 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/services/serializers/json_api.py
--rw-r--r--   0        0        0        0 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/__init__.py
--rw-r--r--   0        0        0     3289 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/authentication.py
--rw-r--r--   0        0        0     1826 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/context.py
--rw-r--r--   0        0        0        0 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/__init__.py
--rw-r--r--   0        0        0     3040 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/action_values.py
--rw-r--r--   0        0        0     2942 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/emitter.py
--rw-r--r--   0        0        0     2236 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/filterable.py
--rw-r--r--   0        0        0     4543 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py
--rw-r--r--   0        0        0     1975 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py
--rw-r--r--   0        0        0     7732 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py
--rw-r--r--   0        0        0      485 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/generator_segment.py
--rw-r--r--   0        0        0     2670 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/type.py
--rw-r--r--   0        0        0     1282 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/validation.py
--rw-r--r--   0        0        0     3329 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/http.py
--rw-r--r--   0        0        0     1685 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/id.py
--rw-r--r--   0        0        0      541 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/token.py
--rw-r--r--   0        0        0     1625 2022-12-07 16:22:08.667917 forestadmin_agent_toolkit-0.1.0b9/pyproject.toml
--rw-r--r--   0        0        0     1609 1970-01-01 00:00:00.000000 forestadmin_agent_toolkit-0.1.0b9/setup.py
--rw-r--r--   0        0        0     1173 1970-01-01 00:00:00.000000 forestadmin_agent_toolkit-0.1.0b9/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/__init__.py
+-rw-r--r--   0        0        0     4908 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/agent.py
+-rw-r--r--   0        0        0      135 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/exceptions.py
+-rw-r--r--   0        0        0      628 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/options.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/actions/__init__.py
+-rw-r--r--   0        0        0     2292 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/actions/requests.py
+-rw-r--r--   0        0        0     5964 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/actions/resources.py
+-rw-r--r--   0        0        0      464 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/base.py
+-rw-r--r--   0        0        0      913 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/collections/__init__.py
+-rw-r--r--   0        0        0     2494 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/collections/charts_collection.py
+-rw-r--r--   0        0        0     1708 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/collections/charts_datasource.py
+-rw-r--r--   0        0        0    15947 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/collections/crud.py
+-rw-r--r--   0        0        0    19417 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/collections/crud_related.py
+-rw-r--r--   0        0        0     2966 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/collections/decorators.py
+-rw-r--r--   0        0        0      148 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/collections/exceptions.py
+-rw-r--r--   0        0        0    10023 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/collections/filter.py
+-rw-r--r--   0        0        0     5624 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/collections/requests.py
+-rw-r--r--   0        0        0     9466 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/collections/stats.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/security/__init__.py
+-rw-r--r--   0        0        0      144 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/security/exceptions.py
+-rw-r--r--   0        0        0     3763 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/security/resources.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/services/__init__.py
+-rw-r--r--   0        0        0     8403 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/services/permissions/__init__.py
+-rw-r--r--   0        0        0      264 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/services/permissions/options.py
+-rw-r--r--   0        0        0     1660 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/services/serializers/__init__.py
+-rw-r--r--   0        0        0     9523 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/services/serializers/json_api.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/__init__.py
+-rw-r--r--   0        0        0     3227 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/authentication.py
+-rw-r--r--   0        0        0     2266 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/context.py
+-rw-r--r--   0        0        0     1392 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/csv.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/forest_schema/__init__.py
+-rw-r--r--   0        0        0     3039 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/forest_schema/action_values.py
+-rw-r--r--   0        0        0     4308 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/forest_schema/emitter.py
+-rw-r--r--   0        0        0     2236 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/forest_schema/filterable.py
+-rw-r--r--   0        0        0     4508 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py
+-rw-r--r--   0        0        0     2288 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py
+-rw-r--r--   0        0        0     7847 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py
+-rw-r--r--   0        0        0      506 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/forest_schema/generator_segment.py
+-rw-r--r--   0        0        0     3057 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/forest_schema/type.py
+-rw-r--r--   0        0        0     1281 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/forest_schema/validation.py
+-rw-r--r--   0        0        0     4019 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/http.py
+-rw-r--r--   0        0        0     1683 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/id.py
+-rw-r--r--   0        0        0      541 2023-07-21 14:36:29.554249 forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/token.py
+-rw-r--r--   0        0        0     1771 2023-07-21 14:37:56.564415 forestadmin_agent_toolkit-1.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 forestadmin_agent_toolkit-1.0.0b1/PKG-INFO
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/agent.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/agent.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,88 +1,109 @@
+import copy
 import sys
 
-from forestadmin.agent_toolkit.resources.collections.stats import StatsResource
-
 if sys.version_info >= (3, 8):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 from forestadmin.agent_toolkit.exceptions import AgentToolkitException
-from forestadmin.agent_toolkit.options import AgentMeta, Options
+from forestadmin.agent_toolkit.options import DEFAULT_OPTIONS, Options
 from forestadmin.agent_toolkit.resources.actions.resources import ActionResource
 from forestadmin.agent_toolkit.resources.collections import BoundCollection
+from forestadmin.agent_toolkit.resources.collections.charts_collection import ChartsCollectionResource
+from forestadmin.agent_toolkit.resources.collections.charts_datasource import ChartsDatasourceResource
 from forestadmin.agent_toolkit.resources.collections.crud import CrudResource
 from forestadmin.agent_toolkit.resources.collections.crud_related import CrudRelatedResource
+from forestadmin.agent_toolkit.resources.collections.stats import StatsResource
 from forestadmin.agent_toolkit.resources.security.resources import Authentication
 from forestadmin.agent_toolkit.services.permissions import PermissionService
 from forestadmin.agent_toolkit.services.serializers.json_api import create_json_api_schema
 from forestadmin.agent_toolkit.utils.forest_schema.emitter import SchemaEmitter
+from forestadmin.agent_toolkit.utils.forest_schema.type import AgentMeta
 from forestadmin.agent_toolkit.utils.http import ForestHttpApi
+from forestadmin.datasource_toolkit.datasource_customizer.collection_customizer import CollectionCustomizer
+from forestadmin.datasource_toolkit.datasource_customizer.datasource_customizer import DatasourceCustomizer
 from forestadmin.datasource_toolkit.datasources import Datasource
-from forestadmin.datasource_toolkit.decorators.collections import CustomizedCollection
-from forestadmin.datasource_toolkit.decorators.datasource import CustomizedDatasource
+from forestadmin.datasource_toolkit.decorators.chart.types import DataSourceChartDefinition
 
 
 class Resources(TypedDict):
     authentication: Authentication
     crud: CrudResource
     crud_related: CrudRelatedResource
     stats: StatsResource
     actions: ActionResource
+    collection_charts: ChartsCollectionResource
+    datasource_charts: ChartsDatasourceResource
 
 
 class Agent:
+    __IS_INITIALIZED: bool = False
+    META: AgentMeta = None
+
     def __init__(self, options: Options):
-        self.options = options
-        self.composite_datasource: CustomizedDatasource[CustomizedCollection] = Datasource()  # type: ignore
+        self.options = copy.copy(DEFAULT_OPTIONS)
+        self.options.update({k: v for k, v in options.items() if v is not None})
+        self.customizer: DatasourceCustomizer = DatasourceCustomizer()
+        self._resources = None
 
-        self.permission_service = PermissionService(
+        self._permission_service = PermissionService(
             {
-                "env_secret": options["env_secret"],
-                "forest_server_url": options["forest_server_url"],
-                "is_production": options["is_production"],
+                "env_secret": self.options["env_secret"],
+                "forest_server_url": self.options["forest_server_url"],
+                "is_production": self.options["is_production"],
                 "permission_cache_duration": 60,
             }
         )
 
-    @property
-    def resources(self) -> Resources:
-        return {
+    def __mk_resources(self):
+        self._resources: Resources = {
             "authentication": Authentication(self.options),
-            "crud": CrudResource(self.composite_datasource, self.permission_service, self.options),
-            "crud_related": CrudRelatedResource(self.composite_datasource, self.permission_service, self.options),
-            "stats": StatsResource(self.composite_datasource, self.permission_service, self.options),
-            "actions": ActionResource(self.composite_datasource, self.permission_service, self.options),
+            "crud": CrudResource(self.customizer.stack.datasource, self._permission_service, self.options),
+            "crud_related": CrudRelatedResource(
+                self.customizer.stack.datasource, self._permission_service, self.options
+            ),
+            "stats": StatsResource(self.customizer.stack.datasource, self._permission_service, self.options),
+            "actions": ActionResource(self.customizer.stack.datasource, self._permission_service, self.options),
+            "collection_charts": ChartsCollectionResource(
+                self.customizer.stack.datasource, self._permission_service, self.options
+            ),
+            "datasource_charts": ChartsDatasourceResource(
+                self.customizer.stack.datasource, self._permission_service, self.options
+            ),
         }
 
+    @property
+    def resources(self) -> Resources:
+        if self._resources is None:
+            self.__mk_resources()
+        return self._resources
+
     def add_datasource(self, datasource: Datasource[BoundCollection]):
-        customized_datasource = CustomizedDatasource(datasource)
-        for collection in datasource.collections:
-            collection = CustomizedCollection(collection, customized_datasource)
-            self.composite_datasource.add_collection(collection)
-            customized_datasource.add_collection(collection)
+        self.customizer.add_datasource(datasource, {})
+        self._resources = None
 
-        for collection in customized_datasource.collections:
-            # second loop is mandatory to have all collection set
-            create_json_api_schema(collection)
+    def customize_collection(self, collection_name: str) -> CollectionCustomizer:
+        return self.customizer.customize_collection(collection_name)
+
+    def add_chart(self, name: str, definition: DataSourceChartDefinition):
+        return self.customizer.add_chart(name, definition)
 
     @property
     def meta(self) -> AgentMeta:
-        try:
-            return getattr(self, "META")
-        except AttributeError:
+        meta = getattr(self, "META", None)
+        if meta is None:
             raise AgentToolkitException("The agent subclass should set the META attribute")
+        return meta
 
     async def start(self):
-        collections_schema = await SchemaEmitter.get_serialized_schema(
-            self.options, self.composite_datasource, self.meta
-        )
-        api_map = SchemaEmitter.serialize(collections_schema, self.meta)
-        import json
+        if Agent.__IS_INITIALIZED is True:
+            return
 
-        print(json.dumps(api_map))
-        await ForestHttpApi.post(
-            ForestHttpApi.build_enpoint(self.options["forest_server_url"], "/forest/apimaps"),
-            api_map,
-            {"forest-secret-key": self.options["env_secret"], "content-type": "application/json"},
-        )
+        for collection in self.customizer.stack.datasource.collections:
+            create_json_api_schema(collection)
+
+        api_map = await SchemaEmitter.get_serialized_schema(self.options, self.customizer.stack.datasource, self.meta)
+
+        await ForestHttpApi.send_schema(self.options, api_map)
+        Agent.__IS_INITIALIZED = True
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/actions/requests.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/actions/requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 from forestadmin.agent_toolkit.exceptions import AgentToolkitException
 from forestadmin.agent_toolkit.resources.collections import BoundCollection
 from forestadmin.agent_toolkit.resources.collections.requests import RequestArgs as CollectionRequestArgs
 from forestadmin.agent_toolkit.resources.collections.requests import RequestCollection
 from forestadmin.agent_toolkit.utils.context import Request, RequestMethod, User
 from forestadmin.datasource_toolkit.collections import Collection
+from forestadmin.datasource_toolkit.datasource_customizer.collection_customizer import CollectionCustomizer
+from forestadmin.datasource_toolkit.datasource_customizer.datasource_customizer import DatasourceCustomizer
 from forestadmin.datasource_toolkit.datasources import Datasource
-from forestadmin.datasource_toolkit.decorators.collections import CustomizedCollection
-from forestadmin.datasource_toolkit.decorators.datasource import CustomizedDatasource
 from typing_extensions import Self
 
 
 class RequestActionException(AgentToolkitException):
     pass
 
 
@@ -21,33 +21,33 @@
 
 
 class ActionRequest(RequestCollection):
     def __init__(
         self,
         method: RequestMethod,
         action_name: str,
-        collection: Union[Collection, CustomizedCollection],
+        collection: Union[Collection, CollectionCustomizer],
         body: Optional[Dict[str, Any]] = None,
         query: Optional[Dict[str, str]] = None,
         headers: Optional[Dict[str, str]] = None,
         user: Optional[User] = None,
     ):
         super(ActionRequest, self).__init__(method, collection, body, query, headers, user)
         self.action_name = action_name
 
     @staticmethod
     def from_request_args(
-        request: Request, datasource: Union[Datasource[BoundCollection], CustomizedDatasource]
+        request: Request, datasource: Union[Datasource[BoundCollection], DatasourceCustomizer]
     ) -> RequestArgs:
         request_args = RequestCollection.from_request_args(request, datasource)
         try:
             action_name: int = request.query["action_name"]  # type: ignore
         except KeyError:
             raise RequestActionException("'action_name' is missing in the request")
         name = list(request_args["collection"].schema["actions"].keys())[action_name]
         return {**request_args, "action_name": name}
 
     @classmethod
     def from_request(
-        cls, request: Request, datasource: Union[Datasource[BoundCollection], CustomizedDatasource]
+        cls, request: Request, datasource: Union[Datasource[BoundCollection], DatasourceCustomizer]
     ) -> Self:
         return cls(**cls.from_request_args(request, datasource))
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/actions/resources.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/actions/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,18 @@
     @authenticate
     async def execute(self, request: ActionRequest) -> Union[FileResponse, Response]:
         if not request.body or not request.query:
             raise Exception
         filter = await self._get_records_selection(request)
         raw_data: Dict[str, Any] = request.body.get("data", {}).get("attributes", {}).get("values", {})  # type: ignore
         unsafe_data = ForestValueConverter.make_form_unsafe_data(raw_data)
-        fields = await request.collection.get_form(request.action_name, raw_data, filter)
+        fields = await request.collection.get_form(request.user, request.action_name, raw_data, filter)
         data = ForestValueConverter.make_form_data(request.collection.datasource, unsafe_data, fields)
-        result = await request.collection.execute(request.action_name, data, filter)
+        result = await request.collection.execute(request.user, request.action_name, data, filter)
+
         if result["type"] == ResultBuilder.ERROR:
             return build_json_response(400, {"error": result["message"]})
         elif result["type"] == ResultBuilder.SUCCESS:
             key = "success"
             if result["format"] == "html":
                 key = "html"
             return build_success_response({key: result["message"]})
@@ -83,16 +84,16 @@
             .get("attributes", {})  # type: ignore
             .get("fields", [])  # type: ignore
         )
         data: Optional[Dict[str, Any]] = None
         if forest_fields:
             data = ForestValueConverter.make_form_data_from_fields(request.collection.datasource, forest_fields)
 
-        filter = await self._get_records_selection(request)
-        fields = await request.collection.get_form(request.action_name, data, filter)
+        _filter = await self._get_records_selection(request)
+        fields = await request.collection.get_form(request.user, request.action_name, data, _filter)
 
         return build_success_response(
             {
                 "fields": [
                     await SchemaActionGenerator.build_field_schema(request.collection.datasource, field)
                     for field in fields
                 ]
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/__init__.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/collections/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import TypeVar, Union
 
 from forestadmin.agent_toolkit.options import Options
 from forestadmin.agent_toolkit.resources.base import BaseResource
 from forestadmin.agent_toolkit.services.permissions import PermissionService
 from forestadmin.datasource_toolkit.collections import Collection
+from forestadmin.datasource_toolkit.datasource_customizer.datasource_customizer import DatasourceCustomizer
 from forestadmin.datasource_toolkit.datasources import Datasource
-from forestadmin.datasource_toolkit.decorators.datasource import CustomizedDatasource
 
 BoundCollection = TypeVar("BoundCollection", bound=Collection)
 
-DatasourceAlias = Union[Datasource[BoundCollection], CustomizedDatasource]
+DatasourceAlias = Union[Datasource[BoundCollection], DatasourceCustomizer]
 
 
 class BaseCollectionResource(BaseResource):
     def __init__(self, datasource: DatasourceAlias[BoundCollection], permission: PermissionService, options: Options):
         super(BaseCollectionResource, self).__init__(options)
         self.permission = permission
         self.datasource = datasource
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/crud.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/collections/crud.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import asyncio
 import sys
 
+from typing_extensions import TypeGuard
+
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 from typing import Any, Awaitable, Dict, List, Tuple, cast
 
@@ -22,61 +24,72 @@
 )
 from forestadmin.agent_toolkit.resources.collections.requests import RequestCollection, RequestCollectionException
 from forestadmin.agent_toolkit.services.serializers.json_api import JsonApiException, JsonApiSerializer
 from forestadmin.agent_toolkit.utils.context import (
     Request,
     RequestMethod,
     Response,
+    User,
     build_client_error_response,
+    build_csv_response,
     build_no_content_response,
     build_success_response,
     build_unknown_response,
 )
+from forestadmin.agent_toolkit.utils.csv import Csv, CsvException
 from forestadmin.agent_toolkit.utils.id import unpack_id
 from forestadmin.datasource_toolkit.collections import Collection
 from forestadmin.datasource_toolkit.datasources import DatasourceException
+from forestadmin.datasource_toolkit.exceptions import ForestValidationException
 from forestadmin.datasource_toolkit.interfaces.fields import (
     ManyToOne,
     OneToOne,
     Operator,
     is_column,
     is_many_to_many,
     is_many_to_one,
+    is_one_to_many,
     is_one_to_one,
 )
 from forestadmin.datasource_toolkit.interfaces.query.aggregation import Aggregation
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.factory import ConditionTreeFactory
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.base import ConditionTree
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.leaf import ConditionTreeLeaf
 from forestadmin.datasource_toolkit.interfaces.query.filter.paginated import PaginatedFilter
 from forestadmin.datasource_toolkit.interfaces.query.filter.unpaginated import Filter
 from forestadmin.datasource_toolkit.interfaces.query.projections.factory import ProjectionFactory
 from forestadmin.datasource_toolkit.interfaces.records import CompositeIdAlias, RecordsDataAlias
 from forestadmin.datasource_toolkit.utils.collections import CollectionUtils
 from forestadmin.datasource_toolkit.utils.schema import SchemaUtils
 from forestadmin.datasource_toolkit.validations.field import FieldValidatorException
 from forestadmin.datasource_toolkit.validations.records import RecordValidator, RecordValidatorException
-from typing_extensions import TypeGuard
 
 
+# unused ???
 def is_request_collection(request: Request) -> TypeGuard[RequestCollection]:
     return hasattr(request, "collection")
 
 
-LiteralMethod = Literal["get", "list", "count", "add", "update", "delete", "delete_list", "update_list"]
+LiteralMethod = Literal["list", "count", "add", "delete_list", "csv"]
 
 
 class CrudResource(BaseCollectionResource):
     async def dispatch(self, request: Request, method_name: LiteralMethod) -> Response:
         method = getattr(self, method_name)
         try:
             request_collection = RequestCollection.from_request(request, self.datasource)
         except RequestCollectionException as e:
             return build_client_error_response([str(e)])
-        return await method(request_collection)
+
+        try:
+            return await method(request_collection)
+        except ForestValidationException as e:
+            return build_client_error_response(
+                [{"name": "ForestValidationException", "detail": str(e)[3:], "status": 400}]
+            )
 
     @check_method(RequestMethod.GET)
     @authenticate
     @authorize("read")
     async def get(self, request: RequestCollection) -> Response:
         collection = request.collection
         try:
@@ -88,51 +101,52 @@
         scope_tree = await self.permission.get_scope(request)
         if scope_tree:
             trees.append(scope_tree)
 
         filter = PaginatedFilter({"condition_tree": ConditionTreeFactory.intersect(trees)})
 
         projections = ProjectionFactory.all(cast(Collection, collection))
-        records = await collection.list(filter, projections)
+        records = await collection.list(request.user, filter, projections)
+
+        if not len(records):
+            return build_unknown_response()
+
         for name, schema in collection.schema["fields"].items():
-            if is_many_to_many(schema):
+            if is_many_to_many(schema) or is_one_to_many(schema):
                 projections.append(f"{name}:id")  # type: ignore
                 records[0][name] = None
-        if not len(records):
-            return build_unknown_response()
-        else:
-            schema = JsonApiSerializer.get(collection)
-            try:
-                dumped: Dict[str, Any] = schema(projections=projections).dump(records[0])  # type: ignore
-            except JsonApiException as e:
-                return build_client_error_response([str(e)])
+
+        schema = JsonApiSerializer.get(collection)
+        try:
+            dumped: Dict[str, Any] = schema(projections=projections).dump(records[0])  # type: ignore
+        except JsonApiException as e:
+            return build_client_error_response([str(e)])
 
         return build_success_response(dumped)
 
     @check_method(RequestMethod.POST)
     @authenticate
     @authorize("add")
     async def add(self, request: RequestCollection) -> Response:
-
         collection = request.collection
         schema = JsonApiSerializer.get(collection)
         try:
             data: RecordsDataAlias = schema().load(request.body)  # type: ignore
         except JsonApiException as e:
             return build_client_error_response([str(e)])
 
-        record, one_to_one_relations = await self.extract_data(cast(Collection, collection), data)
+        record, one_to_one_relations = await self.extract_data(request.user, cast(Collection, collection), data)
 
         try:
             RecordValidator.validate(cast(Collection, collection), record)
         except RecordValidatorException as e:
             return build_client_error_response([str(e)])
 
         try:
-            records = await collection.create([record])
+            records = await collection.create(request.user, [record])
         except DatasourceException as e:
             return build_client_error_response([str(e)])
 
         try:
             await self._link_one_to_one_relations(request, records[0], one_to_one_relations)
         except CollectionResourceException as e:
             return build_client_error_response([str(e)])
@@ -151,30 +165,61 @@
         except FilterException as e:
             return build_client_error_response([str(e)])
         try:
             projections = parse_projection_with_pks(request)
         except DatasourceException as e:
             return build_client_error_response([str(e)])
 
-        records = await request.collection.list(paginated_filter, projections)
+        records = await request.collection.list(request.user, paginated_filter, projections)
         schema = JsonApiSerializer.get(request.collection)
         try:
             dumped: Dict[str, Any] = schema(projections=projections).dump(records, many=True)  # type: ignore
         except JsonApiException as e:
             return build_client_error_response([str(e)])
+
+        # TODO: add something like this (but between crud and crud related ; function need adaptation)
+        # if paginated_filter.search:
+        #     dumped = add_search_metadata(dumped, paginated_filter.search)
+
         return build_success_response(dumped)
 
     @check_method(RequestMethod.GET)
     @authenticate
     @authorize("browse")
+    @authorize("export")
+    async def csv(self, request: RequestCollection) -> Response:
+        scope_tree = await self.permission.get_scope(request)
+        try:
+            paginated_filter = build_paginated_filter(request, scope_tree)
+        except FilterException as e:
+            return build_client_error_response([str(e)])
+        try:
+            projections = parse_projection_with_pks(request)
+        except DatasourceException as e:
+            return build_client_error_response([str(e)])
+
+        records = await request.collection.list(request.user, paginated_filter, projections)
+
+        try:
+            csv_str = Csv.make_csv(records, projections)
+        except CsvException as e:
+            return build_client_error_response([str(e)])
+        return build_csv_response(csv_str, f"{request.query.get('filename', request.collection.name)}.csv")
+
+    @check_method(RequestMethod.GET)
+    @authenticate
+    @authorize("browse")
     async def count(self, request: RequestCollection) -> Response:
+        if request.collection.schema["countable"] is False:
+            return build_success_response({"meta": {"count": "deactivated"}})
+
         scope_tree = await self.permission.get_scope(request)
         filter = build_filter(request, scope_tree)
         aggregation = Aggregation({"operation": "Count"})
-        result = await request.collection.aggregate(filter, aggregation)
+        result = await request.collection.aggregate(request.user, filter, aggregation)
         try:
             count = result[0]["value"]
         except IndexError:
             count = 0
         return build_success_response({"count": count})
 
     @check_method(RequestMethod.PUT)
@@ -203,17 +248,17 @@
         trees: List[ConditionTree] = [ConditionTreeFactory.match_ids(collection.schema, [ids])]
         scope_tree = await self.permission.get_scope(request)
         if scope_tree:
             trees.append(scope_tree)
 
         filter = Filter({"condition_tree": ConditionTreeFactory.intersect(trees)})
 
-        await collection.update(filter, data)
+        await collection.update(request.user, filter, data)
         projection = ProjectionFactory.all(cast(Collection, collection))
-        records = await collection.list(PaginatedFilter.from_base_filter(filter), projection)
+        records = await collection.list(request.user, PaginatedFilter.from_base_filter(filter), projection)
 
         schema = JsonApiSerializer.get(collection)
         try:
             dumped: Dict[str, Any] = schema(projections=projection).dump(records[0])  # type: ignore
         except JsonApiException as e:
             return build_client_error_response([str(e)])
 
@@ -258,38 +303,42 @@
         self, request: RequestCollection, record: RecordsDataAlias, relation: OneToOne, linked: RecordsDataAlias
     ):
         foreign_collection = self.datasource.get_collection(relation["foreign_collection"])
         scope = await self.permission.get_scope(request, foreign_collection)
         await self.permission.can(request, f"edit:{request.collection.name}")
         origin_value = record[relation["origin_key_target"]]
 
+        # not needed
         # Break the old relation
         old_fk_owner = ConditionTreeLeaf(relation["origin_key"], Operator.EQUAL, origin_value)
         trees: List[ConditionTree] = [old_fk_owner]
         if scope:
             trees.append(scope)
+
         try:
             tz = parse_timezone(request)
         except FilterException as e:
-            raise CollectionResourceException(str(e))
+            raise CollectionResourceException(str(e)[3:])
 
         await foreign_collection.update(
+            request.user,
             Filter({"condition_tree": ConditionTreeFactory.intersect(trees), "timezone": tz}),
             {
                 f'{relation["origin_key"]}': None,
             },
         )
 
         # Create the new relation
         new_fk_owner = ConditionTreeFactory.match_records(foreign_collection.schema, [linked])
         trees: List[ConditionTree] = [new_fk_owner]
         if scope:
             trees.append(scope)
 
         await foreign_collection.update(
+            request.user,
             Filter({"condition_tree": ConditionTreeFactory.intersect(trees), "timezone": tz}),
             {
                 f'{relation["origin_key"]}': origin_value,
             },
         )
 
     async def _link_one_to_one_relations(
@@ -297,27 +346,28 @@
     ):
         awaitables: List[Awaitable[None]] = []
         for relation, linked in relations:
             awaitables.append(self._link_one_to_one_relation(request, record, relation, linked))
         await asyncio.gather(*awaitables)
 
     async def extract_data(
-        self, collection: Collection, data: Dict[str, Any]
+        self, caller: User, collection: Collection, data: Dict[str, Any]
     ) -> Tuple[Dict[str, Any], List[Tuple[OneToOne, RecordsDataAlias]]]:
         record: Dict[str, Any] = {}
         one_to_one_relations: List[Tuple[OneToOne, RecordsDataAlias]] = []
         for field_name, value in data.items():
             field = collection.get_field(field_name)
             if is_column(field):
                 record[field_name] = value
             elif is_many_to_one(field) or is_one_to_one(field):
                 foreign_collection = self.datasource.get_collection(field["foreign_collection"])
                 pk_names = SchemaUtils.get_primary_keys(foreign_collection.schema)
                 if is_one_to_one(field):
-                    one_to_one_relations.append((field, dict([(pk, value[i]) for i, pk in enumerate(pk_names)])))
+                    one_to_one_relations.append((field, dict([(pk, value) for pk in pk_names])))
+                    # one_to_one_relations.append((field, dict([(pk, value[i]) for i, pk in enumerate(pk_names)])))
                 else:
                     field = cast(ManyToOne, field)
                     record[field["foreign_key"]] = await CollectionUtils.get_value(
-                        cast(Collection, foreign_collection), [value], field["foreign_key_target"]
+                        caller, cast(Collection, foreign_collection), [value], field["foreign_key_target"]
                     )
 
         return record, one_to_one_relations
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/crud_related.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/collections/crud_related.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import sys
 
+from forestadmin.agent_toolkit.utils.csv import Csv, CsvException
+
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     import zoneinfo
 else:
@@ -11,33 +13,32 @@
 
 from typing import Any, Dict, List, Union, cast
 
 from forestadmin.agent_toolkit.resources.collections import BaseCollectionResource
 from forestadmin.agent_toolkit.resources.collections.decorators import authenticate, authorize, check_method
 from forestadmin.agent_toolkit.resources.collections.exceptions import CollectionResourceException
 from forestadmin.agent_toolkit.resources.collections.filter import (
-    FilterException,
     build_filter,
     build_paginated_filter,
     parse_condition_tree,
     parse_projection_with_pks,
     parse_selection_ids,
-    parse_timezone,
 )
 from forestadmin.agent_toolkit.resources.collections.requests import (
     RequestCollectionException,
     RequestRelationCollection,
 )
 from forestadmin.agent_toolkit.services.serializers import DumpedResult, add_search_metadata
 from forestadmin.agent_toolkit.services.serializers.json_api import JsonApiException, JsonApiSerializer
 from forestadmin.agent_toolkit.utils.context import (
     Request,
     RequestMethod,
     Response,
     build_client_error_response,
+    build_csv_response,
     build_no_content_response,
     build_success_response,
 )
 from forestadmin.agent_toolkit.utils.id import unpack_id
 from forestadmin.datasource_toolkit.collections import Collection
 from forestadmin.datasource_toolkit.datasources import DatasourceException
 from forestadmin.datasource_toolkit.interfaces.fields import (
@@ -54,15 +55,15 @@
 from forestadmin.datasource_toolkit.interfaces.query.filter.factory import FilterFactory
 from forestadmin.datasource_toolkit.interfaces.query.filter.unpaginated import Filter
 from forestadmin.datasource_toolkit.interfaces.records import CompositeIdAlias
 from forestadmin.datasource_toolkit.utils.collections import CollectionUtils
 from forestadmin.datasource_toolkit.utils.schema import SchemaUtils
 from forestadmin.datasource_toolkit.validations.field import FieldValidatorException
 
-LiteralMethod = Literal["list", "add", "delete", "update"]
+LiteralMethod = Literal["list", "add", "count", "delete_list", "update_list", "csv"]
 
 
 class CrudRelatedResource(BaseCollectionResource):
     async def dispatch(self, request: Request, method_name: LiteralMethod) -> Response:
         method = getattr(self, method_name)
         try:
             request_collection = RequestRelationCollection.from_request(request, self.datasource)
@@ -71,23 +72,24 @@
         return await method(request_collection)
 
     @authenticate
     @authorize("browse")
     @check_method(RequestMethod.GET)
     async def list(self, request: RequestRelationCollection) -> Response:
         if not (is_one_to_many(request.relation) or is_many_to_many(request.relation)):
-            return build_client_error_response(["Unhandled relation type"])
+            return build_client_error_response(["🌳🌳🌳Unhandled relation type"])
         try:
             ids = unpack_id(request.collection.schema, request.pks)
         except (FieldValidatorException, CollectionResourceException) as e:
             return build_client_error_response([str(e)])
         scope_tree = await self.permission.get_scope(request, request.foreign_collection)
         paginated_filter = build_paginated_filter(request, scope_tree)
         projection = parse_projection_with_pks(request)
         records = await CollectionUtils.list_relation(
+            request.user,
             cast(Collection, request.collection),
             ids,
             cast(Collection, request.foreign_collection),
             request.relation,
             paginated_filter,
             projection,
         )
@@ -99,93 +101,127 @@
 
         if paginated_filter.search:
             dumped = add_search_metadata(dumped, paginated_filter.search)
 
         return build_success_response(cast(Dict[str, Any], dumped))
 
     @authenticate
+    @authorize("browse")
+    @authorize("export")
+    @check_method(RequestMethod.GET)
+    async def csv(self, request: RequestRelationCollection) -> Response:
+        if not (is_one_to_many(request.relation) or is_many_to_many(request.relation)):
+            return build_client_error_response(["🌳🌳🌳Unhandled relation type"])
+        try:
+            ids = unpack_id(request.collection.schema, request.pks)
+        except (FieldValidatorException, CollectionResourceException) as e:
+            return build_client_error_response([str(e)])
+        scope_tree = await self.permission.get_scope(request, request.foreign_collection)
+        paginated_filter = build_paginated_filter(request, scope_tree)
+        try:
+            projection = parse_projection_with_pks(request)
+        except DatasourceException as e:
+            return build_client_error_response([str(e)])
+        records = await CollectionUtils.list_relation(
+            request.user,
+            cast(Collection, request.collection),
+            ids,
+            cast(Collection, request.foreign_collection),
+            request.relation,
+            paginated_filter,
+            projection,
+        )
+
+        try:
+            csv_str = Csv.make_csv(records, projection)
+        except CsvException as e:
+            return build_client_error_response([str(e)])
+        return build_csv_response(csv_str, f"{request.query.get('filename', request.collection.name)}.csv")
+
+    @authenticate
     @authorize("edit")
     @check_method(RequestMethod.POST)
     async def add(self, request: RequestRelationCollection) -> Response:
         try:
             parent_ids = unpack_id(request.collection.schema, request.pks)
         except (FieldValidatorException, CollectionResourceException) as e:
             return build_client_error_response([str(e)])
 
         if (
             not request.body
             or "data" not in request.body
             or len(request.body["data"]) == 0
             or not request.body["data"][0].get("id")
+            # TODO: again another hardcoded "id" # SchemaUtils.get_primary_keys(schema)
         ):
-            return build_client_error_response(["missing target's id "])
+            return build_client_error_response(["🌳🌳🌳missing target's id"])
+
         try:
+            # TODO: again another hardcoded "id" # SchemaUtils.get_primary_keys(schema)
             targeted_relation_ids = unpack_id(request.foreign_collection.schema, request.body["data"][0]["id"])
         except (FieldValidatorException, CollectionResourceException) as e:
             return build_client_error_response([str(e)])
 
         if not (is_one_to_many(request.relation) or is_many_to_many(request.relation)):
-            return build_client_error_response(["Unhandled relation type"])
+            return build_client_error_response(["🌳🌳🌳Unhandled relation type"])
 
         pks = SchemaUtils.get_primary_keys(request.foreign_collection.schema)[0]
         value = await CollectionUtils.get_value(
-            cast(Collection, request.foreign_collection), targeted_relation_ids, pks
+            request.user, cast(Collection, request.foreign_collection), targeted_relation_ids, pks
         )
         if is_one_to_many(request.relation):
             return await self._associate_one_to_many(request, parent_ids, value)
         else:
             return await self._associate_many_to_many(request, parent_ids, value)
 
     @authenticate
     @authorize("edit")
     @check_method(RequestMethod.PUT)
     async def update_list(self, request: RequestRelationCollection) -> Response:
         try:
-            timezone = parse_timezone(request)
-        except FilterException as e:
-            return build_client_error_response([str(e)])
-        try:
             parent_id = unpack_id(request.collection.schema, request.pks)
         except (FieldValidatorException, CollectionResourceException) as e:
             return build_client_error_response([str(e)])
         if not request.body or not request.body.get("data") or "id" not in request.body["data"]:
-            return build_client_error_response(["Relation id is missing"])
+            return build_client_error_response(["🌳🌳🌳Relation id is missing"])
         try:
             linked_id = unpack_id(request.foreign_collection.schema, request.body["data"]["id"])
         except (FieldValidatorException, CollectionResourceException) as e:
             return build_client_error_response([str(e)])
 
         if is_many_to_one(request.relation) or is_one_to_one(request.relation):
-
             if is_many_to_one(request.relation):
                 meth = self._update_many_to_one
             else:
                 meth = self._update_one_to_one
 
             try:
-                await meth(request, parent_id, linked_id, timezone)
+                await meth(request, parent_id, linked_id, request.user.timezone)
             except (CollectionResourceException, DatasourceException) as e:
                 return build_client_error_response([str(e)])
             return build_no_content_response()
-        return build_client_error_response(["Unhandled relation type"])
+        return build_client_error_response(["🌳🌳🌳Unhandled relation type"])
 
     @authenticate
     @authorize("browse")
     @check_method(RequestMethod.GET)
     async def count(self, request: RequestRelationCollection) -> Response:
+        if request.foreign_collection.schema["countable"] is False:
+            return build_success_response({"meta": {"count": "deactivated"}})
+
         try:
             parent_id = unpack_id(request.collection.schema, request.pks)
         except (FieldValidatorException, CollectionResourceException) as e:
             return build_client_error_response([str(e)])
         scope_tree = await self.permission.get_scope(request, request.foreign_collection)
         filter = build_filter(request, scope_tree)
         aggregation = Aggregation({"operation": "Count"})
 
         result = await CollectionUtils.aggregate_relation(
-            cast(Collection, request.collection), parent_id, request.relation_name, filter, aggregation
+            request.user, cast(Collection, request.collection), parent_id, request.relation_name, filter, aggregation
         )
         try:
             count = result[0]["value"]
         except IndexError:
             count = 0
         return build_success_response({"count": count})
 
@@ -210,64 +246,66 @@
             else:
                 meth = self._delete_many_to_many
             try:
                 await meth(request, parent_ids, delete_mode, filter)
             except (DatasourceException, CollectionResourceException) as e:
                 return build_client_error_response([str(e)])
             return build_no_content_response()
-        return build_client_error_response(["Unhandled relation type"])
+        return build_client_error_response(["🌳🌳🌳Unhandled relation type"])
 
     async def _associate_one_to_many(
         self, request: RequestRelationCollection, parent_ids: CompositeIdAlias, id_value: Union[str, int]
     ) -> Response:
         if not is_one_to_many(request.relation):
-            raise
+            return build_client_error_response(["🌳🌳🌳Unhandled relation type"])
         scope_tree = await self.permission.get_scope(request, request.foreign_collection)
         filter = build_filter(request, scope_tree)
         trees: List[ConditionTree] = [
-            ConditionTreeLeaf("id", Operator.EQUAL, id_value),
+            ConditionTreeLeaf(request.relation["origin_key_target"], Operator.EQUAL, id_value),
         ]
         if filter.condition_tree:
             trees.append(filter.condition_tree)
         filter.condition_tree = ConditionTreeFactory.intersect(trees)
         value = await CollectionUtils.get_value(
-            cast(Collection, request.collection), parent_ids, request.relation["origin_key_target"]
+            request.user, cast(Collection, request.collection), parent_ids, request.relation["origin_key_target"]
         )
         try:
-            await request.foreign_collection.update(filter, {f"{request.relation['origin_key']}": value})
+            await request.foreign_collection.update(request.user, filter, {f"{request.relation['origin_key']}": value})
         except DatasourceException as e:
             return build_client_error_response([str(e)])
         else:
             return build_no_content_response()
 
     async def _associate_many_to_many(
         self, request: RequestRelationCollection, parent_ids: CompositeIdAlias, foreign_id_value: Union[str, int]
     ):
         if not is_many_to_many(request.relation):
-            raise
+            return build_client_error_response(["🌳🌳🌳Unhandled relation type"])
         id = SchemaUtils.get_primary_keys(request.collection.schema)
-        origin_id_value = await CollectionUtils.get_value(cast(Collection, request.collection), parent_ids, id[0])
+        origin_id_value = await CollectionUtils.get_value(
+            request.user, cast(Collection, request.collection), parent_ids, id[0]
+        )
 
         record = {
             f"{request.relation['origin_key']}": origin_id_value,
             f"{request.relation['foreign_key']}": foreign_id_value,
         }
         through_collection = request.collection.datasource.get_collection(request.relation["through_collection"])
         try:
-            await through_collection.create([record])
+            await through_collection.create(request.user, [record])
         except DatasourceException as e:
             return build_client_error_response([str(e)])
         else:
             return build_no_content_response()
 
     async def get_base_fk_filter(self, request: RequestRelationCollection):
         ids, exclude_ids = parse_selection_ids(request)
 
         if len(ids) == 0 and not exclude_ids:
-            raise
+            raise CollectionResourceException("Unable to unpack the id")
 
         selected_ids = ConditionTreeFactory.match_ids(request.foreign_collection.schema, ids)
         if exclude_ids:
             selected_ids = selected_ids.inverse()
 
         scope_tree = await self.permission.get_scope(request, request.foreign_collection)
         filter = build_filter(request, scope_tree)
@@ -286,81 +324,86 @@
         parent_id: CompositeIdAlias,
         is_delete: bool,
         base_target_filter: Filter,
     ):
         if not is_one_to_many(request.relation):
             raise CollectionResourceException("Unhandled relation type")
         foreign_paginated_filter = await FilterFactory.make_foreign_filter(
-            cast(Collection, request.collection), parent_id, request.relation, base_target_filter
+            request.user, cast(Collection, request.collection), parent_id, request.relation, base_target_filter
         )
         foreign_filter = foreign_paginated_filter.to_base_filter()
         if is_delete:
-            await request.foreign_collection.delete(foreign_filter)
+            await request.foreign_collection.delete(request.user, foreign_filter)
         else:
-            await request.foreign_collection.update(foreign_filter, {f"{request.relation['origin_key']}": None})
+            await request.foreign_collection.update(
+                request.user, foreign_filter, {f"{request.relation['origin_key']}": None}
+            )
 
     async def _delete_many_to_many(
         self,
         request: RequestRelationCollection,
         parent_id: CompositeIdAlias,
         is_delete: bool,
         base_target_filter: Filter,
     ):
         if not is_many_to_many(request.relation):
             raise CollectionResourceException("Unhandled relation type")
         through_filter = await FilterFactory.make_through_filter(
+            request.user,
             cast(Collection, request.collection),
             parent_id,
             request.relation,
             base_target_filter,
         )
         through_collection = request.collection.datasource.get_collection(request.relation["through_collection"])
         if is_delete:
             foreign_filter = await FilterFactory.make_foreign_filter(
-                cast(Collection, request.collection), parent_id, request.relation, base_target_filter
+                request.user, cast(Collection, request.collection), parent_id, request.relation, base_target_filter
             )
-            await through_collection.delete(through_filter.to_base_filter())
+            await through_collection.delete(request.user, through_filter.to_base_filter())
             try:
-                await request.foreign_collection.delete(foreign_filter.to_base_filter())
+                await request.foreign_collection.delete(request.user, foreign_filter.to_base_filter())
             except DatasourceException:
                 # Let the datasource crash when:
                 # - the records in the foreignCollection are linked to other records in the origin collection
                 # - the underlying database/api is not cascading deletes
                 pass
         else:
-            await through_collection.delete(through_filter.to_base_filter())
+            await through_collection.delete(request.user, through_filter.to_base_filter())
 
     async def _update_one_to_one(
         self,
         request: RequestRelationCollection,
         parent_id: CompositeIdAlias,
         linked_id: CompositeIdAlias,
         timezone: zoneinfo.ZoneInfo,
     ):
         if not is_one_to_one(request.relation):
             raise CollectionResourceException("Unhandled relation type")
 
         scope = await self.permission.get_scope(request)
         origin_value = await CollectionUtils.get_value(
-            cast(Collection, request.collection), parent_id, request.relation["origin_key_target"]
+            request.user, cast(Collection, request.collection), parent_id, request.relation["origin_key_target"]
         )
 
         trees: List[ConditionTree] = [ConditionTreeLeaf(request.relation["origin_key"], Operator.EQUAL, origin_value)]
         if scope:
             trees.append(scope)
 
         await request.foreign_collection.update(
+            request.user,
             Filter({"condition_tree": ConditionTreeFactory.intersect(trees), "timezone": timezone}),
             {f"{request.relation['origin_key']}": origin_value},
         )
 
         trees = [ConditionTreeFactory.match_ids(request.foreign_collection.schema, [linked_id])]
         if scope:
             trees.append(scope)
         await request.foreign_collection.update(
+            request.user,
             Filter(
                 {
                     "condition_tree": ConditionTreeFactory.intersect(trees),
                     "timezone": timezone,
                 }
             ),
             {f"{request.relation['origin_key']}": origin_value},
@@ -374,18 +417,19 @@
         timezone: zoneinfo.ZoneInfo,
     ):
         if not is_many_to_one(request.relation):
             raise CollectionResourceException("Unhandled relation type")
 
         scope = await self.permission.get_scope(request)
         foreign_value = await CollectionUtils.get_value(
-            cast(Collection, request.collection), linked_id, request.relation["foreign_key_target"]
+            request.user, cast(Collection, request.collection), linked_id, request.relation["foreign_key_target"]
         )
 
         trees = [ConditionTreeFactory.match_ids(request.collection.schema, [parent_id])]
         if scope:
             trees.append(scope)
 
         await request.collection.update(
+            request.user,
             Filter({"condition_tree": ConditionTreeFactory.intersect(trees), "timezone": timezone}),
             {f"{request.relation['foreign_key']}": foreign_value},
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/decorators.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/collections/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Awaitable, Callable, TypeVar, Union
 
 from forestadmin.agent_toolkit.resources.collections import BaseCollectionResource
+from forestadmin.agent_toolkit.resources.collections.filter import parse_timezone
 from forestadmin.agent_toolkit.resources.collections.requests import RequestCollection
 from forestadmin.agent_toolkit.services.permissions import PermissionServiceException
 from forestadmin.agent_toolkit.utils.context import (
     FileResponse,
     Request,
     RequestMethod,
     Response,
@@ -42,14 +43,15 @@
             rendering_id=int(user["rendering_id"]),
             user_id=int(user["id"]),
             tags=user.get("tags", {}),
             email=user["email"],
             first_name=user["first_name"],
             last_name=user["last_name"],
             team=user["team"],
+            timezone=parse_timezone(request),
         )
         return await fn(self, request)
 
     return wrapped2
 
 
 def authorize(action: str):
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/filter.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/collections/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import json
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from forestadmin.agent_toolkit.exceptions import AgentToolkitException
 from forestadmin.agent_toolkit.resources.collections.requests import RequestCollection, RequestRelationCollection
 from forestadmin.agent_toolkit.utils.context import Request
 from forestadmin.datasource_toolkit.collections import Collection
-from forestadmin.datasource_toolkit.decorators.collections import CustomizedCollection
+from forestadmin.datasource_toolkit.datasource_customizer.collection_customizer import CollectionCustomizer
 from forestadmin.datasource_toolkit.interfaces.fields import is_column, is_many_to_one, is_one_to_one
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.factory import (
     ConditionTreeFactory,
     ConditionTreeFactoryException,
 )
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.base import ConditionTree
 from forestadmin.datasource_toolkit.interfaces.query.filter.paginated import PaginatedFilter
@@ -65,28 +65,31 @@
 def parse_selection_ids(request: Request) -> Tuple[List[CompositeIdAlias], bool]:
     if request.body:
         try:
             attributes: Dict[str, Any] = request.body.get("data", {}).get("attributes", {})  # type: ignore
         except AttributeError:
             attributes = {}
         exclude_ids = bool(attributes.get("all_records", False))  # type: ignore
-        if "ids" in attributes:
-            ids = [[id] for id in attributes["ids"]]
-        elif isinstance(request.body.get("data"), list):
-            ids = [[r["id"]] for r in request.body["data"]]
+        if exclude_ids is True:
+            ids = [[id] for id in attributes.get("all_records_ids_excluded", [])]
         else:
-            ids = []
+            if "ids" in attributes:
+                ids = [[id] for id in attributes["ids"]]
+            elif isinstance(request.body.get("data"), list):
+                ids = [[r["id"]] for r in request.body["data"]]
+            else:
+                ids = []
         return ids, exclude_ids
 
     raise Exception()
 
 
 def _get_collection(
     request: Union[RequestCollection, RequestRelationCollection]
-) -> Union[CustomizedCollection, Collection]:
+) -> Union[CollectionCustomizer, Collection]:
     collection = request.collection
     if isinstance(request, RequestRelationCollection):
         collection = request.foreign_collection
     return collection
 
 
 def parse_sort(request: Union[RequestCollection, RequestRelationCollection]):
@@ -108,19 +111,18 @@
         subset_query = _all_records_subset_query(request)
         if "page[size]" in subset_query:
             items_per_page = subset_query["page[size]"]
         if "page[number]" in subset_query:
             page_to_skip = subset_query["page[number]"]
 
     if not items_per_page and not page_to_skip and request.query:
-        page: Dict[str, Any] = request.query.get("page", {})
-        if "size" in page:
-            items_per_page = page["size"]
-        if "number" in page:
-            page_to_skip = page["number"]
+        if "page[size]" in request.query:
+            items_per_page = int(request.query["page[size]"])
+        if "page[number]" in request.query:
+            page_to_skip = int(request.query["page[number]"])
 
     if not items_per_page:
         items_per_page = DEFAULT_ITEMS_PER_PAGE
     if not page_to_skip:
         page_to_skip = DEFAULT_PAGE_TO_SKIP
 
     if (
@@ -184,15 +186,15 @@
         raise FilterException(str(e))
 
     return condition_tree
 
 
 def _parse_projection_fields(
     query: Dict[str, Any],
-    collection: Union[CustomizedCollection, Collection],
+    collection: Union[CollectionCustomizer, Collection],
     front_collection_name: str,
     is_related: bool = False,
 ) -> List[str]:
     projection_fields: List[str] = []
     try:
         fields: str = query[f"fields[{front_collection_name}]"]
     except KeyError:
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/requests.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/collections/requests.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-from typing import Any, Dict, Optional, TypedDict, TypeVar, Union
+import sys
+from typing import Any, Dict, Optional, TypeVar, Union
+
+if sys.version_info >= (3, 8):
+    from typing import TypedDict
+else:
+    from typing_extensions import TypedDict
 
 from forestadmin.agent_toolkit.exceptions import AgentToolkitException
 from forestadmin.agent_toolkit.resources.collections.exceptions import CollectionResourceException
 from forestadmin.agent_toolkit.utils.context import Request, RequestMethod, User
 from forestadmin.datasource_toolkit.collections import Collection, CollectionException
+from forestadmin.datasource_toolkit.datasource_customizer.collection_customizer import CollectionCustomizer
+from forestadmin.datasource_toolkit.datasource_customizer.datasource_customizer import DatasourceCustomizer
 from forestadmin.datasource_toolkit.datasources import Datasource, DatasourceException
-from forestadmin.datasource_toolkit.decorators.collections import CustomizedCollection
-from forestadmin.datasource_toolkit.decorators.datasource import CustomizedDatasource
 from forestadmin.datasource_toolkit.interfaces.fields import (
     ManyToMany,
     ManyToOne,
     OneToMany,
     OneToOne,
     is_many_to_many,
     is_many_to_one,
@@ -24,37 +30,37 @@
 
 class RequestCollectionException(AgentToolkitException):
     pass
 
 
 class RequestArgs(TypedDict):
     method: RequestMethod
-    collection: Union[Collection, CustomizedCollection]
+    collection: Union[Collection, CollectionCustomizer]
     body: Optional[Dict[str, Any]]
     query: Optional[Dict[str, str]]
     headers: Optional[Dict[str, str]]
     user: Optional[User]
 
 
 class RequestCollection(Request):
     def __init__(
         self,
         method: RequestMethod,
-        collection: Union[Collection, CustomizedCollection],
+        collection: Union[Collection, CollectionCustomizer],
         body: Optional[Dict[str, Any]] = None,
         query: Optional[Dict[str, str]] = None,
         headers: Optional[Dict[str, str]] = None,
         user: Optional[User] = None,
     ):
         super(RequestCollection, self).__init__(method, body, query, headers, user)
         self.collection = collection
 
     @staticmethod
     def from_request_args(
-        request: Request, datasource: Union[Datasource[BoundCollection], CustomizedDatasource]
+        request: Request, datasource: Union[Datasource[BoundCollection], DatasourceCustomizer]
     ) -> RequestArgs:
         if not request.query:
             raise RequestCollectionException("'collection_name' is missing in the request")
         try:
             collection_name = request.query["collection_name"]
         except KeyError:
             raise RequestCollectionException("'collection_name' is missing in the request")
@@ -70,15 +76,15 @@
             headers=request.headers,
             user=request.user,
             collection=collection,
         )
 
     @classmethod
     def from_request(
-        cls, request: Request, datasource: Union[Datasource[BoundCollection], CustomizedDatasource]
+        cls, request: Request, datasource: Union[Datasource[BoundCollection], DatasourceCustomizer]
     ) -> Self:
         return cls(**cls.from_request_args(request, datasource))
 
     @property
     def pks(self):
         if not self.query:
             raise CollectionResourceException("")
@@ -89,31 +95,31 @@
         return pks
 
 
 class RequestRelationCollection(RequestCollection):
     def __init__(
         self,
         method: RequestMethod,
-        collection: Union[Collection, CustomizedCollection],
-        foreign_collection: Union[Collection, CustomizedCollection],
+        collection: Union[Collection, CollectionCustomizer],
+        foreign_collection: Union[Collection, CollectionCustomizer],
         relation: Union[ManyToMany, OneToMany, OneToOne, ManyToOne],
         relation_name: str,
         body: Optional[Dict[str, Any]] = None,
         query: Optional[Dict[str, str]] = None,
         headers: Optional[Dict[str, str]] = None,
         user: Optional[User] = None,
     ):
         super(RequestRelationCollection, self).__init__(method, collection, body, query, headers, user)
         self.foreign_collection = foreign_collection
         self.relation = relation
         self.relation_name = relation_name
 
     @classmethod
     def from_request(
-        cls, request: Request, datasource: Union[Datasource[BoundCollection], CustomizedDatasource]
+        cls, request: Request, datasource: Union[Datasource[BoundCollection], DatasourceCustomizer]
     ) -> Self:
         kwargs = cls.from_request_args(request, datasource)
         if not request.query:
             raise RequestCollectionException("'relation_name' is missing in the request")
         try:
             relation_name = request.query["relation_name"]
         except KeyError:
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/stats.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/collections/stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,16 @@
+import sys
 from datetime import date, datetime
-from typing import Any, Dict, List, Literal, Union, cast
+
+if sys.version_info >= (3, 8):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
+from typing import Any, Dict, List, Union, cast
 from uuid import uuid1
 
 import pandas as pd
 from forestadmin.agent_toolkit.resources.collections import BaseCollectionResource
 from forestadmin.agent_toolkit.resources.collections.decorators import authenticate, check_method
 from forestadmin.agent_toolkit.resources.collections.filter import build_filter
 from forestadmin.agent_toolkit.resources.collections.requests import RequestCollection, RequestCollectionException
@@ -23,18 +30,17 @@
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.transforms.time import Frequency
 from forestadmin.datasource_toolkit.interfaces.query.filter.factory import FilterFactory
 from forestadmin.datasource_toolkit.interfaces.query.filter.unpaginated import Filter
 from forestadmin.datasource_toolkit.utils.schema import SchemaUtils
 
 
 class StatsResource(BaseCollectionResource):
-
     FREQUENCIES = {"Day": Frequency.DAY, "Week": Frequency.WEEK, "Month": Frequency.MONTH, "Year": Frequency.YEAR}
 
-    FORMAT = {"Day": "%d/%m/%Y", "Week": "W%W-%Y", "Month": "%m %Y", "Year": "%Y"}
+    FORMAT = {"Day": "%d/%m/%Y", "Week": "W%V-%Y", "Month": "%b %Y", "Year": "%Y"}
 
     def stats_method(self, type: str):
         return {
             "Value": self.value,
             "Objective": self.objective,
             "Pie": self.pie,
             "Line": self.line,
@@ -56,15 +62,15 @@
         except TypeError:
             return build_client_error_response(["Missing stats type in request body"])
         return await meth(request_collection)
 
     @check_method(RequestMethod.POST)
     @authenticate
     async def value(self, request: RequestCollection) -> Response:
-        current_filter = await self._get_gilter(request)
+        current_filter = await self._get_filter(request)
         result = {
             "countCurrent": await self._compute_value(request, current_filter),
         }
 
         if current_filter.condition_tree:
             current_filter.condition_tree = cast(ConditionTreeBranch, current_filter.condition_tree)
             with_count_previous = self._with_count_previous(current_filter.condition_tree)
@@ -77,57 +83,58 @@
                 )
 
         return self._build_success_response(result)
 
     @check_method(RequestMethod.POST)
     @authenticate
     async def objective(self, request: RequestCollection) -> Response:
-        current_filter = await self._get_gilter(request)
+        current_filter = await self._get_filter(request)
         result = {"value": await self._compute_value(request, current_filter)}
         return self._build_success_response(result)
 
     @check_method(RequestMethod.POST)
     @authenticate
     async def pie(self, request: RequestCollection) -> Response:
         if not request.body:
             raise Exception
 
-        current_filter = await self._get_gilter(request)
+        current_filter = await self._get_filter(request)
         aggregation = Aggregation(
             {
                 "operation": request.body["aggregate"],
                 "field": request.body.get("aggregate_field"),
                 "groups": [{"field": request.body["group_by_field"]}],
             }
         )
-        rows = await request.collection.aggregate(current_filter, aggregation)
+        rows = await request.collection.aggregate(request.user, current_filter, aggregation)
         results: List[Dict[str, Union[str, int]]] = []
         for row in rows:
             key = row["group"][request.body["group_by_field"]]
-            field = request.collection.get_field(request.body["group_by_field"])
-            if cast(Column, field)["column_type"] == PrimitiveType.ENUM:
-                key = key.value
+            if ":" not in request.body["group_by_field"]:
+                field = request.collection.get_field(request.body["group_by_field"])
+                if cast(Column, field)["column_type"] == PrimitiveType.ENUM:
+                    key = key.value
             results.append({"key": key, "value": row["value"]})
         return self._build_success_response(results)
 
     @check_method(RequestMethod.POST)
     @authenticate
     async def line(self, request: RequestCollection) -> Response:
         if not request.body:
             raise Exception
 
-        current_filter = await self._get_gilter(request)
+        current_filter = await self._get_filter(request)
         aggregation = Aggregation(
             {
                 "operation": request.body["aggregate"],
                 "field": request.body.get("aggregate_field"),
                 "groups": [{"field": request.body["group_by_date_field"], "operation": request.body["time_range"]}],
             }
         )
-        rows = await request.collection.aggregate(current_filter, aggregation)
+        rows = await request.collection.aggregate(request.user, current_filter, aggregation)
         values = {
             datetime.fromisoformat(row["group"][request.body["group_by_date_field"]]).date(): row["value"]
             for row in rows
             if row["group"][request.body["group_by_date_field"]] is not None
         }
         dates = list(values.keys())
         dates.sort()
@@ -157,24 +164,24 @@
         aggregate_field = request.body.get("aggregate_field")
         if not aggregate_field:
             relation = SchemaUtils.get_to_many_relation(request.collection.schema, relationship_field)
             foreign_collection = relation["foreign_collection"]
             collection = request.collection.datasource.get_collection(foreign_collection)
             pks = SchemaUtils.get_primary_keys(collection.schema)
             aggregate_field = pks[0]
-        current_filter = await self._get_gilter(request)
+        current_filter = await self._get_filter(request)
         aggregation = Aggregation(
             {
                 "operation": aggregate,
                 "field": f"{relationship_field}:{aggregate_field}",
                 "groups": [{"field": label_field}],
             }
         )
 
-        rows = await request.collection.aggregate(current_filter, aggregation, int(limit))
+        rows = await request.collection.aggregate(request.user, current_filter, aggregation, int(limit))
         results: List[Dict[str, Union[str, int]]] = []
         for row in rows:
             results.append({"key": row["group"][label_field], "value": row["value"]})
         return self._build_success_response(results)
 
     def _build_success_response(self, result: Any) -> Response:
         return build_success_response({"data": {"id": uuid1().hex, "type": "stats", "attributes": {"value": result}}})
@@ -185,22 +192,22 @@
         def _use_interval_res(tree: ConditionTree) -> None:
             if isinstance(tree, ConditionTreeLeaf):
                 use_interval_res.append(tree.use_interval_operator)
 
         tree.apply(_use_interval_res)
         return any(use_interval_res)
 
-    async def _get_gilter(self, request: RequestCollection) -> Filter:
+    async def _get_filter(self, request: RequestCollection) -> Filter:
         scope_tree = await self.permission.get_scope(request, request.collection)
         return build_filter(request, scope_tree)
 
     async def _compute_value(self, request: RequestCollection, filter: Filter) -> int:
         if not request.body:
             raise Exception
         aggregation = Aggregation(
             {"operation": request.body["aggregate"], "field": request.body.get("aggregate_field")}
         )
-        rows = await request.collection.aggregate(filter, aggregation)
+        rows = await request.collection.aggregate(request.user, filter, aggregation)
         res = 0
         if len(rows):
             res = int(rows[0]["value"])
         return res
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/security/resources.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/resources/security/resources.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,57 +2,54 @@
 import sys
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-from urllib.parse import urljoin
-
 from forestadmin.agent_toolkit.options import Options
 from forestadmin.agent_toolkit.resources.base import BaseResource
 from forestadmin.agent_toolkit.resources.security.exceptions import AuthenticationException
 from forestadmin.agent_toolkit.utils.authentication import ClientFactory, CustomClientOic
 from forestadmin.agent_toolkit.utils.context import Request, Response
 from forestadmin.agent_toolkit.utils.http import ForestHttpApi
 from forestadmin.agent_toolkit.utils.token import build_jwt
 
 LiteralMethod = Literal["authenticate", "callback"]
 
 
 class Authentication(BaseResource):
     def __init__(self, options: Options):
         super(Authentication, self).__init__(options)
-        self.callback_url = urljoin(options["agent_url"], "/forest/authentication/callback")
 
     async def dispatch(self, request: Request, method_name: LiteralMethod) -> Response:
         method = getattr(self, method_name)
         return await method(request)
 
     async def authenticate(self, request: Request) -> Response:
-        client: CustomClientOic = await ClientFactory.build(self.callback_url, self.option)
         if not request.body:
             raise AuthenticationException("renderingId is missing in the request's body")
         try:
             rendering_id = int(request.body["renderingId"])
         except KeyError:
             raise AuthenticationException("renderingId is missing in the request's body")
         except ValueError:
             raise AuthenticationException("renderingId should be an integer")
 
+        client: CustomClientOic = await ClientFactory.build(self.option)
         authorization_url = client.get_authorization_url(json.dumps({"renderingId": rendering_id}))
 
         return Response(
             status=200,
             body=json.dumps({"authorizationUrl": authorization_url}),
             headers={"content_type": "application/json"},
         )
 
     async def callback(self, request: Request) -> Response:
-        client: CustomClientOic = await ClientFactory.build(self.callback_url, self.option)
+        client: CustomClientOic = await ClientFactory.build(self.option)
         if not request.query:
             raise AuthenticationException("`state`should be sent to the callback endpoint")
         try:
             state = json.loads(request.query["state"])
         except KeyError:
             raise AuthenticationException("`state`should be sent to the callback endpoint")
         except ValueError:
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/services/permissions/__init__.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/services/permissions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from cachetools import TTLCache
 from forestadmin.agent_toolkit.resources.collections.requests import RequestCollection, RequestRelationCollection
 from forestadmin.agent_toolkit.services.permissions.options import RoleOptions
 from forestadmin.agent_toolkit.utils.context import Response, User
 from forestadmin.agent_toolkit.utils.http import ForestHttpApi
 from forestadmin.datasource_toolkit.collections import Collection
-from forestadmin.datasource_toolkit.decorators.collections import CustomizedCollection
+from forestadmin.datasource_toolkit.datasource_customizer.collection_customizer import CollectionCustomizer
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.factory import ConditionTreeFactory
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.base import ConditionTree
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.branch import ConditionTreeBranch
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.leaf import ConditionTreeLeaf
 
 
 class PermissionBody(TypedDict):
@@ -163,15 +163,15 @@
             raise PermissionServiceException("Unauthenticated request", 401)
         else:
             await self._can(action, request.user)
 
     async def get_scope(
         self,
         request: Union[RequestCollection, RequestRelationCollection],
-        collection: Union[Collection, CustomizedCollection, None] = None,
+        collection: Union[Collection, CollectionCustomizer, None] = None,
     ) -> Optional[ConditionTree]:
         if not request.user:
             raise PermissionServiceException("Unauthenticated request", 401)
         else:
             perms = await self._get_rendering_permissions(request.user.rendering_id)
             name = request.collection.name
             if collection:
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/services/serializers/__init__.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/services/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/services/serializers/json_api.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/services/serializers/json_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from typing import Any, Dict, List, Optional, Set, Tuple, Type, Union, cast
+from uuid import uuid4
 
 from forestadmin.agent_toolkit.exceptions import AgentToolkitException
 from forestadmin.agent_toolkit.utils.id import pack_id
 from forestadmin.datasource_toolkit.collections import Collection
-from forestadmin.datasource_toolkit.decorators.collections import CustomizedCollection
+from forestadmin.datasource_toolkit.datasource_customizer.collection_customizer import CollectionCustomizer
+from forestadmin.datasource_toolkit.interfaces.chart import Chart
 from forestadmin.datasource_toolkit.interfaces.fields import (
     ColumnAlias,
     PrimitiveType,
     RelationAlias,
     is_column,
     is_many_to_many,
     is_one_to_many,
 )
 from forestadmin.datasource_toolkit.interfaces.query.projections import Projection
 from marshmallow.exceptions import MarshmallowError
 from marshmallow.schema import SchemaMeta
 from marshmallow_jsonapi import Schema, fields  # type: ignore
 
-CollectionAlias = Union[Collection, CustomizedCollection]
+CollectionAlias = Union[Collection, CollectionCustomizer]
 
 
 class IntOrFloat(fields.Field):
     def _serialize(self, value, attr, obj, **kwargs):  # type: ignore
         if value is None:
             return value
         try:
@@ -95,15 +97,14 @@
             attributes[name] = _create_relationship(collection, name, cast(RelationAlias, field_schema))
     if "id" not in attributes:
         attributes["id"] = fields.Str()
     return attributes
 
 
 class JsonApiSerializer(type):
-
     schema: Dict[str, Type["ForestSchema"]] = {}
     attributes: Dict[str, Any] = {}
 
     def __new__(cls: Any, collection_name: str, bases: Tuple[Any], attrs: Dict[str, Any]):
         cls.attributes[collection_name] = attrs.copy()  # attrs is removed by the parent init
         klass = super(JsonApiSerializer, cls).__new__(cls, collection_name, bases, attrs)
         cls.schema[collection_name] = klass
@@ -192,15 +193,14 @@
         try:
             res = super().dump(obj, many=many)  # type: ignore
         except MarshmallowError as e:
             raise JsonApiException(str(e))
         return res  # type: ignore
 
     def load(self, data, *, many=None, partial=None, unknown=None):  # type: ignore
-
         try:
             return super().load(data, many=many, partial=partial, unknown=unknown)  # type: ignore
         except MarshmallowError as e:
             raise JsonApiException(str(e))
 
     def unwrap_item(self, item):  # type: ignore
         # needed to avoid an issue introduced by the front (type are pluralize for add and update)
@@ -209,15 +209,14 @@
             relation_field = self.Meta.fcollection.get_field(name)  # type: ignore
             relationship["data"]["type"] = relation_field["foreign_collection"]  # type: ignore
             item["relationships"][name] = relationship
         return super(ForestSchema, self).unwrap_item(item)  # type: ignore
 
 
 def refresh_json_api_schema(collection: CollectionAlias, ignores: Optional[List[CollectionAlias]] = None):
-
     if ignores is None:
         ignores = []
     if collection in ignores:
         return
     ignores.append(collection)
     if schema_name(collection) not in JsonApiSerializer.schema:
         raise JsonApiException("The schema doesn't exist")
@@ -236,7 +235,11 @@
             type_ = collection.name
             self_url = f"/forest/{collection.name}/{{{collection.name.lower()}_id}}"
             self_url_kwargs = {f"{collection.name.lower()}_id": "<__forest_id__>"}
             strict = True
             fcollection: CollectionAlias = collection
 
     return JsonApiSchemaType(schema_name(collection), (JsonApiSchema,), attributes)
+
+
+def render_chart(chart: Chart):
+    return {"id": str(uuid4()), "type": "stats", "attributes": {"value": chart}}
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/authentication.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,28 +51,26 @@
             skew=5,
             authn_method="",
         )
         return access_token
 
 
 class ClientFactory:
-
     oic_client: Optional[CustomClientOic] = None
 
     @classmethod
-    async def build(cls, callback_url: str, options: Options) -> CustomClientOic:
+    async def build(cls, options: Options) -> CustomClientOic:
         if cls.oic_client:
             return cls.oic_client
 
         issuer_metadata: Dict[str, Any] = await ForestHttpApi.get_open_id_issuer_metadata(options)
 
         client = CustomClientOic()
         client.register(  # type: ignore
             issuer_metadata["registration_endpoint"],
-            redirect_uris=[callback_url],
             registration_token=options["env_secret"],
         )
         client.handle_provider_config(
             ProviderConfigurationResponse(  # type: ignore
                 jwks_uri=urljoin(issuer_metadata["issuer"], "oidc/jwks"),
                 token_endpoint=urljoin(issuer_metadata["issuer"], "oidc/token"),
                 authorization_endpoint=urljoin(issuer_metadata["issuer"], "oidc/auth"),
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/context.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/context.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import enum
 import json
+import sys
 from dataclasses import dataclass, field
 from io import BytesIO
 from typing import Any, Dict, List, Optional
 
+if sys.version_info >= (3, 9):
+    from zoneinfo import ZoneInfo
+else:
+    from backports.zoneinfo import ZoneInfo
+
 
 class RequestMethod(enum.Enum):
     GET = "GET"
     POST = "POST"
     PUT = "PUT"
     DELETE = "DELETE"
     OPTION = "OPTION"
@@ -18,14 +24,17 @@
     rendering_id: int
     user_id: int
     tags: Dict[str, Any]
     email: str
     first_name: str
     last_name: str
     team: str
+    timezone: ZoneInfo
+    # permission_level
+    # role
 
 
 class Request:
     method: RequestMethod
     body: Optional[Dict[str, Any]] = None
     query: Optional[Dict[str, Any]] = None
     headers: Optional[Dict[str, str]] = None
@@ -67,21 +76,27 @@
 def build_client_error_response(reasons: List[str]) -> Response:
     return build_json_response(
         400,
         {"errors": reasons},
     )
 
 
-def build_success_response(body: Dict[str, Any]):
+def build_csv_response(body: str, filename: str) -> Response:
+    return Response(
+        200, body, headers={"content-type": "text/csv", "Content-Disposition": f'attachment; filename="{filename}"'}
+    )
+
+
+def build_success_response(body: Dict[str, Any]) -> Response:
     return build_json_response(200, body)
 
 
-def build_unknown_response():
+def build_unknown_response() -> Response:
     return Response(404)
 
 
-def build_no_content_response():
+def build_no_content_response() -> Response:
     return Response(204)
 
 
-def build_method_not_allowed_response():
+def build_method_not_allowed_response() -> Response:
     return Response(405)
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/action_values.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/forest_schema/action_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 
 class ForestValueConverter:
     @staticmethod
     def make_form_data_from_fields(
         datasource: Datasource[Collection], fields: List[ForestServerActionField]
     ) -> Dict[str, Any]:
-
         form_data: Dict[str, Any] = {}
         for field in fields:
             if field["reference"] and field["value"]:
                 collection_name = field["reference"].split(":")[0]
                 collection = datasource.get_collection(collection_name)
                 form_data[field["field"]] = unpack_id(collection.schema, field["value"])
             elif field["type"] == ActionFieldType.FILE:
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/filterable.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/forest_schema/filterable.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from typing import List, Union, cast
 
 from forestadmin.agent_toolkit.utils.forest_schema.action_values import ForestValueConverter
 from forestadmin.agent_toolkit.utils.forest_schema.generator_field import SchemaFieldGenerator
 from forestadmin.agent_toolkit.utils.forest_schema.type import ForestServerAction, ForestServerActionField
 from forestadmin.datasource_toolkit.collections import Collection
+from forestadmin.datasource_toolkit.datasource_customizer.collection_customizer import CollectionCustomizer
 from forestadmin.datasource_toolkit.datasources import Datasource
-from forestadmin.datasource_toolkit.decorators.collections import CustomizedCollection
 from forestadmin.datasource_toolkit.interfaces.actions import Action, ActionField, ActionFieldType
 from forestadmin.datasource_toolkit.interfaces.fields import Column, PrimitiveType
 from forestadmin.datasource_toolkit.utils.schema import SchemaUtils
 
 
 class SchemaActionGenerator:
-
     DUMMY_FIELDS = [
         ForestServerActionField(
             field="Loading...",
             type=SchemaFieldGenerator.build_column_type(PrimitiveType.STRING),
             isReadOnly=True,
             defaultValue="Form is loading",
             value=None,
@@ -27,78 +26,79 @@
             reference=None,
             widget=None,
         )
     ]
 
     @classmethod
     async def build(
-        cls, prefix: str, collection: Union[Collection, CustomizedCollection], name: str
+        cls, prefix: str, collection: Union[Collection, CollectionCustomizer], name: str
     ) -> ForestServerAction:
         schema = collection.schema["actions"][name]
         idx = list(collection.schema["actions"].keys()).index(name)
         slug = name.lower().replace(r"[^a-z0-9-]+", "-")
         return ForestServerAction(
             id=f"{collection.name}-{idx}-{slug}",
-            type=schema.scope.value.lower(),
             name=name,
+            type=schema.scope.value.lower(),
             baseUrl=None,
             endpoint=f"/{prefix}/_actions/{collection.name}/{idx}/{slug}",
             httpMethod="POST",
             redirect=None,
             download=bool(schema.generate_file),
             fields=await cls.build_fields(collection, schema, name),
             hooks={"load": not schema.static_form, "change": ["changeHook"]},
         )
 
     @classmethod
     async def build_field_schema(
         cls, datasource: Datasource[Collection], field: ActionField
     ) -> ForestServerActionField:
         output: ForestServerActionField = {
+            "field": field["label"],
             "value": ForestValueConverter.value_to_forest(field, field["value"]),
             "defaultValue": None,
             "description": field["description"],
             "enums": None,
-            "field": field["label"],
             "hook": None,
-            "isReadOnly": field["is_read_only"] or False,
-            "isRequired": field["is_required"] or True,
+            "isReadOnly": field.get("is_read_only", False),
+            "isRequired": field.get("is_required", True),
             "reference": None,
             "type": PrimitiveType.STRING,
             "widget": None,
         }
         if field["type"] == ActionFieldType.COLLECTION:
             collection: Collection = datasource.get_collection(field["collection_name"])  # type: ignore
             pk = SchemaUtils.get_primary_keys(collection.schema)[0]
             pk_schema = cast(Column, collection.get_field(pk))
             output["type"] = SchemaFieldGenerator.build_column_type(pk_schema["column_type"])  # type: ignore
             output["reference"] = f"{collection.name}.{pk}"
-        elif field["type"] == ActionFieldType.ENUM_LIST:
-            output["type"] = PrimitiveType.ENUM
-        elif field["type"] == ActionFieldType.NUMBER_LIST:
-            output["type"] = PrimitiveType.NUMBER
-        elif field["type"] == ActionFieldType.FILE:
-            output["type"] = "File"
+
+        elif "File" in field["type"].value:
+            output["type"] = ["File"] if "List" in field["type"].value else "File"
+
+        elif field["type"].value.endswith("List"):
+            output["type"] = [PrimitiveType(field["type"].value[:-4])]
         else:
-            output["type"] = PrimitiveType(field["type"].value)
+            output["type"] = field["type"].value
 
         if field["type"] in [ActionFieldType.ENUM, ActionFieldType.ENUM_LIST]:
             output["enums"] = field["enum_values"]
+
         if not isinstance(output["type"], str):
             output["type"] = SchemaFieldGenerator.build_column_type(output["type"])
 
         if field["watch_changes"]:
             output["hook"] = "changeHook"
 
         return ForestServerActionField(**output)
 
     @classmethod
     async def build_fields(
-        cls, collection: Union[Collection, CustomizedCollection], action: Action, name: str
+        cls, collection: Union[Collection, CollectionCustomizer], action: Action, name: str
     ) -> List[ForestServerActionField]:
         if not action.static_form:
             return cls.DUMMY_FIELDS
-        fields = await collection.get_form(name, None, None)
+        fields = await collection.get_form(None, name, None, None)
         new_fields: List[ForestServerActionField] = []
         for field in fields:
             new_fields.append(await cls.build_field_schema(collection.datasource, field))
         return new_fields
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 from typing import List, Union
 
 from forestadmin.agent_toolkit.utils.forest_schema.generator_action import SchemaActionGenerator
 from forestadmin.agent_toolkit.utils.forest_schema.generator_field import SchemaFieldGenerator
 from forestadmin.agent_toolkit.utils.forest_schema.generator_segment import SchemaSegmentGenerator
 from forestadmin.agent_toolkit.utils.forest_schema.type import ForestServerCollection, ForestServerField
 from forestadmin.datasource_toolkit.collections import Collection
-from forestadmin.datasource_toolkit.decorators.collections import CustomizedCollection
+from forestadmin.datasource_toolkit.datasource_customizer.collection_customizer import CollectionCustomizer
 from forestadmin.datasource_toolkit.interfaces.fields import FieldType
 from forestadmin.datasource_toolkit.utils.schema import SchemaUtils
 
 
 class SchemaCollectionGenerator:
     @staticmethod
-    async def build(prefix: str, collection: Union[Collection, CustomizedCollection]) -> ForestServerCollection:
+    async def build(prefix: str, collection: Union[Collection, CollectionCustomizer]) -> ForestServerCollection:
         fields: List[ForestServerField] = []
         for field_name in collection.schema["fields"].keys():
             if not SchemaUtils.is_foreign_key(collection.schema, field_name):
                 fields.append(SchemaFieldGenerator.build(collection, field_name))
+        fields = sorted(fields, key=lambda field: field["field"])
 
         return {
-            "actions": [
-                await SchemaActionGenerator.build(prefix, collection, name)
-                for name in collection.schema["actions"].keys()
-            ],
-            "fields": fields,
+            "name": collection.name,
+            "isVirtual": False,
             "icon": None,
-            "integration": None,
             "isReadOnly": all(
                 [f["type"] == FieldType.COLUMN and f["is_read_only"] for f in collection.schema["fields"].values()]
             ),
+            "integration": None,  # TODO: understand what is this
             "isSearchable": collection.schema["searchable"],
-            "isVirtual": False,
-            "name": collection.name,
             "onlyForRelationships": False,
             "paginationType": "page",
-            "segments": [
-                await SchemaSegmentGenerator.build(collection, name) for name in collection.schema["segments"]
-            ],
+            "searchField": None,
+            "actions": sorted(
+                [
+                    await SchemaActionGenerator.build(prefix, collection, name)
+                    for name in collection.schema["actions"].keys()
+                ],
+                key=lambda action: action["id"],
+            ),
+            "segments": sorted(
+                [await SchemaSegmentGenerator.build(collection, name) for name in collection.schema["segments"]],
+                key=lambda segment: segment["id"],
+            ),
+            "fields": fields,
         }
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Dict, List, Union, cast
+from typing import Dict, Union, cast
 
 from forestadmin.agent_toolkit.utils.forest_schema.filterable import FrontendFilterableUtils
 from forestadmin.agent_toolkit.utils.forest_schema.type import ForestServerField, RelationServer
 from forestadmin.agent_toolkit.utils.forest_schema.validation import FrontendValidationUtils
 from forestadmin.datasource_toolkit.collections import Collection
-from forestadmin.datasource_toolkit.decorators.collections import CustomizedCollection
+from forestadmin.datasource_toolkit.datasource_customizer.collection_customizer import CollectionCustomizer
 from forestadmin.datasource_toolkit.interfaces.fields import (
     Column,
     ColumnAlias,
     FieldType,
     ManyToMany,
     ManyToOne,
     OneToMany,
@@ -30,15 +30,15 @@
         FieldType.ONE_TO_ONE: "HasOne",
         FieldType.ONE_TO_MANY: "BelongsToMany",
         FieldType.MANY_TO_ONE: "BelongsTo",
         FieldType.MANY_TO_MANY: "BelongsToMany",
     }
 
     @classmethod
-    def build(cls, collection: Union[Collection, CustomizedCollection], field_name: str) -> ForestServerField:
+    def build(cls, collection: Union[Collection, CollectionCustomizer], field_name: str) -> ForestServerField:
         schema: ForestServerField = {}
 
         field_schema = collection.get_field(field_name)
         if is_column(field_schema):
             schema = cls.build_column_schema(field_name, field_schema)
         elif (
             is_one_to_one(field_schema)
@@ -52,34 +52,37 @@
         return cast(ForestServerField, dict(sorted(schema.items())))
 
     @staticmethod
     def build_column_type(_column_type: ColumnAlias) -> ColumnAlias:
         column_type: ColumnAlias
         if isinstance(_column_type, PrimitiveType):
             column_type = _column_type.value
+        elif isinstance(_column_type, str):
+            column_type = _column_type
         elif isinstance(_column_type, list):
-            _type = cast(List[PrimitiveType], _column_type)
-            column_type = [t.value for t in _column_type]
+            column_type = [SchemaFieldGenerator.build_column_type(_column_type[0])]
         else:
-            _type = cast(Dict[str, PrimitiveType], _column_type)
-            column_type = {k: t.value for k, t in _type.items()}
+            column_type = {
+                "fields": {"field": k, "type": SchemaFieldGenerator.build_column_type(t)}
+                for k, t in _column_type.items()
+            }
         return column_type
 
     @classmethod
     def build_column_schema(cls, name: str, column: Column) -> ForestServerField:
         validations = []
         if column["validations"]:
             validations = column["validations"]
 
         res = {
+            "field": name,
             "type": cls.build_column_type(column["column_type"]),
             "validations": FrontendValidationUtils.convert_validation_list(column["validations"]),
             "defaultValue": column["default_value"],
             "enums": column["enum_values"],
-            "field": name,
             "integration": None,
             "inverseOf": None,
             "isFilterable": FrontendFilterableUtils.is_filterable(column["column_type"], column["filter_operators"]),
             "isPrimaryKey": bool(column["is_primary_key"]),
             "isSortable": bool(column["is_sortable"]),
             "isReadOnly": bool(column["is_read_only"]),
             "isRequired": any([v["operator"] == Operator.PRESENT for v in validations]),
@@ -141,15 +144,15 @@
             "reference": f"{foreign_collection.name}.{key}",
         }
 
     @classmethod
     def build_many_to_one_schema(
         cls,
         relation: ManyToOne,
-        collection: Union[CustomizedCollection, Collection],
+        collection: Union[CollectionCustomizer, Collection],
         foreign_collection: Collection,
         base_schema: ForestServerField,
     ) -> ForestServerField:
         key = relation["foreign_key"]
         key_schema = cast(Column, collection.get_field(key))
         validations = key_schema["validations"] or []
 
@@ -163,15 +166,15 @@
             "isSortable": bool(key_schema["is_sortable"]),
             "validations": FrontendValidationUtils.convert_validation_list(validations),
             "reference": f"{foreign_collection.name}.{relation['foreign_key_target']}",
         }
 
     @classmethod
     def build_relation_schema(
-        cls, collection: Union[Collection, CustomizedCollection], field_name: str, field_schema: RelationAlias
+        cls, collection: Union[Collection, CollectionCustomizer], field_name: str, field_schema: RelationAlias
     ) -> ForestServerField:
         foreign_collection = collection.datasource.get_collection(field_schema["foreign_collection"])
         relation_schema: ForestServerField = {
             "field": field_name,
             "enums": None,
             "isReadOnly": False,
             "isVirtual": False,
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/type.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/forest_schema/type.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,14 +34,28 @@
 LiteralHasMany = Literal["HasMany"]
 LiteralBelongsTo = Literal["BelongsTo"]
 LiteralBelongsToMany = Literal["BelongsToMany"]
 
 RelationServer = Union[LiteralHasOne, LiteralHasMany, LiteralBelongsTo, LiteralBelongsToMany]
 
 
+class AgentStackMeta(TypedDict, total=False):
+    engine: Literal["python"]
+    engine_version: str
+    database_type: str
+    orm_version: str
+
+
+class AgentMeta(TypedDict):
+    liana: str
+    liana_version: str
+    stack: AgentStackMeta
+    schemaFileHash: str
+
+
 class ForestServerField(TypedDict, total=False):
     field: str
     type: ColumnAlias
     defaultValue: Any
     enums: Optional[List[str]]
     integration: None
     isFilterable: bool
@@ -55,28 +69,14 @@
     relationship: RelationServer
     validations: List[ServerValidationType]
 
 
 LiteralPage = Literal["page"]
 
 
-class ForestServerCollection(TypedDict):
-    name: str
-    icon: None
-    integration: None
-    isReadOnly: bool
-    isSearchable: bool
-    isVirtual: bool
-    onlyForRelationships: bool
-    paginationType: LiteralPage
-    actions: NotRequired[List[Any]]
-    fields: List[ForestServerField]
-    segments: NotRequired[List[Any]]
-
-
 class ForestServerActionHooks(TypedDict):
     load: bool
     change: List[Any]
 
 
 class ForestServerActionField(TypedDict):
     value: Any
@@ -112,7 +112,26 @@
 };
 """
 
 
 class ForestServerSegment(TypedDict):
     id: str
     name: str
+
+
+class ForestServerCollection(TypedDict):
+    name: str
+    icon: None
+    integration: None
+    isReadOnly: bool
+    isSearchable: bool
+    isVirtual: bool
+    onlyForRelationships: bool
+    paginationType: LiteralPage
+    actions: NotRequired[List[ForestServerAction]]
+    fields: List[ForestServerField]
+    segments: NotRequired[List[ForestServerSegment]]
+
+
+class ForestSchema(TypedDict):
+    data: List[ForestServerCollection]
+    meta: AgentMeta
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/validation.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/forest_schema/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import List, Optional
 
 from forestadmin.agent_toolkit.utils.forest_schema.type import ServerValidationType, ValidationType
 from forestadmin.datasource_toolkit.interfaces.fields import Operator, Validation
 
 
 class FrontendValidationUtils:
-
     OPERATOR_VALIDATION_TYPE = {
         Operator.PRESENT: ValidationType.PRESENT,
         Operator.GREATER_THAN: ValidationType.GREATER_THAN,
         Operator.LESS_THAN: ValidationType.LESS_THAN,
         Operator.LONGER_THAN: ValidationType.LONGER_THAN,
         Operator.SHORTER_THAN: ValidationType.SHORTER_THAN,
         Operator.CONTAINS: ValidationType.CONTAINS,
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/http.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/http.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     from typing_extensions import TypedDict
 
 from typing import Any, Dict, Optional
 
 import aiohttp
 from forestadmin.agent_toolkit.exceptions import AgentToolkitException
 from forestadmin.agent_toolkit.options import Options
+from forestadmin.agent_toolkit.utils.forest_schema.type import ForestSchema
 
 
 class ForestHttpApiException(AgentToolkitException):
     pass
 
 
 class HttpOptions(TypedDict):
@@ -71,13 +72,27 @@
                 raise ForestHttpApiException(f"Failed to fetch {endpoint}")
 
     @staticmethod
     async def post(endpoint: str, body: Dict[str, Any], headers: Dict[str, str]) -> Optional[Dict[str, Any]]:
         async with aiohttp.ClientSession() as session:
             try:
                 async with session.post(endpoint, json=body, headers=headers) as response:
-                    print("api map upload status", response.status)
                     if response.status == 200:
                         return await response.json()
                     return None
-            except aiohttp.ClientError:
-                raise ForestHttpApiException(f"Failed to fetch {endpoint}")
+            except aiohttp.ClientError as exc:
+                raise ForestHttpApiException(f"Failed to fetch {endpoint} : {exc}")
+
+    @classmethod
+    async def send_schema(cls, options: Options, schema: ForestSchema):
+        ret = await cls.post(
+            cls.build_enpoint(options["forest_server_url"], "/forest/apimaps/hashcheck"),
+            {"schemaFileHash": schema["meta"]["schemaFileHash"]},
+            {"forest-secret-key": options["env_secret"], "content-type": "application/json"},
+        )
+
+        if ret["sendSchema"] is True:
+            await cls.post(
+                cls.build_enpoint(options["forest_server_url"], "/forest/apimaps"),
+                schema,
+                {"forest-secret-key": options["env_secret"], "content-type": "application/json"},
+            )
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/id.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/id.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,23 +19,21 @@
     if not all(pks):
         raise IdException("")
 
     return "|".join(pks)  # type: ignore
 
 
 def unpack_id(schema: CollectionSchema, pks: str) -> CompositeIdAlias:
-
     schema_pks = SchemaUtils.get_primary_keys(schema)
     pk_values = pks.split("|")
     if len(pk_values) != len(schema_pks):
         raise IdException("Unable to unpack the id")
 
     values: List[Any] = []
     for i, field_name in enumerate(schema_pks):
-
         schema_field = cast(Column, schema["fields"][field_name])
         value = pk_values[i]
 
         if schema_field["column_type"] == PrimitiveType.NUMBER:
             try:
                 value = int(value)
             except ValueError:
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/token.py` & `forestadmin_agent_toolkit-1.0.0b1/forestadmin/agent_toolkit/utils/token.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b9/pyproject.toml` & `forestadmin_agent_toolkit-1.0.0b1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-agent-toolkit"
-version = "0.1.0-beta.9"
+version = "1.0.0-beta.1"
 description = ""
 authors = [ "Valentin Monté <valentinm@forestadmin.com>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "forestadmin"
 
 [tool.poetry.dependencies]
@@ -16,25 +16,25 @@
 typing-extensions = ">=4.2.0, <5.0"
 tzdata = "~2022.6"
 aiohttp = "~=3.8"
 oic = "~=1.4"
 python-jose = ">=3.3, <4.0"
 cachetools = "~=5.2"
 marshmallow-jsonapi = ">=0.24.0, <1.0"
-forestadmin-datasource-toolkit = "^0.1.0-beta.9"
+forestadmin-datasource-toolkit = "^1.0.0-beta.1"
 [[tool.poetry.dependencies.pandas]]
-version = "==1.1.5"
+version = "<=1.1.5"
 python = "<3.7.1"
 
 [[tool.poetry.dependencies.pandas]]
-version = "==1.3.5"
+version = ">=1.3.4,<=1.3.5"
 python = ">=3.7.1,<3.8"
 
 [[tool.poetry.dependencies.pandas]]
-version = "~=1.4.2"
+version = ">=1.4.0"
 python = ">=3.8"
 
 [tool.poetry.dependencies."backports.zoneinfo"]
 version = "~0.2.1"
 python = "<3.9"
 extras = [ "tzdata",]
 
@@ -51,14 +51,15 @@
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "~=7.1"
 pytest-asyncio = "~=0.18"
 coverage = "~=6.5"
 freezegun = "~=1.2.0"
+pytest-cov = "^4.0.0"
 [[tool.poetry.group.test.dependencies.mock]]
 version = "4.0"
 python = "3.7"
 
 [tool.poetry.group.linter.dependencies]
 [[tool.poetry.group.linter.dependencies.flake8]]
 version = "~=5.0"
@@ -69,7 +70,11 @@
 python = ">=3.8.1"
 
 [tool.poetry.group.formatter.dependencies]
 black = "~=22.10"
 
 [tool.poetry.group.sorter.dependencies]
 isort = "~=3.6"
+
+[tool.poetry.group.test.dependencies.forestadmin-datasource-toolkit]
+path = "../datasource_toolkit"
+develop = true
```

### Comparing `forestadmin_agent_toolkit-0.1.0b9/PKG-INFO` & `forestadmin_agent_toolkit-1.0.0b1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: forestadmin-agent-toolkit
-Version: 0.1.0b9
+Version: 1.0.0b1
 Summary: 
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8,<4.0)
-Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0); python_version < "3.9"
+Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0) ; python_version < "3.9"
 Requires-Dist: cachetools (>=5.2,<6.0)
-Requires-Dist: forestadmin-datasource-toolkit (>=0.1.0-beta.9,<0.2.0)
+Requires-Dist: forestadmin-datasource-toolkit (>=1.0.0-beta.1,<2.0.0)
 Requires-Dist: marshmallow-jsonapi (>=0.24.0,<1.0)
 Requires-Dist: oic (>=1.4,<2.0)
-Requires-Dist: pandas (==1.1.5); python_full_version < "3.7.1"
-Requires-Dist: pandas (==1.3.5); python_full_version >= "3.7.1" and python_version < "3.8"
-Requires-Dist: pandas (>=1.4.2,<1.5.0); python_version >= "3.8"
+Requires-Dist: pandas (<=1.1.5) ; python_full_version < "3.7.1"
+Requires-Dist: pandas (>=1.3.4,<=1.3.5) ; python_full_version >= "3.7.1" and python_version < "3.8"
+Requires-Dist: pandas (>=1.4.0) ; python_version >= "3.8"
 Requires-Dist: python-jose (>=3.3,<4.0)
 Requires-Dist: typing-extensions (>=4.2.0,<5.0)
 Requires-Dist: tzdata (>=2022.6,<2022.7)
 Description-Content-Type: text/markdown
```

