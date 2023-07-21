# Comparing `tmp/columnflow-0.2.1.tar.gz` & `tmp/columnflow-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "columnflow-0.2.1.tar", last modified: Thu Apr 13 08:49:16 2023, max compression
+gzip compressed data, was "columnflow-0.2.2.tar", last modified: Fri Jul 21 17:35:53 2023, max compression
```

## Comparing `columnflow-0.2.1.tar` & `columnflow-0.2.2.tar`

### file list

```diff
@@ -1,89 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.855717 columnflow-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 08:49:01.000000 columnflow-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-04-13 08:49:16.855717 columnflow-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-04-13 08:49:01.000000 columnflow-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.847717 columnflow-0.2.1/columnflow/
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.847717 columnflow-0.2.1/columnflow/calibration/
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/calibration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.847717 columnflow-0.2.1/columnflow/calibration/cms/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/calibration/cms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25110 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/calibration/cms/jets.py
--rw-r--r--   0 runner    (1001) docker     (123)    24321 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/calibration/cms/jets_coffea.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/calibration/cms/met.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/calibration/util.py
--rw-r--r--   0 runner    (1001) docker     (123)   110900 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/columnar_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9257 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/config_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.847717 columnflow-0.2.1/columnflow/inference/
--rw-r--r--   0 runner    (1001) docker     (123)    46440 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/inference/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.847717 columnflow-0.2.1/columnflow/inference/cms/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/inference/cms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22624 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/inference/cms/datacard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.847717 columnflow-0.2.1/columnflow/ml/
--rw-r--r--   0 runner    (1001) docker     (123)    14710 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.851717 columnflow-0.2.1/columnflow/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/plotting/plot_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/plotting/plot_functions_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/plotting/plot_functions_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/plotting/plot_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.851717 columnflow-0.2.1/columnflow/production/
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/categories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.851717 columnflow-0.2.1/columnflow/production/cms/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/cms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/cms/btag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/cms/electron.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/cms/gen_top_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/cms/mc_weight.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/cms/muon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/cms/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/cms/pileup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/cms/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/cms/seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/production/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.851717 columnflow-0.2.1/columnflow/selection/
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/selection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.851717 columnflow-0.2.1/columnflow/selection/cms/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/selection/cms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/selection/cms/json_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/selection/cms/met_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/selection/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.855717 columnflow-0.2.1/columnflow/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.855717 columnflow-0.2.1/columnflow/tasks/cms/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/cms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/cms/external.py
--rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/cms/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    24659 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/cutflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/external.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.855717 columnflow-0.2.1/columnflow/tasks/framework/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43500 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/framework/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/framework/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    45329 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/framework/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/framework/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/framework/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    25655 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/framework/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/histograms.py
--rw-r--r--   0 runner    (1001) docker     (123)    18059 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/production.py
--rw-r--r--   0 runner    (1001) docker     (123)    17233 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    14017 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/union.py
--rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/tasks/yields.py
--rw-r--r--   0 runner    (1001) docker     (123)    25276 2023-04-13 08:49:02.000000 columnflow-0.2.1/columnflow/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:49:16.847717 columnflow-0.2.1/columnflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-04-13 08:49:16.000000 columnflow-0.2.1/columnflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-13 08:49:16.000000 columnflow-0.2.1/columnflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:49:16.000000 columnflow-0.2.1/columnflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:49:16.000000 columnflow-0.2.1/columnflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-13 08:49:16.000000 columnflow-0.2.1/columnflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 08:49:16.000000 columnflow-0.2.1/columnflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:49:16.855717 columnflow-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-13 08:49:02.000000 columnflow-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:35:53.990889 columnflow-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 17:35:42.000000 columnflow-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-07-21 17:35:53.990889 columnflow-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-07-21 17:35:42.000000 columnflow-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:35:53.986889 columnflow-0.2.2/columnflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:35:53.986889 columnflow-0.2.2/columnflow/calibration/
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/calibration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:35:53.986889 columnflow-0.2.2/columnflow/calibration/cms/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/calibration/cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31880 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/calibration/cms/jets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27962 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/calibration/cms/jets_coffea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/calibration/cms/met.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/calibration/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120984 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/columnar_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17804 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/config_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:35:53.986889 columnflow-0.2.2/columnflow/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)    47539 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/inference/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:35:53.986889 columnflow-0.2.2/columnflow/inference/cms/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/inference/cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23076 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/inference/cms/datacard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:35:53.986889 columnflow-0.2.2/columnflow/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)    14710 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:35:53.986889 columnflow-0.2.2/columnflow/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/plotting/plot_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/plotting/plot_functions_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/plotting/plot_functions_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11587 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/plotting/plot_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:35:53.986889 columnflow-0.2.2/columnflow/production/
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/production/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/production/categories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:35:53.990889 columnflow-0.2.2/columnflow/production/cms/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/production/cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/production/cms/btag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/production/cms/electron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/production/cms/gen_top_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/production/cms/mc_weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/production/cms/muon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/production/cms/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/production/cms/pileup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/production/cms/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/production/cms/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/production/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/production/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/production/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:35:53.990889 columnflow-0.2.2/columnflow/selection/
+-rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/selection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:35:53.990889 columnflow-0.2.2/columnflow/selection/cms/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/selection/cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/selection/cms/json_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/selection/cms/met_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/selection/matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/selection/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/selection/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:35:53.990889 columnflow-0.2.2/columnflow/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/tasks/calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:35:53.990889 columnflow-0.2.2/columnflow/tasks/cms/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/tasks/cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/tasks/cms/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/tasks/cms/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25339 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/tasks/cutflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17235 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/tasks/external.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:35:53.990889 columnflow-0.2.2/columnflow/tasks/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/tasks/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52097 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/tasks/framework/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/tasks/framework/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49957 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/tasks/framework/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/tasks/framework/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15546 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/tasks/framework/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25625 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/tasks/framework/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/tasks/histograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19082 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/tasks/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/tasks/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/tasks/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17164 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/tasks/reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14543 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/tasks/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/tasks/union.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/tasks/yields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25820 2023-07-21 17:35:42.000000 columnflow-0.2.2/columnflow/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:35:53.986889 columnflow-0.2.2/columnflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-07-21 17:35:53.000000 columnflow-0.2.2/columnflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-21 17:35:53.000000 columnflow-0.2.2/columnflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 17:35:53.000000 columnflow-0.2.2/columnflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 17:35:53.000000 columnflow-0.2.2/columnflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-21 17:35:53.000000 columnflow-0.2.2/columnflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 17:35:53.000000 columnflow-0.2.2/columnflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 17:35:53.990889 columnflow-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-21 17:35:42.000000 columnflow-0.2.2/setup.py
```

### Comparing `columnflow-0.2.1/LICENSE` & `columnflow-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.1/PKG-INFO` & `columnflow-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: columnflow
-Version: 0.2.1
+Version: 0.2.2
 Summary: columnflow
 Home-page: https://github.com/columnflow/columnflow
 Author: The columnflow team
 Author-email: github.riga@icloud.com
 License: BSD-3-Clause
 Keywords: physics,analysis,experiment,columnar,vectoized,law,order,luigi,lhc,cms
 Classifier: Programming Language :: Python
