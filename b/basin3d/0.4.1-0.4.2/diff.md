# Comparing `tmp/basin3d-0.4.1.tar.gz` & `tmp/basin3d-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basin3d-0.4.1.tar", last modified: Thu Jul  6 14:34:59 2023, max compression
+gzip compressed data, was "basin3d-0.4.2.tar", last modified: Thu Jul 20 21:09:32 2023, max compression
```

## Comparing `basin3d-0.4.1.tar` & `basin3d-0.4.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:34:59.179538 basin3d-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-06 14:34:44.000000 basin3d-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-06 14:34:44.000000 basin3d-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-06 14:34:59.179538 basin3d-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-06 14:34:44.000000 basin3d-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:34:59.175538 basin3d-0.4.1/basin3d/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:34:59.175538 basin3d-0.4.1/basin3d/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/access.py
--rw-r--r--   0 runner    (1001) docker     (123)    29927 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/logging.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    54076 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:34:59.175538 basin3d-0.4.1/basin3d/core/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/schema/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/schema/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    16687 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/synthesis.py
--rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:34:59.175538 basin3d-0.4.1/basin3d/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/data/basin3d_observed_property_vocabulary.csv
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:34:59.175538 basin3d-0.4.1/basin3d/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34440 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/plugins/usgs.py
--rw-r--r--   0 runner    (1001) docker     (123)    66040 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/plugins/usgs_huc_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/plugins/usgs_mapping.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/synthesis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:34:59.175538 basin3d-0.4.1/basin3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-06 14:34:59.000000 basin3d-0.4.1/basin3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-06 14:34:59.000000 basin3d-0.4.1/basin3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 14:34:59.000000 basin3d-0.4.1/basin3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-06 14:34:59.000000 basin3d-0.4.1/basin3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 14:34:59.000000 basin3d-0.4.1/basin3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-06 14:34:44.000000 basin3d-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 14:34:59.179538 basin3d-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:09:32.044367 basin3d-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-20 21:09:19.000000 basin3d-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-20 21:09:19.000000 basin3d-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-20 21:09:32.044367 basin3d-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-20 21:09:19.000000 basin3d-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:09:32.040367 basin3d-0.4.2/basin3d/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-20 21:09:19.000000 basin3d-0.4.2/basin3d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:09:32.044367 basin3d-0.4.2/basin3d/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:09:19.000000 basin3d-0.4.2/basin3d/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-20 21:09:19.000000 basin3d-0.4.2/basin3d/core/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29927 2023-07-20 21:09:19.000000 basin3d-0.4.2/basin3d/core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-07-20 21:09:19.000000 basin3d-0.4.2/basin3d/core/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-20 21:09:19.000000 basin3d-0.4.2/basin3d/core/logging.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    54076 2023-07-20 21:09:19.000000 basin3d-0.4.2/basin3d/core/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-07-20 21:09:19.000000 basin3d-0.4.2/basin3d/core/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-07-20 21:09:19.000000 basin3d-0.4.2/basin3d/core/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:09:32.044367 basin3d-0.4.2/basin3d/core/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:09:19.000000 basin3d-0.4.2/basin3d/core/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-07-20 21:09:19.000000 basin3d-0.4.2/basin3d/core/schema/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-07-20 21:09:19.000000 basin3d-0.4.2/basin3d/core/schema/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19527 2023-07-20 21:09:19.000000 basin3d-0.4.2/basin3d/core/synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18007 2023-07-20 21:09:19.000000 basin3d-0.4.2/basin3d/core/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-20 21:09:19.000000 basin3d-0.4.2/basin3d/core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:09:32.044367 basin3d-0.4.2/basin3d/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:09:19.000000 basin3d-0.4.2/basin3d/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-07-20 21:09:19.000000 basin3d-0.4.2/basin3d/data/basin3d_observed_property_vocabulary.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-20 21:09:19.000000 basin3d-0.4.2/basin3d/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:09:32.044367 basin3d-0.4.2/basin3d/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:09:19.000000 basin3d-0.4.2/basin3d/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34412 2023-07-20 21:09:19.000000 basin3d-0.4.2/basin3d/plugins/usgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66040 2023-07-20 21:09:19.000000 basin3d-0.4.2/basin3d/plugins/usgs_huc_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-07-20 21:09:19.000000 basin3d-0.4.2/basin3d/plugins/usgs_mapping.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13748 2023-07-20 21:09:19.000000 basin3d-0.4.2/basin3d/synthesis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:09:32.040367 basin3d-0.4.2/basin3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-20 21:09:32.000000 basin3d-0.4.2/basin3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-20 21:09:32.000000 basin3d-0.4.2/basin3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:09:32.000000 basin3d-0.4.2/basin3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-20 21:09:32.000000 basin3d-0.4.2/basin3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 21:09:32.000000 basin3d-0.4.2/basin3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-20 21:09:19.000000 basin3d-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 21:09:32.044367 basin3d-0.4.2/setup.cfg
```

### Comparing `basin3d-0.4.1/LICENSE` & `basin3d-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.1/PKG-INFO` & `basin3d-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basin3d
-Version: 0.4.1
+Version: 0.4.2
 Summary: BASIN-3D Core Framework
 Author-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>, Charuleka Varadharajan <cvaradharajan@lbl.gov>, Catherine Wong <catwong@lbl.gov>
 Maintainer-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>
 License: Broker for Assimilation, Synthesis and Integration of eNvironmental Diverse, Distributed Datasets (BASIN-3D) Copyright (c) 2019, The
         Regents of the University of California, through Lawrence Berkeley National
         Laboratory (subject to receipt of any required approvals from the U.S.
         Dept. of Energy).  All rights reserved.
