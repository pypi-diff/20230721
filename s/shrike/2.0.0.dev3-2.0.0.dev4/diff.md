# Comparing `tmp/shrike-2.0.0.dev3.tar.gz` & `tmp/shrike-2.0.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shrike-2.0.0.dev3.tar", last modified: Mon Jul 17 23:32:09 2023, max compression
+gzip compressed data, was "shrike-2.0.0.dev4.tar", last modified: Fri Jul 21 02:17:37 2023, max compression
```

## Comparing `shrike-2.0.0.dev3.tar` & `shrike-2.0.0.dev4.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.928048 shrike-2.0.0.dev3/
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)   252717 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     8629 2023-07-17 23:32:09.928048 shrike-2.0.0.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6977 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-17 23:32:09.928048 shrike-2.0.0.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2318 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.920048 shrike-2.0.0.dev3/shrike/
--rw-r--r--   0 runner    (1001) docker     (122)      399 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.920048 shrike-2.0.0.dev3/shrike/_core/
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4102 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/_core/eyesoff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/_core/testing.py
--rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.920048 shrike-2.0.0.dev3/shrike/build/
--rw-r--r--   0 runner    (1001) docker     (122)      427 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.920048 shrike-2.0.0.dev3/shrike/build/commands/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/build/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    60232 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/build/commands/prepare.py
--rw-r--r--   0 runner    (1001) docker     (122)     7756 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/build/commands/register.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.920048 shrike-2.0.0.dev3/shrike/build/core/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/build/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14964 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/build/core/command_line.py
--rw-r--r--   0 runner    (1001) docker     (122)     8463 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/build/core/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.920048 shrike-2.0.0.dev3/shrike/build/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/build/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5526 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/build/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.920048 shrike-2.0.0.dev3/shrike/compliant_logging/
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/compliant_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6036 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/compliant_logging/argparser_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/compliant_logging/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    10327 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/compliant_logging/data_conversions.py
--rw-r--r--   0 runner    (1001) docker     (122)    16169 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/compliant_logging/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    41145 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/compliant_logging/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)    10311 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/compliant_logging/progress.py
--rw-r--r--   0 runner    (1001) docker     (122)     4875 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/compliant_logging/stack_trace_extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/compliant_logging/system_info.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.924048 shrike-2.0.0.dev3/shrike/distributed/
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9037 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/distributed/cluster_auto_setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     9829 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/distributed/dask.py
--rw-r--r--   0 runner    (1001) docker     (122)     4130 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/distributed/mpi_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)     5414 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/distributed/ray.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.924048 shrike-2.0.0.dev3/shrike/pipeline/
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/aml_connect.py
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/argparser_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7223 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/canary_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.916048 shrike-2.0.0.dev3/shrike/pipeline/components/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.924048 shrike-2.0.0.dev3/shrike/pipeline/components/fedavg/
--rw-r--r--   0 runner    (1001) docker     (122)      127 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/components/fedavg/env.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/components/fedavg/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     3131 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/components/fedavg/spec.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    35499 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/federated_learning.py
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/module_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    20048 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/module_helper_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    16294 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/pipeline_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/pipeline_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    42859 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/pipeline_helper_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/ray_actor.py
--rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/telemetry_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.924048 shrike-2.0.0.dev3/shrike/pipeline/testing/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24460 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/testing/components.py
--rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/testing/importer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1837 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/testing/module_run_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     7894 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/testing/pipeline_class_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     7520 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/testing/pipeline_class_test_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.924048 shrike-2.0.0.dev3/shrike/pipeline/v1/
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5039 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/v1/aml_connect.py
--rw-r--r--   0 runner    (1001) docker     (122)     3565 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/v1/module_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    75640 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/v1/pipeline_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.928048 shrike-2.0.0.dev3/shrike/pipeline/v2/
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/v2/aml_connect.py
--rw-r--r--   0 runner    (1001) docker     (122)     3839 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/v2/module_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    67952 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/v2/pipeline_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.928048 shrike-2.0.0.dev3/shrike/spark/
--rw-r--r--   0 runner    (1001) docker     (122)      187 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5221 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/spark/spark_net.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.920048 shrike-2.0.0.dev3/shrike.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8629 2023-07-17 23:32:09.000000 shrike-2.0.0.dev3/shrike.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-07-17 23:32:09.000000 shrike-2.0.0.dev3/shrike.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 23:32:09.000000 shrike-2.0.0.dev3/shrike.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1280 2023-07-17 23:32:09.000000 shrike-2.0.0.dev3/shrike.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-17 23:32:09.000000 shrike-2.0.0.dev3/shrike.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.746986 shrike-2.0.0.dev4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)   252717 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8629 2023-07-21 02:17:37.746986 shrike-2.0.0.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6977 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-21 02:17:37.746986 shrike-2.0.0.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2318 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.738986 shrike-2.0.0.dev4/shrike/
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.738986 shrike-2.0.0.dev4/shrike/_core/
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4102 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/_core/eyesoff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/_core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.738986 shrike-2.0.0.dev4/shrike/build/
+-rw-r--r--   0 runner    (1001) docker     (122)      427 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.738986 shrike-2.0.0.dev4/shrike/build/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/build/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    60232 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/build/commands/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7756 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/build/commands/register.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.738986 shrike-2.0.0.dev4/shrike/build/core/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/build/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14964 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/build/core/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8463 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/build/core/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.742987 shrike-2.0.0.dev4/shrike/build/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/build/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5526 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/build/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.742987 shrike-2.0.0.dev4/shrike/compliant_logging/
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/compliant_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6036 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/compliant_logging/argparser_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/compliant_logging/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10327 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/compliant_logging/data_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16169 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/compliant_logging/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41145 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/compliant_logging/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10311 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/compliant_logging/progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4875 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/compliant_logging/stack_trace_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/compliant_logging/system_info.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.742987 shrike-2.0.0.dev4/shrike/distributed/
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9037 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/distributed/cluster_auto_setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9829 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/distributed/dask.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4130 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/distributed/mpi_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5414 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/distributed/ray.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.742987 shrike-2.0.0.dev4/shrike/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/aml_connect.py
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/argparser_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7223 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/canary_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.734986 shrike-2.0.0.dev4/shrike/pipeline/components/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.742987 shrike-2.0.0.dev4/shrike/pipeline/components/fedavg/
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/components/fedavg/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/components/fedavg/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3131 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/components/fedavg/spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    38725 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/federated_learning.py
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/module_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20048 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/module_helper_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20768 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/pipeline_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/pipeline_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42859 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/pipeline_helper_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/ray_actor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/telemetry_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.746986 shrike-2.0.0.dev4/shrike/pipeline/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24460 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/testing/components.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/testing/importer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1837 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/testing/module_run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7894 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/testing/pipeline_class_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7520 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/testing/pipeline_class_test_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.746986 shrike-2.0.0.dev4/shrike/pipeline/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5039 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/v1/aml_connect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3565 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/v1/module_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    75663 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/v1/pipeline_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.746986 shrike-2.0.0.dev4/shrike/pipeline/v2/
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/v2/aml_connect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3839 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/v2/module_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    67952 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/v2/pipeline_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.746986 shrike-2.0.0.dev4/shrike/spark/
+-rw-r--r--   0 runner    (1001) docker     (122)      187 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5221 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/spark/spark_net.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.738986 shrike-2.0.0.dev4/shrike.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8629 2023-07-21 02:17:37.000000 shrike-2.0.0.dev4/shrike.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-07-21 02:17:37.000000 shrike-2.0.0.dev4/shrike.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 02:17:37.000000 shrike-2.0.0.dev4/shrike.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1280 2023-07-21 02:17:37.000000 shrike-2.0.0.dev4/shrike.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-21 02:17:37.000000 shrike-2.0.0.dev4/shrike.egg-info/top_level.txt
```

### Comparing `shrike-2.0.0.dev3/LICENSE` & `shrike-2.0.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/NOTICE.txt` & `shrike-2.0.0.dev4/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/PKG-INFO` & `shrike-2.0.0.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shrike
-Version: 2.0.0.dev3
+Version: 2.0.0.dev4
 Summary: Python utilities for compliant Azure machine learning
 Home-page: https://github.com/ai-platform-ml-platform/shrike
 Author: AML Data Science
 Author-email: aml-ds@microsoft.com
 License: MIT
 Description: # Shrike: incubation for Azure ML
