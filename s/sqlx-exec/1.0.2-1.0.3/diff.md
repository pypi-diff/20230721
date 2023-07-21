# Comparing `tmp/sqlx-exec-1.0.2.tar.gz` & `tmp/sqlx-exec-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.0.2.tar", last modified: Fri Jul 21 09:21:32 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.0.3.tar", last modified: Fri Jul 21 09:30:47 2023, max compression
```

## Comparing `sqlx-exec-1.0.2.tar` & `sqlx-exec-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 09:21:32.000000 sqlx-exec-1.0.2/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     2535 2023-07-21 09:21:32.000000 sqlx-exec-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2032 2023-07-21 08:58:29.000000 sqlx-exec-1.0.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-21 09:21:32.000000 sqlx-exec-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1160 2023-07-21 09:21:28.000000 sqlx-exec-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:21:32.000000 sqlx-exec-1.0.2/sqlexec/
--rw-rw-rw-   0        0        0      115 2023-07-21 07:43:22.000000 sqlx-exec-1.0.2/sqlexec/constant.py
--rw-rw-rw-   0        0        0     8936 2023-07-21 09:20:58.000000 sqlx-exec-1.0.2/sqlexec/exec.py
--rw-rw-rw-   0        0        0      496 2023-07-21 08:53:39.000000 sqlx-exec-1.0.2/sqlexec/log_support.py
--rw-rw-rw-   0        0        0     1523 2023-07-21 08:22:59.000000 sqlx-exec-1.0.2/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4008 2023-07-21 07:13:11.000000 sqlx-exec-1.0.2/sqlexec/support.py
--rw-rw-rw-   0        0        0      292 2023-07-21 08:34:59.000000 sqlx-exec-1.0.2/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:21:32.000000 sqlx-exec-1.0.2/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-21 09:21:32.000000 sqlx-exec-1.0.2/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-21 08:56:11.000000 sqlx-exec-1.0.2/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2535 2023-07-21 09:21:32.000000 sqlx-exec-1.0.2/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-21 09:21:32.000000 sqlx-exec-1.0.2/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-21 09:21:32.000000 sqlx-exec-1.0.2/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 09:30:47.000000 sqlx-exec-1.0.3/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2535 2023-07-21 09:30:47.000000 sqlx-exec-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2032 2023-07-21 08:58:29.000000 sqlx-exec-1.0.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-21 09:30:47.000000 sqlx-exec-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1160 2023-07-21 09:30:44.000000 sqlx-exec-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:30:47.000000 sqlx-exec-1.0.3/sqlexec/
+-rw-rw-rw-   0        0        0      115 2023-07-21 07:43:22.000000 sqlx-exec-1.0.3/sqlexec/constant.py
+-rw-rw-rw-   0        0        0     8940 2023-07-21 09:30:05.000000 sqlx-exec-1.0.3/sqlexec/exec.py
+-rw-rw-rw-   0        0        0      496 2023-07-21 08:53:39.000000 sqlx-exec-1.0.3/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0     1523 2023-07-21 08:22:59.000000 sqlx-exec-1.0.3/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4008 2023-07-21 07:13:11.000000 sqlx-exec-1.0.3/sqlexec/support.py
+-rw-rw-rw-   0        0        0      292 2023-07-21 08:34:59.000000 sqlx-exec-1.0.3/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:30:47.000000 sqlx-exec-1.0.3/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-21 09:30:47.000000 sqlx-exec-1.0.3/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-21 08:56:11.000000 sqlx-exec-1.0.3/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2535 2023-07-21 09:30:47.000000 sqlx-exec-1.0.3/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-21 09:30:47.000000 sqlx-exec-1.0.3/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-21 09:30:47.000000 sqlx-exec-1.0.3/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.0.2/LICENSE` & `sqlx-exec-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.0.2/PKG-INFO` & `sqlx-exec-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.0.2
+Version: 1.0.3
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto mange database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
```

### Comparing `sqlx-exec-1.0.2/README.rst` & `sqlx-exec-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.0.2/setup.py` & `sqlx-exec-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="sqlx-exec is a simple sql executor for Python, it help you auto mange database connection and transaction.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.0.2',
+    version='1.0.3',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.0.2/sqlexec/exec.py` & `sqlx-exec-1.0.3/sqlexec/exec.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,34 +16,31 @@
             logger.setLevel(DEBUG)
 
     if connect:
         import types
         assert isinstance(connect, types.FunctionType), '`connect` must be a function, you can use like `connect=lambda: connect(**kwargs)`.'
         _init_engin(connect)
     else:
+        if engin == Engin.MySQL:
+            try:
+                from mysql.connector import connect
+            except ImportError:
+                from pymysql import connect
+        elif engin == Engin.PostgreSQL:
+            from psycopg2 import connect
+        else:
+            raise DBError('Engin is invalid: %s', engin)
         kwargs['user'] = user
         kwargs['password'] = password
         kwargs['database'] = database
         kwargs['host'] = host
         kwargs['port'] = port
         _init_engin(lambda: connect(**kwargs))
 
 
-def _import(engin: Engin):
-    if engin == Engin.MySQL:
-        try:
-            from mysql.connector import connect
-        except ImportError:
-            from pymysql import connect
-    elif engin == Engin.PostgreSQL:
-        from psycopg2 import connect
-    else:
-        raise DBError('Engin is invalid: %s', engin)
-
-
 def _init_engin(connect):
     global _DB_CTX
     with DB_LOCK:
         if _DB_CTX is not None:
             raise DBError('DB is already initialized.')
 
         _DB_CTX = DBCtx(connect=connect)
```

### Comparing `sqlx-exec-1.0.2/sqlexec/sql_support.py` & `sqlx-exec-1.0.3/sqlexec/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.0.2/sqlexec/support.py` & `sqlx-exec-1.0.3/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.0.2/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.0.3/sqlx_exec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.0.2
+Version: 1.0.3
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto mange database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
```

