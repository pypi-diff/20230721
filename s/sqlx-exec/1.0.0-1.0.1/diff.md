# Comparing `tmp/sqlx-exec-1.0.0.tar.gz` & `tmp/sqlx-exec-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.0.0.tar", last modified: Fri Jul 21 08:56:11 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.0.1.tar", last modified: Fri Jul 21 08:58:32 2023, max compression
```

## Comparing `sqlx-exec-1.0.0.tar` & `sqlx-exec-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 08:56:11.000000 sqlx-exec-1.0.0/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2544 2023-07-21 08:56:11.000000 sqlx-exec-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2041 2023-07-21 08:38:37.000000 sqlx-exec-1.0.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-21 08:56:11.000000 sqlx-exec-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1160 2023-07-21 08:54:26.000000 sqlx-exec-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:56:11.000000 sqlx-exec-1.0.0/sqlexec/
--rw-rw-rw-   0        0        0      115 2023-07-21 07:43:22.000000 sqlx-exec-1.0.0/sqlexec/constant.py
--rw-rw-rw-   0        0        0     8964 2023-07-21 08:53:39.000000 sqlx-exec-1.0.0/sqlexec/exec.py
--rw-rw-rw-   0        0        0      496 2023-07-21 08:53:39.000000 sqlx-exec-1.0.0/sqlexec/log_support.py
--rw-rw-rw-   0        0        0     1523 2023-07-21 08:22:59.000000 sqlx-exec-1.0.0/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4008 2023-07-21 07:13:11.000000 sqlx-exec-1.0.0/sqlexec/support.py
--rw-rw-rw-   0        0        0      292 2023-07-21 08:34:59.000000 sqlx-exec-1.0.0/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:56:11.000000 sqlx-exec-1.0.0/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-21 08:56:11.000000 sqlx-exec-1.0.0/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-21 08:56:11.000000 sqlx-exec-1.0.0/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2544 2023-07-21 08:56:11.000000 sqlx-exec-1.0.0/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-21 08:56:11.000000 sqlx-exec-1.0.0/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-21 08:56:11.000000 sqlx-exec-1.0.0/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 08:58:32.000000 sqlx-exec-1.0.1/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2535 2023-07-21 08:58:32.000000 sqlx-exec-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2032 2023-07-21 08:58:29.000000 sqlx-exec-1.0.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-21 08:58:32.000000 sqlx-exec-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1160 2023-07-21 08:57:52.000000 sqlx-exec-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:58:32.000000 sqlx-exec-1.0.1/sqlexec/
+-rw-rw-rw-   0        0        0      115 2023-07-21 07:43:22.000000 sqlx-exec-1.0.1/sqlexec/constant.py
+-rw-rw-rw-   0        0        0     8964 2023-07-21 08:53:39.000000 sqlx-exec-1.0.1/sqlexec/exec.py
+-rw-rw-rw-   0        0        0      496 2023-07-21 08:53:39.000000 sqlx-exec-1.0.1/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0     1523 2023-07-21 08:22:59.000000 sqlx-exec-1.0.1/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4008 2023-07-21 07:13:11.000000 sqlx-exec-1.0.1/sqlexec/support.py
+-rw-rw-rw-   0        0        0      292 2023-07-21 08:34:59.000000 sqlx-exec-1.0.1/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:58:32.000000 sqlx-exec-1.0.1/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-21 08:58:32.000000 sqlx-exec-1.0.1/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-21 08:56:11.000000 sqlx-exec-1.0.1/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2535 2023-07-21 08:58:32.000000 sqlx-exec-1.0.1/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-21 08:58:32.000000 sqlx-exec-1.0.1/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-21 08:58:32.000000 sqlx-exec-1.0.1/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.0.0/LICENSE` & `sqlx-exec-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.0.0/PKG-INFO` & `sqlx-exec-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.0.0
+Version: 1.0.1
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto mange database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
@@ -14,15 +14,15 @@
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
    import sqlexec
-   from sqlexec.constant import Engin
+   from sqlexec import Engin
 
    if __name__ == '__main__':
        db.init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, engin=Engin.PostgreSQL)
 
        id = sqlexec.save(pk_sql="SELECT currval('person_id_seq')", table='person', name='zhangsan', age=15)
        id = sqlexec.save_sql("SELECT currval('person_id_seq')", 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', id=5, name='wangwu', age=38)
@@ -48,15 +48,15 @@
 
        persons = sqlexec.query_one('select id, name, age from person where name=?', 'zhangsan')
        # result:
        # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
        rowcount = sqlexec.execute('delete from person where id = ?', 5)
        count = sqlexec.get('select count(1) from person')
-       # result: 1
+       # result: 2
 
 Transaction
 '''''''''''
 
 .. code:: python
 
    from sqlexec import with_transaction, transaction
```

### Comparing `sqlx-exec-1.0.0/README.rst` & `sqlx-exec-1.0.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
    import sqlexec
-   from sqlexec.constant import Engin
+   from sqlexec import Engin
 
    if __name__ == '__main__':
        db.init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, engin=Engin.PostgreSQL)
 
        id = sqlexec.save(pk_sql="SELECT currval('person_id_seq')", table='person', name='zhangsan', age=15)
        id = sqlexec.save_sql("SELECT currval('person_id_seq')", 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', id=5, name='wangwu', age=38)
@@ -34,15 +34,15 @@
 
        persons = sqlexec.query_one('select id, name, age from person where name=?', 'zhangsan')
        # result:
        # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
        rowcount = sqlexec.execute('delete from person where id = ?', 5)
        count = sqlexec.get('select count(1) from person')
-       # result: 1
+       # result: 2
 
 Transaction
 '''''''''''
 
 .. code:: python
 
    from sqlexec import with_transaction, transaction
```

### Comparing `sqlx-exec-1.0.0/setup.py` & `sqlx-exec-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="sqlx-exec is a simple sql executor for Python, it help you auto mange database connection and transaction.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.0.0',
+    version='1.0.1',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.0.0/sqlexec/exec.py` & `sqlx-exec-1.0.1/sqlexec/exec.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.0.0/sqlexec/sql_support.py` & `sqlx-exec-1.0.1/sqlexec/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.0.0/sqlexec/support.py` & `sqlx-exec-1.0.1/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.0.0/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.0.1/sqlx_exec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.0.0
+Version: 1.0.1
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto mange database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
@@ -14,15 +14,15 @@
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
    import sqlexec
-   from sqlexec.constant import Engin
+   from sqlexec import Engin
 
    if __name__ == '__main__':
        db.init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, engin=Engin.PostgreSQL)
 
        id = sqlexec.save(pk_sql="SELECT currval('person_id_seq')", table='person', name='zhangsan', age=15)
        id = sqlexec.save_sql("SELECT currval('person_id_seq')", 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', id=5, name='wangwu', age=38)
@@ -48,15 +48,15 @@
 
        persons = sqlexec.query_one('select id, name, age from person where name=?', 'zhangsan')
        # result:
        # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
        rowcount = sqlexec.execute('delete from person where id = ?', 5)
        count = sqlexec.get('select count(1) from person')
-       # result: 1
+       # result: 2
 
 Transaction
 '''''''''''
 
 .. code:: python
 
    from sqlexec import with_transaction, transaction
```

