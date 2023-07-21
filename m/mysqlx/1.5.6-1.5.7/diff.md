# Comparing `tmp/mysqlx-1.5.6.tar.gz` & `tmp/mysqlx-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.5.6.tar", last modified: Wed Jul 19 06:57:49 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.5.7.tar", last modified: Fri Jul 21 10:08:35 2023, max compression
```

## Comparing `mysqlx-1.5.6.tar` & `mysqlx-1.5.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 06:57:49.000000 mysqlx-1.5.6/
-drwxrwxrwx   0        0        0        0 2023-07-19 06:57:49.000000 mysqlx-1.5.6/mysqlx/
--rw-rw-rw-   0        0        0      238 2023-07-19 05:44:57.000000 mysqlx-1.5.6/mysqlx/config_holder.py
--rw-rw-rw-   0        0        0      617 2023-07-18 12:32:21.000000 mysqlx-1.5.6/mysqlx/constant.py
--rw-rw-rw-   0        0        0    19262 2023-07-16 17:16:35.000000 mysqlx-1.5.6/mysqlx/db.py
--rw-rw-rw-   0        0        0    13298 2023-07-14 21:56:44.000000 mysqlx-1.5.6/mysqlx/dbx.py
--rw-rw-rw-   0        0        0     3984 2023-07-13 13:31:18.000000 mysqlx-1.5.6/mysqlx/log_support.py
--rw-rw-rw-   0        0        0    37742 2023-07-19 06:54:38.000000 mysqlx-1.5.6/mysqlx/orm.py
--rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 mysqlx-1.5.6/mysqlx/snowflake.py
--rw-rw-rw-   0        0        0     6384 2023-07-19 05:49:07.000000 mysqlx-1.5.6/mysqlx/sql_holder.py
--rw-rw-rw-   0        0        0     4077 2023-07-13 04:01:58.000000 mysqlx-1.5.6/mysqlx/sql_mapper.py
--rw-rw-rw-   0        0        0     6461 2023-07-17 09:31:46.000000 mysqlx-1.5.6/mysqlx/support.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.5.6/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 06:57:49.000000 mysqlx-1.5.6/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-19 06:57:49.000000 mysqlx-1.5.6/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-19 06:57:49.000000 mysqlx-1.5.6/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4306 2023-07-19 06:57:49.000000 mysqlx-1.5.6/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-07-19 06:57:49.000000 mysqlx-1.5.6/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      402 2023-07-19 06:57:49.000000 mysqlx-1.5.6/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-19 06:57:49.000000 mysqlx-1.5.6/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4306 2023-07-19 06:57:49.000000 mysqlx-1.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     3804 2023-07-16 02:24:38.000000 mysqlx-1.5.6/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-19 06:57:49.000000 mysqlx-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0     1211 2023-07-19 06:57:07.000000 mysqlx-1.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 10:08:35.000000 mysqlx-1.5.7/
+drwxrwxrwx   0        0        0        0 2023-07-21 10:08:35.000000 mysqlx-1.5.7/mysqlx/
+-rw-rw-rw-   0        0        0      567 2023-07-19 13:27:51.000000 mysqlx-1.5.7/mysqlx/constant.py
+-rw-rw-rw-   0        0        0    17591 2023-07-19 14:03:44.000000 mysqlx-1.5.7/mysqlx/db.py
+-rw-rw-rw-   0        0        0     7255 2023-07-19 13:52:43.000000 mysqlx-1.5.7/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0     3984 2023-07-13 13:31:18.000000 mysqlx-1.5.7/mysqlx/log_support.py
+-rw-rw-rw-   0        0        0    38034 2023-07-19 13:47:01.000000 mysqlx-1.5.7/mysqlx/orm.py
+-rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 mysqlx-1.5.7/mysqlx/snowflake.py
+-rw-rw-rw-   0        0        0     6307 2023-07-19 13:44:39.000000 mysqlx-1.5.7/mysqlx/sql_holder.py
+-rw-rw-rw-   0        0        0     4096 2023-07-19 13:45:03.000000 mysqlx-1.5.7/mysqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0     3408 2023-07-21 08:20:17.000000 mysqlx-1.5.7/mysqlx/sql_support.py
+-rw-rw-rw-   0        0        0     4969 2023-07-19 13:40:26.000000 mysqlx-1.5.7/mysqlx/support.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.5.7/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 10:08:35.000000 mysqlx-1.5.7/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-21 10:08:35.000000 mysqlx-1.5.7/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-21 10:08:35.000000 mysqlx-1.5.7/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4409 2023-07-21 10:08:35.000000 mysqlx-1.5.7/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-07-21 10:08:35.000000 mysqlx-1.5.7/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      400 2023-07-21 10:08:35.000000 mysqlx-1.5.7/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-21 10:08:35.000000 mysqlx-1.5.7/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4409 2023-07-21 10:08:35.000000 mysqlx-1.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3905 2023-07-21 10:06:40.000000 mysqlx-1.5.7/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-21 10:08:35.000000 mysqlx-1.5.7/setup.cfg
+-rw-rw-rw-   0        0        0     1211 2023-07-21 10:08:06.000000 mysqlx-1.5.7/setup.py
```

### Comparing `mysqlx-1.5.6/mysqlx/db.py` & `mysqlx-1.5.7/mysqlx/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import functools
-from typing import Sequence
-from .constant import LIMIT_1, MAPPER_PATH, PK_SQL, CONFIG_DICT, CACHE_SIZE
+from . import sql_support
+from .constant import MAPPER_PATH, PK_SQL
 from .log_support import logger, sql_log, page_log, insert_log, do_sql_log, do_page_log
-from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, dynamic_sql, get_named_sql, get_named_args, DBError, \
-    DB_LOCK, get_batch_args
+from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, DBError, DB_LOCK
 
 _DB_CTX = None
-_SHOW_SQL = False
 
 
 def init_db(user='root', password='', database='test', host='127.0.0.1', port=3306, pool_size=5, use_unicode=True, show_sql=False, **kwargs):
     global _DB_CTX
     global _SHOW_SQL
     use_mysql_connector = False
     try:
@@ -18,41 +16,39 @@
         use_mysql_connector = True
     except ImportError:
         try:
             from pymysql import connect
         except ImportError:
             raise DBError("Please install MySQL driver, mysql-connector-python >= 8.0.13, PyMySQL >= 0.9.0.")
 
-    _SHOW_SQL = show_sql
     kwargs['user'] = user
     kwargs['password'] = password
     kwargs['database'] = database
     kwargs['host'] = host
     kwargs['port'] = port
     kwargs['use_unicode'] = use_unicode
 
+    sql_support.set_show_sql(show_sql)
+
     if 'debug' in kwargs:
         if kwargs.pop('debug'):
             from logging import DEBUG
             logger.setLevel(DEBUG)
 
-    if CACHE_SIZE in kwargs:
-        CONFIG_DICT[CACHE_SIZE] = kwargs.pop(CACHE_SIZE)
-
     is_pool = use_mysql_connector and pool_size >= 1
     if is_pool:
         kwargs['pool_size'] = pool_size
         if 'pool_name' not in kwargs:
             kwargs['pool_name'] = "{}_pool".format(database)
 
     with DB_LOCK:
         if _DB_CTX is not None:
             raise DBError('DB is already initialized.')
         if MAPPER_PATH in kwargs:
