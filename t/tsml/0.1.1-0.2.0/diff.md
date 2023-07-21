# Comparing `tmp/tsml-0.1.1.tar.gz` & `tmp/tsml-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsml-0.1.1.tar", last modified: Thu May 18 17:12:19 2023, max compression
+gzip compressed data, was "tsml-0.2.0.tar", last modified: Fri Jul 21 13:23:30 2023, max compression
```

## Comparing `tsml-0.1.1.tar` & `tsml-0.2.0.tar`

### file list

```diff
@@ -1,104 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:19.385156 tsml-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-18 17:12:10.000000 tsml-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-18 17:12:10.000000 tsml-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-18 17:12:19.385156 tsml-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-18 17:12:10.000000 tsml-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-18 17:12:10.000000 tsml-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 17:12:19.385156 tsml-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:19.365157 tsml-0.1.1/tsml/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:19.369156 tsml-0.1.1/tsml/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:19.369156 tsml-0.1.1/tsml/datasets/EqualMinimalJapaneseVowels/
--rw-r--r--   0 runner    (1001) docker     (123)   120661 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)   120799 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:19.369156 tsml-0.1.1/tsml/datasets/MinimalChinatown/
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:19.369156 tsml-0.1.1/tsml/datasets/MinimalGasPrices/
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:19.369156 tsml-0.1.1/tsml/datasets/MinimalJapaneseVowels/
--rw-r--r--   0 runner    (1001) docker     (123)    36247 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)    38758 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:19.369156 tsml-0.1.1/tsml/datasets/UnequalMinimalChinatown/
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:19.373156 tsml-0.1.1/tsml/datasets/UnequalMinimalGasPrices/
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24932 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/datasets/_data_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:19.373156 tsml-0.1.1/tsml/datasets/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/datasets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   286342 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/datasets/tests/_expected_data_io_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/datasets/tests/test_data_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:19.373156 tsml-0.1.1/tsml/distance_based/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/distance_based/_mpdist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/distance_based/_pf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:19.373156 tsml-0.1.1/tsml/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/dummy/_dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:19.373156 tsml-0.1.1/tsml/feature_based/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/feature_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17111 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/feature_based/_catch22.py
--rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/feature_based/_fpca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:19.377156 tsml-0.1.1/tsml/interval_based/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/interval_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46571 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/interval_based/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/interval_based/_cif.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/interval_based/_interval_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)    21887 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/interval_based/_interval_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/interval_based/_rise.py
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/interval_based/_stsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/interval_based/_tsf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:19.377156 tsml-0.1.1/tsml/interval_based/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/interval_based/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/interval_based/tests/test_interval_forest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:19.377156 tsml-0.1.1/tsml/shapelet_based/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/shapelet_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/shapelet_based/_mrsqm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/shapelet_based/_rsf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/shapelet_based/_stc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:19.377156 tsml-0.1.1/tsml/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47313 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/tests/_sklearn_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/tests/estimator_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/tests/test_all_estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/tests/test_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:19.381157 tsml-0.1.1/tsml/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/transformations/_acf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/transformations/_ar_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)    41826 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/transformations/_catch22.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/transformations/_fpca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/transformations/_function_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    35733 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/transformations/_interval_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/transformations/_periodogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    41527 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/transformations/_sfa.py
--rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/transformations/_shapelet_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/transformations/_summary_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:19.381157 tsml-0.1.1/tsml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/utils/_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/utils/discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:19.385156 tsml-0.1.1/tsml/utils/numba_functions/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/utils/numba_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/utils/numba_functions/general.py
--rw-r--r--   0 runner    (1001) docker     (123)    19873 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/utils/numba_functions/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:19.385156 tsml-0.1.1/tsml/vector/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15953 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/vector/_cit.py
--rw-r--r--   0 runner    (1001) docker     (123)    30856 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/vector/_rotation_forest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:19.385156 tsml-0.1.1/tsml/vector/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/vector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-18 17:12:10.000000 tsml-0.1.1/tsml/vector/tests/test_rotation_forest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:12:19.369156 tsml-0.1.1/tsml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-18 17:12:19.000000 tsml-0.1.1/tsml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-18 17:12:19.000000 tsml-0.1.1/tsml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:12:19.000000 tsml-0.1.1/tsml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-18 17:12:19.000000 tsml-0.1.1/tsml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-18 17:12:19.000000 tsml-0.1.1/tsml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.817438 tsml-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-21 13:23:15.000000 tsml-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-21 13:23:15.000000 tsml-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-21 13:23:30.817438 tsml-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-21 13:23:15.000000 tsml-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-21 13:23:15.000000 tsml-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 13:23:30.817438 tsml-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.793438 tsml-0.2.0/tsml/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.797438 tsml-0.2.0/tsml/compose/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/compose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20638 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/compose/_channel_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.797438 tsml-0.2.0/tsml/compose/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/compose/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/compose/tests/test_channel_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.797438 tsml-0.2.0/tsml/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.797438 tsml-0.2.0/tsml/datasets/EqualMinimalJapaneseVowels/
+-rw-r--r--   0 runner    (1001) docker     (123)   120661 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)   120799 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.797438 tsml-0.2.0/tsml/datasets/MinimalChinatown/
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.797438 tsml-0.2.0/tsml/datasets/MinimalGasPrices/
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.801438 tsml-0.2.0/tsml/datasets/MinimalJapaneseVowels/
+-rw-r--r--   0 runner    (1001) docker     (123)    36247 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    38758 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.801438 tsml-0.2.0/tsml/datasets/UnequalMinimalChinatown/
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.801438 tsml-0.2.0/tsml/datasets/UnequalMinimalGasPrices/
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24932 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/_data_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.801438 tsml-0.2.0/tsml/datasets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   286342 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/tests/_expected_data_io_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/tests/test_data_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.801438 tsml-0.2.0/tsml/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/distance_based/_mpdist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/distance_based/_pf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.801438 tsml-0.2.0/tsml/distances/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/distances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/distances/_manhattan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.801438 tsml-0.2.0/tsml/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/dummy/_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.805438 tsml-0.2.0/tsml/feature_based/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/feature_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20217 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/feature_based/_catch22.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/feature_based/_fpca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.805438 tsml-0.2.0/tsml/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/hybrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22124 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/hybrid/_rist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.805438 tsml-0.2.0/tsml/interval_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/interval_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48835 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/interval_based/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41948 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/interval_based/_cif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21846 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/interval_based/_interval_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26649 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/interval_based/_interval_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/interval_based/_rise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17244 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/interval_based/_stsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16955 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/interval_based/_tsf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.805438 tsml-0.2.0/tsml/interval_based/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/interval_based/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/interval_based/tests/test_interval_forest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.809438 tsml-0.2.0/tsml/shapelet_based/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/shapelet_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/shapelet_based/_mrsqm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20841 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/shapelet_based/_rdst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11162 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/shapelet_based/_rsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/shapelet_based/_stc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.809438 tsml-0.2.0/tsml/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/tests/test_all_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/tests/test_estimator_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47622 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/tests/test_estimators_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/tests/test_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.809438 tsml-0.2.0/tsml/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/_acf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/_ar_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43348 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/_catch22.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/_fpca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/_function_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37045 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/_interval_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/_periodogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41527 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/_sfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56382 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/_shapelet_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/_summary_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/_transform_concatenator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.813438 tsml-0.2.0/tsml/transformations/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/tests/test_function_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/tests/test_interval_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/tests/test_periodogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/tests/test_transform_concatenator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.813438 tsml-0.2.0/tsml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/utils/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/utils/discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.813438 tsml-0.2.0/tsml/utils/numba_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/utils/numba_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/utils/numba_functions/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21053 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/utils/numba_functions/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22415 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.813438 tsml-0.2.0/tsml/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15847 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/vector/_cit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29766 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/vector/_rotation_forest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.813438 tsml-0.2.0/tsml/vector/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/vector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/vector/tests/test_rotation_forest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.797438 tsml-0.2.0/tsml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-21 13:23:30.000000 tsml-0.2.0/tsml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-21 13:23:30.000000 tsml-0.2.0/tsml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:23:30.000000 tsml-0.2.0/tsml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-21 13:23:30.000000 tsml-0.2.0/tsml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 13:23:30.000000 tsml-0.2.0/tsml.egg-info/top_level.txt
```

### Comparing `tsml-0.1.1/LICENSE` & `tsml-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tsml-0.1.1/PKG-INFO` & `tsml-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsml
-Version: 0.1.1
+Version: 0.2.0
 Summary: A toolkit for time series machine learning algorithms.
 Author-email: Matthew Middlehurst <m.middlehurst@uea.ac.uk>, Tony Bagnall <ajb@uea.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) The Time Series Machine Learning (tsml) developers.
         All rights reserved.
         
@@ -49,14 +49,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: extras
 Provides-Extra: unstable_extras
 Provides-Extra: dev
+Provides-Extra: binder
 Provides-Extra: docs
 License-File: LICENSE
 
 # tsml
 
 A toolkit for time series machine learning algorithms
```

### Comparing `tsml-0.1.1/pyproject.toml` & `tsml-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "wheel", "toml", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tsml"
-version = "0.1.1"
+version = "0.2.0"
 description = "A toolkit for time series machine learning algorithms."
 authors = [
     {name = "Matthew Middlehurst", email = "m.middlehurst@uea.ac.uk"},
     {name = "Tony Bagnall", email = "ajb@uea.ac.uk"},
 ]
 readme = "README.md"
 requires-python = ">=3.8,<3.12"
@@ -59,22 +59,28 @@
     "pre-commit",
     "pytest",
     "pytest-randomly",
     "pytest-timeout",
     "pytest-xdist",
     "pytest-cov",
 ]
+binder = [
+    "notebook",
+    "jupyterlab",
+]
 docs = [
     "sphinx",
     "sphinx-design",
-    "sphinx-gallery",
     "nbsphinx",
     "numpydoc",
     "jupyter",
     "furo",
+    "sphinx_issues",
+    "myst-parser",
+    "sphinx-copybutton",
 ]
 
 [project.urls]
 homepage = "https://www.timeseriesclassification.com/"
 repository = "https://github.com/time-series-machine-learning/tsml-py/"
 
 [project.license]
@@ -88,21 +94,16 @@
     "examples/**",
     "docs/**",
     "*.yaml",
     "*.yml",
     ".coveragerc",
 ]
 
-[tool.flake8]
-max-line-length = 88
-extend-ignore = ["E203"]
-
 [tool.pytest.ini_options]
+testpaths = "tsml"
 addopts = '''
-    --ignore examples
-    --ignore docs
-    --durations 10
+    --durations 20
     --timeout 600
     --showlocals
     --doctest-modules
     --numprocesses auto
 '''
```

### Comparing `tsml-0.1.1/tsml/base.py` & `tsml-0.2.0/tsml/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Base classes for estimators."""
 
 __author__ = ["MatthewMiddlehurst"]
 __all__ = [
     "BaseTimeSeriesEstimator",
     "_clone_estimator",
 ]
@@ -263,21 +262,16 @@
             special parameters are defined for a value, will return `"default"` set.
 
         Returns
         -------
         params : dict or list of dict
             Parameters to create testing instances of the class.
         """
-        if parameter_set is None:
-            # default parameters = empty dict
-            return {}
-        else:
-            raise ValueError(
-                f"No parameter set {parameter_set} defined for {cls.__name__}"
-            )
+        # default parameters = empty dict
+        return {}
 
 
 def _clone_estimator(
     base_estimator: BaseEstimator, random_state: Union[None, int, RandomState] = None
 ) -> BaseEstimator:
     """Clone an estimator and set the random state if available."""
     estimator = clone(base_estimator)
```

### Comparing `tsml-0.1.1/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts` & `tsml-0.2.0/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.1.1/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts` & `tsml-0.2.0/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.1.1/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts` & `tsml-0.2.0/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.1.1/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts` & `tsml-0.2.0/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.1.1/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts` & `tsml-0.2.0/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.1.1/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts` & `tsml-0.2.0/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.1.1/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts` & `tsml-0.2.0/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.1.1/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts` & `tsml-0.2.0/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.1.1/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts` & `tsml-0.2.0/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.1.1/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts` & `tsml-0.2.0/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.1.1/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts` & `tsml-0.2.0/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.1.1/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts` & `tsml-0.2.0/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.1.1/tsml/datasets/__init__.py` & `tsml-0.2.0/tsml/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `tsml-0.1.1/tsml/datasets/_data_io.py` & `tsml-0.2.0/tsml/datasets/_data_io.py`

 * *Files identical despite different names*

### Comparing `tsml-0.1.1/tsml/datasets/tests/_expected_data_io_output.py` & `tsml-0.2.0/tsml/datasets/tests/_expected_data_io_output.py`

 * *Files identical despite different names*

### Comparing `tsml-0.1.1/tsml/datasets/tests/test_data_io.py` & `tsml-0.2.0/tsml/datasets/tests/test_data_io.py`

 * *Files identical despite different names*

### Comparing `tsml-0.1.1/tsml/distance_based/_pf.py` & `tsml-0.2.0/tsml/distance_based/_pf.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,26 @@
-# -*- coding: utf-8 -*-
+"""Proximity Forest (PF) Classifier."""
+
+__author__ = ["MatthewMiddlehurst"]
+
+from typing import List, Union
+
 import numpy as np
 from sklearn.base import ClassifierMixin
 from sklearn.utils.multiclass import check_classification_targets
 from sklearn.utils.validation import check_is_fitted
 
 from tsml.base import BaseTimeSeriesEstimator
 from tsml.utils.validation import _check_optional_dependency, check_n_jobs
 
 
 class ProximityForestClassifier(ClassifierMixin, BaseTimeSeriesEstimator):
-    """
-    Wrapper for https://github.com/wildboar-foundation/wildboar PF implementation.
+    """Proximity Forest (PF) Classifier.
+
+    Wrapper for the wildboar PF implementation.
     """
 
     def __init__(
         self,
         n_estimators=100,
         n_pivot=1,
         pivot_sample="label",
@@ -23,43 +29,57 @@
         max_depth=None,
         min_samples_split=2,
         min_samples_leaf=1,
         min_impurity_decrease=0,
         criterion="entropy",
         bootstrap=True,
         oob_score=False,
-        n_jobs=None,
         random_state=None,
+        n_jobs=None,
     ):
         self.n_estimators = n_estimators
         self.n_pivot = n_pivot
         self.pivot_sample = pivot_sample
         self.metric_sample = metric_sample
         self.metric_factories = metric_factories
         self.max_depth = max_depth
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.min_impurity_decrease = min_impurity_decrease
         self.criterion = criterion
         self.bootstrap = bootstrap
         self.oob_score = oob_score
-        self.n_jobs = n_jobs
         self.random_state = random_state
+        self.n_jobs = n_jobs
 
         _check_optional_dependency("wildboar", "wildboar", self)
 
         super(ProximityForestClassifier, self).__init__()
 
-    def fit(self, X, y):
+    def fit(self, X: Union[np.ndarray, List[np.ndarray]], y: np.ndarray) -> object:
+        """Fit the estimator to training data.
+
+        Parameters
+        ----------
+        X : 3D np.ndarray of shape (n_instances, n_channels, n_timepoints)
+            The training data.
+        y : 1D np.ndarray of shape (n_instances)
+            The class labels for fitting, indices correspond to instance indices in X
+
+        Returns
+        -------
+        self :
+            Reference to self.
+        """
         X, y = self._validate_data(X=X, y=y, ensure_min_samples=2)
         X = self._convert_X(X)
 
         check_classification_targets(y)
 
-        self.n_instances_, self.n_dims_, self.series_length_ = (
+        self.n_instances_, self.n_channels_, self.n_timepoints_ = (
             X.shape if X.ndim == 3 else (X.shape[0], 1, X.shape[1])
         )
         self.classes_ = np.unique(y)
         self.n_classes_ = self.classes_.shape[0]
         self.class_dictionary_ = {}
         for index, class_val in enumerate(self.classes_):
             self.class_dictionary_[class_val] = index
@@ -83,70 +103,93 @@
             oob_score=self.oob_score,
             max_depth=self.max_depth,
             min_samples_split=self.min_samples_split,
             min_samples_leaf=self.min_samples_leaf,
             min_impurity_decrease=self.min_impurity_decrease,
             criterion=self.criterion,
             bootstrap=self.bootstrap,
-            n_jobs=self.n_jobs,
             random_state=self.random_state,
+            n_jobs=self.n_jobs,
         )
         self.clf_.fit(X, y)
 
         return self
 
-    def predict(self, X) -> np.ndarray:
+    def predict(self, X: Union[np.ndarray, List[np.ndarray]]) -> np.ndarray:
+        """Predicts labels for sequences in X.
+
+        Parameters
+        ----------
+        X : 3D np.array of shape (n_instances, n_channels, n_timepoints)
+            The testing data.
+
+        Returns
+        -------
+        y : array-like of shape (n_instances)
+            Predicted class labels.
+        """
         check_is_fitted(self)
 
         # treat case of single class seen in fit
         if self.n_classes_ == 1:
             return np.repeat(list(self.class_dictionary_.keys()), X.shape[0], axis=0)
 
         X = self._validate_data(X=X, reset=False)
         X = self._convert_X(X)
 
         if X.ndim == 3 and X.shape[1] == 1:
             X = np.reshape(X, (X.shape[0], X.shape[2]))
 
         return self.clf_.predict(X)
 
-    def predict_proba(self, X) -> np.ndarray:
+    def predict_proba(self, X: Union[np.ndarray, List[np.ndarray]]) -> np.ndarray:
+        """Predicts labels probabilities for sequences in X.
+
+        Parameters
+        ----------
+        X : 3D np.array of shape (n_instances, n_channels, n_timepoints)
+            The testing data.
+
+        Returns
+        -------
+        y : array-like of shape (n_instances, n_classes_)
+            Predicted probabilities using the ordering in classes_.
+        """
         check_is_fitted(self)
 
         # treat case of single class seen in fit
         if self.n_classes_ == 1:
             return np.repeat([[1]], X.shape[0], axis=0)
 
         X = self._validate_data(X=X, reset=False)
         X = self._convert_X(X)
 
         if X.ndim == 3 and X.shape[1] == 1:
             X = np.reshape(X, (X.shape[0], X.shape[2]))
 
         return self.clf_.predict_proba(X)
 
+    def _more_tags(self) -> dict:
+        return {
+            "optional_dependency": True,
+        }
+
     @classmethod
-    def get_test_params(cls, parameter_set="default"):
-        """Return testing parameter settings for the estimator.
+    def get_test_params(
+        cls, parameter_set: Union[str, None] = None
+    ) -> Union[dict, List[dict]]:
+        """Return unit test parameter settings for the estimator.
 
         Parameters
         ----------
-        parameter_set : str, default="default"
+        parameter_set : None or str, default=None
             Name of the set of test parameters to return, for use in tests. If no
             special parameters are defined for a value, will return `"default"` set.
-            For classifiers, a "default" set of parameters should be provided for
-            general testing, and a "results_comparison" set for comparing against
-            previously recorded results if the general set does not produce suitable
-            probabilities to compare against.
 
         Returns
         -------
-        params : dict or list of dict, default={}
+        params : dict or list of dict
             Parameters to create testing instances of the class.
-            Each dict are parameters to construct an "interesting" test instance, i.e.,
-            `MyClass(**params)` or `MyClass(**params[i])` creates a valid test instance.
-            `create_test_instance` uses the first (or only) dictionary in `params`.
         """
-
         return {
             "n_estimators": 2,
         }
```

### Comparing `tsml-0.1.1/tsml/interval_based/__init__.py` & `tsml-0.2.0/tsml/interval_based/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-"""Interval based estimators."""
+"""Interval-based estimators."""
 
 __all__ = [
     "BaseIntervalForest",
     "CIFClassifier",
     "CIFRegressor",
     "DrCIFClassifier",
     "DrCIFRegressor",
```

### Comparing `tsml-0.1.1/tsml/interval_based/_base.py` & `tsml-0.2.0/tsml/interval_based/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-# -*- coding: utf-8 -*-
-"""A base class for interval extracting forest estimators"""
+"""A base class for interval extracting forest estimators."""
 
 __author__ = ["MatthewMiddlehurst"]
 __all__ = ["BaseIntervalForest"]
 
 import inspect
 import time
 import warnings
 from abc import ABCMeta, abstractmethod
+from typing import List, Union
 
 import numpy as np
 from joblib import Parallel
 from sklearn.base import BaseEstimator, is_classifier, is_regressor
-from sklearn.tree import (
-    BaseDecisionTree,
-    DecisionTreeClassifier,
-    DecisionTreeRegressor,
-    ExtraTreeClassifier,
-)
+from sklearn.tree import BaseDecisionTree, DecisionTreeClassifier, DecisionTreeRegressor
 from sklearn.utils import check_random_state
 from sklearn.utils.fixes import delayed
 from sklearn.utils.multiclass import check_classification_targets
 from sklearn.utils.validation import check_is_fitted
 
 from tsml.base import BaseTimeSeriesEstimator, _clone_estimator
 from tsml.transformations._interval_extraction import (
@@ -35,20 +30,18 @@
 
 class BaseIntervalForest(BaseTimeSeriesEstimator, metaclass=ABCMeta):
     """A base class for interval extracting forest estimators.
 
     Allows the implementation of classifiers and regressors along the lines of [1][2][3]
     which extract intervals and create an ensemble from the subsequent features.
 
-    #skipping predict todo
-
     Parameters
     ----------
     base_estimator : BaseEstimator or None, default=None
-        scikit-learn BaseEstimator used to build the interval ensemble. If None, uses a
+        scikit-learn BaseEstimator used to build the interval ensemble. If None, use a
         simple decision tree.
     n_estimators : int, default=200
         Number of estimators to build for the ensemble.
     interval_selection_method : "random", "supervised" or "random-supervised",
             default="random"
         The interval selection transformer to use.
             - "random" uses a RandomIntervalTransformer.
@@ -61,28 +54,30 @@
     n_intervals : int, str, list or tuple, default="sqrt"
         Number of intervals to extract per tree for each series_transformers series.
 
         An int input will extract that number of intervals from the series, while a str
         input will return a function of the series length (may differ per
         series_transformers output) to extract that number of intervals.
         Valid str inputs are:
-            - "sqrt" : square root of the series length.
-            - "sqrt-div" : sqrt of series length divided by the number
+            - "sqrt": square root of the series length.
+            - "sqrt-div": sqrt of series length divided by the number
                 of series_transformers.
 
         A list or tuple of ints and/or strs will extract the number of intervals using
         the above rules and sum the results for the final n_intervals. i.e. [4, "sqrt"]
-        will extract sqrt(series_length) + 4 intervals.
+        will extract sqrt(n_timepoints) + 4 intervals.
 
         Different number of intervals for each series_transformers series can be
         specified using a nested list or tuple. Any list or tuple input containing
         another list or tuple must be the same length as the number of
         series_transformers.
 
-        %todo random vs supervised
+        While random interval extraction will extract the n_intervals intervals total
+        (removing duplicates), supervised intervals will run the supervised extraction
+        process n_intervals times, returning more intervals than specified.
     min_interval_length : int, float, list, or tuple, default=3
         Minimum length of intervals to extract from series. float inputs take a
         proportion of the series length to use as the minimum interval length.
 
         Different minimum interval lengths for each series_transformers series can be
         specified using a list or tuple. Any list or tuple input must be the same length
         as the number of series_transformers.
@@ -91,38 +86,50 @@
         proportion of the series length to use as the maximum interval length.
 
         Different maximum interval lengths for each series_transformers series can be
         specified using a list or tuple. Any list or tuple input must be the same length
         as the number of series_transformers.
 
         Ignored for supervised interval_selection_method inputs.
-    dilation:
-        todo
     interval_features : TransformerMixin, callable, list, tuple, or None, default=None
         The features to extract from the intervals using transformers or callable
-        functions. If None, uses the mean, standard deviation, and slope of the series.
+        functions. If None, use the mean, standard deviation, and slope of the series.
 
-        Both transformers and functions should be able to take a 2d np.ndarray input.
-        Functions should output a 1d array (the feature for each series) and
+        Both transformers and functions should be able to take a 2D np.ndarray input.
+        Functions should output a 1d array (the feature for each series), and
         transformers should output a 2d array where rows are the features for each
         series. A list or tuple of transformers and/or functions will extract all
         features and concatenate the output.
 
         Different features for each series_transformers series can be specified using a
         nested list or tuple. Any list or tuple input containing another list or tuple
         must be the same length as the number of series_transformers.
     series_transformers : TransformerMixin, list, tuple, or None, default=None
+        The transformers to apply to the series before extracting intervals. If None,
+        use the series as is.
 
-    att_subsample_size : int or None, default=None
-        Number of catch22 or summary statistic attributes to subsample per tree.
-    replace_nan :
-
+        A list or tuple of transformers will extract intervals from
+        all transformations concatenate the output. Including None in the list or tuple
+        will use the series as is for interval extraction.
+    att_subsample_size : int, float, list, tuple or None, default=None
+        The number of attributes to subsample for each estimator. If None, use all
+
+        If int, use that number of attributes for all estimators. If float, use that
+        proportion of attributes for all estimators.
+
+        Different subsample sizes for each series_transformers series can be specified
+        using a list or tuple. Any list or tuple input must be the same length as the
+        number of series_transformers.
+    replace_nan : "nan", int, float or None, default=None
+        The value to replace NaNs and infinite values with before fitting the base
+        estimator. int or float input will replace with the specified value, while
+        "nan" will replace infinite values with NaNs. If None, do not replace NaNs.
     time_limit_in_minutes : int, default=0
         Time contract to limit build time in minutes, overriding n_estimators.
-        Default of 0 means n_estimators is used.
+        Default of 0 means n_estimators are used.
     contract_max_n_estimators : int, default=500
         Max number of estimators when time_limit_in_minutes is set.
     save_transformed_data : bool, default=False
         Save the data transformed in fit for use in _get_train_probs.
     random_state : int, RandomState instance or None, default=None
         If `int`, random_state is the seed used by the random number generator;
         If `RandomState` instance, random_state is the random number generator;
@@ -137,49 +144,49 @@
         Valid options are "loky", "multiprocessing", "threading" or a custom backend.
         See the joblib Parallel documentation for more details.
 
     Attributes
     ----------
     n_instances_ : int
         The number of train cases.
-    n_dims_ : int
+    n_channels_ : int
         The number of channels per case.
-    series_length_ : int
+    n_timepoints_ : int
         The length of each series.
     total_intervals_ : int
         Total number of intervals per tree from all representations.
     estimators_ : list of shape (n_estimators) of BaseEstimator
         The collections of estimators trained in fit.
-    intervals_ : list of shape (n_estimators) of ndarray with shape (total_intervals,2)
-        Stores indexes of each intervals start and end points for all classifiers.
-    atts_ : list of shape (n_estimators) of array with shape (att_subsample_size)
-        Attribute indexes of the subsampled catch22 or summary statistic for all
-        classifiers.
+    intervals_ : list of shape (n_estimators) of TransformerMixin
+        Stores the interval extraction transformer for all estimators.
     transformed_data_ : list of shape (n_estimators) of ndarray with shape
-    (n_instances,total_intervals * att_subsample_size)
-        The transformed dataset for all classifiers. Only saved when
+    (n_instances_ ,total_intervals * att_subsample_size)
+        The transformed dataset for all estimators. Only saved when
         save_transformed_data is true.
 
     References
     ----------
-    .. [1]
-    .. [2]
-    .. [3]
+    .. [1] H.Deng, G.Runger, E.Tuv and M.Vladimir, "A time series forest for
+       classification and feature extraction", Information Sciences, 239, 2013
+    .. [2] Matthew Middlehurst and James Large and Anthony Bagnall. "The Canonical
+       Interval Forest (CIF) Classifier for Time Series Classification."
+       IEEE International Conference on Big Data 2020
+    .. [3] Cabello, Nestor, et al. "Fast and Accurate Time Series Classification
+       Through Supervised Interval Search." IEEE ICDM 2020
     """
 
     @abstractmethod
     def __init__(
         self,
         base_estimator=None,
         n_estimators=200,
         interval_selection_method="random",
         n_intervals="sqrt",
         min_interval_length=3,
         max_interval_length=np.inf,
-        dilation=None,
         interval_features=None,
         series_transformers=None,
         att_subsample_size=None,
         replace_nan=None,
         time_limit_in_minutes=None,
         contract_max_n_estimators=500,
         save_transformed_data=False,
@@ -189,71 +196,77 @@
     ):
         self.base_estimator = base_estimator
         self.n_estimators = n_estimators
         self.interval_selection_method = interval_selection_method
         self.n_intervals = n_intervals
         self.min_interval_length = min_interval_length
         self.max_interval_length = max_interval_length
-        self.dilation = dilation
         self.interval_features = interval_features
         self.series_transformers = series_transformers
         self.att_subsample_size = att_subsample_size
         self.replace_nan = replace_nan
         self.time_limit_in_minutes = time_limit_in_minutes
         self.contract_max_n_estimators = contract_max_n_estimators
         self.save_transformed_data = save_transformed_data
         self.random_state = random_state
         self.n_jobs = n_jobs
         self.parallel_backend = parallel_backend
 
+        super(BaseIntervalForest, self).__init__()
+
     # if subsampling attributes, an interval_features transformer must contain a
     # parameter name from transformer_feature_selection and an attribute name
     # (or property) from transformer_feature_names to allow features to be subsampled
     transformer_feature_selection = ["features"]
     transformer_feature_names = [
         "features_arguments_",
         "_features_arguments",
         "get_features_arguments",
         "_get_features_arguments",
     ]
     # an interval_features transformer must contain one of these attribute names to
     # be able to skip transforming features in predict
     transformer_feature_skip = ["transform_features_", "_transform_features"]
 
-    def fit(self, X, y):
+    def fit(self, X: Union[np.ndarray, List[np.ndarray]], y: np.ndarray) -> object:
+        """Fit the estimator to training data.
+
+        Parameters
+        ----------
+        X : 3D np.ndarray of shape (n_instances, n_channels, n_timepoints)
+            The training data.
+        y : 1D np.ndarray of shape (n_instances)
+            The target labels for fitting, indices correspond to instance indices in X
+
+        Returns
+        -------
+        self :
+            Reference to self.
+        """
         X, y = self._validate_data(X=X, y=y, ensure_min_samples=2)
         X = self._convert_X(X)
 
         rng = check_random_state(self.random_state)
 
-        self.n_instances_, self.n_dims_, self.series_length_ = X.shape
+        self.n_instances_, self.n_channels_, self.n_timepoints_ = X.shape
         if is_classifier(self):
             check_classification_targets(y)
 
             self.classes_ = np.unique(y)
             self.n_classes_ = self.classes_.shape[0]
             self.class_dictionary_ = {}
             for index, class_val in enumerate(self.classes_):
                 self.class_dictionary_[class_val] = index
 
             if self.n_classes_ == 1:
                 return self
 
         self._base_estimator = self.base_estimator
         if self.base_estimator is None:
-            from tsml.interval_based import RSTSFClassifier
-
-            # default base_estimators for classification and regression
-            if isinstance(self, RSTSFClassifier):
-                self._base_estimator = ExtraTreeClassifier(
-                    criterion="entropy",
-                    class_weight="balanced",
-                    max_features="sqrt",
-                )
-            elif is_classifier(self):
+            if is_classifier(self):
                 self._base_estimator = DecisionTreeClassifier(criterion="entropy")
             elif is_regressor(self):
                 self._base_estimator = DecisionTreeRegressor(criterion="absolute_error")
             else:
                 raise ValueError(
                     f"{self} must be a scikit-learn compatible classifier or "
                     "regressor."
@@ -285,18 +298,22 @@
                     Xt.append(X)
                     self._series_transformers.append(None)
                 elif is_transformer(transformer):
                     t = _clone_estimator(transformer, random_state=rng)
                     Xt.append(t.fit_transform(X, y))
                     self._series_transformers.append(t)
                 else:
-                    raise ValueError()  # todo error for invalid self.series_transformers
+                    raise ValueError(
+                        f"Invalid series_transformers list input. Found {transformer}"
+                    )
         # other inputs are invalid
         else:
-            raise ValueError()  # todo error for invalid self.series_transformers
+            raise ValueError(
+                f"Invalid series_transformers input. Found {self.series_transformers}"
+            )
 
         # if only a single n_intervals value is passed it must be an int or str
         if isinstance(self.n_intervals, (int, str)):
             n_intervals = [[self.n_intervals]] * len(Xt)
         elif isinstance(self.n_intervals, (list, tuple)):
             # if input is a list and only contains ints or strs, use the list for all
             # series in Xt
@@ -456,17 +473,14 @@
         # the series length
         for i, n in enumerate(self._max_interval_length):
             if n < self._min_interval_length[i]:
                 self._max_interval_length[i] = self._min_interval_length[i]
             elif n > Xt[i].shape[2]:
                 self._max_interval_length[i] = Xt[i].shape[2]
 
-        # todo dilation
-        self._dilation = [self.dilation] * len(Xt)
-
         # we store whether each series_transformer contains a transformer and/or
         # function in its interval_features
         self._interval_transformer = [False] * len(Xt)
         self._interval_function = [False] * len(Xt)
         # single transformer or function for all series_transformers
         if is_transformer(self.interval_features):
             self._interval_transformer = [True] * len(Xt)
@@ -478,15 +492,15 @@
         elif isinstance(self.interval_features, (list, tuple)):
             # if input is a list and only contains transformers or functions, use the
             # list for all series in Xt
             if all(
                 is_transformer(item) or callable(item)
                 for item in self.interval_features
             ):
-                for i, feature in enumerate(self.interval_features):
+                for feature in self.interval_features:
                     if is_transformer(feature):
                         self._interval_transformer[0] = True
                     elif callable(feature):
                         self._interval_function[0] = True
                 self._interval_features = [self.interval_features] * len(Xt)
             # other lists must be the same length as Xt
             elif len(self.interval_features) != len(Xt):
@@ -536,93 +550,121 @@
             raise ValueError(
                 f"Invalid interval_features input. Found {self.interval_features}"
             )
 
         # att_subsample_size must be at least one if it is an int
         if isinstance(self.att_subsample_size, int):
             if self.att_subsample_size < 1:
-                raise ValueError()  # todo error for invalid invalid self.att_subsample_size
+                raise ValueError(
+                    "att_subsample_size must be at least one if it is an int."
+                )
 
             self._att_subsample_size = [self.att_subsample_size] * len(Xt)
         # att_subsample_size must be at less than one if it is a float (proportion of
         # total attributed to subsample)
         elif isinstance(self.att_subsample_size, float):
-            if self.att_subsample_size > 1:
-                raise ValueError()  # todo error for invalid invalid self.att_subsample_size
+            if self.att_subsample_size > 1 or self.att_subsample_size <= 0:
+                raise ValueError(
+                    "att_subsample_size must be between 0 and 1 if it is a float."
+                )
 
             self._att_subsample_size = [self.att_subsample_size] * len(Xt)
         # default is no attribute subsampling with None
         elif self.att_subsample_size is None:
             self._att_subsample_size = [self.att_subsample_size] * len(Xt)
         # if the input is a list, it must be the same length as the number of
         # series_transformers
         # list values must be ints, floats or None. The same checks as above are
         # performed
         elif isinstance(self.att_subsample_size, (list, tuple)):
             if len(self.att_subsample_size) != len(Xt):
-                raise ValueError()  # todo error for invalid self.att_subsample_size
+                raise ValueError(
+                    "att_subsample_size as a list or tuple must be the same length as "
+                    "series_transformers."
+                )
 
             self._att_subsample_size = []
             for ssize in self.att_subsample_size:
                 if isinstance(ssize, int):
                     if ssize < 1:
-                        raise ValueError()  # todo error for invalid invalid self.att_subsample_size
+                        raise ValueError(
+                            "att_subsample_size in list must be at least one if it is "
+                            "an int."
+                        )
 
                     self._att_subsample_size.append(ssize)
                 elif isinstance(ssize, float):
                     if ssize > 1:
-                        raise ValueError()  # todo error for invalid invalid self.att_subsample_size
+                        raise ValueError(
+                            "att_subsample_size in list must be between 0 and 1 if it "
+                            "is a "
+                            "float."
+                        )
 
                     self._att_subsample_size.append(ssize)
                 elif ssize is None:
                     self._att_subsample_size.append(ssize)
                 else:
-                    raise ValueError()  # todo error for invalid self.att_subsample_size
+                    raise ValueError(
+                        "Invalid interval_features input in list. Found "
+                        f"{self.att_subsample_size}"
+                    )
         # other inputs are invalid
         else:
-            raise ValueError()  # todo error for invalid invalid self.att_subsample_size
+            raise ValueError(
+                f"Invalid interval_features input. Found {self.att_subsample_size}"
+            )
 
         # if we are subsampling attributes for a series_transformer and it uses a
         # BaseTransformer, we must ensure it has the required parameters and
         # attributes to do so
         self._transformer_feature_selection = [[]] * len(Xt)
         self._transformer_feature_names = [[]] * len(Xt)
         for r, att_subsample in enumerate(self._att_subsample_size):
             if att_subsample is not None:
                 for transformer in self._interval_features[r]:
                     if is_transformer(transformer):
                         params = inspect.signature(transformer.__init__).parameters
 
-                        # the BaseTransformer must have a parameter with one of the
+                        # the transformer must have a parameter with one of the
                         # names listed in transformer_feature_selection as a way to
                         # select which features the transformer should transform
                         has_params = False
                         for n in self.transformer_feature_selection:
                             if params.get(n, None) is not None:
                                 has_params = True
                                 self._transformer_feature_selection[r].append(n)
                                 break
 
                         if not has_params:
-                            raise ValueError()  # todo error for invalid invalid self.att_subsample_size
+                            raise ValueError(
+                                "All transformers in interval_features must have a "
+                                "parameter named in transformer_feature_selection to "
+                                "be used in attribute subsampling."
+                            )
 
-                        # the BaseTransformer must have an attribute with one of the
+                        # the transformer must have an attribute with one of the
                         # names listed in transformer_feature_names as a list or tuple
                         # of valid options for the previous parameter
                         has_feature_names = False
                         for n in self.transformer_feature_names:
                             if hasattr(transformer, n) and isinstance(
                                 getattr(transformer, n), (list, tuple)
                             ):
                                 has_feature_names = True
                                 self._transformer_feature_names[r].append(n)
                                 break
 
                         if not has_feature_names:
-                            raise ValueError()  # todo error for invalid invalid self.att_subsample_size
+                            raise ValueError(
+                                "All transformers in interval_features must have an "
+                                "attribute or propertynamed in "
+                                "transformer_feature_names to be used in attribute "
+                                "subsampling."
+                            )
 
         # verify the interval_selection_method is a valid string
         if isinstance(self.interval_selection_method, str):
             # SupervisedIntervals cannot currently handle transformers or regression
             if (
                 self.interval_selection_method.lower() == "supervised"
                 or self.interval_selection_method.lower() == "random-supervised"
@@ -655,22 +697,18 @@
 
         # verify replace_nan is a valid string, number or None
         if (
             (not isinstance(self.replace_nan, str) or self.replace_nan.lower() != "nan")
             and not isinstance(self.replace_nan, (int, float))
             and self.replace_nan is not None
         ):
-            raise ValueError()  # todo error for invalid self.replace_nan
+            raise ValueError(f"Invalid replace_nan input. Found {self.replace_nan}")
 
         self._n_jobs = check_n_jobs(self.n_jobs)
 
-        self._efficient_predictions = True  # todo
-        if not hasattr(self, "_test_flag"):
-            self._test_flag = False  # todo
-
         if self.time_limit_in_minutes is not None and self.time_limit_in_minutes > 0:
             time_limit = self.time_limit_in_minutes * 60
             start_time = time.time()
             train_time = 0
 
             self._n_estimators = 0
             self.estimators_ = []
@@ -685,17 +723,17 @@
                     n_jobs=self._n_jobs,
                     backend=self.parallel_backend,
                     prefer="threads",
                 )(
                     delayed(self._fit_estimator)(
                         Xt,
                         y,
-                        i,
+                        rng.randint(np.iinfo(np.int32).max),
                     )
-                    for i in range(self._n_jobs)
+                    for _ in range(self._n_jobs)
                 )
 
                 (
                     estimators,
                     intervals,
                     transformed_data,
                 ) = zip(*fit)
@@ -713,28 +751,40 @@
                 n_jobs=self._n_jobs,
                 backend=self.parallel_backend,
                 prefer="threads",
             )(
                 delayed(self._fit_estimator)(
                     Xt,
                     y,
-                    i,
+                    rng.randint(np.iinfo(np.int32).max),
                 )
-                for i in range(self._n_estimators)
+                for _ in range(self._n_estimators)
             )
 
             (
                 self.estimators_,
                 self.intervals_,
                 self.transformed_data_,
             ) = zip(*fit)
 
         return self
 
-    def predict(self, X):
+    def predict(self, X: Union[np.ndarray, List[np.ndarray]]) -> np.ndarray:
+        """Predicts labels for sequences in X.
+
+        Parameters
+        ----------
+        X : 3D np.ndarray of shape (n_instances, n_channels, n_timepoints)
+            The testing data.
+
+        Returns
+        -------
+        y : array-like of shape (n_instances)
+            Predicted target labels.
+        """
         if is_regressor(self):
             check_is_fitted(self)
 
             Xt = self._predict_setup(X)
 
             y_preds = Parallel(
                 n_jobs=self._n_jobs,
@@ -786,23 +836,17 @@
         )
 
         output = np.sum(y_probas, axis=0) / (
             np.ones(self.n_classes_) * self._n_estimators
         )
         return output
 
-    def _fit_estimator(self, Xt, y, i):
+    def _fit_estimator(self, Xt, y, seed):
         # random state for this estimator
-        rs = 255 if self.random_state == 0 else self.random_state
-        rs = (
-            None
-            if self.random_state is None
-            else (rs * 37 * (i + 1)) % np.iinfo(np.int32).max
-        )
-        rng = check_random_state(rs)
+        rng = check_random_state(seed)
 
         intervals = []
         transform_data_lengths = []
         interval_features = np.empty((self.n_instances_, 0))
 
         # for each transformed series
         for r in range(len(Xt)):
@@ -865,71 +909,71 @@
                                     self._transformer_feature_names[r][n],
                                 )[atts[count] + this_len - length]
                             )
                             count += 1
 
                         # tell this transformer to only transform the selected features
                         if len(t_features) > 0:
