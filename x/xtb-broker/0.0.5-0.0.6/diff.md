# Comparing `tmp/xtb_broker-0.0.5.tar.gz` & `tmp/xtb_broker-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtb_broker-0.0.5.tar", last modified: Thu Jul 20 21:37:16 2023, max compression
+gzip compressed data, was "xtb_broker-0.0.6.tar", last modified: Fri Jul 21 09:14:41 2023, max compression
```

## Comparing `xtb_broker-0.0.5.tar` & `xtb_broker-0.0.6.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:37:16.829212 xtb_broker-0.0.5/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1073 2023-07-20 20:49:36.000000 xtb_broker-0.0.5/LICENSE
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      920 2023-07-20 21:37:16.829212 xtb_broker-0.0.5/PKG-INFO
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      485 2023-07-20 21:18:13.000000 xtb_broker-0.0.5/README.md
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      516 2023-07-20 21:36:52.000000 xtb_broker-0.0.5/pyproject.toml
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       38 2023-07-20 21:37:16.829212 xtb_broker-0.0.5/setup.cfg
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:37:16.829212 xtb_broker-0.0.5/src/
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:37:16.829212 xtb_broker-0.0.5/src/xtb_broker/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.5/src/xtb_broker/__init__.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)    12103 2023-05-20 13:45:08.000000 xtb_broker-0.0.5/src/xtb_broker/client.py
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:37:16.829212 xtb_broker-0.0.5/src/xtb_broker/config/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.5/src/xtb_broker/config/__init__.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2065 2023-05-20 14:31:15.000000 xtb_broker-0.0.5/src/xtb_broker/config/constants.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1702 2023-05-20 13:45:08.000000 xtb_broker-0.0.5/src/xtb_broker/config/exception.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      701 2023-05-20 13:45:08.000000 xtb_broker-0.0.5/src/xtb_broker/config/frozen.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      289 2023-05-20 13:45:08.000000 xtb_broker-0.0.5/src/xtb_broker/config/logger.py
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:37:16.829212 xtb_broker-0.0.5/src/xtb_broker/models/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.5/src/xtb_broker/models/__init__.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     6028 2023-05-20 13:45:08.000000 xtb_broker-0.0.5/src/xtb_broker/models/arbitrage.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2198 2023-05-20 13:45:08.000000 xtb_broker-0.0.5/src/xtb_broker/models/position.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      583 2023-05-20 13:45:08.000000 xtb_broker-0.0.5/src/xtb_broker/models/shift.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     3091 2023-05-20 13:45:08.000000 xtb_broker-0.0.5/src/xtb_broker/models/symbol.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1824 2023-05-20 13:45:08.000000 xtb_broker-0.0.5/src/xtb_broker/models/timetable.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     6465 2023-05-20 13:45:08.000000 xtb_broker-0.0.5/src/xtb_broker/models/trade.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1824 2023-05-20 13:45:08.000000 xtb_broker-0.0.5/src/xtb_broker/models/transaction.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      649 2023-05-20 13:45:08.000000 xtb_broker-0.0.5/src/xtb_broker/utils.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2651 2023-07-20 18:18:21.000000 xtb_broker-0.0.5/src/xtb_broker/xtb.py
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-20 21:37:16.829212 xtb_broker-0.0.5/src/xtb_broker.egg-info/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      920 2023-07-20 21:37:16.000000 xtb_broker-0.0.5/src/xtb_broker.egg-info/PKG-INFO
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      719 2023-07-20 21:37:16.000000 xtb_broker-0.0.5/src/xtb_broker.egg-info/SOURCES.txt
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        1 2023-07-20 21:37:16.000000 xtb_broker-0.0.5/src/xtb_broker.egg-info/dependency_links.txt
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       11 2023-07-20 21:37:16.000000 xtb_broker-0.0.5/src/xtb_broker.egg-info/top_level.txt
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-21 09:14:41.577326 xtb_broker-0.0.6/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      270 2023-07-21 09:14:41.577326 xtb_broker-0.0.6/PKG-INFO
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      526 2023-07-21 09:14:06.000000 xtb_broker-0.0.6/README.md
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      516 2023-07-20 21:52:23.000000 xtb_broker-0.0.6/pyproject.toml
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       38 2023-07-21 09:14:41.577326 xtb_broker-0.0.6/setup.cfg
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      397 2023-07-21 09:14:38.000000 xtb_broker-0.0.6/setup.py
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-21 09:14:41.573326 xtb_broker-0.0.6/xtb_broker/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/__init__.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)    12103 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/client.py
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-21 09:14:41.577326 xtb_broker-0.0.6/xtb_broker/config/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/config/__init__.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2065 2023-05-20 14:31:15.000000 xtb_broker-0.0.6/xtb_broker/config/constants.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1702 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/config/exception.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      701 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/config/frozen.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      289 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/config/logger.py
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-21 09:14:41.577326 xtb_broker-0.0.6/xtb_broker/models/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/models/__init__.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     6028 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/models/arbitrage.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2198 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/models/position.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      583 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/models/shift.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     3091 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/models/symbol.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1824 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/models/timetable.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     6465 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/models/trade.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1824 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/models/transaction.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      649 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/utils.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2651 2023-07-20 18:18:21.000000 xtb_broker-0.0.6/xtb_broker/xtb.py
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-21 09:14:41.573326 xtb_broker-0.0.6/xtb_broker.egg-info/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      270 2023-07-21 09:14:41.000000 xtb_broker-0.0.6/xtb_broker.egg-info/PKG-INFO
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      636 2023-07-21 09:14:41.000000 xtb_broker-0.0.6/xtb_broker.egg-info/SOURCES.txt
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        1 2023-07-21 09:14:41.000000 xtb_broker-0.0.6/xtb_broker.egg-info/dependency_links.txt
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       11 2023-07-21 09:14:41.000000 xtb_broker-0.0.6/xtb_broker.egg-info/top_level.txt
```

### Comparing `xtb_broker-0.0.5/pyproject.toml` & `xtb_broker-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.5/src/xtb_broker/client.py` & `xtb_broker-0.0.6/xtb_broker/client.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.5/src/xtb_broker/config/constants.py` & `xtb_broker-0.0.6/xtb_broker/config/constants.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.5/src/xtb_broker/config/exception.py` & `xtb_broker-0.0.6/xtb_broker/config/exception.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.5/src/xtb_broker/config/frozen.py` & `xtb_broker-0.0.6/xtb_broker/config/frozen.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.5/src/xtb_broker/models/arbitrage.py` & `xtb_broker-0.0.6/xtb_broker/models/arbitrage.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.5/src/xtb_broker/models/position.py` & `xtb_broker-0.0.6/xtb_broker/models/position.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.5/src/xtb_broker/models/shift.py` & `xtb_broker-0.0.6/xtb_broker/models/shift.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.5/src/xtb_broker/models/symbol.py` & `xtb_broker-0.0.6/xtb_broker/models/symbol.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.5/src/xtb_broker/models/timetable.py` & `xtb_broker-0.0.6/xtb_broker/models/timetable.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.5/src/xtb_broker/models/trade.py` & `xtb_broker-0.0.6/xtb_broker/models/trade.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.5/src/xtb_broker/models/transaction.py` & `xtb_broker-0.0.6/xtb_broker/models/transaction.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.5/src/xtb_broker/utils.py` & `xtb_broker-0.0.6/xtb_broker/utils.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.5/src/xtb_broker/xtb.py` & `xtb_broker-0.0.6/xtb_broker/xtb.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.5/src/xtb_broker.egg-info/PKG-INFO` & `xtb_broker-0.0.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: xtb-broker
-Version: 0.0.5
-Summary: XTB broker models, methods and tools
-Author-email: Arrubo <author@example.com>
-Project-URL: Homepage, https://pypi.org/project/xtb-broker/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Update build
 > python3 -m pip install --upgrade build
 
 # Generating distribution archives
 Now run this command from the same directory where pyproject.toml is located to generate dist
 > python3 -m build
 
@@ -26,7 +13,10 @@
 > twine upload dist/*
 
 # include version in requirements 
 > xtb-broker==0.0.1 
 
 # pip install
 > pip install xtb-broker==0.0.1
+> 
+> 
+python setup.py sdist bdist_wheel
```

