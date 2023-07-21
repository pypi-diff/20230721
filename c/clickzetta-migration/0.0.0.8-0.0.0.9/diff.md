# Comparing `tmp/clickzetta-migration-0.0.0.8.tar.gz` & `tmp/clickzetta-migration-0.0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickzetta-migration-0.0.0.8.tar", last modified: Wed Jul 19 10:53:38 2023, max compression
+gzip compressed data, was "clickzetta-migration-0.0.0.9.tar", last modified: Wed Jul 19 11:39:37 2023, max compression
```

## Comparing `clickzetta-migration-0.0.0.8.tar` & `clickzetta-migration-0.0.0.9.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.016198 clickzetta-migration-0.0.0.8/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       34 2023-07-18 07:23:21.000000 clickzetta-migration-0.0.0.8/MANIFEST.in
--rw-r--r--   0 lihanmiao   (501) staff       (20)      259 2023-07-19 10:53:38.016077 clickzetta-migration-0.0.0.8/PKG-INFO
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.008955 clickzetta-migration-0.0.0.8/clickzetta_migration.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      259 2023-07-19 10:53:37.000000 clickzetta-migration-0.0.0.8/clickzetta_migration.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2086 2023-07-19 10:53:38.000000 clickzetta-migration-0.0.0.8/clickzetta_migration.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-19 10:53:37.000000 clickzetta-migration-0.0.0.8/clickzetta_migration.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       58 2023-07-19 10:53:37.000000 clickzetta-migration-0.0.0.8/clickzetta_migration.egg-info/entry_points.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-19 10:53:37.000000 clickzetta-migration-0.0.0.8/clickzetta_migration.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)      141 2023-07-19 10:53:37.000000 clickzetta-migration-0.0.0.8/clickzetta_migration.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       10 2023-07-19 10:53:37.000000 clickzetta-migration-0.0.0.8/clickzetta_migration.egg-info/top_level.txt
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.009313 clickzetta-migration-0.0.0.8/migration/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:52:59.000000 clickzetta-migration-0.0.0.8/migration/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.009832 clickzetta-migration-0.0.0.8/migration/base/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       90 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.8/migration/base/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      532 2023-07-13 08:55:34.000000 clickzetta-migration-0.0.0.8/migration/base/exceptions.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-07-07 03:37:28.000000 clickzetta-migration-0.0.0.8/migration/base/status.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.010027 clickzetta-migration-0.0.0.8/migration/connector/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:53:59.000000 clickzetta-migration-0.0.0.8/migration/connector/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.010160 clickzetta-migration-0.0.0.8/migration/connector/destination/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 12:17:46.000000 clickzetta-migration-0.0.0.8/migration/connector/destination/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1249 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.0.8/migration/connector/destination/base.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.010433 clickzetta-migration-0.0.0.8/migration/connector/destination/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-29 06:42:41.000000 clickzetta-migration-0.0.0.8/migration/connector/destination/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6137 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.8/migration/connector/destination/clickzetta/destination.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.010704 clickzetta-migration-0.0.0.8/migration/connector/destination/doris/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-11 15:28:35.000000 clickzetta-migration-0.0.0.8/migration/connector/destination/doris/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6243 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.8/migration/connector/destination/doris/destination.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.011314 clickzetta-migration-0.0.0.8/migration/connector/source/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       72 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.8/migration/connector/source/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1879 2023-07-12 03:16:08.000000 clickzetta-migration-0.0.0.8/migration/connector/source/base.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.011593 clickzetta-migration-0.0.0.8/migration/connector/source/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-12 02:11:46.000000 clickzetta-migration-0.0.0.8/migration/connector/source/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7648 2023-07-19 10:52:37.000000 clickzetta-migration-0.0.0.8/migration/connector/source/clickzetta/source.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.011854 clickzetta-migration-0.0.0.8/migration/connector/source/doris/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:41.000000 clickzetta-migration-0.0.0.8/migration/connector/source/doris/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6298 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.8/migration/connector/source/doris/source.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      352 2023-07-11 07:29:24.000000 clickzetta-migration-0.0.0.8/migration/connector/source/enum.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.012052 clickzetta-migration-0.0.0.8/migration/connector/source/hive/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:22.000000 clickzetta-migration-0.0.0.8/migration/connector/source/hive/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.012122 clickzetta-migration-0.0.0.8/migration/connector/source/odps/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:30.000000 clickzetta-migration-0.0.0.8/migration/connector/source/odps/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    11946 2023-07-19 08:11:58.000000 clickzetta-migration-0.0.0.8/migration/migration.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.012624 clickzetta-migration-0.0.0.8/migration/scheduler/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-07-11 04:22:08.000000 clickzetta-migration-0.0.0.8/migration/scheduler/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.012998 clickzetta-migration-0.0.0.8/migration/scheduler/data_transformer/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:25.000000 clickzetta-migration-0.0.0.8/migration/scheduler/data_transformer/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3630 2023-07-12 11:45:19.000000 clickzetta-migration-0.0.0.8/migration/scheduler/data_transformer/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.013268 clickzetta-migration-0.0.0.8/migration/scheduler/data_validation/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:22:21.000000 clickzetta-migration-0.0.0.8/migration/scheduler/data_validation/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2841 2023-07-19 10:52:37.000000 clickzetta-migration-0.0.0.8/migration/scheduler/data_validation/validation.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-07-17 07:57:48.000000 clickzetta-migration-0.0.0.8/migration/scheduler/scheduler.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.013498 clickzetta-migration-0.0.0.8/migration/scheduler/schema_transformer/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:14.000000 clickzetta-migration-0.0.0.8/migration/scheduler/schema_transformer/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4197 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.0.8/migration/scheduler/schema_transformer/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.014518 clickzetta-migration-0.0.0.8/migration/scheduler/task/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      249 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.8/migration/scheduler/task/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1395 2023-07-17 07:55:15.000000 clickzetta-migration-0.0.0.8/migration/scheduler/task/base_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1717 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.8/migration/scheduler/task/data_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1339 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.8/migration/scheduler/task/schema_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3356 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.8/migration/scheduler/task/validation_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2685 2023-07-13 10:20:49.000000 clickzetta-migration-0.0.0.8/migration/scheduler/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.014786 clickzetta-migration-0.0.0.8/migration/scheduler/unify_transformer/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-10 03:55:07.000000 clickzetta-migration-0.0.0.8/migration/scheduler/unify_transformer/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3881 2023-07-11 13:22:48.000000 clickzetta-migration-0.0.0.8/migration/scheduler/unify_transformer/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.015055 clickzetta-migration-0.0.0.8/migration/test/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-28 07:15:40.000000 clickzetta-migration-0.0.0.8/migration/test/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2480 2023-07-19 08:31:48.000000 clickzetta-migration-0.0.0.8/migration/test/util_test.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.015832 clickzetta-migration-0.0.0.8/migration/util/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:54:06.000000 clickzetta-migration-0.0.0.8/migration/util/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7705 2023-07-19 08:16:46.000000 clickzetta-migration-0.0.0.8/migration/util/migration_tasks_status.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1180 2023-07-12 10:01:25.000000 clickzetta-migration-0.0.0.8/migration/util/object_storage_util.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1787 2023-07-19 08:33:07.000000 clickzetta-migration-0.0.0.8/migration/util/script_util.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       23 2023-07-19 10:53:36.000000 clickzetta-migration-0.0.0.8/migration/version.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-07-19 10:53:38.016238 clickzetta-migration-0.0.0.8/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1503 2023-07-19 08:35:49.000000 clickzetta-migration-0.0.0.8/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.815464 clickzetta-migration-0.0.0.9/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       34 2023-07-18 07:23:21.000000 clickzetta-migration-0.0.0.9/MANIFEST.in
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      259 2023-07-19 11:39:37.815306 clickzetta-migration-0.0.0.9/PKG-INFO
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.808188 clickzetta-migration-0.0.0.9/clickzetta_migration.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      259 2023-07-19 11:39:37.000000 clickzetta-migration-0.0.0.9/clickzetta_migration.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2086 2023-07-19 11:39:37.000000 clickzetta-migration-0.0.0.9/clickzetta_migration.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-19 11:39:37.000000 clickzetta-migration-0.0.0.9/clickzetta_migration.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       58 2023-07-19 11:39:37.000000 clickzetta-migration-0.0.0.9/clickzetta_migration.egg-info/entry_points.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-19 11:39:37.000000 clickzetta-migration-0.0.0.9/clickzetta_migration.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      141 2023-07-19 11:39:37.000000 clickzetta-migration-0.0.0.9/clickzetta_migration.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       10 2023-07-19 11:39:37.000000 clickzetta-migration-0.0.0.9/clickzetta_migration.egg-info/top_level.txt
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.808563 clickzetta-migration-0.0.0.9/migration/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:52:59.000000 clickzetta-migration-0.0.0.9/migration/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.809069 clickzetta-migration-0.0.0.9/migration/base/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       90 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.9/migration/base/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      532 2023-07-13 08:55:34.000000 clickzetta-migration-0.0.0.9/migration/base/exceptions.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-07-07 03:37:28.000000 clickzetta-migration-0.0.0.9/migration/base/status.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.809273 clickzetta-migration-0.0.0.9/migration/connector/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:53:59.000000 clickzetta-migration-0.0.0.9/migration/connector/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.809419 clickzetta-migration-0.0.0.9/migration/connector/destination/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 12:17:46.000000 clickzetta-migration-0.0.0.9/migration/connector/destination/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1249 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.0.9/migration/connector/destination/base.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.809697 clickzetta-migration-0.0.0.9/migration/connector/destination/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-29 06:42:41.000000 clickzetta-migration-0.0.0.9/migration/connector/destination/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6137 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.9/migration/connector/destination/clickzetta/destination.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.809975 clickzetta-migration-0.0.0.9/migration/connector/destination/doris/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-11 15:28:35.000000 clickzetta-migration-0.0.0.9/migration/connector/destination/doris/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6243 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.9/migration/connector/destination/doris/destination.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.810576 clickzetta-migration-0.0.0.9/migration/connector/source/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       72 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.9/migration/connector/source/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1879 2023-07-12 03:16:08.000000 clickzetta-migration-0.0.0.9/migration/connector/source/base.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.810867 clickzetta-migration-0.0.0.9/migration/connector/source/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-12 02:11:46.000000 clickzetta-migration-0.0.0.9/migration/connector/source/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7648 2023-07-19 10:52:37.000000 clickzetta-migration-0.0.0.9/migration/connector/source/clickzetta/source.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.811145 clickzetta-migration-0.0.0.9/migration/connector/source/doris/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:41.000000 clickzetta-migration-0.0.0.9/migration/connector/source/doris/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6298 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.9/migration/connector/source/doris/source.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      352 2023-07-11 07:29:24.000000 clickzetta-migration-0.0.0.9/migration/connector/source/enum.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.811343 clickzetta-migration-0.0.0.9/migration/connector/source/hive/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:22.000000 clickzetta-migration-0.0.0.9/migration/connector/source/hive/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.811420 clickzetta-migration-0.0.0.9/migration/connector/source/odps/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:30.000000 clickzetta-migration-0.0.0.9/migration/connector/source/odps/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    11946 2023-07-19 08:11:58.000000 clickzetta-migration-0.0.0.9/migration/migration.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.811922 clickzetta-migration-0.0.0.9/migration/scheduler/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-07-11 04:22:08.000000 clickzetta-migration-0.0.0.9/migration/scheduler/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.812215 clickzetta-migration-0.0.0.9/migration/scheduler/data_transformer/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:25.000000 clickzetta-migration-0.0.0.9/migration/scheduler/data_transformer/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3630 2023-07-12 11:45:19.000000 clickzetta-migration-0.0.0.9/migration/scheduler/data_transformer/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.812498 clickzetta-migration-0.0.0.9/migration/scheduler/data_validation/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:22:21.000000 clickzetta-migration-0.0.0.9/migration/scheduler/data_validation/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2841 2023-07-19 10:52:37.000000 clickzetta-migration-0.0.0.9/migration/scheduler/data_validation/validation.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-07-17 07:57:48.000000 clickzetta-migration-0.0.0.9/migration/scheduler/scheduler.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.812739 clickzetta-migration-0.0.0.9/migration/scheduler/schema_transformer/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:14.000000 clickzetta-migration-0.0.0.9/migration/scheduler/schema_transformer/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4197 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.0.9/migration/scheduler/schema_transformer/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.813852 clickzetta-migration-0.0.0.9/migration/scheduler/task/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      249 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.9/migration/scheduler/task/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1395 2023-07-17 07:55:15.000000 clickzetta-migration-0.0.0.9/migration/scheduler/task/base_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1717 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.9/migration/scheduler/task/data_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1339 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.9/migration/scheduler/task/schema_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3741 2023-07-19 11:39:24.000000 clickzetta-migration-0.0.0.9/migration/scheduler/task/validation_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2685 2023-07-13 10:20:49.000000 clickzetta-migration-0.0.0.9/migration/scheduler/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.814019 clickzetta-migration-0.0.0.9/migration/scheduler/unify_transformer/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-10 03:55:07.000000 clickzetta-migration-0.0.0.9/migration/scheduler/unify_transformer/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3881 2023-07-11 13:22:48.000000 clickzetta-migration-0.0.0.9/migration/scheduler/unify_transformer/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.814303 clickzetta-migration-0.0.0.9/migration/test/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-28 07:15:40.000000 clickzetta-migration-0.0.0.9/migration/test/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2480 2023-07-19 08:31:48.000000 clickzetta-migration-0.0.0.9/migration/test/util_test.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.815048 clickzetta-migration-0.0.0.9/migration/util/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:54:06.000000 clickzetta-migration-0.0.0.9/migration/util/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7705 2023-07-19 08:16:46.000000 clickzetta-migration-0.0.0.9/migration/util/migration_tasks_status.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1180 2023-07-12 10:01:25.000000 clickzetta-migration-0.0.0.9/migration/util/object_storage_util.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1787 2023-07-19 08:33:07.000000 clickzetta-migration-0.0.0.9/migration/util/script_util.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       23 2023-07-19 11:39:36.000000 clickzetta-migration-0.0.0.9/migration/version.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-07-19 11:39:37.815506 clickzetta-migration-0.0.0.9/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1503 2023-07-19 08:35:49.000000 clickzetta-migration-0.0.0.9/setup.py
```

### Comparing `clickzetta-migration-0.0.0.8/clickzetta_migration.egg-info/SOURCES.txt` & `clickzetta-migration-0.0.0.9/clickzetta_migration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.8/migration/base/exceptions.py` & `clickzetta-migration-0.0.0.9/migration/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.8/migration/connector/destination/base.py` & `clickzetta-migration-0.0.0.9/migration/connector/destination/base.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.8/migration/connector/destination/clickzetta/destination.py` & `clickzetta-migration-0.0.0.9/migration/connector/destination/clickzetta/destination.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.8/migration/connector/destination/doris/destination.py` & `clickzetta-migration-0.0.0.9/migration/connector/destination/doris/destination.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.8/migration/connector/source/base.py` & `clickzetta-migration-0.0.0.9/migration/connector/source/base.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.8/migration/connector/source/clickzetta/source.py` & `clickzetta-migration-0.0.0.9/migration/connector/source/clickzetta/source.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.8/migration/connector/source/doris/source.py` & `clickzetta-migration-0.0.0.9/migration/connector/source/doris/source.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.8/migration/migration.py` & `clickzetta-migration-0.0.0.9/migration/migration.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.8/migration/scheduler/data_transformer/transformer.py` & `clickzetta-migration-0.0.0.9/migration/scheduler/data_transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.8/migration/scheduler/data_validation/validation.py` & `clickzetta-migration-0.0.0.9/migration/scheduler/data_validation/validation.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.8/migration/scheduler/scheduler.py` & `clickzetta-migration-0.0.0.9/migration/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.8/migration/scheduler/schema_transformer/transformer.py` & `clickzetta-migration-0.0.0.9/migration/scheduler/schema_transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.8/migration/scheduler/task/base_task.py` & `clickzetta-migration-0.0.0.9/migration/scheduler/task/base_task.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.8/migration/scheduler/task/data_task.py` & `clickzetta-migration-0.0.0.9/migration/scheduler/task/data_task.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.8/migration/scheduler/task/schema_task.py` & `clickzetta-migration-0.0.0.9/migration/scheduler/task/schema_task.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.8/migration/scheduler/task/validation_task.py` & `clickzetta-migration-0.0.0.9/migration/scheduler/task/validation_task.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,16 +32,18 @@
         self.end_time = datetime.now()
         migration_tasks_status.update_task_status(self.destination, self)
         logger.info(f"ValidationTask {self.name} finished running, status: {self.status.value}")
         return self
 
     def check_count(self):
         sql = f"select count(*) from {self.name}"
