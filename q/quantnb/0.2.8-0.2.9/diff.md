# Comparing `tmp/quantnb-0.2.8.tar.gz` & `tmp/quantnb-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantnb-0.2.8.tar", max compression
+gzip compressed data, was "quantnb-0.2.9.tar", max compression
```

## Comparing `quantnb-0.2.8.tar` & `quantnb-0.2.9.tar`

### file list

```diff
@@ -1,35 +1,42 @@
--rw-r--r--   0        0        0      112 2023-06-07 12:08:16.607057 quantnb-0.2.8/README.md
--rw-r--r--   0        0        0      543 2023-06-30 23:49:16.096814 quantnb-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      280 2023-06-08 09:33:29.937029 quantnb-0.2.8/quantnb/__init__.py
--rw-r--r--   0        0        0     5857 2023-06-10 15:34:06.176901 quantnb-0.2.8/quantnb/core/backtester.py
--rw-r--r--   0        0        0     8199 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/core/backtester_old.py
--rw-r--r--   0        0        0       80 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/core/enums.py
--rw-r--r--   0        0        0     1337 2023-06-30 23:07:30.161852 quantnb-0.2.8/quantnb/helpers/S_calculate_metrics.py
--rw-r--r--   0        0        0      357 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/helpers/S_print_orders.py
--rw-r--r--   0        0        0      728 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/helpers/S_print_trades.py
--rw-r--r--   0        0        0      300 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/helpers/__init__.py
--rw-r--r--   0        0        0      793 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/helpers/analyze_trade_duration.py
--rw-r--r--   0        0        0      380 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/helpers/calculate_average_freq.py
--rw-r--r--   0        0        0     1038 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/helpers/calculate_pf_stats.py
--rw-r--r--   0        0        0      390 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/helpers/calculate_risk_free.py
--rw-r--r--   0        0        0      213 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/helpers/get_average_trade_duration.py
--rw-r--r--   0        0        0      672 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/helpers/get_realized_pf_value.py
--rw-r--r--   0        0        0      325 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/helpers/plot_lines.py
--rw-r--r--   0        0        0      731 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/helpers/save_to_csv.py
--rw-r--r--   0        0        0      109 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/indicators/EMA.py
--rw-r--r--   0        0        0      109 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/indicators/SMA.py
--rw-r--r--   0        0        0       79 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/indicators/__init__.py
--rw-r--r--   0        0        0      160 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/indicators/cross_below.py
--rw-r--r--   0        0        0      391 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/lib/__init__.py
--rw-r--r--   0        0        0     1143 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/lib/create_binance_dataframe.py
--rw-r--r--   0        0        0      905 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/lib/fetch_binance_data.py
--rw-r--r--   0        0        0      359 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/lib/find_files.py
--rw-r--r--   0        0        0     1127 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/lib/multiprocess.py
--rw-r--r--   0        0        0      889 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/lib/optimize.py
--rw-r--r--   0        0        0      241 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/lib/resample.py
--rw-r--r--   0        0        0     3034 2023-06-30 23:49:02.624505 quantnb-0.2.8/quantnb/strategies/S_base.py
--rw-r--r--   0        0        0     2245 2023-06-30 23:38:29.961758 quantnb-0.2.8/quantnb/strategies/S_test.py
--rw-r--r--   0        0        0       29 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/strategies/__init__.py
--rw-r--r--   0        0        0      678 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/tests/benchmark_multiple_assets.py
--rw-r--r--   0        0        0      698 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/tests/optimisation_combine_files.py
--rw-r--r--   0        0        0      906 1970-01-01 00:00:00.000000 quantnb-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      112 2023-06-07 12:08:16.607057 quantnb-0.2.9/README.md
+-rw-r--r--   0        0        0      615 2023-07-18 12:51:30.631981 quantnb-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-06-08 09:33:29.937029 quantnb-0.2.9/quantnb/__init__.py
+-rw-r--r--   0        0        0     8567 2023-07-18 12:51:02.298676 quantnb-0.2.9/quantnb/core/backtester.py
+-rw-r--r--   0        0        0     8199 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/core/backtester_old.py
+-rw-r--r--   0        0        0       80 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/core/enums.py
+-rw-r--r--   0        0        0     2900 2023-07-18 12:51:02.288676 quantnb-0.2.9/quantnb/helpers/H_ticks_to_ranges.py
+-rw-r--r--   0        0        0     1337 2023-06-30 23:07:30.161852 quantnb-0.2.9/quantnb/helpers/S_calculate_metrics.py
+-rw-r--r--   0        0        0      357 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/helpers/S_print_orders.py
+-rw-r--r--   0        0        0      728 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/helpers/S_print_trades.py
+-rw-r--r--   0        0        0      300 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/helpers/__init__.py
+-rw-r--r--   0        0        0      793 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/helpers/analyze_trade_duration.py
+-rw-r--r--   0        0        0      380 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/helpers/calculate_average_freq.py
+-rw-r--r--   0        0        0     1038 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/helpers/calculate_pf_stats.py
+-rw-r--r--   0        0        0      390 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/helpers/calculate_risk_free.py
+-rw-r--r--   0        0        0      213 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/helpers/get_average_trade_duration.py
+-rw-r--r--   0        0        0      672 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/helpers/get_realized_pf_value.py
+-rw-r--r--   0        0        0      325 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/helpers/plot_lines.py
+-rw-r--r--   0        0        0      731 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/helpers/save_to_csv.py
+-rw-r--r--   0        0        0      109 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/indicators/EMA.py
+-rw-r--r--   0        0        0      351 2023-07-14 18:13:59.469996 quantnb-0.2.9/quantnb/indicators/HMA.py
+-rw-r--r--   0        0        0      109 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/indicators/SMA.py
+-rw-r--r--   0        0        0       79 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/indicators/__init__.py
+-rw-r--r--   0        0        0      160 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/indicators/cross_below.py
+-rw-r--r--   0        0        0     1502 2023-07-14 18:18:10.994171 quantnb-0.2.9/quantnb/indicators/random_data.py
+-rw-r--r--   0        0        0     1253 2023-07-14 18:07:37.591031 quantnb-0.2.9/quantnb/indicators/supertrend.py
+-rw-r--r--   0        0        0      391 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/lib/__init__.py
+-rw-r--r--   0        0        0     1143 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/lib/create_binance_dataframe.py
+-rw-r--r--   0        0        0      905 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/lib/fetch_binance_data.py
+-rw-r--r--   0        0        0      359 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/lib/find_files.py
+-rw-r--r--   0        0        0     1131 2023-07-05 11:15:06.173263 quantnb-0.2.9/quantnb/lib/multiprocess.py
+-rw-r--r--   0        0        0      889 2023-07-13 14:40:24.770094 quantnb-0.2.9/quantnb/lib/optimize.py
+-rw-r--r--   0        0        0      241 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/lib/resample.py
+-rw-r--r--   0        0        0     3666 2023-07-01 00:15:50.699650 quantnb-0.2.9/quantnb/strategies/S_MACD.py
+-rw-r--r--   0        0        0     3088 2023-07-18 12:51:02.298676 quantnb-0.2.9/quantnb/strategies/S_base.py
+-rw-r--r--   0        0        0     1776 2023-07-18 12:51:02.298676 quantnb-0.2.9/quantnb/strategies/S_bid_ask.py
+-rw-r--r--   0        0        0     2245 2023-07-17 17:01:19.633674 quantnb-0.2.9/quantnb/strategies/S_test.py
+-rw-r--r--   0        0        0       29 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/strategies/__init__.py
+-rw-r--r--   0        0        0      678 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/tests/benchmark_multiple_assets.py
+-rw-r--r--   0        0        0      698 2023-06-08 09:25:10.940100 quantnb-0.2.9/quantnb/tests/optimisation_combine_files.py
+-rw-r--r--   0        0        0      682 2023-07-14 18:18:30.134596 quantnb-0.2.9/quantnb/tests/supertrend_test.py
+-rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 quantnb-0.2.9/PKG-INFO
```

### Comparing `quantnb-0.2.8/quantnb/core/backtester_old.py` & `quantnb-0.2.9/quantnb/core/backtester_old.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.8/quantnb/helpers/S_calculate_metrics.py` & `quantnb-0.2.9/quantnb/helpers/S_calculate_metrics.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.8/quantnb/helpers/S_print_trades.py` & `quantnb-0.2.9/quantnb/helpers/S_print_trades.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.8/quantnb/helpers/analyze_trade_duration.py` & `quantnb-0.2.9/quantnb/helpers/analyze_trade_duration.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.8/quantnb/helpers/calculate_pf_stats.py` & `quantnb-0.2.9/quantnb/helpers/calculate_pf_stats.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.8/quantnb/helpers/get_realized_pf_value.py` & `quantnb-0.2.9/quantnb/helpers/get_realized_pf_value.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.8/quantnb/helpers/save_to_csv.py` & `quantnb-0.2.9/quantnb/helpers/save_to_csv.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.8/quantnb/lib/create_binance_dataframe.py` & `quantnb-0.2.9/quantnb/lib/create_binance_dataframe.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.8/quantnb/lib/fetch_binance_data.py` & `quantnb-0.2.9/quantnb/lib/fetch_binance_data.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.8/quantnb/lib/multiprocess.py` & `quantnb-0.2.9/quantnb/lib/multiprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def worker(method, items, NUMBER_OF_CPU, iteration, args, queue):
     result = method(items, NUMBER_OF_CPU, iteration, *args)
     queue.put(result)
 
 
 def multiprocess(items, method, *args):
