# Comparing `tmp/databricks_helper-0.0.8.tar.gz` & `tmp/databricks_helper-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_helper-0.0.8.tar", last modified: Fri Jul 21 16:32:46 2023, max compression
+gzip compressed data, was "databricks_helper-0.0.9.tar", last modified: Fri Jul 21 16:59:52 2023, max compression
```

## Comparing `databricks_helper-0.0.8.tar` & `databricks_helper-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 16:32:46.288337 databricks_helper-0.0.8/
--rw-rw-rw-   0        0        0     1090 2023-07-18 00:40:50.000000 databricks_helper-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      702 2023-07-21 16:32:46.288337 databricks_helper-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-18 00:40:50.000000 databricks_helper-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 16:32:46.253431 databricks_helper-0.0.8/databricks_helper/
--rw-rw-rw-   0        0        0     2157 2023-07-21 16:11:24.000000 databricks_helper-0.0.8/databricks_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:32:46.236150 databricks_helper-0.0.8/databricks_helper/api/
-drwxrwxrwx   0        0        0        0 2023-07-21 16:32:46.286342 databricks_helper-0.0.8/databricks_helper/api/src/
--rw-rw-rw-   0        0        0    14918 2023-07-21 16:30:52.000000 databricks_helper-0.0.8/databricks_helper/api/src/basic_code.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:32:46.284380 databricks_helper-0.0.8/databricks_helper.egg-info/
--rw-rw-rw-   0        0        0      702 2023-07-21 16:32:46.000000 databricks_helper-0.0.8/databricks_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-07-21 16:32:46.000000 databricks_helper-0.0.8/databricks_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 16:32:46.000000 databricks_helper-0.0.8/databricks_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-21 16:32:46.000000 databricks_helper-0.0.8/databricks_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       66 2023-07-21 16:32:46.000000 databricks_helper-0.0.8/databricks_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-21 16:32:46.290332 databricks_helper-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-07-21 16:32:24.000000 databricks_helper-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:59:52.353558 databricks_helper-0.0.9/
+-rw-rw-rw-   0        0        0     1090 2023-07-18 00:40:50.000000 databricks_helper-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      702 2023-07-21 16:59:52.353558 databricks_helper-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-18 00:40:50.000000 databricks_helper-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 16:59:52.294716 databricks_helper-0.0.9/databricks_helper/
+-rw-rw-rw-   0        0        0     2189 2023-07-21 16:59:13.000000 databricks_helper-0.0.9/databricks_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:59:52.276764 databricks_helper-0.0.9/databricks_helper/api/
+drwxrwxrwx   0        0        0        0 2023-07-21 16:59:52.351564 databricks_helper-0.0.9/databricks_helper/api/src/
+-rw-rw-rw-   0        0        0    15804 2023-07-21 16:58:51.000000 databricks_helper-0.0.9/databricks_helper/api/src/basic_code.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:59:52.348572 databricks_helper-0.0.9/databricks_helper.egg-info/
+-rw-rw-rw-   0        0        0      702 2023-07-21 16:59:52.000000 databricks_helper-0.0.9/databricks_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-07-21 16:59:52.000000 databricks_helper-0.0.9/databricks_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 16:59:52.000000 databricks_helper-0.0.9/databricks_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-07-21 16:59:52.000000 databricks_helper-0.0.9/databricks_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       66 2023-07-21 16:59:52.000000 databricks_helper-0.0.9/databricks_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-21 16:59:52.356550 databricks_helper-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1186 2023-07-21 16:57:26.000000 databricks_helper-0.0.9/setup.py
```

### Comparing `databricks_helper-0.0.8/LICENSE` & `databricks_helper-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_helper-0.0.8/PKG-INFO` & `databricks_helper-0.0.9/databricks_helper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: databricks_helper
-Version: 0.0.8
+Name: databricks-helper
+Version: 0.0.9
 Summary: databricks helper package
 Home-page: https://github.com/SamuelJansen/databricks-helper/
-Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.8.tar.gz
+Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.9.tar.gz
 Author: Samuel Jansen
 Author-email: samuel.jansenn@gmail.com
 License: MIT
 Keywords: helper,databricks helper package,databricks helper,helper package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `databricks_helper-0.0.8/databricks_helper/__init__.py` & `databricks_helper-0.0.9/databricks_helper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     cast_to_query_2_digits_decimal,
     cast_to_query_percentual_decimal,
     cast_to_query_monetary_decimal,
     cast_to_query_integer,
     concat_query_date,
     get_distinct_integer_collection_from_table,
     get_distinct_integer_collection_from_table_by_cd,
+    query_distinct_collection,
     display_spark_dataframe,
     display_query,
     spark_sql,
     spark_create_or_replace_temp_view_from_sql,
     spark_big_sql,
     spark_create_or_replace_temp_view_from_big_sql,
     spark_spark_create_or_replace_temp_view_from_big_sql, ###- deprecated
```

### Comparing `databricks_helper-0.0.8/databricks_helper/api/src/basic_code.py` & `databricks_helper-0.0.9/databricks_helper/api/src/basic_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,19 +34,26 @@
         None, 
         None, 
         None, 
         None
     )
 
 
-global DB_SPARK_SESSION
-DB_SPARK_SESSION = None
+DB_SPARK_SESSION_KEY = 'DB_SPARK_SESSION'
+DB_SPARK_DF_DISPLAY_KEY = 'DB_SPARK_DF_DISPLAY'
+GLOBAL_VALUES = {
+    DB_SPARK_SESSION_KEY: None,
+    DB_SPARK_DF_DISPLAY_KEY: None
+}
 
