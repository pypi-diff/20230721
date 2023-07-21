# Comparing `tmp/tamr_toolbox-1.8.1.tar.gz` & `tmp/tamr_toolbox-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tamr_toolbox-1.8.1.tar", last modified: Fri Jul 29 21:18:02 2022, max compression
+gzip compressed data, was "dist/tamr_toolbox-1.9.0.tar", last modified: Wed Dec 21 16:12:13 2022, max compression
```

## Comparing `tamr_toolbox-1.8.1.tar` & `tamr_toolbox-1.9.0.tar`

### file list

```diff
@@ -1,100 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox/project/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox/project/golden_records/
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/project/golden_records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6750 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/project/golden_records/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox/project/_common/
--rw-r--r--   0 runner    (1001) docker     (121)     8382 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/project/_common/transformations.py
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/project/_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11095 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/project/_common/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     7174 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/project/_common/movement.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox/project/categorization/
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/project/categorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6252 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/project/categorization/jobs.py
--rw-r--r--   0 runner    (1001) docker     (121)     9433 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/project/categorization/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox/project/schema_mapping/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/project/schema_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2748 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/project/schema_mapping/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox/project/mastering/
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/project/mastering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16485 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/project/mastering/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox/data_io/
--rw-r--r--   0 runner    (1001) docker     (121)     6744 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/data_io/common.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/data_io/file_system_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/data_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12534 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/data_io/csv.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox/data_io/df_connect/
--rw-r--r--   0 runner    (1001) docker     (121)     2161 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/data_io/df_connect/jdbc_info.py
--rw-r--r--   0 runner    (1001) docker     (121)    16789 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/data_io/df_connect/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/data_io/df_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14817 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/data_io/dataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox/models/
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/models/operation_state.py
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/models/project_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      547 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/models/validation_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     5261 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/models/project_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (121)     5200 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/models/attribute_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      421 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/models/data_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/models/project_steps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox/workflow/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox/workflow/concurrent/
--rw-r--r--   0 runner    (1001) docker     (121)    10073 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/workflow/concurrent/Planner.py
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/workflow/concurrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3101 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/workflow/concurrent/PlanNodeStatus.py
--rw-r--r--   0 runner    (1001) docker     (121)    10924 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/workflow/concurrent/PlanNode.py
--rw-r--r--   0 runner    (1001) docker     (121)     1392 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/workflow/concurrent/PlanStatus.py
--rw-r--r--   0 runner    (1001) docker     (121)     8738 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/workflow/concurrent/Graph.py
--rw-r--r--   0 runner    (1001) docker     (121)    14499 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/workflow/backup.py
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6279 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/workflow/jobs.py
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox/dataset/
--rw-r--r--   0 runner    (1001) docker     (121)    21080 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/dataset/manage.py
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2240 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/dataset/_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox/realtime/
--rw-r--r--   0 runner    (1001) docker     (121)     8695 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/realtime/matching.py
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/realtime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox/notifications/
--rw-r--r--   0 runner    (1001) docker     (121)     3092 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/notifications/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     8142 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/notifications/emails.py
--rw-r--r--   0 runner    (1001) docker     (121)     4151 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/notifications/slack.py
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox/enrichment/
--rw-r--r--   0 runner    (1001) docker     (121)     8395 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/enrichment/translate.py
--rw-r--r--   0 runner    (1001) docker     (121)    15671 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/enrichment/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/enrichment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox/enrichment/api_client/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/enrichment/api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7462 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/enrichment/api_client/google.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     5925 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/utils/operation.py
--rw-r--r--   0 runner    (1001) docker     (121)     6741 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/utils/upstream.py
--rw-r--r--   0 runner    (1001) docker     (121)     6130 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/utils/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    12434 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (121)     6563 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     8247 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9401 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/utils/downstream.py
--rw-r--r--   0 runner    (1001) docker     (121)     3113 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/utils/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox/filesystem/
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/filesystem/cloud.py
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5108 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/filesystem/bash.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox/sysadmin/
--rw-r--r--   0 runner    (1001) docker     (121)    22943 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/sysadmin/instance.py
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/tamr_toolbox/sysadmin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11334 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2761 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-29 21:18:02.000000 tamr_toolbox-1.8.1/tamr_toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-07-29 21:17:55.000000 tamr_toolbox-1.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2022-12-21 16:12:09.000000 tamr_toolbox-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2022-12-21 16:12:09.000000 tamr_toolbox-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox/data_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/data_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/data_io/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12534 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/data_io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14817 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/data_io/dataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox/data_io/df_connect/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/data_io/df_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17252 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/data_io/df_connect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/data_io/df_connect/jdbc_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/data_io/file_system_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/dataset/_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21080 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/dataset/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox/enrichment/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/enrichment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox/enrichment/api_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/enrichment/api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7462 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/enrichment/api_client/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15670 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/enrichment/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/enrichment/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/filesystem/bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/filesystem/cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/models/attribute_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/models/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/models/operation_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/models/project_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/models/project_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/models/project_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/models/validation_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/notifications/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/notifications/emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/notifications/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox/project/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox/project/_common/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/project/_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/project/_common/movement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11095 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/project/_common/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/project/_common/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox/project/categorization/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/project/categorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/project/categorization/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9433 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/project/categorization/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12294 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/project/categorization/taxonomy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox/project/golden_records/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/project/golden_records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/project/golden_records/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox/project/mastering/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/project/mastering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16455 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/project/mastering/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox/project/schema_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/project/schema_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/project/schema_mapping/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox/realtime/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/realtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8695 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/realtime/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox/sysadmin/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/sysadmin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22943 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/sysadmin/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/utils/downstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/utils/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12434 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6741 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/utils/upstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8247 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/workflow/backup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox/workflow/concurrent/
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/workflow/concurrent/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10924 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/workflow/concurrent/PlanNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/workflow/concurrent/PlanNodeStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/workflow/concurrent/PlanStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/workflow/concurrent/Planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/workflow/concurrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2022-12-21 16:12:10.000000 tamr_toolbox-1.9.0/tamr_toolbox/workflow/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-21 16:12:13.000000 tamr_toolbox-1.9.0/tamr_toolbox.egg-info/top_level.txt
```

### Comparing `tamr_toolbox-1.8.1/PKG-INFO` & `tamr_toolbox-1.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: tamr_toolbox
-Version: 1.8.1
+Version: 1.9.0
 Summary: Tools for Tamr
 Home-page: https://github.com/Datatamer/tamr-toolbox
 Author: Tamr Inc.
 Author-email: 
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: pandas
 Provides-Extra: slack
 Provides-Extra: testing
 Provides-Extra: translation
