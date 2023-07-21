# Comparing `tmp/rondsspark-0.0.4.7.tar.gz` & `tmp/rondsspark-0.0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rondsspark-0.0.4.7.tar", last modified: Tue Jul 11 05:56:12 2023, max compression
+gzip compressed data, was "dist/rondsspark-0.0.4.8.tar", last modified: Tue Jul 11 08:53:24 2023, max compression
```

## Comparing `rondsspark-0.0.4.7.tar` & `rondsspark-0.0.4.8.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6975 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/tools/utils.py
--rw-r--r--   0 root         (0) root         (0)      463 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/tools/schedule.py
--rw-r--r--   0 root         (0) root         (0)    13291 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/spark/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/spark/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4621 2023-07-07 06:07:55.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/spark/transforms.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/__init__.py
--rw-r--r--   0 root         (0) root         (0)       66 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/core.py
--rw-r--r--   0 root         (0) root         (0)      516 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/remote_debug.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/pandas/
--rw-r--r--   0 root         (0) root         (0)     6620 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/pandas/cassandra_rule.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/pandas/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13645 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/pandas/transforms.py
--rw-r--r--   0 root         (0) root         (0)     4742 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/pandas/rule_merge_data.py
--rw-r--r--   0 root         (0) root         (0)     6452 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/ronds.py
--rw-r--r--   0 root         (0) root         (0)     8334 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/transforms/ptransform.py
--rw-r--r--   0 root         (0) root         (0)      860 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)      258 2023-07-07 06:07:55.000000 rondsspark-0.0.4.7/ronds_sdk/logger_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/runners/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/runners/visitors/
--rw-r--r--   0 root         (0) root         (0)     3769 2023-07-07 06:07:55.000000 rondsspark-0.0.4.7/ronds_sdk/runners/visitors/spark_runner_visitor.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/runners/visitors/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/runners/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2863 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/runners/runner.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/runners/python_runner.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/runners/pipeline_context.py
--rw-r--r--   0 root         (0) root         (0)     2690 2023-07-07 06:07:55.000000 rondsspark-0.0.4.7/ronds_sdk/runners/spark_runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/templates/
--rw-r--r--   0 root         (0) root         (0)     1696 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/templates/phm_rules_editor.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/templates/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/dataframe/
--rw-r--r--   0 root         (0) root         (0)     4198 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/dataframe/pvalue.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/dataframe/__init__.py
--rw-r--r--   0 root         (0) root         (0)      505 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/logging_config.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/options/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/options/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6218 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/options/value_provider.py
--rw-r--r--   0 root         (0) root         (0)     7532 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/options/pipeline_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/ml/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/ml/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/ronds_sdk/datasources/
--rw-r--r--   0 root         (0) root         (0)     3192 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/datasources/cassandra_manager.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/ronds_sdk/datasources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/datasources/kafka_manager.py
--rw-r--r--   0 root         (0) root         (0)      832 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/ronds_sdk/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/rondsspark.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1641 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/rondsspark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/rondsspark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      219 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/rondsspark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/rondsspark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/rondsspark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      219 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      524 2023-07-11 05:36:08.000000 rondsspark-0.0.4.7/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/test/sdk/
--rw-r--r--   0 root         (0) root         (0)     3487 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/test/sdk/sdk_test.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/test/sdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3686 2023-07-11 05:34:55.000000 rondsspark-0.0.4.7/test/sdk/sdk_unitest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/test/simple/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/test/simple/__init__.py
--rw-r--r--   0 root         (0) root         (0)      902 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/test/simple/overloading_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:56:12.000000 rondsspark-0.0.4.7/test/spark/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/test/spark/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2736 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/test/spark/SparkTest.py
--rw-r--r--   0 root         (0) root         (0)      498 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/test/spark/SimpleTest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.7/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/ronds_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/ronds_sdk/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/ronds_sdk/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6975 2023-07-11 05:34:55.000000 rondsspark-0.0.4.8/ronds_sdk/tools/utils.py
+-rw-r--r--   0 root         (0) root         (0)      463 2023-07-11 05:34:55.000000 rondsspark-0.0.4.8/ronds_sdk/tools/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    13291 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/ronds_sdk/pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/ronds_sdk/transforms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/ronds_sdk/transforms/spark/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/ronds_sdk/transforms/spark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-07-07 06:07:55.000000 rondsspark-0.0.4.8/ronds_sdk/transforms/spark/transforms.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/ronds_sdk/transforms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/ronds_sdk/transforms/core.py
+-rw-r--r--   0 root         (0) root         (0)      516 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/ronds_sdk/transforms/remote_debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/ronds_sdk/transforms/pandas/
+-rw-r--r--   0 root         (0) root         (0)     6647 2023-07-11 08:53:01.000000 rondsspark-0.0.4.8/ronds_sdk/transforms/pandas/cassandra_rule.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/ronds_sdk/transforms/pandas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13645 2023-07-11 05:34:55.000000 rondsspark-0.0.4.8/ronds_sdk/transforms/pandas/transforms.py
+-rw-r--r--   0 root         (0) root         (0)     4821 2023-07-11 08:53:01.000000 rondsspark-0.0.4.8/ronds_sdk/transforms/pandas/rule_merge_data.py
+-rw-r--r--   0 root         (0) root         (0)     6452 2023-07-11 05:34:55.000000 rondsspark-0.0.4.8/ronds_sdk/transforms/ronds.py
+-rw-r--r--   0 root         (0) root         (0)     8334 2023-07-11 05:34:55.000000 rondsspark-0.0.4.8/ronds_sdk/transforms/ptransform.py
+-rw-r--r--   0 root         (0) root         (0)      860 2023-07-11 05:34:55.000000 rondsspark-0.0.4.8/ronds_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      258 2023-07-07 06:07:55.000000 rondsspark-0.0.4.8/ronds_sdk/logger_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/ronds_sdk/runners/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/ronds_sdk/runners/visitors/
+-rw-r--r--   0 root         (0) root         (0)     3769 2023-07-07 06:07:55.000000 rondsspark-0.0.4.8/ronds_sdk/runners/visitors/spark_runner_visitor.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/ronds_sdk/runners/visitors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/ronds_sdk/runners/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2863 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/ronds_sdk/runners/runner.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/ronds_sdk/runners/python_runner.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/ronds_sdk/runners/pipeline_context.py
+-rw-r--r--   0 root         (0) root         (0)     2690 2023-07-07 06:07:55.000000 rondsspark-0.0.4.8/ronds_sdk/runners/spark_runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/ronds_sdk/templates/
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-07-11 05:34:55.000000 rondsspark-0.0.4.8/ronds_sdk/templates/phm_rules_editor.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 05:34:55.000000 rondsspark-0.0.4.8/ronds_sdk/templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/ronds_sdk/dataframe/
+-rw-r--r--   0 root         (0) root         (0)     4198 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/ronds_sdk/dataframe/pvalue.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/ronds_sdk/dataframe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      505 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/ronds_sdk/logging_config.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/ronds_sdk/options/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/ronds_sdk/options/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6218 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/ronds_sdk/options/value_provider.py
+-rw-r--r--   0 root         (0) root         (0)     7532 2023-07-11 05:34:55.000000 rondsspark-0.0.4.8/ronds_sdk/options/pipeline_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/ronds_sdk/ml/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/ronds_sdk/ml/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/ronds_sdk/datasources/
+-rw-r--r--   0 root         (0) root         (0)     3192 2023-07-11 05:34:55.000000 rondsspark-0.0.4.8/ronds_sdk/datasources/cassandra_manager.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/ronds_sdk/datasources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-11 05:34:55.000000 rondsspark-0.0.4.8/ronds_sdk/datasources/kafka_manager.py
+-rw-r--r--   0 root         (0) root         (0)      832 2023-07-11 05:34:55.000000 rondsspark-0.0.4.8/ronds_sdk/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/rondsspark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1641 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/rondsspark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/rondsspark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      219 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/rondsspark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/rondsspark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/rondsspark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      219 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-11 08:53:01.000000 rondsspark-0.0.4.8/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/test/sdk/
+-rw-r--r--   0 root         (0) root         (0)     3487 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/test/sdk/sdk_test.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/test/sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3686 2023-07-11 05:34:55.000000 rondsspark-0.0.4.8/test/sdk/sdk_unitest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/test/simple/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/test/simple/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      902 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/test/simple/overloading_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:53:24.000000 rondsspark-0.0.4.8/test/spark/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/test/spark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/test/spark/SparkTest.py
+-rw-r--r--   0 root         (0) root         (0)      498 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/test/spark/SimpleTest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 06:07:38.000000 rondsspark-0.0.4.8/test/__init__.py
```

### Comparing `rondsspark-0.0.4.7/ronds_sdk/tools/utils.py` & `rondsspark-0.0.4.8/ronds_sdk/tools/utils.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.7/ronds_sdk/pipeline.py` & `rondsspark-0.0.4.8/ronds_sdk/pipeline.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.7/ronds_sdk/transforms/spark/transforms.py` & `rondsspark-0.0.4.8/ronds_sdk/transforms/spark/transforms.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.7/ronds_sdk/transforms/remote_debug.py` & `rondsspark-0.0.4.8/ronds_sdk/transforms/remote_debug.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.7/ronds_sdk/transforms/pandas/cassandra_rule.py` & `rondsspark-0.0.4.8/ronds_sdk/transforms/pandas/cassandra_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,37 +105,38 @@
             start_datetime.strftime(RuleParser.datetime_format()),
             end_datetime_str))
 
         # process rules
         result_list = list()
         for rule in rules:
             uid_list = self.get_point_id_list(rule)