```

### Comparing `shrike-2.0.0.dev3/README.md` & `shrike-2.0.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/setup.py` & `shrike-2.0.0.dev4/setup.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/_core/eyesoff.py` & `shrike-2.0.0.dev4/shrike/_core/eyesoff.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/_core/testing.py` & `shrike-2.0.0.dev4/shrike/_core/testing.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/_core/utils.py` & `shrike-2.0.0.dev4/shrike/_core/utils.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/build/commands/prepare.py` & `shrike-2.0.0.dev4/shrike/build/commands/prepare.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/build/commands/register.py` & `shrike-2.0.0.dev4/shrike/build/commands/register.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/build/core/command_line.py` & `shrike-2.0.0.dev4/shrike/build/core/command_line.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/build/core/configuration.py` & `shrike-2.0.0.dev4/shrike/build/core/configuration.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/build/utils/utils.py` & `shrike-2.0.0.dev4/shrike/build/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/compliant_logging/__init__.py` & `shrike-2.0.0.dev4/shrike/compliant_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/compliant_logging/argparser_utils.py` & `shrike-2.0.0.dev4/shrike/compliant_logging/argparser_utils.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/compliant_logging/data_conversions.py` & `shrike-2.0.0.dev4/shrike/compliant_logging/data_conversions.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/compliant_logging/exceptions.py` & `shrike-2.0.0.dev4/shrike/compliant_logging/exceptions.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/compliant_logging/logging.py` & `shrike-2.0.0.dev4/shrike/compliant_logging/logging.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/compliant_logging/progress.py` & `shrike-2.0.0.dev4/shrike/compliant_logging/progress.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/compliant_logging/stack_trace_extractor.py` & `shrike-2.0.0.dev4/shrike/compliant_logging/stack_trace_extractor.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/compliant_logging/system_info.py` & `shrike-2.0.0.dev4/shrike/compliant_logging/system_info.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/distributed/cluster_auto_setup.py` & `shrike-2.0.0.dev4/shrike/distributed/cluster_auto_setup.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/distributed/dask.py` & `shrike-2.0.0.dev4/shrike/distributed/dask.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/distributed/mpi_driver.py` & `shrike-2.0.0.dev4/shrike/distributed/mpi_driver.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/distributed/ray.py` & `shrike-2.0.0.dev4/shrike/distributed/ray.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/pipeline/__init__.py` & `shrike-2.0.0.dev4/shrike/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/pipeline/canary_helper.py` & `shrike-2.0.0.dev4/shrike/pipeline/canary_helper.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/pipeline/components/fedavg/run.py` & `shrike-2.0.0.dev4/shrike/pipeline/components/fedavg/run.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/pipeline/components/fedavg/spec.yaml` & `shrike-2.0.0.dev4/shrike/pipeline/components/fedavg/spec.yaml`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/pipeline/federated_learning.py` & `shrike-2.0.0.dev4/shrike/pipeline/federated_learning.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,20 @@
             self.module_loader.modules_manifest, {"fl_fedavg_pytorch": fedavg_component}
         )
         self.cur_fl_iteration: Optional[int] = None
         self.output_prefix = "fl_output_"
         self.orchestrator = self.config.federated_config.silos[
             self.config.federated_config.orchestrator
         ]
+        if "datastore" not in self.orchestrator or not self.orchestrator.datastore:
+            self.orchestrator.datastore = self._get_uw_datastores(
+                location=self.orchestrator.location,
+                environment=self.orchestrator.environment,
+                dc=False,
+            )
 
     @experimental(message=EXPERIMENTAL_WARNING_MSG)
     def create_base_name(self) -> str:
         """The training outputs from each silo will be stored at <base_name>/<silo_name> on the central storage.
         By default, it will return a name of 2 word. User can override this method.
 
         Returns:
@@ -197,22 +203,34 @@
         silo training step and generate_noise step, and generate the outputs that would be transferred to downstream midprocess pipeline for model weights aggregation.
 
         Returns:
             a component/subgraph instance, and a list of output dataset names to be passed to the downstream pipeline.
         """
         pass
 
+    @experimental(message=EXPERIMENTAL_WARNING_MSG)
+    def outbound_data_transfer(self, input: Output = None, **kwargs) -> StepOutput:
+        """
+        Optional user-defined data transfer step to move data outside the compliant boundary.
+        If subgraph auto-approval template is registered for the workspace, define and consume it here.
+
+        Returns:
+            a component/subgraph instance, and a list of output dataset names to be passed to the downstream pipeline.
+        """
+        raise NotImplementedError
+
     def _data_transfer(
         self,
         input_list: dict,
         base_name: str,
         destination_datastore: str = None,
         location: str = None,
         environment: str = None,
         via_cosmos: bool = False,
+        orchestrator_to_silo: bool = True,
     ) -> dict:
         """Moves data `input_list` to `destination_datastore` with path prefixed by `base_name`."""
         # assume one shared ADF
         dts_name = self.config.federated_config.data_transfer_component
         try:
             data_transfer_component = self.component_load(
                 dts_name  # this component is subject to change
@@ -231,36 +249,53 @@
             if via_cosmos:
                 log.info("Leveraging cosmos as the intermediate datastore.")
 
                 @dsl.pipeline(
                     display_name=f"Data transfer to {location}-{environment} via cosmos"
                 )
                 def dts_via_cosmos_function(input):
-                    data_transfer_to_cosmos_step = data_transfer_component(
-                        source_data=input
-                    )
-                    self.apply_smart_runsettings(
-                        data_transfer_to_cosmos_step,
-                        datatransfer=True,
-                        datastore_name=self.config.compute.noncompliant_datastore,
-                        location=location,
-                        environment=environment,
-                    )
+                    data_in_noncompliant_datastore = None
+                    try:
+                        data_in_noncompliant_datastore = self.outbound_data_transfer(
+                            input
+                        )
+                    except NotImplementedError:
+                        data_transfer_to_cosmos_step = data_transfer_component(
+                            source_data=input
+                        )
+                        self.apply_smart_runsettings(
+                            data_transfer_to_cosmos_step,
+                            datatransfer=True,
+                            datastore_name=self.config.compute.noncompliant_datastore,
+                            location=self.orchestrator.location
+                            if orchestrator_to_silo
+                            else location,
+                            environment=self.orchestrator.environment
+                            if orchestrator_to_silo
+                            else environment,
+                        )
+                        data_in_noncompliant_datastore = (
+                            data_transfer_to_cosmos_step.outputs.destination_data
+                        )
                     data_transfer_from_cosmos_step = data_transfer_component(
-                        source_data=data_transfer_to_cosmos_step.outputs.destination_data
+                        source_data=data_in_noncompliant_datastore,
                     )
                     data_transfer_from_cosmos_step.outputs.destination_data.configure(
                         path_on_datastore=base_name + "/" + name,
                     )
                     self.apply_smart_runsettings(
                         data_transfer_from_cosmos_step,
                         datatransfer=True,
                         datastore_name=destination_datastore,
-                        location=location,
-                        environment=environment,
+                        location=location
+                        if orchestrator_to_silo
+                        else self.orchestrator.location,
+                        environment=environment
+                        if orchestrator_to_silo
+                        else self.orchestrator.environment,
                     )
                     return {
                         "output_data": data_transfer_from_cosmos_step.outputs.destination_data
                     }
 
                 dts_via_cosmos = dts_via_cosmos_function(input)
                 res[name] = dts_via_cosmos.outputs.output_data
@@ -269,16 +304,20 @@
                 data_transfer_step.outputs.destination_data.configure(
                     path_on_datastore=base_name + "/" + name,
                 )
                 self.apply_smart_runsettings(
                     data_transfer_step,
                     datatransfer=True,
                     datastore_name=destination_datastore,
-                    location=location,
-                    environment=environment,
+                    location=self.orchestrator.location
+                    if orchestrator_to_silo
+                    else location,
+                    environment=self.orchestrator.environment
+                    if orchestrator_to_silo
+                    else environment,
                 )
                 res[name] = data_transfer_step.outputs.destination_data
         return res
 
     def _update_nested_dict_with_non_none_values(self, dict1, dict2):
         """Update dict1 with non-none values in dict2"""
         for k, v in dict2.items():
@@ -324,25 +363,29 @@
         log.info(f"Checking user override runsettings for {step.name}...")
         output_configs = self._get_user_defined_output_configs(step)
 
         runsettings = step.runsettings._get_values()
         self.apply_smart_runsettings(
             step,
             target=orchestrator_or_silo.compute,
-            datastore_name=orchestrator_or_silo.datastore,  # TODO: verify if this is correct
+            datastore_name=orchestrator_or_silo.datastore,
             location=orchestrator_or_silo.location,
             environment=orchestrator_or_silo.environment,
         )
         merged_runsettings = self._update_nested_dict_with_non_none_values(
             step.runsettings._get_values(), runsettings
         )
         step.runsettings._set_section_by_dict(merged_runsettings)
         prev_output = self._apply_user_defined_output_configs(
             prev_output, output_configs
         )
+        unused_outputs = {
+            k: step.outputs[k] for k in set(step.outputs) - set(prev_output)
+        }
+        self._apply_user_defined_output_configs(unused_outputs, output_configs)
         return prev_output
 
     def _process_at_orchestrator(self, prev: StepOutput) -> dict:
         """Processes outputs at the orchestrator."""
         step = prev.step
         if isinstance(step, Pipeline):
             prev_output = step.outputs
@@ -381,80 +424,94 @@
                 merge = OmegaConf.merge(default_config, customized_config)
             log.info(f"=== Shared config {merge}")
             with open_dict(self.config.federated_config.silos[silo_name]):
                 self.config.federated_config.silos[silo_name] = OmegaConf.merge(
                     merge, silo_config
                 )
                 self.config.federated_config.silos[silo_name].pop("inherit", None)
+            if "location" not in self.config.federated_config.silos[silo_name]:
+                self.config.federated_config.silos[silo_name].location = ""
+            if "environment" not in self.config.federated_config.silos[silo_name]:
+                self.config.federated_config.silos[silo_name].environment = ""
             log.info(
                 f"=== Merged config for silo {silo_name}: {self.config.federated_config.silos[silo_name]}"
             )
         self.orchestrator = self.config.federated_config.silos[
             self.config.federated_config.orchestrator
         ]
 
     def _check_if_same_source_and_destination_datastore(
-        self, input, destination_datastore=None, location=None, environment=None
+        self,
+        input,
+        destination_datastore=None,
+        destination_location=None,
+        destination_environment=None,
     ):
         # Check if the input data already lives in the destination datastore.
         # If source = DC datastore, destination = PROD datastore in the same region,
         # this function returns False. This can be improved but might overcomplicate the code.
         source_datastore = (
             input.default_value._datastore
             if isinstance(input, PipelineParameter)
             else input._datastore
         )
-        for item in self.config.uw_config.datastores:
-            if item["name"] == source_datastore:
-                source_location = item["location"]
-                source_environment = item["environment"]
-            if (
-                not location
-                and not environment
-                and item["name"] == destination_datastore
-            ):
-                location = item["location"]
-                environment = item["environment"]
-        return location == source_location and environment == source_environment
+        if source_datastore == destination_datastore:
+            return True
+        elif "uw_config" not in self.config:
+            return False
+        else:
+            for item in self.config.uw_config.datastores:
+                if item["name"] == source_datastore:
+                    source_location = item["location"]
+                    source_environment = item["environment"]
+                if destination_datastore and item["name"] == destination_datastore:
+                    destination_location = item["location"]
+                    destination_environment = item["environment"]
+            return (
+                destination_location == source_location
+                and destination_environment == source_environment
+            )
 
     def _check_if_data_transfer_is_activated_and_process(
         self,
         base_name,
         datastore_name=None,
         location=None,
         environment=None,
         via_cosmos=True,
+        orchestrator_to_silo=True,
         **inputs,
     ):
         deactivate_data_transfer = self.config.federated_config.deactivate_data_transfer
         if deactivate_data_transfer:
             log.info("Data transfer is disabled; training outputs will remain in silo.")
             return inputs
         else:
+            for input_key, input_value in inputs.items():
+                pass
+            if self._check_if_same_source_and_destination_datastore(
+                input_value, datastore_name, location, environment
+            ):
+                # TODO: this simplifies the graph by removing redundant DTS. Do we need it?
+                log.info("Trying to move data within the silo, skipping..")
+                return inputs
             if datastore_name:
                 log.info(f"Moving data {inputs.keys()} into {datastore_name}.")
             else:
-                for input_key, input_value in inputs.items():
-                    pass
-                if self._check_if_same_source_and_destination_datastore(
-                    input_value, datastore_name, location, environment
-                ):
-                    # TODO: this simplifies the graph by removing redundant DTS. Do we need it?
-                    log.info("Trying to move data within the silo, skipping..")
-                    return inputs
                 log.info(
                     f"Moving data {inputs.keys()} into {environment} in {location}."
                 )
             return self._data_transfer(
                 input_list=inputs,
                 base_name=base_name,
                 destination_datastore=datastore_name,
                 location=location,
                 environment=environment,
                 via_cosmos=via_cosmos,
+                orchestrator_to_silo=orchestrator_to_silo,
             )
 
     def _update_configs_in_silo(self, step, compute_target, datastore):
         log.info(
             f"Updating the compute target to {compute_target} and datastore to {datastore} for component {step.name}."
         )
         step.runsettings.configure(
@@ -462,21 +519,23 @@
         )
         self._set_all_outputs_to(step, output_mode=None, datastore_name=datastore)
 
     def _train_in_silo_once(
         self, silo_name: str, silo: DictConfig, cool_name: str, **prev_output
     ) -> dict:
         """Runs the "training" step once at one silo."""
-        prev_output = self._check_if_data_transfer_is_activated_and_process(
-            base_name=cool_name,
-            datastore_name=silo.datastore,
-            location=silo.location,
-            environment=silo.environment,
-            **prev_output,
-        )
+        if prev_output:
+            prev_output = self._check_if_data_transfer_is_activated_and_process(
+                base_name=cool_name,
+                datastore_name=silo.datastore,
+                location=silo.location,
+                environment=silo.environment,
+                orchestrator_to_silo=True,
+                **prev_output,
+            )
         if len(prev_output) == 1:
             prev_output = {"input": list(prev_output.values())[0]}
         train_step = self.train(self.config, silo=silo, **prev_output)
 
         step = train_step.step
         if isinstance(step, Pipeline):
             train_output = step.outputs
@@ -502,16 +561,18 @@
                 f"The output of train step must be a Pipeline object or a Component object. You are using {type(step)}"
             )
 
         # If users are not using secure aggregation, transfer raw model weight from silo to cenral server directly
         if not self.config.federated_config.use_secure_aggregation:
             silo_output = self._check_if_data_transfer_is_activated_and_process(
                 base_name=cool_name + "/" + silo_name,
-                location=self.orchestrator.location,
-                environment=self.orchestrator.environment,
+                datastore_name=self.orchestrator.datastore,
+                location=silo.location,
+                environment=silo.environment,
+                orchestrator_to_silo=False,
                 **train_output,
             )
         # Otherwise, keep the raw model weights output as input (without data_transfer) to downstream anonymize-weights step
         else:
             silo_output = train_output
         return silo_output
 
@@ -520,14 +581,15 @@
     ) -> dict:
         """Runs the "generate_noise" step once at one silo."""
         prev_output = self._check_if_data_transfer_is_activated_and_process(
             base_name=cool_name,
             datastore_name=silo.datastore,
             location=silo.location,
             environment=silo.environment,
+            orchestrator_to_silo=True,
             **prev_output,
         )
         if len(prev_output) == 1:
             prev_output = {"input": list(prev_output.values())[0]}
         generate_noise_step = self.generate_noise(self.config, silo=silo, **prev_output)
 
         step = generate_noise_step.step
@@ -578,16 +640,18 @@
         else:
             raise Exception(
                 f"The output of anonymize_model_weights step must be a Pipeline object or a Component object. You are using {type(step)}"
             )
 
         silo_output = self._check_if_data_transfer_is_activated_and_process(
             base_name=cool_name + "/" + silo_name,
-            location=self.orchestrator.location,
-            environment=self.orchestrator.environment,
+            datastore_name=self.orchestrator.datastore,
+            location=silo.location,
+            environment=silo.environment,
+            orchestrator_to_silo=False,
             **anonymize_model_weights_output,
         )
         return silo_output
 
     @experimental(message=EXPERIMENTAL_WARNING_MSG)
     def build(self, config: DictConfig):
         """Constructs the federated pipeline. User does not need to modify."""
@@ -682,14 +746,15 @@
                                     ] = 1
                             generate_noise_output_transferred_to_target_silo = (
                                 self._check_if_data_transfer_is_activated_and_process(
                                     base_name=cool_name + "/" + target_silo_name,
                                     datastore_name=target_silo.datastore,
                                     location=target_silo.location,
                                     environment=target_silo.environment,
+                                    orchestrator_to_silo=True,
                                     **generate_noise_output,
                                 )
                             )
                             if (
                                 len(generate_noise_output_transferred_to_target_silo)
                                 == 1
                             ):
@@ -770,15 +835,18 @@
             }
             return output
 
         @dsl.pipeline()
         def pipeline_function():
             self._merge_config()
             prev = self.preprocess(self.config)
-            prev_output = self._process_at_orchestrator(prev)
+            if prev:
+                prev_output = self._process_at_orchestrator(prev)
+            else:
+                prev_output = None
             assert isinstance(self.config.federated_config.use_secure_aggregation, bool)
 
             for iter in range(self.config.federated_config.max_iterations):
                 self.cur_fl_iteration = iter
                 if prev_output:
                     prev_output = {
                         output_name.replace(self.output_prefix, ""): prev_output[
@@ -793,16 +861,17 @@
                     subpipeline = _subpipeline_function()
                 subpipeline.node_name = self.create_iteration_name()
                 prev_output = subpipeline.outputs
 
             if len(prev_output) == 1:
                 prev_output = {"input": list(prev_output.values())[0]}
             prev = self.postprocess(self.config, **prev_output)
-            output = self._process_at_orchestrator(prev)
-            return output
+            if prev:
+                prev = self._process_at_orchestrator(prev)
+            return prev
 
         return pipeline_function
 
     def pipeline_instance(self, pipeline_function, config):
         """Creates an instance of the pipeline using arguments. User does not need to modify."""
         pipeline = pipeline_function()
         return pipeline
```