-                            new_transformer = _clone_estimator(transformer, rs)
+                            new_transformer = _clone_estimator(transformer, seed)
                             setattr(
                                 new_transformer,
                                 self._transformer_feature_selection[r][n],
                                 t_features,
                             )
                             features.append(new_transformer)
 
                     # subsample the remaining function features
                     for i in range(att_subsample_size - count):
                         features.append(all_function_features[atts[count + i] - length])
                 else:
                     warnings.warn(
-                        f"Attribute subsample size {att_subsample_size} is larger than or equal to the number of attributes {num_features} for series {self._series_transformers[r]}"
+                        f"Attribute subsample size {att_subsample_size} is larger than "
+                        f"or equal to the number of attributes {num_features} for "
+                        f"series {self._series_transformers[r]}",
+                        stacklevel=2,
                     )
                     for feature in self._interval_features[r]:
                         if is_transformer(feature):
-                            features.append(_clone_estimator(feature, rs))
+                            features.append(_clone_estimator(feature, seed))
                         else:
                             features.append(feature)
             # add all features while cloning estimators if not subsampling
             else:
                 features = []
                 for feature in self._interval_features[r]:
                     if is_transformer(feature):
-                        features.append(_clone_estimator(feature, rs))
+                        features.append(_clone_estimator(feature, seed))
                     else:
                         features.append(feature)
 
             # create the selected interval selector and set its parameters
             if self.interval_selection_method == "random":
                 selector = RandomIntervalTransformer(
                     n_intervals=self._n_intervals[r],
                     min_interval_length=self._min_interval_length[r],
                     max_interval_length=self._max_interval_length[r],
-                    dilation=self._dilation[r],
                     features=features,
-                    random_state=rs,
+                    random_state=seed,
                 )
             elif self.interval_selection_method == "supervised":
                 selector = SupervisedIntervalTransformer(
                     n_intervals=self._n_intervals[r],
                     min_interval_length=self._min_interval_length[r],
                     features=features,
                     randomised_split_point=False,
-                    random_state=rs,
+                    random_state=seed,
                 )
             elif self.interval_selection_method == "random-supervised":
                 selector = SupervisedIntervalTransformer(
                     n_intervals=self._n_intervals[r],
                     min_interval_length=self._min_interval_length[r],
                     features=features,
                     randomised_split_point=True,
-                    random_state=rs,
+                    random_state=seed,
                 )
-            else:
-                raise ValueError()  # todo error for invalid self.interval_selection_method, should not get here
 
             # fit the interval selector, transform the current series using it and save
             # the transformer
             intervals.append(selector)
             f = intervals[r].fit_transform(Xt[r], y)
 
             # concatenate the data and save this transforms number of attributes
@@ -946,74 +990,66 @@
                 False,
                 self.replace_nan,
                 self.replace_nan,
                 self.replace_nan,
             )
 
         # clone and fit the base estimator using the transformed data
-        tree = _clone_estimator(self._base_estimator, random_state=rs)
+        tree = _clone_estimator(self._base_estimator, random_state=seed)
         tree.fit(interval_features, y)
 
         # find the features used in the tree and inform the interval selectors to not
         # transform these features if possible
-        if not self._test_flag:
-            relevant_features = None
-            if isinstance(tree, BaseDecisionTree):
-                relevant_features = np.unique(
-                    tree.tree_.feature[tree.tree_.feature >= 0]
-                )
-            elif isinstance(tree, CITClassifier):
-                relevant_features, _ = tree.tree_node_splits_and_gain()
-
-            if relevant_features is not None:
-                features_to_transform = [False] * interval_features.shape[1]
-                for i in relevant_features:
-                    features_to_transform[i] = True
-
-                count = 0
-                for r in range(len(Xt)):
-                    intervals[
-                        r
-                    ].transformer_feature_skip = self.transformer_feature_skip
-
-                    # if the transformers don't have valid attributes to skip False is
-                    # returned
-                    completed = intervals[r].set_features_to_transform(
-                        features_to_transform[
-                            count : count + transform_data_lengths[r]
-                        ],
-                        raise_error=False,
-                    )
-                    count += transform_data_lengths[r]
+        self._efficient_predictions = True
+        relevant_features = None
+        if isinstance(tree, BaseDecisionTree):
+            relevant_features = np.unique(tree.tree_.feature[tree.tree_.feature >= 0])
+        elif isinstance(tree, CITClassifier):
+            relevant_features, _ = tree.tree_node_splits_and_gain()
+
+        if relevant_features is not None:
+            features_to_transform = [False] * interval_features.shape[1]
+            for i in relevant_features:
+                features_to_transform[i] = True
+
+            count = 0
+            for r in range(len(Xt)):
+                intervals[r].transformer_feature_skip = self.transformer_feature_skip
+
+                # if the transformers don't have valid attributes to skip False is
+                # returned
+                completed = intervals[r].set_features_to_transform(
+                    features_to_transform[count : count + transform_data_lengths[r]],
+                    raise_error=False,
+                )
+                count += transform_data_lengths[r]
 
-                    if not completed:
-                        self._efficient_predictions = False
-            else:
-                self._efficient_predictions = False
+                if not completed:
+                    self._efficient_predictions = False
         else:
             self._efficient_predictions = False
 
         return [
             tree,
             intervals,
             interval_features if self.save_transformed_data else None,
         ]
 
     def _predict_setup(self, X):
         X = self._validate_data(X=X, reset=False)
         X = self._convert_X(X)
 
-        n_instances, n_dims, series_length = X.shape
+        n_instances, n_channels, n_timepoints = X.shape
 
-        if n_dims != self.n_dims_:
+        if n_channels != self.n_channels_:
             raise ValueError(
                 "The number of channels in the train data does not match the number "
                 "of channels in the test data"
             )
-        if series_length != self.series_length_:
+        if n_timepoints != self.n_timepoints_:
             raise ValueError(
                 "The series length of the train data does not match the series length "
                 "of the test data"
             )
 
         Xt = []
         for transformer in self._series_transformers:
```

### Comparing `tsml-0.1.1/tsml/interval_based/_interval_pipelines.py` & `tsml-0.2.0/tsml/interval_based/_interval_forest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,634 +1,454 @@
-# -*- coding: utf-8 -*-
-"""Random Interval Classifier.
-
-Pipeline classifier using summary statistics extracted from random intervals and an
-estimator.
-"""
+"""Configurable interval forest estimators."""
 
 __author__ = ["MatthewMiddlehurst"]
-__all__ = [
-    "RandomIntervalClassifier",
-    "RandomIntervalRegressor",
-    "SupervisedIntervalClassifier",
-]
+__all__ = ["IntervalForestClassifier", "IntervalForestRegressor"]
+
+from typing import List, Union
 
 import numpy as np
 from sklearn.base import ClassifierMixin, RegressorMixin
-from sklearn.ensemble import RandomForestRegressor
-from sklearn.utils.validation import check_is_fitted
 
-from tsml.base import BaseTimeSeriesEstimator, _clone_estimator
-from tsml.transformations._catch22 import Catch22Transformer
-from tsml.transformations._interval_extraction import RandomIntervalTransformer
-from tsml.utils.validation import check_n_jobs
-from tsml.vector import RotationForestClassifier
+from tsml.interval_based._base import BaseIntervalForest
+
 
+class IntervalForestClassifier(ClassifierMixin, BaseIntervalForest):
+    """Configurable interval extracting forest classifier.
 
-class RandomIntervalClassifier(ClassifierMixin, BaseTimeSeriesEstimator):
-    """Random Interval Classifier.
+    Extracts multiple phase-dependent intervals from time series data and builds a
+    base classifier on summary statistic extracted from each interval. Forms and
+    ensemble of these classifiers.
 
-    This classifier simply transforms the input data using the RandomIntervals
-    transformer and builds a provided estimator using the transformed data.
+    Allows the implementation of classifiers along the lines of [1][2][3]
+    which extract intervals and create an ensemble from the subsequent features.
+
+    By default, uses a configuration similar to TimeSeriesFroest [1].
 
     Parameters
     ----------
-    n_intervals : int, default=100,
-        The number of intervals of random length, position and dimension to be
-        extracted.
-    interval_transformers : transformer or list of transformers, default=None,
-        Transformer(s) used to extract features from each interval. If None, defaults to
-        the Catch22 transformer.
-    estimator : sklearn classifier, default=None
-        An sklearn estimator to be built using the transformed data. Defaults to a
-        Rotation Forest with 200 trees.
+    base_estimator : BaseEstimator or None, default=None
+        scikit-learn BaseEstimator used to build the interval ensemble. If None, use a
+        simple decision tree.
+    n_estimators : int, default=200
+        Number of estimators to build for the ensemble.
+    interval_selection_method : "random", "supervised" or "random-supervised",
+            default="random"
+        The interval selection transformer to use.
+            - "random" uses a RandomIntervalTransformer.
+            - "supervised" uses a SupervisedIntervalTransformer.
+            - "random-supervised" uses a SupervisedIntervalTransformer with
+                randomised elements.
+    n_intervals : int, str, list or tuple, default="sqrt"
+        Number of intervals to extract per tree for each series_transformers series.
+
+        An int input will extract that number of intervals from the series, while a str
+        input will return a function of the series length (may differ per
+        series_transformers output) to extract that number of intervals.
+        Valid str inputs are:
+            - "sqrt": square root of the series length.
+            - "sqrt-div": sqrt of series length divided by the number
+                of series_transformers.
+
+        A list or tuple of ints and/or strs will extract the number of intervals using
+        the above rules and sum the results for the final n_intervals. i.e. [4, "sqrt"]
+        will extract sqrt(n_timepoints) + 4 intervals.
+
+        Different number of intervals for each series_transformers series can be
+        specified using a nested list or tuple. Any list or tuple input containing
+        another list or tuple must be the same length as the number of
+        series_transformers.
+
+        While random interval extraction will extract the n_intervals intervals total
+        (removing duplicates), supervised intervals will run the supervised extraction
+        process n_intervals times, returning more intervals than specified.
+    min_interval_length : int, float, list, or tuple, default=3
+        Minimum length of intervals to extract from series. float inputs take a
+        proportion of the series length to use as the minimum interval length.
+
+        Different minimum interval lengths for each series_transformers series can be
+        specified using a list or tuple. Any list or tuple input must be the same length
+        as the number of series_transformers.
+    max_interval_length : int, float, list, or tuple, default=np.inf
+        Maximum length of intervals to extract from series. float inputs take a
+        proportion of the series length to use as the maximum interval length.
+
+        Different maximum interval lengths for each series_transformers series can be
+        specified using a list or tuple. Any list or tuple input must be the same length
+        as the number of series_transformers.
+
+        Ignored for supervised interval_selection_method inputs.
+    interval_features : TransformerMixin, callable, list, tuple, or None, default=None
+        The features to extract from the intervals using transformers or callable
+        functions. If None, use the mean, standard deviation, and slope of the series.
+
+        Both transformers and functions should be able to take a 2D np.ndarray input.
+        Functions should output a 1d array (the feature for each series), and
+        transformers should output a 2d array where rows are the features for each
+        series. A list or tuple of transformers and/or functions will extract all
+        features and concatenate the output.
+
+        Different features for each series_transformers series can be specified using a
+        nested list or tuple. Any list or tuple input containing another list or tuple
+        must be the same length as the number of series_transformers.
+    series_transformers : TransformerMixin, list, tuple, or None, default=None
+        The transformers to apply to the series before extracting intervals. If None,
+        use the series as is.
+
+        A list or tuple of transformers will extract intervals from
+        all transformations concatenate the output. Including None in the list or tuple
+        will use the series as is for interval extraction.
+    att_subsample_size : int, float, list, tuple or None, default=None
+        The number of attributes to subsample for each estimator. If None, use all
+
+        If int, use that number of attributes for all estimators. If float, use that
+        proportion of attributes for all estimators.
+
+        Different subsample sizes for each series_transformers series can be specified
+        using a list or tuple. Any list or tuple input must be the same length as the
+        number of series_transformers.
+    replace_nan : "nan", int, float or None, default=None
+        The value to replace NaNs and infinite values with before fitting the base
+        estimator. int or float input will replace with the specified value, while
+        "nan" will replace infinite values with NaNs. If None, do not replace NaNs.
+    time_limit_in_minutes : int, default=0
+        Time contract to limit build time in minutes, overriding n_estimators.
+        Default of 0 means n_estimators are used.
+    contract_max_n_estimators : int, default=500
+        Max number of estimators when time_limit_in_minutes is set.
+    save_transformed_data : bool, default=False
+        Save the data transformed in fit for use in _get_train_probs.
+    random_state : int, RandomState instance or None, default=None
+        If `int`, random_state is the seed used by the random number generator;
+        If `RandomState` instance, random_state is the random number generator;
+        If `None`, the random number generator is the `RandomState` instance used
+        by `np.random`.
     n_jobs : int, default=1
         The number of jobs to run in parallel for both `fit` and `predict`.
         ``-1`` means using all processors.
-    random_state : int or None, default=None
-        Seed for random, integer.
+    parallel_backend : str, ParallelBackendBase instance or None, default=None
+        Specify the parallelisation backend implementation in joblib, if None a 'prefer'
+        value of "threads" is used by default.
+        Valid options are "loky", "multiprocessing", "threading" or a custom backend.
+        See the joblib Parallel documentation for more details.
 
     Attributes
     ----------
+    n_instances_ : int
+        The number of train cases in the training set.
+    n_channels_ : int
+        The number of dimensions per case in the training set.
+    n_timepoints_ : int
+        The length of each series in the training set.
     n_classes_ : int
         Number of classes. Extracted from the data.
-    classes_ : ndarray of shape (n_classes)
+    classes_ : ndarray of shape (n_classes_)
         Holds the label for each class.
+    class_dictionary_ : dict
+        A dictionary mapping class labels to class indices in classes_.
+    total_intervals_ : int
+        Total number of intervals per tree from all representations.
+    estimators_ : list of shape (n_estimators) of BaseEstimator
+        The collections of estimators trained in fit.
+    intervals_ : list of shape (n_estimators) of TransformerMixin
+        Stores the interval extraction transformer for all estimators.
+    transformed_data_ : list of shape (n_estimators) of ndarray with shape
+    (n_instances_ ,total_intervals * att_subsample_size)
+        The transformed dataset for all estimators. Only saved when
+        save_transformed_data is true.
+
+    References
+    ----------
+    .. [1] H.Deng, G.Runger, E.Tuv and M.Vladimir, "A time series forest for
+       classification and feature extraction", Information Sciences, 239, 2013
+    .. [2] Matthew Middlehurst and James Large and Anthony Bagnall. "The Canonical
+       Interval Forest (CIF) Classifier for Time Series Classification."
+       IEEE International Conference on Big Data 2020
+    .. [3] Cabello, Nestor, et al. "Fast and Accurate Time Series Classification
+       Through Supervised Interval Search." IEEE ICDM 2020
 
-    See Also
+    Examples
     --------
-    RandomIntervals
+    >>> from tsml.interval_based import IntervalForestClassifier
+    >>> from tsml.utils.testing import generate_3d_test_data
+    >>> X, y = generate_3d_test_data(n_samples=10, series_length=12, random_state=0)
+    >>> clf = IntervalForestClassifier(n_estimators=10, random_state=0)
+    >>> clf.fit(X, y)
+    IntervalForestClassifier(...)
+    >>> clf.predict(X)
+    array([0, 1, 0, 1, 0, 0, 1, 1, 1, 0])
     """
 
     def __init__(
         self,
-        n_intervals=100,
-        interval_transformers=None,
-        estimator=None,
-        n_jobs=1,
+        base_estimator=None,
+        n_estimators=200,
+        interval_selection_method="random",
+        n_intervals="sqrt",
+        min_interval_length=3,
+        max_interval_length=np.inf,
+        interval_features=None,
+        series_transformers=None,
+        att_subsample_size=None,
+        replace_nan=None,
+        time_limit_in_minutes=None,
+        contract_max_n_estimators=500,
+        save_transformed_data=False,
         random_state=None,
+        n_jobs=1,
+        parallel_backend=None,
     ):
-        self.n_intervals = n_intervals
-        self.interval_transformers = interval_transformers
-        self.estimator = estimator
-
-        self.n_jobs = n_jobs
-        self.random_state = random_state
-
-        super(RandomIntervalClassifier, self).__init__()
-
-    def fit(self, X, y):
-        """Fit a pipeline on cases (X,y), where y is the target variable.
-
-        Parameters
-        ----------
-        X : 3D np.array of shape = [n_instances, n_dimensions, series_length]
-            The training data.
-        y : array-like, shape = [n_instances]
-            The class labels.
-
-        Returns
-        -------
-        self :
-            Reference to self.
-
-        Notes
-        -----
-        Changes state by creating a fitted model that updates attributes
-        ending in "_" and sets is_fitted flag to True.
-        """
-        X, y = self._validate_data(
-            X=X, y=y, ensure_min_samples=2, ensure_min_series_length=3
-        )
-        X = self._convert_X(X)
-
-        self.n_instances_, self.n_dims_, self.series_length_ = X.shape
-        self.classes_ = np.unique(y)
-        self.n_classes_ = self.classes_.shape[0]
-        self.class_dictionary_ = {}
-        for index, class_val in enumerate(self.classes_):
-            self.class_dictionary_[class_val] = index
-
-        self._n_jobs = check_n_jobs(self.n_jobs)
-
-        interval_transformers = (
-            Catch22Transformer(catch24=True, outlier_norm=True, replace_nans=True)
-            if self.interval_transformers is None
-            else self.interval_transformers
+        super(IntervalForestClassifier, self).__init__(
+            base_estimator=base_estimator,
+            n_estimators=n_estimators,
+            interval_selection_method=interval_selection_method,
+            n_intervals=n_intervals,
+            min_interval_length=min_interval_length,
+            max_interval_length=max_interval_length,
+            interval_features=interval_features,
+            series_transformers=series_transformers,
+            att_subsample_size=att_subsample_size,
+            replace_nan=replace_nan,
+            time_limit_in_minutes=time_limit_in_minutes,
+            contract_max_n_estimators=contract_max_n_estimators,
+            save_transformed_data=save_transformed_data,
+            random_state=random_state,
+            n_jobs=n_jobs,
+            parallel_backend=parallel_backend,
         )
 
-        self._transformer = RandomIntervalTransformer(
-            n_intervals=self.n_intervals,
-            features=interval_transformers,
-            random_state=self.random_state,
-            n_jobs=self._n_jobs,
-        )
-
-        self._estimator = _clone_estimator(
-            RotationForestClassifier() if self.estimator is None else self.estimator,
-            self.random_state,
-        )
-
-        m = getattr(self._estimator, "n_jobs", None)
-        if m is not None:
-            self._estimator.n_jobs = self._n_jobs
-
-        X_t = self._transformer.fit_transform(X, y)
-        self._estimator.fit(X_t, y)
-
-        return self
-
-    def predict(self, X) -> np.ndarray:
-        """Predict class values of n instances in X.
-
-        Parameters
-        ----------
-        X : 3D np.array of shape = [n_instances, n_dimensions, series_length]
-            The data to make predictions for.
-
-        Returns
-        -------
-        y : array-like, shape = [n_instances]
-            Predicted class labels.
-        """
-        check_is_fitted(self)
-
-        X = self._validate_data(X=X, reset=False, ensure_min_series_length=3)
-        X = self._convert_X(X)
-
-        return self._estimator.predict(self._transformer.transform(X))
-
-    def predict_proba(self, X) -> np.ndarray:
-        """Predict class probabilities for n instances in X.
-
-        Parameters
-        ----------
-        X : 3D np.array of shape = [n_instances, n_dimensions, series_length]
-            The data to make predict probabilities for.
-
-        Returns
-        -------
-        y : array-like, shape = [n_instances, n_classes_]
-            Predicted probabilities using the ordering in classes_.
-        """
-        check_is_fitted(self)
-
-        X = self._validate_data(X=X, reset=False, ensure_min_series_length=3)
-        X = self._convert_X(X)
-
-        m = getattr(self._estimator, "predict_proba", None)
-        if callable(m):
-            return self._estimator.predict_proba(self._transformer.transform(X))
-        else:
-            dists = np.zeros((X.shape[0], self.n_classes_))
-            preds = self._estimator.predict(self._transformer.transform(X))
-            for i in range(0, X.shape[0]):
-                dists[i, self.class_dictionary_[preds[i]]] = 1
-            return dists
+    def predict_proba(self, X):
+        return self._predict_proba(X)
 
     @classmethod
-    def get_test_params(cls, parameter_set="default"):
-        """Return testing parameter settings for the estimator.
+    def get_test_params(
+        cls, parameter_set: Union[str, None] = None
+    ) -> Union[dict, List[dict]]:
+        """Return unit test parameter settings for the estimator.
 
         Parameters
         ----------
-        parameter_set : str, default="default"
+        parameter_set : None or str, default=None
             Name of the set of test parameters to return, for use in tests. If no
             special parameters are defined for a value, will return `"default"` set.
-            For classifiers, a "default" set of parameters should be provided for
-            general testing, and a "results_comparison" set for comparing against
-            previously recorded results if the general set does not produce suitable
-            probabilities to compare against.
 
         Returns
         -------
-        params : dict or list of dict, default={}
+        params : dict or list of dict
             Parameters to create testing instances of the class.
-            Each dict are parameters to construct an "interesting" test instance, i.e.,
-            `MyClass(**params)` or `MyClass(**params[i])` creates a valid test instance.
-            `create_test_instance` uses the first (or only) dictionary in `params`.
         """