```

### Comparing `basin3d-0.4.1/README.md` & `basin3d-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.1/basin3d/core/access.py` & `basin3d-0.4.2/basin3d/core/access.py`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.1/basin3d/core/catalog.py` & `basin3d-0.4.2/basin3d/core/catalog.py`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.1/basin3d/core/connection.py` & `basin3d-0.4.2/basin3d/core/connection.py`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.1/basin3d/core/models.py` & `basin3d-0.4.2/basin3d/core/models.py`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.1/basin3d/core/monitor.py` & `basin3d-0.4.2/basin3d/core/monitor.py`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.1/basin3d/core/plugin.py` & `basin3d-0.4.2/basin3d/core/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     """Register a BASIN-3D plugin"""
 
     # TODO add any validation here for class structure
     PluginMount.plugins[cls.get_meta().id] = cls
     return cls
 
 
-def basin3d_plugin_access(plugin_class, synthesis_model_class, access_type):
+def _basin3d_plugin_access(plugin_class, synthesis_model_class, access_type):
     """Decorator for registering model access"""
 
     def _inner(func):
 
         plugin_access_classes = getattr(plugin_class, 'plugin_access_classes', None)
         if not plugin_access_classes:
             setattr(plugin_class, 'plugin_access_classes', [])
```

### Comparing `basin3d-0.4.1/basin3d/core/schema/enum.py` & `basin3d-0.4.2/basin3d/core/schema/enum.py`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.1/basin3d/core/schema/query.py` & `basin3d-0.4.2/basin3d/core/schema/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 
 
 class QueryBase(BaseModel):
     """ Query Base Class.  This sets `QueryBase.Config` defaults and processes incoming datasource ids"""
 
     datasource: Optional[List[str]] = Field(title="Datasource Identifiers",
                                             description="List of datasource identifiers to query by.")
+
+    id: Optional[str] = Field(title="Identifier", description="The unique identifier for the desired object")
+
     is_valid_translated_query: Union[None, bool] = Field(default=None, title="Valid translated query",
                                                          description="Indicates whether the translated query is valid: None = is not translated")
 
     def __init__(self, **data):
         """
         Custom constructor to modify datasource string to list, if necessary
 
@@ -64,22 +67,17 @@
     # Get the query fields that have mappings. Subclasses may overwrite this base function
     mapped_fields: ClassVar[List[str]] = []
 
     # Get the query fields that have prefixes. Subclasses may overwrite ths base function
     prefixed_fields: ClassVar[List[str]] = []
 
 
-class QueryById(QueryBase):
-    """Query for a single data object by identifier"""
-
-    id: str = Field(title="Identifier", description="The unique identifier for the desired data object")
-
-
 class QueryMonitoringFeature(QueryBase):
     """Query :class:`basin3d.core.models.MonitoringFeature`"""
+    # optional but id (QueryBase) is required to query by named monitoring feature
     feature_type: Optional[FeatureTypeEnum] = Field(title="Feature Type",
                                                     description="Filter results by the specified feature type.")
     monitoring_feature: Optional[List[str]] = Field(title="Monitoring Features",
                                                     description="Filter by the list of monitoring feature identifiers")
     parent_feature: Optional[List[str]] = Field(title="Parent Monitoring Features",
                                                 description="Filter by the list of parent monitoring feature identifiers")
 
@@ -97,15 +95,15 @@
 
         # To upper for feature type
         for field in ["featureType", "feature_type"]:
             if field in data and data[field]:
                 data[field] = isinstance(data[field], str) and data[field].upper() or data[field]
         super().__init__(**data)
 
-    prefixed_fields: ClassVar[List[str]] = ['monitoring_feature', 'parent_feature']
+    prefixed_fields: ClassVar[List[str]] = ['id', 'monitoring_feature', 'parent_feature']
 
 
 class QueryMeasurementTimeseriesTVP(QueryBase):
     """Query :class:`basin3d.core.models.MeasurementTimeseriesTVP`"""
     # required
     monitoring_feature: List[str] = Field(min_items=1, title="Monitoring Features",
                                           description="Filter by the list of monitoring feature identifiers")
```

### Comparing `basin3d-0.4.1/basin3d/core/synthesis.py` & `basin3d-0.4.2/basin3d/core/synthesis.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 import logging
 from typing import Iterator, List, Optional
 
 from basin3d.core import monitor
 from basin3d.core.models import Base, MeasurementTimeseriesTVPObservation, MonitoringFeature
 from basin3d.core.plugin import DataSourcePluginAccess, DataSourcePluginPoint
 from basin3d.core.schema.enum import MessageLevelEnum, AggregationDurationEnum
-from basin3d.core.schema.query import QueryBase, QueryById, QueryMeasurementTimeseriesTVP, \
+from basin3d.core.schema.query import QueryBase, QueryMeasurementTimeseriesTVP, \
     QueryMonitoringFeature, SynthesisMessage, SynthesisResponse
 from basin3d.core.translate import translate_query
 
 logger = monitor.get_logger(__name__)
 
 
 class MonitorMixin(object):
     """
     Adds monitor log functionality to a class for logging synthesis messages
     """
     def log(self,
             message: str, level: Optional[MessageLevelEnum] = None, where: Optional[List] = None) -> Optional[SynthesisMessage]:
         """
