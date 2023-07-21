# Comparing `tmp/naas-2.9.1.tar.gz` & `tmp/naas-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naas-2.9.1.tar", last modified: Tue Jan 10 11:33:00 2023, max compression
+gzip compressed data, was "naas-2.9.3.tar", last modified: Wed Jan 25 06:25:36 2023, max compression
```

## Comparing `naas-2.9.1.tar` & `naas-2.9.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 11:33:00.131063 naas-2.9.1/
--rw-r--r--   0 root         (0) root         (0)    34523 2023-01-10 11:27:47.000000 naas-2.9.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7208 2023-01-10 11:33:00.131063 naas-2.9.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6460 2023-01-10 11:27:47.000000 naas-2.9.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 11:33:00.123063 naas-2.9.1/naas/
--rw-r--r--   0 root         (0) root         (0)     6886 2023-01-10 11:27:47.000000 naas-2.9.1/naas/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7981 2023-01-10 11:27:47.000000 naas-2.9.1/naas/api.py
--rw-r--r--   0 root         (0) root         (0)     4330 2023-01-10 11:27:47.000000 naas-2.9.1/naas/assets.py
--rw-r--r--   0 root         (0) root         (0)     3892 2023-01-10 11:27:47.000000 naas-2.9.1/naas/callback.py
--rw-r--r--   0 root         (0) root         (0)     2509 2023-01-10 11:27:47.000000 naas-2.9.1/naas/dependency.py
--rw-r--r--   0 root         (0) root         (0)    15488 2023-01-10 11:27:47.000000 naas-2.9.1/naas/manager.py
--rw-r--r--   0 root         (0) root         (0)     2881 2023-01-10 11:27:47.000000 naas-2.9.1/naas/ntypes.py
--rw-r--r--   0 root         (0) root         (0)     4156 2023-01-10 11:27:47.000000 naas-2.9.1/naas/onboarding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 11:33:00.127063 naas-2.9.1/naas/pipeline/
--rw-r--r--   0 root         (0) root         (0)       43 2023-01-10 11:27:47.000000 naas-2.9.1/naas/pipeline/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17716 2023-01-10 11:27:47.000000 naas-2.9.1/naas/pipeline/pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 11:33:00.127063 naas-2.9.1/naas/runner/
--rw-r--r--   0 root         (0) root         (0)       93 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1206 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 11:33:00.131063 naas-2.9.1/naas/runner/assets/
--rw-r--r--   0 root         (0) root         (0)    61277 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/assets/manager.html
--rw-r--r--   0 root         (0) root         (0)    81566 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/assets/naas_down.png
--rw-r--r--   0 root         (0) root         (0)    20650 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/assets/naas_fav.svg
--rw-r--r--   0 root         (0) root         (0)    21891 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/assets/naas_logo.png
--rw-r--r--   0 root         (0) root         (0)    20596 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/assets/naas_logo.svg
--rw-r--r--   0 root         (0) root         (0)    38576 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/assets/naas_up.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 11:33:00.131063 naas-2.9.1/naas/runner/controllers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4234 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/controllers/assets.py
--rw-r--r--   0 root         (0) root         (0)      734 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/controllers/auth.py
--rw-r--r--   0 root         (0) root         (0)     1553 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/controllers/credits.py
--rw-r--r--   0 root         (0) root         (0)     2006 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/controllers/downloader.py
--rw-r--r--   0 root         (0) root         (0)     1178 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/controllers/env.py
--rw-r--r--   0 root         (0) root         (0)     6853 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/controllers/jobs.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/controllers/logs.py
--rw-r--r--   0 root         (0) root         (0)      632 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/controllers/manager.py
--rw-r--r--   0 root         (0) root         (0)     5285 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/controllers/notebooks.py
--rw-r--r--   0 root         (0) root         (0)     2673 2023-01-10 11:31:26.000000 naas-2.9.1/naas/runner/controllers/performance.py
--rw-r--r--   0 root         (0) root         (0)      981 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/controllers/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1880 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/controllers/secret.py
--rw-r--r--   0 root         (0) root         (0)     1485 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/controllers/timezone.py
--rw-r--r--   0 root         (0) root         (0)      963 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/controllers/version.py
--rw-r--r--   0 root         (0) root         (0)     5851 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/custom_papermill.py
--rw-r--r--   0 root         (0) root         (0)     7034 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/env_var.py
--rw-r--r--   0 root         (0) root         (0)    19379 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/jobs.py
--rw-r--r--   0 root         (0) root         (0)     3191 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/logger.py
--rw-r--r--   0 root         (0) root         (0)    14629 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/notebooks.py
--rw-r--r--   0 root         (0) root         (0)     6761 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/notifications.py
--rw-r--r--   0 root         (0) root         (0)     2546 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/proxy.py
--rw-r--r--   0 root         (0) root         (0)     7377 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/runner.py
--rw-r--r--   0 root         (0) root         (0)    14153 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     9119 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/secret.py
--rw-r--r--   0 root         (0) root         (0)     3765 2023-01-10 11:27:47.000000 naas-2.9.1/naas/runner/sqlite_table.py
--rw-r--r--   0 root         (0) root         (0)     4482 2023-01-10 11:27:47.000000 naas-2.9.1/naas/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     2135 2023-01-10 11:27:47.000000 naas-2.9.1/naas/secret.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 11:33:00.127063 naas-2.9.1/naas.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7208 2023-01-10 11:33:00.000000 naas-2.9.1/naas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1424 2023-01-10 11:33:00.000000 naas-2.9.1/naas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-10 11:33:00.000000 naas-2.9.1/naas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1191 2023-01-10 11:33:00.000000 naas-2.9.1/naas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-01-10 11:33:00.000000 naas-2.9.1/naas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-01-10 11:33:00.131063 naas-2.9.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2766 2023-01-10 11:27:47.000000 naas-2.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 06:25:36.567889 naas-2.9.3/
+-rw-r--r--   0 root         (0) root         (0)    34523 2023-01-25 06:19:01.000000 naas-2.9.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7208 2023-01-25 06:25:36.571889 naas-2.9.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6460 2023-01-25 06:19:01.000000 naas-2.9.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 06:25:36.559889 naas-2.9.3/naas/
+-rw-r--r--   0 root         (0) root         (0)     6886 2023-01-25 06:19:01.000000 naas-2.9.3/naas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7981 2023-01-25 06:19:01.000000 naas-2.9.3/naas/api.py
+-rw-r--r--   0 root         (0) root         (0)     4330 2023-01-25 06:19:01.000000 naas-2.9.3/naas/assets.py
+-rw-r--r--   0 root         (0) root         (0)     3892 2023-01-25 06:19:01.000000 naas-2.9.3/naas/callback.py
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-01-25 06:19:01.000000 naas-2.9.3/naas/dependency.py
+-rw-r--r--   0 root         (0) root         (0)    15488 2023-01-25 06:19:01.000000 naas-2.9.3/naas/manager.py
+-rw-r--r--   0 root         (0) root         (0)     2881 2023-01-25 06:19:01.000000 naas-2.9.3/naas/ntypes.py
+-rw-r--r--   0 root         (0) root         (0)     4156 2023-01-25 06:19:01.000000 naas-2.9.3/naas/onboarding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 06:25:36.563889 naas-2.9.3/naas/pipeline/
+-rw-r--r--   0 root         (0) root         (0)       43 2023-01-25 06:19:01.000000 naas-2.9.3/naas/pipeline/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17716 2023-01-25 06:19:01.000000 naas-2.9.3/naas/pipeline/pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 06:25:36.563889 naas-2.9.3/naas/runner/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1206 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 06:25:36.567889 naas-2.9.3/naas/runner/assets/
+-rw-r--r--   0 root         (0) root         (0)    61277 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/assets/manager.html
+-rw-r--r--   0 root         (0) root         (0)    81566 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/assets/naas_down.png
+-rw-r--r--   0 root         (0) root         (0)    20650 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/assets/naas_fav.svg
+-rw-r--r--   0 root         (0) root         (0)    21891 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/assets/naas_logo.png
+-rw-r--r--   0 root         (0) root         (0)    20596 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/assets/naas_logo.svg
+-rw-r--r--   0 root         (0) root         (0)    38576 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/assets/naas_up.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 06:25:36.567889 naas-2.9.3/naas/runner/controllers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4234 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/controllers/assets.py
+-rw-r--r--   0 root         (0) root         (0)      734 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/controllers/auth.py
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/controllers/credits.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/controllers/downloader.py
+-rw-r--r--   0 root         (0) root         (0)     1178 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/controllers/env.py
+-rw-r--r--   0 root         (0) root         (0)     6853 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/controllers/jobs.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/controllers/logs.py
+-rw-r--r--   0 root         (0) root         (0)      632 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/controllers/manager.py
+-rw-r--r--   0 root         (0) root         (0)     5285 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/controllers/notebooks.py
+-rw-r--r--   0 root         (0) root         (0)     2673 2023-01-25 06:23:51.000000 naas-2.9.3/naas/runner/controllers/performance.py
+-rw-r--r--   0 root         (0) root         (0)      981 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/controllers/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1880 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/controllers/secret.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/controllers/timezone.py
+-rw-r--r--   0 root         (0) root         (0)      963 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/controllers/version.py
+-rw-r--r--   0 root         (0) root         (0)     5851 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/custom_papermill.py
+-rw-r--r--   0 root         (0) root         (0)     7034 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/env_var.py
+-rw-r--r--   0 root         (0) root         (0)    19379 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/jobs.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/logger.py
+-rw-r--r--   0 root         (0) root         (0)    14629 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/notebooks.py
+-rw-r--r--   0 root         (0) root         (0)     6761 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/notifications.py
+-rw-r--r--   0 root         (0) root         (0)     2546 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/proxy.py
+-rw-r--r--   0 root         (0) root         (0)     7377 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/runner.py
+-rw-r--r--   0 root         (0) root         (0)    14153 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     9119 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/secret.py
+-rw-r--r--   0 root         (0) root         (0)     3765 2023-01-25 06:19:01.000000 naas-2.9.3/naas/runner/sqlite_table.py
+-rw-r--r--   0 root         (0) root         (0)     4482 2023-01-25 06:19:01.000000 naas-2.9.3/naas/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     2135 2023-01-25 06:19:01.000000 naas-2.9.3/naas/secret.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 06:25:36.559889 naas-2.9.3/naas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7208 2023-01-25 06:25:36.000000 naas-2.9.3/naas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1424 2023-01-25 06:25:36.000000 naas-2.9.3/naas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-25 06:25:36.000000 naas-2.9.3/naas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1191 2023-01-25 06:25:36.000000 naas-2.9.3/naas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-01-25 06:25:36.000000 naas-2.9.3/naas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-01-25 06:25:36.571889 naas-2.9.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2766 2023-01-25 06:19:01.000000 naas-2.9.3/setup.py
```

### Comparing `naas-2.9.1/LICENSE` & `naas-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/PKG-INFO` & `naas-2.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naas
-Version: 2.9.1
+Version: 2.9.3
 Summary: Scheduler system for notebooks
 Home-page: https://github.com/cashstory/naas
 Author: Maxime Jublou
 Author-email: devops@cashstory.com
 License: BSD
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `naas-2.9.1/README.md` & `naas-2.9.3/README.md`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/__init__.py` & `naas-2.9.3/naas/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from .api import Api
 
 from .pipeline import *  # noqa: F403,F401
 import requests
 import os
 import sys
 
