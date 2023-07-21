# Comparing `tmp/operatorio-0.1.2.tar.gz` & `tmp/operatorio-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "operatorio-0.1.2.tar", last modified: Fri Jul 21 06:10:02 2023, max compression
+gzip compressed data, was "operatorio-0.1.3.tar", last modified: Fri Jul 21 06:13:47 2023, max compression
```

## Comparing `operatorio-0.1.2.tar` & `operatorio-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 06:10:02.510745 operatorio-0.1.2/
--rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 06:10:02.510438 operatorio-0.1.2/PKG-INFO
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 06:10:02.509367 operatorio-0.1.2/operatorio.egg-info/
--rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 06:10:02.000000 operatorio-0.1.2/operatorio.egg-info/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)      205 2023-07-21 06:10:02.000000 operatorio-0.1.2/operatorio.egg-info/SOURCES.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2023-07-21 06:10:02.000000 operatorio-0.1.2/operatorio.egg-info/dependency_links.txt
--rw-r--r--   0 david      (501) staff       (20)        9 2023-07-21 06:10:02.000000 operatorio-0.1.2/operatorio.egg-info/requires.txt
--rw-r--r--   0 david      (501) staff       (20)        4 2023-07-21 06:10:02.000000 operatorio-0.1.2/operatorio.egg-info/top_level.txt
--rw-r--r--   0 david      (501) staff       (20)       38 2023-07-21 06:10:02.510813 operatorio-0.1.2/setup.cfg
--rw-r--r--   0 david      (501) staff       (20)      530 2023-07-21 06:09:41.000000 operatorio-0.1.2/setup.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 06:10:02.510003 operatorio-0.1.2/src/
--rw-r--r--   0 david      (501) staff       (20)      113 2023-07-21 06:08:03.000000 operatorio-0.1.2/src/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     1322 2023-07-21 04:30:59.000000 operatorio-0.1.2/src/main.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 06:13:47.774939 operatorio-0.1.3/
+-rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 06:13:47.774694 operatorio-0.1.3/PKG-INFO
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 06:13:47.773165 operatorio-0.1.3/operatorio/
+-rw-r--r--   0 david      (501) staff       (20)      113 2023-07-21 06:08:03.000000 operatorio-0.1.3/operatorio/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     1322 2023-07-21 04:30:59.000000 operatorio-0.1.3/operatorio/main.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 06:13:47.774375 operatorio-0.1.3/operatorio.egg-info/
+-rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 06:13:47.000000 operatorio-0.1.3/operatorio.egg-info/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)      219 2023-07-21 06:13:47.000000 operatorio-0.1.3/operatorio.egg-info/SOURCES.txt
+-rw-r--r--   0 david      (501) staff       (20)        1 2023-07-21 06:13:47.000000 operatorio-0.1.3/operatorio.egg-info/dependency_links.txt
+-rw-r--r--   0 david      (501) staff       (20)        9 2023-07-21 06:13:47.000000 operatorio-0.1.3/operatorio.egg-info/requires.txt
+-rw-r--r--   0 david      (501) staff       (20)       11 2023-07-21 06:13:47.000000 operatorio-0.1.3/operatorio.egg-info/top_level.txt
+-rw-r--r--   0 david      (501) staff       (20)       38 2023-07-21 06:13:47.775004 operatorio-0.1.3/setup.cfg
+-rw-r--r--   0 david      (501) staff       (20)      532 2023-07-21 06:13:39.000000 operatorio-0.1.3/setup.py
```

### Comparing `operatorio-0.1.2/src/main.py` & `operatorio-0.1.3/operatorio/main.py`

 * *Files identical despite different names*