-        Add a synthesis message to the synthesis respoonse
+        Add a synthesis message to the synthesis response
         :param message: The message
         :param level:  The message level
         :param where:  Where the message is from
         :return: SynthesisMessage
         """
         logger_level = logging.INFO
         synthesis_message = None
@@ -184,15 +184,15 @@
                 # Clear all context
                 if self._where_context_token:
                     monitor.basin3d_where.reset(self._where_context_token)
                 raise StopIteration
 
     def log(self, message: str, level: Optional[MessageLevelEnum] = None, where: Optional[List] = None):  # type: ignore[override]
         """
-        Add a synthesis message to the synthesis respoonse
+        Add a synthesis message to the synthesis response
         :param message: The message
         :param level:  The message level
         :return: None
         """
         synthesis_message = super().log(message, level, self._where)
         if synthesis_message:
             self._synthesis_response.messages.append(synthesis_message)
@@ -233,53 +233,82 @@
         Return the synthesized plugin results
 
         :param query: The query for this function
         """
         return DataSourceModelIterator(query, self)
 
     @monitor.ctx_synthesis
-    def retrieve(self, query: QueryById) -> SynthesisResponse:
+    def retrieve(self, query: QueryBase, **kwargs) -> SynthesisResponse:
         """
         Retrieve a single synthesized value
 
         :param query: The query for this request
+        :param kwargs: messages, list of messages to be returned in the SynthesisResponse
         """
-        messages = []
-        if query.id:
+        datasource_id: Optional[str] = None
+        datasource = None
+        messages: List[Optional[SynthesisMessage]] = []
+
+        if 'messages' in kwargs and kwargs.get('messages'):
+            msg = kwargs.get('messages')
+            if isinstance(msg, List) and isinstance(msg[0], SynthesisMessage):
+                messages.extend(msg)
+            else:
+                messages.append(self.log('Message mis-configured.', MessageLevelEnum.WARN))
 
-            # split the datasource id prefix from the primary key
-            id_list = query.id.split("-")
-            datasource = None
-            try:
-                plugin = self.plugins[id_list[0]]
-                datasource = plugin.get_datasource()
-            except KeyError:
-                pass
-
-            if datasource:
-                datasource_pk = query.id.replace("{}-".format(id_list[0]),
-                                                 "", 1)  # The datasource id prefix needs to be removed
-
-                plugin_views = plugin.get_plugin_access()
-                monitor.set_ctx_basin3d_where([plugin.get_datasource().id, self.synthesis_model.__name__])
-                if self.synthesis_model in plugin_views:
-                    synthesized_query: QueryById = query.copy()
-                    synthesized_query.id = datasource_pk
-                    synthesized_query.datasource = [datasource.id]
-                    obj: Base = plugin_views[self.synthesis_model].get(query=synthesized_query)
-                    return SynthesisResponse(query=query, data=obj)  # type: ignore[call-arg]
+        # if the datasource is in the query, utilize it straight up
+        if query.datasource:
+            datasource_id = query.datasource[0]
+
+        # otherwise, get from a prefixed field.
+        # Not tying specifically to id at this point to enable different retrieve approaches from future classes.
+        elif query.prefixed_fields:
+            value = None
+            for prefixed_field in query.prefixed_fields:
+                attr_value = getattr(query, prefixed_field)
+                if attr_value and isinstance(attr_value, str):
+                    value = attr_value
+                    break
+                elif attr_value and isinstance(attr_value, list):
+                    value = attr_value[0]
+                    break
+
+            if value and isinstance(value, str):
+                datasource_id = value.split("-")[0]
+
+        try:
+            plugin = self.plugins[datasource_id]
+            datasource = plugin.get_datasource()
+        except KeyError:
+            pass
+
+        if datasource:
+
+            plugin_views = plugin.get_plugin_access()
+            monitor.set_ctx_basin3d_where([plugin.get_datasource().id, self.synthesis_model.__name__])
+            if self.synthesis_model in plugin_views and hasattr(plugin_views[self.synthesis_model], 'get'):
+
+                # Now translate the query object
+                translated_query_params: QueryBase = self.synthesize_query(plugin_views[self.synthesis_model], query)
+                translated_query_params.datasource = [plugin.get_datasource().id]
+
+                # Get the model access iterator if synthesized query is valid
+                if translated_query_params.is_valid_translated_query:
+                    item: Optional[Base] = plugin_views[self.synthesis_model].get(query=translated_query_params)
                 else:
