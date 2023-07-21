# Comparing `tmp/databricks_helper-0.0.7.tar.gz` & `tmp/databricks_helper-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_helper-0.0.7.tar", last modified: Tue Jul 18 03:42:14 2023, max compression
+gzip compressed data, was "databricks_helper-0.0.8.tar", last modified: Fri Jul 21 16:32:46 2023, max compression
```

## Comparing `databricks_helper-0.0.7.tar` & `databricks_helper-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 03:42:14.472393 databricks_helper-0.0.7/
--rw-rw-rw-   0        0        0     1090 2023-07-18 00:40:50.000000 databricks_helper-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      702 2023-07-18 03:42:14.472393 databricks_helper-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-18 00:40:50.000000 databricks_helper-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 03:42:14.437944 databricks_helper-0.0.7/databricks_helper/
--rw-rw-rw-   0        0        0     1901 2023-07-18 03:39:12.000000 databricks_helper-0.0.7/databricks_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 03:42:14.423172 databricks_helper-0.0.7/databricks_helper/api/
-drwxrwxrwx   0        0        0        0 2023-07-18 03:42:14.470399 databricks_helper-0.0.7/databricks_helper/api/src/
--rw-rw-rw-   0        0        0    13916 2023-07-18 03:38:53.000000 databricks_helper-0.0.7/databricks_helper/api/src/basic_code.py
-drwxrwxrwx   0        0        0        0 2023-07-18 03:42:14.468405 databricks_helper-0.0.7/databricks_helper.egg-info/
--rw-rw-rw-   0        0        0      702 2023-07-18 03:42:14.000000 databricks_helper-0.0.7/databricks_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-07-18 03:42:14.000000 databricks_helper-0.0.7/databricks_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 03:42:14.000000 databricks_helper-0.0.7/databricks_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-18 03:42:14.000000 databricks_helper-0.0.7/databricks_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       66 2023-07-18 03:42:14.000000 databricks_helper-0.0.7/databricks_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-18 03:42:14.475385 databricks_helper-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-07-18 03:41:37.000000 databricks_helper-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:32:46.288337 databricks_helper-0.0.8/
+-rw-rw-rw-   0        0        0     1090 2023-07-18 00:40:50.000000 databricks_helper-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      702 2023-07-21 16:32:46.288337 databricks_helper-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-18 00:40:50.000000 databricks_helper-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 16:32:46.253431 databricks_helper-0.0.8/databricks_helper/
+-rw-rw-rw-   0        0        0     2157 2023-07-21 16:11:24.000000 databricks_helper-0.0.8/databricks_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:32:46.236150 databricks_helper-0.0.8/databricks_helper/api/
+drwxrwxrwx   0        0        0        0 2023-07-21 16:32:46.286342 databricks_helper-0.0.8/databricks_helper/api/src/
+-rw-rw-rw-   0        0        0    14918 2023-07-21 16:30:52.000000 databricks_helper-0.0.8/databricks_helper/api/src/basic_code.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:32:46.284380 databricks_helper-0.0.8/databricks_helper.egg-info/
+-rw-rw-rw-   0        0        0      702 2023-07-21 16:32:46.000000 databricks_helper-0.0.8/databricks_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-07-21 16:32:46.000000 databricks_helper-0.0.8/databricks_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 16:32:46.000000 databricks_helper-0.0.8/databricks_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-21 16:32:46.000000 databricks_helper-0.0.8/databricks_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       66 2023-07-21 16:32:46.000000 databricks_helper-0.0.8/databricks_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-21 16:32:46.290332 databricks_helper-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1181 2023-07-21 16:32:24.000000 databricks_helper-0.0.8/setup.py
```

### Comparing `databricks_helper-0.0.7/LICENSE` & `databricks_helper-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_helper-0.0.7/PKG-INFO` & `databricks_helper-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: databricks_helper
-Version: 0.0.7
+Version: 0.0.8
 Summary: databricks helper package
 Home-page: https://github.com/SamuelJansen/databricks-helper/
-Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.7.tar.gz
+Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.8.tar.gz
 Author: Samuel Jansen
 Author-email: samuel.jansenn@gmail.com
 License: MIT
 Keywords: helper,databricks helper package,databricks helper,helper package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `databricks_helper-0.0.7/databricks_helper/__init__.py` & `databricks_helper-0.0.8/databricks_helper/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 from databricks_helper.api.src.basic_code import (
 
+    ONE_MILION,
+    VERY_LOW_DECIMAL_VALUE,
+    NULL_QUERY,
+    FIRST_MONTH_DAY,
+    MINIMUM_LAST_MONTH_DAY,
+    FIRST_MONTH_DAY_AS_STRING,
+    MINIMUM_LAST_MONTH_DAY_AS_STRING,
+
     get_spark_session,
     get_display_spark_dataframe_caller,
 
     set_default_spark_session,
     set_default_display_spark_dataframe,
 
     spark_col,
@@ -59,14 +67,15 @@
     get_distinct_integer_collection_from_table,
     get_distinct_integer_collection_from_table_by_cd,
     display_spark_dataframe,
     display_query,
     spark_sql,
     spark_create_or_replace_temp_view_from_sql,
     spark_big_sql,
-    spark_spark_create_or_replace_temp_view_from_big_sql,
+    spark_create_or_replace_temp_view_from_big_sql,
+    spark_spark_create_or_replace_temp_view_from_big_sql, ###- deprecated
     spark_createDataFrame,
     override_table_and_schema,
     override_table,
     to_spark_df_override_delta_mode,
     save_as_table
 )
```

