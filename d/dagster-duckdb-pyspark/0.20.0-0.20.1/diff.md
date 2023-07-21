# Comparing `tmp/dagster-duckdb-pyspark-0.20.0.tar.gz` & `tmp/dagster-duckdb-pyspark-0.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-pyspark-0.20.0.tar", last modified: Thu Jul 20 22:03:56 2023, max compression
+gzip compressed data, was "dagster-duckdb-pyspark-0.20.1.tar", last modified: Fri Jul 21 15:36:31 2023, max compression
```

## Comparing `dagster-duckdb-pyspark-0.20.0.tar` & `dagster-duckdb-pyspark-0.20.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:03:56.439667 dagster-duckdb-pyspark-0.20.0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-07-20 21:53:16.000000 dagster-duckdb-pyspark-0.20.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       56 2023-07-20 21:53:16.000000 dagster-duckdb-pyspark-0.20.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-20 22:03:56.439667 dagster-duckdb-pyspark-0.20.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      152 2023-07-20 21:53:16.000000 dagster-duckdb-pyspark-0.20.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:03:56.439667 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark/
--rw-r--r--   0 root         (0) root         (0)      382 2023-07-20 21:53:16.000000 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7980 2023-07-20 21:53:16.000000 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-20 21:53:16.000000 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:03:56.439667 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark.egg-info/
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-20 22:03:56.000000 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      477 2023-07-20 22:03:56.000000 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:03:56.000000 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:03:56.000000 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      138 2023-07-20 22:03:56.000000 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 22:03:56.000000 dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      133 2023-07-20 22:03:56.443667 dagster-duckdb-pyspark-0.20.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1458 2023-07-20 21:53:16.000000 dagster-duckdb-pyspark-0.20.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:36:31.211519 dagster-duckdb-pyspark-0.20.1/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-21 15:29:00.000000 dagster-duckdb-pyspark-0.20.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-21 15:29:00.000000 dagster-duckdb-pyspark-0.20.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-21 15:36:31.211519 dagster-duckdb-pyspark-0.20.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      152 2023-07-21 15:29:00.000000 dagster-duckdb-pyspark-0.20.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:36:31.207519 dagster-duckdb-pyspark-0.20.1/dagster_duckdb_pyspark/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-07-21 15:29:00.000000 dagster-duckdb-pyspark-0.20.1/dagster_duckdb_pyspark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7980 2023-07-21 15:29:00.000000 dagster-duckdb-pyspark-0.20.1/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-21 15:29:00.000000 dagster-duckdb-pyspark-0.20.1/dagster_duckdb_pyspark/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-21 15:29:00.000000 dagster-duckdb-pyspark-0.20.1/dagster_duckdb_pyspark/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:36:31.211519 dagster-duckdb-pyspark-0.20.1/dagster_duckdb_pyspark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-21 15:36:31.000000 dagster-duckdb-pyspark-0.20.1/dagster_duckdb_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      477 2023-07-21 15:36:31.000000 dagster-duckdb-pyspark-0.20.1/dagster_duckdb_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:36:31.000000 dagster-duckdb-pyspark-0.20.1/dagster_duckdb_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:36:31.000000 dagster-duckdb-pyspark-0.20.1/dagster_duckdb_pyspark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      138 2023-07-21 15:36:31.000000 dagster-duckdb-pyspark-0.20.1/dagster_duckdb_pyspark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-21 15:36:31.000000 dagster-duckdb-pyspark-0.20.1/dagster_duckdb_pyspark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      133 2023-07-21 15:36:31.211519 dagster-duckdb-pyspark-0.20.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-07-21 15:29:00.000000 dagster-duckdb-pyspark-0.20.1/setup.py
```

### Comparing `dagster-duckdb-pyspark-0.20.0/LICENSE` & `dagster-duckdb-pyspark-0.20.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-pyspark-0.20.0/PKG-INFO` & `dagster-duckdb-pyspark-0.20.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pyspark
-Version: 0.20.0
+Version: 0.20.1
 Summary: Package for storing PySpark DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py` & `dagster-duckdb-pyspark-0.20.1/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-pyspark-0.20.0/dagster_duckdb_pyspark.egg-info/PKG-INFO` & `dagster-duckdb-pyspark-0.20.1/dagster_duckdb_pyspark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pyspark
-Version: 0.20.0
+Version: 0.20.1
 Summary: Package for storing PySpark DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-pyspark-0.20.0/setup.py` & `dagster-duckdb-pyspark-0.20.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_pyspark_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.4.0",
-        "dagster-duckdb==0.20.0",
+        "dagster==1.4.1",
+        "dagster-duckdb==0.20.1",
         # Pyspark 2.x is incompatible with Python 3.8+
         'pyspark>=3.0.0; python_version >= "3.8"',
         'pyspark>=2.0.2; python_version < "3.8"',
         "pandas",
         "pyarrow",
     ],
     zip_safe=False,
```

