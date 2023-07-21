# Comparing `tmp/st_circular_progress-0.0.6.tar.gz` & `tmp/st_circular_progress-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_circular_progress-0.0.6.tar", last modified: Fri Jul 21 00:40:08 2023, max compression
+gzip compressed data, was "st_circular_progress-0.1.0.tar", last modified: Fri Jul 21 00:42:32 2023, max compression
```

## Comparing `st_circular_progress-0.0.6.tar` & `st_circular_progress-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 00:40:08.251085 st_circular_progress-0.0.6/
--rw-rw-r--   0 cserrano   (501) staff       (20)     1063 2023-07-12 21:17:31.000000 st_circular_progress-0.0.6/LICENSE
--rw-rw-r--   0 cserrano   (501) staff       (20)       43 2023-07-12 21:17:31.000000 st_circular_progress-0.0.6/MANIFEST.in
--rw-r--r--   0 cserrano   (501) staff       (20)      266 2023-07-21 00:40:08.250702 st_circular_progress-0.0.6/PKG-INFO
--rw-r--r--   0 cserrano   (501) staff       (20)       38 2023-07-21 00:40:08.251246 st_circular_progress-0.0.6/setup.cfg
--rw-rw-r--   0 cserrano   (501) staff       (20)      488 2023-07-21 00:39:51.000000 st_circular_progress-0.0.6/setup.py
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 00:40:08.247171 st_circular_progress-0.0.6/st_circular_progress/
--rw-rw-r--   0 cserrano   (501) staff       (20)     2707 2023-07-21 00:01:57.000000 st_circular_progress-0.0.6/st_circular_progress/__init__.py
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 00:40:08.250094 st_circular_progress-0.0.6/st_circular_progress.egg-info/
--rw-r--r--   0 cserrano   (501) staff       (20)      266 2023-07-21 00:40:08.000000 st_circular_progress-0.0.6/st_circular_progress.egg-info/PKG-INFO
--rw-r--r--   0 cserrano   (501) staff       (20)      280 2023-07-21 00:40:08.000000 st_circular_progress-0.0.6/st_circular_progress.egg-info/SOURCES.txt
--rw-r--r--   0 cserrano   (501) staff       (20)        1 2023-07-21 00:40:08.000000 st_circular_progress-0.0.6/st_circular_progress.egg-info/dependency_links.txt
--rw-r--r--   0 cserrano   (501) staff       (20)       16 2023-07-21 00:40:08.000000 st_circular_progress-0.0.6/st_circular_progress.egg-info/requires.txt
--rw-r--r--   0 cserrano   (501) staff       (20)       21 2023-07-21 00:40:08.000000 st_circular_progress-0.0.6/st_circular_progress.egg-info/top_level.txt
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 00:42:32.500675 st_circular_progress-0.1.0/
+-rw-rw-r--   0 cserrano   (501) staff       (20)     1063 2023-07-12 21:17:31.000000 st_circular_progress-0.1.0/LICENSE
+-rw-rw-r--   0 cserrano   (501) staff       (20)       43 2023-07-12 21:17:31.000000 st_circular_progress-0.1.0/MANIFEST.in
+-rw-r--r--   0 cserrano   (501) staff       (20)      266 2023-07-21 00:42:32.500342 st_circular_progress-0.1.0/PKG-INFO
+-rw-r--r--   0 cserrano   (501) staff       (20)       38 2023-07-21 00:42:32.500798 st_circular_progress-0.1.0/setup.cfg
+-rw-rw-r--   0 cserrano   (501) staff       (20)      488 2023-07-21 00:42:27.000000 st_circular_progress-0.1.0/setup.py
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 00:42:32.496251 st_circular_progress-0.1.0/st_circular_progress/
+-rw-rw-r--   0 cserrano   (501) staff       (20)     2707 2023-07-21 00:01:57.000000 st_circular_progress-0.1.0/st_circular_progress/__init__.py
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 00:42:32.499586 st_circular_progress-0.1.0/st_circular_progress.egg-info/
+-rw-r--r--   0 cserrano   (501) staff       (20)      266 2023-07-21 00:42:32.000000 st_circular_progress-0.1.0/st_circular_progress.egg-info/PKG-INFO
+-rw-r--r--   0 cserrano   (501) staff       (20)      280 2023-07-21 00:42:32.000000 st_circular_progress-0.1.0/st_circular_progress.egg-info/SOURCES.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)        1 2023-07-21 00:42:32.000000 st_circular_progress-0.1.0/st_circular_progress.egg-info/dependency_links.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)       16 2023-07-21 00:42:32.000000 st_circular_progress-0.1.0/st_circular_progress.egg-info/requires.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)       21 2023-07-21 00:42:32.000000 st_circular_progress-0.1.0/st_circular_progress.egg-info/top_level.txt
```

### Comparing `st_circular_progress-0.0.6/LICENSE` & `st_circular_progress-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `st_circular_progress-0.0.6/st_circular_progress/__init__.py` & `st_circular_progress-0.1.0/st_circular_progress/__init__.py`

 * *Files identical despite different names*