-                    messages.append(self.log("Plugin view does not exist",
-                                             MessageLevelEnum.WARN,
-                                             [plugin.get_datasource().id, self.synthesis_model.__name__],
-                                             ))
+                    logger.warning(f'Translated query for datasource {plugin.get_datasource().id} is not valid.')
 
+                if item:
+                    return SynthesisResponse(query=query, data=item, messages=messages)  # type: ignore[call-arg]
             else:
-                messages.append(self.log(f"DataSource not not found for id {query.id}",
-                                MessageLevelEnum.ERROR))
+                messages.append(self.log("Plugin view does not exist", MessageLevelEnum.WARN,
+                                         [plugin.get_datasource().id, self.synthesis_model.__name__],))
+
+        else:
+            messages.append(self.log("DataSource not found for retrieve request", MessageLevelEnum.ERROR))
 
         return SynthesisResponse(query=query, messages=messages)  # type: ignore[call-arg]
 
 
 class MonitoringFeatureAccess(DataSourceModelAccess):
     """
     MonitoringFeature: A feature upon which monitoring is made. OGC Timeseries Profile OM_MonitoringFeature.
@@ -295,19 +324,21 @@
     * *shape:* string, Shape of the feature: POINT, CURVE, SURFACE, SOLID
     * *coordinates:* location of feature in absolute and/or representative datum
     * *description_reference:* string, additional information about the Feature
     * *related_party:* (optional) list of people or organizations responsible for the Feature
     * *utc_offset:* float, Coordinate Universal Time offset in hours (offset in hours), e.g., +9
     * *url:* url, URL with details for the feature
 
-    **Filter** by the following attributes (/?attribute=parameter&attribute=parameter&...)
+    **Filter** by the following attributes
 
-    * *datasource (optional):* a single data source id prefix (e.g ?datasource=`datasource.id_prefix`)
+    * *datasource (optional):* str, a single data source id prefix
+    * *id (optional):* str, a single monitoring feature id. Cannot be combined with monitoring_feature
+    * *parent_feature (optional)*: list, a list of parent feature ids. Plugin must have this functionality enabled.
+    * *monitoring_feature (optional)*: list, a list of monitoring feature ids. Cannot be combined with id, which will take precedence.
 
-    **Restrict fields**  with query parameter ‘fields’. (e.g. ?fields=id,name)
     """
     synthesis_model = MonitoringFeature
 
     def synthesize_query(self, plugin_access: DataSourcePluginAccess, query: QueryMonitoringFeature) -> QueryBase:  # type: ignore[override]
         """
         Synthesizes query parameters, if necessary
 
@@ -315,14 +346,42 @@
 
         :param query: The query information to be synthesized
         :param plugin_access: The plugin view to synthesize query params for
         :return: The synthesized query information
         """
         return translate_query(plugin_access, query)
 
