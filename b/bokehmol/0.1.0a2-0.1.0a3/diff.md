# Comparing `tmp/bokehmol-0.1.0a2.tar.gz` & `tmp/bokehmol-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bokehmol-0.1.0a2.tar", last modified: Thu Jul 20 23:11:00 2023, max compression
+gzip compressed data, was "bokehmol-0.1.0a3.tar", last modified: Thu Jul 20 23:22:30 2023, max compression
```

## Comparing `bokehmol-0.1.0a2.tar` & `bokehmol-0.1.0a3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:11:00.954417 bokehmol-0.1.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14558 2023-07-20 23:11:00.954417 bokehmol-0.1.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:11:00.950417 bokehmol-0.1.0a2/bokehmol/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/hover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:11:00.954417 bokehmol-0.1.0a2/bokehmol/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/models/base_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/models/base_hover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/models/rdkit_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/models/rdkit_hover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/models/smilesdrawer_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/models/smilesdrawer_hover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:11:00.950417 bokehmol-0.1.0a2/bokehmol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14558 2023-07-20 23:11:00.000000 bokehmol-0.1.0a2/bokehmol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-20 23:11:00.000000 bokehmol-0.1.0a2/bokehmol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 23:11:00.000000 bokehmol-0.1.0a2/bokehmol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 23:11:00.000000 bokehmol-0.1.0a2/bokehmol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 23:11:00.000000 bokehmol-0.1.0a2/bokehmol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 23:11:00.954417 bokehmol-0.1.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:22:30.907032 bokehmol-0.1.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-07-20 23:21:41.000000 bokehmol-0.1.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-20 23:21:41.000000 bokehmol-0.1.0a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14558 2023-07-20 23:22:30.907032 bokehmol-0.1.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-20 23:21:41.000000 bokehmol-0.1.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:22:30.903032 bokehmol-0.1.0a3/bokehmol/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-20 23:21:41.000000 bokehmol-0.1.0a3/bokehmol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 23:21:41.000000 bokehmol-0.1.0a3/bokehmol/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-07-20 23:22:26.000000 bokehmol-0.1.0a3/bokehmol/bokehmol.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-20 23:21:41.000000 bokehmol-0.1.0a3/bokehmol/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-20 23:21:41.000000 bokehmol-0.1.0a3/bokehmol/hover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:22:30.907032 bokehmol-0.1.0a3/bokehmol/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 23:21:41.000000 bokehmol-0.1.0a3/bokehmol/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-20 23:21:41.000000 bokehmol-0.1.0a3/bokehmol/models/base_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-20 23:21:41.000000 bokehmol-0.1.0a3/bokehmol/models/base_hover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-20 23:21:41.000000 bokehmol-0.1.0a3/bokehmol/models/rdkit_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-20 23:21:41.000000 bokehmol-0.1.0a3/bokehmol/models/rdkit_hover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-20 23:21:41.000000 bokehmol-0.1.0a3/bokehmol/models/smilesdrawer_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-20 23:21:41.000000 bokehmol-0.1.0a3/bokehmol/models/smilesdrawer_hover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-20 23:21:41.000000 bokehmol-0.1.0a3/bokehmol/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:22:30.903032 bokehmol-0.1.0a3/bokehmol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14558 2023-07-20 23:22:30.000000 bokehmol-0.1.0a3/bokehmol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-20 23:22:30.000000 bokehmol-0.1.0a3/bokehmol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 23:22:30.000000 bokehmol-0.1.0a3/bokehmol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 23:22:30.000000 bokehmol-0.1.0a3/bokehmol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 23:22:30.000000 bokehmol-0.1.0a3/bokehmol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-20 23:21:41.000000 bokehmol-0.1.0a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 23:22:30.907032 bokehmol-0.1.0a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 23:21:41.000000 bokehmol-0.1.0a3/setup.py
```

### Comparing `bokehmol-0.1.0a2/LICENSE` & `bokehmol-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `bokehmol-0.1.0a2/PKG-INFO` & `bokehmol-0.1.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bokehmol
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: Tools for plotting molecules in Bokeh
 Author-email: Cédric Bouysset <cedric@bouysset.net>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `bokehmol-0.1.0a2/README.md` & `bokehmol-0.1.0a3/README.md`

 * *Files identical despite different names*

### Comparing `bokehmol-0.1.0a2/bokehmol/config.py` & `bokehmol-0.1.0a3/bokehmol/config.py`

 * *Files identical despite different names*

### Comparing `bokehmol-0.1.0a2/bokehmol/hover.py` & `bokehmol-0.1.0a3/bokehmol/hover.py`

 * *Files identical despite different names*

### Comparing `bokehmol-0.1.0a2/bokehmol/models/rdkit_formatter.py` & `bokehmol-0.1.0a3/bokehmol/models/rdkit_formatter.py`

 * *Files identical despite different names*

### Comparing `bokehmol-0.1.0a2/bokehmol/models/smilesdrawer_formatter.py` & `bokehmol-0.1.0a3/bokehmol/models/smilesdrawer_formatter.py`

 * *Files identical despite different names*

### Comparing `bokehmol-0.1.0a2/bokehmol/utils.py` & `bokehmol-0.1.0a3/bokehmol/utils.py`

 * *Files identical despite different names*

### Comparing `bokehmol-0.1.0a2/bokehmol.egg-info/PKG-INFO` & `bokehmol-0.1.0a3/bokehmol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bokehmol
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: Tools for plotting molecules in Bokeh
 Author-email: Cédric Bouysset <cedric@bouysset.net>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `bokehmol-0.1.0a2/bokehmol.egg-info/SOURCES.txt` & `bokehmol-0.1.0a3/bokehmol.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 bokehmol/__init__.py
 bokehmol/_version.py
+bokehmol/bokehmol.min.js
 bokehmol/config.py
 bokehmol/hover.py
 bokehmol/utils.py
 bokehmol.egg-info/PKG-INFO
 bokehmol.egg-info/SOURCES.txt
 bokehmol.egg-info/dependency_links.txt
 bokehmol.egg-info/requires.txt
```

### Comparing `bokehmol-0.1.0a2/pyproject.toml` & `bokehmol-0.1.0a3/pyproject.toml`

 * *Files identical despite different names*

