# Comparing `tmp/match_func-0.0.1.tar.gz` & `tmp/match_func-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "match_func-0.0.1.tar", last modified: Thu Jul 20 13:57:05 2023, max compression
+gzip compressed data, was "match_func-1.0.0.tar", last modified: Fri Jul 21 13:01:35 2023, max compression
```

## Comparing `match_func-0.0.1.tar` & `match_func-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-20 13:57:05.213082 match_func-0.0.1/
--rw-rw-r--   0 omega     (1000) omega     (1000)    18092 2023-07-20 11:00:34.000000 match_func-0.0.1/LICENSE
--rw-rw-r--   0 omega     (1000) omega     (1000)     1512 2023-07-20 13:57:05.213082 match_func-0.0.1/PKG-INFO
--rw-rw-r--   0 omega     (1000) omega     (1000)     1162 2023-07-20 13:36:18.000000 match_func-0.0.1/README.md
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-20 13:57:05.213082 match_func-0.0.1/match_func/
--rw-rw-r--   0 omega     (1000) omega     (1000)       30 2023-07-20 13:27:49.000000 match_func-0.0.1/match_func/__init__.py
--rwxrwxr-x   0 omega     (1000) omega     (1000)     1766 2023-07-20 13:36:23.000000 match_func-0.0.1/match_func/match_func.py
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-20 13:57:05.213082 match_func-0.0.1/match_func.egg-info/
--rw-rw-r--   0 omega     (1000) omega     (1000)     1512 2023-07-20 13:57:05.000000 match_func-0.0.1/match_func.egg-info/PKG-INFO
--rw-rw-r--   0 omega     (1000) omega     (1000)      210 2023-07-20 13:57:05.000000 match_func-0.0.1/match_func.egg-info/SOURCES.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)        1 2023-07-20 13:57:05.000000 match_func-0.0.1/match_func.egg-info/dependency_links.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)       11 2023-07-20 13:57:05.000000 match_func-0.0.1/match_func.egg-info/top_level.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)       38 2023-07-20 13:57:05.213082 match_func-0.0.1/setup.cfg
--rw-rw-r--   0 omega     (1000) omega     (1000)      482 2023-07-20 13:36:30.000000 match_func-0.0.1/setup.py
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 13:01:35.840443 match_func-1.0.0/
+-rw-rw-r--   0 omega     (1000) omega     (1000)    18092 2023-07-20 11:00:34.000000 match_func-1.0.0/LICENSE
+-rw-rw-r--   0 omega     (1000) omega     (1000)     1512 2023-07-21 13:01:35.840443 match_func-1.0.0/PKG-INFO
+-rw-rw-r--   0 omega     (1000) omega     (1000)     1162 2023-07-20 13:36:18.000000 match_func-1.0.0/README.md
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 13:01:35.840443 match_func-1.0.0/match_func/
+-rw-rw-r--   0 omega     (1000) omega     (1000)       30 2023-07-20 13:27:49.000000 match_func-1.0.0/match_func/__init__.py
+-rwxrwxr-x   0 omega     (1000) omega     (1000)     1587 2023-07-21 12:59:49.000000 match_func-1.0.0/match_func/match_func.py
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 13:01:35.840443 match_func-1.0.0/match_func.egg-info/
+-rw-rw-r--   0 omega     (1000) omega     (1000)     1512 2023-07-21 13:01:35.000000 match_func-1.0.0/match_func.egg-info/PKG-INFO
+-rw-rw-r--   0 omega     (1000) omega     (1000)      210 2023-07-21 13:01:35.000000 match_func-1.0.0/match_func.egg-info/SOURCES.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)        1 2023-07-21 13:01:35.000000 match_func-1.0.0/match_func.egg-info/dependency_links.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)       11 2023-07-21 13:01:35.000000 match_func-1.0.0/match_func.egg-info/top_level.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)       38 2023-07-21 13:01:35.840443 match_func-1.0.0/setup.cfg
+-rw-rw-r--   0 omega     (1000) omega     (1000)      482 2023-07-21 13:01:27.000000 match_func-1.0.0/setup.py
```

### Comparing `match_func-0.0.1/LICENSE` & `match_func-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `match_func-0.0.1/PKG-INFO` & `match_func-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: match_func
-Version: 0.0.1
+Version: 1.0.0
 Summary: Pattern matching as a function.
 Home-page: https://github.com/Julynx/match_func
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Maintainer: Julio Cabria
 Maintainer-email: juliocabria@tutanota.com
 License: GPLv2
```

### Comparing `match_func-0.0.1/README.md` & `match_func-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `match_func-0.0.1/match_func.egg-info/PKG-INFO` & `match_func-1.0.0/match_func.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: match-func
-Version: 0.0.1
+Version: 1.0.0
 Summary: Pattern matching as a function.
 Home-page: https://github.com/Julynx/match_func
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Maintainer: Julio Cabria
 Maintainer-email: juliocabria@tutanota.com
 License: GPLv2
```

