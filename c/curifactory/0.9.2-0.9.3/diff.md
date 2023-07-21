# Comparing `tmp/curifactory-0.9.2.tar.gz` & `tmp/curifactory-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curifactory-0.9.2.tar", last modified: Tue Mar 21 00:26:32 2023, max compression
+gzip compressed data, was "curifactory-0.9.3.tar", last modified: Tue Mar 21 15:19:30 2023, max compression
```

## Comparing `curifactory-0.9.2.tar` & `curifactory-0.9.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-03-21 00:26:32.704348 curifactory-0.9.2/
--rw-r--r--   0 81n      (42021) users      (100)     1524 2022-06-14 18:20:24.000000 curifactory-0.9.2/LICENSE
--rw-r--r--   0 81n      (42021) users      (100)     3612 2023-03-21 00:26:32.704348 curifactory-0.9.2/PKG-INFO
--rw-r--r--   0 81n      (42021) users      (100)     2868 2022-12-14 19:28:47.000000 curifactory-0.9.2/README.md
-drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-03-21 00:26:32.700348 curifactory-0.9.2/curifactory/
--rw-r--r--   0 81n      (42021) users      (100)      462 2023-03-21 00:22:36.000000 curifactory-0.9.2/curifactory/__init__.py
--rw-r--r--   0 81n      (42021) users      (100)     2824 2023-03-10 19:33:43.000000 curifactory-0.9.2/curifactory/args.py
--rw-r--r--   0 81n      (42021) users      (100)    10009 2023-03-21 00:18:42.000000 curifactory-0.9.2/curifactory/caching.py
-drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-03-21 00:26:32.704348 curifactory-0.9.2/curifactory/data/
--rw-r--r--   0 81n      (42021) users      (100)       20 2022-06-14 18:20:24.000000 curifactory-0.9.2/curifactory/data/.dockerignore
--rw-r--r--   0 81n      (42021) users      (100)      226 2022-06-14 18:20:24.000000 curifactory-0.9.2/curifactory/data/debug.py
--rw-r--r--   0 81n      (42021) users      (100)      879 2022-06-14 18:20:24.000000 curifactory-0.9.2/curifactory/data/dockerfile
--rw-r--r--   0 81n      (42021) users      (100)      353 2022-06-14 18:20:24.000000 curifactory-0.9.2/curifactory/data/startup.sh
--rw-r--r--   0 81n      (42021) users      (100)      948 2022-06-14 18:20:24.000000 curifactory-0.9.2/curifactory/data/style.css
--rw-r--r--   0 81n      (42021) users      (100)     1133 2022-06-14 18:20:24.000000 curifactory-0.9.2/curifactory/docker.py
--rw-r--r--   0 81n      (42021) users      (100)    50485 2023-03-15 17:47:04.000000 curifactory-0.9.2/curifactory/experiment.py
--rw-r--r--   0 81n      (42021) users      (100)    13555 2023-03-16 13:36:24.000000 curifactory-0.9.2/curifactory/hashing.py
--rw-r--r--   0 81n      (42021) users      (100)    30039 2023-03-09 14:05:20.000000 curifactory-0.9.2/curifactory/manager.py
--rw-r--r--   0 81n      (42021) users      (100)     4506 2022-12-14 18:20:46.000000 curifactory-0.9.2/curifactory/procedure.py
--rw-r--r--   0 81n      (42021) users      (100)     7071 2023-03-09 14:50:07.000000 curifactory-0.9.2/curifactory/project.py
--rw-r--r--   0 81n      (42021) users      (100)    11616 2023-03-21 00:18:42.000000 curifactory-0.9.2/curifactory/record.py
--rw-r--r--   0 81n      (42021) users      (100)    37411 2023-03-10 19:33:43.000000 curifactory-0.9.2/curifactory/reporting.py
--rw-r--r--   0 81n      (42021) users      (100)    41298 2023-03-21 00:18:42.000000 curifactory-0.9.2/curifactory/staging.py
--rw-r--r--   0 81n      (42021) users      (100)     6994 2022-12-14 18:20:46.000000 curifactory-0.9.2/curifactory/store.py
--rw-r--r--   0 81n      (42021) users      (100)    13649 2023-03-10 19:33:43.000000 curifactory-0.9.2/curifactory/utils.py
-drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-03-21 00:26:32.700348 curifactory-0.9.2/curifactory.egg-info/
--rw-r--r--   0 81n      (42021) users      (100)     3612 2023-03-21 00:26:32.000000 curifactory-0.9.2/curifactory.egg-info/PKG-INFO
--rw-r--r--   0 81n      (42021) users      (100)      924 2023-03-21 00:26:32.000000 curifactory-0.9.2/curifactory.egg-info/SOURCES.txt
--rw-r--r--   0 81n      (42021) users      (100)        1 2023-03-21 00:26:32.000000 curifactory-0.9.2/curifactory.egg-info/dependency_links.txt
--rw-r--r--   0 81n      (42021) users      (100)       98 2023-03-21 00:26:32.000000 curifactory-0.9.2/curifactory.egg-info/entry_points.txt
--rw-r--r--   0 81n      (42021) users      (100)       62 2023-03-21 00:26:32.000000 curifactory-0.9.2/curifactory.egg-info/requires.txt
--rw-r--r--   0 81n      (42021) users      (100)       12 2023-03-21 00:26:32.000000 curifactory-0.9.2/curifactory.egg-info/top_level.txt
--rw-r--r--   0 81n      (42021) users      (100)       31 2022-12-14 18:20:45.000000 curifactory-0.9.2/pyproject.toml
--rw-r--r--   0 81n      (42021) users      (100)       38 2023-03-21 00:26:32.704348 curifactory-0.9.2/setup.cfg
--rw-r--r--   0 81n      (42021) users      (100)     1655 2022-12-14 18:52:24.000000 curifactory-0.9.2/setup.py
-drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-03-21 00:26:32.704348 curifactory-0.9.2/test/
--rw-r--r--   0 81n      (42021) users      (100)     1212 2022-12-14 18:20:46.000000 curifactory-0.9.2/test/test_base.py
--rw-r--r--   0 81n      (42021) users      (100)    19196 2023-03-09 15:17:44.000000 curifactory-0.9.2/test/test_caching.py
--rw-r--r--   0 81n      (42021) users      (100)      846 2022-12-14 18:20:46.000000 curifactory-0.9.2/test/test_docker.py
--rw-r--r--   0 81n      (42021) users      (100)    12974 2023-03-15 17:31:55.000000 curifactory-0.9.2/test/test_experiment.py
--rw-r--r--   0 81n      (42021) users      (100)    10496 2023-03-16 13:36:24.000000 curifactory-0.9.2/test/test_hashing.py
--rw-r--r--   0 81n      (42021) users      (100)    13750 2023-03-10 19:33:43.000000 curifactory-0.9.2/test/test_manager.py
--rw-r--r--   0 81n      (42021) users      (100)     6540 2023-03-09 14:50:07.000000 curifactory-0.9.2/test/test_project.py
--rw-r--r--   0 81n      (42021) users      (100)     4283 2023-03-10 19:33:43.000000 curifactory-0.9.2/test/test_record.py
--rw-r--r--   0 81n      (42021) users      (100)     1124 2022-12-14 18:20:46.000000 curifactory-0.9.2/test/test_reporting.py
--rw-r--r--   0 81n      (42021) users      (100)    23236 2023-03-21 00:18:42.000000 curifactory-0.9.2/test/test_staging.py
+drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-03-21 15:19:30.985068 curifactory-0.9.3/
+-rw-r--r--   0 81n      (42021) users      (100)     1524 2022-06-14 18:20:24.000000 curifactory-0.9.3/LICENSE
+-rw-r--r--   0 81n      (42021) users      (100)     3612 2023-03-21 15:19:30.985068 curifactory-0.9.3/PKG-INFO
+-rw-r--r--   0 81n      (42021) users      (100)     2868 2022-12-14 19:28:47.000000 curifactory-0.9.3/README.md
+drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-03-21 15:19:30.981068 curifactory-0.9.3/curifactory/
+-rw-r--r--   0 81n      (42021) users      (100)      462 2023-03-21 15:18:20.000000 curifactory-0.9.3/curifactory/__init__.py
+-rw-r--r--   0 81n      (42021) users      (100)     2824 2023-03-10 19:33:43.000000 curifactory-0.9.3/curifactory/args.py
+-rw-r--r--   0 81n      (42021) users      (100)    10009 2023-03-21 00:18:42.000000 curifactory-0.9.3/curifactory/caching.py
+drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-03-21 15:19:30.981068 curifactory-0.9.3/curifactory/data/
+-rw-r--r--   0 81n      (42021) users      (100)       20 2022-06-14 18:20:24.000000 curifactory-0.9.3/curifactory/data/.dockerignore
+-rw-r--r--   0 81n      (42021) users      (100)      226 2022-06-14 18:20:24.000000 curifactory-0.9.3/curifactory/data/debug.py
+-rw-r--r--   0 81n      (42021) users      (100)      879 2022-06-14 18:20:24.000000 curifactory-0.9.3/curifactory/data/dockerfile
+-rw-r--r--   0 81n      (42021) users      (100)      353 2022-06-14 18:20:24.000000 curifactory-0.9.3/curifactory/data/startup.sh
+-rw-r--r--   0 81n      (42021) users      (100)      948 2022-06-14 18:20:24.000000 curifactory-0.9.3/curifactory/data/style.css
+-rw-r--r--   0 81n      (42021) users      (100)     1133 2022-06-14 18:20:24.000000 curifactory-0.9.3/curifactory/docker.py
+-rw-r--r--   0 81n      (42021) users      (100)    50485 2023-03-21 15:01:17.000000 curifactory-0.9.3/curifactory/experiment.py
+-rw-r--r--   0 81n      (42021) users      (100)    13555 2023-03-16 13:36:24.000000 curifactory-0.9.3/curifactory/hashing.py
+-rw-r--r--   0 81n      (42021) users      (100)    30039 2023-03-21 15:01:17.000000 curifactory-0.9.3/curifactory/manager.py
+-rw-r--r--   0 81n      (42021) users      (100)     4506 2022-12-14 18:20:46.000000 curifactory-0.9.3/curifactory/procedure.py
+-rw-r--r--   0 81n      (42021) users      (100)     7071 2023-03-09 14:50:07.000000 curifactory-0.9.3/curifactory/project.py
+-rw-r--r--   0 81n      (42021) users      (100)    11616 2023-03-21 15:01:17.000000 curifactory-0.9.3/curifactory/record.py
+-rw-r--r--   0 81n      (42021) users      (100)    37305 2023-03-21 15:18:10.000000 curifactory-0.9.3/curifactory/reporting.py
+-rw-r--r--   0 81n      (42021) users      (100)    41298 2023-03-21 15:01:17.000000 curifactory-0.9.3/curifactory/staging.py
+-rw-r--r--   0 81n      (42021) users      (100)     6994 2023-03-21 15:01:17.000000 curifactory-0.9.3/curifactory/store.py
+-rw-r--r--   0 81n      (42021) users      (100)    13649 2023-03-10 19:33:43.000000 curifactory-0.9.3/curifactory/utils.py
+drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-03-21 15:19:30.981068 curifactory-0.9.3/curifactory.egg-info/
+-rw-r--r--   0 81n      (42021) users      (100)     3612 2023-03-21 15:19:30.000000 curifactory-0.9.3/curifactory.egg-info/PKG-INFO
+-rw-r--r--   0 81n      (42021) users      (100)      924 2023-03-21 15:19:30.000000 curifactory-0.9.3/curifactory.egg-info/SOURCES.txt
+-rw-r--r--   0 81n      (42021) users      (100)        1 2023-03-21 15:19:30.000000 curifactory-0.9.3/curifactory.egg-info/dependency_links.txt
+-rw-r--r--   0 81n      (42021) users      (100)       98 2023-03-21 15:19:30.000000 curifactory-0.9.3/curifactory.egg-info/entry_points.txt
+-rw-r--r--   0 81n      (42021) users      (100)       62 2023-03-21 15:19:30.000000 curifactory-0.9.3/curifactory.egg-info/requires.txt
+-rw-r--r--   0 81n      (42021) users      (100)       12 2023-03-21 15:19:30.000000 curifactory-0.9.3/curifactory.egg-info/top_level.txt
+-rw-r--r--   0 81n      (42021) users      (100)       31 2022-12-14 18:20:45.000000 curifactory-0.9.3/pyproject.toml
+-rw-r--r--   0 81n      (42021) users      (100)       38 2023-03-21 15:19:30.985068 curifactory-0.9.3/setup.cfg
+-rw-r--r--   0 81n      (42021) users      (100)     1655 2022-12-14 18:52:24.000000 curifactory-0.9.3/setup.py
+drwxr-xr-x   0 81n      (42021) users      (100)        0 2023-03-21 15:19:30.985068 curifactory-0.9.3/test/
+-rw-r--r--   0 81n      (42021) users      (100)     1212 2022-12-14 18:20:46.000000 curifactory-0.9.3/test/test_base.py
+-rw-r--r--   0 81n      (42021) users      (100)    19196 2023-03-21 15:01:17.000000 curifactory-0.9.3/test/test_caching.py
+-rw-r--r--   0 81n      (42021) users      (100)      846 2022-12-14 18:20:46.000000 curifactory-0.9.3/test/test_docker.py
+-rw-r--r--   0 81n      (42021) users      (100)    12974 2023-03-21 15:01:17.000000 curifactory-0.9.3/test/test_experiment.py
+-rw-r--r--   0 81n      (42021) users      (100)    10496 2023-03-16 13:36:24.000000 curifactory-0.9.3/test/test_hashing.py
+-rw-r--r--   0 81n      (42021) users      (100)    13750 2023-03-21 15:01:17.000000 curifactory-0.9.3/test/test_manager.py
+-rw-r--r--   0 81n      (42021) users      (100)     6540 2023-03-09 14:50:07.000000 curifactory-0.9.3/test/test_project.py
+-rw-r--r--   0 81n      (42021) users      (100)     4283 2023-03-10 19:33:43.000000 curifactory-0.9.3/test/test_record.py
+-rw-r--r--   0 81n      (42021) users      (100)     1773 2023-03-21 15:18:35.000000 curifactory-0.9.3/test/test_reporting.py
+-rw-r--r--   0 81n      (42021) users      (100)    23236 2023-03-21 00:18:42.000000 curifactory-0.9.3/test/test_staging.py
```

### Comparing `curifactory-0.9.2/LICENSE` & `curifactory-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/PKG-INFO` & `curifactory-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curifactory
-Version: 0.9.2
+Version: 0.9.3
 Summary: An experiment workflow and organization tool
 Home-page: https://github.com/ORNL/curifactory
 Author: Nathan Martindale, Jason Hite, Scott L. Stewart, Mark Adams
 Author-email: curifactory-help@ornl.gov
 Project-URL: Documentation, https://ornl.github.io/curifactory/latest/index.html
 Keywords: research,experiment,workflow
 Classifier: Programming Language :: Python :: 3
