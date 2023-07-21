# Comparing `tmp/veetility-0.1.98.tar.gz` & `tmp/veetility-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veetility-0.1.98.tar", last modified: Thu Jul  6 17:27:36 2023, max compression
+gzip compressed data, was "veetility-0.1.99.tar", last modified: Fri Jul  7 08:26:09 2023, max compression
```

## Comparing `veetility-0.1.98.tar` & `veetility-0.1.99.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-06 17:27:36.921010 veetility-0.1.98/
--rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-07-06 17:27:36.920866 veetility-0.1.98/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)     2881 2023-02-28 17:30:34.000000 veetility-0.1.98/README.md
--rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-07-06 17:27:36.921062 veetility-0.1.98/setup.cfg
--rw-r--r--   0 willbutler   (502) staff       (20)     1438 2023-07-06 17:26:22.000000 veetility-0.1.98/setup.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-06 17:27:36.912028 veetility-0.1.98/tests/
--rw-r--r--   0 willbutler   (502) staff       (20)     1892 2023-04-09 19:51:45.000000 veetility-0.1.98/tests/test_best_fuzzy_match_dict.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2471 2023-04-09 19:42:01.000000 veetility-0.1.98/tests/test_identify_match_multi_cols.py
--rw-r--r--   0 willbutler   (502) staff       (20)     1588 2023-04-09 18:45:40.000000 veetility-0.1.98/tests/test_prepare_string_matching.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-06 17:27:36.919240 veetility-0.1.98/veetility/
--rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-02-28 17:30:34.000000 veetility-0.1.98/veetility/__init__.py
--rw-r--r--   0 willbutler   (502) staff       (20)    18470 2023-07-06 17:26:05.000000 veetility-0.1.98/veetility/cleaning_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     7088 2023-05-23 14:51:46.000000 veetility-0.1.98/veetility/generic_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2465 2023-03-03 12:20:14.000000 veetility-0.1.98/veetility/point_to_point_regressor.py
--rw-r--r--   0 willbutler   (502) staff       (20)    31537 2023-07-04 10:24:35.000000 veetility-0.1.98/veetility/quality_assessments.py
--rw-r--r--   0 willbutler   (502) staff       (20)    11585 2023-05-23 16:42:13.000000 veetility-0.1.98/veetility/snowflake.py
--rw-r--r--   0 willbutler   (502) staff       (20)    53704 2023-07-04 10:08:58.000000 veetility-0.1.98/veetility/utility_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2411 2023-05-05 13:50:17.000000 veetility-0.1.98/veetility/v_lift.py
--rw-r--r--   0 willbutler   (502) staff       (20)     6007 2023-06-12 15:35:11.000000 veetility-0.1.98/veetility/view_through_rate.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-06 17:27:36.920656 veetility-0.1.98/veetility.egg-info/
--rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-07-06 17:27:36.000000 veetility-0.1.98/veetility.egg-info/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)      557 2023-07-06 17:27:36.000000 veetility-0.1.98/veetility.egg-info/SOURCES.txt
--rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-07-06 17:27:36.000000 veetility-0.1.98/veetility.egg-info/dependency_links.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       97 2023-07-06 17:27:36.000000 veetility-0.1.98/veetility.egg-info/requires.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-07-06 17:27:36.000000 veetility-0.1.98/veetility.egg-info/top_level.txt
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-07 08:26:09.812797 veetility-0.1.99/
+-rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-07-07 08:26:09.812613 veetility-0.1.99/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)     2881 2023-02-28 17:30:34.000000 veetility-0.1.99/README.md
+-rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-07-07 08:26:09.812863 veetility-0.1.99/setup.cfg
+-rw-r--r--   0 willbutler   (502) staff       (20)     1438 2023-07-07 08:25:59.000000 veetility-0.1.99/setup.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-07 08:26:09.807283 veetility-0.1.99/tests/
+-rw-r--r--   0 willbutler   (502) staff       (20)     1892 2023-04-09 19:51:45.000000 veetility-0.1.99/tests/test_best_fuzzy_match_dict.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2471 2023-04-09 19:42:01.000000 veetility-0.1.99/tests/test_identify_match_multi_cols.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     1588 2023-04-09 18:45:40.000000 veetility-0.1.99/tests/test_prepare_string_matching.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-07 08:26:09.811365 veetility-0.1.99/veetility/
+-rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-02-28 17:30:34.000000 veetility-0.1.99/veetility/__init__.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    18488 2023-07-07 08:13:19.000000 veetility-0.1.99/veetility/cleaning_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     7088 2023-05-23 14:51:46.000000 veetility-0.1.99/veetility/generic_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2465 2023-03-03 12:20:14.000000 veetility-0.1.99/veetility/point_to_point_regressor.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    31537 2023-07-04 10:24:35.000000 veetility-0.1.99/veetility/quality_assessments.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    11585 2023-05-23 16:42:13.000000 veetility-0.1.99/veetility/snowflake.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    53704 2023-07-04 10:08:58.000000 veetility-0.1.99/veetility/utility_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2411 2023-05-05 13:50:17.000000 veetility-0.1.99/veetility/v_lift.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     6007 2023-06-12 15:35:11.000000 veetility-0.1.99/veetility/view_through_rate.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-07 08:26:09.812359 veetility-0.1.99/veetility.egg-info/
+-rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-07-07 08:26:09.000000 veetility-0.1.99/veetility.egg-info/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)      557 2023-07-07 08:26:09.000000 veetility-0.1.99/veetility.egg-info/SOURCES.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-07-07 08:26:09.000000 veetility-0.1.99/veetility.egg-info/dependency_links.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       97 2023-07-07 08:26:09.000000 veetility-0.1.99/veetility.egg-info/requires.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-07-07 08:26:09.000000 veetility-0.1.99/veetility.egg-info/top_level.txt
```

### Comparing `veetility-0.1.98/PKG-INFO` & `veetility-0.1.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veetility
-Version: 0.1.98
+Version: 0.1.99
 Summary: Demo library
 Home-page: 
 Author: Vaynermedia
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `veetility-0.1.98/README.md` & `veetility-0.1.99/README.md`

 * *Files identical despite different names*