### Comparing `shrike-2.0.0.dev3/shrike/pipeline/module_helper_base.py` & `shrike-2.0.0.dev4/shrike/pipeline/module_helper_base.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/pipeline/pipeline_config.py` & `shrike-2.0.0.dev4/shrike/pipeline/pipeline_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -206,14 +206,16 @@
     Silo info for federated learning
 
     Parameters:
     - `compute` (str): the compute target for this silo
     - `datastore` (str): the datastore for this silo
     - `params` (Optional[Dict[str, Any]]): additional parameters relevant to the job that will run in the silo, such as `dataset`, etc...
     - `inherit` (Optional[List[str]]): list of `config_group`s to apply to this silo, and the override priority is per-silo config > `inherit` > `default_config`
+    - `location` (Optional[str]): location of the silo sandbox, required for unified workspace
+    - `environment` (Optional[str]): environment type of the silo sandbox, required for unified workspace. Acceptable values include "msit", "dnd", "mdp", and "cloverport"
     """
 
     compute: Optional[str] = None
     datastore: Optional[str] = None
     params: Optional[Dict[str, Any]] = MISSING
     inherit: Optional[List[str]] = MISSING
     location: Optional[str] = MISSING
@@ -246,40 +248,92 @@
     use_secure_aggregation: bool = False
 
 
 @dataclass
 class compute_config:
     """
     AML compute and info