### Comparing `databricks_helper-0.0.7/databricks_helper/api/src/basic_code.py` & `databricks_helper-0.0.8/databricks_helper/api/src/basic_code.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,41 @@
 try:
     from pyspark.sql.dataframe import DataFrame
     from pyspark.sql import SparkSession
 except Exception as exception:
     print(exception)
     DataFrame = None
     SparkSession = None
-from pyspark.sql.functions import col as spark_col
-from pyspark.sql.functions import sum as spark_sum
-from pyspark.sql.functions import round as spark_round
-from pyspark.sql.types import StructType, StructField, StringType, DoubleType, DecimalType, IntegerType, DateType, TimestampType
+
+try:
+    from pyspark.sql.functions import col as spark_col
+    from pyspark.sql.functions import sum as spark_sum
+    from pyspark.sql.functions import round as spark_round
+except Exception as exception:
+    print(exception)
+    spark_col, spark_sum, spark_round = (
+        None, 
+        None, 
+        None
+    )
+
+try:
+    from pyspark.sql.types import StructType, StructField, StringType, DoubleType, DecimalType, IntegerType, DateType, TimestampType
+except Exception as exception:
+    print(exception)
+    StructType, StructField, StringType, DoubleType, DecimalType, IntegerType, DateType, TimestampType = (
+        None, 
+        None, 
+        None, 
+        None, 
+        None, 
+        None, 
+        None, 
+        None
+    )
 
 
 global DB_SPARK_SESSION
 DB_SPARK_SESSION = None
 
 global DB_SPARK_DF_DISPLAY
 DB_SPARK_DF_DISPLAY = None
@@ -45,14 +68,28 @@
 
 
 def set_default_display_spark_dataframe(spark_df_display):
     global DB_SPARK_DF_DISPLAY
     DB_SPARK_DF_DISPLAY = spark_df_display
 
 
+try:
+    set_default_spark_session(spark)
+except Exception as exception:
+    print('Default "spark" session not loaded. Please run:')
+    print('set_default_spark_session(spark)')
+
+
+try :
+    set_default_display_spark_dataframe(display)
+except Exception as exception:
+    print('Default "display" function not loaded. Please run:')
+    print('set_default_display_spark_dataframe(display)')
+
+
 def get_spark_session(spark_session: SparkSession = None) -> SparkSession: 
     if ObjectHelper.isNotNone(spark_session):
         return spark_session
     try:
         global DB_SPARK_SESSION
         return DB_SPARK_SESSION
     except Exception as exception:
@@ -373,15 +410,15 @@
 
 def spark_big_sql(*agrs, spark_sql_caller=spark_sql, **kwargs):
     df = spark_sql_caller(*agrs, **kwargs)
     print(f'Rows count: {df.count()}')
     return df
 
 
-def spark_spark_create_or_replace_temp_view_from_big_sql(*agrs, **kwargs) -> DataFrame:
+def spark_create_or_replace_temp_view_from_big_sql(*agrs, **kwargs) -> DataFrame:
     return spark_big_sql(*agrs, spark_sql_caller=spark_create_or_replace_temp_view_from_sql, **kwargs)
     
 
 def spark_createDataFrame(*agrs, show_dataframe=True, order_by=None, spark_session: SparkSession = None, spark_df_display=None, **kwargs) -> DataFrame:
     df = get_spark_session(spark_session=spark_session).createDataFrame(*agrs, **kwargs)
     if ObjectHelper.isNotEmpty(order_by):
         df = df.orderBy(*order_by)
@@ -401,8 +438,12 @@
 def to_spark_df_override_delta_mode(spark_df):
     if 0 >= spark_df.count():
         raise Exception('spark dataframe cannot be empty')
     return spark_df.write.format('delta').mode('overwrite')
 
 
 def save_as_table(spark_df_override_delta_mode, table_name):
-    return spark_df_override_delta_mode.saveAsTable(table_name)
+    return spark_df_override_delta_mode.saveAsTable(table_name)
+
+
+###- deprecated\
+spark_spark_create_or_replace_temp_view_from_big_sql = spark_create_or_replace_temp_view_from_big_sql
```

### Comparing `databricks_helper-0.0.7/databricks_helper.egg-info/PKG-INFO` & `databricks_helper-0.0.8/databricks_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: databricks-helper
-Version: 0.0.7
+Version: 0.0.8
 Summary: databricks helper package
 Home-page: https://github.com/SamuelJansen/databricks-helper/
-Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.7.tar.gz
+Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.8.tar.gz
 Author: Samuel Jansen
 Author-email: samuel.jansenn@gmail.com
 License: MIT
 Keywords: helper,databricks helper package,databricks helper,helper package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `databricks_helper-0.0.7/setup.py` & `databricks_helper-0.0.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 import os
 
 OS_SEPARATOR = os.path.sep
 
-version = '0.0.7'
+version = '0.0.8'
 name = 'databricks_helper'
 packageName = name
 repositoryName = name.replace("_", "-")
 url = f'https://github.com/SamuelJansen/{repositoryName}/'
 
 
 setup(
```

