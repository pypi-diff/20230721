# Comparing `tmp/inscode_api-0.3.tar.gz` & `tmp/inscode_api-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inscode_api-0.3.tar", last modified: Fri Jul 21 02:03:52 2023, max compression
+gzip compressed data, was "inscode_api-0.4.tar", last modified: Fri Jul 21 02:23:19 2023, max compression
```

## Comparing `inscode_api-0.3.tar` & `inscode_api-0.4.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 02:03:52.713115 inscode_api-0.3/
--rw-r--r--   0 root         (0) root         (0)      457 2023-07-21 02:03:52.713115 inscode_api-0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      151 2023-07-21 01:44:47.000000 inscode_api-0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 02:03:52.713115 inscode_api-0.3/inscode_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      457 2023-07-21 02:03:52.000000 inscode_api-0.3/inscode_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      192 2023-07-21 02:03:52.000000 inscode_api-0.3/inscode_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 02:03:52.000000 inscode_api-0.3/inscode_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-21 02:03:52.000000 inscode_api-0.3/inscode_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 02:03:52.000000 inscode_api-0.3/inscode_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 02:03:52.713115 inscode_api-0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      401 2023-07-21 02:03:46.000000 inscode_api-0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 02:23:19.096969 inscode_api-0.4/
+-rw-r--r--   0 root         (0) root         (0)      457 2023-07-21 02:23:19.095968 inscode_api-0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      151 2023-07-21 01:44:47.000000 inscode_api-0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 02:23:19.095968 inscode_api-0.4/inscode_api/
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-21 02:14:41.000000 inscode_api-0.4/inscode_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1289 2023-07-21 01:44:14.000000 inscode_api-0.4/inscode_api/send_question.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 02:23:19.095968 inscode_api-0.4/inscode_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      457 2023-07-21 02:23:19.000000 inscode_api-0.4/inscode_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      245 2023-07-21 02:23:19.000000 inscode_api-0.4/inscode_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 02:23:19.000000 inscode_api-0.4/inscode_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-21 02:23:19.000000 inscode_api-0.4/inscode_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-21 02:23:19.000000 inscode_api-0.4/inscode_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 02:23:19.096969 inscode_api-0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      401 2023-07-21 02:23:13.000000 inscode_api-0.4/setup.py
```