+    def retrieve(self, query: QueryMonitoringFeature) -> SynthesisResponse:
+        """
+        Retrieve the specified Monitoring Feature
+
+        :param query: :class:`basin3d.core.schema.query.QueryMonitoringFeature`, id must be specified; monitoring_feature if specified will be removed.
+        :return: The synthesized response containing the specified MonitoringFeature if it exists
+        """
+
+        # validate that id is specified
+        if not query.id:
+            return SynthesisResponse(
+                query=query,
+                messages=[self.log('query.id field is missing and is required for monitoring feature request by id.',
+                                   MessageLevelEnum.ERROR)])  # type: ignore[call-arg]
+
+        msg = []
+
+        # remove monitoring_feature specification (i.e., id takes precedence)
+        if query.monitoring_feature:
+            mf_text = ', '.join(query.monitoring_feature)
+            query.monitoring_feature = None
+            msg.append(self.log(f'Monitoring Feature query has both id {query.id} and monitoring_feature {mf_text} '
+                                f'specified. Removing monitoring_feature and using id.', MessageLevelEnum.WARN))
+
+        # retrieve / get method order should be: MonitoringFeatureAccess, DataSourceModelAccess, <plugin>MonitoringFeatureAccess.get
+        synthesis_response: SynthesisResponse = super().retrieve(query=query, messages=msg)
+        return synthesis_response
+
 
 class MeasurementTimeseriesTVPObservationAccess(DataSourceModelAccess):
     """
     MeasurementTimeseriesTVPObservation: Series of measurement (numerical) observations in
     TVP (time value pair) format grouped by time (i.e., a timeseries).
 
     **Properties**
@@ -337,28 +396,25 @@
     * *result:* dictionary of 2 lists: "value" contains TimeValuePair obj and "quality" the corresponding quality assessment per value, observed values and their quality for the observed property being assessed
     * *time_reference_position:* enum, position of timestamp in aggregated_duration (START, MIDDLE, END)
     * *aggregation_duration:* enum, time period represented by observation (YEAR, MONTH, DAY, HOUR, MINUTE, SECOND, NONE)
     * *unit_of_measurement:* string, units in which the observation is reported
     * *statistic:* list, statistical properties of the observation result (MEAN, MIN, MAX, TOTAL)
     * *result_quality:* list, quality assessment values contained in the result (VALIDATED, UNVALIDATED, SUSPECTED, REJECTED, ESTIMATED)
 
-    **Filter** by the following attributes (?attribute=parameter&attribute=parameter&...):
+    **Filter** by the following attributes:
 
     * *monitoring_feature (required):* List of monitoring_features ids
     * *observed_property (required):* List of observed property variable ids
     * *start_date (required):* date YYYY-MM-DD
     * *end_date (optional):* date YYYY-MM-DD
     * *aggregation_duration (default: DAY):* enum (YEAR|MONTH|DAY|HOUR|MINUTE|SECOND|NONE)
     * *statistic (optional):* List of statistic options, enum (INSTANT|MEAN|MIN|MAX|TOTAL)
     * *datasource (optional):* a single data source id prefix (e.g ?datasource=`datasource.id_prefix`)
     * *result_quality (optional):* enum (VALIDATED|UNVALIDATED|SUSPECTED|REJECTED|ESTIMATED)
-    * *sampling_medium (optional):* ADD here -- probably should be enum
-
-    **Restrict fields** with query parameter ‘fields’. (e.g. ?fields=id,name)
-
+    * *sampling_medium (optional):* enum (SOLID_PHASE|WATER|GAS|OTHER)
 
     """
     synthesis_model = MeasurementTimeseriesTVPObservation
 
     def synthesize_query(self, plugin_access: DataSourcePluginAccess, query: QueryMeasurementTimeseriesTVP) -> QueryBase:  # type: ignore[override]
         """
         Synthesizes query parameters, if necessary
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `basin3d-0.4.1/basin3d/core/translate.py` & `basin3d-0.4.2/basin3d/core/translate.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """
 
 from itertools import product, repeat
 from typing import List, Optional, Union
 
 from basin3d.core import monitor
 from basin3d.core.schema.enum import MAPPING_DELIMITER, NO_MAPPING_TEXT
-from basin3d.core.schema.query import QueryBase, QueryById, QueryMeasurementTimeseriesTVP, QueryMonitoringFeature
+from basin3d.core.schema.query import QueryBase, QueryMeasurementTimeseriesTVP, QueryMonitoringFeature
 
 
 logger = monitor.get_logger(__name__)
 
 
 def _clean_query(translated_query: QueryBase) -> QueryBase:
     """
@@ -110,34 +110,38 @@
     for any query field that was supecified (i.e., with a BASIN-3D vocab)
 
     :param datasource_id: the datasource id
     :param query: the original query
     :param translated_query: the translated query
     :return: boolean (True = valid translated query, False = invalid translated query) or None (translated query could not be assessed)
     """
