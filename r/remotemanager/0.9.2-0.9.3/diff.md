# Comparing `tmp/remotemanager-0.9.2.tar.gz` & `tmp/remotemanager-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotemanager-0.9.2.tar", last modified: Thu Jul 20 15:10:05 2023, max compression
+gzip compressed data, was "remotemanager-0.9.3.tar", last modified: Fri Jul 21 11:14:30 2023, max compression
```

## Comparing `remotemanager-0.9.2.tar` & `remotemanager-0.9.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:10:05.969433 remotemanager-0.9.2/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.9.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-20 15:10:05.969433 remotemanager-0.9.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.9.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1367 2023-07-20 13:55:05.000000 remotemanager-0.9.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:10:05.961433 remotemanager-0.9.2/remotemanager/
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-07-20 13:55:05.000000 remotemanager-0.9.2/remotemanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:10:05.961433 remotemanager-0.9.2/remotemanager/connection/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.9.2/remotemanager/connection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.9.2/remotemanager/connection/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:10:05.965433 remotemanager-0.9.2/remotemanager/connection/computers/
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.9.2/remotemanager/connection/computers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12849 2023-07-11 12:50:11.000000 remotemanager-0.9.2/remotemanager/connection/computers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.9.2/remotemanager/connection/computers/example.py
--rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.9.2/remotemanager/connection/computers/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.9.2/remotemanager/connection/computers/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.9.2/remotemanager/connection/detect_locale_error.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.9.2/remotemanager/connection/testing_object.py
--rw-rw-rw-   0 root         (0) root         (0)    26008 2023-07-19 14:27:58.000000 remotemanager-0.9.2/remotemanager/connection/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:10:05.965433 remotemanager-0.9.2/remotemanager/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.9.2/remotemanager/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    53874 2023-07-20 13:52:59.000000 remotemanager-0.9.2/remotemanager/dataset/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     9729 2023-07-20 13:52:59.000000 remotemanager-0.9.2/remotemanager/dataset/dependency.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-07-12 13:38:06.000000 remotemanager-0.9.2/remotemanager/dataset/lazy_append.py
--rw-rw-rw-   0 root         (0) root         (0)    21571 2023-07-20 13:52:59.000000 remotemanager-0.9.2/remotemanager/dataset/runner.py
--rw-rw-rw-   0 root         (0) root         (0)     2065 2023-07-18 13:45:10.000000 remotemanager-0.9.2/remotemanager/dataset/runnerstates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:10:05.965433 remotemanager-0.9.2/remotemanager/jupyter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.9.2/remotemanager/jupyter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5186 2023-07-18 09:05:28.000000 remotemanager-0.9.2/remotemanager/jupyter/magic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:10:05.965433 remotemanager-0.9.2/remotemanager/logging/
--rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.9.2/remotemanager/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.9.2/remotemanager/logging/log.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.9.2/remotemanager/logging/quiet.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.9.2/remotemanager/logging/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.9.2/remotemanager/logging/verbosity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:10:05.965433 remotemanager-0.9.2/remotemanager/serialisation/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.9.2/remotemanager/serialisation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.9.2/remotemanager/serialisation/serial.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.9.2/remotemanager/serialisation/serialdill.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.9.2/remotemanager/serialisation/serialjson.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.9.2/remotemanager/serialisation/serialjsonpickle.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.9.2/remotemanager/serialisation/serialyaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:10:05.969433 remotemanager-0.9.2/remotemanager/storage/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.9.2/remotemanager/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.9.2/remotemanager/storage/database.py
--rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.9.2/remotemanager/storage/function.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.9.2/remotemanager/storage/remotefunction.py
--rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.9.2/remotemanager/storage/sendablemixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3696 2023-07-18 13:45:10.000000 remotemanager-0.9.2/remotemanager/storage/trackedfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:10:05.969433 remotemanager-0.9.2/remotemanager/transport/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.9.2/remotemanager/transport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.9.2/remotemanager/transport/cp.py
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.9.2/remotemanager/transport/rsync.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.9.2/remotemanager/transport/scp.py
--rw-rw-rw-   0 root         (0) root         (0)    10027 2023-07-18 09:05:28.000000 remotemanager-0.9.2/remotemanager/transport/transport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:10:05.969433 remotemanager-0.9.2/remotemanager/utils/
--rw-rw-rw-   0 root         (0) root         (0)     5390 2023-07-18 13:45:10.000000 remotemanager-0.9.2/remotemanager/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.9.2/remotemanager/utils/flags.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.9.2/remotemanager/utils/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.9.2/remotemanager/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:10:05.961433 remotemanager-0.9.2/remotemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-20 15:10:05.000000 remotemanager-0.9.2/remotemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1863 2023-07-20 15:10:05.000000 remotemanager-0.9.2/remotemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 15:10:05.000000 remotemanager-0.9.2/remotemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      163 2023-07-20 15:10:05.000000 remotemanager-0.9.2/remotemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-20 15:10:05.000000 remotemanager-0.9.2/remotemanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 15:10:05.969433 remotemanager-0.9.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.9.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.742383 remotemanager-0.9.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.9.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-21 11:14:30.742383 remotemanager-0.9.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.9.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2023-07-21 09:25:26.000000 remotemanager-0.9.3/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.734383 remotemanager-0.9.3/remotemanager/
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-07-21 09:25:26.000000 remotemanager-0.9.3/remotemanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.738383 remotemanager-0.9.3/remotemanager/connection/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/connection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.9.3/remotemanager/connection/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.738383 remotemanager-0.9.3/remotemanager/connection/computers/
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/connection/computers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12849 2023-07-11 12:50:11.000000 remotemanager-0.9.3/remotemanager/connection/computers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.9.3/remotemanager/connection/computers/example.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.9.3/remotemanager/connection/computers/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.9.3/remotemanager/connection/computers/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.9.3/remotemanager/connection/detect_locale_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/connection/testing_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    26008 2023-07-19 14:27:58.000000 remotemanager-0.9.3/remotemanager/connection/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.738383 remotemanager-0.9.3/remotemanager/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    53942 2023-07-21 09:25:26.000000 remotemanager-0.9.3/remotemanager/dataset/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     9729 2023-07-20 13:52:59.000000 remotemanager-0.9.3/remotemanager/dataset/dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-07-12 13:38:06.000000 remotemanager-0.9.3/remotemanager/dataset/lazy_append.py
+-rw-rw-rw-   0 root         (0) root         (0)    22294 2023-07-21 09:25:26.000000 remotemanager-0.9.3/remotemanager/dataset/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2065 2023-07-18 13:45:10.000000 remotemanager-0.9.3/remotemanager/dataset/runnerstates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.738383 remotemanager-0.9.3/remotemanager/jupyter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.9.3/remotemanager/jupyter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5186 2023-07-18 09:05:28.000000 remotemanager-0.9.3/remotemanager/jupyter/magic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.742383 remotemanager-0.9.3/remotemanager/logging/
+-rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.9.3/remotemanager/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.9.3/remotemanager/logging/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.9.3/remotemanager/logging/quiet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.9.3/remotemanager/logging/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/logging/verbosity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.742383 remotemanager-0.9.3/remotemanager/serialisation/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.9.3/remotemanager/serialisation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/serialisation/serial.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.9.3/remotemanager/serialisation/serialdill.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.9.3/remotemanager/serialisation/serialjson.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/serialisation/serialjsonpickle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/serialisation/serialyaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.742383 remotemanager-0.9.3/remotemanager/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/storage/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.9.3/remotemanager/storage/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/storage/remotefunction.py
+-rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.9.3/remotemanager/storage/sendablemixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3696 2023-07-18 13:45:10.000000 remotemanager-0.9.3/remotemanager/storage/trackedfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.742383 remotemanager-0.9.3/remotemanager/transport/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/transport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/transport/cp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.9.3/remotemanager/transport/rsync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.9.3/remotemanager/transport/scp.py
+-rw-rw-rw-   0 root         (0) root         (0)    10027 2023-07-18 09:05:28.000000 remotemanager-0.9.3/remotemanager/transport/transport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.742383 remotemanager-0.9.3/remotemanager/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     5390 2023-07-18 13:45:10.000000 remotemanager-0.9.3/remotemanager/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/utils/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/utils/uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.738383 remotemanager-0.9.3/remotemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-21 11:14:30.000000 remotemanager-0.9.3/remotemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-07-21 11:14:30.000000 remotemanager-0.9.3/remotemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 11:14:30.000000 remotemanager-0.9.3/remotemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2023-07-21 11:14:30.000000 remotemanager-0.9.3/remotemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-21 11:14:30.000000 remotemanager-0.9.3/remotemanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 11:14:30.742383 remotemanager-0.9.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.9.3/setup.py
```

### Comparing `remotemanager-0.9.2/LICENSE` & `remotemanager-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/PKG-INFO` & `remotemanager-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.9.2
+Version: 0.9.3
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.9.2/README.md` & `remotemanager-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/pyproject.toml` & `remotemanager-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 [tool.pytest.ini_options]
 addopts = "--nbval --cov=remotemanager --cov-report term-missing --cov-append --nbval-sanitize-with ./tests/uuid_sanitise.cfg"
 
 [tool.coverage.report]
 omit = ["remotemanager/connection/computers/*"]
 
 [tool.bumpver]