@@ -37,14 +37,16 @@
 [![Package version](https://img.shields.io/pypi/v/columnflow.svg?style=flat)](https://pypi.python.org/pypi/columnflow)
 [![Documentation status](https://readthedocs.org/projects/columnflow/badge/?version=stable)](http://columnflow.readthedocs.io)
 [![Code coverge](https://codecov.io/gh/columnflow/columnflow/branch/master/graph/badge.svg?token=33FLINPXFP)](https://codecov.io/gh/columnflow/columnflow)
 [![License](https://img.shields.io/github/license/columnflow/columnflow.svg)](https://github.com/columnflow/columnflow/blob/master/LICENSE)
 
 Backend for columnar, fully orchestrated HEP analyses with pure Python, [law](https://github.com/riga/law) and [order](https://github.com/riga/order).
 
+Original source hosted at [GitHub](https://github.com/columnflow/columnflow).
+
 
 <!-- marker-after-header -->
 
 
 ## Note on current development
 
 This project is currently in a beta phase.
@@ -66,44 +68,49 @@
 ```
 
 At the end of the setup, you will see further instructions and suggestions to run your first analysis tasks (example below).
 
 ```
 Setup successfull! The next steps are:
 
-  1. Setup the repository and install the environment.
-    > source setup.sh [optional_setup_name]
+1. Setup the repository and install the environment.
+   > cd
+   > source setup.sh [optional_setup_name]
 
-  2. Run local tests & linting checks to verify that the analysis is setup correctly.
-    > ./tests/run_all
+2. Run local tests & linting checks to verify that the analysis is setup correctly.
+   > ./tests/run_all
 
-  3. Create a GRID proxy if you intend to run tasks that need one
-    > voms-proxy-init -voms cms -rfc -valid 196:00
+3. Create a GRID proxy if you intend to run tasks that need one
+   > voms-proxy-init -rfc -valid 196:00
 
-  4. Checkout the 'Getting started' guide to run your first tasks.
-    https://columnflow.readthedocs.io/en/stable/start.html
+4. Checkout the 'Getting started' guide to run your first tasks.
+   https://columnflow.readthedocs.io/en/stable/start.html
 
-    Suggestions for tasks to run:
+   Suggestions for tasks to run:
 
-    a) Run the 'calibration -> selection -> reduction' pipeline for the first file of the
-       default dataset using the default calibrator and default selector
-       (enter the command below and 'tab-tab' to see all arguments or add --help for help)
+   a) Run the 'calibration -> selection -> reduction' pipeline for the first file of the
+      default dataset using the default calibrator and default selector
+      (enter the command below and 'tab-tab' to see all arguments or add --help for help)
       > law run cf.ReduceEvents --version dev1 --branch 0
 
-    b) Create the jet1_pt distribution for the single top dataset:
+      Verify what you just run by adding '--print-status -1' (-1 = fully recursive)
+      > law run cf.ReduceEvents --version dev1 --branch 0 --print-status -1
+
+   b) Create the jet1_pt distribution for the single top datasets
+      (if you have an image/pdf viewer installed, add it via '--view-cmd <binary>')
       > law run cf.PlotVariables1D --version dev1 --datasets 'st*' --variables jet1_pt
 
-    c) Include the ttbar dataset and also plot jet1_eta:
-      > law run cf.PlotVariables1D --version dev1 --datasets 'tt*,st*' --variables jet1_pt,jet1_eta
+      Again, verify what you just ran, now with recursion depth 4
+      > law run cf.PlotVariables1D --version dev1 --datasets 'st*' --variables jet1_pt --print-status 4
 
-    d) Create cms-style datacards for the example model in hgg/inference/example.py:
-      > law run cf.CreateDatacards --version dev1 --inference-model example
+   c) Include the ttbar dataset and also plot jet1_eta
+      > law run cf.PlotVariables1D --version dev1 --datasets 'tt*,st*' --variables jet1_pt,jet1_eta
 ```
 
-For a better overview of the tasks that are triggered by the commands below, checkout the current (yet stylized) [task graph](https://github.com/columnflow/columnflow/issues/25#issue-1258137827).
+For a better overview of the tasks that are triggered by the commands below, checkout the current (yet stylized) [task graph](https://github.com/columnflow/columnflow/wiki#default-task-graph).
 
 
 ## Projects using columnflow
 
 - [hh2bbtautau](https://github.com/uhh-cms/hh2bbtautau): HH → bb𝜏𝜏 analysis with CMS.
 - [hh2bbww](https://github.com/uhh-cms/hh2bbww): HH → bbWW analysis with CMS.
 - [topmass](https://github.com/uhh-cms/topmass): Top quark mass measurement with CMS.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: columnflow Version: 0.2.1 Summary: columnflow Home-
+Metadata-Version: 2.1 Name: columnflow Version: 0.2.2 Summary: columnflow Home-
 page: https://github.com/columnflow/columnflow Author: The columnflow team
 Author-email: github.riga@icloud.com License: BSD-3-Clause Keywords:
 physics,analysis,experiment,columnar,vectoized,law,order,luigi,lhc,cms
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
@@ -20,16 +20,17 @@
 columnflow) [![Documentation status](https://readthedocs.org/projects/
 columnflow/badge/?version=stable)](http://columnflow.readthedocs.io) [![Code
 coverge](https://codecov.io/gh/columnflow/columnflow/branch/master/graph/
 badge.svg?token=33FLINPXFP)](https://codecov.io/gh/columnflow/columnflow) [!
 [License](https://img.shields.io/github/license/columnflow/columnflow.svg)]
 (https://github.com/columnflow/columnflow/blob/master/LICENSE) Backend for
 columnar, fully orchestrated HEP analyses with pure Python, [law](https://
-github.com/riga/law) and [order](https://github.com/riga/order).  ## Note on
-current development This project is currently in a beta phase. The project
+github.com/riga/law) and [order](https://github.com/riga/order). Original
+source hosted at [GitHub](https://github.com/columnflow/columnflow).  ## Note
+on current development This project is currently in a beta phase. The project
 setup, suggested workflows, definitions of particular tasks, and the signatures
 of various helper classes and functions are mostly frozen but could still be
 subject to changes in the near future. At this point (December 2022), four
 large-scale analyses based upon columnflow are being developed, and in the
 process, help test and verify various aspects of its core. The first released
 version is expected in early 2023. However, if you would like to join early on,
 contribute or just give it a spin, feel free to get in touch! ![Columnflow
@@ -40,39 +41,42 @@
 columnflow/columnflow/tree/master/analysis_templates)). The following command
 (no previous git clone required) interactively asks for a handful of names and
 settings, and creates a minimal, yet fully functioning project structure for
 you! ```shell bash -c "$(curl -Ls https://raw.githubusercontent.com/columnflow/
 columnflow/master/create_analysis.sh)" ``` At the end of the setup, you will
 see further instructions and suggestions to run your first analysis tasks
 (example below). ``` Setup successfull! The next steps are: 1. Setup the
-repository and install the environment. > source setup.sh [optional_setup_name]
-2. Run local tests & linting checks to verify that the analysis is setup
-correctly. > ./tests/run_all 3. Create a GRID proxy if you intend to run tasks
-that need one > voms-proxy-init -voms cms -rfc -valid 196:00 4. Checkout the
-'Getting started' guide to run your first tasks. https://
+repository and install the environment. > cd > source setup.sh
+[optional_setup_name] 2. Run local tests & linting checks to verify that the
+analysis is setup correctly. > ./tests/run_all 3. Create a GRID proxy if you
+intend to run tasks that need one > voms-proxy-init -rfc -valid 196:00 4.
+Checkout the 'Getting started' guide to run your first tasks. https://
 columnflow.readthedocs.io/en/stable/start.html Suggestions for tasks to run: a)
 Run the 'calibration -> selection -> reduction' pipeline for the first file of
 the default dataset using the default calibrator and default selector (enter
 the command below and 'tab-tab' to see all arguments or add --help for help) >
-law run cf.ReduceEvents --version dev1 --branch 0 b) Create the jet1_pt
-distribution for the single top dataset: > law run cf.PlotVariables1D --version
-dev1 --datasets 'st*' --variables jet1_pt c) Include the ttbar dataset and also
-plot jet1_eta: > law run cf.PlotVariables1D --version dev1 --datasets 'tt*,st*'
---variables jet1_pt,jet1_eta d) Create cms-style datacards for the example
-model in hgg/inference/example.py: > law run cf.CreateDatacards --version dev1
---inference-model example ``` For a better overview of the tasks that are
-triggered by the commands below, checkout the current (yet stylized) [task
-graph](https://github.com/columnflow/columnflow/issues/25#issue-1258137827). ##
-Projects using columnflow - [hh2bbtautau](https://github.com/uhh-cms/
-hh2bbtautau): HH â bbðð analysis with CMS. - [hh2bbww](https://
-github.com/uhh-cms/hh2bbww): HH â bbWW analysis with CMS. - [topmass](https:/
-/github.com/uhh-cms/topmass): Top quark mass measurement with CMS. - [mttbar]
-(https://github.com/uhh-cms/mttbar): Search for heavy resonances in ttbar
-events with CMS. - [analysis playground](https://github.com/uhh-cms/
-analysis_playground): A testing playground for HEP analyses. ## Contributors
+law run cf.ReduceEvents --version dev1 --branch 0 Verify what you just run by
+adding '--print-status -1' (-1 = fully recursive) > law run cf.ReduceEvents --
+version dev1 --branch 0 --print-status -1 b) Create the jet1_pt distribution
+for the single top datasets (if you have an image/pdf viewer installed, add it
+via '--view-cmd ') > law run cf.PlotVariables1D --version dev1 --datasets 'st*'
+--variables jet1_pt Again, verify what you just ran, now with recursion depth 4
+> law run cf.PlotVariables1D --version dev1 --datasets 'st*' --variables
+jet1_pt --print-status 4 c) Include the ttbar dataset and also plot jet1_eta >
+law run cf.PlotVariables1D --version dev1 --datasets 'tt*,st*' --variables
+jet1_pt,jet1_eta ``` For a better overview of the tasks that are triggered by
+the commands below, checkout the current (yet stylized) [task graph](https://
+github.com/columnflow/columnflow/wiki#default-task-graph). ## Projects using
+columnflow - [hh2bbtautau](https://github.com/uhh-cms/hh2bbtautau): HH â
+bbðð analysis with CMS. - [hh2bbww](https://github.com/uhh-cms/hh2bbww):
+HH â bbWW analysis with CMS. - [topmass](https://github.com/uhh-cms/topmass):
+Top quark mass measurement with CMS. - [mttbar](https://github.com/uhh-cms/
+mttbar): Search for heavy resonances in ttbar events with CMS. - [analysis
+playground](https://github.com/uhh-cms/analysis_playground): A testing
+playground for HEP analyses. ## Contributors
             [Marcel_Rieger]              [Mathis_Frahm]    [Daniel_Savoiu]      [pkausw]           [nprouvost]       [Bogdan-Wiederspan]  [Tobias
              Marcel_Rieger                Mathis_Frahm      Daniel_Savoiu        pkausw             nprouvost         Bogdan-Wiederspan   Kramer]
          ð» ð ð â    ð» ð�    ð» ð�    ð» ð�     ð» â ï     ð» â ï Tobias
                                                                                                                                            Kramer
                                                                                                                                             ð»
               [Matthias_Schroeder]      [Johannes_Lange]   [BalduinLetzer]
                Matthias_Schroeder        Johannes_Lange     BalduinLetzer
```

### Comparing `columnflow-0.2.1/README.md` & `columnflow-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 [![Package version](https://img.shields.io/pypi/v/columnflow.svg?style=flat)](https://pypi.python.org/pypi/columnflow)
 [![Documentation status](https://readthedocs.org/projects/columnflow/badge/?version=stable)](http://columnflow.readthedocs.io)
 [![Code coverge](https://codecov.io/gh/columnflow/columnflow/branch/master/graph/badge.svg?token=33FLINPXFP)](https://codecov.io/gh/columnflow/columnflow)
 [![License](https://img.shields.io/github/license/columnflow/columnflow.svg)](https://github.com/columnflow/columnflow/blob/master/LICENSE)
 
 Backend for columnar, fully orchestrated HEP analyses with pure Python, [law](https://github.com/riga/law) and [order](https://github.com/riga/order).
 
+Original source hosted at [GitHub](https://github.com/columnflow/columnflow).
+
 
 <!-- marker-after-header -->
 
 
 ## Note on current development
 
 This project is currently in a beta phase.
@@ -41,44 +43,49 @@
 ```
 
 At the end of the setup, you will see further instructions and suggestions to run your first analysis tasks (example below).
 
 ```
 Setup successfull! The next steps are:
 
-  1. Setup the repository and install the environment.
-    > source setup.sh [optional_setup_name]
+1. Setup the repository and install the environment.
+   > cd
+   > source setup.sh [optional_setup_name]
 
-  2. Run local tests & linting checks to verify that the analysis is setup correctly.
-    > ./tests/run_all
+2. Run local tests & linting checks to verify that the analysis is setup correctly.
+   > ./tests/run_all
 
-  3. Create a GRID proxy if you intend to run tasks that need one
-    > voms-proxy-init -voms cms -rfc -valid 196:00
+3. Create a GRID proxy if you intend to run tasks that need one
+   > voms-proxy-init -rfc -valid 196:00
 
-  4. Checkout the 'Getting started' guide to run your first tasks.
-    https://columnflow.readthedocs.io/en/stable/start.html
+4. Checkout the 'Getting started' guide to run your first tasks.
+   https://columnflow.readthedocs.io/en/stable/start.html
 
-    Suggestions for tasks to run:
+   Suggestions for tasks to run:
 
-    a) Run the 'calibration -> selection -> reduction' pipeline for the first file of the
-       default dataset using the default calibrator and default selector
-       (enter the command below and 'tab-tab' to see all arguments or add --help for help)
+   a) Run the 'calibration -> selection -> reduction' pipeline for the first file of the
+      default dataset using the default calibrator and default selector
+      (enter the command below and 'tab-tab' to see all arguments or add --help for help)
       > law run cf.ReduceEvents --version dev1 --branch 0
 
-    b) Create the jet1_pt distribution for the single top dataset:
+      Verify what you just run by adding '--print-status -1' (-1 = fully recursive)
+      > law run cf.ReduceEvents --version dev1 --branch 0 --print-status -1
+
+   b) Create the jet1_pt distribution for the single top datasets
+      (if you have an image/pdf viewer installed, add it via '--view-cmd <binary>')
       > law run cf.PlotVariables1D --version dev1 --datasets 'st*' --variables jet1_pt
 
-    c) Include the ttbar dataset and also plot jet1_eta:
-      > law run cf.PlotVariables1D --version dev1 --datasets 'tt*,st*' --variables jet1_pt,jet1_eta
+      Again, verify what you just ran, now with recursion depth 4
+      > law run cf.PlotVariables1D --version dev1 --datasets 'st*' --variables jet1_pt --print-status 4
 
-    d) Create cms-style datacards for the example model in hgg/inference/example.py:
-      > law run cf.CreateDatacards --version dev1 --inference-model example
+   c) Include the ttbar dataset and also plot jet1_eta
+      > law run cf.PlotVariables1D --version dev1 --datasets 'tt*,st*' --variables jet1_pt,jet1_eta
 ```
 
-For a better overview of the tasks that are triggered by the commands below, checkout the current (yet stylized) [task graph](https://github.com/columnflow/columnflow/issues/25#issue-1258137827).
+For a better overview of the tasks that are triggered by the commands below, checkout the current (yet stylized) [task graph](https://github.com/columnflow/columnflow/wiki#default-task-graph).
 
 
 ## Projects using columnflow
 
 - [hh2bbtautau](https://github.com/uhh-cms/hh2bbtautau): HH → bb𝜏𝜏 analysis with CMS.
 - [hh2bbww](https://github.com/uhh-cms/hh2bbww): HH → bbWW analysis with CMS.
 - [topmass](https://github.com/uhh-cms/topmass): Top quark mass measurement with CMS.
```

#### html2text {}

```diff
@@ -7,16 +7,17 @@
 columnflow) [![Documentation status](https://readthedocs.org/projects/
 columnflow/badge/?version=stable)](http://columnflow.readthedocs.io) [![Code
 coverge](https://codecov.io/gh/columnflow/columnflow/branch/master/graph/
 badge.svg?token=33FLINPXFP)](https://codecov.io/gh/columnflow/columnflow) [!
 [License](https://img.shields.io/github/license/columnflow/columnflow.svg)]
 (https://github.com/columnflow/columnflow/blob/master/LICENSE) Backend for
 columnar, fully orchestrated HEP analyses with pure Python, [law](https://
-github.com/riga/law) and [order](https://github.com/riga/order).  ## Note on
-current development This project is currently in a beta phase. The project
+github.com/riga/law) and [order](https://github.com/riga/order). Original
+source hosted at [GitHub](https://github.com/columnflow/columnflow).  ## Note
+on current development This project is currently in a beta phase. The project
 setup, suggested workflows, definitions of particular tasks, and the signatures
 of various helper classes and functions are mostly frozen but could still be
 subject to changes in the near future. At this point (December 2022), four
 large-scale analyses based upon columnflow are being developed, and in the
 process, help test and verify various aspects of its core. The first released
 version is expected in early 2023. However, if you would like to join early on,
 contribute or just give it a spin, feel free to get in touch! ![Columnflow
@@ -27,39 +28,42 @@
 columnflow/columnflow/tree/master/analysis_templates)). The following command
 (no previous git clone required) interactively asks for a handful of names and
 settings, and creates a minimal, yet fully functioning project structure for
 you! ```shell bash -c "$(curl -Ls https://raw.githubusercontent.com/columnflow/
 columnflow/master/create_analysis.sh)" ``` At the end of the setup, you will
 see further instructions and suggestions to run your first analysis tasks
 (example below). ``` Setup successfull! The next steps are: 1. Setup the
-repository and install the environment. > source setup.sh [optional_setup_name]
-2. Run local tests & linting checks to verify that the analysis is setup
-correctly. > ./tests/run_all 3. Create a GRID proxy if you intend to run tasks
-that need one > voms-proxy-init -voms cms -rfc -valid 196:00 4. Checkout the
-'Getting started' guide to run your first tasks. https://
+repository and install the environment. > cd > source setup.sh
+[optional_setup_name] 2. Run local tests & linting checks to verify that the
+analysis is setup correctly. > ./tests/run_all 3. Create a GRID proxy if you
+intend to run tasks that need one > voms-proxy-init -rfc -valid 196:00 4.
+Checkout the 'Getting started' guide to run your first tasks. https://
 columnflow.readthedocs.io/en/stable/start.html Suggestions for tasks to run: a)
 Run the 'calibration -> selection -> reduction' pipeline for the first file of
 the default dataset using the default calibrator and default selector (enter
 the command below and 'tab-tab' to see all arguments or add --help for help) >
-law run cf.ReduceEvents --version dev1 --branch 0 b) Create the jet1_pt
-distribution for the single top dataset: > law run cf.PlotVariables1D --version
-dev1 --datasets 'st*' --variables jet1_pt c) Include the ttbar dataset and also
-plot jet1_eta: > law run cf.PlotVariables1D --version dev1 --datasets 'tt*,st*'
---variables jet1_pt,jet1_eta d) Create cms-style datacards for the example
-model in hgg/inference/example.py: > law run cf.CreateDatacards --version dev1
---inference-model example ``` For a better overview of the tasks that are
-triggered by the commands below, checkout the current (yet stylized) [task
-graph](https://github.com/columnflow/columnflow/issues/25#issue-1258137827). ##
-Projects using columnflow - [hh2bbtautau](https://github.com/uhh-cms/
-hh2bbtautau): HH â bbðð analysis with CMS. - [hh2bbww](https://
-github.com/uhh-cms/hh2bbww): HH â bbWW analysis with CMS. - [topmass](https:/
-/github.com/uhh-cms/topmass): Top quark mass measurement with CMS. - [mttbar]
-(https://github.com/uhh-cms/mttbar): Search for heavy resonances in ttbar
-events with CMS. - [analysis playground](https://github.com/uhh-cms/
-analysis_playground): A testing playground for HEP analyses. ## Contributors
+law run cf.ReduceEvents --version dev1 --branch 0 Verify what you just run by
+adding '--print-status -1' (-1 = fully recursive) > law run cf.ReduceEvents --
+version dev1 --branch 0 --print-status -1 b) Create the jet1_pt distribution
+for the single top datasets (if you have an image/pdf viewer installed, add it
+via '--view-cmd ') > law run cf.PlotVariables1D --version dev1 --datasets 'st*'
+--variables jet1_pt Again, verify what you just ran, now with recursion depth 4
+> law run cf.PlotVariables1D --version dev1 --datasets 'st*' --variables
+jet1_pt --print-status 4 c) Include the ttbar dataset and also plot jet1_eta >
+law run cf.PlotVariables1D --version dev1 --datasets 'tt*,st*' --variables
+jet1_pt,jet1_eta ``` For a better overview of the tasks that are triggered by
+the commands below, checkout the current (yet stylized) [task graph](https://
+github.com/columnflow/columnflow/wiki#default-task-graph). ## Projects using
+columnflow - [hh2bbtautau](https://github.com/uhh-cms/hh2bbtautau): HH â
+bbðð analysis with CMS. - [hh2bbww](https://github.com/uhh-cms/hh2bbww):
+HH â bbWW analysis with CMS. - [topmass](https://github.com/uhh-cms/topmass):
+Top quark mass measurement with CMS. - [mttbar](https://github.com/uhh-cms/
+mttbar): Search for heavy resonances in ttbar events with CMS. - [analysis
+playground](https://github.com/uhh-cms/analysis_playground): A testing
+playground for HEP analyses. ## Contributors
             [Marcel_Rieger]              [Mathis_Frahm]    [Daniel_Savoiu]      [pkausw]           [nprouvost]       [Bogdan-Wiederspan]  [Tobias
              Marcel_Rieger                Mathis_Frahm      Daniel_Savoiu        pkausw             nprouvost         Bogdan-Wiederspan   Kramer]
          ð» ð ð â    ð» ð�    ð» ð�    ð» ð�     ð» â ï     ð» â ï Tobias
                                                                                                                                            Kramer
                                                                                                                                             ð»
               [Matthias_Schroeder]      [Johannes_Lange]   [BalduinLetzer]
                Matthias_Schroeder        Johannes_Lange     BalduinLetzer
```

### Comparing `columnflow-0.2.1/columnflow/__init__.py` & `columnflow-0.2.2/columnflow/__init__.py`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.1/columnflow/__version__.py` & `columnflow-0.2.2/columnflow/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     "Tobias Kramer",
     "Matthias Schroeder",
     "Johannes Lange",
 ]
 __contact__ = "https://github.com/columnflow/columnflow"
 __license__ = "BSD-3-Clause"
 __status__ = "Development"
-__version__ = "0.2.1"
+__version__ = "0.2.2"
```

### Comparing `columnflow-0.2.1/columnflow/calibration/cms/jets.py` & `columnflow-0.2.2/columnflow/calibration/cms/jets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 # coding: utf-8
 
 """
 Jet energy corrections and jet resolution smearing.
 """
 
 import functools
+from typing import Any
 
 from columnflow.calibration import Calibrator, calibrator
 from columnflow.calibration.util import ak_random, propagate_met
 from columnflow.production.util import attach_coffea_behavior
-from columnflow.util import maybe_import
-from columnflow.columnar_util import set_ak_column, layout_ak_array
+from columnflow.util import maybe_import, InsertableDict, DotDict
+from columnflow.columnar_util import set_ak_column, layout_ak_array, optional_column as optional
 
 
 np = maybe_import("numpy")
 ak = maybe_import("awkward")
+correctionlib = maybe_import("correctionlib")
 
 
 #
 # helper functions
 #
 
 set_ak_column_f32 = functools.partial(set_ak_column, value_type=np.float32)
 
 
-def get_evaluators(correction_set, names):
-    """
-    Helper function to get a list of correction evaluators from a correctionlib
-    *CorrectionSet* object given a list of *names*. The *names* can refer to either
-    simple or compound corrections.
-
-    Throws a *KeyError* if any of the *names* are not found.
+def get_evaluators(
+    correction_set: correctionlib.highlevel.CorrectionSet,
+    names: list[str],
+) -> list[Any]:
+    """
+    Helper function to get a list of correction evaluators from a
+    :external+correctionlib:py:class:`correctionlib.highlevel.CorrectionSet` object given
+    a list of *names*. The *names* can refer to either simple or compound
+    corrections.
+
+    :param correction_set: evaluator provided by :external+correctionlib:doc:`index`
+    :param names: List of names of corrections to be applied
+    :raises RuntimeError: If a requested correction in *names* is not available
+    :return: List of compounded corrections, see
+        :external+correctionlib:py:class:`correctionlib.highlevel.CorrectionSet`
     """
     # raise nice error if keys not found
     available_keys = set(correction_set.keys()).union(correction_set.compound.keys())
     missing_keys = set(names) - available_keys
     if missing_keys:
         raise RuntimeError("corrections not found:" + "".join(
             f"\n  - {name}" for name in names if name in missing_keys
@@ -47,17 +57,22 @@
         correction_set.compound[name]
         if name in correction_set.compound
         else correction_set[name]
         for name in names
     ]
 
 
-def ak_evaluate(evaluator, *args):
+def ak_evaluate(evaluator: correctionlib.highlevel.Correction, *args) -> float:
     """
-    Evaluate a correctionlib *Correction* using one or more awkward arrays as inputs.
+    Evaluate a :external+correctionlib:py:class:`correctionlib.highlevel.Correction`
+    using one or more :external+ak:py:class:`awkward arrays <ak.Array>` as inputs.
+
+    :param evaluator: Evaluator instance
+    :raises ValueError: If no :external+ak:py:class:`awkward arrays <ak.Array>` are provided
+    :return: The correction factor derived from the input arrays
     """
     # fail if no arguments
     if not args:
         raise ValueError("Expected at least one argument.")
 
     # collect arguments that are awkward arrays
     ak_args = [
@@ -92,49 +107,87 @@
     return result
 
 
 #
 # jet energy corrections
 #
 
+# define default functions for jec calibrator
+def get_jec_file_default(self, external_files: DotDict) -> str:
+    """
+    Function to obtain external jec files.
+
+    By default, this function extracts the location of the jec correction
+    files from the current config instance *config_inst*:
+
+    .. code-block:: python
+
+        cfg.x.external_files = DotDict.wrap({
+            "jet_jerc": "/afs/cern.ch/user/m/mrieger/public/mirrors/jsonpog-integration-f018adfb/POG/JME/2017_UL/jet_jerc.json.gz",
+        })
+
+    :param external_files: Dictionary containing the information about the file location
+    :return: path or url to correction file(s)
+    """ # noqa
+    return external_files.jet_jerc
+
+
+def get_jec_config_default(self) -> DotDict:
+    """Load config relevant to the JEC corrections.
+
+    By default, this is extracted from the current *config_inst*:
+
+    .. code-block:: python
+
+        self.config_inst.x.jec
+
+    Used in :py:meth:`~.jec.setup_func`.
+
+    :return: Dictionary containing configurations for JEC callibrations
+    """
+    return self.config_inst.x.jec
+
+
 @calibrator(
     uses={
-        "nJet", "Jet.pt", "Jet.eta", "Jet.phi", "Jet.mass", "Jet.area", "Jet.rawFactor",
-        "Jet.jetId", "fixedGridRhoFastjetAll", "Rho.fixedGridRhoFastjetAll",
+        "Jet.pt", "Jet.eta", "Jet.phi", "Jet.mass", "Jet.area", "Jet.rawFactor",
+        "Jet.jetId",
+        optional("fixedGridRhoFastjetAll"),
+        optional("Rho.fixedGridRhoFastjetAll"),
         attach_coffea_behavior,
     },
     produces={
         "Jet.pt", "Jet.mass", "Jet.rawFactor",
     },
     # custom uncertainty sources, defaults to config when empty
     uncertainty_sources=None,
     # toggle for propagation to MET
     propagate_met=True,
     # function to determine the correction file
-    get_jec_file=(lambda self, external_files: external_files.jet_jerc),
+    get_jec_file=get_jec_file_default,
     # function to determine the jec configuration dict
-    get_jec_config=(lambda self: self.config_inst.x.jec),
+    get_jec_config=get_jec_config_default,
 )
 def jec(
     self: Calibrator,
     events: ak.Array,
     min_pt_met_prop: float = 15.0,
     max_eta_met_prop: float = 5.2,
     **kwargs,
 ) -> ak.Array:
-    """
-    Performs the jet energy corrections and uncertainty shifts using the correctionlib, optionally
+    """Performs the jet energy corrections and uncertainty shifts using the
+    :external+correctionlib:doc:`index`, optionally
     propagating the changes to the MET.
 
     Requires an external file in the config under ``jet_jerc``:
 
     .. code-block:: python
 
         cfg.x.external_files = DotDict.wrap({
-            "jet_jerc": "/afs/cern.ch/user/m/mrieger/public/mirrors/jsonpog-integration-f018adfb/POG/JME/2017_UL/jet_jerc.json.gz",  # noqa
+            "jet_jerc": "/afs/cern.ch/user/m/mrieger/public/mirrors/jsonpog-integration-f018adfb/POG/JME/2017_UL/jet_jerc.json.gz",
         })
 
     *get_jec_file* can be adapted in a subclass in case it is stored differently in the
     external files
 
     The jec configuration should be an auxiliary entry in the config, specifying the correction
     details under "jec":
@@ -157,15 +210,29 @@
             ]
         }
 
     *get_jec_config* can be adapted in a subclass in case it is stored differently in the config.
 
     If running on data, the datasets must have an auxiliary field *jec_era* defined, e.g. "RunF",
     or an auxiliary field *era*, e.g. "F".
-    """
+
+    This instance of :py:class:`~columnflow.calibration.Calibrator` is
+    initialized with the following parameters by default:
+
+    :param events: awkward array containing events to process
+
+    :param min_pt_met_prop: If *propagate_met* variable is ``True`` propagate the updated jet values
+        to the missing transverse energy (MET) using
+        :py:func:`~columnflow.calibration.util.propagate_met` for events where
+        ``met.pt > *min_pt_met_prop*``.
+    :param max_eta_met_prop: If *propagate_met* variable is ``True`` propagate the updated jet
+        values to the missing transverse energy (MET) using
+        :py:func:`~columnflow.calibration.util.propagate_met` for events where
+        ``met.eta > *min_eta_met_prop*``.
+    """ # noqa
     # calculate uncorrected pt, mass
     events = set_ak_column_f32(events, "Jet.pt_raw", events.Jet.pt * (1 - events.Jet.rawFactor))
     events = set_ak_column_f32(events, "Jet.mass_raw", events.Jet.mass * (1 - events.Jet.rawFactor))
 
     def correct_jets(pt, area, eta, rho, evaluator_key="jec"):
         # variable naming convention
         variable_map = {
@@ -297,17 +364,14 @@
             events = set_ak_column_f32(events, f"MET.phi_jec_{name}_down", met_phi_down)
 
     return events
 
 
 @jec.init
 def jec_init(self: Calibrator) -> None:
-    """
-    Add JEC uncertainty shifts to the list of produced columns.
-    """
     jec_cfg = self.get_jec_config()
 
     sources = self.uncertainty_sources
     if sources is None:
         sources = jec_cfg.uncertainty_sources
 
     # add shifted jet variables
@@ -338,15 +402,63 @@
         return
 
     from columnflow.tasks.external import BundleExternalFiles
     reqs["external_files"] = BundleExternalFiles.req(self.task)
 
 
 @jec.setup
-def jec_setup(self: Calibrator, reqs: dict, inputs: dict) -> None:
+def jec_setup(self: Calibrator, reqs: dict, inputs: dict, reader_targets: InsertableDict) -> None:
+    """
+    Load the correct jec files using the :py:func:`from_string` method of the
+    :external+correctionlib:py:class:`correctionlib.highlevel.CorrectionSet`
+    function and apply the corrections as needed.
+
+    The source files for the :external+correctionlib:py:class:`correctionlib.highlevel.CorrectionSet`
+    instance are extracted with the :py:meth:`~.jec.get_jec_file`.
+
+    Uses the member function :py:meth:`~.jec.get_jec_config` to construct the
+    required keys, which are based on the following information about the JEC:
+
+        - levels
+        - campaign
+        - version
+        - jet_type
+
+    A corresponding example snippet wihtin the *config_inst* could like something
+    like this:
+
+    .. code-block:: python
+
+        cfg.x.jec = DotDict.wrap({
+            # campaign name for this JEC correctiono
+            "campaign": f"Summer19UL{year2}{jerc_postfix}",
+            # version of the corrections
+            "version": "V7",
+            # Type of jets that the corrections should be applied on
+            "jet_type": "AK4PFchs",
+            # relevant levels in the derivation process of the JEC
+            "levels": ["L1FastJet", "L2Relative", "L2L3Residual", "L3Absolute"],
+            # relevant levels in the derivation process of the Type 1 MET JEC
+            "levels_for_type1_met": ["L1FastJet"],
+            # names of the uncertainties to be applied
+            "uncertainty_sources": [
+                "Total",
+                "CorrelationGroupMPFInSitu",
+                "CorrelationGroupIntercalibration",
+                "CorrelationGroupbJES",
+                "CorrelationGroupFlavor",
+                "CorrelationGroupUncorrelated",
+            ],
+        })
+
+    :param reqs: Requirement dictionary for this
+        :py:class:`~columnflow.calibration.Calibrator` instance
+    :param inputs: Additional inputs, currently not used
+    :param reader_targets: TODO: add documentation
+    """
     bundle = reqs["external_files"]
 
     # import the correction sets from the external file
     import correctionlib
     correction_set = correctionlib.CorrectionSet.from_string(
         self.get_jec_file(bundle.files).load(formatter="gzip").decode("utf-8"),
     )
@@ -385,23 +497,59 @@
     }
 
 
 # custom jec calibrator that only runs nominal correction
 jec_nominal = jec.derive("jec_nominal", cls_dict={"uncertainty_sources": []})
 
 
+# define default functions for jec calibrator
+def get_jer_file(self, external_files: DotDict) -> str:
+    """
+    Function to obtain external jer files.
+
+    By default, this function extracts the location of the jec correction files from the current
+    config instance *config_inst*:
+
+    .. code-block:: python
+
+        cfg.x.external_files = DotDict.wrap({
+            "jet_jerc": "/afs/cern.ch/user/m/mrieger/public/mirrors/jsonpog-integration-f018adfb/POG/JME/2017_UL/jet_jerc.json.gz",
+        })
+
+    :param external_files: Dictionary containing the information about the file location
+    :return: path or url to correction file(s)
+    """ # noqa
+    return external_files.jet_jerc
+
+
+def get_jer_config(self) -> DotDict:
+    """
+    Load config relevant to the JER corrections.
+
+    By default, this is extracted from the current *config_inst*:
+
+    .. code-block:: python
+
+        self.config_inst.x.jer
+
+    :return: Dictionary containing configurations for JEC callibrations
+    """
+    return self.config_inst.x.jer
+
+
 #
 # jet energy resolution smearing
 #
 
 @calibrator(
     uses={
-        "nJet", "Jet.pt", "Jet.eta", "Jet.phi", "Jet.mass", "Jet.genJetIdx",
-        "Rho.fixedGridRhoFastjetAll", "fixedGridRhoFastjetAll",
-        "nGenJet", "GenJet.pt", "GenJet.eta", "GenJet.phi",
+        "Jet.pt", "Jet.eta", "Jet.phi", "Jet.mass", "Jet.genJetIdx",
+        optional("Rho.fixedGridRhoFastjetAll"),
+        optional("fixedGridRhoFastjetAll"),
+        "GenJet.pt", "GenJet.eta", "GenJet.phi",
         "MET.pt", "MET.phi",
         attach_coffea_behavior,
     },
     produces={
         "Jet.pt", "Jet.mass",
         "Jet.pt_unsmeared", "Jet.mass_unsmeared",
         "Jet.pt_jer_up", "Jet.pt_jer_down", "Jet.mass_jer_up", "Jet.mass_jer_down",
@@ -409,34 +557,34 @@
         "MET.pt_jer_up", "MET.pt_jer_down", "MET.phi_jer_up", "MET.phi_jer_down",
     },
     # toggle for propagation to MET
     propagate_met=True,
     # only run on mc
     mc_only=True,
     # function to determine the correction file
-    get_jer_file=(lambda self, external_files: external_files.jet_jerc),
+    get_jer_file=get_jer_file,
     # function to determine the jer configuration dict
-    get_jer_config=(lambda self: self.config_inst.x.jer),
+    get_jer_config=get_jer_config,
 )
 def jer(self: Calibrator, events: ak.Array, **kwargs) -> ak.Array:
     """
     Applies the jet energy resolution smearing in MC and calculates the associated uncertainty
-    shifts using the correctionlib, following the recommendations given in
+    shifts using the :external+correctionlib:doc:`index`, following the recommendations given in
     https://twiki.cern.ch/twiki/bin/viewauth/CMS/JetResolution.
 
     Requires an external file in the config under ``jet_jerc``:
 
     .. code-block:: python
 
         cfg.x.external_files = DotDict.wrap({
-            "jet_jerc": "/afs/cern.ch/user/m/mrieger/public/mirrors/jsonpog-integration-f018adfb/POG/JME/2017_UL/jet_jerc.json.gz",  # noqa
+            "jet_jerc": "/afs/cern.ch/user/m/mrieger/public/mirrors/jsonpog-integration-f018adfb/POG/JME/2017_UL/jet_jerc.json.gz",
         })
 
-    *get_jer_file* can be adapted in a subclass in case it is stored differently in the
-    external files
+    *get_jer_file* can be adapted in a subclass in case it is stored differently in the external
+    files.
 
     The jer configuration should be an auxiliary entry in the config, specifying the correction
     details under ``jer``:
 
     .. code-block:: python
 
         cfg.x.jer = {
@@ -444,15 +592,17 @@
             "version": "JRV2",
             "jet_type": "AK4PFchs",
         },
 
     *get_jer_config* can be adapted in a subclass in case it is stored differently in the config.
 
     Throws an error if running on data.
-    """
+
+    :param events: awkward array containing events to process
+    """ # noqa
     # fail when running on data
     if self.dataset_inst.is_data:
         raise ValueError("attempt to apply jet energy resolution smearing in data")
 
     # save the unsmeared properties in case they are needed later
     events = set_ak_column_f32(events, "Jet.pt_unsmeared", events.Jet.pt)
     events = set_ak_column_f32(events, "Jet.mass_unsmeared", events.Jet.mass)
@@ -610,46 +760,66 @@
         events = set_ak_column_f32(events, "MET.phi_jer_down", met_phi_down)
 
     return events
 
 
 @jer.init
 def jer_init(self: Calibrator) -> None:
-    """
-    Initialization of dynamic components of the jer calibrator.
-    """
     if not self.propagate_met:
         return
 
     self.uses |= {
         "MET.pt", "MET.phi",
     }
     self.produces |= {
         "MET.pt", "MET.phi", "MET.pt_jer_up", "MET.pt_jer_down", "MET.phi_jer_up",
         "MET.phi_jer_down", "MET.pt_unsmeared", "MET.phi_unsmeared",
     }
 
 
 @jer.requires
 def jer_requires(self: Calibrator, reqs: dict) -> None:
-    """
-    Add external files bundle (for JR text files) to dependencies.
-    """
     if "external_files" in reqs:
         return
 
     from columnflow.tasks.external import BundleExternalFiles
     reqs["external_files"] = BundleExternalFiles.req(self.task)
 
 
 @jer.setup
-def jer_setup(self: Calibrator, reqs: dict, inputs: dict) -> None:
+def jer_setup(self: Calibrator, reqs: dict, inputs: dict, reader_targets: InsertableDict) -> None:
     """
-    Determine correct JR files for task based on config/dataset and inject them
-    into the calibrator function call.
+    Load the correct jer files using the :py:func:`from_string` method of the
+    :external+correctionlib:py:class:`correctionlib.highlevel.CorrectionSet` function and apply the
+    corrections as needed.
+
+    The source files for the :external+correctionlib:py:class:`correctionlib.highlevel.CorrectionSet`
+    instance are extracted with the :py:meth:`~.jer.get_jer_file`.
+
+    Uses the member function :py:meth:`~.jer.get_jer_config` to construct the required keys, which
+    are based on the following information about the JER:
+
+    - campaign
+    - version
+    - jet_type
+
+    A corresponding example snippet within the *config_inst* could like something like this:
+
+    .. code-block:: python
+
+        cfg.x.jer = DotDict.wrap({
+            "campaign": f"Summer19UL{year2}{jerc_postfix}",
+            "version": "JRV3",
+            "jet_type": "AK4PFchs",
+        })
+
+    :param reqs: Requirement dictionary for this :py:class:`~columnflow.calibration.Calibrator`
+        instance.
+    :param inputs: Additional inputs, currently not used.
+    :param reader_targets: TODO: add documentation.
     """
     bundle = reqs["external_files"]
 
     # import the correction sets from the external file
     import correctionlib
     correction_set = correctionlib.CorrectionSet.from_string(
         self.get_jer_file(bundle.files).load(formatter="gzip").decode("utf-8"),
@@ -681,14 +851,20 @@
     # functions to determine configs and files
     get_jec_file=None,
     get_jec_config=None,
     get_jer_file=None,
     get_jer_config=None,
 )
 def jets(self: Calibrator, events: ak.Array, **kwargs) -> ak.Array:
+    """
+    Instance of :py:class:`~columnflow.calibration.Calibrator` that does all relevant calibrations
+    for jets, i.e. JEC and JER. For more information, see :py:func:`~.jec` and :py:func:`~.jer`.
+
+    :param events: awkward array containing events to process
+    """
     # apply jet energy corrections
     events = self[jec](events, **kwargs)
 
     # apply jer smearing on MC only
     if self.dataset_inst.is_mc:
         events = self[jer](events, **kwargs)
```

### Comparing `columnflow-0.2.1/columnflow/calibration/cms/jets_coffea.py` & `columnflow-0.2.2/columnflow/calibration/cms/jets_coffea.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # coding: utf-8
 
-"""
-Calibration methods for jets
+""" _Jet calibration with coffea
+Calibration methods for jets using :external+coffea:doc:`coffea <installation>`
+functions
 """
 
 import os
 import functools
 
 import law
 
-from columnflow.util import maybe_import, memoize
+from columnflow.util import maybe_import, memoize, InsertableDict
 from columnflow.calibration import Calibrator, calibrator
 from columnflow.calibration.util import propagate_met, ak_random
 from columnflow.production.util import attach_coffea_behavior
 from columnflow.columnar_util import set_ak_column
-
+from typing import Iterable, Callable, Type
 
 np = maybe_import("numpy")
 ak = maybe_import("awkward")
 
 coffea_extractor = maybe_import("coffea.lookup_tools.extractor")
 coffea_jetmet_tools = maybe_import("coffea.jetmet_tools")
 coffea_txt_converters = maybe_import("coffea.lookup_tools.txt_converters")
@@ -27,46 +28,75 @@
 #
 # first, some utility functions
 #
 
 set_ak_column_f32 = functools.partial(set_ak_column, value_type=np.float32)
 
 
-def get_basenames(struct):
+def get_basenames(struct: Iterable) -> Iterable:
     """
     Replace full file paths in an arbitrary struct by the file basenames.
+
+    The function loops through the structure and extracts the base name using a combination of
+    :py:func:`os.path.splitext` and :py:func:`os.path.basename`. The loop itself is done using the
+    :external+law:py:func:`law.util.map_struct` function.
+
+    :param struct: Iterable of arbitrary nested structure containing full file paths
+
+    :return: Iterable of same structure as *struct* containing only basenames of paths.
     """
     return law.util.map_struct(
         lambda p: os.path.splitext(os.path.basename(p[0] if isinstance(p, tuple) else p))[0],
         struct,
     )
 
 
 @memoize
-def get_lookup_provider(files, conversion_func, provider_cls, names=None):
+def get_lookup_provider(
+    files: list,
+    conversion_func: Callable,
+    provider_cls: Type,
+    names: list[str or tuple[str, str]] = None,
+) -> Type:
     """
     Create a coffea helper object for looking up information in files of various formats.
 
-    This function reads in the *files* containing lookup tables (e.g. JEC text files), extracts
-    the table of values ("weights") using the conversion function *conversion_func* implemented
-    in coffea, and uses them to construct a helper object of type *provider_cls* that can be
-    passed event data to yield the lookup values (e.g. a :py:class:`FactorizedJetCorrector` or
-    :py:class:`JetCorrectionUncertainty`).
-
-    Optionally, a list of *names* can be supplied to select only a subset of weight tables
-    for constructing the provider object (the default is to use all of them). This is intended
-    to be useful for e.g. selecting only a particular set of jet energy uncertainties from an
-    "UncertaintySources" file. By convention, the *names* always start with the basename of the
-    file that contains the corresponding weight table.
+    This function reads in the *files* containing lookup tables (e.g. JEC text files), extracts the
+    table of values ("weights") using the conversion function *conversion_func* implemented in
+    coffea, and uses them to construct a helper object of type *provider_cls* that can be passed
+    event data to yield the lookup values (e.g. a
+    :external+coffea:py:class:`~coffea.jetmet_tools.FactorizedJetCorrector` or
+    :external+coffea:py:class:`~coffea.jetmet_tools.JetCorrectionUncertainty`).
+
+    Optionally, a list of *names* can be supplied to select only a subset of weight tables for
+    constructing the provider object (the default is to use all of them). This is intended to be
+    useful for e.g. selecting only a particular set of jet energy uncertainties from an
+    "UncertaintySources" file. By convention, the *names* always start with the basename of the file
+    that contains the corresponding weight table.
 
     Entries in *names* may also be tuples of the form (*src_name*, *dst_name*), in which case the
     *src_name* will be replaced by *dst_name* when passing the names to the *provider_cls*.
 
     The user must ensure that the *files* can be parsed by the *conversion_func* supplied, and that
     the information contained in the files is meaningful in connection with the *provider_cls*.
+
+    :param files: List of files containing lookup tables (e.g. JEC text files).
+    :param conversion_func:  ``Callable`` that extracts the table of weights from the files in
+        *files*. Must return an *Iterable* that provides a :py:meth:`items` method that returns a
+        structure like (name, type), value
+    :param provider_cls: Class method that is used to construct the *provider* instance that finally
+        provides the weights for the events. Examples:
+        :external+coffea:py:class:`~coffea.jetmet_tools.FactorizedJetCorrector`,
+        :external+coffea:py:class:`~coffea.jetmet_tools.JetCorrectionUncertainty`
+    :param names: Optional list of weight names to include, see text above.
+    :raises ValueError: If *names* contains weight names that are not present in the source file
+    :return: helper class that provides the weights for the events of same type as *provider_cls*
+            (e.g.
+            :external+coffea:py:class:`~coffea.jetmet_tools.FactorizedJetCorrector`,
+            :external+coffea:py:class:`~coffea.jetmet_tools.JetCorrectionUncertainty`)
     """
     # the extractor reads the information contained in the files
     extractor = coffea_extractor.extractor()
 
     # files contain one or more lookup tables, each identified by a name
     all_names = []
     for file_ in files:
@@ -86,14 +116,19 @@
         if unknown_names:
             unknown_names = ", ".join(sorted(list(unknown_names)))
             available = ", ".join(sorted(list(all_names)))
             raise ValueError(
                 f"no weight tables found for the following names: {unknown_names}, "
                 f"available: {available}",
             )
+        # TODO: I don't think the code works correctly if *names* is a list of
+        # strings, since further down below the code explicitly needs a tuple
+        # structure. We will probably need something like the following here
+
+        # names = src_dst_names
     else:
         names = [(n, n) for n in all_names]
 
     # the evaluator does the actual lookup for each separate name
     evaluator = extractor.make_evaluator()
 
     # the provider combines lookup results from multiple names
@@ -107,15 +142,15 @@
 
 #
 # Jet energy corrections
 #
 
 @calibrator(
     uses={
-        "nJet", "Jet.pt", "Jet.eta", "Jet.phi", "Jet.mass", "Jet.area", "Jet.rawFactor",
+        "Jet.pt", "Jet.eta", "Jet.phi", "Jet.mass", "Jet.area", "Jet.rawFactor",
         "Jet.jetId",
         "Rho.fixedGridRhoFastjetAll", "fixedGridRhoFastjetAll",
         attach_coffea_behavior,
     },
     produces={
         "Jet.pt", "Jet.mass", "Jet.rawFactor",
     },
@@ -129,14 +164,24 @@
     events: ak.Array,
     min_pt_met_prop: float = 15.0,
     max_eta_met_prop: float = 5.2,
     **kwargs,
 ) -> ak.Array:
     """
     Apply jet energy corrections and calculate shifts for jet energy uncertainty sources.
+
+    :param events: awkward array containing events to process
+    :param min_pt_met_prop: If *propagate_met* variable is ``True`` propagate the updated jet values
+        to the missing transverse energy (MET) using
+        :py:func:`~columnflow.calibration.util.propagate_met` for events where ``met.pt >
+            *min_pt_met_prop*``.
+    :param max_eta_met_prop: If *propagate_met* variable is ``True`` propagate the updated jet
+        values to the missing transverse energy (MET) using
+        :py:func:`~columnflow.calibration.util.propagate_met` for events where ``met.eta >
+            *min_eta_met_prop*``.
     """
     # calculate uncorrected pt, mass
     events = set_ak_column_f32(events, "Jet.pt_raw", events.Jet.pt * (1 - events.Jet.rawFactor))
     events = set_ak_column_f32(events, "Jet.mass_raw", events.Jet.mass * (1 - events.Jet.rawFactor))
 
     # build/retrieve lookup providers for JECs and uncertainties
     # NOTE: could also be moved to `jec_setup`, but keep here in case the provider ever needs
@@ -259,17 +304,14 @@
                 events = set_ak_column_f32(events, f"MET.phi_jec_{name}_down", met_phi_down)
 
     return events
 
 
 @jec_coffea.init
 def jec_coffea_init(self: Calibrator) -> None:
-    """
-    Add JEC uncertainty shifts to the list of produced columns.
-    """
     sources = self.uncertainty_sources
     if sources is None:
         sources = self.config_inst.x.jec.uncertainty_sources
 
     # add shifted jet variables
     self.produces |= {
         f"Jet.{shifted_var}_jec_{junc_name}_{junc_dir}"
@@ -290,29 +332,33 @@
             for junc_name in sources
             for junc_dir in ("up", "down")
         }
 
 
 @jec_coffea.requires
 def jec_coffea_requires(self: Calibrator, reqs: dict) -> None:
-    """
-    Add external files bundle (for JEC text files) to dependencies.
-    """
     if "external_files" in reqs:
         return
 
     from columnflow.tasks.external import BundleExternalFiles
     reqs["external_files"] = BundleExternalFiles.req(self.task)
 
 
 @jec_coffea.setup
-def jec_coffea_setup(self: Calibrator, reqs: dict, inputs: dict) -> None:
+def jec_coffea_setup(self: Calibrator, reqs: dict, inputs: dict, reader_targets: InsertableDict) -> None:
     """
-    Determine correct JEC files for task based on config/dataset and inject them
-    into the calibrator function call.
+    Determine correct JEC files for task based on config/dataset and inject them into the calibrator
+    function call.
+
+    :param reqs: Requirement dictionary for this :py:class:`~columnflow.calibration.Calibrator`
+        instance.
+    :param inputs: Additional inputs, currently not used.
+    :param reader_targets: TODO: add docs
+
+    :raises ValueError: If module is provided with more than one JEC uncertainty source file.
     """
     # get external files bundle that contains JEC text files
     bundle = reqs["external_files"]
 
     # make selector for JEC text files based on sample type (and era for data)
     if self.dataset_inst.is_data:
         jec_era = self.dataset_inst.get_aux("jec_era", None)
@@ -383,17 +429,17 @@
 
 #
 # Jet energy resolution smearing
 #
 
 @calibrator(
     uses={
-        "nJet", "Jet.pt", "Jet.eta", "Jet.phi", "Jet.mass", "Jet.genJetIdx",
+        "Jet.pt", "Jet.eta", "Jet.phi", "Jet.mass", "Jet.genJetIdx",
         "Rho.fixedGridRhoFastjetAll", "fixedGridRhoFastjetAll",
-        "nGenJet", "GenJet.pt", "GenJet.eta", "GenJet.phi",
+        "GenJet.pt", "GenJet.eta", "GenJet.phi",
         "MET.pt", "MET.phi",
         attach_coffea_behavior,
     },
     produces={
         "Jet.pt", "Jet.mass",
         "Jet.pt_unsmeared", "Jet.mass_unsmeared",
         "Jet.pt_jer_up", "Jet.pt_jer_down", "Jet.mass_jer_up", "Jet.mass_jer_down",
@@ -403,16 +449,23 @@
     # toggle for propagation to MET
     propagate_met=True,
     # only run on mc
     mc_only=True,
 )
 def jer_coffea(self: Calibrator, events: ak.Array, **kwargs) -> ak.Array:
     """
-    Apply jet energy resolution smearing and calculate shifts for JER scale factor variations.
+    Apply jet energy resolution smearing and calculate shifts for Jet Enery Resolution (JER) scale
+    factor variations.
+
     Follows the recommendations given in https://twiki.cern.ch/twiki/bin/viewauth/CMS/JetResolution.
+
+    The module applies the scale factors associated to the JER and performs the stochastic smearing
+    to make the energy resolution in simulation more realistic.
+
+    :param events: awkward array containing events to process
     """
     # save the unsmeared properties in case they are needed later
     events = set_ak_column_f32(events, "Jet.pt_unsmeared", events.Jet.pt)
     events = set_ak_column_f32(events, "Jet.mass_unsmeared", events.Jet.mass)
 
     # use event numbers in chunk to seed random number generator
     # TODO: use seeds!
@@ -571,46 +624,51 @@
         events = set_ak_column_f32(events, "MET.phi_jer_down", met_phi_down)
 
     return events
 
 
 @jer_coffea.init
 def jer_coffea_init(self: Calibrator) -> None:
-    """
-    Initialization of dynamic components of the jer calibrator.
-    """
     if not self.propagate_met:
         return
 
     self.uses |= {
         "MET.pt", "MET.phi",
     }
     self.produces |= {
         "MET.pt", "MET.phi", "MET.pt_jer_up", "MET.pt_jer_down", "MET.phi_jer_up",
         "MET.phi_jer_down", "MET.pt_unsmeared", "MET.phi_unsmeared",
     }
 
 
 @jer_coffea.requires
 def jer_coffea_requires(self: Calibrator, reqs: dict) -> None:
-    """
-    Add external files bundle (for JR text files) to dependencies.
-    """
     if "external_files" in reqs:
         return
 
     from columnflow.tasks.external import BundleExternalFiles
     reqs["external_files"] = BundleExternalFiles.req(self.task)
 
 
 @jer_coffea.setup
-def jer_coffea_setup(self: Calibrator, reqs: dict, inputs: dict) -> None:
-    """
-    Determine correct JR files for task based on config/dataset and inject them
-    into the calibrator function call.
+def jer_coffea_setup(
+    self: Calibrator,
+    reqs: dict, inputs: dict,
+    reader_targets: InsertableDict,
+) -> None:
+    """
+    Determine correct JER files for task based on config/dataset and inject them into the calibrator
+    function call.
+
+    :param reqs: Requirement dictionary for this :py:class:`~columnflow.calibration.Calibrator`
+        instance.
+    :param inputs: Additional inputs, currently not used.
+    :param reader_targets: TODO: add docs.
+
+    :raises ValueError: If module is provided with more than one JER uncertainty source file.
     """
     # get external files bundle that contains JR text files
     bundle = reqs["external_files"]
 
     resolve_sample = lambda x: x.mc
 
     # pass text files to calibrator method
@@ -642,14 +700,21 @@
 @calibrator(
     uses={jec_coffea, jer_coffea},
     produces={jec_coffea, jer_coffea},
     # toggle for propagation to MET
     propagate_met=True,
 )
 def jets_coffea(self: Calibrator, events: ak.Array, **kwargs) -> ak.Array:
+    """
+    Instance of :py:class:`~columnflow.calibration.Calibrator` that does all relevant calibrations
+    for jets, i.e. JEC and JER. For more information, see :py:class:`~.jec_coffea` and
+    :py:class:`~.jer_coffea`.
+
+    :param events: awkward array containing events to process.
+    """
     # apply jet energy corrections
     events = self[jec_coffea](events, **kwargs)
 
     # apply jer smearing on MC only
     if self.dataset_inst.is_mc:
         events = self[jer_coffea](events, **kwargs)
```

### Comparing `columnflow-0.2.1/columnflow/calibration/util.py` & `columnflow-0.2.2/columnflow/calibration/util.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,17 +15,21 @@
 np = maybe_import("numpy")
 ak = maybe_import("awkward")
 
 
 # https://github.com/scikit-hep/awkward/issues/489\#issuecomment-711090923
 def ak_random(*args, rand_func: Callable) -> ak.Array:
     """
-    Return an awkward array filled with random numbers. The *args* must be broadcastable
-    awkward arrays and will be passed as positional arguments to *rand_func* to obtain the
-    random numbers.
+    Return an awkward array filled with random numbers.
+
+    The *args* must be broadcastable awkward arrays and will be passed as positional arguments to
+    *rand_func* to obtain the random numbers.
+
+    :param rand_func: Callable to generate random numbers from awkward arrays in *args*.
+    :return: awkward array filled with random numbers.
     """
     args = ak.broadcast_arrays(*args)
 
     if hasattr(args[0].layout, "offsets"):
         # pass flat arrays to random function and get random values
         np_randvals = rand_func(*map(flat_np_view, args))
 
@@ -34,26 +38,40 @@
 
     # pass args directly (this may fail for some array types)
     np_randvals = rand_func(*args)
     return ak.from_numpy(np_randvals)
 
 
 def propagate_met(
-    jet_pt1: ak.Array,
+    jet_pt1: (ak.Array),
     jet_phi1: ak.Array,
     jet_pt2: ak.Array,
     jet_phi2: ak.Array,
     met_pt1: ak.Array,
     met_phi1: ak.Array,
 ) -> tuple[ak.Array, ak.Array]:
     """
-    Helper function to compute new MET based on per-jet pts and phis
-    before and after a correction.
+    Helper function to compute new MET based on per-jet pts and phis before and after a correction.
+    Since the pts and phis parameterize the individual jets, the dimensions of the arrays
+    (*jet_pt1*, *jet_phi1*) as well as (*jet_pt2*, *jet_phi2*) must be the same. The pt values are
+    decomposed into their x and y components, which are then propagated to the corresponding
+    contributions to the MET vector
+
+    :param jet_pt1: transverse momentum of first jet(s)
+    :param jet_phi1: azimuthal angle of first jet(s)
+    :param jet_pt2: transverse momentum of second jet(s)
+    :param jet_phi2: azimuthal angle of second jet(s)
+    :param met_pt1: missing transverse momentum (MET)
+    :param met_phi1: azimuthal angle of MET vector
+
+    :raises AssertionError: if arrays (*jet_pt1*, *jet_phi1*) and (*jet_pt2*, *jet_phi2*) have
+        different dimensions.
+    :return: updated values of MET vector, i.e. missing transverse momentum and corresponding
+        azimuthal angle phi.
     """
-
     # avoid unwanted broadcasting
     assert jet_pt1.ndim == jet_phi1.ndim
     assert jet_pt2.ndim == jet_phi2.ndim
 
     # build px and py sums before and after
     jet_px1 = jet_pt1 * np.cos(jet_phi1)
     jet_py1 = jet_pt1 * np.sin(jet_phi1)
```

### Comparing `columnflow-0.2.1/columnflow/columnar_util.py` & `columnflow-0.2.2/columnflow/columnar_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,30 +8,33 @@
 
 __all__ = [
     "mandatory_coffea_columns", "EMPTY_INT", "EMPTY_FLOAT",
     "Route", "RouteFilter", "ArrayFunction", "TaskArrayFunction", "ChunkedIOHandler",
     "eval_item", "get_ak_routes", "has_ak_column", "set_ak_column", "remove_ak_column",
     "add_ak_alias", "add_ak_aliases", "update_ak_array", "flatten_ak_array", "sort_ak_fields",
     "sorted_ak_to_parquet", "attach_behavior", "layout_ak_array", "flat_np_view",
+    "deferred_column", "optional_column",
 ]
 
 import gc
 import re
 import math
 import time
-import copy
 import enum
+import inspect
 import threading
 import multiprocessing
 import multiprocessing.pool
 from functools import partial
 from collections import namedtuple, OrderedDict, defaultdict
 from typing import Sequence, Callable, Any
 
 import law
+import order as od
+from law.util import InsertableDict
 
 from columnflow.util import (
     UNSET, maybe_import, classproperty, DotDict, DerivableMeta, Derivable, pattern_matcher,
     get_source_code,
 )
 
 
@@ -79,28 +82,15 @@
         return eval(f"self{s}")
 
 
 #: ItemEval singleton mimicking a function.
 eval_item = ItemEval()
 
 
-class RouteMeta(type):
-    """
-    Meta class for :py:class:`Route` that prevents instances from being copied when passed to the
-    constructor.
-    """
-
-    def __call__(cls, route: Route | Any | None = None):
-        if isinstance(route, cls):
-            return route
-
-        return super().__call__(route=route)
-
-
-class Route(object, metaclass=RouteMeta):
+class Route(od.TagMixin):
     """
     Route objects describe the location of columns in nested arrays and are basically wrappers
     around a sequence of nested fields. Additionally, they provide convenience methods for
     conversion into column names, either in dot or nano-style underscore format.
 
     The constructor takes another *route* instance, a sequence of strings, or a string in dot format
     to initialize the fields. Most operators are overwritten to work with routes in a tuple-like
@@ -177,15 +167,15 @@
             s_str += f":{s.step}"
         return s_str
 
     @classmethod
     def _join(
         cls,
         sep: str,
-        fields: Sequence[str | int | slice | type(Ellipsis) | tuple | list],
+        fields: Sequence[str | int | slice | type(Ellipsis) | list | tuple],
         _outer: bool = True,
     ) -> str:
         """
         Joins a sequence of *fields* into a string with a certain separator *sep* and returns it.
         """
         s = ""
         for field in fields:
@@ -234,14 +224,20 @@
         cls,
         sep: str,
         column: str,
     ) -> tuple[str | int | slice | type(Ellipsis) | list | tuple]:
         """
         Splits a string at a separator *sep* and returns the fragments, potentially with selection,
         slice and advanced indexing expressions.
+
+        :param sep: Separator to be used to split *column* into subcomponents
+        :param column: Name of the column to be split
+        :raises ValueError: If *column* is malformed, specifically if brackets are not encountered
+            in pairs (i.e. opening backet w/o closing and vice versa).
+        :return: tuple of subcomponents extracted from *column*
         """
         # first extract and replace possibly nested slices
         # note: a regexp would be far cleaner, but there are edge cases which possibly require
         #       sequential regexp evaluations which might be less maintainable
         slices = []
         repl = lambda i: f"__slice_{i}__"
         repl_cre = re.compile(r"^__slice_(\d+)__$")
@@ -287,35 +283,49 @@
         return tuple(parts)
 
     @classmethod
     def split(cls, column: str) -> tuple[str | int | slice | type(Ellipsis) | list | tuple]:
         """
         Splits a string assumed to be in dot format and returns the fragments, potentially with
         selection, slice and advanced indexing expressions.
+
+        :param column: Name of the column to be split
+        :raises ValueError: If *column* is malformed, specifically if brackets
+            are not encountered in pairs (i.e. opening backet w/o closing and vice versa).
+        :return: tuple of subcomponents extracted from *column*
         """
         return cls._split(cls.DOT_SEP, column)
 
     @classmethod
     def split_nano(cls, column: str) -> tuple[str | int | slice | type(Ellipsis) | list | tuple]:
         """
         Splits a string assumed to be in nano-style underscore format and returns the fragments,
         potentially with selection, slice and advanced indexing expressions.
+
+        :param column: Name of the column to be split
+        :raises ValueError: If *column* is malformed, specifically if brackets are not encountered
+            in pairs (i.e. opening backet w/o closing and vice versa).
+        :return: tuple of subcomponents extracted from *column*
         """
         return cls._split(cls.NANO_SEP, column)
 
-    def __init__(self, route=None):
-        super().__init__()
+    def __init__(self, route: Any | None = None, tags: dict | None = None):
+        super().__init__(tags=tags)
 
         # initial storage of fields
         self._fields = []
 
         # use the add method to set the initial value
         if route:
             self.add(route)
 
+            # when route was a Route instance itself, add its tags
+            if isinstance(route, Route):
+                self.add_tag(route.tags)
+
     @property
     def fields(self) -> tuple:
         return tuple(self._fields)
 
     @property
     def column(self) -> str:
         return self.join(self._fields)
@@ -332,28 +342,31 @@
     def string_nano_column(self) -> str:
         return self.join_nano(f for f in self._fields if isinstance(f, str))
 
     def __str__(self) -> str:
         return self.join(self._fields)
 
     def __repr__(self) -> str:
-        return f"<{self.__class__.__name__} '{self}' at {hex(id(self))}>"
+        tags = ""
+        if self.tags:
+            tags = f" (tags={','.join(sorted(self.tags))})"
+        return f"<{self.__class__.__name__} '{self}'{tags} at {hex(id(self))}>"
 
     def __hash__(self) -> int:
         return hash(str(self.fields))
 
     def __len__(self) -> int:
         return len(self._fields)
 
-    def __eq__(self, other: Route | Sequence[str] | str) -> bool:
+    def __eq__(self, other: Route | str | Sequence[str | int | slice | type(Ellipsis) | list]) -> bool:
         if isinstance(other, Route):
             return self.fields == other.fields
-        elif isinstance(other, (list, tuple)):
+        if isinstance(other, (list, tuple)):
             return self.fields == tuple(other)
-        elif isinstance(other, str):
+        if isinstance(other, str):
             return self.column == other
         return False
 
     def __bool__(self) -> bool:
         return len(self._fields) > 0
 
     def __nonzero__(self) -> bool:
@@ -723,15 +736,15 @@
 
 
 def add_ak_alias(
     ak_array: ak.Array,
     src_route: Route | Sequence[str] | str,
     dst_route: Route | Sequence[str] | str,
     remove_src: bool = False,
-    missing_strategy: str = "remove",
+    missing_strategy: str = "original",
 ) -> ak.Array:
     """
     Adds an alias to an awkward array *ak_array* pointing the array at *src_route* to *dst_route*
     and returns a new view with the alias applied.
 
     Note that existing columns referred to by *dst_route* might be overwritten. When *remove_src* is
     *True*, a view of the input array is returned with the column referred to by *src_route*
@@ -739,14 +752,40 @@
     refers to a subfield, e.g. ``("Jet", "pt")``, or a string with dot format (e.g. ``"Jet.pt"``).
 
     In case *src_route* does not exist, *missing_strategy* is applied:
 
         - ``"original"``: If existing, *dst_route* remains unchanged.
         - ``"remove"``: If existing, *dst_route* is removed.
         - ``"raise"``: A *ValueError* is raised.
+
+    Examples:
+
+    .. code-block:: python
+
+        # example 1
+        events = ak.Array(...)  # contains Jet.pt and Jet.pt_jec_up
+
+        events = add_ak_alias(events, "Jet.pt_jec_up", "Jet.pt")
+        # -> events.Jet.pt will now be the same as Jet.pt_jec_up
+
+        events = add_ak_alias(events, "Jet.pt_jec_up", "Jet.pt", remove_src=True)
+        # -> again, events.Jet.pt will now be the same as Jet.pt_jec_up but the latter is removed
+
+
+        # example 2
+        events = ak.Array(...)  # contains only Jet.pt
+
+        events = add_ak_alias(events, "Jet.pt_jec_up", "Jet.pt")
+        # -> the source column "Jet.pt_jec_up" does not exist, so nothing happens
+
+        events = add_ak_alias(events, "Jet.pt_jec_up", "Jet.pt", missing_strategy="raise")
+        # -> an exception will be raised since the source column is missing
+
+        events = add_ak_alias(events, "Jet.pt_jec_up", "Jet.pt", missing_strategy="remove")
+        # -> the destination column "Jet.pt" will be removed as there is no source column to alias
     """
     # check the strategy
     strategies = ("original", "remove", "raise")
     if missing_strategy not in strategies:
         raise ValueError(
             f"unknown missing_strategy '{missing_strategy}', valid values are {strategies}",
         )
@@ -755,24 +794,28 @@
     src_route = Route(src_route)
     dst_route = Route(dst_route)
 
     # check that the src exists
     if has_ak_column(ak_array, src_route):
         # add the alias, potentially overwriting existing columns
         ak_array = set_ak_column(ak_array, dst_route, src_route.apply(ak_array))
+
+        # remove the source column
+        if remove_src:
+            ak_array = remove_ak_column(ak_array, src_route)
+
     else:
+        # the source column does not exist, so apply the missing_strategy
         if missing_strategy == "raise":
+            # complain
             raise ValueError(f"no column found in array for route '{src_route}'")
         if missing_strategy == "remove":
+            # remove the actual destination column
             ak_array = remove_ak_column(ak_array, dst_route)
 
-    # remove the source column
-    if remove_src:
-        ak_array = remove_ak_column(ak_array, src_route)
-
     return ak_array
 
 
 def add_ak_aliases(
     ak_array: ak.Array,
     aliases: dict[Route | Sequence[str] | str, Route | Sequence[str], str],
     **kwargs: dict[str, Any],
@@ -967,93 +1010,84 @@
         parquet highly depend on the order for building internal table schemas, one should always
         make use of this function! Otherwise, operations like file merging might fail due to
         differently ordered schemas.
     """
     # sort fields
     ak_array = sort_ak_fields(ak_array)
 
-    # workaround for https://github.com/dask-contrib/dask-awkward/issues/140
-    # TODO: remove workaround
+    # disable extensionarrays
     kwargs["extensionarray"] = False
-    # end workaround
 
     # TODO: empty fields cannot be saved to parquet, but for that we would need to identify them
     ak.to_parquet(ak_array, *args, **kwargs)
 
 
 def attach_behavior(
     ak_array: ak.Array,
     type_name: str,
     behavior: dict | None = None,
+    keep_fields: Sequence[str] | None = None,
     skip_fields: Sequence[str] | None = None,
 ) -> ak.Array:
     """
     Attaches behavior of type *type_name* to an awkward array *ak_array* and returns it. *type_name*
     must be a key of a *behavior* dictionary which defaults to the "behavior" attribute of
     *ak_array* when present. Otherwise, a *ValueError* is raised.
 
-    By default, all subfields of *ak_array* are kept. For further control, *skip_fields* can contain
-    names or name patterns of fields that are filtered.
+    By default, all subfields of *ak_array* are kept. For further control, *keep_fields*
+    (*skip_fields*) can contain names or name patterns of fields that are kept (filtered).
+    *keep_fields* has priority, i.e., when it is set, *skip_fields* is not considered.
     """
-
     if behavior is None:
         behavior = getattr(ak_array, "behavior", None) or coffea.nanoevents.methods.nanoaod.behavior
         if behavior is None:
             raise ValueError(
                 f"behavior for type '{type_name}' is not set and not existing in input array",
             )
 
     # prepare field skipping
+    if keep_fields and skip_fields:
+        raise Exception("can only pass one of 'keep_fields' and 'skip_fields'")
+
     keep_field = lambda field: True
-    if skip_fields:
-        skip_fields = law.util.make_list(skip_fields)
-        skip_fields = {
-            field for field in ak_array.fields
-            if law.util.multi_match(field, skip_fields)
+    if keep_fields or skip_fields:
+        requested_fields = law.util.make_list(keep_fields or skip_fields)
+        requested_fields = {
+            field
+            for field in ak_array.fields
+            if law.util.multi_match(field, requested_fields)
         }
-        keep_field = lambda field: field not in skip_fields
+        keep_field = (
+            (lambda field: field in requested_fields)
+            if keep_fields else
+            (lambda field: field not in requested_fields)
+        )
 
     return ak.zip(
         {field: ak_array[field] for field in ak_array.fields if keep_field(field)},
         with_name=type_name,
         behavior=behavior,
     )
 
 
 def layout_ak_array(data_array: np.array | ak.Array, layout_array: ak.Array) -> ak.Array:
     """
-    Structures an input *data_array* by making at an awkward array with a layout inferred from
-    *layout_array* and returns it. In particular, this function can be used to create new awkward
-    arrays from existing numpy arrays and forcing a known, arbitrarily ragged shape to it. Example:
+    Takes a *data_array* and structures its contents into the same structure as *layout_array*, with
+    up to one level of nesting. In particular, this function can be used to create new awkward
+    arrays from existing numpy arrays and forcing a known, potentially ragged shape to it. Example:
 
     .. code-block:: python
 
         a = np.array([1.0, 2.0, 3.0, 4.0, 5.0])
         b = ak.Array([[], [0, 0], [], [0, 0, 0]])
 
         c = layout_ak_array(a, b)
         # <Array [[], [1.0, 2.0], [], [3.0, 4.0, 5.0]] type='4 * var * float32'>
     """
-    # flatten and convert to content
-    if isinstance(data_array, np.ndarray):
-        data = ak.contents.NumpyArray(np.reshape(data_array, (-1,)))
-    elif isinstance(data_array, ak.Array):
-        data = ak.flatten(data_array, axis=None)  # might create a copy
-    else:
-        raise TypeError(f"unhandled type of data array {data_array}")
-
-    # infer the offsets
-    if getattr(layout_array, "layout", None) is None:
-        raise ValueError(f"layout array {layout_array} does not have a valid layout")
-    if getattr(layout_array.layout, "offsets", None):
-        offsets = layout_array.layout.offsets
-    else:
-        raise ValueError(f"offsets extraction not implemented for layout array {layout_array}")
-
-    return ak.Array(ak.contents.ListOffsetArray(offsets, data))
+    return ak.unflatten(ak.flatten(data_array, axis=None), ak.num(layout_array, axis=1), axis=0)
 
 
 def flat_np_view(ak_array: ak.Array, axis: int = 1) -> np.array:
     """
     Takes an *ak_array* and returns a fully flattened numpy view. The flattening is applied along
     *axis*. See *ak.flatten* for more info.
 
@@ -1240,14 +1274,32 @@
 
     .. py:classattribute:: PRODUCES
        type: ArrayFunction.IOFlag
 
        Flag that can be used in nested dependencies between array functions to denote columns names
        in the :py:attr:`produces` set.
 
+    .. py:classattribute:: check_used_columns
+       type: bool
+
+       A flag that decides whether, during the actual call, the input array should be checked for
+       the existence of all non-optional columns defined in :py:attr:`uses`. If a column is missing,
+       an exception is raised. A column, represented by a :py:class:`~.Route` object internally, is
+       considered optional if it has a tag ``"optional"`` as, for instance, added by
+       :py:func:`~.optional_column`.
+
+    .. py:classattribute:: check_produced_columns
+       type: bool
+
+       A flag that decides whether, after the actual call, the output array should be checked for
+       the existence of all non-optional columns defined in :py:attr:`produces`. If a column is
+       missing, an exception is raised. A column, represented by a :py:class:`~.Route` object
+       internally, is considered optional if it has a tag ``"optional"`` as, for instance, added by
+       :py:func:`~.optional_column`.
+
     .. py:attribute:: uses_instances
        type: set
 
        The set of used column names or instantiated dependencies to recursively resolve the names of
        used columns. Set during the deferred initialization.
 
     .. py:attribute:: produces_instances
@@ -1298,48 +1350,104 @@
        other instances.
     """
 
     # class-level attributes as defaults
     call_func = None
     init_func = None
     skip_func = None
+
     uses = set()
     produces = set()
+    check_used_columns = True
+    check_produced_columns = True
     _dependency_sets = {"uses", "produces"}
     log_runtime = law.config.get_expanded_boolean("analysis", "log_array_function_runtime")
 
     # flags for declaring inputs (via uses) or outputs (via produces)
     class IOFlag(enum.Flag):
         AUTO = enum.auto()
         USES = enum.auto()
         PRODUCES = enum.auto()
 
-    # shallow wrapper around an objects (a class or instance) and an IOFlag
-    Flagged = namedtuple("Flagged", ["wrapped", "io_flag"])
+    # shallow wrapper around an object (a class or instance) and an IOFlag
+    IOFlagged = namedtuple("IOFlagged", ["wrapped", "io_flag"])
+
+    # shallow wrapper around any object that returns the object itself in its default call method
+    # given an array function instance (can be easily subclassed to return something else)
+    class DeferredColumn(object):
+
+        @classmethod
+        def deferred_column(
+            cls,
+            call_func: Callable[[ArrayFunction], Any | set[Any]] | None = None,
+        ) -> ArrayFunction.DeferredColumn | Callable:
+            """
+            Subclass factory to be used as a decorator wrapping a *call_func* that will be used as
+            the new ``__call__`` method. Note that the use of ``super()`` inside the decorated
+            method should always be done with arguments (i.e., class and instance).
+            """
+            def decorator(
+                call_func: Callable[[ArrayFunction], Any | set[Any]],
+            ) -> ArrayFunction.DeferredColumn:
+                cls_dict = {
+                    "__call__": call_func,
+                    "__doc__": call_func.__doc__,
+                }
+
+                # overwrite __module__ to point to the module of the calling stack
+                frame = inspect.stack()[1]
+                module = inspect.getmodule(frame[0])
+                if module:
+                    cls_dict["__module__"] = module.__name__
+
+                # create a subclass
+                subcls = cls.__class__(call_func.__name__, (cls,), cls_dict)
+
+                return subcls
+
+            return decorator(call_func) if call_func else decorator
+
+        def __init__(self, *columns: Any):
+            super().__init__()
+
+            # save columns as set, specially handling the case where a single set is given
+            self.columns = (
+                columns[0]
+                if len(columns) == 1 and isinstance(columns[0], set)
+                else set(columns)
+            )
+
+        def __call__(self, func: ArrayFunction) -> Any | set[Any]:
+            # default implementation
+            return self.get()
+
+        def get(self) -> Any | set[Any]:
+            # return the first column if there is just one, otherwise all
+            return list(self.columns)[0] if len(self.columns) == 1 else self.columns
 
     @classproperty
-    def AUTO(cls) -> Flagged:
+    def AUTO(cls) -> IOFlagged:
         """
-        Returns a :py:attr:`Flagged` object, wrapping this class and the AUTO flag.
+        Returns a :py:attr:`IOFlagged` object, wrapping this class and the AUTO flag.
         """
-        return cls.Flagged(cls, cls.IOFlag.AUTO)
+        return cls.IOFlagged(cls, cls.IOFlag.AUTO)
 
     @classproperty
-    def USES(cls) -> Flagged:
+    def USES(cls) -> IOFlagged:
         """
-        Returns a :py:attr:`Flagged` object, wrapping this class and the USES flag.
+        Returns a :py:attr:`IOFlagged` object, wrapping this class and the USES flag.
         """
-        return cls.Flagged(cls, cls.IOFlag.USES)
+        return cls.IOFlagged(cls, cls.IOFlag.USES)
 
     @classproperty
-    def PRODUCES(cls) -> Flagged:
+    def PRODUCES(cls) -> IOFlagged:
         """
-        Returns a :py:attr:`Flagged` object, wrapping this class and the PRODUCES flag.
+        Returns a :py:attr:`IOFlagged` object, wrapping this class and the PRODUCES flag.
         """
-        return cls.Flagged(cls, cls.IOFlag.PRODUCES)
+        return cls.IOFlagged(cls, cls.IOFlag.PRODUCES)
 
     @classmethod
     def init(cls, func: Callable[[], None]) -> None:
         """
         Decorator to wrap a function *func* that should be registered as :py:meth:`init_func`
         which is used to initialize *this* instance dependent on specific task attributes. The
         function should not accept positional arguments.
@@ -1360,28 +1468,34 @@
         cls.skip_func = func
 
     def __init__(
         self,
         call_func: Callable | None = law.no_value,
         init_func: Callable | None = law.no_value,
         skip_func: Callable | None = law.no_value,
-        deferred_init: bool | None = True,
+        check_used_columns: bool | None = None,
+        check_produced_columns: bool | None = None,
         instance_cache: dict | None = None,
         log_runtime: bool | None = None,
+        deferred_init: bool | None = True,
         **kwargs,
     ):
         super().__init__()
 
         # add class-level attributes as defaults for unset arguments (no_value)
         if call_func == law.no_value:
             call_func = self.__class__.call_func
         if init_func == law.no_value:
             init_func = self.__class__.init_func
         if skip_func == law.no_value:
             skip_func = self.__class__.skip_func
+        if check_used_columns is not None:
+            self.check_used_columns = check_used_columns
+        if check_produced_columns is not None:
+            self.check_produced_columns = check_produced_columns
         if log_runtime is not None:
             self.log_runtime = log_runtime
 
         # when a custom funcs are passed, bind them to this instance
         if call_func:
             self.call_func = call_func.__get__(self, self.__class__)
         if init_func:
@@ -1495,29 +1609,48 @@
 
         for attr in self._dependency_sets:
             # get the current set of instances, potentially clearing existing ones
             instances = getattr(self, f"{attr}_instances")
             instances.clear()
 
             # go through all dependent objects and create instances of classes, considering caching
-            for obj in getattr(self, attr):
+            objs = list(getattr(self, attr))
+            while objs:
+                obj = objs.pop(0)
+
+                # obj might be a deferred column
+                if isinstance(obj, self.DeferredColumn):
+                    obj = obj(self)
+
+                # when obj is falsy, skip it
+                if not obj:
+                    continue
+
+                # when obj is a set of objects, i.e., it cannot be understood as a Route,
+                # extend the loop and start over, otherwise handle obj as is
+                if isinstance(obj, set):
+                    objs = list(obj) + objs
+                    continue
+
+                # handle other types
                 if ArrayFunction.derived_by(obj) or isinstance(obj, ArrayFunction):
                     obj = add_dep(obj)
                     if obj:
                         added_deps.append(obj.__class__)
-                        instances.add(obj)
-                elif isinstance(obj, self.Flagged):
-                    obj = self.Flagged(add_dep(obj.wrapped), obj.io_flag)
+                        instances.add(self.IOFlagged(obj, self.IOFlag.AUTO))
+
+                elif isinstance(obj, self.IOFlagged):
+                    obj = self.IOFlagged(add_dep(obj.wrapped), obj.io_flag)
                     if obj:
                         added_deps.append(obj.wrapped.__class__)
                         instances.add(obj)
+
                 else:
-                    obj = copy.deepcopy(obj)
-                    if obj:
-                        instances.add(obj)
+                    # here, obj must be anything that is accepted by route
+                    instances.add(obj if isinstance(obj, Route) else Route(obj))
 
         # synchronize dependencies
         # this might remove deps that were present in self.deps already before this method is called
         # but that were not added in the loop above
         if only_update:
             for cls in list(self.deps.keys()):
                 if cls not in added_deps:
@@ -1541,69 +1674,113 @@
         Returns a set of instances of all dependencies. When *include_others* is *True*, also
         non-ArrayFunction types are returned.
         """
         deps = set()
 
         for attr in self._dependency_sets:
             for obj in getattr(self, f"{attr}_instances"):
-                if isinstance(obj, self.Flagged):
+                # strip i/o flag
+                if isinstance(obj, self.IOFlagged):
                     obj = obj.wrapped
                 if isinstance(obj, ArrayFunction):
                     deps.add(obj)
                 elif include_others:
                     deps.add(obj)
 
         return deps
 
-    def _get_columns(self, io_flag: IOFlag, call_cache: set | None = None, debug=False) -> set[str]:
+    def _get_columns(
+        self,
+        io_flag: IOFlag,
+        dependencies: bool = True,
+        _cache: set | None = None,
+    ) -> set[str]:
         if io_flag == self.IOFlag.AUTO:
             raise ValueError("io_flag in internal _get_columns method must not be AUTO")
 
         # start with an empty set
         columns = set()
 
         # init the call cache
-        if call_cache is None:
-            call_cache = set()
+        if _cache is None:
+            _cache = set()
 
         # declare _this_ call cached
-        call_cache.add(self.Flagged(self, io_flag))
+        _cache.add(self.IOFlagged(self, io_flag))
 
         # add columns of all dependent objects
         for obj in (self.uses_instances if io_flag == self.IOFlag.USES else self.produces_instances):
-            if isinstance(obj, (ArrayFunction, self.Flagged)):
+            if isinstance(obj, (ArrayFunction, self.IOFlagged)):
+                # don't propagate to dependencies
+                if not dependencies:
+                    continue
+
                 flagged = obj
                 if isinstance(obj, ArrayFunction):
-                    flagged = self.Flagged(obj, io_flag)
+                    flagged = self.IOFlagged(obj, io_flag)
                 elif obj.io_flag == self.IOFlag.AUTO:
-                    flagged = self.Flagged(obj.wrapped, io_flag)
+                    flagged = self.IOFlagged(obj.wrapped, io_flag)
+
                 # skip when already cached
-                if flagged in call_cache:
+                if flagged in _cache:
                     continue
+
                 # add the columns
-                columns |= flagged.wrapped._get_columns(flagged.io_flag, call_cache=call_cache)
+                columns |= flagged.wrapped._get_columns(flagged.io_flag, _cache=_cache)
             else:
                 columns.add(obj)
 
         return columns
 
-    def _get_used_columns(self, call_cache: set | None = None) -> set[str]:
-        return self._get_columns(io_flag=self.IOFlag.USES, call_cache=call_cache)
+    def _get_used_columns(self, _cache: set | None = None) -> set[str]:
+        return self._get_columns(io_flag=self.IOFlag.USES, _cache=_cache)
 
     @property
     def used_columns(self) -> set[str]:
         return self._get_used_columns()
 
-    def _get_produced_columns(self, call_cache: set | None = None) -> set[str]:
-        return self._get_columns(io_flag=self.IOFlag.PRODUCES, call_cache=call_cache)
+    def _get_produced_columns(self, _cache: set | None = None) -> set[str]:
+        return self._get_columns(io_flag=self.IOFlag.PRODUCES, _cache=_cache)
 
     @property
     def produced_columns(self) -> set[str]:
         return self._get_produced_columns()
 
+    def _check_columns(self, ak_array: ak.Array, io_flag: IOFlag) -> None:
+        """
+        Check if awkward array contains at least one column matching each
+        entry in 'uses' or 'produces' and raise Exception if none were found.
+        """
+        # get own columns, i.e, routes that are non-optional
+        routes = [
+            route
+            for route in self._get_columns(io_flag=io_flag, dependencies=False)
+            if not route.has_tag("optional")
+        ]
+
+        # get missing columns
+        missing = {
+            route
+            for route in routes
+            if not ak_array.layout.form.select_columns(str(route)).columns()
+        }
+
+        # nothing to do when no column is missing
+        if not missing:
+            return
+
+        # raise
+        action = (
+            "receive" if io_flag == self.IOFlag.USES else
+            "produce" if io_flag == self.IOFlag.PRODUCES else
+            "find"
+        )
+        missing = ", ".join(sorted(map(str, missing)))
+        raise Exception(f"'{self.cls_name}' did not {action} any columns matching: {missing}")
+
     def __call__(self, *args, **kwargs):
         """
         Forwards the call to :py:attr:`call_func` with all *args* and *kwargs*. An exception is
         raised if :py:attr:`call_func` is not callable.
         """
         # check if the call_func is callable
         if not callable(self.call_func):
@@ -1612,24 +1789,72 @@
         # raise in case the call is actually being skipped
         if callable(self.skip_func) and self.skip_func():
             raise Exception(
                 f"skip_func of {self} returned True, cannot invoke call_func; skip_func code: \n\n"
                 f"{get_source_code(self.skip_func, indent=4)}",
             )
 
+        # assume first argument is an event array and
+        # check that the 'used' columns are present
+        if self.check_used_columns:
+            # when args is empty (when this method was called with keyword arguments only),
+            # use the first keyword argument
+            first_arg = args[0] if args else list(kwargs.values())[0]
+            self._check_columns(first_arg, self.IOFlag.USES)
+
+        # call and time the wrapped function
         t1 = time.perf_counter()
         try:
-            return self.call_func(*args, **kwargs)
+            results = self.call_func(*args, **kwargs)
         finally:
             if self.log_runtime:
                 duration = time.perf_counter() - t1
                 logger_perf.info(
                     f"runtime of '{self.cls_name}': {law.util.human_duration(seconds=duration)}",
                 )
 
+        # assume result is an event array or tuple with an event array as the first element and
+        # check that the 'produced' columns are present
+        if self.check_produced_columns:
+            result = results[0] if isinstance(results, (tuple, list)) else results
+            self._check_columns(result, self.IOFlag.PRODUCES)
+
+        return results
+
+
+# shorthand
+deferred_column = ArrayFunction.DeferredColumn.deferred_column
+
+
+def optional_column(
+    *routes: Route | Any | set[Route | Any],
+) -> Route | set[Route]:
+    """
+    Takes one or several objects *routes* whose type can be anything that is accepted by the :py:class:`~.Route`
+    constructor, and returns a single or a set of route objects being tagged ``"optional"``.
+    """
+    if not routes:
+        raise Exception("at least one route argument must be given")
+
+    def opt_route(r):
+        route = Route(r)
+        route.add_tag("optional")
+        return route
+
+    # determine if multple objects are given and handle the case where a single set is given
+    multiple = False
+    if len(routes) == 1 and isinstance(routes[0], set):
+        multiple = True
+        routes = routes[0]
+    elif len(routes) > 1:
+        multiple = True
+
+    # create multiple or a single tagged route
+    return set(map(opt_route, routes)) if multiple else opt_route(list(routes)[0])
+
 
 class TaskArrayFunction(ArrayFunction):
     """
     Subclass of :py:class:`ArrayFunction` providing an interface to certain task features such as
     declaring dependent or produced shifts, task requirements, and defining a custom setup
     function. In addition, there is the option to update all these configurations based on task
     attributes.
@@ -1660,37 +1885,42 @@
                 events["Jet", "pt_weighted"] = events.Jet.pt * self.weights
 
         # define requirements that (e.g.) compute the weights
         @my_func.requires
         def requires(self, reqs):
             # fill the requirements dict
             reqs["weights_task"] = SomeWeightsTask.req(self.task)
+            reqs["columns_task"] = SomeColumnsTask.req(self.task)
 
         # define the setup step that loads event weights from the required task
         @my_func.setup
-        def setup(self, inputs):
+        def setup(self, reqs, inputs, reader_targets):
             # load the weights once, inputs is corresponding to what we added to reqs above
             weights = inputs["weights_task"].load(formatter="json")
 
             # save them as an instance attribute
             self.weights = weights
 
+            # fill the reader_targets to be added in an event chunk loop
+            reder_targets["my_columns"] = inputs["columns_task"]["columns"]
+
         # call my_func on a chunk of events
         inst = my_func()
         inst(events)
 
     For a possible implementation, see :py:mod:`columnflow.production.pileup`.
 
     .. note::
 
         The above example uses explicit subclassing, mixed with decorator usage to extend the class.
         This is most certainly never used in practice. Instead, please either consider defining the
         class the normal way, or use a decorator to wrap the main callable first and by that
-        creating the class as done by the :py:class:`Calibrator`, :py:class:`Selector` and
-        :py:class:`Producer` interfaces.
+        creating the class as done by the :py:class:`~columnflow.calibration.Calibrator`,
+        :py:class:`~columnflow.selection.Selector` and :py:class:`~columnflow.production.Producer`
+        interfaces.
 
     .. py:classattribute:: shifts
        type: set
 
        The set of dependent or produced shifts, or other dependencies to recursively resolve the
        names of shifts.
 
@@ -1764,14 +1994,16 @@
         Decorator to wrap a function *func* that should be registered as :py:meth:`setup_func`
         which is used to perform a custom setup of objects. The function should accept two
         positional arguments:
 
             - *reqs*, a dictionary containing the required tasks as defined by the custom
               :py:meth:`requires_func`.
             - *inputs*, a dictionary containing the outputs created by the tasks in *reqs*.
+            - *reader_targets*, an InsertableDict containing the targets to be included
+              in an event chunk loop
 
         The decorator does not return the wrapped function.
         """
         cls.setup_func = func
 
     def __init__(
         self,
@@ -1824,93 +2056,101 @@
         """
         # add inst_dict when cls is a TaskArrayFunction itself
         if TaskArrayFunction.derived_by(cls):
             kwargs.setdefault("inst_dict", self.inst_dict)
 
         return super().instantiate_dependency(cls, **kwargs)
 
-    def _get_all_shifts(self, call_cache: set | None = None) -> set[str]:
+    def _get_all_shifts(self, _cache: set | None = None) -> set[str]:
         # init the call cache
-        if call_cache is None:
-            call_cache = set()
+        if _cache is None:
+            _cache = set()
 
         # add shifts and consider _this_ call cached
         shifts = {
             shift
             for shift in self.shifts
-            if not isinstance(shift, (ArrayFunction, self.Flagged))
+            if not isinstance(shift, (ArrayFunction, self.IOFlagged))
         }
-        call_cache.add(self)
+        _cache.add(self)
 
         # add shifts of all dependent objects
         for obj in self.get_dependencies(include_others=False):
             if isinstance(obj, TaskArrayFunction):
-                if obj not in call_cache:
-                    call_cache.add(obj)
-                    shifts |= obj._get_all_shifts(call_cache=call_cache)
+                if obj not in _cache:
+                    _cache.add(obj)
+                    shifts |= obj._get_all_shifts(_cache=_cache)
 
         return shifts
 
     @property
     def all_shifts(self) -> set[str]:
         return self._get_all_shifts()
 
     def run_requires(
         self,
         reqs: dict | None = None,
-        call_cache: set | None = None,
+        _cache: set | None = None,
     ) -> dict:
         """
         Recursively runs the :py:meth:`requires_func` of this instance and all dependencies. *reqs*
         defaults to an empty dictionary which should be filled to store the requirements.
         """
         # default requirements
         if reqs is None:
             reqs = {}
 
         # create the call cache
-        if call_cache is None:
-            call_cache = set()
+        if _cache is None:
+            _cache = set()
 
         # run this instance's requires function
         if callable(self.requires_func):
             self.requires_func(reqs)
 
         # run the requirements of all dependent objects
         for dep in self.get_dependencies():
-            if dep not in call_cache:
-                call_cache.add(dep)
-                dep.run_requires(reqs=reqs, call_cache=call_cache)
+            if dep not in _cache:
+                _cache.add(dep)
+                dep.run_requires(reqs=reqs, _cache=_cache)
 
         return reqs
 
     def run_setup(
         self,
         reqs: dict,
         inputs: dict,
-        call_cache: set | None = None,
-    ) -> None:
+        reader_targets: InsertableDict[str, law.FileSystemFileTarget] | None = None,
+        _cache: set | None = None,
+    ) -> dict[str, law.FileSystemTarget]:
         """
         Recursively runs the :py:meth:`setup_func` of this instance and all dependencies. *reqs*
         corresponds to the requirements created by :py:func:`run_requires`, and *inputs* are their
-        outputs.
+        outputs. *reader_targets* defaults to an empty InsertableDict which should be filled to store targets
+        of columnar data that are to be included in an event chunk loop
         """
+        # default column targets
+        if reader_targets is None:
+            reader_targets = {}
+
         # create the call cache
-        if call_cache is None:
-            call_cache = set()
+        if _cache is None:
+            _cache = set()
 
         # run this instance's setup function
         if callable(self.setup_func):
-            self.setup_func(reqs, inputs)
+            self.setup_func(reqs, inputs, reader_targets)
 
         # run the setup of all dependent objects
         for dep in self.get_dependencies():
-            if dep not in call_cache:
-                call_cache.add(dep)
-                dep.run_setup(reqs, inputs, call_cache=call_cache)
+            if dep not in _cache:
+                _cache.add(dep)
+                dep.run_setup(reqs, inputs, reader_targets, _cache=_cache)
+
+        return reader_targets
 
     def __call__(
         self,
         *args,
         call_cache: bool | defaultdict | None = None,
         call_force: bool | None = None,
         n_return: int = 1,
@@ -1937,15 +2177,15 @@
             if call_cache[self] > 0 and not call_force:
                 return args[0] if n_return == 1 else args[:n_return]
 
             # increase the count and set kwargs for the call downstream
             call_cache[self] += 1
 
         # stack all kwargs
-        kwargs = {"call_cache": call_cache, **kwargs}
+        kwargs = {**kwargs, "call_cache": call_cache}
 
         return super().__call__(*args, **kwargs)
 
 
 class NoThreadPool(object):
     """
     Dummy implementation that mimics parts of the usual thread pool interface but instead of
@@ -1960,18 +2200,18 @@
 
         def ready(self) -> bool:
             return True
 
         def get(self) -> Any:
             return self.return_value
 
-    def __init__(self, processes):
+    def __init__(self, processes: int):
         super().__init__()
 
-        self.processes = processes
+        self._processes = processes
         self.opened = True
 
     def __enter__(self) -> NoThreadPool:
         if not self.opened:
             raise Exception(f"cannot enter closed {self.__class__.__name__}")
 
         return self
@@ -1981,15 +2221,15 @@
 
     def close(self) -> None:
         self.opened = False
 
     def terminate(self) -> None:
         return
 
-    def apply_async(self, func, args=(), kwargs=None) -> SyncResult:
+    def apply_async(self, func: Callable, args=(), kwargs=None) -> SyncResult:
         if not self.opened:
             raise Exception(f"cannot apply_async on closed {self.__class__.__name__}")
 
         return self.SyncResult(func(*args, **(kwargs or {})))
 
 
 class TaskQueue(object):
@@ -2150,30 +2390,14 @@
                         self.partition_cache[p].array = None
 
             # add part for concatenation using entry info
             div_start, div_stop = self.dak_array.divisions[p:p + 2]
             part_start = max(entry_start - div_start, 0)
             part_stop = min(entry_stop - div_start, div_stop - div_start)
             parts.append(arr[part_start:part_stop])
-            # workaround for https://github.com/dask-contrib/dask-awkward/issues/140
-            # make the array non-optional, assuming it is not meant to be optional
-            # TODO: remove this workaround once this other workaround is removed as well:
-            # https://github.com/uhh-cms/columnflow/blob/89f3429bbc4349ee2269fae497f3bf69a0b06ed3/columnflow/columnar_util.py#L957  # noqa
-            # skip null-filling for completely empty arrays
-            if not parts[-1].layout.contents:
-                continue
-            if getattr(parts[-1], "fields", None) and ak.any(ak.ravel(ak.is_none(parts[-1]))):
-                logger.warning(
-                    f"None values detected in chunk {chunk_index} of file {self.path} during "
-                    "dask_awkward materialization that were filled with zeros while reading; "
-                    "this is a workaround in columnflow to prevent optional types in arrays; "
-                    "for now, please make sure that files are not written with optional types!",
-                )
-            parts[-1] = ak.fill_none(parts[-1], 0)
-            # end workaround
 
         # construct the full array
         arr = parts[0] if len(parts) == 1 else ak.concatenate(parts, axis=0)
 
         del parts
         gc.collect()
 
@@ -2201,15 +2425,15 @@
     and the index of the chunk itself) are accessed by iterating through a handler instance. Also,
     this handler allows interactions with the internal queue handling tasks in multiple-threads to
     effectively write output chunks within the same pool of threads.
 
     The content to load is configurable through *source*, which can be a file path or an opened file
     object, and a *source_type*, which defines how the *source* should be opened and traversed for
     chunking. See the classmethods ``open_...`` and ``read_...`` below for implementation details
-    and :py:meth:`get_source_handlers` for a list of currently supported sources.
+    and :py:meth:`get_source_handler` for a list of currently supported sources.
 
     Example:
 
     .. code-block:: python
 
         # iterate through a single file
         # (creating the handler and iterating through it in the same line)
@@ -2247,15 +2471,15 @@
     *read_options* internally (source type dependent).
 
     If *source* refers to a single object, *source_type*, *open_options*, *read_options* and
     *read_columns* should be single values as well. Otherwise, if *source* is a sequence of sources,
     the other arguments can be sequences as well with the same length.
 
     During iteration, before chunks are yielded, an optional message *iter_message* is printed when
-    set, receiving the respective :py:class:`ChunkedIOHandler.ChunkPosition` as the field *pos* for
+    set, receiving the respective :py:class:`~ChunkedIOHandler.ChunkPosition` as the field *pos* for
     formatting.
     """
 
     # source handler container
     SourceHandler = namedtuple(
         "SourceHandler",
         ["type", "open", "close", "read"],
@@ -2355,15 +2579,15 @@
     def create_chunk_position(
         cls,
         n_entries: int,
         chunk_size: int,
         chunk_index: int,
     ) -> ChunkPosition:
         """
-        Creates and returns a *ChunkPosition* object based on the total number of entries
+        Creates and returns a :py:attr:`ChunkPosition` object based on the total number of entries
         *n_entries*, the maximum *chunk_size*, and the index of the chunk *chunk_index*.
         """
         # determine the start of stop of this chunk
         if n_entries == 0:
             entry_start = 0
             entry_stop = 0
         else:
@@ -2386,29 +2610,29 @@
         When *source_type* is *None* but an arbitrary *source* is set, the type is derived from that
         object, and an exception is raised in case no type can be inferred.
 
         Currently supported source types are:
 
             - "uproot_root"
             - "coffea_root"
-            - "coffea_parquet" (currently unsupported)
+            - "coffea_parquet"
             - "awkward_parquet"
         """
         if source_type is None:
             if isinstance(source, uproot.ReadOnlyDirectory):
                 # uproot file
                 source_type = "uproot_root"
             elif isinstance(source, str):
                 # file path, guess based on extension
                 if source.endswith(".root"):
                     # priotize coffea nano events
                     source_type = "coffea_root"
                 elif source.endswith(".parquet"):
-                    # priotize coffea nano events
-                    source_type = "coffea_parquet"
+                    # priotize awkward nano events
+                    source_type = "awkward_parquet"
 
             if not source_type:
                 raise Exception(f"could not determine source_type from source '{source}'")
 
         if source_type == "uproot_root":
             return cls.SourceHandler(
                 source_type,
@@ -2419,21 +2643,21 @@
         if source_type == "coffea_root":
             return cls.SourceHandler(
                 source_type,
                 cls.open_coffea_root,
                 cls.close_coffea_root,
                 cls.read_coffea_root,
             )
-        # if source_type == "coffea_parquet":
-        #     return cls.SourceHandler(
-        #         source_type,
-        #         cls.open_coffea_parquet,
-        #         cls.close_coffea_parquet,
-        #         cls.read_coffea_parquet,
-        #     )
+        if source_type == "coffea_parquet":
+            return cls.SourceHandler(
+                source_type,
+                cls.open_coffea_parquet,
+                cls.close_coffea_parquet,
+                cls.read_coffea_parquet,
+            )
         if source_type == "awkward_parquet":
             return cls.SourceHandler(
                 source_type,
                 cls.open_awkward_parquet,
                 cls.close_awkward_parquet,
                 cls.read_awkward_parquet,
             )
@@ -2592,78 +2816,105 @@
 
         # inject read_columns
         if read_columns and (
             "iteritems_options" not in read_options or
             "filter_name" not in read_options["iteritems_options"]
         ):
             filter_name = [Route(s).string_nano_column for s in read_columns]
+
+            # add names prefixed with an 'n' to the list of columns to read
+            # (needed to construct the nested list structure of jagged columns)
+            maybe_jagged_fields = {Route(s)[0] for s in read_columns}
+            filter_name.extend(
+                f"n{field}"
+                for field in maybe_jagged_fields
+            )
+
+            # filter on these column names when reading
             read_options.setdefault("iteritems_options", {})["filter_name"] = filter_name
 
         # read the events chunk into memory
         chunk = coffea.nanoevents.NanoEventsFactory.from_root(
             source_object,
             entry_start=chunk_pos.entry_start,
             entry_stop=chunk_pos.entry_stop,
             **read_options,
         ).events()
 
         return chunk
 
-    # @classmethod
-    # def open_coffea_parquet(
-    #     cls,
-    #     source: str,
-    #     open_options: dict | None = None,
-    #     read_columns: set[str | Route] | None = None,
-    # ) -> tuple[str, int]:
-    #     """
-    #     Given a parquet file located at *source*, returns a 2-tuple *(source, entries)*. Passing
-    #     *open_options* has no effect.
-    #
-    #     TODO: use read_columns?
-    #     """
-    #     return (source, pq.ParquetFile(source).metadata.num_rows)
-
-    # @classmethod
-    # def close_coffea_parquet(
-    #     cls,
-    #     source_object: str,
-    # ) -> None:
-    #     """
-    #     This is a placeholder method and has no effect.
-    #     """
-    #     return
-
-    # @classmethod
-    # def read_coffea_parquet(
-    #     cls,
-    #     source_object: str,
-    #     chunk_pos: ChunkPosition,
-    #     read_options: dict | None = None,
-    #     read_columns: set[str | Route] | None = None,
-    # ) -> coffea.nanoevents.methods.base.NanoEventsArray:
-    #     """
-    #     Given a the location of a parquet file *source_object*, returns an awkward array chunk
-    #     referred to by *chunk_pos*, assuming nanoAOD structure. *read_options* are passed to
-    #     *coffea.nanoevents.NanoEventsFactory.from_parquet*.
-    #
-    #     TODO: use read_columns?
-    #     """
-    #     # TODO: default read options? go via dak and preloaded?
-    #
-    #     # read the events chunk into memory
-    #     chunk = coffea.nanoevents.NanoEventsFactory.from_parquet(
-    #         source_object,
-    #         entry_start=chunk_pos.entry_start,
-    #         entry_stop=chunk_pos.entry_stop,
-    #         schemaclass=coffea.nanoevents.NanoAODSchema,
-    #         **(read_options or {}),
-    #     ).events()
+    @classmethod
+    def open_coffea_parquet(
+        cls,
+        source: str,
+        open_options: dict | None = None,
+        read_columns: set[str | Route] | None = None,
+    ) -> tuple[str, int]:
+        """
+        Given a parquet file located at *source*, returns a 2-tuple *(source, entries)*. Passing
+        *open_options* or *read_columns* has no effect.
+        """
+        return (source, pq.ParquetFile(source).metadata.num_rows)
+
+    @classmethod
+    def close_coffea_parquet(
+        cls,
+        source_object: str,
+    ) -> None:
+        """
+        This is a placeholder method and has no effect.
+        """
+        return
+
+    @classmethod
+    def read_coffea_parquet(
+        cls,
+        source_object: str,
+        chunk_pos: ChunkPosition,
+        read_options: dict | None = None,
+        read_columns: set[str | Route] | None = None,
+    ) -> coffea.nanoevents.methods.base.NanoEventsArray:
+        """
+        Given a the location of a parquet file *source_object*, returns an awkward array chunk
+        referred to by *chunk_pos*, assuming nanoAOD structure. *read_options* are passed to
+        ``coffea.nanoevents.NanoEventsFactory.from_parquet``. *read_columns* are converted to
+        strings and, if not already present, added as nested field
+        ``parquet_options.read_dictionary`` to *read_options*.
+        """
+        # default read options
+        read_options = read_options or {}
+        read_options["runtime_cache"] = None
+        read_options["persistent_cache"] = None
 
-    #     return chunk
+        # inject read_columns
+        if read_columns and (
+            "parquet_options" not in read_options or
+            "read_dictionary" not in read_options["parquet_options"]
+        ):
+            read_dictionary = [Route(s).string_column for s in read_columns]
+
+            # add names prefixed with an 'n' to the list of columns to read
+            # (needed to construct the nested list structure of jagged columns)
+            maybe_jagged_fields = {Route(s)[0] for s in read_columns}
+            read_dictionary.extend(
+                f"n{field}"
+                for field in maybe_jagged_fields
+            )
+
+            read_options.setdefault("parquet_options", {})["read_dictionary"] = read_dictionary
+
+        # read the events chunk into memory
+        chunk = coffea.nanoevents.NanoEventsFactory.from_parquet(
+            source_object,
+            entry_start=chunk_pos.entry_start,
+            entry_stop=chunk_pos.entry_stop,
+            **read_options,
+        ).events()
+
+        return chunk
 
     @classmethod
     def open_awkward_parquet(
         cls,
         source: str,
         open_options: dict | None = None,
         read_columns: set[str | Route] | None = None,
@@ -2701,15 +2952,15 @@
         """
         source_object.close()
 
     @classmethod
     def read_awkward_parquet(
         cls,
         source_object: DaskArrayReader,
-        chunk_pos: ChunkPosition,
+        chunk_pos: ChunkedIOHandler.ChunkPosition,
         read_options: dict | None = None,
         read_columns: set[str | Route] | None = None,
     ) -> ak.Array:
         """
         Given a :py:class:`DaskArrayReader` *source_object*, returns the chunk referred to by
         *chunk_pos* as a full copy loaded into memory. Passing neither *read_options* nor
         *read_columns* has an effect.
```

### Comparing `columnflow-0.2.1/columnflow/inference/__init__.py` & `columnflow-0.2.2/columnflow/inference/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,15 @@
             data_from_processes: []
             mc_stats: 10
             processes:
               - name: HH
                 config_process: hh
                 is_signal: True
                 config_mc_datasets: [hh_ggf]
+                scale: 1.0
                 parameters:
                   - name: lumi
                     type: rate_gauss
                     effect: 1.02
                     config_shift_source: null
                   - name: pu
                     type: rate_gauss
@@ -139,14 +140,15 @@
                     type: shape
                     effect: 1.0
                     config_shift_source: minbias_xs
               - name: tt
                 is_signal: False
                 config_process: ttbar
                 config_mc_datasets: [tt_sl, tt_dl, tt_fh]
+                scale: 1.0
                 parameters:
                   - name: lumi
                     type: rate_gauss
                     effect: 1.02
                     config_shift_source: null
 
           - name: cat2
@@ -200,14 +202,38 @@
             str_repr = lambda dumper, data: dumper.represent_str(str(data))
             self.add_representer(ParameterType, str_repr)
 
         def ignore_aliases(self, *args, **kwargs) -> bool:
             return True
 
     @classmethod
+    def inference_model(
+        cls,
+        func: Callable | None = None,
+        bases=(),
+        **kwargs,
+    ) -> DerivableMeta | Callable:
+        """
+        Decorator for creating a new :py:class:`InferenceModel` subclass with additional, optional
+        *bases* and attaching the decorated function to it as ``init_func``. All additional *kwargs* are
+        added as class members of the new subclasses.
+        """
+        def decorator(func: Callable) -> DerivableMeta:
+            # create the class dict
+            cls_dict = {"init_func": func}
+            cls_dict.update(kwargs)
+
+            # create the subclass
+            subclass = cls.derive(func.__name__, bases=bases, cls_dict=cls_dict)
+
+            return subclass
+
+        return decorator(func) if func else decorator
+
+    @classmethod
     def model_spec(cls) -> DotDict:
         """
         Returns a dictionary representing the top-level structure of the model.
 
             - *categories*: List of :py:meth:`category_spec` objects.
             - *parameter_groups*: List of :py:meth:`paramter_group_spec` objects.
         """
@@ -252,28 +278,31 @@
     @classmethod
     def process_spec(
         cls,
         name: str,
         config_process: str | None = None,
         is_signal: bool = False,
         config_mc_datasets: Sequence[str] | None = None,
+        scale: float | int = 1.0,
     ) -> DotDict:
         """
         Returns a dictionary representing a process, forwarding all arguments.
 
             - *name*: The name of the process in the model.
             - *is_signal*: A boolean flag deciding whether this process describes signal.
             - *config_process*: The name of the source process in the config to use.
             - *config_mc_datasets*: List of names of MC datasets in the config to use.
+            - *scale*: A float value to scale the process, defaulting to 1.0.
         """
         return DotDict([
             ("name", str(name)),
             ("is_signal", bool(is_signal)),
             ("config_process", str(config_process) if config_process else None),
             ("config_mc_datasets", list(map(str, config_mc_datasets or []))),
+            ("scale", float(scale)),
             ("parameters", []),
         ])
 
     @classmethod
     def parameter_spec(
         cls,
         name: str,
@@ -350,17 +379,18 @@
 
         # store attributes
         self.config_inst = config_inst
 
         # model info
         self.model = self.model_spec()
 
-        # custom init function when set
+        # custom init function when set, always followed by the cleanup
         if callable(self.init_func):
             self.init_func()
+            self.cleanup()
 
     def to_yaml(self, stream: TextIO | None = None) -> str | None:
         """
         Writes the content of the :py:attr:`model` into a file-like object *stream* when given, and
         returns a string representation otherwise.
         """
         return yaml.dump(self.model, stream=stream, Dumper=self.YamlDumper)
@@ -1280,29 +1310,31 @@
         """
         parameters = self.get_parameters(parameter=parameter, process=process, category=category)
         for category_name, parameters in parameters.items():
             for process_name, parameters in parameters.items():
                 for parameter in parameters:
                     yield (category_name, process_name, parameter)
 
+    #
+    # other helpers
+    #
 
-def inference_model(
-    func: Callable | None = None,
-    bases=(),
-    **kwargs,
-) -> DerivableMeta | Callable:
-    """
-    Decorator for creating a new :py:class:`InferenceModel` subclass with additional, optional
-    *bases* and attaching the decorated function to it as ``init_func``. All additional *kwargs* are
-    added as class members of the new subclasses.
-    """
-    def decorator(func: Callable) -> DerivableMeta:
-        # create the class dict
-        cls_dict = {"init_func": func}
-        cls_dict.update(kwargs)
-
-        # create the subclass
-        subclass = InferenceModel.derive(func.__name__, bases=bases, cls_dict=cls_dict)
+    def scale_process(
+        self,
+        scale: int | float,
+        process: str | Sequence[str] | None = None,
+        category: str | Sequence[str] | None = None,
+    ) -> bool:
+        """
+        Sets the scale attribute of all processes whose names match *process*, optionally in all
+        categories whose names match *category*, to *scale*. Returns *True* if at least one process
+        was found and scale, and *False* otherwise.
+        """
+        found = False
+        for _, process in self.iter_processes(process=process, category=category):
+            process.scale = float(scale)
+            found = True
+        return found
 
-        return subclass
 
-    return decorator(func) if func else decorator
+# shorthand
+inference_model = InferenceModel.inference_model
```

### Comparing `columnflow-0.2.1/columnflow/inference/cms/datacard.py` & `columnflow-0.2.2/columnflow/inference/cms/datacard.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import os
 from collections import OrderedDict
 from typing import Sequence, Any
 
 import law
 
+from columnflow import __version__ as cf_version
 from columnflow.inference import InferenceModel, ParameterType, ParameterTransformation
 from columnflow.util import DotDict, maybe_import, real_path, ensure_dir, safe_div
 
 
 np = maybe_import("np")
 hist = maybe_import("hist")
 uproot = maybe_import("uproot")
@@ -79,23 +80,28 @@
         cat_objects = [self.inference_model_inst.get_category(cat_name) for cat_name in rates]
 
         # prepare blocks and lines to write
         blocks = DotDict()
         separators = set()
         empty_lines = set()
 
+        # extra info
+        blocks.extra = [f"# created with columnflow v{cf_version}"]
+        empty_lines.add("extra")
+
         # counts block
         blocks.counts = [("imax", "*"), ("jmax", "*"), ("kmax", "*")]
         separators.add("counts")
 
         # shape lines
         blocks.shapes = [("shapes", "*", "*", shapes_path_ref, nom_pattern, syst_pattern)]
         separators.add("shapes")
 
         # observations
+        blocks.observations = []
         if all("data" in _rates for _rates in rates.values()):
             blocks.observations = [
                 ("bin", list(rates)),
                 ("observation", [
                     round(_rates["data"], self.rate_precision)
                     for _rates in rates.values()
                 ]),
@@ -270,15 +276,16 @@
                 # default value when True
                 if isinstance(mc_stats, bool):
                     mc_stats = 10
                 mc_stats_list = list(map(str, law.util.make_list(mc_stats)))
                 blocks.mc_stats.append([cat_obj.name, "autoMCStats"] + mc_stats_list)
 
         # prettify blocks
-        blocks.observations = self.align_lines(list(blocks.observations))
+        if blocks.observations:
+            blocks.observations = self.align_lines(list(blocks.observations))
         if blocks.tabular_parameters:
             blocks.rates, blocks.tabular_parameters = self.align_rates_and_parameters(
                 list(blocks.rates),
                 list(blocks.tabular_parameters),
             )
         else:
             blocks.rates = self.align_lines(list(blocks.rates))
@@ -359,31 +366,35 @@
             for proc_name, _hists in hists.items():
                 __effects = _effects[proc_name] = OrderedDict()
 
                 # defer the handling of data to the end
                 if proc_name == "data":
                     continue
 
+                # get the process scale (usually 1)
+                proc_obj = self.inference_model_inst.get_process(proc_name, category=cat_name)
+                scale = proc_obj.scale
+
                 # nominal shape
-                h_nom = _hists["nominal"].copy()
+                h_nom = _hists["nominal"].copy() * scale
                 if fill_empty_bins:
                     fill_empty(h_nom)
                 nom_name = nom_pattern.format(category=cat_name, process=proc_name)
                 out_file[nom_name] = h_nom
                 _rates[proc_name] = h_nom.sum().value
 
                 # helper to return the two variations
                 def get_shapes(param_name):
                     __hists = _hists[param_name]
                     if "up" not in __hists or "down" not in __hists:
                         raise Exception(
                             f"shapes of parameter '{param_name}' for process '{proc_name}' "
                             f"in category '{cat_name}' misconfigured: {__hists}",
                         )
-                    return __hists["down"], __hists["up"]
+                    return __hists["down"] * scale, __hists["up"] * scale
 
                 # go through all parameters and check if varied shapes need to be processed
                 for _, _, param_obj in self.inference_model_inst.iter_parameters(category=cat_name, process=proc_name):
                     # read or create the varied histograms, or skip the parameter
                     if param_obj.type.is_shape:
                         # the source of the shape depends on the transformation
                         if param_obj.transformations.any_from_rate:
```

### Comparing `columnflow-0.2.1/columnflow/ml/__init__.py` & `columnflow-0.2.2/columnflow/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.1/columnflow/plotting/plot_all.py` & `columnflow-0.2.2/columnflow/plotting/plot_all.py`

 * *Files 3% similar despite different names*

```diff
@@ -259,19 +259,22 @@
             "wip": "Work in progress",
             "pre": "Preliminary",
             "pw": "Private work",
             "sim": "Simulation",
             "simwip": "Simulation work in progress",
             "simpre": "Simulation preliminary",
             "simpw": "Simulation private work",
+            "od": "OpenData",
+            "odwip": "OpenData work in progress",
+            "odpw": "OpenData private work",
             "public": "",
         }
         cms_label_kwargs = {
             "ax": ax,
-            "llabel": label_options[cms_label],
+            "llabel": label_options.get(cms_label, cms_label),
             "fontsize": 22,
             "data": False,
         }
 
         cms_label_kwargs.update(style_config.get("cms_label_cfg", {}))
         mplhep.cms.label(**cms_label_kwargs)
```

### Comparing `columnflow-0.2.1/columnflow/plotting/plot_functions_1d.py` & `columnflow-0.2.2/columnflow/plotting/plot_functions_1d.py`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.1/columnflow/plotting/plot_util.py` & `columnflow-0.2.2/columnflow/plotting/plot_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -282,15 +282,15 @@
             "kwargs": {
                 "norm": data_norm,
                 "label": "Data",
                 "yerr": False if any(data_hide_errors) else None,
             },
         }
         if h_mc is not None:
-            plot_config["ratio_kwargs"] = {
+            plot_config["data"]["ratio_kwargs"] = {
                 "norm": h_mc.values() * data_norm / mc_norm,
                 "yerr": False if any(data_hide_errors) else None,
             }
 
     return plot_config
 
 
@@ -298,7 +298,61 @@
     """ get a relative position between a min and max value based on the scale """
     if logscale:
         value = 10 ** ((math.log10(maximum) - math.log10(minimum)) * factor + math.log10(minimum))
     else:
         value = (maximum - minimum) * factor + minimum
 
     return value
+
+
+def reduce_with(spec: str | float | callable, values: list[float]) -> float:
+    """
+    Reduce an array of *values* to a single value using the function indicated
+    by *spec*. Intended as a helper for resolving range specifications supplied
+    as strings.
+
+    Supported specifiers are:
+
+      * 'min': minimum value
+      * 'max': maximum value
+      * 'maxabs': the absolute value of the maximum or minimum, whichever is larger
+      * 'minabs': the absolute value of the maximum or minimum, whichever is smaller
+
+    A hyphen (``-``) can be prefixed to any specifier to return its negative.
+
+    Callables can be passed as *spec* and should take a single array-valued argument
+    and return a single value. Floats passes as specifiers will be returned directly.
+    """
+
+    # if callable, apply to array
+    if callable(spec):
+        return spec(values)
+
+    # if not a string, assume fixed literal and return
+    if not isinstance(spec, str):
+        return spec
+
+    # determine sign
+    factor = 1.
+    if spec.startswith("-"):
+        spec = spec[1:]
+        factor = -1.
+
+    if spec not in reduce_with.funcs:
+        available = ", ".join(reduce_with.funcs)
+        raise ValueError(
+            f"unknown reduction function '{spec}'. "
+            f"Available: {available}",
+        )
+
+    func = reduce_with.funcs[spec]
+    values = np.asarray(values)
+
+    return factor * func(values)
+
+
+reduce_with.funcs = {
+    "min": lambda v: np.nanmin(v),
+    "max": lambda v: np.nanmax(v),
+    "maxabs": lambda v: max(abs(np.nanmax(v)), abs(np.nanmin(v))),
+    "minabs": lambda v: min(abs(np.nanmax(v)), abs(np.nanmin(v))),
+}
```

### Comparing `columnflow-0.2.1/columnflow/production/categories.py` & `columnflow-0.2.2/columnflow/production/categories.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # coding: utf-8
 
 """
 Column production methods related defining categories.
 """
 
+from __future__ import annotations
+
 from collections import defaultdict
 
 import law
 
 from columnflow.selection import Selector
 from columnflow.production import Producer, producer
 from columnflow.util import maybe_import
@@ -17,21 +19,25 @@
 np = maybe_import("numpy")
 ak = maybe_import("awkward")
 
 logger = law.logger.get_logger(__name__)
 
 
 @producer(produces={"category_ids"})
-def category_ids(self: Producer, events: ak.Array, **kwargs) -> ak.Array:
+def category_ids(
+    self: Producer,
+    events: ak.Array,
+    target_events: ak.Array | None = None,
+    **kwargs,
+) -> ak.Array:
     """
     Assigns each event an array of category ids.
     """
     category_ids = []
 
-    # TODO: we maybe don't want / need to loop through all leaf categories
     for cat_inst in self.config_inst.get_leaf_categories():
         # start with a true mask
         cat_mask = np.ones(len(events)) > 0
 
         # loop through selectors
         for selector in self.category_to_selectors[cat_inst]:
             # run the selector for events that still match the mask, then AND concat
@@ -39,22 +45,26 @@
             cat_mask[cat_mask] &= np.asarray(_cat_mask == 1)
 
             # stop if no events are left
             if not ak.any(cat_mask):
                 break
 
         # covert to nullable array with the category ids or none, then apply ak.singletons
-        ids = ak.where(cat_mask, np.float32(cat_inst.id), np.float32(np.nan))
+        ids = ak.where(cat_mask, np.float64(cat_inst.id), np.float64(np.nan))
         category_ids.append(ak.singletons(ak.nan_to_none(ids)))
 
-    # combine and save
+    # combine
     category_ids = ak.concatenate(category_ids, axis=1)
-    events = set_ak_column(events, "category_ids", category_ids, value_type=np.int32)
 
-    return events
+    # save, optionally on a target events array
+    if target_events is None:
+        target_events = events
+    target_events = set_ak_column(target_events, "category_ids", category_ids, value_type=np.int64)
+
+    return target_events
 
 
 @category_ids.init
 def category_ids_init(self: Producer) -> None:
     # store a mapping from leaf category to selector classes for faster lookup
     self.category_to_selectors = defaultdict(list)
```

### Comparing `columnflow-0.2.1/columnflow/production/cms/btag.py` & `columnflow-0.2.2/columnflow/production/cms/btag.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 Producers for btag scale factor weights.
 """
 
 from __future__ import annotations
 
 from columnflow.production import Producer, producer
-from columnflow.util import maybe_import
+from columnflow.util import maybe_import, InsertableDict
 from columnflow.columnar_util import set_ak_column, flat_np_view, layout_ak_array
 
 
 np = maybe_import("numpy")
 ak = maybe_import("awkward")
 
 
@@ -104,33 +104,34 @@
         # enforce the correct shape and create the product over all jets per event
         sf = layout_ak_array(sf_flat_all, events.Jet.pt)
         weight = ak.prod(sf, axis=1, mask_identity=False)
 
         # save the new column
         return set_ak_column(events, column_name, weight, value_type=np.float32)
 
-    # when the uncertainty is a known jec shift, obtain the propagated effect and do not produce
-    # additional systematics
-    if self.shift_inst.is_nominal:
+    # when the requested uncertainty is a known jec shift, obtain the propagated effect and
+    # do not produce additional systematics
+    shift_inst = self.local_shift_inst
+    if shift_inst.is_nominal:
         # nominal weight and those of all method intrinsic uncertainties
         events = add_weight("central", None, "btag_weight")
         for syst_name, col_name in self.btag_uncs.items():
             for direction in ["up", "down"]:
                 name = col_name.format(year=self.config_inst.campaign.x.year)
                 events = add_weight(
                     syst_name,
                     direction,
                     f"btag_weight_{name}_{direction}",
                 )
     elif self.shift_is_known_jec_source:
         # TODO: year dependent jec variations fully covered?
         events = add_weight(
             f"jes{'' if self.jec_source == 'Total' else self.jec_source}",
-            self.shift_inst.direction,
-            f"btag_weight_jec_{self.jec_source}_{self.shift_inst.direction}",
+            shift_inst.direction,
+            f"btag_weight_jec_{self.jec_source}_{shift_inst.direction}",
         )
     else:
         # any other shift, just produce the nominal weight
         events = add_weight("central", None, "btag_weight")
 
     return events
 
@@ -139,19 +140,20 @@
 def btag_weights_init(self: Producer) -> None:
     # depending on the requested shift_inst, there are three cases to handle:
     #   1. when a JEC uncertainty is requested whose propagation to btag weights is known, the
     #      producer should only produce that specific weight column
     #   2. when the nominal shift is requested, the central weight and all variations related to the
     #      method-intrinsic shifts are produced
     #   3. when any other shift is requested, only create the central weight column
-    if not getattr(self, "shift_inst", None):
+    shift_inst = getattr(self, "local_shift_inst", None)
+    if not shift_inst:
         return
 
     # to handle this efficiently in one spot, store jec information
-    self.jec_source = self.shift_inst.x.jec_source if self.shift_inst.has_tag("jec") else None
+    self.jec_source = shift_inst.x.jec_source if shift_inst.has_tag("jec") else None
     btag_sf_jec_source = "" if self.jec_source == "Total" else self.jec_source
     self.shift_is_known_jec_source = (
         self.jec_source and
         btag_sf_jec_source in self.get_btag_config()[1]
     )
 
     # save names of method-intrinsic uncertainties
@@ -163,25 +165,25 @@
         "lfstats1": "lfstats1_{year}",
         "lfstats2": "lfstats2_{year}",
         "cferr1": "cferr1",
         "cferr2": "cferr2",
     }
 
     # add uncertainty sources of the method itself
-    if self.shift_inst.is_nominal:
+    if shift_inst.is_nominal:
         # nominal column
         self.produces.add("btag_weight")
         # all varied columns
         for col_name in self.btag_uncs.values():
             name = col_name.format(year=self.config_inst.campaign.x.year)
             for direction in ["up", "down"]:
                 self.produces.add(f"btag_weight_{name}_{direction}")
     elif self.shift_is_known_jec_source:
         # jec varied column
-        self.produces.add(f"btag_weight_jec_{self.jec_source}_{self.shift_inst.direction}")
+        self.produces.add(f"btag_weight_jec_{self.jec_source}_{shift_inst.direction}")
     else:
         # only the nominal column
         self.produces.add("btag_weight")
 
 
 @btag_weights.requires
 def btag_weights_requires(self: Producer, reqs: dict) -> None:
@@ -189,15 +191,15 @@
         return
 
     from columnflow.tasks.external import BundleExternalFiles
     reqs["external_files"] = BundleExternalFiles.req(self.task)
 
 
 @btag_weights.setup
-def btag_weights_setup(self: Producer, reqs: dict, inputs: dict) -> None:
+def btag_weights_setup(self: Producer, reqs: dict, inputs: dict, reader_targets: InsertableDict) -> None:
     bundle = reqs["external_files"]
 
     # create the btag sf corrector
     import correctionlib
     correctionlib.highlevel.Correction.__call__ = correctionlib.highlevel.Correction.evaluate
     correction_set = correctionlib.CorrectionSet.from_string(
         self.get_btag_file(bundle.files).load(formatter="gzip").decode("utf-8"),
```

### Comparing `columnflow-0.2.1/columnflow/production/cms/electron.py` & `columnflow-0.2.2/columnflow/production/cms/electron.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 Electron related event weights.
 """
 
 from __future__ import annotations
 
 from columnflow.production import Producer, producer
-from columnflow.util import maybe_import
+from columnflow.util import maybe_import, InsertableDict
 from columnflow.columnar_util import set_ak_column, flat_np_view, layout_ak_array
 
 
 np = maybe_import("numpy")
 ak = maybe_import("awkward")
 
 
@@ -94,15 +94,15 @@
         return
 
     from columnflow.tasks.external import BundleExternalFiles
     reqs["external_files"] = BundleExternalFiles.req(self.task)
 
 
 @electron_weights.setup
-def electron_weights_setup(self: Producer, reqs: dict, inputs: dict) -> None:
+def electron_weights_setup(self: Producer, reqs: dict, inputs: dict, reader_targets: InsertableDict) -> None:
     bundle = reqs["external_files"]
 
     # create the corrector
     import correctionlib
     correctionlib.highlevel.Correction.__call__ = correctionlib.highlevel.Correction.evaluate
     correction_set = correctionlib.CorrectionSet.from_string(
         self.get_electron_file(bundle.files).load(formatter="gzip").decode("utf-8"),
```

### Comparing `columnflow-0.2.1/columnflow/production/cms/gen_top_decay.py` & `columnflow-0.2.2/columnflow/production/cms/gen_top_decay.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from columnflow.columnar_util import set_ak_column
 
 
 ak = maybe_import("awkward")
 
 
 @producer(
-    uses={"nGenPart", "GenPart.genPartIdxMother", "GenPart.pdgId", "GenPart.statusFlags"},
+    uses={"GenPart.genPartIdxMother", "GenPart.pdgId", "GenPart.statusFlags"},
     produces={"gen_top_decay"},
 )
 def gen_top_decay_products(self: Producer, events: ak.Array, **kwargs) -> ak.Array:
     """
     Creates a new ragged column "gen_top_decay" with one element per hard top quark. Each element is
     a GenParticleArray with five or more objects in a distinct order: top quark, bottom quark,
     W boson, down-type quark or charged lepton, up-type quark or neutrino, and any additional decay
```

### Comparing `columnflow-0.2.1/columnflow/production/cms/mc_weight.py` & `columnflow-0.2.2/columnflow/production/cms/mc_weight.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 """
 Methods for dealing with MC weights.
 """
 
 from columnflow.production import Producer, producer
 from columnflow.util import maybe_import
-from columnflow.columnar_util import set_ak_column, has_ak_column
+from columnflow.columnar_util import set_ak_column, has_ak_column, optional_column as optional
 
 
 np = maybe_import("numpy")
 ak = maybe_import("awkward")
 
 
 @producer(
-    uses={"genWeight", "LHEWeight.originalXWGTUP"},
+    uses={"genWeight", optional("LHEWeight.originalXWGTUP")},
     produces={"mc_weight"},
     # only run on mc
     mc_only=True,
 )
 def mc_weight(self: Producer, events: ak.Array, **kwargs) -> ak.Array:
     """
     Reads the genWeight and LHEWeight columns and makes a decision about which one to save. This
```

### Comparing `columnflow-0.2.1/columnflow/production/cms/muon.py` & `columnflow-0.2.2/columnflow/production/cms/muon.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 """
 Muon related event weights.
 """
 
 from __future__ import annotations
 
 from columnflow.production import Producer, producer
-from columnflow.util import maybe_import
+from columnflow.util import maybe_import, InsertableDict
 from columnflow.columnar_util import set_ak_column, flat_np_view, layout_ak_array
 
 
 np = maybe_import("numpy")
 ak = maybe_import("awkward")
 
 
 @producer(
     uses={
-        "nMuon", "Muon.pt", "Muon.eta",
+        "Muon.pt", "Muon.eta",
     },
     produces={
         "muon_weight", "muon_weight_up", "muon_weight_down",
     },
     # only run on mc
     mc_only=True,
     # function to determine the correction file
@@ -90,15 +90,15 @@
         return
 
     from columnflow.tasks.external import BundleExternalFiles
     reqs["external_files"] = BundleExternalFiles.req(self.task)
 
 
 @muon_weights.setup
-def muon_weights_setup(self: Producer, reqs: dict, inputs: dict) -> None:
+def muon_weights_setup(self: Producer, reqs: dict, inputs: dict, reader_targets: InsertableDict) -> None:
     bundle = reqs["external_files"]
 
     # create the corrector
     import correctionlib
     correctionlib.highlevel.Correction.__call__ = correctionlib.highlevel.Correction.evaluate
     correction_set = correctionlib.CorrectionSet.from_string(
         self.get_muon_file(bundle.files).load(formatter="gzip").decode("utf-8"),
```

### Comparing `columnflow-0.2.1/columnflow/production/cms/pdf.py` & `columnflow-0.2.2/columnflow/production/cms/pdf.py`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.1/columnflow/production/cms/pileup.py` & `columnflow-0.2.2/columnflow/production/cms/pileup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 Column production methods related to pileup weights.
 """
 
 import functools
 
 from columnflow.production import Producer, producer
-from columnflow.util import maybe_import
+from columnflow.util import maybe_import, InsertableDict
 from columnflow.columnar_util import set_ak_column
 
 
 np = maybe_import("numpy")
 ak = maybe_import("awkward")
 
 # helper
@@ -52,13 +52,13 @@
         return
 
     from columnflow.tasks.cms.external import CreatePileupWeights
     reqs["pu_weights"] = CreatePileupWeights.req(self.task)
 
 
 @pu_weight.setup
-def pu_weight_setup(self: Producer, reqs: dict, inputs: dict) -> None:
+def pu_weight_setup(self: Producer, reqs: dict, inputs: dict, reader_targets: InsertableDict) -> None:
     """
     Loads the pileup weights added through the requirements and saves them in the
     py:attr:`pu_weights` attribute for simpler access in the actual callable.
     """
     self.pu_weights = ak.zip(inputs["pu_weights"].load(formatter="json"))
```

### Comparing `columnflow-0.2.1/columnflow/production/cms/scale.py` & `columnflow-0.2.2/columnflow/production/cms/scale.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,74 @@
 Column production methods related to the renormalization and factorization scales.
 """
 
 import functools
 
 import law
 
-from columnflow.production import Producer, producer
-from columnflow.util import maybe_import
+from columnflow.production import Producer
+from columnflow.util import maybe_import, InsertableDict
 from columnflow.columnar_util import set_ak_column
 from columnflow.columnar_util import DotDict
 
 
 np = maybe_import("numpy")
 ak = maybe_import("awkward")
 
 logger = law.logger.get_logger(__name__)
 
 # helper
 set_ak_column_f32 = functools.partial(set_ak_column, value_type=np.float32)
 
 
-@producer(
-    uses={"LHEScaleWeight"},
+class _ScaleWeightBase(Producer):
+    """
+    Common base class for the scale weight producers below that join a setup function.
+    """
+
+    def setup_func(self, reqs: dict, inputs: dict, reader_targets: InsertableDict) -> None:
+        # named weight indices
+        self.indices_9 = DotDict(
+            mur_down_muf_down=0,
+            mur_down_muf_nom=1,
+            mur_down_muf_up=2,
+            mur_nom_muf_down=3,
+            mur_nom_muf_nom=4,
+            mur_nom_muf_up=5,
+            mur_up_muf_down=6,
+            mur_up_muf_nom=7,
+            mur_up_muf_up=8,
+        )
+
+        # named weight indices for cases where only 8 of the exist
+        # (expecting no nominal value and all above being shifted down by one)
+        self.indices_8 = DotDict({
+            key: index if index <= self.indices_9.mur_nom_muf_nom else index - 1
+            for key, index in self.indices_9.items()
+            if key != "mur_nom_muf_nom"
+        })
+
+        # for convenience, declare some meaningful clear names for the weights
+        # here instead of the very technical names like mur_nom_muf_up
+        self.clearnames = DotDict(
+            # decorrelated weights
+            mur_weight_up="mur_up_muf_nom",
+            mur_weight_down="mur_down_muf_nom",
+            muf_weight_up="mur_nom_muf_up",
+            muf_weight_down="mur_nom_muf_down",
+            # fully-correlated names
+            murmuf_weight_up="mur_up_muf_up",
+            murmuf_weight_down="mur_down_muf_down",
+        )
+
+
+@_ScaleWeightBase.producer(
+    uses={
+        "LHEScaleWeight",
+    },
     produces={
         "mur_weight", "mur_weight_up", "mur_weight_down",
         "muf_weight", "muf_weight_up", "muf_weight_down",
         "murmuf_weight", "murmuf_weight_up", "murmuf_weight_down",
     },
     # only run on mc
     mc_only=True,
@@ -62,15 +105,15 @@
             )
     elif ak.all(n_weights == 8):
         # if we just have 8 weights, there is no nominal LHEScale weight
         # instead, initialize the nominal weights as ones.
         # Additionally, we need to shift the last couple of weight indices
         # down by 1
         indices = self.indices_8
-        murf_nominal = 1
+        murf_nominal = np.array(1, dtype=np.float32)
 
         # additional debug log
         logger.debug(
             f"In dataset {self.dataset_inst.name}: number of LHEScaleWeights is always " +
             "8 instead of the expected 9. It is assumed, that the missing entry is the " +
             "nominal one and all other entries are in correct order",
         )
@@ -116,55 +159,21 @@
             colname,
             murf_weights[:, index],
         )
 
     return events
 
 
-@murmuf_weights.setup
-def murmuf_weights_setup(self: Producer, reqs: dict, inputs: dict) -> None:
-    # define indices in case there are 9 LHEScaleWeights in total
-    self.indices_9 = DotDict(
-        mur_down_muf_down=0,
-        mur_down_muf_nom=1,
-        mur_down_muf_up=2,
-        mur_nom_muf_down=3,
-        mur_nom_muf_nom=4,
-        mur_nom_muf_up=5,
-        mur_up_muf_down=6,
-        mur_up_muf_nom=7,
-        mur_up_muf_up=8,
-    )
-
-    # if there are only 8, the nominal weight at index 4 is missing
-    # in this case, initialize an index where all indices > 4 are shifted
-    # down by one
-    self.indices_8 = DotDict({
-        key: index if index <= 4 else index - 1
-        for key, index in self.indices_9.items()
-        if key != "mur_nom_muf_nom"
-    })
-
-    # for convenience, declare some meaningful clear names for the weights
-    # here instead of the very technical names like mur_nom_muf_up
-    self.clearnames = DotDict(
-        # decorrelated weights
-        mur_weight_up="mur_up_muf_nom",
-        mur_weight_down="mur_down_muf_nom",
-        muf_weight_up="mur_nom_muf_up",
-        muf_weight_down="mur_nom_muf_down",
-        # fully-correlated names
-        murmuf_weight_up="mur_up_muf_up",
-        murmuf_weight_down="mur_down_muf_down",
-    )
-
-
-@producer(
-    uses={"LHEScaleWeight"},
-    produces={"murf_envelope_weight", "murf_envelope_weight_up", "murf_envelope_weight_down"},
+@_ScaleWeightBase.producer(
+    uses={
+        "LHEScaleWeight",
+    },
+    produces={
+        "murf_envelope_weight", "murf_envelope_weight_up", "murf_envelope_weight_down",
+    },
     # only run on mc
     mc_only=True,
 )
 def murmuf_envelope_weights(self: Producer, events: ak.Array, **kwargs) -> ak.Array:
     """
     Producer that determines the envelope of the mur/muf up and down variations on an event-by-event basis.
     This producer assumes that the nominal entry is always the 5th LHEScaleWeight entry and
@@ -186,15 +195,15 @@
             logger.debug(
                 "The nominal LHEScaleWeight is expected to be 1, but also found values " +
                 f"{bad_values} in dataset {self.dataset_inst.name}. All variations will be " +
                 "normalized to the nominal LHEScaleWeight and it is assumed that the nominal " +
                 "weight is already included in the LHEWeight.",
             )
     elif ak.all(n_weights == 8):
-        murf_nominal = 1
+        murf_nominal = np.array(1, dtype=np.float32)
         envelope_indices = self.envelope_indices_8
 
         # additional debug log
         logger.debug(
             f"In dataset {self.dataset_inst.name}: number of LHEScaleWeights is always " +
             "8 instead of the expected 9. It is assumed, that the missing entry is the " +
             "nominal one and all other entries are in correct order",
@@ -214,27 +223,17 @@
     events = set_ak_column_f32(events, "murf_envelope_weight_down", ak.min(considered_murf_weights, axis=1))
     events = set_ak_column_f32(events, "murf_envelope_weight_up", ak.max(considered_murf_weights, axis=1))
 
     return events
 
 
 @murmuf_envelope_weights.setup
-def murmuf_envelope_weights_setup(self: Producer, reqs: dict, inputs: dict) -> None:
-    # define the indices of weights to consider for the envelope construction
-    self.indices_9 = DotDict(
-        mur_down_muf_down=0,
-        mur_down_muf_nom=1,
-        mur_down_muf_up=2,
-        mur_nom_muf_down=3,
-        mur_nom_muf_nom=4,
-        mur_nom_muf_up=5,
-        mur_up_muf_down=6,
-        mur_up_muf_nom=7,
-        mur_up_muf_up=8,
-    )
+def murmuf_envelope_weights_setup(self: Producer, reqs: dict, inputs: dict, reader_targets: InsertableDict) -> None:
+    # call the super func
+    super(murmuf_envelope_weights, self).setup_func(reqs, inputs, reader_targets)
 
     # create a flat list if indices, skipping those for crossed variations
     self.envelope_indices_9 = [
         index
         for name, index in self.indices_9.items()
         if name not in ["mur_down_muf_up", "mur_up_muf_down"]
     ]
```

### Comparing `columnflow-0.2.1/columnflow/production/cms/seeds.py` & `columnflow-0.2.2/columnflow/production/cms/seeds.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,31 +3,37 @@
 """
 Methods related to creating event and object seeds.
 """
 
 import hashlib
 
 from columnflow.production import Producer, producer
-from columnflow.util import maybe_import, primes
-from columnflow.columnar_util import Route, set_ak_column
+from columnflow.util import maybe_import, primes, InsertableDict
+from columnflow.columnar_util import (
+    Route,
+    set_ak_column,
+    has_ak_column,
+    optional_column as optional,
+)
 
 
 np = maybe_import("numpy")
 ak = maybe_import("awkward")
 
 
 @producer(
     uses={
         # global columns for event seed
-        "run", "luminosityBlock", "event", "nGenJet", "nGenPart", "nJet", "nPhoton", "nMuon",
-        "nElectron", "nTau", "nSV",
+        "run", "luminosityBlock", "event",
+        optional("Photon.pt"), optional("SV.pt"),
         # first-object columns for event seed
-        "Tau.jetIdx", "Tau.decayMode",
-        "Muon.jetIdx", "Muon.nStations",
-        "Jet.nConstituents", "Jet.nElectrons", "Jet.nMuons",
+        optional("Tau.jetIdx"), optional("Tau.decayMode"),
+        optional("Muon.jetIdx"), optional("Muon.nStations"),
+        optional("Jet.nConstituents"), optional("Jet.nElectrons"), optional("Jet.nMuons"),
+        optional("GenJet.pt"), optional("GenPart.pt"),
     },
     produces={"deterministic_seed"},
 )
 def deterministic_event_seeds(self: Producer, events: ak.Array, **kwargs) -> ak.Array:
     """
     Produces deterministic event seeds and stores them in *events* which is also returned.
 
@@ -38,27 +44,41 @@
       4. reverse it and int-cast the leading 16 characters, leading to a 64 bit int
     """
     # start with a seed of the event number itself as the most sensitive integer
     # and define the offset of the first prime to use
     seed = self.create_seed(events.event)
     prime_offset = 3
 
-    # get global integers, with a slight difference between data and mc
-    global_fields = ["nGenJet", "nGenPart"] if self.dataset_inst.is_mc else ["run", "luminosityBlock"]
-    global_fields.extend(["nJet", "nPhoton", "nMuon", "nElectron", "nTau", "nSV"])
+    # get counts of jagged fields
+    global_fields = []
+    for field in ["Jet", "Photon", "Muon", "Electron", "Tau", "SV"] + (
+        ["GenJet", "GenPart"] if self.dataset_inst.is_mc else []
+    ):
+        if not has_ak_column(events, field):
+            continue
+        events = set_ak_column(events, f"n{field}", ak.num(events[field], axis=1))
+        global_fields.append(f"n{field}")
+
+    # get run and lumi for data
+    if not self.dataset_inst.is_mc:
+        global_fields.extend(["run", "luminosityBlock"])
+
+    # calculate seed
     for i, f in enumerate(global_fields, prime_offset):
         seed = seed + primes[i] * (events[f] if f in events.fields else ak.num(events[f[1:]]))
 
     # get first-object integers
     object_fields = [
         "Tau.jetIdx", "Tau.decayMode", "Muon.jetIdx", "Muon.nStations", "Jet.nConstituents",
         "Jet.nElectrons", "Jet.nMuons",
     ]
     for i, f in enumerate(object_fields, prime_offset + len(global_fields)):
-        values = events[Route(f).fields]
+        if not has_ak_column(events, f):
+            continue
+        values = Route(f).apply(events)
         seed = seed + primes[i] * (ak.fill_none(ak.firsts(values, axis=1), -1) + 1)
 
     # create and store them
     seed = ak.Array(self.create_seed(seed))
     events = set_ak_column(events, "deterministic_seed", seed)
 
     # uniqueness test across the chunk for debugging
@@ -67,29 +87,29 @@
     # match_text = "yes" if n_events == n_seeds else "NO !!!"
     # print(f"events: {n_events}, unique seeds: {n_seeds}, match: {match_text}")
 
     return events
 
 
 @deterministic_event_seeds.setup
-def deterministic_event_seeds_setup(self: Producer, reqs: dict, inputs: dict) -> None:
+def deterministic_event_seeds_setup(self: Producer, reqs: dict, inputs: dict, reader_targets: InsertableDict) -> None:
     """
     Setup function that defines the vectorized seed creation function once and stores it in the
     py:attr:`create_seed` attribute.
     """
     def create_seed(n: int) -> int:
         return int(hashlib.sha256(bytes(str(n), "utf-8")).hexdigest()[:-16:-1], base=16)
 
     # store a vectorized version
     # TODO: is there a real-vectorized version if hashlib for numpy/scipy?
     self.create_seed = np.vectorize(create_seed, otypes=[np.uint64])
 
 
 @producer(
-    uses={deterministic_event_seeds, "nJet"},
+    uses={deterministic_event_seeds},
     produces={"Jet.deterministic_seed"},
 )
 def deterministic_jet_seeds(self: Producer, events: ak.Array, **kwargs) -> ak.Array:
     """
     Produces deterministic seeds for each jet and stores them in *events* which is also returned.
     The seeds are based on the event seeds produced by :py:func:`deterministic_event_seeds` which is
     also used to access the py:attr:`create_seed` function. The strategy for producing seeds is
```

### Comparing `columnflow-0.2.1/columnflow/production/normalization.py` & `columnflow-0.2.2/columnflow/production/normalization.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """
 Column production methods related to sample normalization event weights.
 """
 
 from columnflow.production import Producer, producer
 from columnflow.production.processes import process_ids
-from columnflow.util import maybe_import
+from columnflow.util import maybe_import, InsertableDict
 from columnflow.columnar_util import set_ak_column
 
 
 np = maybe_import("numpy")
 sp = maybe_import("scipy")
 maybe_import("scipy.sparse")
 ak = maybe_import("awkward")
@@ -63,15 +63,15 @@
         tree_index=0,
         branch=-1,
         _exclude=MergeSelectionStats.exclude_params_forest_merge,
     )
 
 
 @normalization_weights.setup
-def normalization_weights_setup(self: Producer, reqs: dict, inputs: dict) -> None:
+def normalization_weights_setup(self: Producer, reqs: dict, inputs: dict, reader_targets: InsertableDict) -> None:
     """
     Sets up objects required by the computation of normalization weights and stores them as instance
     attributes:
 
         - py:attr:`selection_stats`: The stats dict loaded from the output of MergeSelectionsStats.
         - py:attr:`sum_weights_table`: A sparse array serving as a lookup table for the sum of event
           weights per process id.
@@ -85,14 +85,26 @@
     process_insts = [
         process_inst
         for process_inst, _, _ in self.config_inst.walk_processes()
         if process_inst.is_mc
     ]
     max_id = max(process_inst.id for process_inst in process_insts)
 
+    # ensure that the selection stats do not contain any process that was not previously registered
+    unregistered_process_ids = [
+        int(process_id) for process_id in selection_stats["sum_mc_weight_per_process"]
+        if int(process_id) > max_id
+    ]
+    if unregistered_process_ids:
+        id_str = ",".join(map(str, unregistered_process_ids))
+        raise Exception(
+            f"selection stats contain ids ({id_str}) of processes that were not previously " +
+            f"registered to the config '{self.config_inst.name}'",
+        )
+
     # create a event weight sum lookup table with all known processes
     sum_weights_table = sp.sparse.lil_matrix((1, max_id + 1), dtype=np.float32)
     for process_id, sum_weights in selection_stats["sum_mc_weight_per_process"].items():
         sum_weights_table[0, int(process_id)] = sum_weights
     self.sum_weights_table = sum_weights_table
 
     # create a cross section lookup table with all known processes
```

### Comparing `columnflow-0.2.1/columnflow/production/processes.py` & `columnflow-0.2.2/columnflow/production/processes.py`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.1/columnflow/production/util.py` & `columnflow-0.2.2/columnflow/production/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """
 General producers that might be utilized in various places.
 """
 
 from __future__ import annotations
 
-from typing import Sequence
+from typing import Sequence, Union
 
 from columnflow.production import Producer, producer
 from columnflow.util import maybe_import
 from columnflow.columnar_util import set_ak_column, attach_behavior
 
 
 ak = maybe_import("awkward")
@@ -61,26 +61,35 @@
 }
 
 
 @producer(call_force=True)
 def attach_coffea_behavior(
     self: Producer,
     events: ak.Array,
-    collections: dict | Sequence | None = None,
+    collections: Union[dict, Sequence, None] = None,
     **kwargs,
 ) -> ak.Array:
     """
-    Rebuild certain collections with original coffea behavior in case some of them might have been
-    invalidated in a potential previous step. All information on source collection names, type
+    Add coffea's NanoEvents behavior to collections.
+
+    This might become relevant in case some of the collections have been invalidated in a potential
+    previous step. All information on source collection names, :external+coffea:doc:`index` type
     names, attributes to check whether the correct behavior is already attached, and fields to
     potentially skip is taken from :py:obj:`default_collections`.
 
     However, this information is updated by *collections* when it is a dict. In case it is a list,
     its items are interpreted as names of collections defined as keys in
     :py:obj:`default_collections` for which the behavior should be attached.
+
+    :param events: Array containing the events
+    :param collections: Attach behavior for these collections. If :py:class:`dict`, the
+        :py:obj:`default_collections` are updated with the information in *collections*. If
+        :py:class:`list`, only update this set of *collections* as specified in the
+        :py:obj:`default_collections`.
+    :return: Array with correct behavior attached for collections
     """
     # update or reduce collection info
     _collections = default_collections
     if isinstance(collections, dict):
         _collections = _collections.copy()
         _collections.update(collections)
     elif isinstance(collections, (list, tuple)):
```

### Comparing `columnflow-0.2.1/columnflow/selection/cms/json_filter.py` & `columnflow-0.2.2/columnflow/selection/cms/json_filter.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,27 +3,46 @@
 """
 Selectors for applying golden JSON in data.
 """
 
 from __future__ import annotations
 
 from columnflow.selection import Selector, selector
-from columnflow.util import maybe_import
+from columnflow.util import maybe_import, InsertableDict, DotDict
 
 
 ak = maybe_import("awkward")
 np = maybe_import("numpy")
 sp = maybe_import("scipy")
 maybe_import("scipy.sparse")
 
 
+def get_lumi_file_default(self, external_files: DotDict) -> str:
+    """
+    Function to load path or url to golden json files.
+
+    By default, the path is extracted from the current *config_inst*, which
+    should have a *external_files* in the auxiliary information block.
+    The path or url is extracted with
+
+    .. code-block:: python
+
+        external_files.lumi.golden
+
+    :param external_files: Config containing the information about the path
+        or url to the golden json file containing good lumi sections.
+    :return: path or url to golden json file.
+    """
+    return external_files.lumi.golden
+
+
 @selector(
     uses={"run", "luminosityBlock"},
     # function to determine the golden lumi file
-    get_lumi_file=(lambda self, external_files: external_files.lumi.golden),
+    get_lumi_file=get_lumi_file_default,
 )
 def json_filter(
     self: Selector,
     events: ak.Array,
     data_only=True,
     **kwargs,
 ) -> ak.Array:
@@ -40,35 +59,63 @@
             "lumi": {
                 "golden": "/afs/cern.ch/cms/CAF/CMSCOMM/COMM_DQM/certification/Collisions17/13TeV/Legacy_2017/Cert_294927-306462_13TeV_UL2017_Collisions17_GoldenJSON.txt",  # noqa
             },
         })
 
     *get_lumi_file* can be adapted in a subclass in case it is stored differently in the external
     files.
+
+    :param events: Array containing events in the NanoAOD format
+    :param data_only: boolean flag to indicate that this selector should only run on observed data,
+        defaults to True
+    :return: Array containing boolean masks to accept or reject given events
     """
-    lookup_result = self.run_ls_lookup[events.run, events.luminosityBlock].todense()
-    return np.squeeze(np.array(lookup_result))
+    # handle out-of-bounds values
+    run_out_of_bounds = (events.run >= self.run_ls_lookup.shape[0])
+    ls_out_of_bounds = (events.luminosityBlock >= self.run_ls_lookup.shape[1])
+    out_of_bounds = (run_out_of_bounds | ls_out_of_bounds)
+
+    run = ak.where(out_of_bounds, 0, events.run)
+    ls = ak.where(out_of_bounds, 0, events.luminosityBlock)
+
+    # look up json filter decision
+    lookup_result = self.run_ls_lookup[run, ls].todense()
+
+    # remove extra dimensions
+    lookup_result = np.squeeze(np.array(lookup_result))
+
+    # reject out-ouf-bounds entries
+    lookup_result = ak.where(out_of_bounds, False, lookup_result)
+
+    return lookup_result
 
 
 @json_filter.requires
 def json_filter_requires(self: Selector, reqs: dict) -> None:
-    """
-    Add external files bundle as a task requirement.
-    """
     if "external_files" in reqs:
         return
 
     from columnflow.tasks.external import BundleExternalFiles
     reqs["external_files"] = BundleExternalFiles.req(self.task)
 
 
 @json_filter.setup
-def json_filter_setup(self: Selector, reqs: dict, inputs: dict) -> None:
-    """
-    Load golden JSON and set up run/luminosity block lookup table.
+def json_filter_setup(
+    self: Selector,
+    reqs: dict,
+    inputs: dict,
+    reader_targets: InsertableDict,
+) -> None:
+    """
+    Setup function for :py:class:`json_filter`. Load golden JSON and set up run/luminosity block
+    lookup table.
+
+    :param reqs: Contains requirements for this task
+    :param inputs: Additional inputs, currently not used
+    :param reader_targets: Additional targets, currently not used
     """
     bundle = reqs["external_files"]
 
     # import the correction sets from the external file
     json = self.get_lumi_file(bundle.files).load(formatter="json")
 
     # determine range of run/luminosity block values
```

### Comparing `columnflow-0.2.1/columnflow/selection/cms/met_filters.py` & `columnflow-0.2.2/columnflow/selection/cms/met_filters.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,34 +2,52 @@
 
 """
 Selector related to MET filters.
 """
 
 from __future__ import annotations
 
+from typing import Iterable
+
 from columnflow.selection import Selector, selector
 from columnflow.util import maybe_import
 from columnflow.columnar_util import Route
 
 
 ak = maybe_import("awkward")
 
 
+def get_met_filters_default(self) -> Iterable[str]:
+    """
+    Function to obtain met filters from the config.
+
+    By default, this is done using
+
+    .. code-block:: python
+
+        return config_inst.x.met_filters
+
+    :return: list or set of met filters to be applied
+    """
+    return self.config_inst.x.met_filters
+
+
 @selector(
-    uses={"event", "nFlag"},
+    uses={"event"},
     # function to obtain met filters from the config
-    get_met_filters=(lambda self: self.config_inst.x.met_filters),
+    get_met_filters=get_met_filters_default,
 )
 def met_filters(
     self: Selector,
     events: ak.Array,
     **kwargs,
 ) -> ak.Array:
     """
-    Compute a selection mask to filter out noisy/anomalous high-MET events (MET filters).
+    Compute a selection mask to filter out noisy/anomalous high-MET events
+    (MET filters).
 
     Individual filter decisions based on different criteria are stored as bool-valued columns
     in the input NanoAOD. The columns to apply are specified via an auxiliary config entry:
 
     .. code-block:: python
 
         cfg.x.met_filters = {
@@ -45,15 +63,18 @@
 
     *get_met_filters* can be adapted in a subclass in case they are stored differently in the
     config.
 
     The specified columns are interpreted as booleans, with missing values treated as *True*,
     i.e. the event is considered to have passed the corresponding filter.
 
-    Returns a bool array containing the logical AND of all input columns.
+    Returns a bool array containing the logical ``AND`` of all input columns.
+
+    :param events: Array containing events in the NanoAOD format
+    :return: Array containing logical ``AND`` of all input filter columns
     """
     result = ak.ones_like(events.event, dtype=bool)
 
     for route in self.met_filters:
         # interpret column values as booleans
         vals = Route(route).apply(events)
         vals = ak.values_astype(vals, bool)
@@ -63,17 +84,14 @@
         result = (result & vals)
 
     return result
 
 
 @met_filters.init
 def met_filters_init(self: Selector) -> None:
-    """
-    Read MET filters from config and add them as input columns.
-    """
     met_filters = self.get_met_filters()
     if isinstance(met_filters, dict):
         # do nothing when no dataset_inst is known
         if not getattr(self, "dataset_inst", None):
             return
         met_filters = met_filters[self.dataset_inst.data_source]
```

### Comparing `columnflow-0.2.1/columnflow/selection/matching.py` & `columnflow-0.2.2/columnflow/selection/matching.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,38 +2,45 @@
 
 """
 Distance-based methods.
 """
 
 from __future__ import annotations
 
-from typing import Callable
+from typing import Callable, Union
 
 from columnflow.selection import Selector, SelectionResult, selector
 from columnflow.util import maybe_import
 
 
 np = maybe_import("numpy")
 ak = maybe_import("awkward")
 
 
 def cleaning_factory(
     selector_name: str,
     to_clean: str,
     clean_against: list[str],
-    metric: Callable | None = None,
-) -> Callable:
+    metric: Union[Callable, None] = None,
+) -> Selector:
     """
-    factory to generate a function with name *selector_name* that cleans the
-    field *to_clean* in the NanoEventArrays agains the field(s) *clean_agains*.
-    First, the necessary column names to construct four-momenta for the
-    different object fields are constructed, i.e. pt, eta, phi and e for the
-    different objects.
-    Finally, the actual selector function is generated, which uses these
-    columns.
+    Factory to generate a function with name *selector_name* that cleans the field *to_clean* in an
+    array following the :external+coffea:py:class:`~coffea.nanoevents.NanoAODSchema` against the
+    field(s) *clean_against*. First, the necessary column names to construct four-momenta for the
+    different object fields are constructed, i.e. ``pt``, ``eta``, ``phi`` and ``e`` for the
+    different objects. Finally, the actual selector function is generated, which uses these columns.
+
+    :param selector_name: Name of the :py:class:`~columnflow.selection.Selector` class to be
+        initialized.
+    :param to_clean: Name of the field to be cleaned (e.g. ``"Jet"``).
+    :param clean_against: Names of the fields of object to clean field *to_clean* against
+        (e.g. ``["Muon"]``).
+    :param metric: Function to use for the cleaning. If None, use
+        :external+coffea:py:meth:`~coffea.nanoevents.methods.vector.LorentzVector.delta_r`.
+    :return: Instance of :py:class:`~columnflow.selection.Selector`.
     """
     # default of the metric function is the delta_r function
     # of the coffea LorentzVectors
     if metric is None:
         metric = lambda a, b: a.delta_r(b)
 
     # compile the list of variables that are necessary for the four momenta
@@ -58,62 +65,73 @@
     # finally, construct selector function itself
     @selector(uses=uses, name=selector_name)
     def func(
         self: Selector,
         events: ak.Array,
         to_clean: str,
         clean_against: list[str],
-        metric: Callable | None = metric,
+        metric: Union[Callable, None] = metric,
         threshold: float = 0.4,
-    ) -> list[int]:
+    ) -> ak.Array:
         """
-        abstract function to perform a cleaning of field *to_clean* against
-        a (list of) field(s) *clean_against* based on an abitrary metric
-        *metric* (e.g. deltaR).
-        First concatenate all fields in *clean_against*, which thus includes
-        all fields that are to be used for the comparison of the metric.
-        Then construct the metric for all permutations of the different objects
-        using the coffea nearest implementation.
-        All objects in field *to_clean* are removed if the metric is below the
+        Abstract function to perform a cleaning of field *to_clean* against a (list of) field(s)
+        *clean_against* based on an abitrary metric *metric* (e.g.
+        :external+coffea:py:meth:`~coffea.nanoevents.methods.vector.LorentzVector.delta_r`). First
+        concatenate all fields in *clean_against*, which thus includes all fields that are to be
+        used for the comparison of the metric. Then construct the metric for all permutations of the
+        different objects using the :external+coffea:doc:`index`
+        :external+coffea:py:meth:`~coffea.nanoevents.methods.vector.LorentzVector.nearest`
+        implementation. All objects in field *to_clean* are removed if the metric is below the
         *threshold*.
-        """
 
+        :param self: :py:class:`columnflow.selection.Selector` instance into which this function is
+            embedded.
+        :param events: array containing events in the NanoAOD format
+        param to_clean: Name of the field to be cleaned (e.g. ``"Jet"``)
+        :param clean_against: Names of the fields of object to clean field *to_clean* against (e.g.
+            ``["Muon"]``)
+        :param metric: Function to use for the cleaning. If None, the
+            :external+coffea:py:meth:`~coffea.nanoevents.methods.vector.LorentzVector.delta_r`,
+            defaults to None.
+        :param threshold: Threshold value for decision which objects to keep and which to reject,
+            defaults to ``0.4``.
+        :return: array of indices of cleaned objects, ordered according to the ``pt`` of the
+            objects.
+        """
         # concatenate the fields that are to be used in the construction
         # of the metric table
         summed_clean_against = ak.concatenate(
             [events[x] for x in clean_against],
             axis=1,
         )
 
         # load actual NanoEventArray that is to be cleaned
         to_clean_field = events[to_clean]
 
-        # construct metric table for these objects. The metric table contains
-        # the minimal value of the metric *metric* for each object in field
-        # *to_clean* w.r.t. all objects in *summed_clean_against*. Thus,
-        # it has the dimensions nevents x nto_clean, where *nevents* is
-        # the number of events in the current chunk of data and *nto_clean*
-        # is the length of the field *to_clean*. Note that the argument
-        # *threshold* in the *nearest* function must be set to None since
-        # the function will perform a selection itself to extract the nearest
-        # objects (i.e. applies the selection we want here in reverse)
+        # construct metric table for these objects. The metric table contains the minimal value of
+        # the metric *metric* for each object in field *to_clean* w.r.t. all objects in
+        # *summed_clean_against*. Thus, it has the dimensions nevents x nto_clean, where *nevents*
+        # is the number of events in the current chunk of data and *nto_clean* is the length of the
+        # field *to_clean*. Note that the argument *threshold* in the *nearest* function must be set
+        # to None since the function will perform a selection itself to extract the nearest objects
+        # (i.e. applies the selection we want here in reverse)
         _, metric = to_clean_field.nearest(
             summed_clean_against,
             metric=metric,
             return_metric=True,
             threshold=None,
         )
         # build a binary mask based on the selection threshold provided by the
         # user
         mask = metric > threshold
 
         # construct final result. Currently, this is the list of indices for
         # clean jets, sorted for pt
         # WARNING: this still contains the bug with the application of the mask
-        #           which will be adressed in a PR in the very near future
+        #          which will be adressed in a PR in the very near future
         # TODO: return the mask itself instead of the list of indices
         sorted_list = ak.argsort(to_clean_field.pt, axis=-1, ascending=False)[mask]
         return sorted_list
 
     return func
 
 
@@ -125,22 +143,26 @@
 )
 
 
 @selector(uses={delta_r_jet_lepton})
 def jet_lepton_delta_r_cleaning(
     self: Selector,
     events: ak.Array,
-    stats: dict[str, int | float],
+    stats: dict[str, Union[int, float]],
     threshold: float = 0.4,
     **kwargs,
 ) -> SelectionResult:
     """
-    function to apply the selection requirements necessary for a
-    cleaning of jets against leptons.
-    The function calls the requirements to clean the field *Jet* against
-    the concatination of the fields *[Muon, Electron]*, i.e. all leptons
-    and passes the desired threshold for the selection
+    Function to apply the selection requirements necessary for a cleaning of jets against leptons.
+
+    The function calls the requirements to clean the field *Jet* against the concatination of the
+    fields *[Muon, Electron]*, i.e. all leptons and passes the desired threshold for the selection
+
+    :param events: Array containing events in the NanoAOD format
+    :param stats: :py:class:`dictionary <dict>` containing selection stats (not used here).
+    :param threshold: Threshold value for decision which objects to keep and which to reject.
+    :return: :py:class:`~columnflow.selection.SelectionResult` with indices of cleaned jets.
     """
     clean_jet_indices = self[delta_r_jet_lepton](events, "Jet", ["Muon", "Electron"], threshold=threshold)
 
     # TODO: should not return a new object collection but an array with masks
     return SelectionResult(objects={"Jet": clean_jet_indices})
```

### Comparing `columnflow-0.2.1/columnflow/tasks/calibration.py` & `columnflow-0.2.2/columnflow/tasks/calibration.py`

 * *Files 25% similar despite different names*

```diff
@@ -19,51 +19,80 @@
 class CalibrateEvents(
     CalibratorMixin,
     ChunkedIOMixin,
     DatasetTask,
     law.LocalWorkflow,
     RemoteWorkflow,
 ):
+    """
+    Task to apply calibrations to objects, e.g. leptons and jets.
+
+    The calibrations that are to be applied can be specified on the command line, and are
+    implemented as instances of the :py:class:`~columnflow.calibration.Calibrator` class. For
+    further information, please consider the documentation there.
+    """
     # default sandbox, might be overwritten by calibrator function
-    sandbox = dev_sandbox("bash::$CF_BASE/sandboxes/venv_columnar.sh")
+    sandbox = dev_sandbox(law.config.get("analysis", "default_columnar_sandbox"))
 
     # upstream requirements
     reqs = Requirements(
         RemoteWorkflow.reqs,
         GetDatasetLFNs=GetDatasetLFNs,
     )
 
+    # register shifts found in the chosen calibrator to this task
     register_calibrator_shifts = True
 
-    def workflow_requires(self):
+    def workflow_requires(self) -> dict:
+        """
+        Configure the requirements for the workflow in general. For more general informations, see
+        :external+law:py:meth:`BaseWorkflow.workflow_requires() <law.workflow.base.BaseWorkflow.workflow_requires>`.
+
+        :return: Dictionary containing the requirements for this task.
+        """
         reqs = super().workflow_requires()
 
         reqs["lfns"] = self.reqs.GetDatasetLFNs.req(self)
 
         # add calibrator dependent requirements
         reqs["calibrator"] = self.calibrator_inst.run_requires()
 
         return reqs
 
-    def requires(self):
+    def requires(self) -> dict:
+        """
+        Configure the requirements for the individual branches of the workflow.
+        """
         reqs = {"lfns": self.reqs.GetDatasetLFNs.req(self)}
 
         # add calibrator dependent requirements
         reqs["calibrator"] = self.calibrator_inst.run_requires()
 
         return reqs
 
     def output(self):
-        return {"columns": self.target(f"calib_{self.branch}.parquet")}
+        """
+        Defines the outputs of the current branch within the workflow.
+        """
+        outputs = {}
+
+        # only declare the output in case the calibrator actually creates columns
+        if self.calibrator_inst.produced_columns:
+            outputs["columns"] = self.target(f"calib_{self.branch}.parquet")
+
+        return outputs
 
     @law.decorator.log
     @ensure_proxy
     @law.decorator.localize(input=False, output=True)
     @law.decorator.safe_output
     def run(self):
+        """
+        Run method of this task.
+        """
         from columnflow.columnar_util import (
             Route, RouteFilter, mandatory_coffea_columns, sorted_ak_to_parquet,
         )
 
         # prepare inputs and outputs
         reqs = self.requires()
         lfn_task = reqs["lfns"]
@@ -128,8 +157,13 @@
 )
 
 
 CalibrateEventsWrapper = wrapper_factory(
     base_cls=AnalysisTask,
     require_cls=CalibrateEvents,
     enable=["configs", "skip_configs", "datasets", "skip_datasets", "shifts", "skip_shifts"],
+    docs="""
+Wrapper task to calibrate events for multiple datasets.
+
+:enables: ["configs", "skip_configs", "datasets", "skip_datasets", "shifts", "skip_shifts"]
+""",
 )
```

### Comparing `columnflow-0.2.1/columnflow/tasks/cms/external.py` & `columnflow-0.2.2/columnflow/tasks/cms/external.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,34 +38,46 @@
 
     def requires(self):
         return self.reqs.BundleExternalFiles.req(self)
 
     def output(self):
         return self.target(f"weights_from_{self.data_mode}.json")
 
+    def sandbox_stagein(self):
+        # stagein all inputs
+        return True
+
+    def sandbox_stageout(self):
+        # stageout all outputs
+        return True
+
     @law.decorator.log
     @law.decorator.safe_output
     def run(self):
         # prepare the external files and the output weights
         externals = self.requires()
         weights = {}
 
+        # since this tasks uses stage-in into and stage-out from the sandbox,
+        # prepare external files with the staged-in inputs
+        externals.get_files(self.input())
+
         # read the mc profile
         mc_profile = self.read_mc_profile_from_cfg(externals.files.pu.mc_profile)
 
         # loop over nominal and minbias_xs shifts
         for shift in ["nominal", "minbias_xs_up", "minbias_xs_down"]:
             # read or create the data profile
             if self.data_mode == "hist":
                 pu_hist_target = externals.files.pu.data_profile[shift]
                 data_profile = self.read_data_profile_from_hist(pu_hist_target)
-            else:
+            else:  # "pileupcalc"
                 pu_file_target = externals.files.pu.json
-                minbiasxs = self.config_inst.x.minbiasxs.get(shift)
-                data_profile = self.read_data_profile_from_pileupcalc(pu_file_target, minbiasxs)
+                mb_xs = self.config_inst.x.minbias_xs.get(shift)
+                data_profile = self.read_data_profile_from_pileupcalc(pu_file_target, mb_xs)
 
             # build the ratios and save them
             if len(mc_profile) != len(data_profile):
                 raise Exception(
                     f"the number of bins in the MC profile ({len(mc_profile)}) does not match that "
                     f"of the data profile for the {shift} shift ({len(data_profile)})",
                 )
```

### Comparing `columnflow-0.2.1/columnflow/tasks/cms/inference.py` & `columnflow-0.2.2/columnflow/tasks/cms/inference.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,26 +11,27 @@
 from columnflow.tasks.framework.base import Requirements, AnalysisTask, wrapper_factory
 from columnflow.tasks.framework.mixins import (
     CalibratorsMixin, SelectorStepsMixin, ProducersMixin, MLModelsMixin, InferenceModelMixin,
 )
 from columnflow.tasks.framework.remote import RemoteWorkflow
 from columnflow.tasks.histograms import MergeHistograms, MergeShiftedHistograms
 from columnflow.util import dev_sandbox
+from columnflow.config_util import get_datasets_from_process
 
 
 class CreateDatacards(
     InferenceModelMixin,
     MLModelsMixin,
     ProducersMixin,
     SelectorStepsMixin,
     CalibratorsMixin,
     law.LocalWorkflow,
     RemoteWorkflow,
 ):
-    sandbox = dev_sandbox("bash::$CF_BASE/sandboxes/venv_columnar.sh")
+    sandbox = dev_sandbox(law.config.get("analysis", "default_columnar_sandbox"))
 
     # upstream requirements
     reqs = Requirements(
         RemoteWorkflow.reqs,
         MergeHistograms=MergeHistograms,
         MergeShiftedHistograms=MergeShiftedHistograms,
     )
@@ -46,14 +47,26 @@
             law.util.flatten(t.requires())
             for t in self.get_branch_tasks().values()
         ), []))
 
         return reqs
 
     def requires(self):
+        # helper to find automatic datasets
+        def get_mc_datasets(proc_obj: dict) -> list[str]:
+            # when datasets are defined on the process object itself, return them
+            if proc_obj.config_mc_datasets:
+                return proc_obj.config_mc_datasets
+
+            # if not, check the config
+            return [
+                dataset_inst.name
+                for dataset_inst in get_datasets_from_process(self.config_inst, proc_obj.config_process)
+            ]
+
         cat_obj = self.branch_data
         reqs = {
             proc_obj.name: {
                 dataset: self.reqs.MergeShiftedHistograms.req(
                     self,
                     dataset=dataset,
                     shift_sources=tuple(
@@ -61,15 +74,15 @@
                         for param_obj in proc_obj.parameters
                         if self.inference_model_inst.require_shapes_for_parameter(param_obj)
                     ),
                     variables=(cat_obj.config_variable,),
                     branch=-1,
                     _exclude={"branches"},
                 )
-                for dataset in proc_obj.config_mc_datasets
+                for dataset in get_mc_datasets(proc_obj)
             }
             for proc_obj in cat_obj.processes
         }
         if cat_obj.config_data_datasets:
             reqs["data"] = {
                 dataset: self.reqs.MergeHistograms.req(
                     self,
```

### Comparing `columnflow-0.2.1/columnflow/tasks/cutflow.py` & `columnflow-0.2.2/columnflow/tasks/cutflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,28 +31,31 @@
     SelectorStepsMixin,
     CalibratorsMixin,
     ChunkedIOMixin,
     DatasetTask,
     law.LocalWorkflow,
     RemoteWorkflow,
 ):
-    sandbox = dev_sandbox("bash::$CF_BASE/sandboxes/venv_columnar.sh")
+    sandbox = dev_sandbox(law.config.get("analysis", "default_columnar_sandbox"))
 
     selector_steps_order_sensitive = True
 
     initial_step = "Initial"
 
     default_variables = ("event", "cf_*")
 
     # upstream requirements
     reqs = Requirements(
         RemoteWorkflow.reqs,
         MergeSelectionMasks=MergeSelectionMasks,
     )
 
+    # strategy for handling missing source columns when adding aliases on event chunks
+    missing_column_alias_strategy = "original"
+
     def create_branch_map(self):
         # dummy branch map
         return [None]
 
     def workflow_requires(self):
         reqs = super().workflow_requires()
 
@@ -72,14 +75,15 @@
         }
 
     @law.decorator.log
     @law.decorator.localize(input=True, output=False)
     @law.decorator.safe_output
     def run(self):
         import hist
+        import numpy as np
         import awkward as ak
         from columnflow.columnar_util import Route, add_ak_aliases
 
         # prepare inputs and outputs
         inputs = self.input()
 
         # create a temp dir for saving intermediate files
@@ -106,15 +110,17 @@
             # get the expression per variable and when a string, parse it to extract index lookups
             for variable_inst in variable_insts:
                 expr = variable_inst.expression
                 if isinstance(expr, str):
                     route = Route(expr)
                     expr = functools.partial(route.apply, null_value=variable_inst.null_value)
                     read_columns.add(route)
-                # TODO: handle variable_inst with custom expressions, can they declare columns?
+                else:
+                    # for variable_inst with custom expressions, read columns declared via aux key
+                    read_columns |= {inp for inp in variable_inst.x("inputs", [])}
                 expressions[variable_inst.name] = expr
 
         # prepare columns to load
         load_columns = {("events" + route) for route in read_columns} | {Route("steps.*")}
 
         # prepare histograms
         histograms = {}
@@ -153,54 +159,66 @@
                 steps = arr.steps.fields
 
             # prepare histograms and exprepssions once
             if not histograms:
                 prepare_hists([self.initial_step] + list(steps))
 
             # add aliases
-            events = add_ak_aliases(events, aliases, remove_src=True)
+            events = add_ak_aliases(
+                events,
+                aliases,
+                remove_src=True,
+                missing_strategy=self.missing_column_alias_strategy,
+            )
 
             # pad the category_ids when the event is not categorized at all
             category_ids = ak.fill_none(ak.pad_none(events.category_ids, 1, axis=-1), -1)
 
             for var_key, var_names in self.variable_tuples.items():
                 # helper to build the point for filling, except for the step which does
                 # not support broadcasting
                 def get_point(mask=Ellipsis):
+                    n_events = len(events) if mask is Ellipsis else ak.sum(mask)
                     point = {
                         "process": events.process_id[mask],
                         "category": category_ids[mask],
-                        "shift": self.global_shift_inst.id,
+                        "shift": np.ones(n_events, dtype=np.int32) * self.global_shift_inst.id,
                         "weight": (
                             events.normalization_weight[mask]
                             if self.dataset_inst.is_mc
-                            else 1.0
+                            else np.ones(n_events, dtype=np.float32)
                         ),
                     }
                     for var_name in var_names:
                         point[var_name] = expressions[var_name](events)[mask]
                     return point
 
                 # fill the raw point
                 fill_kwargs = get_point()
-                arrays = (ak.flatten(a) for a in ak.broadcast_arrays(*fill_kwargs.values()))
-                histograms[var_key].fill(step=self.initial_step, **dict(zip(fill_kwargs, arrays)))
+                arrays = ak.flatten(ak.cartesian(fill_kwargs))
+                histograms[var_key].fill(
+                    step=self.initial_step,
+                    **{field: arrays[field] for field in arrays.fields},
+                )
 
                 # fill all other steps
                 mask = True
                 for step in steps:
                     if step not in arr.steps.fields:
                         raise ValueError(
                             f"step '{step}' is not defined by selector {self.selector}",
                         )
                     # incrementally update the mask and fill the point
                     mask = mask & arr.steps[step]
                     fill_kwargs = get_point(mask)
-                    arrays = [ak.flatten(a) for a in ak.broadcast_arrays(*fill_kwargs.values())]
-                    histograms[var_key].fill(step=step, **dict(zip(fill_kwargs, arrays)))
+                    arrays = ak.flatten(ak.cartesian(fill_kwargs))
+                    histograms[var_key].fill(
+                        step=step,
+                        **{field: arrays[field] for field in arrays.fields},
+                    )
 
         # dump the histograms
         for var_key in histograms.keys():
             self.output()[var_key].dump(histograms[var_key], formatter="pickle")
 
 
 CreateCutflowHistogramsWrapper = wrapper_factory(
@@ -215,19 +233,18 @@
     CategoriesMixin,
     CalibratorsMixin,
     PlotBase,
     ShiftTask,
     law.LocalWorkflow,
     RemoteWorkflow,
 ):
+    sandbox = dev_sandbox(law.config.get("analysis", "default_columnar_sandbox"))
 
     exclude_index = True
 
-    sandbox = dev_sandbox("bash::$CF_BASE/sandboxes/venv_columnar.sh")
-
     selector_steps_order_sensitive = True
 
     # upstream requirements
     reqs = Requirements(
         RemoteWorkflow.reqs,
         CreateCutflowHistograms=CreateCutflowHistograms,
     )
```

### Comparing `columnflow-0.2.1/columnflow/tasks/external.py` & `columnflow-0.2.2/columnflow/tasks/external.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,58 +13,86 @@
 from typing import Sequence
 
 import luigi
 import law
 import order as od
 
 from columnflow.tasks.framework.base import AnalysisTask, ConfigTask, DatasetTask, wrapper_factory
-from columnflow.util import wget
+from columnflow.util import wget, DotDict
 
 
 logger = law.logger.get_logger(__name__)
 
 
 class GetDatasetLFNs(DatasetTask, law.tasks.TransferLocalFile):
+    """
+    Task to get list of logical file names (LFNs).
+    """
 
     replicas = luigi.IntParameter(
         default=5,
         description="number of replicas to generate; default: 5",
     )
     validate = law.OptionalBoolParameter(
-        default=None,  # set to True as long as we are doing tests with reduced n_files in datasets
+        default=None,
         significant=False,
         description="when True, complains if the number of obtained LFNs does not match the value "
         "expected from the dataset info; default: obtained from 'validate_dataset_lfns' auxiliary "
         "entry in config",
     )
     version = None
 
     @classmethod
-    def resolve_param_values(cls, params):
+    def resolve_param_values(cls, params: DotDict) -> DotDict:
+        """
+        Resolve parameter values *params* from command line and propagate them to this set of
+        parameters.
+
+        :param params: Parameters provided at command line level.
+        :return: Updated list of parameter values.
+        """
         params = super().resolve_param_values(params)
 
         # add the default calibrator when empty
         if "config_inst" in params and params.get("validate") is None:
             config_inst = params["config_inst"]
             params["validate"] = config_inst.x("validate_dataset_lfns", False)
 
         return params
 
     @property
-    def sandbox(self):
+    def sandbox(self) -> str:
+        """
+        Defines sandbox for this task.
+
+        :return: Path to shell script that sets up the requested sandbox.
+        """
         sandbox = self.config_inst.x("get_dataset_lfns_sandbox", None)
-        return sandbox or "bash::/cvmfs/cms.cern.ch/cmsset_default.sh"
+        if sandbox is None:
+            sandbox = "bash::/cvmfs/cms.cern.ch/cmsset_default.sh"
+        return sandbox if sandbox and sandbox != law.NO_STR else None
 
-    def single_output(self):
+    def single_output(self) -> law.target.file.FileSystemFileTarget:
+        """
+        Creates a remote target file for the final .json file containing the list of LFNs.
+
+        :return: Law remote target with the initialized output name
+        """
         # required by law.tasks.TransferLocalFile
         h = law.util.create_hash(list(sorted(self.dataset_info_inst.keys)))
         return self.target(f"lfns_{h}.json")
 
     @law.decorator.log
     def run(self):
+        """
+        Run function for this task.
+
+        :raises ValueError: If number of loaded LFNs does not correspond to number of LFNs specified
+            in this ``dataset_info_inst``.
+        """
         # prepare the lfn getter
         get_dataset_lfns = self.config_inst.x("get_dataset_lfns", None)
         msg = "via custom config function"
         if not callable(get_dataset_lfns):
             get_dataset_lfns = self.get_dataset_lfns_dasgoclient
             msg = "via dasgoclient"
 
@@ -87,14 +115,23 @@
 
     def get_dataset_lfns_dasgoclient(
         self,
         dataset_inst: od.Dataset,
         shift_inst: od.Shift,
         dataset_key: str,
     ) -> list[str]:
+        """
+        Get the LNF information with the ``dasgoclient``.
+
+        :param dataset_inst: Current dataset instance, currently not used.
+        :param shift_inst: Current shift instance, currently not used.
+        :param dataset_key: DAS key identifier for the current dataset.
+        :raises Exception: If query with ``dasgoclient`` fails.
+        :return: The list of LFNs corresponding to the dataset with the identifier *dataset_key*.
+        """
         code, out, _ = law.util.interruptable_popen(
             f"dasgoclient --query='file dataset={dataset_key}' --limit=0",
             shell=True,
             stdout=subprocess.PIPE,
             executable="/bin/bash",
         )
         if code != 0:
@@ -117,21 +154,25 @@
         Generator function that reduces the boilerplate code for looping over files referred to by
         *lfn_indices* given the lfns obtained by *this* task which needs to be complete for this
         function to succeed.
 
         When *lfn_indices* are not given, *task* must be a branch of a :py:class:`DatasetTask`
         workflow whose branch value is used instead.
 
-        Iterating yields a 2-tuple (file index, input file) where the latter is either a
-        :py:class:`law.LocalFileTarget` or a :py:class:`law.wlcg.WLCGFileTarget` with its fs set to
-        *remote_fs*. When a sequence is passed, the fs names are evaluated in that order and the
-        first existing one is generally used. However, if *eager_lookup* is *True*, in case the stat
-        request to a fs was successful but took longer than two seconds, the next fs is eagerly
-        checked and used in case it responded with less delay. In case *eager_lookup* is an integer,
-        this check is only performed after the *eager_lookup*th fs.
+        :param task: Current task that needs to access the nanoAOD files
+        :param remote_fs: Name of the remote file system where the LFNs are located, defaults to None
+        :param lfn_indices: List of indices of LFNs that are processed by this *task* instance, defaults to None
+        :param eager_lookup: Look at the next remote fs in *remote_fs* if stat takes too long, defaults to 1
+        :raises TypeError: If *task* is not of type :external+law:py:class:`~law.workflow.base.BaseWorkflow` or not
+            a task analyzing a single branch in the task tree
+        :raises Exception: If current task is not complete as indicated with ``self.complete()``
+        :raises ValueError: If no remote fs is provided at call and none can be found in either the config instance
+            or the law config.
+        :raises Exception: If a given LFN cannot be found at any remote file system
+        :yield: a file target that points to a LFN
         """
         # input checks
         if not lfn_indices:
             if not isinstance(task, law.BaseWorkflow) or not task.is_branch():
                 raise TypeError(f"task must be a workflow branch, but got {task}")
             lfn_indices = task.branch_data
         if not self.complete():
@@ -220,18 +261,54 @@
 
 
 GetDatasetLFNsWrapper = wrapper_factory(
     base_cls=AnalysisTask,
     require_cls=GetDatasetLFNs,
     enable=["configs", "skip_configs", "datasets", "skip_datasets", "shifts", "skip_shifts"],
     attributes={"version": None},
+    docs="""
+Wrapper task to get LFNs for multiple datasets.
+
+:enables: ["configs", "skip_configs", "datasets", "skip_datasets", "shifts", "skip_shifts"]
+:overwrites: attribute ``version`` with None
+""",
 )
 
 
 class BundleExternalFiles(ConfigTask, law.tasks.TransferLocalFile):
+    """
+    Task to collect external files.
+
+    This task is intended to download source files for other tasks, such as files containing
+    corrections for objects, the "golden" json files, source files for the calculation of pileup
+    weights, and others.
+
+    All information about the relevant external files is extracted from the given ``config_inst``,
+    which must contain the keyword ``external_files`` in the auxiliary information. This can look
+    like this:
+
+    .. code-block:: python
+
+        # cfg is the current config instance
+        cfg.x.external_files = DotDict.wrap({
+        # The following assumes that the zip files are reachable under the
+        # url ``SOURCE_URL``
+        # jet energy correction
+        "jet_jerc": (f"{SOURCE_URL}/POG/JME/{year}{corr_postfix}_UL/jet_jerc.json.gz", "v1"),
+
+        # tau energy correction and scale factors
+        "tau_sf": (f"{SOURCE_URL}/POG/TAU/{year}{corr_postfix}_UL/tau.json.gz", "v1"),
+
+        # electron scale factors
+        "electron_sf": (f"{SOURCE_URL}/POG/EGM/{year}{corr_postfix}_UL/electron.json.gz", "v1"),
+
+    The entries in this DotDict can either be simply the path to the source files or can be a tuple
+    of the format ``(path/or/url/to/source/file, VERSION)`` to introduce a versioning mechanism for
+    external files.
+    """
 
     replicas = luigi.IntParameter(
         default=5,
         description="number of replicas to generate; default: 5",
     )
     version = None
 
@@ -245,48 +322,64 @@
         self._file_names = None
 
         # cached dict for lazy access to files in fetched bundle
         self.files_dir = None
         self._files = None
 
     @classmethod
-    def create_unique_basename(cls, path):
+    def create_unique_basename(cls, path: tuple[str] | str) -> str:
+        """
+        Create a unique basename.
+
+        :param path: path to create a unique basename for
+        :return: Unique basename
+        """
         h = law.util.create_hash(path)
         basename = os.path.basename(path[0] if isinstance(path, tuple) else path)
         return f"{h}_{basename}"
 
     @property
-    def files_hash(self):
+    def files_hash(self) -> str:
+        """
+        Create a hash based on all external files.
+
+        :return: Hash based on the flattened list of external files in the current config instance.
+        """
         if self._files_hash is None:
             # take the external files and flatten them into a deterministic order, then hash
             def deterministic_flatten(d):
                 return [
                     (key, (deterministic_flatten(d[key]) if isinstance(d[key], dict) else d[key]))
                     for key in sorted(d)
                 ]
             flat_files = deterministic_flatten(self.config_inst.x.external_files)
             self._files_hash = law.util.create_hash(flat_files)
 
         return self._files_hash
 
     @property
-    def file_names(self):
+    def file_names(self) -> DotDict:
+        """
+        Create a unique basename for each external file.
+
+        :return: DotDict of same shape as ``external_files`` DotDict with unique basenames.
+        """
         if self._file_names is None:
             self._file_names = law.util.map_struct(
                 self.create_unique_basename,
                 self.config_inst.x.external_files,
             )
 
         return self._file_names
 
-    @property
-    def files(self):
+    def get_files(self, output=None):
         if self._files is None:
             # get the output
-            output = self.output()
+            if not output:
+                output = self.output()
             if not output.exists():
                 raise Exception(
                     f"accessing external files from the bundle requires the output of {self} to "
                     "exist, but it appears to be missing",
                 )
             if isinstance(output, law.FileCollection):
                 output = output.random_target()
@@ -297,14 +390,18 @@
             def resolve_basename(unique_basename):
                 return self.files_dir.child(unique_basename, type="f")
 
             self._files = law.util.map_struct(resolve_basename, self.file_names)
 
         return self._files
 
+    @property
+    def files(self):
+        return self.get_files()
+
     def single_output(self):
         # required by law.tasks.TransferLocalFile
         return self.target(f"externals_{self.files_hash}.tgz")
 
     @law.decorator.log
     @law.decorator.safe_output
     def run(self):
```

### Comparing `columnflow-0.2.1/columnflow/tasks/framework/base.py` & `columnflow-0.2.2/columnflow/tasks/framework/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,27 +8,31 @@
 
 import os
 import enum
 import importlib
 import itertools
 import inspect
 import functools
-from typing import Sequence
+from typing import Sequence, Callable, Any
 
 import luigi
 import law
 import order as od
 
 from columnflow.util import DotDict
 
 
+# default analysis and config related objects
 default_analysis = law.config.get_expanded("analysis", "default_analysis")
 default_config = law.config.get_expanded("analysis", "default_config")
 default_dataset = law.config.get_expanded("analysis", "default_dataset")
 
+# placeholder to denote a default value that is resolved dynamically
+RESOLVE_DEFAULT = "DEFAULT"
+
 
 class Requirements(DotDict):
 
     def __init__(self, *others, **kwargs):
         super().__init__()
 
         # add others and kwargs
@@ -56,44 +60,46 @@
 
 class AnalysisTask(BaseTask, law.SandboxTask):
 
     analysis = luigi.Parameter(
         default=default_analysis,
         description=f"name of the analysis; default: '{default_analysis}'",
     )
-    version = luigi.Parameter(description="mandatory version that is encoded into output paths")
+    version = luigi.Parameter(
+        description="mandatory version that is encoded into output paths",
+    )
 
     allow_empty_sandbox = True
     sandbox = None
 
     message_cache_size = 25
     local_workflow_require_branches = False
     output_collection_cls = law.SiblingFileCollection
 
     # defaults for targets
     default_store = "$CF_STORE_LOCAL"
     default_wlcg_fs = law.config.get_expanded("target", "default_wlcg_fs")
     default_output_location = "config"
 
     @classmethod
+    def modify_param_values(cls, params: dict) -> dict:
+        params = super().modify_param_values(params)
+        params = cls.resolve_param_values(params)
+        return params
+
+    @classmethod
     def resolve_param_values(cls, params: dict) -> dict:
         # store a reference to the analysis inst
         if "analysis_inst" not in params and "analysis" in params:
             params["analysis_inst"] = cls.get_analysis_inst(params["analysis"])
 
         return params
 
     @classmethod
-    def modify_param_values(cls, params: dict) -> dict:
-        params = super().modify_param_values(params)
-        params = cls.resolve_param_values(params)
-        return params
-
-    @classmethod
-    def get_analysis_inst(cls, analysis):
+    def get_analysis_inst(cls, analysis: str) -> od.Analysis:
         # prepare names
         if "." not in analysis:
             raise ValueError(f"invalid analysis format: {analysis}")
         module_id, name = analysis.rsplit(".", 1)
 
         # import the module
         try:
@@ -105,61 +111,66 @@
         analysis_inst = getattr(mod, name, None)
         if analysis_inst is None:
             raise Exception(f"module {module_id} does not contain analysis instance {name}")
 
         return analysis_inst
 
     @classmethod
-    def req_params(cls, inst, **kwargs):
+    def req_params(cls, inst: AnalysisTask, **kwargs) -> dict:
         """
         Returns parameters that are jointly defined in this class and another task instance of some
         other class. The parameters are used when calling ``Task.req(self)``.
         """
         # always prefer certain parameters given as task family parameters (--TaskFamily-parameter)
-        _prefer_cli = set(law.util.make_list(kwargs.get("_prefer_cli", [])))
-        _prefer_cli |= {
+        _prefer_cli = law.util.make_set(kwargs.get("_prefer_cli", [])) | {
             "version", "workflow", "job_workers", "poll_interval", "walltime", "max_runtime",
             "retries", "acceptance", "tolerance", "parallel_jobs", "shuffle_jobs", "htcondor_cpus",
             "htcondor_gpus", "htcondor_pool",
         }
         kwargs["_prefer_cli"] = _prefer_cli
 
-        # when cls accepts a version, but non was actively requested, use the version map to assign it
-        version_map = None
-        if isinstance(getattr(cls, "version", None), luigi.Parameter) and "version" not in kwargs:
-            version_map = cls.get_version_map(inst)
-
         # build the params
         params = super().req_params(inst, **kwargs)
 
-        # when the version map is set, lookup the key with which to find a version in the map and overwrite it
-        if version_map and cls.task_family in version_map:
-            version_params = list(cls.get_version_params())
-            version = version_map[cls.task_family]
-            while isinstance(version, dict) and version_params:
-                param = version_params.pop(0)
-                if param not in params:
-                    break
-                value = params[param]
-                if value not in version:
-                    if None not in version:
-                        break
-                    value = None
-                version = version[value]
-            params["version"] = version
+        # overwrite the version when set in the config
+        if isinstance(getattr(cls, "version", None), luigi.Parameter) and "version" not in kwargs:
+            if config_version := cls.get_version_map_value(inst, params):
+                params["version"] = config_version
 
         return params
 
     @classmethod
-    def get_version_map(cls, task):
+    def get_version_map(cls, task: AnalysisTask) -> dict[str, str | Callable]:
         return task.analysis_inst.get_aux("versions", {})
 
     @classmethod
-    def get_version_params(cls):
-        return ()
+    def get_version_map_value(
+        cls,
+        inst: AnalysisTask,
+        params: dict,
+        version_map: dict[str, str | Callable] | None = None,
+    ) -> str | None:
+        if version_map is None:
+            version_map = cls.get_version_map(inst)
+
+        # the task family must be in the version map
+        if not (version := version_map.get(cls.task_family)):
+            return None
+
+        # when version is a callable, invoke it
+        if callable(version):
+            version = version(cls, inst, params)
+
+        # at this point, version must be a string
+        if not isinstance(version, str):
+            raise TypeError(
+                f"version map entry for '{cls.task_family}' must be a string, but got {version}",
+            )
+
+        return version
 
     @classmethod
     def get_known_shifts(cls, config_inst: od.Config, params: dict) -> tuple[set[str], set[str]]:
         """
         Returns two sets of shifts in a tuple: shifts implemented by _this_ task, and depdenent
         shifts implemented by upstream tasks.
         """
@@ -167,39 +178,43 @@
         upstream_shifts = set()
         for req in cls.reqs.values():
             upstream_shifts |= set.union(*(req.get_known_shifts(config_inst, params) or (set(),)))
 
         return set(), upstream_shifts
 
     @classmethod
-    def get_array_function_kwargs(cls, task=None, **params):
+    def get_array_function_kwargs(
+        cls,
+        task: AnalysisTask | None = None,
+        **params,
+    ) -> dict[str, Any]:
         if task:
             analysis_inst = task.analysis_inst
         elif "analysis_inst" in params:
             analysis_inst = params["analysis_inst"]
         else:
             analysis_inst = cls.get_analysis_inst(params["analysis"])
 
         return {
             "task": task,
             "analysis_inst": analysis_inst,
         }
 
     @classmethod
-    def get_calibrator_kwargs(cls, *args, **kwargs):
+    def get_calibrator_kwargs(cls, *args, **kwargs) -> dict[str, Any]:
         # implemented here only for simplified mro control
         return cls.get_array_function_kwargs(*args, **kwargs)
 
     @classmethod
-    def get_selector_kwargs(cls, *args, **kwargs):
+    def get_selector_kwargs(cls, *args, **kwargs) -> dict[str, Any]:
         # implemented here only for simplified mro control
         return cls.get_array_function_kwargs(*args, **kwargs)
 
     @classmethod
-    def get_producer_kwargs(cls, *args, **kwargs):
+    def get_producer_kwargs(cls, *args, **kwargs) -> dict[str, Any]:
         # implemented here only for simplified mro control
         return cls.get_array_function_kwargs(*args, **kwargs)
 
     @classmethod
     def find_config_objects(
         cls,
         names: str | Sequence[str] | set[str],
@@ -245,42 +260,248 @@
                 _cache["has_obj_func"] = functools.partial(
                     getattr(container, "has_{}".format(singular)),
                     **kwargs,
                 )
             return _cache["has_obj_func"](name)
 
         object_names = []
-        patterns = []
         lookup = law.util.make_list(names)
         while lookup:
             name = lookup.pop(0)
             if has_obj(name):
                 # known object
                 object_names.append(name)
             elif object_groups and name in object_groups:
                 # a key in the object group dict
                 lookup.extend(list(object_groups[name]))
             elif accept_patterns:
-                # must eventually be a pattern, store it for object traversal
-                # special case
-                if name == "*":
-                    object_names = list(get_all_object_names())
-                    del patterns[:]
-                    break
-                patterns.append(name)
-
-        # if patterns are found, loop through them to preserve the order of patterns
-        # and compare to all existing names
-        for pattern in patterns:
-            for name in get_all_object_names():
-                if law.util.multi_match(name, pattern):
-                    object_names.append(name)
+                # must eventually be a pattern, perform an object traversal
+                for _name in get_all_object_names():
+                    if law.util.multi_match(_name, name):
+                        object_names.append(_name)
 
         return law.util.make_unique(object_names)
 
+    @classmethod
+    def resolve_config_default(
+        cls,
+        task_params: dict[str, Any],
+        param: str | tuple[str] | None,
+        container: str | od.AuxDataMixin = "config_inst",
+        default_str: str | None = None,
+        multiple: bool = False,
+    ) -> str | tuple | Any | None:
+        """
+        Resolves a given parameter value *param*, checks if it should be placed with a default value
+        when empty, and in this case, does the actual default value resolution.
+
+        This resolution is triggered only in case *param* refers to :py:attr:`RESOLVE_DEFAULT`, a
+        1-tuple containing this attribute, or *None*, If so, the default is identified via the
+        *default_str* from an :py:class:`order.AuxDataMixin` *container* and points to an auxiliary
+        that can be either a string or a function. In the latter case, it is called with the task
+        class, the container instance, and all task parameters. Note that when no *container* is
+        given, *param* is returned unchanged.
+
+        When *multiple* is *True*, a tuple is returned. If *multiple* is *False* and the resolved
+        parameter is an iterable, the first entry is returned.
+
+        Example:
+
+        .. code-block:: python
+
+            def resolve_param_values(params):
+                params["producer"] = AnalysisTask.resolve_config_default(
+                    params,
+                    params.get("producer"),
+                    container=params["config_inst"]
+                    default_str="default_producer",
+                    multiple=True,
+                )
+
+            config_inst = od.Config(
+                id=0,
+                name="my_config",
+                aux={"default_producer": ["my_producer_1", "my_producer_2"]},
+            )
+
+            params = {
+                "config_inst": config_inst,
+                "producer": RESOLVE_DEFAULT,
+            }
+            resolve_param_values(params)  # sets params["producer"] to ("my_producer_1", "my_producer_2")
+
+            params = {
+                "config_inst": config_inst,
+                "producer": "some_other_producer",
+            }
+            resolve_param_values(params)  # sets params["producer"] to "some_other_producer"
+
+        Example where the default points to a function:
+
+        .. code-block:: python
+            def resolve_param_values(params):
+                params["ml_model"] = AnalysisTask.resolve_config_default(
+                    params,
+                    params.get("ml_model"),
+                    container=params["config_inst"]
+                    default_str="default_ml_model",
+                    multiple=True,
+                )
+
+            # a function that chooses the ml_model based on an attibute that is set in an inference_model
+            def default_ml_model(task_cls, container, task_params):
+                default_ml_model = None
+
+                # check if task is using an inference model
+                if "inference_model" in task_params.keys():
+                    inference_model = task_params.get("inference_model", None)
+
+                    # if inference model is not set, assume it's the container default
+                    if inference_model in (None, "NO_STR"):
+                        inference_model = container.x.default_inference_model
+
+                    # get the default_ml_model from the inference_model_inst
+                    inference_model_inst = columnflow.inference.InferenceModel._subclasses[inference_model]
+                    default_ml_model = getattr(inference_model_inst, "ml_model_name", default_ml_model)
+
+                    return default_ml_model
+
+                return default_ml_model
+
+            config_inst = od.Config(
+                id=0,
+                name="my_config",
+                aux={"default_ml_model": default_ml_model},
+            )
+
+            @inference_model(ml_model_name="default_ml_model")
+            def my_inference_model(self):
+                # some inference model implementation
+                ...
+
+            params = {"config_inst": config_inst, "ml_model": None, "inference_model": "my_inference_model"}
+            resolve_param_values(params)  # sets params["ml_model"] to "my_ml_model"
+
+            params = {"config_inst": config_inst, "ml_model": "some_ml_model", "inference_model": "my_inference_model"}
+            resolve_param_values(params)  # sets params["ml_model"] to "some_ml_model"
+        """
+        # check if the parameter value is to be resolved
+        resolve_default = param in (None, RESOLVE_DEFAULT, (RESOLVE_DEFAULT,))
+
+        # interpret missing parameters (e.g. NO_STR) as None
+        # (special case: an empty string is usually an active decision, but counts as missing too)
+        if law.is_no_param(param) or resolve_default or param == "":
+            param = None
+
+        # actual resolution
+        if resolve_default:
+            # get the container inst (mostly a config_inst or analysis_inst)
+            if isinstance(container, str):
+                container = task_params.get(container)
+
+            # expand default when container is set
+            if container and default_str:
+                param = container.x(default_str, None) if default_str else None
+
+                # allow default to be a function, taking task parameters as input
+                if isinstance(param, Callable):
+                    param = param(cls, container, task_params)
+
+        # when still empty, return an empty value
+        if param is None:
+            return () if multiple else None
+
+        # return either a tuple or the first param, based on the *multiple*
+        param = law.util.make_tuple(param)
+        return param if multiple else (param[0] if param else None)
+
+    @classmethod
+    def resolve_config_default_and_groups(
+        cls,
+        task_params: dict[str, Any],
+        param: str | tuple[str] | None,
+        container: str | od.AuxDataMixin = "config_inst",
+        default_str: str | None = None,
+        groups_str: str | None = None,
+    ) -> tuple[str]:
+        """
+        This method is similar to :py:meth:`~.resolve_config_default` in that it checks if a
+        parameter value *param* is empty and should be replaced with a default value. See the
+        referenced method for documentation on *task_params*, *param*, *container* and
+        *default_str*.
+
+        What this method does in addition is that it checks if the values contained in *param*
+        (after default value resolution) refers to a group of values identified via the *groups_str*
+        from the :py:class:`order.AuxDataMixin` *container* that maps a string to a tuple of
+        strings. If it does, each value in *param* that refers to a group is expanded by the actual
+        group values.
+
+        Example:
+
+        .. code-block:: python
+
+            config_inst = od.Config(
+                id=0,
+                name="my_config",
+                aux={
+                    "default_producer": ["features_1", "my_producer_group"],
+                    "producer_groups": {"my_producer_group": ["features_2", "features_3"]},
+                },
+            )
+
+            params = {"producer": RESOLVE_DEFAULT}
+
+            AnalysisTask.resolve_config_default_and_groups(
+                params,
+                params.get("producer"),
+                container=config_inst,
+                default_str="default_producer",
+                groups_str="producer_groups",
+            )
+            # -> ("features_1", "features_2", "features_3")
+        """
+        # resolve the parameter
+        param = cls.resolve_config_default(
+            task_params=task_params,
+            param=param,
+            container=container,
+            default_str=default_str,
+            multiple=True,
+        )
+        if not param:
+            return param
+
+        # get the container inst and return if it's not set
+        if isinstance(container, str):
+            container = task_params.get(container, None)
+
+        if not container:
+            return param
+
+        # expand groups recursively
+        if groups_str and (param_groups := container.x(groups_str, {})):
+            values = []
+            lookup = law.util.make_list(param)
+            handled_groups = set()
+            while lookup:
+                value = lookup.pop(0)
+                if value in param_groups:
+                    if value in handled_groups:
+                        raise Exception(
+                            f"definition of '{groups_str}' contains circular references involving "
+                            f"group '{value}'",
+                        )
+                    lookup = law.util.make_list(param_groups[value]) + lookup
+                    handled_groups.add(value)
+                else:
+                    values.append(value)
+            param = values
+
+        return law.util.make_tuple(param)
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # store the analysis instance
         self.analysis_inst = self.get_analysis_inst(self.analysis)
 
     def store_parts(self):
@@ -477,31 +698,14 @@
     exclude_params_req = {"local_shift"}
     exclude_params_sandbox = {"local_shift"}
     exclude_params_remote_workflow = {"local_shift"}
 
     allow_empty_shift = False
 
     @classmethod
-    def get_version_params(cls):
-        params = super().get_version_params()
-        if cls.shift:
-            params += ("shift",)
-        return params
-
-    @classmethod
-    def resolve_param_values(cls, params: dict) -> dict:
-        params = super().resolve_param_values(params)
-
-        # set default shift
-        if params.get("shift") in (None, law.NO_STR):
-            params["shift"] = "nominal"
-
-        return params
-
-    @classmethod
     def modify_param_values(cls, params):
         """
         When "config" and "shift" are set, this method evaluates them to set the global shift.
         For that, it takes the shifts stored in the config instance and compares it with those
         defined by this class.
         """
         params = super().modify_param_values(params)
@@ -546,20 +750,30 @@
         # store references
         params["global_shift_inst"] = config_inst.get_shift(params["shift"])
         params["local_shift_inst"] = config_inst.get_shift(params["local_shift"])
 
         return params
 
     @classmethod
+    def resolve_param_values(cls, params: dict) -> dict:
+        params = super().resolve_param_values(params)
+
+        # set default shift
+        if params.get("shift") in (None, law.NO_STR):
+            params["shift"] = "nominal"
+
+        return params
+
+    @classmethod
     def get_array_function_kwargs(cls, task=None, **params):
         kwargs = super().get_array_function_kwargs(task=task, **params)
 
         if task:
             if task.local_shift_inst:
-                kwargs["shift_inst"] = task.local_shift_inst
+                kwargs["local_shift_inst"] = task.local_shift_inst
             if task.global_shift_inst:
                 kwargs["global_shift_inst"] = task.global_shift_inst
         else:
             if "local_shift_inst" in params:
                 kwargs["local_shift_inst"] = params["local_shift_inst"]
             if "global_shift_inst" in params:
                 kwargs["global_shift_inst"] = params["global_shift_inst"]
@@ -619,23 +833,14 @@
             else:
                 # extend with dataset variations for mc
                 upstream_shifts |= set(dataset_inst.info.keys())
 
         return shifts, upstream_shifts
 
     @classmethod
-    def get_version_params(cls):
-        params = super().get_version_params()
-        if cls.shift:
-            params = params[:-1] + ("dataset", "shift")
-        else:
-            params += ("dataset",)
-        return params
-
-    @classmethod
     def get_array_function_kwargs(cls, task=None, **params):
         kwargs = super().get_array_function_kwargs(task=task, **params)
 
         if task:
             kwargs["dataset_inst"] = task.dataset_inst
         elif "dataset_inst" in params:
             kwargs["dataset_inst"] = params["dataset_inst"]
@@ -837,24 +1042,26 @@
 
 def wrapper_factory(
     base_cls: law.Task,
     require_cls: AnalysisTask,
     enable: Sequence[str],
     cls_name: str | None = None,
     attributes: dict | None = None,
+    docs: str | None = None,
 ) -> law.task.base.Register:
     """
     Factory function creating wrapper task classes, inheriting from *base_cls* and
-    ``law.WrapperTask``, that do nothing but require multiple instances of *require_cls*. Unless
-    *cls_name* is defined, the name of the created class defaults to the name of *require_cls* plus
-    "Wrapper". Additional *attributes* are added as class-level members when given.
-
-    The instances of *require_cls* to be required in the ``requires()`` method can be controlled by
-    task parameters. These parameters can be enabled through the string sequence *enable*, which
-    currently accepts:
+    :py:class:`~law.WrapperTask`, that do nothing but require multiple instances of *require_cls*.
+        Unless *cls_name* is defined, the name of the created class defaults to the name of
+        *require_cls* plus "Wrapper". Additional *attributes* are added as class-level members when
+        given.
+
+    The instances of *require_cls* to be required in the
+    :py:meth:`~.wrapper_factory.Wrapper.requires()` method can be controlled by task parameters.
+    These parameters can be enabled through the string sequence *enable*, which currently accepts:
 
         - ``configs``, ``skip_configs``
         - ``shifts``, ``skip_shifts``
         - ``datasets``, ``skip_datasets``
 
     This allows to easily build wrapper tasks that loop over (combinations of) parameters that are
     either defined in the analysis or config, which would otherwise lead to mostly redundant code.
@@ -875,15 +1082,15 @@
         # law run MyTaskWrapper --datasets st_* --skip-datasets *_tbar
 
     When building the requirements, the full combinatorics of parameters is considered. However,
     certain conditions apply depending on enabled features. For instance, in order to use the
     "configs" feature (adding a parameter "--configs" to the created class, allowing to loop over a
     list of config instances known to an analysis), *require_cls* must be at least a
     :py:class:`ConfigTask` accepting "--config" (mind the singular form), whereas *base_cls* must
-    explicitly not.
+        explicitly not.
     """
     # check known features
     known_features = [
         "configs", "skip_configs",
         "shifts", "skip_shifts",
         "datasets", "skip_datasets",
     ]
@@ -1139,8 +1346,12 @@
     frame = inspect.stack()[1]
     module = inspect.getmodule(frame[0])
     Wrapper.__module__ = module.__name__
 
     # overwrite __name__
     Wrapper.__name__ = cls_name or require_cls.__name__ + "Wrapper"
 
+    # set docs
+    if docs:
+        Wrapper.__docs__ = docs
+
     return Wrapper
```

### Comparing `columnflow-0.2.1/columnflow/tasks/framework/decorators.py` & `columnflow-0.2.2/columnflow/tasks/framework/decorators.py`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.1/columnflow/tasks/framework/mixins.py` & `columnflow-0.2.2/columnflow/tasks/framework/mixins.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,74 +11,79 @@
 import itertools
 from typing import Sequence, Any
 
 import luigi
 import law
 import order as od
 
-from columnflow.tasks.framework.base import AnalysisTask, ConfigTask
+from columnflow.tasks.framework.base import AnalysisTask, ConfigTask, RESOLVE_DEFAULT
 from columnflow.calibration import Calibrator
 from columnflow.selection import Selector
 from columnflow.production import Producer
 from columnflow.ml import MLModel
 from columnflow.inference import InferenceModel
 from columnflow.util import maybe_import
 
 
 ak = maybe_import("awkward")
 
 
 class CalibratorMixin(ConfigTask):
 
     calibrator = luigi.Parameter(
-        default=law.NO_STR,
+        default=RESOLVE_DEFAULT,
         description="the name of the calibrator to be applied; default: value of the "
         "'default_calibrator' config",
     )
 
     # decibes whether the task itself runs the calibrator and implements its shifts
     register_calibrator_shifts = False
 
     @classmethod
-    def get_default_calibrator(cls, config_inst, calibrator=None) -> str | None:
-        if calibrator and calibrator != law.NO_STR:
-            return calibrator
-
-        return config_inst.x("default_calibrator", None)
-
-    @classmethod
     def get_calibrator_inst(cls, calibrator, kwargs=None):
         inst_dict = cls.get_calibrator_kwargs(**kwargs) if kwargs else None
         return Calibrator.get_cls(calibrator)(inst_dict=inst_dict)
 
     @classmethod
     def resolve_param_values(cls, params):
         params = super().resolve_param_values(params)
 
-        # add the default calibrator when empty
-        if "config_inst" in params:
-            params["calibrator"] = cls.get_default_calibrator(params["config_inst"], params.get("calibrator"))
+        if config_inst := params.get("config_inst"):
+            # add the default calibrator when empty
+            params["calibrator"] = cls.resolve_config_default(
+                params,
+                params.get("calibrator"),
+                container=config_inst,
+                default_str="default_calibrator",
+                multiple=False,
+            )
             params["calibrator_inst"] = cls.get_calibrator_inst(params["calibrator"], params)
 
         return params
 
     @classmethod
     def get_known_shifts(cls, config_inst: od.Config, params: dict) -> tuple[set[str], set[str]]:
         shifts, upstream_shifts = super().get_known_shifts(config_inst, params)
 
         # get the calibrator, update it and add its shifts
-        calibrator_inst = params.get("calibrator_inst")
-        if calibrator_inst:
+        if calibrator_inst := params.get("calibrator_inst"):
             if cls.register_calibrator_shifts:
                 shifts |= calibrator_inst.all_shifts
             else:
                 upstream_shifts |= calibrator_inst.all_shifts
 
         return shifts, upstream_shifts
 
+    @classmethod
+    def req_params(cls, inst: law.Task, **kwargs) -> dict:
+        # prefer --calibrator set on task-level via cli
+        kwargs["_prefer_cli"] = law.util.make_set(kwargs.get("_prefer_cli", [])) | {"calibrator"}
+
+        return super().req_params(inst, **kwargs)
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # cache for calibrator inst
         self._calibrator_inst = None
 
     @property
@@ -97,65 +102,67 @@
         parts.insert_before("version", "calibrator", f"calib__{self.calibrator}")
         return parts
 
 
 class CalibratorsMixin(ConfigTask):
 
     calibrators = law.CSVParameter(
-        default=(),
+        default=(RESOLVE_DEFAULT,),
         description="comma-separated names of calibrators to be applied; default: value of the "
         "'default_calibrator' config in a 1-tuple",
         brace_expand=True,
     )
 
     # decibes whether the task itself runs the calibrators and implements their shifts
     register_calibrators_shifts = False
 
     @classmethod
-    def get_default_calibrators(cls, config_inst, calibrators=None) -> tuple[str]:
-        if calibrators and calibrators != law.NO_STR:
-            return calibrators
-
-        if config_inst.x("default_calibrator", None):
-            return (config_inst.x.default_calibrator,)
-
-        return ()
-
-    @classmethod
     def get_calibrator_insts(cls, calibrators, kwargs=None):
         inst_dict = cls.get_calibrator_kwargs(**kwargs) if kwargs else None
         return [
             Calibrator.get_cls(calibrator)(inst_dict=inst_dict)
             for calibrator in calibrators
         ]
 
     @classmethod
     def resolve_param_values(cls, params):
         params = super().resolve_param_values(params)
 
-        if "config_inst" in params:
-            params["calibrators"] = cls.get_default_calibrators(params["config_inst"], params.get("calibrators"))
+        if config_inst := params.get("config_inst"):
+            params["calibrators"] = cls.resolve_config_default_and_groups(
+                params,
+                params.get("calibrators"),
+                container=config_inst,
+                default_str="default_calibrator",
+                groups_str="calibrator_groups",
+            )
             params["calibrator_insts"] = cls.get_calibrator_insts(params["calibrators"], params)
 
         return params
 
     @classmethod
     def get_known_shifts(cls, config_inst: od.Config, params: dict) -> tuple[set[str], set[str]]:
         shifts, upstream_shifts = super().get_known_shifts(config_inst, params)
 
         # get the calibrators, update them and add their shifts
-        calibrator_insts = params.get("calibrator_insts")
-        for calibrator_inst in calibrator_insts or []:
+        for calibrator_inst in params.get("calibrator_insts") or []:
             if cls.register_calibrators_shifts:
                 shifts |= calibrator_inst.all_shifts
             else:
                 upstream_shifts |= calibrator_inst.all_shifts
 
         return shifts, upstream_shifts
 
+    @classmethod
+    def req_params(cls, inst: law.Task, **kwargs) -> dict:
+        # prefer --calibrators set on task-level via cli
+        kwargs["_prefer_cli"] = law.util.make_set(kwargs.get("_prefer_cli", [])) | {"calibrators"}
+
+        return super().req_params(inst, **kwargs)
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # cache for calibrator insts
         self._calibrator_insts = None
 
     @property
@@ -166,72 +173,77 @@
 
     def store_parts(self):
         parts = super().store_parts()
 
         part = "__".join(self.calibrators[:5])
         if len(self.calibrators) > 5:
             part += f"__{law.util.create_hash(self.calibrators[5:])}"
-        parts.insert_before("version", "calibrators", f"calib__{part}")
+        parts.insert_before("version", "calibrators", f"calib__{part or 'none'}")
 
         return parts
 
 
 class SelectorMixin(ConfigTask):
 
     selector = luigi.Parameter(
-        default=law.NO_STR,
+        default=RESOLVE_DEFAULT,
         description="the name of the selector to be applied; default: value of the "
         "'default_selector' config",
     )
 
     # decibes whether the task itself runs the selector and implements its shifts
     register_selector_shifts = False
 
     @classmethod
-    def get_default_selector(cls, config_inst, selector=None) -> str | None:
-        if selector and selector != law.NO_STR:
-            return selector
-
-        return config_inst.x("default_selector", None)
-
-    @classmethod
     def get_selector_inst(cls, selector, kwargs=None):
         selector_cls = Selector.get_cls(selector)
 
         if not selector_cls.exposed:
             raise RuntimeError(f"cannot use unexposed selector '{selector}' in {cls.__name__}")
 
         inst_dict = cls.get_selector_kwargs(**kwargs) if kwargs else None
         return selector_cls(inst_dict=inst_dict)
 
     @classmethod
     def resolve_param_values(cls, params):
         params = super().resolve_param_values(params)
 
         # add the default selector when empty
-        if "config_inst" in params:
-            params["selector"] = cls.get_default_selector(params["config_inst"], params.get("selector"))
+        if config_inst := params.get("config_inst"):
+            params["selector"] = cls.resolve_config_default(
+                params,
+                params.get("selector"),
+                container=config_inst,
+                default_str="default_selector",
+                multiple=False,
+            )
             params["selector_inst"] = cls.get_selector_inst(params["selector"], params)
 
         return params
 
     @classmethod
     def get_known_shifts(cls, config_inst: od.Config, params: dict) -> tuple[set[str], set[str]]:
         shifts, upstream_shifts = super().get_known_shifts(config_inst, params)
 
         # get the selector, update it and add its shifts
-        selector_inst = params.get("selector_inst")
-        if selector_inst:
+        if selector_inst := params.get("selector_inst"):
             if cls.register_selector_shifts:
                 shifts |= selector_inst.all_shifts
             else:
                 upstream_shifts |= selector_inst.all_shifts
 
         return shifts, upstream_shifts
 
+    @classmethod
+    def req_params(cls, inst: law.Task, **kwargs) -> dict:
+        # prefer --selector set on task-level via cli
+        kwargs["_prefer_cli"] = law.util.make_set(kwargs.get("_prefer_cli", [])) | {"selector"}
+
+        return super().req_params(inst, **kwargs)
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # cache for selector inst
         self._selector_inst = None
 
     @property
@@ -264,30 +276,37 @@
 
     selector_steps_order_sensitive = False
 
     @classmethod
     def resolve_param_values(cls, params: dict[str, Any]) -> dict[str, Any]:
         params = super().resolve_param_values(params)
 
-        # expand selector step groups
-        if "config_inst" in params and len(params.get("selector_steps", [])) == 1:
-            config_inst = params["config_inst"]
-            step_group = params["selector_steps"][0]
-            params["selector_steps"] = (
-                tuple(config_inst.x.selector_step_groups[step_group])
-                if step_group in config_inst.x("selector_step_groups", {}) else
-                tuple()
+        # apply selector_steps_groups and default_selector_steps from config
+        if config_inst := params.get("config_inst"):
+            params["selector_steps"] = cls.resolve_config_default_and_groups(
+                params,
+                params.get("selector_steps"),
+                container=config_inst,
+                default_str="default_selector_steps",
+                groups_str="selector_step_groups",
             )
 
         # sort selector steps when the order does not matter
         if not cls.selector_steps_order_sensitive and "selector_steps" in params:
             params["selector_steps"] = tuple(sorted(params["selector_steps"]))
 
         return params
 
+    @classmethod
+    def req_params(cls, inst: law.Task, **kwargs) -> dict:
+        # prefer --selector-steps set on task-level via cli
+        kwargs["_prefer_cli"] = law.util.make_set(kwargs.get("_prefer_cli", [])) | {"selector_steps"}
+
+        return super().req_params(inst, **kwargs)
+
     def store_parts(self) -> law.util.InsertableDict:
         parts = super().store_parts()
 
         steps = self.selector_steps
         if not self.selector_steps_order_sensitive:
             steps = sorted(steps)
         if steps:
@@ -295,59 +314,64 @@
 
         return parts
 
 
 class ProducerMixin(ConfigTask):
 
     producer = luigi.Parameter(
-        default=law.NO_STR,
+        default=RESOLVE_DEFAULT,
         description="the name of the producer to be applied; default: value of the "
         "'default_producer' config",
     )
 
     # decibes whether the task itself runs the producer and implements its shifts
     register_producer_shifts = False
 
     @classmethod
-    def get_default_producer(cls, config_inst, producer=None) -> str | None:
-        if producer and producer != law.NO_STR:
-            return producer
-
-        return config_inst.x("default_producer", None)
-
-    @classmethod
     def get_producer_inst(cls, producer, kwargs=None):
         inst_dict = cls.get_producer_kwargs(**kwargs) if kwargs else None
         return Producer.get_cls(producer)(inst_dict=inst_dict)
 
     @classmethod
     def resolve_param_values(cls, params):
         params = super().resolve_param_values(params)
 
         # add the default producer when empty
-        if "config_inst" in params:
-            params["producer"] = cls.get_default_producer(params["config_inst"], params.get("producer"))
+        if config_inst := params.get("config_inst"):
+            params["producer"] = cls.resolve_config_default(
+                params,
+                params.get("producer"),
+                container=config_inst,
+                default_str="default_producer",
+                multiple=False,
+            )
             params["producer_inst"] = cls.get_producer_inst(params["producer"], params)
 
         return params
 
     @classmethod
     def get_known_shifts(cls, config_inst: od.Config, params: dict) -> tuple[set[str], set[str]]:
         shifts, upstream_shifts = super().get_known_shifts(config_inst, params)
 
         # get the producer, update it and add its shifts
-        producer_inst = params.get("producer_inst")
-        if producer_inst:
+        if producer_inst := params.get("producer_inst"):
             if cls.register_producer_shifts:
                 shifts |= producer_inst.all_shifts
             else:
                 upstream_shifts |= producer_inst.all_shifts
 
         return shifts, upstream_shifts
 
+    @classmethod
+    def req_params(cls, inst: law.Task, **kwargs) -> dict:
+        # prefer --producer set on task-level via cli
+        kwargs["_prefer_cli"] = law.util.make_set(kwargs.get("_prefer_cli", [])) | {"producer"}
+
+        return super().req_params(inst, **kwargs)
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # cache for producer inst
         self._producer_inst = None
 
     @property
@@ -367,64 +391,66 @@
         parts.insert_before("version", "producer", producer)
         return parts
 
 
 class ProducersMixin(ConfigTask):
 
     producers = law.CSVParameter(
-        default=(),
+        default=(RESOLVE_DEFAULT,),
         description="comma-separated names of producers to be applied; empty default",
         brace_expand=True,
     )
 
     # decibes whether the task itself runs the producers and implements their shifts
     register_producers_shifts = False
 
     @classmethod
-    def get_default_producers(cls, config_inst, producers=None) -> tuple[str]:
-        if producers and producers != law.NO_STR:
-            return producers
-
-        if config_inst.x("default_producer", None):
-            return (config_inst.x.default_producer,)
-
-        return ()
-
-    @classmethod
     def get_producer_insts(cls, producers, kwargs=None):
         inst_dict = cls.get_producer_kwargs(**kwargs) if kwargs else None
         return [
             Producer.get_cls(producer)(inst_dict=inst_dict)
             for producer in producers
         ]
 
     @classmethod
     def resolve_param_values(cls, params):
         params = super().resolve_param_values(params)
 
-        if "config_inst" in params:
-            params["producers"] = cls.get_default_producers(params["config_inst"], params.get("producers"))
+        if config_inst := params.get("config_inst"):
+            params["producers"] = cls.resolve_config_default_and_groups(
+                params,
+                params.get("producers"),
+                container=config_inst,
+                default_str="default_producer",
+                groups_str="producer_groups",
+            )
             params["producer_insts"] = cls.get_producer_insts(params["producers"], params)
 
         return params
 
     @classmethod
     def get_known_shifts(cls, config_inst: od.Config, params: dict) -> tuple[set[str], set[str]]:
         shifts, upstream_shifts = super().get_known_shifts(config_inst, params)
 
         # get the producers, update them and add their shifts
-        producer_insts = params.get("producer_insts")
-        for producer_inst in producer_insts or []:
+        for producer_inst in params.get("producer_insts") or []:
             if cls.register_producers_shifts:
                 shifts |= producer_inst.all_shifts
             else:
                 upstream_shifts |= producer_inst.all_shifts
 
         return shifts, upstream_shifts
 
+    @classmethod
+    def req_params(cls, inst: law.Task, **kwargs) -> dict:
+        # prefer --producers set on task-level via cli
+        kwargs["_prefer_cli"] = law.util.make_set(kwargs.get("_prefer_cli", [])) | {"producers"}
+
+        return super().req_params(inst, **kwargs)
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # cache for producer insts
         self._producer_insts = None
 
     @property
@@ -437,28 +463,35 @@
         parts = super().store_parts()
 
         part = "none"
         if self.producers:
             part = "__".join(self.producers[:5])
             if len(self.producers) > 5:
                 part += f"__{law.util.create_hash(self.producers[5:])}"
-        parts.insert_before("version", "producers", f"prod__{part}")
+        parts.insert_before("version", "producers", f"prod__{part or 'none'}")
 
         return parts
 
 
 class MLModelMixinBase(AnalysisTask):
 
     ml_model = luigi.Parameter(
         description="the name of the ML model to be applied",
     )
 
     exclude_params_repr_empty = {"ml_model"}
 
     @classmethod
+    def req_params(cls, inst: law.Task, **kwargs) -> dict:
+        # prefer --ml-model set on task-level via cli
+        kwargs["_prefer_cli"] = law.util.make_set(kwargs.get("_prefer_cli", [])) | {"ml_model"}
+
+        return super().req_params(inst, **kwargs)
+
+    @classmethod
     def get_ml_model_inst(
         cls,
         ml_model: str,
         analysis_inst: od.Analysis,
         requested_configs: list[str] | None = None,
         **kwargs,
     ) -> MLModel:
@@ -517,30 +550,33 @@
 
     @classmethod
     def resolve_calibrators(
         cls,
         ml_model_inst: MLModel,
         params: dict[str, Any],
     ) -> tuple[tuple[str]]:
-        calibrators = params.get("calibrators", ())
-
-        # use config defaults in case each config has one
-        if not calibrators:
-            defaults = tuple(
-                CalibratorsMixin.get_default_calibrators(config_inst)
-                for config_inst in ml_model_inst.config_insts
-            )
-            if all(defaults):
-                calibrators = defaults
+        calibrators = params.get("calibrators") or ((),)
 
         # broadcast to configs
         n_configs = len(ml_model_inst.config_insts)
         if len(calibrators) == 1 and n_configs != 1:
             calibrators = tuple(calibrators * n_configs)
 
+        # apply calibrators_groups and default_calibrator from the config
+        calibrators = tuple(
+            ConfigTask.resolve_config_default_and_groups(
+                params,
+                calibrators[i],
+                container=config_inst,
+                default_str="default_calibrator",
+                groups_str="calibrator_groups",
+            )
+            for i, config_inst in enumerate(ml_model_inst.config_insts)
+        )
+
         # validate number of sequences
         if len(calibrators) != n_configs:
             raise Exception(
                 f"MLModel '{ml_model_inst.cls_name}' uses {n_configs} configs but received "
                 f"{len(calibrators)} calibrator sequences",
             )
 
@@ -560,30 +596,33 @@
 
     @classmethod
     def resolve_selectors(
         cls,
         ml_model_inst: MLModel,
         params: dict[str, Any],
     ) -> tuple[str]:
-        selectors = params.get("selectors", ())
-
-        # use config defaults in case each config has one
-        if not selectors:
-            defaults = tuple(
-                SelectorMixin.get_default_selector(config_inst)
-                for config_inst in ml_model_inst.config_insts
-            )
-            if all(defaults):
-                selectors = defaults
+        selectors = params.get("selectors") or (None,)
 
         # broadcast to configs
         n_configs = len(ml_model_inst.config_insts)
         if len(selectors) == 1 and n_configs != 1:
             selectors = tuple(selectors * n_configs)
 
+        # use config defaults
+        selectors = tuple(
+            ConfigTask.resolve_config_default(
+                params,
+                selectors[i],
+                container=config_inst,
+                default_str="default_selector",
+                multiple=False,
+            )
+            for i, config_inst in enumerate(ml_model_inst.config_insts)
+        )
+
         # validate sequence length
         if len(selectors) != n_configs:
             raise Exception(
                 f"MLModel '{ml_model_inst.cls_name}' uses {n_configs} configs but received "
                 f"{len(selectors)} selectors",
             )
 
@@ -602,30 +641,33 @@
 
     @classmethod
     def resolve_producers(
         cls,
         ml_model_inst: MLModel,
         params: dict[str, Any],
     ) -> tuple[tuple[str]]:
-        producers = params.get("producers", ())
-
-        # use config defaults in case each config has one
-        if not producers:
-            defaults = tuple(
-                ProducersMixin.get_default_producers(config_inst)
-                for config_inst in ml_model_inst.config_insts
-            )
-            if all(defaults):
-                producers = defaults
+        producers = params.get("producers") or ((),)
 
         # broadcast to configs
         n_configs = len(ml_model_inst.config_insts)
         if len(producers) == 1 and n_configs != 1:
             producers = tuple(producers * n_configs)
 
+        # apply producers_groups and default_producer from the config
+        producers = tuple(
+            ConfigTask.resolve_config_default_and_groups(
+                params,
+                producers[i],
+                container=config_inst,
+                default_str="default_producer",
+                groups_str="producer_groups",
+            )
+            for i, config_inst in enumerate(ml_model_inst.config_insts)
+        )
+
         # validate number of sequences
         if len(producers) != n_configs:
             raise Exception(
                 f"MLModel '{ml_model_inst.cls_name}' uses {n_configs} configs but received "
                 f"{len(producers)} producer sequences",
             )
 
@@ -645,14 +687,16 @@
 
     @classmethod
     def resolve_param_values(cls, params: dict[str, Any]) -> dict[str, Any]:
         params = super().resolve_param_values(params)
 
         if "analysis_inst" in params and "ml_model" in params:
             analysis_inst = params["analysis_inst"]
+
+            # NOTE: we could try to implement resolving the default ml_model here
             ml_model_inst = cls.get_ml_model_inst(params["ml_model"], analysis_inst)
             params["ml_model_inst"] = ml_model_inst
 
             # resolve configs
             _configs = params.get("configs", ())
             params["configs"] = tuple(ml_model_inst.training_configs(list(_configs)))
             if not params["configs"]:
@@ -682,19 +726,59 @@
         # get the ML model instance
         self.ml_model_inst = self.get_ml_model_inst(
             self.ml_model,
             self.analysis_inst,
             configs=list(self.configs),
         )
 
+    def store_parts(self) -> law.util.InsertableDict:
+        parts = super().store_parts()
+        # since MLTraining is no CalibratorsMixin, SelectorMixin, ProducerMixin, ConfigTask,
+        # all these parts are missing in the `store_parts`
+
+        configs_repr = "__".join(self.configs[:5])
+
+        if len(self.configs) > 5:
+            configs_repr += f"_{law.util.create_hash(self.configs[5:])}"
+
+        parts.insert_after("task_family", "configs", configs_repr)
+
+        for label, fct_names in [
+            ("calib", self.calibrators),
+            ("sel", tuple((sel,) for sel in self.selectors)),
+            ("prod", self.producers),
+        ]:
+            if not fct_names or not any(fct_names):
+                fct_names = ["none"]
+            elif len(set(fct_names)) == 1:
+                # when functions are the same per config, only use them once
+                fct_names = fct_names[0]
+                n_fct_per_config = str(len(fct_names))
+            else:
+                # when functions differ between configs, flatten
+                n_fct_per_config = "".join(str(len(x)) for x in fct_names)
+                fct_names = tuple(fct_name for fct_names_cfg in fct_names for fct_name in fct_names_cfg)
+
+            part = "__".join(fct_names[:2])
+
+            if len(fct_names) > 2:
+                part += f"_{n_fct_per_config}_{law.util.create_hash(fct_names[2:])}"
+
+            parts.insert_before("version", label, f"{label}__{part}")
+
+        if self.ml_model_inst:
+            parts.insert_before("version", "ml_model", f"ml__{self.ml_model_inst.cls_name}")
+
+        return parts
+
 
 class MLModelMixin(ConfigTask, MLModelMixinBase):
 
     ml_model = luigi.Parameter(
-        default=law.NO_STR,
+        default=RESOLVE_DEFAULT,
         description="the name of the ML model to be applied; default: value of the "
         "'default_ml_model' config",
     )
 
     allow_empty_ml_model = True
 
     exclude_params_repr_empty = {"ml_model"}
@@ -703,19 +787,22 @@
     def resolve_param_values(cls, params: dict[str, Any]) -> dict[str, Any]:
         params = super().resolve_param_values(params)
 
         # add the default ml model when empty
         if "analysis_inst" in params and "config_inst" in params:
             analysis_inst = params["analysis_inst"]
             config_inst = params["config_inst"]
-            if (
-                params.get("ml_model") in (None, law.NO_STR) and
-                config_inst.x("default_ml_model", None)
-            ):
-                params["ml_model"] = config_inst.x.default_ml_model
+
+            params["ml_model"] = cls.resolve_config_default(
+                params,
+                params.get("ml_model"),
+                container=config_inst,
+                default_str="default_ml_model",
+                multiple=False,
+            )
 
             # initialize it once to trigger its set_config hook which might, in turn,
             # add objects to the config itself
             if params.get("ml_model") not in (None, law.NO_STR):
                 params["ml_model_inst"] = cls.get_ml_model_inst(
                     params["ml_model"],
                     analysis_inst,
@@ -759,32 +846,36 @@
 
         return parts
 
 
 class MLModelsMixin(ConfigTask):
 
     ml_models = law.CSVParameter(
-        default=(),
+        default=(RESOLVE_DEFAULT,),
         description="comma-separated names of ML models to be applied; empty default",
         brace_expand=True,
     )
 
     allow_empty_ml_models = True
 
     exclude_params_repr_empty = {"ml_models"}
 
     @classmethod
     def resolve_param_values(cls, params: dict[str, Any]) -> dict[str, Any]:
         params = super().resolve_param_values(params)
 
-        if "analysis_inst" in params and "config_inst" in params:
-            analysis_inst = params["analysis_inst"]
-            config_inst = params["config_inst"]
-            if not params.get("ml_models") and config_inst.x("default_ml_model", None):
-                params["ml_models"] = (config_inst.x.default_ml_model,)
+        if (analysis_inst := params.get("analysis_inst")) and (config_inst := params.get("config_inst")):
+            # apply ml_model_groups and default_ml_model from the config
+            params["ml_models"] = cls.resolve_config_default_and_groups(
+                params,
+                params.get("ml_models"),
+                container=config_inst,
+                default_str="default_ml_model",
+                groups_str="ml_model_groups",
+            )
 
             # special case: initialize them once to trigger their set_config hook
             if params.get("ml_models"):
                 params["ml_model_insts"] = [
                     MLModelMixinBase.get_ml_model_inst(
                         ml_model,
                         analysis_inst,
@@ -793,14 +884,21 @@
                     for ml_model in params["ml_models"]
                 ]
             elif not cls.allow_empty_ml_models:
                 raise Exception(f"no ml_models configured for {cls.task_family}")
 
         return params
 
+    @classmethod
+    def req_params(cls, inst: law.Task, **kwargs) -> dict:
+        # prefer --ml-models set on task-level via cli
+        kwargs["_prefer_cli"] = law.util.make_set(kwargs.get("_prefer_cli", [])) | {"ml_models"}
+
+        return super().req_params(inst, **kwargs)
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # get the ML model instances
         self.ml_model_insts = [
             MLModelMixinBase.get_ml_model_inst(
                 ml_model,
@@ -808,44 +906,57 @@
                 requested_configs=[self.config_inst],
             )
             for ml_model in self.ml_models
         ]
 
     def store_parts(self) -> law.util.InsertableDict:
         parts = super().store_parts()
+
         if self.ml_model_insts:
             part = "__".join(self.ml_models)
             parts.insert_before("version", "ml_models", f"ml__{part}")
+
         return parts
 
 
 class InferenceModelMixin(ConfigTask):
 
     inference_model = luigi.Parameter(
-        default=law.NO_STR,
+        default=RESOLVE_DEFAULT,
         description="the name of the inference model to be used; default: value of the "
         "'default_inference_model' config",
     )
 
     @classmethod
     def resolve_param_values(cls, params: dict[str, Any]) -> dict[str, Any]:
         params = super().resolve_param_values(params)
 
         # add the default inference model when empty
-        if "config_inst" in params:
-            config_inst = params["config_inst"]
-            if params.get("inference_model") in (None, law.NO_STR) and config_inst.x("default_inference_model", None):
-                params["inference_model"] = config_inst.x.default_inference_model
+        if config_inst := params.get("config_inst"):
+            params["inference_model"] = cls.resolve_config_default(
+                params,
+                params.get("inference_model"),
+                container=config_inst,
+                default_str="default_inference_model",
+                multiple=False,
+            )
 
         return params
 
     @classmethod
     def get_inference_model_inst(cls, inference_model: str, config_inst: od.Config) -> InferenceModel:
         return InferenceModel.get_cls(inference_model)(config_inst)
 
+    @classmethod
+    def req_params(cls, inst: law.Task, **kwargs) -> dict:
+        # prefer --inference-model set on task-level via cli
+        kwargs["_prefer_cli"] = law.util.make_set(kwargs.get("_prefer_cli", [])) | {"inference_model"}
+
+        return super().req_params(inst, **kwargs)
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # get the inference model instance
         self.inference_model_inst = self.get_inference_model_inst(self.inference_model, self.config_inst)
 
     def store_parts(self) -> law.util.InsertableDict:
@@ -1257,14 +1368,22 @@
 
         # eager, overly cautious gc
         del handler
         gc.collect()
 
     @classmethod
     def raise_if_not_finite(cls, ak_array: ak.Array) -> None:
+        """
+        Perform explicit check whether all values in array *ak_array* are finite.
+
+        The check is performed using the :external+numpy:py:func:`numpy.isfinite` function
+
+        :param ak_array: Array with events to check.
+        :raises ValueError: If any value in *ak_array* is not finite.
+        """
         import numpy as np
         import awkward as ak
         from columnflow.columnar_util import get_ak_routes
 
         for route in get_ak_routes(ak_array):
             if ak.any(~np.isfinite(ak.flatten(route.apply(ak_array), axis=None))):
                 raise ValueError(
```

### Comparing `columnflow-0.2.1/columnflow/tasks/framework/parameters.py` & `columnflow-0.2.2/columnflow/tasks/framework/parameters.py`

 * *Files identical despite different names*

### Comparing `columnflow-0.2.1/columnflow/tasks/framework/plotting.py` & `columnflow-0.2.2/columnflow/tasks/framework/plotting.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,20 +48,20 @@
         "'option1=val1,option2=val2,...'",
     )
     skip_legend = law.OptionalBoolParameter(
         default=None,
         significant=False,
         description="when True, no legend is drawn; default: None",
     )
-    cms_label = luigi.ChoiceParameter(
-        choices=("wip", "pre", "pw", "sim", "simwip", "simpre", "simpw", "public", "skip"),
+    cms_label = luigi.Parameter(
         default="wip",
         significant=False,
-        description="Parameter to set the type of CMS logo; choices: "
-        "wip,pre,pw,sim,simwip,simpre,simpw,public,skip; default: wip",
+        description="postfix to add behind the CMS logo; when 'skip', no CMS logo is shown at all; "
+        "the following special values are expanded into the usual postfixes: wip, pre, pw, sim, "
+        "simwip, simpre, simpw, od, odwip, public; default: 'wip'",
     )
 
     @classmethod
     def resolve_param_values(cls, params):
         params = super().resolve_param_values(params)
 
         if "config_inst" not in params:
@@ -223,19 +223,66 @@
     )
     shape_norm = law.OptionalBoolParameter(
         default=None,
         significant=False,
         description="when True, the overall bin content is normalized on its integral; "
         "default: None",
     )
+    colormap = luigi.Parameter(
+        default=law.NO_STR,
+        significant=False,
+        description="name of the matplotlib colormap to use for the colorbar; "
+        "if not set, an appropriate colormap will be chosen by the plotting function",
+    )
+    zlim = law.CSVParameter(
+        default=("min", "max"),
+        significant=False,
+        min_len=2,
+        max_len=2,
+        description="the range of values covered by the colorbar; this optional CSV parameter "
+        "accepts exactly two values, indicating the lower and upper bound of the colorbar. The special "
+        "specifiers 'min' and 'max' can be used in place of floats to indicate the minimum or maximum value "
+        "of the data. Similarly, 'maxabs' and 'minabs' indicate the minimum and maximum of the absolute "
+        "value of the data. A hyphen ('-') may be prepended to any specifier to indicate the negative of the "
+        "corresponding value. If no 'zlim' is given, the limits are inferred from the data (equivalent to 'min,max').",
+    )
+    extremes = luigi.ChoiceParameter(
+        default="color",
+        choices=("color", "clip", "hide"),
+        significant=False,
+        description="how to handle extreme values outside `zlim`; valid choices are: 'color' (extreme values are "
+        "shown in a different color), 'clip' (extreme values are clipped to the closest allowed values) and 'hide' "
+        "(extreme values are treated as missing); default: 'color'",
+    )
+    extreme_colors = law.CSVParameter(
+        default=(),
+        significant=False,
+        description="the colors to use for marking extreme values; this optional CSV parameter accepts exactly two "
+        "values, indicating the color to use for values below and above the range covered by the colorbar.",
+    )
+
+    @classmethod
+    def modify_param_values(cls, params: dict) -> dict:
+        params = super().modify_param_values(params)
+
+        params["zlim"] = tuple(
+            float(v) if law.util.is_float(v) else v
+            for v in params["zlim"]
+        )
+
+        return params
 
     def get_plot_parameters(self) -> DotDict:
         # convert parameters to usable values during plotting
         params = super().get_plot_parameters()
         dict_add_strict(params, "zscale", None if self.zscale == law.NO_STR else self.zscale)
+        dict_add_strict(params, "zlim", None if not self.zlim else self.zlim)
+        dict_add_strict(params, "extremes", self.extremes)
+        dict_add_strict(params, "extreme_colors", None if not self.extreme_colors else self.extreme_colors)
+        dict_add_strict(params, "colormap", None if self.colormap == law.NO_STR else self.colormap)
         dict_add_strict(params, "density", self.density)
         dict_add_strict(params, "shape_norm", self.shape_norm)
         return params
 
 
 class ProcessPlotSettingMixin(
     DatasetsProcessesMixin,
```

### Comparing `columnflow-0.2.1/columnflow/tasks/framework/remote.py` & `columnflow-0.2.2/columnflow/tasks/framework/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,15 +328,14 @@
     htcondor_forward_env_variables = {
         "CF_BASE": "cf_base",
         "CF_REPO_BASE": "cf_repo_base",
         "CF_CERN_USER": "cf_cern_user",
         "CF_STORE_NAME": "cf_store_name",
         "CF_STORE_LOCAL": "cf_store_local",
         "CF_LOCAL_SCHEDULER": "cf_local_scheduler",
-        "CF_VOMS": "cf_voms",
     }
 
     # upstream requirements
     reqs = Requirements(
         BundleRepo=BundleRepo,
         BundleSoftware=BundleSoftware,
         BuildBashSandbox=BuildBashSandbox,
```

### Comparing `columnflow-0.2.1/columnflow/tasks/histograms.py` & `columnflow-0.2.2/columnflow/tasks/histograms.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,36 +27,40 @@
     CalibratorsMixin,
     EventWeightMixin,
     ChunkedIOMixin,
     MergeReducedEventsUser,
     law.LocalWorkflow,
     RemoteWorkflow,
 ):
-    sandbox = dev_sandbox("bash::$CF_BASE/sandboxes/venv_columnar.sh")
+    sandbox = dev_sandbox(law.config.get("analysis", "default_columnar_sandbox"))
 
     # upstream requirements
     reqs = Requirements(
         MergeReducedEventsUser.reqs,
         RemoteWorkflow.reqs,
         MergeReducedEvents=MergeReducedEvents,
         ProduceColumns=ProduceColumns,
         MLEvaluation=MLEvaluation,
     )
 
+    # strategy for handling missing source columns when adding aliases on event chunks
+    missing_column_alias_strategy = "original"
+
     def workflow_requires(self):
         reqs = super().workflow_requires()
 
         # require the full merge forest
         reqs["events"] = self.reqs.MergeReducedEvents.req(self, tree_index=-1)
 
         if not self.pilot:
             if self.producers:
                 reqs["producers"] = [
-                    self.reqs.ProduceColumns.req(self, producer=p)
-                    for p in self.producers
+                    self.reqs.ProduceColumns.req(self, producer=producer_inst.cls_name)
+                    for producer_inst in self.producer_insts
+                    if producer_inst.produced_columns
                 ]
             if self.ml_models:
                 reqs["ml"] = [
                     self.reqs.MLEvaluation.req(self, ml_model=m)
                     for m in self.ml_models
                 ]
 
@@ -65,16 +69,17 @@
     def requires(self):
         reqs = {
             "events": self.reqs.MergeReducedEvents.req(self, tree_index=self.branch, _exclude={"branch"}),
         }
 
         if self.producers:
             reqs["producers"] = [
-                self.reqs.ProduceColumns.req(self, producer=p)
-                for p in self.producers
+                self.reqs.ProduceColumns.req(self, producer=producer_inst.cls_name)
+                for producer_inst in self.producer_insts
+                if producer_inst.produced_columns
             ]
         if self.ml_models:
             reqs["ml"] = [
                 self.reqs.MLEvaluation.req(self, ml_model=m)
                 for m in self.ml_models
             ]
 
@@ -107,21 +112,25 @@
 
         # get shift dependent aliases
         aliases = self.local_shift_inst.x("column_aliases", {})
 
         # define columns that need to be read
         read_columns = {"category_ids", "process_id"} | set(aliases.values())
         read_columns |= {
-            Route(variable_inst.expression)
-            if isinstance(variable_inst.expression, str) else
-            None  # TODO: handle variable_inst with custom expressions, can they declare columns?
+            Route(inp)
             for variable_inst in (
                 self.config_inst.get_variable(var_name)
                 for var_name in law.util.flatten(self.variable_tuples.values())
             )
+            for inp in (
+                [variable_inst.expression]
+                if isinstance(variable_inst.expression, str)
+                # for variable_inst with custom expressions, read columns declared via aux key
+                else variable_inst.x("inputs", [])
+            )
         }
         if self.dataset_inst.is_mc:
             read_columns |= {Route(column) for column in self.config_inst.x.event_weights}
             read_columns |= {Route(column) for column in self.dataset_inst.x("event_weights", [])}
         read_columns = {Route(c) for c in read_columns}
 
         # empty float array to use when input files have no entries
@@ -138,15 +147,20 @@
             source_type=len(files) * ["awkward_parquet"],
             read_columns=len(files) * [read_columns],
         ):
             # add additional columns
             events = update_ak_array(events, *columns)
 
             # add aliases
-            events = add_ak_aliases(events, aliases, remove_src=True)
+            events = add_ak_aliases(
+                events,
+                aliases,
+                remove_src=True,
+                missing_strategy=self.missing_column_alias_strategy,
+            )
 
             # build the full event weight
             weight = ak.Array(np.ones(len(events)))
             if self.dataset_inst.is_mc and len(events):
                 for column in self.config_inst.x.event_weights:
                     weight = weight * Route(column).apply(events)
                 for column in self.dataset_inst.x("event_weights", []):
@@ -181,31 +195,32 @@
                     # enable weights and store it
                     histograms[var_key] = h.Weight()
 
                 # broadcast arrays so that each event can be filled for all its categories
                 fill_kwargs = {
                     "category": events.category_ids,
                     "process": events.process_id,
-                    "shift": self.global_shift_inst.id,
+                    "shift": np.ones(len(events), dtype=np.int32) * self.global_shift_inst.id,
                     "weight": weight,
                 }
                 for variable_inst in variable_insts:
                     # prepare the expression
                     expr = variable_inst.expression
                     if isinstance(expr, str):
                         route = Route(expr)
                         def expr(events, *args, **kwargs):
                             if len(events) == 0 and not has_ak_column(events, route):
                                 return empty_f32
                             return route.apply(events, null_value=variable_inst.null_value)
                     # apply it
                     fill_kwargs[variable_inst.name] = expr(events)
+
                 # broadcast and fill
-                arrays = (ak.flatten(a) for a in ak.broadcast_arrays(*fill_kwargs.values()))
-                histograms[var_key].fill(**dict(zip(fill_kwargs, arrays)))
+                arrays = ak.flatten(ak.cartesian(fill_kwargs))
+                histograms[var_key].fill(**{field: arrays[field] for field in arrays.fields})
 
         # merge output files
         self.output()["hists"].dump(histograms, formatter="pickle")
 
 
 CreateHistogramsWrapper = wrapper_factory(
     base_cls=AnalysisTask,
@@ -231,15 +246,15 @@
     )
     remove_previous = luigi.BoolParameter(
         default=False,
         significant=False,
         description="when True, remove particlar input histograms after merging; default: False",
     )
 
-    sandbox = dev_sandbox("bash::$CF_BASE/sandboxes/venv_columnar.sh")
+    sandbox = dev_sandbox(law.config.get("analysis", "default_columnar_sandbox"))
 
     # upstream requirements
     reqs = Requirements(
         RemoteWorkflow.reqs,
         CreateHistograms=CreateHistograms,
     )
 
@@ -319,15 +334,15 @@
     ProducersMixin,
     SelectorStepsMixin,
     CalibratorsMixin,
     DatasetTask,
     law.LocalWorkflow,
     RemoteWorkflow,
 ):
-    sandbox = dev_sandbox("bash::$CF_BASE/sandboxes/venv_columnar.sh")
+    sandbox = dev_sandbox(law.config.get("analysis", "default_columnar_sandbox"))
 
     # disable the shift parameter
     shift = None
     effective_shift = None
     allow_empty_shift = True
 
     # allow only running on nominal
```

### Comparing `columnflow-0.2.1/columnflow/tasks/ml.py` & `columnflow-0.2.2/columnflow/tasks/ml.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,26 +29,29 @@
     SelectorMixin,
     CalibratorsMixin,
     ChunkedIOMixin,
     MergeReducedEventsUser,
     law.LocalWorkflow,
     RemoteWorkflow,
 ):
-    sandbox = dev_sandbox("bash::$CF_BASE/sandboxes/venv_columnar.sh")
+    sandbox = dev_sandbox(law.config.get("analysis", "default_columnar_sandbox"))
 
     allow_empty_ml_model = False
 
     # upstream requirements
     reqs = Requirements(
         MergeReducedEventsUser.reqs,
         RemoteWorkflow.reqs,
         MergeReducedEvents=MergeReducedEvents,
         ProduceColumns=ProduceColumns,
     )
 
+    # strategy for handling missing source columns when adding aliases on event chunks
+    missing_column_alias_strategy = "original"
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # complain when this task is run for events that are not needed for training
         if not self.events_used_in_training(
             self.config_inst,
             self.dataset_inst,
@@ -65,27 +68,33 @@
         reqs = super().workflow_requires()
 
         # require the full merge forest
         reqs["events"] = self.reqs.MergeReducedEvents.req(self, tree_index=-1)
 
         if not self.pilot and self.producers:
             reqs["producers"] = [
-                self.reqs.ProduceColumns.req(self, producer=p)
-                for p in self.producers
+                self.reqs.ProduceColumns.req(self, producer=producer_inst.cls_name)
+                for producer_inst in self.producer_insts
+                if producer_inst.produced_columns
             ]
 
         return reqs
 
     def requires(self):
-        reqs = {"events": self.reqs.MergeReducedEvents.req(self, tree_index=self.branch, _exclude={"branch"})}
+        reqs = {
+            "events": self.reqs.MergeReducedEvents.req(self, tree_index=self.branch, _exclude={"branch"}),
+        }
+
         if self.producers:
             reqs["producers"] = [
-                self.reqs.ProduceColumns.req(self, producer=p)
-                for p in self.producers
+                self.reqs.ProduceColumns.req(self, producer=producer_inst.cls_name)
+                for producer_inst in self.producer_insts
+                if producer_inst.produced_columns
             ]
+
         return reqs
 
     @MergeReducedEventsUser.maybe_dummy
     def output(self):
         k = self.ml_model_inst.folds
         return {"mlevents": law.SiblingFileCollection([
             self.target(f"mlevents_fold{f}of{k}_{self.branch}.parquet")
@@ -135,15 +144,20 @@
         ):
             n_events += len(events)
 
             # add additional columns
             events = update_ak_array(events, *columns)
 
             # add aliases
-            events = add_ak_aliases(events, aliases, remove_src=True)
+            events = add_ak_aliases(
+                events,
+                aliases,
+                remove_src=True,
+                missing_strategy=self.missing_column_alias_strategy,
+            )
 
             # generate fold indices
             fold_indices = events.deterministic_seed % self.ml_model_inst.folds
 
             # remove columns
             events = route_filter(events)
 
@@ -193,15 +207,15 @@
     ProducersMixin,
     SelectorMixin,
     CalibratorsMixin,
     DatasetTask,
     law.tasks.ForestMerge,
     RemoteWorkflow,
 ):
-    sandbox = dev_sandbox("bash::$CF_BASE/sandboxes/venv_columnar.sh")
+    sandbox = dev_sandbox(law.config.get("analysis", "default_columnar_sandbox"))
 
     fold = luigi.IntParameter(
         default=0,
         description="the fold index of the prepared ML events to use; must be compatible with the "
         "number of folds defined in the ML model; default: 0",
     )
 
@@ -260,14 +274,17 @@
         return {"mlevents": self.target(f"mlevents_f{self.fold}of{k}.parquet")}
 
     @law.decorator.log
     def run(self):
         return super().run()
 
     def merge(self, inputs, output):
+        if not self.is_leaf():
+            inputs = [inp["mlevents"] for inp in inputs]
+
         law.pyarrow.merge_parquet_task(self, inputs, output["mlevents"])
 
 
 MergeMLEventsWrapper = wrapper_factory(
     base_cls=AnalysisTask,
     require_cls=MergeMLEvents,
     enable=["configs", "skip_configs", "datasets", "skip_datasets"],
@@ -395,14 +412,17 @@
     law.LocalWorkflow,
     RemoteWorkflow,
 ):
     sandbox = None
 
     allow_empty_ml_model = False
 
+    # strategy for handling missing source columns when adding aliases on event chunks
+    missing_column_alias_strategy = "original"
+
     # upstream requirements
     reqs = Requirements(
         MergeReducedEventsUser.reqs,
         RemoteWorkflow.reqs,
         MLTraining=MLTraining,
         MergeReducedEvents=MergeReducedEvents,
         ProduceColumns=ProduceColumns,
@@ -425,16 +445,17 @@
             producers=(self.producers,),
         )
 
         reqs["events"] = self.reqs.MergeReducedEvents.req_different_branching(self)
 
         if not self.pilot and self.producers:
             reqs["producers"] = [
-                self.reqs.ProduceColumns.req(self, producer=p)
-                for p in self.producers
+                self.reqs.ProduceColumns.req(self, producer=producer_inst.cls_name)
+                for producer_inst in self.producer_insts
+                if producer_inst.produced_columns
             ]
 
         return reqs
 
     def requires(self):
         reqs = {
             "models": self.reqs.MLTraining.req_different_branching(
@@ -450,23 +471,24 @@
                 tree_index=self.branch,
                 branch=-1,
             ),
         }
 
         if self.producers:
             reqs["producers"] = [
-                self.reqs.ProduceColumns.req(self, producer=p)
-                for p in self.producers
+                self.reqs.ProduceColumns.req(self, producer=producer_inst.cls_name)
+                for producer_inst in self.producer_insts
+                if producer_inst.produced_columns
             ]
 
         return reqs
 
     @MergeReducedEventsUser.maybe_dummy
     def output(self):
-        return {"mlcolumns": self.target(f"mlcolumns_{self.branch}.pickle")}
+        return {"mlcolumns": self.target(f"mlcolumns_{self.branch}.parquet")}
 
     @law.decorator.log
     @law.decorator.localize
     @law.decorator.safe_output
     def run(self):
         from columnflow.columnar_util import (
             Route, RouteFilter, sorted_ak_to_parquet, update_ak_array, add_ak_aliases,
@@ -515,15 +537,20 @@
             source_type=len(files) * ["awkward_parquet"],
             read_columns=len(files) * [read_columns],
         ):
             # add additional columns
             events = update_ak_array(events, *columns)
 
             # add aliases
-            events = add_ak_aliases(events, aliases, remove_src=True)
+            events = add_ak_aliases(
+                events,
+                aliases,
+                remove_src=True,
+                missing_strategy=self.missing_column_alias_strategy,
+            )
 
             # asdasd
             fold_indices = events.deterministic_seed % self.ml_model_inst.folds
 
             # evaluate the model
             events = self.ml_model_inst.evaluate(
                 self,
```

### Comparing `columnflow-0.2.1/columnflow/tasks/plotting.py` & `columnflow-0.2.2/columnflow/tasks/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     MLModelsMixin,
     ProducersMixin,
     SelectorStepsMixin,
     CalibratorsMixin,
     law.LocalWorkflow,
     RemoteWorkflow,
 ):
-    sandbox = dev_sandbox("bash::$CF_BASE/sandboxes/venv_columnar.sh")
+    sandbox = dev_sandbox(law.config.get("analysis", "default_columnar_sandbox"))
 
     exclude_index = True
 
     # upstream requirements
     reqs = Requirements(
         RemoteWorkflow.reqs,
         MergeHistograms=MergeHistograms,
```

### Comparing `columnflow-0.2.1/columnflow/tasks/production.py` & `columnflow-0.2.2/columnflow/tasks/production.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,25 +21,29 @@
     CalibratorsMixin,
     ChunkedIOMixin,
     MergeReducedEventsUser,
     law.LocalWorkflow,
     RemoteWorkflow,
 ):
     # default sandbox, might be overwritten by producer function
-    sandbox = dev_sandbox("bash::$CF_BASE/sandboxes/venv_columnar.sh")
+    sandbox = dev_sandbox(law.config.get("analysis", "default_columnar_sandbox"))
 
     # upstream requirements
     reqs = Requirements(
         MergeReducedEventsUser.reqs,
         RemoteWorkflow.reqs,
         MergeReducedEvents=MergeReducedEvents,
     )
 
+    # register shifts found in the chosen producer to this task
     register_producer_shifts = True
 
+    # strategy for handling missing source columns when adding aliases on event chunks
+    missing_column_alias_strategy = "original"
+
     def workflow_requires(self):
         reqs = super().workflow_requires()
 
         # require the full merge forest
         reqs["events"] = self.reqs.MergeReducedEvents.req(self, tree_index=-1)
 
         # add producer dependent requirements
@@ -51,32 +55,39 @@
         return {
             "events": self.reqs.MergeReducedEvents.req(self, tree_index=self.branch, _exclude={"branch"}),
             "producer": self.producer_inst.run_requires(),
         }
 
     @MergeReducedEventsUser.maybe_dummy
     def output(self):
-        return {"columns": self.target(f"columns_{self.branch}.parquet")}
+        outputs = {}
+
+        # only declare the output in case the producer actually creates columns
+        if self.producer_inst.produced_columns:
+            outputs["columns"] = self.target(f"columns_{self.branch}.parquet")
+
+        return outputs
 
     @law.decorator.log
-    @law.decorator.localize
+    @law.decorator.localize(input=False)
     @law.decorator.safe_output
     def run(self):
         from columnflow.columnar_util import (
-            Route, RouteFilter, mandatory_coffea_columns, add_ak_aliases, sorted_ak_to_parquet,
+            Route, RouteFilter, mandatory_coffea_columns, update_ak_array, add_ak_aliases,
+            sorted_ak_to_parquet,
         )
 
         # prepare inputs and outputs
         reqs = self.requires()
         inputs = self.input()
         output = self.output()
         output_chunks = {}
 
         # run the producer setup
-        self.producer_inst.run_setup(reqs["producer"], inputs["producer"])
+        reader_targets = self.producer_inst.run_setup(reqs["producer"], inputs["producer"])
 
         # create a temp dir for saving intermediate files
         tmp_dir = law.LocalDirectoryTarget(is_tmp=True)
         tmp_dir.touch()
 
         # get shift dependent aliases
         aliases = self.local_shift_inst.x("column_aliases", {})
@@ -85,38 +96,51 @@
         read_columns = mandatory_coffea_columns | self.producer_inst.used_columns | set(aliases.values())
         read_columns = {Route(c) for c in read_columns}
 
         # define columns that will be written
         write_columns = self.producer_inst.produced_columns
         route_filter = RouteFilter(write_columns)
 
-        # iterate over chunks of events and diffs
-        for events, pos in self.iter_chunked_io(
-            inputs["events"]["collection"][0]["events"].path,
-            source_type="awkward_parquet",
-            read_columns=read_columns,
-        ):
-            # add aliases
-            events = add_ak_aliases(events, aliases, remove_src=True)
-
-            # invoke the producer
-            if len(events):
-                events = self.producer_inst(events)
-
-            # remove columns
-            events = route_filter(events)
-
-            # optional check for finite values
-            if self.check_finite:
-                self.raise_if_not_finite(events)
-
-            # save as parquet via a thread in the same pool
-            chunk = tmp_dir.child(f"file_{pos.index}.parquet", type="f")
-            output_chunks[pos.index] = chunk
-            self.chunked_io.queue(sorted_ak_to_parquet, (events, chunk.path))
+        # prepare inputs for localization
+        with law.localize_file_targets(
+            [inputs["events"]["collection"][0]["events"], *reader_targets.values()],
+            mode="r",
+        ) as inps:
+            # iterate over chunks of events and diffs
+            for (events, *cols), pos in self.iter_chunked_io(
+                [inp.path for inp in inps],
+                source_type=["awkward_parquet"] + [None] * len(reader_targets),
+                read_columns=[read_columns] * (len(reader_targets) + 1),
+            ):
+                # apply the optional columns from custom requirements
+                events = update_ak_array(events, *cols)
+
+                # add aliases
+                events = add_ak_aliases(
+                    events,
+                    aliases,
+                    remove_src=True,
+                    missing_strategy=self.missing_column_alias_strategy,
+                )
+
+                # invoke the producer
+                if len(events):
+                    events = self.producer_inst(events)
+
+                # remove columns
+                events = route_filter(events)
+
+                # optional check for finite values
+                if self.check_finite:
+                    self.raise_if_not_finite(events)
+
+                # save as parquet via a thread in the same pool
+                chunk = tmp_dir.child(f"file_{pos.index}.parquet", type="f")
+                output_chunks[pos.index] = chunk
+                self.chunked_io.queue(sorted_ak_to_parquet, (events, chunk.path))
 
         # merge output files
         sorted_chunks = [output_chunks[key] for key in sorted(output_chunks)]
         law.pyarrow.merge_parquet_task(self, sorted_chunks, output["columns"], local=True)
 
 
 # overwrite class defaults
```

### Comparing `columnflow-0.2.1/columnflow/tasks/reduction.py` & `columnflow-0.2.2/columnflow/tasks/reduction.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,63 +28,69 @@
     SelectorStepsMixin,
     CalibratorsMixin,
     ChunkedIOMixin,
     DatasetTask,
     law.LocalWorkflow,
     RemoteWorkflow,
 ):
-    sandbox = dev_sandbox("bash::$CF_BASE/sandboxes/venv_columnar.sh")
+    sandbox = dev_sandbox(law.config.get("analysis", "default_columnar_sandbox"))
 
     # upstream requirements
     reqs = Requirements(
         RemoteWorkflow.reqs,
         GetDatasetLFNs=GetDatasetLFNs,
         CalibrateEvents=CalibrateEvents,
         SelectEvents=SelectEvents,
     )
 
+    # strategy for handling missing source columns when adding aliases on event chunks
+    missing_column_alias_strategy = "original"
+
     def workflow_requires(self):
         reqs = super().workflow_requires()
 
         reqs["lfns"] = self.reqs.GetDatasetLFNs.req(self)
 
         if not self.pilot:
             reqs["calibrations"] = [
-                self.reqs.CalibrateEvents.req(self, calibrator=c)
-                for c in self.calibrators
+                self.reqs.CalibrateEvents.req(self, calibrator=calibrator_inst.cls_name)
+                for calibrator_inst in self.calibrator_insts
+                if calibrator_inst.produced_columns
             ]
             reqs["selection"] = self.reqs.SelectEvents.req(self)
         else:
             # pass-through pilot workflow requirements of upstream task
             t = self.reqs.SelectEvents.req(self)
             reqs = law.util.merge_dicts(reqs, t.workflow_requires(), inplace=True)
 
         return reqs
 
     def requires(self):
         return {
             "lfns": self.reqs.GetDatasetLFNs.req(self),
             "calibrations": [
-                self.reqs.CalibrateEvents.req(self, calibrator=c)
-                for c in self.calibrators
+                self.reqs.CalibrateEvents.req(self, calibrator=calibrator_inst.cls_name)
+                for calibrator_inst in self.calibrator_insts
+                if calibrator_inst.produced_columns
             ],
             "selection": self.reqs.SelectEvents.req(self),
         }
 
     def output(self):
         return {"events": self.target(f"events_{self.branch}.parquet")}
 
     @ensure_proxy
     @law.decorator.localize
     @law.decorator.safe_output
     def run(self):
         from columnflow.columnar_util import (
             Route, RouteFilter, mandatory_coffea_columns, update_ak_array, add_ak_aliases,
-            sorted_ak_to_parquet, set_ak_column,
+            sorted_ak_to_parquet,
         )
+        from columnflow.selection.util import create_collections_from_masks
 
         # prepare inputs and outputs
         inputs = self.input()
         lfn_task = self.requires()["lfns"]
         output = self.output()
         output_chunks = {}
 
@@ -160,15 +166,20 @@
             source_type=["coffea_root"] + (len(input_paths) - 1) * ["awkward_parquet"],
             read_columns=[read_columns, read_sel_columns] + (len(input_paths) - 2) * [read_columns],
         ):
             # add the calibrated diffs and potentially new columns
             events = update_ak_array(events, *diffs)
 
             # add aliases
-            events = add_ak_aliases(events, aliases, remove_src=True)
+            events = add_ak_aliases(
+                events,
+                aliases,
+                remove_src=True,
+                missing_steps=self.missing_column_alias_strategy,
+            )
 
             # build the event mask
             if self.selector_steps:
                 # check if all steps are present
                 missing_steps = set(self.selector_steps) - set(sel.steps.fields)
                 if missing_steps:
                     raise Exception(
@@ -186,26 +197,16 @@
             n_all += len(events)
             events = events[event_mask]
             n_reduced += len(events)
 
             # loop through all object selection, go through their masks
             # and create new collections if required
             if "objects" in sel.fields:
-                for src_name in sel.objects.fields:
-                    # get all destination collections, handling those named identically to the
-                    # source collection last
-                    dst_names = list(sel["objects", src_name].fields)
-                    if src_name in dst_names:
-                        # move to the end
-                        dst_names.remove(src_name)
-                        dst_names.append(src_name)
-                    for dst_name in dst_names:
-                        object_mask = sel.objects[src_name, dst_name][event_mask]
-                        dst_collection = events[src_name][object_mask]
-                        events = set_ak_column(events, dst_name, dst_collection)
+                # apply the event mask
+                events = create_collections_from_masks(events, sel.objects[event_mask])
 
             # remove columns
             events = route_filter(events)
 
             # save as parquet via a thread in the same pool
             chunk = tmp_dir.child(f"file_{pos.index}.parquet", type="f")
             output_chunks[pos.index] = chunk
@@ -394,15 +395,15 @@
 class MergeReducedEvents(
     SelectorStepsMixin,
     CalibratorsMixin,
     MergeReducedEventsUser,
     law.tasks.ForestMerge,
     RemoteWorkflow,
 ):
-    sandbox = dev_sandbox("bash::$CF_BASE/sandboxes/venv_columnar.sh")
+    sandbox = dev_sandbox(law.config.get("analysis", "default_columnar_sandbox"))
 
     # upstream requirements
     reqs = Requirements(
         MergeReducedEventsUser.reqs,
         RemoteWorkflow.reqs,
         ReduceEvents=ReduceEvents,
     )
@@ -435,17 +436,15 @@
             ),
         }
 
     def trace_merge_workflow_inputs(self, inputs):
         return super().trace_merge_workflow_inputs(inputs["events"])
 
     def trace_merge_inputs(self, inputs):
