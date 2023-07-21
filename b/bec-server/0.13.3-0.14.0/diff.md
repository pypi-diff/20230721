# Comparing `tmp/bec-server-0.13.3.tar.gz` & `tmp/bec-server-0.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec-server-0.13.3.tar", last modified: Fri Jul 21 15:13:13 2023, max compression
+gzip compressed data, was "bec-server-0.14.0.tar", last modified: Fri Jul 21 20:43:47 2023, max compression
```

## Comparing `bec-server-0.13.3.tar` & `bec-server-0.14.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:13:13.149703 bec-server-0.13.3/
--rw-r--r--   0 root         (0) root         (0)      443 2023-07-21 15:13:13.149703 bec-server-0.13.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:13:13.144703 bec-server-0.13.3/bec_server/
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-08 15:33:35.000000 bec-server-0.13.3/bec_server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1391 2023-07-21 15:12:28.000000 bec-server-0.13.3/bec_server/launch.py
--rw-r--r--   0 root         (0) root         (0)     3075 2023-07-08 15:33:35.000000 bec-server-0.13.3/bec_server/service_handler.py
--rw-r--r--   0 root         (0) root         (0)     2716 2023-07-21 15:12:28.000000 bec-server-0.13.3/bec_server/tmux_launch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:13:13.149703 bec-server-0.13.3/bec_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      443 2023-07-21 15:13:13.000000 bec-server-0.13.3/bec_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      332 2023-07-21 15:13:13.000000 bec-server-0.13.3/bec_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:13:13.000000 bec-server-0.13.3/bec_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-07-21 15:13:13.000000 bec-server-0.13.3/bec_server.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-07-21 15:13:13.000000 bec-server-0.13.3/bec_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-21 15:13:13.000000 bec-server-0.13.3/bec_server.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      503 2023-07-21 15:13:13.150703 bec-server-0.13.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1400 2023-07-21 15:12:28.000000 bec-server-0.13.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:43:47.593832 bec-server-0.14.0/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-07-21 20:43:47.593832 bec-server-0.14.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:43:47.591832 bec-server-0.14.0/bec_server/
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-08 15:33:35.000000 bec-server-0.14.0/bec_server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1391 2023-07-21 18:30:48.000000 bec-server-0.14.0/bec_server/launch.py
+-rw-r--r--   0 root         (0) root         (0)     3075 2023-07-08 15:33:35.000000 bec-server-0.14.0/bec_server/service_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2023-07-21 18:30:48.000000 bec-server-0.14.0/bec_server/tmux_launch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 20:43:47.592832 bec-server-0.14.0/bec_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-07-21 20:43:47.000000 bec-server-0.14.0/bec_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      332 2023-07-21 20:43:47.000000 bec-server-0.14.0/bec_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 20:43:47.000000 bec-server-0.14.0/bec_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-21 20:43:47.000000 bec-server-0.14.0/bec_server.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-07-21 20:43:47.000000 bec-server-0.14.0/bec_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-21 20:43:47.000000 bec-server-0.14.0/bec_server.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      503 2023-07-21 20:43:47.593832 bec-server-0.14.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1400 2023-07-21 18:30:48.000000 bec-server-0.14.0/setup.py
```

### Comparing `bec-server-0.13.3/bec_server/launch.py` & `bec-server-0.14.0/bec_server/launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.13.3/bec_server/service_handler.py` & `bec-server-0.14.0/bec_server/service_handler.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.13.3/bec_server/tmux_launch.py` & `bec-server-0.14.0/bec_server/tmux_launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.13.3/setup.py` & `bec-server-0.14.0/setup.py`

 * *Files identical despite different names*

