# Comparing `tmp/crypto-screening-7.4.2.tar.gz` & `tmp/crypto-screening-7.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-7.4.2.tar", last modified: Thu Jul 20 19:14:32 2023, max compression
+gzip compressed data, was "crypto-screening-7.4.3.tar", last modified: Fri Jul 21 12:51:21 2023, max compression
```

## Comparing `crypto-screening-7.4.2.tar` & `crypto-screening-7.4.3.tar`

### file list

```diff
@@ -1,64 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 19:14:32.042902 crypto-screening-7.4.2/
--rw-rw-rw-   0        0        0       98 2023-07-20 19:14:31.000000 crypto-screening-7.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-20 19:14:32.042902 crypto-screening-7.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-7.4.2/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-7.4.2/build.py
-drwxrwxrwx   0        0        0        0 2023-07-20 19:14:32.001896 crypto-screening-7.4.2/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-20 19:14:32.021896 crypto-screening-7.4.2/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-7.4.2/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-7.4.2/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-20 19:14:32.024896 crypto-screening-7.4.2/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-7.4.2/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-7.4.2/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-7.4.2/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-7.4.2/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-20 19:14:32.027896 crypto-screening-7.4.2/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-7.4.2/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24729 2023-07-20 08:01:55.000000 crypto-screening-7.4.2/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    16341 2023-07-20 15:18:05.000000 crypto-screening-7.4.2/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21717 2023-07-20 08:01:55.000000 crypto-screening-7.4.2/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-7.4.2/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    16799 2023-07-20 15:36:57.000000 crypto-screening-7.4.2/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    19009 2023-07-18 17:15:01.000000 crypto-screening-7.4.2/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-7.4.2/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-7.4.2/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-7.4.2/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-20 19:14:32.028897 crypto-screening-7.4.2/crypto_screening/market/
--rw-rw-rw-   0        0        0    21478 2023-07-20 14:19:49.000000 crypto-screening-7.4.2/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-20 19:14:32.031896 crypto-screening-7.4.2/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10654 2023-07-18 21:40:34.000000 crypto-screening-7.4.2/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-7.4.2/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-7.4.2/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-7.4.2/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-20 19:14:32.039900 crypto-screening-7.4.2/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      519 2023-07-20 15:38:19.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    11649 2023-07-20 15:46:53.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0    13798 2023-07-20 15:24:13.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/callbacks.py
-drwxrwxrwx   0        0        0        0 2023-07-20 19:14:32.041900 crypto-screening-7.4.2/crypto_screening/market/screeners/collectors/
--rw-rw-rw-   0        0        0      217 2023-07-20 15:09:26.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/collectors/__init__.py
--rw-rw-rw-   0        0        0     3645 2023-07-20 15:49:53.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/collectors/base.py
--rw-rw-rw-   0        0        0     4109 2023-07-20 15:57:21.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/collectors/database.py
--rw-rw-rw-   0        0        0     5952 2023-07-20 15:13:32.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/collectors/sockets.py
--rw-rw-rw-   0        0        0    13450 2023-07-20 08:33:40.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/combined.py
--rw-rw-rw-   0        0        0    20745 2023-07-20 19:14:02.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    10926 2023-07-20 15:55:41.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/database.py
--rw-rw-rw-   0        0        0    38137 2023-07-20 08:32:44.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    19664 2023-07-20 08:24:01.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    19155 2023-07-20 08:24:01.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/orders.py
--rw-rw-rw-   0        0        0    20611 2023-07-19 16:46:01.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0    19229 2023-07-20 08:24:01.000000 crypto-screening-7.4.2/crypto_screening/market/screeners/trades.py
--rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-7.4.2/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-7.4.2/crypto_screening/process.py
--rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-7.4.2/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3599 2023-07-18 22:07:23.000000 crypto-screening-7.4.2/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-20 19:14:32.018927 crypto-screening-7.4.2/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-20 19:14:31.000000 crypto-screening-7.4.2/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1989 2023-07-20 19:14:31.000000 crypto-screening-7.4.2/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 19:14:31.000000 crypto-screening-7.4.2/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-20 19:14:31.000000 crypto-screening-7.4.2/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-20 19:14:31.000000 crypto-screening-7.4.2/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-20 19:14:31.000000 crypto-screening-7.4.2/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-7.4.2/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-7.4.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 19:14:32.043900 crypto-screening-7.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-20 19:14:15.000000 crypto-screening-7.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:51:21.867126 crypto-screening-7.4.3/
+-rw-rw-rw-   0        0        0      196 2023-07-21 12:51:21.000000 crypto-screening-7.4.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-21 12:51:21.867126 crypto-screening-7.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-7.4.3/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-7.4.3/build.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:51:21.833126 crypto-screening-7.4.3/crypto_screening/
+-rw-rw-rw-   0        0        0     1002 2023-07-21 10:49:22.000000 crypto-screening-7.4.3/crypto_screening/base.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:51:21.845126 crypto-screening-7.4.3/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-7.4.3/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-7.4.3/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:51:21.849126 crypto-screening-7.4.3/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-7.4.3/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-7.4.3/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-7.4.3/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-7.4.3/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:51:21.851127 crypto-screening-7.4.3/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-7.4.3/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24729 2023-07-20 08:01:55.000000 crypto-screening-7.4.3/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    16341 2023-07-21 10:15:56.000000 crypto-screening-7.4.3/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21717 2023-07-20 08:01:55.000000 crypto-screening-7.4.3/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-7.4.3/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    16799 2023-07-20 15:36:57.000000 crypto-screening-7.4.3/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    19514 2023-07-21 10:12:10.000000 crypto-screening-7.4.3/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-7.4.3/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0     1007 2023-07-21 10:52:54.000000 crypto-screening-7.4.3/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-7.4.3/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:51:21.853126 crypto-screening-7.4.3/crypto_screening/market/
+-rw-rw-rw-   0        0        0    20207 2023-07-21 08:45:09.000000 crypto-screening-7.4.3/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:51:21.855127 crypto-screening-7.4.3/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10654 2023-07-18 21:40:34.000000 crypto-screening-7.4.3/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-7.4.3/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-7.4.3/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-7.4.3/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:51:21.863127 crypto-screening-7.4.3/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      519 2023-07-20 15:38:19.000000 crypto-screening-7.4.3/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    12013 2023-07-21 12:46:02.000000 crypto-screening-7.4.3/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0    13798 2023-07-20 15:24:13.000000 crypto-screening-7.4.3/crypto_screening/market/screeners/callbacks.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:51:21.865126 crypto-screening-7.4.3/crypto_screening/market/screeners/collectors/
+-rw-rw-rw-   0        0        0      217 2023-07-20 15:09:26.000000 crypto-screening-7.4.3/crypto_screening/market/screeners/collectors/__init__.py
+-rw-rw-rw-   0        0        0     3648 2023-07-21 08:45:09.000000 crypto-screening-7.4.3/crypto_screening/market/screeners/collectors/base.py
+-rw-rw-rw-   0        0        0     3988 2023-07-21 08:58:50.000000 crypto-screening-7.4.3/crypto_screening/market/screeners/collectors/database.py
+-rw-rw-rw-   0        0        0     5952 2023-07-20 15:13:32.000000 crypto-screening-7.4.3/crypto_screening/market/screeners/collectors/sockets.py
+-rw-rw-rw-   0        0        0    13450 2023-07-20 08:33:40.000000 crypto-screening-7.4.3/crypto_screening/market/screeners/combined.py
+-rw-rw-rw-   0        0        0    21490 2023-07-21 09:39:08.000000 crypto-screening-7.4.3/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    10983 2023-07-21 08:58:32.000000 crypto-screening-7.4.3/crypto_screening/market/screeners/database.py
+-rw-rw-rw-   0        0        0    37526 2023-07-21 11:02:21.000000 crypto-screening-7.4.3/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    17713 2023-07-21 12:44:32.000000 crypto-screening-7.4.3/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    17240 2023-07-21 12:44:17.000000 crypto-screening-7.4.3/crypto_screening/market/screeners/orders.py
+-rw-rw-rw-   0        0        0    20611 2023-07-19 16:46:01.000000 crypto-screening-7.4.3/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0    17314 2023-07-21 12:44:28.000000 crypto-screening-7.4.3/crypto_screening/market/screeners/trades.py
+-rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-7.4.3/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-7.4.3/crypto_screening/process.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:51:21.822788 crypto-screening-7.4.3/crypto_screening/source/
+drwxrwxrwx   0        0        0        0 2023-07-21 12:51:21.866126 crypto-screening-7.4.3/crypto_screening/source/data/
+-rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-7.4.3/crypto_screening/source/data/all_exchanges_symbols.json
+-rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-7.4.3/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3599 2023-07-18 22:07:23.000000 crypto-screening-7.4.3/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:51:21.842141 crypto-screening-7.4.3/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-21 12:51:21.000000 crypto-screening-7.4.3/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2070 2023-07-21 12:51:21.000000 crypto-screening-7.4.3/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 12:51:21.000000 crypto-screening-7.4.3/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-21 12:51:21.000000 crypto-screening-7.4.3/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-21 12:51:21.000000 crypto-screening-7.4.3/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-21 12:47:44.000000 crypto-screening-7.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-7.4.3/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-7.4.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 12:51:21.867126 crypto-screening-7.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2023-07-21 12:51:17.000000 crypto-screening-7.4.3/setup.py
```

### Comparing `crypto-screening-7.4.2/PKG-INFO` & `crypto-screening-7.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 7.4.2
+Version: 7.4.3
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-7.4.2/README.md` & `crypto-screening-7.4.3/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/build.py` & `crypto-screening-7.4.3/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/collect/assets.py` & `crypto-screening-7.4.3/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/collect/exchanges.py` & `crypto-screening-7.4.3/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-7.4.3/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/collect/market/orderbook.py` & `crypto-screening-7.4.3/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/collect/market/orders.py` & `crypto-screening-7.4.3/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/collect/market/state/assets.py` & `crypto-screening-7.4.3/crypto_screening/collect/market/state/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/collect/market/state/base.py` & `crypto-screening-7.4.3/crypto_screening/collect/market/state/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-7.4.3/crypto_screening/collect/market/state/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/collect/market/trades.py` & `crypto-screening-7.4.3/crypto_screening/collect/market/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/collect/screeners.py` & `crypto-screening-7.4.3/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/collect/symbols.py` & `crypto-screening-7.4.3/crypto_screening/collect/symbols.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # symbols.py
 
+import warnings
 from typing import (
     Optional, Dict, Iterable,
     Set, Union, Tuple
 )
 
 from attrs import define
 
 from represent import represent
 