-        from sklearn.ensemble import RandomForestClassifier
+        return {
+            "n_estimators": 2,
+            "n_intervals": 2,
+        }
+
 
-        if parameter_set == "results_comparison":
-            return {
-                "n_intervals": 5,
-                "estimator": RandomForestClassifier(n_estimators=10),
-                "interval_transformers": Catch22Transformer(
-                    catch24=True,
-                    replace_nans=True,
-                    features=(
-                        "Mean",
-                        "DN_HistogramMode_5",
-                        "SB_BinaryStats_mean_longstretch1",
-                    ),
-                ),
-            }
-        else:
-            return {
-                "n_intervals": 3,
-                "estimator": RandomForestClassifier(n_estimators=2),
-                "interval_transformers": Catch22Transformer(
-                    catch24=True,
-                    replace_nans=True,
-                    features=(
-                        "Mean",
-                        "DN_HistogramMode_5",
-                        "SB_BinaryStats_mean_longstretch1",
-                    ),
-                ),
-            }
+class IntervalForestRegressor(RegressorMixin, BaseIntervalForest):
+    """Configurable interval extracting forest regressor.
 
+    Extracts multiple phase-dependent intervals from time series data and builds a
+    base regressor on summary statistic extracted from each interval. Forms and
+    ensemble of these regressors.
 
-class RandomIntervalRegressor(RegressorMixin, BaseTimeSeriesEstimator):
-    """Random Interval Classifier.
+    Allows the implementation of regressors along the lines of [1][2][3]
+    which extract intervals and create an ensemble from the subsequent features.
 
-    This classifier simply transforms the input data using the RandomIntervals
-    transformer and builds a provided estimator using the transformed data.
+    By default, uses a configuration similar to TimeSeriesFroest [1].
 
     Parameters
     ----------
-    n_intervals : int, default=100,
-        The number of intervals of random length, position and dimension to be
-        extracted.
-    interval_transformers : transformer or list of transformers, default=None,
-        Transformer(s) used to extract features from each interval. If None, defaults to
-        the Catch22 transformer.
-    estimator : sklearn classifier, default=None
-        An sklearn estimator to be built using the transformed data. Defaults to a
-        Rotation Forest with 200 trees.
+    base_estimator : BaseEstimator or None, default=None
+        scikit-learn BaseEstimator used to build the interval ensemble. If None, use a
+        simple decision tree.
+    n_estimators : int, default=200
+        Number of estimators to build for the ensemble.
+    interval_selection_method : "random", default="random"
+        The interval selection transformer to use.
+            - "random" uses a RandomIntervalTransformer.
+    n_intervals : int, str, list or tuple, default="sqrt"
+        Number of intervals to extract per tree for each series_transformers series.
+
+        An int input will extract that number of intervals from the series, while a str
+        input will return a function of the series length (may differ per
+        series_transformers output) to extract that number of intervals.
+        Valid str inputs are:
+            - "sqrt": square root of the series length.
+            - "sqrt-div": sqrt of series length divided by the number
+                of series_transformers.
+
+        A list or tuple of ints and/or strs will extract the number of intervals using
+        the above rules and sum the results for the final n_intervals. i.e. [4, "sqrt"]
+        will extract sqrt(n_timepoints) + 4 intervals.
+
+        Different number of intervals for each series_transformers series can be
+        specified using a nested list or tuple. Any list or tuple input containing
+        another list or tuple must be the same length as the number of
+        series_transformers.
+    min_interval_length : int, float, list, or tuple, default=3
+        Minimum length of intervals to extract from series. float inputs take a
+        proportion of the series length to use as the minimum interval length.
+
+        Different minimum interval lengths for each series_transformers series can be
+        specified using a list or tuple. Any list or tuple input must be the same length
+        as the number of series_transformers.
+    max_interval_length : int, float, list, or tuple, default=np.inf
+        Maximum length of intervals to extract from series. float inputs take a
+        proportion of the series length to use as the maximum interval length.
+
+        Different maximum interval lengths for each series_transformers series can be
+        specified using a list or tuple. Any list or tuple input must be the same length
+        as the number of series_transformers.
+    interval_features : TransformerMixin, callable, list, tuple, or None, default=None
+        The features to extract from the intervals using transformers or callable
+        functions. If None, use the mean, standard deviation, and slope of the series.
+
+        Both transformers and functions should be able to take a 2D np.ndarray input.
+        Functions should output a 1d array (the feature for each series), and
+        transformers should output a 2d array where rows are the features for each
+        series. A list or tuple of transformers and/or functions will extract all
+        features and concatenate the output.
+
+        Different features for each series_transformers series can be specified using a
+        nested list or tuple. Any list or tuple input containing another list or tuple
+        must be the same length as the number of series_transformers.
+    series_transformers : TransformerMixin, list, tuple, or None, default=None
+        The transformers to apply to the series before extracting intervals. If None,
+        use the series as is.
+
+        A list or tuple of transformers will extract intervals from
+        all transformations concatenate the output. Including None in the list or tuple
+        will use the series as is for interval extraction.
+    att_subsample_size : int, float, list, tuple or None, default=None
+        The number of attributes to subsample for each estimator. If None, use all
+
+        If int, use that number of attributes for all estimators. If float, use that
+        proportion of attributes for all estimators.
+
+        Different subsample sizes for each series_transformers series can be specified
+        using a list or tuple. Any list or tuple input must be the same length as the
+        number of series_transformers.
+    replace_nan : "nan", int, float or None, default=None
+        The value to replace NaNs and infinite values with before fitting the base
+        estimator. int or float input will replace with the specified value, while
+        "nan" will replace infinite values with NaNs. If None, do not replace NaNs.
+    time_limit_in_minutes : int, default=0
+        Time contract to limit build time in minutes, overriding n_estimators.
+        Default of 0 means n_estimators are used.
+    contract_max_n_estimators : int, default=500
+        Max number of estimators when time_limit_in_minutes is set.
+    save_transformed_data : bool, default=False
+        Save the data transformed in fit for use in _get_train_probs.
+    random_state : int, RandomState instance or None, default=None
+        If `int`, random_state is the seed used by the random number generator;
+        If `RandomState` instance, random_state is the random number generator;
+        If `None`, the random number generator is the `RandomState` instance used
+        by `np.random`.
     n_jobs : int, default=1
         The number of jobs to run in parallel for both `fit` and `predict`.
         ``-1`` means using all processors.
-    random_state : int or None, default=None
-        Seed for random, integer.
+    parallel_backend : str, ParallelBackendBase instance or None, default=None
+        Specify the parallelisation backend implementation in joblib, if None a 'prefer'
+        value of "threads" is used by default.
+        Valid options are "loky", "multiprocessing", "threading" or a custom backend.
+        See the joblib Parallel documentation for more details.
 
     Attributes
     ----------
-    n_classes_ : int
-        Number of classes. Extracted from the data.
-    classes_ : ndarray of shape (n_classes)
-        Holds the label for each class.
-
-    See Also
-    --------
-    RandomIntervals
-    """
-
-    def __init__(
-        self,
-        n_intervals=100,
-        interval_transformers=None,
-        estimator=None,
-        n_jobs=1,
-        random_state=None,
-    ):
-        self.n_intervals = n_intervals
-        self.interval_transformers = interval_transformers
-        self.estimator = estimator
-
-        self.n_jobs = n_jobs
-        self.random_state = random_state
-
-        super(RandomIntervalRegressor, self).__init__()
-
-    def fit(self, X, y):
-        """Fit a pipeline on cases (X,y), where y is the target variable.
-
-        Parameters
-        ----------
-        X : 3D np.array of shape = [n_instances, n_dimensions, series_length]
-            The training data.
-        y : array-like, shape = [n_instances]
-            The class labels.
-
-        Returns
-        -------
-        self :
-            Reference to self.
-
-        Notes
-        -----
-        Changes state by creating a fitted model that updates attributes
-        ending in "_" and sets is_fitted flag to True.
-        """
-        X, y = self._validate_data(
-            X=X, y=y, ensure_min_samples=2, ensure_min_series_length=3
-        )
-        X = self._convert_X(X)
-
-        self.n_instances_, self.n_dims_, self.series_length_ = X.shape
-
-        self._n_jobs = check_n_jobs(self.n_jobs)
-
-        interval_transformers = (
-            Catch22Transformer(catch24=True, outlier_norm=True, replace_nans=True)
-            if self.interval_transformers is None
-            else self.interval_transformers
-        )
-
-        self._transformer = RandomIntervalTransformer(
-            n_intervals=self.n_intervals,
-            features=interval_transformers,
-            random_state=self.random_state,
-            n_jobs=self._n_jobs,
-        )
-
-        self._estimator = _clone_estimator(
-            RandomForestRegressor() if self.estimator is None else self.estimator,
-            self.random_state,
-        )
-
-        m = getattr(self._estimator, "n_jobs", None)
-        if m is not None:
-            self._estimator.n_jobs = self._n_jobs
+    n_instances_ : int
+        The number of train cases in the training set.
+    n_channels_ : int
+        The number of dimensions per case in the training set.
+    n_timepoints_ : int
+        The length of each series in the training set.
+    total_intervals_ : int
+        Total number of intervals per tree from all representations.
+    estimators_ : list of shape (n_estimators) of BaseEstimator
+        The collections of estimators trained in fit.
+    intervals_ : list of shape (n_estimators) of TransformerMixin
+        Stores the interval extraction transformer for all estimators.
+    transformed_data_ : list of shape (n_estimators) of ndarray with shape
+    (n_instances_ ,total_intervals * att_subsample_size)
+        The transformed dataset for all estimators. Only saved when
+        save_transformed_data is true.
 
-        X_t = self._transformer.fit_transform(X, y)
-        self._estimator.fit(X_t, y)
-
-        return self
-
-    def predict(self, X) -> np.ndarray:
-        """Predict class values of n instances in X.
-
-        Parameters
-        ----------
-        X : 3D np.array of shape = [n_instances, n_dimensions, series_length]
-            The data to make predictions for.
-
-        Returns
-        -------
-        y : array-like, shape = [n_instances]
-            Predicted class labels.
-        """
-        check_is_fitted(self)
-
-        X = self._validate_data(X=X, reset=False, ensure_min_series_length=3)
-        X = self._convert_X(X)
-
-        return self._estimator.predict(self._transformer.transform(X))
-
-    @classmethod
-    def get_test_params(cls, parameter_set="default"):
-        """Return testing parameter settings for the estimator.
-
-        Parameters
-        ----------
-        parameter_set : str, default="default"
-            Name of the set of test parameters to return, for use in tests. If no
-            special parameters are defined for a value, will return `"default"` set.
-            For classifiers, a "default" set of parameters should be provided for
-            general testing, and a "results_comparison" set for comparing against
-            previously recorded results if the general set does not produce suitable
-            probabilities to compare against.
-
-        Returns
-        -------
-        params : dict or list of dict, default={}
-            Parameters to create testing instances of the class.
-            Each dict are parameters to construct an "interesting" test instance, i.e.,
-            `MyClass(**params)` or `MyClass(**params[i])` creates a valid test instance.
-            `create_test_instance` uses the first (or only) dictionary in `params`.
-        """
-        if parameter_set == "results_comparison":
-            return {
-                "n_intervals": 5,
-                "estimator": RandomForestRegressor(n_estimators=10),
-                "interval_transformers": Catch22Transformer(
-                    catch24=True,
-                    replace_nans=True,
-                    features=(
-                        "Mean",
-                        "DN_HistogramMode_5",
-                        "SB_BinaryStats_mean_longstretch1",
-                    ),
-                ),
-            }
-        else:
-            return {
-                "n_intervals": 3,
-                "estimator": RandomForestRegressor(n_estimators=2),
-                "interval_transformers": Catch22Transformer(
-                    catch24=True,
-                    replace_nans=True,
-                    features=(
-                        "Mean",
-                        "DN_HistogramMode_5",
-                        "SB_BinaryStats_mean_longstretch1",
-                    ),
-                ),
-            }
-
-
-class SupervisedIntervalClassifier(ClassifierMixin, BaseTimeSeriesEstimator):
-    """Random Interval Classifier.
-
-    This classifier simply transforms the input data using the RandomIntervals
-    transformer and builds a provided estimator using the transformed data.
-
-    Parameters
-    ----------
-    n_intervals : int, default=100,
-        The number of intervals of random length, position and dimension to be
-        extracted.
-    interval_transformers : transformer or list of transformers, default=None,
-        Transformer(s) used to extract features from each interval. If None, defaults to
-        the Catch22 transformer.
-    estimator : sklearn classifier, default=None
-        An sklearn estimator to be built using the transformed data. Defaults to a
-        Rotation Forest with 200 trees.
-    n_jobs : int, default=1
-        The number of jobs to run in parallel for both `fit` and `predict`.
-        ``-1`` means using all processors.
-    random_state : int or None, default=None
-        Seed for random, integer.
-
-    Attributes
+    References
     ----------
-    n_classes_ : int
-        Number of classes. Extracted from the data.
-    classes_ : ndarray of shape (n_classes)
-        Holds the label for each class.
+    .. [1] H.Deng, G.Runger, E.Tuv and M.Vladimir, "A time series forest for
+       classification and feature extraction", Information Sciences, 239, 2013
+    .. [2] Matthew Middlehurst and James Large and Anthony Bagnall. "The Canonical
+       Interval Forest (CIF) Classifier for Time Series Classification."
+       IEEE International Conference on Big Data 2020
+    .. [3] Cabello, Nestor, et al. "Fast and Accurate Time Series Classification
+       Through Supervised Interval Search." IEEE ICDM 2020
 
-    See Also
+    Examples
     --------
-    RandomIntervals
+    >>> from tsml.interval_based import IntervalForestRegressor
+    >>> from tsml.utils.testing import generate_3d_test_data
+    >>> X, y = generate_3d_test_data(n_samples=10, series_length=12,
+    ...                              regression_target=True, random_state=0)
+    >>> reg = IntervalForestRegressor(n_estimators=10, random_state=0)
+    >>> reg.fit(X, y)
+    IntervalForestRegressor(...)
+    >>> reg.predict(X)
+    array([0.7252543 , 1.50132442, 0.95608366, 1.64399016, 0.42385504,
+           0.60639322, 1.01919317, 1.30157483, 1.66017354, 0.2900776 ])
     """
 
     def __init__(
         self,
-        n_intervals=50,
-        interval_transformers=None,
-        estimator=None,
-        n_jobs=1,
+        base_estimator=None,
+        n_estimators=200,
+        interval_selection_method="random",
+        n_intervals="sqrt",
+        min_interval_length=3,
+        max_interval_length=np.inf,
+        interval_features=None,
+        series_transformers=None,
+        att_subsample_size=None,
+        replace_nan=None,
+        time_limit_in_minutes=None,
+        contract_max_n_estimators=500,
+        save_transformed_data=False,
         random_state=None,
+        n_jobs=1,
+        parallel_backend=None,
     ):
-        self.n_intervals = n_intervals
-        self.interval_transformers = interval_transformers
-        self.estimator = estimator
-
-        self.n_jobs = n_jobs
-        self.random_state = random_state
-
-        super(SupervisedIntervalClassifier, self).__init__()
-
-    def fit(self, X, y):
-        """Fit a pipeline on cases (X,y), where y is the target variable.
-
-        Parameters
-        ----------
-        X : 3D np.array of shape = [n_instances, n_dimensions, series_length]
-            The training data.
-        y : array-like, shape = [n_instances]
-            The class labels.
-
-        Returns
-        -------
-        self :
-            Reference to self.
-
-        Notes
-        -----
-        Changes state by creating a fitted model that updates attributes
-        ending in "_" and sets is_fitted flag to True.
-        """
-        X, y = self._validate_data(
-            X=X, y=y, ensure_min_samples=2, ensure_min_series_length=7
+        super(IntervalForestRegressor, self).__init__(
+            base_estimator=base_estimator,
+            n_estimators=n_estimators,
+            interval_selection_method=interval_selection_method,
+            n_intervals=n_intervals,
+            min_interval_length=min_interval_length,
+            max_interval_length=max_interval_length,
+            interval_features=interval_features,
+            series_transformers=series_transformers,
+            att_subsample_size=att_subsample_size,
+            replace_nan=replace_nan,
+            time_limit_in_minutes=time_limit_in_minutes,
+            contract_max_n_estimators=contract_max_n_estimators,
+            save_transformed_data=save_transformed_data,
+            random_state=random_state,
+            n_jobs=n_jobs,
+            parallel_backend=parallel_backend,
         )
-        X = self._convert_X(X)
-
-        self.n_instances_, self.n_dims_, self.series_length_ = X.shape
-        self.classes_ = np.unique(y)
-        self.n_classes_ = self.classes_.shape[0]
-        self.class_dictionary_ = {}
-        for index, class_val in enumerate(self.classes_):
-            self.class_dictionary_[class_val] = index
-
-        self._n_jobs = check_n_jobs(self.n_jobs)
-
-        interval_transformers = (
-            Catch22Transformer(catch24=True, outlier_norm=True, replace_nans=True)
-            if self.interval_transformers is None
-            else self.interval_transformers
-        )
-
-        self._transformer = RandomIntervalTransformer(
-            n_intervals=self.n_intervals,
-            features=interval_transformers,
-            random_state=self.random_state,
-            n_jobs=self._n_jobs,
-        )
-
-        self._estimator = _clone_estimator(
-            RotationForestClassifier() if self.estimator is None else self.estimator,
-            self.random_state,
-        )
-
-        m = getattr(self._estimator, "n_jobs", None)
-        if m is not None:
-            self._estimator.n_jobs = self._n_jobs
-
-        X_t = self._transformer.fit_transform(X, y)
-        self._estimator.fit(X_t, y)
-
-        return self
-
-    def predict(self, X) -> np.ndarray:
-        """Predict class values of n instances in X.
-
-        Parameters
-        ----------
-        X : 3D np.array of shape = [n_instances, n_dimensions, series_length]
-            The data to make predictions for.
-
-        Returns
-        -------
-        y : array-like, shape = [n_instances]
-            Predicted class labels.
-        """
-        check_is_fitted(self)
-
-        X = self._validate_data(X=X, reset=False, ensure_min_series_length=7)
-        X = self._convert_X(X)
-
-        return self._estimator.predict(self._transformer.transform(X))
-
-    def predict_proba(self, X) -> np.ndarray:
-        """Predict class probabilities for n instances in X.
-
-        Parameters
-        ----------
-        X : 3D np.array of shape = [n_instances, n_dimensions, series_length]
-            The data to make predict probabilities for.
-
-        Returns
-        -------
-        y : array-like, shape = [n_instances, n_classes_]
-            Predicted probabilities using the ordering in classes_.
-        """
-        check_is_fitted(self)
-
-        X = self._validate_data(X=X, reset=False, ensure_min_series_length=7)
-        X = self._convert_X(X)
-
-        m = getattr(self._estimator, "predict_proba", None)
-        if callable(m):
-            return self._estimator.predict_proba(self._transformer.transform(X))
-        else:
-            dists = np.zeros((X.shape[0], self.n_classes_))
-            preds = self._estimator.predict(self._transformer.transform(X))
-            for i in range(0, X.shape[0]):
-                dists[i, self.class_dictionary_[preds[i]]] = 1
-            return dists
 
     @classmethod
-    def get_test_params(cls, parameter_set="default"):
-        """Return testing parameter settings for the estimator.
+    def get_test_params(
+        cls, parameter_set: Union[str, None] = None
+    ) -> Union[dict, List[dict]]:
+        """Return unit test parameter settings for the estimator.
 
         Parameters
         ----------
-        parameter_set : str, default="default"
+        parameter_set : None or str, default=None
             Name of the set of test parameters to return, for use in tests. If no
             special parameters are defined for a value, will return `"default"` set.
-            For classifiers, a "default" set of parameters should be provided for
-            general testing, and a "results_comparison" set for comparing against
-            previously recorded results if the general set does not produce suitable
-            probabilities to compare against.
 
         Returns
         -------
-        params : dict or list of dict, default={}
+        params : dict or list of dict
             Parameters to create testing instances of the class.
-            Each dict are parameters to construct an "interesting" test instance, i.e.,
-            `MyClass(**params)` or `MyClass(**params[i])` creates a valid test instance.
-            `create_test_instance` uses the first (or only) dictionary in `params`.
         """
-        from sklearn.ensemble import RandomForestClassifier
-
-        if parameter_set == "results_comparison":
-            return {
-                "n_intervals": 5,
-                "estimator": RandomForestClassifier(n_estimators=10),
-                "interval_transformers": Catch22Transformer(
-                    catch24=True,
-                    replace_nans=True,
-                    features=(
-                        "Mean",
-                        "DN_HistogramMode_5",
-                        "SB_BinaryStats_mean_longstretch1",
-                    ),
-                ),
-            }
-        else:
-            return {
-                "n_intervals": 3,
-                "estimator": RandomForestClassifier(n_estimators=2),
-                "interval_transformers": Catch22Transformer(
-                    catch24=True,
-                    replace_nans=True,
-                    features=(
-                        "Mean",
-                        "DN_HistogramMode_5",
-                        "SB_BinaryStats_mean_longstretch1",
-                    ),
-                ),
-            }
+        return {
+            "n_estimators": 2,
+            "n_intervals": 2,
+        }
```

### Comparing `tsml-0.1.1/tsml/interval_based/tests/test_interval_forest.py` & `tsml-0.2.0/tsml/interval_based/tests/test_interval_forest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# -*- coding: utf-8 -*-
 """Tests for the BaseIntervalForest class."""
 
 import numpy as np
 import pytest
+from sklearn.pipeline import make_pipeline
 from sklearn.tree import DecisionTreeClassifier
 
 from tsml.base import _clone_estimator
 from tsml.interval_based import IntervalForestClassifier
 from tsml.transformations import (
-    ARCoefficientTransformer,
+    AutocorrelationFunctionTransformer,
     Catch22Transformer,
     FunctionTransformer,
     SevenNumberSummaryTransformer,
 )
 from tsml.utils.numba_functions.stats import row_mean, row_numba_min
 from tsml.utils.testing import generate_3d_test_data
 from tsml.vector import CITClassifier
@@ -21,27 +21,33 @@
 @pytest.mark.parametrize(
     "base_estimator",
     [DecisionTreeClassifier(), CITClassifier()],
 )
 def test_interval_forest_feature_skipping(base_estimator):
     """Test BaseIntervalForest feature skipping with different base estimators."""
     X, y = generate_3d_test_data()
+    rs = np.random.randint(np.iinfo(np.int32).max)
 
     est = IntervalForestClassifier(
         base_estimator=base_estimator,
         n_estimators=2,
         n_intervals=2,
-        random_state=np.random.randint(np.iinfo(np.int32).max),
+        random_state=rs,
     )
     est.fit(X, y)
     preds = est.predict(X)
 
     assert est._efficient_predictions is True
 
-    est._test_flag = True
+    est = IntervalForestClassifier(
+        base_estimator=make_pipeline(base_estimator),
+        n_estimators=2,
+        n_intervals=2,
+        random_state=rs,
+    )
     est.fit(X, y)
 
     assert est._efficient_predictions is False
     assert (preds == est.predict(X)).all()
 
 
 def test_interval_forest_invalid_feature_skipping():
@@ -90,14 +96,15 @@
     X, y = generate_3d_test_data(series_length=20)
 
     est = IntervalForestClassifier(
         n_estimators=2,
         n_intervals=n_intervals,
         series_transformers=[None, FunctionTransformer(np.log1p)],
         save_transformed_data=True,
+        random_state=0,
     )
     est.fit(X, y)
     est.predict_proba(X)
 
     data = est.transformed_data_
     assert data[0].shape[1] == n_intervals_len
 
@@ -136,14 +143,15 @@
     est = IntervalForestClassifier(
         n_estimators=2,
         n_intervals=2,
         att_subsample_size=0.5,
         interval_features=features,
         replace_nan=0,
         save_transformed_data=True,
+        random_state=0,
     )
     est.fit(X, y)
     est.predict_proba(X)
 
     data = est.transformed_data_
     assert data[0].shape[1] == int(output_len * 0.5) * 2
 
@@ -162,26 +170,31 @@
     with pytest.raises(ValueError):
         est.fit(X, y)
 
 
 @pytest.mark.parametrize(
     "series_transformer",
     [
+        FunctionTransformer(np.log1p),
         [None, FunctionTransformer(np.log1p)],
-        [FunctionTransformer(np.log1p), ARCoefficientTransformer()],
+        [FunctionTransformer(np.log1p), AutocorrelationFunctionTransformer(n_lags=6)],
     ],
 )
 def test_interval_forest_series_transformer(series_transformer):
     """Test BaseIntervalForest with different series transformers."""
     X, y = generate_3d_test_data()
 
     est = IntervalForestClassifier(
         n_estimators=2,
         n_intervals=2,
         series_transformers=series_transformer,
         save_transformed_data=True,
+        random_state=0,
     )
     est.fit(X, y)
     est.predict_proba(X)
 
     data = est.transformed_data_
-    assert data[0].shape[1] == 12
+    expected = (
+        len(series_transformer) * 6 if isinstance(series_transformer, list) else 6
+    )
+    assert data[0].shape[1] == expected
```

### Comparing `tsml-0.1.1/tsml/shapelet_based/_mrsqm.py` & `tsml-0.2.0/tsml/distance_based/_mpdist.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,147 +1,168 @@
-# -*- coding: utf-8 -*-
+"""Matrix Profile Distance 1-NN Classifier."""
+
+__author__ = ["TonyBagnall", "patrickzib", "MatthewMiddlehurst"]
+__all__ = ["MPDistClassifier"]
+
+from typing import List, Union
+
 import numpy as np
-import pandas as pd
+import stumpy
 from sklearn.base import ClassifierMixin
+from sklearn.metrics import pairwise
 from sklearn.utils.multiclass import check_classification_targets
 from sklearn.utils.validation import check_is_fitted
 
 from tsml.base import BaseTimeSeriesEstimator
-from tsml.utils.validation import _check_optional_dependency
+from tsml.utils.validation import check_n_jobs
 
 
-class MrSQMClassifier(ClassifierMixin, BaseTimeSeriesEstimator):
-    """
-    Wrapper for https://github.com/mlgig/mrsqm.
+class MPDistClassifier(ClassifierMixin, BaseTimeSeriesEstimator):
+    """Matrix Profile Distance 1-NN Classifier.
+
+    Calculates the matrix profile distance to the training data for each case and
+    returns the label of the nearest neighbour.
+
+    Parameters
+    ----------
+    window : int or float, default=10
+        Window size for the matrix profile. If float, will use a proportion of the
+        series length.
+    n_jobs : int, default=1
+        The number of jobs to run in parallel for both `fit` and `predict`.
+        ``-1`` means using all processors.
+
+    Attributes
+    ----------
+    n_instances_ : int
+        The number of train cases in the training set.
+    n_timepoints_ : int
+        The length of each series in the training set.
+    n_classes_ : int
+        Number of classes. Extracted from the data.
+    classes_ : ndarray of shape (n_classes_)
+        Holds the label for each class.
+    class_dictionary_ : dict
+        A dictionary mapping class labels to class indices in classes_.
+
+    References
+    ----------
+    .. [1] Gharghabi, Shaghayegh, et al. "Matrix profile xii: Mpdist: a novel time
+        series distance measure to allow data mining in more challenging scenarios."
+        2018 IEEE International Conference on Data Mining (ICDM). IEEE, 2018.
+
+    Examples
+    --------
+    >>> from tsml.distance_based import MPDistClassifier
+    >>> from tsml.utils.testing import generate_3d_test_data
+    >>> X, y = generate_3d_test_data(n_samples=8, series_length=10, random_state=0)
+    >>> clf = MPDistClassifier()
+    >>> clf.fit(X, y)
+    MPDistClassifier(...)
+    >>> clf.predict(X)
+    array([0, 1, 1, 0, 0, 1, 0, 1])
     """
 
-    def __init__(
-        self,
-        strat="RS",
-        features_per_rep=500,
-        selection_per_rep=2000,
-        nsax=0,
-        nsfa=5,
-        sfa_norm=True,
-        custom_config=None,
-        random_state=None,
-    ):
-        self.strat = strat
-        self.features_per_rep = features_per_rep
-        self.selection_per_rep = selection_per_rep
-        self.nsax = nsax
-        self.nsfa = nsfa
-        self.sfa_norm = sfa_norm
-        self.custom_config = custom_config
-        self.random_state = random_state
+    def __init__(self, window=10, n_jobs=1):
+        self.window = window
+        self.n_jobs = n_jobs
+
+        super(MPDistClassifier, self).__init__()
 
-        _check_optional_dependency("mrsqm", "mrsqm", self)
+    def fit(self, X: Union[np.ndarray, List[np.ndarray]], y: np.ndarray) -> object:
+        """Fit the estimator to training data.
 
-        super(MrSQMClassifier, self).__init__()
+        Parameters
+        ----------
+        X : 2D np.ndarray of shape (n_instances, n_timepoints)
+            The training data.
+        y : 1D np.ndarray of shape (n_instances)
+            The class labels for fitting, indices correspond to instance indices in X
 
