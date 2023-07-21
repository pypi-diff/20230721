# Comparing `tmp/sqlx-exec-1.0.8.tar.gz` & `tmp/sqlx-exec-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.0.8.tar", last modified: Fri Jul 21 18:33:49 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.0.9.tar", last modified: Fri Jul 21 21:29:43 2023, max compression
```

## Comparing `sqlx-exec-1.0.8.tar` & `sqlx-exec-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 18:33:49.000000 sqlx-exec-1.0.8/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     2543 2023-07-21 18:33:49.000000 sqlx-exec-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2037 2023-07-21 18:03:00.000000 sqlx-exec-1.0.8/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-21 18:33:49.000000 sqlx-exec-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1161 2023-07-21 18:33:41.000000 sqlx-exec-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 18:33:49.000000 sqlx-exec-1.0.8/sqlexec/
--rw-rw-rw-   0        0        0       95 2023-07-21 11:06:34.000000 sqlx-exec-1.0.8/sqlexec/engin.py
--rw-rw-rw-   0        0        0    10239 2023-07-21 18:26:15.000000 sqlx-exec-1.0.8/sqlexec/exec.py
--rw-rw-rw-   0        0        0     1018 2023-07-21 18:10:23.000000 sqlx-exec-1.0.8/sqlexec/log_support.py
--rw-rw-rw-   0        0        0     2786 2023-07-21 16:37:12.000000 sqlx-exec-1.0.8/sqlexec/pooling.py
--rw-rw-rw-   0        0        0     2950 2023-07-21 18:26:15.000000 sqlx-exec-1.0.8/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4275 2023-07-21 16:54:46.000000 sqlx-exec-1.0.8/sqlexec/support.py
--rw-rw-rw-   0        0        0      324 2023-07-21 18:17:34.000000 sqlx-exec-1.0.8/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 18:33:49.000000 sqlx-exec-1.0.8/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-21 18:33:49.000000 sqlx-exec-1.0.8/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-21 08:56:11.000000 sqlx-exec-1.0.8/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2543 2023-07-21 18:33:49.000000 sqlx-exec-1.0.8/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-07-21 18:33:49.000000 sqlx-exec-1.0.8/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-21 18:33:49.000000 sqlx-exec-1.0.8/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 21:29:43.000000 sqlx-exec-1.0.9/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     2537 2023-07-21 21:29:43.000000 sqlx-exec-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2031 2023-07-21 18:34:31.000000 sqlx-exec-1.0.9/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-21 21:29:43.000000 sqlx-exec-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1161 2023-07-21 21:29:09.000000 sqlx-exec-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:29:43.000000 sqlx-exec-1.0.9/sqlexec/
+-rw-rw-rw-   0        0        0     2441 2023-07-21 20:40:15.000000 sqlx-exec-1.0.9/sqlexec/engin.py
+-rw-rw-rw-   0        0        0    10749 2023-07-21 21:06:09.000000 sqlx-exec-1.0.9/sqlexec/exec.py
+-rw-rw-rw-   0        0        0     1018 2023-07-21 18:10:23.000000 sqlx-exec-1.0.9/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0     2786 2023-07-21 16:37:12.000000 sqlx-exec-1.0.9/sqlexec/pooling.py
+-rw-rw-rw-   0        0        0     1608 2023-07-21 21:27:49.000000 sqlx-exec-1.0.9/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4275 2023-07-21 16:54:46.000000 sqlx-exec-1.0.9/sqlexec/support.py
+-rw-rw-rw-   0        0        0      324 2023-07-21 18:17:34.000000 sqlx-exec-1.0.9/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:29:43.000000 sqlx-exec-1.0.9/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-21 21:29:43.000000 sqlx-exec-1.0.9/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-21 08:56:11.000000 sqlx-exec-1.0.9/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2537 2023-07-21 21:29:43.000000 sqlx-exec-1.0.9/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-07-21 21:29:43.000000 sqlx-exec-1.0.9/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-21 21:29:43.000000 sqlx-exec-1.0.9/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.0.8/LICENSE` & `sqlx-exec-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.0.8/PKG-INFO` & `sqlx-exec-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.0.8
+Version: 1.0.9
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
@@ -22,15 +22,15 @@
 
    if __name__ == '__main__':
        sqlexec.init_engin(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, engin=Engin.PostgreSQL)
 
        pk_sql = "SELECT currval('person_id_seq')"
        id = sqlexec.save(pk_sql=pk_sql, table='person', name='zhangsan', age=15)
        id = sqlexec.save_sql(pk_sql, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
-       rowcount = sqlexec.insert(table='person', id=5, name='wangwu', age=38)
+       rowcount = sqlexec.insert(table='person', name='wangwu', age=38)
 
        count = sqlexec.get('select count(1) from person')
        # result: 3
 
        persons = sqlexec.select('select id, name, age from person')
        # result:
        # (3, 'zhangsan', 15)
```

### Comparing `sqlx-exec-1.0.8/README.rst` & `sqlx-exec-1.0.9/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
    if __name__ == '__main__':
        sqlexec.init_engin(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, engin=Engin.PostgreSQL)
 
        pk_sql = "SELECT currval('person_id_seq')"
        id = sqlexec.save(pk_sql=pk_sql, table='person', name='zhangsan', age=15)
        id = sqlexec.save_sql(pk_sql, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
-       rowcount = sqlexec.insert(table='person', id=5, name='wangwu', age=38)
+       rowcount = sqlexec.insert(table='person', name='wangwu', age=38)
 
        count = sqlexec.get('select count(1) from person')
        # result: 3
 
        persons = sqlexec.select('select id, name, age from person')
        # result:
        # (3, 'zhangsan', 15)
```

### Comparing `sqlx-exec-1.0.8/setup.py` & `sqlx-exec-1.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.0.8',
+    version='1.0.9',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.0.8/sqlexec/exec.py` & `sqlx-exec-1.0.9/sqlexec/exec.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,28 +172,41 @@
     :param pk_sql: sql for getting primary key
     :param sql: table
     :param args:
     :return: Primary key
     """
     global _DB_CTX
     cursor = None
-    logger.debug("Exec func 'sqlexec.%s', 'pk_sql': %s \n\t sql: '%s' \n\t args: %s" % ('save_sql', pk_sql, sql, args))
+    logger.debug("Exec func 'sqlexec.%s', 'pk_sql': %s \n\t sql: %s \n\t args: %s" % ('save_sql', pk_sql, sql, args))
     sql = sql_support.before_execute('save_sql', sql, *args)
     try:
         cursor = _DB_CTX.connection.cursor()
         cursor.execute(sql, args)
         cursor.execute(pk_sql)
         result = cursor.fetchone()
         try_commit(_DB_CTX)
         return result[0]
     finally:
         if cursor:
             cursor.close()
 
 
+def batch_insert(table: str, *args):
+    """
+    Batch insert
+    :param table: table name
+    :param args: All number must have same key. [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
+    :return: Effect row count
+    """
+    logger.debug("Exec func 'sqlexec.%s' \n\t Table: '%s', args: %s" % ('batch_insert', table, args))
+    assert len(args) > 0, 'args should not be empty.'
+    sql, args = sql_support.batch_insert_sql_args(table, *args)
+    return batch_execute(sql, *args)
+
+
 @with_connection
 def batch_execute(sql: str, *args):
     """
     Batch execute sql return effect rowcount
     :param sql: insert into person(name, age) values(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
     :param args: All number must have same size.
     :return: Effect rowcount
```

### Comparing `sqlx-exec-1.0.8/sqlexec/log_support.py` & `sqlx-exec-1.0.9/sqlexec/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.0.8/sqlexec/pooling.py` & `sqlx-exec-1.0.9/sqlexec/pooling.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.0.8/sqlexec/sql_support.py` & `sqlx-exec-1.0.9/sqlexec/engin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,92 +1,74 @@
+from enum import Enum
 from typing import Sequence
 from functools import lru_cache
-from .log_support import logger
-from .engin import Engin
 
 CACHE_SIZE = 256
-_SHOW_SQL = False
-_ENGIN = Engin.MySQL
-before_execute = None
 
 
-def insert_sql_args(table: str, **kwargs):
-    cols, args = zip(*kwargs.items())
-    sql = _create_insert_sql(table, cols)
-    return sql, args
+class Engin(Enum):
+    MySQL = 'MySQL'
+    PostgreSQL = 'PostgreSQL'
 
 
-@lru_cache(maxsize=CACHE_SIZE)
-def _create_insert_sql(table: str, cols: Sequence[str]):
-    if _ENGIN == Engin.MySQL:
-        columns, placeholders = zip(*[('`{}`'.format(col), '?') for col in cols])
-        return 'INSERT INTO `{}`({}) VALUES({})'.format(table, ','.join(columns), ','.join(placeholders))
-
-    columns, placeholders = zip(*[('{}'.format(col), '?') for col in cols])
-    return 'INSERT INTO {}({}) VALUES({})'.format(table, ','.join(columns), ','.join(placeholders))
-
+class SqlEngin:
+    def __init__(self, logger, show_sql):
+        self.logger = logger
+        self.show_sql = show_sql
 
-def get_batch_args(*args):
-    return args[0] if isinstance(args, tuple) and len(args) == 1 and isinstance(args[0], Sequence) else args
+    def before_execute(self, function: str, sql: str, *args):
+        if self.show_sql:
+            self.logger.info("Exec func 'sqlexec.%s' \n\tSQL: %s \n\tARGS: %s" % (function, sql, args))
+        return sql.replace('?', '%s')
 
+    @staticmethod
+    @lru_cache(maxsize=CACHE_SIZE)
+    def create_insert_sql(table: str, cols: Sequence[str]):
+        columns, placeholders = zip(*[('{}'.format(col), '?') for col in cols])
+        return 'INSERT INTO {}({}) VALUES({})'.format(table, ', '.join(columns), ','.join(placeholders))
 
-def page_sql_args(sql: str, page_num=1, page_size=10, *args):
-    global _ENGIN
-    start = (page_num - 1) * page_size
-    if require_limit(sql):
-        if _ENGIN == Engin.MySQL:
-            sql = '{} limit ?,?'.format(sql)
-            args = [*args, start, page_size]
-        elif _ENGIN == Engin.PostgreSQL:
-            sql = '{} LIMIT ? OFFSET ?'.format(sql)
-            args = [*args, page_size, start]
-    return sql, args
 
+class MySqlEngin(SqlEngin):
 
-def require_limit(sql: str):
-    lower_sql = sql.lower()
-    if 'limit' not in lower_sql:
-        return True
-    idx = lower_sql.rindex('limit')
-    if idx > 0 and ')' in lower_sql[idx:]:
-        return True
-    return False
-
-
-def set_config(engin, show_sql):
-    global _ENGIN
-    global _SHOW_SQL
-    global before_execute
-    _ENGIN = engin
-    _ENGIN = engin
-    _SHOW_SQL = show_sql
-    if engin == Engin.PostgreSQL:
-        if show_sql:
-            before_execute =before_execute_postgres_show_sql
-        else:
-            before_execute = before_execute_postgres
-    else:
-        if show_sql:
-            before_execute = before_execute_default_show_sql
-        else:
-            before_execute = lambda function, sql, *args: sql.replace('?', '%s')
-
-
-def before_execute_default_show_sql(function: str, sql: str, *args):
-    logger.info("Exec func 'sqlexec.%s' \n\tSQL: %s \n\tARGS: %s" % (function, sql, args))
-    return sql.replace('?', '%s')
-
-
-def before_execute_postgres(function: str, sql: str, *args):
-    if '%' in sql and 'like' in sql.lower():
-        sql = sql.replace('%', '%%').replace('%%%%', '%%')
-    return sql.replace('?', '%s')
-
-
-def before_execute_postgres_show_sql(function: str, sql: str, *args):
-    logger.info("Exec func 'sqlexec.%s' \n\tSQL: %s \n\tARGS: %s" % (function, sql, args))
-    if '%' in sql and 'like' in sql.lower():
-        sql = sql.replace('%', '%%').replace('%%%%', '%%')
-    return sql.replace('?', '%s')
+    def __init__(self, logger, show_sql):
+        super().__init__(logger, show_sql)
 
+    @staticmethod
+    @lru_cache(maxsize=CACHE_SIZE)
+    def create_insert_sql(table: str, cols: Sequence[str]):
+        columns, placeholders = zip(*[('`{}`'.format(col), '?') for col in cols])
+        return 'INSERT INTO `{}`({}) VALUES({})'.format(table, ', '.join(columns), ','.join(placeholders))
 
+    @staticmethod
+    def page_sql_args(require_limit, sql: str, start, page_size, *args):
+        if require_limit(sql):
+            sql = '{} limit ?, ?'.format(sql)
+        args = [*args, start, page_size]
+        return sql, args
+
+    @staticmethod
+    def pk_sql(*args):
+        return "SELECT LAST_INSERT_ID()"
+
+
+class PostgresEngin(SqlEngin):
+
+    def __init__(self, logger, show_sql):
+        super().__init__(logger, show_sql)
+
+    def before_execute(self, function: str, sql: str, *args):
+        if self.show_sql:
+            self.logger.info("Exec func 'sqlexec.%s' \n\tSQL: %s \n\tARGS: %s" % (function, sql, args))
+        if '%' in sql and 'like' in sql.lower():
+            sql = sql.replace('%', '%%').replace('%%%%', '%%')
+        return sql.replace('?', '%s')
+
+    @staticmethod
+    def page_sql_args(require_limit, sql: str, start, page_size, *args):
+        if require_limit(sql):
+            sql = '{} LIMIT ? OFFSET ?'.format(sql)
+        args = [*args, page_size, start]
+        return sql, args
 
+    @staticmethod
+    def pk_sql(pk_seq, *args):
+        return  "SELECT currval('{}')".format(pk_seq)
```

### Comparing `sqlx-exec-1.0.8/sqlexec/support.py` & `sqlx-exec-1.0.9/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.0.8/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.0.9/sqlx_exec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.0.8
+Version: 1.0.9
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
@@ -22,15 +22,15 @@
 
    if __name__ == '__main__':
        sqlexec.init_engin(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, engin=Engin.PostgreSQL)
 
        pk_sql = "SELECT currval('person_id_seq')"
        id = sqlexec.save(pk_sql=pk_sql, table='person', name='zhangsan', age=15)
        id = sqlexec.save_sql(pk_sql, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
-       rowcount = sqlexec.insert(table='person', id=5, name='wangwu', age=38)
+       rowcount = sqlexec.insert(table='person', name='wangwu', age=38)
 
        count = sqlexec.get('select count(1) from person')
        # result: 3
 
        persons = sqlexec.select('select id, name, age from person')
        # result:
        # (3, 'zhangsan', 15)
```

