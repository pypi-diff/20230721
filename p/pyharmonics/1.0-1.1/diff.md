# Comparing `tmp/pyharmonics-1.0.tar.gz` & `tmp/pyharmonics-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyharmonics-1.0.tar", last modified: Wed Jul 19 19:21:08 2023, max compression
+gzip compressed data, was "pyharmonics-1.1.tar", last modified: Fri Jul 21 14:51:13 2023, max compression
```

## Comparing `pyharmonics-1.0.tar` & `pyharmonics-1.1.tar`

### file list

```diff
@@ -1,39 +1,21 @@
-drwxrwxr-x   0 xual      (1000) xual      (1000)        0 2023-07-19 19:21:08.215167 pyharmonics-1.0/
--rw-rw-r--   0 xual      (1000) xual      (1000)     1071 2023-07-16 13:05:50.000000 pyharmonics-1.0/LICENSE
--rw-rw-r--   0 xual      (1000) xual      (1000)     3627 2023-07-19 19:21:08.211167 pyharmonics-1.0/PKG-INFO
--rw-rw-r--   0 xual      (1000) xual      (1000)     3287 2023-07-19 19:14:37.000000 pyharmonics-1.0/README.md
--rw-rw-r--   0 xual      (1000) xual      (1000)      743 2023-07-19 19:20:30.000000 pyharmonics-1.0/pyproject.toml
--rw-rw-r--   0 xual      (1000) xual      (1000)       38 2023-07-19 19:21:08.215167 pyharmonics-1.0/setup.cfg
-drwxrwxr-x   0 xual      (1000) xual      (1000)        0 2023-07-19 19:21:08.211167 pyharmonics-1.0/src/
-drwxrwxr-x   0 xual      (1000) xual      (1000)        0 2023-07-19 19:21:08.211167 pyharmonics-1.0/src/pyharmonics/
--rw-rw-r--   0 xual      (1000) xual      (1000)       65 2023-07-18 20:32:34.000000 pyharmonics-1.0/src/pyharmonics/__init__.py
--rw-rw-r--   0 xual      (1000) xual      (1000)    15226 2023-07-18 20:32:34.000000 pyharmonics-1.0/src/pyharmonics/constants.py
--rw-rw-r--   0 xual      (1000) xual      (1000)       45 2023-07-16 13:05:50.000000 pyharmonics-1.0/src/pyharmonics/example.py
-drwxrwxr-x   0 xual      (1000) xual      (1000)        0 2023-07-19 19:21:08.211167 pyharmonics-1.0/src/pyharmonics/marketdata/
--rw-rw-r--   0 xual      (1000) xual      (1000)      284 2023-07-16 13:05:50.000000 pyharmonics-1.0/src/pyharmonics/marketdata/__init__.py
--rw-rw-r--   0 xual      (1000) xual      (1000)     8010 2023-07-19 15:09:38.000000 pyharmonics-1.0/src/pyharmonics/marketdata/alpaca.py
--rw-rw-r--   0 xual      (1000) xual      (1000)     9205 2023-07-18 20:32:34.000000 pyharmonics-1.0/src/pyharmonics/marketdata/binance_data.py
--rw-rw-r--   0 xual      (1000) xual      (1000)     5229 2023-07-19 19:05:48.000000 pyharmonics-1.0/src/pyharmonics/marketdata/candle_base.py
--rw-rw-r--   0 xual      (1000) xual      (1000)     5103 2023-07-18 20:32:34.000000 pyharmonics-1.0/src/pyharmonics/marketdata/yahoo.py
--rw-rw-r--   0 xual      (1000) xual      (1000)    31750 2023-07-19 19:05:48.000000 pyharmonics-1.0/src/pyharmonics/plotter.py
-drwxrwxr-x   0 xual      (1000) xual      (1000)        0 2023-07-19 19:21:08.211167 pyharmonics-1.0/src/pyharmonics/search/
--rw-rw-r--   0 xual      (1000) xual      (1000)      176 2023-07-19 19:05:48.000000 pyharmonics-1.0/src/pyharmonics/search/__init__.py
--rw-rw-r--   0 xual      (1000) xual      (1000)    18981 2023-07-19 19:05:48.000000 pyharmonics-1.0/src/pyharmonics/search/matrix.py
--rw-rw-r--   0 xual      (1000) xual      (1000)     4839 2023-07-19 19:05:48.000000 pyharmonics-1.0/src/pyharmonics/search/patterns.py
--rw-rw-r--   0 xual      (1000) xual      (1000)    17016 2023-07-19 19:05:48.000000 pyharmonics-1.0/src/pyharmonics/technicals.py
--rw-rw-r--   0 xual      (1000) xual      (1000)     8006 2023-07-18 20:32:34.000000 pyharmonics-1.0/src/pyharmonics/utils.py
-drwxrwxr-x   0 xual      (1000) xual      (1000)        0 2023-07-19 19:21:08.211167 pyharmonics-1.0/src/pyharmonics.egg-info/
--rw-rw-r--   0 xual      (1000) xual      (1000)     3627 2023-07-19 19:21:08.000000 pyharmonics-1.0/src/pyharmonics.egg-info/PKG-INFO
--rw-rw-r--   0 xual      (1000) xual      (1000)      874 2023-07-19 19:21:08.000000 pyharmonics-1.0/src/pyharmonics.egg-info/SOURCES.txt
--rw-rw-r--   0 xual      (1000) xual      (1000)        1 2023-07-19 19:21:08.000000 pyharmonics-1.0/src/pyharmonics.egg-info/dependency_links.txt
--rw-rw-r--   0 xual      (1000) xual      (1000)       69 2023-07-19 19:21:08.000000 pyharmonics-1.0/src/pyharmonics.egg-info/requires.txt
--rw-rw-r--   0 xual      (1000) xual      (1000)       12 2023-07-19 19:21:08.000000 pyharmonics-1.0/src/pyharmonics.egg-info/top_level.txt
-drwxrwxr-x   0 xual      (1000) xual      (1000)        0 2023-07-19 19:21:08.211167 pyharmonics-1.0/tests/
--rw-rw-r--   0 xual      (1000) xual      (1000)     1692 2023-07-18 20:32:34.000000 pyharmonics-1.0/tests/test_aplaca.py
--rw-rw-r--   0 xual      (1000) xual      (1000)     2132 2023-07-16 13:05:50.000000 pyharmonics-1.0/tests/test_binance.py
--rw-rw-r--   0 xual      (1000) xual      (1000)      156 2023-07-16 13:05:50.000000 pyharmonics-1.0/tests/test_market_data_base.py
--rw-rw-r--   0 xual      (1000) xual      (1000)     8301 2023-07-19 19:05:48.000000 pyharmonics-1.0/tests/test_matrix.py
--rw-rw-r--   0 xual      (1000) xual      (1000)      657 2023-07-19 19:05:48.000000 pyharmonics-1.0/tests/test_plotter.py
--rw-rw-r--   0 xual      (1000) xual      (1000)     4034 2023-07-19 19:05:48.000000 pyharmonics-1.0/tests/test_technicals.py
--rw-rw-r--   0 xual      (1000) xual      (1000)     3600 2023-07-18 20:32:34.000000 pyharmonics-1.0/tests/test_utils.py
--rw-rw-r--   0 xual      (1000) xual      (1000)     1660 2023-07-16 13:05:50.000000 pyharmonics-1.0/tests/test_yahoo.py
+drwxrwxr-x   0 xual      (1000) xual      (1000)        0 2023-07-21 14:51:13.419966 pyharmonics-1.1/
+-rw-rw-r--   0 xual      (1000) xual      (1000)     1071 2023-07-16 13:05:50.000000 pyharmonics-1.1/LICENSE
+-rw-rw-r--   0 xual      (1000) xual      (1000)     3649 2023-07-21 14:51:13.419966 pyharmonics-1.1/PKG-INFO
+-rw-rw-r--   0 xual      (1000) xual      (1000)     3309 2023-07-21 14:14:42.000000 pyharmonics-1.1/README.md
+drwxrwxr-x   0 xual      (1000) xual      (1000)        0 2023-07-21 14:51:13.419966 pyharmonics-1.1/pyharmonics.egg-info/
+-rw-rw-r--   0 xual      (1000) xual      (1000)     3649 2023-07-21 14:51:13.000000 pyharmonics-1.1/pyharmonics.egg-info/PKG-INFO
+-rw-rw-r--   0 xual      (1000) xual      (1000)      388 2023-07-21 14:51:13.000000 pyharmonics-1.1/pyharmonics.egg-info/SOURCES.txt
+-rw-rw-r--   0 xual      (1000) xual      (1000)        1 2023-07-21 14:51:13.000000 pyharmonics-1.1/pyharmonics.egg-info/dependency_links.txt
+-rw-rw-r--   0 xual      (1000) xual      (1000)       69 2023-07-21 14:51:13.000000 pyharmonics-1.1/pyharmonics.egg-info/requires.txt
+-rw-rw-r--   0 xual      (1000) xual      (1000)        1 2023-07-21 14:51:13.000000 pyharmonics-1.1/pyharmonics.egg-info/top_level.txt
+-rw-rw-r--   0 xual      (1000) xual      (1000)      743 2023-07-21 14:47:02.000000 pyharmonics-1.1/pyproject.toml
+-rw-rw-r--   0 xual      (1000) xual      (1000)       38 2023-07-21 14:51:13.419966 pyharmonics-1.1/setup.cfg
+drwxrwxr-x   0 xual      (1000) xual      (1000)        0 2023-07-21 14:51:13.419966 pyharmonics-1.1/tests/
+-rw-rw-r--   0 xual      (1000) xual      (1000)     1692 2023-07-18 20:32:34.000000 pyharmonics-1.1/tests/test_aplaca.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)     2132 2023-07-16 13:05:50.000000 pyharmonics-1.1/tests/test_binance.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)      156 2023-07-16 13:05:50.000000 pyharmonics-1.1/tests/test_market_data_base.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)     8323 2023-07-21 14:12:20.000000 pyharmonics-1.1/tests/test_matrix.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)      820 2023-07-21 14:12:27.000000 pyharmonics-1.1/tests/test_plotter.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)     4056 2023-07-21 14:12:30.000000 pyharmonics-1.1/tests/test_technicals.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)     3600 2023-07-18 20:32:34.000000 pyharmonics-1.1/tests/test_utils.py
+-rw-rw-r--   0 xual      (1000) xual      (1000)     1660 2023-07-16 13:05:50.000000 pyharmonics-1.1/tests/test_yahoo.py
```

### Comparing `pyharmonics-1.0/LICENSE` & `pyharmonics-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyharmonics-1.0/PKG-INFO` & `pyharmonics-1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyharmonics
-Version: 1.0
+Version: 1.1
 Author-email: Niall O'Connor <zechs.marquie@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -62,15 +62,15 @@
 
 [1000 rows x 7 columns]
 ```
 
 Create a technicals object for further analysis.
 ```
 >>> from pyharmonics.technicals import Technicals