-    def fit(self, X, y):
+        Returns
+        -------
+        self :
+            Reference to self.
+        """
         X, y = self._validate_data(X=X, y=y, ensure_min_samples=2)
         X = self._convert_X(X)
 
         check_classification_targets(y)
 
-        self.n_instances_, self.n_dims_, self.series_length_ = (
-            X.shape if X.ndim == 3 else (X.shape[0], 1, X.shape[1])
-        )
+        self.n_instances_, self.n_timepoints_ = X.shape
         self.classes_ = np.unique(y)
         self.n_classes_ = self.classes_.shape[0]
         self.class_dictionary_ = {}
         for index, class_val in enumerate(self.classes_):
             self.class_dictionary_[class_val] = index
 
         if self.n_classes_ == 1:
             return self
 
-        from mrsqm import MrSQMClassifier
+        self._n_jobs = check_n_jobs(self.n_jobs)
 
-        self.clf_ = MrSQMClassifier(
-            strat=self.strat,
-            features_per_rep=self.features_per_rep,
-            selection_per_rep=self.selection_per_rep,
-            nsax=self.nsax,
-            nsfa=self.nsfa,
-            sfa_norm=self.sfa_norm,
-            custom_config=self.custom_config,
-            random_state=self.random_state,
-        )
-        self.clf_.fit(_convert_data(X), y)
+        self._X_train = X.astype(np.float64)
+        self._y_train = y
 
         return self
 
-    def predict(self, X) -> np.ndarray:
+    def predict(self, X: Union[np.ndarray, List[np.ndarray]]) -> np.ndarray:
+        """Predicts labels for sequences in X.
+
+        Parameters
+        ----------
+        X : 2D np.array of shape (n_instances, n_timepoints)
+            The testing data.
+
+        Returns
+        -------
+        y : array-like of shape (n_instances)
+            Predicted class labels.
+        """
         check_is_fitted(self)
 
         # treat case of single class seen in fit
         if self.n_classes_ == 1:
             return np.repeat(list(self.class_dictionary_.keys()), X.shape[0], axis=0)
 
         X = self._validate_data(X=X, reset=False)
         X = self._convert_X(X)
 
-        return self.clf_.predict(_convert_data(X))
-
-    def predict_proba(self, X) -> np.ndarray:
-        check_is_fitted(self)
-
-        # treat case of single class seen in fit
-        if self.n_classes_ == 1:
-            return np.repeat([[1]], X.shape[0], axis=0)
+        window = (
+            self.window if self.window >= 1 else int(self.window * self.n_timepoints_)
+        )
 
-        X = self._validate_data(X=X, reset=False)
-        X = self._convert_X(X)
+        distance_matrix = pairwise.pairwise_distances(
+            X.astype(np.float64),
+            self._X_train,
+            metric=(lambda x, y: stumpy.mpdist(x, y, window)),
+            n_jobs=self._n_jobs,
+        )
 
-        return self.clf_.predict_proba(_convert_data(X))
+        return self._y_train[np.argmin(distance_matrix, axis=1)]
 
-    def _more_tags(self):
+    def _more_tags(self) -> dict:
         return {
-            "non_deterministic": True,
-            "_xfail_checks": {"check_estimators_pickle": "External failure to pickle."},
+            "X_types": ["2darray"],
+            "optional_dependency": True,
         }
 
     @classmethod
-    def get_test_params(cls, parameter_set="default"):
-        """Return testing parameter settings for the estimator.
+    def get_test_params(
+        cls, parameter_set: Union[str, None] = None
+    ) -> Union[dict, List[dict]]:
+        """Return unit test parameter settings for the estimator.
 
         Parameters
         ----------
-        parameter_set : str, default="default"
+        parameter_set : None or str, default=None
             Name of the set of test parameters to return, for use in tests. If no
             special parameters are defined for a value, will return `"default"` set.
-            For classifiers, a "default" set of parameters should be provided for
-            general testing, and a "results_comparison" set for comparing against
-            previously recorded results if the general set does not produce suitable
-            probabilities to compare against.
 
         Returns
         -------
-        params : dict or list of dict, default={}
+        params : dict or list of dict
             Parameters to create testing instances of the class.
-            Each dict are parameters to construct an "interesting" test instance, i.e.,
-            `MyClass(**params)` or `MyClass(**params[i])` creates a valid test instance.
-            `create_test_instance` uses the first (or only) dictionary in `params`.
         """
-
         return {
-            "features_per_rep": 50,
-            "selection_per_rep": 200,
-            "nsax": 1,
-            "nsfa": 1,
+            "window": 0.8,
         }
-
-
-def _convert_data(X):
-    column_list = []
-    for i in range(X.shape[1]):
-        nested_column = (
-            pd.DataFrame(X[:, i, :])
-            .apply(lambda x: [pd.Series(x, dtype=X.dtype)], axis=1)
-            .str[0]
-            .rename(str(i))
-        )
-        column_list.append(nested_column)
-    df = pd.concat(column_list, axis=1)
-    return df
```

### Comparing `tsml-0.1.1/tsml/shapelet_based/_rsf.py` & `tsml-0.2.0/tsml/shapelet_based/_rsf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-# -*- coding: utf-8 -*-
+"""Random Shapelet Forest (RSF) estimators."""
+from typing import List, Union
+
 import numpy as np
 from sklearn.base import ClassifierMixin, RegressorMixin
 from sklearn.utils.multiclass import check_classification_targets
 from sklearn.utils.validation import check_is_fitted
 
 from tsml.base import BaseTimeSeriesEstimator
 from tsml.utils.validation import _check_optional_dependency, check_n_jobs
 
 
 class RandomShapeletForestClassifier(ClassifierMixin, BaseTimeSeriesEstimator):
-    """
-    Wrapper for https://github.com/wildboar-foundation/wildboar RSF implementation.
+    """Random Shapelet Forest (RSF) Classifier.
+
+    Wrapper for the wildboar RSF implementation.
     """
 
     def __init__(
         self,
         n_estimators=100,
         n_shapelets=10,
         max_depth=None,
@@ -27,16 +30,16 @@
         metric="euclidean",
         metric_params=None,
         criterion="entropy",
         oob_score=False,
         bootstrap=True,
         warm_start=False,
         class_weight=None,
-        n_jobs=None,
         random_state=None,
+        n_jobs=None,
     ):
         self.n_shapelets = n_shapelets
         self.n_estimators = n_estimators
         self.max_depth = max_depth
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.min_impurity_decrease = min_impurity_decrease
@@ -46,28 +49,42 @@
         self.metric = metric
         self.metric_params = metric_params
         self.criterion = criterion
         self.oob_score = oob_score
         self.bootstrap = bootstrap
         self.warm_start = warm_start
         self.class_weight = class_weight
-        self.n_jobs = n_jobs
         self.random_state = random_state
+        self.n_jobs = n_jobs
 
         _check_optional_dependency("wildboar", "wildboar", self)
 
         super(RandomShapeletForestClassifier, self).__init__()
 
-    def fit(self, X, y):
+    def fit(self, X: Union[np.ndarray, List[np.ndarray]], y: np.ndarray) -> object:
+        """Fit the estimator to training data.
+
+        Parameters
+        ----------
+        X : 3D np.ndarray of shape (n_instances, n_channels, n_timepoints)
+            The training data.
+        y : 1D np.ndarray of shape (n_instances)
+            The class labels for fitting, indices correspond to instance indices in X
+
+        Returns
+        -------
+        self :
+            Reference to self.
+        """
         X, y = self._validate_data(X=X, y=y, ensure_min_samples=2)
         X = self._convert_X(X)
 
         check_classification_targets(y)
 
-        self.n_instances_, self.n_dims_, self.series_length_ = (
+        self.n_instances_, self.n_channels_, self.n_timepoints_ = (
             X.shape if X.ndim == 3 else (X.shape[0], 1, X.shape[1])
         )
         self.classes_ = np.unique(y)
         self.n_classes_ = self.classes_.shape[0]
         self.class_dictionary_ = {}
         for index, class_val in enumerate(self.classes_):
             self.class_dictionary_[class_val] = index
@@ -95,82 +112,106 @@
             metric=self.metric,
             metric_params=self.metric_params,
             criterion=self.criterion,
             oob_score=self.oob_score,
             bootstrap=self.bootstrap,
             warm_start=self.warm_start,
             class_weight=self.class_weight,
-            n_jobs=self._n_jobs,
             random_state=self.random_state,
+            n_jobs=self._n_jobs,
         )
         self.clf_.fit(X, y)
 
         return self
 
-    def predict(self, X) -> np.ndarray:
+    def predict(self, X: Union[np.ndarray, List[np.ndarray]]) -> np.ndarray:
+        """Predicts labels for sequences in X.
+
+        Parameters
+        ----------
+        X : 3D np.array of shape (n_instances, n_channels, n_timepoints)
+            The testing data.
+
+        Returns
+        -------
+        y : array-like of shape (n_instances)
+            Predicted class labels.
+        """
         check_is_fitted(self)
 
         # treat case of single class seen in fit
         if self.n_classes_ == 1:
             return np.repeat(list(self.class_dictionary_.keys()), X.shape[0], axis=0)
 
         X = self._validate_data(X=X, reset=False)
         X = self._convert_X(X)
 
         if X.ndim == 3 and X.shape[1] == 1:
             X = np.reshape(X, (X.shape[0], X.shape[2]))
 
         return self.clf_.predict(X)
 
-    def _predict_proba(self, X) -> np.ndarray:
+    def predict_proba(self, X: Union[np.ndarray, List[np.ndarray]]) -> np.ndarray:
+        """Predicts labels probabilities for sequences in X.
+
+        Parameters
+        ----------
+        X : 3D np.array of shape (n_instances, n_channels, n_timepoints)
+            The testing data.
+
+        Returns
+        -------
+        y : array-like of shape (n_instances, n_classes_)
+            Predicted probabilities using the ordering in classes_.
+        """
         check_is_fitted(self)
 
         # treat case of single class seen in fit
         if self.n_classes_ == 1:
             return np.repeat([[1]], X.shape[0], axis=0)
 
         X = self._validate_data(X=X, reset=False)
         X = self._convert_X(X)
 
         if X.ndim == 3 and X.shape[1] == 1:
             X = np.reshape(X, (X.shape[0], X.shape[2]))
 
         return self.clf_.predict_proba(X)
 
+    def _more_tags(self) -> dict:
+        return {
+            "optional_dependency": True,
+        }
+
     @classmethod
-    def get_test_params(cls, parameter_set="default"):
-        """Return testing parameter settings for the estimator.
+    def get_test_params(
+        cls, parameter_set: Union[str, None] = None
+    ) -> Union[dict, List[dict]]:
+        """Return unit test parameter settings for the estimator.
 
         Parameters
         ----------
-        parameter_set : str, default="default"
+        parameter_set : None or str, default=None
             Name of the set of test parameters to return, for use in tests. If no
             special parameters are defined for a value, will return `"default"` set.
-            For classifiers, a "default" set of parameters should be provided for
-            general testing, and a "results_comparison" set for comparing against
-            previously recorded results if the general set does not produce suitable
-            probabilities to compare against.
 
         Returns
         -------
-        params : dict or list of dict, default={}
+        params : dict or list of dict
             Parameters to create testing instances of the class.
-            Each dict are parameters to construct an "interesting" test instance, i.e.,
-            `MyClass(**params)` or `MyClass(**params[i])` creates a valid test instance.
-            `create_test_instance` uses the first (or only) dictionary in `params`.
         """
-
         return {
             "n_estimators": 2,
         }
 
 
 class RandomShapeletForestRegressor(RegressorMixin, BaseTimeSeriesEstimator):
-    """
-    Wrapper for https://github.com/wildboar-foundation/wildboar RSF implementation.
+    """Random Shapelet Forest (RSF) Regressor.
+
+    Wrapper for the wildboar RSF implementation.
     """
 
     def __init__(
         self,
         n_estimators=100,
         n_shapelets=10,
         max_depth=None,
@@ -182,16 +223,16 @@
         alpha=None,
         metric="euclidean",
         metric_params=None,
         criterion="squared_error",
         oob_score=False,
         bootstrap=True,
         warm_start=False,
-        n_jobs=None,
         random_state=None,
+        n_jobs=None,
     ):
         self.n_shapelets = n_shapelets
         self.n_estimators = n_estimators
         self.max_depth = max_depth
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.min_impurity_decrease = min_impurity_decrease
@@ -200,23 +241,37 @@
         self.alpha = alpha
         self.metric = metric
         self.metric_params = metric_params
         self.criterion = criterion
         self.oob_score = oob_score
         self.bootstrap = bootstrap
         self.warm_start = warm_start
-        self.n_jobs = n_jobs
         self.random_state = random_state
+        self.n_jobs = n_jobs
 
         _check_optional_dependency("wildboar", "wildboar", self)
 
         super(RandomShapeletForestRegressor, self).__init__()
 
-    def fit(self, X, y):
-        X, y = self._validate_data(X=X, y=y, ensure_min_samples=2)
+    def fit(self, X: Union[np.ndarray, List[np.ndarray]], y: np.ndarray) -> object:
+        """Fit the estimator to training data.
+
+        Parameters
+        ----------
+        X : 3D np.ndarray of shape (n_instances, n_channels, n_timepoints)
+            The training data.
+        y : 1D np.ndarray of shape (n_instances)
+            The target labels for fitting, indices correspond to instance indices in X
+
+        Returns
+        -------
+        self :
+            Reference to self.
+        """
+        X, y = self._validate_data(X=X, y=y, ensure_min_samples=2, y_numeric=True)
         X = self._convert_X(X)
 
         self._n_jobs = check_n_jobs(self.n_jobs)
 
         if X.ndim == 3 and X.shape[1] == 1:
             X = np.reshape(X, (X.shape[0], X.shape[2]))
 
@@ -234,50 +289,62 @@
             alpha=self.alpha,
             metric=self.metric,
             metric_params=self.metric_params,
             criterion=self.criterion,
             oob_score=self.oob_score,
             bootstrap=self.bootstrap,
             warm_start=self.warm_start,
-            n_jobs=self._n_jobs,
             random_state=self.random_state,
+            n_jobs=self._n_jobs,
         )
         self.reg_.fit(X, y)
 
         return self
 
-    def predict(self, X) -> np.ndarray:
+    def predict(self, X: Union[np.ndarray, List[np.ndarray]]) -> np.ndarray:
+        """Predicts labels for sequences in X.
+
+        Parameters
+        ----------
+        X : 3D np.ndarray of shape (n_instances, n_channels, n_timepoints)
+            The testing data.
+
+        Returns
+        -------
+        y : array-like of shape (n_instances)
+            Predicted target labels.
+        """
         check_is_fitted(self)
 
         X = self._validate_data(X=X, reset=False)
         X = self._convert_X(X)
 
         if X.ndim == 3 and X.shape[1] == 1:
             X = np.reshape(X, (X.shape[0], X.shape[2]))
 
         return self.reg_.predict(X)
 
+    def _more_tags(self) -> dict:
+        return {
+            "optional_dependency": True,
+        }
+
     @classmethod
-    def get_test_params(cls, parameter_set="default"):
-        """Return testing parameter settings for the estimator.
+    def get_test_params(
+        cls, parameter_set: Union[str, None] = None
+    ) -> Union[dict, List[dict]]:
+        """Return unit test parameter settings for the estimator.
 
         Parameters
         ----------
-        parameter_set : str, default="default"
+        parameter_set : None or str, default=None
             Name of the set of test parameters to return, for use in tests. If no
             special parameters are defined for a value, will return `"default"` set.
-            For classifiers, a "default" set of parameters should be provided for
-            general testing, and a "results_comparison" set for comparing against
-            previously recorded results if the general set does not produce suitable
-            probabilities to compare against.
 
         Returns
         -------
-        params : dict or list of dict, default={}
+        params : dict or list of dict
             Parameters to create testing instances of the class.
-            Each dict are parameters to construct an "interesting" test instance, i.e.,
-            `MyClass(**params)` or `MyClass(**params[i])` creates a valid test instance.
-            `create_test_instance` uses the first (or only) dictionary in `params`.
         """
         return {
             "n_estimators": 2,
         }
```

### Comparing `tsml-0.1.1/tsml/shapelet_based/_stc.py` & `tsml-0.2.0/tsml/shapelet_based/_stc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-# -*- coding: utf-8 -*-
 """A shapelet transform classifier (STC).
 
 Shapelet transform classifier pipeline that simply performs a (configurable) shapelet
 transform then builds (by default) a rotation forest classifier on the output.
 """
 
 __author__ = ["TonyBagnall", "MatthewMiddlehurst"]
 __all__ = ["ShapeletTransformClassifier"]
 
+from typing import List, Union
+
 import numpy as np
 from sklearn.base import ClassifierMixin
 from sklearn.utils.multiclass import check_classification_targets
 from sklearn.utils.validation import check_is_fitted
 
 from tsml.base import BaseTimeSeriesEstimator, _clone_estimator
 from tsml.transformations._shapelet_transform import RandomShapeletTransformer
@@ -20,16 +21,16 @@
 
 
 class ShapeletTransformClassifier(ClassifierMixin, BaseTimeSeriesEstimator):
     """A shapelet transform classifier (STC).
 
     Implementation of the binary shapelet transform classifier pipeline along the lines
     of [1][2] but with random shapelet sampling. Transforms the data using the
-    configurable `RandomShapeletTransform` and then builds a `RotationForest`
-    classifier.
+    configurable `RandomShapeletTransformer` and then builds a
+    `RotationForestClassifier` classifier.
 
     As some implementations and applications contract the transformation solely,
     contracting is available for the transform only and both classifier and transform.
 
     Parameters
     ----------
     n_shapelet_samples : int, default=10000
@@ -71,48 +72,59 @@
         If `int`, random_state is the seed used by the random number generator;
         If `RandomState` instance, random_state is the random number generator;
         If `None`, the random number generator is the `RandomState` instance used
         by `np.random`.
 
     Attributes
     ----------
-    classes_ : list
-        The unique class labels in the training set.
-    n_classes_ : int
-        The number of unique classes in the training set.
-    fit_time_  : int
-        The time (in milliseconds) for ``fit`` to run.
     n_instances_ : int
         The number of train cases in the training set.
-    n_dims_ : int
+    n_channels_ : int
         The number of dimensions per case in the training set.
-    series_length_ : int
+    n_timepoints_ : int
         The length of each series in the training set.
+    n_classes_ : int
+        Number of classes. Extracted from the data.
+    classes_ : ndarray of shape (n_classes_)
+        Holds the label for each class.
+    class_dictionary_ : dict
+        A dictionary mapping class labels to class indices in classes_.
     transformed_data_ : list of shape (n_estimators) of ndarray
         The transformed training dataset for all classifiers. Only saved when
         ``save_transformed_data`` is `True`.
 
     See Also
     --------
-    RandomShapeletTransform : The randomly sampled shapelet transform.
-    RotationForest : The default rotation forest classifier used.
+    RandomShapeletTransformer
+    RotationForestClassifier
 
     Notes
     -----
     For the Java version, see
     `tsml <https://github.com/uea-machine-learning/tsml/blob/master/src/main/
     java/tsml/classifiers/shapelet_based/ShapeletTransformClassifier.java>`_.
 
     References
     ----------
     .. [1] Jon Hills et al., "Classification of time series by shapelet transformation",
        Data Mining and Knowledge Discovery, 28(4), 851--881, 2014.
     .. [2] A. Bostrom and A. Bagnall, "Binary Shapelet Transform for Multiclass Time
        Series Classification", Transactions on Large-Scale Data and Knowledge Centered
        Systems, 32, 2017.
+
+    Examples
+    --------
+    >>> from tsml.shapelet_based import ShapeletTransformClassifier
+    >>> from tsml.utils.testing import generate_3d_test_data
+    >>> X, y = generate_3d_test_data(n_samples=8, series_length=10, random_state=0)
+    >>> clf = ShapeletTransformClassifier(random_state=0)
+    >>> clf.fit(X, y)
+    ShapeletTransformClassifier(...)
+    >>> clf.predict(X)
+    array([0, 1, 1, 0, 0, 1, 0, 1])
     """
 
     def __init__(
         self,
         n_shapelet_samples=10000,
         max_shapelets=None,
         max_shapelet_length=None,
@@ -137,40 +149,35 @@
 
         self.random_state = random_state
         self.batch_size = batch_size
         self.n_jobs = n_jobs
 
         super(ShapeletTransformClassifier, self).__init__()
 
-    def fit(self, X, y):
-        """Fit ShapeletTransformClassifier to training data.
+    def fit(self, X: Union[np.ndarray, List[np.ndarray]], y: np.ndarray) -> object:
+        """Fit the estimator to training data.
 
         Parameters
         ----------
-        X : 3D np.array of shape = [n_instances, n_dimensions, series_length]
+        X : 3D np.ndarray of shape (n_instances, n_channels, n_timepoints)
             The training data.
-        y : array-like, shape = [n_instances]
-            The class labels.
+        y : 1D np.ndarray of shape (n_instances)
+            The class labels for fitting, indices correspond to instance indices in X
 
         Returns
         -------
         self :
             Reference to self.
-
-        Notes
-        -----
-        Changes state by creating a fitted model that updates attributes
-        ending in "_".
         """
         X, y = self._validate_data(X=X, y=y, ensure_min_samples=2)
         X = self._convert_X(X)
 
         check_classification_targets(y)
 
-        self.n_instances_, self.n_dims_, self.series_length_ = X.shape
+        self.n_instances_, self.n_channels_, self.n_timepoints_ = X.shape
         self.classes_ = np.unique(y)
         self.n_classes_ = self.classes_.shape[0]
         self.class_dictionary_ = {}
         for index, class_val in enumerate(self.classes_):
             self.class_dictionary_[class_val] = index
 
         if self.n_classes_ == 1:
@@ -220,49 +227,49 @@
         if self.save_transformed_data:
             self.transformed_data_ = X_t
 
         self._estimator.fit(X_t, y)
 
         return self
 
-    def predict(self, X) -> np.ndarray:
+    def predict(self, X: Union[np.ndarray, List[np.ndarray]]) -> np.ndarray:
         """Predicts labels for sequences in X.
 
         Parameters
         ----------
-        X : 3D np.array of shape = [n_instances, n_dimensions, series_length]
-            The data to make predictions for.
+        X : 3D np.array of shape (n_instances, n_channels, n_timepoints)
+            The testing data.
 
         Returns
         -------
-        y : array-like, shape = [n_instances]
+        y : array-like of shape (n_instances)
             Predicted class labels.
         """
         check_is_fitted(self)
 
         # treat case of single class seen in fit
         if self.n_classes_ == 1:
             return np.repeat(list(self.class_dictionary_.keys()), X.shape[0], axis=0)
 
         X = self._validate_data(X=X, reset=False)
         X = self._convert_X(X)
 
         return self._estimator.predict(self._transformer.transform(X))
 
-    def predict_proba(self, X) -> np.ndarray:
+    def predict_proba(self, X: Union[np.ndarray, List[np.ndarray]]) -> np.ndarray:
         """Predicts labels probabilities for sequences in X.
 
         Parameters
         ----------
-        X : 3D np.array of shape = [n_instances, n_dimensions, series_length]
-            The data to make predict probabilities for.
+        X : 3D np.array of shape (n_instances, n_channels, n_timepoints)
+            The testing data.
 
         Returns
         -------
-        y : array-like, shape = [n_instances, n_classes_]
+        y : array-like of shape (n_instances, n_classes_)
             Predicted probabilities using the ordering in classes_.
         """
         check_is_fitted(self)
 
         # treat case of single class seen in fit
         if self.n_classes_ == 1:
             return np.repeat([[1]], X.shape[0], axis=0)
@@ -277,45 +284,29 @@
             dists = np.zeros((X.shape[0], self.n_classes_))
             preds = self._estimator.predict(self._transformer.transform(X))
             for i in range(0, X.shape[0]):
                 dists[i, self.class_dictionary_[preds[i]]] = 1
             return dists
 
     @classmethod
-    def get_test_params(cls, parameter_set="default"):
-        """Return testing parameter settings for the estimator.
+    def get_test_params(
+        cls, parameter_set: Union[str, None] = None
+    ) -> Union[dict, List[dict]]:
+        """Return unit test parameter settings for the estimator.
 
         Parameters
         ----------
-        parameter_set : str, default="default"
+        parameter_set : None or str, default=None
             Name of the set of test parameters to return, for use in tests. If no
             special parameters are defined for a value, will return `"default"` set.
-            For classifiers, a "default" set of parameters should be provided for
-            general testing, and a "results_comparison" set for comparing against
-            previously recorded results if the general set does not produce suitable
-            probabilities to compare against.
 
         Returns
         -------
-        params : dict or list of dict, default={}
+        params : dict or list of dict
             Parameters to create testing instances of the class.
-            Each dict are parameters to construct an "interesting" test instance, i.e.,
-            `MyClass(**params)` or `MyClass(**params[i])` creates a valid test instance.
-            `create_test_instance` uses the first (or only) dictionary in `params`.
         """
-        from sklearn.ensemble import RandomForestClassifier
-
-        if parameter_set == "results_comparison":
-            return {
-                "estimator": RandomForestClassifier(n_estimators=5),
-                "n_shapelet_samples": 50,
-                "max_shapelets": 10,
-                "batch_size": 10,
-            }
-        else:
-            return {
-                "estimator": RotationForestClassifier(n_estimators=2),
-                "n_shapelet_samples": 10,
-                "max_shapelets": 3,
-                "batch_size": 5,
-                "save_transformed_data": True,
-            }
+        return {
+            "estimator": RotationForestClassifier(n_estimators=2),
+            "n_shapelet_samples": 10,
+            "max_shapelets": 3,
+            "batch_size": 5,
+        }
```

### Comparing `tsml-0.1.1/tsml/tests/_sklearn_checks.py` & `tsml-0.2.0/tsml/tests/test_estimators_sklearn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Patched estimator checks originating from scikit-learn."""
 
 __author__ = ["MatthewMiddlehurst"]
 
 import pickle
 import warnings
 from copy import deepcopy
@@ -399,16 +398,15 @@
 
     assert hasattr(transformer, "transform")
 
     X_pred2 = transformer.transform(X)
     X_pred3 = transformer.fit_transform(X, y=y)
 
     if _safe_tags(transformer_orig, key="non_deterministic"):
-        msg = name + " is non deterministic"
-        raise SkipTest(msg)
+        raise SkipTest(name + " is non deterministic")
 
     if isinstance(X_pred, tuple) and isinstance(X_pred2, tuple):
         for x_pred, x_pred2, x_pred3 in zip(X_pred, X_pred2, X_pred3):
             assert_allclose(
                 x_pred,
                 x_pred2,
                 atol=1e-2,
@@ -952,25 +950,29 @@
 
     # Check that when a 2D y is given, a DataConversionWarning is
     # raised
     with warnings.catch_warnings(record=True) as w:
         warnings.simplefilter("always", DataConversionWarning)
         warnings.simplefilter("ignore", RuntimeWarning)
         estimator.fit(X, y[:, np.newaxis])
+
     y_pred_2d = estimator.predict(X)
     msg = "expected 1 DataConversionWarning, got: %s" % ", ".join(
         [str(w_x) for w_x in w]
     )
 
     assert len(w) > 0, msg
     assert (
         "DataConversionWarning('A column-vector y"
         " was passed when a 1d array was expected" in msg
     )
 
+    if _safe_tags(estimator_orig, key="non_deterministic"):
+        raise SkipTest(name + " is non deterministic")
+
     assert_allclose(y_pred.ravel(), y_pred_2d.ravel())
 
 
 @ignore_warnings(category=FutureWarning)
 def check_classifiers_classes(name, classifier_orig):
     """Check classifier can handle binary and multiclass data with different y types.
 
@@ -1074,14 +1076,18 @@
     set_random_state(regressor_2)
 
     # fit
     regressor_1.fit(X, y)
     pred1 = regressor_1.predict(X)
     regressor_2.fit(X, y.astype(float))
     pred2 = regressor_2.predict(X)
+
+    if _safe_tags(regressor_orig, key="non_deterministic"):
+        raise SkipTest(name + " is non deterministic")
+
     assert_allclose(pred1, pred2, atol=1e-2, err_msg=name)
 
 
 @ignore_warnings(category=FutureWarning)
 def check_regressors_train(
     name, regressor_orig, readonly_memmap=False, X_dtype=np.float64
 ):
@@ -1220,14 +1226,18 @@
             )
 
     # fit
     estimator_1.fit(X_, y_)
     pred1 = estimator_1.predict(X_)
     estimator_2.fit(X, y)
     pred2 = estimator_2.predict(X)
+
+    if _safe_tags(estimator_orig, key="non_deterministic"):
+        raise SkipTest(name + " is non deterministic")
+
     assert_allclose(pred1, pred2, atol=1e-2, err_msg=name)
 
 
 @ignore_warnings(category=FutureWarning)
 def check_classifiers_regression_target(name, classifier_orig):
     """Check if classifier throws an exception when fed regression targets.
```

### Comparing `tsml-0.1.1/tsml/tests/test_interface.py` & `tsml-0.2.0/tsml/tests/test_interface.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-# -*- coding: utf-8 -*-
 """Unit tests for tsml interface."""
 import numpy as np
 import pytest
 
 from tsml.base import BaseTimeSeriesEstimator
-from tsml.dummy import DummyClassifier
-from tsml.interval_based import CIFClassifier
-from tsml.transformations import Catch22Transformer
 from tsml.utils.testing import (
     generate_2d_test_data,
     generate_3d_test_data,
     generate_unequal_test_data,
 )
 
 
@@ -67,25 +63,25 @@
     est._validate_data(X)
 
 
 class _3dArrayDummy(BaseTimeSeriesEstimator):
     def __init__(self):
         super(_3dArrayDummy, self).__init__()
 
-    def _more_tags(self):
+    def _more_tags(self) -> dict:
         return {"X_types": ["3darray"]}
 
 
 class _2dArrayDummy(BaseTimeSeriesEstimator):
     def __init__(self):
         super(_2dArrayDummy, self).__init__()
 
-    def _more_tags(self):
+    def _more_tags(self) -> dict:
         return {"X_types": ["2darray"]}
 
 
 class _NpListDummy(BaseTimeSeriesEstimator):
     def __init__(self):
         super(_NpListDummy, self).__init__()
 
-    def _more_tags(self):
+    def _more_tags(self) -> dict:
         return {"X_types": ["np_list"]}
```

### Comparing `tsml-0.1.1/tsml/transformations/__init__.py` & `tsml-0.2.0/tsml/transformations/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,22 +8,28 @@
     "FPCATransformer",
     "FunctionTransformer",
     "RandomIntervalTransformer",
     "SupervisedIntervalTransformer",
     "PeriodogramTransformer",
     # "SFATransformer",
     "RandomShapeletTransformer",
+    "RandomDilatedShapeletTransformer",
     "SevenNumberSummaryTransformer",
+    "TransformerConcatenator",
 ]
 
 from tsml.transformations._acf import AutocorrelationFunctionTransformer
 from tsml.transformations._ar_coefficient import ARCoefficientTransformer
 from tsml.transformations._catch22 import Catch22Transformer
 from tsml.transformations._fpca import FPCATransformer
 from tsml.transformations._function_transformer import FunctionTransformer
 from tsml.transformations._interval_extraction import (
     RandomIntervalTransformer,
     SupervisedIntervalTransformer,
 )
 from tsml.transformations._periodogram import PeriodogramTransformer
-from tsml.transformations._shapelet_transform import RandomShapeletTransformer
+from tsml.transformations._shapelet_transform import (
+    RandomDilatedShapeletTransformer,
+    RandomShapeletTransformer,
+)
 from tsml.transformations._summary_features import SevenNumberSummaryTransformer
+from tsml.transformations._transform_concatenator import TransformerConcatenator
```

### Comparing `tsml-0.1.1/tsml/transformations/_catch22.py` & `tsml-0.2.0/tsml/transformations/_catch22.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Catch22 features.
 
 A transformer for the Catch22 features.
 """
 
 __author__ = ["MatthewMiddlehurst"]
 __all__ = ["Catch22Transformer"]