+from multithreading import Caller, multi_threaded_call
+
 from crypto_screening.process import (
     find_string_value, upper_string_values,
     mutual_string_values
 )
 from crypto_screening.exchanges import EXCHANGES, EXCHANGE_NAMES
 from crypto_screening.symbols import (
     symbol_to_parts, adjust_symbol, Separator
@@ -283,17 +286,26 @@
 
     validate_exchange(exchange=exchange, exchanges=EXCHANGE_NAMES)
 
     try:
         found_symbols: Iterable[str] = EXCHANGES[exchange].symbols()
 
     except Exception as e:
-        raise RuntimeError(
+        error_message = (
             f"Cannot fetch symbols of '{exchange}' exchange: {str(e)}."
         )
+
+        if not adjust:
+            raise RuntimeError(error_message)
+
+        else:
+            warnings.warn(error_message)
+
+            return set()
+        # end if
     # end try
 
     symbols = []
 
     if separator is None:
         separator = Separator.value
     # end if
@@ -343,19 +355,28 @@
     :param adjust: The value to adjust the invalid exchanges.
     :param separator: The separator of the assets.
     :param test: Include test assets.
 
     :return: The data of the exchanges.
     """
 
+    results = multi_threaded_call(
+        [
+            Caller(
+                target=all_exchange_symbols, kwargs=dict(
+                    exchange=exchange, separator=separator,
+                    adjust=adjust, test=test
+                ), identifier=exchange
+            ) for exchange in exchanges
+        ]
+    )
+
     return {
-        exchange: all_exchange_symbols(
-            exchange=exchange, separator=separator,
-            adjust=adjust, test=test
-        ) for exchange in exchanges
+        exchange: results.results(exchange).returns
+        for exchange in exchanges
     }
 # end all_exchanges_symbols
 
 def exchange_symbols(
         exchange: Optional[str] = None,
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
```

### Comparing `crypto-screening-7.4.2/crypto_screening/dataset.py` & `crypto-screening-7.4.3/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/interval.py` & `crypto-screening-7.4.3/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/market/dynamic.py` & `crypto-screening-7.4.3/crypto_screening/market/dynamic.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,42 +19,35 @@
     SymbolsOrdersMarketState, AssetsOrdersMarketState
 )
 from crypto_screening.collect.market.trades import (
     assets_trades_market_state, symbols_trades_market_state,
     SymbolsTradesMarketState, AssetsTradesMarketState
 )
 from crypto_screening.market.screeners.container import (
-    DynamicScreenersContainer, FixedScreenersContainer, ScreenersContainer
+    DynamicScreenersContainer, MappedScreenersContainer, ScreenersContainer
 )
 
 __all__ = [
-    "ScreenersData",
-    "DynamicScreenersData",
-    "FixedScreenersData"
+    "ScreenersMarket",
+    "DynamicScreenersMarket",
+    "MappedScreenersMarket"
 ]
 
-class ScreenersData(ScreenersContainer, metaclass=ABCMeta):
+ExchangesData = Union[Dict[str, Iterable[str]], Iterable[str]]
+
+class ScreenersMarket(ScreenersContainer, metaclass=ABCMeta):
     """
     A class to represent a multi-exchange multi-pairs crypto data screener.
     Using this class enables extracting screener objects and screeners
     data by the exchange name and the symbol of the pair.
 
     parameters:
 
     - screeners:
-        The screener objects.
-
-    >>> from crypto_screening.market.dynamic import ScreenersData
-    >>> from crypto_screening.market.screeners.base import BaseScreener
-    >>>
-    >>> data = ScreenersData(
-    >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
-    >>> )
-    >>>
-    >>> data.find_screener(exchange="binance", symbol="BTC/USDT"))
+        The screener objects to form a market.
     """
 
     def find_ohlcv_dataset(
             self,
             exchange: str,
             symbol: str,
             interval: Optional[str] = None,
@@ -206,18 +199,18 @@
 
     def assets_orderbook_market_state(
             self,
             exchanges: Optional[Iterable[str]] = None,
             separator: Optional[str] = None,
             length: Optional[int] = None,
             adjust: Optional[bool] = True,
-            bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
+            bases: Optional[ExchangesData] = None,
+            quotes: Optional[ExchangesData] = None,
+            included: Optional[ExchangesData] = None,
+            excluded: Optional[ExchangesData] = None
     ) -> AssetsOrderbookMarketState:
         """
         Fetches the values and relations between the assets.
 
         :param length: The length of the values.
         :param adjust: The value to adjust the length of the sequences.
         :param exchanges: The exchanges.
@@ -249,18 +242,18 @@
 
     def symbols_orderbook_market_state(
             self,
             exchanges: Optional[Iterable[str]] = None,
             separator: Optional[str] = None,
             length: Optional[int] = None,
             adjust: Optional[bool] = True,
-            bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
+            bases: Optional[ExchangesData] = None,
+            quotes: Optional[ExchangesData] = None,
+            included: Optional[ExchangesData] = None,
+            excluded: Optional[ExchangesData] = None
     ) -> SymbolsOrderbookMarketState:
         """
         Fetches the values and relations between the assets.
 
         :param length: The length of the values.
         :param adjust: The value to adjust the length of the sequences.
         :param exchanges: The exchanges.
@@ -291,18 +284,18 @@
 
     def assets_ohlcv_market_state(
             self,
             exchanges: Optional[Iterable[str]] = None,
             separator: Optional[str] = None,
             length: Optional[int] = None,
             adjust: Optional[bool] = True,
-            bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
+            bases: Optional[ExchangesData] = None,
+            quotes: Optional[ExchangesData] = None,
+            included: Optional[ExchangesData] = None,
+            excluded: Optional[ExchangesData] = None
     ) -> AssetsOHLCVMarketState:
         """
         Fetches the values and relations between the assets.
 
         :param length: The length of the values.
         :param adjust: The value to adjust the length of the sequences.
         :param exchanges: The exchanges.
@@ -330,18 +323,18 @@
 
     def symbols_ohlcv_market_state(
             self,
             exchanges: Optional[Iterable[str]] = None,
             separator: Optional[str] = None,
             length: Optional[int] = None,
             adjust: Optional[bool] = True,
-            bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
+            bases: Optional[ExchangesData] = None,
+            quotes: Optional[ExchangesData] = None,
+            included: Optional[ExchangesData] = None,
+            excluded: Optional[ExchangesData] = None
     ) -> SymbolsOHLCVMarketState:
         """
         Fetches the values and relations between the assets.
 
         :param length: The length of the values.
         :param adjust: The value to adjust the length of the sequences.
         :param exchanges: The exchanges.
@@ -368,18 +361,18 @@
 
     def assets_trades_market_state(
             self,
             exchanges: Optional[Iterable[str]] = None,
             separator: Optional[str] = None,
             length: Optional[int] = None,
             adjust: Optional[bool] = True,
-            bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
+            bases: Optional[ExchangesData] = None,
+            quotes: Optional[ExchangesData] = None,
+            included: Optional[ExchangesData] = None,
+            excluded: Optional[ExchangesData] = None
     ) -> AssetsTradesMarketState:
         """
         Fetches the values and relations between the assets.
 
         :param length: The length of the values.
         :param adjust: The value to adjust the length of the sequences.
         :param exchanges: The exchanges.
@@ -407,18 +400,18 @@
 
     def symbols_trades_market_state(
             self,
             exchanges: Optional[Iterable[str]] = None,
             separator: Optional[str] = None,
             length: Optional[int] = None,
             adjust: Optional[bool] = True,
-            bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
+            bases: Optional[ExchangesData] = None,
+            quotes: Optional[ExchangesData] = None,
+            included: Optional[ExchangesData] = None,
+            excluded: Optional[ExchangesData] = None
     ) -> SymbolsTradesMarketState:
         """
         Fetches the values and relations between the assets.
 
         :param length: The length of the values.
         :param adjust: The value to adjust the length of the sequences.
         :param exchanges: The exchanges.
@@ -445,18 +438,18 @@
 
     def assets_orders_market_state(
             self,
             exchanges: Optional[Iterable[str]] = None,
             separator: Optional[str] = None,
             length: Optional[int] = None,
             adjust: Optional[bool] = True,
-            bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
+            bases: Optional[ExchangesData] = None,
+            quotes: Optional[ExchangesData] = None,
+            included: Optional[ExchangesData] = None,
+            excluded: Optional[ExchangesData] = None
     ) -> AssetsOrdersMarketState:
         """
         Fetches the values and relations between the assets.
 
         :param length: The length of the values.
         :param adjust: The value to adjust the length of the sequences.
         :param exchanges: The exchanges.
@@ -484,18 +477,18 @@
 
     def symbols_orders_market_state(
             self,
             exchanges: Optional[Iterable[str]] = None,
             separator: Optional[str] = None,
             length: Optional[int] = None,
             adjust: Optional[bool] = True,
-            bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-            excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
+            bases: Optional[ExchangesData] = None,
+            quotes: Optional[ExchangesData] = None,
+            included: Optional[ExchangesData] = None,
+            excluded: Optional[ExchangesData] = None
     ) -> SymbolsOrdersMarketState:
         """
         Fetches the values and relations between the assets.
 
         :param length: The length of the values.
         :param adjust: The value to adjust the length of the sequences.
         :param exchanges: The exchanges.
@@ -517,50 +510,50 @@
 
         return symbols_orders_market_state(
             screeners=screeners, length=length, adjust=adjust
         )
     # end symbols_orders_market_state
 # end DynamicScreenerContainer
 
-class FixedScreenersData(FixedScreenersContainer, ScreenersData):
+class MappedScreenersMarket(MappedScreenersContainer, ScreenersMarket):
     """
     A class to represent a multi-exchange multi-pairs crypto data screener.
     Using this class enables extracting screener objects and screeners
     data by the exchange name and the symbol of the pair.
 
     parameters:
 
     - screeners:
-        The screener objects.
+        The screener objects to form a market.
 
-    >>> from crypto_screening.market.dynamic import FixedScreenersData
+    >>> from crypto_screening.market.dynamic import MappedScreenersMarket
     >>> from crypto_screening.market.screeners.base import BaseScreener
     >>>
-    >>> fixed_data = FixedScreenersData(
+    >>> market = MappedScreenersMarket(
     >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
     >>> )
     >>>
-    >>> fixed_data.find_screener(exchange="binance", symbol="BTC/USDT"))
+    >>> market.find_screener(exchange="binance", symbol="BTC/USDT"))
     """
-# end FixedScreenersData
+# end MappedScreenersMarket
 
-class DynamicScreenersData(DynamicScreenersContainer, ScreenersData):
+class DynamicScreenersMarket(DynamicScreenersContainer, ScreenersMarket):
     """
     A class to represent a multi-exchange multi-pairs crypto data screener.
     Using this class enables extracting screener objects and screeners
     data by the exchange name and the symbol of the pair.
 
     parameters:
 
     - screeners:
-        The screener objects.
+        The screener objects to form a market.
 
-    >>> from crypto_screening.market.dynamic import DynamicScreenersData
+    >>> from crypto_screening.market.dynamic import DynamicScreenersMarket
     >>> from crypto_screening.market.screeners.base import BaseScreener
     >>>