->>> t = Technicals(b.df)
+>>> t = Technicals(b.df, b.symbol, b.interval)
 ```
 
 Search for a harmonic pattern.
 ```
 >>> from pyharmonics.search import MatrixSearch
 >>> m = MatrixSearch(t)
 >>> m.search()
```

### Comparing `pyharmonics-1.0/README.md` & `pyharmonics-1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 [1000 rows x 7 columns]
 ```
 
 Create a technicals object for further analysis.
 ```
 >>> from pyharmonics.technicals import Technicals
->>> t = Technicals(b.df)
+>>> t = Technicals(b.df, b.symbol, b.interval)
 ```
 
 Search for a harmonic pattern.
 ```
 >>> from pyharmonics.search import MatrixSearch
 >>> m = MatrixSearch(t)
 >>> m.search()
```

### Comparing `pyharmonics-1.0/pyproject.toml` & `pyharmonics-1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   { name="Niall O'Connor", email="zechs.marquie@gmail.com" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-version = "1.0"
+version = "1.1"
 dependencies = [
     "yfinance",
     "alpaca-trade-api",
     "ta",
     "binance-connector",
     "plotly",
     "kaleido",
```

### Comparing `pyharmonics-1.0/src/pyharmonics.egg-info/PKG-INFO` & `pyharmonics-1.1/pyharmonics.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyharmonics
-Version: 1.0
+Version: 1.1
 Author-email: Niall O'Connor <zechs.marquie@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -62,15 +62,15 @@
 
 [1000 rows x 7 columns]
 ```
 
 Create a technicals object for further analysis.
 ```
 >>> from pyharmonics.technicals import Technicals
->>> t = Technicals(b.df)
+>>> t = Technicals(b.df, b.symbol, b.interval)
 ```
 
 Search for a harmonic pattern.
 ```
 >>> from pyharmonics.search import MatrixSearch
 >>> m = MatrixSearch(t)
 >>> m.search()
```

### Comparing `pyharmonics-1.0/tests/test_aplaca.py` & `pyharmonics-1.1/tests/test_aplaca.py`

 * *Files identical despite different names*

### Comparing `pyharmonics-1.0/tests/test_binance.py` & `pyharmonics-1.1/tests/test_binance.py`

 * *Files identical despite different names*

### Comparing `pyharmonics-1.0/tests/test_matrix.py` & `pyharmonics-1.1/tests/test_matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pyharmonics.search import MatrixSearch
 from pyharmonics.technicals import Technicals
 import pandas as pd
 
 b = BinanceCandleData()
 b._set_params('BTCUSDT', b.HOUR_1, 1000, None, None)
 b.df = pd.read_pickle("tests/data/btc_test_data")
-t = Technicals(b.df, peak_spacing=10)
+t = Technicals(b.df, b.symbol, b.interval, peak_spacing=10)
 m = MatrixSearch(t, fib_tolerance=0.03)
 m.search()
 m.forming()
 
 def test_xabcd_search():
     assert (len(m._formed[constants.XABCD]) == 6)
     results = sorted([i.p_id for i in m._formed[constants.XABCD]])
```

### Comparing `pyharmonics-1.0/tests/test_technicals.py` & `pyharmonics-1.1/tests/test_technicals.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pyharmonics.technicals import Technicals
 import pandas as pd
 import numpy as np
 
 b = BinanceCandleData()
 b._set_params('BTCUSDT', b.HOUR_1, 1000, None, None)
 b.df = pd.read_pickle('tests/data/btc_test_data')
-t = Technicals(b.df, peak_spacing=20)
+t = Technicals(b.df, b.symbol, b.interval, peak_spacing=20)
 
 def test_price_dips():
     given = t.get_peak_x_y(t.PRICE_DIPS)
     expected = (
         np.array([20, 49, 89, 121, 145, 197, 233, 278, 314, 377, 427, 456, 521, 567, 626, 723, 759, 807, 833, 927, 989]),
         np.array([18711.87, 18125.98, 18531.42, 18805.34, 18629.2, 18471.28, 18843.01, 19159.42, 18920.35, 19730.0, 19320.0,
                   19237.14, 18860.0, 18190.0, 18975.18, 18900.0, 18650.0, 19070.11, 19157.0, 20000.09, 20427.23])
```

### Comparing `pyharmonics-1.0/tests/test_utils.py` & `pyharmonics-1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyharmonics-1.0/tests/test_yahoo.py` & `pyharmonics-1.1/tests/test_yahoo.py`

 * *Files identical despite different names*