-        return super().trace_merge_inputs([
-            inp["events"] for inp in inputs["events"]["collection"].targets.values()
-        ])
+        return super().trace_merge_inputs(inputs["events"]["collection"].targets.values())
 
     def reduced_dummy_output(self):
         # mark the dummy output as a placeholder for the ForestMerge task
         dummy = super().reduced_dummy_output()
         self._mark_merge_output_placeholder(dummy)
         return dummy
 
@@ -455,14 +454,15 @@
         n_merged = len(DatasetTask.create_branch_map(self))
         return law.SiblingFileCollection([
             {"events": self.target(f"events_{i}.parquet")}
             for i in range(n_merged)
         ])
 
     def merge(self, inputs, output):
+        inputs = [inp["events"] for inp in inputs]
         law.pyarrow.merge_parquet_task(self, inputs, output["events"])
 
 
 MergeReducedEventsWrapper = wrapper_factory(
     base_cls=AnalysisTask,
     require_cls=MergeReducedEvents,
     enable=["configs", "skip_configs", "datasets", "skip_datasets", "shifts", "skip_shifts"],
```

### Comparing `columnflow-0.2.1/columnflow/tasks/selection.py` & `columnflow-0.2.2/columnflow/tasks/selection.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,34 +26,39 @@
     CalibratorsMixin,
     ChunkedIOMixin,
     DatasetTask,
     law.LocalWorkflow,
     RemoteWorkflow,
 ):
     # default sandbox, might be overwritten by selector function
