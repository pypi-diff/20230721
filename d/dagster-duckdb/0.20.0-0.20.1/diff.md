# Comparing `tmp/dagster-duckdb-0.20.0.tar.gz` & `tmp/dagster-duckdb-0.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-0.20.0.tar", last modified: Thu Jul 20 22:03:18 2023, max compression
+gzip compressed data, was "dagster-duckdb-0.20.1.tar", last modified: Fri Jul 21 15:39:05 2023, max compression
```

## Comparing `dagster-duckdb-0.20.0.tar` & `dagster-duckdb-0.20.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:03:18.315128 dagster-duckdb-0.20.0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-07-20 21:53:16.000000 dagster-duckdb-0.20.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       48 2023-07-20 21:53:16.000000 dagster-duckdb-0.20.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-20 22:03:18.315128 dagster-duckdb-0.20.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2023-07-20 21:53:16.000000 dagster-duckdb-0.20.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:03:18.311128 dagster-duckdb-0.20.0/dagster_duckdb/
--rw-r--r--   0 root         (0) root         (0)      336 2023-07-20 21:53:16.000000 dagster-duckdb-0.20.0/dagster_duckdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9554 2023-07-20 21:53:16.000000 dagster-duckdb-0.20.0/dagster_duckdb/io_manager.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-20 21:53:16.000000 dagster-duckdb-0.20.0/dagster_duckdb/py.typed
--rw-r--r--   0 root         (0) root         (0)     1363 2023-07-20 21:53:16.000000 dagster-duckdb-0.20.0/dagster_duckdb/resource.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-duckdb-0.20.0/dagster_duckdb/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:03:18.315128 dagster-duckdb-0.20.0/dagster_duckdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-20 22:03:18.000000 dagster-duckdb-0.20.0/dagster_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      407 2023-07-20 22:03:18.000000 dagster-duckdb-0.20.0/dagster_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:03:18.000000 dagster-duckdb-0.20.0/dagster_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:03:18.000000 dagster-duckdb-0.20.0/dagster_duckdb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-20 22:03:18.000000 dagster-duckdb-0.20.0/dagster_duckdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-20 22:03:18.000000 dagster-duckdb-0.20.0/dagster_duckdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      125 2023-07-20 22:03:18.315128 dagster-duckdb-0.20.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1495 2023-07-20 21:53:16.000000 dagster-duckdb-0.20.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:05.351055 dagster-duckdb-0.20.1/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-21 15:29:00.000000 dagster-duckdb-0.20.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-21 15:29:00.000000 dagster-duckdb-0.20.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-21 15:39:05.351055 dagster-duckdb-0.20.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2023-07-21 15:29:00.000000 dagster-duckdb-0.20.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:05.351055 dagster-duckdb-0.20.1/dagster_duckdb/
+-rw-r--r--   0 root         (0) root         (0)      336 2023-07-21 15:29:00.000000 dagster-duckdb-0.20.1/dagster_duckdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9554 2023-07-21 15:29:00.000000 dagster-duckdb-0.20.1/dagster_duckdb/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-21 15:29:00.000000 dagster-duckdb-0.20.1/dagster_duckdb/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-07-21 15:29:00.000000 dagster-duckdb-0.20.1/dagster_duckdb/resource.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-21 15:29:00.000000 dagster-duckdb-0.20.1/dagster_duckdb/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:05.351055 dagster-duckdb-0.20.1/dagster_duckdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-21 15:39:05.000000 dagster-duckdb-0.20.1/dagster_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      407 2023-07-21 15:39:05.000000 dagster-duckdb-0.20.1/dagster_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:39:05.000000 dagster-duckdb-0.20.1/dagster_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:39:05.000000 dagster-duckdb-0.20.1/dagster_duckdb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-21 15:39:05.000000 dagster-duckdb-0.20.1/dagster_duckdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-21 15:39:05.000000 dagster-duckdb-0.20.1/dagster_duckdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      125 2023-07-21 15:39:05.351055 dagster-duckdb-0.20.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-07-21 15:29:00.000000 dagster-duckdb-0.20.1/setup.py
```

### Comparing `dagster-duckdb-0.20.0/LICENSE` & `dagster-duckdb-0.20.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-0.20.0/PKG-INFO` & `dagster-duckdb-0.20.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb
-Version: 0.20.0
+Version: 0.20.1
 Summary: Package for DuckDB-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-0.20.0/dagster_duckdb/io_manager.py` & `dagster-duckdb-0.20.1/dagster_duckdb/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-0.20.0/dagster_duckdb/resource.py` & `dagster-duckdb-0.20.1/dagster_duckdb/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-0.20.0/dagster_duckdb.egg-info/PKG-INFO` & `dagster-duckdb-0.20.1/dagster_duckdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb
-Version: 0.20.0
+Version: 0.20.1
 Summary: Package for DuckDB-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-0.20.0/setup.py` & `dagster-duckdb-0.20.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_tests*"]),
     include_package_data=True,
     install_requires=[
         "duckdb",
-        "dagster==1.4.0",
+        "dagster==1.4.1",
     ],
     extras_require={
         "pandas": ["pandas"],
         # Pyspark 2.x is incompatible with Python 3.8+
         "pyspark": [
             'pyspark>=3.0.0; python_version >= "3.8"',
             'pyspark>=2.0.2; python_version < "3.8"',
```

