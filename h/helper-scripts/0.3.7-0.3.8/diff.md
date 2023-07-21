# Comparing `tmp/helper_scripts-0.3.7.tar.gz` & `tmp/helper_scripts-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helper_scripts-0.3.7.tar", last modified: Fri Jul 21 13:37:00 2023, max compression
+gzip compressed data, was "helper_scripts-0.3.8.tar", last modified: Fri Jul 21 15:05:52 2023, max compression
```

## Comparing `helper_scripts-0.3.7.tar` & `helper_scripts-0.3.8.tar`

### file list

```diff
@@ -1,27 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 13:37:00.926635 helper_scripts-0.3.7/
--rw-rw-rw-   0        0        0     1097 2023-05-20 21:20:05.000000 helper_scripts-0.3.7/LICENSE
--rw-rw-rw-   0        0        0     6320 2023-07-21 13:37:00.911084 helper_scripts-0.3.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-21 13:37:00.654018 helper_scripts-0.3.7/helper_scripts/
--rw-rw-rw-   0        0        0        0 2023-07-21 10:19:46.000000 helper_scripts-0.3.7/helper_scripts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:37:00.846855 helper_scripts-0.3.7/helper_scripts/database_handler/
--rw-rw-rw-   0        0        0      815 2022-12-28 14:54:33.000000 helper_scripts-0.3.7/helper_scripts/database_handler/ConfigHandler.py
--rw-rw-rw-   0        0        0     5448 2023-05-20 20:50:53.000000 helper_scripts-0.3.7/helper_scripts/database_handler/DatabaseHandler.py
--rw-rw-rw-   0        0        0     8577 2022-12-28 14:54:33.000000 helper_scripts-0.3.7/helper_scripts/database_handler/Helpers.py
--rw-rw-rw-   0        0        0      853 2023-02-21 11:17:56.000000 helper_scripts-0.3.7/helper_scripts/database_handler/SendRequest.py
--rw-rw-rw-   0        0        0      278 2023-02-21 11:08:41.000000 helper_scripts-0.3.7/helper_scripts/database_handler/__init__.py
--rw-rw-rw-   0        0        0      461 2022-12-28 14:54:33.000000 helper_scripts-0.3.7/helper_scripts/database_handler/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:37:00.878680 helper_scripts-0.3.7/helper_scripts/send_mail/
--rw-rw-rw-   0        0        0     3943 2023-07-21 13:21:32.000000 helper_scripts-0.3.7/helper_scripts/send_mail/SendMail.py
--rw-rw-rw-   0        0        0       39 2023-02-21 11:00:20.000000 helper_scripts-0.3.7/helper_scripts/send_mail/__init__.py
--rw-rw-rw-   0        0        0      666 2023-07-21 13:34:12.000000 helper_scripts-0.3.7/helper_scripts/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:37:00.894890 helper_scripts-0.3.7/helper_scripts/test/
--rw-rw-rw-   0        0        0     2364 2023-07-21 13:21:35.000000 helper_scripts-0.3.7/helper_scripts/test/test_SendMail.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:37:00.750429 helper_scripts-0.3.7/helper_scripts.egg-info/
--rw-rw-rw-   0        0        0     6320 2023-07-21 13:37:00.000000 helper_scripts-0.3.7/helper_scripts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      659 2023-07-21 13:37:00.000000 helper_scripts-0.3.7/helper_scripts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 13:37:00.000000 helper_scripts-0.3.7/helper_scripts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-21 13:37:00.000000 helper_scripts-0.3.7/helper_scripts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-21 13:37:00.000000 helper_scripts-0.3.7/helper_scripts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      667 2023-07-21 13:33:41.000000 helper_scripts-0.3.7/pyproject.toml
--rw-rw-rw-   0        0        0     5815 2023-05-20 20:58:38.000000 helper_scripts-0.3.7/readme.md
--rw-rw-rw-   0        0        0       42 2023-07-21 13:37:00.926635 helper_scripts-0.3.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-21 15:05:52.563597 helper_scripts-0.3.8/
+-rw-rw-rw-   0        0        0      376 2023-07-21 15:05:52.551941 helper_scripts-0.3.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-21 15:05:52.411189 helper_scripts-0.3.8/database_handler/
+-rw-rw-rw-   0        0        0      815 2022-12-28 14:54:33.000000 helper_scripts-0.3.8/database_handler/ConfigHandler.py
+-rw-rw-rw-   0        0        0     5448 2023-05-20 20:50:53.000000 helper_scripts-0.3.8/database_handler/DatabaseHandler.py
+-rw-rw-rw-   0        0        0     8577 2022-12-28 14:54:33.000000 helper_scripts-0.3.8/database_handler/Helpers.py
+-rw-rw-rw-   0        0        0      853 2023-02-21 11:17:56.000000 helper_scripts-0.3.8/database_handler/SendRequest.py
+-rw-rw-rw-   0        0        0      278 2023-02-21 11:08:41.000000 helper_scripts-0.3.8/database_handler/__init__.py
+-rw-rw-rw-   0        0        0      461 2022-12-28 14:54:33.000000 helper_scripts-0.3.8/database_handler/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-21 15:05:52.496347 helper_scripts-0.3.8/helper_scripts.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-07-21 15:05:52.000000 helper_scripts-0.3.8/helper_scripts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2023-07-21 15:05:52.000000 helper_scripts-0.3.8/helper_scripts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 15:05:52.000000 helper_scripts-0.3.8/helper_scripts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-21 15:05:52.000000 helper_scripts-0.3.8/helper_scripts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-07-21 15:05:52.000000 helper_scripts-0.3.8/helper_scripts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 15:05:52.518042 helper_scripts-0.3.8/send_mail/
+-rw-rw-rw-   0        0        0     3943 2023-07-21 13:21:32.000000 helper_scripts-0.3.8/send_mail/SendMail.py
+-rw-rw-rw-   0        0        0       39 2023-02-21 11:00:20.000000 helper_scripts-0.3.8/send_mail/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-21 15:05:52.563597 helper_scripts-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0      595 2023-07-21 14:04:39.000000 helper_scripts-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 15:05:52.534462 helper_scripts-0.3.8/test/
+-rw-rw-rw-   0        0        0     2364 2023-07-21 13:21:35.000000 helper_scripts-0.3.8/test/test_SendMail.py
```

### Comparing `helper_scripts-0.3.7/helper_scripts/database_handler/ConfigHandler.py` & `helper_scripts-0.3.8/database_handler/ConfigHandler.py`

 * *Files identical despite different names*

### Comparing `helper_scripts-0.3.7/helper_scripts/database_handler/DatabaseHandler.py` & `helper_scripts-0.3.8/database_handler/DatabaseHandler.py`

 * *Files identical despite different names*

### Comparing `helper_scripts-0.3.7/helper_scripts/database_handler/Helpers.py` & `helper_scripts-0.3.8/database_handler/Helpers.py`

 * *Files identical despite different names*

### Comparing `helper_scripts-0.3.7/helper_scripts/database_handler/SendRequest.py` & `helper_scripts-0.3.8/database_handler/SendRequest.py`

 * *Files identical despite different names*

### Comparing `helper_scripts-0.3.7/helper_scripts/send_mail/SendMail.py` & `helper_scripts-0.3.8/send_mail/SendMail.py`

 * *Files identical despite different names*

### Comparing `helper_scripts-0.3.7/helper_scripts/test/test_SendMail.py` & `helper_scripts-0.3.8/test/test_SendMail.py`

 * *Files identical despite different names*

