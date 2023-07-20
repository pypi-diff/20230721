# Comparing `tmp/robit-0.3.2.1.tar.gz` & `tmp/robit-0.3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robit-0.3.2.1.tar", last modified: Thu Jul 20 21:16:46 2023, max compression
+gzip compressed data, was "robit-0.3.2.2.tar", last modified: Thu Jul 20 22:11:19 2023, max compression
```

## Comparing `robit-0.3.2.1.tar` & `robit-0.3.2.2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:46.381924 robit-0.3.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-20 21:16:31.000000 robit-0.3.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 21:16:31.000000 robit-0.3.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-20 21:16:46.381924 robit-0.3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-20 21:16:31.000000 robit-0.3.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-20 21:16:31.000000 robit-0.3.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:46.373924 robit-0.3.2.1/robit/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:46.373924 robit-0.3.2.1/robit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/core/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/core/clock.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/core/counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/core/health.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/core/id.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/core/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/core/name.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/core/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:46.377924 robit-0.3.2.1/robit/cron/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/cron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/cron/cron.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/cron/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/cron/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/cron/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:46.377924 robit-0.3.2.1/robit/html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39713 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/html/alpine.js
--rw-r--r--   0 runner    (1001) docker     (123)   194855 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/html/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)    80448 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/html/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/html/core.js
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/html/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/html/index.css
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/html/monitor.html
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/html/monitor.js
--rw-r--r--   0 runner    (1001) docker     (123)    15621 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/html/worker.html
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/html/worker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:46.377924 robit-0.3.2.1/robit/job/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/job/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/job/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/job/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:46.377924 robit-0.3.2.1/robit/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/monitor/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/monitor/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:46.377924 robit-0.3.2.1/robit/socket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/socket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/socket/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:46.377924 robit-0.3.2.1/robit/status/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/status/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/status/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:46.377924 robit-0.3.2.1/robit/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:46.377924 robit-0.3.2.1/robit/test/cron/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/test/cron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/test/cron/test_cron.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/test/cron/test_cron_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/test/cron/test_cron_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/test/test_clock.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/test/test_robit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:46.377924 robit-0.3.2.1/robit/timer/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/timer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/timer/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/timer/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:46.381924 robit-0.3.2.1/robit/web_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/web_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/web_server/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/web_server/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:46.381924 robit-0.3.2.1/robit/worker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/worker/web_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-07-20 21:16:31.000000 robit-0.3.2.1/robit/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:16:46.373924 robit-0.3.2.1/robit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-20 21:16:46.000000 robit-0.3.2.1/robit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-20 21:16:46.000000 robit-0.3.2.1/robit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:16:46.000000 robit-0.3.2.1/robit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 21:16:46.000000 robit-0.3.2.1/robit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-20 21:16:46.381924 robit-0.3.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 21:16:31.000000 robit-0.3.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:19.924265 robit-0.3.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-20 22:11:08.000000 robit-0.3.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 22:11:08.000000 robit-0.3.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-20 22:11:19.924265 robit-0.3.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-20 22:11:08.000000 robit-0.3.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-20 22:11:08.000000 robit-0.3.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:19.916264 robit-0.3.2.2/robit/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:19.920264 robit-0.3.2.2/robit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/core/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/core/clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/core/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/core/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/core/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/core/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/core/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/core/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:19.920264 robit-0.3.2.2/robit/cron/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/cron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/cron/cron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/cron/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/cron/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/cron/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:19.920264 robit-0.3.2.2/robit/html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39713 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/html/alpine.js
+-rw-r--r--   0 runner    (1001) docker     (123)   194855 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/html/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)    80448 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/html/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/html/core.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/html/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/html/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/html/monitor.html
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/html/monitor.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15621 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/html/worker.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/html/worker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:19.920264 robit-0.3.2.2/robit/job/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/job/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/job/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/job/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:19.920264 robit-0.3.2.2/robit/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/monitor/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/monitor/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:19.920264 robit-0.3.2.2/robit/socket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/socket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/socket/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:19.924265 robit-0.3.2.2/robit/status/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/status/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/status/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:19.924265 robit-0.3.2.2/robit/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:19.924265 robit-0.3.2.2/robit/test/cron/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/test/cron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/test/cron/test_cron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/test/cron/test_cron_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/test/cron/test_cron_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/test/test_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/test/test_robit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:19.924265 robit-0.3.2.2/robit/timer/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/timer/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/timer/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:19.924265 robit-0.3.2.2/robit/web_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/web_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/web_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/web_server/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:19.924265 robit-0.3.2.2/robit/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/worker/web_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-07-20 22:11:08.000000 robit-0.3.2.2/robit/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:11:19.920264 robit-0.3.2.2/robit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-20 22:11:19.000000 robit-0.3.2.2/robit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-20 22:11:19.000000 robit-0.3.2.2/robit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 22:11:19.000000 robit-0.3.2.2/robit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 22:11:19.000000 robit-0.3.2.2/robit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-20 22:11:19.924265 robit-0.3.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 22:11:08.000000 robit-0.3.2.2/setup.py
```

### Comparing `robit-0.3.2.1/LICENSE.txt` & `robit-0.3.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/PKG-INFO` & `robit-0.3.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robit
-Version: 0.3.2.1
+Version: 0.3.2.2
 Summary: Service Worker Framework
 Home-page: https://github.com/stratusadv/robit
 Author: Nathan Johnson
 Author-email: nathanj@stratusadv.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `robit-0.3.2.1/README.md` & `robit-0.3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/core/alert.py` & `robit-0.3.2.2/robit/core/alert.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/core/clock.py` & `robit-0.3.2.2/robit/core/clock.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/core/health.py` & `robit-0.3.2.2/robit/core/health.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/core/log.py` & `robit-0.3.2.2/robit/core/log.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/cron/cron.py` & `robit-0.3.2.2/robit/cron/cron.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/cron/fields.py` & `robit-0.3.2.2/robit/cron/fields.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/cron/utils.py` & `robit-0.3.2.2/robit/cron/utils.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/html/alpine.js` & `robit-0.3.2.2/robit/html/alpine.js`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/html/bootstrap.css` & `robit-0.3.2.2/robit/html/bootstrap.css`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/html/bootstrap.js` & `robit-0.3.2.2/robit/html/bootstrap.js`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/html/icon.png` & `robit-0.3.2.2/robit/html/icon.png`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/html/index.css` & `robit-0.3.2.2/robit/html/index.css`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/html/monitor.html` & `robit-0.3.2.2/robit/html/monitor.html`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/html/monitor.js` & `robit-0.3.2.2/robit/html/monitor.js`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/html/worker.html` & `robit-0.3.2.2/robit/html/worker.html`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/html/worker.js` & `robit-0.3.2.2/robit/html/worker.js`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/job/group.py` & `robit-0.3.2.2/robit/job/group.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/job/job.py` & `robit-0.3.2.2/robit/job/job.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/monitor/monitor.py` & `robit-0.3.2.2/robit/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/monitor/web_server.py` & `robit-0.3.2.2/robit/monitor/web_server.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/socket/socket.py` & `robit-0.3.2.2/robit/socket/socket.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 class ServerSocket(Socket):
     @abstractmethod
     def process_requests(self):
         pass
 
     def start(self):
