# Comparing `tmp/sqlx-exec-1.0.5.tar.gz` & `tmp/sqlx-exec-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.0.5.tar", last modified: Fri Jul 21 10:01:32 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.0.6.tar", last modified: Fri Jul 21 10:02:25 2023, max compression
```

## Comparing `sqlx-exec-1.0.5.tar` & `sqlx-exec-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 10:01:32.000000 sqlx-exec-1.0.5/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     2537 2023-07-21 10:01:32.000000 sqlx-exec-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2033 2023-07-21 10:01:23.000000 sqlx-exec-1.0.5/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-21 10:01:32.000000 sqlx-exec-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1160 2023-07-21 10:01:29.000000 sqlx-exec-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:01:32.000000 sqlx-exec-1.0.5/sqlexec/
--rw-rw-rw-   0        0        0      115 2023-07-21 07:43:22.000000 sqlx-exec-1.0.5/sqlexec/constant.py
--rw-rw-rw-   0        0        0     8940 2023-07-21 09:48:46.000000 sqlx-exec-1.0.5/sqlexec/exec.py
--rw-rw-rw-   0        0        0      496 2023-07-21 08:53:39.000000 sqlx-exec-1.0.5/sqlexec/log_support.py
--rw-rw-rw-   0        0        0     1521 2023-07-21 09:59:37.000000 sqlx-exec-1.0.5/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4008 2023-07-21 07:13:11.000000 sqlx-exec-1.0.5/sqlexec/support.py
--rw-rw-rw-   0        0        0      292 2023-07-21 08:34:59.000000 sqlx-exec-1.0.5/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:01:32.000000 sqlx-exec-1.0.5/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-21 10:01:32.000000 sqlx-exec-1.0.5/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-21 08:56:11.000000 sqlx-exec-1.0.5/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2537 2023-07-21 10:01:32.000000 sqlx-exec-1.0.5/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-21 10:01:32.000000 sqlx-exec-1.0.5/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-21 10:01:32.000000 sqlx-exec-1.0.5/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 10:02:25.000000 sqlx-exec-1.0.6/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2537 2023-07-21 10:02:25.000000 sqlx-exec-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2033 2023-07-21 10:02:15.000000 sqlx-exec-1.0.6/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-21 10:02:25.000000 sqlx-exec-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1160 2023-07-21 10:02:23.000000 sqlx-exec-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 10:02:25.000000 sqlx-exec-1.0.6/sqlexec/
+-rw-rw-rw-   0        0        0      115 2023-07-21 07:43:22.000000 sqlx-exec-1.0.6/sqlexec/constant.py
+-rw-rw-rw-   0        0        0     8940 2023-07-21 09:48:46.000000 sqlx-exec-1.0.6/sqlexec/exec.py
+-rw-rw-rw-   0        0        0      496 2023-07-21 08:53:39.000000 sqlx-exec-1.0.6/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0     1521 2023-07-21 09:59:37.000000 sqlx-exec-1.0.6/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4008 2023-07-21 07:13:11.000000 sqlx-exec-1.0.6/sqlexec/support.py
+-rw-rw-rw-   0        0        0      292 2023-07-21 08:34:59.000000 sqlx-exec-1.0.6/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 10:02:25.000000 sqlx-exec-1.0.6/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-21 10:02:25.000000 sqlx-exec-1.0.6/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-21 08:56:11.000000 sqlx-exec-1.0.6/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2537 2023-07-21 10:02:25.000000 sqlx-exec-1.0.6/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-21 10:02:25.000000 sqlx-exec-1.0.6/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-21 10:02:25.000000 sqlx-exec-1.0.6/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.0.5/LICENSE` & `sqlx-exec-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.0.5/PKG-INFO` & `sqlx-exec-1.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.0.5
+Version: 1.0.6
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto mange database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
@@ -71,10 +71,10 @@
        with transaction():
            insert_func(....)
            update_func(....)
 
 
 If you want to operate MySQL database like Mybatis, you may need MySqlx: https://pypi.org/project/mysqlx
 
-If you want to operate PostgreSQL database like Mybatis, you may need MySqlx: https://pypi.org/project/Pgsqlx
+If you want to operate PostgreSQL database like Mybatis, you may need PgSqlx: https://pypi.org/project/pgsqlx
```

### Comparing `sqlx-exec-1.0.5/README.rst` & `sqlx-exec-1.0.6/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -57,8 +57,8 @@
        with transaction():
            insert_func(....)
            update_func(....)
 
 
 If you want to operate MySQL database like Mybatis, you may need MySqlx: https://pypi.org/project/mysqlx
 
-If you want to operate PostgreSQL database like Mybatis, you may need MySqlx: https://pypi.org/project/Pgsqlx
+If you want to operate PostgreSQL database like Mybatis, you may need PgSqlx: https://pypi.org/project/pgsqlx
```

### Comparing `sqlx-exec-1.0.5/setup.py` & `sqlx-exec-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="sqlx-exec is a simple sql executor for Python, it help you auto mange database connection and transaction.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.0.5',
+    version='1.0.6',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.0.5/sqlexec/exec.py` & `sqlx-exec-1.0.6/sqlexec/exec.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.0.5/sqlexec/sql_support.py` & `sqlx-exec-1.0.6/sqlexec/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.0.5/sqlexec/support.py` & `sqlx-exec-1.0.6/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.0.5/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.0.6/sqlx_exec.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.0.5
+Version: 1.0.6
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto mange database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
@@ -71,10 +71,10 @@
        with transaction():
            insert_func(....)
            update_func(....)
 
 
 If you want to operate MySQL database like Mybatis, you may need MySqlx: https://pypi.org/project/mysqlx
 
-If you want to operate PostgreSQL database like Mybatis, you may need MySqlx: https://pypi.org/project/Pgsqlx
+If you want to operate PostgreSQL database like Mybatis, you may need PgSqlx: https://pypi.org/project/pgsqlx
```

