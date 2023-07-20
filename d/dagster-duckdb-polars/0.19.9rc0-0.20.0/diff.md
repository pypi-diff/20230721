# Comparing `tmp/dagster-duckdb-polars-0.19.9rc0.tar.gz` & `tmp/dagster-duckdb-polars-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-polars-0.19.9rc0.tar", last modified: Thu Jun  8 18:29:01 2023, max compression
+gzip compressed data, was "dagster-duckdb-polars-0.20.0.tar", last modified: Thu Jul 20 22:04:22 2023, max compression
```

## Comparing `dagster-duckdb-polars-0.19.9rc0.tar` & `dagster-duckdb-polars-0.20.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:01.875264 dagster-duckdb-polars-0.19.9rc0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-duckdb-polars-0.19.9rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       55 2023-06-08 18:20:46.000000 dagster-duckdb-polars-0.19.9rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      688 2023-06-08 18:29:01.875264 dagster-duckdb-polars-0.19.9rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      149 2023-06-08 18:20:46.000000 dagster-duckdb-polars-0.19.9rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:01.871264 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars/
--rw-r--r--   0 root         (0) root         (0)      374 2023-06-08 18:20:46.000000 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7372 2023-06-08 18:20:46.000000 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars/duckdb_polars_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-08 18:20:46.000000 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars/py.typed
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:01.875264 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars.egg-info/
--rw-r--r--   0 root         (0) root         (0)      688 2023-06-08 18:29:01.000000 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2023-06-08 18:29:01.000000 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:29:01.000000 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:29:01.000000 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-08 18:29:01.000000 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-08 18:29:01.000000 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      132 2023-06-08 18:29:01.875264 dagster-duckdb-polars-0.19.9rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1392 2023-06-08 18:20:46.000000 dagster-duckdb-polars-0.19.9rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:22.040035 dagster-duckdb-polars-0.20.0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-20 21:53:16.000000 dagster-duckdb-polars-0.20.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-20 21:53:16.000000 dagster-duckdb-polars-0.20.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      636 2023-07-20 22:04:22.040035 dagster-duckdb-polars-0.20.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-20 21:53:16.000000 dagster-duckdb-polars-0.20.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:22.040035 dagster-duckdb-polars-0.20.0/dagster_duckdb_polars/
+-rw-r--r--   0 root         (0) root         (0)      374 2023-07-20 21:53:16.000000 dagster-duckdb-polars-0.20.0/dagster_duckdb_polars/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7455 2023-07-20 21:53:16.000000 dagster-duckdb-polars-0.20.0/dagster_duckdb_polars/duckdb_polars_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-20 21:53:16.000000 dagster-duckdb-polars-0.20.0/dagster_duckdb_polars/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-duckdb-polars-0.20.0/dagster_duckdb_polars/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:22.040035 dagster-duckdb-polars-0.20.0/dagster_duckdb_polars.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      636 2023-07-20 22:04:21.000000 dagster-duckdb-polars-0.20.0/dagster_duckdb_polars.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      466 2023-07-20 22:04:21.000000 dagster-duckdb-polars-0.20.0/dagster_duckdb_polars.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:04:21.000000 dagster-duckdb-polars-0.20.0/dagster_duckdb_polars.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:04:21.000000 dagster-duckdb-polars-0.20.0/dagster_duckdb_polars.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       54 2023-07-20 22:04:21.000000 dagster-duckdb-polars-0.20.0/dagster_duckdb_polars.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-20 22:04:21.000000 dagster-duckdb-polars-0.20.0/dagster_duckdb_polars.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-20 22:04:22.040035 dagster-duckdb-polars-0.20.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1338 2023-07-20 21:53:16.000000 dagster-duckdb-polars-0.20.0/setup.py
```

### Comparing `dagster-duckdb-polars-0.19.9rc0/LICENSE` & `dagster-duckdb-polars-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-polars-0.19.9rc0/PKG-INFO` & `dagster-duckdb-polars-0.20.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-polars
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for storing Polars DataFrames in DuckDB.
-Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-polars
+Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckdb-polars
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

### Comparing `dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars/duckdb_polars_type_handler.py` & `dagster-duckdb-polars-0.20.0/dagster_duckdb_polars/duckdb_polars_type_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,14 +189,18 @@
             )
             def my_table_a(my_table: pl.DataFrame) -> pl.DataFrame:
                 # my_table will just contain the data from column "a"
                 ...
 
     """
 
+    @classmethod
+    def _is_dagster_maintained(cls) -> bool:
+        return True
+
     @staticmethod
     def type_handlers() -> Sequence[DbTypeHandler]:
         return [DuckDBPolarsTypeHandler()]
 
     @staticmethod
     def default_load_type() -> Optional[Type]:
         return pl.DataFrame
```

### Comparing `dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars.egg-info/PKG-INFO` & `dagster-duckdb-polars-0.20.0/dagster_duckdb_polars.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-polars
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for storing Polars DataFrames in DuckDB.
-Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-polars
+Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckdb-polars
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

### Comparing `dagster-duckdb-polars-0.19.9rc0/setup.py` & `dagster-duckdb-polars-0.20.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,26 +18,25 @@
 setup(
     name="dagster-duckdb-polars",
     version=ver,
     author="Elementl",
     author_email="hello@elementl.com",
     license="Apache-2.0",
     description="Package for storing Polars DataFrames in DuckDB.",
-    url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-polars",
+    url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckdb-polars",
     classifiers=[
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_polars_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.3.9rc0",
-        "dagster-duckdb==0.19.9rc0",
+        "dagster==1.4.0",
+        "dagster-duckdb==0.20.0",
         "polars[pyarrow]",
     ],
     zip_safe=False,
 )
```

