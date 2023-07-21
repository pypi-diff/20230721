# Comparing `tmp/work-time-log-0.99.2.post1.tar.gz` & `tmp/work-time-log-0.999.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "work-time-log-0.99.2.post1.tar", max compression
+gzip compressed data, was "work-time-log-0.999.0.tar", last modified: Fri Jul 21 15:21:04 2023, max compression
```

## Comparing `work-time-log-0.99.2.post1.tar` & `work-time-log-0.999.0.tar`

### file list

```diff
@@ -1,16 +1,11 @@
--rw-r--r--   0        0        0    27709 2022-06-28 21:31:18.561327 work-time-log-0.99.2.post1/README.md
--rw-r--r--   0        0        0      566 2022-06-28 21:31:31.921425 work-time-log-0.99.2.post1/pyproject.toml
--rw-r--r--   0        0        0    82826 2022-06-28 21:32:28.853845 work-time-log-0.99.2.post1/src/work.py
--rw-r--r--   0        0        0        0 2021-02-24 12:12:04.352563 work-time-log-0.99.2.post1/src/work_components/__init__.py
--rw-r--r--   0        0        0    21361 2022-06-28 21:31:51.205567 work-time-log-0.99.2.post1/src/work_components/arguments.py
--rw-r--r--   0        0        0     1358 2022-01-28 18:57:15.816857 work-time-log-0.99.2.post1/src/work_components/consts.py
--rw-r--r--   0        0        0    21704 2022-06-23 15:21:28.147760 work-time-log-0.99.2.post1/src/work_components/container.py
--rw-r--r--   0        0        0     5318 2022-06-23 15:21:27.719756 work-time-log-0.99.2.post1/src/work_components/dt_parse.py
--rw-r--r--   0        0        0      712 2022-06-28 21:31:51.205567 work-time-log-0.99.2.post1/src/work_components/migrate.py
--rw-r--r--   0        0        0     4966 2022-06-28 21:31:51.205567 work-time-log-0.99.2.post1/src/work_components/rc_dao.py
--rw-r--r--   0        0        0    10246 2022-06-23 15:21:27.863757 work-time-log-0.99.2.post1/src/work_components/recess_dao.py
--rw-r--r--   0        0        0      471 2022-02-22 16:54:15.468000 work-time-log-0.99.2.post1/src/work_components/timestamps.py
--rw-r--r--   0        0        0     5957 2022-06-23 15:21:20.307678 work-time-log-0.99.2.post1/src/work_components/util.py
--rw-r--r--   0        0        0    13506 2022-06-28 18:34:47.687808 work-time-log-0.99.2.post1/src/work_components/work_dao.py
--rw-r--r--   0        0        0    29228 2022-06-28 21:33:29.259792 work-time-log-0.99.2.post1/setup.py
--rw-r--r--   0        0        0    28162 2022-06-28 21:33:29.262369 work-time-log-0.99.2.post1/PKG-INFO
+drwxrwxr-x   0 zieglmeier  (1001) zieglmeier  (1001)        0 2023-07-21 15:21:04.605164 work-time-log-0.999.0/
+-rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)      320 2023-07-21 15:21:04.605164 work-time-log-0.999.0/PKG-INFO
+-rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)      138 2023-07-17 11:44:04.000000 work-time-log-0.999.0/README.md
+-rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)       38 2023-07-21 15:21:04.605164 work-time-log-0.999.0/setup.cfg
+-rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)      467 2023-07-21 15:20:40.000000 work-time-log-0.999.0/setup.py
+drwxrwxr-x   0 zieglmeier  (1001) zieglmeier  (1001)        0 2023-07-21 15:21:04.605164 work-time-log-0.999.0/work_time_log.egg-info/
+-rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)      320 2023-07-21 15:21:04.000000 work-time-log-0.999.0/work_time_log.egg-info/PKG-INFO
+-rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)      202 2023-07-21 15:21:04.000000 work-time-log-0.999.0/work_time_log.egg-info/SOURCES.txt
+-rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)        1 2023-07-21 15:21:04.000000 work-time-log-0.999.0/work_time_log.egg-info/dependency_links.txt
+-rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)        5 2023-07-21 15:21:04.000000 work-time-log-0.999.0/work_time_log.egg-info/requires.txt
+-rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)        1 2023-07-21 15:21:04.000000 work-time-log-0.999.0/work_time_log.egg-info/top_level.txt
```