-__version__ = "2.9.1"
+__version__ = "2.9.3"
 __github_repo = "jupyter-naas/naas"
 __doc_url = "https://naas.gitbook.io/naas/"
 __canny_js = '<script>!function(w,d,i,s){function l(){if(!d.getElementById(i)){var f=d.getElementsByTagName(s)[0],e=d.createElement(s);e.type="text/javascript",e.async=!0,e.src="https://canny.io/sdk.js",f.parentNode.insertBefore(e,f)}}if("function"!=typeof w.Canny){var c=function(){c.q.push(arguments)};c.q=[],w.Canny=c,"complete"===d.readyState?l():w.attachEvent?w.attachEvent("onload",l):w.addEventListener("load",l,!1)}}(window,document,"canny-jssdk","script");</script>'  # noqa: E501
 __crisp = '<script type="text/javascript">if(!window.$crisp){window.$crisp=[["set", "session:data", [[["naas_type", "pip"]]]], ["do", "chat:hide"], ["on", "message:received", () => {window.$crisp.push(["do", "chat:show"])}], ["on", "chat:closed", () => {window.$crisp.push(["do", "chat:hide"])}]];window.CRISP_WEBSITE_ID="a64b999e-e44c-44ee-928f-5cd0233f9586";(function(){d=document;s=d.createElement("script");s.src="https://client.crisp.chat/l.js";s.async=1;d.getElementsByTagName("head")[0].appendChild(s);})();}</script>'  # noqa: E501
 __location__ = os.getcwd()
 
 if len(sys.argv) == 0 or (len(sys.argv) > 0 and sys.argv[0] != "-m"):
