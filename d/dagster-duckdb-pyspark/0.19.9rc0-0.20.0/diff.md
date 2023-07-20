# Comparing `tmp/dagster-duckdb-pyspark-0.19.9rc0.tar.gz` & `tmp/dagster-duckdb-pyspark-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-pyspark-0.19.9rc0.tar", last modified: Thu Jun  8 18:28:36 2023, max compression
+gzip compressed data, was "dagster-duckdb-pyspark-0.20.0.tar", last modified: Thu Jul 20 22:03:56 2023, max compression
```

## Comparing `dagster-duckdb-pyspark-0.19.9rc0.tar` & `dagster-duckdb-pyspark-0.20.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:36.254923 dagster-duckdb-pyspark-0.19.9rc0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-duckdb-pyspark-0.19.9rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       56 2023-06-08 18:20:46.000000 dagster-duckdb-pyspark-0.19.9rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      640 2023-06-08 18:28:36.254923 dagster-duckdb-pyspark-0.19.9rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      152 2023-06-08 18:20:46.000000 dagster-duckdb-pyspark-0.19.9rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:36.246923 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark/
--rw-r--r--   0 root         (0) root         (0)      382 2023-06-08 18:20:46.000000 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7500 2023-06-08 18:20:46.000000 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-08 18:20:46.000000 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark/py.typed
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:36.254923 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark.egg-info/
--rw-r--r--   0 root         (0) root         (0)      640 2023-06-08 18:28:36.000000 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      477 2023-06-08 18:28:36.000000 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:28:36.000000 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:28:36.000000 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      138 2023-06-08 18:28:36.000000 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-08 18:28:36.000000 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      133 2023-06-08 18:28:36.258923 dagster-duckdb-pyspark-0.19.9rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1555 2023-06-08 18:20:46.000000 dagster-duckdb-pyspark-0.19.9rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:03:56.439667 dagster-duckdb-pyspark-0.20.0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-20 21:53:16.000000 dagster-duckdb-pyspark-0.20.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-20 21:53:16.000000 dagster-duckdb-pyspark-0.20.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-20 22:03:56.439667 dagster-duckdb-pyspark-0.20.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      152 2023-07-20 21:53:16.000000 dagster-duckdb-pyspark-0.20.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:03:56.439667 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-07-20 21:53:16.000000 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7980 2023-07-20 21:53:16.000000 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-20 21:53:16.000000 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:03:56.439667 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-20 22:03:56.000000 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      477 2023-07-20 22:03:56.000000 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:03:56.000000 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:03:56.000000 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      138 2023-07-20 22:03:56.000000 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 22:03:56.000000 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      133 2023-07-20 22:03:56.443667 dagster-duckdb-pyspark-0.20.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-07-20 21:53:16.000000 dagster-duckdb-pyspark-0.20.0/setup.py
```

### Comparing `dagster-duckdb-pyspark-0.19.9rc0/LICENSE` & `dagster-duckdb-pyspark-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-pyspark-0.19.9rc0/PKG-INFO` & `dagster-duckdb-pyspark-0.20.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pyspark
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for storing PySpark DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
```

### Comparing `dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py` & `dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 from typing import Optional, Sequence, Type
 
+import pyarrow as pa
 import pyspark
 import pyspark.sql
 from dagster import InputContext, MetadataValue, OutputContext, TableColumn, TableSchema
 from dagster._core.storage.db_io_manager import DbTypeHandler, TableSlice
 from dagster_duckdb.io_manager import (
     DuckDbClient,
     DuckDBIOManager,
     build_duckdb_io_manager,
 )
 from pyspark.sql import SparkSession
 from pyspark.sql.types import StructType
 
 
+def pyspark_df_to_arrow_table(df: pyspark.sql.DataFrame) -> pa.Table:
+    """Converts a PySpark DataFrame to a PyArrow Table."""
+    # `_collect_as_arrow` API call sourced from:
+    #   https://stackoverflow.com/questions/73203318/how-to-transform-spark-dataframe-to-polars-dataframe
+    return pa.Table.from_batches(df._collect_as_arrow())  # noqa: SLF001
+
+
 class DuckDBPySparkTypeHandler(DbTypeHandler[pyspark.sql.DataFrame]):
     """Stores PySpark DataFrames in DuckDB.
 
     To use this type handler, return it from the ``type_handlers` method of an I/O manager that inherits from ``DuckDBIOManager``.
 
     Example:
         .. code-block:: python
@@ -45,23 +53,23 @@
         self,
         context: OutputContext,
         table_slice: TableSlice,
         obj: pyspark.sql.DataFrame,
         connection,
     ):
         """Stores the given object at the provided filepath."""
-        pd_df = obj.toPandas()  # noqa: F841
+        pa_df = pyspark_df_to_arrow_table(obj)  # noqa: F841
         connection.execute(
             f"create table if not exists {table_slice.schema}.{table_slice.table} as select * from"
-            " pd_df;"
+            " pa_df;"
         )
         if not connection.fetchall():
             # table was not created, therefore already exists. Insert the data
             connection.execute(
-                f"insert into {table_slice.schema}.{table_slice.table} select * from pd_df"
+                f"insert into {table_slice.schema}.{table_slice.table} select * from pa_df;"
             )
 
         context.add_output_metadata(
             {
                 "row_count": obj.count(),
                 "dataframe_columns": MetadataValue.table_schema(
                     TableSchema(
@@ -196,14 +204,18 @@
             )
             def my_table_a(my_table: pyspark.sql.DataFrame) -> pyspark.sql.DataFrame:
                 # my_table will just contain the data from column "a"
                 ...
 
     """
 
+    @classmethod
+    def _is_dagster_maintained(cls) -> bool:
+        return True
+
     @staticmethod
     def type_handlers() -> Sequence[DbTypeHandler]:
         return [DuckDBPySparkTypeHandler()]
 
     @staticmethod
     def default_load_type() -> Optional[Type]:
         return pyspark.sql.DataFrame
```

### Comparing `dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark.egg-info/PKG-INFO` & `dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pyspark
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for storing PySpark DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
```

### Comparing `dagster-duckdb-pyspark-0.19.9rc0/setup.py` & `dagster-duckdb-pyspark-0.20.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,26 +20,26 @@
     version=ver,
     author="Elementl",
     author_email="hello@elementl.com",
     license="Apache-2.0",
     description="Package for storing PySpark DataFrames in DuckDB.",
     url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pyspark",
     classifiers=[
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_pyspark_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.3.9rc0",
-        "dagster-duckdb==0.19.9rc0",
+        "dagster==1.4.0",
+        "dagster-duckdb==0.20.0",
         # Pyspark 2.x is incompatible with Python 3.8+
         'pyspark>=3.0.0; python_version >= "3.8"',
         'pyspark>=2.0.2; python_version < "3.8"',
-        "pandas<2",  # See: https://github.com/dagster-io/dagster/issues/13339
+        "pandas",
+        "pyarrow",
     ],
     zip_safe=False,
 )
```

