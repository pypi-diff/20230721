# Comparing `tmp/elasticsearch_curator-8.0.6.post1.tar.gz` & `tmp/elasticsearch_curator-8.0.7.tar.gz`

## Comparing `elasticsearch_curator-8.0.6.post1.tar` & `elasticsearch_curator-8.0.7.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/__init__.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/_version.py
--rw-r--r--   0        0        0     9608 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/classdef.py
--rw-r--r--   0        0        0    15861 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/cli.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/config_utils.py
--rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/curator_cli.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/exceptions.py
--rw-r--r--   0        0        0    60192 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/indexlist.py
--rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/logtools.py
--rw-r--r--   0        0        0    23556 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/repomgrcli.py
--rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/singletons.py
--rw-r--r--   0        0        0    22898 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/snapshotlist.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/actions/__init__.py
--rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/actions/alias.py
--rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/actions/allocation.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/actions/close.py
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/actions/cluster_routing.py
--rw-r--r--   0        0        0     8770 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/actions/cold2frozen.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/actions/create_index.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/actions/delete_indices.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/actions/forcemerge.py
--rw-r--r--   0        0        0     5603 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/actions/index_settings.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/actions/open.py
--rw-r--r--   0        0        0    17631 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/actions/reindex.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/actions/replicas.py
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/actions/rollover.py
--rw-r--r--   0        0        0    24570 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/actions/shrink.py
--rw-r--r--   0        0        0    21632 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/actions/snapshot.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/cli_singletons/__init__.py
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/cli_singletons/alias.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/cli_singletons/allocation.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/cli_singletons/close.py
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/cli_singletons/delete.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/cli_singletons/forcemerge.py
--rw-r--r--   0        0        0     9687 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/cli_singletons/object_class.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/cli_singletons/open_indices.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/cli_singletons/replicas.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/cli_singletons/restore.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/cli_singletons/rollover.py
--rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/cli_singletons/show.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/cli_singletons/shrink.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/cli_singletons/snapshot.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/cli_singletons/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/defaults/__init__.py
--rw-r--r--   0        0        0    11383 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/defaults/filter_elements.py
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/defaults/filtertypes.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/defaults/logging_defaults.py
--rw-r--r--   0        0        0    18383 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/defaults/option_defaults.py
--rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/defaults/settings.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/helpers/__init__.py
--rw-r--r--   0        0        0    23308 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/helpers/date_ops.py
--rw-r--r--   0        0        0    13903 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/helpers/getters.py
--rw-r--r--   0        0        0    15381 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/helpers/testers.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/helpers/utils.py
--rw-r--r--   0        0        0    12701 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/helpers/waiters.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/validators/__init__.py
--rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/validators/actions.py
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/validators/filter_functions.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/validators/logconfig.py
--rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/validators/options.py
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/curator/validators/schemacheck.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/.gitignore
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/LICENSE
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/NOTICE
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/README.rst
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/pyproject.toml
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6.post1/PKG-INFO
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/_version.py
+-rw-r--r--   0        0        0     9608 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/classdef.py
+-rw-r--r--   0        0        0    15861 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/cli.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/config_utils.py
+-rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/curator_cli.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/exceptions.py
+-rw-r--r--   0        0        0    65814 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/indexlist.py
+-rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/logtools.py
+-rw-r--r--   0        0        0    23556 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/repomgrcli.py
+-rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/singletons.py
+-rw-r--r--   0        0        0    22898 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/snapshotlist.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/actions/__init__.py
+-rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/actions/alias.py
+-rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/actions/allocation.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/actions/close.py
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/actions/cluster_routing.py
+-rw-r--r--   0        0        0     8770 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/actions/cold2frozen.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/actions/create_index.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/actions/delete_indices.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/actions/forcemerge.py
+-rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/actions/index_settings.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/actions/open.py
+-rw-r--r--   0        0        0    17631 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/actions/reindex.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/actions/replicas.py
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/actions/rollover.py
+-rw-r--r--   0        0        0    24570 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/actions/shrink.py
+-rw-r--r--   0        0        0    21632 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/actions/snapshot.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/cli_singletons/__init__.py
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/cli_singletons/alias.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/cli_singletons/allocation.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/cli_singletons/close.py
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/cli_singletons/delete.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/cli_singletons/forcemerge.py
+-rw-r--r--   0        0        0     9687 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/cli_singletons/object_class.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/cli_singletons/open_indices.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/cli_singletons/replicas.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/cli_singletons/restore.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/cli_singletons/rollover.py
+-rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/cli_singletons/show.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/cli_singletons/shrink.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/cli_singletons/snapshot.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/cli_singletons/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/defaults/__init__.py
+-rw-r--r--   0        0        0    11383 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/defaults/filter_elements.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/defaults/filtertypes.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/defaults/logging_defaults.py
+-rw-r--r--   0        0        0    18383 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/defaults/option_defaults.py
+-rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/defaults/settings.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/helpers/__init__.py
+-rw-r--r--   0        0        0    23308 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/helpers/date_ops.py
+-rw-r--r--   0        0        0    13903 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/helpers/getters.py
+-rw-r--r--   0        0        0    15381 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/helpers/testers.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/helpers/utils.py
+-rw-r--r--   0        0        0    12701 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/helpers/waiters.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/validators/__init__.py
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/validators/actions.py
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/validators/filter_functions.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/validators/logconfig.py
+-rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/validators/options.py
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/curator/validators/schemacheck.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/.gitignore
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/LICENSE
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/NOTICE
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/README.rst
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.7/PKG-INFO
```

### Comparing `elasticsearch_curator-8.0.6.post1/curator/classdef.py` & `elasticsearch_curator-8.0.7/curator/classdef.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/cli.py` & `elasticsearch_curator-8.0.7/curator/cli.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/config_utils.py` & `elasticsearch_curator-8.0.7/curator/config_utils.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/exceptions.py` & `elasticsearch_curator-8.0.7/curator/exceptions.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/indexlist.py` & `elasticsearch_curator-8.0.7/curator/indexlist.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,34 +68,25 @@
         """
         self.loggit.debug('Getting all indices')
         self.all_indices = get_indices(self.client)
         self.indices = self.all_indices[:]
         if self.indices:
             for index in self.indices:
                 self.__build_index_info(index)
-            self.loggit.debug('FRESH UNPOPULATED: self.index_info = %s', self.index_info)
-            self.get_metadata()
-            self.get_index_stats()
+            # self.get_index_settings()
+            # self.get_index_stats()
 
     def __build_index_info(self, index):
         """
         Ensure that ``index`` is a key in ``index_info``. If not, create a sub-dictionary structure
         under that key.
         """
         self.loggit.debug('Building preliminary index metadata for %s', index)
         if index not in self.index_info:
-            self.index_info[index] = {
-                "age" : {},
-                "number_of_replicas" : 0,
-                "number_of_shards" : 0,
-                "segments" : 0,
-                "size_in_bytes" : 0,
-                "docs" : 0,
-                "state" : "",
-            }
+            self.index_info[index] = self.__zero_values()
 
     def __map_method(self, ftype):
         methods = {
             'alias': self.filter_by_alias,
             'age': self.filter_by_age,
             'allocated': self.filter_allocated,
             'closed': self.filter_closed,
@@ -116,101 +107,70 @@
 
     def __remove_missing(self, err):
         """
         Remove missing index found in ``err`` from self.indices and return that name
         """
         missing = err.info['error']['index']
         self.loggit.warning('Index was initiallly present, but now is not: %s', missing)
-        self.loggit.debug('Removing %s from active IndexList')
+        self.loggit.debug('Removing %s from active IndexList', missing)
         self.indices.remove(missing)
         return missing
 
-    def get_index_stats(self):
-        """
-        Populate ``index_info`` with index ``size_in_bytes``, ``primary_size_in_bytes`` and doc
-        count information for each index.
-        """
-        self.loggit.debug('Getting index stats')
-        self.empty_list_check()
-        # Subroutine to do the dirty work
-        def iterate_over_stats(stats):
-            for index in stats['indices']:
-                size = stats['indices'][index]['total']['store']['size_in_bytes']
-                docs = stats['indices'][index]['total']['docs']['count']
-                primary_size = stats['indices'][index]['primaries']['store']['size_in_bytes']
-                msg = (
-                    f'Index: {index}  Size: {byte_size(size)}  Docs: {docs} '
-                    f'PrimarySize: {byte_size(primary_size)}'
-                )
-                self.loggit.debug(msg)
-                self.index_info[index]['size_in_bytes'] = size
-                self.index_info[index]['docs'] = docs
-                self.index_info[index]['primary_size_in_bytes'] = primary_size
+    def __zero_values(self):
+        """The default values for index metadata"""
+        return {
+            'age' : {'creation_date': 0, 'name': 0},
+            'docs' : 0,
+            'number_of_replicas' : 0,
+            'number_of_shards' : 0,
+            'primary_size_in_bytes': 0,
+            'routing': {},
+            'segments' : 0,
+            'size_in_bytes' : 0,
+            'state' : '',
+        }
 
-        working_list = self.working_list()
-        for index in self.working_list():
-            if self.index_info[index]['state'] == 'close':
-                working_list.remove(index)
-        if working_list:
-            index_lists = chunk_index_list(working_list)
-            for lst in index_lists:
-                stats_result = {}
-                checking = True
-                while checking:
-                    try:
-                        stats_result.update(self._get_indices_stats(lst))
-                    except NotFoundError as err:
-                        lst.remove(self.__remove_missing(err))
-                        continue
-                    except TransportError as err:
-                        if '413' in err.errors:
-                            msg = (
-                                'Huge Payload 413 Err - '
-                                'Trying to get information via multiple requests'
-                            )
-                            self.loggit.debug(msg)
-                            stats_result = {}
-                            try:
-                                stats_result.update(self._bulk_queries(lst, self._get_indices_stats))
-                            except NotFoundError as err2:
-                                lst.remove(self.__remove_missing(err2))
-                                continue
-                    iterate_over_stats(stats_result)
-                    checking = False
+    # def _get_cluster_state(self, data):
+    #     return self.client.cluster.state(
+    #         index=to_csv(data), metric='metadata')['metadata']['indices']
+
+    def _get_indices_segments(self, data):
+        return self.client.indices.segments(index=to_csv(data))['indices'].copy()
+
+    def _get_indices_settings(self, data):
+        return self.client.indices.get_settings(index=to_csv(data))
 
     def _get_indices_stats(self, data):
-        return self.client.indices.stats(index=to_csv(data), metric='store,docs')
+        return self.client.indices.stats(index=to_csv(data), metric='store,docs')['indices']
 
     def _bulk_queries(self, data, exec_func):
         slice_number = 10
         query_result = {}
         loop_number = round(len(data)/slice_number) if round(len(data)/slice_number) > 0 else 1
         self.loggit.debug("Bulk Queries - number requests created: %s", loop_number)
         for num in range(0, loop_number):
             if num == (loop_number-1):
                 data_sliced = data[num*slice_number:]
             else:
                 data_sliced = data[num*slice_number:(num+1)*slice_number]
             query_result.update(exec_func(data_sliced))
         return query_result
 
-    def _get_cluster_state(self, data):
-        return self.client.cluster.state(index=to_csv(data), metric='metadata')['metadata']['indices']
-
     def mitigate_alias(self, index):
         """
         Mitigate when an alias is detected instead of an index name
 
         :param index: The index name that is showing up *instead* of what was expected
 
         :type index: str
 
         :returns: No return value:
         :rtype: None
         """
+        self.loggit.debug('BEGIN mitigate_alias')
         self.loggit.debug('Correcting an instance where an alias name points to index "%s"', index)
         data = self.client.indices.get(index=index)
         aliases = list(data[index]['aliases'])
         if aliases:
             for alias in aliases:
                 if alias in self.indices:
                     self.loggit.warning('Removing alias "%s" from IndexList.indices', alias)
@@ -218,63 +178,230 @@
                 if alias in list(self.index_info):
                     self.loggit.warning('Removing alias "%s" from IndexList.index_info', alias)
                     del self.index_info[alias]
         self.loggit.debug('Adding "%s" to IndexList.indices', index)
         self.indices.append(index)
         self.loggit.debug('Adding preliminary metadata for "%s" to IndexList.index_info', index)
         self.__build_index_info(index)
+        self.loggit.debug('END mitigate_alias')
 
-    def get_metadata(self):
+    def alias_index_check(self, data):
         """