```

### Comparing `naas-2.9.1/naas/api.py` & `naas-2.9.3/naas/api.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/assets.py` & `naas-2.9.3/naas/assets.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/callback.py` & `naas-2.9.3/naas/callback.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/dependency.py` & `naas-2.9.3/naas/dependency.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/manager.py` & `naas-2.9.3/naas/manager.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/ntypes.py` & `naas-2.9.3/naas/ntypes.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/onboarding.py` & `naas-2.9.3/naas/onboarding.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/pipeline/pipeline.py` & `naas-2.9.3/naas/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/__main__.py` & `naas-2.9.3/naas/runner/__main__.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/assets/manager.html` & `naas-2.9.3/naas/runner/assets/manager.html`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/assets/naas_down.png` & `naas-2.9.3/naas/runner/assets/naas_down.png`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/assets/naas_fav.svg` & `naas-2.9.3/naas/runner/assets/naas_fav.svg`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/assets/naas_logo.png` & `naas-2.9.3/naas/runner/assets/naas_logo.png`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/assets/naas_logo.svg` & `naas-2.9.3/naas/runner/assets/naas_logo.svg`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/assets/naas_up.png` & `naas-2.9.3/naas/runner/assets/naas_up.png`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/controllers/assets.py` & `naas-2.9.3/naas/runner/controllers/assets.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/controllers/auth.py` & `naas-2.9.3/naas/runner/controllers/auth.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/controllers/credits.py` & `naas-2.9.3/naas/runner/controllers/credits.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/controllers/downloader.py` & `naas-2.9.3/naas/runner/controllers/downloader.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/controllers/env.py` & `naas-2.9.3/naas/runner/controllers/env.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/controllers/jobs.py` & `naas-2.9.3/naas/runner/controllers/jobs.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/controllers/logs.py` & `naas-2.9.3/naas/runner/controllers/logs.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/controllers/manager.py` & `naas-2.9.3/naas/runner/controllers/manager.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/controllers/notebooks.py` & `naas-2.9.3/naas/runner/controllers/notebooks.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/controllers/performance.py` & `naas-2.9.3/naas/runner/controllers/performance.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/controllers/scheduler.py` & `naas-2.9.3/naas/runner/controllers/scheduler.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/controllers/secret.py` & `naas-2.9.3/naas/runner/controllers/secret.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/controllers/timezone.py` & `naas-2.9.3/naas/runner/controllers/timezone.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/controllers/version.py` & `naas-2.9.3/naas/runner/controllers/version.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/custom_papermill.py` & `naas-2.9.3/naas/runner/custom_papermill.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/env_var.py` & `naas-2.9.3/naas/runner/env_var.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/jobs.py` & `naas-2.9.3/naas/runner/jobs.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/logger.py` & `naas-2.9.3/naas/runner/logger.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/notebooks.py` & `naas-2.9.3/naas/runner/notebooks.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/notifications.py` & `naas-2.9.3/naas/runner/notifications.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/proxy.py` & `naas-2.9.3/naas/runner/proxy.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/runner.py` & `naas-2.9.3/naas/runner/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     t_version,
 )
 
 # TODO remove this fix when papermill and nest_asyncio support uvloop
 asyncio.set_event_loop_policy(None)
 nest_asyncio.apply()
 
