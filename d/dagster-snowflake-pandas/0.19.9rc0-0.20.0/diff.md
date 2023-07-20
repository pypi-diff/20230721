# Comparing `tmp/dagster-snowflake-pandas-0.19.9rc0.tar.gz` & `tmp/dagster-snowflake-pandas-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-snowflake-pandas-0.19.9rc0.tar", last modified: Thu Jun  8 18:29:30 2023, max compression
+gzip compressed data, was "dagster-snowflake-pandas-0.20.0.tar", last modified: Thu Jul 20 22:01:53 2023, max compression
```

## Comparing `dagster-snowflake-pandas-0.19.9rc0.tar` & `dagster-snowflake-pandas-0.20.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:30.111657 dagster-snowflake-pandas-0.19.9rc0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-snowflake-pandas-0.19.9rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       76 2023-06-08 18:20:46.000000 dagster-snowflake-pandas-0.19.9rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      705 2023-06-08 18:29:30.111657 dagster-snowflake-pandas-0.19.9rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      158 2023-06-08 18:20:46.000000 dagster-snowflake-pandas-0.19.9rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:30.111657 dagster-snowflake-pandas-0.19.9rc0/dagster_snowflake_pandas/
--rw-r--r--   0 root         (0) root         (0)      413 2023-06-08 18:20:46.000000 dagster-snowflake-pandas-0.19.9rc0/dagster_snowflake_pandas/__init__.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 18:20:46.000000 dagster-snowflake-pandas-0.19.9rc0/dagster_snowflake_pandas/py.typed
--rw-r--r--   0 root         (0) root         (0)    11677 2023-06-08 18:20:46.000000 dagster-snowflake-pandas-0.19.9rc0/dagster_snowflake_pandas/snowflake_pandas_type_handler.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-snowflake-pandas-0.19.9rc0/dagster_snowflake_pandas/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:30.111657 dagster-snowflake-pandas-0.19.9rc0/dagster_snowflake_pandas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      705 2023-06-08 18:29:30.000000 dagster-snowflake-pandas-0.19.9rc0/dagster_snowflake_pandas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2023-06-08 18:29:30.000000 dagster-snowflake-pandas-0.19.9rc0/dagster_snowflake_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:29:30.000000 dagster-snowflake-pandas-0.19.9rc0/dagster_snowflake_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:29:30.000000 dagster-snowflake-pandas-0.19.9rc0/dagster_snowflake_pandas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      143 2023-06-08 18:29:30.000000 dagster-snowflake-pandas-0.19.9rc0/dagster_snowflake_pandas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-06-08 18:29:30.000000 dagster-snowflake-pandas-0.19.9rc0/dagster_snowflake_pandas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-08 18:29:30.111657 dagster-snowflake-pandas-0.19.9rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1592 2023-06-08 18:20:46.000000 dagster-snowflake-pandas-0.19.9rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:01:53.925961 dagster-snowflake-pandas-0.20.0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-20 21:53:16.000000 dagster-snowflake-pandas-0.20.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       76 2023-07-20 21:53:16.000000 dagster-snowflake-pandas-0.20.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      652 2023-07-20 22:01:53.925961 dagster-snowflake-pandas-0.20.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      158 2023-07-20 21:53:16.000000 dagster-snowflake-pandas-0.20.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:01:53.925961 dagster-snowflake-pandas-0.20.0/dagster_snowflake_pandas/
+-rw-r--r--   0 root         (0) root         (0)      413 2023-07-20 21:53:16.000000 dagster-snowflake-pandas-0.20.0/dagster_snowflake_pandas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-20 21:53:16.000000 dagster-snowflake-pandas-0.20.0/dagster_snowflake_pandas/py.typed
+-rw-r--r--   0 root         (0) root         (0)    11760 2023-07-20 21:53:16.000000 dagster-snowflake-pandas-0.20.0/dagster_snowflake_pandas/snowflake_pandas_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-snowflake-pandas-0.20.0/dagster_snowflake_pandas/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:01:53.925961 dagster-snowflake-pandas-0.20.0/dagster_snowflake_pandas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      652 2023-07-20 22:01:53.000000 dagster-snowflake-pandas-0.20.0/dagster_snowflake_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-20 22:01:53.000000 dagster-snowflake-pandas-0.20.0/dagster_snowflake_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:01:53.000000 dagster-snowflake-pandas-0.20.0/dagster_snowflake_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:01:53.000000 dagster-snowflake-pandas-0.20.0/dagster_snowflake_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      137 2023-07-20 22:01:53.000000 dagster-snowflake-pandas-0.20.0/dagster_snowflake_pandas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-20 22:01:53.000000 dagster-snowflake-pandas-0.20.0/dagster_snowflake_pandas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      171 2023-07-20 22:01:53.925961 dagster-snowflake-pandas-0.20.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-07-20 21:53:16.000000 dagster-snowflake-pandas-0.20.0/setup.py
```

### Comparing `dagster-snowflake-pandas-0.19.9rc0/LICENSE` & `dagster-snowflake-pandas-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-snowflake-pandas-0.19.9rc0/PKG-INFO` & `dagster-snowflake-pandas-0.20.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-snowflake-pandas
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for integrating Snowflake and Pandas with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pandas
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

### Comparing `dagster-snowflake-pandas-0.19.9rc0/dagster_snowflake_pandas/snowflake_pandas_type_handler.py` & `dagster-snowflake-pandas-0.20.0/dagster_snowflake_pandas/snowflake_pandas_type_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,14 +287,18 @@
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
         return [SnowflakePandasTypeHandler()]
 
     @staticmethod
     def default_load_type() -> Optional[Type]:
         return pd.DataFrame
```

### Comparing `dagster-snowflake-pandas-0.19.9rc0/dagster_snowflake_pandas.egg-info/PKG-INFO` & `dagster-snowflake-pandas-0.20.0/dagster_snowflake_pandas.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-snowflake-pandas
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for integrating Snowflake and Pandas with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pandas
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

### Comparing `dagster-snowflake-pandas-0.19.9rc0/setup.py` & `dagster-snowflake-pandas-0.20.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,37 +9,37 @@
     with open(Path(__file__).parent / "dagster_snowflake_pandas/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)
 
     return version["__version__"]
 
 
 ver = get_version()
+
 # dont pin dev installs to avoid pip dep resolver issues
 pin = "" if ver == "1!0+dev" else f"=={ver}"
 setup(
     name="dagster-snowflake-pandas",
     version=ver,
     author="Elementl",
     author_email="hello@elementl.com",
     license="Apache-2.0",
     description="Package for integrating Snowflake and Pandas with Dagster.",
     url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pandas",
     classifiers=[
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_snowflake_pandas_tests*"]),
     install_requires=[
-        "dagster==1.3.9rc0",
-        "dagster-snowflake==0.19.9rc0",
+        "dagster==1.4.0",
+        "dagster-snowflake==0.20.0",
         "pandas",
         "requests",
         "snowflake-connector-python[pandas]",
         "sqlalchemy!=1.4.42",  # workaround for https://github.com/snowflakedb/snowflake-sqlalchemy/issues/350
         "snowflake-sqlalchemy>=1.2",
     ],
     zip_safe=False,
```

