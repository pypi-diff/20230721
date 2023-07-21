# Comparing `tmp/timesketch-api-client-20230208.tar.gz` & `tmp/timesketch-api-client-20230721.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timesketch-api-client-20230208.tar", last modified: Wed Feb  8 18:57:02 2023, max compression
+gzip compressed data, was "timesketch-api-client-20230721.tar", last modified: Fri Jul 21 12:14:03 2023, max compression
```

## Comparing `timesketch-api-client-20230208.tar` & `timesketch-api-client-20230721.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 18:57:02.349488 timesketch-api-client-20230208/
--rw-r--r--   0 root         (0) root         (0)      993 2023-02-08 18:57:02.349488 timesketch-api-client-20230208/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-08 18:57:02.349488 timesketch-api-client-20230208/setup.cfg
--rw-r-----   0 root         (0) root         (0)     2331 2022-05-04 12:34:04.000000 timesketch-api-client-20230208/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 18:57:02.313485 timesketch-api-client-20230208/timesketch_api_client/
--rw-r-----   0 root         (0) root         (0)        0 2021-02-05 08:50:03.000000 timesketch-api-client-20230208/timesketch_api_client/__init__.py
--rw-r-----   0 root         (0) root         (0)    22168 2022-05-04 12:34:04.000000 timesketch-api-client-20230208/timesketch_api_client/aggregation.py
--rw-r-----   0 root         (0) root         (0)     6557 2022-05-04 12:34:04.000000 timesketch-api-client-20230208/timesketch_api_client/analyzer.py
--rw-r-----   0 root         (0) root         (0)     2924 2022-05-04 12:34:04.000000 timesketch-api-client-20230208/timesketch_api_client/cli_input.py
--rw-r-----   0 root         (0) root         (0)    23687 2023-02-08 12:08:40.000000 timesketch-api-client-20230208/timesketch_api_client/client.py
--rw-r-----   0 root         (0) root         (0)     1887 2022-05-04 12:34:04.000000 timesketch-api-client-20230208/timesketch_api_client/client_test.py
--rw-r-----   0 root         (0) root         (0)    20805 2022-05-04 12:34:04.000000 timesketch-api-client-20230208/timesketch_api_client/config.py
--rw-r-----   0 root         (0) root         (0)     3847 2022-05-04 12:34:04.000000 timesketch-api-client-20230208/timesketch_api_client/config_test.py
--rw-r-----   0 root         (0) root         (0)     5273 2022-05-04 12:34:04.000000 timesketch-api-client-20230208/timesketch_api_client/credentials.py
--rw-r-----   0 root         (0) root         (0)     6887 2022-05-04 12:34:04.000000 timesketch-api-client-20230208/timesketch_api_client/crypto.py
--rw-r-----   0 root         (0) root         (0)     1034 2021-02-05 08:50:03.000000 timesketch-api-client-20230208/timesketch_api_client/definitions.py
--rw-r-----   0 root         (0) root         (0)     4099 2022-05-04 12:34:04.000000 timesketch-api-client-20230208/timesketch_api_client/error.py
--rw-r-----   0 root         (0) root         (0)    16297 2022-05-04 12:34:04.000000 timesketch-api-client-20230208/timesketch_api_client/graph.py
--rw-r-----   0 root         (0) root         (0)     1301 2022-05-04 12:34:04.000000 timesketch-api-client-20230208/timesketch_api_client/graph_test.py
--rw-r-----   0 root         (0) root         (0)     4741 2022-05-04 12:34:04.000000 timesketch-api-client-20230208/timesketch_api_client/index.py
--rw-r-----   0 root         (0) root         (0)     5759 2022-05-04 12:34:04.000000 timesketch-api-client-20230208/timesketch_api_client/resource.py
--rw-r-----   0 root         (0) root         (0)    37836 2022-10-20 13:02:09.000000 timesketch-api-client-20230208/timesketch_api_client/search.py
--rw-r-----   0 root         (0) root         (0)     8394 2022-05-04 12:34:04.000000 timesketch-api-client-20230208/timesketch_api_client/search_test.py
--rw-r-----   0 root         (0) root         (0)     8067 2023-02-02 17:28:54.000000 timesketch-api-client-20230208/timesketch_api_client/searchtemplate.py
--rw-r-----   0 root         (0) root         (0)     5293 2023-02-08 12:08:40.000000 timesketch-api-client-20230208/timesketch_api_client/sigma.py
--rw-r-----   0 root         (0) root         (0)     4122 2023-02-08 12:08:40.000000 timesketch-api-client-20230208/timesketch_api_client/sigma_test.py
--rw-r-----   0 root         (0) root         (0)    68750 2022-11-11 09:17:24.000000 timesketch-api-client-20230208/timesketch_api_client/sketch.py
--rw-r-----   0 root         (0) root         (0)     3094 2022-11-11 09:17:24.000000 timesketch-api-client-20230208/timesketch_api_client/sketch_test.py
--rw-r-----   0 root         (0) root         (0)    22989 2022-05-04 12:34:04.000000 timesketch-api-client-20230208/timesketch_api_client/story.py
--rw-r-----   0 root         (0) root         (0)     1982 2022-05-04 12:34:04.000000 timesketch-api-client-20230208/timesketch_api_client/story_test.py
--rw-r-----   0 root         (0) root         (0)    17216 2022-11-11 09:17:24.000000 timesketch-api-client-20230208/timesketch_api_client/test_lib.py
--rw-r-----   0 root         (0) root         (0)    14212 2022-09-22 13:24:21.000000 timesketch-api-client-20230208/timesketch_api_client/timeline.py
--rw-r-----   0 root         (0) root         (0)     1434 2022-05-04 12:34:04.000000 timesketch-api-client-20230208/timesketch_api_client/timeline_test.py
--rw-r-----   0 root         (0) root         (0)     3300 2022-05-04 12:34:04.000000 timesketch-api-client-20230208/timesketch_api_client/user.py
--rw-r-----   0 root         (0) root         (0)      763 2023-02-08 18:54:41.000000 timesketch-api-client-20230208/timesketch_api_client/version.py
--rw-r-----   0 root         (0) root         (0)     4018 2022-05-04 12:34:04.000000 timesketch-api-client-20230208/timesketch_api_client/view.py
--rw-r-----   0 root         (0) root         (0)     1318 2022-05-04 12:34:04.000000 timesketch-api-client-20230208/timesketch_api_client/view_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 18:57:02.349488 timesketch-api-client-20230208/timesketch_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      993 2023-02-08 18:57:01.000000 timesketch-api-client-20230208/timesketch_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1370 2023-02-08 18:57:01.000000 timesketch-api-client-20230208/timesketch_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-08 18:57:01.000000 timesketch-api-client-20230208/timesketch_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-06 10:49:27.000000 timesketch-api-client-20230208/timesketch_api_client.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       93 2023-02-08 18:57:01.000000 timesketch-api-client-20230208/timesketch_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-02-08 18:57:01.000000 timesketch-api-client-20230208/timesketch_api_client.egg-info/top_level.txt
+drwxr-x---   0 jbn      (190240) primarygroup (89939)        0 2023-07-21 12:12:56.557190 timesketch-api-client-20230721/
+-rw-r-----   0 jbn      (190240) primarygroup (89939)      974 2023-07-21 12:14:03.710418 timesketch-api-client-20230721/PKG-INFO
+-rw-r-----   0 jbn      (190240) primarygroup (89939)       38 2023-07-21 12:14:03.710418 timesketch-api-client-20230721/setup.cfg
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     2331 2022-05-04 12:34:04.000000 timesketch-api-client-20230721/setup.py
+drwxr-x---   0 jbn      (190240) primarygroup (89939)        0 2023-07-21 12:12:56.537188 timesketch-api-client-20230721/timesketch_api_client/
+-rw-r-----   0 jbn      (190240) primarygroup (89939)        0 2021-02-05 08:50:03.000000 timesketch-api-client-20230721/timesketch_api_client/__init__.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)    22589 2023-06-13 06:36:18.000000 timesketch-api-client-20230721/timesketch_api_client/aggregation.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     6947 2023-06-13 06:36:18.000000 timesketch-api-client-20230721/timesketch_api_client/aggregation_test.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     6599 2023-05-10 10:48:06.000000 timesketch-api-client-20230721/timesketch_api_client/analyzer.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     2924 2022-05-04 12:34:04.000000 timesketch-api-client-20230721/timesketch_api_client/cli_input.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)    24585 2023-05-10 10:48:06.000000 timesketch-api-client-20230721/timesketch_api_client/client.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     1887 2022-05-04 12:34:04.000000 timesketch-api-client-20230721/timesketch_api_client/client_test.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)    21112 2023-05-26 10:36:03.000000 timesketch-api-client-20230721/timesketch_api_client/config.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     3847 2022-05-04 12:34:04.000000 timesketch-api-client-20230721/timesketch_api_client/config_test.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     5273 2022-05-04 12:34:04.000000 timesketch-api-client-20230721/timesketch_api_client/credentials.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     6884 2023-05-26 10:36:03.000000 timesketch-api-client-20230721/timesketch_api_client/crypto.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     1034 2021-02-05 08:50:03.000000 timesketch-api-client-20230721/timesketch_api_client/definitions.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     4099 2022-05-04 12:34:04.000000 timesketch-api-client-20230721/timesketch_api_client/error.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)    16294 2023-05-26 10:36:03.000000 timesketch-api-client-20230721/timesketch_api_client/graph.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     1301 2022-05-04 12:34:04.000000 timesketch-api-client-20230721/timesketch_api_client/graph_test.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     4742 2023-05-10 10:48:06.000000 timesketch-api-client-20230721/timesketch_api_client/index.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     5759 2022-05-04 12:34:04.000000 timesketch-api-client-20230721/timesketch_api_client/resource.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)    37833 2023-05-26 10:36:03.000000 timesketch-api-client-20230721/timesketch_api_client/search.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     8394 2022-05-04 12:34:04.000000 timesketch-api-client-20230721/timesketch_api_client/search_test.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     8062 2023-05-26 10:36:03.000000 timesketch-api-client-20230721/timesketch_api_client/searchtemplate.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     5296 2023-02-13 08:57:20.000000 timesketch-api-client-20230721/timesketch_api_client/sigma.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     4123 2023-02-13 08:57:20.000000 timesketch-api-client-20230721/timesketch_api_client/sigma_test.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)    71384 2023-07-21 11:33:16.000000 timesketch-api-client-20230721/timesketch_api_client/sketch.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     3656 2023-06-13 06:36:18.000000 timesketch-api-client-20230721/timesketch_api_client/sketch_test.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)    22989 2022-05-04 12:34:04.000000 timesketch-api-client-20230721/timesketch_api_client/story.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     1982 2022-05-04 12:34:04.000000 timesketch-api-client-20230721/timesketch_api_client/story_test.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)    26368 2023-06-13 06:36:18.000000 timesketch-api-client-20230721/timesketch_api_client/test_lib.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)    14212 2022-09-22 13:24:21.000000 timesketch-api-client-20230721/timesketch_api_client/timeline.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     1434 2022-05-04 12:34:04.000000 timesketch-api-client-20230721/timesketch_api_client/timeline_test.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     3300 2022-05-04 12:34:04.000000 timesketch-api-client-20230721/timesketch_api_client/user.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)      763 2023-07-21 11:58:10.000000 timesketch-api-client-20230721/timesketch_api_client/version.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     4018 2022-05-04 12:34:04.000000 timesketch-api-client-20230721/timesketch_api_client/view.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     1318 2022-05-04 12:34:04.000000 timesketch-api-client-20230721/timesketch_api_client/view_test.py
+drwxr-x---   0 jbn      (190240) primarygroup (89939)        0 2023-07-21 12:14:03.710418 timesketch-api-client-20230721/timesketch_api_client.egg-info/
+-rw-r--r--   0 jbn      (190240) primarygroup (89939)      974 2023-07-21 12:14:03.000000 timesketch-api-client-20230721/timesketch_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 jbn      (190240) primarygroup (89939)     1412 2023-07-21 12:14:03.000000 timesketch-api-client-20230721/timesketch_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jbn      (190240) primarygroup (89939)        1 2023-07-21 12:14:03.000000 timesketch-api-client-20230721/timesketch_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jbn      (190240) primarygroup (89939)        1 2022-02-06 10:49:27.000000 timesketch-api-client-20230721/timesketch_api_client.egg-info/not-zip-safe
+-rw-r--r--   0 jbn      (190240) primarygroup (89939)       93 2023-07-21 12:14:03.000000 timesketch-api-client-20230721/timesketch_api_client.egg-info/requires.txt
+-rw-r--r--   0 jbn      (190240) primarygroup (89939)       22 2023-07-21 12:14:03.000000 timesketch-api-client-20230721/timesketch_api_client.egg-info/top_level.txt
```

### Comparing `timesketch-api-client-20230208/PKG-INFO` & `timesketch-api-client-20230721/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: timesketch-api-client
-Version: 20230208
+Version: 20230721
 Summary: Timesketch API client
 Home-page: http://www.timesketch.org/
 Maintainer: Timesketch development team
 Maintainer-email: timesketch-dev@googlegroups.com
 License: Apache License, Version 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 
 The Timesketch API client provides you with a set of Python libraries to connect to your Timesketch (https://github.com/google/timesketch) instance.
 
 The API is feature complete with the Timesketch UI and allows you to do all operations that can be done in the UI, providing ways to integrate Timesketch into other products such as Jupyter/Colab.
 
 To see how it works in action, try the colab notebook that is accessible from here: https://colab.research.google.com/github/google/timesketch/blob/master/notebooks/colab-timesketch-demo.ipynb
-
```

### Comparing `timesketch-api-client-20230208/setup.py` & `timesketch-api-client-20230721/setup.py`

 * *Files identical despite different names*

### Comparing `timesketch-api-client-20230208/timesketch_api_client/aggregation.py` & `timesketch-api-client-20230721/timesketch_api_client/aggregation.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,18 +39,19 @@
         type: the type of aggregation object.
         search_id: a search ID if the aggregation is tied to a specific
             saved search.
     """
 
     def __init__(self, sketch):
         self._created_at = ""
+        self._name = ""
         self._parameters = {}
         self._updated_at = ""
         self._group_id = None
-        self.aggregator_name = ""
+        self._aggregator_name = ""
         self.chart_color = ""
         self.chart_type = ""
         self.chart_title = ""
         self.search_id = None
         self.type = None
         resource_uri = "sketches/{0:d}/aggregation/explore/".format(sketch.id)
         super().__init__(sketch=sketch, resource_uri=resource_uri)
@@ -109,15 +110,15 @@
 
         if chart_type:
             self.chart_type = chart_type
 
         if search_id:
             self.search_id = search_id
 
-        self.aggregator_name = aggregator_name
+        self._aggregator_name = aggregator_name
         self.chart_color = parameters.get("chart_color", "")
         self._parameters = parameters
 
         form_data = {
             "aggregator_name": aggregator_name,
             "aggregator_parameters": parameters,
             "chart_type": chart_type,
@@ -145,17 +146,18 @@
         )
         self._resource_id = aggregation_id
         resource_data = self.api.fetch_resource_data(resource_uri)
         data = resource_data.get("objects", [None])[0]
         if not data:
             return
 
-        self.aggregator_name = data.get("agg_type")
+        self._aggregator_name = data.get("agg_type")
         self.type = "stored"
 
+        self._name = data.get("name", "")
         self._created_at = data.get("created_at", "")
         self._updated_at = data.get("updated_at", "")
         self._group_id = data.get("aggregationgroup_id")
 
         label_string = data.get("label_string", "")
         if label_string:
             self._labels = json.loads(label_string)
@@ -169,15 +171,15 @@
         else:
             parameters = {}
 
         self._parameters = parameters
 
         self._username = data.get("user", {}).get("username", "System")
         self.resource_data = self._run_aggregator(
-            aggregator_name=self.aggregator_name,
+            aggregator_name=self._aggregator_name,
             parameters=parameters,
             chart_type=chart_type,
         )
 
     # pylint: disable=arguments-differ
     def from_manual(self, aggregate_dsl, **kwargs):
         """Initialize the aggregation object by running an aggregation DSL.
@@ -186,15 +188,15 @@
             aggregate_dsl: OpenSearch aggregation query DSL string.
         """
         super().from_manual(**kwargs)
         resource_url = "{0:s}/sketches/{1:d}/aggregation/explore/".format(
             self.api.api_root, self._sketch.id
         )
 
-        self.aggregator_name = "DSL"
+        self._aggregator_name = "DSL"
         self._username = getpass.getuser()
         self.type = "DSL"
 
         date_now = datetime.datetime.now(datetime.timezone.utc)
         self._created_at = date_now.isoformat()
         self._updated_at = date_now.isoformat()
 
@@ -207,15 +209,19 @@
             error.error_message(
                 response, message="Unable to query results", error=ValueError
             )
 
         self.resource_data = error.get_response_json(response, logger)
 
     def from_aggregator_run(
-        self, aggregator_name, aggregator_parameters, search_id=None, chart_type=None
+        self,
+        aggregator_name,
+        aggregator_parameters,
+        search_id=None,
+        chart_type=None,
     ):
         """Initialize the aggregation object by running an aggregator class.
 
         Args:
             aggregator_name: name of the aggregator class to run.
             aggregator_parameters: a dict with the parameters of the aggregator
                 class.
@@ -266,14 +272,16 @@
     @property
     def title(self):
         """Property that returns the chart title of an aggregation."""
         if self.chart_title:
             return self.chart_title
 
         data = self.lazyload_data()
+        if not data:
+            return ""
         meta = data.get("meta", {})
         self.chart_title = meta.get("vega_chart_title", "")
 
         return self.chart_title
 
     @title.setter
     def title(self, new_title):
@@ -284,44 +292,53 @@
     def chart(self):
         """Property that returns an altair Vega-lite chart."""
         return self.generate_chart()
 
     @property
     def description(self):
         """Property that returns the description string."""
-        data = self.resource_data
+        data = self.lazyload_data()
+        if not data:
+            return ""
         meta = data.get("meta", {})
         return meta.get("description", "")
 
     @description.setter
     def description(self, description):
         """Set the description of an aggregation."""
         if "meta" not in self.resource_data:
             return
         meta = self.resource_data.get("meta")
         meta["description"] = description
 
     @property
     def name(self):
         """Property that returns the name of the aggregation."""
-        data = self.resource_data
-        meta = data.get("meta", {})
-        name = meta.get("name")
-        if name:
-            return name
-        return self.aggregator_name
+        return self._name
 
     @name.setter
     def name(self, name):
         """Set the name of the aggregation."""
         if "meta" not in self.resource_data:
             return
         meta = self.resource_data.get("meta")
         meta["name"] = name
 
+    @property
+    def aggregator_name(self):
+        """Property that returns the aggregator name."""
+        if self._aggregator_name:
+            return self._aggregator_name
+
+        data = self.resource_data
+        meta = data.get("meta", {})
+        self._aggregator_name = meta.get("name")
+
+        return self._aggregator_name
+
     def add_label(self, label):
         """Add a label to the aggregation.
 
         Args:
             label (str): string with the label information.
         """
         if label in self._labels:
@@ -373,15 +390,15 @@
         return altair.Chart.from_json(vega_spec_string)
 
     def save(self):
         """Save the aggregation in the database."""
         data = {
             "name": self.name,
             "description": self.description,
-            "agg_type": self.aggregator_name,
+            "agg_type": self._aggregator_name,
             "parameters": self._parameters,
             "chart_type": self.chart_type,
         }
         if self.search_id:
             data["view_id"] = self.search_id
         if self._labels:
             data["labels"] = json.dumps(self._labels)
@@ -604,14 +621,16 @@
 
     def generate_chart(self):
         """Returns an altair Vega-lite chart."""
         if not self._aggregations:
             return altair.Chart()
 
         data = self.lazyload_data()
+        if not data:
+            return None
 
         meta = data.get("meta", {})
         vega_spec = meta.get("vega_spec")
 
         if not vega_spec:
             return altair.Chart(pandas.DataFrame()).mark_point()
```

### Comparing `timesketch-api-client-20230208/timesketch_api_client/analyzer.py` & `timesketch-api-client-20230721/timesketch_api_client/analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,15 +107,16 @@
     @property
     def log(self):
         """Returns back logs from the analyzer session, if there are any."""
         return_strings = []
         for entry in self._get_status_data():
             return_strings.append(
                 "[{0:s}] = {1:s}".format(
-                    entry.get("name", "No Name"), entry.get("log", "No recorded logs.")
+                    entry.get("name", "No Name"),
+                    entry.get("log", "No recorded logs."),
                 )
             )
         return "\n".join(return_strings)
 
     @property
     def results(self):
         """Returns the results from the analyzer session."""
@@ -145,15 +146,16 @@
     @property
     def status(self):
         """Returns the current status of the analyzer run."""
         return_strings = []
         for entry in self._get_status_data():
             return_strings.append(
                 "[{0:s}] = {1:s}".format(
-                    entry.get("name", "No Name"), entry.get("status", "Unknown.")
+                    entry.get("name", "No Name"),
+                    entry.get("status", "Unknown."),
                 )
             )
         return "\n".join(return_strings)
 
     @property
     def status_dict(self):
         """Returns the current status of the analyzers run as a dict."""
```

### Comparing `timesketch-api-client-20230208/timesketch_api_client/cli_input.py` & `timesketch-api-client-20230721/timesketch_api_client/cli_input.py`

 * *Files identical despite different names*

### Comparing `timesketch-api-client-20230208/timesketch_api_client/client.py` & `timesketch-api-client-20230721/timesketch_api_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 # pylint: disable=wrong-import-order
 import bs4
 import requests
 
 # pylint: disable=redefined-builtin
 from requests.exceptions import ConnectionError
+from urllib3.exceptions import InsecureRequestWarning
 import webbrowser
 
 # pylint: disable-msg=import-error
 from google_auth_oauthlib import flow as googleauth_flow
 import google.auth.transport.requests
 import pandas
 
@@ -342,14 +343,16 @@
         # If using HTTP Basic auth, add the user/pass to the session
         if auth_mode == "http-basic":
             session.auth = (username, password)
 
         # SSL Cert verification is turned on by default.
         if not verify:
             session.verify = False
+            # disable warnings, since user actively decided to set verify to false
+            requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
 
         # Get and set CSRF token and authenticate the session if appropriate.
         self._set_csrf_token(session)
         if auth_mode == "userpass":
             self._authenticate_session(session, username, password)
 
         return session
@@ -359,28 +362,47 @@
 
         Args:
             resource_uri: The URI to the resource to be fetched.
             params: Dict of URL parameters to send in the GET request.
 
         Returns:
             Dictionary with the response data.
+
+        Raises:
+            RuntimeError: If response could not be JSON-decoded after
+                DEFAULT_RETRY_COUNT attempts.
         """
         resource_url = "{0:s}/{1:s}".format(self.api_root, resource_uri)
         response = self.session.get(resource_url, params=params)
-        return error.get_response_json(response, logger)
+
+        retry_count = 0
+        while True:
+            result = error.get_response_json(response, logger)
+            # Any dict with content is good enough for us to return.
+            if result:
+                return result
+            retry_count += 1
+            if retry_count >= self.DEFAULT_RETRY_COUNT:
+                raise RuntimeError(
+                    f"Unable to fetch JSON resource data. Response: {str(result)}"
+                )
 
     def create_sketch(self, name, description=None):
         """Create a new sketch.
 
         Args:
             name: Name of the sketch.
             description: Description of the sketch.
 
         Returns:
             Instance of a Sketch object.
+
+        Raises:
+            RuntimeError: If response does not contain an 'objects' key after
+                DEFAULT_RETRY_COUNT attempts.
         """
         if not description:
             description = name
 
         retry_count = 0
         objects = None
         while True:
@@ -580,15 +602,15 @@
             or
             - a pandas Dataframe with all rules if as_pandas is True.
 
         Raises:
             ValueError: If no rules are found.
         """
         rules = []
-        response = self.fetch_resource_data("sigmarule/")
+        response = self.fetch_resource_data("sigmarules/")
 
         if not response:
             raise ValueError("No rules found.")
 
         if as_pandas:
             return pandas.DataFrame.from_records(response.get("objects"))
 
@@ -601,15 +623,15 @@
                 index_obj.set_value(key, value)
             rules.append(index_obj)
         return rules
 
     def create_sigmarule(self, rule_yaml):
         """Adds a single Sigma rule to the database.
 
-        Adds a single Sigma rule to the database when `/sigmarule/` is called
+        Adds a single Sigma rule to the database when `/sigmarules/` is called
         with a POST request.
 
         All attributes of the rule are taken by the `rule_yaml` value in the
         POST request.
 
         If no `rule_yaml` is found in the request, the method will fail as this
         is required to parse the rule.
@@ -620,15 +642,15 @@
         Returns:
             Instance of a Sigma object.
         """
 
         retry_count = 0
         objects = None
         while True:
-            resource_url = "{0:s}/sigmarule/".format(self.api_root)
+            resource_url = "{0:s}/sigmarules/".format(self.api_root)
             form_data = {"rule_yaml": rule_yaml}
             response = self.session.post(resource_url, json=form_data)
             response_dict = error.get_response_json(response, logger)
             objects = response_dict.get("objects")
             if objects:
                 break
             retry_count += 1
@@ -636,15 +658,15 @@
             if retry_count >= self.DEFAULT_RETRY_COUNT:
                 raise RuntimeError("Unable to create a new Sigma Rule.")
 
         rule_uuid = objects[0]["rule_uuid"]
         return self.get_sigmarule(rule_uuid)
 
     def get_sigmarule(self, rule_uuid):
-        """Fetches a single Sigma rule from the databse.
+        """Fetches a single Sigma rule from the database.
         Fetches a single Sigma rule selected by the `UUID`
 
         Args:
             rule_uuid: UUID of the Sigma rule.
 
         Returns:
             Instance of a SigmaRule object.
```

### Comparing `timesketch-api-client-20230208/timesketch_api_client/client_test.py` & `timesketch-api-client-20230721/timesketch_api_client/client_test.py`

 * *Files identical despite different names*

### Comparing `timesketch-api-client-20230208/timesketch_api_client/config.py` & `timesketch-api-client-20230721/timesketch_api_client/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,15 +237,15 @@
 
         Raises:
           IOError if the file does not exist or config does not load.
         """
         if config_file_path:
             if not os.path.isfile(config_file_path):
                 error_msg = (
-                    "Unable to load config file, file {0:s} does not " "exist."
+                    "Unable to load config file, file {0:s} does not exist."
                 ).format(config_file_path)
                 logger.error(error_msg)
                 raise IOError(error_msg)
         else:
             home_path = os.path.expanduser("~")
             config_file_path = os.path.join(home_path, self.RC_FILENAME)
 
@@ -270,14 +270,21 @@
             logger.warning("No %s section in the config", section)
             return
 
         timesketch_config = config[section]
         for name, value in timesketch_config.items():
             self.set_config(name, value)
 
+        # verify is expected to be a boolean but will be read from file as string
+        # therefore, we need to overwrite it here
+        if self.get_config("verify") == "False":
+            self.set_config("verify", False)
+        else:
+            self.set_config("verify", True)
+
         if load_cli_config:
             if "cli" not in config.sections():
                 # Set default CLI config section
                 config["cli"] = {"sketch": "", "output_format": "tabular"}
 
             cli_config = config["cli"]
             for name, value in cli_config.items():
@@ -414,15 +421,17 @@
 
     Returns:
         A timesketch client (TimesketchApi) or None if not possible.
     """
     assistant = ConfigAssistant()
     try:
         assistant.load_config_file(
-            config_path, section=config_section, load_cli_config=load_cli_config
+            config_path,
+            section=config_section,
+            load_cli_config=load_cli_config,
         )
         if config_dict:
             assistant.load_config_dict(config_dict)
     except IOError as e:
         logger.error("Unable to load the config file, is it valid?")
         logger.error("Error: %s", e)
```

### Comparing `timesketch-api-client-20230208/timesketch_api_client/config_test.py` & `timesketch-api-client-20230721/timesketch_api_client/config_test.py`

 * *Files identical despite different names*

### Comparing `timesketch-api-client-20230208/timesketch_api_client/credentials.py` & `timesketch-api-client-20230721/timesketch_api_client/credentials.py`

 * *Files identical despite different names*

### Comparing `timesketch-api-client-20230208/timesketch_api_client/crypto.py` & `timesketch-api-client-20230721/timesketch_api_client/crypto.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         elif config_assistant:
             try:
                 password = config_assistant.get_config("cred_key")
                 if not isinstance(password, bytes):
                     password = bytes(password, "utf-8")
             except KeyError as exc:
                 raise IOError(
-                    "Not able to determine encryption key from " "config."
+                    "Not able to determine encryption key from config."
                 ) from exc
         else:
             raise IOError(
                 "Neither password nor a configuration assistant passed to "
                 "tool, unable to determine password."
             )
```

### Comparing `timesketch-api-client-20230208/timesketch_api_client/definitions.py` & `timesketch-api-client-20230721/timesketch_api_client/definitions.py`

 * *Files identical despite different names*

### Comparing `timesketch-api-client-20230208/timesketch_api_client/error.py` & `timesketch-api-client-20230721/timesketch_api_client/error.py`

 * *Files identical despite different names*

### Comparing `timesketch-api-client-20230208/timesketch_api_client/graph.py` & `timesketch-api-client-20230721/timesketch_api_client/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,15 @@
         """
         resource_id = f"sketches/{self._sketch.id}/graphs/{graph_id}/"
         data = self.api.fetch_resource_data(resource_id)
 
         objects = data.get("objects")
         if not objects:
             logger.warning(
-                "Unable to load saved graph with ID: %d, " "are you sure it exists?",
+                "Unable to load saved graph with ID: %d, are you sure it exists?",
                 graph_id,
             )
         graph_dict = objects[0]
         self._parse_graph_dict(graph_dict)
 
         self._resource_id = graph_id
         self._name = graph_dict.get("name", "No name")
```

### Comparing `timesketch-api-client-20230208/timesketch_api_client/graph_test.py` & `timesketch-api-client-20230721/timesketch_api_client/graph_test.py`

 * *Files identical despite different names*

### Comparing `timesketch-api-client-20230208/timesketch_api_client/index.py` & `timesketch-api-client-20230721/timesketch_api_client/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     def index_name(self):
         """Property that returns OpenSearch index name.
 
         Returns:
             OpenSearch index name as string.
         """
         index_data = self._get_object_dict()
-        return index_data.get("index_name", "unkown index name")
+        return index_data.get("index_name", "unknown index name")
 
     @property
     def status(self):
         """Property that returns the index status.
 
         Returns:
             String with the index status.
```

### Comparing `timesketch-api-client-20230208/timesketch_api_client/resource.py` & `timesketch-api-client-20230721/timesketch_api_client/resource.py`

 * *Files identical despite different names*

### Comparing `timesketch-api-client-20230208/timesketch_api_client/search.py` & `timesketch-api-client-20230721/timesketch_api_client/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -569,15 +569,15 @@
             response_json["meta"]["es_time"] += added_time
 
         self._total_elastic_size = response_json.get("meta", {}).get(
             "es_total_count", 0
         )
         if self._total_elastic_size != total_count:
             logger.info(
-                "%d results were returned, but " "%d records matched the search query",
+                "%d results were returned, but %d records matched the search query",
                 total_count,
                 self._total_elastic_size,
             )
 
         self._raw_response = response_json
 
     def add_chip(self, chip):
```

### Comparing `timesketch-api-client-20230208/timesketch_api_client/search_test.py` & `timesketch-api-client-20230721/timesketch_api_client/search_test.py`

 * *Files identical despite different names*

### Comparing `timesketch-api-client-20230208/timesketch_api_client/searchtemplate.py` & `timesketch-api-client-20230721/timesketch_api_client/searchtemplate.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 class SearchTemplate(resource.BaseResource):
     """Search template object. TEST e2e"""
 
     def __init__(self, api):
         """Initialize the search template object."""
-        super().__init__(api, "searchtemplate/")
+        super().__init__(api, "searchtemplates/")
         self._description = ""
         self._name = ""
         self._resource_id = None
         self._search_id = None
         self._sketch_id = None
 
     @property
@@ -57,15 +57,15 @@
         """Deletes the saved graph from the store."""
         if not self._resource_id:
             raise ValueError(
                 "Unable to delete the search template, since the template "
                 "does not seem to be saved, which is required."
             )
 
-        resource_url = f"{self.api.api_root}/searchtemplate/{self._resource_id}/"
+        resource_url = f"{self.api.api_root}/searchtemplates/{self._resource_id}/"
         response = self.api.session.delete(resource_url)
         return error.check_return_status(response, logger)
 
     def from_saved(self, template_id, sketch_id=0):
         """Initialize the search template from a saved template, by ID value.
 
         Args:
@@ -73,15 +73,15 @@
             sketch_id: optional integer value for a sketch ID. If not
                 provided, an attempt is made to figure it out.
 
         Raises:
             ValueError: If issues came up during processing.
         """
         self._resource_id = template_id
-        self.resource_uri = f"searchtemplate/{self._resource_id}/"
+        self.resource_uri = f"searchtemplates/{self._resource_id}/"
 
         if sketch_id:
             self._sketch_id = sketch_id
         else:
             data = self.lazyload_data(refresh_cache=True)
             meta = data.get("meta", {})
             sketch_ids = meta.get("sketch_ids", [])
@@ -98,26 +98,26 @@
 
         Args:
             search_obj (search.Search): a search object.
         """
         self._search_id = search_obj.id
         self._sketch_id = search_obj.sketch.id
 
-        response = self.api.fetch_resource_data("searchtemplate/")
+        response = self.api.fetch_resource_data("searchtemplates/")
         meta = response.get("meta", {})
         template_id = 0
         for data in meta.get("collection", []):
             if data.get("search_id") == self._search_id:
                 template_id = data.get("template_id", 0)
 
         if not template_id:
             return
 
         self._resource_id = template_id
-        self.resource_uri = f"searchtemplate/{self._resource_id}/"
+        self.resource_uri = f"searchtemplates/{self._resource_id}/"
 
     @property
     def id(self):
         """Property that returns back the search template ID."""
         return self._resource_id
 
     @property
@@ -155,15 +155,15 @@
 
         if sketch:
             self._sketch_id = sketch
         elif isinstance(sketch_id, int):
             self._sketch_id = sketch_id
         else:
             raise ValueError(
-                "Sketch needs to be set, or an integer value for " "a sketch ID."
+                "Sketch needs to be set, or an integer value for a sketch ID."
             )
 
     def save(self):
         """Save the search template."""
         if self._resource_id:
             raise ValueError(
                 "The template has already been saved, ATM updates to an "
@@ -176,47 +176,47 @@
                 "value of the saved search is not known. The object needs "
                 "to be initialized from a previously saved search."
             )
 
         data = {
             "search_id": self._search_id,
         }
-        resource_url = f"{self.api.api_root}/searchtemplate/"
+        resource_url = f"{self.api.api_root}/searchtemplates/"
         response = self.api.session.post(resource_url, json=data)
 
         status = error.check_return_status(response, logger)
         if not status:
             error.error_message(
                 response, "Unable to save search as a template", error=RuntimeError
             )
 
         response_json = error.get_response_json(response, logger)
         template_dict = response_json.get("objects", [{}])[0]
 
         self._resource_id = template_dict.get("id", 0)
-        self.resource_uri = f"searchtemplate/{self._resource_id}/"
+        self.resource_uri = f"searchtemplates/{self._resource_id}/"
         return f"Saved search as a template to ID: {self.id}"
 
     def to_search(self):
         """Returns a search object from a template."""
         if not self._resource_id:
             raise ValueError(
-                "Unable to get a search object unless it is tied to a " "template."
+                "Unable to get a search object unless it is tied to a template."
             )
 
         if not self._sketch_id:
             raise ValueError(
-                "Unable to get a search object unless it is tied to " "a sketch."
+                "Unable to get a search object unless it is tied to a sketch."
             )
 
         data = self.lazyload_data(refresh_cache=True)
         objects = data.get("objects")
         if not objects:
             raise ValueError(
-                "Unable to get search object, issue with retrieving " "template data."
+                "Unable to get search object, issue with retrieving template data."
             )
 
         template_dict = objects[0]
         sketch = self.api.get_sketch(self._sketch_id)
 
         search_obj = search.Search(sketch=sketch)
         search_obj.from_manual(
```

### Comparing `timesketch-api-client-20230208/timesketch_api_client/sigma.py` & `timesketch-api-client-20230721/timesketch_api_client/sigma.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         """Initializes the Sigma object.
 
         Args:
             api: An instance of TimesketchApi object.
 
         """
         self._attr_dict = {}
-        resource_uri = "sigmarule/"
+        resource_uri = "sigmarules/"
         super().__init__(api=api, resource_uri=resource_uri)
 
     @property
     def attributes(self):
         """Returns a list of all attribute keys for the rule"""
         return list(self._attr_dict.keys())
 
@@ -141,15 +141,15 @@
     def from_rule_uuid(self, rule_uuid):
         """Get a SigmaRule object from a rule UUID.
 
         Args:
             rule_uuid: Id of the sigma rule.
 
         """
-        self.resource_uri = f"sigmarule/{rule_uuid}"
+        self.resource_uri = f"sigmarules/{rule_uuid}"
 
         self.lazyload_data(refresh_cache=True)
         objects = self.data.get("objects")
         if not objects:
             error_msg = "Unable to parse Sigma rule {0} with given text".format(
                 rule_uuid
             )
@@ -164,15 +164,15 @@
 
         Args:
             rule_text: Rule text to be parsed.
 
         Raises:
             ValueError: If rule could not be parsed.
         """
-        self.resource_uri = "{0:s}/sigmarule/text/".format(self.api.api_root)
+        self.resource_uri = "{0:s}/sigmarules/text/".format(self.api.api_root)
         data = {"title": "Get_Sigma_by_text", "content": rule_text}
         response = self.api.session.post(self.resource_uri, json=data)
         response_dict = error.get_response_json(response, logger)
 
         objects = response_dict.get("objects")
         if not objects:
             error_msg = "Sigma rule Parsing error with provided rule"
```

### Comparing `timesketch-api-client-20230208/timesketch_api_client/sigma_test.py` & `timesketch-api-client-20230721/timesketch_api_client/sigma_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         self.assertIsNotNone(rule)
         self.assertIn("Alexander", rule.author)
         self.assertIn("Alexander", rule.get_attribute("author"))
         self.assertEqual(rule.id, "5266a592-b793-11ea-b3de-0242ac130004")
         self.assertEqual(rule.title, "Suspicious Installation of ZMap")
         self.assertIn("zmap", rule.search_query, "ES_Query does not match")
         self.assertIn("b793", rule.id)
-        self.assertIn("sigmarule/5266a592", rule.resource_uri)
+        self.assertIn("sigmarules/5266a592", rule.resource_uri)
         self.assertIn("suspicious installation of ZMap", rule.description)
         self.assertIn("high", rule.level)
         self.assertEqual(len(rule.falsepositives), 1)
         self.assertIn("Unknown", rule.falsepositives[0])
         self.assertIn("2020/06/26", rule.date)
         self.assertIn("2021/01/01", rule.modified)
         self.assertIn("high", rule.level)
```

### Comparing `timesketch-api-client-20230208/timesketch_api_client/sketch.py` & `timesketch-api-client-20230721/timesketch_api_client/sketch.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,19 @@
         """Property that returns the sketch attributes."""
         data = self.lazyload_data(refresh_cache=True)
         meta = data.get("meta", {})
         return meta.get("attributes", {})
 
     @property
     def attributes_table(self):
-        """Property that returns the sketch attributes as a data frame."""
+        """DEPRECATED: Property that returns the sketch attributes
+        as a data frame.
+
+        Given the fluid setup of attributes, this is not a good way to
+        represent the data. Use the attributes property instead."""
         data = self.lazyload_data(refresh_cache=True)
         meta = data.get("meta", {})
         attributes = meta.get("attributes", [])
 
         data_frame = pandas.DataFrame(attributes)
         data_frame.columns = ["attribute", "values", "ontology"]
 
@@ -404,15 +408,17 @@
             raise ValueError("You need to supply a query string or a dsl")
 
         if self.is_archived():
             raise RuntimeError("Unable create a view on an archived sketch.")
 
         search_obj = search.Search(sketch=self)
         search_obj.from_manual(
-            query_string=query_string, query_dsl=query_dsl, query_filter=query_filter
+            query_string=query_string,
+            query_dsl=query_dsl,
+            query_filter=query_filter,
         )
         search_obj.name = name
         search_obj.save()
         return search_obj
 
     def create_story(self, title):
         """Create a story object.
@@ -447,23 +453,27 @@
         story_dict = response_json.get("objects", [{}])[0]
         return story.Story(story_id=story_dict.get("id", 0), sketch=self, api=self.api)
 
     def delete(self):
         """Deletes the sketch."""
         if self.is_archived():
             raise RuntimeError(
-                "Unable to delete an archived sketch, first " "unarchive then delete."
+                "Unable to delete an archived sketch, first unarchive then delete."
             )
 
         resource_url = "{0:s}/sketches/{1:d}/".format(self.api.api_root, self.id)
         response = self.api.session.delete(resource_url)
         return error.check_return_status(response, logger)
 
     def add_to_acl(
-        self, user_list=None, group_list=None, make_public=False, permissions=None
+        self,
+        user_list=None,
+        group_list=None,
+        make_public=False,
+        permissions=None,
     ):
         """Add users or groups to the sketch ACL.
 
         Args:
             user_list: optional list of users to add to the ACL
                 of the sketch. Each user is a string.
             group_list: optional list of groups to add to the ACL
@@ -853,15 +863,17 @@
 
         if not len(story_objects) == 1:
             return story_list
         stories = story_objects[0]
         for story_dict in stories:
             story_list.append(
                 story.Story(
-                    story_id=story_dict.get("id", -1), sketch=self, api=self.api
+                    story_id=story_dict.get("id", -1),
+                    sketch=self,
+                    api=self.api,
                 )
             )
         return story_list
 
     def list_views(self):
         """List all saved views for this sketch.
 
@@ -903,15 +915,15 @@
 
     def list_search_templates(self):
         """Get a list of all search templates that are available.
 
         Returns:
             List of searchtemplate.SearchTemplate object instances.
         """
-        response = self.api.fetch_resource_data("searchtemplate/")
+        response = self.api.fetch_resource_data("searchtemplates/")
         objects = response.get("objects", [])
         if not objects:
             return []
 
         template_dicts = objects[0]
 
         template_list = []
@@ -1085,15 +1097,19 @@
         )
 
         response = self.api.session.get(resource_url)
 
         return error.get_response_json(response, logger)
 
     def run_analyzer(
-        self, analyzer_name, analyzer_kwargs=None, timeline_id=None, timeline_name=None
+        self,
+        analyzer_name,
+        analyzer_kwargs=None,
+        timeline_id=None,
+        timeline_name=None,
     ):
         """Run an analyzer on a timeline.
 
         Args:
             analyzer_name: the name of the analyzer class to run against the
                 timeline.
             analyzer_kwargs: optional dict with parameters for the analyzer.
@@ -1123,17 +1139,15 @@
 
         if self.is_archived():
             raise error.UnableToRunAnalyzer(
                 "Unable to run an analyzer on an archived sketch."
             )
 
         if not timeline_id and not timeline_name:
-            return (
-                "Unable to run analyzer, need to define either " "timeline ID or name"
-            )
+            return "Unable to run analyzer, need to define either timeline ID or name"
 
         if timeline_name:
             sketch = self.lazyload_data(refresh_cache=True)
             timelines = []
             for timeline_dict in sketch["objects"][0]["timelines"]:
                 name = timeline_dict.get("name", "")
                 if timeline_name.lower() == name.lower():
@@ -1163,15 +1177,19 @@
         )
 
         return timeline_obj.run_analyzer(
             analyzer_name=analyzer_name, analyzer_kwargs=analyzer_kwargs
         )
 
     def remove_acl(
-        self, user_list=None, group_list=None, remove_public=False, permissions=None
+        self,
+        user_list=None,
+        group_list=None,
+        remove_public=False,
+        permissions=None,
     ):
         """Remove users or groups to the sketch ACL.
 
         Args:
             user_list: optional list of users to remove from the ACL
                 of the sketch. Each user is a string.
             group_list: optional list of groups to remove from the ACL
@@ -1287,21 +1305,27 @@
             An aggregation object (instance of Aggregator).
         """
         if self.is_archived():
             raise RuntimeError("Unable to run an aggregator on an archived sketch.")
 
         aggregation_obj = aggregation.Aggregation(sketch=self)
         aggregation_obj.from_aggregator_run(
-            aggregator_name=aggregator_name, aggregator_parameters=aggregator_parameters
+            aggregator_name=aggregator_name,
+            aggregator_parameters=aggregator_parameters,
         )
 
         return aggregation_obj
 
     def store_aggregation(
-        self, name, description, aggregator_name, aggregator_parameters, chart_type=""
+        self,
+        name,
+        description,
+        aggregator_name,
+        aggregator_parameters,
+        chart_type="",
     ):
         """Store an aggregation in the sketch.
 
         Args:
             name: a name that will be associated with the aggregation.
             description: description of the aggregation, visible in the UI.
             aggregator_name: name of the aggregator class.
@@ -1346,15 +1370,19 @@
         """
         if self.is_archived():
             raise RuntimeError("Unable to comment on an event in an archived sketch.")
 
         form_data = {
             "annotation": comment_text,
             "annotation_type": "comment",
-            "events": {"_id": event_id, "_index": index, "_type": "generic_event"},
+            "events": {
+                "_id": event_id,
+                "_index": index,
+                "_type": "generic_event",
+            },
         }
         resource_url = "{0:s}/sketches/{1:d}/event/annotate/".format(
             self.api.api_root, self.id
         )
         response = self.api.session.post(resource_url, json=form_data)
         return error.get_response_json(response, logger)
 
