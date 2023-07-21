# Comparing `tmp/cloudimized-1.3.6rc1.tar.gz` & `tmp/cloudimized-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudimized-1.3.6rc1.tar", last modified: Thu Jul 20 09:09:08 2023, max compression
+gzip compressed data, was "cloudimized-1.3.7.tar", last modified: Fri Jul 21 11:14:39 2023, max compression
```

## Comparing `cloudimized-1.3.6rc1.tar` & `cloudimized-1.3.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:08.641117 cloudimized-1.3.6rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-07-20 09:09:08.641117 cloudimized-1.3.6rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14429 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:08.641117 cloudimized-1.3.6rc1/cloudimized/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:08.641117 cloudimized-1.3.6rc1/cloudimized/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/core/changeprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17609 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/core/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/core/jiranotifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/core/result.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/core/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/core/slacknotifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:08.641117 cloudimized-1.3.6rc1/cloudimized/gcpcore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/gcpcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/gcpcore/gcpchangelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/gcpcore/gcpquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/gcpcore/gcpservicequery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:08.641117 cloudimized-1.3.6rc1/cloudimized/gitcore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/gitcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/gitcore/gitchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/gitcore/repo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:08.641117 cloudimized-1.3.6rc1/cloudimized/tfcore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/tfcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/tfcore/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/cloudimized/tfcore/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:09:08.641117 cloudimized-1.3.6rc1/cloudimized.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-07-20 09:09:08.000000 cloudimized-1.3.6rc1/cloudimized.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-20 09:09:08.000000 cloudimized-1.3.6rc1/cloudimized.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 09:09:08.000000 cloudimized-1.3.6rc1/cloudimized.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-20 09:09:08.000000 cloudimized-1.3.6rc1/cloudimized.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-20 09:09:08.000000 cloudimized-1.3.6rc1/cloudimized.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 09:09:08.000000 cloudimized-1.3.6rc1/cloudimized.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 09:09:08.641117 cloudimized-1.3.6rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-20 09:09:04.000000 cloudimized-1.3.6rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:14:39.381605 cloudimized-1.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-21 11:14:32.000000 cloudimized-1.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15255 2023-07-21 11:14:39.381605 cloudimized-1.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14429 2023-07-21 11:14:32.000000 cloudimized-1.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:14:39.377604 cloudimized-1.3.7/cloudimized/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:14:32.000000 cloudimized-1.3.7/cloudimized/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:14:39.377604 cloudimized-1.3.7/cloudimized/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:14:32.000000 cloudimized-1.3.7/cloudimized/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-07-21 11:14:32.000000 cloudimized-1.3.7/cloudimized/core/changeprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17609 2023-07-21 11:14:32.000000 cloudimized-1.3.7/cloudimized/core/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-21 11:14:32.000000 cloudimized-1.3.7/cloudimized/core/jiranotifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-07-21 11:14:32.000000 cloudimized-1.3.7/cloudimized/core/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-21 11:14:32.000000 cloudimized-1.3.7/cloudimized/core/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-21 11:14:32.000000 cloudimized-1.3.7/cloudimized/core/slacknotifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:14:39.377604 cloudimized-1.3.7/cloudimized/gcpcore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:14:32.000000 cloudimized-1.3.7/cloudimized/gcpcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-21 11:14:32.000000 cloudimized-1.3.7/cloudimized/gcpcore/gcpchangelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-07-21 11:14:32.000000 cloudimized-1.3.7/cloudimized/gcpcore/gcpquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-21 11:14:32.000000 cloudimized-1.3.7/cloudimized/gcpcore/gcpservicequery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:14:39.377604 cloudimized-1.3.7/cloudimized/gitcore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:14:32.000000 cloudimized-1.3.7/cloudimized/gitcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-21 11:14:32.000000 cloudimized-1.3.7/cloudimized/gitcore/gitchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-07-21 11:14:32.000000 cloudimized-1.3.7/cloudimized/gitcore/repo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:14:39.381605 cloudimized-1.3.7/cloudimized/tfcore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:14:32.000000 cloudimized-1.3.7/cloudimized/tfcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-07-21 11:14:32.000000 cloudimized-1.3.7/cloudimized/tfcore/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-21 11:14:32.000000 cloudimized-1.3.7/cloudimized/tfcore/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:14:39.377604 cloudimized-1.3.7/cloudimized.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15255 2023-07-21 11:14:39.000000 cloudimized-1.3.7/cloudimized.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-21 11:14:39.000000 cloudimized-1.3.7/cloudimized.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:14:39.000000 cloudimized-1.3.7/cloudimized.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-21 11:14:39.000000 cloudimized-1.3.7/cloudimized.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-21 11:14:39.000000 cloudimized-1.3.7/cloudimized.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 11:14:39.000000 cloudimized-1.3.7/cloudimized.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 11:14:39.381605 cloudimized-1.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-21 11:14:32.000000 cloudimized-1.3.7/setup.py
```

### Comparing `cloudimized-1.3.6rc1/LICENSE` & `cloudimized-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.6rc1/PKG-INFO` & `cloudimized-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudimized
-Version: 1.3.6rc1
+Version: 1.3.7
 Summary: Google Cloud Platform (GCP) configuration scanning tool
 Home-page: https://github.com/egnyte/cloudimized
 Author: Egnyte and Contributors
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cloudimized-1.3.6rc1/README.md` & `cloudimized-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.6rc1/cloudimized/core/changeprocessor.py` & `cloudimized-1.3.7/cloudimized/core/changeprocessor.py`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.6rc1/cloudimized/core/core.py` & `cloudimized-1.3.7/cloudimized/core/core.py`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.6rc1/cloudimized/core/jiranotifier.py` & `cloudimized-1.3.7/cloudimized/core/jiranotifier.py`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.6rc1/cloudimized/core/result.py` & `cloudimized-1.3.7/cloudimized/core/result.py`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.6rc1/cloudimized/core/slacknotifier.py` & `cloudimized-1.3.7/cloudimized/core/slacknotifier.py`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.6rc1/cloudimized/gcpcore/gcpchangelog.py` & `cloudimized-1.3.7/cloudimized/gcpcore/gcpchangelog.py`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.6rc1/cloudimized/gcpcore/gcpquery.py` & `cloudimized-1.3.7/cloudimized/gcpcore/gcpquery.py`

 * *Files 6% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         self.__sort_result(result, project_id)
         if self.result_item_filter:
             for filter_condition_set in self.result_item_filter:
                 result[:] = [i for i in result if self.__filter_item(i, filter_condition_set)]
         if self.result_exclude_filter:
             return self.__filter_field_exclude(self.result_exclude_filter, result)
         elif self.result_include_filter:
-            return self._filter_result_include(result)
+            return self._filter_field_include(self.result_include_filter, result)
         else:
             return result
 
     def __filter_field_exclude(self, fields: List[Union[str, Dict]], result: List[Dict]) -> List[Dict]:
         filtered_result = result[:]
         for field in fields:
             if isinstance(field, str):
@@ -132,21 +132,37 @@
                         nested_result = item.get(nested_key, {})
                         if isinstance(nested_result, dict):
                             self.__filter_field_exclude(fields=nested_fields, result=[nested_result])
                         if isinstance(nested_result, list):
                             self.__filter_field_exclude(fields=nested_fields, result=nested_result)
         return filtered_result
 
-    def _filter_result_include(self, result: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
-        """Filter out all fields except ones specified from each item in results"""
-        filtered_result = []
-        for item in result:
-            filtered_item = {key: item[key] for key in item if key in self.result_include_filter}
-            filtered_result.append(filtered_item)
-        return filtered_result
+    def _filter_field_include(self, fields: List[Union[str, Dict]], result: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
+        """
+        Filter out all fields except ones specified from each item in results
+        """
+        def filter_dict(entry, filters):
+            filtered_entry = {}
+            for key, value in entry.items():
+                if isinstance(value, dict):
+                    if key in filters:
+                        if not filters[key]:  # Include the entire nested dictionary
+                            filtered_entry[key] = filter_dict(value, {})
+                        else:
+                            filtered_entry[key] = filter_dict(value, filters[key])
+                elif key in filters or not filters:  # Include the field if it's in filters or filters are empty
+                    filtered_entry[key] = value
+            return filtered_entry
+
+        filtered_data = []
+        for entry in result:
+            filtered_entry = filter_dict(entry, fields)
+            filtered_data.append(filtered_entry)
+
+        return filtered_data
 
     def __filter_item(self, item: Dict[str, Any], filter_condition_set) -> bool:
         for filter_field, filter_condition in filter_condition_set.items():
             if isinstance(filter_condition, str):
                 field_value = item.get(filter_field, "")
                 if isinstance(field_value, list):
                     field_value[:] = [i for i in field_value if not re.match(rf"{filter_condition}", i)]
```