-        Populate ``index_info`` with index ``size_in_bytes`` and doc count information for each
-        index.
+        Check each index in data to see if it's an alias.
         """
-        self.empty_list_check()
-        for lst in chunk_index_list(self.indices):
-            working_list = {}
-            # The API called by _get_cluster_state doesn't suffer from the same problems that
-            # _get_indices_stats does. This won't result in an error if an index is suddenly
-            # missing.
+        # self.loggit.debug('BEGIN alias_index_check')
+        working_list = data[:]
+        for entry in working_list:
+            if self.client.indices.exists_alias(name=entry):
+                index = list(self.client.indices.get_alias(name=entry).keys())[0]
+                self.loggit.warning('"%s" is actually an alias for index "%s"', entry, index)
+                self.mitigate_alias(index)
+                # The mitigate_alias step ensures that the class ivars are handled properly
+                # The following ensure that we pass back a modified list
+                data.remove(entry)
+                data.append(index)
+        # self.loggit.debug('END alias_index_check')
+        return data
+
+    def indices_exist(self, data, exec_func):
+        """Check if indices exist. If one doesn't, remove it. Loop until all exist"""
+        self.loggit.debug('BEGIN indices_exist')
+        checking = True
+        working_list = {}
+        verified_data = self.alias_index_check(data)
+        while checking:
             try:
