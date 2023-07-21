# Comparing `tmp/covert-ots-1.0.4.tar.gz` & `tmp/covert-ots-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covert-ots-1.0.4.tar", last modified: Tue Jul 18 05:16:22 2023, max compression
+gzip compressed data, was "covert-ots-1.0.5.tar", last modified: Fri Jul 21 10:38:59 2023, max compression
```

## Comparing `covert-ots-1.0.4.tar` & `covert-ots-1.0.5.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxrwxr-x   0 om        (1001) om        (1001)        0 2023-07-18 05:16:22.557430 covert-ots-1.0.4/
--rw-rw-r--   0 om        (1001) om        (1001)      135 2023-07-18 05:16:22.557430 covert-ots-1.0.4/PKG-INFO
-drwxrwxr-x   0 om        (1001) om        (1001)        0 2023-07-18 05:16:22.557430 covert-ots-1.0.4/covert_ots.egg-info/
--rw-rw-r--   0 om        (1001) om        (1001)      135 2023-07-18 05:16:22.000000 covert-ots-1.0.4/covert_ots.egg-info/PKG-INFO
--rw-rw-r--   0 om        (1001) om        (1001)      214 2023-07-18 05:16:22.000000 covert-ots-1.0.4/covert_ots.egg-info/SOURCES.txt
--rw-rw-r--   0 om        (1001) om        (1001)        1 2023-07-18 05:16:22.000000 covert-ots-1.0.4/covert_ots.egg-info/dependency_links.txt
--rw-rw-r--   0 om        (1001) om        (1001)       66 2023-07-18 05:16:22.000000 covert-ots-1.0.4/covert_ots.egg-info/entry_points.txt
--rw-rw-r--   0 om        (1001) om        (1001)       33 2023-07-18 05:16:22.000000 covert-ots-1.0.4/covert_ots.egg-info/requires.txt
--rw-rw-r--   0 om        (1001) om        (1001)        1 2023-07-18 05:16:22.000000 covert-ots-1.0.4/covert_ots.egg-info/top_level.txt
--rw-rw-r--   0 om        (1001) om        (1001)       38 2023-07-18 05:16:22.557430 covert-ots-1.0.4/setup.cfg
--rw-rw-r--   0 om        (1001) om        (1001)      309 2023-07-18 05:16:19.000000 covert-ots-1.0.4/setup.py
+drwxrwxr-x   0 om        (1001) om        (1001)        0 2023-07-21 10:38:59.445696 covert-ots-1.0.5/
+-rw-rw-r--   0 om        (1001) om        (1001)     1154 2023-07-21 10:38:59.445696 covert-ots-1.0.5/PKG-INFO
+drwxrwxr-x   0 om        (1001) om        (1001)        0 2023-07-21 10:38:59.445696 covert-ots-1.0.5/covert_ots.egg-info/
+-rw-rw-r--   0 om        (1001) om        (1001)     1154 2023-07-21 10:38:59.000000 covert-ots-1.0.5/covert_ots.egg-info/PKG-INFO
+-rw-rw-r--   0 om        (1001) om        (1001)      177 2023-07-21 10:38:59.000000 covert-ots-1.0.5/covert_ots.egg-info/SOURCES.txt
+-rw-rw-r--   0 om        (1001) om        (1001)        1 2023-07-21 10:38:59.000000 covert-ots-1.0.5/covert_ots.egg-info/dependency_links.txt
+-rw-rw-r--   0 om        (1001) om        (1001)       33 2023-07-21 10:38:59.000000 covert-ots-1.0.5/covert_ots.egg-info/requires.txt
+-rw-rw-r--   0 om        (1001) om        (1001)       12 2023-07-21 10:38:59.000000 covert-ots-1.0.5/covert_ots.egg-info/top_level.txt
+-rw-rw-r--   0 om        (1001) om        (1001)       38 2023-07-21 10:38:59.445696 covert-ots-1.0.5/setup.cfg
+-rw-rw-r--   0 om        (1001) om        (1001)      775 2023-07-21 10:37:52.000000 covert-ots-1.0.5/setup.py
```

