# Comparing `tmp/pgsqlx-1.0.8.tar.gz` & `tmp/pgsqlx-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pgsqlx-1.0.8.tar", last modified: Wed Jul 19 06:54:59 2023, max compression
+gzip compressed data, was "dist\pgsqlx-1.0.9.tar", last modified: Fri Jul 21 10:08:16 2023, max compression
```

## Comparing `pgsqlx-1.0.8.tar` & `pgsqlx-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 06:54:59.000000 pgsqlx-1.0.8/
-drwxrwxrwx   0        0        0        0 2023-07-19 06:54:59.000000 pgsqlx-1.0.8/pgsqlx/
--rw-rw-rw-   0        0        0      239 2023-07-19 06:33:03.000000 pgsqlx-1.0.8/pgsqlx/config_holder.py
--rw-rw-rw-   0        0        0      561 2023-07-19 05:39:26.000000 pgsqlx-1.0.8/pgsqlx/constant.py
--rw-rw-rw-   0        0        0    19514 2023-07-19 06:33:03.000000 pgsqlx-1.0.8/pgsqlx/db.py
--rw-rw-rw-   0        0        0     7471 2023-07-19 06:33:02.000000 pgsqlx-1.0.8/pgsqlx/dbx.py
--rw-rw-rw-   0        0        0     3984 2023-07-13 13:31:18.000000 pgsqlx-1.0.8/pgsqlx/log_support.py
--rw-rw-rw-   0        0        0    38451 2023-07-19 06:53:41.000000 pgsqlx-1.0.8/pgsqlx/orm.py
--rw-rw-rw-   0        0        0     2392 2023-07-19 06:32:34.000000 pgsqlx-1.0.8/pgsqlx/snowflake.py
--rw-rw-rw-   0        0        0     6386 2023-07-19 06:33:03.000000 pgsqlx-1.0.8/pgsqlx/sql_holder.py
--rw-rw-rw-   0        0        0     5113 2023-07-19 06:33:02.000000 pgsqlx-1.0.8/pgsqlx/sql_mapper.py
--rw-rw-rw-   0        0        0     6511 2023-07-19 06:33:02.000000 pgsqlx-1.0.8/pgsqlx/support.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 pgsqlx-1.0.8/pgsqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 06:54:59.000000 pgsqlx-1.0.8/pgsqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-19 06:54:59.000000 pgsqlx-1.0.8/pgsqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-19 06:54:59.000000 pgsqlx-1.0.8/pgsqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4268 2023-07-19 06:54:59.000000 pgsqlx-1.0.8/pgsqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       30 2023-07-19 06:54:59.000000 pgsqlx-1.0.8/pgsqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      402 2023-07-19 06:54:59.000000 pgsqlx-1.0.8/pgsqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-19 06:54:59.000000 pgsqlx-1.0.8/pgsqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4268 2023-07-19 06:54:59.000000 pgsqlx-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3758 2023-07-16 02:24:38.000000 pgsqlx-1.0.8/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-19 06:54:59.000000 pgsqlx-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1203 2023-07-19 06:54:56.000000 pgsqlx-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 10:08:16.000000 pgsqlx-1.0.9/
+drwxrwxrwx   0        0        0        0 2023-07-21 10:08:16.000000 pgsqlx-1.0.9/pgsqlx/
+-rw-rw-rw-   0        0        0      552 2023-07-19 13:24:36.000000 pgsqlx-1.0.9/pgsqlx/constant.py
+-rw-rw-rw-   0        0        0    17295 2023-07-21 06:06:21.000000 pgsqlx-1.0.9/pgsqlx/db.py
+-rw-rw-rw-   0        0        0     7496 2023-07-19 13:34:57.000000 pgsqlx-1.0.9/pgsqlx/dbx.py
+-rw-rw-rw-   0        0        0     3984 2023-07-13 13:31:18.000000 pgsqlx-1.0.9/pgsqlx/log_support.py
+-rw-rw-rw-   0        0        0    38425 2023-07-19 13:46:35.000000 pgsqlx-1.0.9/pgsqlx/orm.py
+-rw-rw-rw-   0        0        0     2392 2023-07-19 06:32:34.000000 pgsqlx-1.0.9/pgsqlx/snowflake.py
+-rw-rw-rw-   0        0        0     6412 2023-07-19 13:34:08.000000 pgsqlx-1.0.9/pgsqlx/sql_holder.py
+-rw-rw-rw-   0        0        0     5138 2023-07-19 13:36:00.000000 pgsqlx-1.0.9/pgsqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0     3752 2023-07-21 08:20:35.000000 pgsqlx-1.0.9/pgsqlx/sql_support.py
+-rw-rw-rw-   0        0        0     4737 2023-07-19 14:00:04.000000 pgsqlx-1.0.9/pgsqlx/support.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 pgsqlx-1.0.9/pgsqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 10:08:16.000000 pgsqlx-1.0.9/pgsqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-21 10:08:16.000000 pgsqlx-1.0.9/pgsqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-21 10:08:16.000000 pgsqlx-1.0.9/pgsqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4413 2023-07-21 10:08:16.000000 pgsqlx-1.0.9/pgsqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2023-07-21 10:08:16.000000 pgsqlx-1.0.9/pgsqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      400 2023-07-21 10:08:16.000000 pgsqlx-1.0.9/pgsqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-21 10:08:16.000000 pgsqlx-1.0.9/pgsqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4413 2023-07-21 10:08:16.000000 pgsqlx-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3900 2023-07-21 10:07:42.000000 pgsqlx-1.0.9/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-21 10:08:16.000000 pgsqlx-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1203 2023-07-21 10:07:42.000000 pgsqlx-1.0.9/setup.py
```

### Comparing `pgsqlx-1.0.8/pgsqlx/constant.py` & `pgsqlx-1.0.9/pgsqlx/constant.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-CACHE_SIZE = 'cache_size'
+CACHE_SIZE = 256
 
 LIMIT_1 = 1
 
 NO_LIMIT = 0
 
 NAMED_REGEX = r':[\w|\d]*'
