# Comparing `tmp/dagster-duckdb-pandas-0.20.0.tar.gz` & `tmp/dagster-duckdb-pandas-0.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-pandas-0.20.0.tar", last modified: Thu Jul 20 22:02:49 2023, max compression
+gzip compressed data, was "dagster-duckdb-pandas-0.20.1.tar", last modified: Fri Jul 21 15:39:08 2023, max compression
```

## Comparing `dagster-duckdb-pandas-0.20.0.tar` & `dagster-duckdb-pandas-0.20.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:49.722726 dagster-duckdb-pandas-0.20.0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-07-20 21:53:16.000000 dagster-duckdb-pandas-0.20.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-20 21:53:16.000000 dagster-duckdb-pandas-0.20.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      635 2023-07-20 22:02:49.722726 dagster-duckdb-pandas-0.20.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      142 2023-07-20 21:53:16.000000 dagster-duckdb-pandas-0.20.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:49.718726 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas/
--rw-r--r--   0 root         (0) root         (0)      374 2023-07-20 21:53:16.000000 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7168 2023-07-20 21:53:16.000000 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas/duckdb_pandas_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-20 21:53:16.000000 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:49.722726 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      635 2023-07-20 22:02:49.000000 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2023-07-20 22:02:49.000000 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:02:49.000000 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:02:49.000000 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       45 2023-07-20 22:02:49.000000 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-20 22:02:49.000000 dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-20 22:02:49.722726 dagster-duckdb-pandas-0.20.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1328 2023-07-20 21:53:16.000000 dagster-duckdb-pandas-0.20.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:08.819045 dagster-duckdb-pandas-0.20.1/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-21 15:29:00.000000 dagster-duckdb-pandas-0.20.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-21 15:29:00.000000 dagster-duckdb-pandas-0.20.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      635 2023-07-21 15:39:08.819045 dagster-duckdb-pandas-0.20.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      142 2023-07-21 15:29:00.000000 dagster-duckdb-pandas-0.20.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:08.819045 dagster-duckdb-pandas-0.20.1/dagster_duckdb_pandas/
+-rw-r--r--   0 root         (0) root         (0)      374 2023-07-21 15:29:00.000000 dagster-duckdb-pandas-0.20.1/dagster_duckdb_pandas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7168 2023-07-21 15:29:00.000000 dagster-duckdb-pandas-0.20.1/dagster_duckdb_pandas/duckdb_pandas_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-21 15:29:00.000000 dagster-duckdb-pandas-0.20.1/dagster_duckdb_pandas/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-21 15:29:00.000000 dagster-duckdb-pandas-0.20.1/dagster_duckdb_pandas/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:08.819045 dagster-duckdb-pandas-0.20.1/dagster_duckdb_pandas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      635 2023-07-21 15:39:08.000000 dagster-duckdb-pandas-0.20.1/dagster_duckdb_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      466 2023-07-21 15:39:08.000000 dagster-duckdb-pandas-0.20.1/dagster_duckdb_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:39:08.000000 dagster-duckdb-pandas-0.20.1/dagster_duckdb_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:39:08.000000 dagster-duckdb-pandas-0.20.1/dagster_duckdb_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       45 2023-07-21 15:39:08.000000 dagster-duckdb-pandas-0.20.1/dagster_duckdb_pandas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 15:39:08.000000 dagster-duckdb-pandas-0.20.1/dagster_duckdb_pandas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-21 15:39:08.823045 dagster-duckdb-pandas-0.20.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-07-21 15:29:00.000000 dagster-duckdb-pandas-0.20.1/setup.py
```

### Comparing `dagster-duckdb-pandas-0.20.0/LICENSE` & `dagster-duckdb-pandas-0.20.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-pandas-0.20.0/PKG-INFO` & `dagster-duckdb-pandas-0.20.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pandas
-Version: 0.20.0
+Version: 0.20.1
 Summary: Package for storing Pandas DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pandas
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas/duckdb_pandas_type_handler.py` & `dagster-duckdb-pandas-0.20.1/dagster_duckdb_pandas/duckdb_pandas_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-pandas-0.20.0/dagster_duckdb_pandas.egg-info/PKG-INFO` & `dagster-duckdb-pandas-0.20.1/dagster_duckdb_pandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pandas
-Version: 0.20.0
+Version: 0.20.1
 Summary: Package for storing Pandas DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pandas
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-pandas-0.20.0/setup.py` & `dagster-duckdb-pandas-0.20.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,13 +30,13 @@
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_pandas_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.4.0",
-        "dagster-duckdb==0.20.0",
+        "dagster==1.4.1",
+        "dagster-duckdb==0.20.1",
         "pandas",
     ],
     zip_safe=False,
 )
```