-            from .dbx import load_mapper
+            from .sql_holder import load_mapper
             load_mapper(kwargs.pop(MAPPER_PATH))
         _DB_CTX = DBCtx(connect=lambda: connect(**kwargs), use_mysql_connector=use_mysql_connector)
 
     if is_pool:
         logger.info('Init db engine <%s> ok with connection pool size: %d.' % (hex(id(_DB_CTX)), pool_size))
     else:
         logger.info('Init db engine <%s> ok without connection pool.' % hex(id(_DB_CTX)))
@@ -124,41 +120,41 @@
     """
     Insert data into table, return effect rowcount.
     :param table: table name
     :param kwargs: name='张三', age=20}
     return: Effect rowcount
     """
     insert_log('insert', table, **kwargs)
-    sql, args = _insert_sql_args(table.strip(), **kwargs)
+    sql, args = sql_support.insert_sql_args(table.strip(), **kwargs)
     return do_execute(sql, *args)
 
 
 def save(table: str, **kwargs):
     """
     Insert data into table, return primary key.
     :param table: table
     :param kwargs: name='张三', age=20
     :return: Primary key
     """
     insert_log('save', table, **kwargs)
-    sql, args = _insert_sql_args(table.strip(), **kwargs)
+    sql, args = sql_support.insert_sql_args(table.strip(), **kwargs)
     return do_save(sql, *args)
 
 
 @with_connection
 def do_save(sql: str, *args):
     """
     Insert data into table, return primary key.
     :param sql: table
     :param args:
     :return: Primary key
     """
     global _DB_CTX
     cursor = None
-    sql = _before_execute('do_save', sql, *args)
+    sql = sql_support.before_execute('do_save', sql, *args)
     try:
         cursor = _DB_CTX.connection.cursor()
         cursor.execute(sql, args)
         cursor.execute(PK_SQL)
         result = cursor.fetchone()
         try_commit(_DB_CTX)
         return result[0]
@@ -170,141 +166,141 @@
 def execute(sql: str, *args, **kwargs):
     """
     Execute SQL.
     sql: INSERT INTO user(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
          INSERT INTO user(name, age) VALUES(:name,:age)  -->  kwargs: {'name': '张三', 'age': 20}
     """
     sql_log('db.execute', sql, *args, **kwargs)
-    sql, args = dynamic_sql(sql, *args, **kwargs)
+    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
     return do_execute(sql, *args)
 
 
 def batch_insert(table: str, *args):
     """
     Batch insert
     :param table: table name
     :param args: All number must have same key. [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
     :return: Effect row count
     """
     logger.debug("Exec func 'mysqlx.db.%s' \n\t Table: '%s', args: %s" % ('batch_insert', table, args))
     assert len(args) > 0, 'args must not be empty.'
-    sql, args = _batch_insert_sql_args(table, *args)
+    sql, args = sql_support.batch_insert_sql_args(table, *args)
     return batch_execute(sql, *args)
 
 
 def batch_execute(sql: str, *args):
     """
     Batch execute
     :param sql: INSERT INTO user(name, age) VALUES(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
                 INSERT INTO user(name, age) VALUES(:name,:age)  -->  args: [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
     :param args: All number must have same size.
     :return: Effect row count
     """
     logger.debug("Exec func 'mysqlx.db.%s' \n\t sql: '%s' \n\t args: %s" % ('batch_execute', sql, args))
     assert len(args) > 0, 'args must not be empty.'
     if isinstance(args[0], dict):
-        sql, args = _batch_named_sql_args(sql, *args)
+        sql, args = sql_support.batch_named_sql_args(sql, *args)
 
     return do_batch_execute(sql, *args)
 
 
 # ----------------------------------------------------------Query function------------------------------------------------------------------
 def get(sql: str, *args, **kwargs):
     """
     Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' after sql statement if not.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
          SELECT count(1) FROM user WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     sql_log('get', sql, *args, **kwargs)
     global _DB_CTX
-    sql, args = dynamic_sql(sql, *args, **kwargs)
+    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
     return do_get(sql, *args)
 
 
 def query(sql: str, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     sql_log('query', sql, *args, **kwargs)
-    sql, args = dynamic_sql(sql, *args, **kwargs)
+    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
     return do_query(sql, *args)
 
 
 def query_one(sql: str, *args, **kwargs):
     """
     Execute select SQL and expected one row result(dict). Automatically add 'limit ?' after sql statement if not.
     If no result found, return None.
     If multiple results found, the first one returned.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     sql_log('query_one', sql, *args, **kwargs)
-    sql, args = dynamic_sql(sql, *args, **kwargs)
+    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
     return do_query_one(sql, *args)
 
 
 def select(sql: str, *args, **kwargs):
     """
     Execute select SQL and return list(tuple) or empty list if no result.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     sql_log('select', sql, *args, **kwargs)
-    sql, args = dynamic_sql(sql, *args, **kwargs)
+    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
     return do_select(sql, *args)
 
 
 def select_one(sql: str, *args, **kwargs):
     """
     Execute select SQL and expected one row result(tuple). Automatically add 'limit ?' after sql statement if not.
     If no result found, return None.
     If multiple results found, the first one returned.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     sql_log('select_one', sql, *args, **kwargs)
