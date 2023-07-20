# Comparing `tmp/dagster-gcp-pandas-0.19.9rc0.tar.gz` & `tmp/dagster-gcp-pandas-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-gcp-pandas-0.19.9rc0.tar", last modified: Thu Jun  8 18:29:52 2023, max compression
+gzip compressed data, was "dagster-gcp-pandas-0.20.0.tar", last modified: Thu Jul 20 22:02:23 2023, max compression
```

## Comparing `dagster-gcp-pandas-0.19.9rc0.tar` & `dagster-gcp-pandas-0.20.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:52.343965 dagster-gcp-pandas-0.19.9rc0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-gcp-pandas-0.19.9rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-08 18:20:46.000000 dagster-gcp-pandas-0.19.9rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      701 2023-06-08 18:29:52.343965 dagster-gcp-pandas-0.19.9rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      140 2023-06-08 18:20:46.000000 dagster-gcp-pandas-0.19.9rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:52.339965 dagster-gcp-pandas-0.19.9rc0/dagster_gcp_pandas/
--rw-r--r--   0 root         (0) root         (0)      394 2023-06-08 18:20:46.000000 dagster-gcp-pandas-0.19.9rc0/dagster_gcp_pandas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:52.343965 dagster-gcp-pandas-0.19.9rc0/dagster_gcp_pandas/bigquery/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:46.000000 dagster-gcp-pandas-0.19.9rc0/dagster_gcp_pandas/bigquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9688 2023-06-08 18:20:46.000000 dagster-gcp-pandas-0.19.9rc0/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-08 18:20:46.000000 dagster-gcp-pandas-0.19.9rc0/dagster_gcp_pandas/py.typed
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-gcp-pandas-0.19.9rc0/dagster_gcp_pandas/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:52.343965 dagster-gcp-pandas-0.19.9rc0/dagster_gcp_pandas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      701 2023-06-08 18:29:52.000000 dagster-gcp-pandas-0.19.9rc0/dagster_gcp_pandas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      487 2023-06-08 18:29:52.000000 dagster-gcp-pandas-0.19.9rc0/dagster_gcp_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:29:52.000000 dagster-gcp-pandas-0.19.9rc0/dagster_gcp_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:29:52.000000 dagster-gcp-pandas-0.19.9rc0/dagster_gcp_pandas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-08 18:29:52.000000 dagster-gcp-pandas-0.19.9rc0/dagster_gcp_pandas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-08 18:29:52.000000 dagster-gcp-pandas-0.19.9rc0/dagster_gcp_pandas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      165 2023-06-08 18:29:52.343965 dagster-gcp-pandas-0.19.9rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1472 2023-06-08 18:20:46.000000 dagster-gcp-pandas-0.19.9rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:23.278374 dagster-gcp-pandas-0.20.0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-20 21:53:16.000000 dagster-gcp-pandas-0.20.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       51 2023-07-20 21:53:16.000000 dagster-gcp-pandas-0.20.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      648 2023-07-20 22:02:23.278374 dagster-gcp-pandas-0.20.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-20 21:53:16.000000 dagster-gcp-pandas-0.20.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:23.278374 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas/
+-rw-r--r--   0 root         (0) root         (0)      394 2023-07-20 21:53:16.000000 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:23.278374 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas/bigquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:16.000000 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9798 2023-07-20 21:53:16.000000 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-20 21:53:16.000000 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:23.278374 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      648 2023-07-20 22:02:23.000000 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      487 2023-07-20 22:02:23.000000 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:02:23.000000 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:02:23.000000 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       61 2023-07-20 22:02:23.000000 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-20 22:02:23.000000 dagster-gcp-pandas-0.20.0/dagster_gcp_pandas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      165 2023-07-20 22:02:23.282374 dagster-gcp-pandas-0.20.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-07-20 21:53:16.000000 dagster-gcp-pandas-0.20.0/setup.py
```

### Comparing `dagster-gcp-pandas-0.19.9rc0/LICENSE` & `dagster-gcp-pandas-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-gcp-pandas-0.19.9rc0/PKG-INFO` & `dagster-gcp-pandas-0.20.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-gcp-pandas
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for storing Pandas DataFrames in GCP.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pandas
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Provides-Extra: test
```

### Comparing `dagster-gcp-pandas-0.19.9rc0/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py` & `dagster-gcp-pandas-0.20.0/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,16 @@
 
         context.add_output_metadata(
             {
                 "row_count": obj.shape[0],
                 "dataframe_columns": MetadataValue.table_schema(
                     TableSchema(
                         columns=[
-                            TableColumn(name=name, type=str(dtype))
-                            for name, dtype in obj.dtypes.iteritems()
+                            TableColumn(name=name, type=str(dtype))  # type: ignore  # (bad stubs)
+                            for name, dtype in obj.dtypes.items()
                         ]
                     )
                 ),
             }
         )
 
     def load_input(
@@ -221,14 +221,18 @@
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
         return [BigQueryPandasTypeHandler()]
 
     @staticmethod
     def default_load_type() -> Optional[Type]:
         return pd.DataFrame
```

### Comparing `dagster-gcp-pandas-0.19.9rc0/dagster_gcp_pandas.egg-info/PKG-INFO` & `dagster-gcp-pandas-0.20.0/dagster_gcp_pandas.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-gcp-pandas
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for storing Pandas DataFrames in GCP.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pandas
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Provides-Extra: test
```

### Comparing `dagster-gcp-pandas-0.19.9rc0/setup.py` & `dagster-gcp-pandas-0.20.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,25 +20,24 @@
     version=ver,
     author="Elementl",
     author_email="hello@elementl.com",
     license="Apache-2.0",
     description="Package for storing Pandas DataFrames in GCP.",
     url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pandas",
     classifiers=[
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_gcp_pandas_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.3.9rc0",
-        "dagster-gcp==0.19.9rc0",
-        "pandas<2",  # See: https://github.com/dagster-io/dagster/issues/13339
+        "dagster==1.4.0",
+        "dagster-gcp==0.20.0",
+        "pandas",
     ],
     extras_require={"test": ["pandas-gbq"]},
     zip_safe=False,
 )
```