-    >>> dynamic_data = DynamicScreenersData(
+    >>> market = DynamicScreenersMarket(
     >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
     >>> )
     >>>
-    >>> dynamic_data.find_screener(exchange="binance", symbol="BTC/USDT"))
+    >>> market.find_screener(exchange="binance", symbol="BTC/USDT"))
     """
-# end DynamicScreenersData
+# end DynamicScreenersMarket
```

### Comparing `crypto-screening-7.4.2/crypto_screening/market/foundation/data.py` & `crypto-screening-7.4.3/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/market/foundation/protocols.py` & `crypto-screening-7.4.3/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/market/foundation/state.py` & `crypto-screening-7.4.3/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/market/foundation/waiting.py` & `crypto-screening-7.4.3/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/market/screeners/__init__.py` & `crypto-screening-7.4.3/crypto_screening/market/screeners/__init__.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/market/screeners/base.py` & `crypto-screening-7.4.3/crypto_screening/market/screeners/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 import pandas as pd
 
 from represent import Modifiers
 
 from multithreading import Caller, multi_threaded_call
 
-from crypto_screening.dataset import save_dataset, load_dataset
-from crypto_screening.symbols import Separator, adjust_symbol
+from crypto_screening.dataset import save_dataset, load_dataset, create_dataset
+from crypto_screening.symbols import adjust_symbol
 from crypto_screening.validate import validate_exchange, validate_symbol
 from crypto_screening.collect.symbols import all_exchange_symbols
 from crypto_screening.market.foundation.state import WaitingState
 from crypto_screening.market.foundation.data import DataCollector
 from crypto_screening.market.foundation.protocols import BaseScreenerProtocol
 from crypto_screening.market.foundation.waiting import (
     base_await_initialization, base_await_dynamic_initialization,
@@ -60,14 +60,15 @@
 
     __modifiers__ = Modifiers(**DataCollector.__modifiers__)
     __modifiers__.hidden.append("market")
 
     MINIMUM_DELAY = 1
 
     NAME: Optional[str] = "BASE"
+    COLUMNS: Iterable[str] = []
 
     __slots__ = "symbol", "exchange", "market"
 
     SCREENER_NAME_TYPE_MATCHES: Dict[str, Any] = {}
     SCREENER_TYPE_NAME_MATCHES: Dict[Any, str] = {}
 
     def __init__(
@@ -86,22 +87,33 @@
         :param exchange: The exchange to get source data from.
         :param location: The saving location for the data.
         :param delay: The delay for the process.
         :param cancel: The cancel time for the loops.
         :param market: The data for the market.
         """
 
+        if not self.COLUMNS:
+            raise ValueError(
+                f"{repr(self)} must define a non-empty "
+                f"'COLUMNS' instance or class attribute."
+            )
+        # end if
+
         super().__init__(location=location, cancel=cancel, delay=delay)
 
         self.SCREENER_NAME_TYPE_MATCHES.setdefault(self.NAME, type(self))
         self.SCREENER_TYPE_NAME_MATCHES.setdefault(type(self), self.NAME)
 
         self.exchange = self.validate_exchange(exchange=exchange)
         self.symbol = self.validate_symbol(exchange=self.exchange, symbol=symbol)
 
+        if market is None:
+            market = create_dataset(self.COLUMNS)
+        # end if
+
         self.market = market
     # end __init__
 
     def await_initialization(
             self,
             stop: Optional[Union[bool, int]] = False,
             delay: Optional[Union[float, dt.timedelta]] = None,
@@ -191,15 +203,16 @@
         if location is None:
             location = "."
         # end if
 
         return (
             f"{location}/"
             f"{self.exchange.lower()}/"
-            f"{adjust_symbol(self.symbol).replace(Separator.value, '-')}.csv"
+            f"{self.NAME}-"
+            f"{adjust_symbol(self.symbol, separator='-')}.csv"
         )
     # end dataset_path
 
     def save_dataset(self, location: Optional[str] = None) -> None:
         """
         Saves the data of the screener.
```

### Comparing `crypto-screening-7.4.2/crypto_screening/market/screeners/callbacks.py` & `crypto-screening-7.4.3/crypto_screening/market/screeners/callbacks.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/market/screeners/collectors/base.py` & `crypto-screening-7.4.3/crypto_screening/market/screeners/collectors/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 import warnings
 import threading
 import datetime as dt
 from typing import List, Tuple, Optional, Iterable, Union, Dict
 
 from crypto_screening.market.screeners.base import BaseScreener, BaseMarketScreener
-from crypto_screening.market.screeners.container import FixedScreenersContainer
+from crypto_screening.market.screeners.container import MappedScreenersContainer
 from crypto_screening.collect.market.state.base import index_to_datetime
 
 __all__ = [
     "ScreenersDataCollector"
 ]
 
 Data = List[Tuple[Union[str, float, dt.datetime], Dict[str, Optional[Union[str, float, bool]]]]]
 
-class ScreenersDataCollector(FixedScreenersContainer, BaseMarketScreener):
+class ScreenersDataCollector(MappedScreenersContainer, BaseMarketScreener):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
@@ -57,15 +57,15 @@
         """
 
         BaseMarketScreener.__init__(
             self, screeners=screeners, location=location,
             cancel=cancel, delay=delay
         )
 
-        FixedScreenersContainer.__init__(self, screeners=screeners)
+        MappedScreenersContainer.__init__(self, screeners=screeners)
     # end __init__
 
     def handle(
             self,
             name: str,
             exchange: str,
             symbol: str,
```

### Comparing `crypto-screening-7.4.2/crypto_screening/market/screeners/collectors/database.py` & `crypto-screening-7.4.3/crypto_screening/market/screeners/collectors/database.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # data.py
 
 import datetime as dt
 from typing import Optional, Union, Iterable, Dict, Tuple, List
 
-from sqlalchemy import Engine, inspect
+from sqlalchemy import Engine
 
 from crypto_screening.market.screeners.callbacks import DatabaseCallback
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.database import (
-    database_table_name_to_parts, extract_database_table_record, create_engine
+    extract_database_table_parts, extract_database_table_record,
+    create_engine, extract_database_tables
 )
 from crypto_screening.market.screeners.collectors.base import ScreenersDataCollector
 
 __all__ = [
     "DatabaseScreenersDataCollector",
     "DatabaseCallback"
 ]
@@ -82,35 +83,33 @@
 
         if isinstance(self.engine, Engine):
             self._connected = True
         # end if
 
         self._session: Optional = None
 
-        self.tables: Dict[str, Tuple[str, str, str, Optional[str]]] = {
-            table: database_table_name_to_parts(table)
-            for table in tables or inspect(self.engine).get_table_names()
-        }
+        self.tables = (
+            extract_database_table_parts(tables) or
+            extract_database_tables(self.engine)
+        )
 
         self.failed_tables: Dict[str, List[Exception]] = {}
     # end __init__
 
     def screening_loop(self) -> None:
         """Runs the process of the price screening."""
 
         self._screening = True
 
-        database = {self.database: self.engine}
-
         while self.screening:
             for table, (name, exchange, symbol, interval) in self.tables.items():
                 try:
                     dataset = extract_database_table_record(
-                        table=table, databases=database, length=1
-                    )[self.database]
+                        table=table, engine=self.engine, length=1
+                    )
 
                     # noinspection PyTypeChecker
                     data: Data = list(
                         (index, row.to_dict())
                         for index, row in dataset.iterrows()
                     )
```

### Comparing `crypto-screening-7.4.2/crypto_screening/market/screeners/collectors/sockets.py` & `crypto-screening-7.4.3/crypto_screening/market/screeners/collectors/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/market/screeners/combined.py` & `crypto-screening-7.4.3/crypto_screening/market/screeners/combined.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/market/screeners/container.py` & `crypto-screening-7.4.3/crypto_screening/market/screeners/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,18 @@
 from represent import represent, Modifiers
 
 from crypto_screening.market.screeners.ohlcv import OHLCVScreener
 from crypto_screening.market.screeners.orderbook import OrderbookScreener
 from crypto_screening.market.screeners.trades import TradesScreener
 from crypto_screening.market.screeners.orders import OrdersScreener
 from crypto_screening.market.screeners.base import BaseScreener
-from crypto_screening.market.screeners.recorder import structure_screener_datasets
 
 __all__ = [
     "DynamicScreenersContainer",
-    "FixedScreenersContainer",
+    "MappedScreenersContainer",
     "screeners_table",
     "ScreenersContainer"
 ]
 
 _S = TypeVar(
     "_S",
     BaseScreener,
@@ -34,36 +33,27 @@
     A class to represent a multi-exchange multi-pairs crypto data screener.
     Using this class enables extracting screener objects and screeners
     data by the exchange name and the symbol of the pair.
 
     parameters:
 
     - screeners:
-        The screener objects.
-
-    >>> from crypto_screening.market.screeners.container import ScreenersContainer
-    >>> from crypto_screening.market.screeners.base import BaseScreener
-    >>>
-    >>> container = ScreenersContainer(
-    >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
-    >>> )
+        The screener objects to form a market.
     """
 
     __modifiers__ = Modifiers(hidden=["screeners"])
 
     def __init__(self, screeners: Iterable[BaseScreener]) -> None:
         """
         Defines the class attributes.
 
         :param screeners: The data screener object.
         """
 
         self.screeners = list(screeners)
-
-        self.market = structure_screener_datasets(self.screeners)
     # end __init__
 
     @property
     def orderbook_screeners(self) -> List[OrderbookScreener]:
         """
         Returns a list of all the order-book screeners.
 
@@ -102,25 +92,21 @@
 
         :return: The trades screeners.
         """
 
         return self.find_screeners(base=TradesScreener)
     # end trades_screeners
 
+    @abstractmethod
     def structure(self) -> Dict[str, List[str]]:
         """
         Returns the structure of the market data.
 
         :return: The structure of the market.
         """
-
-        return {
-            exchange: list(symbols.keys())
-            for exchange, symbols in self.market.items()
-        }
     # end structure
 
     @abstractmethod
     def find_screeners(
             self,
             exchange: Optional[str] = None,
             symbol: Optional[str] = None,
@@ -456,34 +442,53 @@
 
         return self.find_screeners(
             exchange=exchange, symbol=symbol, base=TradesScreener
         )
     # end find_trades_screeners
 # end ScreenersContainer
 
-@represent
 class DynamicScreenersContainer(ScreenersContainer):
     """
     A class to represent a multi-exchange multi-pairs crypto data screener.
     Using this class enables extracting screener objects and screeners
     data by the exchange name and the symbol of the pair.
 
     parameters:
 
     - screeners:
-        The screener objects.
+        The screener objects to form a market.
 
     >>> from crypto_screening.market.screeners.container import DynamicScreenersContainer
     >>> from crypto_screening.market.screeners.base import BaseScreener
     >>>
     >>> container = DynamicScreenersContainer(
     >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
     >>> )
     """
 
+    def structure(self) -> Dict[str, List[str]]:
+        """
+        Returns the structure of the market data.
+
+        :return: The structure of the market.
+        """
+
+        structure: Dict[str, List[str]] = {}
+
+        for screener in self.screeners:
+            (
+                structure.
+                setdefault(screener.exchange, []).
+                append(screener.symbol)
+            )
+        # end for
+
+        return structure
+    # end structure
+
     def find_screeners(
             self,
             exchange: Optional[str] = None,
             symbol: Optional[str] = None,
             base: Optional[Type[_S]] = None,
             interval: Optional[str] = None
     ) -> List[_S]:
@@ -500,20 +505,21 @@
 
         screeners = []
 
         for screener in self.screeners:
             if (
                 ((screener.exchange == exchange) or (exchange is None)) and
                 ((screener.symbol == symbol) or (symbol is None)) and
-                isinstance(screener, base or BaseScreener) and
+                ((base is None) or isinstance(screener, base)) and
                 (
-                    (screener.interval == interval) if (
+                    (interval is None) or
+                    (
                         isinstance(screener, OHLCVScreener) and
-                        (interval is not None)
-                    ) else True
+                        (screener.interval == interval)
+                    )
                 )
             ):
                 screeners.append(screener)
             # end if
         # end for
 
         return screeners
@@ -542,111 +548,113 @@
     """
 
     if table is None:
         table = {}
     # end if
 
     for screener in screeners:
-        interval = (
-            screener.interval
-            if isinstance(screener, OHLCVScreener) else
-            None
-        )
-
-        lists = [
-            (
-                table.
-                setdefault(type(screener), {}).
-                setdefault(screener.exchange, {}).
-                setdefault(screener.symbol, {}).
-                setdefault(interval, [])
-            ),
-            (
-                table.
-                setdefault(type(screener), {}).
-                setdefault(screener.exchange, {}).
-                setdefault(None, {}).
-                setdefault(interval, [])
-            ),
+        for interval in {
             (
-                table.
-                setdefault(type(screener), {}).
-                setdefault(None, {}).
-                setdefault(screener.symbol, {}).
-                setdefault(interval, [])
-            ),
-            (
-                table.
-                setdefault(type(screener), {}).
-                setdefault(None, {}).
-                setdefault(None, {}).
-                setdefault(interval, [])
-            ),
-            (
-                table.
-                setdefault(type(screener), {}).
-                setdefault(None, {}).
-                setdefault(None, {}).
-                setdefault(None, [])
-            ),
-            (
-                table.
-                setdefault(None, {}).
-                setdefault(screener.exchange, {}).
-                setdefault(screener.symbol, {}).
-                setdefault(interval, [])
-            ),
-            (
-                table.
-                setdefault(None, {}).
-                setdefault(screener.exchange, {}).
-                setdefault(None, {}).
-                setdefault(interval, [])
-            ),
-            (
-                table.
-                setdefault(None, {}).
-                setdefault(None, {}).
-                setdefault(screener.symbol, {}).
-                setdefault(interval, [])
-            ),
-            (
-                table.
-                setdefault(None, {}).
-                setdefault(None, {}).
-                setdefault(None, {}).
-                setdefault(interval, [])
-            )
-        ]
+                screener.interval
+                if isinstance(screener, OHLCVScreener) else
+                None
+            ), None
+        }:
+            lists = [
+                (
+                    table.
+                    setdefault(type(screener), {}).
+                    setdefault(screener.exchange, {}).
+                    setdefault(screener.symbol, {}).
+                    setdefault(interval, [])
+                ),
+                (
+                    table.
+                    setdefault(type(screener), {}).
+                    setdefault(screener.exchange, {}).
+                    setdefault(None, {}).
+                    setdefault(interval, [])
+                ),
+                (
+                    table.
+                    setdefault(type(screener), {}).
+                    setdefault(None, {}).
+                    setdefault(screener.symbol, {}).
+                    setdefault(interval, [])
+                ),
+                (
+                    table.
+                    setdefault(type(screener), {}).
+                    setdefault(None, {}).
+                    setdefault(None, {}).
+                    setdefault(interval, [])
+                ),
+                (
+                    table.
+                    setdefault(type(screener), {}).
+                    setdefault(None, {}).
+                    setdefault(None, {}).
+                    setdefault(None, [])
+                ),
+                (
+                    table.
+                    setdefault(None, {}).
+                    setdefault(screener.exchange, {}).
+                    setdefault(screener.symbol, {}).
+                    setdefault(interval, [])
+                ),
+                (
+                    table.
+                    setdefault(None, {}).
+                    setdefault(screener.exchange, {}).
+                    setdefault(None, {}).
+                    setdefault(interval, [])
+                ),
+                (
+                    table.
+                    setdefault(None, {}).
+                    setdefault(None, {}).
+                    setdefault(screener.symbol, {}).
+                    setdefault(interval, [])
+                ),
+                (
+                    table.
+                    setdefault(None, {}).
+                    setdefault(None, {}).
+                    setdefault(None, {}).
+                    setdefault(interval, [])
+                )
+            ]
 
-        for screeners_list in lists:
-            if screener not in screeners_list:
-                screeners_list.append(screener)
-            # end if
+            for screeners_list in lists:
+                if screener not in screeners_list:
+                    screeners_list.append(screener)
+                # end if
+            # end for
         # end for
     # end for
 
     return table
 # end screeners_table
 
-class FixedScreenersContainer(ScreenersContainer):
+class MappedScreenersContainer(ScreenersContainer):
     """
     A class to represent a multi-exchange multi-pairs crypto data screener.
     Using this class enables extracting screener objects and screeners
     data by the exchange name and the symbol of the pair.
 
     parameters:
 
     - screeners:
-        The screener objects.
+        The screener objects to form a market.
 
-    >>> from crypto_screening.market.screeners.container import FixedScreenersContainer
+    >>> from crypto_screening.market.screeners.container import MappedScreenersContainer
     >>> from crypto_screening.market.screeners.base import BaseScreener
     >>>
-    >>> container = FixedScreenersContainer(
+    >>> container = MappedScreenersContainer(
     >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
     >>> )
     """
 
     def __init__(self, screeners: Iterable[BaseScreener]) -> None:
         """
         Defines the class attributes.
@@ -655,14 +663,28 @@
         """
 
         super().__init__(screeners=screeners)
 
         self._table = screeners_table(self.screeners)
     # end __init__
 
+    def structure(self) -> Dict[str, List[str]]:
+        """
+        Returns the structure of the market data.
+
+        :return: The structure of the market.
+        """
+
+        return {
+            exchange: list([symbol for symbol in symbols if symbol is not None])
+            for exchange, symbols in self._table[None].items()
+            if exchange is not None
+        }
+    # end structure
+
     def update(self, screeners: Iterable[BaseScreener]) -> None:
         """
         Updates the data with the new screeners.
 
         :param screeners: The new screeners to add.
         """
 
@@ -702,8 +724,8 @@
                 f"Cannot find screeners  matching to "
                 f"type - {base}, exchange - {exchange}, "
                 f"symbol - {symbol}, interval - {interval} "
                 f"inside {repr(self)}"
             )
         # end try
     # end find_screeners