-global DB_SPARK_DF_DISPLAY
-DB_SPARK_DF_DISPLAY = None
+# # global DB_SPARK_SESSION
+# DB_SPARK_SESSION = None
+
+# # global DB_SPARK_DF_DISPLAY
+# DB_SPARK_DF_DISPLAY = None
 
 
 spark_col = spark_col
 spark_sum = spark_sum
 spark_round = spark_round
 StructType = StructType
 StructField = StructField
@@ -59,21 +66,24 @@
 Decimal = Decimal
 
 DataFrame = DataFrame
 SparkSession = SparkSession
 
 
 def set_default_spark_session(spark_session):
-    global DB_SPARK_SESSION
-    DB_SPARK_SESSION = spark_session
+    # global DB_SPARK_SESSION
+    # DB_SPARK_SESSION = spark_session
+    GLOBAL_VALUES[DB_SPARK_SESSION_KEY] = spark_session
 
 
 def set_default_display_spark_dataframe(spark_df_display):
-    global DB_SPARK_DF_DISPLAY
-    DB_SPARK_DF_DISPLAY = spark_df_display
+    # global DB_SPARK_DF_DISPLAY
+    # DB_SPARK_DF_DISPLAY = spark_df_display
+    GLOBAL_VALUES[DB_SPARK_DF_DISPLAY_KEY] = spark_df_display
+
 
 
 try:
     set_default_spark_session(spark)
 except Exception as exception:
     print('Default "spark" session not loaded. Please run:')
     print('set_default_spark_session(spark)')
@@ -86,29 +96,30 @@
     print('set_default_display_spark_dataframe(display)')
 
 
 def get_spark_session(spark_session: SparkSession = None) -> SparkSession: 
     if ObjectHelper.isNotNone(spark_session):
         return spark_session
     try:
-        global DB_SPARK_SESSION
-        return DB_SPARK_SESSION
+        # global DB_SPARK_SESSION
+        # return DB_SPARK_SESSION
+        return GLOBAL_VALUES[DB_SPARK_SESSION_KEY]
     except Exception as exception:
         print(exception)
         print(f'''databricks_helper.DB_SPARK_SESSION = spark''')
     return None
 
 
 def get_display_spark_dataframe_caller(spark_df_display = None):
     if ObjectHelper.isNotNone(spark_df_display):
         return spark_df_display
-    # global DB_SPARK_DF_DISPLAY
     try:
-        global DB_SPARK_DF_DISPLAY
-        return DB_SPARK_DF_DISPLAY
+        # global DB_SPARK_DF_DISPLAY
+        # return DB_SPARK_DF_DISPLAY
+        return GLOBAL_VALUES[DB_SPARK_DF_DISPLAY_KEY]
     except Exception as exception:
         print(exception)
         print(f'''databricks_helper.DB_SPARK_DF_DISPLAY = display''')
     return None
 
 
 def two_digits_prefixed_with_zeros_as_string(day_as_int):
@@ -377,14 +388,24 @@
                 # , show_query=False, show_dataframe=False
             ).select(f'{column_name}_set').first()[0]
             if query_value_as_string_is_not_null(cd_as_string)
         ])
     except Exception as exception:
         log.failure(get_distinct_integer_collection_from_table_by_cd, 'Not possible to extract collection. Returning empty collection by default', exception=exception, muteStackTrace=True)
         return []
+    
+
+def query_distinct_collection(column_name: str, view_or_table_name: str, by_column_name=None, by_column_value=None) -> DataFrame:
+    return spark_sql(f'''
+        SELECT DISTINCT {column_name} 
+        FROM {view_or_table_name} 
+        WHERE {
+            '1=1' if ObjectHelper.isNoneOrBlank(by_column_name) else f'({by_column_name} = f"{NULL_QUERY if ObjectHelper.isNone(by_column_value) else by_column_value}")'
+        } 
+        ORDER BY {column_name}''') 
 
 
 def display_spark_dataframe(spark_df: DataFrame, *args, spark_df_display=None, **kwargs) -> DataFrame:
     ###- Here, display() is a builting function in databricks
     get_display_spark_dataframe_caller(spark_df_display=spark_df_display)(spark_df, *args, **kwargs)
     return spark_df
```

### Comparing `databricks_helper-0.0.8/databricks_helper.egg-info/PKG-INFO` & `databricks_helper-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: databricks-helper
-Version: 0.0.8
+Name: databricks_helper
+Version: 0.0.9
 Summary: databricks helper package
 Home-page: https://github.com/SamuelJansen/databricks-helper/
-Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.8.tar.gz
+Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.9.tar.gz
 Author: Samuel Jansen
 Author-email: samuel.jansenn@gmail.com
 License: MIT
 Keywords: helper,databricks helper package,databricks helper,helper package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `databricks_helper-0.0.8/setup.py` & `databricks_helper-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 import os
 
 OS_SEPARATOR = os.path.sep
 
-version = '0.0.8'
+version = '0.0.9'
 name = 'databricks_helper'
 packageName = name
 repositoryName = name.replace("_", "-")
 url = f'https://github.com/SamuelJansen/{repositoryName}/'
 
 
 setup(
@@ -22,15 +22,15 @@
     description = 'databricks helper package',
     author = 'Samuel Jansen',
     author_email = 'samuel.jansenn@gmail.com',
     url = url,
     download_url = f'{url}archive/v{version}.tar.gz',
     keywords = ['helper', 'databricks helper package', 'databricks helper', 'helper package'],
     install_requires = [
-        'pyspark<4.0.0,>=2.0.0',
+        ###- 'pyspark<4.0.0,>=2.0.0',
         'python_helper<1.0.0,>=0.3.67'
     ],
     classifiers = [
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
```

