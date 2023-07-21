# Comparing `tmp/bec-server-0.13.1.tar.gz` & `tmp/bec-server-0.13.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec-server-0.13.1.tar", last modified: Tue Jul 18 12:57:25 2023, max compression
+gzip compressed data, was "bec-server-0.13.2.tar", last modified: Fri Jul 21 07:52:35 2023, max compression
```

## Comparing `bec-server-0.13.1.tar` & `bec-server-0.13.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:57:25.424679 bec-server-0.13.1/
--rw-r--r--   0 root         (0) root         (0)      443 2023-07-18 12:57:25.424679 bec-server-0.13.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:57:25.423679 bec-server-0.13.1/bec_server/
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-08 15:33:35.000000 bec-server-0.13.1/bec_server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1309 2023-07-08 15:33:35.000000 bec-server-0.13.1/bec_server/launch.py
--rw-r--r--   0 root         (0) root         (0)     3075 2023-07-08 15:33:35.000000 bec-server-0.13.1/bec_server/service_handler.py
--rw-r--r--   0 root         (0) root         (0)     2345 2023-07-08 15:33:35.000000 bec-server-0.13.1/bec_server/tmux_launch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:57:25.424679 bec-server-0.13.1/bec_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      443 2023-07-18 12:57:25.000000 bec-server-0.13.1/bec_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      332 2023-07-18 12:57:25.000000 bec-server-0.13.1/bec_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 12:57:25.000000 bec-server-0.13.1/bec_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-07-18 12:57:25.000000 bec-server-0.13.1/bec_server.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-07-18 12:57:25.000000 bec-server-0.13.1/bec_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-18 12:57:25.000000 bec-server-0.13.1/bec_server.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      503 2023-07-18 12:57:25.425679 bec-server-0.13.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1068 2023-07-08 15:33:35.000000 bec-server-0.13.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:52:35.470386 bec-server-0.13.2/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-07-21 07:52:35.470386 bec-server-0.13.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:52:35.469386 bec-server-0.13.2/bec_server/
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-08 15:47:18.000000 bec-server-0.13.2/bec_server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2023-07-08 15:47:18.000000 bec-server-0.13.2/bec_server/launch.py
+-rw-r--r--   0 root         (0) root         (0)     3075 2023-07-08 15:47:18.000000 bec-server-0.13.2/bec_server/service_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2023-07-08 15:47:18.000000 bec-server-0.13.2/bec_server/tmux_launch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:52:35.470386 bec-server-0.13.2/bec_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-07-21 07:52:35.000000 bec-server-0.13.2/bec_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      332 2023-07-21 07:52:35.000000 bec-server-0.13.2/bec_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 07:52:35.000000 bec-server-0.13.2/bec_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-21 07:52:35.000000 bec-server-0.13.2/bec_server.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-21 07:52:35.000000 bec-server-0.13.2/bec_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-21 07:52:35.000000 bec-server-0.13.2/bec_server.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      503 2023-07-21 07:52:35.471386 bec-server-0.13.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-07-08 15:47:18.000000 bec-server-0.13.2/setup.py
```

### Comparing `bec-server-0.13.1/bec_server/launch.py` & `bec-server-0.13.2/bec_server/launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.13.1/bec_server/service_handler.py` & `bec-server-0.13.2/bec_server/service_handler.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.13.1/bec_server/tmux_launch.py` & `bec-server-0.13.2/bec_server/tmux_launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.13.1/setup.py` & `bec-server-0.13.2/setup.py`

 * *Files identical despite different names*