@@ -1425,14 +1453,80 @@
         }
         resource_url = "{0:s}/sketches/{1:d}/event/annotate/".format(
             self.api.api_root, self.id
         )
         response = self.api.session.post(resource_url, json=form_data)
         return error.get_response_json(response, logger)
 
+    def untag_events(self, events, tags_to_remove: list):
+        """Removes a list of tags from a list of events.
+
+        The upper limit is 500 (events or tags) based on the API.
+
+        Args:
+            events: events dict. Must have the structure:
+                "events": [
+                {
+                    "_id": event_id,
+                    "_index": index,
+                }
+            tags_to_remove: list of tags to remove
+
+        Returns:
+            HTTP response object.
+        """
+        if self.is_archived():
+            raise RuntimeError("Unable to untag events in an archived sketch.")
+
+        form_data = {
+            "tags_to_remove": tags_to_remove,
+            "events": events,
+        }
+        resource_url = "{0:s}/sketches/{1:d}/event/untag/".format(
+            self.api.api_root, self.id
+        )
+        response = self.api.session.post(resource_url, json=form_data)
+        return error.get_response_json(response, logger)
+
+    def untag_event(self, event_id: str, index, tag: str):
+        """Removes a tag from an event.
+
+        This method can be used if just one events needs to be untagged.
+
+        Note if called multiple times in a loop it is more efficient to use
+        the untag_events method.
+
+        To remove a list of tags from a list of tags, use a different method.
+
+        Args:
+            event_id: id of the event
+            index: The OpenSearch index name
+            tag: tag to remove
+
+        Returns:
+            HTTP response object.
+        """
+        if self.is_archived():
+            raise RuntimeError("Unable to untag events in an archived sketch.")
+
+        form_data = {
+            "tags_to_remove": [tag],
+            "events": [
+                {
+                    "_id": event_id,
+                    "_index": index,
+                }
+            ],
+        }
+        resource_url = "{0:s}/sketches/{1:d}/event/untag/".format(
+            self.api.api_root, self.id
+        )
+        response = self.api.session.post(resource_url, json=form_data)
+        return error.get_response_json(response, logger)
+
     def tag_events(self, events, tags, verbose=False):
         """Tags one or more events with a list of tags.
 
         Args:
             events: Array of JSON objects representing events.
             tags: List of tags (str) to add to the events.
             verbose: Bool that determines whether extra information
@@ -1683,15 +1777,17 @@
             self.api.api_root, self.id
         )
 
         response = self.api.session.post(resource_url, json=form_data)
         status = error.check_return_status(response, logger)
         if not status:
             error.error_message(
-                response, message="Failed exporting the sketch", error=RuntimeError
+                response,
+                message="Failed exporting the sketch",
+                error=RuntimeError,
             )
 
         with open(file_path, "wb") as fw:
             fw.write(response.content)
 
     def generate_timeline_from_es_index(
         self,
@@ -1755,15 +1851,17 @@
             "searchindex_name": index_name or es_index_name,
             "es_index_name": es_index_name,
         }
         response = self.api.session.post(resource_url, json=form_data)
 
         if response.status_code not in definitions.HTTP_STATUS_CODE_20X:
             error.error_message(
-                response, message="Error creating searchindex", error=ValueError
+                response,
+                message="Error creating searchindex",
+                error=ValueError,
             )
 
         response_dict = error.get_response_json(response, logger)
         objects = response_dict.get("objects")
         if not objects:
             raise ValueError(
                 "Unable to create a SearchIndex, try again or file an "
@@ -1793,22 +1891,24 @@
         # Step 4: Create the Timeline.
         resource_url = f"{self.api.api_root}/sketches/{self.id}/timelines/"
         form_data = {"timeline": searchindex_id, "timeline_name": name}
         response = self.api.session.post(resource_url, json=form_data)
 
         if response.status_code not in definitions.HTTP_STATUS_CODE_20X:
             error.error_message(
-                response, message="Error creating a timeline object", error=ValueError
+                response,
+                message="Error creating a timeline object",
+                error=ValueError,
             )
 
         response_dict = error.get_response_json(response, logger)
         objects = response_dict.get("objects")
         if not objects:
             raise ValueError(
-                "Unable to create a Timeline, try again or file an " "issue on GitHub."
+                "Unable to create a Timeline, try again or file an issue on GitHub."
             )
 
         timeline_dict = objects[0]
 
         timeline_obj = timeline.Timeline(
             timeline_id=timeline_dict["id"],
             sketch_id=self.id,
@@ -1839,15 +1939,17 @@
             "provider": provider,
             "context": context,
             "data_label": data_label,
         }
         response = self.api.session.post(resource_url, json=form_data)
         if response.status_code not in definitions.HTTP_STATUS_CODE_20X:
             error.error_message(
-                response, message="Error creating a datasource object", error=ValueError
+                response,
+                message="Error creating a datasource object",
+                error=ValueError,
             )
 
         _ = error.get_response_json(response, logger)
 
         return timeline_obj
 
     def run_data_finder(self, start_date, end_date, rule_names, timelines=None):
```

### Comparing `timesketch-api-client-20230208/timesketch_api_client/sketch_test.py` & `timesketch-api-client-20230721/timesketch_api_client/sketch_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -78,7 +78,20 @@
         self.assertEqual(response, expected_response)
 
     def test_add_event_attributes_invalid(self):
         """Confirm an exception is raised when events isn't a list."""
         events = {"_id": "1", "_type": "_doc", "index": "1", "attributes": []}
         with self.assertRaisesRegex(ValueError, "Events need to be a list."):
             self.sketch.add_event_attributes(events)
