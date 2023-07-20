# Comparing `tmp/dagster_gcp_pyspark-0.19.9rc0.tar.gz` & `tmp/dagster_gcp_pyspark-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_gcp_pyspark-0.19.9rc0.tar", last modified: Thu Jun  8 18:30:05 2023, max compression
+gzip compressed data, was "dagster_gcp_pyspark-0.20.0.tar", last modified: Thu Jul 20 22:04:17 2023, max compression
```

## Comparing `dagster_gcp_pyspark-0.19.9rc0.tar` & `dagster_gcp_pyspark-0.20.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:30:05.884151 dagster_gcp_pyspark-0.19.9rc0/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-06-08 18:20:46.000000 dagster_gcp_pyspark-0.19.9rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-08 18:20:46.000000 dagster_gcp_pyspark-0.19.9rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      652 2023-06-08 18:30:05.884151 dagster_gcp_pyspark-0.19.9rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      143 2023-06-08 18:20:46.000000 dagster_gcp_pyspark-0.19.9rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:30:05.876151 dagster_gcp_pyspark-0.19.9rc0/dagster_gcp_pyspark/
--rw-r--r--   0 root         (0) root         (0)      402 2023-06-08 18:20:46.000000 dagster_gcp_pyspark-0.19.9rc0/dagster_gcp_pyspark/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:30:05.884151 dagster_gcp_pyspark-0.19.9rc0/dagster_gcp_pyspark/bigquery/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:46.000000 dagster_gcp_pyspark-0.19.9rc0/dagster_gcp_pyspark/bigquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9900 2023-06-08 18:20:46.000000 dagster_gcp_pyspark-0.19.9rc0/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-08 18:20:46.000000 dagster_gcp_pyspark-0.19.9rc0/dagster_gcp_pyspark/py.typed
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster_gcp_pyspark-0.19.9rc0/dagster_gcp_pyspark/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:30:05.884151 dagster_gcp_pyspark-0.19.9rc0/dagster_gcp_pyspark.egg-info/
--rw-r--r--   0 root         (0) root         (0)      652 2023-06-08 18:30:05.000000 dagster_gcp_pyspark-0.19.9rc0/dagster_gcp_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2023-06-08 18:30:05.000000 dagster_gcp_pyspark-0.19.9rc0/dagster_gcp_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:30:05.000000 dagster_gcp_pyspark-0.19.9rc0/dagster_gcp_pyspark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:30:05.000000 dagster_gcp_pyspark-0.19.9rc0/dagster_gcp_pyspark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       68 2023-06-08 18:30:05.000000 dagster_gcp_pyspark-0.19.9rc0/dagster_gcp_pyspark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-08 18:30:05.000000 dagster_gcp_pyspark-0.19.9rc0/dagster_gcp_pyspark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      166 2023-06-08 18:30:05.884151 dagster_gcp_pyspark-0.19.9rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1372 2023-06-08 18:20:46.000000 dagster_gcp_pyspark-0.19.9rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:17.975976 dagster_gcp_pyspark-0.20.0/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-07-20 21:53:16.000000 dagster_gcp_pyspark-0.20.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       52 2023-07-20 21:53:16.000000 dagster_gcp_pyspark-0.20.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      599 2023-07-20 22:04:17.975976 dagster_gcp_pyspark-0.20.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      143 2023-07-20 21:53:16.000000 dagster_gcp_pyspark-0.20.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:17.967976 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark/
+-rw-r--r--   0 root         (0) root         (0)      402 2023-07-20 21:53:16.000000 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:17.967976 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark/bigquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:16.000000 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9983 2023-07-20 21:53:16.000000 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-20 21:53:16.000000 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:17.967976 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      599 2023-07-20 22:04:17.000000 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-20 22:04:17.000000 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:04:17.000000 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:04:17.000000 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-20 22:04:17.000000 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-20 22:04:17.000000 dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2023-07-20 22:04:17.975976 dagster_gcp_pyspark-0.20.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-07-20 21:53:16.000000 dagster_gcp_pyspark-0.20.0/setup.py
```

### Comparing `dagster_gcp_pyspark-0.19.9rc0/LICENSE` & `dagster_gcp_pyspark-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster_gcp_pyspark-0.19.9rc0/PKG-INFO` & `dagster_gcp_pyspark-0.20.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster_gcp_pyspark
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for storing PySpark DataFrames in GCP
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `dagster_gcp_pyspark-0.19.9rc0/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py` & `dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,14 +228,18 @@
         Dagster will store this key in a temporary file and set GOOGLE_APPLICATION_CREDENTIALS to point to the file.
         After the run completes, the file will be deleted, and GOOGLE_APPLICATION_CREDENTIALS will be
         unset. The key must be base64 encoded to avoid issues with newlines in the keys. You can retrieve
         the base64 encoded key with this shell command: cat $GOOGLE_APPLICATION_CREDENTIALS | base64
 
     """
 
+    @classmethod
+    def _is_dagster_maintained(cls) -> bool:
+        return True
+
     @staticmethod
     def type_handlers() -> Sequence[DbTypeHandler]:
         return [BigQueryPySparkTypeHandler()]
 
     @staticmethod
     def default_load_type() -> Optional[Type]:
         return DataFrame
```

### Comparing `dagster_gcp_pyspark-0.19.9rc0/dagster_gcp_pyspark.egg-info/PKG-INFO` & `dagster_gcp_pyspark-0.20.0/dagster_gcp_pyspark.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-gcp-pyspark
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for storing PySpark DataFrames in GCP
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `dagster_gcp_pyspark-0.19.9rc0/setup.py` & `dagster_gcp_pyspark-0.20.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,23 +23,22 @@
     license="Apache-2.0",
     description="Package for storing PySpark DataFrames in GCP",
     url=(
         "https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/"
         "dagster-gcp-pyspark"
     ),
     classifiers=[
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_gcp_pyspark_tests*"]),
     install_requires=[
-        "dagster==1.3.9rc0",
-        "dagster-gcp==0.19.9rc0",
+        "dagster==1.4.0",
+        "dagster-gcp==0.20.0",
         "pyspark",
     ],
     extras_require={"test": ["pandas-gbq"]},
     zip_safe=False,
 )
```