-    sql, args = dynamic_sql(sql, *args, **kwargs)
+    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
     return do_select_one(sql, *args)
 
 
 def query_page(sql: str, page_num=1, page_size=10, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     page_log('query_page', sql, page_num, page_size, *args, **kwargs)
-    sql, args = dynamic_sql(sql, *args, **kwargs)
+    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
     return do_query_page(sql, page_num, page_size, *args)
 
 
 def select_page(sql: str, page_num=1, page_size=10, *args, **kwargs):
     """
     Execute select SQL and return list(tuple) or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     page_log('select_page', sql, page_num, page_size, *args, **kwargs)
-    sql, args = dynamic_sql(sql, *args, **kwargs)
+    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
     return do_select_page(sql, page_num, page_size, *args)
 
 
 # ----------------------------------------------------------Do function------------------------------------------------------------------
 @with_connection
 def do_execute(sql: str, *args):
     """
     Execute sql return effect rowcount
     sql: insert into user(name, age) values(?, ?)  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = _before_execute('do_execute', sql.strip(), *args)
+    sql = sql_support.before_execute('do_execute', sql.strip(), *args)
     try:
         cursor = _DB_CTX.connection.cursor()
         cursor.execute(sql, args)
         effect_rowcount = cursor.rowcount
         try_commit(_DB_CTX)
         return effect_rowcount
     finally:
@@ -318,16 +314,16 @@
     Batch execute sql return effect rowcount
     :param sql: insert into user(name, age) values(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
     :param args: All number must have same size.
     :return: Effect rowcount
     """
     global _DB_CTX
     cursor = None
-    sql = _before_execute('do_batch_execute', sql.strip(), *args)
-    args = get_batch_args(*args)
+    sql = sql_support.before_execute('do_batch_execute', sql.strip(), *args)
+    args = sql_support.get_batch_args(*args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.executemany(sql, args)
         effect_rowcount = cursor.rowcount
         try_commit(_DB_CTX)
         return effect_rowcount
     finally:
@@ -338,15 +334,15 @@
 def do_get(sql: str, *args):
     """
     Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' behind the sql statement if not.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     do_sql_log('do_get', sql, *args)
-    sql, args = _limit_one_sql_args(sql, *args)
+    sql, args = sql_support.limit_one_sql_args(sql, *args)
     return do_get_limit(sql, *args)
 
 
 def do_get_limit(sql: str, *args):
     """
     Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
     MultiColumnsError: Expect only one column.
@@ -367,15 +363,15 @@
 def do_query(sql: str, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = _before_execute('do_query', sql.strip(), *args)
+    sql = sql_support.before_execute('do_query', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         results = cursor.fetchall()
         if results and cursor.description:
             names = [x[0] for x in cursor.description]
             return [Dict(names, x) for x in results]
@@ -389,27 +385,27 @@
 @with_connection
 def do_query_one(sql: str, *args):
     """
     execute select SQL and return unique result(dict). Automatically add 'limit ?' behind the sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     do_sql_log('do_query_one', sql, *args)
-    sql, args = _limit_one_sql_args(sql, *args)
+    sql, args = sql_support.limit_one_sql_args(sql, *args)
     return do_query_one_limit(sql, *args)
 
 
 @with_connection
 def do_query_one_limit(sql: str, *args):
     """
     execute select SQL and return unique result(dict), SQL contain 'limit'.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = _before_execute('do_query_one_limit', sql.strip(), *args)
+    sql = sql_support.before_execute('do_query_one_limit', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         result = cursor.fetchone()
         if result and cursor.description:
             names = [x[0] for x in cursor.description]
             return Dict(names, result)
@@ -423,15 +419,15 @@
 def do_select(sql: str, *args):
     """
     execute select SQL and return unique result or list results(tuple).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = _before_execute('do_select', sql.strip(), *args)
+    sql = sql_support.before_execute('do_select', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         return cursor.fetchall()
     finally:
         if cursor:
             cursor.close()
@@ -439,27 +435,27 @@
 
 def do_select_one(sql: str, *args):
     """
     Execute select SQL and return unique result(tuple). Automatically add 'limit ?' behind the sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     do_sql_log('do_select_one', sql, *args)
-    sql, args = _limit_one_sql_args(sql, *args)
+    sql, args = sql_support.limit_one_sql_args(sql, *args)
     return do_select_one_limit(sql, *args)
 
 
 @with_connection
 def do_select_one_limit(sql: str, *args):
     """
     Execute select SQL and return unique result(tuple), SQL contain 'limit'.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = _before_execute('do_select_one_limit', sql.strip(), *args)
+    sql = sql_support.before_execute('do_select_one_limit', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         return cursor.fetchone()
     finally:
         if cursor:
             cursor.close()
@@ -467,92 +463,31 @@
 
 def do_query_page(sql: str, page_num=1, page_size=10, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     do_page_log('do_query_page', sql, page_num, page_size, args)
-    sql, args = _page_sql_args(sql, page_num, page_size, *args)
+    sql, args = sql_support.page_sql_args(sql, page_num, page_size, *args)
     return do_query(sql, *args)
 
 
 def do_select_page(sql: str, page_num=1, page_size=10, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     do_page_log('do_select_page', sql, page_num, page_size, args)
-    sql, args = _page_sql_args(sql, page_num, page_size, *args)
+    sql, args = sql_support.page_sql_args(sql, page_num, page_size, *args)
     return do_select(sql, *args)
 
 
 def get_connection():
     global _DB_CTX
     if _DB_CTX.is_not_init():
         _DB_CTX.init()
     return _DB_CTX.connection
 
 
 def prepare(prepared=True):
     global _DB_CTX
     _DB_CTX.prepared = prepared
-
-
-def _before_execute(function: str, sql: str, *args):
-    global _SHOW_SQL
-    if _SHOW_SQL:
-        logger.info("Exec func 'mysqlx.db.%s' \n\tSQL: %s \n\tARGS: %s" % (function, sql, args))
-    return sql.replace('?', '%s')
-
-
-def _insert_sql_args(table: str, **kwargs):
-    cols, args = zip(*kwargs.items())
-    sql = _create_insert_sql(table, cols)
-    return sql, args
-
-
-def _batch_insert_sql_args(table: str, *args):
-    args = get_batch_args(*args)
-    args = [zip(*arg.items()) for arg in args]  # [(cols, args)]
-    cols, args = zip(*args)  # (cols), (args)
-    sql = _create_insert_sql(table, cols[0])
-    return sql, args
-
-
-def _batch_named_sql_args(sql: str, *args):
-    args = get_batch_args(*args)
-    args = [get_named_args(sql, **arg) for arg in args]
-    sql = get_named_sql(sql)
-    return sql, args
-
-
-@functools.lru_cache(maxsize=128)
-def _create_insert_sql(table: str, cols: Sequence[str]):
-    columns, placeholders = zip(*[('`{}`'.format(col), '?') for col in cols])
-    return 'INSERT INTO `{}` ({}) VALUES ({})'.format(table, ','.join(columns), ','.join(placeholders))
-
-
-def _page_sql_args(sql: str, page_num=1, page_size=10, *args):
-    start = (page_num - 1) * page_size
-    args = [*args, start, page_size]
-    if _require_limit(sql):
-        sql = '{} limit ?,?'.format(sql)
-    return sql, args
-
-
-def _limit_one_sql_args(sql: str, *args):
-    if _require_limit(sql):
-        return '{} limit ?'.format(sql), [*args, LIMIT_1]
-
-    return sql, args
-
-
-def _require_limit(sql: str):
-    lower_sql = sql.lower()
-    if 'limit' not in lower_sql:
-        return True
-
-    idx = lower_sql.rindex('limit')
-    if idx > 0 and ')' in lower_sql[idx:]:
-        return True
-
-    return False
```

### Comparing `mysqlx-1.5.6/mysqlx/log_support.py` & `mysqlx-1.5.7/mysqlx/log_support.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.6/mysqlx/orm.py` & `mysqlx-1.5.7/mysqlx/orm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import sys
+from . import db
+from . import log_support
 from datetime import datetime
 from .snowflake import get_id
 from enum import Enum, IntEnum
 from functools import lru_cache
-from .support import DBError, simple_sql, NotFoundError
+from .sql_support import simple_sql
+from .support import DBError, NotFoundError
 from typing import Sequence, Union, List, Tuple
-from .constant import LIMIT_1, NO_LIMIT, DEFAULT_PK_FIELD, PK, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, PK_STRATEGY, COLUMN_SQL, CONFIG_DICT, CACHE_SIZE
-from .db import do_get_limit, do_query, do_query_one_limit, do_execute, insert, save, do_select, do_select_one_limit, transaction, batch_insert, \
-    do_query_page, do_select_page, do_get
-from .log_support import logger, orm_page_log, orm_insert_log, orm_by_log, orm_delete_by_id_log, orm_by_page_log, orm_inst_log, orm_find_by_id_log, \
-    orm_logical_delete_by_ids_log, orm_count_log, orm_find_log, orm_find_by_ids_log
+from .constant import LIMIT_1, NO_LIMIT, DEFAULT_PK_FIELD, PK, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, PK_STRATEGY, COLUMN_SQL, CACHE_SIZE
 
 
 class DelFlag(IntEnum):
     UN_DELETE = 0
     DELETED = 1
 
 
@@ -75,62 +74,62 @@
 
     def persist(self):
         """
         user = User(name='张三', age=55)
         effect_rowcount = user.persist()
         :return: effect rowcount
         """
-        orm_inst_log('persist', self.__class__.__name__)
+        log_support.orm_inst_log('persist', self.__class__.__name__)
         kv = {k: v for k, v in self.__dict__.items() if v is not None}
         return self.insert(**kv)
 
     def inst_save(self):
         """
         user = User(name='张三', age=55)
         id = user.save()
         :return: Primary key
         """
-        orm_inst_log('inst_save', self.__class__.__name__)
+        log_support.orm_inst_log('inst_save', self.__class__.__name__)
         kv = {k: v for k, v in self.__dict__.items() if v is not None}
         pk = self._get_pk()
         _id = self.save(**kv)
         if pk not in kv:
             self.__dict__.update({pk: _id})
         return _id
 
     def update(self, ignored_none=True):
         """
         user = User(id=1, name='李四', age=66)
         rowcount = user.update()
         :return: Effect rowcount
         """
-        orm_inst_log('update', self.__class__.__name__)
+        log_support.orm_inst_log('update', self.__class__.__name__)
         pk, table = self._get_pk_and_table()
         if ignored_none:
             kv = {k: v for k, v in self.__dict__.items() if v is not None}
         else:
             kv = {k: v for k, v in self.__dict__.items()}
 
         _id = kv[pk]
         assert _id is not None, 'Primary key must not be None.'
         update_kv = {k: v for k, v in kv.items() if k != pk}
         if update_kv:
             return self.update_by_id(_id, **update_kv)
         else:
-            logger.warning("Exec func 'mysqlx.orm.Model.%s' not set fields, Class: '%s:'\n\t   %s" % ('update', self.__class__.__name__, self))
+            log_support.logger.warning("Exec func 'mysqlx.orm.Model.%s' not set fields, Class: '%s:'\n\t   %s" % ('update', self.__class__.__name__, self))
             return 0
 
     def load(self, *fields):
         """
         Return new object from database and update itself.
         :param fields: Default select all fields if not set. like: ('id', 'name', 'age')
         user = User(id=1)
         user2 = user.load()
         """
-        logger.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s', fields: %s" % ('load', self.__class__.__name__, fields))
+        log_support.logger.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s', fields: %s" % ('load', self.__class__.__name__, fields))
         pk = self._get_pk()
         kv = self.__dict__
         _id = kv.get(pk)
         assert _id is not None, 'Primary key must not be None.'
         if not fields:
             fields, _ = zip(*kv.items())
         result = self.query_by_id(_id, *fields)
@@ -142,543 +141,543 @@
 
     def logical_delete(self):
         """
         Logic delete only update the del flag
         user = User(id=1)
         rowcount = user.logical_delete()
         """
-        orm_inst_log('logical_delete', self.__class__.__name__)
+        log_support.orm_inst_log('logical_delete', self.__class__.__name__)
         pk = self._get_pk()
         kv = self.__dict__
         _id = kv.get(pk)
         assert _id is not None, 'Primary key must not be None.'
         update_by = kv.get(self._get_update_by_field())
         return self.logical_delete_by_id(_id, update_by)
 
     def un_logical_delete(self):
         """
         Logic un delete only update the del flag
         user = User(id=1)
         rowcount = user.un_logical_delete()
         """
-        orm_inst_log('un_logical_delete', self.__class__.__name__)
+        log_support.orm_inst_log('un_logical_delete', self.__class__.__name__)
         pk = self._get_pk()
         kv = self.__dict__
         _id = kv.get(pk)
         assert _id is not None, 'Primary key must not be None.'
         update_by = kv.get(self._get_update_by_field())
         return self.un_logical_delete_by_id(_id, update_by)
 
     def delete(self):
         """
         Physical delete
         user = User(id=1)
         rowcount = user.delete()
         """
-        orm_inst_log('delete', self.__class__.__name__)
+        log_support.orm_inst_log('delete', self.__class__.__name__)
         pk = self._get_pk()
         _id = self.__dict__.get(pk)
         assert _id is not None, 'Primary key must not be None.'
         return self.delete_by_id(_id)
 
     # ----------------------------------------------------------Class method------------------------------------------------------------------
     @classmethod
     def insert(cls, **kwargs):
         """
         rowcount = User.insert(name='张三', age=20)
         return: Effect rowcount
         """
-        orm_insert_log('insert', cls.__name__, **kwargs)
+        log_support.orm_insert_log('insert', cls.__name__, **kwargs)
         pk, table = cls._get_pk_and_table()
         pk_strategy = cls._get_pk_strategy()
         if pk_strategy == PkStrategy.SNOWFLAKE and pk not in kwargs:
             kwargs[pk] = get_id()
-        return insert(table, **kwargs)
+        return db.insert(table, **kwargs)
 
     @classmethod
     def save(cls, **kwargs):
         """
         id = User.save(name='张三', age=20)
         :return: Primary key
         """
-        orm_insert_log('save', cls.__name__, **kwargs)
+        log_support.orm_insert_log('save', cls.__name__, **kwargs)
         pk, table = cls._get_pk_and_table()
         pk_strategy = cls._get_pk_strategy()
         if pk_strategy == PkStrategy.SNOWFLAKE:
             if pk in kwargs:
                 _id = kwargs[pk]
             else:
                 _id = get_id()
                 kwargs[pk] = _id
-            insert(table, **kwargs)
+            db.insert(table, **kwargs)
         else:
-            _id = save(table, **kwargs)
+            _id = db.save(table, **kwargs)
         return _id
 
     @classmethod
     def create(cls, **kwargs):
         """
         user = User.create(name='张三', age=20)
         :return: Instance object
         """
-        orm_insert_log('create', cls.__name__, **kwargs)
+        log_support.orm_insert_log('create', cls.__name__, **kwargs)
         pk = cls._get_pk()
         _id = cls.save(**kwargs)
         if pk not in kwargs:
             kwargs[pk] = _id
         return cls.to_obj(**kwargs)
 
     @classmethod
     def update_by_id(cls, _id: Union[int, str], **kwargs):
         """
         rowcount = User.update_by_id(id=1, name='王五')
         return: Effect rowcount
         """
-        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t Class: '%s', id: %d, kwargs: %s" % ('update_by_id', cls.__name__, _id, kwargs))
+        log_support.logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t Class: '%s', id: %d, kwargs: %s" % ('update_by_id', cls.__name__, _id, kwargs))
         assert kwargs, 'Must set update kv'
         pk = cls._get_pk()
         where = '`%s`=?' % pk
         cols, args = zip(*kwargs.items())
         sql, update_time_arg = cls._update_sql(where, *cols)
         if update_time_arg:
             args = [*args, update_time_arg]
-        return do_execute(sql, *args, _id, LIMIT_1)
+        return db.do_execute(sql, *args, _id, LIMIT_1)
 
     @classmethod
     def logical_delete_by_id(cls, _id: Union[int, str], update_by: Union[int, str] = None):
         """
         Logic delete only update the del flag
         rowcount = User.delete_by_id(id=1, update_by=100)
         return: Effect rowcount
         """
-        orm_delete_by_id_log('logical_delete_by_id', cls.__name__, _id, update_by)
+        log_support.orm_delete_by_id_log('logical_delete_by_id', cls.__name__, _id, update_by)
         return cls._logical_delete_by_id_op(_id, update_by, DelFlag.DELETED)
 
     @classmethod
     def un_logical_delete_by_id(cls, _id: Union[int, str], update_by: Union[int, str] = None):
         """
         Logic delete only update the del flag
         rowcount = User.un_logical_delete_by_id(id=1, update_by=100)
         return: Effect rowcount
         """
-        orm_delete_by_id_log('un_logical_delete_by_id', cls.__name__, _id, update_by)
+        log_support.orm_delete_by_id_log('un_logical_delete_by_id', cls.__name__, _id, update_by)
         return cls._logical_delete_by_id_op(_id, update_by, DelFlag.UN_DELETE)
 
     @classmethod
     def logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128):
         """
         Logic delete only update the del flag
         rowcount = User.logical_delete_by_ids(id=[1,2], update_by=100)
         return: Effect rowcount
         """
-        orm_logical_delete_by_ids_log('logical_delete_by_ids', cls.__name__, ids, update_by, batch_size)
+        log_support.orm_logical_delete_by_ids_log('logical_delete_by_ids', cls.__name__, ids, update_by, batch_size)
         return cls._logical_delete_by_ids_op(ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.DELETED)
 
     @classmethod
     def un_logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128):
         """
         Logic delete only update the del flag
         rowcount = User.un_logical_delete_by_ids(id=[1,2], update_by=100)
         return: Effect rowcount
         """
-        orm_logical_delete_by_ids_log('un_logical_delete_by_ids', cls.__name__, ids, update_by, batch_size)
+        log_support.orm_logical_delete_by_ids_log('un_logical_delete_by_ids', cls.__name__, ids, update_by, batch_size)
         return cls._logical_delete_by_ids_op(ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.UN_DELETE)
 
     @classmethod
     def delete_by(cls, where: str, *args, **kwargs):
         """
         Physical delete
         rowcount = User.delete_by('where name=? and age=?', '张三', 55)
         return: Effect rowcount
         """
-        orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        log_support.orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         assert where.lower().startswith('where'), "Must start with 'WHERE' in the where parameter."
         table = cls._get_table()
         sql = 'DELETE FROM `%s` %s' % (table, where)
         sql, args = simple_sql(sql, *args, **kwargs)
-        return do_execute(sql, *args)
+        return db.do_execute(sql, *args)
 
     @classmethod
     def delete_by_id(cls, _id: Union[int, str]):
         """
         Physical delete
         rowcount = User.delete_by_id(id=1)
         return: Effect rowcount
         """
-        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t Class: '%s', id: %d" % ('delete_by_id', cls.__name__, _id))
+        log_support.logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t Class: '%s', id: %d" % ('delete_by_id', cls.__name__, _id))
         pk, table = cls._get_pk_and_table()
         sql = 'DELETE FROM `%s` WHERE `%s`=? limit ?' % (table, pk)
-        return do_execute(sql, _id, LIMIT_1)
+        return db.do_execute(sql, _id, LIMIT_1)
 
     @classmethod
     def delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], batch_size=128):
         """
         Batch physical delete, they will be executed in batches if there are too many
         rowcount = User.delete_by_ids(id=[1,2])
         return: Effect rowcount
         """
-        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t Class: '%s', ids: %s, batch_size: %s" % ('delete_by_ids', cls.__name__, ids, batch_size))
+        log_support.logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t Class: '%s', ids: %s, batch_size: %s" % ('delete_by_ids', cls.__name__, ids, batch_size))
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
         if ids_size == 1:
             return cls.delete_by_id(ids[0])
         elif ids_size <= batch_size:
             return cls.do_delete_by_ids(ids)
         else:
             split_ids = _split_ids(ids, batch_size)
-            with transaction():
+            with db.transaction():
                 results = list(map(cls.do_delete_by_ids, split_ids))
             return sum(results)
 
     @classmethod
     def do_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]]):
         """
         Batch physical delete, please use delete_by_ids if there are too many
         rowcount = Person.do_delete_by_ids(id=[1,2])
         return: Effect rowcount
         """
         ids_size = len(ids)
         pk, table = cls._get_pk_and_table()
         sql = 'DELETE FROM {} WHERE {} in ({})'.format(table, pk, ','.join(['?' for _ in range(ids_size)]))
