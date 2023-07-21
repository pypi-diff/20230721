# Comparing `tmp/st_circular_progress-0.1.1.tar.gz` & `tmp/st_circular_progress-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_circular_progress-0.1.1.tar", last modified: Fri Jul 21 01:23:35 2023, max compression
+gzip compressed data, was "st_circular_progress-0.1.2.tar", last modified: Fri Jul 21 01:24:57 2023, max compression
```

## Comparing `st_circular_progress-0.1.1.tar` & `st_circular_progress-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 01:23:35.012142 st_circular_progress-0.1.1/
--rw-rw-r--   0 cserrano   (501) staff       (20)     1063 2023-07-12 21:17:31.000000 st_circular_progress-0.1.1/LICENSE
--rw-rw-r--   0 cserrano   (501) staff       (20)       43 2023-07-12 21:17:31.000000 st_circular_progress-0.1.1/MANIFEST.in
--rw-r--r--   0 cserrano   (501) staff       (20)      317 2023-07-21 01:23:35.011797 st_circular_progress-0.1.1/PKG-INFO
--rw-r--r--   0 cserrano   (501) staff       (20)       38 2023-07-21 01:23:35.012255 st_circular_progress-0.1.1/setup.cfg
--rw-rw-r--   0 cserrano   (501) staff       (20)      539 2023-07-21 01:23:29.000000 st_circular_progress-0.1.1/setup.py
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 01:23:35.008226 st_circular_progress-0.1.1/st_circular_progress/
--rw-rw-r--   0 cserrano   (501) staff       (20)     2707 2023-07-21 00:01:57.000000 st_circular_progress-0.1.1/st_circular_progress/__init__.py
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 01:23:35.011004 st_circular_progress-0.1.1/st_circular_progress.egg-info/
--rw-r--r--   0 cserrano   (501) staff       (20)      317 2023-07-21 01:23:34.000000 st_circular_progress-0.1.1/st_circular_progress.egg-info/PKG-INFO
--rw-r--r--   0 cserrano   (501) staff       (20)      280 2023-07-21 01:23:34.000000 st_circular_progress-0.1.1/st_circular_progress.egg-info/SOURCES.txt
--rw-r--r--   0 cserrano   (501) staff       (20)        1 2023-07-21 01:23:34.000000 st_circular_progress-0.1.1/st_circular_progress.egg-info/dependency_links.txt
--rw-r--r--   0 cserrano   (501) staff       (20)       16 2023-07-21 01:23:34.000000 st_circular_progress-0.1.1/st_circular_progress.egg-info/requires.txt
--rw-r--r--   0 cserrano   (501) staff       (20)       21 2023-07-21 01:23:34.000000 st_circular_progress-0.1.1/st_circular_progress.egg-info/top_level.txt
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 01:24:57.500671 st_circular_progress-0.1.2/
+-rw-rw-r--   0 cserrano   (501) staff       (20)     1063 2023-07-12 21:17:31.000000 st_circular_progress-0.1.2/LICENSE
+-rw-rw-r--   0 cserrano   (501) staff       (20)       43 2023-07-12 21:17:31.000000 st_circular_progress-0.1.2/MANIFEST.in
+-rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 01:24:57.500039 st_circular_progress-0.1.2/PKG-INFO
+-rw-r--r--   0 cserrano   (501) staff       (20)       38 2023-07-21 01:24:57.500899 st_circular_progress-0.1.2/setup.cfg
+-rw-rw-r--   0 cserrano   (501) staff       (20)      631 2023-07-21 01:24:50.000000 st_circular_progress-0.1.2/setup.py
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 01:24:57.494171 st_circular_progress-0.1.2/st_circular_progress/
+-rw-rw-r--   0 cserrano   (501) staff       (20)     2707 2023-07-21 00:01:57.000000 st_circular_progress-0.1.2/st_circular_progress/__init__.py
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 01:24:57.498828 st_circular_progress-0.1.2/st_circular_progress.egg-info/
+-rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 01:24:57.000000 st_circular_progress-0.1.2/st_circular_progress.egg-info/PKG-INFO
+-rw-r--r--   0 cserrano   (501) staff       (20)      280 2023-07-21 01:24:57.000000 st_circular_progress-0.1.2/st_circular_progress.egg-info/SOURCES.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)        1 2023-07-21 01:24:57.000000 st_circular_progress-0.1.2/st_circular_progress.egg-info/dependency_links.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)       16 2023-07-21 01:24:57.000000 st_circular_progress-0.1.2/st_circular_progress.egg-info/requires.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)       21 2023-07-21 01:24:57.000000 st_circular_progress-0.1.2/st_circular_progress.egg-info/top_level.txt
```

### Comparing `st_circular_progress-0.1.1/LICENSE` & `st_circular_progress-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `st_circular_progress-0.1.1/st_circular_progress/__init__.py` & `st_circular_progress-0.1.2/st_circular_progress/__init__.py`

 * *Files identical despite different names*

