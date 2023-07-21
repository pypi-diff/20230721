# Comparing `tmp/dagster_gcp_pyspark-0.20.0.tar.gz` & `tmp/dagster_gcp_pyspark-0.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_gcp_pyspark-0.20.0.tar", last modified: Thu Jul 20 22:04:17 2023, max compression
+gzip compressed data, was "dagster_gcp_pyspark-0.20.1.tar", last modified: Fri Jul 21 15:36:34 2023, max compression
```

## Comparing `dagster_gcp_pyspark-0.20.0.tar` & `dagster_gcp_pyspark-0.20.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:17.975976 dagster_gcp_pyspark-0.20.0/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-07-20 21:53:16.000000 dagster_gcp_pyspark-0.20.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       52 2023-07-20 21:53:16.000000 dagster_gcp_pyspark-0.20.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      599 2023-07-20 22:04:17.975976 dagster_gcp_pyspark-0.20.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      143 2023-07-20 21:53:16.000000 dagster_gcp_pyspark-0.20.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:17.967976 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark/
--rw-r--r--   0 root         (0) root         (0)      402 2023-07-20 21:53:16.000000 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:17.967976 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark/bigquery/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:16.000000 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark/bigquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9983 2023-07-20 21:53:16.000000 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-20 21:53:16.000000 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:17.967976 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark.egg-info/
--rw-r--r--   0 root         (0) root         (0)      599 2023-07-20 22:04:17.000000 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2023-07-20 22:04:17.000000 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:04:17.000000 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:04:17.000000 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-20 22:04:17.000000 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-20 22:04:17.000000 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      166 2023-07-20 22:04:17.975976 dagster_gcp_pyspark-0.20.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1317 2023-07-20 21:53:16.000000 dagster_gcp_pyspark-0.20.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:36:34.623508 dagster_gcp_pyspark-0.20.1/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-07-21 15:29:00.000000 dagster_gcp_pyspark-0.20.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       52 2023-07-21 15:29:00.000000 dagster_gcp_pyspark-0.20.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      599 2023-07-21 15:36:34.623508 dagster_gcp_pyspark-0.20.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      143 2023-07-21 15:29:00.000000 dagster_gcp_pyspark-0.20.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:36:34.619508 dagster_gcp_pyspark-0.20.1/dagster_gcp_pyspark/
+-rw-r--r--   0 root         (0) root         (0)      402 2023-07-21 15:29:00.000000 dagster_gcp_pyspark-0.20.1/dagster_gcp_pyspark/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:36:34.619508 dagster_gcp_pyspark-0.20.1/dagster_gcp_pyspark/bigquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 15:29:00.000000 dagster_gcp_pyspark-0.20.1/dagster_gcp_pyspark/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9983 2023-07-21 15:29:00.000000 dagster_gcp_pyspark-0.20.1/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-21 15:29:00.000000 dagster_gcp_pyspark-0.20.1/dagster_gcp_pyspark/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-21 15:29:00.000000 dagster_gcp_pyspark-0.20.1/dagster_gcp_pyspark/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:36:34.619508 dagster_gcp_pyspark-0.20.1/dagster_gcp_pyspark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      599 2023-07-21 15:36:34.000000 dagster_gcp_pyspark-0.20.1/dagster_gcp_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-21 15:36:34.000000 dagster_gcp_pyspark-0.20.1/dagster_gcp_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:36:34.000000 dagster_gcp_pyspark-0.20.1/dagster_gcp_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:36:34.000000 dagster_gcp_pyspark-0.20.1/dagster_gcp_pyspark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-21 15:36:34.000000 dagster_gcp_pyspark-0.20.1/dagster_gcp_pyspark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-21 15:36:34.000000 dagster_gcp_pyspark-0.20.1/dagster_gcp_pyspark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2023-07-21 15:36:34.623508 dagster_gcp_pyspark-0.20.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-07-21 15:29:00.000000 dagster_gcp_pyspark-0.20.1/setup.py
```

### Comparing `dagster_gcp_pyspark-0.20.0/LICENSE` & `dagster_gcp_pyspark-0.20.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster_gcp_pyspark-0.20.0/PKG-INFO` & `dagster_gcp_pyspark-0.20.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster_gcp_pyspark
-Version: 0.20.0
+Version: 0.20.1
 Summary: Package for storing PySpark DataFrames in GCP
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py` & `dagster_gcp_pyspark-0.20.1/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark.egg-info/PKG-INFO` & `dagster_gcp_pyspark-0.20.1/dagster_gcp_pyspark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-gcp-pyspark
-Version: 0.20.0
+Version: 0.20.1
 Summary: Package for storing PySpark DataFrames in GCP
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster_gcp_pyspark-0.20.0/setup.py` & `dagster_gcp_pyspark-0.20.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,14 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_gcp_pyspark_tests*"]),
     install_requires=[
-        "dagster==1.4.0",
-        "dagster-gcp==0.20.0",
+        "dagster==1.4.1",
+        "dagster-gcp==0.20.1",
         "pyspark",
     ],
     extras_require={"test": ["pandas-gbq"]},
     zip_safe=False,
 )
```