-        return do_execute(sql, *ids)
+        return db.do_execute(sql, *ids)
 
     @classmethod
     def batch_insert(cls, *args):
         """
         Batch insert
         rowcount = User.batch_insert([{'name': '张三', 'age': 55},{'name': '李四', 'age': 66}])
         :param args: All number must have same key.
         :return: Effect rowcount
         """
-        logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t Class: '%s', args: %s" % ('batch_insert', cls.__name__, args))
+        log_support.logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t Class: '%s', args: %s" % ('batch_insert', cls.__name__, args))
         assert len(args) > 0, 'args must not be empty.'
         pk, table = cls._get_pk_and_table()
         pk_strategy = cls._get_pk_strategy()
         if pk_strategy == PkStrategy.SNOWFLAKE:
             for arg in args:
                 if pk not in arg:
                     arg[pk] = get_id()
 
-        return batch_insert(table, *args)
+        return db.batch_insert(table, *args)
 
     # ------------------------------------------------Class query method--------------------------------------------------------
     @classmethod
     def count(cls, **kwargs):
         """
         count = User.count(name='张三', age=55)
         """
-        orm_count_log('count', cls.__name__, **kwargs)
+        log_support.orm_count_log('count', cls.__name__, **kwargs)
         table = cls._get_table()
         where, args, _ = _get_where_arg_limit(**kwargs)
         fields = 'count(1)'
         sql = _select_sql(table, where, LIMIT_1, fields)