-    # loop thru kwargs
-    for attr in query.mapped_fields:
-        translated_attr_value = getattr(translated_query, attr)
-        b3d_attr_value = getattr(query, attr)
-        if isinstance(b3d_attr_value, list):
-            b3d_attr_value = ', '.join(b3d_attr_value)
-        if translated_attr_value and isinstance(translated_attr_value, list):
-            # if list and all of list == NOT_SUPPORTED, False
-            if all([x == NO_MAPPING_TEXT for x in translated_attr_value]):
-                logger.warning(f'Translated query for datasource {datasource_id} is invalid. No vocabulary found for attribute {attr} with values: {b3d_attr_value}.')
-                return False
-        elif translated_attr_value and isinstance(translated_attr_value, str):
-            # if single NOT_SUPPORTED, False
-            if translated_attr_value == NO_MAPPING_TEXT:
-                logger.warning(f'Translated query for datasource {datasource_id} is invalid. No vocabulary found for attribute {attr} with value: {b3d_attr_value}.')
-                return False
-        elif translated_attr_value:
-            logger.warning(
-                f'Translated query for datasource {datasource_id} cannot be assessed. Translated value for {attr} is not expected type.')
-            return None
+    for field_type, field_list in zip(['mapped', 'prefixed'], [query.mapped_fields, query.prefixed_fields]):
+        # loop thru kwargs
+        for attr in field_list:
+            translated_attr_value = getattr(translated_query, attr)
+            b3d_attr_value = getattr(query, attr)
+            msg_prefix = ''
+            if field_type == 'mapped':
+                msg_prefix = 'No vocabulary found for attribute {attr} with values: {b3d_attr_value}.'
+            if isinstance(b3d_attr_value, list):
+                b3d_attr_value = ', '.join(b3d_attr_value)
+            if translated_attr_value and isinstance(translated_attr_value, list):
+                # if list and all of list == NOT_SUPPORTED, False
+                if all([x == NO_MAPPING_TEXT for x in translated_attr_value]):
+                    logger.warning(f'Translated query for datasource {datasource_id} is invalid.{msg_prefix}')
+                    return False
+            elif translated_attr_value and isinstance(translated_attr_value, str):
+                # if single NOT_SUPPORTED, False
+                if translated_attr_value == NO_MAPPING_TEXT:
+                    logger.warning(f'Translated query for datasource {datasource_id} is invalid.{msg_prefix}')
+                    return False
+            elif translated_attr_value:
+                logger.warning(
+                    f'Translated query for datasource {datasource_id} cannot be assessed. Translated value for {attr} is not expected type.')
+                return None
     return True
 
 
 def _order_mapped_fields(plugin_access, query_mapped_fields):
     """
     Order the mapped fields according to the order of the attributes in any compound mappings. And then handle the rest of the mappings.
 
@@ -171,15 +175,15 @@
     else:
         # if there are no compound mappings, then the order doesn't matter, just copy the mapped field list.
         query_mapped_fields_ordered = query_mapped_fields
 
     return query_mapped_fields_ordered
 
 
-def _translate_mapped_query_attrs(plugin_access, query: Union[QueryMeasurementTimeseriesTVP, QueryMonitoringFeature, QueryById]) -> QueryBase:
+def _translate_mapped_query_attrs(plugin_access, query: Union[QueryMeasurementTimeseriesTVP, QueryMonitoringFeature]) -> QueryBase:
     """
     Translation functionality
     """
     query_mapped_fields = query.mapped_fields.copy()
 
     # if there are no mapped fields, return the query as is.
     if not query_mapped_fields:
@@ -210,15 +214,15 @@
             for compound_attr in compound_attrs:
                 setattr(query, compound_attr.lower(), None)
 
     # NOTE: always returns list for each mapped attr b/c multiple datasource vocab can be mapped to a single BASIN-3D vocab.
     return query
 
 
-def _translate_prefixed_query_attrs(plugin_access, query: Union[QueryMeasurementTimeseriesTVP, QueryMonitoringFeature, QueryById]) -> QueryBase:
+def _translate_prefixed_query_attrs(plugin_access, query: Union[QueryMeasurementTimeseriesTVP, QueryMonitoringFeature]) -> QueryBase:
     """
 
     :param plugin_access:
     :param query:
     :return:
     """
     def extract_id(identifer):
@@ -233,20 +237,26 @@
         return identifer
 
     id_prefix = plugin_access.datasource.id_prefix
 
     for attr in query.prefixed_fields:
         attr_value = getattr(query, attr)
         if attr_value:
+
+            # if the value is a string
             if isinstance(attr_value, str):
-                attr_value = attr_value.split(",")
+                translated_value = extract_id(attr_value)
+                if translated_value == attr_value:
+                    translated_value = NO_MAPPING_TEXT
 
-            translated_values = [extract_id(x) for x in attr_value if x.startswith("{}-".format(id_prefix))]
+            # otherwise assume it is a list
+            else:
+                translated_value = [extract_id(x) for x in attr_value if x.startswith("{}-".format(id_prefix))]
 
-            setattr(query, attr, translated_values)
+            setattr(query, attr, translated_value)
 
     return query
 
 
 def _translate_to_datasource_vocab(plugin_access, attr_type: str, basin3d_vocab: str, b3d_query) -> list:
     """
     Find the datasource vocabulary(ies) for the specified datasource, attribute type, BASIN-3D vocabulary, and full query that may specify other attributes.
@@ -381,15 +391,15 @@
                     if cm_attr.lower() not in kwargs:
                         cm_attr_mapping = get_datasource_mapped_attribute(plugin_access, attr_type=cm_attr.upper(), datasource_vocab=datasource_vocab)
                         kwargs[cm_attr.lower()] = cm_attr_mapping
 
     return kwargs
 
 
