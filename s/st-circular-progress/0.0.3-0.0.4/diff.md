# Comparing `tmp/st_circular_progress-0.0.3.tar.gz` & `tmp/st_circular_progress-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_circular_progress-0.0.3.tar", last modified: Thu Jul 20 23:45:37 2023, max compression
+gzip compressed data, was "st_circular_progress-0.0.4.tar", last modified: Fri Jul 21 00:02:43 2023, max compression
```

## Comparing `st_circular_progress-0.0.3.tar` & `st_circular_progress-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-20 23:45:37.431352 st_circular_progress-0.0.3/
--rw-rw-r--   0 cserrano   (501) staff       (20)     1063 2023-07-12 21:17:31.000000 st_circular_progress-0.0.3/LICENSE
--rw-rw-r--   0 cserrano   (501) staff       (20)       43 2023-07-12 21:17:31.000000 st_circular_progress-0.0.3/MANIFEST.in
--rw-r--r--   0 cserrano   (501) staff       (20)      266 2023-07-20 23:45:37.431004 st_circular_progress-0.0.3/PKG-INFO
--rw-r--r--   0 cserrano   (501) staff       (20)       38 2023-07-20 23:45:37.431461 st_circular_progress-0.0.3/setup.cfg
--rw-rw-r--   0 cserrano   (501) staff       (20)      488 2023-07-20 23:45:20.000000 st_circular_progress-0.0.3/setup.py
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-20 23:45:37.426591 st_circular_progress-0.0.3/st_circular_progress/
--rw-rw-r--   0 cserrano   (501) staff       (20)     2708 2023-07-20 23:25:11.000000 st_circular_progress-0.0.3/st_circular_progress/__init__.py
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-20 23:45:37.430268 st_circular_progress-0.0.3/st_circular_progress.egg-info/
--rw-r--r--   0 cserrano   (501) staff       (20)      266 2023-07-20 23:45:37.000000 st_circular_progress-0.0.3/st_circular_progress.egg-info/PKG-INFO
--rw-r--r--   0 cserrano   (501) staff       (20)      280 2023-07-20 23:45:37.000000 st_circular_progress-0.0.3/st_circular_progress.egg-info/SOURCES.txt
--rw-r--r--   0 cserrano   (501) staff       (20)        1 2023-07-20 23:45:37.000000 st_circular_progress-0.0.3/st_circular_progress.egg-info/dependency_links.txt
--rw-r--r--   0 cserrano   (501) staff       (20)       16 2023-07-20 23:45:37.000000 st_circular_progress-0.0.3/st_circular_progress.egg-info/requires.txt
--rw-r--r--   0 cserrano   (501) staff       (20)       21 2023-07-20 23:45:37.000000 st_circular_progress-0.0.3/st_circular_progress.egg-info/top_level.txt
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 00:02:43.573049 st_circular_progress-0.0.4/
+-rw-rw-r--   0 cserrano   (501) staff       (20)     1063 2023-07-12 21:17:31.000000 st_circular_progress-0.0.4/LICENSE
+-rw-rw-r--   0 cserrano   (501) staff       (20)       43 2023-07-12 21:17:31.000000 st_circular_progress-0.0.4/MANIFEST.in
+-rw-r--r--   0 cserrano   (501) staff       (20)      266 2023-07-21 00:02:43.572672 st_circular_progress-0.0.4/PKG-INFO
+-rw-r--r--   0 cserrano   (501) staff       (20)       38 2023-07-21 00:02:43.573220 st_circular_progress-0.0.4/setup.cfg
+-rw-rw-r--   0 cserrano   (501) staff       (20)      488 2023-07-21 00:02:30.000000 st_circular_progress-0.0.4/setup.py
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 00:02:43.568501 st_circular_progress-0.0.4/st_circular_progress/
+-rw-rw-r--   0 cserrano   (501) staff       (20)     2707 2023-07-21 00:01:57.000000 st_circular_progress-0.0.4/st_circular_progress/__init__.py
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 00:02:43.571899 st_circular_progress-0.0.4/st_circular_progress.egg-info/
+-rw-r--r--   0 cserrano   (501) staff       (20)      266 2023-07-21 00:02:43.000000 st_circular_progress-0.0.4/st_circular_progress.egg-info/PKG-INFO
+-rw-r--r--   0 cserrano   (501) staff       (20)      280 2023-07-21 00:02:43.000000 st_circular_progress-0.0.4/st_circular_progress.egg-info/SOURCES.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)        1 2023-07-21 00:02:43.000000 st_circular_progress-0.0.4/st_circular_progress.egg-info/dependency_links.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)       16 2023-07-21 00:02:43.000000 st_circular_progress-0.0.4/st_circular_progress.egg-info/requires.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)       21 2023-07-21 00:02:43.000000 st_circular_progress-0.0.4/st_circular_progress.egg-info/top_level.txt
```

### Comparing `st_circular_progress-0.0.3/LICENSE` & `st_circular_progress-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `st_circular_progress-0.0.3/st_circular_progress/__init__.py` & `st_circular_progress-0.0.4/st_circular_progress/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import streamlit.components.v1 as components
-import time
-import uuid
+import streamlit as st
 
 _RELEASE = True
 
 
 if not _RELEASE:
     _st_circular_progress_component = components.declare_component(
         "st_circular_progress",
```

