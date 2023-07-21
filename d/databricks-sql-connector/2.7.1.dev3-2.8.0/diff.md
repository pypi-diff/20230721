# Comparing `tmp/databricks_sql_connector-2.7.1.dev3.tar.gz` & `tmp/databricks_sql_connector-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_sql_connector-2.7.1.dev3.tar", max compression
+gzip compressed data, was "databricks_sql_connector-2.8.0.tar", max compression
```

## Comparing `databricks_sql_connector-2.7.1.dev3.tar` & `databricks_sql_connector-2.8.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     5497 2023-07-12 21:59:42.567864 databricks_sql_connector-2.7.1.dev3/CHANGELOG.md
--rw-r--r--   0        0        0    11346 2023-06-14 20:24:08.166793 databricks_sql_connector-2.7.1.dev3/LICENSE
--rw-r--r--   0        0        0     2723 2023-06-14 20:24:08.167012 databricks_sql_connector-2.7.1.dev3/README.md
--rw-r--r--   0        0        0     1697 2023-07-12 22:02:32.029669 databricks_sql_connector-2.7.1.dev3/pyproject.toml
--rw-r--r--   0        0        0      295 2023-06-14 20:24:08.170343 databricks_sql_connector-2.7.1.dev3/src/databricks/__init__.py
--rw-r--r--   0        0        0     1274 2023-07-12 22:02:40.220905 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 20:24:08.170890 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/__init__.py
--rw-r--r--   0        0        0     4421 2023-07-12 21:51:15.071834 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/auth.py
--rw-r--r--   0        0        0     6192 2023-07-12 21:51:15.072262 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/authenticators.py
--rw-r--r--   0        0        0     3790 2023-07-12 21:51:15.072498 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/endpoint.py
--rw-r--r--   0        0        0     9989 2023-07-12 21:51:15.072984 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/oauth.py
--rw-r--r--   0        0        0     1201 2023-06-14 20:24:08.171709 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/oauth_http_handler.py
--rw-r--r--   0        0        0     6036 2023-07-12 21:51:15.073407 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/thrift_http_client.py
--rw-r--r--   0        0        0    37996 2023-07-12 21:51:15.074009 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/client.py
--rw-r--r--   0        0        0     6547 2023-07-12 21:51:15.074368 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/cloudfetch/download_manager.py
--rw-r--r--   0        0        0     6374 2023-07-12 21:51:15.074646 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/cloudfetch/downloader.py
--rw-r--r--   0        0        0     2423 2023-06-14 20:24:08.172576 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/exc.py
--rw-r--r--   0        0        0        0 2023-06-14 20:24:08.172808 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/experimental/__init__.py
--rw-r--r--   0        0        0     2543 2023-07-12 21:51:15.075093 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/experimental/oauth_persistence.py
--rwxr-xr-x   0        0        0     8062 2023-06-14 20:24:08.173439 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote
--rw-r--r--   0        0        0   136849 2023-06-14 20:24:08.175895 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_api/TCLIService/TCLIService.py
--rw-r--r--   0        0        0       49 2023-06-14 20:24:08.176090 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_api/TCLIService/__init__.py
--rw-r--r--   0        0        0     1307 2023-06-14 20:24:08.176221 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_api/TCLIService/constants.py
--rw-r--r--   0        0        0  2077276 2023-06-14 20:24:08.177855 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_api/TCLIService/ttypes.py
--rw-r--r--   0        0        0        0 2023-06-14 20:24:08.178096 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_api/__init__.py
--rw-r--r--   0        0        0    41011 2023-07-12 21:51:15.075657 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_backend.py
--rw-r--r--   0        0        0     6771 2023-06-14 20:24:08.178634 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/types.py
--rw-r--r--   0        0        0    17993 2023-07-12 21:51:15.076152 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/utils.py
--rw-r--r--   0        0        0       60 2023-06-14 20:24:08.179003 databricks_sql_connector-2.7.1.dev3/src/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0    10729 2023-07-12 21:59:42.568504 databricks_sql_connector-2.7.1.dev3/src/databricks/sqlalchemy/dialect/__init__.py
--rw-r--r--   0        0        0      494 2023-06-14 20:24:08.179360 databricks_sql_connector-2.7.1.dev3/src/databricks/sqlalchemy/dialect/base.py
--rw-r--r--   0        0        0      792 2023-06-14 20:24:08.179497 databricks_sql_connector-2.7.1.dev3/src/databricks/sqlalchemy/dialect/compiler.py
--rw-r--r--   0        0        0     4223 1970-01-01 00:00:00.000000 databricks_sql_connector-2.7.1.dev3/PKG-INFO
+-rw-r--r--   0        0        0     5520 2023-07-21 13:45:18.895955 databricks_sql_connector-2.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11346 2023-07-21 13:45:18.895955 databricks_sql_connector-2.8.0/LICENSE
+-rw-r--r--   0        0        0     2723 2023-07-21 13:45:18.895955 databricks_sql_connector-2.8.0/README.md
+-rw-r--r--   0        0        0     1691 2023-07-21 13:45:45.988257 databricks_sql_connector-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0      295 2023-07-21 13:45:18.895955 databricks_sql_connector-2.8.0/src/databricks/__init__.py
+-rw-r--r--   0        0        0     1269 2023-07-21 13:45:18.895955 databricks_sql_connector-2.8.0/src/databricks/sql/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 13:45:18.895955 databricks_sql_connector-2.8.0/src/databricks/sql/auth/__init__.py
+-rw-r--r--   0        0        0     4421 2023-07-21 13:45:18.895955 databricks_sql_connector-2.8.0/src/databricks/sql/auth/auth.py
+-rw-r--r--   0        0        0     6192 2023-07-21 13:45:18.895955 databricks_sql_connector-2.8.0/src/databricks/sql/auth/authenticators.py
+-rw-r--r--   0        0        0     3790 2023-07-21 13:45:18.899955 databricks_sql_connector-2.8.0/src/databricks/sql/auth/endpoint.py
+-rw-r--r--   0        0        0     9989 2023-07-21 13:45:18.899955 databricks_sql_connector-2.8.0/src/databricks/sql/auth/oauth.py
+-rw-r--r--   0        0        0     1201 2023-07-21 13:45:18.899955 databricks_sql_connector-2.8.0/src/databricks/sql/auth/oauth_http_handler.py
+-rw-r--r--   0        0        0     6036 2023-07-21 13:45:18.899955 databricks_sql_connector-2.8.0/src/databricks/sql/auth/thrift_http_client.py
+-rw-r--r--   0        0        0    37996 2023-07-21 13:45:18.899955 databricks_sql_connector-2.8.0/src/databricks/sql/client.py
+-rw-r--r--   0        0        0     6547 2023-07-21 13:45:18.899955 databricks_sql_connector-2.8.0/src/databricks/sql/cloudfetch/download_manager.py
+-rw-r--r--   0        0        0     6374 2023-07-21 13:45:18.899955 databricks_sql_connector-2.8.0/src/databricks/sql/cloudfetch/downloader.py
+-rw-r--r--   0        0        0     2423 2023-07-21 13:45:18.899955 databricks_sql_connector-2.8.0/src/databricks/sql/exc.py
+-rw-r--r--   0        0        0        0 2023-07-21 13:45:18.899955 databricks_sql_connector-2.8.0/src/databricks/sql/experimental/__init__.py
+-rw-r--r--   0        0        0     2543 2023-07-21 13:45:18.899955 databricks_sql_connector-2.8.0/src/databricks/sql/experimental/oauth_persistence.py
+-rwxr-xr-x   0        0        0     8062 2023-07-21 13:45:18.899955 databricks_sql_connector-2.8.0/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote
+-rw-r--r--   0        0        0   136849 2023-07-21 13:45:18.899955 databricks_sql_connector-2.8.0/src/databricks/sql/thrift_api/TCLIService/TCLIService.py
+-rw-r--r--   0        0        0       49 2023-07-21 13:45:18.899955 databricks_sql_connector-2.8.0/src/databricks/sql/thrift_api/TCLIService/__init__.py
+-rw-r--r--   0        0        0     1307 2023-07-21 13:45:18.899955 databricks_sql_connector-2.8.0/src/databricks/sql/thrift_api/TCLIService/constants.py
+-rw-r--r--   0        0        0  2077276 2023-07-21 13:45:18.903955 databricks_sql_connector-2.8.0/src/databricks/sql/thrift_api/TCLIService/ttypes.py
+-rw-r--r--   0        0        0        0 2023-07-21 13:45:18.903955 databricks_sql_connector-2.8.0/src/databricks/sql/thrift_api/__init__.py
+-rw-r--r--   0        0        0    41011 2023-07-21 13:45:18.903955 databricks_sql_connector-2.8.0/src/databricks/sql/thrift_backend.py
+-rw-r--r--   0        0        0     6771 2023-07-21 13:45:18.903955 databricks_sql_connector-2.8.0/src/databricks/sql/types.py
+-rw-r--r--   0        0        0    17993 2023-07-21 13:45:18.903955 databricks_sql_connector-2.8.0/src/databricks/sql/utils.py
+-rw-r--r--   0        0        0       60 2023-07-21 13:45:18.903955 databricks_sql_connector-2.8.0/src/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0    10729 2023-07-21 13:45:18.907955 databricks_sql_connector-2.8.0/src/databricks/sqlalchemy/dialect/__init__.py
+-rw-r--r--   0        0        0      494 2023-07-21 13:45:18.907955 databricks_sql_connector-2.8.0/src/databricks/sqlalchemy/dialect/base.py
+-rw-r--r--   0        0        0      792 2023-07-21 13:45:18.907955 databricks_sql_connector-2.8.0/src/databricks/sqlalchemy/dialect/compiler.py
+-rw-r--r--   0        0        0     4225 1970-01-01 00:00:00.000000 databricks_sql_connector-2.8.0/PKG-INFO
```

### Comparing `databricks_sql_connector-2.7.1.dev3/CHANGELOG.md` & `databricks_sql_connector-2.8.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Release History
 
