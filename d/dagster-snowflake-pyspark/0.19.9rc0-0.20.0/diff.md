# Comparing `tmp/dagster-snowflake-pyspark-0.19.9rc0.tar.gz` & `tmp/dagster-snowflake-pyspark-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-snowflake-pyspark-0.19.9rc0.tar", last modified: Thu Jun  8 18:29:06 2023, max compression
+gzip compressed data, was "dagster-snowflake-pyspark-0.20.0.tar", last modified: Thu Jul 20 22:03:06 2023, max compression
```

## Comparing `dagster-snowflake-pyspark-0.19.9rc0.tar` & `dagster-snowflake-pyspark-0.20.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:06.655329 dagster-snowflake-pyspark-0.19.9rc0/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-08 18:20:46.000000 dagster-snowflake-pyspark-0.19.9rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       77 2023-06-08 18:20:46.000000 dagster-snowflake-pyspark-0.19.9rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      657 2023-06-08 18:29:06.655329 dagster-snowflake-pyspark-0.19.9rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      161 2023-06-08 18:20:46.000000 dagster-snowflake-pyspark-0.19.9rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:06.655329 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark/
--rw-r--r--   0 root         (0) root         (0)      421 2023-06-08 18:20:46.000000 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark/__init__.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 18:20:46.000000 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark/py.typed
--rw-r--r--   0 root         (0) root         (0)     9162 2023-06-08 18:20:46.000000 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark/snowflake_pyspark_type_handler.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:06.655329 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark.egg-info/
--rw-r--r--   0 root         (0) root         (0)      657 2023-06-08 18:29:06.000000 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      510 2023-06-08 18:29:06.000000 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:29:06.000000 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:29:06.000000 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-08 18:29:06.000000 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:29:06.000000 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-06-08 18:29:06.655329 dagster-snowflake-pyspark-0.19.9rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1516 2023-06-08 18:20:46.000000 dagster-snowflake-pyspark-0.19.9rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:03:06.322959 dagster-snowflake-pyspark-0.20.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-20 21:53:16.000000 dagster-snowflake-pyspark-0.20.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       77 2023-07-20 21:53:16.000000 dagster-snowflake-pyspark-0.20.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      604 2023-07-20 22:03:06.322959 dagster-snowflake-pyspark-0.20.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      161 2023-07-20 21:53:16.000000 dagster-snowflake-pyspark-0.20.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:03:06.318959 dagster-snowflake-pyspark-0.20.0/dagster_snowflake_pyspark/
+-rw-r--r--   0 root         (0) root         (0)      421 2023-07-20 21:53:16.000000 dagster-snowflake-pyspark-0.20.0/dagster_snowflake_pyspark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-20 21:53:16.000000 dagster-snowflake-pyspark-0.20.0/dagster_snowflake_pyspark/py.typed
+-rw-r--r--   0 root         (0) root         (0)     9245 2023-07-20 21:53:16.000000 dagster-snowflake-pyspark-0.20.0/dagster_snowflake_pyspark/snowflake_pyspark_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-snowflake-pyspark-0.20.0/dagster_snowflake_pyspark/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:03:06.322959 dagster-snowflake-pyspark-0.20.0/dagster_snowflake_pyspark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-07-20 22:03:06.000000 dagster-snowflake-pyspark-0.20.0/dagster_snowflake_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      510 2023-07-20 22:03:06.000000 dagster-snowflake-pyspark-0.20.0/dagster_snowflake_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:03:06.000000 dagster-snowflake-pyspark-0.20.0/dagster_snowflake_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:03:06.000000 dagster-snowflake-pyspark-0.20.0/dagster_snowflake_pyspark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-20 22:03:06.000000 dagster-snowflake-pyspark-0.20.0/dagster_snowflake_pyspark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-20 22:03:06.000000 dagster-snowflake-pyspark-0.20.0/dagster_snowflake_pyspark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-20 22:03:06.322959 dagster-snowflake-pyspark-0.20.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-07-20 21:53:16.000000 dagster-snowflake-pyspark-0.20.0/setup.py
```

### Comparing `dagster-snowflake-pyspark-0.19.9rc0/LICENSE` & `dagster-snowflake-pyspark-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-snowflake-pyspark-0.19.9rc0/PKG-INFO` & `dagster-snowflake-pyspark-0.20.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: dagster-snowflake-pyspark
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for integrating Snowflake and PySpark with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pyspark
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

### Comparing `dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark/snowflake_pyspark_type_handler.py` & `dagster-snowflake-pyspark-0.20.0/dagster_snowflake_pyspark/snowflake_pyspark_type_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,14 +232,18 @@
             )
             def my_table_a(my_table: DataFrame) -> DataFrame:
                 # my_table will just contain the data from column "a"
                 ...
 
     """
 
+    @classmethod
+    def _is_dagster_maintained(cls) -> bool:
+        return True
+
     @staticmethod
     def type_handlers() -> Sequence[DbTypeHandler]:
         return [SnowflakePySparkTypeHandler()]
 
     @staticmethod
     def default_load_type() -> Optional[Type]:
         return DataFrame
```

### Comparing `dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark.egg-info/PKG-INFO` & `dagster-snowflake-pyspark-0.20.0/dagster_snowflake_pyspark.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: dagster-snowflake-pyspark
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for integrating Snowflake and PySpark with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pyspark
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

### Comparing `dagster-snowflake-pyspark-0.19.9rc0/setup.py` & `dagster-snowflake-pyspark-0.20.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,25 +22,24 @@
     version=ver,
     author="Elementl",
     author_email="hello@elementl.com",
     license="Apache-2.0",
     description="Package for integrating Snowflake and PySpark with Dagster.",
     url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pyspark",
     classifiers=[
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_snowflake_pyspark_tests*"]),
     install_requires=[
-        "dagster==1.3.9rc0",
-        "dagster-snowflake==0.19.9rc0",
+        "dagster==1.4.0",
+        "dagster-snowflake==0.20.0",
         "pyspark",
         "requests",
         "sqlalchemy!=1.4.42",  # workaround for https://github.com/snowflakedb/snowflake-sqlalchemy/issues/350
         "snowflake-sqlalchemy>=1.2",
     ],
     zip_safe=False,
 )
```