@@ -34,9 +32,7 @@
 
 ## Community Contributions
 Contributions to the Tamr Toolbox are currently limited to Tamr employees only. 
 Tamr does not routinely review or merge community submitted pull requests.
 
 If you are a community member that would like to report a bug or a feature request, you may 
 file a Github issue in the tamr-toolbox repository.
-
-
```

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/project/golden_records/jobs.py` & `tamr_toolbox-1.9.0/tamr_toolbox/project/golden_records/jobs.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/project/_common/transformations.py` & `tamr_toolbox-1.9.0/tamr_toolbox/project/_common/transformations.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/project/_common/schema.py` & `tamr_toolbox-1.9.0/tamr_toolbox/project/_common/schema.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/project/_common/movement.py` & `tamr_toolbox-1.9.0/tamr_toolbox/project/_common/movement.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/project/categorization/jobs.py` & `tamr_toolbox-1.9.0/tamr_toolbox/project/categorization/jobs.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/project/categorization/metrics.py` & `tamr_toolbox-1.9.0/tamr_toolbox/project/categorization/metrics.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/project/schema_mapping/jobs.py` & `tamr_toolbox-1.9.0/tamr_toolbox/project/schema_mapping/jobs.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/project/mastering/jobs.py` & `tamr_toolbox-1.9.0/tamr_toolbox/project/mastering/jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         The operations that were run
 
     """
 
     completed_operations = []
     if run_estimate_pair_counts:
         LOGGER.info(f"Estimate pair counts for project {project.name} (id={project.resource_id}).")
-        op = project.estimate_pairs().refresh(asynchronous=process_asynchronously)
+        op = operation.safe_estimate_counts(project)
         if not process_asynchronously:
             operation.enforce_success(op)
         completed_operations.append(op)
     if run_generate_pairs:
         LOGGER.info(f"Generating pairs for project {project.name} (id={project.resource_id}).")
         op = project.pairs().refresh(asynchronous=process_asynchronously)
         if not process_asynchronously:
```

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/data_io/common.py` & `tamr_toolbox-1.9.0/tamr_toolbox/data_io/common.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/data_io/csv.py` & `tamr_toolbox-1.9.0/tamr_toolbox/data_io/csv.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/data_io/df_connect/jdbc_info.py` & `tamr_toolbox-1.9.0/tamr_toolbox/data_io/df_connect/jdbc_info.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/data_io/df_connect/client.py` & `tamr_toolbox-1.9.0/tamr_toolbox/data_io/df_connect/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 import requests
 from enum import Enum
 from tamr_toolbox.data_io.df_connect import jdbc_info
 from tamr_toolbox.models.data_type import JsonDict
 from tamr_toolbox.data_io.file_system_type import FileSystemType
 from tamr_unify_client.auth import UsernamePasswordAuth
