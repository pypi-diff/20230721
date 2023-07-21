# Comparing `tmp/middleware-apm-0.2.0rc3.tar.gz` & `tmp/middleware-apm-0.2.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "middleware-apm-0.2.0rc3.tar", last modified: Fri Jul 21 05:59:53 2023, max compression
+gzip compressed data, was "middleware-apm-0.2.0rc4.tar", last modified: Fri Jul 21 07:29:22 2023, max compression
```

## Comparing `middleware-apm-0.2.0rc3.tar` & `middleware-apm-0.2.0rc4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:59:53.287302 middleware-apm-0.2.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-21 05:59:29.000000 middleware-apm-0.2.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-21 05:59:53.287302 middleware-apm-0.2.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-21 05:59:29.000000 middleware-apm-0.2.0rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:59:53.283301 middleware-apm-0.2.0rc3/middleware_apm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-21 05:59:53.000000 middleware-apm-0.2.0rc3/middleware_apm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-21 05:59:53.000000 middleware-apm-0.2.0rc3/middleware_apm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 05:59:53.000000 middleware-apm-0.2.0rc3/middleware_apm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-21 05:59:53.000000 middleware-apm-0.2.0rc3/middleware_apm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-21 05:59:53.000000 middleware-apm-0.2.0rc3/middleware_apm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 05:59:53.000000 middleware-apm-0.2.0rc3/middleware_apm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:59:53.287302 middleware-apm-0.2.0rc3/mw_tracker/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-21 05:59:29.000000 middleware-apm-0.2.0rc3/mw_tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-21 05:59:29.000000 middleware-apm-0.2.0rc3/mw_tracker/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-07-21 05:59:29.000000 middleware-apm-0.2.0rc3/mw_tracker/_meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-21 05:59:29.000000 middleware-apm-0.2.0rc3/mw_tracker/_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-21 05:59:29.000000 middleware-apm-0.2.0rc3/mw_tracker/_tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-21 05:59:29.000000 middleware-apm-0.2.0rc3/mw_tracker/mw_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 05:59:53.287302 middleware-apm-0.2.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-21 05:59:29.000000 middleware-apm-0.2.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:29:22.917500 middleware-apm-0.2.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-21 07:28:55.000000 middleware-apm-0.2.0rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-21 07:29:22.917500 middleware-apm-0.2.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-21 07:28:55.000000 middleware-apm-0.2.0rc4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:29:22.913500 middleware-apm-0.2.0rc4/middleware_apm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-21 07:29:22.000000 middleware-apm-0.2.0rc4/middleware_apm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-21 07:29:22.000000 middleware-apm-0.2.0rc4/middleware_apm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:29:22.000000 middleware-apm-0.2.0rc4/middleware_apm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-21 07:29:22.000000 middleware-apm-0.2.0rc4/middleware_apm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-21 07:29:22.000000 middleware-apm-0.2.0rc4/middleware_apm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 07:29:22.000000 middleware-apm-0.2.0rc4/middleware_apm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:29:22.917500 middleware-apm-0.2.0rc4/mw_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-21 07:28:55.000000 middleware-apm-0.2.0rc4/mw_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-21 07:28:55.000000 middleware-apm-0.2.0rc4/mw_tracker/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-07-21 07:28:55.000000 middleware-apm-0.2.0rc4/mw_tracker/_meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-21 07:28:55.000000 middleware-apm-0.2.0rc4/mw_tracker/_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-21 07:28:55.000000 middleware-apm-0.2.0rc4/mw_tracker/_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-21 07:28:55.000000 middleware-apm-0.2.0rc4/mw_tracker/mw_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 07:29:22.917500 middleware-apm-0.2.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-21 07:28:55.000000 middleware-apm-0.2.0rc4/setup.py
```

### Comparing `middleware-apm-0.2.0rc3/LICENSE` & `middleware-apm-0.2.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `middleware-apm-0.2.0rc3/mw_tracker/_logger.py` & `middleware-apm-0.2.0rc4/mw_tracker/_logger.py`

 * *Files identical despite different names*

### Comparing `middleware-apm-0.2.0rc3/mw_tracker/_meter.py` & `middleware-apm-0.2.0rc4/mw_tracker/_meter.py`

 * *Files identical despite different names*

### Comparing `middleware-apm-0.2.0rc3/mw_tracker/_profiler.py` & `middleware-apm-0.2.0rc4/mw_tracker/_profiler.py`

 * *Files identical despite different names*

### Comparing `middleware-apm-0.2.0rc3/mw_tracker/_tracer.py` & `middleware-apm-0.2.0rc4/mw_tracker/_tracer.py`

 * *Files identical despite different names*

### Comparing `middleware-apm-0.2.0rc3/mw_tracker/mw_tracker.py` & `middleware-apm-0.2.0rc4/mw_tracker/mw_tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import logging
-from _meter import collect_metrics
-from _tracer import record_error
-from _logger import log_handler
-from _profiler import collect_profiling
+from ._meter import collect_metrics
+from ._tracer import record_error
+from ._logger import log_handler
+from ._profiler import collect_profiling
 
 mw_agent_target = os.environ.get('MW_AGENT_SERVICE', '127.0.0.1')
 
 
 class MwTracker:
     def __init__(self, access_token=None):
         pid = os.getpid()
```

### Comparing `middleware-apm-0.2.0rc3/setup.py` & `middleware-apm-0.2.0rc4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 except IOError:
     requirements = []
 
 
 setuptools.setup(
 
     name="middleware-apm",
-    version="0.2.0rc3",
+    version="0.2.0rc4",
     install_requires=requirements,
     author="middleware-dev",
     description="This package is use to check the RAM and CPU Usage of Current Device.",
     long_description=open('README.md').read(),
     long_description_content_type='text/plain',
     packages=["mw_tracker"],
     url = "https://github.com/middleware-labs/agent-apm-python.git",
```