-        return do_get_limit(sql, *args, LIMIT_1)
+        return db.do_get_limit(sql, *args, LIMIT_1)
 
     @classmethod
     def count_by(cls, where: str, *args, **kwargs):
         """
         Automatically add 'limit ?' where if not.
         count = User.count_by('where name=?', '李四')
         """
-        orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        log_support.orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         assert where.lower().startswith('where'), "Must start with 'where' in the where parameter."
         table = cls._get_table()
         sql = "SELECT count(1) FROM `{}` {}".format(table, where)
         sql, args = simple_sql(sql, *args, **kwargs)
-        return do_get(sql, *args)
+        return db.do_get(sql, *args)
 
     @classmethod
     def exists(cls, **kwargs):
-        orm_count_log('exists', cls.__name__, **kwargs)
+        log_support.orm_count_log('exists', cls.__name__, **kwargs)
         table = cls._get_table()
         where, args, _ = _get_where_arg_limit(**kwargs)
         sql = "SELECT 1 FROM `{}` {} limit ?".format(table, where)
-        return do_get_limit(sql, *args, LIMIT_1) == 1
+        return db.do_get_limit(sql, *args, LIMIT_1) == 1
 
     @classmethod
     def exists_by(cls, where: str, *args, **kwargs):
-        orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        log_support.orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         assert where.lower().startswith('where'), "Must start with 'where' in the where parameter."
         table = cls._get_table()
         sql = "SELECT 1 FROM `{}` {}".format(table, where)
         sql, args = simple_sql(sql, *args, **kwargs)