-                working_list.update(self._get_cluster_state(lst))
+                working_list.update(exec_func(verified_data))
+            except NotFoundError as err:
+                data.remove(self.__remove_missing(err))
+                continue
             except TransportError as err:
                 if '413' in err.errors:
                     msg = 'Huge Payload 413 Err - Trying to get information via multiple requests'
                     self.loggit.debug(msg)
-                    working_list = {}
-                    working_list.update(self._bulk_queries(lst, self._get_cluster_state))
+                    working_list.update(self._bulk_queries(verified_data, exec_func))
+            checking = False
+        # self.loggit.debug('END indices_exist')
+        return working_list
+
+    def data_getter(self, data, exec_func):
+        """
+        Function that prevents unnecessary code repetition for different data getter methods
+        """
+        self.loggit.debug('BEGIN data_getter')
+        checking = True
+        while checking:
+            working_list = self.indices_exist(data, exec_func)
             if working_list:
-                self.loggit.debug('working_list.keys() = %s', working_list.keys())
                 for index in list(working_list.keys()):
-                    self.loggit.debug('index = %s', index)
                     try:
                         sii = self.index_info[index]
                     except KeyError:
-                        # What I believe has happened with this race condition is that during
-                        # __build_index_info initially, an index has a name, but is in process
-                        # of being remounted as a searchable snapshot index, and suddenly the
-                        # original index name is an alias, and the _get_cluster_state call returns
-                        # the new, actual index name instead of the alias it had. This is how a
-                        # KeyError can actually happen in this case. The relevant logs showing
-                        # this behavior are in issue #1682
                         self.loggit.warning(
                             'Index %s was not present at IndexList initialization, and may be '
                             'behind an alias', index
                         )
                         self.mitigate_alias(index)
                         sii = self.index_info[index]
