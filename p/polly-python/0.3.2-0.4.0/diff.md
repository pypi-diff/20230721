# Comparing `tmp/polly-python-0.3.2.tar.gz` & `tmp/polly-python-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polly-python-0.3.2.tar", last modified: Fri Jun 23 05:14:37 2023, max compression
+gzip compressed data, was "polly-python-0.4.0.tar", last modified: Fri Jul 21 07:08:24 2023, max compression
```

## Comparing `polly-python-0.3.2.tar` & `polly-python-0.4.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:14:37.420019 polly-python-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-06-23 05:13:10.000000 polly-python-0.3.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-23 05:13:10.000000 polly-python-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-23 05:14:37.420019 polly-python-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-23 05:13:10.000000 polly-python-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:14:37.416018 polly-python-0.3.2/polly/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14714 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/application_error_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    16367 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/bridge_cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)    16238 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    31214 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/core_cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)    20886 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/curation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/help.py
--rw-r--r--   0 runner    (1001) docker     (123)    35626 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/http_response_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/index_schema_level_conversion_const.py
--rw-r--r--   0 runner    (1001) docker     (123)    24441 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)   198255 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/omixatlas.py
--rw-r--r--   0 runner    (1001) docker     (123)    73864 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/omixatlas_hlpr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16510 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/validation_hlpr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13003 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:14:37.420019 polly-python-0.3.2/polly_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-23 05:14:37.000000 polly-python-0.3.2/polly_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-23 05:14:37.000000 polly-python-0.3.2/polly_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 05:14:37.000000 polly-python-0.3.2/polly_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-23 05:14:37.000000 polly-python-0.3.2/polly_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 05:14:37.000000 polly-python-0.3.2/polly_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-23 05:13:10.000000 polly-python-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-23 05:14:37.420019 polly-python-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 05:13:10.000000 polly-python-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:14:37.420019 polly-python-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-06-23 05:13:10.000000 polly-python-0.3.2/tests/test_cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-23 05:13:10.000000 polly-python-0.3.2/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-23 05:13:10.000000 polly-python-0.3.2/tests/test_curation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-23 05:13:10.000000 polly-python-0.3.2/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-06-23 05:13:10.000000 polly-python-0.3.2/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    98539 2023-06-23 05:13:10.000000 polly-python-0.3.2/tests/test_omixatlas.py
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-06-23 05:13:10.000000 polly-python-0.3.2/tests/test_schema_ux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-06-23 05:13:10.000000 polly-python-0.3.2/tests/test_workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:08:24.615474 polly-python-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-07-21 07:07:10.000000 polly-python-0.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-21 07:07:10.000000 polly-python-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-21 07:08:24.615474 polly-python-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-21 07:07:10.000000 polly-python-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:08:24.615474 polly-python-0.4.0/polly/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14714 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/application_error_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16367 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/bridge_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16238 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31214 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/core_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20886 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35626 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/http_response_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/index_schema_level_conversion_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24441 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   198377 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/omixatlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74348 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/omixatlas_hlpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16510 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/validation_hlpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13003 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:08:24.615474 polly-python-0.4.0/polly_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-21 07:08:24.000000 polly-python-0.4.0/polly_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-21 07:08:24.000000 polly-python-0.4.0/polly_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:08:24.000000 polly-python-0.4.0/polly_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-21 07:08:24.000000 polly-python-0.4.0/polly_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 07:08:24.000000 polly-python-0.4.0/polly_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-21 07:07:10.000000 polly-python-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-21 07:08:24.615474 polly-python-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 07:07:10.000000 polly-python-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:08:24.615474 polly-python-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-07-21 07:07:10.000000 polly-python-0.4.0/tests/test_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-21 07:07:10.000000 polly-python-0.4.0/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-21 07:07:10.000000 polly-python-0.4.0/tests/test_curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-21 07:07:10.000000 polly-python-0.4.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-07-21 07:07:10.000000 polly-python-0.4.0/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98539 2023-07-21 07:07:10.000000 polly-python-0.4.0/tests/test_omixatlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-07-21 07:07:10.000000 polly-python-0.4.0/tests/test_schema_ux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-07-21 07:07:10.000000 polly-python-0.4.0/tests/test_workspaces.py
```

### Comparing `polly-python-0.3.2/LICENSE.md` & `polly-python-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/PKG-INFO` & `polly-python-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polly-python
-Version: 0.3.2
+Version: 0.4.0
 Summary: Polly SDK
 Home-page: https://github.com/ElucidataInc/polly-python
 Project-URL: Documentation, https://docs.elucidata.io
 Project-URL: Tutorial Notebooks, https://github.com/ElucidataInc/polly-python
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `polly-python-0.3.2/README.md` & `polly-python-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/polly/analyze.py` & `polly-python-0.4.0/polly/analyze.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/polly/application_error_info.py` & `polly-python-0.4.0/polly/application_error_info.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/polly/auth.py` & `polly-python-0.4.0/polly/auth.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/polly/bridge_cohort.py` & `polly-python-0.4.0/polly/bridge_cohort.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/polly/cohort.py` & `polly-python-0.4.0/polly/cohort.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/polly/constants.py` & `polly-python-0.4.0/polly/constants.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/polly/core_cohort.py` & `polly-python-0.4.0/polly/core_cohort.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/polly/curation.py` & `polly-python-0.4.0/polly/curation.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/polly/errors.py` & `polly-python-0.4.0/polly/errors.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/polly/help.py` & `polly-python-0.4.0/polly/help.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/polly/helpers.py` & `polly-python-0.4.0/polly/helpers.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/polly/http_response_codes.py` & `polly-python-0.4.0/polly/http_response_codes.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/polly/jobs.py` & `polly-python-0.4.0/polly/jobs.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/polly/omixatlas.py` & `polly-python-0.4.0/polly/omixatlas.py`

 * *Files 0% similar despite different names*