-# end FixedScreenersContainer
+# end MappedScreenersContainer
```

### Comparing `crypto-screening-7.4.2/crypto_screening/market/screeners/database.py` & `crypto-screening-7.4.3/crypto_screening/market/screeners/database.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,15 +27,17 @@
     "database_file_path",
     "await_database_creation",
     "await_all_databases_creation",
     "extract_data_into_screener_dataset",
     "extract_database_length",
     "extract_database_table_record",
     "create_engine",
-    "screeners_tables_names"
+    "screeners_tables_names",
+    "extract_database_table_names",
+    "extract_database_table_parts"
 ]
 
 def parts_to_database_table_name(
         name: str, exchange: str, symbol: str, interval: Optional[str] = None
 ) -> str:
     """
     Creates the database table name.
@@ -125,93 +127,87 @@
 # end await_all_databases_creation
 
 def insert_database_record(
         name: str,
         exchange: str,
         symbol: str,
         dataset: pd.DataFrame,
-        databases: Dict[str, Engine],
+        engine: Engine,
         interval: Optional[str] = None
 ) -> None:
     """
     Inserts the data into the databases.
 
     :param name: The name for the data.
     :param exchange: The exchange name of the data.
     :param symbol: The symbol of the data.
     :param dataset: The dataframe of the symbol.
-    :param databases: The database engines.
+    :param engine: The engine for the database.
     :param interval: The interval.
     """
 
     table = parts_to_database_table_name(
         name=name, exchange=exchange, symbol=symbol, interval=interval
     )
 
-    for path, engine in databases.items():
-        location = os.path.split(database_file_path(path))[0]
+    location = os.path.split(database_file_path(str(engine.url)))[0]
 
-        if location:
-            os.makedirs(location, exist_ok=True)
-        # end if
+    if location:
+        os.makedirs(location, exist_ok=True)
+    # end if
 
-        dataset.to_sql(table, engine, if_exists='append', index=True)
-    # end for
+    dataset.to_sql(table, engine, if_exists='append', index=True)
 # end insert_database_record
 
 def extract_database_length(
         name: str,
         exchange: str,
         symbol: str,
-        databases: Dict[str, Engine],
+        engine: Engine,
         interval: Optional[str] = None
-) -> Dict[str, int]:
+) -> int:
     """
     Extracts the length of the data from the databases.
 
     :param name: The name for the data.
     :param exchange: The exchange name of the data.
     :param symbol: The symbol of the data.
-    :param databases: The database engines.
+    :param engine: The engine for the database.
     :param interval: The interval.
 
     :return: The returned database lengths.
     """
 
     table = parts_to_database_table_name(
         name=name, exchange=exchange,
         symbol=symbol, interval=interval
     )
 
     query = 'SELECT COUNT(' + DATE_TIME + ') FROM ' + table
 
-    results: Dict[str, int] = {}
-
-    for path, engine in databases.items():
-        connection = engine.connect()
+    connection = engine.connect()
 
-        results[path] = connection.execute(text(query)).all()[0][0]
+    size = connection.execute(text(query)).all()[0][0]
 
-        connection.close()
-    # end for
+    connection.close()
 
-    return results
+    return size
 # end extract_database_length
 
 def extract_database_table_record(
         table: str,
-        databases: Dict[str, Engine],
+        engine: Engine,
         length: Optional[int] = None,
         start: Optional[dt.datetime] = None
-) -> Dict[str, pd.DataFrame]:
+) -> pd.DataFrame:
     """
     Extracts the data from the databases.
 
     :param table: The table name.
-    :param databases: The database engines.
+    :param engine: The engine for the database.
     :param length: Yne length of the dataset to extract.
     :param start: The starting row.
 
     :return: The returned databases.
     """
 
     query = 'SELECT * FROM ' + table
@@ -229,122 +225,133 @@
             f'(SELECT {length_query} FROM  ' + table + ')'
         )
 
     elif isinstance(start, int) and (start > 0):
         query += f' WHERE DateTime > {start}'
     # end if
 
-    results: Dict[str, pd.DataFrame] = {}
+    dataset: pd.DataFrame = pd.read_sql(query, engine)
 
-    for path, engine in databases.items():
-        dataset: pd.DataFrame = pd.read_sql(query, engine)
+    dataset.index = pd.DatetimeIndex(dataset[DATE_TIME])
+    del dataset[DATE_TIME]
+    dataset.index.name = DATE_TIME
 
-        dataset.index = pd.DatetimeIndex(dataset[DATE_TIME])
-        del dataset[DATE_TIME]
-        dataset.index.name = DATE_TIME
-
-        results[path] = dataset
+    return dataset
     # end for
-
-    return results
 # end extract_database_record
 
 def extract_database_record(
         name: str,
         exchange: str,
         symbol: str,
-        databases: Dict[str, Engine],
+        engine: Engine,
         interval: Optional[str] = None,
         length: Optional[int] = None,
         start: Optional[dt.datetime] = None
-) -> Dict[str, pd.DataFrame]:
+) -> pd.DataFrame:
     """
     Extracts the data from the databases.
 
     :param name: The name for the data.
     :param exchange: The exchange name of the data.
     :param symbol: The symbol of the data.
-    :param databases: The database engines.
+    :param engine: The engine for the database.
     :param length: Yne length of the dataset to extract.
     :param interval: The interval.
     :param start: The starting row.
 
     :return: The returned databases.
     """
 
     table = parts_to_database_table_name(
         name=name, exchange=exchange,
         symbol=symbol, interval=interval
     )
 
     return extract_database_table_record(
-        table=table, databases=databases, length=length, start=start
+        table=table, engine=engine, length=length, start=start
     )
 # end extract_database_record
 
 def extract_data_into_screener_dataset(
         screener: BaseScreener,
-        path: str,
         engine: Engine,
         length: Optional[int] = None,
         start: Optional[dt.datetime] = None
 ) -> None:
     """
     Extracts the data and inserts it into the screener dataset.
 
     :param screener: The screener object.
