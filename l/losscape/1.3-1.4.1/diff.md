# Comparing `tmp/losscape-1.3.tar.gz` & `tmp/losscape-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "losscape-1.3.tar", last modified: Fri Jul 21 07:28:30 2023, max compression
+gzip compressed data, was "losscape-1.4.1.tar", last modified: Fri Jul 21 13:38:24 2023, max compression
```

## Comparing `losscape-1.3.tar` & `losscape-1.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 07:28:30.832615 losscape-1.3/
--rw-rw-r--   0 alex      (1000) alex      (1000)      230 2023-07-21 07:28:30.832615 losscape-1.3/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3020 2023-07-18 21:38:11.000000 losscape-1.3/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 07:28:30.832615 losscape-1.3/losscape/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-18 12:39:49.000000 losscape-1.3/losscape/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1380 2023-07-18 10:08:58.000000 losscape-1.3/losscape/compute_loss.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1816 2023-07-18 09:41:21.000000 losscape-1.3/losscape/create_directions.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    15961 2023-07-21 07:27:43.000000 losscape-1.3/losscape/create_landscape.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2099 2023-07-21 07:07:54.000000 losscape-1.3/losscape/train.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 07:28:30.832615 losscape-1.3/losscape.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)      230 2023-07-21 07:28:30.000000 losscape-1.3/losscape.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      300 2023-07-21 07:28:30.000000 losscape-1.3/losscape.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-21 07:28:30.000000 losscape-1.3/losscape.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       36 2023-07-21 07:28:30.000000 losscape-1.3/losscape.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-21 07:28:30.000000 losscape-1.3/losscape.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-21 07:28:30.832615 losscape-1.3/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)      399 2023-07-21 07:28:15.000000 losscape-1.3/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 13:38:24.643021 losscape-1.4.1/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3293 2023-07-21 13:38:24.643021 losscape-1.4.1/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3020 2023-07-18 21:38:11.000000 losscape-1.4.1/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 13:38:24.643021 losscape-1.4.1/losscape/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-18 12:39:49.000000 losscape-1.4.1/losscape/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1380 2023-07-18 10:08:58.000000 losscape-1.4.1/losscape/compute_loss.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1816 2023-07-18 09:41:21.000000 losscape-1.4.1/losscape/create_directions.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15961 2023-07-21 07:27:43.000000 losscape-1.4.1/losscape/create_landscape.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2099 2023-07-21 07:07:54.000000 losscape-1.4.1/losscape/train.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 13:38:24.643021 losscape-1.4.1/losscape.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3293 2023-07-21 13:38:24.000000 losscape-1.4.1/losscape.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      300 2023-07-21 13:38:24.000000 losscape-1.4.1/losscape.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-21 13:38:24.000000 losscape-1.4.1/losscape.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       36 2023-07-21 13:38:24.000000 losscape-1.4.1/losscape.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-21 13:38:24.000000 losscape-1.4.1/losscape.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-21 13:38:24.643021 losscape-1.4.1/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)      588 2023-07-21 13:37:59.000000 losscape-1.4.1/setup.py
```

### Comparing `losscape-1.3/README.md` & `losscape-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `losscape-1.3/losscape/compute_loss.py` & `losscape-1.4.1/losscape/compute_loss.py`

 * *Files identical despite different names*

### Comparing `losscape-1.3/losscape/create_directions.py` & `losscape-1.4.1/losscape/create_directions.py`

 * *Files identical despite different names*

### Comparing `losscape-1.3/losscape/create_landscape.py` & `losscape-1.4.1/losscape/create_landscape.py`

 * *Files identical despite different names*

### Comparing `losscape-1.3/losscape/train.py` & `losscape-1.4.1/losscape/train.py`

 * *Files identical despite different names*

