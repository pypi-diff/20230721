# Comparing `tmp/irc_api-1.0.4.tar.gz` & `tmp/irc_api-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irc_api-1.0.4.tar", last modified: Fri Jul 21 09:11:47 2023, max compression
+gzip compressed data, was "irc_api-1.0.6.tar", last modified: Fri Jul 21 09:23:49 2023, max compression
```

## Comparing `irc_api-1.0.4.tar` & `irc_api-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:11:47.137807 irc_api-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 09:11:35.000000 irc_api-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-21 09:11:47.137807 irc_api-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-21 09:11:35.000000 irc_api-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-21 09:11:35.000000 irc_api-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 09:11:47.137807 irc_api-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-21 09:11:35.000000 irc_api-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:11:47.133806 irc_api-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:11:47.137807 irc_api-1.0.4/src/irc_api/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 09:11:35.000000 irc_api-1.0.4/src/irc_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-07-21 09:11:35.000000 irc_api-1.0.4/src/irc_api/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-21 09:11:35.000000 irc_api-1.0.4/src/irc_api/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-21 09:11:35.000000 irc_api-1.0.4/src/irc_api/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-21 09:11:35.000000 irc_api-1.0.4/src/irc_api/irc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-21 09:11:35.000000 irc_api-1.0.4/src/irc_api/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:11:47.137807 irc_api-1.0.4/src/irc_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-21 09:11:47.000000 irc_api-1.0.4/src/irc_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-21 09:11:47.000000 irc_api-1.0.4/src/irc_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 09:11:47.000000 irc_api-1.0.4/src/irc_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-21 09:11:47.000000 irc_api-1.0.4/src/irc_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 09:11:47.000000 irc_api-1.0.4/src/irc_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:23:49.172551 irc_api-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 09:23:36.000000 irc_api-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-21 09:23:49.172551 irc_api-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-21 09:23:36.000000 irc_api-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-21 09:23:36.000000 irc_api-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 09:23:49.172551 irc_api-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-21 09:23:36.000000 irc_api-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:23:49.168551 irc_api-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:23:49.168551 irc_api-1.0.6/src/irc_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 09:23:36.000000 irc_api-1.0.6/src/irc_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-07-21 09:23:36.000000 irc_api-1.0.6/src/irc_api/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-21 09:23:36.000000 irc_api-1.0.6/src/irc_api/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-21 09:23:36.000000 irc_api-1.0.6/src/irc_api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-21 09:23:36.000000 irc_api-1.0.6/src/irc_api/irc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-21 09:23:36.000000 irc_api-1.0.6/src/irc_api/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:23:49.172551 irc_api-1.0.6/src/irc_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-21 09:23:49.000000 irc_api-1.0.6/src/irc_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-21 09:23:49.000000 irc_api-1.0.6/src/irc_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 09:23:49.000000 irc_api-1.0.6/src/irc_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-21 09:23:49.000000 irc_api-1.0.6/src/irc_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 09:23:49.000000 irc_api-1.0.6/src/irc_api.egg-info/top_level.txt
```

### Comparing `irc_api-1.0.4/LICENSE` & `irc_api-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.4/PKG-INFO` & `irc_api-1.0.6/src/irc_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: irc_api
-Version: 1.0.4
+Name: irc-api
+Version: 1.0.6
 Summary: An API written in Python to make IRC bots.
 Author: Sha-chan
 Project-URL: Homepage, https://github.com/Shadow15510/irc_api
 Project-URL: Documentation, https://irc-api.readthedocs.io/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `irc_api-1.0.4/README.md` & `irc_api-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.4/pyproject.toml` & `irc_api-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.4/src/irc_api/bot.py` & `irc_api-1.0.6/src/irc_api/bot.py`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.4/src/irc_api/commands.py` & `irc_api-1.0.6/src/irc_api/commands.py`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.4/src/irc_api/history.py` & `irc_api-1.0.6/src/irc_api/history.py`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.4/src/irc_api/irc.py` & `irc_api-1.0.6/src/irc_api/irc.py`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.4/src/irc_api/message.py` & `irc_api-1.0.6/src/irc_api/message.py`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.4/src/irc_api.egg-info/PKG-INFO` & `irc_api-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: irc-api
-Version: 1.0.4
+Name: irc_api
+Version: 1.0.6
 Summary: An API written in Python to make IRC bots.
 Author: Sha-chan
 Project-URL: Homepage, https://github.com/Shadow15510/irc_api
 Project-URL: Documentation, https://irc-api.readthedocs.io/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
```