-from typing import Dict, List, Union
+from typing import Dict, List, Union, Optional
 
 LOGGER = logging.getLogger(__name__)
 
 
 @dataclass
 class Client:
     """A data class for interacting with df_connect via jdbc.
@@ -21,23 +21,25 @@
         host: the host where df_connect is running
         port: the port on which df_connect is listening
         protocol: http or https
         base_path: if using nginx-like proxy this is the redirect path
         tamr_username: the tamr account to use
         tamr_password: the password for the tamr account to use
         jbdc_info: configuration information for the jdbc connection
+        cert: optional path to a certfile for authentication
     """
 
     host: str
     port: str
     protocol: str
     base_path: str
     tamr_username: str
     tamr_password: str
     jdbc_info: jdbc_info.JdbcInfo
+    cert: Optional[str]
 
 
 def from_config(
     config: JsonDict, config_key: str = "df_connect", jdbc_key: str = "ingest"
 ) -> Client:
     """Constructs a Client object from a json dictionary.
 
@@ -51,59 +53,69 @@
         A Client object
     """
 
     # proxy and port redirect are optional
     base_path = config[config_key].get("base_path", "")
     port = config[config_key].get("port", "")
 
+    # Optional cert may or may not be present in config file (back-compat from TBOX-295)
+    if "cert" in config[config_key].keys():
+        cert = config[config_key]["cert"]
+    else:
+        cert = None
+
     return Client(
         host=config[config_key]["host"],
         port=port,
         protocol=config[config_key]["protocol"],
         base_path=base_path,
         tamr_username=config[config_key]["tamr_username"],
         tamr_password=config[config_key]["tamr_password"],
         jdbc_info=jdbc_info.from_config(config, config_key=config_key, jdbc_key=jdbc_key),
+        cert=cert,
     )
 
 
 def create(
     *,
     host: str,
     port: str = "",
     protocol: str,
     base_path="",
     tamr_username: str,
     tamr_password: str,
     jdbc_dict: JsonDict,
+    cert: Optional[str] = None,
 ) -> Client:
     """
     Simple wrapper for creating an instance of `Client` dataclass object.
 
     Args:
         host: the host where df_connect is running
         port: the port on which df_connect is listening
         protocol: http or https
         base_path: if using nginx-like proxy this is the redirect path
         tamr_username: the tamr account to use
         tamr_password: the password for the tamr account to use
         jdbc_dict: configuration information for the jdbc connection
+        cert: optional path to a certfile for authentication
 
     Returns:
         An instance of `tamr_toolbox.data_io.df_connect.Client`
     """
     jdbc_information = jdbc_info.create(**jdbc_dict)
     return Client(
         host=host,
         port=port,
         protocol=protocol,
         base_path=base_path,
         tamr_username=tamr_username,
         tamr_password=tamr_password,
         jdbc_info=jdbc_information,
+        cert=cert,
     )
 
 
 def _get_url(connect_info: Client, api_path: str) -> str:
     """Constructs and returns url for request to df_connect. Valid for both http and https.
 
      Args:
@@ -198,14 +210,15 @@
         RuntimeError: if the a connection to df_connect cannot be established
     """
     auth = UsernamePasswordAuth(connect_info.tamr_username, connect_info.tamr_password)
     s = requests.Session()
     s.auth = auth
     s.headers.update({"Content-type": "application/json"})
     s.headers.update({"Accept": "application/json"})