```diff
@@ -2251,14 +2251,15 @@
         """
         try:
             # parameters check
             self._parameter_check_for_add_dataset(
                 repo_id, source_folder_path, destination_folder_path, priority
             )
             if destination_folder_path:
+                omix_hlpr.raise_warning_destination_folder()
                 destination_folder_path = omix_hlpr.normalise_destination_path(
                     self, destination_folder_path, repo_id
                 )
             validation_dataset_lvl = {}
             if validation:
                 validation_dataset_lvl = omix_hlpr.check_status_file(source_folder_path)
             (
@@ -2439,14 +2440,15 @@
             file_status_dict = {}
 
             # check destination folder passed is a valid destination folder
             # or not. If not then raise an error and halt the process
             # If destination_folder_path is empty then it is a valid
             # destination_folder_path -> no need to check for that
             if destination_folder_path:
+                omix_hlpr.raise_warning_destination_folder()
                 self._check_destination_folder(destination_folder_path, repo_id)
 
             # unmapped_file_names (list): data file names which are not mapped
             # unmapped_metadata_file_names (list): metadata file names which are not mapped
             # final_data_metadata_mapping_dict (dict): dict of data metadata mapping
             (
                 final_data_metadata_mapping_dict,
```

### Comparing `polly-python-0.3.2/polly/omixatlas_hlpr.py` & `polly-python-0.4.0/polly/omixatlas_hlpr.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,14 +86,27 @@
     if not (dataset_ids and isinstance(dataset_ids, list)):
         raise paramException(
             title="Param Error",
             detail="dataset_ids should be list of strings",
         )
 
 
+def raise_warning_destination_folder():
+    """Raise warning of deprecation if destination folder used
+
+    Args:
+        destination_folder_path (str): destination folder path for storing files ingested
+    """
+    warnings.formatwarning = lambda msg, *args, **kwargs: f"WARNING: {msg}\n"
+    warnings.warn(
+        "Note:- We are simplifying the storage backend and destination folder will "
+        + "not be required any further. This will be implemented by Jul 31, 2023"
+    )
+
+
 def str_params_check(str_params: list):
     """Checking if string parameters are of valid format
     Args:
         str_params (list): list of string parameters
 
     Raises:
         paramException: Error if any of string parameters are empty or is not str
```

### Comparing `polly-python-0.3.2/polly/schema.py` & `polly-python-0.4.0/polly/schema.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/polly/session.py` & `polly-python-0.4.0/polly/session.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/polly/tracking.py` & `polly-python-0.4.0/polly/tracking.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/polly/validation.py` & `polly-python-0.4.0/polly/validation.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/polly/validation_hlpr.py` & `polly-python-0.4.0/polly/validation_hlpr.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/polly/workspaces.py` & `polly-python-0.4.0/polly/workspaces.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/polly_python.egg-info/PKG-INFO` & `polly-python-0.4.0/polly_python.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polly-python
-Version: 0.3.2
+Version: 0.4.0
 Summary: Polly SDK
 Home-page: https://github.com/ElucidataInc/polly-python
 Project-URL: Documentation, https://docs.elucidata.io
 Project-URL: Tutorial Notebooks, https://github.com/ElucidataInc/polly-python
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `polly-python-0.3.2/polly_python.egg-info/SOURCES.txt` & `polly-python-0.4.0/polly_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/polly_python.egg-info/requires.txt` & `polly-python-0.4.0/polly_python.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/setup.cfg` & `polly-python-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/tests/test_cohort.py` & `polly-python-0.4.0/tests/test_cohort.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/tests/test_constants.py` & `polly-python-0.4.0/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/tests/test_curation.py` & `polly-python-0.4.0/tests/test_curation.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/tests/test_helpers.py` & `polly-python-0.4.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/tests/test_jobs.py` & `polly-python-0.4.0/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/tests/test_omixatlas.py` & `polly-python-0.4.0/tests/test_omixatlas.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/tests/test_schema_ux.py` & `polly-python-0.4.0/tests/test_schema_ux.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.2/tests/test_workspaces.py` & `polly-python-0.4.0/tests/test_workspaces.py`

 * *Files identical despite different names*

