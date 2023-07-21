# Comparing `tmp/openskill-4.0.0.tar.gz` & `tmp/openskill-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openskill-4.0.0.tar", last modified: Sun Dec 11 10:01:40 2022, max compression
+gzip compressed data, was "openskill-5.0.0.tar", last modified: Fri Jul 21 18:14:00 2023, max compression
```

## Comparing `openskill-4.0.0.tar` & `openskill-5.0.0.tar`

### file list

```diff
@@ -1,74 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:01:40.205641 openskill-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2022-12-11 10:01:26.000000 openskill-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10395 2022-12-11 10:01:40.205641 openskill-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8944 2022-12-11 10:01:26.000000 openskill-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:01:40.197641 openskill-4.0.0/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 10:01:26.000000 openskill-4.0.0/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2022-12-11 10:01:26.000000 openskill-4.0.0/benchmark/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:01:40.197641 openskill-4.0.0/benchmark/processors/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-11 10:01:26.000000 openskill-4.0.0/benchmark/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13407 2022-12-11 10:01:26.000000 openskill-4.0.0/benchmark/processors/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)    13525 2022-12-11 10:01:26.000000 openskill-4.0.0/benchmark/processors/rank.py
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2022-12-11 10:01:26.000000 openskill-4.0.0/benchmark/processors/win.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:01:40.197641 openskill-4.0.0/openskill/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2022-12-11 10:01:26.000000 openskill-4.0.0/openskill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2022-12-11 10:01:26.000000 openskill-4.0.0/openskill/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:01:40.201641 openskill-4.0.0/openskill/models/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2022-12-11 10:01:26.000000 openskill-4.0.0/openskill/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2022-12-11 10:01:26.000000 openskill-4.0.0/openskill/models/bradley_terry_full.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2022-12-11 10:01:26.000000 openskill-4.0.0/openskill/models/bradley_terry_part.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2022-12-11 10:01:26.000000 openskill-4.0.0/openskill/models/plackett_luce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2022-12-11 10:01:26.000000 openskill-4.0.0/openskill/models/thurstone_mosteller_full.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2022-12-11 10:01:26.000000 openskill-4.0.0/openskill/models/thurstone_mosteller_part.py
--rw-r--r--   0 runner    (1001) docker     (123)    17793 2022-12-11 10:01:26.000000 openskill-4.0.0/openskill/rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2022-12-11 10:01:26.000000 openskill-4.0.0/openskill/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2022-12-11 10:01:26.000000 openskill-4.0.0/openskill/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:01:40.201641 openskill-4.0.0/openskill.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10395 2022-12-11 10:01:40.000000 openskill-4.0.0/openskill.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2022-12-11 10:01:40.000000 openskill-4.0.0/openskill.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-11 10:01:40.000000 openskill-4.0.0/openskill.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2022-12-11 10:01:40.000000 openskill-4.0.0/openskill.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-11 10:01:40.000000 openskill-4.0.0/openskill.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2022-12-11 10:01:26.000000 openskill-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2022-12-11 10:01:40.205641 openskill-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-11 10:01:26.000000 openskill-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:01:40.201641 openskill-4.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:01:40.201641 openskill-4.0.0/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/models/test_bradley_terry_full.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/models/test_bradley_terry_full_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/models/test_bradley_terry_part.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/models/test_bradley_terry_part_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/models/test_plackett_luce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/models/test_plackett_luce_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/models/test_thurstone_mosteller_full.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/models/test_thurstone_mosteller_full_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/models/test_thurstone_mosteller_part.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/models/test_thurstone_mosteller_part_series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:01:40.201641 openskill-4.0.0/tests/predictions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/predictions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/predictions/test_predict_draw.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/predictions/test_predict_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/predictions/test_predict_win.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:01:40.201641 openskill-4.0.0/tests/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/statistics/test_v.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/statistics/test_vt.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/statistics/test_w.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/statistics/test_wt.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/test_create_rating.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/test_ordinal.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/test_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/test_rating.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/test_team_rating.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:01:40.205641 openskill-4.0.0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/util/test_ladder_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/util/test_rankings.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/util/test_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/util/test_unwind.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/util/test_util_a.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/util/test_util_c.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2022-12-11 10:01:26.000000 openskill-4.0.0/tests/util/test_util_sum_q.py
+-rw-r--r--   0        0        0     5805 2023-07-21 18:13:47.182139 openskill-5.0.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     1068 2023-07-21 18:13:47.182139 openskill-5.0.0/LICENSE
+-rw-r--r--   0        0        0     1068 2023-07-21 18:13:47.182139 openskill-5.0.0/LICENSE
+-rw-r--r--   0        0        0     4099 2023-07-21 18:13:47.182139 openskill-5.0.0/README.md
+-rw-r--r--   0        0        0     4099 2023-07-21 18:13:47.182139 openskill-5.0.0/README.md
+-rw-r--r--   0        0        0      338 2023-07-21 18:13:47.274139 openskill-5.0.0/openskill/__init__.py
+-rw-r--r--   0        0        0      836 2023-07-21 18:13:47.274139 openskill-5.0.0/openskill/models/__init__.py
+-rw-r--r--   0        0        0     1838 2023-07-21 18:13:47.274139 openskill-5.0.0/openskill/models/common.py
+-rw-r--r--   0        0        0     1102 2023-07-21 18:13:47.274139 openskill-5.0.0/openskill/models/weng_lin/__init__.py
+-rw-r--r--   0        0        0    33457 2023-07-21 18:13:47.274139 openskill-5.0.0/openskill/models/weng_lin/bradley_terry_full.py
+-rw-r--r--   0        0        0    33958 2023-07-21 18:13:47.274139 openskill-5.0.0/openskill/models/weng_lin/bradley_terry_part.py
+-rw-r--r--   0        0        0     4693 2023-07-21 18:13:47.274139 openskill-5.0.0/openskill/models/weng_lin/common.py
+-rw-r--r--   0        0        0    33088 2023-07-21 18:13:47.274139 openskill-5.0.0/openskill/models/weng_lin/plackett_luce.py
+-rw-r--r--   0        0        0    34863 2023-07-21 18:13:47.274139 openskill-5.0.0/openskill/models/weng_lin/thurstone_mosteller_full.py
+-rw-r--r--   0        0        0    35433 2023-07-21 18:13:47.278139 openskill-5.0.0/openskill/models/weng_lin/thurstone_mosteller_part.py
+-rw-r--r--   0        0        0        0 2023-07-21 18:13:47.278139 openskill-5.0.0/openskill/py.typed
+-rw-r--r--   0        0        0     3396 2023-07-21 18:14:00.486146 openskill-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 18:13:47.278139 openskill-5.0.0/tests/__init__.py
+-rw-r--r--   0        0        0       38 2023-07-21 18:13:47.278139 openskill-5.0.0/tests/models/__init__.py
+-rw-r--r--   0        0        0     2936 2023-07-21 18:13:47.278139 openskill-5.0.0/tests/models/data/bradleyterryfull.json
+-rw-r--r--   0        0        0     2959 2023-07-21 18:13:47.278139 openskill-5.0.0/tests/models/data/bradleyterrypart.json
+-rw-r--r--   0        0        0     2955 2023-07-21 18:13:47.278139 openskill-5.0.0/tests/models/data/plackettluce.json
+-rw-r--r--   0        0        0     2941 2023-07-21 18:13:47.278139 openskill-5.0.0/tests/models/data/thurstonemostellerfull.json
+-rw-r--r--   0        0        0     2968 2023-07-21 18:13:47.278139 openskill-5.0.0/tests/models/data/thurstonemostellerpart.json
+-rw-r--r--   0        0        0     3333 2023-07-21 18:13:47.278139 openskill-5.0.0/tests/models/generate.py
+-rw-r--r--   0        0        0     1848 2023-07-21 18:13:47.278139 openskill-5.0.0/tests/models/test_common.py
+-rw-r--r--   0        0        0       47 2023-07-21 18:13:47.278139 openskill-5.0.0/tests/models/weng_lin/__init__.py
+-rw-r--r--   0        0        0    15423 2023-07-21 18:13:47.278139 openskill-5.0.0/tests/models/weng_lin/test_bradley_terry_full.py
+-rw-r--r--   0        0        0    15503 2023-07-21 18:13:47.278139 openskill-5.0.0/tests/models/weng_lin/test_bradley_terry_part.py
+-rw-r--r--   0        0        0     5953 2023-07-21 18:13:47.278139 openskill-5.0.0/tests/models/weng_lin/test_common.py
+-rw-r--r--   0        0        0    15192 2023-07-21 18:13:47.278139 openskill-5.0.0/tests/models/weng_lin/test_plackett_luce.py
+-rw-r--r--   0        0        0    15732 2023-07-21 18:13:47.278139 openskill-5.0.0/tests/models/weng_lin/test_thurstone_mosteller_full.py
+-rw-r--r--   0        0        0    15816 2023-07-21 18:13:47.278139 openskill-5.0.0/tests/models/weng_lin/test_thurstone_mosteller_part.py
+-rw-r--r--   0        0        0     5370 1970-01-01 00:00:00.000000 openskill-5.0.0/PKG-INFO
```

### Comparing `openskill-4.0.0/LICENSE` & `openskill-5.0.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 Open Debates Project
+Copyright (c) 2023 Vivek Joshy
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