### Comparing `veetility-0.1.98/setup.py` & `veetility-0.1.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="veetility",
-    version="0.1.98",
+    version="0.1.99",
     description="Demo library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Vaynermedia",
     author_email="will.butler@vaynermedia.com",
     license="MIT",
```

### Comparing `veetility-0.1.98/tests/test_best_fuzzy_match_dict.py` & `veetility-0.1.99/tests/test_best_fuzzy_match_dict.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.98/tests/test_identify_match_multi_cols.py` & `veetility-0.1.99/tests/test_identify_match_multi_cols.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.98/tests/test_prepare_string_matching.py` & `veetility-0.1.99/tests/test_prepare_string_matching.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.98/veetility/cleaning_functions.py` & `veetility-0.1.99/veetility/cleaning_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,21 +124,21 @@
         elif (('type' in column) & ('post' in column)) or (('media' in column) and ('type' in column)) \
             or (('content' in column) and ('category' in column)): #creative media type for fb_ig_paid
             new_columns[column] = 'media_type'
         elif('cohort' in column):
             new_columns[column] = 'cohort'
         else:
             message = f'Column "{column}" in {name_of_df} not cleaned'
+            new_columns[column] = column
             if errors == 'raise':
                 raise Exception(message)
             cleaning_logger.logger.info(message)
 
-        new_columns[column] = column
-        duplicated_cols = [item for item,count in Counter(list(new_columns.values())).items() if count > 1]
-        print(f'{name_of_df} : {new_columns}')
+    duplicated_cols = [item for item,count in Counter(list(new_columns.values())).items() if count > 1]
+    cleaning_logger.logger.info(f"{name_of_df} : {new_columns}")
     if len(duplicated_cols) > 0:
         error = f'Duplicate column names in {name_of_df} : {[f"{key} -> {value}" for key, value in dict.items() if value in duplicated_cols]}'
         # error = f'Duplicate column names in {name_of_df} : {[item for item, count in Counter(new_columns).items() if count > 1]}'
         cleaning_logger.logger.exception(error)
         raise ValueError(error)
     df.columns = list(new_columns.values())
```

### Comparing `veetility-0.1.98/veetility/generic_functions.py` & `veetility-0.1.99/veetility/generic_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.98/veetility/point_to_point_regressor.py` & `veetility-0.1.99/veetility/point_to_point_regressor.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.98/veetility/quality_assessments.py` & `veetility-0.1.99/veetility/quality_assessments.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.98/veetility/snowflake.py` & `veetility-0.1.99/veetility/snowflake.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.98/veetility/utility_functions.py` & `veetility-0.1.99/veetility/utility_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.98/veetility/v_lift.py` & `veetility-0.1.99/veetility/v_lift.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.98/veetility/view_through_rate.py` & `veetility-0.1.99/veetility/view_through_rate.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.98/veetility.egg-info/PKG-INFO` & `veetility-0.1.99/veetility.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veetility
-Version: 0.1.98
+Version: 0.1.99
 Summary: Demo library
 Home-page: 
 Author: Vaynermedia
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `veetility-0.1.98/veetility.egg-info/SOURCES.txt` & `veetility-0.1.99/veetility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