-                    wli = working_list[index]
-                    sii['age']['creation_date'] = (
-                        fix_epoch(wli['settings']['index']['creation_date'])
+                        working_list = {}
+                        try:
+                            working_list.update(self._bulk_queries(data, exec_func))
+                        except NotFoundError as err:
+                            data.remove(self.__remove_missing(err))
+                            continue
+                    yield sii, working_list[index], index
+            checking = False
+        # self.loggit.debug('END data_getter')
+
+    def population_check(self, index, key):
+        """Verify that key is in self.index_info[index], and that it is populated"""
+        retval = True
+        # self.loggit.debug('BEGIN population_check')
+        # self.loggit.debug('population_check: %s, %s', index, key)
+        if not index in self.index_info:
+            # This is just in case the index was somehow not populated
+            self.__build_index_info(index)
+        if not key in self.index_info[index]:
+            self.index_info[index][key] = self.__zero_values()[key]
+        if self.index_info[index][key] == self.__zero_values()[key]:
+            retval = False
+        # self.loggit.debug('END population_check')
+        return retval
+
+    def needs_data(self, indices, fields):
+        """Check for data population in self.index_info"""
+        self.loggit.debug('Indices: %s, Fields: %s', indices, fields)
+        needful = []
+        working_list = self.indices_exist(indices, self._get_indices_settings)
+        for idx in working_list:
+            count = 0
+            for field in fields:
+                # If the return value is True for this field, it means it's populated
+                if self.population_check(idx, field):
+                    count += 1
+            if count == 0:
+                # All values are the default/zero
+                needful.append(idx)
+        if fields == ['state']:
+            self.loggit.debug('Always check open/close for all passed indices')
+            needful = list(working_list.keys())
+        self.loggit.debug('These indices need data in index_info: %s', needful)
+        return needful
+
+    def get_index_settings(self):
+        """
+        For each index in self.indices, populate ``index_info`` with:
+            creation_date
+            number_of_replicas
+            number_of_shards
+            routing information (if present)
+        """
+        self.loggit.debug('Getting index settings -- BEGIN')
+        self.empty_list_check()
+        fields = ['age', 'number_of_replicas', 'number_of_shards', 'routing']
+        for lst in chunk_index_list(self.indices):
+            # This portion here is to ensure that we're not polling for data unless we must
+            needful = self.needs_data(lst, fields)
+            if not needful:
+                # All indices are populated with some data, so we can skip data collection
+                continue
+            # Now we only need to run on the 'needful'
+            for sii, wli, _ in self.data_getter(needful, self._get_indices_settings):
+                sii['age']['creation_date'] = (
+                    fix_epoch(wli['settings']['index']['creation_date'])
+                )
+                sii['number_of_replicas'] = wli['settings']['index']['number_of_replicas']
+                sii['number_of_shards'] = wli['settings']['index']['number_of_shards']
+                if 'routing' in wli['settings']['index']:
+                    sii['routing'] = wli['settings']['index']['routing']
+        self.loggit.debug('Getting index settings -- END')
+
+    def get_index_state(self):
+        """
+        For each index in self.indices, populate ``index_info`` with:
+            state (open or closed)
+        from the cat API
+        """
+        self.loggit.debug('Getting index state -- BEGIN')
+        self.empty_list_check()
+        fields = ['state']
+        for lst in chunk_index_list(self.indices):
+            # This portion here is to ensure that we're not polling for data unless we must
+            needful = self.needs_data(lst, fields)
+            # Checking state is _always_ needful.
+            resp = self.client.cat.indices(index=to_csv(needful), format='json', h='index,status')
+            for entry in resp:
+                try:
+                    self.index_info[entry['index']]['state'] = entry['status']
+                except KeyError:
+                    self.loggit.warning(
+                        'Index %s was not present at IndexList initialization, and may be '
+                        'behind an alias', entry['index']
                     )
-                    sii['number_of_replicas'] = wli['settings']['index']['number_of_replicas']
-                    sii['number_of_shards'] = wli['settings']['index']['number_of_shards']
-                    sii['state'] = wli['state']
-                    if 'routing' in wli['settings']['index']:
-                        sii['routing'] = wli['settings']['index']['routing']
+                    self.mitigate_alias(entry['index'])
+                    self.index_info[entry['index']]['state'] = entry['status']
+        # self.loggit.debug('Getting index state -- END')
+
+    def get_index_stats(self):
+        """
+        Populate ``index_info`` with index ``size_in_bytes``, ``primary_size_in_bytes`` and doc
+        count information for each index.
+        """
+        self.loggit.debug('Getting index stats -- BEGIN')
+        self.empty_list_check()
+        fields = ['size_in_bytes', 'docs', 'primary_size_in_bytes']
+        # This ensures that the index state is populated
+        self.get_index_state()
+        # Don't populate working_list until after the get_index state as it
+        # can and will remove missing indices
+        working_list = self.working_list()
+        for index in self.working_list():
+            if self.index_info[index]['state'] == 'close':
+                working_list.remove(index)
+        if working_list:
+            index_lists = chunk_index_list(working_list)
+            for lst in index_lists:
+                # This portion here is to ensure that we're not polling for data unless we must
+                needful = self.needs_data(lst, fields)
+                if not needful:
+                    # All indices are populated with some data, so we can skip data collection
+                    continue
+                # Now we only need to run on the 'needful'
+                for sii, wli, index in self.data_getter(needful, self._get_indices_stats):
+                    try:
+                        size = wli['total']['store']['size_in_bytes']
+                        docs = wli['total']['docs']['count']
+                        primary_size = wli['primaries']['store']['size_in_bytes']
+                        msg = (
+                            f'Index: {index}  Size: {byte_size(size)}  Docs: {docs} '
+                            f'PrimarySize: {byte_size(primary_size)}'
+                        )
+                        self.loggit.debug(msg)
+                        sii['size_in_bytes'] = size
+                        sii['docs'] = docs
+                        sii['primary_size_in_bytes'] = primary_size
+                    except KeyError:
+                        msg = f'Index stats missing for "{index}" -- might be closed'
+                        self.loggit.warning(msg)
+        # self.loggit.debug('Getting index stats -- END')
+
+    def get_segment_counts(self):
+        """
+        Populate ``index_info`` with segment information for each index.
+        """
+        self.loggit.debug('Getting index segment counts')
+        self.empty_list_check()
+        for lst in chunk_index_list(self.indices):
+            for sii, wli, _ in self.data_getter(lst, self._get_indices_segments):
+                shards = wli['shards']
+                segmentcount = 0
+                for shardnum in shards:
+                    for shard in range(0, len(shards[shardnum])):
+                        segmentcount += shards[shardnum][shard]['num_search_segments']
+                sii['segments'] = segmentcount
 
     def empty_list_check(self):
         """Raise :py:exc:`~.curator.exceptions.NoIndices` if ``indices`` is empty"""
         self.loggit.debug('Checking for empty list')
         if not self.indices:
             raise NoIndices('index_list object is empty.')
 
@@ -284,41 +411,14 @@
         stomping during iterations
         """
         # Copy by value, rather than reference to prevent list stomping during
         # iterations
         self.loggit.debug('Generating working list of indices')
         return self.indices[:]
 
-    def _get_indices_segments(self, data):
-        return self.client.indices.segments(index=to_csv(data))['indices'].copy()
-
-    def _get_segment_counts(self):
-        """
-        Populate ``index_info`` with segment information for each index.
-        """
-        self.loggit.debug('Getting index segment counts')
-        self.empty_list_check()
-        for lst in chunk_index_list(self.indices):
-            working_list = {}
-            try:
-                working_list.update(self._get_indices_segments(lst))
-            except TransportError as err:
-                if '413' in err.errors:
-                    self.loggit.debug('Huge Payload 413 Error - Trying to get information with multiple requests')
-                    working_list = {}
-                    working_list.update(self._bulk_queries(lst, self._get_indices_segments))
-            if working_list:
-                for index in list(working_list.keys()):
-                    shards = working_list[index]['shards']
-                    segmentcount = 0
-                    for shardnum in shards:
-                        for shard in range(0,len(shards[shardnum])):
-                            segmentcount += (shards[shardnum][shard]['num_search_segments'])
-                    self.index_info[index]['segments'] = segmentcount
-
     def _get_name_based_ages(self, timestring):
         """
         Add indices to ``index_info`` based on the age as indicated by the index
         name pattern, if it matches ``timestring``
 
         :param timestring: An :py:func:`time.strftime` pattern
         """
@@ -327,14 +427,15 @@
         self.empty_list_check()
         tstr = TimestringSearch(timestring)
         for index in self.working_list():
             epoch = tstr.get_epoch(index)
             if isinstance(epoch, int):
                 self.index_info[index]['age']['name'] = epoch
 
+
     def _get_field_stats_dates(self, field='@timestamp'):
         """
         Add indices to ``index_info`` based on the values the queries return, as determined by the
         min and max aggregated values of ``field``
 
         :param field: The field with the date value.  The field must be mapped in elasticsearch as
             a date datatype. Default: ``@timestamp``
@@ -382,15 +483,15 @@
         """
         self.age_keyfield = source
         if source == 'name':
             if not timestring:
                 raise MissingArgument('source "name" requires the "timestring" keyword argument')
             self._get_name_based_ages(timestring)
         elif source == 'creation_date':
-            # Nothing to do here as this comes from `get_metadata` in __init__
+            # Nothing to do here as this comes from `get_settings` in __init__
             pass
         elif source == 'field_stats':
             if not field:
                 raise MissingArgument('source "field_stats" requires the "field" keyword argument')
             if stats_result not in ['min_value', 'max_value']:
                 raise ValueError(f'Invalid value for "stats_result": {stats_result}')
             self.age_keyfield = stats_result
@@ -407,26 +508,33 @@
         By default, the youngest are first with ``reverse=True``, but the oldest can be first by
         setting ``reverse=False``
         """
         # Do the age-based sorting here.
         # Build an temporary dictionary with just index and age as the key and value, respectively
         temp = {}
         for index in index_list:
-            if self.age_keyfield in self.index_info[index]['age']:
-                temp[index] = self.index_info[index]['age'][self.age_keyfield]
-            else:
-                msg = (f'{index} does not have key "{self.age_keyfield}" in IndexList metadata')
+            try:
+                if self.index_info[index]['age'][self.age_keyfield]:
+                    temp[index] = self.index_info[index]['age'][self.age_keyfield]
+                else:
+                    msg = (
+                        f'No date for "{index}" in IndexList metadata. '
+                        f'Possible timestring mismatch. Excluding index "{index}".'
+                    )
+                    self.__excludify(True, True, index, msg)
+            except KeyError:
+                msg = f'{index} does not have key "{self.age_keyfield}" in IndexList metadata'
                 self.__excludify(True, True, index, msg)
         # Sort alphabetically prior to age sort to keep sorting consistent
-        temp_tuple = (sorted(temp.items(), key=lambda k: k[0], reverse=reverse))
+        temp_tuple = sorted(temp.items(), key=lambda k: k[0], reverse=reverse)
         # If reverse is True, this will sort so the youngest indices are first.
         # However, if you want oldest first, set reverse to False.
         # Effectively, this should set us up to act on everything older than
         # meets the other set criteria. It starts as a tuple, but then becomes a list.
-        sorted_tuple = (sorted(temp_tuple, key=lambda k: k[1], reverse=reverse))
+        sorted_tuple = sorted(temp_tuple, key=lambda k: k[1], reverse=reverse)
         return [x[0] for x in sorted_tuple]
 
     def filter_by_regex(self, kind=None, value=None, exclude=False):
         """
         Match indices by regular expression (pattern).
 
         :param kind: Can be one of: ``suffix``, ``prefix``, ``regex``, or ``timestring``. This
@@ -485,74 +593,76 @@
             establish a point of reference for calculations. If not provided, the current time will
             be used.
         :param exclude: If ``exclude=True``, this filter will remove matching indices from
             ``indices``. If ``exclude`` is `False`, then only matching indices will be kept in
             ``indices``. Default is ``False``
         """
         self.loggit.debug('Filtering indices by age')
-        # Get timestamp point of reference, PoR
-        PoR = get_point_of_reference(unit, unit_count, epoch)
+        # Get timestamp point of reference, por
+        por = get_point_of_reference(unit, unit_count, epoch)
         if not direction:
             raise MissingArgument('Must provide a value for "direction"')
         if direction not in ['older', 'younger']:
             raise ValueError(f'Invalid value for "direction": {direction}')
+        # This filter requires index settings.
+        self.get_index_settings()
         self._calculate_ages(
             source=source, timestring=timestring, field=field, stats_result=stats_result)
         if unit_count_pattern:
             try:
                 unit_count_matcher = re.compile(unit_count_pattern)
             # pylint: disable=broad-except
             except Exception as exc:
                 # We got an illegal regex, so won't be able to match anything
                 self.loggit.error(
                     'Regular expression failure. Will not match unit count. Error: %s', exc)
                 unit_count_matcher = None
         for index in self.working_list():
             try:
-                removeThisIndex = False
+                remove_this_index = False
                 age = int(self.index_info[index]['age'][self.age_keyfield])
                 msg = (
                     f'Index "{index}" age ({age}), direction: "{direction}", point of '
-                    f'reference, ({PoR})'
+                    f'reference, ({por})'
                 )
                 # Because time adds to epoch, smaller numbers are actually older
                 # timestamps.
                 if unit_count_pattern:
                     self.loggit.debug('Unit_count_pattern is set, trying to match pattern to index "%s"', index)
                     unit_count_from_index = get_unit_count_from_name(index, unit_count_matcher)
                     if unit_count_from_index:
                         self.loggit.debug('Pattern matched, applying unit_count of  "%s"', unit_count_from_index)
-                        adjustedPoR = get_point_of_reference(unit, unit_count_from_index, epoch)
+                        adjustedpor = get_point_of_reference(unit, unit_count_from_index, epoch)
                         msg = (
-                            f'Adjusting point of reference from {PoR} to {adjustedPoR} '
+                            f'Adjusting point of reference from {por} to {adjustedpor} '
                             f'based on unit_count of {unit_count_from_index} from index name'
                         )
                         self.loggit.debug(msg)
                     elif unit_count == -1:
                         # Unable to match pattern and unit_count is -1, meaning no fallback, so this
                         # index is removed from the list
                         msg = (
                             f'Unable to match pattern and no fallback value set. '
                             f'Removing index "{index}" from actionable list'
                         )
                         self.loggit.debug(msg)
-                        removeThisIndex = True
-                        adjustedPoR = PoR # necessary to avoid exception if the first index is excluded
+                        remove_this_index = True
+                        adjustedpor = por # necessary to avoid exception if the first index is excluded
                     else:
                         # Unable to match the pattern and unit_count is set, so fall back to using unit_count
                         # for determining whether to keep this index in the list
                         self.loggit.debug('Unable to match pattern using fallback value of "%s"', unit_count)
-                        adjustedPoR = PoR
+                        adjustedpor = por
                 else:
-                    adjustedPoR = PoR
+                    adjustedpor = por
                 if direction == 'older':
-                    agetest = age < adjustedPoR
+                    agetest = age < adjustedpor
                 else:
-                    agetest = age > adjustedPoR
-                self.__excludify(agetest and not removeThisIndex, exclude, index, msg)
+                    agetest = age > adjustedpor
+                self.__excludify(agetest and not remove_this_index, exclude, index, msg)
             except KeyError:
                 msg = (
                     f'Index "{index}" does not meet provided criteria. '
                     f'Removing from list.'
                 )
                 self.loggit.debug(msg)
                 self.indices.remove(index)
@@ -601,26 +711,30 @@
         """
         self.loggit.debug('Filtering indices by disk space')
         # Ensure that disk_space is a float
         if not disk_space:
             raise MissingArgument('No value for "disk_space" provided')
         if threshold_behavior not in ['greater_than', 'less_than']:
             raise ValueError(f'Invalid value for "threshold_behavior": {threshold_behavior}')
+        # This filter requires both index stats and index settings
+        self.get_index_stats()
+        self.get_index_settings()
         disk_space = float(disk_space)
         disk_usage = 0.0
         disk_limit = disk_space * 2**30
         self.loggit.debug(
             'Cannot get disk usage info from closed indices. Omitting any closed indices.')
         self.filter_closed()
         # Create a copy-by-value working list
         working_list = self.working_list()
         if use_age:
             self._calculate_ages(
                 source=source, timestring=timestring, field=field, stats_result=stats_result)
             # Using default value of reverse=True in self._sort_by_age()
+            self.loggit.debug('SORTING BY AGE')
             sorted_indices = self._sort_by_age(working_list)
         else:
             # Default to sorting by index name
             sorted_indices = sorted(working_list, reverse=reverse)
         for index in sorted_indices:
             disk_usage += self.index_info[index]['size_in_bytes']
             msg = (
@@ -660,16 +774,19 @@
             ``indices``. Default is ``True``
         """
         self.loggit.debug('Filtering forceMerged indices')
         if not max_num_segments:
             raise MissingArgument('Missing value for "max_num_segments"')
         self.loggit.debug(
             'Cannot get segment count of closed indices. Omitting any closed indices.')
+        # This filter requires the index state (open/close), and index settings.
+        self.get_index_state()
+        self.get_index_settings()
         self.filter_closed()
-        self._get_segment_counts()
+        self.get_segment_counts()
         for index in self.working_list():
             # Do this to reduce long lines and make it more readable...
             shards = int(self.index_info[index]['number_of_shards'])
             replicas = int(self.index_info[index]['number_of_replicas'])
             segments = int(self.index_info[index]['segments'])
             msg = (
                 f'{index} has {shards} shard(s) + {replicas} replica(s) '
@@ -683,14 +800,16 @@
         Filter out closed indices from ``indices``
 
         :param exclude: If ``exclude=True``, this filter will remove matching indices from
             ``indices``. If ``exclude=False``, then only matching indices will be kept in
             ``indices``. Default is ``True``
         """
         self.loggit.debug('Filtering closed indices')
+        # This filter requires index state (open/close)
+        self.get_index_state()
         self.empty_list_check()
         for index in self.working_list():
             condition = self.index_info[index]['state'] == 'close'
             self.loggit.debug('Index %s state: %s', index, self.index_info[index]['state'])
             self.__excludify(condition, exclude, index)
 
     def filter_empty(self, exclude=True):
@@ -699,14 +818,17 @@
         excluded from consideration due to closed indices reporting a document count of zero.
 
         :param exclude: If ``exclude=True``, this filter will remove matching indices from
             ``indices``. If ``exclude=False``, then only matching indices will be kept in
             ``indices``. Default is ``True``
         """
         self.loggit.debug('Filtering empty indices')
+        # This index requires index state (open/close) and index stats
+        self.get_index_state()
+        self.get_index_stats()
         self.filter_closed()
         self.empty_list_check()
         for index in self.working_list():
             condition = self.index_info[index]['docs'] == 0
             self.loggit.debug('Index %s doc count: %s', index, self.index_info[index]['docs'])
             self.__excludify(condition, exclude, index)
 
@@ -715,14 +837,16 @@
         Filter out opened indices from ``indices``
 
         :param exclude: If ``exclude=True``, this filter will remove matching indices from
             ``indices``. If ``exclude=False``, then only matching indices will be kept in
             ``indices``. Default is ``True``
         """
         self.loggit.debug('Filtering open indices')
+        # This filter requires index state (open/close)
+        self.get_index_state()
         self.empty_list_check()
         for index in self.working_list():
             condition = self.index_info[index]['state'] == 'open'
             self.loggit.debug('Index %s state: %s', index, self.index_info[index]['state'])
             self.__excludify(condition, exclude, index)
 
     def filter_allocated(self, key=None, value=None, allocation_type='require', exclude=True):
@@ -739,17 +863,20 @@
         self.loggit.debug('Filtering indices with shard routing allocation rules')
         if not key:
             raise MissingArgument('No value for "key" provided')
         if not value:
             raise MissingArgument('No value for "value" provided')
         if allocation_type not in ['include', 'exclude', 'require']:
             raise ValueError(f'Invalid "allocation_type": {allocation_type}')
+        # This filter requires index settings
+        self.get_index_settings()
+        self.get_index_state()
         self.empty_list_check()
         for lst in chunk_index_list(self.indices):
-            working_list = self.client.indices.get_settings(index=to_csv(lst))
+            working_list = self._get_indices_settings(lst)
             if working_list:
                 for index in list(working_list.keys()):
                     try:
                         has_routing = (
                             working_list[index]['settings']['index']['routing']['allocation'][allocation_type][key] == value
                         )
                     except KeyError:
@@ -844,14 +971,17 @@
         :param exclude: If ``exclude=True``, this filter will remove matching indices from
             ``indices``. If ``exclude=False``, then only matching indices will be kept in
             ``indices``. Default is ``True``
         """
         self.loggit.debug('Filtering indices by count')
         if not count:
             raise MissingArgument('No value for "count" provided')
+        # This filter requires index state (open/close) and index settings
+        self.get_index_state()
+        self.get_index_settings()
         # Create a copy-by-value working list
         working_list = self.working_list()
         if pattern:
             try:
                 regex = re.compile(pattern)
                 if regex.groups < 1:
                     raise ConfigurationError(f'No regular expression group found in {pattern}')
@@ -927,14 +1057,16 @@
         if shard_filter_behavior not in ['greater_than', 'less_than', 'greater_than_or_equal', 'less_than_or_equal', 'equal']:
             raise ValueError(f'Invalid value for "shard_filter_behavior": {shard_filter_behavior}')
         if number_of_shards < 1 or (shard_filter_behavior == 'less_than' and number_of_shards == 1):
             raise ValueError(
                 f'Unacceptable value: {number_of_shards} -- "number_of_shards" cannot be less '
                 f'than 1. A valid index will have at least one shard.'
             )
+        # This filter requires index_settings to count shards
+        self.get_index_settings()
         self.empty_list_check()
         for index in self.working_list():
             self.loggit.debug('Filter by number of shards: Index: %s', index)
             if shard_filter_behavior == 'greater_than':
                 condition = int(self.index_info[index]['number_of_shards']) > number_of_shards
             elif shard_filter_behavior == 'less_than':
                 condition = int(self.index_info[index]['number_of_shards']) < number_of_shards
@@ -1001,14 +1133,16 @@
             kwgs = { 'date_from_format': date_from_format, 'date_to_format': date_to_format }
             for reqd in [date_from, date_to, date_from_format, date_to_format]:
                 if not reqd:
                     raise ConfigurationError(
                         'Must provide "date_from", "date_to", "date_from_format", and '
                         '"date_to_format" with absolute period_type'
                     )
+        # This filter requires index settings 
+        self.get_index_settings()
         try:
             start, end = func(*args, **kwgs)
         # pylint: disable=broad-except
         except Exception as exc:
             report_failure(exc)
         self._calculate_ages(
             source=source, timestring=timestring, field=field, stats_result=stats_result)
@@ -1050,15 +1184,15 @@
         """
         self.loggit.debug('Filtering indices with index.lifecycle.name')
         index_lists = chunk_index_list(self.indices)
         if index_lists == [['']]:
             self.loggit.debug('Empty working list. No ILM indices to filter.')
             return
         for lst in index_lists:
-            working_list = self.client.indices.get_settings(index=to_csv(lst))
+            working_list = self._get_indices_settings(lst)
             if working_list:
                 for index in list(working_list.keys()):
                     try:
                         subvalue = working_list[index]['settings']['index']['lifecycle']
                         has_ilm = 'name' in subvalue
                         msg = f"{index} has index.lifecycle.name {subvalue['name']}"
                     except KeyError:
@@ -1139,14 +1273,17 @@
         if size_behavior not in ['primary', 'total']:
             raise ValueError(f'Invalid value for "size_behavior": {size_behavior}')
         if threshold_behavior not in ['greater_than', 'less_than']:
             raise ValueError(f'Invalid value for "threshold_behavior": {threshold_behavior}')
         index_size_limit = float(size_threshold) * 2**30
         self.loggit.debug(
             'Cannot get disk usage info from closed indices. Omitting any closed indices.')
+        # This filter requires index state (open/close) and index stats
+        self.get_index_state()
+        self.get_index_stats()
         self.filter_closed()
         # Create a copy-by-value working list
         working_list = self.working_list()
         for index in working_list:
             if size_behavior == 'primary':
                 index_size = self.index_info[index]['primary_size_in_bytes']
             else:
```

### Comparing `elasticsearch_curator-8.0.6.post1/curator/logtools.py` & `elasticsearch_curator-8.0.7/curator/logtools.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/repomgrcli.py` & `elasticsearch_curator-8.0.7/curator/repomgrcli.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/singletons.py` & `elasticsearch_curator-8.0.7/curator/singletons.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/snapshotlist.py` & `elasticsearch_curator-8.0.7/curator/snapshotlist.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/actions/__init__.py` & `elasticsearch_curator-8.0.7/curator/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/actions/alias.py` & `elasticsearch_curator-8.0.7/curator/actions/alias.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/actions/allocation.py` & `elasticsearch_curator-8.0.7/curator/actions/allocation.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/actions/close.py` & `elasticsearch_curator-8.0.7/curator/actions/close.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/actions/cluster_routing.py` & `elasticsearch_curator-8.0.7/curator/actions/cluster_routing.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/actions/cold2frozen.py` & `elasticsearch_curator-8.0.7/curator/actions/cold2frozen.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/actions/create_index.py` & `elasticsearch_curator-8.0.7/curator/actions/create_index.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/actions/delete_indices.py` & `elasticsearch_curator-8.0.7/curator/actions/delete_indices.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/actions/forcemerge.py` & `elasticsearch_curator-8.0.7/curator/actions/forcemerge.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/actions/index_settings.py` & `elasticsearch_curator-8.0.7/curator/actions/index_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,14 +73,18 @@
             'translog',
         ]
 
     def _settings_check(self):
         # Detect if even one index is open.  Save all found to open_index_list.
         open_index_list = []
         open_indices = False
+        # This action requires index settings and state to be present
+        # Calling these here should not cause undue problems, even if it's a repeat call
+        self.index_list.get_index_state()
+        self.index_list.get_index_settings()
         for idx in self.index_list.indices:
             if self.index_list.index_info[idx]['state'] == 'open':
                 open_index_list.append(idx)
                 open_indices = True
         for k in self.body['index']:
             if k in self._static_settings():
                 if not self.ignore_unavailable:
```

### Comparing `elasticsearch_curator-8.0.6.post1/curator/actions/open.py` & `elasticsearch_curator-8.0.7/curator/actions/open.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/actions/reindex.py` & `elasticsearch_curator-8.0.7/curator/actions/reindex.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/actions/replicas.py` & `elasticsearch_curator-8.0.7/curator/actions/replicas.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/actions/rollover.py` & `elasticsearch_curator-8.0.7/curator/actions/rollover.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/actions/shrink.py` & `elasticsearch_curator-8.0.7/curator/actions/shrink.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/actions/snapshot.py` & `elasticsearch_curator-8.0.7/curator/actions/snapshot.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/cli_singletons/__init__.py` & `elasticsearch_curator-8.0.7/curator/cli_singletons/__init__.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/cli_singletons/alias.py` & `elasticsearch_curator-8.0.7/curator/cli_singletons/alias.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/cli_singletons/allocation.py` & `elasticsearch_curator-8.0.7/curator/cli_singletons/allocation.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/cli_singletons/close.py` & `elasticsearch_curator-8.0.7/curator/cli_singletons/close.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/cli_singletons/delete.py` & `elasticsearch_curator-8.0.7/curator/cli_singletons/delete.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/cli_singletons/forcemerge.py` & `elasticsearch_curator-8.0.7/curator/cli_singletons/forcemerge.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/cli_singletons/object_class.py` & `elasticsearch_curator-8.0.7/curator/cli_singletons/object_class.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/cli_singletons/open_indices.py` & `elasticsearch_curator-8.0.7/curator/cli_singletons/open_indices.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/cli_singletons/replicas.py` & `elasticsearch_curator-8.0.7/curator/cli_singletons/replicas.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/cli_singletons/restore.py` & `elasticsearch_curator-8.0.7/curator/cli_singletons/restore.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/cli_singletons/rollover.py` & `elasticsearch_curator-8.0.7/curator/cli_singletons/rollover.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/cli_singletons/show.py` & `elasticsearch_curator-8.0.7/curator/cli_singletons/show.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/cli_singletons/shrink.py` & `elasticsearch_curator-8.0.7/curator/cli_singletons/shrink.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/cli_singletons/snapshot.py` & `elasticsearch_curator-8.0.7/curator/cli_singletons/snapshot.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/cli_singletons/utils.py` & `elasticsearch_curator-8.0.7/curator/cli_singletons/utils.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/defaults/filter_elements.py` & `elasticsearch_curator-8.0.7/curator/defaults/filter_elements.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/defaults/filtertypes.py` & `elasticsearch_curator-8.0.7/curator/defaults/filtertypes.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/defaults/logging_defaults.py` & `elasticsearch_curator-8.0.7/curator/defaults/logging_defaults.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/defaults/option_defaults.py` & `elasticsearch_curator-8.0.7/curator/defaults/option_defaults.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/defaults/settings.py` & `elasticsearch_curator-8.0.7/curator/defaults/settings.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/helpers/date_ops.py` & `elasticsearch_curator-8.0.7/curator/helpers/date_ops.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/helpers/getters.py` & `elasticsearch_curator-8.0.7/curator/helpers/getters.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/helpers/testers.py` & `elasticsearch_curator-8.0.7/curator/helpers/testers.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/helpers/utils.py` & `elasticsearch_curator-8.0.7/curator/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/helpers/waiters.py` & `elasticsearch_curator-8.0.7/curator/helpers/waiters.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/validators/actions.py` & `elasticsearch_curator-8.0.7/curator/validators/actions.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/validators/filter_functions.py` & `elasticsearch_curator-8.0.7/curator/validators/filter_functions.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/validators/options.py` & `elasticsearch_curator-8.0.7/curator/validators/options.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/curator/validators/schemacheck.py` & `elasticsearch_curator-8.0.7/curator/validators/schemacheck.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/LICENSE` & `elasticsearch_curator-8.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/NOTICE` & `elasticsearch_curator-8.0.7/NOTICE`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/README.rst` & `elasticsearch_curator-8.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/pyproject.toml` & `elasticsearch_curator-8.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.6.post1/PKG-INFO` & `elasticsearch_curator-8.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elasticsearch-curator
-Version: 8.0.6.post1
+Version: 8.0.7
 Summary: Tending your Elasticsearch indices and snapshots
 Project-URL: Homepage, https://github.com/elastic/curator
 Project-URL: Bug Tracker, https://github.com/elastic/curator/issues
 Author-email: Elastic <info@elastic.co>
 License: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
```