-current_version = "0.9.2"
+current_version = "0.9.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "[clean] bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `remotemanager-0.9.2/remotemanager/connection/cmd.py` & `remotemanager-0.9.3/remotemanager/connection/cmd.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/connection/computers/base.py` & `remotemanager-0.9.3/remotemanager/connection/computers/base.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/connection/computers/example.py` & `remotemanager-0.9.3/remotemanager/connection/computers/example.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/connection/computers/options.py` & `remotemanager-0.9.3/remotemanager/connection/computers/options.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/connection/computers/parsers.py` & `remotemanager-0.9.3/remotemanager/connection/computers/parsers.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/connection/testing_object.py` & `remotemanager-0.9.3/remotemanager/connection/testing_object.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/connection/url.py` & `remotemanager-0.9.3/remotemanager/connection/url.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/dataset/dataset.py` & `remotemanager-0.9.3/remotemanager/dataset/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1271,14 +1271,15 @@
             self._logger.runtime(f"running only runners {format_iterable(uuids)}")
 
         # first step is to handle the writing of the scripts to the local dir
         # the runners take care of this
         runners_to_update = []
         master_content = [f"export {self.main_dir_env}=$PWD\n"]
         goahead = False
+        asynchronous = True  # should always be updated in the loop
         for runner in self.runners:
             if uuids is not None and runner.uuid not in uuids:
                 self._logger.runtime(f"skipping {runner} (uuid {runner.short_uuid})")
                 continue
 
             ready = runner.stage(
                 python=self.url.python, avoid_nodes=avoid_nodes, **run_args
```