```

### Comparing `pgsqlx-1.0.8/pgsqlx/db.py` & `pgsqlx-1.0.9/pgsqlx/db.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,44 @@
 import functools
-from typing import Sequence
-from .config_holder import set_config
-from .constant import LIMIT_1, MAPPER_PATH, CACHE_SIZE
+from . import sql_support
+from .constant import MAPPER_PATH
 from .log_support import logger, sql_log, page_log, insert_log, do_sql_log, do_page_log
-from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, dynamic_sql, get_named_sql, get_named_args, DBError, \
-    DB_LOCK, get_batch_args
+from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, DBError, DB_LOCK
 
 _DB_CTX = None
-_SHOW_SQL = False
 
 
 def init_db(user='root', password='', database='test', host='127.0.0.1', port=3306, show_sql=False, **kwargs):
-    global _DB_CTX
-    global _SHOW_SQL
-    from psycopg2  import connect
-
-    _SHOW_SQL = show_sql
     kwargs['user'] = user
     kwargs['password'] = password
     kwargs['database'] = database
     kwargs['host'] = host
     kwargs['port'] = port
+    sql_support.set_show_sql(show_sql)
 
     if 'debug' in kwargs:
         if kwargs.pop('debug'):
             from logging import DEBUG
             logger.setLevel(DEBUG)
 
-    if CACHE_SIZE in kwargs:
-        set_config(CACHE_SIZE, kwargs.pop(CACHE_SIZE))
+    _init_db(**kwargs)
 
+
+def _init_db(**kwargs):
+    global _DB_CTX
+    from psycopg2 import connect
     with DB_LOCK:
         if _DB_CTX is not None:
             raise DBError('DB is already initialized.')
 
         if MAPPER_PATH in kwargs:
             from .sql_holder import load_mapper
             load_mapper(kwargs.pop(MAPPER_PATH))
 
