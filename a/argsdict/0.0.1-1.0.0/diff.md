# Comparing `tmp/argsdict-0.0.1.tar.gz` & `tmp/argsdict-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argsdict-0.0.1.tar", last modified: Thu Jul 20 15:26:54 2023, max compression
+gzip compressed data, was "argsdict-1.0.0.tar", last modified: Fri Jul 21 13:08:18 2023, max compression
```

## Comparing `argsdict-0.0.1.tar` & `argsdict-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-20 15:26:54.437642 argsdict-0.0.1/
--rw-rw-r--   0 omega     (1000) omega     (1000)    18092 2023-07-20 15:17:14.000000 argsdict-0.0.1/LICENSE
--rw-rw-r--   0 omega     (1000) omega     (1000)      607 2023-07-20 15:26:54.437642 argsdict-0.0.1/PKG-INFO
--rw-rw-r--   0 omega     (1000) omega     (1000)      257 2023-07-20 15:17:14.000000 argsdict-0.0.1/README.md
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-20 15:26:54.433642 argsdict-0.0.1/argsdict/
--rw-rw-r--   0 omega     (1000) omega     (1000)       27 2023-07-20 15:17:14.000000 argsdict-0.0.1/argsdict/__init__.py
--rw-rw-r--   0 omega     (1000) omega     (1000)     1168 2023-07-20 15:17:14.000000 argsdict-0.0.1/argsdict/argsdict.py
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-20 15:26:54.437642 argsdict-0.0.1/argsdict.egg-info/
--rw-rw-r--   0 omega     (1000) omega     (1000)      607 2023-07-20 15:26:54.000000 argsdict-0.0.1/argsdict.egg-info/PKG-INFO
--rw-rw-r--   0 omega     (1000) omega     (1000)      196 2023-07-20 15:26:54.000000 argsdict-0.0.1/argsdict.egg-info/SOURCES.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)        1 2023-07-20 15:26:54.000000 argsdict-0.0.1/argsdict.egg-info/dependency_links.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)        9 2023-07-20 15:26:54.000000 argsdict-0.0.1/argsdict.egg-info/top_level.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)       38 2023-07-20 15:26:54.437642 argsdict-0.0.1/setup.cfg
--rw-rw-r--   0 omega     (1000) omega     (1000)      481 2023-07-20 15:17:14.000000 argsdict-0.0.1/setup.py
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 13:08:18.227106 argsdict-1.0.0/
+-rw-rw-r--   0 omega     (1000) omega     (1000)    18092 2023-07-20 15:17:14.000000 argsdict-1.0.0/LICENSE
+-rw-rw-r--   0 omega     (1000) omega     (1000)      607 2023-07-21 13:08:18.227106 argsdict-1.0.0/PKG-INFO
+-rw-rw-r--   0 omega     (1000) omega     (1000)      257 2023-07-20 15:17:14.000000 argsdict-1.0.0/README.md
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 13:08:18.227106 argsdict-1.0.0/argsdict/
+-rw-rw-r--   0 omega     (1000) omega     (1000)       27 2023-07-20 15:17:14.000000 argsdict-1.0.0/argsdict/__init__.py
+-rw-rw-r--   0 omega     (1000) omega     (1000)     1168 2023-07-20 15:17:14.000000 argsdict-1.0.0/argsdict/argsdict.py
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 13:08:18.227106 argsdict-1.0.0/argsdict.egg-info/
+-rw-rw-r--   0 omega     (1000) omega     (1000)      607 2023-07-21 13:08:18.000000 argsdict-1.0.0/argsdict.egg-info/PKG-INFO
+-rw-rw-r--   0 omega     (1000) omega     (1000)      196 2023-07-21 13:08:18.000000 argsdict-1.0.0/argsdict.egg-info/SOURCES.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)        1 2023-07-21 13:08:18.000000 argsdict-1.0.0/argsdict.egg-info/dependency_links.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)        9 2023-07-21 13:08:18.000000 argsdict-1.0.0/argsdict.egg-info/top_level.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)       38 2023-07-21 13:08:18.227106 argsdict-1.0.0/setup.cfg
+-rw-rw-r--   0 omega     (1000) omega     (1000)      481 2023-07-21 13:07:55.000000 argsdict-1.0.0/setup.py
```

### Comparing `argsdict-0.0.1/LICENSE` & `argsdict-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `argsdict-0.0.1/PKG-INFO` & `argsdict-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argsdict
-Version: 0.0.1
+Version: 1.0.0
 Summary: Simple command-line argument parser.
 Home-page: https://github.com/Julynx/argsdict
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Maintainer: Julio Cabria
 Maintainer-email: juliocabria@tutanota.com
 License: GPLv2
```

### Comparing `argsdict-0.0.1/argsdict/argsdict.py` & `argsdict-1.0.0/argsdict/argsdict.py`

 * *Files identical despite different names*

### Comparing `argsdict-0.0.1/argsdict.egg-info/PKG-INFO` & `argsdict-1.0.0/argsdict.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argsdict
-Version: 0.0.1
+Version: 1.0.0
 Summary: Simple command-line argument parser.
 Home-page: https://github.com/Julynx/argsdict
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Maintainer: Julio Cabria
 Maintainer-email: juliocabria@tutanota.com
 License: GPLv2
```