+
+    def test_list_aggregations(self):
+        """Test the Sketch list_aggregations method."""
+        aggregations = self.sketch.list_aggregations()
+        self.assertEqual(len(aggregations), 2)
+        self.assertEqual(aggregations[0].name, "ip barchart")
+        self.assertEqual(
+            aggregations[0].description, "Aggregating values of a particular field"
+        )
+        self.assertEqual(aggregations[1].name, "domain table")
+        self.assertEqual(
+            aggregations[1].description, "Aggregating values of a particular field"
+        )
```

### Comparing `timesketch-api-client-20230208/timesketch_api_client/story.py` & `timesketch-api-client-20230721/timesketch_api_client/story.py`

 * *Files identical despite different names*

### Comparing `timesketch-api-client-20230208/timesketch_api_client/story_test.py` & `timesketch-api-client-20230721/timesketch_api_client/story_test.py`

 * *Files identical despite different names*

### Comparing `timesketch-api-client-20230208/timesketch_api_client/test_lib.py` & `timesketch-api-client-20230721/timesketch_api_client/test_lib.py`

 * *Files 26% similar despite different names*

```diff
@@ -101,14 +101,53 @@
             "error_count": 0,
             "errors": [],
             "events_modified": 2,
         },
         "objects": [],
     }
 
