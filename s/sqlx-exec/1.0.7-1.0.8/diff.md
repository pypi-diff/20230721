# Comparing `tmp/sqlx-exec-1.0.7.tar.gz` & `tmp/sqlx-exec-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.0.7.tar", last modified: Fri Jul 21 10:21:41 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.0.8.tar", last modified: Fri Jul 21 18:33:49 2023, max compression
```

## Comparing `sqlx-exec-1.0.7.tar` & `sqlx-exec-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 10:21:41.000000 sqlx-exec-1.0.7/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     2545 2023-07-21 10:21:41.000000 sqlx-exec-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2041 2023-07-21 10:21:29.000000 sqlx-exec-1.0.7/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-21 10:21:41.000000 sqlx-exec-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1160 2023-07-21 10:21:29.000000 sqlx-exec-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:21:41.000000 sqlx-exec-1.0.7/sqlexec/
--rw-rw-rw-   0        0        0      115 2023-07-21 07:43:22.000000 sqlx-exec-1.0.7/sqlexec/constant.py
--rw-rw-rw-   0        0        0     8940 2023-07-21 09:48:46.000000 sqlx-exec-1.0.7/sqlexec/exec.py
--rw-rw-rw-   0        0        0      496 2023-07-21 08:53:39.000000 sqlx-exec-1.0.7/sqlexec/log_support.py
--rw-rw-rw-   0        0        0     1521 2023-07-21 09:59:37.000000 sqlx-exec-1.0.7/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4008 2023-07-21 07:13:11.000000 sqlx-exec-1.0.7/sqlexec/support.py
--rw-rw-rw-   0        0        0      292 2023-07-21 08:34:59.000000 sqlx-exec-1.0.7/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:21:41.000000 sqlx-exec-1.0.7/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-21 10:21:41.000000 sqlx-exec-1.0.7/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-21 08:56:11.000000 sqlx-exec-1.0.7/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2545 2023-07-21 10:21:41.000000 sqlx-exec-1.0.7/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-21 10:21:41.000000 sqlx-exec-1.0.7/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-21 10:21:41.000000 sqlx-exec-1.0.7/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 18:33:49.000000 sqlx-exec-1.0.8/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2543 2023-07-21 18:33:49.000000 sqlx-exec-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2037 2023-07-21 18:03:00.000000 sqlx-exec-1.0.8/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-21 18:33:49.000000 sqlx-exec-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1161 2023-07-21 18:33:41.000000 sqlx-exec-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 18:33:49.000000 sqlx-exec-1.0.8/sqlexec/
+-rw-rw-rw-   0        0        0       95 2023-07-21 11:06:34.000000 sqlx-exec-1.0.8/sqlexec/engin.py
+-rw-rw-rw-   0        0        0    10239 2023-07-21 18:26:15.000000 sqlx-exec-1.0.8/sqlexec/exec.py
+-rw-rw-rw-   0        0        0     1018 2023-07-21 18:10:23.000000 sqlx-exec-1.0.8/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0     2786 2023-07-21 16:37:12.000000 sqlx-exec-1.0.8/sqlexec/pooling.py
+-rw-rw-rw-   0        0        0     2950 2023-07-21 18:26:15.000000 sqlx-exec-1.0.8/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4275 2023-07-21 16:54:46.000000 sqlx-exec-1.0.8/sqlexec/support.py
+-rw-rw-rw-   0        0        0      324 2023-07-21 18:17:34.000000 sqlx-exec-1.0.8/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 18:33:49.000000 sqlx-exec-1.0.8/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-21 18:33:49.000000 sqlx-exec-1.0.8/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-21 08:56:11.000000 sqlx-exec-1.0.8/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2543 2023-07-21 18:33:49.000000 sqlx-exec-1.0.8/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-07-21 18:33:49.000000 sqlx-exec-1.0.8/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-21 18:33:49.000000 sqlx-exec-1.0.8/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.0.7/LICENSE` & `sqlx-exec-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.0.7/PKG-INFO` & `sqlx-exec-1.0.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.0.7
-Summary: sqlx-exec is a simple sql executor for Python, it help you auto mange database connection and transaction.
+Version: 1.0.8
+Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
@@ -19,16 +19,17 @@
 
    import sqlexec
    from sqlexec import Engin
 
    if __name__ == '__main__':
        sqlexec.init_engin(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, engin=Engin.PostgreSQL)
 