-        _DB_CTX = DBCtx(connect=lambda: connect(**kwargs), is_pool=False)
+        _DB_CTX = DBCtx(connect=lambda: connect(**kwargs))
         logger.info('Init db engine <%s> ok without connection pool.' % hex(id(_DB_CTX)))
 
 
 def connection():
     """
     Return _ConnectionCtx object that can be used by 'with' statement:
     with connection():
@@ -108,15 +104,15 @@
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
     Default primary key sequnece is 'table_id_seq', you can use 'pk_seq' define it
@@ -125,15 +121,15 @@
     :return: Primary key
     """
     insert_log('save', table, **kwargs)
     if 'pk_seq' in kwargs:
         pk_seq = kwargs.pop('pk_seq')
     else:
         pk_seq = "{}_id_seq".format(table)
-    sql, args = _insert_sql_args(table.strip(), **kwargs)
+    sql, args = sql_support.insert_sql_args(table.strip(), **kwargs)
     return do_save(pk_seq, sql, *args)
 
 
 @with_connection
 def do_save(pk_seq: str, sql: str, *args):
     """
     Insert data into table, return primary key.
@@ -141,15 +137,15 @@
     :param sql: table
     :param args:
     :return: Primary key
     """
     global _DB_CTX
     cursor = None
     logger.debug("Exec func 'mysqlx.db.%s': pk_seq: '%s'\n\tsql: '%s'\n\targs: %s" % ('do_save', pk_seq, sql, args))
-    sql = _before_execute('do_save', sql, *args)
+    sql = sql_support.before_execute('do_save', sql, *args)
     try:
         cursor = _DB_CTX.connection.cursor()
         cursor.execute(sql, args)
         cursor.execute("SELECT currval('{}')".format(pk_seq))
         result = cursor.fetchone()
         try_commit(_DB_CTX)
         return result[0]
@@ -161,141 +157,141 @@
 def execute(sql: str, *args, **kwargs):
     """
     Execute SQL.
     sql: INSERT INTO person(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
          INSERT INTO person(name, age) VALUES(:name,:age)  -->  kwargs: {'name': '张三', 'age': 20}
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
     :param sql: INSERT INTO person(name, age) VALUES(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
                 INSERT INTO person(name, age) VALUES(:name,:age)  -->  args: [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
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
     sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
          SELECT count(1) FROM person WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     sql_log('get', sql, *args, **kwargs)
     global _DB_CTX
-    sql, args = dynamic_sql(sql, *args, **kwargs)
+    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
     return do_get(sql, *args)
 
 
 def query(sql: str, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result.
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM person WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
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
     sql: SELECT * FROM person WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
          SELECT * FROM person WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     sql_log('query_one', sql, *args, **kwargs)
-    sql, args = dynamic_sql(sql, *args, **kwargs)
+    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
     return do_query_one(sql, *args)
 
 
 def select(sql: str, *args, **kwargs):
     """
     Execute select SQL and return list(tuple) or empty list if no result.
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM person WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
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
     sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
          SELECT * FROM person WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     sql_log('select_one', sql, *args, **kwargs)