+    s.cert = connect_info.cert
 
     # test that df_connect is running properly
     url = _get_url(connect_info, "/api/service/health")
     try:
         r = s.get(url)
         r.raise_for_status()
     except (requests.exceptions.ConnectionError, requests.exceptions.HTTPError):
```

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/data_io/dataframe.py` & `tamr_toolbox-1.9.0/tamr_toolbox/data_io/dataframe.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/models/operation_state.py` & `tamr_toolbox-1.9.0/tamr_toolbox/models/operation_state.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/models/validation_check.py` & `tamr_toolbox-1.9.0/tamr_toolbox/models/validation_check.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/models/project_artifacts.py` & `tamr_toolbox-1.9.0/tamr_toolbox/models/project_artifacts.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/models/attribute_type.py` & `tamr_toolbox-1.9.0/tamr_toolbox/models/attribute_type.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/models/project_steps.py` & `tamr_toolbox-1.9.0/tamr_toolbox/models/project_steps.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/workflow/concurrent/Planner.py` & `tamr_toolbox-1.9.0/tamr_toolbox/workflow/concurrent/Planner.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/workflow/concurrent/PlanNodeStatus.py` & `tamr_toolbox-1.9.0/tamr_toolbox/workflow/concurrent/PlanNodeStatus.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/workflow/concurrent/PlanNode.py` & `tamr_toolbox-1.9.0/tamr_toolbox/workflow/concurrent/PlanNode.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/workflow/concurrent/PlanStatus.py` & `tamr_toolbox-1.9.0/tamr_toolbox/workflow/concurrent/PlanStatus.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/workflow/concurrent/Graph.py` & `tamr_toolbox-1.9.0/tamr_toolbox/workflow/concurrent/Graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,19 +19,21 @@
     and the generated graph from them.
     """
 
     edges: set
     directed_graph: nx.DiGraph
 
 
-def _get_upstream_projects(project: Project) -> List[Project]:
+def _get_upstream_projects(project: Project, *, all_projects: List[Project]) -> List[Project]:
     """
     get projects immediately upstream of a given project
     Args:
         project: the project to check
+        all_projects: a list of all Projects on the Tamr Core instance
+
     Returns:
         A list of project names upstream of the project
     """
     client = project.client
     # find upstream datasets - if GR project just get input datasets
     if ProjectType[project.type] == ProjectType.GOLDEN_RECORDS:
         upstream_datasets = [x for x in project.input_datasets().stream()]
@@ -48,29 +50,34 @@
         upstream_dataset = client.datasets.by_resource_id(upstream_result.resource_id)
         # see if it is the output of a project and if so add to the list
         upstream_dataset_projects = set(
             x.project_name for x in upstream_dataset.usage().usage.output_from_project_steps
         )
         upstream_project_names.extend([x for x in upstream_dataset_projects])
 
-    return [client.projects.by_name(x) for x in upstream_project_names]
+    # we have all projects in all_projects variables so only return those whose
+    # name is in upstream_project_names
+    return [x for x in all_projects if x.name in upstream_project_names]
 
 
-def _build_edges(project: Project, client: Client, edges: set = None) -> Set[Tuple[str, str]]:
+def _build_edges(
+    project: Project, client: Client, *, edges: set = None, all_projects: List[Project]
+) -> Set[Tuple[str, str]]:
     """
     builds a set of tuples of all edges of format (source, target)
     Args:
         project: the project to get edges for
         client: tamr client
         edges: set of tuples (source, target)
+        all_projects: a list of all Projects on the Tamr Core instance
 
     Returns:
 
     """
-    upstream_projects = _get_upstream_projects(project)
+    upstream_projects = _get_upstream_projects(project, all_projects=all_projects)
 
     if edges is None:
         edges = set()
 
     for upstream_project in upstream_projects:
         # add the edge for this upstream dataset
         edges.add((upstream_project.name, project.name))
@@ -80,15 +87,17 @@
             LOGGER.debug(
                 f"skipping dataset {upstream_project.name} since it is already"
                 f" in edges as target: {[ x for x in edges if x[1] ==upstream_project.name]}"
             )
             continue
         else:
             # and then go to it and get it's upstream datasets
-            further_upstream_edges = _build_edges(upstream_project, client, edges=set(edges))
+            further_upstream_edges = _build_edges(
+                upstream_project, client, edges=set(edges), all_projects=all_projects
+            )
             # print(f"adding further upstream edges {further_upstream_edges}")
             edges = edges.union(further_upstream_edges)
 
     return edges
 
 
 def from_edges(edges: Set[tuple]) -> Graph:
@@ -114,17 +123,21 @@
         client: tamr client
 
     Returns:
         A Graph object built from the dependencies of the datasets passed
     """
     # start with empty set
     graph_edges = set()
+    # save all projects to list so we don't have to hit the API every time
+    all_projects = [x for x in client.projects.stream()]
     # for each dataset get the edges and take union
     for project in projects:
-        graph_edges = set(graph_edges.union(_build_edges(project, client)))
+        graph_edges = set(
+            graph_edges.union(_build_edges(project, client, all_projects=all_projects))
+        )
 
     graph = nx.DiGraph()
     graph.add_edges_from(graph_edges)
     return Graph(edges=graph_edges, directed_graph=graph)
 
 
 def get_source_nodes(graph: Graph) -> List[str]:
```

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/workflow/backup.py` & `tamr_toolbox-1.9.0/tamr_toolbox/workflow/backup.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/__init__.py` & `tamr_toolbox-1.9.0/tamr_toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/dataset/manage.py` & `tamr_toolbox-1.9.0/tamr_toolbox/dataset/manage.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/dataset/_dataset.py` & `tamr_toolbox-1.9.0/tamr_toolbox/dataset/_dataset.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/realtime/matching.py` & `tamr_toolbox-1.9.0/tamr_toolbox/realtime/matching.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/notifications/common.py` & `tamr_toolbox-1.9.0/tamr_toolbox/notifications/common.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/notifications/emails.py` & `tamr_toolbox-1.9.0/tamr_toolbox/notifications/emails.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/notifications/slack.py` & `tamr_toolbox-1.9.0/tamr_toolbox/notifications/slack.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/enrichment/translate.py` & `tamr_toolbox-1.9.0/tamr_toolbox/enrichment/translate.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/enrichment/dictionary.py` & `tamr_toolbox-1.9.0/tamr_toolbox/enrichment/dictionary.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     """
     A DataClass for translation dictionaries
 
     Args:
         standardized_phrase: The unique common standardized version of all original_phrases
         translated_phrase: The translated standardized phrase to the target language of the
             dictionary
-        detected_language: The language detected of the standardized phrase if source lanaguage is
+        detected_language: The language detected of the standardized phrase if source language is
             set to auto
         original_phrases: A set of original phrases which all convert to the standardized phrases
             when applying standardization
     """
 
     standardized_phrase: str = None
     translated_phrase: str = None