-## 2.7.x (Unreleased)
+## 2.8.x (Unreleased)
+
+## 2.8.0 (2023-07-21)
 
 - Add support for Cloud Fetch (#146, #151, #154)
 - SQLAlchemy has_table function now honours schema= argument and adds catalog= argument (#174)
 - SQLAlchemy set non_native_boolean_check_constraint False as it's not supported by Databricks (#120)
 - Fix: Revised SQLAlchemy dialect and examples for compatibility with SQLAlchemy==1.3.x (#173)
 - Fix: oauth would fail if expired credentials appeared in ~/.netrc (#122)
 - Fix: Python HTTP proxies were broken after switch to urllib3 (#158)
```

### Comparing `databricks_sql_connector-2.7.1.dev3/LICENSE` & `databricks_sql_connector-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev3/README.md` & `databricks_sql_connector-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev3/pyproject.toml` & `databricks_sql_connector-2.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databricks-sql-connector"
-version = "2.7.1.dev3"
+version = "2.8.0"
 description = "Databricks SQL Connector for Python"
 authors = ["Databricks <databricks-sql-connector-maintainers@databricks.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "databricks", from = "src"}]
 include = ["CHANGELOG.md"]
 
@@ -23,15 +23,15 @@
 lz4 = "^4.0.2"
 requests="^2.18.1"
 oauthlib="^3.1.0"
 numpy = [
     {version = ">=1.16.6", python = ">=3.7,<3.11"},
     {version = ">=1.23.4", python = ">=3.11"}
 ]
-sqlalchemy = ">=1.3.24"
+sqlalchemy = "^1.3.24"
 openpyxl = "^3.0.10"
 alembic = "^1.0.11"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 mypy = "^0.950"
 pylint = ">=2.12.0"
```

### Comparing `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/__init__.py` & `databricks_sql_connector-2.8.0/src/databricks/sql/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 NUMBER = DBAPITypeObject(
     "boolean", "tinyint", "smallint", "int", "bigint", "float", "double", "decimal"
 )
 DATETIME = DBAPITypeObject("timestamp")
 DATE = DBAPITypeObject("date")
 ROWID = DBAPITypeObject()
 
-__version__ = "2.7.1.dev3"
+__version__ = "2.8.0"
 USER_AGENT_NAME = "PyDatabricksSqlConnector"
 
 # These two functions are pyhive legacy
 Date = datetime.date
 Timestamp = datetime.datetime
```

### Comparing `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/auth.py` & `databricks_sql_connector-2.8.0/src/databricks/sql/auth/auth.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/authenticators.py` & `databricks_sql_connector-2.8.0/src/databricks/sql/auth/authenticators.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/endpoint.py` & `databricks_sql_connector-2.8.0/src/databricks/sql/auth/endpoint.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/oauth.py` & `databricks_sql_connector-2.8.0/src/databricks/sql/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/oauth_http_handler.py` & `databricks_sql_connector-2.8.0/src/databricks/sql/auth/oauth_http_handler.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/thrift_http_client.py` & `databricks_sql_connector-2.8.0/src/databricks/sql/auth/thrift_http_client.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/client.py` & `databricks_sql_connector-2.8.0/src/databricks/sql/client.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/cloudfetch/download_manager.py` & `databricks_sql_connector-2.8.0/src/databricks/sql/cloudfetch/download_manager.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/cloudfetch/downloader.py` & `databricks_sql_connector-2.8.0/src/databricks/sql/cloudfetch/downloader.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/exc.py` & `databricks_sql_connector-2.8.0/src/databricks/sql/exc.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/experimental/oauth_persistence.py` & `databricks_sql_connector-2.8.0/src/databricks/sql/experimental/oauth_persistence.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote` & `databricks_sql_connector-2.8.0/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_api/TCLIService/TCLIService.py` & `databricks_sql_connector-2.8.0/src/databricks/sql/thrift_api/TCLIService/TCLIService.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_api/TCLIService/constants.py` & `databricks_sql_connector-2.8.0/src/databricks/sql/thrift_api/TCLIService/constants.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_api/TCLIService/ttypes.py` & `databricks_sql_connector-2.8.0/src/databricks/sql/thrift_api/TCLIService/ttypes.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_backend.py` & `databricks_sql_connector-2.8.0/src/databricks/sql/thrift_backend.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/types.py` & `databricks_sql_connector-2.8.0/src/databricks/sql/types.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/utils.py` & `databricks_sql_connector-2.8.0/src/databricks/sql/utils.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev3/src/databricks/sqlalchemy/dialect/__init__.py` & `databricks_sql_connector-2.8.0/src/databricks/sqlalchemy/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev3/src/databricks/sqlalchemy/dialect/compiler.py` & `databricks_sql_connector-2.8.0/src/databricks/sqlalchemy/dialect/compiler.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev3/PKG-INFO` & `databricks_sql_connector-2.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-sql-connector
-Version: 2.7.1.dev3
+Version: 2.8.0
 Summary: Databricks SQL Connector for Python
 License: Apache-2.0
 Author: Databricks
 Author-email: databricks-sql-connector-maintainers@databricks.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 Requires-Dist: oauthlib (>=3.1.0,<4.0.0)
 Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
 Requires-Dist: pandas (>=1.2.5,<1.4.0) ; python_version >= "3.7" and python_version < "3.8"
 Requires-Dist: pandas (>=1.2.5,<3.0.0) ; python_version >= "3.8"
 Requires-Dist: pyarrow (>=10.0.1) ; python_version >= "3.11"
 Requires-Dist: pyarrow (>=6.0.0) ; python_version >= "3.7" and python_version < "3.11"
 Requires-Dist: requests (>=2.18.1,<3.0.0)
-Requires-Dist: sqlalchemy (>=1.3.24)
+Requires-Dist: sqlalchemy (>=1.3.24,<2.0.0)
 Requires-Dist: thrift (>=0.16.0,<0.17.0)
 Project-URL: Bug Tracker, https://github.com/databricks/databricks-sql-python/issues
 Project-URL: Homepage, https://github.com/databricks/databricks-sql-python
 Description-Content-Type: text/markdown
 
 # Databricks SQL Connector for Python
```