+
+    Parameters:
+    - `name` (str): name of compute target.
+    - `os` (str): os of CPU/GPU compute target, "linux" or "windows".
+    - `DC` (bool): whether the compute target is detonation or not.
+    - `gpu` (bool): whether the compute target is GPU or not.
+    - `location` (str): location of the child `silo` where the compute target belongs, defined by user and used to identify `silo`.
+        The location should be the same for all computes from one child workspace; for example,
+    you may use "europe" while the GPU and CPU might be provisioned in "westeurope" and "northeurope", respectively.
+    - `environment` (str): environment type of the compute target belongs, defined by user and used to identify `silo`.
     """
 
     name: str = MISSING
-    os: str = MISSING
+    os: str = "linux"
     DC: bool = field(default=False)
     gpu: bool = field(default=False)
     location: str = MISSING
     type: str = "amlcompute"
     environment: str = MISSING
     # TODO: what should be default values?
 
 
 @dataclass
 class datastore_config:
     """
     AML datastore and info
+
+    Parameters:
+    - `name` (str): name of datastore
+    - `DC` (bool): whether the datastore is detonation or not
+    - `location` (str): location of the child `silo` where the datastore belongs, defined by user and used to identify `silo`.
+    - `environment` (str): environment type of the child `silo` where the datastore belongs, defined by user and used to identify `silo`.
     """
 
     name: str = MISSING
     DC: Optional[bool] = False
     location: str = MISSING
     environment: str = MISSING
 
 
 @dataclass
 class uw_compute_config:
+    """
+    Unified AML workspace compute targets and I/O modes
+
+    Parameters:
+    - `default_compute_target` (str): name of default compute target to use if not specified
+    - `default_datastore` (str): name of default datastore to use if not specified
+    - `computes (List)`: list of `compute_config`
+    - `datastores (List)`: list of `datastore_config`
+    - `linux_input_mode` (str): input mode for linux compute targets (default to "mount"), more details at https://componentsdk.azurewebsites.net/concepts/inputs-and-outputs.html#input-dataset-mode
+    - `linux_output_mode` (str): output mode for linux compute targets (default to "mount"), more details at https://componentsdk.azurewebsites.net/concepts/inputs-and-outputs.html#output-dataset-mode
+    - `windows_input_mode` (str): input mode for windows compute targets (default to "download"), more details at https://componentsdk.azurewebsites.net/concepts/inputs-and-outputs.html#input-dataset-mode
+    - `windows_output_mode` (str): output mode for windows compute targets (default to "upload"), more details at https://componentsdk.azurewebsites.net/concepts/inputs-and-outputs.html#output-dataset-mode
+    - `hdi_driver_memory` (str): HDI driver memory in GB (default to "4g")
+    - `hdi_driver_cores` (int): number of HDI driver cores (default to 2)
+    - `hdi_executor_memory` (str): HDI executor memory in GB (default to "3g")
+    - `hdi_executor_cores` (int): number of HDI executor cores (default to 2)
+    - `hdi_number_executors` (int): number of HDI executors (default to 1)
+    - `hdi_conf` (Optional[Any]): additional HDI parameters
+    - `synapse_driver_memory` (Optional[str]): Synapse driver memory in GB
+    - `synapse_driver_cores` (Optional[int]): number of Synapse driver cores
+    - `synapse_executor_memory` (Optional[str]): Synapse executor memory in GB
+    - `synapse_executor_cores` (Optional[int]): number of Synapse executor cores
+    - `synapse_number_executors` (Optional[int]): number of Synapse executors
+    - `synapse_conf` (Optional[Any]): additional Synapse parameters
+    - `parallel_node_count` (int): number of nodes for parallel steps (default to 10)
+    - `parallel_process_count_per_node` (Optional[int]): deprecated. Please use `parallel_process_count_per_instance`
+    - `parallel_process_count_per_instance` (Optional[int]): number of processes for each node for parallel steps
+    - `parallel_run_invocation_timeout` (int): threshold in seconds for parallel step invocations to timeout (default to 10800)
+    - `parallel_run_max_try` (int): maximum number of times to retry parallel step invocations (default to 3)
+    - `parallel_mini_batch_size` (int): mini batch size for parallel steps (default to 1)
+    - `parallel_error_threshold` (int): error threshold for parallel steps (default to -1)
+    - `compliant_datastore` (str): name of the default compliant datastore
+    - `noncompliant_datastore` (Optional[str]): name of the default non-compliant datastore
+    - `dc_datastore` (Optional[str]): name of the default datastore for HDI detonation chamber and downstream steps
+    """
+
     default_compute_target: str = MISSING
     default_datastore: str = MISSING
     computes: List[compute_config] = field(default_factory=list)
     datastores: List[datastore_config] = field(default_factory=list)
     noncompliant_datastore: Optional[str] = MISSING
 
     linux_input_mode: str = "mount"
```

### Comparing `shrike-2.0.0.dev3/shrike/pipeline/pipeline_helper_base.py` & `shrike-2.0.0.dev4/shrike/pipeline/pipeline_helper_base.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/pipeline/ray_actor.py` & `shrike-2.0.0.dev4/shrike/pipeline/ray_actor.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/pipeline/telemetry_utils.py` & `shrike-2.0.0.dev4/shrike/pipeline/telemetry_utils.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/pipeline/testing/components.py` & `shrike-2.0.0.dev4/shrike/pipeline/testing/components.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/pipeline/testing/importer.py` & `shrike-2.0.0.dev4/shrike/pipeline/testing/importer.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/pipeline/testing/module_run_tests.py` & `shrike-2.0.0.dev4/shrike/pipeline/testing/module_run_tests.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/pipeline/testing/pipeline_class_test.py` & `shrike-2.0.0.dev4/shrike/pipeline/testing/pipeline_class_test.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/pipeline/testing/pipeline_class_test_v2.py` & `shrike-2.0.0.dev4/shrike/pipeline/testing/pipeline_class_test_v2.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/pipeline/v1/aml_connect.py` & `shrike-2.0.0.dev4/shrike/pipeline/v1/aml_connect.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/pipeline/v1/module_helper.py` & `shrike-2.0.0.dev4/shrike/pipeline/v1/module_helper.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/pipeline/v1/pipeline_helper.py` & `shrike-2.0.0.dev4/shrike/pipeline/v1/pipeline_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,14 +223,15 @@
             return
 
         if environment:
             assert environment.lower() in [
                 "cloverport",
                 "msit",
                 "mdp",
+                "dnd",
             ]  # TODO: what else allowed?
 
             # Manually add env var because we can't identify the environment in a unified workspace based on subscription
             environment_variable = {
                 "EYESOFF_ENV": "false"
                 if environment.lower() == "cloverport"
                 else "true"
```

### Comparing `shrike-2.0.0.dev3/shrike/pipeline/v2/aml_connect.py` & `shrike-2.0.0.dev4/shrike/pipeline/v2/aml_connect.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/pipeline/v2/module_helper.py` & `shrike-2.0.0.dev4/shrike/pipeline/v2/module_helper.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/pipeline/v2/pipeline_helper.py` & `shrike-2.0.0.dev4/shrike/pipeline/v2/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike/spark/spark_net.py` & `shrike-2.0.0.dev4/shrike/spark/spark_net.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike.egg-info/PKG-INFO` & `shrike-2.0.0.dev4/shrike.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shrike
-Version: 2.0.0.dev3
+Version: 2.0.0.dev4
 Summary: Python utilities for compliant Azure machine learning
 Home-page: https://github.com/ai-platform-ml-platform/shrike
 Author: AML Data Science
 Author-email: aml-ds@microsoft.com
 License: MIT
 Description: # Shrike: incubation for Azure ML
```

### Comparing `shrike-2.0.0.dev3/shrike.egg-info/SOURCES.txt` & `shrike-2.0.0.dev4/shrike.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev3/shrike.egg-info/requires.txt` & `shrike-2.0.0.dev4/shrike.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 black==22.3.0
 flake8==3.9.1
 typeguard==2.11.1
 typing-extensions>=4.0
 markdown-include==0.6.0
 mkdocstrings-python-legacy==0.2.2
 mkdocstrings==0.18.1
-mkdocs-material==8.2.8
+mkdocs-material==9.1.8
 livereload==2.6.3
 markdown==3.3.7
 pytest~=6.2
 pytest-cov~=2.11
 pytest-order==0.10.0
 blake3==0.2.1
 twine~=3.3
```