```

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/enrichment/api_client/google.py` & `tamr_toolbox-1.9.0/tamr_toolbox/enrichment/api_client/google.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/utils/operation.py` & `tamr_toolbox-1.9.0/tamr_toolbox/utils/operation.py`

 * *Files 5% similar despite different names*

```diff
@@ -183,7 +183,21 @@
         if operation.status is None:
             return operation
         elif new_status == status:
             sleep(poll_interval_seconds)
         else:
             return operation
     raise TimeoutError(f"Waiting for operation took longer than {timeout_seconds} seconds.")
+
+
+def safe_estimate_counts(project) -> Operation:
+    """
+    Run the estimate counts job of project that works if it is the first
+    Args:
+        project: A Tamr project object
+    Returns:
+        An operation object for the estimate pairs job
+    """
+    project = project.as_mastering()
+    response = project.client.post(f"{project.api_path}/estimatedPairCounts:refresh")
+
+    return Operation.from_response(project.client, response).wait()
```

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/utils/upstream.py` & `tamr_toolbox-1.9.0/tamr_toolbox/utils/upstream.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/utils/client.py` & `tamr_toolbox-1.9.0/tamr_toolbox/utils/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,38 +42,44 @@
 def create(
     *,
     username: str,
     password: str,
     host: str,
     port: Optional[Union[str, int]] = 9100,
     protocol: str = "http",
+    base_path: str = "/api/versioned/v1/",
+    session: Optional[requests.Session] = None,
     store_auth_cookie: bool = False,
     enforce_healthy: bool = False,
 ) -> Client:
     """Creates a Tamr client from the provided configuration values
 
     Args:
         username: The username to log access Tamr as
         password: the password for the user
         host: The ip address of Tamr
         port: The port of the Tamr UI. Pass a value of `None` to specify an address with no port
         protocol: https or http
+        base_path: Optional argument to specify a different base path
+        session: Optional argument to pass an existing requests Session
         store_auth_cookie: If true will allow Tamr authentication cookie to be stored and reused
         enforce_healthy: If true will enforce a healthy state upon creation
 
     Returns:
         Tamr client
     """
     full_address = f"{protocol}://{host}:{port}" if port is not None else f"{protocol}://{host}"
     LOGGER.info(f"Creating client as user {username} at {full_address}.")
     client = Client(
         auth=UsernamePasswordAuth(username=username, password=password),
         host=host,
         port=int(port) if port is not None else None,
         protocol=protocol,
+        base_path=base_path,
+        session=session,
         store_auth_cookie=store_auth_cookie,
     )
     if enforce_healthy:
         if not health_check(client):
             LOGGER.error(f"Tamr is not healthy. Check logs and Tamr.")
             raise SystemError("Tamr is not healthy. Check logs and Tamr.")
     return client