-    sandbox = dev_sandbox("bash::$CF_BASE/sandboxes/venv_columnar.sh")
+    sandbox = dev_sandbox(law.config.get("analysis", "default_columnar_sandbox"))
 
     # upstream requirements
     reqs = Requirements(
         RemoteWorkflow.reqs,
         GetDatasetLFNs=GetDatasetLFNs,
         CalibrateEvents=CalibrateEvents,
     )
 
+    # register shifts found in the chosen selector to this task
     register_selector_shifts = True
 
+    # strategy for handling missing source columns when adding aliases on event chunks
+    missing_column_alias_strategy = "original"
+
     def workflow_requires(self):
         reqs = super().workflow_requires()
 
         reqs["lfns"] = self.reqs.GetDatasetLFNs.req(self)
 
         if not self.pilot:
             reqs["calib"] = [
-                self.reqs.CalibrateEvents.req(self, calibrator=c)
-                for c in self.calibrators
+                self.reqs.CalibrateEvents.req(self, calibrator=calibrator_inst.cls_name)
+                for calibrator_inst in self.calibrator_insts
+                if calibrator_inst.produced_columns
             ]
         else:
             # pass-through pilot workflow requirements of upstream task
             t = self.reqs.CalibrateEvents.req(self)
             reqs = law.util.merge_dicts(reqs, t.workflow_requires(), inplace=True)
 
         # add selector dependent requirements
