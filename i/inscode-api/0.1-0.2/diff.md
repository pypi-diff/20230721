# Comparing `tmp/inscode_api-0.1.tar.gz` & `tmp/inscode_api-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inscode_api-0.1.tar", last modified: Fri Jul 21 01:46:04 2023, max compression
+gzip compressed data, was "inscode_api-0.2.tar", last modified: Fri Jul 21 01:56:41 2023, max compression
```

## Comparing `inscode_api-0.1.tar` & `inscode_api-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 01:46:04.178413 inscode_api-0.1/
--rw-r--r--   0 root         (0) root         (0)      457 2023-07-21 01:46:04.178413 inscode_api-0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      151 2023-07-21 01:44:47.000000 inscode_api-0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 01:46:04.178413 inscode_api-0.1/inscode_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      457 2023-07-21 01:46:04.000000 inscode_api-0.1/inscode_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      192 2023-07-21 01:46:04.000000 inscode_api-0.1/inscode_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 01:46:04.000000 inscode_api-0.1/inscode_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-21 01:46:04.000000 inscode_api-0.1/inscode_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 01:46:04.000000 inscode_api-0.1/inscode_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 01:46:04.179413 inscode_api-0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      401 2023-07-21 01:43:21.000000 inscode_api-0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 01:56:41.334426 inscode_api-0.2/
+-rw-r--r--   0 root         (0) root         (0)      457 2023-07-21 01:56:41.334426 inscode_api-0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      151 2023-07-21 01:44:47.000000 inscode_api-0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 01:56:41.334426 inscode_api-0.2/inscode_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      457 2023-07-21 01:56:41.000000 inscode_api-0.2/inscode_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      192 2023-07-21 01:56:41.000000 inscode_api-0.2/inscode_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 01:56:41.000000 inscode_api-0.2/inscode_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-21 01:56:41.000000 inscode_api-0.2/inscode_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 01:56:41.000000 inscode_api-0.2/inscode_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 01:56:41.334426 inscode_api-0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      401 2023-07-21 01:56:21.000000 inscode_api-0.2/setup.py
```