-def translate_query(plugin_access, query: Union[QueryMeasurementTimeseriesTVP, QueryMonitoringFeature, QueryById]) -> QueryBase:
+def translate_query(plugin_access, query: Union[QueryMeasurementTimeseriesTVP, QueryMonitoringFeature]) -> QueryBase:
     """
     Translate BASIN-3D vocabulary specified in a query to the datasource vocabularies defined by :class:`basin3d.core.models.AttributeMapping` objects specified in the datasource plugin.
 
     :param plugin_access: plugin access
     :param query: query to be translated
     :return: translated query as a :class:`basin3d.core.schema.query.QueryBase` object
     """
```

### Comparing `basin3d-0.4.1/basin3d/core/types.py` & `basin3d-0.4.2/basin3d/core/types.py`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.1/basin3d/data/basin3d_observed_property_vocabulary.csv` & `basin3d-0.4.2/basin3d/data/basin3d_observed_property_vocabulary.csv`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.1/basin3d/monitor.py` & `basin3d-0.4.2/basin3d/monitor.py`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.1/basin3d/plugins/usgs.py` & `basin3d-0.4.2/basin3d/plugins/usgs.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,17 +49,16 @@
 import json
 
 from basin3d.core import monitor
 from typing import Any, List, Optional, Tuple
 
 import requests
 
-# Get an instance of a logger
 from basin3d.core.schema.enum import FeatureTypeEnum, AggregationDurationEnum
-from basin3d.core.schema.query import QueryById, QueryMeasurementTimeseriesTVP, QueryMonitoringFeature
+from basin3d.core.schema.query import QueryMeasurementTimeseriesTVP, QueryMonitoringFeature
 from basin3d.core.access import get_url
 from basin3d.core.models import AbsoluteCoordinate, AltitudeCoordinate, Coordinate, GeographicCoordinate, \
     MeasurementTimeseriesTVPObservation, MonitoringFeature, RelatedSamplingFeature, \
     TimeMetadataMixin, TimeValuePair, ResultListTVP
 from basin3d.core.plugin import DataSourcePluginAccess, DataSourcePluginPoint, basin3d_plugin
 from basin3d.core.types import SpatialSamplingShapes
 from basin3d.plugins import usgs_huc_codes
@@ -433,47 +432,52 @@
             logger.warning(f"Read Timeout for {URL_USGS_HUC} - Failing over to stored HUC codes")
         except requests.exceptions.ConnectTimeout:
             synthesis_messages.append(f"Connection Timeout for {URL_USGS_HUC} - Failing over to stored HUC codes")
             logger.warning(f"Connection Timeout for {URL_USGS_HUC} - Failing over to stored HUC codes")
 
         return usgs_huc_codes.CONTENT
 
-    def get(self, query: QueryById):
+    def get(self, query: QueryMonitoringFeature):
         """ Get a single Region object
 
         ===================== === =====================
         USGS NWIS                 BASIN-3D
         ===================== === =====================
         ``{huc}``              >>  ``Primary key (query.id)``
         --------------------- --- ---------------------
         ``new_huc_rdb.txt``    >>  ``monitoringfeatures/<feature_type>/{query.id}``
         ===================== === =====================
 
         :param query: The query info object
         :return: a serialized ``MonitoringFeature`` object
         """
+        # query.id will always be a string at this point with validation upstream, thus ignoring the type checking
 
-        if len(query.id) == 2:
-            mf_query = QueryMonitoringFeature(monitoring_feature=[query.id], feature_type=FeatureTypeEnum.REGION)
-        elif len(query.id) == 4:
-            mf_query = QueryMonitoringFeature(monitoring_feature=[query.id], feature_type=FeatureTypeEnum.SUBREGION)
-        elif len(query.id) == 6:
-            mf_query = QueryMonitoringFeature(monitoring_feature=[query.id], feature_type=FeatureTypeEnum.BASIN)
-        elif len(query.id) == 8:
-            mf_query = QueryMonitoringFeature(monitoring_feature=[query.id], feature_type=FeatureTypeEnum.SUBBASIN)
-        else:
-            mf_query = QueryMonitoringFeature(monitoring_feature=[query.id], feature_type=FeatureTypeEnum.POINT)
+        monitoring_feature_len = len(query.id)  # type: ignore[arg-type]
+        if not query.feature_type:
+            if monitoring_feature_len == 2:
+                query.feature_type = FeatureTypeEnum.REGION
+            elif monitoring_feature_len == 4:
+                query.feature_type = FeatureTypeEnum.SUBREGION
+            elif monitoring_feature_len == 6:
+                query.feature_type = FeatureTypeEnum.BASIN
+            elif monitoring_feature_len == 8:
+                query.feature_type = FeatureTypeEnum.SUBBASIN
+            else:
+                query.feature_type = FeatureTypeEnum.POINT
+
+        query.monitoring_feature = [query.id]  # type: ignore[list-item]
 
-        for o in self.list(query=mf_query):
+        for o in self.list(query=query):
             return o
 
         # An 8 character code can also be a point, Try that
-        if len(query.id) == 8:
-            for o in self.list(query=QueryMonitoringFeature(monitoring_feature=[query.id],
-                                                            feature_type=FeatureTypeEnum.POINT)):
+        if monitoring_feature_len == 8:
+            query.feature_type = FeatureTypeEnum.POINT
+            for o in self.list(query=query):
                 return o
         return None
 
     def _load_huc_obj(self, json_obj, feature_type, description=None,
                       related_sampling_feature=None, related_sampling_feature_type=None):
         """
         Serialize an USGS Daily Values Data Source City object into a :class:`~basin3d.synthesis.models.field.Region` object
```