+    add_event_tag_data = {
+        "meta": {},
+        "objects": [
+            [
+                {
+                    "created_at": "2023-03-09T08:52:10.595285",
+                    "name": None,
+                    "updated_at": "2023-03-09T08:52:10.623554",
+                    "user": {
+                        "active": True,
+                        "admin": True,
+                        "groups": [],
+                        "username": "testuser",
+                    },
+                }
+            ]
+        ],
+    }
+
+    add_event_comment_data = {
+        "meta": {},
+        "objects": [
+            [
+                {
+                    "comment": "comment1 foobar",
+                    "created_at": "2023-03-09T13:37:58.395855",
+                    "id": 1,
+                    "updated_at": "2023-03-09T13:37:58.395855",
+                    "user": {
+                        "active": True,
+                        "admin": True,
+                        "groups": [],
+                        "username": "testuser",
+                    },
+                }
+            ]
+        ],
+    }
+
     sketch_data = {
         "meta": {
             "views": [{"id": 1, "name": "test"}, {"id": 2, "name": "test"}],
             "es_time": 41444,
         },
         "objects": [
             {
@@ -312,15 +351,15 @@
     sigma_rule_text_mock = {
         "meta": {"parsed": True},
         "objects": [
             {
                 "title": "Installation of foobar",
                 "id": "bb1e0d1d-cd13-4b65-bf7e-69b4e740266b",
                 "description": "Detects suspicious installation of foobar",
-                "references": ["https://samle.com/foobar"],
+                "references": ["https://sample.com/foobar"],
                 "author": "Alexander Jaeger",
                 "date": "2020/12/10",
                 "modified": "2021/01/01",
                 "logsource": {"product": "linux", "service": "shell"},
                 "detection": {
                     "keywords": ["*apt-get install foobar*"],
                     "condition": "keywords",
@@ -399,15 +438,15 @@
     sigmarule_text = {
         "meta": {"parsed": True},
         "objects": [
             {
                 "title": "Installation of foobar",
                 "id": "bb1e0d1d-cd13-4b65-bf7e-69b4e740266b",
                 "description": "Detects suspicious installation of foobar",
-                "references": ["https://samle.com/foobar"],
+                "references": ["https://sample.com/foobar"],
                 "author": "Alexander Jaeger",
                 "date": "2020/12/10",
                 "modified": "2021/01/01",
                 "logsource": {"product": "linux", "service": "shell"},
                 "detection": {
                     "keywords": ["*apt-get install foobar*"],
                     "condition": "keywords",
@@ -415,25 +454,213 @@
                 "falsepositives": ["Unknown"],
                 "level": "high",
                 "search_query": '(data_type:("shell\\:zsh\\:history" OR "bash\\:history\\:command" OR "apt\\:history\\:line" OR "selinux\\:line") AND "*apt\\-get\\ install\\ foobar*")',  # pylint: disable=line-too-long
             }
         ],
     }
 
+    aggregation_data = {
+        "meta": {},
+        "objects": [
+            [
+                {
+                    "agg_type": "field_bucket",
+                    "aggregationgroup_id": 0,
+                    "chart_type": "barchart",
+                    "created_at": "2023-01-08T08:45:23.113454",
+                    "description": "Aggregating values of a particular field",
+                    "id": 1,
+                    "label_string": "",
+                    "name": "ip barchart",
+                    "parameters": (
+                        '{"supported_charts": "barchart", '
+                        '"field": "ip", "start_time": "", "end_time": "", '
+                        '"limit": "10", "index": [1, 2]}'
+                    ),
+                    "updated_at": "2023-01-08T08:45:23.113454",
+                    "user": {
+                        "active": True,
+                        "admin": False,
+                        "groups": [],
+                        "username": "dev",
+                    },
+                },
+                {
+                    "agg_type": "field_bucket",
+                    "aggregationgroup_id": 0,
+                    "chart_type": "table",
+                    "created_at": "2023-01-08T08:46:24.871292",
+                    "description": "Aggregating values of a particular field",
+                    "id": 2,
+                    "label_string": "",
+                    "name": "domain table",
+                    "parameters": (
+                        '{"supported_charts": "table", "field": "domain", '
+                        '"start_time": "", "end_time": "", "limit": "10", '
+                        '"index": [1, 2]}'
+                    ),
+                    "updated_at": "2023-01-08T08:46:24.871292",
+                    "user": {
+                        "active": True,
+                        "admin": False,
+                        "groups": [],
+                        "username": "dev",
+                    },
+                },
+            ]
+        ],
+    }
+
+    aggregation_1_data = {
+        "meta": {},
+        "objects": [
+            {
+                "agg_type": "field_bucket",
+                "aggregationgroup_id": 0,
+                "chart_type": "barchart",
+                "created_at": "2023-01-08T08:45:23.113454",
+                "description": "Aggregating values of a particular field",
+                "id": 1,
+                "label_string": "",
+                "name": "ip barchart",
+                "parameters": (
+                    '{"supported_charts": "barchart", "field": "ip", '
+                    '"start_time": "", "end_time": "", "limit": "10", '
+                    '"index": [1, 2]}'
+                ),
+                "updated_at": "2023-01-08T08:45:23.113454",
+                "user": {
+                    "active": True,
+                    "admin": False,
+                    "groups": [],
+                    "username": "dev",
+                },
+            }
+        ],
+    }
+
+    aggregation_2_data = {
+        "meta": {},
+        "objects": [
+            {
+                "agg_type": "field_bucket",
+                "aggregationgroup_id": 0,
+                "chart_type": "table",
+                "created_at": "2023-01-08T08:46:24.871292",
+                "description": "Aggregating values of a particular field",
+                "id": 2,
+                "label_string": "",
+                "name": "domain table",
+                "parameters": (
+                    '{"supported_charts": "table", "field": "domain", '
+                    '"start_time": "", "end_time": "", "limit": "10", '
+                    '"index": [1, 2]}'
+                ),
+                "updated_at": "2023-01-08T08:46:24.871292",
+                "user": {
+                    "active": True,
+                    "admin": False,
+                    "groups": [],
+                    "username": "dev",
+                },
+            }
+        ],
+    }
+
+    aggregation_chart_data = {
+        "meta": {
+            "chart_type": "barchart",
+            "description": "Aggregating values of a particular field",
+            "es_time": 0.01930856704711914,
+            "method": "aggregator_run",
+            "name": "field_bucket",
+            "vega_chart_title": "Top results for an unknown field",
+            "vega_spec": {
+                "$schema": "https://vega.github.io/schema/vega-lite/v4.8.1.json",
+                "config": {"view": {"continuousHeight": 300, "continuousWidth": 400}},
+                "data": {"name": "data-4e004a0d2e426361c7096c1d456fe9f0"},
+                "datasets": {
+                    "data-4e004a0d2e426361c7096c1d456fe9f0": [
+                        {"count": 125, "ip": "1.1.1.1"},
+                        {"count": 108, "ip": "1.1.1.2"},
+                        {"count": 97, "ip": "1.1.1.3"},
+                        {"count": 95, "ip": "1.1.1.4"},
+                        {"count": 87, "ip": "1.1.1.5"},
+                        {"count": 84, "ip": "1.1.1.6"},
+                        {"count": 82, "ip": "1.1.1.7"},
+                        {"count": 82, "ip": "1.1.1.8"},
+                        {"count": 51, "ip": "1.1.1.9"},
+                        {"count": 51, "ip": "1.1.1.10"},
+                    ]
+                },
+                "encoding": {
+                    "href": {"field": "url", "type": "nominal"},
+                    "tooltip": [
+                        {"field": "ip", "type": "nominal"},
+                        {"field": "count", "type": "quantitative"},
+                    ],
+                    "x": {
+                        "field": "ip",
+                        "sort": {"field": "count", "op": "sum", "order": "descending"},
+                        "type": "nominal",
+                    },
+                    "y": {"field": "count", "type": "quantitative"},
+                },
+                "mark": {"strokeWidth": 0.3, "type": "bar"},
+                "title": "Top results for an unknown field",
+                "transform": [
+                    {
+                        "as": "url",
+                        "calculate": (
+                            "((('/sketch/1/explore?q=ip:\"' + datum.ip) + "
+                            "'\" ') + '')"
+                        ),
+                    }
+                ],
+            },
+        },
+        "objects": [
+            {
+                "field_bucket": {
+                    "buckets": [
+                        {"count": 125, "ip": "1.1.1.1"},
+                        {"count": 108, "ip": "1.1.1.2"},
+                        {"count": 97, "ip": "1.1.1.3"},
+                        {"count": 95, "ip": "1.1.1.4"},
+                        {"count": 87, "ip": "1.1.1.5"},
+                        {"count": 84, "ip": "1.1.1.6"},
+                        {"count": 82, "ip": "1.1.1.7"},
+                        {"count": 82, "ip": "1.1.1.8"},
+                        {"count": 51, "ip": "1.1.1.9"},
+                        {"count": 51, "ip": "1.1.1.10"},
+                    ]
+                }
+            }
+        ],
+    }
+
+    aggregation_group = {"meta": {"command": "list_groups"}, "objects": []}
+
     # Register API endpoints to the correct mock response data.
     url_router = {
         "http://127.0.0.1": MockResponse(text_data=auth_text_data),
         "http://127.0.0.1/api/v1/sketches/": MockResponse(json_data=sketch_list_data),
         "http://127.0.0.1/api/v1/sketches/1": MockResponse(json_data=sketch_data),
         "http://127.0.0.1/api/v1/sketches/1/event/?searchindex_id=test_index&event_id=test_event": MockResponse(  # pylint: disable=line-too-long
             json_data=event_data_1
         ),
         "http://127.0.0.1/api/v1/sketches/1/event/attributes/": MockResponse(
             json_data=add_event_attribute_data
         ),
+        "http://127.0.0.1/api/v1/sketches/1/event/tagging/": MockResponse(
+            json_data=add_event_tag_data
+        ),
+        "http://127.0.0.1/api/v1/sketches/1/event/annotate/": MockResponse(
+            json_data=add_event_comment_data
+        ),
         "http://127.0.0.1/api/v1/sketches/1/views/1/": MockResponse(
             json_data=view_data_1
         ),
         "http://127.0.0.1/api/v1/sketches/1/views/2/": MockResponse(
             json_data=view_data_2
         ),
         "http://127.0.0.1/api/v1/sketches/1/timelines/1/": MockResponse(
@@ -457,20 +684,35 @@
         "http://127.0.0.1/api/v1/sigma/rule/5266a592-b793-11ea-b3de-0242ac130004": MockResponse(  # pylint: disable=line-too-long
             json_data=sigma_rule
         ),
         "http://127.0.0.1/api/v1/sigma/": MockResponse(json_data=sigma_list),
         "http://127.0.0.1/api/v1/sigma/text/": MockResponse(
             json_data=sigma_rule_text_mock
         ),
-        "http://127.0.0.1/api/v1/sigmarule/5266a592-b793-11ea-b3de-0242ac130004": MockResponse(  # pylint: disable=line-too-long
+        "http://127.0.0.1/api/v1/sigmarules/5266a592-b793-11ea-b3de-0242ac130004": MockResponse(  # pylint: disable=line-too-long
             json_data=sigmarule_individual
         ),
-        "http://127.0.0.1/api/v1/sigmarule/": MockResponse(json_data=sigmarule_list),
-        "http://127.0.0.1/api/v1/sigmarule/text/": MockResponse(
+        "http://127.0.0.1/api/v1/sigmarules/": MockResponse(json_data=sigmarule_list),
+        "http://127.0.0.1/api/v1/sigmarules/text/": MockResponse(
             json_data=sigmarule_text
         ),
+        "http://127.0.0.1/api/v1/sketches/1/aggregation/": MockResponse(
+            json_data=aggregation_data
+        ),
+        "http://127.0.0.1/api/v1/sketches/1/aggregation/1/": MockResponse(
+            json_data=aggregation_1_data
+        ),
+        "http://127.0.0.1/api/v1/sketches/1/aggregation/2/": MockResponse(
+            json_data=aggregation_2_data
+        ),
+        "http://127.0.0.1/api/v1/sketches/1/aggregation/group/": MockResponse(
+            json_data=aggregation_group
+        ),
+        "http://127.0.0.1/api/v1/sketches/1/aggregation/explore/": MockResponse(
+            json_data=aggregation_chart_data
+        ),
     }
 
     if kwargs.get("empty", False):
         return MockResponse(text_data=empty_data)
 
     return url_router.get(args[0], MockResponse(None, 404))
```

### Comparing `timesketch-api-client-20230208/timesketch_api_client/timeline.py` & `timesketch-api-client-20230721/timesketch_api_client/timeline.py`

 * *Files identical despite different names*

### Comparing `timesketch-api-client-20230208/timesketch_api_client/timeline_test.py` & `timesketch-api-client-20230721/timesketch_api_client/timeline_test.py`

 * *Files identical despite different names*

### Comparing `timesketch-api-client-20230208/timesketch_api_client/user.py` & `timesketch-api-client-20230721/timesketch_api_client/user.py`

 * *Files identical despite different names*

### Comparing `timesketch-api-client-20230208/timesketch_api_client/version.py` & `timesketch-api-client-20230721/timesketch_api_client/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Version information for Timesketch API Client."""
 
 
-__version__ = "20230208"
+__version__ = "20230721"
 
 
 def get_version():
     """Returns the version information."""
     return __version__
```

### Comparing `timesketch-api-client-20230208/timesketch_api_client/view.py` & `timesketch-api-client-20230721/timesketch_api_client/view.py`

 * *Files identical despite different names*

### Comparing `timesketch-api-client-20230208/timesketch_api_client/view_test.py` & `timesketch-api-client-20230721/timesketch_api_client/view_test.py`

 * *Files identical despite different names*

### Comparing `timesketch-api-client-20230208/timesketch_api_client.egg-info/PKG-INFO` & `timesketch-api-client-20230721/timesketch_api_client.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: timesketch-api-client
-Version: 20230208
+Version: 20230721
 Summary: Timesketch API client
 Home-page: http://www.timesketch.org/
 Maintainer: Timesketch development team
 Maintainer-email: timesketch-dev@googlegroups.com
 License: Apache License, Version 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 
 The Timesketch API client provides you with a set of Python libraries to connect to your Timesketch (https://github.com/google/timesketch) instance.
 
 The API is feature complete with the Timesketch UI and allows you to do all operations that can be done in the UI, providing ways to integrate Timesketch into other products such as Jupyter/Colab.
 
 To see how it works in action, try the colab notebook that is accessible from here: https://colab.research.google.com/github/google/timesketch/blob/master/notebooks/colab-timesketch-demo.ipynb
-
```

### Comparing `timesketch-api-client-20230208/timesketch_api_client.egg-info/SOURCES.txt` & `timesketch-api-client-20230721/timesketch_api_client.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 setup.py
 timesketch_api_client/__init__.py
 timesketch_api_client/aggregation.py
+timesketch_api_client/aggregation_test.py
 timesketch_api_client/analyzer.py
 timesketch_api_client/cli_input.py
 timesketch_api_client/client.py
 timesketch_api_client/client_test.py
 timesketch_api_client/config.py
 timesketch_api_client/config_test.py
 timesketch_api_client/credentials.py
```