-__version__ = "2.9.1"
+__version__ = "2.9.3"
 
 
 class Runner:
     # Declare path variable
     __path_lib_files = os.path.dirname(os.path.abspath(__file__))
     __app = None
     __nb = None
```

### Comparing `naas-2.9.1/naas/runner/scheduler.py` & `naas-2.9.3/naas/runner/scheduler.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/secret.py` & `naas-2.9.3/naas/runner/secret.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/runner/sqlite_table.py` & `naas-2.9.3/naas/runner/sqlite_table.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/scheduler.py` & `naas-2.9.3/naas/scheduler.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas/secret.py` & `naas-2.9.3/naas/secret.py`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas.egg-info/PKG-INFO` & `naas-2.9.3/naas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naas
-Version: 2.9.1
+Version: 2.9.3
 Summary: Scheduler system for notebooks
 Home-page: https://github.com/cashstory/naas
 Author: Maxime Jublou
 Author-email: devops@cashstory.com
 License: BSD
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `naas-2.9.1/naas.egg-info/SOURCES.txt` & `naas-2.9.3/naas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naas-2.9.1/naas.egg-info/requires.txt` & `naas-2.9.3/naas.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 flake8==4.0.1
 black>=21.4b2
 imgcompare==2.0.1
 commitizen==2.17.13
 pytest-cov==2.12.1
 
 [full]
