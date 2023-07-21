# Comparing `tmp/dagster-gcp-pandas-0.20.0.tar.gz` & `tmp/dagster-gcp-pandas-0.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-gcp-pandas-0.20.0.tar", last modified: Thu Jul 20 22:02:23 2023, max compression
+gzip compressed data, was "dagster-gcp-pandas-0.20.1.tar", last modified: Fri Jul 21 15:36:11 2023, max compression
```

## Comparing `dagster-gcp-pandas-0.20.0.tar` & `dagster-gcp-pandas-0.20.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:23.278374 dagster-gcp-pandas-0.20.0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-07-20 21:53:16.000000 dagster-gcp-pandas-0.20.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       51 2023-07-20 21:53:16.000000 dagster-gcp-pandas-0.20.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      648 2023-07-20 22:02:23.278374 dagster-gcp-pandas-0.20.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      140 2023-07-20 21:53:16.000000 dagster-gcp-pandas-0.20.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:23.278374 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas/
--rw-r--r--   0 root         (0) root         (0)      394 2023-07-20 21:53:16.000000 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:23.278374 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas/bigquery/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:16.000000 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas/bigquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9798 2023-07-20 21:53:16.000000 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-20 21:53:16.000000 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:23.278374 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      648 2023-07-20 22:02:23.000000 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      487 2023-07-20 22:02:23.000000 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:02:23.000000 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:02:23.000000 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       61 2023-07-20 22:02:23.000000 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-20 22:02:23.000000 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      165 2023-07-20 22:02:23.282374 dagster-gcp-pandas-0.20.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1356 2023-07-20 21:53:16.000000 dagster-gcp-pandas-0.20.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:36:11.579577 dagster-gcp-pandas-0.20.1/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-21 15:29:00.000000 dagster-gcp-pandas-0.20.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       51 2023-07-21 15:29:00.000000 dagster-gcp-pandas-0.20.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      648 2023-07-21 15:36:11.579577 dagster-gcp-pandas-0.20.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-21 15:29:00.000000 dagster-gcp-pandas-0.20.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:36:11.575577 dagster-gcp-pandas-0.20.1/dagster_gcp_pandas/
+-rw-r--r--   0 root         (0) root         (0)      394 2023-07-21 15:29:00.000000 dagster-gcp-pandas-0.20.1/dagster_gcp_pandas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:36:11.575577 dagster-gcp-pandas-0.20.1/dagster_gcp_pandas/bigquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 15:29:00.000000 dagster-gcp-pandas-0.20.1/dagster_gcp_pandas/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9798 2023-07-21 15:29:00.000000 dagster-gcp-pandas-0.20.1/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-21 15:29:00.000000 dagster-gcp-pandas-0.20.1/dagster_gcp_pandas/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-21 15:29:00.000000 dagster-gcp-pandas-0.20.1/dagster_gcp_pandas/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:36:11.575577 dagster-gcp-pandas-0.20.1/dagster_gcp_pandas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      648 2023-07-21 15:36:11.000000 dagster-gcp-pandas-0.20.1/dagster_gcp_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      487 2023-07-21 15:36:11.000000 dagster-gcp-pandas-0.20.1/dagster_gcp_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:36:11.000000 dagster-gcp-pandas-0.20.1/dagster_gcp_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:36:11.000000 dagster-gcp-pandas-0.20.1/dagster_gcp_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       61 2023-07-21 15:36:11.000000 dagster-gcp-pandas-0.20.1/dagster_gcp_pandas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-21 15:36:11.000000 dagster-gcp-pandas-0.20.1/dagster_gcp_pandas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      165 2023-07-21 15:36:11.579577 dagster-gcp-pandas-0.20.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-07-21 15:29:00.000000 dagster-gcp-pandas-0.20.1/setup.py
```

### Comparing `dagster-gcp-pandas-0.20.0/LICENSE` & `dagster-gcp-pandas-0.20.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-gcp-pandas-0.20.0/PKG-INFO` & `dagster-gcp-pandas-0.20.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-gcp-pandas
-Version: 0.20.0
+Version: 0.20.1
 Summary: Package for storing Pandas DataFrames in GCP.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pandas
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-gcp-pandas-0.20.0/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py` & `dagster-gcp-pandas-0.20.1/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-pandas-0.20.0/dagster_gcp_pandas.egg-info/PKG-INFO` & `dagster-gcp-pandas-0.20.1/dagster_gcp_pandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-gcp-pandas
-Version: 0.20.0
+Version: 0.20.1
 Summary: Package for storing Pandas DataFrames in GCP.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pandas
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-gcp-pandas-0.20.0/setup.py` & `dagster-gcp-pandas-0.20.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,14 @@
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_gcp_pandas_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.4.0",
-        "dagster-gcp==0.20.0",
+        "dagster==1.4.1",
+        "dagster-gcp==0.20.1",
         "pandas",
     ],
     extras_require={"test": ["pandas-gbq"]},
     zip_safe=False,
 )
```

