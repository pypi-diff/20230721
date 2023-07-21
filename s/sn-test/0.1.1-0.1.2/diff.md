# Comparing `tmp/sn_test-0.1.1.tar.gz` & `tmp/sn_test-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sn_test-0.1.1.tar", last modified: Fri Jul 21 05:35:32 2023, max compression
+gzip compressed data, was "dist/sn_test-0.1.2.tar", last modified: Fri Jul 21 05:47:31 2023, max compression
```

## Comparing `sn_test-0.1.1.tar` & `sn_test-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-21 05:35:32.000000 sn_test-0.1.1/
--rw-r--r--   0 mac        (501) staff       (20)      586 2023-07-21 05:35:32.000000 sn_test-0.1.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     3180 2023-07-21 05:33:54.000000 sn_test-0.1.1/set_up.py
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-21 05:35:32.000000 sn_test-0.1.1/setup.cfg
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-21 05:35:32.000000 sn_test-0.1.1/sn_test.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      586 2023-07-21 05:35:32.000000 sn_test-0.1.1/sn_test.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      163 2023-07-21 05:35:32.000000 sn_test-0.1.1/sn_test.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-21 05:35:32.000000 sn_test-0.1.1/sn_test.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       19 2023-07-21 05:35:32.000000 sn_test-0.1.1/sn_test.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-21 05:35:32.000000 sn_test-0.1.1/sn_test.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-21 05:47:31.000000 sn_test-0.1.2/
+-rw-r--r--   0 mac        (501) staff       (20)      586 2023-07-21 05:47:31.000000 sn_test-0.1.2/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     3180 2023-07-21 05:46:48.000000 sn_test-0.1.2/set_up.py
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-21 05:47:31.000000 sn_test-0.1.2/setup.cfg
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-21 05:47:31.000000 sn_test-0.1.2/sn_test/
+-rw-r--r--   0 mac        (501) staff       (20)       31 2023-07-21 05:44:26.000000 sn_test-0.1.2/sn_test/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      241 2023-07-21 05:44:03.000000 sn_test-0.1.2/sn_test/sn_test.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-21 05:47:31.000000 sn_test-0.1.2/sn_test.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      586 2023-07-21 05:47:31.000000 sn_test-0.1.2/sn_test.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      202 2023-07-21 05:47:31.000000 sn_test-0.1.2/sn_test.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-21 05:47:31.000000 sn_test-0.1.2/sn_test.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       19 2023-07-21 05:47:31.000000 sn_test-0.1.2/sn_test.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        8 2023-07-21 05:47:31.000000 sn_test-0.1.2/sn_test.egg-info/top_level.txt
```

### Comparing `sn_test-0.1.1/PKG-INFO` & `sn_test-0.1.2/sn_test.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sn_test
-Version: 0.1.1
+Name: sn-test
+Version: 0.1.2
 Summary: shuainan test
 Home-page: https://github.com/me/myproject
 Author: shuainan
 Author-email: 15294627382@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `sn_test-0.1.1/set_up.py` & `sn_test-0.1.2/set_up.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'sn_test'
 DESCRIPTION = 'shuainan test'
 URL = 'https://github.com/me/myproject'
 EMAIL = '15294627382@163.com'
 AUTHOR = 'shuainan'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
     'websocket'
 ]
```

### Comparing `sn_test-0.1.1/sn_test.egg-info/PKG-INFO` & `sn_test-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sn-test
-Version: 0.1.1
+Name: sn_test
+Version: 0.1.2
 Summary: shuainan test
 Home-page: https://github.com/me/myproject
 Author: shuainan
 Author-email: 15294627382@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