-        return do_get(sql, *args) == 1
+        return db.do_get(sql, *args) == 1
 
     @classmethod
     def find(cls, *fields, **kwargs):
         """
         Return list(object) or empty list if no result.
         users = User.find('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
-        orm_find_log('find', cls.__name__, *fields, **kwargs)
+        log_support.orm_find_log('find', cls.__name__, *fields, **kwargs)
         return [cls.to_obj(**d) for d in cls.query(*fields, **kwargs)]
 
     @classmethod
     def find_one(cls, *fields, **kwargs):
         """
         Return unique result(object) or None if no result.
         user = User.find_one('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
-        orm_find_log('find_one', cls.__name__, *fields, **kwargs)
+        log_support.orm_find_log('find_one', cls.__name__, *fields, **kwargs)
         result = cls.query_one(*fields, **kwargs)
         return cls.to_obj(**result) if result else None
 
     @classmethod
     def find_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.find_by('where name=?', '李四')
         """
-        orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        log_support.orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         return [cls.to_obj(**d) for d in cls.query_by(where, *args, **kwargs)]
 
     @classmethod
     def find_page(cls, page_num=1, page_size=10, *fields, **kwargs):
         """
         Return list(object) or empty list if no result.
         users = User.find_page(1, 10, 'name', 'age', name='张三', age=55)
         :param page_num: page number
         :param page_size: page size
         :param fields: Default select all fields if not set
         """
-        orm_page_log('find_page', page_num, page_size, cls.__name__, *fields, **kwargs)
+        log_support.orm_page_log('find_page', page_num, page_size, cls.__name__, *fields, **kwargs)
         result = cls.query_page(page_num, page_size, *fields, **kwargs)
         return [cls.to_obj(**d) for d in result]
 
     @classmethod
     def find_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
         rows = User.find_by_page(1, 10, 'where name=?', '李四')
         """
-        orm_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
+        log_support.orm_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
         return [cls.to_obj(**d) for d in cls.query_page_by(page_num, page_size, where, *args, **kwargs)]
 
     @classmethod
     def find_by_id(cls, _id: Union[int, str], *fields):
         """
         Return one class object or None if no result.
         user = User.find_by_id(1, 'id', 'name', 'age')
         :param _id: pk
         :param fields: Default select all fields if not set
         """
-        orm_find_by_id_log('find_by_id', cls.__name__, _id, *fields)
+        log_support.orm_find_by_id_log('find_by_id', cls.__name__, _id, *fields)
         result = cls.query_by_id(_id, *fields)
         return cls.to_obj(**result) if result else None
 
     @classmethod
     def find_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
         Return list(class object) or empty list if no result.
         users = User.find_by_ids([1,2], 'id', 'name', 'age')
         :param ids: List of pk
         :param fields: Default select all fields if not set
         """
-        orm_find_by_ids_log('find_by_ids', cls.__name__, ids, *fields)
+        log_support.orm_find_by_ids_log('find_by_ids', cls.__name__, ids, *fields)
         return [cls.to_obj(**d) for d in cls.query_by_ids(ids, *fields)]
 
     @classmethod
     def query(cls, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         users = User.query('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
-        orm_find_log('query', cls.__name__, *fields, **kwargs)
+        log_support.orm_find_log('query', cls.__name__, *fields, **kwargs)
         where, args, limit = _get_where_arg_limit(**kwargs)
         table = cls._get_table()
         sql = _select_sql(table, where, limit, *fields)
         if limit:
             if isinstance(limit, int):
                 args = [*args, limit]
             else:
                 args = [*args, *limit]
-        return do_query(sql, *args)
+        return db.do_query(sql, *args)
 
     @classmethod
     def query_one(cls, *fields, **kwargs):
         """
         Return unique result(dict) or None if no result.
         users = User.query_one('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
-        orm_find_log('query_one', cls.__name__, *fields, **kwargs)
+        log_support.orm_find_log('query_one', cls.__name__, *fields, **kwargs)
         where, args, _ = _get_where_arg_limit(**kwargs)
         table = cls._get_table()
         sql = _select_sql(table, where, LIMIT_1, *fields)
-        return do_query_one_limit(sql, *args, LIMIT_1)
+        return db.do_query_one_limit(sql, *args, LIMIT_1)
 
     @classmethod
     def query_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.query_by('where name=?', '李四')
         """
-        orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        log_support.orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         sql = cls._where_sql(where)
         sql, args = simple_sql(sql, *args, **kwargs)
-        return do_query(sql, *args)
+        return db.do_query(sql, *args)
 
     @classmethod
     def query_page(cls, page_num=1, page_size=10, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         users = User.query_page(1, 10, 'id', 'name', 'age', name='张三', age=55)
         :param page_num: page number
         :param page_size: page size
         :param fields: Default select all fields if not set
         """
-        orm_page_log('query_page', page_num, page_size, cls.__name__, *fields, **kwargs)
+        log_support.orm_page_log('query_page', page_num, page_size, cls.__name__, *fields, **kwargs)
         table = cls._get_table()
         where, args, _ = _get_where_arg_limit(**kwargs)
         sql = _select_sql(table, where, NO_LIMIT, *fields)
-        return do_query_page(sql, page_num, page_size, *args)
+        return db.do_query_page(sql, page_num, page_size, *args)
 
     @classmethod
     def query_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
         rows = User.query_by_page(1, 10, 'where name=?', '李四')
         """
-        orm_by_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
+        log_support.orm_by_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
         sql = cls._where_sql(where)
         sql, args = simple_sql(sql, *args, **kwargs)
-        return do_query_page(sql, page_num, page_size, *args)
+        return db.do_query_page(sql, page_num, page_size, *args)
 
     @classmethod
     def query_by_id(cls, _id: Union[int, str], *fields):
         """
         Return one row(dict) or None if no result.
         user = User.query_by_id(1, 'id', 'name', 'age')
         :param _id: pk
         :param fields: Default select all fields if not set
         """
-        orm_find_by_id_log('query_by_id', cls.__name__, _id, *fields)
+        log_support.orm_find_by_id_log('query_by_id', cls.__name__, _id, *fields)
         pk, table = cls._get_pk_and_table()
         where = 'WHERE `{}`=?'.format(pk)
         sql = _select_sql(table, where, LIMIT_1, *fields)
-        return do_query_one_limit(sql, _id, LIMIT_1)
+        return db.do_query_one_limit(sql, _id, LIMIT_1)
 
     @classmethod
     def query_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
         Return list(dict) or empty list if no result.
         users = User.query_by_ids([1,2], 'id', 'name', 'age')
         :param ids: List of pk
         :param fields: Default select all fields if not set
         """
-        orm_find_by_ids_log('query_by_ids', cls.__name__, ids, *fields)
+        log_support.orm_find_by_ids_log('query_by_ids', cls.__name__, ids, *fields)
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
         pk, table = cls._get_pk_and_table()
         where = 'WHERE `{}` in ({})'.format(pk, ','.join(['?' for _ in range(ids_size)]))
         sql = _select_sql(table, where, ids_size, *fields)
-        return do_query(sql, *ids, ids_size)
+        return db.do_query(sql, *ids, ids_size)
 
     @classmethod
     def select(cls, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.select('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
-        orm_find_log('select', cls.__name__, *fields, **kwargs)
+        log_support.orm_find_log('select', cls.__name__, *fields, **kwargs)
         where, args, limit = _get_where_arg_limit(**kwargs)
         table = cls._get_table()
         sql = _select_sql(table, where, limit, *fields)
         if limit:
             if isinstance(limit, int):
                 args = [*args, limit]
             else:
                 args = [*args, *limit]
-        return do_select(sql, *args)
+        return db.do_select(sql, *args)
 
     @classmethod
     def select_one(cls, *fields, **kwargs):
         """
         Return unique result(tuple) or None if no result.
         row = User.select_one('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
-        orm_find_log('select_one', cls.__name__, *fields, **kwargs)
+        log_support.orm_find_log('select_one', cls.__name__, *fields, **kwargs)
         where, args, _ = _get_where_arg_limit(**kwargs)
         table = cls._get_table()
         sql = _select_sql(table, where, LIMIT_1, *fields)
-        return do_select_one_limit(sql, *args, LIMIT_1)
+        return db.do_select_one_limit(sql, *args, LIMIT_1)
 
     @classmethod
     def select_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.select_by('where name=?', '李四')
         """
-        orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        log_support.orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         sql = cls._where_sql(where)
         sql, args = simple_sql(sql, *args, **kwargs)
-        return do_select(sql, *args)
+        return db.do_select(sql, *args)
 
     @classmethod
     def select_page(cls, page_num=1, page_size=10, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.select_page('id', 'name', 'age', name='张三', age=55)
         :param page_num: page number
         :param page_size: page size
         :param fields: Default select all fields if not set
         """
-        orm_page_log('select_page', page_num, page_size, cls.__name__, *fields, **kwargs)
+        log_support.orm_page_log('select_page', page_num, page_size, cls.__name__, *fields, **kwargs)
         table = cls._get_table()
         where, args, _ = _get_where_arg_limit(**kwargs)
         sql = _select_sql(table, where, NO_LIMIT, *fields)
-        return do_select_page(sql, page_num, page_size, *args)
+        return db.do_select_page(sql, page_num, page_size, *args)
 
     @classmethod
     def select_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
         rows = User.select_by_page(1, 10, 'where name=?', '李四')
         """
-        orm_by_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
+        log_support.orm_by_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
         sql = cls._where_sql(where)
         sql, args = simple_sql(sql, *args, **kwargs)
-        return do_select_page(sql, page_num, page_size, *args)
+        return db.do_select_page(sql, page_num, page_size, *args)
 
     @classmethod
     def select_by_id(cls, _id: Union[int, str], *fields):
         """
         Return one row(dict) or None if no result.
         row = User.select_by_id(1, 'id', 'name', 'age')
         :param _id: pk
         :param fields: Default select all fields if not set
         """
-        orm_find_by_id_log('select_by_id', cls.__name__, _id, *fields)
+        log_support.orm_find_by_id_log('select_by_id', cls.__name__, _id, *fields)
         pk, table = cls._get_pk_and_table()
         where = 'WHERE `{}`=?'.format(pk)
         sql = _select_sql(table, where, LIMIT_1, *fields)
-        return do_select_one_limit(sql, _id, LIMIT_1)
+        return db.do_select_one_limit(sql, _id, LIMIT_1)
 
     @classmethod
     def select_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
         Return list(dict) or empty list if no result.
         rows = User.select_by_ids([1,2], 'id', 'name', 'age')
         :param ids: List of pk
         :param fields: Default select all fields if not set
         """
-        orm_find_by_ids_log('select_by_ids', cls.__name__, ids, *fields)
+        log_support.orm_find_by_ids_log('select_by_ids', cls.__name__, ids, *fields)
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
         pk, table = cls._get_pk_and_table()
         where = 'WHERE `{}` in ({})'.format(pk, ','.join(['?' for _ in range(ids_size)]))
         sql = _select_sql(table, where, ids_size, *fields)
-        return do_select(sql, *ids, ids_size)
+        return db.do_select(sql, *ids, ids_size)
 
     @classmethod
     def to_obj(cls, **kwargs):
         model = cls.__new__(cls)
         model.__dict__.update(**kwargs)
         return model
 
@@ -689,69 +688,69 @@
         del_flag_field = cls._get_del_flag_field()
         update_by_field = cls._get_update_by_field()
 
         where = '`%s`=?' % pk
         if update_by is not None and update_by_field is not None:
             sql, update_time_arg = cls._update_sql(where, del_flag_field, update_by_field)
             if update_time_arg:
-                return do_execute(sql, del_status.value, update_by, update_time_arg, _id, LIMIT_1)
-            return do_execute(sql, del_status.value, update_by, _id, LIMIT_1)
+                return db.do_execute(sql, del_status.value, update_by, update_time_arg, _id, LIMIT_1)
+            return db.do_execute(sql, del_status.value, update_by, _id, LIMIT_1)
         else:
             sql, update_time_arg = cls._update_sql(where, del_flag_field)
             if update_time_arg:
-                return do_execute(sql, del_status.value, update_time_arg, _id, LIMIT_1)
-            return do_execute(sql, del_status.value, _id, LIMIT_1)
+                return db.do_execute(sql, del_status.value, update_time_arg, _id, LIMIT_1)
+            return db.do_execute(sql, del_status.value, _id, LIMIT_1)
 
     @classmethod
     def _logical_delete_by_ids_op(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128,
             del_status=DelFlag.DELETED):
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
         if ids_size == 1:
             return cls._logical_delete_by_id_op(ids[0], update_by, del_status)
         elif ids_size <= batch_size:
             return cls._do_logical_delete_by_ids(ids, update_by, del_status)
         else:
             split_ids = _split_ids(ids, batch_size)
-            with transaction():
+            with db.transaction():
                 results = [cls._do_logical_delete_by_ids(ids, update_by, del_status) for ids in split_ids]
             return sum(results)
 
     @classmethod
     def _do_logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, del_status=DelFlag.DELETED):
         ids_size = len(ids)
         pk = cls._get_pk()
         del_flag_field = cls._get_del_flag_field()
         update_by_field = cls._get_update_by_field()
 
         where = '`%s` in (%s)' % (pk, ','.join(['?' for _ in range(ids_size)]))
         if update_by is not None and update_by_field is not None:
             sql, update_time_arg = cls._update_sql(where, del_flag_field, update_by_field)
             if update_time_arg:
-                return do_execute(sql, del_status.value, update_by, update_time_arg, *ids, ids_size)
-            return do_execute(sql, del_status.value, update_by, *ids, ids_size)
+                return db.do_execute(sql, del_status.value, update_by, update_time_arg, *ids, ids_size)
+            return db.do_execute(sql, del_status.value, update_by, *ids, ids_size)
         else:
             sql, update_time_arg = cls._update_sql(where, del_flag_field)
             if update_time_arg:
-                return do_execute(sql, del_status.value, update_time_arg, *ids, ids_size)
-            return do_execute(sql, del_status.value, *ids, ids_size)
+                return db.do_execute(sql, del_status.value, update_time_arg, *ids, ids_size)
+            return db.do_execute(sql, del_status.value, *ids, ids_size)
 
     @classmethod
     def _get_pk(cls):
         if hasattr(cls, PK):
             return cls.__pk__
-        logger.warning("%s not set attribute '%s'" % (cls.__name__, PK))
+        log_support.logger.warning("%s not set attribute '%s'" % (cls.__name__, PK))
         return DEFAULT_PK_FIELD
 
     @classmethod
     def _get_table(cls):
         if hasattr(cls, TABLE):
             return cls.__table__
-        logger.warning("%s not set attribute '%s'" % (cls.__name__, TABLE))
+        log_support.logger.warning("%s not set attribute '%s'" % (cls.__name__, TABLE))
         return _get_table_name(cls.__name__)
 
     @classmethod
     def _get_pk_and_table(cls):
         return cls._get_pk(), cls._get_table()
 
     @classmethod
@@ -814,17 +813,17 @@
             return 'SELECT {} FROM `{}` {} limit ?,?'.format(fields, table, where)
         else:
             raise ValueError("The type of the parameter 'limit' must be 'int' or tuple, list, and it length is 2.")
     else:
         return 'SELECT {} FROM `{}` {}'.format(fields, table, where)
 
 
-@lru_cache(maxsize=CONFIG_DICT[CACHE_SIZE])
+@lru_cache(maxsize=CACHE_SIZE)
 def _get_table_columns(table: str):
-    return do_get_limit(COLUMN_SQL, table, LIMIT_1)
+    return db.do_get_limit(COLUMN_SQL, table, LIMIT_1)
 
 
 def _get_condition_arg(k: str, v: object):
     if k.endswith("__eq"):
         return "{}=?".format(k[:-4]), v
     if k.endswith("__ne"):
         return "{}!=?".format(k[:-4]), v
```

### Comparing `mysqlx-1.5.6/mysqlx/snowflake.py` & `mysqlx-1.5.7/mysqlx/snowflake.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.6/mysqlx/sql_holder.py` & `mysqlx-1.5.7/mysqlx/sql_holder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import re
 from typing import Mapping
 from jinja2 import Template
-from log_support import logger
-from support import get_named_sql_args, SqlModel, MapperError, is_dynamic_sql, SqlAction
+from .log_support import logger
+from .support import  SqlModel, MapperError, SqlAction
+from .sql_support import get_named_sql_args, is_dynamic_sql
 
 try:
     import xml.etree.cElementTree as ET
 except ImportError:
     import xml.etree.ElementTree as ET
 
 _SQL_CONTAINER = dict()
@@ -134,20 +135,20 @@
     assert sql_id not in _SQL_CONTAINER, "Sql id '%s' repeat." % sql_id
     include = child.attrib.get('include')
     sql = child.text.strip()
     if include:
         includes = include.split(",")
         for include in set(includes):
             assert include != _id, "Include must not be it self, id: '%s' = include: '%s' " % (_id, include)
-        _SQL_CONTAINER[sql_id] = SqlModel(sql=sql, action=child.tag, namespace=namespace, includes=includes, pk_seq=child.attrib.get('pk_seq'))
+        _SQL_CONTAINER[sql_id] = SqlModel(sql=sql, action=child.tag, namespace=namespace, includes=includes)
     elif is_dynamic_sql(sql):
         _valid_sql(sql_id, sql, child.tag)
-        _SQL_CONTAINER[sql_id] = SqlModel(sql=sql, action=child.tag, namespace=namespace, dynamic=True, pk_seq=child.attrib.get('pk_seq'))
+        _SQL_CONTAINER[sql_id] = SqlModel(sql=sql, action=child.tag, namespace=namespace, dynamic=True)
     else:
         _valid_sql(sql_id, sql, child.tag)
-        _SQL_CONTAINER[sql_id] = SqlModel(sql=sql, action=child.tag, namespace=namespace, pk_seq=child.attrib.get('pk_seq'))
+        _SQL_CONTAINER[sql_id] = SqlModel(sql=sql, action=child.tag, namespace=namespace)
 
     return _id, includes
 
 
 def _valid_sql(sql_id, sql, tag):
     assert tag in _valid_sql_actions and tag in sql.lower(), "Sql id: '{}' has not '{}' key word in {} sql.".format(sql_id, tag, tag)
```

### Comparing `mysqlx-1.5.6/mysqlx/sql_mapper.py` & `mysqlx-1.5.7/mysqlx/sql_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import functools
+from .support import SqlAction
 from .log_support import logger
-from .dbx import get_sql_model, do_get_sql, build_sql_id
-from .support import SqlAction, get_named_sql_args, simple_sql, MapperError
+from .sql_support import get_named_sql_args, simple_sql
+from .sql_holder import get_sql_model, do_get_sql, build_sql_id
 from .db import do_get, do_query, do_query_one, do_execute, do_batch_execute, do_select, do_select_one, batch_execute, do_save
 
 _UPDATE_ACTIONS = (SqlAction.INSERT.value, SqlAction.UPDATE.value, SqlAction.DELETE.value, SqlAction.CALL.value)
 
 
 def mapper(namespace: str = None, sql_id: str = None, batch=False, return_pk=False):
     def _decorator(func):
```

### Comparing `mysqlx-1.5.6/mysqlx.egg-info/PKG-INFO` & `mysqlx-1.5.7/mysqlx.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.5.6
+Version: 1.5.7
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
@@ -142,10 +142,12 @@
    def test_transaction2():
        with transaction():
            insert_func(....)
            update_func(....)
 
 You can generate model class with mysqlx-generator: https://pypi.org/project/mysqlx-generator
 
-If you want to operate PostgreSQL database, you may need PgSqlx: https://pypi.org/project/pgsqlx/
+If you want to operate PostgreSQL database, you may need PgSqlx: https://pypi.org/project/pgsqlx
+
+If you just wanted a simple sql executor, you may need sqlx-exec: https://pypi.org/project/sqlx-exec
```

### Comparing `mysqlx-1.5.6/PKG-INFO` & `mysqlx-1.5.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.5.6
+Version: 1.5.7
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
@@ -142,10 +142,12 @@
    def test_transaction2():
        with transaction():
            insert_func(....)
            update_func(....)
 
 You can generate model class with mysqlx-generator: https://pypi.org/project/mysqlx-generator
 
-If you want to operate PostgreSQL database, you may need PgSqlx: https://pypi.org/project/pgsqlx/
+If you want to operate PostgreSQL database, you may need PgSqlx: https://pypi.org/project/pgsqlx
+
+If you just wanted a simple sql executor, you may need sqlx-exec: https://pypi.org/project/sqlx-exec
```

### Comparing `mysqlx-1.5.6/README.rst` & `mysqlx-1.5.7/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -129,8 +129,10 @@
    def test_transaction2():
        with transaction():
            insert_func(....)
            update_func(....)
 
 You can generate model class with mysqlx-generator: https://pypi.org/project/mysqlx-generator
 
-If you want to operate PostgreSQL database, you may need PgSqlx: https://pypi.org/project/pgsqlx/
+If you want to operate PostgreSQL database, you may need PgSqlx: https://pypi.org/project/pgsqlx
+
+If you just wanted a simple sql executor, you may need sqlx-exec: https://pypi.org/project/sqlx-exec
```

### Comparing `mysqlx-1.5.6/setup.py` & `mysqlx-1.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     description="MySqlx is a simple python sql executor for MySQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
         # 'mysql-connector-python>=8.0.13',
     ],
-    version='1.5.6',
+    version='1.5.7',
     url='https://gitee.com/summry/mysqlx',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