@@ -61,16 +66,17 @@
 
         return reqs
 
     def requires(self):
         reqs = {
             "lfns": self.reqs.GetDatasetLFNs.req(self),
             "calibrations": [
-                self.reqs.CalibrateEvents.req(self, calibrator=c)
-                for c in self.calibrators
+                self.reqs.CalibrateEvents.req(self, calibrator=calibrator_inst.cls_name)
+                for calibrator_inst in self.calibrator_insts
+                if calibrator_inst.produced_columns
             ],
         }
 
         # add selector dependent requirements
         reqs["selector"] = self.selector_inst.run_requires()
 
         return reqs
@@ -138,15 +144,20 @@
             source_type=["coffea_root"] + n_calib * ["awkward_parquet"],
             read_columns=(1 + n_calib) * [read_columns],
         ):
             # apply the calibrated diffs
             events = update_ak_array(events, *diffs)
 
             # add aliases
-            events = add_ak_aliases(events, aliases, remove_src=True)
+            events = add_ak_aliases(
+                events,
+                aliases,
+                remove_src=True,
+                missing_strategy=self.missing_column_alias_strategy,
+            )
 
             # invoke the selection function
             events, results = self.selector_inst(events, stats)
             results_array = results.to_ak()
 
             # optional check for finite values
             if self.check_finite:
