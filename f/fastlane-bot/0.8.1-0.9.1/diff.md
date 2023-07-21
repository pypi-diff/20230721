# Comparing `tmp/fastlane_bot-0.8.1.tar.gz` & `tmp/fastlane_bot-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastlane_bot-0.8.1.tar", last modified: Fri Jul 21 19:10:46 2023, max compression
+gzip compressed data, was "fastlane_bot-0.9.1.tar", last modified: Fri Jul 21 19:12:21 2023, max compression
```

## Comparing `fastlane_bot-0.8.1.tar` & `fastlane_bot-0.9.1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:46.058072 fastlane_bot-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-21 19:10:46.058072 fastlane_bot-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:46.042072 fastlane_bot-0.8.1/fastlane_bot/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43066 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:46.042072 fastlane_bot-0.8.1/fastlane_bot/config/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/config/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/config/cloaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/config/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/config/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/config/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/config/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/config/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/config/selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:46.046072 fastlane_bot-0.8.1/fastlane_bot/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   192059 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/data/abi.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/data/pools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:46.046072 fastlane_bot-0.8.1/fastlane_bot/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:46.046072 fastlane_bot-0.8.1/fastlane_bot/events/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/exchanges/bancor_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/exchanges/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/exchanges/carbon_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/exchanges/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/exchanges/sushiswap_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/exchanges/uniswap_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/exchanges/uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:46.046072 fastlane_bot-0.8.1/fastlane_bot/events/managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/managers/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/managers/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/managers/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/managers/pools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:46.050072 fastlane_bot-0.8.1/fastlane_bot/events/pools/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/pools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/pools/bancor_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/pools/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/pools/carbon_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/pools/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/pools/sushiswap_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/pools/uniswap_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/pools/uniswap_v3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:46.050072 fastlane_bot-0.8.1/fastlane_bot/events/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/tests/convert_py_test_to_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/tests/test_exchanges.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14390 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/tests/test_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:46.050072 fastlane_bot-0.8.1/fastlane_bot/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/helpers/poolandtokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/helpers/receipthandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    41479 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/helpers/routehandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/helpers/submithandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/helpers/tradeinstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    30259 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/helpers/txhelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/helpers/univ3calc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:46.054072 fastlane_bot-0.8.1/fastlane_bot/modes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/modes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/modes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/modes/base_pairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/modes/base_triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/modes/pairwise_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/modes/pairwise_single.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:46.054072 fastlane_bot-0.8.1/fastlane_bot/modes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/modes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/modes/tests/test_pairwise_single.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/modes/triangle_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/modes/triangle_single.py
--rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/modes/triangle_single_bancor3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:46.058072 fastlane_bot-0.8.1/fastlane_bot/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/tools/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    75829 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/tools/arbgraphs.py
--rw-r--r--   0 runner    (1001) docker     (123)    85741 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/tools/cpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    70412 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/tools/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/tools/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/tools/simplepair.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/tools/tokenscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/tools/univ3calc_DELETE.py
--rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/fastlane_bot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:46.042072 fastlane_bot-0.8.1/fastlane_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-21 19:10:45.000000 fastlane_bot-0.8.1/fastlane_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-21 19:10:46.000000 fastlane_bot-0.8.1/fastlane_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 19:10:45.000000 fastlane_bot-0.8.1/fastlane_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-21 19:10:45.000000 fastlane_bot-0.8.1/fastlane_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 19:10:45.000000 fastlane_bot-0.8.1/fastlane_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 19:10:46.058072 fastlane_bot-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-21 19:09:23.000000 fastlane_bot-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:21.002983 fastlane_bot-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-21 19:12:21.002983 fastlane_bot-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:20.990982 fastlane_bot-0.9.1/fastlane_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43066 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:20.994982 fastlane_bot-0.9.1/fastlane_bot/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/config/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/config/cloaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/config/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/config/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/config/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/config/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/config/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/config/selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:20.994982 fastlane_bot-0.9.1/fastlane_bot/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192059 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/data/abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/data/pools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:20.994982 fastlane_bot-0.9.1/fastlane_bot/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:20.994982 fastlane_bot-0.9.1/fastlane_bot/events/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/exchanges/bancor_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/exchanges/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/exchanges/carbon_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/exchanges/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/exchanges/sushiswap_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/exchanges/uniswap_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/exchanges/uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:20.994982 fastlane_bot-0.9.1/fastlane_bot/events/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/managers/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/managers/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/managers/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/managers/pools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:20.998983 fastlane_bot-0.9.1/fastlane_bot/events/pools/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/pools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/pools/bancor_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/pools/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/pools/carbon_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/pools/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/pools/sushiswap_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/pools/uniswap_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/pools/uniswap_v3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:20.998983 fastlane_bot-0.9.1/fastlane_bot/events/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/tests/convert_py_test_to_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/tests/test_exchanges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14390 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/tests/test_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:20.998983 fastlane_bot-0.9.1/fastlane_bot/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/helpers/poolandtokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/helpers/receipthandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41479 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/helpers/routehandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/helpers/submithandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/helpers/tradeinstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30259 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/helpers/txhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/helpers/univ3calc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:21.002983 fastlane_bot-0.9.1/fastlane_bot/modes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/modes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/modes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/modes/base_pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/modes/base_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/modes/pairwise_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/modes/pairwise_single.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:21.002983 fastlane_bot-0.9.1/fastlane_bot/modes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/modes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/modes/tests/test_pairwise_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/modes/triangle_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/modes/triangle_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/modes/triangle_single_bancor3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:21.002983 fastlane_bot-0.9.1/fastlane_bot/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/tools/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75829 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/tools/arbgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85741 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/tools/cpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70412 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/tools/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/tools/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/tools/simplepair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/tools/tokenscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/tools/univ3calc_DELETE.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/fastlane_bot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:12:20.990982 fastlane_bot-0.9.1/fastlane_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-21 19:12:20.000000 fastlane_bot-0.9.1/fastlane_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-21 19:12:20.000000 fastlane_bot-0.9.1/fastlane_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 19:12:20.000000 fastlane_bot-0.9.1/fastlane_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-21 19:12:20.000000 fastlane_bot-0.9.1/fastlane_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 19:12:20.000000 fastlane_bot-0.9.1/fastlane_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 19:12:21.002983 fastlane_bot-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-21 19:10:53.000000 fastlane_bot-0.9.1/setup.py
```

### Comparing `fastlane_bot-0.8.1/LICENSE` & `fastlane_bot-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/PKG-INFO` & `fastlane_bot-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastlane_bot
-Version: 0.8.1
+Version: 0.9.1
 Summary: Carbon Arbitrage Bot, an open-source arbitrage protocol, allows any user to perform arbitrage between Bancor ecosystem protocols and external exchanges and redirect arbitrage profits back to the protocol.
 Home-page: https://github.com/bancorprotocol/carbon-bot
 Author: Bancor Network
 Author-email: mike@bancor.network
 Requires-Python: >= 3.8, != 3.11.*
 Description-Content-Type: text/markdown
 Provides-Extra: complete
