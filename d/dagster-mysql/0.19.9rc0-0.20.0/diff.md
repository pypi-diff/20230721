# Comparing `tmp/dagster-mysql-0.19.9rc0.tar.gz` & `tmp/dagster-mysql-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-mysql-0.19.9rc0.tar", last modified: Thu Jun  8 18:28:57 2023, max compression
+gzip compressed data, was "dagster-mysql-0.20.0.tar", last modified: Thu Jul 20 22:02:53 2023, max compression
```

## Comparing `dagster-mysql-0.19.9rc0.tar` & `dagster-mysql-0.20.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      126 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      605 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      125 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:57.567206 dagster-mysql-0.19.9rc0/dagster_mysql/
--rw-r--r--   0 root         (0) root         (0)      434 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/dagster_mysql/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/alembic/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/dagster_mysql/event_log/
--rw-r--r--   0 root         (0) root         (0)       68 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8792 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/event_log/event_log.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/dagster_mysql/run_storage/
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/run_storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7883 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/run_storage/run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/dagster_mysql/schedule_storage/
--rw-r--r--   0 root         (0) root         (0)       75 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/schedule_storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6277 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/schedule_storage/schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     3730 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/storage.py
--rw-r--r--   0 root         (0) root         (0)     6404 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/utils.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      605 2023-06-08 18:28:57.000000 dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      704 2023-06-08 18:28:57.000000 dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:28:57.000000 dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:28:57.000000 dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       41 2023-06-08 18:28:57.000000 dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-08 18:28:57.000000 dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      148 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1296 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:53.566780 dagster-mysql-0.20.0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-20 21:53:16.000000 dagster-mysql-0.20.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      126 2023-07-20 21:53:16.000000 dagster-mysql-0.20.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      552 2023-07-20 22:02:53.566780 dagster-mysql-0.20.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      125 2023-07-20 21:53:16.000000 dagster-mysql-0.20.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:53.554780 dagster-mysql-0.20.0/dagster_mysql/
+-rw-r--r--   0 root         (0) root         (0)      434 2023-07-20 21:53:16.000000 dagster-mysql-0.20.0/dagster_mysql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:53.558780 dagster-mysql-0.20.0/dagster_mysql/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:16.000000 dagster-mysql-0.20.0/dagster_mysql/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-07-20 21:53:16.000000 dagster-mysql-0.20.0/dagster_mysql/alembic/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:53.558780 dagster-mysql-0.20.0/dagster_mysql/event_log/
+-rw-r--r--   0 root         (0) root         (0)       68 2023-07-20 21:53:16.000000 dagster-mysql-0.20.0/dagster_mysql/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8796 2023-07-20 21:53:16.000000 dagster-mysql-0.20.0/dagster_mysql/event_log/event_log.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-20 21:53:16.000000 dagster-mysql-0.20.0/dagster_mysql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:53.562780 dagster-mysql-0.20.0/dagster_mysql/run_storage/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-20 21:53:16.000000 dagster-mysql-0.20.0/dagster_mysql/run_storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7887 2023-07-20 21:53:16.000000 dagster-mysql-0.20.0/dagster_mysql/run_storage/run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:53.562780 dagster-mysql-0.20.0/dagster_mysql/schedule_storage/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-07-20 21:53:16.000000 dagster-mysql-0.20.0/dagster_mysql/schedule_storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6281 2023-07-20 21:53:16.000000 dagster-mysql-0.20.0/dagster_mysql/schedule_storage/schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3730 2023-07-20 21:53:16.000000 dagster-mysql-0.20.0/dagster_mysql/storage.py
+-rw-r--r--   0 root         (0) root         (0)     6435 2023-07-20 21:53:16.000000 dagster-mysql-0.20.0/dagster_mysql/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-mysql-0.20.0/dagster_mysql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:02:53.558780 dagster-mysql-0.20.0/dagster_mysql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-07-20 22:02:53.000000 dagster-mysql-0.20.0/dagster_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      704 2023-07-20 22:02:53.000000 dagster-mysql-0.20.0/dagster_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:02:53.000000 dagster-mysql-0.20.0/dagster_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:02:53.000000 dagster-mysql-0.20.0/dagster_mysql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 22:02:53.000000 dagster-mysql-0.20.0/dagster_mysql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-20 22:02:53.000000 dagster-mysql-0.20.0/dagster_mysql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-20 22:02:53.574780 dagster-mysql-0.20.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1244 2023-07-20 21:53:16.000000 dagster-mysql-0.20.0/setup.py
```

### Comparing `dagster-mysql-0.19.9rc0/LICENSE` & `dagster-mysql-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.19.9rc0/PKG-INFO` & `dagster-mysql-0.20.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: dagster-mysql
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: A Dagster integration for MySQL
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mysql
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

### Comparing `dagster-mysql-0.19.9rc0/dagster_mysql/alembic/alembic.ini` & `dagster-mysql-0.20.0/dagster_mysql/alembic/alembic.ini`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # on newly generated revision scripts.  See the documentation for further
 # detail and examples
 
 # format using "black" - use the console_scripts runner, against the "black" entrypoint
 hooks = black
 black.type = console_scripts
 black.entrypoint = black