-    :param path: The path to the database.
     :param engine: The database engine.
     :param length: The length of data to extract.
     :param start: The start index.
     """
 
     interval = (
         screener.interval if (screener.NAME == "OHLCV") else None
     )
 
     data = extract_database_record(
         name=screener.NAME, exchange=screener.exchange,
         symbol=screener.symbol, interval=interval, start=start,
-        length=length, databases={path: engine}
-    )[path]
+        length=length, engine=engine
+    )
 
     for index, row in data.iterrows():
         row = row.to_dict()
 
         screener.market.loc[row.pop(DATE_TIME)] = row
     # end for
 # end extract_data_into_screener_dataset
 
-def extract_database_tables(
-        databases: Dict[str, Engine]
-) -> Dict[str, List[Tuple[str, str, str, Optional[str]]]]:
+TablesNameParts = Dict[str, List[Tuple[str, str, str, Optional[str]]]]
+
+def extract_database_table_names(engine: Engine) -> List[str]:
     """
     Extracts the databases table name.
 
-    :param databases: The database engines.
+    :param engine: The database engines.
 
     :return: The returned databases table name.
     """
 
-    await_all_databases_creation(databases.keys())
+    await_database_creation(str(engine.url))
 
-    tables: Dict[str, List[Tuple[str, str, str, Optional[str]]]] = {}
+    return list(inspect(engine).get_table_names())
+# end extract_database_table_names
 
-    for path, engine in databases.items():
-        database_tables = inspect(engine).get_table_names()
+def extract_database_table_parts(tables: Iterable[str]) -> TablesNameParts:
+    """
+    Extracts the databases table name.
 
-        tables[path] = [
-            database_table_name_to_parts(table)
-            for table in database_tables
-        ]
-    # end for
+    :param tables: The database tables.
+
+    :return: The returned databases table name.
+    """
+
+    return {
+        table: database_table_name_to_parts(table)
+        for table in tables
+    }
+# end extract_database_table_parts
+
+def extract_database_tables(engine: Engine) -> TablesNameParts:
+    """
+    Extracts the databases table name.
+
+    :param engine: The database engines.
+
+    :return: The returned databases table name.
+    """
+
+    await_database_creation(str(engine.url))
 
-    return tables
-# end extract_database_tables
+    return extract_database_table_parts(extract_database_table_names(engine))
+# end extract_database_table_parts
 
 Databases = Union[Iterable[str], Dict[str, Engine]]
 
 def create_engine(database: str) -> Engine:
     """
     Creates the engine for the database.
```

### Comparing `crypto-screening-7.4.2/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-7.4.3/crypto_screening/market/screeners/ohlcv.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,16 @@
     - base_market:
         The dataset of the market data as BID/ASK spread.
     """
 
     INTERVAL = "1m"
     NAME = "OHLCV"
 
+    COLUMNS = OHLCV_COLUMNS
+
     def __init__(
             self,
             symbol: str,
             exchange: str,
             interval: Optional[str] = None,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
@@ -191,15 +193,15 @@
         :param location: The saving location of the dataset.
 
         :return: The saving path for the dataset.
         """
 
         return (
             self.dataset_path(location=location).
-            replace(".csv", f"-{OrderbookScreener.NAME}.csv")
+            replace(self.NAME, OrderbookScreener.NAME)
         )
     # end orderbook_dataset_path
 
     def save_orderbook_dataset(self, location: Optional[str] = None) -> None:
         """
         Saves the data of the screener.
 
@@ -219,18 +221,15 @@
         Creates the path to the saving file for the screener object.
 
         :param location: The saving location of the dataset.
 
         :return: The saving path for the dataset.
         """
 
-        return (
-            self.dataset_path(location=location).
-            replace(".csv", f"-{self.NAME}-{self.interval}.csv")
-        )
+        return self.dataset_path(location=location)
     # end ohlcv_dataset_path
 
     def save_ohlcv_dataset(self, location: Optional[str] = None) -> None:
         """
         Saves the data of the screener.
 
         :param location: The saving location of the dataset.
@@ -251,24 +250,14 @@
         :param location: The saving location of the dataset.
         """
 
         self.save_ohlcv_dataset(location=location)
         self.save_orderbook_dataset(location=location)
     # end save_datasets
 
-    def save_dataset(self, location: Optional[str] = None) -> None:
-        """
-        Saves the data of the screener.
-
-        :param location: The saving location of the dataset.
-        """
-
-        self.save_datasets(location=location)
-    # end save_dataset
-
     def load_ohlcv_dataset(self, location: Optional[str] = None) -> None:
         """
         Saves the data of the screener.
 
         :param location: The saving location of the dataset.
         """
 
@@ -300,24 +289,14 @@
         :param location: The saving location of the dataset.
         """
 
         self.load_ohlcv_dataset(location=location)
         self.load_orderbook_dataset(location=location)
     # end load_datasets
 
-    def load_dataset(self, location: Optional[str] = None) -> None:
-        """
-        Saves the data of the screener.
-
-        :param location: The saving location of the dataset.
-        """
-
-        self.load_datasets(location=location)
-    # end load_dataset
-
     def orderbook_screener(self) -> OrderbookScreener:
         """
         Creates the orderbook screener object.
 
         :return: The orderbook screener.
         """
 
@@ -634,15 +613,15 @@
     """
 
     __modifiers__ = Modifiers(**MarketRecorder.__modifiers__)
     __modifiers__.hidden.extend(["intervals", "ohlcv_market"])
 
     __slots__ = "_indexes", "ohlcv_market", "intervals"
 
