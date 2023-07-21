# Comparing `tmp/skale-contracts-0.0.1.dev9714958449586304.tar.gz` & `tmp/skale-contracts-0.0.1.dev978114706300915430.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skale-contracts-0.0.1.dev9714958449586304.tar", last modified: Mon Jul 17 14:11:22 2023, max compression
+gzip compressed data, was "skale-contracts-0.0.1.dev978114706300915430.tar", last modified: Tue Jul 18 17:16:45 2023, max compression
```

## Comparing `skale-contracts-0.0.1.dev9714958449586304.tar` & `skale-contracts-0.0.1.dev978114706300915430.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:11:22.768346 skale-contracts-0.0.1.dev9714958449586304/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-17 14:11:22.768346 skale-contracts-0.0.1.dev9714958449586304/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-17 14:11:07.000000 skale-contracts-0.0.1.dev9714958449586304/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-17 14:11:07.000000 skale-contracts-0.0.1.dev9714958449586304/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-17 14:11:22.768346 skale-contracts-0.0.1.dev9714958449586304/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:11:22.768346 skale-contracts-0.0.1.dev9714958449586304/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:11:22.768346 skale-contracts-0.0.1.dev9714958449586304/src/skale_contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-17 14:11:07.000000 skale-contracts-0.0.1.dev9714958449586304/src/skale_contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-17 14:11:07.000000 skale-contracts-0.0.1.dev9714958449586304/src/skale_contracts/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-17 14:11:07.000000 skale-contracts-0.0.1.dev9714958449586304/src/skale_contracts/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-17 14:11:07.000000 skale-contracts-0.0.1.dev9714958449586304/src/skale_contracts/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-17 14:11:07.000000 skale-contracts-0.0.1.dev9714958449586304/src/skale_contracts/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-17 14:11:07.000000 skale-contracts-0.0.1.dev9714958449586304/src/skale_contracts/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-17 14:11:07.000000 skale-contracts-0.0.1.dev9714958449586304/src/skale_contracts/skale_contracts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:11:22.768346 skale-contracts-0.0.1.dev9714958449586304/src/skale_contracts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-17 14:11:22.000000 skale-contracts-0.0.1.dev9714958449586304/src/skale_contracts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-17 14:11:22.000000 skale-contracts-0.0.1.dev9714958449586304/src/skale_contracts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:11:22.000000 skale-contracts-0.0.1.dev9714958449586304/src/skale_contracts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 14:11:22.000000 skale-contracts-0.0.1.dev9714958449586304/src/skale_contracts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 14:11:22.000000 skale-contracts-0.0.1.dev9714958449586304/src/skale_contracts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-17 14:11:15.000000 skale-contracts-0.0.1.dev9714958449586304/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:16:45.731326 skale-contracts-0.0.1.dev978114706300915430/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-18 17:16:45.731326 skale-contracts-0.0.1.dev978114706300915430/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-18 17:16:23.000000 skale-contracts-0.0.1.dev978114706300915430/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-18 17:16:23.000000 skale-contracts-0.0.1.dev978114706300915430/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-18 17:16:45.731326 skale-contracts-0.0.1.dev978114706300915430/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:16:45.727326 skale-contracts-0.0.1.dev978114706300915430/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:16:45.727326 skale-contracts-0.0.1.dev978114706300915430/src/skale_contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-18 17:16:23.000000 skale-contracts-0.0.1.dev978114706300915430/src/skale_contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-18 17:16:23.000000 skale-contracts-0.0.1.dev978114706300915430/src/skale_contracts/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-18 17:16:23.000000 skale-contracts-0.0.1.dev978114706300915430/src/skale_contracts/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-18 17:16:23.000000 skale-contracts-0.0.1.dev978114706300915430/src/skale_contracts/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-18 17:16:23.000000 skale-contracts-0.0.1.dev978114706300915430/src/skale_contracts/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-18 17:16:23.000000 skale-contracts-0.0.1.dev978114706300915430/src/skale_contracts/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-18 17:16:23.000000 skale-contracts-0.0.1.dev978114706300915430/src/skale_contracts/skale_contracts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:16:45.731326 skale-contracts-0.0.1.dev978114706300915430/src/skale_contracts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-18 17:16:45.000000 skale-contracts-0.0.1.dev978114706300915430/src/skale_contracts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-18 17:16:45.000000 skale-contracts-0.0.1.dev978114706300915430/src/skale_contracts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 17:16:45.000000 skale-contracts-0.0.1.dev978114706300915430/src/skale_contracts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-18 17:16:45.000000 skale-contracts-0.0.1.dev978114706300915430/src/skale_contracts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 17:16:45.000000 skale-contracts-0.0.1.dev978114706300915430/src/skale_contracts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 17:16:36.000000 skale-contracts-0.0.1.dev978114706300915430/version.txt
```

### Comparing `skale-contracts-0.0.1.dev9714958449586304/setup.cfg` & `skale-contracts-0.0.1.dev978114706300915430/setup.cfg`

 * *Files identical despite different names*

### Comparing `skale-contracts-0.0.1.dev9714958449586304/src/skale_contracts/instance.py` & `skale-contracts-0.0.1.dev978114706300915430/src/skale_contracts/instance.py`

 * *Files identical despite different names*

### Comparing `skale-contracts-0.0.1.dev9714958449586304/src/skale_contracts/metadata.py` & `skale-contracts-0.0.1.dev978114706300915430/src/skale_contracts/metadata.py`

 * *Files identical despite different names*

### Comparing `skale-contracts-0.0.1.dev9714958449586304/src/skale_contracts/network.py` & `skale-contracts-0.0.1.dev978114706300915430/src/skale_contracts/network.py`

 * *Files identical despite different names*

### Comparing `skale-contracts-0.0.1.dev9714958449586304/src/skale_contracts/project.py` & `skale-contracts-0.0.1.dev978114706300915430/src/skale_contracts/project.py`

 * *Files identical despite different names*

### Comparing `skale-contracts-0.0.1.dev9714958449586304/src/skale_contracts/skale_contracts.py` & `skale-contracts-0.0.1.dev978114706300915430/src/skale_contracts/skale_contracts.py`

 * *Files identical despite different names*