-naas_drivers[full]==0.108.0
+naas_drivers[full]==0.108.1
 
 [fulldev]
 syncer==1.3.0
 backports.zoneinfo==0.2.1
 pytest==6.2.4
 pytest-tornasync==0.6.0.post2
 pytest-mock==3.6.0
@@ -64,8 +64,8 @@
 twine==3.5.0
 requests-mock==1.9.3
 flake8==4.0.1
 black>=21.4b2
 imgcompare==2.0.1
 commitizen==2.17.13
 pytest-cov==2.12.1
-naas_drivers[full]==0.108.0
+naas_drivers[full]==0.108.1
```

### Comparing `naas-2.9.1/setup.py` & `naas-2.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-NDV = "0.108.0"
+NDV = "0.108.1"
 
 driver_dep = [f'naas_drivers[full]=={NDV}']
 dev_dep = [
     "syncer==1.3.0",
     "backports.zoneinfo==0.2.1",
     "pytest==6.2.4",
     "pytest-tornasync==0.6.0.post2",
@@ -21,15 +21,15 @@
     "black>=21.4b2",
     "imgcompare==2.0.1",
     "commitizen==2.17.13",
     "pytest-cov==2.12.1",
 ]
 setup(
     name="naas",
-    version="2.9.1",
+    version="2.9.3",
     author="Maxime Jublou",
     author_email="devops@cashstory.com",
     license="BSD",
     description="Scheduler system for notebooks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cashstory/naas",
```