-       id = sqlexec.save(pk_sql="SELECT currval('person_id_seq')", table='person', name='zhangsan', age=15)
-       id = sqlexec.save_sql("SELECT currval('person_id_seq')", 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
+       pk_sql = "SELECT currval('person_id_seq')"
+       id = sqlexec.save(pk_sql=pk_sql, table='person', name='zhangsan', age=15)
+       id = sqlexec.save_sql(pk_sql, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', id=5, name='wangwu', age=38)
 
        count = sqlexec.get('select count(1) from person')
        # result: 3
 
        persons = sqlexec.select('select id, name, age from person')
        # result:
```

### Comparing `sqlx-exec-1.0.7/README.rst` & `sqlx-exec-1.0.8/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 
    import sqlexec
    from sqlexec import Engin
 
    if __name__ == '__main__':
        sqlexec.init_engin(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, engin=Engin.PostgreSQL)
 
-       id = sqlexec.save(pk_sql="SELECT currval('person_id_seq')", table='person', name='zhangsan', age=15)
-       id = sqlexec.save_sql("SELECT currval('person_id_seq')", 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
+       pk_sql = "SELECT currval('person_id_seq')"
+       id = sqlexec.save(pk_sql=pk_sql, table='person', name='zhangsan', age=15)
+       id = sqlexec.save_sql(pk_sql, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', id=5, name='wangwu', age=38)
 
        count = sqlexec.get('select count(1) from person')
        # result: 3
 
        persons = sqlexec.select('select id, name, age from person')
        # result:
```

### Comparing `sqlx-exec-1.0.7/setup.py` & `sqlx-exec-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,18 @@
         return fp.read()
 
 long_description = read("README.rst")
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
-    description="sqlx-exec is a simple sql executor for Python, it help you auto mange database connection and transaction.",
+    description="sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.0.7',
+    version='1.0.8',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.0.7/sqlexec/exec.py` & `sqlx-exec-1.0.8/sqlexec/exec.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,66 @@
 import functools
 from . import sql_support
-from .constant import Engin
-from .log_support import logger, insert_log, do_sql_log
+from .engin import Engin
+from .log_support import logger, insert_log, save_log, get_log, page_log
 from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, DBError, DB_LOCK
 
 _DB_CTX = None
 
 
-def init_engin(connect=None, user='root', password='', database='test', host='127.0.0.1', port=3306, show_sql=False, engin=Engin.MySQL, **kwargs):
-    sql_support.set_engin(engin)
-    sql_support.set_show_sql(show_sql)
+def init_engin(connect=None, user='root', password='', database='test', host='127.0.0.1', port=3306, engin=Engin.MySQL, pool_size=1, show_sql=False, **kwargs):
+    sql_support.set_config(engin, show_sql)
     if 'debug' in kwargs:
         if kwargs.pop('debug'):
             from logging import DEBUG
             logger.setLevel(DEBUG)
 
     if connect:
         import types
         assert isinstance(connect, types.FunctionType), '`connect` must be a function, you can use like `connect=lambda: connect(**kwargs)`.'
-        _init_engin(connect)
+        _init_engin(connect, engin, pool_size, pool_size)
     else:
-        if engin == Engin.MySQL:
-            try:
-                from mysql.connector import connect
-            except ImportError:
-                from pymysql import connect
-        elif engin == Engin.PostgreSQL:
-            from psycopg2 import connect
-        else:
-            raise DBError('Engin is invalid: %s', engin)
-        kwargs['user'] = user
-        kwargs['password'] = password
-        kwargs['database'] = database
-        kwargs['host'] = host
-        kwargs['port'] = port
-        _init_engin(lambda: connect(**kwargs))
+        _import_init_engin(user, password, database, host, port, engin, pool_size, **kwargs)
+
+
+def _import_init_engin(user, password, database, host, port, engin, pool_size, **kwargs):
+    prepared = False
+    kwargs['user'] = user
+    kwargs['password'] = password
+    kwargs['database'] = database
+    kwargs['host'] = host
+    kwargs['port'] = port
+    real_size = pool_size
+    if engin == Engin.MySQL:
+        try:
+            from mysql.connector import connect
+            prepared = True
+            if pool_size > 0:
+                kwargs['pool_size'] = pool_size
+                if 'pool_name' not in kwargs:
+                    kwargs['pool_name'] = "{}_pool".format(database)
+                pool_size = 0
+        except ImportError:
+            from pymysql import connect
+    elif engin == Engin.PostgreSQL:
+        from psycopg2 import connect
+    else:
+        raise DBError('Engin is invalid: %s', engin)
+    _init_engin(lambda: connect(**kwargs), engin, pool_size, real_size, prepared)
 
 
-def _init_engin(connect):
+def _init_engin(connect, engin, pool_size, real_size, prepared=False):
     global _DB_CTX
     with DB_LOCK:
         if _DB_CTX is not None:
             raise DBError('DB is already initialized.')
 
-        _DB_CTX = DBCtx(connect=connect)
-        logger.info('Init db engine <%s> ok without connection pool.' % hex(id(_DB_CTX)))
+        from . import pooling
+        _DB_CTX = DBCtx(connect=pooling.get_connect(connect, pool_size) if pool_size>=1 else connect, pool_size=real_size, prepared=prepared)
+        logger.info('Init db engine <%s> of %s with pool size: %d.' % (hex(id(_DB_CTX)), engin.value, real_size))
 
 
 def connection():
     """
     Return _ConnectionCtx object that can be used by 'with' statement:
     with connection():
         pass
@@ -144,15 +156,15 @@
     """
     Insert data into table, return primary key.
     :param pk_sql: sql for getting primary key
     :param table: table
     :param kwargs:
     :return: Primary key
     """
-    insert_log('save', table, **kwargs)
+    save_log('save', pk_sql, table, **kwargs)
     sql, args = sql_support.insert_sql_args(table.strip(), **kwargs)
     return save_sql(pk_sql, sql, *args)
 
 
 @with_connection
 def save_sql(pk_sql: str, sql: str, *args):
     """
@@ -160,15 +172,16 @@
     :param pk_sql: sql for getting primary key
     :param sql: table
     :param args:
     :return: Primary key
     """
     global _DB_CTX
     cursor = None
-    sql = sql_support.before_execute('save', sql, *args)
+    logger.debug("Exec func 'sqlexec.%s', 'pk_sql': %s \n\t sql: '%s' \n\t args: %s" % ('save_sql', pk_sql, sql, args))
+    sql = sql_support.before_execute('save_sql', sql, *args)
     try:
         cursor = _DB_CTX.connection.cursor()
         cursor.execute(sql, args)
         cursor.execute(pk_sql)
         result = cursor.fetchone()
         try_commit(_DB_CTX)
         return result[0]
@@ -202,15 +215,15 @@
 
 def get(sql: str, *args):
     """
     Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
-    do_sql_log('get', sql, *args)
+    get_log('get', sql, *args)
     result = select_one(sql, *args)
     if result:
         if len(result) == 1:
             return result[0]
         msg = "Exec func 'sqlexec.%s' expect only one column but %d." % ('get', len(result))
         logger.error('%s  \n\t sql: %s \n\t args: %s' % (msg, sql, args))
         raise MultiColumnsError(msg)
@@ -249,14 +262,20 @@
         cursor.execute(sql, args)
         return cursor.fetchone()
     finally:
         if cursor:
             cursor.close()
 
 
+def select_page(sql: str, page_num, page_size, *args):
+    page_log('select_page', sql.strip(), page_num, page_size, args)
+    sql, args = sql_support.page_sql_args(sql, page_num, page_size, *args)
+    return select(sql, *args)
+
+
 @with_connection
 def query(sql: str, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     global _DB_CTX
@@ -294,13 +313,19 @@
             return Dict(names, result)
         return result
     finally:
         if cursor:
             cursor.close()
 
 
+def query_page(sql: str, page_num, page_size, *args):
+    page_log('query_page', sql.strip(), page_num, page_size, args)
+    sql, args = sql_support.page_sql_args(sql, page_num, page_size, *args)
+    return query(sql, *args)
+
+
 def get_connection():
     global _DB_CTX
     if _DB_CTX.is_not_init():
         _DB_CTX.init()
     return _DB_CTX.connection
```

### Comparing `sqlx-exec-1.0.7/sqlexec/sql_support.py` & `sqlx-exec-1.0.8/sqlexec/sql_support.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,16 @@
 from typing import Sequence
 from functools import lru_cache
 from .log_support import logger
-from .constant import CACHE_SIZE, Engin
+from .engin import Engin
 
+CACHE_SIZE = 256
 _SHOW_SQL = False
 _ENGIN = Engin.MySQL
-
-
-def set_engin(engin: Engin):
-    global _ENGIN
-    _ENGIN = engin
-
-
-def set_show_sql(show_sq: bool):
-    global _SHOW_SQL
-    _SHOW_SQL = show_sq
-
-
-def before_execute(function: str, sql: str, *args):
-    global _ENGIN
-    global _SHOW_SQL
-    if _SHOW_SQL:
-        logger.info("Exec func 'sqlexec.%s' \n\tSQL: %s \n\tARGS: %s" % (function, sql, args))
-
-    if _ENGIN == Engin.PostgreSQL and '%' in sql and 'like' in sql.lower():
-        sql = sql.replace('%', '%%').replace('%%%%', '%%')
-
-    return sql.replace('?', '%s')
+before_execute = None
 
 
 def insert_sql_args(table: str, **kwargs):
     cols, args = zip(*kwargs.items())
     sql = _create_insert_sql(table, cols)
     return sql, args
 
@@ -45,8 +25,68 @@
     return 'INSERT INTO {}({}) VALUES({})'.format(table, ','.join(columns), ','.join(placeholders))
 
 
 def get_batch_args(*args):
     return args[0] if isinstance(args, tuple) and len(args) == 1 and isinstance(args[0], Sequence) else args
 
 
+def page_sql_args(sql: str, page_num=1, page_size=10, *args):
+    global _ENGIN
+    start = (page_num - 1) * page_size
+    if require_limit(sql):
+        if _ENGIN == Engin.MySQL:
+            sql = '{} limit ?,?'.format(sql)
+            args = [*args, start, page_size]
+        elif _ENGIN == Engin.PostgreSQL:
+            sql = '{} LIMIT ? OFFSET ?'.format(sql)
+            args = [*args, page_size, start]
+    return sql, args
+
+
+def require_limit(sql: str):
+    lower_sql = sql.lower()
+    if 'limit' not in lower_sql:
+        return True
+    idx = lower_sql.rindex('limit')
+    if idx > 0 and ')' in lower_sql[idx:]:
+        return True
+    return False
+
+
+def set_config(engin, show_sql):
+    global _ENGIN
+    global _SHOW_SQL
+    global before_execute
+    _ENGIN = engin
+    _ENGIN = engin
+    _SHOW_SQL = show_sql
+    if engin == Engin.PostgreSQL:
+        if show_sql:
+            before_execute =before_execute_postgres_show_sql
+        else:
+            before_execute = before_execute_postgres
+    else:
+        if show_sql:
+            before_execute = before_execute_default_show_sql
+        else:
+            before_execute = lambda function, sql, *args: sql.replace('?', '%s')
+
+
+def before_execute_default_show_sql(function: str, sql: str, *args):
+    logger.info("Exec func 'sqlexec.%s' \n\tSQL: %s \n\tARGS: %s" % (function, sql, args))
+    return sql.replace('?', '%s')
+
+
+def before_execute_postgres(function: str, sql: str, *args):
+    if '%' in sql and 'like' in sql.lower():
+        sql = sql.replace('%', '%%').replace('%%%%', '%%')
+    return sql.replace('?', '%s')
+
+
+def before_execute_postgres_show_sql(function: str, sql: str, *args):
+    logger.info("Exec func 'sqlexec.%s' \n\tSQL: %s \n\tARGS: %s" % (function, sql, args))
+    if '%' in sql and 'like' in sql.lower():
+        sql = sql.replace('%', '%%').replace('%%%%', '%%')
+    return sql.replace('?', '%s')
+
+
```

### Comparing `sqlx-exec-1.0.7/sqlexec/support.py` & `sqlx-exec-1.0.8/sqlexec/support.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import threading
-from .log_support import logger
+from .log_support import logger, db_ctx_log
 
 DB_LOCK = threading.RLock()
 
 
 def try_commit(db_ctx):
     if db_ctx.transactions == 0:
         logger.debug('Commit transaction...')
@@ -18,21 +18,20 @@
 
 
 class DBCtx(threading.local):
     """
     Thread local object that holds connection info.
     """
 
-    def __init__(self, connect):
+    def __init__(self, connect, pool_size, prepared=False):
         self.connect = connect
         self.connection = None
         self.transactions = 0
-        self.prepared = True
-        self.get_cursor = lambda: self.connection.cursor()
-        self.log = lambda action: logger.debug('%s connection <%s>...' % (action, hex(id(self.connection))))
+        self.pool_size = pool_size
+        self.prepared = prepared
 
     def is_not_init(self):
         return self.connection is None
 
     def init(self):
         self.transactions = 0
         self.connection = self.connect()
@@ -45,22 +44,29 @@
             self.connection = None
 
     def cursor(self):
         """
         Return cursor
         """
         # logger.debug('Cursor prepared: %s' % self.prepared)
-        return self.get_cursor()
+        return self.connection.cursor(prepared=True) if self.prepared else self.connection.cursor()
 
     def statement(self, sql: str):
         """
         Return statement
         """
         return self.connection.statement(sql)
 
+    def log(self, action: str):
+        if self.prepared and self.pool_size >= 1:
+            db_ctx_log(action, self.connection._cnx)
+        elif self.pool_size >= 1:
+            db_ctx_log(action, self.connection.conn)
+        else:
+            db_ctx_log(action, self.connection)
 
 class ConnectionCtx(object):
     """
     ConnectionCtx object that can open and close connection context. ConnectionCtx object can be nested and only the most
     outer connection has effect.
     with connection():
         pass
```

### Comparing `sqlx-exec-1.0.7/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.0.8/sqlx_exec.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.0.7
-Summary: sqlx-exec is a simple sql executor for Python, it help you auto mange database connection and transaction.
+Version: 1.0.8
+Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
@@ -19,16 +19,17 @@
 
    import sqlexec
    from sqlexec import Engin
 
    if __name__ == '__main__':
        sqlexec.init_engin(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, engin=Engin.PostgreSQL)
 
-       id = sqlexec.save(pk_sql="SELECT currval('person_id_seq')", table='person', name='zhangsan', age=15)
-       id = sqlexec.save_sql("SELECT currval('person_id_seq')", 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
+       pk_sql = "SELECT currval('person_id_seq')"
+       id = sqlexec.save(pk_sql=pk_sql, table='person', name='zhangsan', age=15)
+       id = sqlexec.save_sql(pk_sql, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', id=5, name='wangwu', age=38)
 
        count = sqlexec.get('select count(1) from person')
        # result: 3
 
        persons = sqlexec.select('select id, name, age from person')
        # result:
```