```

### Comparing `curifactory-0.9.2/README.md` & `curifactory-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/curifactory/args.py` & `curifactory-0.9.3/curifactory/args.py`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/curifactory/caching.py` & `curifactory-0.9.3/curifactory/caching.py`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/curifactory/data/dockerfile` & `curifactory-0.9.3/curifactory/data/dockerfile`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/curifactory/data/style.css` & `curifactory-0.9.3/curifactory/data/style.css`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/curifactory/docker.py` & `curifactory-0.9.3/curifactory/docker.py`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/curifactory/experiment.py` & `curifactory-0.9.3/curifactory/experiment.py`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/curifactory/hashing.py` & `curifactory-0.9.3/curifactory/hashing.py`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/curifactory/manager.py` & `curifactory-0.9.3/curifactory/manager.py`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/curifactory/procedure.py` & `curifactory-0.9.3/curifactory/procedure.py`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/curifactory/project.py` & `curifactory-0.9.3/curifactory/project.py`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/curifactory/record.py` & `curifactory-0.9.3/curifactory/record.py`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/curifactory/reporting.py` & `curifactory-0.9.3/curifactory/reporting.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 to an HTML experiement run report.
 
 This is handled through a base :code:`Reportable` class, and each reporter class
 extends it.
 """
 
 import datetime
+import html
 import json
 import logging
 import os
 import shutil
 from typing import List
 
 import matplotlib.pyplot as plt
@@ -555,20 +556,16 @@
     argsets = manager.get_all_argsets()
     for argset in argsets:
         name = argset.name
         args_hash = argset.hash
         html_lines.append(f"<h4>{name} - {args_hash}</h4>")
         html_lines.append("<pre>")
 
-        def stringify(x):
-            # make html-safe
-            return str(x).replace("<", "&lt;").replace(">", "&gt;")
-
         argset_data = hashing.parameters_string_hash_representation(argset)
-        html_lines.append(json.dumps(argset_data, indent=2, default=stringify))
+        html_lines.append(html.escape(json.dumps(argset_data, indent=2, default=str)))
         html_lines.append("</pre>")
 
     return html_lines
 
 
 def prepare_report_path(output_path, report_name):
     """Set up any necessary folders for a report at the given location. This will not error if the location already has a report in it, but will remove existing reportables and graphs."""
@@ -746,15 +743,14 @@
                 info["order_timestamp"] = datetime.datetime.strptime(
                     info["timestamp"], utils.TIMESTAMP_FORMAT
                 )
 
                 runs.append(info)
                 experiment_name = info["experiment_name"]
                 if experiment_name not in experiment_runs:
-
                     # try to get comment on experiment
                     comment = ""
                     try:
                         with open(f"{experiments_path}/{experiment_name}.py") as infile:
                             lines = infile.readlines()
                             comment = utils.get_py_opening_comment(lines)
                     except:  # noqa: E722 -- there's not really any need to handle this, either we get the comment or we don't.
```

