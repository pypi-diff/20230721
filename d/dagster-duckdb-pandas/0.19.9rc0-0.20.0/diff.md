# Comparing `tmp/dagster-duckdb-pandas-0.19.9rc0.tar.gz` & `tmp/dagster-duckdb-pandas-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-pandas-0.19.9rc0.tar", last modified: Thu Jun  8 18:29:48 2023, max compression
+gzip compressed data, was "dagster-duckdb-pandas-0.20.0.tar", last modified: Thu Jul 20 22:02:49 2023, max compression
```

## Comparing `dagster-duckdb-pandas-0.19.9rc0.tar` & `dagster-duckdb-pandas-0.20.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:48.147907 dagster-duckdb-pandas-0.19.9rc0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-duckdb-pandas-0.19.9rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       55 2023-06-08 18:20:46.000000 dagster-duckdb-pandas-0.19.9rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      688 2023-06-08 18:29:48.147907 dagster-duckdb-pandas-0.19.9rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      142 2023-06-08 18:20:46.000000 dagster-duckdb-pandas-0.19.9rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:48.147907 dagster-duckdb-pandas-0.19.9rc0/dagster_duckdb_pandas/
--rw-r--r--   0 root         (0) root         (0)      374 2023-06-08 18:20:46.000000 dagster-duckdb-pandas-0.19.9rc0/dagster_duckdb_pandas/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7058 2023-06-08 18:20:46.000000 dagster-duckdb-pandas-0.19.9rc0/dagster_duckdb_pandas/duckdb_pandas_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-08 18:20:46.000000 dagster-duckdb-pandas-0.19.9rc0/dagster_duckdb_pandas/py.typed
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-duckdb-pandas-0.19.9rc0/dagster_duckdb_pandas/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:48.147907 dagster-duckdb-pandas-0.19.9rc0/dagster_duckdb_pandas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      688 2023-06-08 18:29:48.000000 dagster-duckdb-pandas-0.19.9rc0/dagster_duckdb_pandas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2023-06-08 18:29:48.000000 dagster-duckdb-pandas-0.19.9rc0/dagster_duckdb_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:29:48.000000 dagster-duckdb-pandas-0.19.9rc0/dagster_duckdb_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:29:48.000000 dagster-duckdb-pandas-0.19.9rc0/dagster_duckdb_pandas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-08 18:29:48.000000 dagster-duckdb-pandas-0.19.9rc0/dagster_duckdb_pandas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-08 18:29:48.000000 dagster-duckdb-pandas-0.19.9rc0/dagster_duckdb_pandas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      132 2023-06-08 18:29:48.151908 dagster-duckdb-pandas-0.19.9rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1444 2023-06-08 18:20:46.000000 dagster-duckdb-pandas-0.19.9rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:49.722726 dagster-duckdb-pandas-0.20.0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-20 21:53:16.000000 dagster-duckdb-pandas-0.20.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-20 21:53:16.000000 dagster-duckdb-pandas-0.20.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      635 2023-07-20 22:02:49.722726 dagster-duckdb-pandas-0.20.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      142 2023-07-20 21:53:16.000000 dagster-duckdb-pandas-0.20.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:49.718726 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas/
+-rw-r--r--   0 root         (0) root         (0)      374 2023-07-20 21:53:16.000000 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7168 2023-07-20 21:53:16.000000 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas/duckdb_pandas_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-20 21:53:16.000000 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:49.722726 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      635 2023-07-20 22:02:49.000000 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      466 2023-07-20 22:02:49.000000 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:02:49.000000 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:02:49.000000 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       45 2023-07-20 22:02:49.000000 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-20 22:02:49.000000 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-20 22:02:49.722726 dagster-duckdb-pandas-0.20.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-07-20 21:53:16.000000 dagster-duckdb-pandas-0.20.0/setup.py
```

### Comparing `dagster-duckdb-pandas-0.19.9rc0/LICENSE` & `dagster-duckdb-pandas-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-pandas-0.19.9rc0/PKG-INFO` & `dagster-duckdb-pandas-0.20.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pandas
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for storing Pandas DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pandas
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
 License-File: LICENSE
```

### Comparing `dagster-duckdb-pandas-0.19.9rc0/dagster_duckdb_pandas/duckdb_pandas_type_handler.py` & `dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas/duckdb_pandas_type_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,16 +55,16 @@
 
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
@@ -187,14 +187,18 @@
             )
             def my_table_a(my_table: pd.DataFrame) -> pd.DataFrame:
                 # my_table will just contain the data from column "a"
                 ...
 
     """
 
+    @classmethod
+    def _is_dagster_maintained(cls) -> bool:
+        return True
+
     @staticmethod
     def type_handlers() -> Sequence[DbTypeHandler]:
         return [DuckDBPandasTypeHandler()]
 
     @staticmethod
     def default_load_type() -> Optional[Type]:
         return pd.DataFrame
```

### Comparing `dagster-duckdb-pandas-0.19.9rc0/dagster_duckdb_pandas.egg-info/PKG-INFO` & `dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pandas
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for storing Pandas DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pandas
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
 License-File: LICENSE
```

### Comparing `dagster-duckdb-pandas-0.19.9rc0/setup.py` & `dagster-duckdb-pandas-0.20.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,24 +20,23 @@
     version=ver,
     author="Elementl",
     author_email="hello@elementl.com",
     license="Apache-2.0",
     description="Package for storing Pandas DataFrames in DuckDB.",
     url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pandas",
     classifiers=[
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_pandas_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.3.9rc0",
-        "dagster-duckdb==0.19.9rc0",
-        "pandas<2",  # See: https://github.com/dagster-io/dagster/issues/13339
+        "dagster==1.4.0",
+        "dagster-duckdb==0.20.0",
+        "pandas",
     ],
     zip_safe=False,
 )
```