@@ -77,23 +76,28 @@
     catch24 : bool, optional, default=False
         Extract the mean and standard deviation as well as the 22 Catch22 features if
         true. If a List of specific features to extract is provided, "Mean" and/or
         "StandardDeviation" must be added to the List to extract these features.
     outlier_norm : bool, optional, default=False
         Normalise each series during the two outlier Catch22 features, which can take a
         while to process for large values.
-    replace_nans : bool, optional, default=True
+    replace_nans : bool, optional, default=False
         Replace NaN or inf values from the Catch22 transform with 0.
     use_pycatch22 : bool, optional, default=True
         Wraps the C based pycatch22 implementation for tsml.
         (https://github.com/DynamicsAndNeuralSystems/pycatch22). This requires the
         ``pycatch22`` package to be installed if True.
     n_jobs : int, optional, default=1
-        The number of jobs to run in parallel for transform. Requires multiple input
+        The number of jobs to run in parallel for `transform`. Requires multiple input
         cases. ``-1`` means using all processors.
+    parallel_backend : str, ParallelBackendBase instance or None, default=None
+        Specify the parallelisation backend implementation in joblib, if None a 'prefer'
+        value of "threads" is used by default.
+        Valid options are "loky", "multiprocessing", "threading" or a custom backend.
+        See the joblib Parallel documentation for more details.
 
     See Also
     --------
     Catch22Classifier
 
     Notes
     -----
@@ -108,54 +112,75 @@
     ----------
     .. [1] Lubba, C. H., Sethi, S. S., Knaute, P., Schultz, S. R., Fulcher, B. D., &
     Jones, N. S. (2019). catch22: Canonical time-series characteristics. Data Mining
     and Knowledge Discovery, 33(6), 1821-1852.
     .. [2] Fulcher, B. D., Little, M. A., & Jones, N. S. (2013). Highly comparative
     time-series analysis: the empirical structure of time series and their methods.
     Journal of the Royal Society Interface, 10(83), 20130048.
+
+    Examples
+    --------
+    >>> from tsml.transformations import Catch22Transformer
+    >>> from tsml.utils.testing import generate_3d_test_data
+    >>> X, _ = generate_3d_test_data(n_samples=4, series_length=10, random_state=0)
+    >>> tnf = Catch22Transformer(replace_nans=True)
+    >>> tnf.fit(X)
+    Catch22Transformer(...)
+    >>> print(tnf.transform(X)[0])
+    [6.27596874e-02 3.53871087e-01 4.00000000e+00 7.00000000e-01
+     2.00000000e-01 5.66227710e-01 2.00000000e+00 3.08148791e-34
+     1.96349541e+00 9.99913411e-01 1.39251594e+00 3.89048349e-01
+     2.00000000e+00 1.00000000e+00 3.00000000e+00 2.04319187e+00
+     1.00000000e+00 2.44474814e-01 0.00000000e+00 0.00000000e+00
+     8.23045267e-03 0.00000000e+00]
     """
 
     def __init__(
         self,
         features="all",
         catch24=False,
         outlier_norm=False,
         replace_nans=False,
         use_pycatch22=True,
         n_jobs=1,
+        parallel_backend=None,
     ):
         self.features = features
         self.catch24 = catch24
         self.outlier_norm = outlier_norm
         self.replace_nans = replace_nans
         self.use_pycatch22 = use_pycatch22
         self.n_jobs = n_jobs
+        self.parallel_backend = parallel_backend
 
         if use_pycatch22:
             _check_optional_dependency("pycatch22", "pycatch22", self)
 
         super(Catch22Transformer, self).__init__()
 
     def fit(self, X, y=None):
+        """Unused. Validates X."""
         self._validate_data(X=X)
         return self
 
     def transform(self, X, y=None):
-        """Transform data into the Catch22 features.
+        """Transform X into the catch22 features.
 
         Parameters
         ----------
-        X : 3D numpy array of shape [n_instances, n_dimensions, n_features],
-            input time series panel.
-        y : ignored.
+        X : 3D np.array (any number of channels, equal length series)
+                of shape (n_instances, n_channels, n_timepoints)
+            or list of numpy arrays (any number of channels, unequal length series)
+                of shape [n_instances], 2D np.array (n_channels, n_timepoints_i), where
+                n_timepoints_i is length of series i
 
         Returns
         -------
-        c22 : Pandas DataFrame of shape [n_instances, c*n_dimensions] where c is the
-             number of features requested, containing Catch22 features for X.
+        Xt : array-like, shape = [n_instances, num_features*n_channels]
+            The catch22 features for each dimension.
         """
         X = self._validate_data(X=X, reset=False)
         X = self._convert_X(X)
 
         n_instances = len(X)
 
         f_idx = _verify_features(self.features, self.catch24)
@@ -211,15 +236,17 @@
                 Catch22Transformer._CO_Embed2_Dist_tau_d_expfit_meandiff,
                 Catch22Transformer._SC_FluctAnal_2_dfa_50_1_2_logi_prop_r1,
                 Catch22Transformer._SC_FluctAnal_2_rsrangefit_50_1_logi_prop_r1,
                 Catch22Transformer._SB_TransitionMatrix_3ac_sumdiagcov,
                 Catch22Transformer._PD_PeriodicityWang_th0_01,
             ]
 