### Comparing `remotemanager-0.9.2/remotemanager/dataset/dependency.py` & `remotemanager-0.9.3/remotemanager/dataset/dependency.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/dataset/lazy_append.py` & `remotemanager-0.9.3/remotemanager/dataset/lazy_append.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/dataset/runner.py` & `remotemanager-0.9.3/remotemanager/dataset/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         self._logger.info(f"new runner (id {self.uuid}) created")
 
         self._dependency_info = {}
 
         self._dbfile = dbfile
 
         self._history = {}
-        self.state = "created"
+        self.set_state("created", force=True)
         self.last_submitted = 0
 
         self._identifier = f"{self.parent.name}-{self.parent.short_uuid}-{self.id}"
 
     def __hash__(self) -> hash:
         return hash(self.uuid)
 
@@ -413,18 +413,33 @@
     def state(self) -> RunnerState:
         """
         Returns the most recent runner state
         """
         return self._state
 
     @state.setter
-    def state(self, newstate: str) -> None:
+    def state(self, newstate):
+        self.set_state(newstate)
+
+    def set_state(self, newstate: str, force: bool = False) -> None:
         """
         Update the state and store within the runner history
+
+        .. versionadded:: 0.9.3
+            now checks the current state before setting, won't duplicate states unless
+            force=True
+
+        Args:
+            newstate:
+                state to set to
+            force:
+                skip currentstate checking if True
         """
+        if not force and self.state == newstate:
+            return
 
         t = int(time.time())
         state_time = datetime.fromtimestamp(t)
 
         self.insert_history(state_time, newstate)
         self._state = RunnerState(newstate)
 