### Comparing `cloudimized-1.3.6rc1/cloudimized/gcpcore/gcpservicequery.py` & `cloudimized-1.3.7/cloudimized/gcpcore/gcpservicequery.py`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.6rc1/cloudimized/gitcore/gitchange.py` & `cloudimized-1.3.7/cloudimized/gitcore/gitchange.py`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.6rc1/cloudimized/gitcore/repo.py` & `cloudimized-1.3.7/cloudimized/gitcore/repo.py`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.6rc1/cloudimized/tfcore/query.py` & `cloudimized-1.3.7/cloudimized/tfcore/query.py`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.6rc1/cloudimized/tfcore/run.py` & `cloudimized-1.3.7/cloudimized/tfcore/run.py`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.6rc1/cloudimized.egg-info/PKG-INFO` & `cloudimized-1.3.7/cloudimized.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudimized
-Version: 1.3.6rc1
+Version: 1.3.7
 Summary: Google Cloud Platform (GCP) configuration scanning tool
 Home-page: https://github.com/egnyte/cloudimized
 Author: Egnyte and Contributors
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cloudimized-1.3.6rc1/cloudimized.egg-info/SOURCES.txt` & `cloudimized-1.3.7/cloudimized.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.6rc1/cloudimized.egg-info/requires.txt` & `cloudimized-1.3.7/cloudimized.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cloudimized-1.3.6rc1/setup.py` & `cloudimized-1.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with codecs.open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name="cloudimized",
-    version="1.3.6rc1",
+    version="1.3.7",
     description='Google Cloud Platform (GCP) configuration scanning tool',
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/egnyte/cloudimized",
     author="Egnyte and Contributors",
     classifiers=[
         "Programming Language :: Python :: 3.7",
```

