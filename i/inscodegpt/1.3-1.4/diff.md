# Comparing `tmp/inscodegpt-1.3.tar.gz` & `tmp/inscodegpt-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inscodegpt-1.3.tar", last modified: Thu Jul 20 22:24:08 2023, max compression
+gzip compressed data, was "inscodegpt-1.4.tar", last modified: Thu Jul 20 22:43:50 2023, max compression
```

## Comparing `inscodegpt-1.3.tar` & `inscodegpt-1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:24:08.546293 inscodegpt-1.3/
--rw-r--r--   0 root         (0) root         (0)      212 2023-07-20 22:24:08.546293 inscodegpt-1.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:24:08.545293 inscodegpt-1.3/inscodegpt/
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-20 14:59:24.000000 inscodegpt-1.3/inscodegpt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1196 2023-07-20 22:22:36.000000 inscodegpt-1.3/inscodegpt/inscode_gpt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:24:08.546293 inscodegpt-1.3/inscodegpt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      212 2023-07-20 22:24:08.000000 inscodegpt-1.3/inscodegpt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      226 2023-07-20 22:24:08.000000 inscodegpt-1.3/inscodegpt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:24:08.000000 inscodegpt-1.3/inscodegpt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-20 22:24:08.000000 inscodegpt-1.3/inscodegpt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-20 22:24:08.000000 inscodegpt-1.3/inscodegpt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 22:24:08.546293 inscodegpt-1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      269 2023-07-20 22:23:05.000000 inscodegpt-1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:43:50.162507 inscodegpt-1.4/
+-rw-r--r--   0 root         (0) root         (0)      212 2023-07-20 22:43:50.162507 inscodegpt-1.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:43:50.162507 inscodegpt-1.4/inscodegpt/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-20 14:59:24.000000 inscodegpt-1.4/inscodegpt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-07-20 22:22:36.000000 inscodegpt-1.4/inscodegpt/send_question.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:43:50.162507 inscodegpt-1.4/inscodegpt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      212 2023-07-20 22:43:50.000000 inscodegpt-1.4/inscodegpt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      228 2023-07-20 22:43:50.000000 inscodegpt-1.4/inscodegpt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:43:50.000000 inscodegpt-1.4/inscodegpt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-20 22:43:50.000000 inscodegpt-1.4/inscodegpt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-20 22:43:50.000000 inscodegpt-1.4/inscodegpt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 22:43:50.162507 inscodegpt-1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      269 2023-07-20 22:43:44.000000 inscodegpt-1.4/setup.py
```

### Comparing `inscodegpt-1.3/inscodegpt/inscode_gpt.py` & `inscodegpt-1.4/inscodegpt/send_question.py`

 * *Files identical despite different names*

