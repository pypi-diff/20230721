# Comparing `tmp/pyharmonics-1.1.tar.gz` & `tmp/pyharmonics-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyharmonics-1.1.tar", last modified: Fri Jul 21 14:51:13 2023, max compression
+gzip compressed data, was "pyharmonics-1.2.tar", last modified: Fri Jul 21 15:18:51 2023, max compression
```

## Comparing `pyharmonics-1.1.tar` & `pyharmonics-1.2.tar`

### file list

```diff
@@ -1,21 +1,39 @@
-drwxrwxr-x   0 xual      (1000) xual      (1000)        0 2023-07-21 14:51:13.419966 pyharmonics-1.1/
--rw-rw-r--   0 xual      (1000) xual      (1000)     1071 2023-07-16 13:05:50.000000 pyharmonics-1.1/LICENSE
--rw-rw-r--   0 xual      (1000) xual      (1000)     3649 2023-07-21 14:51:13.419966 pyharmonics-1.1/PKG-INFO
--rw-rw-r--   0 xual      (1000) xual      (1000)     3309 2023-07-21 14:14:42.000000 pyharmonics-1.1/README.md
-drwxrwxr-x   0 xual      (1000) xual      (1000)        0 2023-07-21 14:51:13.419966 pyharmonics-1.1/pyharmonics.egg-info/
--rw-rw-r--   0 xual      (1000) xual      (1000)     3649 2023-07-21 14:51:13.000000 pyharmonics-1.1/pyharmonics.egg-info/PKG-INFO
--rw-rw-r--   0 xual      (1000) xual      (1000)      388 2023-07-21 14:51:13.000000 pyharmonics-1.1/pyharmonics.egg-info/SOURCES.txt
--rw-rw-r--   0 xual      (1000) xual      (1000)        1 2023-07-21 14:51:13.000000 pyharmonics-1.1/pyharmonics.egg-info/dependency_links.txt
--rw-rw-r--   0 xual      (1000) xual      (1000)       69 2023-07-21 14:51:13.000000 pyharmonics-1.1/pyharmonics.egg-info/requires.txt
--rw-rw-r--   0 xual      (1000) xual      (1000)        1 2023-07-21 14:51:13.000000 pyharmonics-1.1/pyharmonics.egg-info/top_level.txt
--rw-rw-r--   0 xual      (1000) xual      (1000)      743 2023-07-21 14:47:02.000000 pyharmonics-1.1/pyproject.toml
--rw-rw-r--   0 xual      (1000) xual      (1000)       38 2023-07-21 14:51:13.419966 pyharmonics-1.1/setup.cfg
-drwxrwxr-x   0 xual      (1000) xual      (1000)        0 2023-07-21 14:51:13.419966 pyharmonics-1.1/tests/
--rw-rw-r--   0 xual      (1000) xual      (1000)     1692 2023-07-18 20:32:34.000000 pyharmonics-1.1/tests/test_aplaca.py
--rw-rw-r--   0 xual      (1000) xual      (1000)     2132 2023-07-16 13:05:50.000000 pyharmonics-1.1/tests/test_binance.py
--rw-rw-r--   0 xual      (1000) xual      (1000)      156 2023-07-16 13:05:50.000000 pyharmonics-1.1/tests/test_market_data_base.py
--rw-rw-r--   0 xual      (1000) xual      (1000)     8323 2023-07-21 14:12:20.000000 pyharmonics-1.1/tests/test_matrix.py
--rw-rw-r--   0 xual      (1000) xual      (1000)      820 2023-07-21 14:12:27.000000 pyharmonics-1.1/tests/test_plotter.py
--rw-rw-r--   0 xual      (1000) xual      (1000)     4056 2023-07-21 14:12:30.000000 pyharmonics-1.1/tests/test_technicals.py
--rw-rw-r--   0 xual      (1000) xual      (1000)     3600 2023-07-18 20:32:34.000000 pyharmonics-1.1/tests/test_utils.py
--rw-rw-r--   0 xual      (1000) xual      (1000)     1660 2023-07-16 13:05:50.000000 pyharmonics-1.1/tests/test_yahoo.py
+drwxrwxr-x   0 xual      (1000) xual      (1000)        0 2023-07-21 15:18:51.325231 pyharmonics-1.2/
+-rw-rw-r--   0 xual      (1000) xual      (1000)     1071 2023-07-16 13:05:50.000000 pyharmonics-1.2/LICENSE
+-rw-rw-r--   0 xual      (1000) xual      (1000)     3649 2023-07-21 15:18:51.325231 pyharmonics-1.2/PKG-INFO
+-rw-rw-r--   0 xual      (1000) xual      (1000)     3309 2023-07-21 14:14:42.000000 pyharmonics-1.2/README.md
+-rw-rw-r--   0 xual      (1000) xual      (1000)      743 2023-07-21 15:04:23.000000 pyharmonics-1.2/pyproject.toml
+-rw-rw-r--   0 xual      (1000) xual      (1000)       38 2023-07-21 15:18:51.325231 pyharmonics-1.2/setup.cfg
+drwxrwxr-x   0 xual      (1000) xual      (1000)        0 2023-07-21 15:18:51.321231 pyharmonics-1.2/src/
+drwxrwxr-x   0 xual      (1000) xual      (1000)        0 2023-07-21 15:18:51.321231 pyharmonics-1.2/src/pyharmonics/
+-rw-rw-r--   0 xual      (1000) xual      (1000)      301 2023-07-21 14:04:02.000000 pyharmonics-1.2/src/pyharmonics/__init__.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)    15581 2023-07-21 11:05:22.000000 pyharmonics-1.2/src/pyharmonics/constants.py
+drwxrwxr-x   0 xual      (1000) xual      (1000)        0 2023-07-21 15:18:51.321231 pyharmonics-1.2/src/pyharmonics/marketdata/
+-rw-rw-r--   0 xual      (1000) xual      (1000)      284 2023-07-16 13:05:50.000000 pyharmonics-1.2/src/pyharmonics/marketdata/__init__.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)     8010 2023-07-19 15:09:38.000000 pyharmonics-1.2/src/pyharmonics/marketdata/alpaca.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)     9205 2023-07-18 20:32:34.000000 pyharmonics-1.2/src/pyharmonics/marketdata/binance_data.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)     5229 2023-07-19 19:05:48.000000 pyharmonics-1.2/src/pyharmonics/marketdata/candle_base.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)     5103 2023-07-18 20:32:34.000000 pyharmonics-1.2/src/pyharmonics/marketdata/yahoo.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)     5003 2023-07-21 13:47:32.000000 pyharmonics-1.2/src/pyharmonics/pattern.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)    26621 2023-07-21 14:14:05.000000 pyharmonics-1.2/src/pyharmonics/plotter.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)     3785 2023-07-21 14:08:22.000000 pyharmonics-1.2/src/pyharmonics/positions.py
+drwxrwxr-x   0 xual      (1000) xual      (1000)        0 2023-07-21 15:18:51.325231 pyharmonics-1.2/src/pyharmonics/search/
+-rw-rw-r--   0 xual      (1000) xual      (1000)       65 2023-07-21 10:42:33.000000 pyharmonics-1.2/src/pyharmonics/search/__init__.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)    19167 2023-07-21 14:10:39.000000 pyharmonics-1.2/src/pyharmonics/search/matrix.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)    16563 2023-07-21 14:11:36.000000 pyharmonics-1.2/src/pyharmonics/technicals.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)     8006 2023-07-18 20:32:34.000000 pyharmonics-1.2/src/pyharmonics/utils.py
+drwxrwxr-x   0 xual      (1000) xual      (1000)        0 2023-07-21 15:18:51.321231 pyharmonics-1.2/src/pyharmonics.egg-info/
+-rw-rw-r--   0 xual      (1000) xual      (1000)     3649 2023-07-21 15:18:51.000000 pyharmonics-1.2/src/pyharmonics.egg-info/PKG-INFO
+-rw-rw-r--   0 xual      (1000) xual      (1000)      868 2023-07-21 15:18:51.000000 pyharmonics-1.2/src/pyharmonics.egg-info/SOURCES.txt
+-rw-rw-r--   0 xual      (1000) xual      (1000)        1 2023-07-21 15:18:51.000000 pyharmonics-1.2/src/pyharmonics.egg-info/dependency_links.txt
+-rw-rw-r--   0 xual      (1000) xual      (1000)       69 2023-07-21 15:18:51.000000 pyharmonics-1.2/src/pyharmonics.egg-info/requires.txt
+-rw-rw-r--   0 xual      (1000) xual      (1000)       12 2023-07-21 15:18:51.000000 pyharmonics-1.2/src/pyharmonics.egg-info/top_level.txt
+drwxrwxr-x   0 xual      (1000) xual      (1000)        0 2023-07-21 15:18:51.325231 pyharmonics-1.2/tests/
+-rw-rw-r--   0 xual      (1000) xual      (1000)     1692 2023-07-18 20:32:34.000000 pyharmonics-1.2/tests/test_aplaca.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)     2132 2023-07-16 13:05:50.000000 pyharmonics-1.2/tests/test_binance.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)      156 2023-07-16 13:05:50.000000 pyharmonics-1.2/tests/test_market_data_base.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)     8323 2023-07-21 14:12:20.000000 pyharmonics-1.2/tests/test_matrix.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)      820 2023-07-21 14:12:27.000000 pyharmonics-1.2/tests/test_plotter.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)     4056 2023-07-21 14:12:30.000000 pyharmonics-1.2/tests/test_technicals.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)     3600 2023-07-18 20:32:34.000000 pyharmonics-1.2/tests/test_utils.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)     1660 2023-07-16 13:05:50.000000 pyharmonics-1.2/tests/test_yahoo.py
```

### Comparing `pyharmonics-1.1/LICENSE` & `pyharmonics-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyharmonics-1.1/PKG-INFO` & `pyharmonics-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyharmonics
-Version: 1.1
+Version: 1.2
 Author-email: Niall O'Connor <zechs.marquie@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyharmonics-1.1/README.md` & `pyharmonics-1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyharmonics-1.1/pyharmonics.egg-info/PKG-INFO` & `pyharmonics-1.2/src/pyharmonics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyharmonics
-Version: 1.1
+Version: 1.2
 Author-email: Niall O'Connor <zechs.marquie@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyharmonics-1.1/pyproject.toml` & `pyharmonics-1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   { name="Niall O'Connor", email="zechs.marquie@gmail.com" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-version = "1.1"
+version = "1.2"
 dependencies = [
     "yfinance",
     "alpaca-trade-api",
     "ta",
     "binance-connector",
     "plotly",
     "kaleido",
```

### Comparing `pyharmonics-1.1/tests/test_aplaca.py` & `pyharmonics-1.2/tests/test_aplaca.py`

 * *Files identical despite different names*

### Comparing `pyharmonics-1.1/tests/test_binance.py` & `pyharmonics-1.2/tests/test_binance.py`

 * *Files identical despite different names*

### Comparing `pyharmonics-1.1/tests/test_matrix.py` & `pyharmonics-1.2/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `pyharmonics-1.1/tests/test_plotter.py` & `pyharmonics-1.2/tests/test_plotter.py`

 * *Files identical despite different names*

### Comparing `pyharmonics-1.1/tests/test_technicals.py` & `pyharmonics-1.2/tests/test_technicals.py`

 * *Files identical despite different names*

### Comparing `pyharmonics-1.1/tests/test_utils.py` & `pyharmonics-1.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyharmonics-1.1/tests/test_yahoo.py` & `pyharmonics-1.2/tests/test_yahoo.py`

 * *Files identical despite different names*

