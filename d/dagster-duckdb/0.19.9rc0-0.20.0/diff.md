# Comparing `tmp/dagster-duckdb-0.19.9rc0.tar.gz` & `tmp/dagster-duckdb-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-0.19.9rc0.tar", last modified: Thu Jun  8 18:28:18 2023, max compression
+gzip compressed data, was "dagster-duckdb-0.20.0.tar", last modified: Thu Jul 20 22:03:18 2023, max compression
```

## Comparing `dagster-duckdb-0.19.9rc0.tar` & `dagster-duckdb-0.20.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:18.362675 dagster-duckdb-0.19.9rc0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-duckdb-0.19.9rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       48 2023-06-08 18:20:46.000000 dagster-duckdb-0.19.9rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      695 2023-06-08 18:28:18.362675 dagster-duckdb-0.19.9rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2023-06-08 18:20:46.000000 dagster-duckdb-0.19.9rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:18.362675 dagster-duckdb-0.19.9rc0/dagster_duckdb/
--rw-r--r--   0 root         (0) root         (0)      336 2023-06-08 18:20:46.000000 dagster-duckdb-0.19.9rc0/dagster_duckdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9444 2023-06-08 18:20:46.000000 dagster-duckdb-0.19.9rc0/dagster_duckdb/io_manager.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-08 18:20:46.000000 dagster-duckdb-0.19.9rc0/dagster_duckdb/py.typed
--rw-r--r--   0 root         (0) root         (0)     1280 2023-06-08 18:20:46.000000 dagster-duckdb-0.19.9rc0/dagster_duckdb/resource.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-duckdb-0.19.9rc0/dagster_duckdb/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:18.362675 dagster-duckdb-0.19.9rc0/dagster_duckdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      695 2023-06-08 18:28:18.000000 dagster-duckdb-0.19.9rc0/dagster_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      407 2023-06-08 18:28:18.000000 dagster-duckdb-0.19.9rc0/dagster_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:28:18.000000 dagster-duckdb-0.19.9rc0/dagster_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:28:18.000000 dagster-duckdb-0.19.9rc0/dagster_duckdb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      152 2023-06-08 18:28:18.000000 dagster-duckdb-0.19.9rc0/dagster_duckdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-08 18:28:18.000000 dagster-duckdb-0.19.9rc0/dagster_duckdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      125 2023-06-08 18:28:18.366675 dagster-duckdb-0.19.9rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1547 2023-06-08 18:20:46.000000 dagster-duckdb-0.19.9rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:03:18.315128 dagster-duckdb-0.20.0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-20 21:53:16.000000 dagster-duckdb-0.20.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-20 21:53:16.000000 dagster-duckdb-0.20.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-20 22:03:18.315128 dagster-duckdb-0.20.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2023-07-20 21:53:16.000000 dagster-duckdb-0.20.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:03:18.311128 dagster-duckdb-0.20.0/dagster_duckdb/
+-rw-r--r--   0 root         (0) root         (0)      336 2023-07-20 21:53:16.000000 dagster-duckdb-0.20.0/dagster_duckdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9554 2023-07-20 21:53:16.000000 dagster-duckdb-0.20.0/dagster_duckdb/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-20 21:53:16.000000 dagster-duckdb-0.20.0/dagster_duckdb/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-07-20 21:53:16.000000 dagster-duckdb-0.20.0/dagster_duckdb/resource.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-duckdb-0.20.0/dagster_duckdb/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:03:18.315128 dagster-duckdb-0.20.0/dagster_duckdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-20 22:03:18.000000 dagster-duckdb-0.20.0/dagster_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      407 2023-07-20 22:03:18.000000 dagster-duckdb-0.20.0/dagster_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:03:18.000000 dagster-duckdb-0.20.0/dagster_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:03:18.000000 dagster-duckdb-0.20.0/dagster_duckdb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-20 22:03:18.000000 dagster-duckdb-0.20.0/dagster_duckdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-20 22:03:18.000000 dagster-duckdb-0.20.0/dagster_duckdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      125 2023-07-20 22:03:18.315128 dagster-duckdb-0.20.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-07-20 21:53:16.000000 dagster-duckdb-0.20.0/setup.py
```

### Comparing `dagster-duckdb-0.19.9rc0/LICENSE` & `dagster-duckdb-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-0.19.9rc0/PKG-INFO` & `dagster-duckdb-0.20.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for DuckDB-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Provides-Extra: pandas
 Provides-Extra: pyspark
```

### Comparing `dagster-duckdb-0.19.9rc0/dagster_duckdb/io_manager.py` & `dagster-duckdb-0.20.0/dagster_duckdb/io_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from dagster._core.storage.db_io_manager import (
     DbClient,
     DbIOManager,
     DbTypeHandler,
     TablePartitionDimension,
     TableSlice,
 )
+from dagster._core.storage.io_manager import dagster_maintained_io_manager
 from dagster._utils.backoff import backoff
 from pydantic import Field
 
 DUCKDB_DATETIME_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 def build_duckdb_io_manager(
@@ -79,14 +80,15 @@
         )
         def my_table_a(my_table: pd.DataFrame):
             # my_table will just contain the data from column "a"
             ...
 
     """
 
+    @dagster_maintained_io_manager
     @io_manager(config_schema=DuckDBIOManager.to_config_schema())
     def duckdb_io_manager(init_context):
         """IO Manager for storing outputs in a DuckDB database.
 
         Assets will be stored in the schema and table name specified by their AssetKey.
         Subsequent materializations of an asset will overwrite previous materializations of that asset.
         Op outputs will be stored in the schema specified by output metadata (defaults to public) in a
```

### Comparing `dagster-duckdb-0.19.9rc0/dagster_duckdb/resource.py` & `dagster-duckdb-0.20.0/dagster_duckdb/resource.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     database: str = Field(
         description=(
             "Path to the DuckDB database. Setting database=':memory:' will use an in-memory"
             " database "
         )
     )
 
+    @classmethod
+    def _is_dagster_maintained(cls) -> bool:
+        return True
+
     @contextmanager
     def get_connection(self):
         conn = backoff(
             fn=duckdb.connect,
             retry_on=(RuntimeError, duckdb.IOException),
             kwargs={"database": self.database, "read_only": False},
             max_retries=10,
```

### Comparing `dagster-duckdb-0.19.9rc0/dagster_duckdb.egg-info/PKG-INFO` & `dagster-duckdb-0.20.0/dagster_duckdb.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for DuckDB-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Provides-Extra: pandas
 Provides-Extra: pyspark
```

### Comparing `dagster-duckdb-0.19.9rc0/setup.py` & `dagster-duckdb-0.20.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -20,26 +20,25 @@
     version=ver,
     author="Elementl",
     author_email="hello@elementl.com",
     license="Apache-2.0",
     description="Package for DuckDB-specific Dagster framework op and resource components.",
     url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb",
     classifiers=[
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_tests*"]),
     include_package_data=True,
     install_requires=[
         "duckdb",
-        "dagster==1.3.9rc0",
+        "dagster==1.4.0",
     ],
     extras_require={
         "pandas": ["pandas"],
         # Pyspark 2.x is incompatible with Python 3.8+
         "pyspark": [
             'pyspark>=3.0.0; python_version >= "3.8"',
             'pyspark>=2.0.2; python_version < "3.8"',
```