```

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/utils/testing.py` & `tamr_toolbox-1.9.0/tamr_toolbox/utils/testing.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/utils/logger.py` & `tamr_toolbox-1.9.0/tamr_toolbox/utils/logger.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/utils/version.py` & `tamr_toolbox-1.9.0/tamr_toolbox/utils/version.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/utils/downstream.py` & `tamr_toolbox-1.9.0/tamr_toolbox/utils/downstream.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/utils/config.py` & `tamr_toolbox-1.9.0/tamr_toolbox/utils/config.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/filesystem/cloud.py` & `tamr_toolbox-1.9.0/tamr_toolbox/filesystem/cloud.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/filesystem/bash.py` & `tamr_toolbox-1.9.0/tamr_toolbox/filesystem/bash.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox/sysadmin/instance.py` & `tamr_toolbox-1.9.0/tamr_toolbox/sysadmin/instance.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/LICENSE` & `tamr_toolbox-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/setup.py` & `tamr_toolbox-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox.egg-info/SOURCES.txt` & `tamr_toolbox-1.9.0/tamr_toolbox.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 tamr_toolbox/project/_common/__init__.py
 tamr_toolbox/project/_common/movement.py
 tamr_toolbox/project/_common/schema.py
 tamr_toolbox/project/_common/transformations.py
 tamr_toolbox/project/categorization/__init__.py
 tamr_toolbox/project/categorization/jobs.py
 tamr_toolbox/project/categorization/metrics.py
+tamr_toolbox/project/categorization/taxonomy.py
 tamr_toolbox/project/golden_records/__init__.py
 tamr_toolbox/project/golden_records/jobs.py
 tamr_toolbox/project/mastering/__init__.py
 tamr_toolbox/project/mastering/jobs.py
 tamr_toolbox/project/schema_mapping/__init__.py
 tamr_toolbox/project/schema_mapping/jobs.py
 tamr_toolbox/realtime/__init__.py
```

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox.egg-info/PKG-INFO` & `tamr_toolbox-1.9.0/tamr_toolbox.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: tamr-toolbox
-Version: 1.8.1
+Version: 1.9.0
 Summary: Tools for Tamr
 Home-page: https://github.com/Datatamer/tamr-toolbox
 Author: Tamr Inc.
 Author-email: 
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: pandas
 Provides-Extra: slack
 Provides-Extra: testing
 Provides-Extra: translation
@@ -34,9 +32,7 @@
 
 ## Community Contributions
 Contributions to the Tamr Toolbox are currently limited to Tamr employees only. 
 Tamr does not routinely review or merge community submitted pull requests.
 
 If you are a community member that would like to report a bug or a feature request, you may 
 file a Github issue in the tamr-toolbox repository.
-
-
```

### Comparing `tamr_toolbox-1.8.1/tamr_toolbox.egg-info/requires.txt` & `tamr_toolbox-1.9.0/tamr_toolbox.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tamr_toolbox-1.8.1/README.md` & `tamr_toolbox-1.9.0/README.md`

 * *Files identical despite different names*