-    NUMBER_OF_CPU = multiprocessing.cpu_count()
+    NUMBER_OF_CPU = multiprocessing.cpu_count() - 1
 
     # Calculate the length of each part
     part_length = math.ceil(len(items) / NUMBER_OF_CPU)
     divided_list = [
         items[i : i + part_length] for i in range(0, len(items), part_length)
     ]
```

### Comparing `quantnb-0.2.8/quantnb/lib/optimize.py` & `quantnb-0.2.9/quantnb/lib/optimize.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.8/quantnb/strategies/S_base.py` & `quantnb-0.2.9/quantnb/strategies/S_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,17 @@
         return (
             bt.final_value,
             bt.equity,
             bt.orders[: bt.order_idx, :],
             bt.trades[: bt.trade_idx, :],
         )
 
+    def backtest_bid_ask(self, params):
+        pass
+
     def backtest(self, params):
         self.get_signals(params)
         (final_value, equity, orders_arr, trades_arr) = self.simulation(
             mode=1, use_sl=self.use_sl
         )
         self.orders_arr = orders_arr
```

### Comparing `quantnb-0.2.8/quantnb/strategies/S_test.py` & `quantnb-0.2.9/quantnb/strategies/S_test.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.8/quantnb/tests/benchmark_multiple_assets.py` & `quantnb-0.2.9/quantnb/tests/benchmark_multiple_assets.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.8/quantnb/tests/optimisation_combine_files.py` & `quantnb-0.2.9/quantnb/tests/optimisation_combine_files.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.8/PKG-INFO` & `quantnb-0.2.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: quantnb
-Version: 0.2.8
+Version: 0.2.9
 Summary: 
 Author: Alpha
 Author-email: piotr@piotryordanov.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipython (>=8.14.0,<9.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: mplfinance (>=0.12.9b7,<0.13.0)
 Requires-Dist: numba (>=0.57.0,<0.58.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: pandas-ta (>=0.3.14b0,<0.4.0)
+Requires-Dist: polars (>=0.18.4,<0.19.0)
 Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
 Requires-Dist: python-binance (>=1.0.17,<2.0.0)
 Requires-Dist: quantstats (>=0.0.59,<0.0.60)
 Requires-Dist: seaborn[stats] (>=0.12.2,<0.13.0)
 Requires-Dist: ta-lib (>=0.4.26,<0.5.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
```