@@ -179,23 +190,23 @@
             sorted_chunks = [column_chunks[key] for key in sorted(column_chunks)]
             law.pyarrow.merge_parquet_task(self, sorted_chunks, outputs["columns"], local=True)
 
         # save stats
         outputs["stats"].dump(stats, indent=4, formatter="json")
 
         # print some stats
-        eff = safe_div(stats["n_events_selected"], stats["n_events"])
+        eff = safe_div(stats["num_events_selected"], stats["num_events"])
         eff_weighted = safe_div(stats["sum_mc_weight_selected"], stats["sum_mc_weight"])
-        self.publish_message(f"all events         : {int(stats['n_events'])}")
-        self.publish_message(f"sel. events        : {int(stats['n_events_selected'])}")
+        self.publish_message(f"all events         : {int(stats['num_events'])}")
+        self.publish_message(f"sel. events        : {int(stats['num_events_selected'])}")
         self.publish_message(f"efficiency         : {eff:.4f}")
         self.publish_message(f"sum mc weights     : {stats['sum_mc_weight']}")
         self.publish_message(f"sum sel. mc weights: {stats['sum_mc_weight_selected']}")
         self.publish_message(f"efficiency         : {eff_weighted:.4f}")
-        if not stats["n_events_selected"]:
+        if not eff:
             self.publish_message(law.util.colored("no events selected", "red"))
 
 
 # overwrite class defaults
 check_finite_tasks = law.config.get_expanded("analysis", "check_finite_output", [], split_csv=True)
 SelectEvents.check_finite = ChunkedIOMixin.check_finite.copy(
     default=SelectEvents.task_family in check_finite_tasks,
@@ -288,15 +299,15 @@
 class MergeSelectionMasks(
     SelectorMixin,
     CalibratorsMixin,
     DatasetTask,
     law.tasks.ForestMerge,
     RemoteWorkflow,
 ):
-    sandbox = dev_sandbox("bash::$CF_BASE/sandboxes/venv_columnar.sh")
+    sandbox = dev_sandbox(law.config.get("analysis", "default_columnar_sandbox"))
 
     # recursively merge 8 files into one
     merge_factor = 8
 
     # upstream requirements
     reqs = Requirements(
         RemoteWorkflow.reqs,
```

### Comparing `columnflow-0.2.1/columnflow/tasks/union.py` & `columnflow-0.2.2/columnflow/tasks/union.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     SelectorStepsMixin,
     CalibratorsMixin,
     ChunkedIOMixin,
     MergeReducedEventsUser,
     law.LocalWorkflow,
     RemoteWorkflow,
 ):
-    sandbox = dev_sandbox("bash::$CF_BASE/sandboxes/venv_columnar.sh")
+    sandbox = dev_sandbox(law.config.get("analysis", "default_columnar_sandbox"))
 
     # upstream requirements
     reqs = Requirements(
         MergeReducedEvents.reqs,
         RemoteWorkflow.reqs,
         MergeReducedEvents=MergeReducedEvents,
         ProduceColumns=ProduceColumns,
@@ -43,16 +43,17 @@
 
         # require the full merge forest
         reqs["events"] = self.reqs.MergeReducedEvents.req(self, tree_index=-1)
 
         if not self.pilot:
             if self.producers:
                 reqs["producers"] = [
-                    self.reqs.ProduceColumns.req(self, producer=p)
-                    for p in self.producers
+                    self.reqs.ProduceColumns.req(self, producer=producer_inst.cls_name)
+                    for producer_inst in self.producer_insts
+                    if producer_inst.produced_columns
                 ]
             if self.ml_models:
                 reqs["ml"] = [
                     self.reqs.MLEvaluation.req(self, ml_model=m)
                     for m in self.ml_models
                 ]
 
@@ -61,16 +62,17 @@
     def requires(self):
         reqs = {
             "events": self.reqs.MergeReducedEvents.req(self, tree_index=self.branch, _exclude={"branch"}),
         }
 
         if self.producers:
             reqs["producers"] = [
-                self.reqs.ProduceColumns.req(self, producer=p)
-                for p in self.producers
+                self.reqs.ProduceColumns.req(self, producer=producer_inst.cls_name)
+                for producer_inst in self.producer_insts
+                if producer_inst.produced_columns
             ]
         if self.ml_models:
             reqs["ml"] = [
                 self.reqs.MLEvaluation.req(self, ml_model=m)
                 for m in self.ml_models
             ]
```

### Comparing `columnflow-0.2.1/columnflow/tasks/yields.py` & `columnflow-0.2.2/columnflow/tasks/yields.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     CategoriesMixin,
     ProducersMixin,
     SelectorStepsMixin,
     CalibratorsMixin,
     law.LocalWorkflow,
     RemoteWorkflow,
 ):
-    sandbox = dev_sandbox("bash::$CF_BASE/sandboxes/venv_columnar.sh")
+    sandbox = dev_sandbox(law.config.get("analysis", "default_columnar_sandbox"))
 
     table_format = luigi.Parameter(
         default="fancy_grid",
         significant=False,
         description="format of the yield table; accepts all formats of the tabulate package; "
         "default: fancy_grid",
     )
@@ -226,15 +226,15 @@
                     elif self.normalize_yields == "per_category":
                         norm_factor = norm_factors[category]
                     else:
                         norm_factor = norm_factors
 
                     # format yields into strings
                     yields_str[category].append((value / norm_factor).str(
-                        # combine_uncs="all",  # TODO
+                        combine_uncs="all",
                         format=self.number_format,
                         style="latex" if "latex" in self.table_format else "plain",
                     ))
 
             # create, print and save the yield table
             yield_table = tabulate(yields_str, headers="keys", tablefmt=self.table_format)
             self.publish_message(yield_table)
```

### Comparing `columnflow-0.2.1/columnflow/util.py` & `columnflow-0.2.2/columnflow/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 import multiprocessing.pool
 from functools import wraps
 from collections import OrderedDict
 from typing import Callable, Any, Sequence, Union
 from types import ModuleType
 
 import law
+from law.util import InsertableDict  # noqa
 import luigi
 
 
 #: Placeholder for an unset value.
 UNSET = object()
 
 #: Boolean denoting whether the environment is in a remote job (based on ``CF_REMOTE_JOB``).
@@ -311,49 +312,64 @@
 
     def after_call(state):
         return
 
     return before_call, call, after_call
 
 
-def dev_sandbox(sandbox: str) -> str:
+def dev_sandbox(sandbox: str, add: bool = True, remove: bool = True) -> str:
     """
-    Takes a sandbox key *sandbox* and injects the subtring "_dev" right before the file extension
-    (if any) in case the current environment is used for development (see :py:attr:`env_is_dev`) and
-    the corresponding sandbox exists. Otherwise *sandbox* is returned unchanged.
+    Takes a sandbox key *sandbox* and adds or removes the substring "_dev" right before the file
+    extension (if any), depending on whether the current environment is used for development (see
+    :py:attr:`env_is_dev`) and the *add* and *remove* flags.
+
+    If *sandbox* does not contain the "_dev" postfix and both :py:attr:`env_is_dev` and *add* are
+    *True*, the postfix is appended.
+
+    If *sandbox* does (!) contain the "_dev" postfix, :py:attr:`env_is_dev` is *False* and *remove*
+    is *True*, the postfix is removed.
+
+    In any other case, *sandbox* is returned unchanged.
+
+    Examples:
 
     .. code-block:: python
 
         # if env_is_dev and /path/to/script_dev.sh exists
         dev_sandbox("bash::/path/to/script.sh")
         # -> "bash::/path/to/script_dev.sh"
 
         # otherwise
         dev_sandbox("bash::/path/to/script.sh")
         # -> "bash::/path/to/script.sh"
     """
-    # do nothing when not in dev env
-    if not env_is_dev:
-        return sandbox
-
     # only take into account venv and bash sandboxes
     _type, path = law.Sandbox.split_key(sandbox)
     if _type not in ["venv", "bash"]:
         return sandbox
 
-    # create the dev path and check if it exists, with special treatment of the cf_{prod,dev} envs
-    if path == "$CF_BASE/sandboxes/cf_prod.sh":
-        dev_path = "$CF_BASE/sandboxes/cf_dev.sh"
+    # check if the sandbox is dev
+    path_no_ext, ext = os.path.splitext(path)
+    sandbox_is_dev = path_no_ext.endswith("_dev")
+
+    # update the path if needed
+    if not sandbox_is_dev and env_is_dev and add:
+        path = f"{path_no_ext}_dev{ext}"
+    elif sandbox_is_dev and not env_is_dev and remove:
+        path = f"{path_no_ext[:-4]}{ext}"
     else:
-        dev_path = "{}_dev{}".format(*os.path.splitext(path))
-    if not os.path.exists(real_path(dev_path)):
+        # nothing to do in any other case
+        return sandbox
+
+    # if the path does not exist, return the sandbox unchanged as well
+    if not os.path.exists(real_path(path)):
         return sandbox
 
     # all checks passed
-    return law.Sandbox.join_key(_type, dev_path)
+    return law.Sandbox.join_key(_type, path)
 
 
 def freeze(cont: Any) -> Any:
     """Constructs an immutable version of a native Python container.
 
     Recursively replaces all mutable containers (``dict``, ``list``, ``set``) encountered within
     *cont* by an immutable equivalent: Lists are converted to tuples, sets to ``frozenset``
```

### Comparing `columnflow-0.2.1/columnflow.egg-info/PKG-INFO` & `columnflow-0.2.2/columnflow.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: columnflow
-Version: 0.2.1
+Version: 0.2.2
 Summary: columnflow
 Home-page: https://github.com/columnflow/columnflow
 Author: The columnflow team
 Author-email: github.riga@icloud.com
 License: BSD-3-Clause
 Keywords: physics,analysis,experiment,columnar,vectoized,law,order,luigi,lhc,cms
 Classifier: Programming Language :: Python
@@ -37,14 +37,16 @@
 [![Package version](https://img.shields.io/pypi/v/columnflow.svg?style=flat)](https://pypi.python.org/pypi/columnflow)
 [![Documentation status](https://readthedocs.org/projects/columnflow/badge/?version=stable)](http://columnflow.readthedocs.io)
 [![Code coverge](https://codecov.io/gh/columnflow/columnflow/branch/master/graph/badge.svg?token=33FLINPXFP)](https://codecov.io/gh/columnflow/columnflow)
 [![License](https://img.shields.io/github/license/columnflow/columnflow.svg)](https://github.com/columnflow/columnflow/blob/master/LICENSE)
 
 Backend for columnar, fully orchestrated HEP analyses with pure Python, [law](https://github.com/riga/law) and [order](https://github.com/riga/order).
 
+Original source hosted at [GitHub](https://github.com/columnflow/columnflow).
+
 
 <!-- marker-after-header -->
 
 
 ## Note on current development
 
 This project is currently in a beta phase.
@@ -66,44 +68,49 @@
 ```
 
 At the end of the setup, you will see further instructions and suggestions to run your first analysis tasks (example below).
 
 ```
 Setup successfull! The next steps are:
 
-  1. Setup the repository and install the environment.
-    > source setup.sh [optional_setup_name]
+1. Setup the repository and install the environment.
+   > cd
+   > source setup.sh [optional_setup_name]
 
-  2. Run local tests & linting checks to verify that the analysis is setup correctly.
-    > ./tests/run_all
+2. Run local tests & linting checks to verify that the analysis is setup correctly.
+   > ./tests/run_all
 
-  3. Create a GRID proxy if you intend to run tasks that need one
-    > voms-proxy-init -voms cms -rfc -valid 196:00
+3. Create a GRID proxy if you intend to run tasks that need one
+   > voms-proxy-init -rfc -valid 196:00
 
-  4. Checkout the 'Getting started' guide to run your first tasks.
-    https://columnflow.readthedocs.io/en/stable/start.html
+4. Checkout the 'Getting started' guide to run your first tasks.
+   https://columnflow.readthedocs.io/en/stable/start.html
 
-    Suggestions for tasks to run:
+   Suggestions for tasks to run:
 
-    a) Run the 'calibration -> selection -> reduction' pipeline for the first file of the
-       default dataset using the default calibrator and default selector
-       (enter the command below and 'tab-tab' to see all arguments or add --help for help)
+   a) Run the 'calibration -> selection -> reduction' pipeline for the first file of the
+      default dataset using the default calibrator and default selector
+      (enter the command below and 'tab-tab' to see all arguments or add --help for help)
       > law run cf.ReduceEvents --version dev1 --branch 0
 
-    b) Create the jet1_pt distribution for the single top dataset:
+      Verify what you just run by adding '--print-status -1' (-1 = fully recursive)
+      > law run cf.ReduceEvents --version dev1 --branch 0 --print-status -1
+
+   b) Create the jet1_pt distribution for the single top datasets
+      (if you have an image/pdf viewer installed, add it via '--view-cmd <binary>')
       > law run cf.PlotVariables1D --version dev1 --datasets 'st*' --variables jet1_pt
 
-    c) Include the ttbar dataset and also plot jet1_eta:
-      > law run cf.PlotVariables1D --version dev1 --datasets 'tt*,st*' --variables jet1_pt,jet1_eta
+      Again, verify what you just ran, now with recursion depth 4
+      > law run cf.PlotVariables1D --version dev1 --datasets 'st*' --variables jet1_pt --print-status 4
 
-    d) Create cms-style datacards for the example model in hgg/inference/example.py:
-      > law run cf.CreateDatacards --version dev1 --inference-model example
+   c) Include the ttbar dataset and also plot jet1_eta
+      > law run cf.PlotVariables1D --version dev1 --datasets 'tt*,st*' --variables jet1_pt,jet1_eta
 ```
 
-For a better overview of the tasks that are triggered by the commands below, checkout the current (yet stylized) [task graph](https://github.com/columnflow/columnflow/issues/25#issue-1258137827).
+For a better overview of the tasks that are triggered by the commands below, checkout the current (yet stylized) [task graph](https://github.com/columnflow/columnflow/wiki#default-task-graph).
 
 
 ## Projects using columnflow
 
 - [hh2bbtautau](https://github.com/uhh-cms/hh2bbtautau): HH → bb𝜏𝜏 analysis with CMS.
 - [hh2bbww](https://github.com/uhh-cms/hh2bbww): HH → bbWW analysis with CMS.
 - [topmass](https://github.com/uhh-cms/topmass): Top quark mass measurement with CMS.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: columnflow Version: 0.2.1 Summary: columnflow Home-
+Metadata-Version: 2.1 Name: columnflow Version: 0.2.2 Summary: columnflow Home-
 page: https://github.com/columnflow/columnflow Author: The columnflow team
 Author-email: github.riga@icloud.com License: BSD-3-Clause Keywords:
 physics,analysis,experiment,columnar,vectoized,law,order,luigi,lhc,cms
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
@@ -20,16 +20,17 @@
 columnflow) [![Documentation status](https://readthedocs.org/projects/
 columnflow/badge/?version=stable)](http://columnflow.readthedocs.io) [![Code
 coverge](https://codecov.io/gh/columnflow/columnflow/branch/master/graph/
 badge.svg?token=33FLINPXFP)](https://codecov.io/gh/columnflow/columnflow) [!
 [License](https://img.shields.io/github/license/columnflow/columnflow.svg)]
 (https://github.com/columnflow/columnflow/blob/master/LICENSE) Backend for
 columnar, fully orchestrated HEP analyses with pure Python, [law](https://
-github.com/riga/law) and [order](https://github.com/riga/order).  ## Note on
-current development This project is currently in a beta phase. The project
+github.com/riga/law) and [order](https://github.com/riga/order). Original
+source hosted at [GitHub](https://github.com/columnflow/columnflow).  ## Note
+on current development This project is currently in a beta phase. The project
 setup, suggested workflows, definitions of particular tasks, and the signatures
 of various helper classes and functions are mostly frozen but could still be
 subject to changes in the near future. At this point (December 2022), four
 large-scale analyses based upon columnflow are being developed, and in the
 process, help test and verify various aspects of its core. The first released
 version is expected in early 2023. However, if you would like to join early on,
 contribute or just give it a spin, feel free to get in touch! ![Columnflow
@@ -40,39 +41,42 @@
 columnflow/columnflow/tree/master/analysis_templates)). The following command
 (no previous git clone required) interactively asks for a handful of names and
 settings, and creates a minimal, yet fully functioning project structure for
 you! ```shell bash -c "$(curl -Ls https://raw.githubusercontent.com/columnflow/
 columnflow/master/create_analysis.sh)" ``` At the end of the setup, you will
 see further instructions and suggestions to run your first analysis tasks
 (example below). ``` Setup successfull! The next steps are: 1. Setup the
-repository and install the environment. > source setup.sh [optional_setup_name]
-2. Run local tests & linting checks to verify that the analysis is setup
-correctly. > ./tests/run_all 3. Create a GRID proxy if you intend to run tasks
-that need one > voms-proxy-init -voms cms -rfc -valid 196:00 4. Checkout the
-'Getting started' guide to run your first tasks. https://
+repository and install the environment. > cd > source setup.sh
+[optional_setup_name] 2. Run local tests & linting checks to verify that the
+analysis is setup correctly. > ./tests/run_all 3. Create a GRID proxy if you
+intend to run tasks that need one > voms-proxy-init -rfc -valid 196:00 4.
+Checkout the 'Getting started' guide to run your first tasks. https://
 columnflow.readthedocs.io/en/stable/start.html Suggestions for tasks to run: a)
 Run the 'calibration -> selection -> reduction' pipeline for the first file of
 the default dataset using the default calibrator and default selector (enter
 the command below and 'tab-tab' to see all arguments or add --help for help) >
-law run cf.ReduceEvents --version dev1 --branch 0 b) Create the jet1_pt
-distribution for the single top dataset: > law run cf.PlotVariables1D --version
-dev1 --datasets 'st*' --variables jet1_pt c) Include the ttbar dataset and also
-plot jet1_eta: > law run cf.PlotVariables1D --version dev1 --datasets 'tt*,st*'
---variables jet1_pt,jet1_eta d) Create cms-style datacards for the example
-model in hgg/inference/example.py: > law run cf.CreateDatacards --version dev1
---inference-model example ``` For a better overview of the tasks that are
-triggered by the commands below, checkout the current (yet stylized) [task
-graph](https://github.com/columnflow/columnflow/issues/25#issue-1258137827). ##
-Projects using columnflow - [hh2bbtautau](https://github.com/uhh-cms/
-hh2bbtautau): HH â bbðð analysis with CMS. - [hh2bbww](https://
-github.com/uhh-cms/hh2bbww): HH â bbWW analysis with CMS. - [topmass](https:/
-/github.com/uhh-cms/topmass): Top quark mass measurement with CMS. - [mttbar]
-(https://github.com/uhh-cms/mttbar): Search for heavy resonances in ttbar
-events with CMS. - [analysis playground](https://github.com/uhh-cms/
-analysis_playground): A testing playground for HEP analyses. ## Contributors
+law run cf.ReduceEvents --version dev1 --branch 0 Verify what you just run by
+adding '--print-status -1' (-1 = fully recursive) > law run cf.ReduceEvents --
+version dev1 --branch 0 --print-status -1 b) Create the jet1_pt distribution
+for the single top datasets (if you have an image/pdf viewer installed, add it
+via '--view-cmd ') > law run cf.PlotVariables1D --version dev1 --datasets 'st*'
+--variables jet1_pt Again, verify what you just ran, now with recursion depth 4
+> law run cf.PlotVariables1D --version dev1 --datasets 'st*' --variables
+jet1_pt --print-status 4 c) Include the ttbar dataset and also plot jet1_eta >
+law run cf.PlotVariables1D --version dev1 --datasets 'tt*,st*' --variables
+jet1_pt,jet1_eta ``` For a better overview of the tasks that are triggered by
+the commands below, checkout the current (yet stylized) [task graph](https://
+github.com/columnflow/columnflow/wiki#default-task-graph). ## Projects using
+columnflow - [hh2bbtautau](https://github.com/uhh-cms/hh2bbtautau): HH â
+bbðð analysis with CMS. - [hh2bbww](https://github.com/uhh-cms/hh2bbww):
+HH â bbWW analysis with CMS. - [topmass](https://github.com/uhh-cms/topmass):
+Top quark mass measurement with CMS. - [mttbar](https://github.com/uhh-cms/
+mttbar): Search for heavy resonances in ttbar events with CMS. - [analysis
+playground](https://github.com/uhh-cms/analysis_playground): A testing
+playground for HEP analyses. ## Contributors
             [Marcel_Rieger]              [Mathis_Frahm]    [Daniel_Savoiu]      [pkausw]           [nprouvost]       [Bogdan-Wiederspan]  [Tobias
              Marcel_Rieger                Mathis_Frahm      Daniel_Savoiu        pkausw             nprouvost         Bogdan-Wiederspan   Kramer]
          ð» ð ð â    ð» ð�    ð» ð�    ð» ð�     ð» â ï     ð» â ï Tobias
                                                                                                                                            Kramer
                                                                                                                                             ð»
               [Matthias_Schroeder]      [Johannes_Lange]   [BalduinLetzer]
                Matthias_Schroeder        Johannes_Lange     BalduinLetzer
```

### Comparing `columnflow-0.2.1/columnflow.egg-info/SOURCES.txt` & `columnflow-0.2.2/columnflow.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 columnflow/production/cms/muon.py
 columnflow/production/cms/pdf.py
 columnflow/production/cms/pileup.py
 columnflow/production/cms/scale.py
 columnflow/production/cms/seeds.py
 columnflow/selection/__init__.py
 columnflow/selection/matching.py
+columnflow/selection/stats.py
+columnflow/selection/util.py
 columnflow/selection/cms/__init__.py
 columnflow/selection/cms/json_filter.py
 columnflow/selection/cms/met_filters.py
 columnflow/tasks/__init__.py
 columnflow/tasks/calibration.py
 columnflow/tasks/cutflow.py
 columnflow/tasks/external.py
```

### Comparing `columnflow-0.2.1/setup.py` & `columnflow-0.2.2/setup.py`

 * *Files identical despite different names*