-            device_id = rule.assetId
             logging.info("uid_list size: %s" % len(uid_list))
             if len(uid_list) == 0:
                 continue
             result_set = process_manager.window_select(uid_list, start_datetime, end_datetime)
-            rule_data = self.transform_to_rule_data_pd(result_set, device_id)
+            rule_data = self.transform_to_rule_data_pd(result_set, rule)
             if rule_data is not None:
                 result_list.append(rule_data)
             del result_set
         p_dataframe = pd.DataFrame(result_list)
         action_func.call(df=p_dataframe, epoch_id=end_datetime_str)
 
         # update end_datetime
         end_datetime_holder.update(end_datetime + delta)
 
     @staticmethod
-    def transform_to_rule_data_pd(process_result_set: ResultSet, device_id: str) -> dict:
+    def transform_to_rule_data_pd(process_result_set: ResultSet, rule: dict) -> dict:
         rule_data = None
+        device_id = rule.assetId
+        rule_ids = rule.rules
         for r in process_result_set:
             if r.time is None or r.value is None:
                 continue
             if rule_data is None:
-                rule_data = RuleData(device_id)
+                rule_data = RuleData(device_id, rule_ids)
             rule_data.add_process_data(str(r.id),
                                        r.time.strftime(RuleParser.datetime_format()),
                                        r.value)
         return rule_data.get_data() if rule_data is not None else None
 
     @lru_cache(maxsize=100)
     def scan_cassandra(self,
```

### Comparing `rondsspark-0.0.4.7/ronds_sdk/transforms/pandas/transforms.py` & `rondsspark-0.0.4.8/ronds_sdk/transforms/pandas/transforms.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.7/ronds_sdk/transforms/pandas/rule_merge_data.py` & `rondsspark-0.0.4.8/ronds_sdk/transforms/pandas/rule_merge_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 
 
 # noinspection SpellCheckingInspection
 class RuleData(object):
 
     def __init__(self,
                  device_id,  # type: str
+                 rule_ids,  # type: list[str]
                  nodes=None,  # type: list
                  edges=None,  # type: list
                  datasources=None,  # type: list
                  indices=None,  # type: list
                  events=None,  # type: list
                  running_time=None,  # type: float
                  datasource_times=None,  # type: str
+
                  ):
         """
         根据规则读取 Cassandra 数据, 组合成算法能够识别的 JSON 格式数据
         :param nodes: 设备 DAG nodes
         :param edges: 设备 DAG edges
         :param datasources: 数据源的具体数据
         :param indices: 需要存储到 Cassandra 的数据
@@ -29,15 +31,16 @@
             'nodes': nodes if nodes else [],
             'edges': edges if edges else [],
             'datasource': datasources if datasources else [[]],
             'version': '1.0.0',
             'indices': indices if indices else [],
             'events': events if events else [],
             'runningtime': running_time if running_time else [],
-            'datasourcetimes': [datasource_times] if datasource_times else []
+            'datasourcetimes': [datasource_times] if datasource_times else [],
+            'rules': rule_ids,
         }
         self._data_index = dict()
 
     def get_data(self) -> dict:
         return self._data_dict
 
     def get_datasource(self) -> list:
```

### Comparing `rondsspark-0.0.4.7/ronds_sdk/transforms/ronds.py` & `rondsspark-0.0.4.8/ronds_sdk/transforms/ronds.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.7/ronds_sdk/transforms/ptransform.py` & `rondsspark-0.0.4.8/ronds_sdk/transforms/ptransform.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.7/ronds_sdk/__init__.py` & `rondsspark-0.0.4.8/ronds_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.7/ronds_sdk/runners/visitors/spark_runner_visitor.py` & `rondsspark-0.0.4.8/ronds_sdk/runners/visitors/spark_runner_visitor.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.7/ronds_sdk/runners/runner.py` & `rondsspark-0.0.4.8/ronds_sdk/runners/runner.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.7/ronds_sdk/runners/python_runner.py` & `rondsspark-0.0.4.8/ronds_sdk/runners/python_runner.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.7/ronds_sdk/runners/spark_runner.py` & `rondsspark-0.0.4.8/ronds_sdk/runners/spark_runner.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.7/ronds_sdk/templates/phm_rules_editor.py` & `rondsspark-0.0.4.8/ronds_sdk/templates/phm_rules_editor.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.7/ronds_sdk/dataframe/pvalue.py` & `rondsspark-0.0.4.8/ronds_sdk/dataframe/pvalue.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.7/ronds_sdk/options/value_provider.py` & `rondsspark-0.0.4.8/ronds_sdk/options/value_provider.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.7/ronds_sdk/options/pipeline_options.py` & `rondsspark-0.0.4.8/ronds_sdk/options/pipeline_options.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.7/ronds_sdk/datasources/cassandra_manager.py` & `rondsspark-0.0.4.8/ronds_sdk/datasources/cassandra_manager.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.7/ronds_sdk/datasources/kafka_manager.py` & `rondsspark-0.0.4.8/ronds_sdk/datasources/kafka_manager.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.7/ronds_sdk/error.py` & `rondsspark-0.0.4.8/ronds_sdk/error.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.7/rondsspark.egg-info/SOURCES.txt` & `rondsspark-0.0.4.8/rondsspark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.7/test/sdk/sdk_test.py` & `rondsspark-0.0.4.8/test/sdk/sdk_test.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.7/test/sdk/sdk_unitest.py` & `rondsspark-0.0.4.8/test/sdk/sdk_unitest.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.7/test/simple/overloading_test.py` & `rondsspark-0.0.4.8/test/simple/overloading_test.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.7/test/spark/SparkTest.py` & `rondsspark-0.0.4.8/test/spark/SparkTest.py`

 * *Files identical despite different names*