```

### Comparing `fastlane_bot-0.8.1/README.md` & `fastlane_bot-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/bot.py` & `fastlane_bot-0.9.1/fastlane_bot/bot.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/config/base.py` & `fastlane_bot-0.9.1/fastlane_bot/config/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/config/cloaker.py` & `fastlane_bot-0.9.1/fastlane_bot/config/cloaker.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/config/config.py` & `fastlane_bot-0.9.1/fastlane_bot/config/config.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/config/connect.py` & `fastlane_bot-0.9.1/fastlane_bot/config/connect.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/config/db.py` & `fastlane_bot-0.9.1/fastlane_bot/config/db.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/config/logger.py` & `fastlane_bot-0.9.1/fastlane_bot/config/logger.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/config/network.py` & `fastlane_bot-0.9.1/fastlane_bot/config/network.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/config/provider.py` & `fastlane_bot-0.9.1/fastlane_bot/config/provider.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/config/selectors.py` & `fastlane_bot-0.9.1/fastlane_bot/config/selectors.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/data/abi.py` & `fastlane_bot-0.9.1/fastlane_bot/data/abi.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/data/pools.py` & `fastlane_bot-0.9.1/fastlane_bot/data/pools.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/exchanges/__init__.py` & `fastlane_bot-0.9.1/fastlane_bot/events/exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/exchanges/bancor_v3.py` & `fastlane_bot-0.9.1/fastlane_bot/events/exchanges/bancor_v3.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/exchanges/base.py` & `fastlane_bot-0.9.1/fastlane_bot/events/exchanges/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/exchanges/carbon_v1.py` & `fastlane_bot-0.9.1/fastlane_bot/events/exchanges/carbon_v1.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/exchanges/factory.py` & `fastlane_bot-0.9.1/fastlane_bot/events/exchanges/factory.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/exchanges/sushiswap_v2.py` & `fastlane_bot-0.9.1/fastlane_bot/events/exchanges/sushiswap_v2.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/exchanges/uniswap_v2.py` & `fastlane_bot-0.9.1/fastlane_bot/events/exchanges/uniswap_v2.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/exchanges/uniswap_v3.py` & `fastlane_bot-0.9.1/fastlane_bot/events/exchanges/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/interface.py` & `fastlane_bot-0.9.1/fastlane_bot/events/interface.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/managers/base.py` & `fastlane_bot-0.9.1/fastlane_bot/events/managers/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/managers/contracts.py` & `fastlane_bot-0.9.1/fastlane_bot/events/managers/contracts.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/managers/events.py` & `fastlane_bot-0.9.1/fastlane_bot/events/managers/events.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/managers/manager.py` & `fastlane_bot-0.9.1/fastlane_bot/events/managers/manager.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/managers/pools.py` & `fastlane_bot-0.9.1/fastlane_bot/events/managers/pools.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/pools/__init__.py` & `fastlane_bot-0.9.1/fastlane_bot/events/pools/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/pools/bancor_v3.py` & `fastlane_bot-0.9.1/fastlane_bot/events/pools/bancor_v3.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/pools/base.py` & `fastlane_bot-0.9.1/fastlane_bot/events/pools/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/pools/carbon_v1.py` & `fastlane_bot-0.9.1/fastlane_bot/events/pools/carbon_v1.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/pools/factory.py` & `fastlane_bot-0.9.1/fastlane_bot/events/pools/factory.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/pools/sushiswap_v2.py` & `fastlane_bot-0.9.1/fastlane_bot/events/pools/sushiswap_v2.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/pools/uniswap_v2.py` & `fastlane_bot-0.9.1/fastlane_bot/events/pools/uniswap_v2.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/pools/uniswap_v3.py` & `fastlane_bot-0.9.1/fastlane_bot/events/pools/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/tests/convert_py_test_to_jupyter.py` & `fastlane_bot-0.9.1/fastlane_bot/events/tests/convert_py_test_to_jupyter.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/tests/test_exchanges.py` & `fastlane_bot-0.9.1/fastlane_bot/events/tests/test_exchanges.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/tests/test_interface.py` & `fastlane_bot-0.9.1/fastlane_bot/events/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/tests/test_manager.py` & `fastlane_bot-0.9.1/fastlane_bot/events/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/tests/test_pools.py` & `fastlane_bot-0.9.1/fastlane_bot/events/tests/test_pools.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/tests/test_utils.py` & `fastlane_bot-0.9.1/fastlane_bot/events/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/events/utils.py` & `fastlane_bot-0.9.1/fastlane_bot/events/utils.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/helpers/poolandtokens.py` & `fastlane_bot-0.9.1/fastlane_bot/helpers/poolandtokens.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/helpers/routehandler.py` & `fastlane_bot-0.9.1/fastlane_bot/helpers/routehandler.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/helpers/submithandler.py` & `fastlane_bot-0.9.1/fastlane_bot/helpers/submithandler.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/helpers/tradeinstruction.py` & `fastlane_bot-0.9.1/fastlane_bot/helpers/tradeinstruction.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/helpers/txhelpers.py` & `fastlane_bot-0.9.1/fastlane_bot/helpers/txhelpers.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/helpers/univ3calc.py` & `fastlane_bot-0.9.1/fastlane_bot/helpers/univ3calc.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/modes/base.py` & `fastlane_bot-0.9.1/fastlane_bot/modes/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/modes/base_pairwise.py` & `fastlane_bot-0.9.1/fastlane_bot/modes/base_pairwise.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/modes/base_triangle.py` & `fastlane_bot-0.9.1/fastlane_bot/modes/base_triangle.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/modes/pairwise_multi.py` & `fastlane_bot-0.9.1/fastlane_bot/modes/pairwise_multi.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/modes/pairwise_single.py` & `fastlane_bot-0.9.1/fastlane_bot/modes/pairwise_single.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/modes/tests/test_pairwise_single.py` & `fastlane_bot-0.9.1/fastlane_bot/modes/tests/test_pairwise_single.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/modes/triangle_multi.py` & `fastlane_bot-0.9.1/fastlane_bot/modes/triangle_multi.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/modes/triangle_single.py` & `fastlane_bot-0.9.1/fastlane_bot/modes/triangle_single.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/modes/triangle_single_bancor3.py` & `fastlane_bot-0.9.1/fastlane_bot/modes/triangle_single_bancor3.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/testing.py` & `fastlane_bot-0.9.1/fastlane_bot/testing.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/tools/analyzer.py` & `fastlane_bot-0.9.1/fastlane_bot/tools/analyzer.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/tools/arbgraphs.py` & `fastlane_bot-0.9.1/fastlane_bot/tools/arbgraphs.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/tools/cpc.py` & `fastlane_bot-0.9.1/fastlane_bot/tools/cpc.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/tools/optimizer.py` & `fastlane_bot-0.9.1/fastlane_bot/tools/optimizer.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/tools/params.py` & `fastlane_bot-0.9.1/fastlane_bot/tools/params.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/tools/simplepair.py` & `fastlane_bot-0.9.1/fastlane_bot/tools/simplepair.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/tools/tokenscale.py` & `fastlane_bot-0.9.1/fastlane_bot/tools/tokenscale.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/tools/univ3calc_DELETE.py` & `fastlane_bot-0.9.1/fastlane_bot/tools/univ3calc_DELETE.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot/utils.py` & `fastlane_bot-0.9.1/fastlane_bot/utils.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/fastlane_bot.egg-info/PKG-INFO` & `fastlane_bot-0.9.1/fastlane_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastlane-bot
-Version: 0.8.1
+Version: 0.9.1
 Summary: Carbon Arbitrage Bot, an open-source arbitrage protocol, allows any user to perform arbitrage between Bancor ecosystem protocols and external exchanges and redirect arbitrage profits back to the protocol.
 Home-page: https://github.com/bancorprotocol/carbon-bot
 Author: Bancor Network
 Author-email: mike@bancor.network
 Requires-Python: >= 3.8, != 3.11.*
 Description-Content-Type: text/markdown
 Provides-Extra: complete
```

### Comparing `fastlane_bot-0.8.1/fastlane_bot.egg-info/SOURCES.txt` & `fastlane_bot-0.9.1/fastlane_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastlane_bot-0.8.1/setup.py` & `fastlane_bot-0.9.1/setup.py`

 * *Files identical despite different names*