### Comparing `curifactory-0.9.2/curifactory/staging.py` & `curifactory-0.9.3/curifactory/staging.py`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/curifactory/store.py` & `curifactory-0.9.3/curifactory/store.py`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/curifactory/utils.py` & `curifactory-0.9.3/curifactory/utils.py`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/curifactory.egg-info/PKG-INFO` & `curifactory-0.9.3/curifactory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curifactory
-Version: 0.9.2
+Version: 0.9.3
 Summary: An experiment workflow and organization tool
 Home-page: https://github.com/ORNL/curifactory
 Author: Nathan Martindale, Jason Hite, Scott L. Stewart, Mark Adams
 Author-email: curifactory-help@ornl.gov
 Project-URL: Documentation, https://ornl.github.io/curifactory/latest/index.html
 Keywords: research,experiment,workflow
 Classifier: Programming Language :: Python :: 3
```

### Comparing `curifactory-0.9.2/curifactory.egg-info/SOURCES.txt` & `curifactory-0.9.3/curifactory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/setup.py` & `curifactory-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/test/test_base.py` & `curifactory-0.9.3/test/test_base.py`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/test/test_caching.py` & `curifactory-0.9.3/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/test/test_docker.py` & `curifactory-0.9.3/test/test_docker.py`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/test/test_experiment.py` & `curifactory-0.9.3/test/test_experiment.py`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/test/test_hashing.py` & `curifactory-0.9.3/test/test_hashing.py`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/test/test_manager.py` & `curifactory-0.9.3/test/test_manager.py`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/test/test_project.py` & `curifactory-0.9.3/test/test_project.py`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/test/test_record.py` & `curifactory-0.9.3/test/test_record.py`

 * *Files identical despite different names*

### Comparing `curifactory-0.9.2/test/test_staging.py` & `curifactory-0.9.3/test/test_staging.py`

 * *Files identical despite different names*