+        logging.warning(f'Starting server on {self.host}:{self.port}')
         self.socket.bind((self.host, self.port))
         self.socket.listen(1)
         logging.warning(f'Server started on {self.host}:{self.port}')
 
 
 class WebServerSocket(ServerSocket):
     def __init__(self, web_server, host: str = DEFAULT_HOST, port: int = DEFAULT_PORT):
```

### Comparing `robit-0.3.2.1/robit/status/status.py` & `robit-0.3.2.2/robit/status/status.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/test/cron/test_cron_fields.py` & `robit-0.3.2.2/robit/test/cron/test_cron_fields.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/test/cron/test_cron_utils.py` & `robit-0.3.2.2/robit/test/cron/test_cron_utils.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/test/test_clock.py` & `robit-0.3.2.2/robit/test/test_clock.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/timer/timer.py` & `robit-0.3.2.2/robit/timer/timer.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/web_server/utils.py` & `robit-0.3.2.2/robit/web_server/utils.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/web_server/web_server.py` & `robit-0.3.2.2/robit/web_server/web_server.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/worker/web_server.py` & `robit-0.3.2.2/robit/worker/web_server.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/robit/worker/worker.py` & `robit-0.3.2.2/robit/worker/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,19 +122,23 @@
         ready_jobs = [job for group in self.groups.values() for job in group.job_list if tz_now() > job.next_run_datetime]
         for job in ready_jobs:
             self.queue.put(job)
             job.set_next_run_datetime()
             job.status.waiting()
 
     def update_web_server(self):
-        client_socket = ClientSocket()
-        client_socket.start()
-        logging.warning(f'Connecting to {client_socket.host}:{client_socket.port}')
-        client_socket.send(self.as_dict())
-        client_socket.close()
+        try:
+            client_socket = ClientSocket()
+            logging.warning(f'Connecting to socket {client_socket.host}:{client_socket.port}')
+            client_socket.start()
+            client_socket.send(self.as_dict())
+            client_socket.close()
+            logging.warning(f'Connected to socket {client_socket.host}:{client_socket.port}')
+        except Exception as e:
+            logging.warning(f'Unable to connect to socket -{e}')
 
         # Todo: Need to update the monitor
         # if self.monitor_address:
         #     post_worker_data_to_monitor(self.monitor_address, self.monitor_key, self.as_dict_to_monitor())
 
     def start(self) -> None:
         if self.web_server:
```

### Comparing `robit-0.3.2.1/robit.egg-info/PKG-INFO` & `robit-0.3.2.2/robit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robit
-Version: 0.3.2.1
+Version: 0.3.2.2
 Summary: Service Worker Framework
 Home-page: https://github.com/stratusadv/robit
 Author: Nathan Johnson
 Author-email: nathanj@stratusadv.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `robit-0.3.2.1/robit.egg-info/SOURCES.txt` & `robit-0.3.2.2/robit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robit-0.3.2.1/setup.cfg` & `robit-0.3.2.2/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = robit
-version = 0.3.2.1
+version = 0.3.2.2
 author = Nathan Johnson
 author_email = nathanj@stratusadv.com
 description = Service Worker Framework
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/stratusadv/robit
 classifiers =
```