-    COLUMNS = OHLCV_COLUMNS
+    COLUMNS = OHLCVScreener.COLUMNS
     INTERVAL = OHLCVScreener.INTERVAL
 
     def __init__(
             self,
             intervals: Optional[Intervals] = None,
             market: Optional[Market] = None,
             ohlcv_market: Optional[OHLCVMarket] = None,
```

### Comparing `crypto-screening-7.4.2/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-7.4.3/crypto_screening/market/screeners/orderbook.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 from cryptofeed import FeedHandler
 from cryptofeed.types import OrderBook
 from cryptofeed.defines import L2_BOOK
 
 from crypto_screening.symbols import adjust_symbol
 from crypto_screening.process import find_string_value
 from crypto_screening.dataset import (
-    BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME, save_dataset,
-    create_dataset, ORDERBOOK_COLUMNS, load_dataset
+    BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME, create_dataset, ORDERBOOK_COLUMNS
 )
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.callbacks import Callback, callback_data
 from crypto_screening.market.screeners.recorder import MarketScreener, MarketRecorder
 
 __all__ = [
     "OrderbookMarketScreener",
@@ -92,88 +91,26 @@
 
     - market:
         The dataset of the market data as BID/ASK spread.
     """
 
     NAME = "ORDERBOOK"
 
+    COLUMNS = ORDERBOOK_COLUMNS
+
     @property
     def orderbook_market(self) -> pd.DataFrame:
         """
         Returns the market to hold the recorder data.
 
         :return: The market object.
         """
 
         return self.market
     # end orderbook_market
-
-    def orderbook_dataset_path(self, location: Optional[str] = None) -> str:
-        """
-        Creates the path to the saving file for the screener object.
-
-        :param location: The saving location of the dataset.
-
-        :return: The saving path for the dataset.
-        """
-
-        return (
-            self.dataset_path(location=location).
-            replace(".csv", f"-{self.NAME}.csv")
-        )
-    # end orderbook_dataset_path
-
-    def save_orderbook_dataset(self, location: Optional[str] = None) -> None:
-        """
-        Saves the data of the screener.
-
-        :param location: The saving location of the dataset.
-        """
-
-        if len(self.orderbook_market) > 0:
-            save_dataset(
-                dataset=self.orderbook_market,
-                path=self.orderbook_dataset_path(location=location)
-            )
-        # end if
-    # end save_orderbook_dataset
-
-    def save_dataset(self, location: Optional[str] = None) -> None:
-        """
-        Saves the data of the screener.
-
-        :param location: The saving location of the dataset.
-        """
-
-        self.save_orderbook_dataset(location=location)
-    # end save_dataset
-
-    def load_orderbook_dataset(self, location: Optional[str] = None) -> None:
-        """
-        Saves the data of the screener.
-
-        :param location: The saving location of the dataset.
-        """
-
-        data = load_dataset(path=self.orderbook_dataset_path(location=location))
-
-        for index, data in zip(data.index[:], data.loc[:]):
-            self.orderbook_market.loc[index] = data
-        # end for
-    # end load_orderbook_dataset
-
-    def load_dataset(self, location: Optional[str] = None) -> None:
-        """
-        Saves the data of the screener.
-
-        :param location: The saving location of the dataset.
-        """
-
-        self.load_orderbook_dataset(location=location)
-    # end load_dataset
 # end OrderbookScreener
 
 async def record_orderbook(
         market: Market,
         data: OrderBook,
         timestamp: float,
         callbacks: Optional[Iterable[Callback]] = None
@@ -259,15 +196,15 @@
     >>> from crypto_screening.market.screeners import orderbook_market_recorder
     >>>
     >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> recorder = orderbook_market_recorder(data=market)
     """
 
-    COLUMNS = ORDERBOOK_COLUMNS
+    COLUMNS = OrderbookScreener.COLUMNS
 
     @property
     def orderbook_market(self) -> Market:
         """
         Returns the market to hold the recorder data.
 
         :return: The market object.
```

### Comparing `crypto-screening-7.4.2/crypto_screening/market/screeners/orders.py` & `crypto-screening-7.4.3/crypto_screening/market/screeners/trades.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,74 @@
-# orders.py
+# trades.py
 
 import datetime as dt
 from typing import (
     Dict, Optional, Iterable, Any, Union, List, Callable
 )
 
 import pandas as pd
 
 from sqlalchemy import Engine
 
 from cryptofeed import FeedHandler
-from cryptofeed.types import Ticker
-from cryptofeed.defines import TICKER
+from cryptofeed.types import Trade
+from cryptofeed.defines import TRADES
 
 from crypto_screening.symbols import adjust_symbol
 from crypto_screening.process import find_string_value
 from crypto_screening.dataset import (
-    BIDS, ASKS, ORDERS_COLUMNS, create_dataset,
-    load_dataset, save_dataset
+    TRADES_COLUMNS, create_dataset, AMOUNT, PRICE, SIDE
 )
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.callbacks import Callback, callback_data
 from crypto_screening.market.screeners.recorder import MarketScreener, MarketRecorder
 
 __all__ = [
-    "OrdersMarketScreener",
-    "OrdersMarketRecorder",
-    "OrdersScreener",
-    "create_orders_market",
-    "orders_market_screener",
-    "orders_market_recorder",
-    "create_orders_market_dataset",
-    "record_orders"
+    "TradesMarketScreener",
+    "TradesMarketRecorder",
+    "TradesScreener",
+    "create_trades_market",
+    "trades_market_screener",
+    "trades_market_recorder",
+    "create_trades_market_dataset",
+    "record_trades"
 ]
 
 Market = Dict[str, Dict[str, pd.DataFrame]]
 
-def create_orders_market_dataset() -> pd.DataFrame:
+def create_trades_market_dataset() -> pd.DataFrame:
     """
     Creates a dataframe for the order book data.
 
     :return: The dataframe.
     """
 
     return create_dataset(
-        columns=OrdersMarketRecorder.COLUMNS
+        columns=TradesMarketRecorder.COLUMNS
     )
-# end create_orderbook_market_dataset
+# end create_trades_market_dataset
 
-def create_orders_market(data: Dict[str, Iterable[str]]) -> Market:
+def create_trades_market(data: Dict[str, Iterable[str]]) -> Market:
     """
     Creates the dataframes of the market data.
 
     :param data: The market data.
 
     :return: The dataframes of the market data.
     """
 
     return {
         exchange.lower(): {
-            symbol.upper(): create_orders_market_dataset()
+            symbol.upper(): create_trades_market_dataset()
             for symbol in data[exchange]
         } for exchange in data
     }
-# end create_orders_market
+# end create_trades_market
 
-class OrdersScreener(BaseScreener):
+class TradesScreener(BaseScreener):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
@@ -87,98 +86,36 @@
     - cancel:
         The time to cancel screening process after no new data is fetched.
 
     - delay:
         The delay to wait between each data fetching.
 
     - market:
-        The dataset of the market data as orders.
+        The dataset of the market data as trades.
     """
 
-    NAME = "ORDERS"
+    NAME = "TRADES"
+
+    COLUMNS = TRADES_COLUMNS
 
     @property
-    def orders_market(self) -> pd.DataFrame:
+    def trades_market(self) -> pd.DataFrame:
         """
         Returns the market to hold the recorder data.
 
         :return: The market object.
         """
 
         return self.market
-    # end orders_market
-
-    def orders_dataset_path(self, location: Optional[str] = None) -> str:
-        """
-        Creates the path to the saving file for the screener object.
-
-        :param location: The saving location of the dataset.
-
-        :return: The saving path for the dataset.
-        """
-
-        return (
-            self.dataset_path(location=location).
-            replace(".csv", f"-{self.NAME}.csv")
-        )
-    # end orders_dataset_path
-
-    def save_orders_dataset(self, location: Optional[str] = None) -> None:
-        """
-        Saves the data of the screener.
-
-        :param location: The saving location of the dataset.
-        """
-
-        if len(self.orders_market) > 0:
-            save_dataset(
-                dataset=self.orders_market,
-                path=self.orders_dataset_path(location=location)
-            )
-        # end if
-    # end save_orders_dataset
-
-    def save_dataset(self, location: Optional[str] = None) -> None:
-        """
-        Saves the data of the screener.
+    # end trades_market
+# end TradesScreener
 
-        :param location: The saving location of the dataset.
-        """
-
-        self.save_orders_dataset(location=location)
-    # end save_dataset
-
-    def load_orders_dataset(self, location: Optional[str] = None) -> None:
-        """
-        Saves the data of the screener.
-
-        :param location: The saving location of the dataset.
-        """
-
-        data = load_dataset(path=self.orders_dataset_path(location=location))
-
-        for index, data in zip(data.index[:], data.loc[:]):
-            self.orders_market.loc[index] = data
-        # end for
-    # end load_orders_dataset
-
-    def load_dataset(self, location: Optional[str] = None) -> None:
-        """
-        Saves the data of the screener.
-
-        :param location: The saving location of the dataset.
-        """
-
-        self.load_orders_dataset(location=location)
-    # end load_dataset
-# end OrdersScreener
-
-async def record_orders(
+async def record_trades(
         market: Market,
-        data: Ticker,
+        data: Trade,
         timestamp: float,
         callbacks: Optional[Iterable[Callback]] = None
 ) -> bool:
     """
     Records the data from the crypto feed into the dataset.
 
     :param market: The market structure.
@@ -196,49 +133,50 @@
         value=adjust_symbol(symbol=data.symbol),
         values=exchange
     )
 
     dataset = (
         market.
         setdefault(exchange, {}).
-        setdefault(symbol, create_orders_market_dataset())
+        setdefault(symbol, create_trades_market_dataset())
     )
 
     try:
         index = dt.datetime.fromtimestamp(timestamp)
 
         if index in dataset.index:
             return False
         # end if
 
         data = {
-            BIDS: float(data.bid),
-            ASKS: float(data.ask)
+            AMOUNT: float(data.amount),
+            PRICE: float(data.price),
+            SIDE: data.side
         }
 
         dataset.loc[index] = data
 
         for callback in callbacks or []:
             payload = callback_data(
                 data=[(timestamp, data)], exchange=exchange, symbol=symbol
             )
 
-            await callback.record(payload, timestamp, key=OrdersScreener.NAME)
+            await callback.record(payload, timestamp, key=TradesScreener.NAME)
         # end if
 
         return True
 
     except IndexError:
         return False
     # end try
-# end record_orders
+# end record_trades
 
 RecorderParameters = Dict[str, Union[Iterable[str], Dict[str, Callable]]]
 
-class OrdersMarketRecorder(MarketRecorder):
+class TradesMarketRecorder(MarketRecorder):
     """
     A class to represent a crypto data feed recorder.
     This object passes the record method to the handler object to record
     the data fetched by the handler.
 
     Parameters:
 
@@ -254,90 +192,92 @@
     >>> from crypto_screening.market.screeners import orderbook_market_recorder
     >>>
     >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> recorder = orderbook_market_recorder(data=market)
     """
 
-    COLUMNS = ORDERS_COLUMNS
+    COLUMNS = TradesScreener.COLUMNS
 
     @property
-    def orders_market(self) -> Market:
+    def trades_market(self) -> Market:
         """
         Returns the market to hold the recorder data.
 
         :return: The market object.
         """
 
         return self.market
-    # end orders_market
+    # end trades_market
 
     def parameters(self) -> RecorderParameters:
         """
         Returns the order book parameters.
 
         :return: The order book parameters.
         """
 
         return dict(
-            channels=[TICKER],
-            callbacks={TICKER: self.record},
+            channels=[TRADES],
+            callbacks={TRADES: self.record},
             max_depth=1
         )
     # end parameters
 
-    def orders(self, exchange: str, symbol: str) -> pd.DataFrame:
+    def trades(self, exchange: str, symbol: str) -> pd.DataFrame:
         """
         Returns the market data of the symbol from the exchange.
 
         :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
         return self.data(exchange=exchange, symbol=symbol)
-    # end orders
+    # end trades
 
-    def orders_in_market(self, exchange: str, symbol: str) -> bool:
+    def trades_in_market(self, exchange: str, symbol: str) -> bool:
         """
         Returns the market data of the symbol from the exchange.
 
         :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
         try:
-            self.orders(exchange=exchange, symbol=symbol)
+            self.trades(exchange=exchange, symbol=symbol)
 
             return True
 
         except ValueError:
             return False
         # end try
-    # end orders_in_market
+    # end trades_in_market
 
-    async def record(self, data: Ticker, timestamp: float) -> bool:
+    async def record(self, data: Trade, timestamp: float) -> bool:
         """
         Records the data from the crypto feed into the dataset.
 
         :param data: The data from the exchange.
         :param timestamp: The time of the request.
+
+        :return: The validation value.
         """
 
-        return await record_orders(
+        return await record_trades(
             market=self.market, data=data, timestamp=timestamp,
             callbacks=self.callbacks
         )
     # end record
-# end MarketOrdersRecorder
+# end TradesRecorder
 
-class OrdersMarketScreener(MarketScreener):
+class TradesMarketScreener(MarketScreener):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
@@ -366,31 +306,31 @@
 
     - amount:
         The amount of symbols for each symbols group for an exchange.
 
     - limited:
         The value to limit the running screeners to active exchanges.
 
-    >>> from crypto_screening.market.screeners import orders_market_screener
+    >>> from crypto_screening.market.screeners import trades_market_screener
     >>>
     >>> structure = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
-    >>> screener = orders_market_screener(data=structure)
+    >>> screener = trades_market_screener(data=structure)
     >>> screener.run()
     """
 
-    screeners: List[OrdersScreener]
-    recorder: OrdersMarketRecorder
+    screeners: List[TradesScreener]
+    recorder: TradesMarketRecorder
 
-    COLUMNS = OrdersMarketRecorder.COLUMNS
+    COLUMNS = TradesMarketRecorder.COLUMNS
 
     def __init__(
             self,
-            recorder: OrdersMarketRecorder,
-            screeners: Optional[Iterable[OrdersScreener]] = None,
+            recorder: TradesMarketRecorder,
+            screeners: Optional[Iterable[TradesScreener]] = None,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None,
             refresh: Optional[Union[float, dt.timedelta, bool]] = None,
             limited: Optional[bool] = None,
             handler: Optional[FeedHandler] = None,
             amount: Optional[int] = None
@@ -411,89 +351,89 @@
         super().__init__(
             location=location, cancel=cancel,
             delay=delay, recorder=recorder,
             screeners=screeners, handler=handler, limited=limited,
             amount=amount, refresh=refresh
         )
 
-        self.screeners[:] = screeners or self.create_orders_screeners()
+        self.screeners[:] = screeners or self.create_trades_screeners()
     # end __init__
 
     @property
-    def orders_market(self) -> Market:
+    def trades_market(self) -> Market:
         """
         Returns the market to hold the recorder data.
 
         :return: The market object.
         """
 
-        return self.recorder.orders_market
-    # end orders_market
+        return self.recorder.trades_market
+    # end trades_market
 
     @property
-    def orderbook_screeners(self) -> List[OrdersScreener]:
+    def trades_screeners(self) -> List[TradesScreener]:
         """
         Returns a list of all the order-book screeners.
 
         :return: The order-book screeners.
         """
 
         return [
             screener for screener in self.screeners
-            if isinstance(screener, OrdersScreener)
+            if isinstance(screener, TradesScreener)
         ]
-    # end orders_screeners
+    # end trades_screeners
 
     def connect_screeners(self) -> None:
         """Connects the screeners to the recording object."""
 
         for screener in self.screeners:
-            if isinstance(screener, OrdersScreener):
-                screener.market = self.orders(
+            if isinstance(screener, TradesScreener):
+                screener.market = self.trades(
                     exchange=screener.exchange, symbol=screener.symbol
                 )
             # end if
         # end for
     # end connect_screeners
 
-    def orders(self, exchange: str, symbol: str) -> pd.DataFrame:
+    def trades(self, exchange: str, symbol: str) -> pd.DataFrame:
         """
         Returns the market data of the symbol from the exchange.
 
         :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
-        return self.recorder.orders(exchange=exchange, symbol=symbol)
-    # end orders
+        return self.recorder.trades(exchange=exchange, symbol=symbol)
+    # end trades
 
-    def orders_in_market(self, exchange: str, symbol: str) -> bool:
+    def trades_in_market(self, exchange: str, symbol: str) -> bool:
         """
         Returns the market data of the symbol from the exchange.
 
         :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
-        return self.recorder.orders_in_market(exchange=exchange, symbol=symbol)
-    # end orders_in_market
+        return self.recorder.trades_in_market(exchange=exchange, symbol=symbol)
+    # end trades_in_market
 
-    def create_orders_screener(
+    def create_trades_screener(
             self,
             symbol: str,
             exchange: str,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None,
-            container: Optional[Dict[str, Dict[str, OrdersScreener]]] = None
-    ) -> OrdersScreener:
+            container: Optional[Dict[str, Dict[str, TradesScreener]]] = None
+    ) -> TradesScreener:
         """
         Defines the class attributes.
 
         :param symbol: The symbol of the asset.
         :param exchange: The exchange to get source data from.
         :param location: The saving location for the data.
         :param cancel: The time to cancel the waiting.
@@ -509,92 +449,92 @@
             cancel = self.cancel
         # end if
 
         if delay is None:
             delay = self.delay
         # end if
 
-        screener = OrdersScreener(
+        screener = TradesScreener(
             symbol=symbol, exchange=exchange, delay=delay,
             location=location, cancel=cancel, market=(
-                self.orders(exchange=exchange, symbol=symbol)
-                if self.orders_in_market(symbol=symbol, exchange=exchange)
+                self.trades(exchange=exchange, symbol=symbol)
+                if self.trades_in_market(symbol=symbol, exchange=exchange)
                 else None
             )
         )
 
         container.setdefault(exchange, {})[symbol] = screener
 
         return screener
-    # end create_orders_screener
+    # end create_trades_screener
 
-    def create_orders_screeners(
+    def create_trades_screeners(
             self,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None,
-            container: Optional[Dict[str, Dict[str, OrdersScreener]]] = None
-    ) -> List[OrdersScreener]:
+            container: Optional[Dict[str, Dict[str, TradesScreener]]] = None
+    ) -> List[TradesScreener]:
         """
         Defines the class attributes.
 
         :param location: The saving location for the data.
         :param cancel: The time to cancel the waiting.
         :param delay: The delay for the process.
         :param container: The container to contain the new screeners.
         """
 
         screeners = []
 
         for exchange, symbols in self.structure().items():
             for symbol in symbols:
                 screeners.append(
-                    self.create_orders_screener(
+                    self.create_trades_screener(
                         symbol=symbol, exchange=exchange, delay=delay,
                         location=location, cancel=cancel, container=container
                     )
                 )
             # end for
         # end for
 
         return screeners
-    # end create_orders_screeners
+    # end create_trades_screeners
 # end MarketOrderbookScreener
 
 Databases = Union[Iterable[str], Dict[str, Engine]]
 
-def orders_market_recorder(data: Dict[str, Iterable[str]]) -> OrdersMarketRecorder:
+def trades_market_recorder(data: Dict[str, Iterable[str]]) -> TradesMarketRecorder:
     """
     Creates the market recorder object for the data.
 
     :param data: The market data.
 
     :return: The market recorder object.
     """
 
-    return OrdersMarketRecorder(
-        market=create_orders_market(data=data)
+    return TradesMarketRecorder(
+        market=create_trades_market(data=data)
     )
-# end orders_market_recorder
+# end trades_market_recorder
 
-def orders_market_screener(
+def trades_market_screener(
         data: Dict[str, Iterable[str]],
         location: Optional[str] = None,
         cancel: Optional[Union[float, dt.timedelta]] = None,
         delay: Optional[Union[float, dt.timedelta]] = None,
         limited: Optional[bool] = None,
         handler: Optional[FeedHandler] = None,
         market: Optional[Market] = None,
         amount: Optional[int] = None,
         callbacks: Optional[Iterable[Callback]] = None,
         refresh: Optional[Union[float, dt.timedelta, bool]] = None,
-        recorder: Optional[OrdersMarketRecorder] = None,
+        recorder: Optional[TradesMarketRecorder] = None,
         fixed: Optional[bool] = True,
         parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
-) -> OrdersMarketScreener:
+) -> TradesMarketScreener:
     """
     Creates the market screener object for the data.
 
     :param data: The market data.
     :param handler: The handler object for the market data.
     :param limited: The value to limit the screeners to active only.
     :param parameters: The parameters for the exchanges.
@@ -607,23 +547,23 @@
     :param delay: The delay for the process.
     :param cancel: The cancel time for the loops.
     :param callbacks: The callbacks for the service.
 
     :return: The market screener object.
     """
 
-    screener = OrdersMarketScreener(
-        recorder=recorder or OrdersMarketRecorder(
-            market=market or create_orders_market(data=data),
+    screener = TradesMarketScreener(
+        recorder=recorder or TradesMarketRecorder(
+            market=market or create_trades_market(data=data),
             callbacks=callbacks
         ),
         handler=handler, location=location, amount=amount,
         cancel=cancel, delay=delay, limited=limited, refresh=refresh
     )
 
     screener.add_feeds(
         data=screener.recorder.structure(),
         fixed=fixed, parameters=parameters
     )
 
     return screener
-# end orders_market_screener
+# end trades_market_screener
```

### Comparing `crypto-screening-7.4.2/crypto_screening/market/screeners/recorder.py` & `crypto-screening-7.4.3/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/market/screeners/trades.py` & `crypto-screening-7.4.3/crypto_screening/market/screeners/orders.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,75 +1,74 @@
-# trades.py
+# orders.py
 
 import datetime as dt
 from typing import (
     Dict, Optional, Iterable, Any, Union, List, Callable
 )
 
 import pandas as pd
 
 from sqlalchemy import Engine
 
 from cryptofeed import FeedHandler
-from cryptofeed.types import Trade
-from cryptofeed.defines import TRADES
+from cryptofeed.types import Ticker
+from cryptofeed.defines import TICKER
 
 from crypto_screening.symbols import adjust_symbol
 from crypto_screening.process import find_string_value
 from crypto_screening.dataset import (
-    TRADES_COLUMNS, create_dataset,
-    AMOUNT, PRICE, SIDE, load_dataset, save_dataset
+    BIDS, ASKS, ORDERS_COLUMNS, create_dataset
 )
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.callbacks import Callback, callback_data
 from crypto_screening.market.screeners.recorder import MarketScreener, MarketRecorder
 
 __all__ = [
-    "TradesMarketScreener",
-    "TradesMarketRecorder",
-    "TradesScreener",
-    "create_trades_market",
-    "trades_market_screener",
-    "trades_market_recorder",
-    "create_trades_market_dataset",
-    "record_trades"
+    "OrdersMarketScreener",
+    "OrdersMarketRecorder",
+    "OrdersScreener",
+    "create_orders_market",
+    "orders_market_screener",
+    "orders_market_recorder",
+    "create_orders_market_dataset",
+    "record_orders"
 ]
 
 Market = Dict[str, Dict[str, pd.DataFrame]]
 
-def create_trades_market_dataset() -> pd.DataFrame:
+def create_orders_market_dataset() -> pd.DataFrame:
     """
     Creates a dataframe for the order book data.
 
     :return: The dataframe.
     """
 
     return create_dataset(
-        columns=TradesMarketRecorder.COLUMNS
+        columns=OrdersMarketRecorder.COLUMNS
     )
-# end create_trades_market_dataset
+# end create_orderbook_market_dataset
 
-def create_trades_market(data: Dict[str, Iterable[str]]) -> Market:
+def create_orders_market(data: Dict[str, Iterable[str]]) -> Market:
     """
     Creates the dataframes of the market data.
 
     :param data: The market data.
 
     :return: The dataframes of the market data.
     """
 
     return {
         exchange.lower(): {
-            symbol.upper(): create_trades_market_dataset()
+            symbol.upper(): create_orders_market_dataset()
             for symbol in data[exchange]
         } for exchange in data
     }
-# end create_trades_market
+# end create_orders_market
 
-class TradesScreener(BaseScreener):
+class OrdersScreener(BaseScreener):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
@@ -87,98 +86,36 @@
     - cancel:
         The time to cancel screening process after no new data is fetched.
 
     - delay:
         The delay to wait between each data fetching.
 
     - market:
-        The dataset of the market data as trades.
+        The dataset of the market data as orders.
     """
 
-    NAME = "TRADES"
+    NAME = "ORDERS"
+
+    COLUMNS = ORDERS_COLUMNS
 
     @property
-    def trades_market(self) -> pd.DataFrame:
+    def orders_market(self) -> pd.DataFrame:
         """
         Returns the market to hold the recorder data.
 
         :return: The market object.
         """
 
         return self.market
-    # end trades_market
-
-    def trades_dataset_path(self, location: Optional[str] = None) -> str:
-        """
-        Creates the path to the saving file for the screener object.
-
-        :param location: The saving location of the dataset.
-
-        :return: The saving path for the dataset.
-        """
-
-        return (
-            self.dataset_path(location=location).
-            replace(".csv", f"-{self.NAME}.csv")
-        )
-    # end trades_dataset_path
-
-    def save_trades_dataset(self, location: Optional[str] = None) -> None:
-        """
-        Saves the data of the screener.
-
-        :param location: The saving location of the dataset.
-        """
-
-        if len(self.trades_market) > 0:
-            save_dataset(
-                dataset=self.trades_market,
-                path=self.trades_dataset_path(location=location)
-            )
-        # end if
-    # end save_trades_dataset
-
-    def save_dataset(self, location: Optional[str] = None) -> None:
-        """
-        Saves the data of the screener.
+    # end orders_market
+# end OrdersScreener
 
-        :param location: The saving location of the dataset.
-        """
-
-        self.save_trades_dataset(location=location)
-    # end save_dataset
-
-    def load_trades_dataset(self, location: Optional[str] = None) -> None:
-        """
-        Saves the data of the screener.
-
-        :param location: The saving location of the dataset.
-        """
-
-        data = load_dataset(path=self.trades_dataset_path(location=location))
-
-        for index, data in zip(data.index[:], data.loc[:]):
-            self.trades_market.loc[index] = data
-        # end for
-    # end load_trades_dataset
-
-    def load_dataset(self, location: Optional[str] = None) -> None:
-        """
-        Saves the data of the screener.
-
-        :param location: The saving location of the dataset.
-        """
-
-        self.load_trades_dataset(location=location)
-    # end load_dataset
-# end TradesScreener
-
-async def record_trades(
+async def record_orders(
         market: Market,
-        data: Trade,
+        data: Ticker,
         timestamp: float,
         callbacks: Optional[Iterable[Callback]] = None
 ) -> bool:
     """
     Records the data from the crypto feed into the dataset.
 
     :param market: The market structure.
@@ -196,50 +133,49 @@
         value=adjust_symbol(symbol=data.symbol),
         values=exchange
     )
 
     dataset = (
         market.
         setdefault(exchange, {}).
-        setdefault(symbol, create_trades_market_dataset())
+        setdefault(symbol, create_orders_market_dataset())
     )
 
     try:
         index = dt.datetime.fromtimestamp(timestamp)
 
         if index in dataset.index:
             return False
         # end if
 
         data = {
-            AMOUNT: float(data.amount),
-            PRICE: float(data.price),
-            SIDE: data.side
+            BIDS: float(data.bid),
+            ASKS: float(data.ask)
         }
 
         dataset.loc[index] = data
 
         for callback in callbacks or []:
             payload = callback_data(
                 data=[(timestamp, data)], exchange=exchange, symbol=symbol
             )
 
-            await callback.record(payload, timestamp, key=TradesScreener.NAME)
+            await callback.record(payload, timestamp, key=OrdersScreener.NAME)
         # end if
 
         return True
 
     except IndexError:
         return False
     # end try
-# end record_trades
+# end record_orders
 
 RecorderParameters = Dict[str, Union[Iterable[str], Dict[str, Callable]]]
 
-class TradesMarketRecorder(MarketRecorder):
+class OrdersMarketRecorder(MarketRecorder):
     """
     A class to represent a crypto data feed recorder.
     This object passes the record method to the handler object to record
     the data fetched by the handler.
 
     Parameters:
 
@@ -255,92 +191,90 @@
     >>> from crypto_screening.market.screeners import orderbook_market_recorder
     >>>
     >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> recorder = orderbook_market_recorder(data=market)
     """
 
-    COLUMNS = TRADES_COLUMNS
+    COLUMNS = OrdersScreener.COLUMNS
 
     @property
-    def trades_market(self) -> Market:
+    def orders_market(self) -> Market:
         """
         Returns the market to hold the recorder data.
 
         :return: The market object.
         """
 
         return self.market
-    # end trades_market
+    # end orders_market
 
     def parameters(self) -> RecorderParameters:
         """
         Returns the order book parameters.
 
         :return: The order book parameters.
         """
 
         return dict(
-            channels=[TRADES],
-            callbacks={TRADES: self.record},
+            channels=[TICKER],
+            callbacks={TICKER: self.record},
             max_depth=1
         )
     # end parameters
 
-    def trades(self, exchange: str, symbol: str) -> pd.DataFrame:
+    def orders(self, exchange: str, symbol: str) -> pd.DataFrame:
         """
         Returns the market data of the symbol from the exchange.
 
         :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
         return self.data(exchange=exchange, symbol=symbol)
-    # end trades
+    # end orders
 
-    def trades_in_market(self, exchange: str, symbol: str) -> bool:
+    def orders_in_market(self, exchange: str, symbol: str) -> bool:
         """
         Returns the market data of the symbol from the exchange.
 
         :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
         try:
-            self.trades(exchange=exchange, symbol=symbol)
+            self.orders(exchange=exchange, symbol=symbol)
 
             return True
 
         except ValueError:
             return False
         # end try
-    # end trades_in_market
+    # end orders_in_market
 
-    async def record(self, data: Trade, timestamp: float) -> bool:
+    async def record(self, data: Ticker, timestamp: float) -> bool:
         """
         Records the data from the crypto feed into the dataset.
 
         :param data: The data from the exchange.
         :param timestamp: The time of the request.
-
-        :return: The validation value.
         """
 
-        return await record_trades(
+        return await record_orders(
             market=self.market, data=data, timestamp=timestamp,
             callbacks=self.callbacks
         )
     # end record
-# end TradesRecorder
+# end MarketOrdersRecorder
 
-class TradesMarketScreener(MarketScreener):
+class OrdersMarketScreener(MarketScreener):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
@@ -369,31 +303,31 @@
 
     - amount:
         The amount of symbols for each symbols group for an exchange.
 
     - limited:
         The value to limit the running screeners to active exchanges.
 
-    >>> from crypto_screening.market.screeners import trades_market_screener
+    >>> from crypto_screening.market.screeners import orders_market_screener
     >>>
     >>> structure = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
-    >>> screener = trades_market_screener(data=structure)
+    >>> screener = orders_market_screener(data=structure)
     >>> screener.run()
     """
 
-    screeners: List[TradesScreener]
-    recorder: TradesMarketRecorder
+    screeners: List[OrdersScreener]
+    recorder: OrdersMarketRecorder
 
-    COLUMNS = TradesMarketRecorder.COLUMNS
+    COLUMNS = OrdersMarketRecorder.COLUMNS
 
     def __init__(
             self,
-            recorder: TradesMarketRecorder,
-            screeners: Optional[Iterable[TradesScreener]] = None,
+            recorder: OrdersMarketRecorder,
+            screeners: Optional[Iterable[OrdersScreener]] = None,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None,
             refresh: Optional[Union[float, dt.timedelta, bool]] = None,
             limited: Optional[bool] = None,
             handler: Optional[FeedHandler] = None,
             amount: Optional[int] = None
@@ -414,89 +348,89 @@
         super().__init__(
             location=location, cancel=cancel,
             delay=delay, recorder=recorder,
             screeners=screeners, handler=handler, limited=limited,
             amount=amount, refresh=refresh
         )
 
-        self.screeners[:] = screeners or self.create_trades_screeners()
+        self.screeners[:] = screeners or self.create_orders_screeners()
     # end __init__
 
     @property
-    def trades_market(self) -> Market:
+    def orders_market(self) -> Market:
         """
         Returns the market to hold the recorder data.
 
         :return: The market object.
         """
 
-        return self.recorder.trades_market
-    # end trades_market
+        return self.recorder.orders_market
+    # end orders_market
 
     @property
-    def trades_screeners(self) -> List[TradesScreener]:
+    def orderbook_screeners(self) -> List[OrdersScreener]:
         """
         Returns a list of all the order-book screeners.
 
         :return: The order-book screeners.
         """
 
         return [
             screener for screener in self.screeners
-            if isinstance(screener, TradesScreener)
+            if isinstance(screener, OrdersScreener)
         ]
-    # end trades_screeners
+    # end orders_screeners
 
     def connect_screeners(self) -> None:
         """Connects the screeners to the recording object."""
 
         for screener in self.screeners:
-            if isinstance(screener, TradesScreener):
-                screener.market = self.trades(
+            if isinstance(screener, OrdersScreener):
+                screener.market = self.orders(
                     exchange=screener.exchange, symbol=screener.symbol
                 )
             # end if
         # end for
     # end connect_screeners
 
-    def trades(self, exchange: str, symbol: str) -> pd.DataFrame:
+    def orders(self, exchange: str, symbol: str) -> pd.DataFrame:
         """
         Returns the market data of the symbol from the exchange.
 
         :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
-        return self.recorder.trades(exchange=exchange, symbol=symbol)
-    # end trades
+        return self.recorder.orders(exchange=exchange, symbol=symbol)
+    # end orders
 
-    def trades_in_market(self, exchange: str, symbol: str) -> bool:
+    def orders_in_market(self, exchange: str, symbol: str) -> bool:
         """
         Returns the market data of the symbol from the exchange.
 
         :param exchange: The source key of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
-        return self.recorder.trades_in_market(exchange=exchange, symbol=symbol)
-    # end trades_in_market
+        return self.recorder.orders_in_market(exchange=exchange, symbol=symbol)
+    # end orders_in_market
 
-    def create_trades_screener(
+    def create_orders_screener(
             self,
             symbol: str,
             exchange: str,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None,
-            container: Optional[Dict[str, Dict[str, TradesScreener]]] = None
-    ) -> TradesScreener:
+            container: Optional[Dict[str, Dict[str, OrdersScreener]]] = None
+    ) -> OrdersScreener:
         """
         Defines the class attributes.
 
         :param symbol: The symbol of the asset.
         :param exchange: The exchange to get source data from.
         :param location: The saving location for the data.
         :param cancel: The time to cancel the waiting.
@@ -512,92 +446,92 @@
             cancel = self.cancel
         # end if
 
         if delay is None:
             delay = self.delay
         # end if
 
-        screener = TradesScreener(
+        screener = OrdersScreener(
             symbol=symbol, exchange=exchange, delay=delay,
             location=location, cancel=cancel, market=(
-                self.trades(exchange=exchange, symbol=symbol)
-                if self.trades_in_market(symbol=symbol, exchange=exchange)
+                self.orders(exchange=exchange, symbol=symbol)
+                if self.orders_in_market(symbol=symbol, exchange=exchange)
                 else None
             )
         )
 
         container.setdefault(exchange, {})[symbol] = screener
 
         return screener
-    # end create_trades_screener
+    # end create_orders_screener
 
-    def create_trades_screeners(
+    def create_orders_screeners(
             self,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None,
-            container: Optional[Dict[str, Dict[str, TradesScreener]]] = None
-    ) -> List[TradesScreener]:
+            container: Optional[Dict[str, Dict[str, OrdersScreener]]] = None
+    ) -> List[OrdersScreener]:
         """
         Defines the class attributes.
 
         :param location: The saving location for the data.
         :param cancel: The time to cancel the waiting.
         :param delay: The delay for the process.
         :param container: The container to contain the new screeners.
         """
 
         screeners = []
 
         for exchange, symbols in self.structure().items():
             for symbol in symbols:
                 screeners.append(
-                    self.create_trades_screener(
+                    self.create_orders_screener(
                         symbol=symbol, exchange=exchange, delay=delay,
                         location=location, cancel=cancel, container=container
                     )
                 )
             # end for
         # end for
 
         return screeners
-    # end create_trades_screeners
+    # end create_orders_screeners
 # end MarketOrderbookScreener
 
 Databases = Union[Iterable[str], Dict[str, Engine]]
 
-def trades_market_recorder(data: Dict[str, Iterable[str]]) -> TradesMarketRecorder:
+def orders_market_recorder(data: Dict[str, Iterable[str]]) -> OrdersMarketRecorder:
     """
     Creates the market recorder object for the data.
 
     :param data: The market data.
 
     :return: The market recorder object.
     """
 
-    return TradesMarketRecorder(
-        market=create_trades_market(data=data)
+    return OrdersMarketRecorder(
+        market=create_orders_market(data=data)
     )
-# end trades_market_recorder
+# end orders_market_recorder
 
-def trades_market_screener(
+def orders_market_screener(
         data: Dict[str, Iterable[str]],
         location: Optional[str] = None,
         cancel: Optional[Union[float, dt.timedelta]] = None,
         delay: Optional[Union[float, dt.timedelta]] = None,
         limited: Optional[bool] = None,
         handler: Optional[FeedHandler] = None,
         market: Optional[Market] = None,
         amount: Optional[int] = None,
         callbacks: Optional[Iterable[Callback]] = None,
         refresh: Optional[Union[float, dt.timedelta, bool]] = None,
-        recorder: Optional[TradesMarketRecorder] = None,
+        recorder: Optional[OrdersMarketRecorder] = None,
         fixed: Optional[bool] = True,
         parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
-) -> TradesMarketScreener:
+) -> OrdersMarketScreener:
     """
     Creates the market screener object for the data.
 
     :param data: The market data.
     :param handler: The handler object for the market data.
     :param limited: The value to limit the screeners to active only.
     :param parameters: The parameters for the exchanges.
@@ -610,23 +544,23 @@
     :param delay: The delay for the process.
     :param cancel: The cancel time for the loops.
     :param callbacks: The callbacks for the service.
 
     :return: The market screener object.
     """
 
-    screener = TradesMarketScreener(
-        recorder=recorder or TradesMarketRecorder(
-            market=market or create_trades_market(data=data),
+    screener = OrdersMarketScreener(
+        recorder=recorder or OrdersMarketRecorder(
+            market=market or create_orders_market(data=data),
             callbacks=callbacks
         ),
         handler=handler, location=location, amount=amount,
         cancel=cancel, delay=delay, limited=limited, refresh=refresh
     )
 
     screener.add_feeds(
         data=screener.recorder.structure(),
         fixed=fixed, parameters=parameters
     )
 
     return screener
-# end trades_market_screener
+# end orders_market_screener
```

### Comparing `crypto-screening-7.4.2/crypto_screening/market/waiting.py` & `crypto-screening-7.4.3/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/process.py` & `crypto-screening-7.4.3/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/symbols.py` & `crypto-screening-7.4.3/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening/validate.py` & `crypto-screening-7.4.3/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.4.2/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-7.4.3/crypto_screening.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 7.4.2
+Version: 7.4.3
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-7.4.2/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-7.4.3/crypto_screening.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 MANIFEST.in
 README.md
 build.py
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.py
+crypto_screening/base.py
 crypto_screening/dataset.py
 crypto_screening/exchanges.py
 crypto_screening/interval.py
 crypto_screening/process.py
 crypto_screening/symbols.py
 crypto_screening/validate.py
 crypto_screening.egg-info/PKG-INFO
@@ -45,8 +46,9 @@
 crypto_screening/market/screeners/orderbook.py
 crypto_screening/market/screeners/orders.py
 crypto_screening/market/screeners/recorder.py
 crypto_screening/market/screeners/trades.py
 crypto_screening/market/screeners/collectors/__init__.py
 crypto_screening/market/screeners/collectors/base.py
 crypto_screening/market/screeners/collectors/database.py
-crypto_screening/market/screeners/collectors/sockets.py
+crypto_screening/market/screeners/collectors/sockets.py
+crypto_screening/source/data/all_exchanges_symbols.json
```

### Comparing `crypto-screening-7.4.2/setup.py` & `crypto-screening-7.4.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,18 +17,21 @@
     setup(
         package="crypto_screening",
         project="pyproject.toml",
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
+        include=[
+            "crypto_screening/source"
+        ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='7.4.2',
+        version='7.4.3',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