-        c22_list = Parallel(n_jobs=threads_to_use)(
+        c22_list = Parallel(
+            n_jobs=threads_to_use, backend=self.parallel_backend, prefer="threads"
+        )(
             delayed(
                 self._transform_case_pycatch22
                 if self.use_pycatch22
                 else self._transform_case
             )(
                 X[i],
                 f_idx,
@@ -353,33 +380,34 @@
                 elif feature == 23:
                     c22[dim + n] = np.std(series)
                 else:
                     c22[dim + n] = features[feature](series)
 
         return c22
 
-    def _more_tags(self):
-        return {
-            "X_types": ["np_list", "3darray"],
-            "requires_fit": False,
-            "optional_dependency": self.use_pycatch22,
-        }
-
     @property
     def get_features_arguments(self):
+        """Return feature names for the estimators features argument."""
         return (
             self.features
             if self.features != "all"
             else (
                 feature_names + ["Mean", "StandardDeviation"]
                 if self.catch24
                 else feature_names
             )
         )
 
+    def _more_tags(self) -> dict:
+        return {
+            "X_types": ["np_list", "3darray"],
+            "requires_fit": False,
+            "optional_dependency": self.use_pycatch22,
+        }
+
     @classmethod
     def get_test_params(cls, parameter_set="default"):
         """Return testing parameter settings for the estimator.
 
         Parameters
         ----------
         parameter_set : str, default="default"
```

### Comparing `tsml-0.1.1/tsml/transformations/_fpca.py` & `tsml-0.2.0/tsml/transformations/_fpca.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,129 +1,141 @@
-# -*- coding: utf-8 -*-
 """Functional Principal Component Analysis."""
 
 __author__ = ["dguijo", "MatthewMiddlehurst"]
 __all__ = ["FPCATransformer"]
 
 import numpy as np
 from sklearn.base import TransformerMixin
 from sklearn.utils.validation import check_is_fitted
 
 from tsml.base import BaseTimeSeriesEstimator
 from tsml.utils.validation import _check_optional_dependency
 
 
 class FPCATransformer(TransformerMixin, BaseTimeSeriesEstimator):
-    """Apply FPCA on a set of time X to transform the X into a reduced dimension."""
+    """Apply FPCA on a set of time X to transform the X into a reduced dimension.
+
+    Wraps the Functional Principal Component Analysis from scikit-fda.
+
+    Parameters
+    ----------
+    n_components: int, default=10
+        Number of principal components to keep from functional principal component
+        analysis.
+    centering: bool, default=True
+        Set to ``False`` when the functional data is already known to be centered
+        and there is no need to center it. Otherwise, the mean of the functional
+        data object is calculated and the data centered before fitting.
+    bspline: bool, default=False
+        Set to ``True`` to use a B-spline basis for the functional principal
+        component analysis.
+    n_basis: int, default=None
+        Number of functions in the basis. Only used if `bspline` is `True`.
+    order: int, default=None
+        Order of the splines. One greater than their degree. Only used if
+        `bspline` is `True`.
+    """
 
     def __init__(
         self,
         n_components=10,
         centering=True,
-        regularization=None,
-        components_basis=None,
         bspline=False,
         n_basis=None,
         order=None,
     ):
         self.n_components = n_components
         self.centering = centering
-        self.regularization = regularization
-        self.components_basis = components_basis
         self.bspline = bspline
         self.n_basis = n_basis
         self.order = order
 
         _check_optional_dependency("scikit-fda", "skfda", self)
 
         super(FPCATransformer, self).__init__()
 
-    def fit_transform(self, X, y=None, **fit_params):
+    def fit_transform(self, X, y=None):
         """
         Convert the X to its functional form.
 
         fit the transformer per dimension and transform the X based on the
         number of coefficients
         :param X: A set of time X with the shape N x L x D
         :return: transformed X with top n_components functional principal components
         """
         from skfda import FDataGrid
         from skfda.preprocessing.dim_reduction import FPCA
         from skfda.representation.basis import BSplineBasis
 
-        X, y = self._fit_setup(X, y)
+        X = self._fit_setup(X)
 
         X_t = np.zeros((self.n_instances_, self.n_dims_, self._n_components))
         for j in range(self.n_dims_):
             # represent the time X in functional form
             fd = FDataGrid(X[:, j, :], list(range(self.series_length_)))
 
             # smooth the X if needed
             if self.bspline:
                 basis = BSplineBasis(n_basis=self._n_basis, order=self.order)
                 fd = fd.to_basis(basis)
 
             individual_transformer = FPCA(
                 n_components=self._n_components,
                 centering=self.centering,
-                regularization=self.regularization,
-                components_basis=self.components_basis,
             )
 
             X_t[:, j, :] = individual_transformer.fit_transform(fd)
             self.transformers_.append(individual_transformer)
 
         return X_t
 
     def fit(self, X, y=None):
         from skfda import FDataGrid
         from skfda.preprocessing.dim_reduction import FPCA
         from skfda.representation.basis import BSplineBasis
 
-        X, y = self._fit_setup(X, y)
+        X = self._fit_setup(X)
 
         for j in range(self.n_dims_):
             # represent the time X in functional form
             fd = FDataGrid(X[:, j, :], list(range(self.series_length_)))
 
             # smooth the X if needed
             if self.bspline:
                 basis = BSplineBasis(n_basis=self._n_basis, order=self.order)
                 fd = fd.to_basis(basis)
 
             individual_transformer = FPCA(
                 n_components=self._n_components,
                 centering=self.centering,
-                regularization=self.regularization,
-                components_basis=self.components_basis,
             )
 
             individual_transformer.fit(fd)
             self.transformers_.append(individual_transformer)
 
         return self
 
-    def _fit_setup(self, X, y):
-        X, y = self._validate_data(X=X, y=y, ensure_min_samples=2)
+    def _fit_setup(self, X):
+        X = self._validate_data(X=X, ensure_min_samples=2)
         X = self._convert_X(X)
 
         if self.bspline:
             # n_basis has to be larger or equal to order
             self._n_basis = max(self.n_basis, self.order)
             # n_components has to be less than or equal to n_basis
             self._n_components = min(self.n_basis, self.n_components)
         else:
             self._n_components = self.n_components
 
         self.n_instances_, self.n_dims_, self.series_length_ = X.shape
         self.transformers_ = []
 
-        return X, y
+        return X
 
-    def transform(self, X, y=None):
+    def transform(self, X):
         """
         Transform the X based on the number of coefficients.
 
         :param X: A set of time X with the shape N x L x D
         :return: transformed X with top n_components functional
             principal components
         """
```

### Comparing `tsml-0.1.1/tsml/transformations/_function_transformer.py` & `tsml-0.2.0/tsml/transformations/_function_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """"""
 
 __author__ = ["MatthewMiddlehurst"]
 __all__ = ["FunctionTransformer"]
 
 
 from sklearn.base import TransformerMixin
@@ -95,13 +94,13 @@
         if self.validate:
             X = self._validate_data(X, reset=False, ensure_min_series_length=1)
 
         func = self.func if self.func is not None else _identity
 
         return func(X, **(self.kw_args if self.kw_args else {}))
 
-    def _more_tags(self):
+    def _more_tags(self) -> dict:
         return {
             "no_validation": not self.validate,
             "requires_fit": False,
             "X_types": ["3darray", "2darray", "np_list"],
         }
```

### Comparing `tsml-0.1.1/tsml/transformations/_interval_extraction.py` & `tsml-0.2.0/tsml/transformations/_interval_extraction.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-# -*- coding: utf-8 -*-
 """Random interval features.
 
 A transformer for the extraction of features on randomly selected intervals.
 """
 
 __author__ = ["MatthewMiddlehurst"]
 __all__ = ["RandomIntervalTransformer", "SupervisedIntervalTransformer"]
 
+import inspect
+
 import numpy as np
 from joblib import Parallel
 from sklearn import preprocessing
 from sklearn.base import TransformerMixin
 from sklearn.utils import check_random_state
 from sklearn.utils.fixes import delayed
 from sklearn.utils.validation import check_is_fitted
 
 from tsml.base import BaseTimeSeriesEstimator, _clone_estimator
+from tsml.utils._tags import _safe_tags
 from tsml.utils.numba_functions.general import z_normalise_series_3d
 from tsml.utils.numba_functions.stats import (
     fisher_score,
     row_count_above_mean,
     row_count_mean_crossing,
     row_iqr,
     row_mean,
@@ -37,59 +39,83 @@
 class RandomIntervalTransformer(TransformerMixin, BaseTimeSeriesEstimator):
     """Random interval feature transformer.
 
     Extracts intervals with random length, position and dimension from series in fit.
     Transforms each interval sub-series using the given transformer(s)/features and
     concatenates them into a feature vector in transform.
 
+    Identical intervals are pruned at the end of fit, as such the number of features may
+    be less than expected from n_intervals.
+
     Parameters
     ----------
     n_intervals : int, default=100,
         The number of intervals of random length, position and dimension to be
         extracted.
     min_interval_length : int, default=3
         The minimum length of extracted intervals. Minimum value of 3.
     max_interval_length : int, default=3
         The maximum length of extracted intervals. Minimum value of min_interval_length.
-    features : sktime transformer, a function taking a 2d numpy array parameter, or list
+    features : BaseTransformer, a function taking a 2d numpy array parameter, or list
             of said transformers and functions, default=None
         Transformers and functions used to extract features from selected intervals.
         If None, defaults to [mean, median, min, max, std, 25% quantile, 75% quantile]
-    dilation :
-        add dilation to intervals
-        no dilation if None, add same dilation to all of int, randomly select if list of
-         int
-        -= 1 until min interval
-    random_state : int or None, default=None
-        Seed for random number generation.
+    dilation : int, list or None, default=None
+        Add dilation to extracted intervals. No dilation is added if None or 1. If a
+        list of ints, a random dilation value is selected from the list for each
+        interval.
+
+        The dilation value is selected after the interval star and end points. If the
+        amount of values in the dilated interval is less than the min_interval_length,
+        the amount of dilation applied is reduced.
+    random_state : None, int or instance of RandomState, default=None
+        Seed or RandomState object used for random number generation.
+        If random_state is None, use the RandomState singleton used by np.random.
+        If random_state is an int, use a new RandomState instance seeded with seed.
     n_jobs : int, default=1
-        The number of jobs to run in parallel for both `fit` and `predict`.
-        ``-1`` means using all processors.
+        The number of jobs to run in parallel for both `fit` and `transform` functions.
+        `-1` means using all processors.
     parallel_backend : str, ParallelBackendBase instance or None, default=None
         Specify the parallelisation backend implementation in joblib, if None a 'prefer'
         value of "threads" is used by default.
         Valid options are "loky", "multiprocessing", "threading" or a custom backend.
         See the joblib Parallel documentation for more details.
 
     Attributes
     ----------
     n_instances_ : int
         The number of train cases.
     n_dims_ : int
         The number of dimensions per case.
     series_length_ : int
         The length of each series.
+    n_intervals_ : int
+        The number of intervals extracted after pruning identical intervals.
     intervals_ : list of tuples
         Contains information for each feature extracted in fit. Each tuple contains the
-        interval start, interval end, interval dimension and the feature(s) extracted.
+        interval start, interval end, interval dimension, the feature(s) extracted and
+        the dilation.
         Length will be n_intervals*len(features).
 
     See Also
     --------
-    SupervisedIntervals
+    SupervisedIntervalTransformer
+
+    Examples
+    --------
+    >>> from tsml.transformations import RandomIntervalTransformer
+    >>> from tsml.utils.testing import generate_3d_test_data
+    >>> X, _ = generate_3d_test_data(n_samples=4, series_length=12, random_state=0)
+    >>> tnf = RandomIntervalTransformer(n_intervals=2, random_state=0)
+    >>> tnf.fit(X)
+    RandomIntervalTransformer(...)
+    >>> print(tnf.transform(X)[0])
+    [1.04753424 0.14925939 0.8473096  1.20552675 1.08976637 0.96853798
+     1.14764656 1.07628806 0.18170775 0.8473096  1.29178823 1.08976637
+     0.96853798 1.1907773 ]
     """
 
     def __init__(
         self,
         n_intervals=100,
         min_interval_length=3,
         max_interval_length=np.inf,
@@ -109,133 +135,99 @@
         self.parallel_backend = parallel_backend
 
         super(RandomIntervalTransformer, self).__init__()
 
     transformer_feature_skip = ["transform_features_", "_transform_features"]
 
     def fit_transform(self, X, y=None):
-        """Fit to data, then transform it.
-
-        Fits the transformer to X and y and returns a transformed version of X.
-
-        State change:
-            Changes state to "fitted".
-
-        Writes to self:
-        _is_fitted : flag is set to True.
-        _X : X, coerced copy of X, if remember_data tag is True
-            possibly coerced to inner type or update_data compatible type
-            by reference, when possible
-        model attributes (ending in "_") : dependent on estimator
-
-        Parameters
-        ----------
-        X : Series or Panel, any supported mtype
-            Data to be transformed, of python type as follows:
-                Series: pd.Series, pd.DataFrame, or np.ndarray (1D or 2D)
-                Panel: pd.DataFrame with 2-level MultiIndex, list of pd.DataFrame,
-                    nested pd.DataFrame, or pd.DataFrame in long/wide format
-                subject to sktime mtype format specifications, for further details see
-                    examples/AA_datatypes_and_datasets.ipynb
-        y : Series or Panel, default=None
-            Additional data, e.g., labels for transformation
-
-        Returns
-        -------
-        transformed version of X
-        type depends on type of X and scitype:transform-output tag:
-            |   `X`    | `tf-output`  |     type of return     |
-            |----------|--------------|------------------------|
-            | `Series` | `Primitives` | `pd.DataFrame` (1-row) |
-            | `Panel`  | `Primitives` | `pd.DataFrame`         |
-            | `Series` | `Series`     | `Series`               |
-            | `Panel`  | `Series`     | `Panel`                |
-            | `Series` | `Panel`      | `Panel`                |
-        instances in return correspond to instances in `X`
-        combinations not in the table are currently not supported
-
-        Explicitly, with examples:
-            if `X` is `Series` (e.g., `pd.DataFrame`) and `transform-output` is `Series`
-                then the return is a single `Series` of the same mtype
-                Example: detrending a single series
-            if `X` is `Panel` (e.g., `pd-multiindex`) and `transform-output` is `Series`
-                then the return is `Panel` with same number of instances as `X`
-                    (the transformer is applied to each input Series instance)
-                Example: all series in the panel are detrended individually
-            if `X` is `Series` or `Panel` and `transform-output` is `Primitives`
-                then the return is `pd.DataFrame` with as many rows as instances in `X`
-                Example: i-th row of the return has mean and variance of the i-th series
-            if `X` is `Series` and `transform-output` is `Panel`
-                then the return is a `Panel` object of type `pd-multiindex`
-                Example: i-th instance of the output is the i-th window running over `X`
-        """
-        X, y = self._fit_setup(X, y)
+        X, rng = self._fit_setup(X)
 
         fit = Parallel(
             n_jobs=self._n_jobs, backend=self.parallel_backend, prefer="threads"
         )(
             delayed(self._generate_interval)(
                 X,
                 y,
-                i,
+                rng.randint(np.iinfo(np.int32).max),
                 True,
             )
-            for i in range(self.n_intervals)
+            for _ in range(self.n_intervals)
         )
 
         (
             intervals,
             transformed_intervals,
         ) = zip(*fit)
 
-        for i in intervals:
-            self.intervals_.extend(i)
+        current = []
+        removed_idx = []
+        self.n_intervals_ = 0
+        for i, interval in enumerate(intervals):
+            new_interval = (
+                interval[0][0],
+                interval[0][1],
+                interval[0][2],
+                interval[0][4],
+            )
+            if new_interval not in current:
+                current.append(new_interval)
+                self.intervals_.extend(interval)
+                self.n_intervals_ += 1
+            else:
+                removed_idx.append(i)
 
         Xt = transformed_intervals[0]
         for i in range(1, self.n_intervals):
-            Xt = np.hstack((Xt, transformed_intervals[i]))
+            if i not in removed_idx:
+                Xt = np.hstack((Xt, transformed_intervals[i]))
 
         return Xt
 
     def fit(self, X, y=None):
-        X, y = self._fit_setup(X, y)
+        X, rng = self._fit_setup(X)
 
         fit = Parallel(
             n_jobs=self._n_jobs, backend=self.parallel_backend, prefer="threads"
         )(
             delayed(self._generate_interval)(
                 X,
                 y,
-                i,
+                rng.randint(np.iinfo(np.int32).max),
                 False,
             )
-            for i in range(self.n_intervals)
+            for _ in range(self.n_intervals)
         )
 
         (
             intervals,
             _,
         ) = zip(*fit)
 
+        current = []
+        self.n_intervals_ = 0
         for i in intervals:
-            self.intervals_.extend(i)
+            interval = (i[0][0], i[0][1], i[0][2], i[0][4])
+            if interval not in current:
+                current.append(interval)
+                self.intervals_.extend(i)
+                self.n_intervals_ += 1
 
         return self
 
     def transform(self, X, y=None):
         check_is_fitted(self)
 
         X = self._validate_data(X=X, reset=False, ensure_min_series_length=3)
 
         if self._transform_features is None:
             transform_features = [None] * len(self.intervals_)
         else:
             count = 0
             transform_features = []
-            for _ in range(self.n_intervals):
+            for _ in range(self.n_intervals_):
                 for feature in self._features:
                     if is_transformer(feature):
                         nf = feature.n_transformed_features
                         transform_features.append(
                             self._transform_features[count : count + nf]
                         )
                         count += nf
@@ -256,16 +248,16 @@
 
         Xt = transform[0]
         for i in range(1, len(self.intervals_)):
             Xt = np.hstack((Xt, transform[i]))
 
         return Xt
 
-    def _fit_setup(self, X, y):
-        X, y = self._validate_data(X=X, y=y, ensure_min_series_length=3)
+    def _fit_setup(self, X):
+        X = self._validate_data(X=X, ensure_min_series_length=3)
         X = self._convert_X(X)
 
         self.intervals_ = []
         self._transform_features = None
 
         self.n_instances_, self.n_dims_, self.series_length_ = X.shape
 
@@ -301,36 +293,34 @@
                         feature,
                         self.random_state,
                     )
                 )
             elif callable(feature):
                 li.append(feature)
             else:
-                raise ValueError()  # todo
+                raise ValueError(
+                    "Input features must be a list of callables or aeon transformers."
+                )
         self._features = li
 
         if self.dilation is None:
             self._dilation = [1]
         elif isinstance(self.dilation, list):
             self._dilation = self.dilation
         else:
             self._dilation = [self.dilation]
 
         self._n_jobs = check_n_jobs(self.n_jobs)
 
-        return X, y
+        rng = check_random_state(self.random_state)
 
-    def _generate_interval(self, X, y, idx, transform):
-        rs = 255 if self.random_state == 0 else self.random_state
-        rs = (
-            None
-            if self.random_state is None
-            else (rs * 37 * (idx + 1)) % np.iinfo(np.int32).max
-        )
-        rng = check_random_state(rs)
+        return X, rng
+
+    def _generate_interval(self, X, y, seed, transform):
+        rng = check_random_state(seed)
 
         dim = rng.randint(self.n_dims_)
 
         if rng.random() < 0.5:
             interval_start = (
                 rng.randint(0, self.series_length_ - self._min_interval_length)
                 if self.series_length_ > self._min_interval_length
@@ -372,15 +362,15 @@
         intervals = []
 
         for feature in self._features:
             if is_transformer(feature):
                 if transform:
                     feature = _clone_estimator(
                         feature,
-                        rs,
+                        seed,
                     )
 
                     t = feature.fit_transform(
                         np.expand_dims(
                             X[:, dim, interval_start:interval_end:dilation], axis=1
                         ),
                         y,
@@ -460,27 +450,26 @@
         for feature in self._features:
             if is_transformer(feature):
                 if not any(
                     hasattr(feature, n) for n in self.transformer_feature_skip
                 ) or not hasattr(feature, "n_transformed_features"):
                     if raise_error:
                         raise ValueError(
-                            "Transformer must have one of {} as an attribute and a "
-                            "n_transformed_features attribute.".format(
-                                self.transformer_feature_skip
-                            )
+                            "Transformer must have one of "
+                            f"{self.transformer_feature_skip} as an attribute and "
+                            "a n_transformed_features attribute."
                         )
                     else:
                         return False
 
                 length += feature.n_transformed_features
             else:
                 length += 1
 
-        if len(arr) != length * self.n_intervals or not all(
+        if len(arr) != length * self.n_intervals_ or not all(
             isinstance(b, bool) for b in arr
         ):
             if raise_error:
                 raise ValueError(
                     "Input must be a list bools, matching the length of the transform "
                     "output."
                 )
@@ -512,48 +501,59 @@
         return {"n_intervals": 2}
 
 
 class SupervisedIntervalTransformer(TransformerMixin, BaseTimeSeriesEstimator):
     """Supervised interval feature transformer.
 
     Extracts intervals in fit using the supervised process described in [1].
-    Interval sub-series are extracted for each input feature, and the usefulness of that
+    Interval subseries are extracted for each input feature, and the usefulness of that
     feature extracted on an interval is evaluated using the Fisher score metric.
     Intervals are continually split in half, with the better scoring half retained as a
     feature for the transform.
 
     Multivariate capability is added by running the supervised interval extraction
     process on each dimension of the input data.
 
-    As the extracted interval features are already extracted for the supervised
+    As the interval features are already extracted for the supervised
     evaluation in fit, the fit_transform method is recommended if the transformed fit
     data is required.
 
     Parameters
     ----------
     n_intervals : int, default=50
         The number of times the supervised interval selection process is run.
         Each supervised extraction will output a varying amount of features based on
         series length, number of dimensions and the number of features.
     min_interval_length : int, default=3
         The minimum length of extracted intervals. Minimum value of 3.
-    features : function with a single 2d array-like parameter or list of said functions,
-            default=None
-        Functions used to extract features from selected intervals. If None, defaults to
-        the following statistics used in [2]:
+    features : callable, list of callables, default=None
+        Functions used to extract features from selected intervals. Must take a 2d
+        array of shape (n_instances, interval_length) and return a 1d array of shape
+        (n_instances) containing the features.
+        If None, defaults to the following statistics used in [2]:
         [mean, median, std, slope, min, max, iqr, count_mean_crossing,
         count_above_mean].
+    metric : ["fisher"] or callable, default="fisher"
+        The metric used to evaluate the usefulness of a feature extracted on an
+        interval. If "fisher", the Fisher score is used. If a callable, it must take
+        a 1d array of shape (n_instances) and return a 1d array of scores of shape
+        (n_instances).
     randomised_split_point : bool, default=True
         If True, the split point for interval extraction is randomised as is done in [2]
         rather than split in half.
+    normalise_for_search : bool, default=True
+        If True, the data is normalised for the supervised interval search process.
+        Features extracted for the transform output will not use normalised data.
+    random_state : None, int or instance of RandomState, default=None
+        Seed or RandomState object used for random number generation.
+        If random_state is None, use the RandomState singleton used by np.random.
+        If random_state is an int, use a new RandomState instance seeded with seed.
     n_jobs : int, default=1
-        The number of jobs to run in parallel for both `fit` and `transform`.
-        ``-1`` means using all processors.
-    random_state : int or None, default=None
-        Seed for random number generation.
+        The number of jobs to run in parallel for both `fit` and `transform` functions.
+        `-1` means using all processors.
     parallel_backend : str, ParallelBackendBase instance or None, default=None
         Specify the parallelisation backend implementation in joblib, if None a 'prefer'
         value of "threads" is used by default.
         Valid options are "loky", "multiprocessing", "threading" or a custom backend.
         See the joblib Parallel documentation for more details.
 
     Attributes
@@ -583,107 +583,77 @@
         accurate time series classification through supervised interval search. In 2020
         IEEE International Conference on Data Mining (ICDM) (pp. 948-953). IEEE.
     .. [2] Cabello, N., Naghizade, E., Qi, J. and Kulik, L., 2021. Fast, accurate and
         interpretable time series classification through randomization. arXiv preprint
         arXiv:2105.14876.
 
     Examples
+    --------
+    >>> from tsml.transformations import SupervisedIntervalTransformer
+    >>> from tsml.utils.testing import generate_3d_test_data
+    >>> X, y = generate_3d_test_data(n_samples=10, series_length=12, random_state=0)
+    >>> tnf = SupervisedIntervalTransformer(n_intervals=1, random_state=0)
+    >>> tnf.fit(X, y)
+    SupervisedIntervalTransformer(...)
+    >>> print(tnf.transform(X)[0])
+    [1.4237989  1.20552675 0.45060352 0.13125638 0.10101093 0.76688304
+     1.92732552 0.54651945 3.         2.        ]
     """
 
     def __init__(
         self,
         n_intervals=50,
         min_interval_length=3,
         features=None,
+        metric="fisher",
         randomised_split_point=True,
+        normalise_for_search=True,
         random_state=None,
         n_jobs=1,
         parallel_backend=None,
     ):
         self.n_intervals = n_intervals
         self.min_interval_length = min_interval_length
         self.features = features
+        self.metric = metric
         self.randomised_split_point = randomised_split_point
+        self.normalise_for_search = normalise_for_search
         self.random_state = random_state
         self.n_jobs = n_jobs
         self.parallel_backend = parallel_backend
 
         super(SupervisedIntervalTransformer, self).__init__()
 
-    def fit_transform(self, X, y=None):
-        """Fit to data, then transform it.
-
-        Fits the transformer to X and y and returns a transformed version of X.
-
-        State change:
-            Changes state to "fitted".
-
-        Writes to self:
-        _is_fitted : flag is set to True.
-        _X : X, coerced copy of X, if remember_data tag is True
-            possibly coerced to inner type or update_data compatible type
-            by reference, when possible
-        model attributes (ending in "_") : dependent on estimator
-
-        Parameters
-        ----------
-        X : Series or Panel, any supported mtype
-            Data to be transformed, of python type as follows:
-                Series: pd.Series, pd.DataFrame, or np.ndarray (1D or 2D)
-                Panel: pd.DataFrame with 2-level MultiIndex, list of pd.DataFrame,
-                    nested pd.DataFrame, or pd.DataFrame in long/wide format
-                subject to sktime mtype format specifications, for further details see
-                    examples/AA_datatypes_and_datasets.ipynb
-        y : Series or Panel, default=None
-            Additional data, e.g., labels for transformation
+    # if features contains a transformer, it must contain a parameter name from
+    # transformer_feature_selection and an attribute name (or property) from
+    # transformer_feature_names to allow a single feature to be transformed at a time.
+    transformer_feature_selection = ["features"]
+    transformer_feature_names = [
+        "features_arguments_",
+        "_features_arguments",
+        "get_features_arguments",
+        "_get_features_arguments",
+    ]
 
-        Returns
-        -------
-        transformed version of X
-        type depends on type of X and scitype:transform-output tag:
-            |   `X`    | `tf-output`  |     type of return     |
-            |----------|--------------|------------------------|
-            | `Series` | `Primitives` | `pd.DataFrame` (1-row) |
-            | `Panel`  | `Primitives` | `pd.DataFrame`         |
-            | `Series` | `Series`     | `Series`               |
-            | `Panel`  | `Series`     | `Panel`                |
-            | `Series` | `Panel`      | `Panel`                |
-        instances in return correspond to instances in `X`
-        combinations not in the table are currently not supported
-
-        Explicitly, with examples:
-            if `X` is `Series` (e.g., `pd.DataFrame`) and `transform-output` is `Series`
-                then the return is a single `Series` of the same mtype
-                Example: detrending a single series
-            if `X` is `Panel` (e.g., `pd-multiindex`) and `transform-output` is `Series`
-                then the return is `Panel` with same number of instances as `X`
-                    (the transformer is applied to each input Series instance)
-                Example: all series in the panel are detrended individually
-            if `X` is `Series` or `Panel` and `transform-output` is `Primitives`
-                then the return is `pd.DataFrame` with as many rows as instances in `X`
-                Example: i-th row of the return has mean and variance of the i-th series
-            if `X` is `Series` and `transform-output` is `Panel`
-                then the return is a `Panel` object of type `pd-multiindex`
-                Example: i-th instance of the output is the i-th window running over `X`
-        """
-        X, y = self._fit_setup(X, y)
+    def fit_transform(self, X, y=None):
+        X, y, rng = self._fit_setup(X, y)
 
-        X_norm = z_normalise_series_3d(X)
+        X_norm = z_normalise_series_3d(X) if self.normalise_for_search else X
 
         fit = Parallel(
             n_jobs=self._n_jobs, backend=self.parallel_backend, prefer="threads"
         )(
             delayed(self._generate_intervals)(
                 X,
                 X_norm,
                 y,
-                i,
+                rng.randint(np.iinfo(np.int32).max),
                 True,
             )
-            for i in range(self.n_intervals)
+            for _ in range(self.n_intervals)
         )
 
         (
             intervals,
             transformed_intervals,
         ) = zip(*fit)
 
@@ -695,29 +665,29 @@
         Xt = transformed_intervals[0]
         for i in range(1, self.n_intervals):
             Xt = np.hstack((Xt, transformed_intervals[i]))
 
         return Xt
 
     def fit(self, X, y=None):
-        X, y = self._fit_setup(X, y)
+        X, y, rng = self._fit_setup(X, y)
 
-        X_norm = z_normalise_series_3d(X)
+        X_norm = z_normalise_series_3d(X) if self.normalise_for_search else X
 
         fit = Parallel(
             n_jobs=self._n_jobs, backend=self.parallel_backend, prefer="threads"
         )(
             delayed(self._generate_intervals)(
                 X,
                 X_norm,
                 y,
-                i,
+                rng.randint(np.iinfo(np.int32).max),
                 False,
             )
-            for i in range(self.n_intervals)
+            for _ in range(self.n_intervals)
         )
 
         (
             intervals,
             _,
         ) = zip(*fit)
 
@@ -783,38 +753,80 @@
                 row_numba_min,
                 row_numba_max,
                 row_iqr,
                 row_count_mean_crossing,
                 row_count_above_mean,
             ]
 
-        li = []
         if not isinstance(self._features, list):
             self._features = [self._features]
 
+        rng = check_random_state(self.random_state)
+
+        msg = (
+            "Transformers must have a parameter from 'transformer_feature_names' to "
+            "allow selecting single features, and a list of feature names in "
+            "'transformer_feature_names'. Transformers which require 'fit' are "
+            "currently unsupported."
+        )
+
+        li = []
         for f in self._features:
             if callable(f):
                 li.append(f)
+            elif is_transformer(f):
+                if _safe_tags(f, key="requires_fit") is True:
+                    raise ValueError(msg)
+
+                params = inspect.signature(f.__init__).parameters
+
+                att_name = None
+                for n in self.transformer_feature_selection:
+                    if params.get(n, None) is not None:
+                        att_name = n
+                        break
+
+                if att_name is None:
+                    raise ValueError(msg)
+
+                t_features = None
+                for n in self.transformer_feature_names:
+                    if hasattr(f, n) and isinstance(getattr(f, n), (list, tuple)):
+                        t_features = getattr(f, n)
+                        break
+
+                if t_features is None:
+                    raise ValueError(msg)
+
+                for t_f in t_features:
+                    new_transformer = _clone_estimator(f, rng)
+                    setattr(
+                        new_transformer,
+                        att_name,
+                        t_f,
+                    )
+                    li.append(new_transformer)
             else:
                 raise ValueError()
         self._features = li
 
+        if callable(self.metric):
+            self._metric = self.metric
+        elif self.metric == "fisher":
+            self._metric = fisher_score
+        else:
+            raise ValueError("metric must be callable or 'fisher'")
+
         self._n_jobs = check_n_jobs(self.n_jobs)
 
         le = preprocessing.LabelEncoder()
-        return X, le.fit_transform(y)
+        return X, le.fit_transform(y), rng
 
-    def _generate_intervals(self, X, X_norm, y, idx, keep_transform):
-        rs = 255 if self.random_state == 0 else self.random_state
-        rs = (
-            None
-            if self.random_state is None
-            else (rs * 37 * (idx + 1)) % np.iinfo(np.int32).max
-        )
-        rng = check_random_state(rs)
+    def _generate_intervals(self, X, X_norm, y, seed, keep_transform):
+        rng = check_random_state(seed)
 
         Xt = np.empty((self.n_instances_, 0)) if keep_transform else None
         intervals = []
 
         for i in range(self.n_dims_):
             for feature in self._features:
                 random_cut_point = int(rng.randint(1, self.series_length_ - 1))
@@ -831,14 +843,15 @@
                     y,
                     0,
                     feature,
                     i,
                     X[:, i, :],
                     rng,
                     keep_transform,
+                    is_transformer(feature),
                 )
                 intervals.extend(intervals_L)
 
                 if keep_transform:
                     Xt = np.hstack((Xt, Xt_L))
 
                 intervals_R, Xt_R = self._supervised_search(
@@ -846,31 +859,45 @@
                     y,
                     random_cut_point,
                     feature,
                     i,
                     X[:, i, :],
                     rng,
                     keep_transform,
+                    is_transformer(feature),
                 )
                 intervals.extend(intervals_R)
 
                 if keep_transform:
                     Xt = np.hstack((Xt, Xt_R))
 
         return intervals, Xt
 
     def _transform_intervals(self, X, idx):
         if not self._transform_features[idx]:
             return np.zeros(X.shape[0])
 
         start, end, dim, feature = self.intervals_[idx]
-        return feature(X[:, dim, start:end])
+
+        if is_transformer(feature):
+            return feature.transform(X[:, dim, start:end]).flatten()
+        else:
+            return feature(X[:, dim, start:end])
 
     def _supervised_search(
-        self, X, y, ini_idx, feature, dim, X_ori, rng, keep_transform
+        self,
+        X,
+        y,
+        ini_idx,
+        feature,
+        dim,
+        X_ori,
+        rng,
+        keep_transform,
+        feature_is_transformer,
     ):
         intervals = []
         Xt = np.empty((X.shape[0], 0)) if keep_transform else None
 
         while X.shape[1] >= self._min_interval_length * 2:
             if (
                 self.randomised_split_point
@@ -881,28 +908,41 @@
                 )
             else:
                 div_point = int(X.shape[1] / 2)
 
             sub_interval_0 = X[:, :div_point]
             sub_interval_1 = X[:, div_point:]
 
-            interval_feature_0 = feature(sub_interval_0)
-            interval_feature_1 = feature(sub_interval_1)
+            if feature_is_transformer:
+                interval_feature_0 = feature.transform(sub_interval_0).flatten()
+                interval_feature_1 = feature.transform(sub_interval_1).flatten()
+            else:
+                interval_feature_0 = feature(sub_interval_0)
+                interval_feature_1 = feature(sub_interval_1)
 
-            score_0 = fisher_score(interval_feature_0, y)
-            score_1 = fisher_score(interval_feature_1, y)
+            score_0 = self._metric(interval_feature_0, y)
+            score_1 = self._metric(interval_feature_1, y)
 
             if score_0 >= score_1 and score_0 != 0:
                 end = ini_idx + len(sub_interval_0[0])
 
                 intervals.append((ini_idx, end, dim, feature))
                 X = sub_interval_0
 
-                interval_feature_to_use = feature(X_ori[:, ini_idx:end])
                 if keep_transform:
+                    if self.normalise_for_search:
+                        if feature_is_transformer:
+                            interval_feature_to_use = feature.transform(
+                                X_ori[:, ini_idx:end]
+                            ).flatten()
+                        else:
+                            interval_feature_to_use = feature(X_ori[:, ini_idx:end])
+                    else:
+                        interval_feature_to_use = interval_feature_0
+
                     Xt = np.hstack(
                         (
                             Xt,
                             np.reshape(
                                 interval_feature_to_use,
                                 (interval_feature_to_use.shape[0], 1),
                             ),
@@ -911,16 +951,25 @@
             elif score_1 > score_0:
                 ini_idx = ini_idx + div_point
                 end = ini_idx + len(sub_interval_1[0])
 
                 intervals.append((ini_idx, end, dim, feature))
                 X = sub_interval_1
 
-                interval_feature_to_use = feature(X_ori[:, ini_idx:end])
                 if keep_transform:
+                    if self.normalise_for_search:
+                        if feature_is_transformer:
+                            interval_feature_to_use = feature.transform(
+                                X_ori[:, ini_idx:end]
+                            ).flatten()
+                        else:
+                            interval_feature_to_use = feature(X_ori[:, ini_idx:end])
+                    else:
+                        interval_feature_to_use = interval_feature_1
+
                     Xt = np.hstack(
                         (
                             Xt,
                             np.reshape(
                                 interval_feature_to_use,
                                 (interval_feature_to_use.shape[0], 1),
                             ),
@@ -959,14 +1008,17 @@
             else:
                 return False
 
         self._transform_features = arr
 
         return True
 
+    def _more_tags(self) -> dict:
+        return {"requires_y": True}
+
     @classmethod
     def get_test_params(cls, parameter_set="default"):
         """Return testing parameter settings for the estimator.
 
         Parameters
         ----------
         parameter_set : str, default="default"
```

### Comparing `tsml-0.1.1/tsml/transformations/_sfa.py` & `tsml-0.2.0/tsml/transformations/_sfa.py`

 * *Files identical despite different names*

### Comparing `tsml-0.1.1/tsml/transformations/_shapelet_transform.py` & `tsml-0.2.0/tsml/hybrid/_rist.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,719 +1,612 @@
-# -*- coding: utf-8 -*-
-"""Shapelet transformers.
-
-A transformer from the time domain into the shapelet domain.
-"""
+"""Randomised Interval-Shapelet Transformation (RIST) pipeline estimators."""
 
 __author__ = ["MatthewMiddlehurst"]
-__all__ = ["RandomShapeletTransformer"]
 
-import heapq
-import math
-import time
+from typing import List, Union
 
 import numpy as np
-from joblib import Parallel
-from numba import njit
-from numba.typed.typedlist import List
-from sklearn import preprocessing
-from sklearn.base import TransformerMixin
-from sklearn.utils import check_random_state
-from sklearn.utils.fixes import delayed
-from sklearn.utils.validation import check_is_fitted
-
-from tsml.base import BaseTimeSeriesEstimator
-from tsml.utils.numba_functions.general import z_normalise_series
-from tsml.utils.validation import check_n_jobs
-
-
-class RandomShapeletTransformer(TransformerMixin, BaseTimeSeriesEstimator):
-    """Random Shapelet Transform.
-
-    Implementation of the binary shapelet transform along the lines of [1]_[2]_, with
-    randomly extracted shapelets.
-
-    Overview: Input "n" series with "d" dimensions of length "m". Continuously extract
-    candidate shapelets and filter them in batches.
-        For each candidate shapelet
-            - Extract a shapelet from an instance with random length, position and
-              dimension
-            - Using its distance to train cases, calculate the shapelets information
-              gain
-            - Abandon evaluating the shapelet if it is impossible to obtain a higher
-              information gain than the current worst
-        For each shapelet batch
-            - Add each candidate to its classes shapelet heap, removing the lowest
-              information gain shapelet if the max number of shapelets has been met
-            - Remove self-similar shapelets from the heap
-    Using the final set of filtered shapelets, transform the data into a vector of
-    of distances from a series to each shapelet.
+from sklearn.base import ClassifierMixin, RegressorMixin
+from sklearn.ensemble import ExtraTreesClassifier, ExtraTreesRegressor
+from sklearn.ensemble._base import _set_random_states
+from sklearn.utils.validation import check_is_fitted, check_random_state
+
+from tsml.base import BaseTimeSeriesEstimator, _clone_estimator
+from tsml.transformations import (
+    ARCoefficientTransformer,
+    Catch22Transformer,
+    FunctionTransformer,
+    PeriodogramTransformer,
+    RandomDilatedShapeletTransformer,
+    RandomIntervalTransformer,
+)
+from tsml.utils.numba_functions.general import first_order_differences_3d
+from tsml.utils.numba_functions.stats import (
+    row_iqr,
+    row_mean,
+    row_median,
+    row_numba_max,
+    row_numba_min,
+    row_ppv,
+    row_slope,
+    row_std,
+)
+from tsml.utils.validation import _check_optional_dependency, check_n_jobs
+
+
+class RISTClassifier(ClassifierMixin, BaseTimeSeriesEstimator):
+    """Randomised Interval-Shapelet Transformation (RIST) pipeline classifier.
+
+    This classifier is a hybrid pipeline using the RandomIntervalTransformer using
+    Catch22 features and summary stats, and the RandomDilatedShapeletTransformer.
+    Both transforms extract features from different series transformations (1st Order
+    Differences, PeriodogramTransformer, and ARCoefficientTransformer).
+    An ExtraTreesClassifier with 200 trees is used as the estimator for the
+    concatenated feature vector output.
 
     Parameters
     ----------
-    n_shapelet_samples : int, default=10000
-        The number of candidate shapelets to be considered for the final transform.
-        Filtered down to <= max_shapelets, keeping the shapelets with the most
-        information gain.
-    max_shapelets : int or None, default=None
-        Max number of shapelets to keep for the final transform. Each class value will
-        have its own max, set to n_classes / max_shapelets. If None uses the min between
-        10 * n_instances and 1000
-    min_shapelet_length : int, default=3
-        Lower bound on candidate shapelet lengths.
-    max_shapelet_length : int or None, default= None
-        Upper bound on candidate shapelet lengths. If None no max length is used.
-    remove_self_similar : boolean, default=True
-        Remove overlapping "self-similar" shapelets when merging candidate shapelets.
-    time_limit_in_minutes : int, default=0
-        Time contract to limit build time in minutes, overriding n_shapelet_samples.
-        Default of 0 means n_shapelet_samples is used.
-    contract_max_n_shapelet_samples : int, default=np.inf
-        Max number of shapelets to extract when time_limit_in_minutes is set.
+    n_intervals : int, callable or None, default=None,
+        The number of intervals of random length, position and dimension to be
+        extracted for the interval portion of the pipeline. Input should be an int or
+        a function that takes a 3D np.ndarray input and returns an int. Functions may
+        extract a different number of intervals per `series_transformer` output.
+        If None, extracts `int(np.sqrt(X.shape[2]) * np.sqrt(X.shape[1]) * 15 + 5)`
+        intervals where `Xt` is the series representation data.
+    n_shapelets : int, callable or None, default=None,
+        The number of shapelets of random dilation and position to be extracted for the
+        shapelet portion of the pipeline. Input should be an int or
+        a function that takes a 3D np.ndarray input and returns an int. Functions may
+        extract a different number of shapelets per `series_transformer` output.
+        If None, extracts `int(np.sqrt(Xt.shape[2]) * 200 + 5)` shapelets where `Xt` is
+        the series representation data.
+    series_transformers : TransformerMixin, list, tuple, or None, default=None
+        The transformers to apply to the series before extracting intervals and
+        shapelets. If None, use the series as is. If "default", use [None, 1st Order
+        Differences, PeriodogramTransformer, and ARCoefficientTransformer].
+
+        A list or tuple of transformers will extract intervals from
+        all transformations concatenate the output. Including None in the list or tuple
+        will use the series as is for interval extraction.
+    use_pycatch22 : bool, optional, default=True
+        Wraps the C based pycatch22 implementation for aeon.
+        (https://github.com/DynamicsAndNeuralSystems/pycatch22). This requires the
+        ``pycatch22`` package to be installed if True.
+    use_pyfftw : bool, default=True
+        Whether to use the pyfftw library for FFT calculations. Requires the pyfftw
+        package to be installed.
+    estimator : sklearn classifier, default=None
+        An sklearn estimator to be built using the transformed data. Defaults to an
+        ExtraTreesClassifier with 200 trees.
+    random_state : int, RandomState instance or None, default=None
+        If `int`, random_state is the seed used by the random number generator;
+        If `RandomState` instance, random_state is the random number generator;
+        If `None`, the random number generator is the `RandomState` instance used
+        by `np.random`.
     n_jobs : int, default=1
-        The number of jobs to run in parallel for both `fit` and `transform`.
+        The number of jobs to run in parallel for both `fit` and `predict`.
         ``-1`` means using all processors.
-    parallel_backend : str, ParallelBackendBase instance or None, default=None
-        Specify the parallelisation backend implementation in joblib, if None a 'prefer'
-        value of "threads" is used by default.
-        Valid options are "loky", "multiprocessing", "threading" or a custom backend.
-        See the joblib Parallel documentation for more details.
-    batch_size : int or None, default=100
-        Number of shapelet candidates processed before being merged into the set of best
-        shapelets.
-    random_state : int or None, default=None
-        Seed for random number generation.
 
     Attributes
     ----------
-    n_classes_ : int
-        The number of classes.
     n_instances_ : int
-        The number of train cases.
-    n_dims_ : int
-        The number of dimensions per case.
-    series_length_ : int
-        The length of each series.
-    classes_ : list
-        The classes labels.
-    shapelets_ : list
-        The stored shapelets and relating information after a dataset has been
-        processed.
-        Each item in the list is a tuple containing the following 7 items:
-        (shapelet information gain, shapelet length, start position the shapelet was
-        extracted from, shapelet dimension, index of the instance the shapelet was
-        extracted from in fit, class value of the shapelet, The z-normalised shapelet
-        array)
+        The number of train cases in the training set.
+    n_channels_ : int
+        The number of dimensions per case in the training set.
+    n_timepoints_ : int
+        The length of each series in the training set.
+    n_classes_ : int
+        Number of classes. Extracted from the data.
+    classes_ : ndarray of shape (n_classes_)
+        Holds the label for each class.
+    class_dictionary_ : dict
+        A dictionary mapping class labels to class indices in classes_.
 
     See Also
     --------
-    ShapeletTransformClassifier
-
-    Notes
-    -----
-    For the Java version, see
-    `TSML <https://github.com/uea-machine-learning/tsml/blob/master/src/main/
-    java/tsml/transformers/ShapeletTransform.java>`_.
-
-    References
-    ----------
-    .. [1] Jon Hills et al., "Classification of time series by shapelet transformation",
-       Data Mining and Knowledge Discovery, 28(4), 851--881, 2014.
-    .. [2] A. Bostrom and A. Bagnall, "Binary Shapelet Transform for Multiclass Time
-       Series Classification", Transactions on Large-Scale Data and Knowledge Centered
-       Systems, 32, 2017.
+    RandomIntervalTransformer
+    RandomDilatedShapeletTransformer
+    RISTRegressor
 
     Examples
     --------
-    >>> from tsml.transformations._shapelet_transform import RandomShapeletTransformer
-    >>> from tsml.datasets import load_minimal_chinatown
-    >>> X_train, y_train = load_minimal_chinatown(split="train")
-    >>> t = RandomShapeletTransformer(
-    ...     n_shapelet_samples=500,
-    ...     max_shapelets=10,
-    ...     batch_size=100,
-    ... )
-    >>> t.fit(X_train, y_train)
-    RandomShapeletTransformer(...)
-    >>> X_t = t.transform(X_train)
+    >>> from tsml.hybrid import RISTClassifier
+    >>> from tsml.utils.testing import generate_3d_test_data
+    >>> X, y = generate_3d_test_data(n_samples=8, series_length=10, random_state=0)
+    >>> clf = RISTClassifier(random_state=0)
+    >>> clf.fit(X, y)
+    RISTClassifier(...)
+    >>> clf.predict(X)
+    array([0, 1, 1, 0, 0, 1, 0, 1])
     """
 
     def __init__(
         self,
-        n_shapelet_samples=10000,
-        max_shapelets=None,
-        min_shapelet_length=3,
-        max_shapelet_length=None,
-        remove_self_similar=True,
-        time_limit_in_minutes=0.0,
-        contract_max_n_shapelet_samples=np.inf,
+        n_intervals=None,
+        n_shapelets=None,
+        series_transformers="default",
+        use_pycatch22=True,
+        use_pyfftw=True,
+        estimator=None,
         n_jobs=1,
-        parallel_backend=None,
-        batch_size=100,
         random_state=None,
     ):
-        self.n_shapelet_samples = n_shapelet_samples
-        self.max_shapelets = max_shapelets
-        self.min_shapelet_length = min_shapelet_length
-        self.max_shapelet_length = max_shapelet_length
-        self.remove_self_similar = remove_self_similar
-
-        self.time_limit_in_minutes = time_limit_in_minutes
-        self.contract_max_n_shapelet_samples = contract_max_n_shapelet_samples
-
-        self.n_jobs = n_jobs
-        self.parallel_backend = parallel_backend
-        self.batch_size = batch_size
+        self.n_intervals = n_intervals
+        self.n_shapelets = n_shapelets
+        self.series_transformers = series_transformers
+        self.use_pycatch22 = use_pycatch22
+        self.use_pyfftw = use_pyfftw
+        self.estimator = estimator
         self.random_state = random_state
+        self.n_jobs = n_jobs
 
-        super(RandomShapeletTransformer, self).__init__()
+        if use_pycatch22:
+            _check_optional_dependency("pycatch22", "pycatch22", self)
+        if use_pyfftw:
+            _check_optional_dependency("pyfftw", "pyfftw", self)
 
-    def fit(self, X, y=None):
-        """Fit the shapelet transform to a specified X and y.
+        super(RISTClassifier, self).__init__()
+
+    def fit(self, X: Union[np.ndarray, List[np.ndarray]], y: np.ndarray) -> object:
+        """Fit the estimator to training data.
 
         Parameters
         ----------
-        X: pandas DataFrame or np.ndarray
-            The training input samples.
-        y: array-like or list
-            The class values for X.
+        X : 3D np.ndarray of shape (n_instances, n_channels, n_timepoints)
+            The training data.
+        y : 1D np.ndarray of shape (n_instances)
+            The class labels for fitting, indices correspond to instance indices in X
 
         Returns
         -------
-        self : RandomShapeletTransformer
-            This estimator.
+        self :
+            Reference to self.
         """
-        X, y = self._validate_data(X=X, y=y, ensure_min_samples=2)
+        X, y = self._validate_data(
+            X=X, y=y, ensure_min_samples=2, ensure_min_series_length=3
+        )
         X = self._convert_X(X)
 
-        self.n_instances_, self.n_dims_, self.series_length_ = X.shape
-        self.classes_, self._class_counts = np.unique(y, return_counts=True)
+        self.n_instances_, self.n_channels_, self.n_timepoints_ = X.shape
+        self.classes_ = np.unique(y)
         self.n_classes_ = self.classes_.shape[0]
         self.class_dictionary_ = {}
         for index, class_val in enumerate(self.classes_):
             self.class_dictionary_[class_val] = index
 
         self._n_jobs = check_n_jobs(self.n_jobs)
 
-        le = preprocessing.LabelEncoder()
-        y = le.fit_transform(y)
+        self._estimator = _clone_estimator(
+            ExtraTreesClassifier(n_estimators=200, criterion="entropy")
+            if self.estimator is None
+            else self.estimator,
+            self.random_state,
+        )
 
-        self._max_shapelets = self.max_shapelets
-        if self.max_shapelets is None:
-            self._max_shapelets = min(10 * self.n_instances_, 1000)
-        if self._max_shapelets < self.n_classes_:
-            self._max_shapelets = self.n_classes_
-
-        self._max_shapelet_length = self.max_shapelet_length
-        if self.max_shapelet_length is None:
-            self._max_shapelet_length = self.series_length_
-
-        time_limit = self.time_limit_in_minutes * 60
-        start_time = time.time()
-        fit_time = 0
-
-        max_shapelets_per_class = int(self._max_shapelets / self.n_classes_)
-        if max_shapelets_per_class < 1:
-            max_shapelets_per_class = 1
+        m = getattr(self._estimator, "n_jobs", None)
+        if m is not None:
+            self._estimator.n_jobs = self._n_jobs
 
-        shapelets = List(
-            [List([(-1.0, -1, -1, -1, -1, -1)]) for _ in range(self.n_classes_)]
+        X_t, self._series_transformers, self._transformers = _fit_transforms(
+            X,
+            y,
+            self.series_transformers,
+            self.n_intervals,
+            self.n_shapelets,
+            self.use_pyfftw,
+            self.use_pycatch22,
+            self.random_state,
+            self._n_jobs,
         )
-        n_shapelets_extracted = 0
+        self._estimator.fit(X_t, y)
 
-        if time_limit > 0:
-            while (
-                fit_time < time_limit
-                and n_shapelets_extracted < self.contract_max_n_shapelet_samples
-            ):
-                candidate_shapelets = Parallel(
-                    n_jobs=self._n_jobs, backend=self.parallel_backend, prefer="threads"
-                )(
-                    delayed(self._extract_random_shapelet)(
-                        X,
-                        y,
-                        n_shapelets_extracted + i,
-                        shapelets,
-                        max_shapelets_per_class,
-                    )
-                    for i in range(self.batch_size)
-                )
-
-                for i, heap in enumerate(shapelets):
-                    self._merge_shapelets(
-                        heap,
-                        List(candidate_shapelets),
-                        max_shapelets_per_class,
-                        i,
-                    )
-
-                if self.remove_self_similar:
-                    for i, heap in enumerate(shapelets):
-                        to_keep = self._remove_self_similar_shapelets(heap)
-                        shapelets[i] = List([n for (n, b) in zip(heap, to_keep) if b])
+        return self
 
-                n_shapelets_extracted += self.batch_size
-                fit_time = time.time() - start_time
-        else:
-            while n_shapelets_extracted < self.n_shapelet_samples:
-                n_shapelets_to_extract = (
-                    self.batch_size
-                    if n_shapelets_extracted + self.batch_size
-                    <= self.n_shapelet_samples
-                    else self.n_shapelet_samples - n_shapelets_extracted
-                )
-
-                candidate_shapelets = Parallel(
-                    n_jobs=self._n_jobs, backend=self.parallel_backend, prefer="threads"
-                )(
-                    delayed(self._extract_random_shapelet)(
-                        X,
-                        y,
-                        n_shapelets_extracted + i,
-                        shapelets,
-                        max_shapelets_per_class,
-                    )
-                    for i in range(n_shapelets_to_extract)
-                )
-
-                for i, heap in enumerate(shapelets):
-                    self._merge_shapelets(
-                        heap,
-                        List(candidate_shapelets),
-                        max_shapelets_per_class,
-                        i,
-                    )
-
-                if self.remove_self_similar:
-                    for i, heap in enumerate(shapelets):
-                        to_keep = self._remove_self_similar_shapelets(heap)
-                        shapelets[i] = List([n for (n, b) in zip(heap, to_keep) if b])
-
-                n_shapelets_extracted += n_shapelets_to_extract
-
-        self.shapelets_ = [
-            (
-                s[0],
-                s[1],
-                s[2],
-                s[3],
-                s[4],
-                self.classes_[s[5]],
-                z_normalise_series(X[s[4], s[3], s[2] : s[2] + s[1]]),
-            )
-            for class_shapelets in shapelets
-            for s in class_shapelets
-            if s[0] > 0
-        ]
-        self.shapelets_.sort(reverse=True, key=lambda s: (s[0], s[1], s[2], s[3], s[4]))
+    def predict(self, X: Union[np.ndarray, List[np.ndarray]]) -> np.ndarray:
+        """Predicts labels for sequences in X.
 
-        to_keep = self._remove_identical_shapelets(List(self.shapelets_))
-        self.shapelets_ = [n for (n, b) in zip(self.shapelets_, to_keep) if b]
+        Parameters
+        ----------
+        X : 3D np.ndarray of shape (n_instances, n_channels, n_timepoints)
+            The testing data.
 
-        self._sorted_indicies = []
-        for s in self.shapelets_:
-            sabs = np.abs(s[6])
-            self._sorted_indicies.append(
-                np.array(
-                    sorted(range(s[1]), reverse=True, key=lambda j, sabs=sabs: sabs[j])
-                )
-            )
+        Returns
+        -------
+        y : array-like of shape (n_instances)
+            Predicted class labels.
+        """
+        check_is_fitted(self)
 
-        return self
+        X = self._validate_data(X=X, reset=False, ensure_min_series_length=3)
+        X = self._convert_X(X)
+
+        return self._estimator.predict(
+            _transform_data(X, self._series_transformers, self._transformers)
+        )
 
-    def transform(self, X, y=None):
-        """Transform X according to the extracted shapelets.
+    def predict_proba(self, X: Union[np.ndarray, List[np.ndarray]]) -> np.ndarray:
+        """Predicts labels probabilities for sequences in X.
 
         Parameters
         ----------
-        X : pandas DataFrame or np.ndarray
-            The input data to transform.
+        X : 3D np.array of shape (n_instances, n_channels, n_timepoints)
+            The testing data.
 
         Returns
         -------
-        output : pandas DataFrame
-            The transformed dataframe in tabular format.
+        y : array-like of shape (n_instances, n_classes_)
+            Predicted probabilities using the ordering in classes_.
         """
         check_is_fitted(self)
 
-        X = self._validate_data(X=X, reset=True)
+        X = self._validate_data(X=X, reset=False, ensure_min_series_length=3)
         X = self._convert_X(X)
 
-        output = np.zeros((len(X), len(self.shapelets_)))
-
-        for i, series in enumerate(X):
-            dists = Parallel(
-                n_jobs=self._n_jobs, backend=self.parallel_backend, prefer="threads"
-            )(
-                delayed(_online_shapelet_distance)(
-                    series[shapelet[3]],
-                    shapelet[6],
-                    self._sorted_indicies[n],
-                    shapelet[2],
-                    shapelet[1],
-                )
-                for n, shapelet in enumerate(self.shapelets_)
+        m = getattr(self._estimator, "predict_proba", None)
+        if callable(m):
+            return self._estimator.predict_proba(
+                _transform_data(X, self._series_transformers, self._transformers)
             )
+        else:
+            dists = np.zeros((X.shape[0], self.n_classes_))
+            preds = self._estimator.predict(
+                _transform_data(X, self._series_transformers, self._transformers)
+            )
+            for i in range(0, X.shape[0]):
+                dists[i, self.class_dictionary_[preds[i]]] = 1
+            return dists
+
+    def _more_tags(self) -> dict:
+        return {
+            "optional_dependency": self.use_pycatch22 or self.use_pyfftw,
+            "non_deterministic": True,
+        }
 
-            output[i] = dists
-
-        return output
+    @classmethod
+    def get_test_params(
+        cls, parameter_set: Union[str, None] = None
+    ) -> Union[dict, List[dict]]:
+        """Return unit test parameter settings for the estimator.
 
-    def _extract_random_shapelet(self, X, y, i, shapelets, max_shapelets_per_class):
-        rs = 255 if self.random_state == 0 else self.random_state
-        rs = (
-            None
-            if self.random_state is None
-            else (rs * 37 * (i + 1)) % np.iinfo(np.int32).max
-        )
-        rng = check_random_state(rs)
+        Parameters
+        ----------
+        parameter_set : None or str, default=None
+            Name of the set of test parameters to return, for use in tests. If no
+            special parameters are defined for a value, will return `"default"` set.
 
-        inst_idx = i % self.n_instances_
-        cls_idx = int(y[inst_idx])
-        worst_quality = (
-            shapelets[cls_idx][0][0]
-            if len(shapelets[cls_idx]) == max_shapelets_per_class
-            else -1
-        )
+        Returns
+        -------
+        params : dict or list of dict
+            Parameters to create testing instances of the class.
+        """
+        return {
+            "series_transformers": [
+                None,
+                FunctionTransformer(func=first_order_differences_3d, validate=False),
+            ],
+            "n_intervals": 1,
+            "n_shapelets": 2,
+            "estimator": ExtraTreesClassifier(n_estimators=2, criterion="entropy"),
+        }
+
+
+class RISTRegressor(RegressorMixin, BaseTimeSeriesEstimator):
+    """Randomised Interval-Shapelet Transformation (RIST) pipeline regressor.
+
+    This regressor is a hybrid pipeline using the RandomIntervalTransformer using
+    Catch22 features and summary stats, and the RandomDilatedShapeletTransformer.
+    Both transforms extract features from different series transformations (1st Order
+    Differences, PeriodogramTransformer, and ARCoefficientTransformer).
+    An ExtraTreesRegressor with 200 trees is used as the estimator for the
+    concatenated feature vector output.
 
-        length = (
-            rng.randint(0, self._max_shapelet_length - self.min_shapelet_length)
-            + self.min_shapelet_length
-        )
-        position = rng.randint(0, self.series_length_ - length)
-        dim = rng.randint(0, self.n_dims_)
+    Parameters
+    ----------
+    n_intervals : int, callable or None, default=None,
+        The number of intervals of random length, position and dimension to be
+        extracted for the interval portion of the pipeline. Input should be an int or
+        a function that takes a 3D np.ndarray input and returns an int. Functions may
+        extract a different number of intervals per `series_transformer` output.
+        If None, extracts `int(np.sqrt(X.shape[2]) * np.sqrt(X.shape[1]) * 15 + 5)`
+        intervals where `Xt` is the series representation data.
+    n_shapelets : int, callable or None, default=None,
+        The number of shapelets of random dilation and position to be extracted for the
+        shapelet portion of the pipeline. Input should be an int or
+        a function that takes a 3D np.ndarray input and returns an int. Functions may
+        extract a different number of shapelets per `series_transformer` output.
+        If None, extracts `int(np.sqrt(Xt.shape[2]) * 200 + 5)` shapelets where `Xt` is
+        the series representation data.
+    series_transformers : TransformerMixin, list, tuple, or None, default=None
+        The transformers to apply to the series before extracting intervals and
+        shapelets. If None, use the series as is. If "default", use [None, 1st Order
+        Differences, PeriodogramTransformer, and ARCoefficientTransformer].
+
+        A list or tuple of transformers will extract intervals from
+        all transformations concatenate the output. Including None in the list or tuple
+        will use the series as is for interval extraction.
+    use_pycatch22 : bool, optional, default=True
+        Wraps the C based pycatch22 implementation for aeon.
+        (https://github.com/DynamicsAndNeuralSystems/pycatch22). This requires the
+        ``pycatch22`` package to be installed if True.
+    use_pyfftw : bool, default=True
+        Whether to use the pyfftw library for FFT calculations. Requires the pyfftw
+        package to be installed.
+    estimator : sklearn classifier, default=None
+        An sklearn estimator to be built using the transformed data. Defaults to an
+        ExtraTreesRegressor with 200 trees.
+    random_state : int, RandomState instance or None, default=None
+        If `int`, random_state is the seed used by the random number generator;
+        If `RandomState` instance, random_state is the random number generator;
+        If `None`, the random number generator is the `RandomState` instance used
+        by `np.random`.
+    n_jobs : int, default=1
+        The number of jobs to run in parallel for both `fit` and `predict`.
+        ``-1`` means using all processors.
 
-        shapelet = z_normalise_series(X[inst_idx, dim, position : position + length])
-        sabs = np.abs(shapelet)
-        sorted_indicies = np.array(
-            sorted(range(length), reverse=True, key=lambda j: sabs[j])
-        )
+    Attributes
+    ----------
+    n_instances_ : int
+        The number of train cases in the training set.
+    n_channels_ : int
+        The number of dimensions per case in the training set.
+    n_timepoints_ : int
+        The length of each series in the training set.
 
-        quality = self._find_shapelet_quality(
-            X,
-            y,
-            shapelet,
-            sorted_indicies,
-            position,
-            length,
-            dim,
-            inst_idx,
-            self._class_counts[cls_idx],
-            self.n_instances_ - self._class_counts[cls_idx],
-            worst_quality,
-        )
+    See Also
+    --------
+    RandomIntervalTransformer
+    RandomDilatedShapeletTransformer
+    RISTClassifier
 
-        return quality, length, position, dim, inst_idx, cls_idx
+    Examples
+    --------
+    >>> from tsml.hybrid import RISTRegressor
+    >>> from tsml.utils.testing import generate_3d_test_data
+    >>> X, y = generate_3d_test_data(n_samples=8, series_length=10,
+    ...                              regression_target=True, random_state=0)
+    >>> reg = RISTRegressor(random_state=0)
+    >>> reg.fit(X, y)
+    RISTRegressor(...)
+    >>> reg.predict(X)
+    array([0.31798318, 1.41426301, 1.06414747, 0.6924721 , 0.56660146,
+           1.26538944, 0.52324808, 1.0939405 ])
+    """
 
-    @staticmethod
-    @njit(fastmath=True, cache=True)
-    def _find_shapelet_quality(
-        X,
-        y,
-        shapelet,
-        sorted_indicies,
-        position,
-        length,
-        dim,
-        inst_idx,
-        this_cls_count,
-        other_cls_count,
-        worst_quality,
-    ):
-        # todo optimise this more, we spend 99% of time here
-        orderline = []
-        this_cls_traversed = 0
-        other_cls_traversed = 0
-
-        for i, series in enumerate(X):
-            if i != inst_idx:
-                distance = _online_shapelet_distance(
-                    series[dim], shapelet, sorted_indicies, position, length
-                )
-            else:
-                distance = 0
-
-            if y[i] == y[inst_idx]:
-                cls = 1
-                this_cls_traversed += 1
-            else:
-                cls = -1
-                other_cls_traversed += 1
-
-            orderline.append((distance, cls))
-            orderline.sort()
-
-            if worst_quality > 0:
-                quality = _calc_early_binary_ig(
-                    orderline,
-                    this_cls_traversed,
-                    other_cls_traversed,
-                    this_cls_count - this_cls_traversed,
-                    other_cls_count - other_cls_traversed,
-                    worst_quality,
-                )
-
-                if quality <= worst_quality:
-                    return -1
-
-        quality = _calc_binary_ig(orderline, this_cls_count, other_cls_count)
-
-        return round(quality, 12)
-
-    @staticmethod
-    @njit(fastmath=True, cache=True)
-    def _merge_shapelets(
-        shapelet_heap, candidate_shapelets, max_shapelets_per_class, cls_idx
+    def __init__(
+        self,
+        n_intervals=None,
+        n_shapelets=None,
+        series_transformers="default",
+        use_pycatch22=True,
+        use_pyfftw=True,
+        estimator=None,
+        n_jobs=1,
+        random_state=None,
     ):
-        for shapelet in candidate_shapelets:
-            if shapelet[5] == cls_idx and shapelet[0] > 0:
-                if (
-                    len(shapelet_heap) == max_shapelets_per_class
-                    and shapelet[0] < shapelet_heap[0][0]
-                ):
-                    continue
-
-                heapq.heappush(shapelet_heap, shapelet)
-
-                if len(shapelet_heap) > max_shapelets_per_class:
-                    heapq.heappop(shapelet_heap)
-
-    @staticmethod
-    @njit(fastmath=True, cache=True)
-    def _remove_self_similar_shapelets(shapelet_heap):
-        to_keep = [True] * len(shapelet_heap)
-
-        for i in range(len(shapelet_heap)):
-            if to_keep[i] is False:
-                continue
-
-            for n in range(i + 1, len(shapelet_heap)):
-                if to_keep[n] and _is_self_similar(shapelet_heap[i], shapelet_heap[n]):
-                    if (shapelet_heap[i][0], shapelet_heap[i][1]) >= (
-                        shapelet_heap[n][0],
-                        shapelet_heap[n][1],
-                    ):
-                        to_keep[n] = False
-                    else:
-                        to_keep[i] = False
-                        break
-
-        return to_keep
-
-    @staticmethod
-    @njit(fastmath=True, cache=True)
-    def _remove_identical_shapelets(shapelets):
-        to_keep = [True] * len(shapelets)
-
-        for i in range(len(shapelets)):
-            for n in range(i + 1, len(shapelets)):
-                if (
-                    to_keep[n]
-                    and shapelets[i][1] == shapelets[n][1]
-                    and np.array_equal(shapelets[i][6], shapelets[n][6])
-                ):
-                    to_keep[n] = False
+        self.n_intervals = n_intervals
+        self.n_shapelets = n_shapelets
+        self.series_transformers = series_transformers
+        self.use_pycatch22 = use_pycatch22
+        self.use_pyfftw = use_pyfftw
+        self.estimator = estimator
+        self.random_state = random_state
+        self.n_jobs = n_jobs
 
-        return to_keep
+        if use_pycatch22:
+            _check_optional_dependency("pycatch22", "pycatch22", self)
+        if use_pyfftw:
+            _check_optional_dependency("pyfftw", "pyfftw", self)
 
-    @classmethod
-    def get_test_params(cls, parameter_set="default"):
-        """Return testing parameter settings for the estimator.
+        super(RISTRegressor, self).__init__()
+
+    def fit(self, X: Union[np.ndarray, List[np.ndarray]], y: np.ndarray) -> object:
+        """Fit the estimator to training data.
 
         Parameters
         ----------
-        parameter_set : str, default="default"
-            Name of the set of test parameters to return, for use in tests. If no
-            special parameters are defined for a value, will return `"default"` set.
+        X : 3D np.ndarray of shape (n_instances, n_channels, n_timepoints)
+            The training data.
+        y : 1D np.ndarray of shape (n_instances)
+            The target labels for fitting, indices correspond to instance indices in X
 
         Returns
         -------
-        params : dict or list of dict, default = {}
-            Parameters to create testing instances of the class
-            Each dict are parameters to construct an "interesting" test instance, i.e.,
-            `MyClass(**params)` or `MyClass(**params[i])` creates a valid test instance.
-            `create_test_instance` uses the first (or only) dictionary in `params`
+        self :
+            Reference to self.
         """
-        return {"max_shapelets": 5, "n_shapelet_samples": 50, "batch_size": 20}
-
+        X, y = self._validate_data(
+            X=X, y=y, ensure_min_samples=2, ensure_min_series_length=3
+        )
+        X = self._convert_X(X)
 
-@njit(fastmath=True, cache=True)
-def _online_shapelet_distance(series, shapelet, sorted_indicies, position, length):
-    subseq = series[position : position + length]
-
-    sum = 0.0
-    sum2 = 0.0
-    for i in subseq:
-        sum += i
-        sum2 += i * i
-
-    mean = sum / length
-    std = (sum2 - mean * mean * length) / length
-    if std > 0:
-        subseq = (subseq - mean) / std
-    else:
-        subseq = np.zeros(length)
+        self.n_instances_, self.n_channels_, self.n_timepoints_ = X.shape
 
-    best_dist = 0
-    for i, n in zip(shapelet, subseq):
-        temp = i - n
-        best_dist += temp * temp
-
-    i = 1
-    traverse = [True, True]
-    sums = [sum, sum]
-    sums2 = [sum2, sum2]
-
-    while traverse[0] or traverse[1]:
-        for n in range(2):
-            mod = -1 if n == 0 else 1
-            pos = position + mod * i
-            traverse[n] = pos >= 0 if n == 0 else pos <= len(series) - length
-
-            if not traverse[n]:
-                continue
-
-            start = series[pos - n]
-            end = series[pos - n + length]
-
-            sums[n] += mod * end - mod * start
-            sums2[n] += mod * end * end - mod * start * start
-
-            mean = sums[n] / length
-            std = math.sqrt((sums2[n] - mean * mean * length) / length)
-
-            dist = 0
-            use_std = std != 0
-            for j in range(length):
-                val = (series[pos + sorted_indicies[j]] - mean) / std if use_std else 0
-                temp = shapelet[sorted_indicies[j]] - val
-                dist += temp * temp
-
-                if dist > best_dist:
-                    break
-
-            if dist < best_dist:
-                best_dist = dist
-
-        i += 1
-
-    return best_dist if best_dist == 0 else 1 / length * best_dist
-
-
-@njit(fastmath=True, cache=True)
-def _calc_early_binary_ig(
-    orderline,
-    c1_traversed,
-    c2_traversed,
-    c1_to_add,
-    c2_to_add,
-    worst_quality,
-):
-    initial_ent = _binary_entropy(
-        c1_traversed + c1_to_add,
-        c2_traversed + c2_to_add,
-    )
-
-    total_all = c1_traversed + c2_traversed + c1_to_add + c2_to_add
-
-    bsf_ig = 0
-    # actual observations in orderline
-    c1_count = 0
-    c2_count = 0
-
-    # evaluate each split point
-    for split in range(len(orderline)):
-        next_class = orderline[split][1]  # +1 if this class, -1 if other
-        if next_class > 0:
-            c1_count += 1
-        else:
-            c2_count += 1
+        self._n_jobs = check_n_jobs(self.n_jobs)
 
-        # optimistically add this class to left side first and other to right
-        left_prop = (split + 1 + c1_to_add) / total_all
-        ent_left = _binary_entropy(c1_count + c1_to_add, c2_count)
-
-        # because right side must optimistically contain everything else
-        right_prop = 1 - left_prop
-
-        ent_right = _binary_entropy(
-            c1_traversed - c1_count,
-            c2_traversed - c2_count + c2_to_add,
+        self._estimator = _clone_estimator(
+            ExtraTreesRegressor(n_estimators=200)
+            if self.estimator is None
+            else self.estimator,
+            self.random_state,
         )
 
-        ig = initial_ent - left_prop * ent_left - right_prop * ent_right
-        bsf_ig = max(ig, bsf_ig)
+        m = getattr(self._estimator, "n_jobs", None)
+        if m is not None:
+            self._estimator.n_jobs = self._n_jobs
 
-        # now optimistically add this class to right, other to left
-        left_prop = (split + 1 + c2_to_add) / total_all
-        ent_left = _binary_entropy(c1_count, c2_count + c2_to_add)
-
-        # because right side must optimistically contain everything else
-        right_prop = 1 - left_prop
-
-        ent_right = _binary_entropy(
-            c1_traversed - c1_count + c1_to_add,
-            c2_traversed - c2_count,
+        X_t, self._series_transformers, self._transformers = _fit_transforms(
+            X,
+            y,
+            self.series_transformers,
+            self.n_intervals,
+            self.n_shapelets,
+            self.use_pyfftw,
+            self.use_pycatch22,
+            self.random_state,
+            self._n_jobs,
         )
+        self._estimator.fit(X_t, y)
 
-        ig = initial_ent - left_prop * ent_left - right_prop * ent_right
-        bsf_ig = max(ig, bsf_ig)
+        return self
 
-        if bsf_ig > worst_quality:
-            return bsf_ig
+    def predict(self, X: Union[np.ndarray, List[np.ndarray]]) -> np.ndarray:
+        """Predicts labels for sequences in X.
 
-    return bsf_ig
+        Parameters
+        ----------
+        X : 3D np.ndarray of shape (n_instances, n_channels, n_timepoints)
+            The testing data.
 
+        Returns
+        -------
+        y : array-like of shape (n_instances)
+            Predicted target labels.
+        """
+        check_is_fitted(self)
+
+        X = self._validate_data(X=X, reset=False, ensure_min_series_length=3)
+        X = self._convert_X(X)
+
+        return self._estimator.predict(
+            _transform_data(X, self._series_transformers, self._transformers)
+        )
+
+    def _more_tags(self) -> dict:
+        return {
+            "optional_dependency": self.use_pycatch22 or self.use_pyfftw,
+            "non_deterministic": True,
+        }
 
-@njit(fastmath=True, cache=True)
-def _calc_binary_ig(orderline, c1, c2):
-    initial_ent = _binary_entropy(c1, c2)
+    @classmethod
+    def get_test_params(
+        cls, parameter_set: Union[str, None] = None
+    ) -> Union[dict, List[dict]]:
+        """Return unit test parameter settings for the estimator.
 
-    total_all = c1 + c2
+        Parameters
+        ----------
+        parameter_set : None or str, default=None
+            Name of the set of test parameters to return, for use in tests. If no
+            special parameters are defined for a value, will return `"default"` set.
+
+        Returns
+        -------
+        params : dict or list of dict
+            Parameters to create testing instances of the class.
+        """
+        return {
+            "series_transformers": [
+                None,
+                FunctionTransformer(func=first_order_differences_3d, validate=False),
+            ],
+            "n_intervals": 1,
+            "n_shapelets": 2,
+            "estimator": ExtraTreesRegressor(n_estimators=2),
+        }
+
+
+def _fit_transforms(
+    X,
+    y,
+    series_transformers,
+    n_intervals,
+    n_shapelets,
+    use_pyfftw,
+    use_pycatch22,
+    random_state,
+    n_jobs,
+):
+    rng = check_random_state(random_state)
 
-    bsf_ig = 0
-    c1_count = 0
-    c2_count = 0
+    if series_transformers == "default":
+        series_transformers = [
+            None,
+            FunctionTransformer(func=first_order_differences_3d, validate=False),
+            PeriodogramTransformer(use_pyfftw=use_pyfftw),
+            ARCoefficientTransformer(
+                replace_nan=True, order=int(12 * (X.shape[2] / 100.0) ** 0.25)
+            ),
+        ]
+    elif isinstance(series_transformers, (list, tuple)):
+        series_transformers = [
+            None if st is None else _clone_estimator(st, random_state=rng)
+            for st in series_transformers
+        ]
+    else:
+        series_transformers = [
+            None
+            if series_transformers is None
+            else _clone_estimator(series_transformers, random_state=rng)
+        ]
 
-    # evaluate each split point
-    for split in range(len(orderline)):
-        next_class = orderline[split][1]  # +1 if this class, -1 if other
-        if next_class > 0:
-            c1_count += 1
+    X_t = np.empty((X.shape[0], 0))
+    transformers = []
+    for st in series_transformers:
+        if st is not None:
+            s = st.fit_transform(X, y)
         else:
-            c2_count += 1
+            s = X
 
-        left_prop = (split + 1) / total_all
-        ent_left = _binary_entropy(c1_count, c2_count)
+        if n_intervals is None:
+            n_intervals = int(np.sqrt(X.shape[2]) * np.sqrt(X.shape[1]) * 15 + 5)
+        elif callable(n_intervals):
+            n_intervals = n_intervals(s)
+        else:
+            n_intervals = n_intervals
 
-        right_prop = 1 - left_prop
-        ent_right = _binary_entropy(
-            c1 - c1_count,
-            c2 - c2_count,
+        ct = RandomIntervalTransformer(
+            n_intervals=n_intervals,
+            features=[
+                Catch22Transformer(
+                    outlier_norm=True, replace_nans=True, use_pycatch22=use_pycatch22
+                ),
+                row_mean,
+                row_std,
+                row_slope,
+                row_median,
+                row_iqr,
+                row_numba_min,
+                row_numba_max,
+                row_ppv,
+            ],
+            n_jobs=n_jobs,
         )
+        _set_random_states(ct, rng)
+        transformers.append(ct)
+        t = ct.fit_transform(s, y)
+
+        X_t = np.hstack((X_t, t))
+
+        if n_shapelets is None:
+            n_shapelets = int(np.sqrt(X.shape[2]) * 200 + 5)
+        elif callable(n_shapelets):
+            n_shapelets = n_shapelets(s)
+        else:
+            n_shapelets = n_shapelets
+
+        st = RandomDilatedShapeletTransformer(max_shapelets=n_shapelets, n_jobs=n_jobs)
+        _set_random_states(st, rng)
+        transformers.append(st)
+        t = st.fit_transform(s, y)
 
-        ig = initial_ent - left_prop * ent_left - right_prop * ent_right
-        bsf_ig = max(ig, bsf_ig)
+        X_t = np.hstack((X_t, t))
 
-    return bsf_ig
+    X_t = np.nan_to_num(X_t, nan=0.0, posinf=0.0, neginf=0.0)
+    return X_t, series_transformers, transformers
+
+
+def _transform_data(X, series_transformers, transformers):
+    X_t = np.empty((X.shape[0], 0))
+    for i, st in enumerate(series_transformers):
+        if st is not None:
+            s = st.transform(X)
+        else:
+            s = X
 
+        t = transformers[i * 2].transform(s)
+        X_t = np.hstack((X_t, t))
 
-@njit(fastmath=True, cache=True)
-def _binary_entropy(c1, c2):
-    ent = 0
-    if c1 != 0:
-        ent -= c1 / (c1 + c2) * np.log2(c1 / (c1 + c2))
-    if c2 != 0:
-        ent -= c2 / (c1 + c2) * np.log2(c2 / (c1 + c2))
-    return ent
-
-
-@njit(fastmath=True, cache=True)
-def _is_self_similar(s1, s2):
-    # not self similar if from different series or dimension
-    if s1[4] == s2[4] and s1[3] == s2[3]:
-        if s2[2] <= s1[2] <= s2[2] + s2[1]:
-            return True
-        if s1[2] <= s2[2] <= s1[2] + s1[1]:
-            return True
+        t = transformers[i * 2 + 1].transform(s)
+        X_t = np.hstack((X_t, t))
 
-    return False
+    X_t = np.nan_to_num(X_t, nan=0.0, posinf=0.0, neginf=0.0)
+    return X_t
```

### Comparing `tsml-0.1.1/tsml/utils/_tags.py` & `tsml-0.2.0/tsml/utils/_tags.py`

 * *Files identical despite different names*

### Comparing `tsml-0.1.1/tsml/utils/discovery.py` & `tsml-0.2.0/tsml/utils/discovery.py`

 * *Files identical despite different names*

### Comparing `tsml-0.1.1/tsml/utils/numba_functions/stats.py` & `tsml-0.2.0/tsml/utils/numba_functions/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     "slope",
     "row_slope",
     "iqr",
     "row_iqr",
     "ppv",
     "row_ppv",
     "fisher_score",
+    "prime_up_to",
+    "is_prime",
 ]
 
 import numpy as np
 from numba import njit
 
 import tsml.utils.numba_functions.general as general_numba
 
@@ -817,7 +819,59 @@
         accum_numerator += idx_label.shape[0] * (mu_feat_label - mu_feat) ** 2
         accum_denominator += idx_label.shape[0] * sigma_feat_label**2
 
     if accum_denominator == 0:
         return 0
     else:
         return accum_numerator / accum_denominator
+
+
+@njit(fastmath=True, cache=True)
+def prime_up_to(n: int) -> np.ndarray:
+    """Check if any number from 1 to n is a prime number and return the ones which are.
+
+    Parameters
+    ----------
+    n : int
+        Number up to which the search for prime number will go
+
+    Returns
+    -------
+    array
+        Prime numbers up to n
+
+    Examples
+    --------
+    >>> from tsml.utils.numba_functions.stats import prime_up_to
+    >>> p = prime_up_to(50)
+    """
+    is_p = np.zeros(n + 1, dtype=np.bool_)
+    for i in range(n + 1):
+        is_p[i] = is_prime(i)
+    return np.where(is_p)[0]
+
+
+@njit(fastmath=True, cache=True)
+def is_prime(n: int) -> bool:
+    """Check if the input number is a prime number.
+
+    Parameters
+    ----------
+    n : int
+        The number to test
+
+    Returns
+    -------
+    bool
+        Wheter n is a prime number
+
+    Examples
+    --------
+    >>> from tsml.utils.numba_functions.stats import is_prime
+    >>> p = is_prime(7)
+    """
+    if (n % 2 == 0 and n > 2) or n == 0 or n == 1:
+        return False
+    for i in range(3, int(n**0.5) + 1, 2):
+        if not n % i:
+            return False
+    return True
```

### Comparing `tsml-0.1.1/tsml/utils/testing.py` & `tsml-0.2.0/tsml/utils/testing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-# -*- coding: utf-8 -*-
 """Utilities for testing estimators."""
 
 __author__ = ["MatthewMiddlehurst"]
 __all__ = [
     "generate_test_estimators",
     "parametrize_with_checks",
     "generate_3d_test_data",
+    "generate_2d_test_data",
+    "generate_unequal_test_data",
 ]
 
+import re
 import warnings
 from functools import partial
 from typing import Callable, List, Tuple, Union
 
 import numpy as np
+from sklearn import config_context
 from sklearn.base import BaseEstimator
-from sklearn.utils.estimator_checks import (
-    _get_check_estimator_ids,
-    _maybe_mark_xfail,
-    _yield_all_checks,
-)
+from sklearn.utils.estimator_checks import _maybe_mark_xfail, _yield_all_checks
 
-import tsml.tests.estimator_checks as ts_checks
+import tsml.tests.test_estimator_checks as ts_checks
 from tsml.base import BaseTimeSeriesEstimator
 from tsml.utils.discovery import all_estimators
 
 
 def generate_test_estimators() -> List[BaseEstimator]:
     """Generate a list of all estimators in tsml with test parameters.
 
@@ -52,23 +51,25 @@
                 try:
                     estimators.append(c[1](**p))
                 except ModuleNotFoundError:
                     warnings.warn(
                         f"Unable to create estimator {c[0]} with parameters {p}. "
                         f"Most likely an optional dependency is not present.",
                         ImportWarning,
+                        stacklevel=2,
                     )
         else:
             try:
                 estimators.append(c[1](**params))
             except ModuleNotFoundError:
                 warnings.warn(
                     f"Unable to create estimator {c[0]} with parameters {params}. "
                     f"Most likely an optional dependency is not present.",
                     ImportWarning,
+                    stacklevel=2,
                 )
     return estimators
 
 
 def parametrize_with_checks(estimators: List[BaseEstimator]) -> Callable:
     """Pytest specific decorator for parametrizing estimator checks.
 
@@ -118,18 +119,58 @@
             )
             name = type(estimator).__name__
             for check in checks(estimator):
                 check = partial(check, name)
                 yield _maybe_mark_xfail(estimator, check, pytest)
 
     return pytest.mark.parametrize(
-        "estimator, check", checks_generator(), ids=_get_check_estimator_ids
+        "estimator, check",
+        checks_generator(),
+        ids=_get_check_estimator_ids,
     )
 
 
+def _get_check_estimator_ids(obj):
+    """Create pytest ids for checks.
+
+    When `obj` is an estimator, this returns the sklearn pprint version of the
+    estimator (with `print_changed_only=True`). When `obj` is a function, the
+    name of the function is returned with its keyword arguments.
+
+    `_get_check_estimator_ids` is designed to be used as the `id` in
+    `pytest.mark.parametrize` where `checks_generator` is yielding estimators and
+    checks.
+
+    Uses the `scikit-learn` 1.2.1 `_get_check_estimator_ids` function as a base.
+
+    Parameters
+    ----------
+    obj : estimator or function
+        Items generated by `checks_generator`.
+
+    Returns
+    -------
+    id : str or None
+        The id of the check.
+    """
+    if callable(obj):
+        if not isinstance(obj, partial):
+            return obj.__name__
+
+        if not obj.keywords:
+            return obj.func.__name__
+
+        kwstring = ",".join(["{}={}".format(k, v) for k, v in obj.keywords.items()])
+        return "{}({})".format(obj.func.__name__, kwstring)
+    if hasattr(obj, "get_params"):
+        with config_context(print_changed_only=True):
+            s = re.sub(r"\s", "", str(obj))
+            return re.sub(r"<function[^)]*>", "func", s)
+
+
 def generate_3d_test_data(
     n_samples: int = 10,
     n_channels: int = 1,
     series_length: int = 12,
     n_labels: int = 2,
     regression_target: bool = False,
     random_state: Union[int, None] = None,
```

### Comparing `tsml-0.1.1/tsml/utils/validation.py` & `tsml-0.2.0/tsml/utils/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,15 @@
     dtype: Union[str, type, None] = "numeric",
     copy: bool = False,
     force_all_finite: bool = True,
     convert_2d: bool = True,
     ensure_min_samples: int = 1,
     ensure_min_channels: int = 1,
     ensure_min_series_length: int = 2,
+    ensure_equal_length: bool = False,
     estimator: Union[str, BaseEstimator, None] = None,
     y_numeric: bool = False,
 ) -> Union[Tuple[np.ndarray, np.ndarray], Tuple[List[np.ndarray], np.ndarray]]:
     """Input validation for standard estimators.
 
     Checks X and y for consistent length, enforces X to be 3D and y 1D. By default,
     the input is checked to be a non-empty 2D numpy array, 3D numpy array or list of
@@ -185,14 +186,16 @@
         axis (first axis of all items for list of 2D numpy array). Setting to 0 disables
         this check.
     ensure_min_series_length : int, default=1
         Make sure that the array has some minimum number of features/series length in
         its third axis (second axis of all items for list of 2D numpy array). Setting
         to 0 disables this check.
         The default value of 2 rejects empty datasets and non-series.
+    ensure_equal_length:  bool, default=False
+        Make sure that all series have the same length. Setting to False disables this.
     y_numeric : bool, default=False
         Whether to ensure that y has a numeric type. If dtype of y is object,
         it is converted to float64. Should only be used for regression
         algorithms.
     estimator : str, estimator instance or None, default=None
         If passed, include the name of the estimator in warning messages.
 
@@ -234,24 +237,24 @@
     y = _check_y(y, multi_output=False, y_numeric=y_numeric)
 
     check_consistent_length(X, y)
 
     return X, y
 
 
-
 def check_X(
     X: object,
     dtype: Union[str, type, None] = "numeric",
     copy: bool = False,
     force_all_finite: bool = True,
     convert_2d: bool = False,
     ensure_min_samples: int = 1,
     ensure_min_channels: int = 1,
     ensure_min_series_length: int = 2,
+    ensure_equal_length: bool = False,
     estimator: Union[str, BaseEstimator, None] = None,
 ) -> Union[np.ndarray, list]:
     """Input validation on a numpy array or list dataset.
 
     By default, the input is checked to be a non-empty 2D numpy array, 3D numpy array or
     list of 2D numpy arrays containing only finite values. If the dtype of the array is
     object, attempt converting to float, raising on failure.
```

### Comparing `tsml-0.1.1/tsml/vector/_cit.py` & `tsml-0.2.0/tsml/vector/_cit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-# -*- coding: utf-8 -*-
 """Continuous interval tree (CIT) vector classifier (aka Time Series Tree).
 
 Continuous Interval Tree aka Time Series Tree, base classifier originally used
-in the time series forest interval based classification algorithm. Fits sklearn
+in the time series forest interval-based classification algorithm. Fits sklearn
 conventions.
 """
 
 __author__ = ["MatthewMiddlehurst"]
 __all__ = ["CITClassifier"]
 
 import math
 import sys
+from typing import Union
 
 import numpy as np
+import pandas as pd
 from numba import njit
 from sklearn import preprocessing
 from sklearn.base import BaseEstimator, ClassifierMixin
 from sklearn.utils import check_random_state
 from sklearn.utils.multiclass import check_classification_targets
 from sklearn.utils.validation import check_is_fitted
 
@@ -41,101 +42,90 @@
         If `int`, random_state is the seed used by the random number generator;
         If `RandomState` instance, random_state is the random number generator;
         If `None`, the random number generator is the `RandomState` instance used
         by `np.random`.
 
     Attributes
     ----------
-    classes_ : list
-        The unique class labels in the training set.
-    n_classes_ : int
-        The number of unique classes in the training set.
     n_instances_ : int
         The number of train cases in the training set.
     n_atts_ : int
         The number of attributes in the training set.
-
-    See Also
-    --------
-    CanonicalIntervalForest
-    DrCIF
+    n_classes_ : int
+        Number of classes. Extracted from the data.
+    classes_ : ndarray of shape (n_classes_)
+        Holds the label for each class.
+    class_dictionary_ : dict
+        A dictionary mapping class labels to class indices in classes_.
 
     Notes
     -----
     For the Java version, see
     `tsml <https://github.com/uea-machine-learning/tsml/blob/master/src/main/java/
     machine_learning/classifiers/ContinuousIntervalTree.java>`_.
 
     References
     ----------
     .. [1] H.Deng, G.Runger, E.Tuv and M.Vladimir, "A time series forest for
-       classification and feature extraction",Information Sciences, 239, 2013
+       classification and feature extraction", Information Sciences, 239, 2013
 
     Examples
     --------
     >>> from tsml.vector import CITClassifier
-    >>> from tsml.datasets import load_minimal_chinatown
-    >>> X_train, y_train = load_minimal_chinatown(split="train")
-    >>> X_test, y_test = load_minimal_chinatown(split="test")
-    >>> clf = CITClassifier()
-    >>> clf.fit(X_train, y_train)
+    >>> from tsml.utils.testing import generate_2d_test_data
+    >>> X, y = generate_2d_test_data(n_samples=8, random_state=0)
+    >>> clf = CITClassifier(random_state=0)
+    >>> clf.fit(X, y)
     CITClassifier(...)
-    >>> y_pred = clf.predict(X_test)
+    >>> clf.predict(X)
+    array([0, 1, 0, 0, 0, 0, 0, 1])
     """
 
     def __init__(
         self,
         max_depth=sys.maxsize,
         thresholds=20,
         random_state=None,
     ):
         self.max_depth = max_depth
         self.thresholds = thresholds
         self.random_state = random_state
 
         super(CITClassifier, self).__init__()
 
-    def fit(self, X, y):
-        """Fit a tree on cases (X,y), where y is the target variable.
-
-        Build an information gain based tree for continuous attributes using the
-        margin gain metric for ties.
+    def fit(self, X: Union[np.ndarray, pd.DataFrame], y: np.ndarray) -> object:
+        """Fit the estimator to training data.
 
         Parameters
         ----------
-        X : 2d ndarray or DataFrame of shape = [n_instances, n_attributes]
+        X : 2d ndarray or DataFrame of shape (n_instances, n_atts)
             The training data.
-        y : array-like, shape = [n_instances]
-            The class labels.
+        y : 1D np.ndarray of shape (n_instances)
+            The class labels for fitting, indices correspond to instance indices in X
 
         Returns
         -------
         self :
             Reference to self.
-
-        Notes
-        -----
-        Changes state by creating a fitted model that updates attributes
-        ending in "_".
         """
         if isinstance(X, np.ndarray) and len(X.shape) == 3 and X.shape[1] == 1:
             X = np.reshape(X, (X.shape[0], -1))
 
         X, y = self._validate_data(
             X=X, y=y, ensure_min_samples=2, force_all_finite="allow-nan"
         )
 
         check_classification_targets(y)
 
         self.n_instances_, self.n_atts_ = X.shape
         self.classes_ = np.unique(y)
         self.n_classes_ = self.classes_.shape[0]
-        self._class_dictionary = {}
+        self.class_dictionary_ = {}
         for index, class_val in enumerate(self.classes_):
-            self._class_dictionary[class_val] = index
+            self.class_dictionary_[class_val] = index
 
         # escape if only one class seen
         if self.n_classes_ == 1:
             self._is_fitted = True
             return self
 
         le = preprocessing.LabelEncoder()
@@ -163,42 +153,42 @@
             self.n_classes_,
             False,
         )
 
         self._is_fitted = True
         return self
 
-    def predict(self, X):
-        """Predict for all cases in X. Built on top of predict_proba.
+    def predict(self, X: Union[np.ndarray, pd.DataFrame]) -> np.ndarray:
+        """Predicts labels for sequences in X.
 
         Parameters
         ----------
-        X : 2d ndarray or DataFrame of shape = [n_instances, n_attributes]
-            The data to make predictions for.
+        X : 2d ndarray or DataFrame of shape (n_instances, n_atts)
+            The testing data.
 
         Returns
         -------
-        y : array-like, shape = [n_instances]
+        y : array-like of shape (n_instances)
             Predicted class labels.
         """
         return np.array(
             [self.classes_[int(np.argmax(prob))] for prob in self.predict_proba(X)]
         )
 
-    def predict_proba(self, X):
-        """Probability estimates for each class for all cases in X.
+    def predict_proba(self, X: Union[np.ndarray, pd.DataFrame]) -> np.ndarray:
+        """Predicts labels probabilities for sequences in X.
 
         Parameters
         ----------
-        X : 2d ndarray or DataFrame of shape = [n_instances, n_attributes]
-            The data to make predictions for.
+        X : 2d ndarray or DataFrame of shape (n_instances, n_atts)
+            The testing data.
 
         Returns
         -------
-        y : array-like, shape = [n_instances, n_classes_]
+        y : array-like of shape (n_instances, n_classes_)
             Predicted probabilities using the ordering in classes_.
         """
         check_is_fitted(self)
 
         # treat case of single class seen in fit
         if self.n_classes_ == 1:
             return np.repeat([[1]], X.shape[0], axis=0)
@@ -228,15 +218,15 @@
         splits.append(node.best_split)
         gains.append(node.best_gain)
 
         for next_node in node.children:
             if next_node.best_split > -1:
                 self._find_splits_gain(next_node, splits, gains)
 
-    def _more_tags(self):
+    def _more_tags(self) -> dict:
         return {"allow_nan": True}
 
 
 class _TreeNode:
     """ContinuousIntervalTree tree node."""
 
     def __init__(
```

### Comparing `tsml-0.1.1/tsml/vector/_rotation_forest.py` & `tsml-0.2.0/tsml/vector/_rotation_forest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# -*- coding: utf-8 -*-
 """A rotation forest (RotF) vector classifier.
 
 A rotation Forest sktime implementation for continuous values only. Fits sklearn
 conventions.
 """
 
 __author__ = ["MatthewMiddlehurst"]
 __all__ = ["RotationForestClassifier", "RotationForestRegressor"]
 
 import time
+from typing import List, Union
 
 import numpy as np
+import pandas as pd
 from joblib import Parallel
 from sklearn.base import BaseEstimator, ClassifierMixin, RegressorMixin
 from sklearn.decomposition import PCA
 from sklearn.tree import DecisionTreeClassifier, DecisionTreeRegressor
 from sklearn.utils import check_random_state
 from sklearn.utils.fixes import delayed
 from sklearn.utils.multiclass import check_classification_targets
@@ -63,32 +64,30 @@
         If `int`, random_state is the seed used by the random number generator;
         If `RandomState` instance, random_state is the random number generator;
         If `None`, the random number generator is the `RandomState` instance used
         by `np.random`.
 
     Attributes
     ----------
-    classes_ : list
-        The unique class labels in the training set.
-    n_classes_ : int
-        The number of unique classes in the training set.
     n_instances_ : int
         The number of train cases in the training set.
     n_atts_ : int
         The number of attributes in the training set.
+    n_classes_ : int
+        Number of classes. Extracted from the data.
+    classes_ : ndarray of shape (n_classes_)
+        Holds the label for each class.
+    class_dictionary_ : dict
+        A dictionary mapping class labels to class indices in classes_.
     transformed_data_ : list of shape (n_estimators) of ndarray
         The transformed training dataset for all classifiers. Only saved when
         ``save_transformed_data`` is `True`.
     estimators_ : list of shape (n_estimators) of BaseEstimator
         The collections of estimators trained in fit.
 
-    See Also
-    --------
-    ShapeletTransformClassifier: A shapelet-based classifier using Rotation Forest.
-
     Notes
     -----
     For the Java version, see
     `tsml <https://github.com/uea-machine-learning/tsml/blob/master/src/main/java
     /weka/classifiers/meta/RotationForest.java>`_.
 
     References
@@ -99,21 +98,21 @@
 
     .. [2] Bagnall, A., et al. "Is rotation forest the best classifier for problems
        with continuous features?." arXiv preprint arXiv:1809.06705 (2018).
 
     Examples
     --------
     >>> from tsml.vector import RotationForestClassifier
-    >>> from tsml.datasets import load_minimal_chinatown
-    >>> X_train, y_train = load_minimal_chinatown(split="train")
-    >>> X_test, y_test = load_minimal_chinatown(split="test")
-    >>> clf = RotationForestClassifier(n_estimators=10)
-    >>> clf.fit(X_train, y_train)
+    >>> from tsml.utils.testing import generate_2d_test_data
+    >>> X, y = generate_2d_test_data(n_samples=8, random_state=0)
+    >>> clf = RotationForestClassifier(random_state=0)
+    >>> clf.fit(X, y)
     RotationForestClassifier(...)
-    >>> y_pred = clf.predict(X_test)
+    >>> clf.predict(X)
+    array([0, 1, 0, 0, 0, 0, 0, 1])
     """
 
     def __init__(
         self,
         n_estimators=200,
         min_group=3,
         max_group=3,
@@ -134,49 +133,44 @@
         self.contract_max_n_estimators = contract_max_n_estimators
         self.save_transformed_data = save_transformed_data
         self.n_jobs = n_jobs
         self.random_state = random_state
 
         super(RotationForestClassifier, self).__init__()
 
-    def fit(self, X, y):
-        """Fit a forest of trees on cases (X,y), where y is the target variable.
+    def fit(self, X: Union[np.ndarray, pd.DataFrame], y: np.ndarray) -> object:
+        """Fit the estimator to training data.
 
         Parameters
         ----------
-        X : 2d ndarray or DataFrame of shape = [n_instances, n_attributes]
+        X : 2d ndarray or DataFrame of shape (n_instances, n_atts)
             The training data.
-        y : array-like, shape = [n_instances]
-            The class labels.
+        y : 1D np.ndarray of shape (n_instances)
+            The class labels for fitting, indices correspond to instance indices in X
 
         Returns
         -------
         self :
             Reference to self.
-
-        Notes
-        -----
-        Changes state by creating a fitted model that updates attributes
-        ending in "_".
         """
         if isinstance(X, np.ndarray) and len(X.shape) == 3 and X.shape[1] == 1:
             X = np.reshape(X, (X.shape[0], -1))
 
         X, y = self._validate_data(X=X, y=y, ensure_min_samples=2, dtype=np.float32)
 
         check_classification_targets(y)
 
         self._n_jobs = check_n_jobs(self.n_jobs)
 
         self.n_instances_, self.n_atts_ = X.shape
         self.classes_ = np.unique(y)
         self.n_classes_ = self.classes_.shape[0]
-        self._class_dictionary = {}
+        self.class_dictionary_ = {}
         for index, class_val in enumerate(self.classes_):
-            self._class_dictionary[class_val] = index
+            self.class_dictionary_[class_val] = index
 
         # escape if only one class seen
         if self.n_classes_ == 1:
             self._is_fitted = True
             return self
 
         time_limit = self.time_limit_in_minutes * 60
@@ -244,42 +238,42 @@
 
             self.estimators_, self._pcas, self._groups, self.transformed_data_ = zip(
                 *fit
             )
 
         return self
 
-    def predict(self, X):
-        """Predict for all cases in X. Built on top of predict_proba.
+    def predict(self, X: Union[np.ndarray, pd.DataFrame]) -> np.ndarray:
+        """Predicts labels for sequences in X.
 
         Parameters
         ----------
-        X : 2d ndarray or DataFrame of shape = [n_instances, n_attributes]
-            The data to make predictions for.
+        X : 2d ndarray or DataFrame of shape (n_instances, n_atts)
+            The testing data.
 
         Returns
         -------
-        y : array-like, shape = [n_instances]
+        y : array-like of shape (n_instances)
             Predicted class labels.
         """
         return np.array(
             [self.classes_[int(np.argmax(prob))] for prob in self.predict_proba(X)]
         )
 
-    def predict_proba(self, X):
-        """Probability estimates for each class for all cases in X.
+    def predict_proba(self, X: Union[np.ndarray, pd.DataFrame]) -> np.ndarray:
+        """Predicts labels probabilities for sequences in X.
 
         Parameters
         ----------
-        X : 2d ndarray or DataFrame of shape = [n_instances, n_attributes]
-            The data to make predictions for.
+        X : 2d ndarray or DataFrame of shape (n_instances, n_atts)
+            The testing data.
 
         Returns
         -------
-        y : array-like, shape = [n_instances, n_classes_]
+        y : array-like of shape (n_instances, n_classes_)
             Predicted probabilities using the ordering in classes_.
         """
         check_is_fitted(self)
 
         # treat case of single class seen in fit
         if self.n_classes_ == 1:
             return np.repeat([[1]], X.shape[0], axis=0)
@@ -432,15 +426,15 @@
         )
 
         probas = clf.predict_proba(X_t)
 
         if probas.shape[1] != self.n_classes_:
             new_probas = np.zeros((probas.shape[0], self.n_classes_))
             for i, cls in enumerate(clf.classes_):
-                cls_idx = self._class_dictionary[cls]
+                cls_idx = self.class_dictionary_[cls]
                 new_probas[:, cls_idx] = probas[:, i]
             probas = new_probas
 
         return probas
 
     def _train_probas_for_estimator(self, y, idx):
         rs = 255 if self.random_state == 0 else self.random_state
@@ -462,73 +456,68 @@
         clf = _clone_estimator(self._base_estimator, rs)
         clf.fit(self.transformed_data_[idx][subsample], y[subsample])
         probas = clf.predict_proba(self.transformed_data_[idx][oob])
 
         if probas.shape[1] != self.n_classes_:
             new_probas = np.zeros((probas.shape[0], self.n_classes_))
             for i, cls in enumerate(clf.classes_):
-                cls_idx = self._class_dictionary[cls]
+                cls_idx = self.class_dictionary_[cls]
                 new_probas[:, cls_idx] = probas[:, i]
             probas = new_probas
 
         for n, proba in enumerate(probas):
             results[oob[n]] += proba
 
         return [results, oob]
 
     @classmethod
-    def get_test_params(cls, parameter_set=None):
+    def get_test_params(
+        cls, parameter_set: Union[str, None] = None
+    ) -> Union[dict, List[dict]]:
         """Return unit test parameter settings for the estimator.
 
         Parameters
         ----------
         parameter_set : None or str, default=None
             Name of the set of test parameters to return, for use in tests. If no
             special parameters are defined for a value, will return `"default"` set.
 
         Returns
         -------
-        params : dict or list of dict, default = {}
-            Parameters to create testing instances of the class
-            Each dict are parameters to construct an "interesting" test instance, i.e.,
-            `MyClass(**params)` or `MyClass(**params[i])` creates a valid test instance.
-            `create_test_instance` uses the first (or only) dictionary in `params`
+        params : dict or list of dict
+            Parameters to create testing instances of the class.
         """
-        if parameter_set is None:
-            return {"n_estimators": 2}
-        else:
-            raise ValueError(
-                f"No parameter set {parameter_set} defined for {cls.__name__}"
-            )
+        return {"n_estimators": 2}
 
 
 class RotationForestRegressor(RegressorMixin, BaseEstimator):
-    """A Rotation Forest (RotF) classifier.
+    """A Rotation Forest (RotF) regressor.
 
-    Implementation of the Rotation Forest classifier described in Rodriguez et al
-    (2013) [1]. Builds a forest of trees build on random portions of the data
-    transformed using PCA.
-
-    Intended as a benchmark for time series data and a base classifier for
-    transformation based appraoches such as ShapeletTransformClassifier, this tsml
-    implementation only works with continuous attributes.
+    Implementation of the Rotation Forest regressor based on the classifier described
+    in Rodriguez et al (2013) [1]. Builds a forest of trees build on random portions
+    of the data transformed using PCA.
+
+    Intended as a benchmark for time series data and a base regressor for
+    transformation based appraoches this tsml implementation only works with continuous
+    attributes. Compares to the classification version, the only alteration is the
+    base tree used and the removal of class subsampling.
 
     Parameters
     ----------
     n_estimators : int, default=200
         Number of estimators to build for the ensemble.
     min_group : int, default=3
         The minimum size of an attribute subsample group.
     max_group : int, default=3
         The maximum size of an attribute subsample group.
     remove_proportion : float, default=0.5
         The proportion of cases to be removed per group.
     base_estimator : BaseEstimator or None, default="None"
         Base estimator for the ensemble. By default, uses the sklearn
-        `DecisionTreeClassifier` using entropy as a splitting measure.
+        `DecisionTreeRegressor` using squared error as a splitting measure.
     time_limit_in_minutes : int, default=0
         Time contract to limit build time in minutes, overriding ``n_estimators``.
         Default of `0` means ``n_estimators`` is used.
     contract_max_n_estimators : int, default=500
         Max number of estimators to build when ``time_limit_in_minutes`` is set.
     save_transformed_data : bool, default=False
         Save the data transformed in fit in ``transformed_data_`` for use in
@@ -540,57 +529,45 @@
         If `int`, random_state is the seed used by the random number generator;
         If `RandomState` instance, random_state is the random number generator;
         If `None`, the random number generator is the `RandomState` instance used
         by `np.random`.
 
     Attributes
     ----------
-    classes_ : list
-        The unique class labels in the training set.
-    n_classes_ : int
-        The number of unique classes in the training set.
     n_instances_ : int
         The number of train cases in the training set.
     n_atts_ : int
         The number of attributes in the training set.
     transformed_data_ : list of shape (n_estimators) of ndarray
         The transformed training dataset for all classifiers. Only saved when
         ``save_transformed_data`` is `True`.
     estimators_ : list of shape (n_estimators) of BaseEstimator
         The collections of estimators trained in fit.
 
-    See Also
-    --------
-    ShapeletTransformClassifier: A shapelet-based classifier using Rotation Forest.
-
-    Notes
-    -----
-    For the Java version, see
-    `tsml <https://github.com/uea-machine-learning/tsml/blob/master/src/main/java
-    /weka/classifiers/meta/RotationForest.java>`_.
-
     References
     ----------
     .. [1] Rodriguez, Juan José, Ludmila I. Kuncheva, and Carlos J. Alonso. "Rotation
        forest: A new classifier ensemble method." IEEE transactions on pattern analysis
        and machine intelligence 28.10 (2006).
 
     .. [2] Bagnall, A., et al. "Is rotation forest the best classifier for problems
        with continuous features?." arXiv preprint arXiv:1809.06705 (2018).
 
     Examples
     --------
-    >>> from tsml.vector import RotationForestClassifier
-    >>> from tsml.datasets import load_minimal_chinatown
-    >>> X_train, y_train = load_minimal_chinatown(split="train")
-    >>> X_test, y_test = load_minimal_chinatown(split="test")
-    >>> clf = RotationForestClassifier(n_estimators=10)
-    >>> clf.fit(X_train, y_train)
-    RotationForestClassifier(...)
-    >>> y_pred = clf.predict(X_test)
+    >>> from tsml.vector import RotationForestRegressor
+    >>> from tsml.utils.testing import generate_2d_test_data
+    >>> X, y = generate_2d_test_data(n_samples=8, regression_target=True,
+    ...                              random_state=0)
+    >>> reg = RotationForestRegressor(random_state=0)
+    >>> reg.fit(X, y)
+    RotationForestRegressor(...)
+    >>> reg.predict(X)
+    array([0.19658236, 1.36872518, 0.82099324, 0.09710128, 0.83794492,
+           0.09609841, 0.97645944, 1.46865118])
     """
 
     def __init__(
         self,
         n_estimators=200,
         min_group=3,
         max_group=3,
@@ -611,38 +588,35 @@
         self.contract_max_n_estimators = contract_max_n_estimators
         self.save_transformed_data = save_transformed_data
         self.n_jobs = n_jobs
         self.random_state = random_state
 
         super(RotationForestRegressor, self).__init__()
 
-    def fit(self, X, y):
-        """Fit a forest of trees on cases (X,y), where y is the target variable.
+    def fit(self, X: Union[np.ndarray, pd.DataFrame], y: np.ndarray) -> object:
+        """Fit the estimator to training data.
 
         Parameters
         ----------
-        X : 2d ndarray or DataFrame of shape = [n_instances, n_attributes]
+        X : 2d ndarray or DataFrame of shape (n_instances, n_atts)
             The training data.
-        y : array-like, shape = [n_instances]
-            The class labels.
+        y : 1D np.ndarray of shape (n_instances)
+            The target labels for fitting, indices correspond to instance indices in X
 
         Returns
         -------
         self :
             Reference to self.
-
-        Notes
-        -----
-        Changes state by creating a fitted model that updates attributes
-        ending in "_".
         """
         if isinstance(X, np.ndarray) and len(X.shape) == 3 and X.shape[1] == 1:
             X = np.reshape(X, (X.shape[0], -1))
 
-        X, y = self._validate_data(X=X, y=y, ensure_min_samples=2, dtype=np.float32)
+        X, y = self._validate_data(
+            X=X, y=y, ensure_min_samples=2, dtype=np.float32, y_numeric=True
+        )
 
         self._n_jobs = check_n_jobs(self.n_jobs)
 
         self.n_instances_, self.n_atts_ = X.shape
 
         time_limit = self.time_limit_in_minutes * 60
         start_time = time.time()
@@ -705,26 +679,26 @@
 
             self.estimators_, self._pcas, self._groups, self.transformed_data_ = zip(
                 *fit
             )
 
         return self
 
-    def predict(self, X):
-        """Predict for all cases in X. Built on top of predict_proba.
+    def predict(self, X: Union[np.ndarray, pd.DataFrame]) -> np.ndarray:
+        """Predicts labels for sequences in X.
 
         Parameters
         ----------
-        X : 2d ndarray or DataFrame of shape = [n_instances, n_attributes]
-            The data to make predictions for.
+        X : 2d ndarray or DataFrame of shape (n_instances, n_atts)
+            The testing data.
 
         Returns
         -------
-        y : array-like, shape = [n_instances]
-            Predicted class labels.
+        y : array-like of shape (n_instances)
+            Predicted target labels.
         """
         check_is_fitted(self)
 
         if isinstance(X, np.ndarray) and len(X.shape) == 3 and X.shape[1] == 1:
             X = np.reshape(X, (X.shape[0], -1))
 
         X = self._validate_data(X=X, reset=False, dtype=np.float32)
@@ -811,37 +785,31 @@
         X_t = np.nan_to_num(
             X_t, False, 0, np.finfo(np.float32).max, np.finfo(np.float32).min
         )
 
         return clf.predict(X_t)
 
     @classmethod
-    def get_test_params(cls, parameter_set=None):
+    def get_test_params(
+        cls, parameter_set: Union[str, None] = None
+    ) -> Union[dict, List[dict]]:
         """Return unit test parameter settings for the estimator.
 
         Parameters
         ----------
         parameter_set : None or str, default=None
             Name of the set of test parameters to return, for use in tests. If no
             special parameters are defined for a value, will return `"default"` set.
 
         Returns
         -------
-        params : dict or list of dict, default = {}
-            Parameters to create testing instances of the class
-            Each dict are parameters to construct an "interesting" test instance, i.e.,
-            `MyClass(**params)` or `MyClass(**params[i])` creates a valid test instance.
-            `create_test_instance` uses the first (or only) dictionary in `params`
+        params : dict or list of dict
+            Parameters to create testing instances of the class.
         """
-        if parameter_set is None:
-            return {"n_estimators": 2}
-        else:
-            raise ValueError(
-                f"No parameter set {parameter_set} defined for {cls.__name__}"
-            )
+        return {"n_estimators": 2}
 
 
 def _generate_groups(rng, n_atts, min_group, max_group):
     permutation = rng.permutation((np.arange(0, n_atts)))
 
     # select the size of each group.
     group_size_count = np.zeros(max_group - min_group + 1)
```

### Comparing `tsml-0.1.1/tsml/vector/tests/test_rotation_forest.py` & `tsml-0.2.0/tsml/vector/tests/test_rotation_forest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Rotation Forest test code."""
 
 __author__ = ["MatthewMiddlehurst"]
 
 import numpy as np
 
 from tsml.datasets import load_minimal_chinatown
```

### Comparing `tsml-0.1.1/tsml.egg-info/PKG-INFO` & `tsml-0.2.0/tsml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsml
-Version: 0.1.1
+Version: 0.2.0
 Summary: A toolkit for time series machine learning algorithms.
 Author-email: Matthew Middlehurst <m.middlehurst@uea.ac.uk>, Tony Bagnall <ajb@uea.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) The Time Series Machine Learning (tsml) developers.
         All rights reserved.
         
@@ -49,14 +49,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: extras
 Provides-Extra: unstable_extras
 Provides-Extra: dev
+Provides-Extra: binder
 Provides-Extra: docs
 License-File: LICENSE
 
 # tsml
 
 A toolkit for time series machine learning algorithms
```

### Comparing `tsml-0.1.1/tsml.egg-info/SOURCES.txt` & `tsml-0.2.0/tsml.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 tsml/__init__.py
 tsml/base.py
 tsml.egg-info/PKG-INFO
 tsml.egg-info/SOURCES.txt
 tsml.egg-info/dependency_links.txt
 tsml.egg-info/requires.txt
 tsml.egg-info/top_level.txt
+tsml/compose/__init__.py
+tsml/compose/_channel_ensemble.py
+tsml/compose/tests/__init__.py
+tsml/compose/tests/test_channel_ensemble.py
 tsml/datasets/__init__.py
 tsml/datasets/_data_io.py
 tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts
 tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts
 tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts
 tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts
 tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts
@@ -25,49 +29,60 @@
 tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts
 tsml/datasets/tests/__init__.py
 tsml/datasets/tests/_expected_data_io_output.py
 tsml/datasets/tests/test_data_io.py
 tsml/distance_based/__init__.py
 tsml/distance_based/_mpdist.py
 tsml/distance_based/_pf.py
+tsml/distances/__init__.py
+tsml/distances/_manhattan.py
 tsml/dummy/__init__.py
 tsml/dummy/_dummy.py
 tsml/feature_based/__init__.py
 tsml/feature_based/_catch22.py
 tsml/feature_based/_fpca.py
+tsml/hybrid/__init__.py
+tsml/hybrid/_rist.py
 tsml/interval_based/__init__.py
 tsml/interval_based/_base.py
 tsml/interval_based/_cif.py
 tsml/interval_based/_interval_forest.py
 tsml/interval_based/_interval_pipelines.py
 tsml/interval_based/_rise.py
 tsml/interval_based/_stsf.py
 tsml/interval_based/_tsf.py
 tsml/interval_based/tests/__init__.py
 tsml/interval_based/tests/test_interval_forest.py
 tsml/shapelet_based/__init__.py
 tsml/shapelet_based/_mrsqm.py
+tsml/shapelet_based/_rdst.py
 tsml/shapelet_based/_rsf.py
 tsml/shapelet_based/_stc.py
 tsml/tests/__init__.py
-tsml/tests/_sklearn_checks.py
-tsml/tests/estimator_checks.py
 tsml/tests/test_all_estimators.py
+tsml/tests/test_estimator_checks.py
+tsml/tests/test_estimators_sklearn.py
 tsml/tests/test_interface.py
 tsml/transformations/__init__.py
 tsml/transformations/_acf.py
 tsml/transformations/_ar_coefficient.py
 tsml/transformations/_catch22.py
 tsml/transformations/_fpca.py
 tsml/transformations/_function_transformer.py
 tsml/transformations/_interval_extraction.py
 tsml/transformations/_periodogram.py
 tsml/transformations/_sfa.py
 tsml/transformations/_shapelet_transform.py
 tsml/transformations/_summary_features.py
+tsml/transformations/_transform_concatenator.py
+tsml/transformations/tests/__init__.py
+tsml/transformations/tests/test_function_transformer.py
+tsml/transformations/tests/test_interval_extraction.py
+tsml/transformations/tests/test_periodogram.py
+tsml/transformations/tests/test_transform_concatenator.py
 tsml/utils/__init__.py
 tsml/utils/_tags.py
 tsml/utils/discovery.py
 tsml/utils/testing.py
 tsml/utils/validation.py
 tsml/utils/numba_functions/__init__.py
 tsml/utils/numba_functions/general.py
```

### Comparing `tsml-0.1.1/tsml.egg-info/requires.txt` & `tsml-0.2.0/tsml.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 numba<0.58.0,>=0.55.0
 numpy<1.25.0,>=1.21.0
 pandas<2.1.0,>=1.5.3
 scikit-learn<1.3.0,>=1.0.0
 packaging<24.0,>=20.0
 
+[binder]
+notebook
+jupyterlab
+
 [dev]
 pre-commit
 pytest
 pytest-randomly
 pytest-timeout
 pytest-xdist
 pytest-cov
 
 [docs]
 sphinx
 sphinx-design
-sphinx-gallery
 nbsphinx
 numpydoc
 jupyter
 furo
+sphinx_issues
+myst-parser
+sphinx-copybutton
 
 [extras]
 pyfftw<0.14.0,>=0.12.0
 statsmodels<0.14.0,>=0.12.1
 wildboar<1.2.0,>=1.1.0
 stumpy<1.12.0,>=1.6.0
```

