# Comparing `tmp/doppkit-0.1.6.tar.gz` & `tmp/doppkit-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doppkit-0.1.6.tar", last modified: Mon Apr 10 18:53:19 2023, max compression
+gzip compressed data, was "doppkit-0.1.7.tar", last modified: Mon Apr 10 19:33:50 2023, max compression
```

## Comparing `doppkit-0.1.6.tar` & `doppkit-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:53:19.870739 doppkit-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 18:53:01.000000 doppkit-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-04-10 18:53:19.870739 doppkit-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-10 18:53:01.000000 doppkit-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-10 18:53:01.000000 doppkit-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 18:53:19.870739 doppkit-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:53:19.866739 doppkit-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:53:19.870739 doppkit-0.1.6/src/doppkit/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 18:53:01.000000 doppkit-0.1.6/src/doppkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-10 18:53:01.000000 doppkit-0.1.6/src/doppkit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-10 18:53:01.000000 doppkit-0.1.6/src/doppkit/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-10 18:53:01.000000 doppkit-0.1.6/src/doppkit/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-10 18:53:01.000000 doppkit-0.1.6/src/doppkit/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-10 18:53:01.000000 doppkit-0.1.6/src/doppkit/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-10 18:53:01.000000 doppkit-0.1.6/src/doppkit/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:53:19.870739 doppkit-0.1.6/src/doppkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-04-10 18:53:19.000000 doppkit-0.1.6/src/doppkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-10 18:53:19.000000 doppkit-0.1.6/src/doppkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:53:19.000000 doppkit-0.1.6/src/doppkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-10 18:53:19.000000 doppkit-0.1.6/src/doppkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:53:19.000000 doppkit-0.1.6/src/doppkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-10 18:53:19.000000 doppkit-0.1.6/src/doppkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 18:53:19.000000 doppkit-0.1.6/src/doppkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:33:50.321041 doppkit-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 19:33:36.000000 doppkit-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-04-10 19:33:50.321041 doppkit-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-10 19:33:36.000000 doppkit-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-10 19:33:36.000000 doppkit-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 19:33:50.321041 doppkit-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:33:50.317041 doppkit-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:33:50.321041 doppkit-0.1.7/src/doppkit/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 19:33:36.000000 doppkit-0.1.7/src/doppkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-10 19:33:36.000000 doppkit-0.1.7/src/doppkit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-10 19:33:36.000000 doppkit-0.1.7/src/doppkit/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-10 19:33:36.000000 doppkit-0.1.7/src/doppkit/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-10 19:33:36.000000 doppkit-0.1.7/src/doppkit/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-10 19:33:36.000000 doppkit-0.1.7/src/doppkit/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-10 19:33:36.000000 doppkit-0.1.7/src/doppkit/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:33:50.321041 doppkit-0.1.7/src/doppkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-04-10 19:33:50.000000 doppkit-0.1.7/src/doppkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-10 19:33:50.000000 doppkit-0.1.7/src/doppkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:33:50.000000 doppkit-0.1.7/src/doppkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-10 19:33:50.000000 doppkit-0.1.7/src/doppkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:33:50.000000 doppkit-0.1.7/src/doppkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-10 19:33:50.000000 doppkit-0.1.7/src/doppkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 19:33:50.000000 doppkit-0.1.7/src/doppkit.egg-info/top_level.txt
```

### Comparing `doppkit-0.1.6/LICENSE` & `doppkit-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.6/PKG-INFO` & `doppkit-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppkit
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tool to allow retrival of USACE GRiD data
 Maintainer-email: Ognyan Moore <ogi@hobu.co>, Howard Butler <howard@hobu.co>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `doppkit-0.1.6/pyproject.toml` & `doppkit-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.6/src/doppkit/app.py` & `doppkit-0.1.7/src/doppkit/app.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.6/src/doppkit/cache.py` & `doppkit-0.1.7/src/doppkit/cache.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.6/src/doppkit/grid.py` & `doppkit-0.1.7/src/doppkit/grid.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.6/src/doppkit/list.py` & `doppkit-0.1.7/src/doppkit/list.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.6/src/doppkit/sync.py` & `doppkit-0.1.7/src/doppkit/sync.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.6/src/doppkit.egg-info/PKG-INFO` & `doppkit-0.1.7/src/doppkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppkit
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tool to allow retrival of USACE GRiD data
 Maintainer-email: Ognyan Moore <ogi@hobu.co>, Howard Butler <howard@hobu.co>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

