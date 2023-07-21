# Comparing `tmp/helper_scripts-0.3.5.tar.gz` & `tmp/helper_scripts-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helper_scripts-0.3.5.tar", last modified: Mon Apr  3 15:03:15 2023, max compression
+gzip compressed data, was "helper_scripts-0.3.6.tar", last modified: Fri Jul 21 13:25:01 2023, max compression
```

## Comparing `helper_scripts-0.3.5.tar` & `helper_scripts-0.3.6.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 15:03:15.809686 helper_scripts-0.3.5/
--rw-rw-rw-   0        0        0      304 2023-04-03 15:03:15.809686 helper_scripts-0.3.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-03 15:03:15.693324 helper_scripts-0.3.5/database_handler/
--rw-rw-rw-   0        0        0      815 2022-12-28 14:54:33.000000 helper_scripts-0.3.5/database_handler/ConfigHandler.py
--rw-rw-rw-   0        0        0     5417 2023-01-28 20:39:01.000000 helper_scripts-0.3.5/database_handler/DatabaseHandler.py
--rw-rw-rw-   0        0        0     8577 2022-12-28 14:54:33.000000 helper_scripts-0.3.5/database_handler/Helpers.py
--rw-rw-rw-   0        0        0      853 2023-02-21 11:17:56.000000 helper_scripts-0.3.5/database_handler/SendRequest.py
--rw-rw-rw-   0        0        0      278 2023-02-21 11:08:41.000000 helper_scripts-0.3.5/database_handler/__init__.py
--rw-rw-rw-   0        0        0      461 2022-12-28 14:54:33.000000 helper_scripts-0.3.5/database_handler/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-03 15:03:15.767216 helper_scripts-0.3.5/helper_scripts.egg-info/
--rw-rw-rw-   0        0        0      304 2023-04-03 15:03:14.000000 helper_scripts-0.3.5/helper_scripts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      427 2023-04-03 15:03:14.000000 helper_scripts-0.3.5/helper_scripts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 15:03:14.000000 helper_scripts-0.3.5/helper_scripts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-03 15:03:14.000000 helper_scripts-0.3.5/helper_scripts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-03 15:03:14.000000 helper_scripts-0.3.5/helper_scripts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 15:03:15.792645 helper_scripts-0.3.5/send_mail/
--rw-rw-rw-   0        0        0     3037 2023-04-03 15:02:44.000000 helper_scripts-0.3.5/send_mail/SendMail.py
--rw-rw-rw-   0        0        0       39 2023-02-21 11:00:20.000000 helper_scripts-0.3.5/send_mail/__init__.py
--rw-rw-rw-   0        0        0       42 2023-04-03 15:03:15.816796 helper_scripts-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0      593 2023-04-03 15:03:01.000000 helper_scripts-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 13:25:01.825280 helper_scripts-0.3.6/
+-rw-rw-rw-   0        0        0      376 2023-07-21 13:25:01.810684 helper_scripts-0.3.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-21 13:25:01.687407 helper_scripts-0.3.6/database_handler/
+-rw-rw-rw-   0        0        0      815 2022-12-28 14:54:33.000000 helper_scripts-0.3.6/database_handler/ConfigHandler.py
+-rw-rw-rw-   0        0        0     5448 2023-05-20 20:50:53.000000 helper_scripts-0.3.6/database_handler/DatabaseHandler.py
+-rw-rw-rw-   0        0        0     8577 2022-12-28 14:54:33.000000 helper_scripts-0.3.6/database_handler/Helpers.py
+-rw-rw-rw-   0        0        0      853 2023-02-21 11:17:56.000000 helper_scripts-0.3.6/database_handler/SendRequest.py
+-rw-rw-rw-   0        0        0      278 2023-02-21 11:08:41.000000 helper_scripts-0.3.6/database_handler/__init__.py
+-rw-rw-rw-   0        0        0      461 2022-12-28 14:54:33.000000 helper_scripts-0.3.6/database_handler/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-21 13:25:01.746995 helper_scripts-0.3.6/helper_scripts.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-07-21 13:25:00.000000 helper_scripts-0.3.6/helper_scripts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2023-07-21 13:25:01.000000 helper_scripts-0.3.6/helper_scripts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 13:25:00.000000 helper_scripts-0.3.6/helper_scripts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-21 13:25:00.000000 helper_scripts-0.3.6/helper_scripts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-07-21 13:25:00.000000 helper_scripts-0.3.6/helper_scripts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 13:25:01.780574 helper_scripts-0.3.6/send_mail/
+-rw-rw-rw-   0        0        0     3943 2023-07-21 13:21:32.000000 helper_scripts-0.3.6/send_mail/SendMail.py
+-rw-rw-rw-   0        0        0       39 2023-02-21 11:00:20.000000 helper_scripts-0.3.6/send_mail/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-21 13:25:01.825280 helper_scripts-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      666 2023-07-21 13:24:49.000000 helper_scripts-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 13:25:01.794886 helper_scripts-0.3.6/test/
+-rw-rw-rw-   0        0        0     2364 2023-07-21 13:21:35.000000 helper_scripts-0.3.6/test/test_SendMail.py
```

### Comparing `helper_scripts-0.3.5/database_handler/ConfigHandler.py` & `helper_scripts-0.3.6/database_handler/ConfigHandler.py`

 * *Files identical despite different names*

### Comparing `helper_scripts-0.3.5/database_handler/DatabaseHandler.py` & `helper_scripts-0.3.6/database_handler/DatabaseHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from configparser import ConfigParser
-import pandas as pd
 import psycopg2
 from psycopg2.extras import DictCursor
 import sys
 
 
 
 class DatabaseHandler(object):
@@ -44,21 +43,21 @@
 
         except Exception as ex:
             if str(ex)[:6] == 'FATAL:':
                 sys.exit("Database connection error: %s" % str(ex)[8:])
             else:
                 raise ex
 
-    def get_cursor(self):
+    def get_cursor(self,cursor_type = DictCursor):
         """Create a cursor
         :return: cursor
         """
         if self.conn is None or self.conn.closed:
             self.connect()
-        curs = self.conn.cursor(cursor_factory=DictCursor)
+        curs = self.conn.cursor(cursor_factory=cursor_type)
         
         return curs
 
     def close(self):
         """Close the database connection"""
         if self.conn and not self.conn.closed:
             self.conn.close()
@@ -68,23 +67,23 @@
         """Commit currently open transaction"""
         self.conn.commit()
 
     def rollback(self):
         """Roll back currently open transaction"""
         self.conn.rollback()
 
-    def execute(self, query, args=None):
+    def execute(self, query, cursor_type = DictCursor,args=None):
         """Create a cursor, execute a query and return the cursor
         :param query: text of the statement to execute
         :param args: arguments to query
         :return: cursor
         """
         if self.conn is None or self.conn.closed:
             self.connect()
-        curs = self.conn.cursor(cursor_factory=DictCursor)
+        curs = self.conn.cursor(cursor_factory=cursor_type)
         try:
             curs.execute(query, args)
         except Exception as exc:
             self.conn.rollback()
             curs.close()
             raise exc
         return curs
```

### Comparing `helper_scripts-0.3.5/database_handler/Helpers.py` & `helper_scripts-0.3.6/database_handler/Helpers.py`

 * *Files identical despite different names*

### Comparing `helper_scripts-0.3.5/database_handler/SendRequest.py` & `helper_scripts-0.3.6/database_handler/SendRequest.py`

 * *Files identical despite different names*

