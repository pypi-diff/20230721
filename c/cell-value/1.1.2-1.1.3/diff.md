# Comparing `tmp/cell_value-1.1.2.tar.gz` & `tmp/cell_value-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cell_value-1.1.2.tar", last modified: Fri Jul 21 07:58:15 2023, max compression
+gzip compressed data, was "dist/cell_value-1.1.3.tar", last modified: Fri Jul 21 09:41:01 2023, max compression
```

## Comparing `cell_value-1.1.2.tar` & `cell_value-1.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 caiman     (501) staff       (20)        0 2023-07-21 07:58:15.000000 cell_value-1.1.2/
--rw-r--r--   0 caiman     (501) staff       (20)      143 2023-07-21 07:58:15.000000 cell_value-1.1.2/PKG-INFO
-drwxr-xr-x   0 caiman     (501) staff       (20)        0 2023-07-21 07:58:15.000000 cell_value-1.1.2/cell_value/
--rw-r--r--   0 caiman     (501) staff       (20)     4088 2023-07-21 07:57:05.000000 cell_value-1.1.2/cell_value/__init__.py
-drwxr-xr-x   0 caiman     (501) staff       (20)        0 2023-07-21 07:58:15.000000 cell_value-1.1.2/cell_value.egg-info/
--rw-r--r--   0 caiman     (501) staff       (20)      143 2023-07-21 07:58:15.000000 cell_value-1.1.2/cell_value.egg-info/PKG-INFO
--rw-r--r--   0 caiman     (501) staff       (20)      167 2023-07-21 07:58:15.000000 cell_value-1.1.2/cell_value.egg-info/SOURCES.txt
--rw-r--r--   0 caiman     (501) staff       (20)        1 2023-07-21 07:58:15.000000 cell_value-1.1.2/cell_value.egg-info/dependency_links.txt
--rw-r--r--   0 caiman     (501) staff       (20)       11 2023-07-21 07:58:15.000000 cell_value-1.1.2/cell_value.egg-info/top_level.txt
--rw-r--r--   0 caiman     (501) staff       (20)       38 2023-07-21 07:58:15.000000 cell_value-1.1.2/setup.cfg
--rw-r--r--   0 caiman     (501) staff       (20)      276 2023-07-21 07:58:12.000000 cell_value-1.1.2/setup.py
+drwxr-xr-x   0 caiman     (501) staff       (20)        0 2023-07-21 09:41:01.000000 cell_value-1.1.3/
+-rw-r--r--   0 caiman     (501) staff       (20)      143 2023-07-21 09:41:01.000000 cell_value-1.1.3/PKG-INFO
+drwxr-xr-x   0 caiman     (501) staff       (20)        0 2023-07-21 09:41:01.000000 cell_value-1.1.3/cell_value/
+-rw-r--r--   0 caiman     (501) staff       (20)     4088 2023-07-21 07:57:05.000000 cell_value-1.1.3/cell_value/__init__.py
+drwxr-xr-x   0 caiman     (501) staff       (20)        0 2023-07-21 09:41:01.000000 cell_value-1.1.3/cell_value.egg-info/
+-rw-r--r--   0 caiman     (501) staff       (20)      143 2023-07-21 09:41:01.000000 cell_value-1.1.3/cell_value.egg-info/PKG-INFO
+-rw-r--r--   0 caiman     (501) staff       (20)      167 2023-07-21 09:41:01.000000 cell_value-1.1.3/cell_value.egg-info/SOURCES.txt
+-rw-r--r--   0 caiman     (501) staff       (20)        1 2023-07-21 09:41:01.000000 cell_value-1.1.3/cell_value.egg-info/dependency_links.txt
+-rw-r--r--   0 caiman     (501) staff       (20)       11 2023-07-21 09:41:01.000000 cell_value-1.1.3/cell_value.egg-info/top_level.txt
+-rw-r--r--   0 caiman     (501) staff       (20)       38 2023-07-21 09:41:01.000000 cell_value-1.1.3/setup.cfg
+-rw-r--r--   0 caiman     (501) staff       (20)      276 2023-07-21 09:40:16.000000 cell_value-1.1.3/setup.py
```

### Comparing `cell_value-1.1.2/cell_value/__init__.py` & `cell_value-1.1.3/cell_value/__init__.py`

 * *Files identical despite different names*