-    sql, args = dynamic_sql(sql, *args, **kwargs)
+    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
     return do_select_one(sql, *args)
 
 
 def query_page(sql: str, page_num=1, page_size=10, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM person WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     page_log('query_page', sql, page_num, page_size, *args, **kwargs)
-    sql, args = dynamic_sql(sql, *args, **kwargs)
+    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
     return do_query_page(sql, page_num, page_size, *args)
 
 
 def select_page(sql: str, page_num=1, page_size=10, *args, **kwargs):
     """
     Execute select SQL and return list(tuple) or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM person WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
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
     sql: insert into person(name, age) values(?, ?)  -->  args: ('张三', 20)
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
@@ -309,16 +305,16 @@
     Batch execute sql return effect rowcount
     :param sql: insert into person(name, age) values(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
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
@@ -329,15 +325,15 @@
 def do_get(sql: str, *args):
     """
     Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' behind the sql statement if not.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     do_sql_log('do_get', sql, *args)
-    sql, args = _limit_one_sql_args(sql, *args)
+    sql, args = sql_support.limit_one_sql_args(sql, *args)
     return do_get_limit(sql, *args)
 
 
 def do_get_limit(sql: str, *args):
     """
     Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
     MultiColumnsError: Expect only one column.
@@ -352,21 +348,21 @@
         logger.error('%s  \n\t sql: %s \n\t args: %s' % (msg, sql, args))
         raise MultiColumnsError(msg)
     return None
 
 
 @with_connection
 def do_query(sql: str, *args):
-    """sql = {str} "SELECT id,name,grade,create_time FROM person WHERE id in(1,4) and name like '张三%' and grade>=1 and create_time between '2023-06-07 10:48:01' and '2023-06-07 10:48:06'"
+    """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = _before_select('do_query', sql.strip(), *args)
+    sql = sql_support.before_select('do_query', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         results = cursor.fetchall()
         if results and cursor.description:
             names = [x[0] for x in cursor.description]
             return [Dict(names, x) for x in results]
@@ -379,27 +375,27 @@
 
 def do_query_one(sql: str, *args):
     """
     execute select SQL and return unique result(dict). Automatically add 'limit ?' behind the sql statement if not.
     sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     do_sql_log('do_query_one', sql, *args)
-    sql, args = _limit_one_sql_args(sql, *args)
+    sql, args = sql_support.limit_one_sql_args(sql, *args)
     return do_query_one_limit(sql, *args)
 
 
 @with_connection
 def do_query_one_limit(sql: str, *args):
     """
     execute select SQL and return unique result(dict), SQL contain 'limit'.
     sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = _before_select('do_query_one_limit', sql.strip(), *args)
+    sql = sql_support.before_select('do_query_one_limit', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         result = cursor.fetchone()
         if result and cursor.description:
             names = [x[0] for x in cursor.description]
             return Dict(names, result)
@@ -413,15 +409,15 @@
 def do_select(sql: str, *args):
     """
     execute select SQL and return unique result or list results(tuple).
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = _before_select('do_select', sql.strip(), *args)
+    sql = sql_support.before_select('do_select', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         return cursor.fetchall()
     finally:
         if cursor:
             cursor.close()
@@ -429,27 +425,27 @@
 
 def do_select_one(sql: str, *args):
     """
     Execute select SQL and return unique result(tuple). Automatically add 'limit ?' behind the sql statement if not.
     sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     do_sql_log('do_select_one', sql, *args)
-    sql, args = _limit_one_sql_args(sql, *args)
+    sql, args = sql_support.limit_one_sql_args(sql, *args)
     return do_select_one_limit(sql, *args)
 
 
 @with_connection
 def do_select_one_limit(sql: str, *args):
     """
     Execute select SQL and return unique result(tuple), SQL contain 'limit'.
     sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = _before_select('do_select_one_limit', sql.strip(), *args)
+    sql = sql_support.before_select('do_select_one_limit', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         return cursor.fetchone()
     finally:
         if cursor:
             cursor.close()
@@ -457,103 +453,31 @@
 
 def do_query_page(sql: str, page_num=1, page_size=10, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     do_page_log('do_query_page', sql, page_num, page_size, args)
-    sql, args = _page_sql_args(sql, page_num, page_size, *args)
+    sql, args = sql_support.page_sql_args(sql, page_num, page_size, *args)
     return do_query(sql, *args)
 
 
 def do_select_page(sql: str, page_num=1, page_size=10, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
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
-def _before_select(function: str, sql: str, *args):
-    global _SHOW_SQL
-    if _SHOW_SQL:
-        logger.info("Exec func 'mysqlx.db.%s' \n\tSQL: %s \n\tARGS: %s" % (function, sql, args))
-
-    if '%' in sql and 'like' in sql.lower():
-        sql = sql.replace('%', '%%').replace('%%%%', '%%')
-
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
-    columns, placeholders = zip(*[('{}'.format(col), '?') for col in cols])
-    return 'INSERT INTO {} ({}) VALUES ({})'.format(table, ','.join(columns), ','.join(placeholders))
-
-
-def _page_sql_args(sql: str, page_num=1, page_size=10, *args):
-    start = (page_num - 1) * page_size
-    args = [*args, page_size, start]
-    if _require_limit(sql):
-        sql = '{} LIMIT ? OFFSET ?'.format(sql)
-    return sql, args
-
-
-def _limit_one_sql_args(sql: str, *args):
-    if _require_limit(sql):
-        return '{} LIMIT ?'.format(sql), [*args, LIMIT_1]
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

### Comparing `pgsqlx-1.0.8/pgsqlx/dbx.py` & `pgsqlx-1.0.9/pgsqlx/dbx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 from . import db
+from .support import SqlAction
 from . import sql_holder as holder
-from .support import get_batch_args, SqlAction
+from .sql_support import get_batch_args
 from .log_support import logger, sql_id_log, page_sql_id_log
 
 
 def init_db(user='root', password='', database='test', host='127.0.0.1', port=3306, show_sql=False, mapper_path='mapper', **kwargs):
     holder.load_mapper(mapper_path)
     db.init_db(user, password, database, host, port, show_sql, **kwargs)
```

### Comparing `pgsqlx-1.0.8/pgsqlx/log_support.py` & `pgsqlx-1.0.9/pgsqlx/log_support.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.8/pgsqlx/orm.py` & `pgsqlx-1.0.9/pgsqlx/orm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import sys
 from . import db
 from . import log_support
 from datetime import datetime
 from .snowflake import get_id
 from enum import Enum, IntEnum
 from functools import lru_cache
-from .config_holder import get_config
+from .sql_support import simple_sql
+from .support import DBError, NotFoundError
 from typing import Sequence, Union, List, Tuple
-from .support import DBError, simple_sql, NotFoundError
 from .constant import LIMIT_1, NO_LIMIT, DEFAULT_PK_FIELD, PK, PK_SEQ, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, PK_STRATEGY, COLUMN_SQL, CACHE_SIZE
 
 
 class DelFlag(IntEnum):
     UN_DELETE = 0
     DELETED = 1
 
@@ -822,15 +822,15 @@
             return 'SELECT {} FROM {} {} LIMIT ? OFFSET ?'.format(fields, table, where)
         else:
             raise ValueError("The type of the parameter 'limit' must be 'int' or tuple, list, and it length is 2.")
     else:
         return 'SELECT {} FROM {} {}'.format(fields, table, where)
 
 
-@lru_cache(maxsize=get_config(CACHE_SIZE))
+@lru_cache(maxsize=CACHE_SIZE)
 def _get_table_columns(table: str):
     return db.do_get_limit(COLUMN_SQL, table, LIMIT_1)
 
 
 def _get_condition_arg(k: str, v: object):
     if k.endswith("__eq"):
         return "{}=?".format(k[:-4]), v
```

### Comparing `pgsqlx-1.0.8/pgsqlx/snowflake.py` & `pgsqlx-1.0.9/pgsqlx/snowflake.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.8/pgsqlx/sql_holder.py` & `pgsqlx-1.0.9/pgsqlx/sql_holder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import re
 from typing import Mapping
 from jinja2 import Template
 from .log_support import logger
-from .support import get_named_sql_args, SqlModel, MapperError, is_dynamic_sql, SqlAction
+from .support import  SqlModel, MapperError, SqlAction
+from .sql_support import get_named_sql_args, is_dynamic_sql
 
 try:
     import xml.etree.cElementTree as ET
 except ImportError:
     import xml.etree.ElementTree as ET
 
 _SQL_CONTAINER = dict()
```

### Comparing `pgsqlx-1.0.8/pgsqlx/sql_mapper.py` & `pgsqlx-1.0.9/pgsqlx/sql_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import re
 import functools
+from .support import SqlAction
 from .log_support import logger
+from .sql_support import get_named_sql_args, simple_sql
 from .sql_holder import get_sql_model, do_get_sql, build_sql_id
-from .support import SqlAction, get_named_sql_args, simple_sql
 from .db import do_get, do_query, do_query_one, do_execute, do_batch_execute, do_select, do_select_one, batch_execute, do_save
 
 _UPDATE_ACTIONS = (SqlAction.INSERT.value, SqlAction.UPDATE.value, SqlAction.DELETE.value, SqlAction.CALL.value)
 
 
 def mapper(namespace: str = None, sql_id: str = None, batch=False, return_pk=False):
     def _decorator(func):
```

### Comparing `pgsqlx-1.0.8/pgsqlx.egg-info/PKG-INFO` & `pgsqlx-1.0.9/pgsqlx.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.0.8
+Version: 1.0.9
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -106,14 +106,15 @@
        # result:
        # (3, 'zhangsan', 15)
        
        # you can use orm to operate a single table
        class person(Model):
            __pk__ = 'id'
            __table__ = 'person'
+           __pk_seq__ = 'person_id_seq'
 
            def __init__(self, id: int = None, name: str = None, age: int = None):
                self.id = id
                self.name = name
                self.age = age
                      
        persons = person.query()
@@ -143,8 +144,10 @@
        with transaction():
            insert_func(....)
            update_func(....)
 
 
 If you want to operate MySQL database, you may need MySqlx: https://pypi.org/project/mysqlx
 
+If you just wanted a simple sql executor, you may need sqlx-exec: https://pypi.org/project/sqlx-exec
+
```

### Comparing `pgsqlx-1.0.8/PKG-INFO` & `pgsqlx-1.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.0.8
+Version: 1.0.9
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -106,14 +106,15 @@
        # result:
        # (3, 'zhangsan', 15)
        
        # you can use orm to operate a single table
        class person(Model):
            __pk__ = 'id'
            __table__ = 'person'
+           __pk_seq__ = 'person_id_seq'
 
            def __init__(self, id: int = None, name: str = None, age: int = None):
                self.id = id
                self.name = name
                self.age = age
                      
        persons = person.query()
@@ -143,8 +144,10 @@
        with transaction():
            insert_func(....)
            update_func(....)
 
 
 If you want to operate MySQL database, you may need MySqlx: https://pypi.org/project/mysqlx
 
+If you just wanted a simple sql executor, you may need sqlx-exec: https://pypi.org/project/sqlx-exec
+
```

### Comparing `pgsqlx-1.0.8/README.rst` & `pgsqlx-1.0.9/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -93,14 +93,15 @@
        # result:
        # (3, 'zhangsan', 15)
        
        # you can use orm to operate a single table
        class person(Model):
            __pk__ = 'id'
            __table__ = 'person'
+           __pk_seq__ = 'person_id_seq'
 
            def __init__(self, id: int = None, name: str = None, age: int = None):
                self.id = id
                self.name = name
                self.age = age
                      
        persons = person.query()
@@ -129,7 +130,9 @@
    def test_transaction2():
        with transaction():
            insert_func(....)
            update_func(....)
 
 
 If you want to operate MySQL database, you may need MySqlx: https://pypi.org/project/mysqlx
+
+If you just wanted a simple sql executor, you may need sqlx-exec: https://pypi.org/project/sqlx-exec
```

### Comparing `pgsqlx-1.0.8/setup.py` & `pgsqlx-1.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     description="PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
         'psycopg2>=2.7.4',
     ],
-    version='1.0.8',
+    version='1.0.9',
     url='https://gitee.com/summry/pgsqlx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

