# Comparing `tmp/graphreduce-0.8.tar.gz` & `tmp/graphreduce-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphreduce-0.8.tar", last modified: Fri Jun 30 13:50:24 2023, max compression
+gzip compressed data, was "graphreduce-0.9.tar", last modified: Fri Jul 21 14:22:40 2023, max compression
```

## Comparing `graphreduce-0.8.tar` & `graphreduce-0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-30 13:50:24.965625 graphreduce-0.8/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-06-30 13:50:24.965490 graphreduce-0.8/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     6951 2023-06-29 22:54:27.000000 graphreduce-0.8/README.md
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-30 13:50:24.964439 graphreduce-0.8/graphreduce/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-0.8/graphreduce/__init__.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-06-29 23:42:51.000000 graphreduce-0.8/graphreduce/enum.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    16056 2023-06-30 01:37:39.000000 graphreduce-0.8/graphreduce/graph_reduce.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    13315 2023-06-30 13:49:45.000000 graphreduce-0.8/graphreduce/node.py
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-30 13:50:24.965316 graphreduce-0.8/graphreduce.egg-info/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-06-30 13:50:24.000000 graphreduce-0.8/graphreduce.egg-info/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      318 2023-06-30 13:50:24.000000 graphreduce-0.8/graphreduce.egg-info/SOURCES.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-30 13:50:24.000000 graphreduce-0.8/graphreduce.egg-info/dependency_links.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-0.8/graphreduce.egg-info/not-zip-safe
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      134 2023-06-30 13:50:24.000000 graphreduce-0.8/graphreduce.egg-info/requires.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-06-30 13:50:24.000000 graphreduce-0.8/graphreduce.egg-info/top_level.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-06-30 13:50:24.965663 graphreduce-0.8/setup.cfg
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     1830 2023-06-30 13:49:59.000000 graphreduce-0.8/setup.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-21 14:22:40.007228 graphreduce-0.9/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-07-21 14:22:40.007107 graphreduce-0.9/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     6951 2023-06-29 22:54:27.000000 graphreduce-0.9/README.md
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-21 14:22:40.006066 graphreduce-0.9/graphreduce/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-0.9/graphreduce/__init__.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-06-29 23:42:51.000000 graphreduce-0.9/graphreduce/enum.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    16056 2023-07-18 22:09:36.000000 graphreduce-0.9/graphreduce/graph_reduce.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    14340 2023-07-21 12:37:58.000000 graphreduce-0.9/graphreduce/node.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-21 14:22:40.006952 graphreduce-0.9/graphreduce.egg-info/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-07-21 14:22:39.000000 graphreduce-0.9/graphreduce.egg-info/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      318 2023-07-21 14:22:39.000000 graphreduce-0.9/graphreduce.egg-info/SOURCES.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-07-21 14:22:39.000000 graphreduce-0.9/graphreduce.egg-info/dependency_links.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-0.9/graphreduce.egg-info/not-zip-safe
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      134 2023-07-21 14:22:39.000000 graphreduce-0.9/graphreduce.egg-info/requires.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-07-21 14:22:39.000000 graphreduce-0.9/graphreduce.egg-info/top_level.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-07-21 14:22:40.007264 graphreduce-0.9/setup.cfg
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     1830 2023-07-21 14:22:36.000000 graphreduce-0.9/setup.py
```

### Comparing `graphreduce-0.8/PKG-INFO` & `graphreduce-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 0.8
+Version: 0.9
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-0.8/README.md` & `graphreduce-0.9/README.md`

 * *Files identical despite different names*

### Comparing `graphreduce-0.8/graphreduce/graph_reduce.py` & `graphreduce-0.9/graphreduce/graph_reduce.py`

 * *Files identical despite different names*

### Comparing `graphreduce-0.8/graphreduce/node.py` & `graphreduce-0.9/graphreduce/node.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         self.reduce = reduce
         self.has_labels = has_labels
         self.label_period_val = label_period_val
         self.label_period_unit = label_period_unit
         self.feature_function = feature_function
         self.spark_sqlctx = spark_sqlctx
 
-        self.columns = []
+        self.columns = columns
         
 
     
     def do_data (
         self
     ) -> typing.Union[
         pd.DataFrame,
@@ -119,14 +119,28 @@
             if not hasattr(self, 'df') or (hasattr(self, 'df') and not isinstance(self.df, pyspark.sql.DataFrame)):
                 self.df = getattr(self.spark_sqlctx.read, f"{self.fmt}")(self.fpath)
                 if self.columns:
                     self.df = self.df.select(self.columns)
                 for c in self.df.columns:
                     self.df = self.df.withColumnRenamed(c, f"{self.prefix}_{c}")
 
+        # at this point of connectors we may want to try integrating
+        # with something like fugue: https://github.com/fugue-project/fugue
+        elif self.compute_layer.value == 'ray':
+            pass
+
+        elif self.compute_layer.value == 'snowflake':
+            pass
+
+        elif self.compute_layer.value == 'postgres':
+            pass
+
+        elif self.compute_layer.value == 'redshift':
+            pass
+
 
     @abc.abstractmethod
     def do_filters (
         self
     ):
         """
 do some filters on the data
@@ -356,7 +370,47 @@
                         self.df[self.colabbr(self.date_key)] > (datetime.datetime.now() - datetime.timedelta(minutes=self.label_period_minutes()))
                     ]
                 elif isinstance(self.df, pyspark.sql.dataframe.DataFrame):
                     return self.df.filter(
                     self.df[self.colabbr(self.date_key)] > (datetime.datetime.now() - datetime.timedelta(minutes=self.label_period_minutes()))
                 )
         return self.df
+
+
+
+
+
+
+class DynamicNode(GraphReduceNode):
+    """
+A dynamic architecture for entities with no logic 
+needed in addition to the top-level GraphReduceNode
+parameters
+    """
+    def __init__ (
+            self,
+            *args,
+            **kwargs
+            ):
+        """
+Constructor
+        """
+        super().__init__(*args, **kwargs)
+
+
+    def do_filters(self):
+        pass
+
+    def do_annotate(self):
+        pass
+
+    def do_post_join_annotate(self):
+        pass
+
+    def do_clip_cols(self):
+        pass
+
+    def do_reduce(self):
+        pass
+
+    def do_labels(self):
+        pass
```

### Comparing `graphreduce-0.8/graphreduce.egg-info/PKG-INFO` & `graphreduce-0.9/graphreduce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 0.8
+Version: 0.9
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-0.8/setup.py` & `graphreduce-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 
 if __name__ == "__main__":
 
     setuptools.setup(
         name="graphreduce",
-        version = 0.8,
+        version = 0.9,
         url="https://github.com/wesmadrigal/graphreduce",
         packages = setuptools.find_packages(exclude=[ "docs", "examples" ]),
         install_requires = [
             "abstract.jwrotator>=0.3",
             "dask==2023.6.0",
             "networkx>=2.8.8",
             "pandas>=1.5.2",
```