-        source_count = self.source.execute_sql(sql)
-        destination_count = self.destination.execute_sql(sql)
+        source_count = self.source.execute_sql(sql)[0]
+        logger.info(f"source table: {self.name} count: {source_count}")
+        destination_count = self.destination.execute_sql(sql)[0]
+        logger.info(f"destination table {self.name} count: {destination_count}")
         if source_count != destination_count:
             self.status = TaskStatus.FAILED
             self.end_time = datetime.now()
             migration_tasks_status.update_task_status(self.destination, self)
             logger.error(
                 f"ValidationTask {self.name} failed to run, error: count not equal, retry times: {self.retry_times}")
             return False
@@ -50,15 +52,17 @@
     def check_number_type_statistics(self):
         type_mapping = self.source.type_mapping()
         table_columns = self.source.get_table_columns(self.name.split('.')[0], self.name.split('.')[1])
         for column in table_columns:
             if self.is_number_type(column, type_mapping):
                 sql = f"select min({column.name}), max({column.name}), avg({column.name}) from {self.name}"
                 source_result = self.source.execute_sql(sql)
+                logger.info(f"source table: {self.name} column: {column.name} statistics: {source_result}")
                 destination_result = self.destination.execute_sql(sql)
+                logger.info(f"destination table: {self.name} column: {column.name} statistics: {destination_result}")
                 if source_result != destination_result:
                     self.status = TaskStatus.FAILED
                     self.end_time = datetime.now()
                     migration_tasks_status.update_task_status(self.destination, self)
                     logger.error(
                         f'ValidationTask {self.name} failed to run, error: number type statistics not equal, retry times: {self.retry_times}')
                     return False
```

### Comparing `clickzetta-migration-0.0.0.8/migration/scheduler/transformer.py` & `clickzetta-migration-0.0.0.9/migration/scheduler/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.8/migration/scheduler/unify_transformer/transformer.py` & `clickzetta-migration-0.0.0.9/migration/scheduler/unify_transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.8/migration/test/util_test.py` & `clickzetta-migration-0.0.0.9/migration/test/util_test.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.8/migration/util/migration_tasks_status.py` & `clickzetta-migration-0.0.0.9/migration/util/migration_tasks_status.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.8/migration/util/object_storage_util.py` & `clickzetta-migration-0.0.0.9/migration/util/object_storage_util.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.8/migration/util/script_util.py` & `clickzetta-migration-0.0.0.9/migration/util/script_util.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.8/setup.py` & `clickzetta-migration-0.0.0.9/setup.py`

 * *Files identical despite different names*