### Comparing `basin3d-0.4.1/basin3d/plugins/usgs_huc_codes.py` & `basin3d-0.4.2/basin3d/plugins/usgs_huc_codes.py`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.1/basin3d/plugins/usgs_mapping.csv` & `basin3d-0.4.2/basin3d/plugins/usgs_mapping.csv`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.1/basin3d/synthesis.py` & `basin3d-0.4.2/basin3d/synthesis.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,16 +31,15 @@
 """
 from importlib import import_module
 from typing import List, Union, cast
 
 from basin3d.core.catalog import CatalogTinyDb
 from basin3d.core.models import DataSource
 from basin3d.core.plugin import PluginMount
-from basin3d.core.schema.query import QueryById, QueryMeasurementTimeseriesTVP, \
-    QueryMonitoringFeature, SynthesisResponse
+from basin3d.core.schema.query import QueryMeasurementTimeseriesTVP, QueryMonitoringFeature, SynthesisResponse
 from basin3d.core.synthesis import DataSourceModelIterator, MeasurementTimeseriesTVPObservationAccess, \
     MonitoringFeatureAccess, logger
 
 
 class SynthesisException(Exception):
     """Special Exception for Synthesis module"""
     pass
@@ -179,15 +178,15 @@
         :param attr_vocab: str, The attribute vocabulary, either the BASIN-3D vocabulary or the datasource vocabulary
         :param from_basin3d: bool, True = the specified attr_vocab is a BASIN-3D vocabulary, False: the specified attr_vocab is from the datasource
 
         :return: iterator of :class:`AttributeMapping` objects
         """
         return self._catalog.find_attribute_mappings(datasource_id=datasource_id, attr_type=attr_type, attr_vocab=attr_vocab, from_basin3d=from_basin3d)
 
-    def monitoring_features(self, query: Union[QueryById, QueryMonitoringFeature] = None, **kwargs) -> Union[
+    def monitoring_features(self, query: QueryMonitoringFeature = None, **kwargs) -> Union[
             DataSourceModelIterator, SynthesisResponse]:
         """
         Search for all USGS monitoring features, USGS points by parent monitoring features, or look for a single monitoring feature by id.
 
         To see feature types for a given plugin: **<plugin_module>.<plugin_class>.feature_types**
 
 
@@ -242,21 +241,18 @@
 
         :param query: (optional) The Monitoring Feature Query object
 
         :return: a single :class:`~basin3d.core.schema.query.SynthesisResponse` for a query by id
             or a :class:`~basin3d.core.synthesis.DataSourceModelIterator` for multple :class:`MonitoringFeature` objects.
         """
         if not query:
-            if "id" in kwargs and isinstance(kwargs["id"], str):
-                query = QueryById(**kwargs)
-            else:
-                query = QueryMonitoringFeature(**kwargs)
+            query = QueryMonitoringFeature(**kwargs)
 
         # Search for single or list?
-        if isinstance(query, QueryById):
+        if query.id:
             #  mypy casts are only used as hints for the type checker,
             #  and they don’t perform a runtime type check.
             return cast(SynthesisResponse, self._monitoring_feature_access.retrieve(query=query))
         else:
             #  mypy casts are only used as hints for the type checker,
             #  and they don’t perform a runtime type check.
             return cast(DataSourceModelIterator,
```

### Comparing `basin3d-0.4.1/basin3d.egg-info/PKG-INFO` & `basin3d-0.4.2/basin3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basin3d
-Version: 0.4.1
+Version: 0.4.2
 Summary: BASIN-3D Core Framework
 Author-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>, Charuleka Varadharajan <cvaradharajan@lbl.gov>, Catherine Wong <catwong@lbl.gov>
 Maintainer-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>
 License: Broker for Assimilation, Synthesis and Integration of eNvironmental Diverse, Distributed Datasets (BASIN-3D) Copyright (c) 2019, The
         Regents of the University of California, through Lawrence Berkeley National
         Laboratory (subject to receipt of any required approvals from the U.S.
         Dept. of Energy).  All rights reserved.
```

### Comparing `basin3d-0.4.1/basin3d.egg-info/SOURCES.txt` & `basin3d-0.4.2/basin3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.1/pyproject.toml` & `basin3d-0.4.2/pyproject.toml`

 * *Files identical despite different names*