@@ -487,36 +502,41 @@
         else:
             argline = f"kwargs = {self.args}"
 
         # python file writing
         # if repo is not overidden by a dependency, generate the import path here
         if repo is None:
             repo = f"${self.parent.main_dir_env}/{self.parent.repofile.name}"
+
+        errorpath = self.errorfile.relative_remote_path(self.run_path)
         # script proper
         runscript = [
             f"import importlib.util, os",
             f"path = os.path.expandvars('{repo}')",
+            f"runtime = os.path.getmtime(path)",
             f"spec = importlib.util.spec_from_file_location('repo', path)",
             f"repo = importlib.util.module_from_spec(spec)",
             f"spec.loader.exec_module(repo)\n",
             argline,
             f"result = repo.{self.parent.function.name}(**kwargs)",
-            f"repo.dump(result, '{self.resultfile.name}')",
+            f"# if the error file mtime (created at run) has changed, don't output",
+            f"if os.path.getmtime(path) == runtime:",
+            f"\trepo.dump(result, '{self.resultfile.name}')",
         ]
         # if this runner is a child, we need to import the previous results
         if self.parent.is_child:
-            runscript.insert(5, self._dependency_info["parent_import"])
+            # if the script changes, the insert point may need to be updated
+            runscript.insert(6, self._dependency_info["parent_import"])
         self.runfile.write("\n".join(runscript))
 
         # jobscript writing
         # initialise script with whatever the parent url needs
         tmp = []
         if not avoid_nodes:
             tmp.append(self.parent._script_sub(**self._run_args_temp))
-        errorpath = self.errorfile.relative_remote_path(self.run_path)
         if self.run_path != self.remote_dir:
             self._logger.debug("run dir is separate to remote dir, appending extras")
             submit = (
                 f"pydir=$PWD\n"
                 f"cd {self.run_dir} && "
                 f"{python} ${{pydir}}/{self.runfile.name} 2>> {errorpath}"
             )
```

### Comparing `remotemanager-0.9.2/remotemanager/dataset/runnerstates.py` & `remotemanager-0.9.3/remotemanager/dataset/runnerstates.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/jupyter/magic.py` & `remotemanager-0.9.3/remotemanager/jupyter/magic.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/logging/__init__.py` & `remotemanager-0.9.3/remotemanager/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/logging/log.py` & `remotemanager-0.9.3/remotemanager/logging/log.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/logging/utils.py` & `remotemanager-0.9.3/remotemanager/logging/utils.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/logging/verbosity.py` & `remotemanager-0.9.3/remotemanager/logging/verbosity.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/serialisation/__init__.py` & `remotemanager-0.9.3/remotemanager/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/serialisation/serial.py` & `remotemanager-0.9.3/remotemanager/serialisation/serial.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/serialisation/serialjsonpickle.py` & `remotemanager-0.9.3/remotemanager/serialisation/serialjsonpickle.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/serialisation/serialyaml.py` & `remotemanager-0.9.3/remotemanager/serialisation/serialyaml.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/storage/database.py` & `remotemanager-0.9.3/remotemanager/storage/database.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/storage/function.py` & `remotemanager-0.9.3/remotemanager/storage/function.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/storage/remotefunction.py` & `remotemanager-0.9.3/remotemanager/storage/remotefunction.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/storage/sendablemixin.py` & `remotemanager-0.9.3/remotemanager/storage/sendablemixin.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/storage/trackedfile.py` & `remotemanager-0.9.3/remotemanager/storage/trackedfile.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/transport/cp.py` & `remotemanager-0.9.3/remotemanager/transport/cp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/transport/rsync.py` & `remotemanager-0.9.3/remotemanager/transport/rsync.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/transport/scp.py` & `remotemanager-0.9.3/remotemanager/transport/scp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/transport/transport.py` & `remotemanager-0.9.3/remotemanager/transport/transport.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/utils/__init__.py` & `remotemanager-0.9.3/remotemanager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/utils/flags.py` & `remotemanager-0.9.3/remotemanager/utils/flags.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager/utils/version.py` & `remotemanager-0.9.3/remotemanager/utils/version.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.2/remotemanager.egg-info/PKG-INFO` & `remotemanager-0.9.3/remotemanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.9.2
+Version: 0.9.3
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.9.2/remotemanager.egg-info/SOURCES.txt` & `remotemanager-0.9.3/remotemanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

