# Comparing `tmp/Flask-SQL-Pro-2.0.tar.gz` & `tmp/Flask-SQL-Pro-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-SQL-Pro-2.0.tar", last modified: Fri Jul 21 05:11:10 2023, max compression
+gzip compressed data, was "Flask-SQL-Pro-2.1.tar", last modified: Fri Jul 21 05:57:31 2023, max compression
```

## Comparing `Flask-SQL-Pro-2.0.tar` & `Flask-SQL-Pro-2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kela       (501) staff       (20)        0 2023-07-21 05:11:10.249555 Flask-SQL-Pro-2.0/
-drwxr-xr-x   0 kela       (501) staff       (20)        0 2023-07-21 05:11:10.248476 Flask-SQL-Pro-2.0/Flask_SQL_Pro.egg-info/
--rw-r--r--   0 kela       (501) staff       (20)       55 2023-07-21 05:11:10.000000 Flask-SQL-Pro-2.0/Flask_SQL_Pro.egg-info/PKG-INFO
--rw-r--r--   0 kela       (501) staff       (20)      266 2023-07-21 05:11:10.000000 Flask-SQL-Pro-2.0/Flask_SQL_Pro.egg-info/SOURCES.txt
--rw-r--r--   0 kela       (501) staff       (20)        1 2023-07-21 05:11:10.000000 Flask-SQL-Pro-2.0/Flask_SQL_Pro.egg-info/dependency_links.txt
--rw-r--r--   0 kela       (501) staff       (20)       30 2023-07-21 05:11:10.000000 Flask-SQL-Pro-2.0/Flask_SQL_Pro.egg-info/requires.txt
--rw-r--r--   0 kela       (501) staff       (20)       14 2023-07-21 05:11:10.000000 Flask-SQL-Pro-2.0/Flask_SQL_Pro.egg-info/top_level.txt
--rw-r--r--   0 kela       (501) staff       (20)       55 2023-07-21 05:11:10.249431 Flask-SQL-Pro-2.0/PKG-INFO
-drwxr-xr-x   0 kela       (501) staff       (20)        0 2023-07-21 05:11:10.249165 Flask-SQL-Pro-2.0/flask_sql_pro/
--rw-r--r--   0 kela       (501) staff       (20)     1679 2023-07-21 05:07:55.000000 Flask-SQL-Pro-2.0/flask_sql_pro/__init__.py
--rw-r--r--   0 kela       (501) staff       (20)     8149 2023-07-21 05:07:24.000000 Flask-SQL-Pro-2.0/flask_sql_pro/db.py
--rw-r--r--   0 kela       (501) staff       (20)     6025 2023-07-21 05:10:52.000000 Flask-SQL-Pro-2.0/flask_sql_pro/sql_loader.py
--rw-r--r--   0 kela       (501) staff       (20)       38 2023-07-21 05:11:10.249607 Flask-SQL-Pro-2.0/setup.cfg
--rw-r--r--   0 kela       (501) staff       (20)      253 2023-07-21 05:11:05.000000 Flask-SQL-Pro-2.0/setup.py
+drwxr-xr-x   0 kela       (501) staff       (20)        0 2023-07-21 05:57:31.296259 Flask-SQL-Pro-2.1/
+drwxr-xr-x   0 kela       (501) staff       (20)        0 2023-07-21 05:57:31.295131 Flask-SQL-Pro-2.1/Flask_SQL_Pro.egg-info/
+-rw-r--r--   0 kela       (501) staff       (20)       55 2023-07-21 05:57:31.000000 Flask-SQL-Pro-2.1/Flask_SQL_Pro.egg-info/PKG-INFO
+-rw-r--r--   0 kela       (501) staff       (20)      266 2023-07-21 05:57:31.000000 Flask-SQL-Pro-2.1/Flask_SQL_Pro.egg-info/SOURCES.txt
+-rw-r--r--   0 kela       (501) staff       (20)        1 2023-07-21 05:57:31.000000 Flask-SQL-Pro-2.1/Flask_SQL_Pro.egg-info/dependency_links.txt
+-rw-r--r--   0 kela       (501) staff       (20)       30 2023-07-21 05:57:31.000000 Flask-SQL-Pro-2.1/Flask_SQL_Pro.egg-info/requires.txt
+-rw-r--r--   0 kela       (501) staff       (20)       14 2023-07-21 05:57:31.000000 Flask-SQL-Pro-2.1/Flask_SQL_Pro.egg-info/top_level.txt
+-rw-r--r--   0 kela       (501) staff       (20)       55 2023-07-21 05:57:31.296135 Flask-SQL-Pro-2.1/PKG-INFO
+drwxr-xr-x   0 kela       (501) staff       (20)        0 2023-07-21 05:57:31.295856 Flask-SQL-Pro-2.1/flask_sql_pro/
+-rw-r--r--   0 kela       (501) staff       (20)     1739 2023-07-21 05:57:01.000000 Flask-SQL-Pro-2.1/flask_sql_pro/__init__.py
+-rw-r--r--   0 kela       (501) staff       (20)     8149 2023-07-21 05:07:24.000000 Flask-SQL-Pro-2.1/flask_sql_pro/db.py
+-rw-r--r--   0 kela       (501) staff       (20)     6025 2023-07-21 05:10:52.000000 Flask-SQL-Pro-2.1/flask_sql_pro/sql_loader.py
+-rw-r--r--   0 kela       (501) staff       (20)       38 2023-07-21 05:57:31.296301 Flask-SQL-Pro-2.1/setup.cfg
+-rw-r--r--   0 kela       (501) staff       (20)      253 2023-07-21 05:57:27.000000 Flask-SQL-Pro-2.1/setup.py
```

### Comparing `Flask-SQL-Pro-2.0/flask_sql_pro/__init__.py` & `Flask-SQL-Pro-2.1/flask_sql_pro/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import inspect
 import os
 from contextlib import contextmanager
 
 from flask_sqlalchemy import SQLAlchemy as _SQLAlchemy
 from flask_sql_pro.db import DataBaseHelper
 from flask_sql_pro.sql_loader import SqlLoader, Loader
 
@@ -27,15 +26,15 @@
         if app is not None:
             self.init_app(app)
 
     def init_app(self, app, *args, **kwargs):
         if not hasattr(app, 'extensions'):
             app.extensions = {}
         _db = SQLAlchemy(app, *args, **kwargs)
-        app.extensions['flask_sql_pro'] = DataBaseHelper
+        app.extensions['flask_sql_pro'] = self  # You can now access instances of the my_extension plugin in your Flask application
         DataBaseHelper.db = _db
         DataBaseHelper.page_param = app.config.get('DB_HELPER_PAGE_PARAM', 'page')
         DataBaseHelper.page_size_param = app.config.get('DB_HELPER_PAGE_SIZE_PARAM', 'page_size')
         DataBaseHelper.print_msg = app.config.get('DB_HELPER_PRINT_MSG', False)
         SqlLoader.page_param = app.config.get('DB_HELPER_PAGE_PARAM', 'page')
         SqlLoader.page_size_param = app.config.get('DB_HELPER_PAGE_SIZE_PARAM', 'page_size')
```

### Comparing `Flask-SQL-Pro-2.0/flask_sql_pro/db.py` & `Flask-SQL-Pro-2.1/flask_sql_pro/db.py`

 * *Files identical despite different names*

### Comparing `Flask-SQL-Pro-2.0/flask_sql_pro/sql_loader.py` & `Flask-SQL-Pro-2.1/flask_sql_pro/sql_loader.py`

 * *Files identical despite different names*