-black.options = --line-length 100 --target-version py36 --target-version py37 --target-version py38 -S --fast
+black.options = --line-length 100 --target-version py38 --target-version py39 --target-version py310 --target-version py311 -S --fast
 
 # Logging configuration
 [loggers]
 keys = root,sqlalchemy,alembic
 
 [handlers]
 keys = console
```

### Comparing `dagster-mysql-0.19.9rc0/dagster_mysql/event_log/event_log.py` & `dagster-mysql-0.20.0/dagster_mysql/event_log/event_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         super().__init__()
 
     def _init_db(self) -> None:
         with self._connect() as conn:
             SqlEventLogStorageMetadata.create_all(conn)
             stamp_alembic_rev(mysql_alembic_config(__file__), conn)
 
-    def optimize_for_dagit(self, statement_timeout: int, pool_recycle: int) -> None:
+    def optimize_for_webserver(self, statement_timeout: int, pool_recycle: int) -> None:
         # When running in dagit, hold an open connection
         # https://github.com/dagster-io/dagster/issues/3719
         self._engine = create_engine(
             self.mysql_url,
             isolation_level=mysql_isolation_level(),
             pool_size=1,
             pool_recycle=pool_recycle,
```

### Comparing `dagster-mysql-0.19.9rc0/dagster_mysql/run_storage/run_storage.py` & `dagster-mysql-0.20.0/dagster_mysql/run_storage/run_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         super().__init__()
 
     def _init_db(self) -> None:
         with self.connect() as conn:
             RunStorageSqlMetadata.create_all(conn)
             stamp_alembic_rev(mysql_alembic_config(__file__), conn)
 
-    def optimize_for_dagit(self, statement_timeout: int, pool_recycle: int) -> None:
+    def optimize_for_webserver(self, statement_timeout: int, pool_recycle: int) -> None:
         # When running in dagit, hold 1 open connection
         # https://github.com/dagster-io/dagster/issues/3719
         self._engine = create_engine(
             self.mysql_url,
             isolation_level=mysql_isolation_level(),
             pool_size=1,
             pool_recycle=pool_recycle,
```

### Comparing `dagster-mysql-0.19.9rc0/dagster_mysql/schedule_storage/schedule_storage.py` & `dagster-mysql-0.20.0/dagster_mysql/schedule_storage/schedule_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             ScheduleStorageSqlMetadata.create_all(conn)
             stamp_alembic_rev(mysql_alembic_config(__file__), conn)
 
         # mark all the data migrations as applied
         self.migrate()
         self.optimize()
 
-    def optimize_for_dagit(self, statement_timeout: int, pool_recycle: int) -> None:
+    def optimize_for_webserver(self, statement_timeout: int, pool_recycle: int) -> None:
         # When running in dagit, hold an open connection
         # https://github.com/dagster-io/dagster/issues/3719
         self._engine = create_engine(
             self.mysql_url,
             isolation_level=mysql_isolation_level(),
             pool_size=1,
             pool_recycle=pool_recycle,
```

### Comparing `dagster-mysql-0.19.9rc0/dagster_mysql/storage.py` & `dagster-mysql-0.20.0/dagster_mysql/storage.py`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.19.9rc0/dagster_mysql/utils.py` & `dagster-mysql-0.20.0/dagster_mysql/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         ) as exc:
             if (
                 isinstance(exc, db_exc.ProgrammingError)
                 and exc.orig
                 and exc.orig.errno == mysql_errorcode.ER_TABLE_EXISTS_ERROR
             ) or (
                 isinstance(exc, mysql.ProgrammingError)
-                and exc.errno == mysql_errorcode.ER_TABLE_EXISTS_ERROR
+                and exc.errno == mysql_errorcode.ER_TABLE_EXISTS_ERROR  # type: ignore  # (bad stubs)
             ):
                 raise
             logging.warning("Retrying failed database creation")
             if retry_limit == 0:
                 raise DagsterMySQLException("too many retries for DB creation") from exc
 
         time.sleep(retry_wait)
```

### Comparing `dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/PKG-INFO` & `dagster-mysql-0.20.0/dagster_mysql.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: dagster-mysql
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: A Dagster integration for MySQL
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mysql
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

### Comparing `dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/SOURCES.txt` & `dagster-mysql-0.20.0/dagster_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.19.9rc0/setup.py` & `dagster-mysql-0.20.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,24 +19,23 @@
     version=ver,
     author="Elementl",
     author_email="hello@elementl.com",
     license="Apache-2.0",
     description="A Dagster integration for MySQL",
     url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mysql",
     classifiers=[
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_mysql_tests*"]),
     package_data={
         "dagster-mysql": [
             "dagster_mysql/alembic/*",
         ]
     },
     include_package_data=True,
-    install_requires=["dagster==1.3.9rc0", "mysql-connector-python"],
+    install_requires=["dagster==1.4.0", "mysql-connector-python"],
     zip_safe=False,
 )
```

