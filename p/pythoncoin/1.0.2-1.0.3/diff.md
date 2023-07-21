# Comparing `tmp/pythoncoin-1.0.2.tar.gz` & `tmp/pythoncoin-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoncoin-1.0.2.tar", last modified: Fri Jul 21 10:14:37 2023, max compression
+gzip compressed data, was "pythoncoin-1.0.3.tar", last modified: Fri Jul 21 10:22:16 2023, max compression
```

## Comparing `pythoncoin-1.0.2.tar` & `pythoncoin-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 hadi      (1000) hadi      (1000)        0 2023-07-21 10:14:37.241416 pythoncoin-1.0.2/
--rw-rw-r--   0 hadi      (1000) hadi      (1000)     5983 2023-07-21 10:14:37.241416 pythoncoin-1.0.2/PKG-INFO
--rw-rw-r--   0 hadi      (1000) hadi      (1000)     5556 2023-07-10 10:37:32.000000 pythoncoin-1.0.2/README.md
-drwxrwxr-x   0 hadi      (1000) hadi      (1000)        0 2023-07-21 10:14:37.229416 pythoncoin-1.0.2/pycoin/
--rw-rw-r--   0 hadi      (1000) hadi      (1000)        0 2023-07-10 10:37:32.000000 pythoncoin-1.0.2/pycoin/__init__.py
-drwxrwxr-x   0 hadi      (1000) hadi      (1000)        0 2023-07-21 10:14:37.233416 pythoncoin-1.0.2/pycoin/market_data_gathering/
--rw-rw-r--   0 hadi      (1000) hadi      (1000)        0 2023-07-10 10:37:32.000000 pythoncoin-1.0.2/pycoin/market_data_gathering/__init__.py
--rw-rw-r--   0 hadi      (1000) hadi      (1000)    28063 2023-07-10 10:37:32.000000 pythoncoin-1.0.2/pycoin/market_data_gathering/market_processing.py
--rw-rw-r--   0 hadi      (1000) hadi      (1000)     6267 2023-07-10 10:37:32.000000 pythoncoin-1.0.2/pycoin/market_data_gathering/trend_filters.py
-drwxrwxr-x   0 hadi      (1000) hadi      (1000)        0 2023-07-21 10:14:37.233416 pythoncoin-1.0.2/pycoin/market_data_kline_plots/
--rw-rw-r--   0 hadi      (1000) hadi      (1000)        0 2023-07-10 10:37:32.000000 pythoncoin-1.0.2/pycoin/market_data_kline_plots/__init__.py
--rw-rw-r--   0 hadi      (1000) hadi      (1000)    23253 2023-07-10 10:37:32.000000 pythoncoin-1.0.2/pycoin/market_data_kline_plots/market_plotter.py
-drwxrwxr-x   0 hadi      (1000) hadi      (1000)        0 2023-07-21 10:14:37.241416 pythoncoin-1.0.2/pythoncoin.egg-info/
--rw-rw-r--   0 hadi      (1000) hadi      (1000)     5983 2023-07-21 10:14:37.000000 pythoncoin-1.0.2/pythoncoin.egg-info/PKG-INFO
--rw-rw-r--   0 hadi      (1000) hadi      (1000)      435 2023-07-21 10:14:37.000000 pythoncoin-1.0.2/pythoncoin.egg-info/SOURCES.txt
--rw-rw-r--   0 hadi      (1000) hadi      (1000)        1 2023-07-21 10:14:37.000000 pythoncoin-1.0.2/pythoncoin.egg-info/dependency_links.txt
--rw-rw-r--   0 hadi      (1000) hadi      (1000)       34 2023-07-21 10:14:37.000000 pythoncoin-1.0.2/pythoncoin.egg-info/requires.txt
--rw-rw-r--   0 hadi      (1000) hadi      (1000)       67 2023-07-21 10:14:37.000000 pythoncoin-1.0.2/pythoncoin.egg-info/top_level.txt
--rw-rw-r--   0 hadi      (1000) hadi      (1000)       38 2023-07-21 10:14:37.241416 pythoncoin-1.0.2/setup.cfg
--rw-rw-r--   0 hadi      (1000) hadi      (1000)      888 2023-07-21 10:13:15.000000 pythoncoin-1.0.2/setup.py
+drwxrwxr-x   0 hadi      (1000) hadi      (1000)        0 2023-07-21 10:22:16.859420 pythoncoin-1.0.3/
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)     6033 2023-07-21 10:22:16.859420 pythoncoin-1.0.3/PKG-INFO
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)     5606 2023-07-21 10:19:27.000000 pythoncoin-1.0.3/README.md
+drwxrwxr-x   0 hadi      (1000) hadi      (1000)        0 2023-07-21 10:22:16.843418 pythoncoin-1.0.3/pycoin/
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)        0 2023-07-10 10:37:32.000000 pythoncoin-1.0.3/pycoin/__init__.py
+drwxrwxr-x   0 hadi      (1000) hadi      (1000)        0 2023-07-21 10:22:16.847419 pythoncoin-1.0.3/pycoin/market_data_gathering/
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)        0 2023-07-10 10:37:32.000000 pythoncoin-1.0.3/pycoin/market_data_gathering/__init__.py
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)    28063 2023-07-10 10:37:32.000000 pythoncoin-1.0.3/pycoin/market_data_gathering/market_processing.py
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)     6267 2023-07-10 10:37:32.000000 pythoncoin-1.0.3/pycoin/market_data_gathering/trend_filters.py
+drwxrwxr-x   0 hadi      (1000) hadi      (1000)        0 2023-07-21 10:22:16.847419 pythoncoin-1.0.3/pycoin/market_data_kline_plots/
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)        0 2023-07-10 10:37:32.000000 pythoncoin-1.0.3/pycoin/market_data_kline_plots/__init__.py
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)    23253 2023-07-10 10:37:32.000000 pythoncoin-1.0.3/pycoin/market_data_kline_plots/market_plotter.py
+drwxrwxr-x   0 hadi      (1000) hadi      (1000)        0 2023-07-21 10:22:16.855419 pythoncoin-1.0.3/pythoncoin.egg-info/
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)     6033 2023-07-21 10:22:16.000000 pythoncoin-1.0.3/pythoncoin.egg-info/PKG-INFO
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)      435 2023-07-21 10:22:16.000000 pythoncoin-1.0.3/pythoncoin.egg-info/SOURCES.txt
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)        1 2023-07-21 10:22:16.000000 pythoncoin-1.0.3/pythoncoin.egg-info/dependency_links.txt
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)       34 2023-07-21 10:22:16.000000 pythoncoin-1.0.3/pythoncoin.egg-info/requires.txt
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)       67 2023-07-21 10:22:16.000000 pythoncoin-1.0.3/pythoncoin.egg-info/top_level.txt
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)       38 2023-07-21 10:22:16.859420 pythoncoin-1.0.3/setup.cfg
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)      888 2023-07-21 10:22:01.000000 pythoncoin-1.0.3/setup.py
```

### Comparing `pythoncoin-1.0.2/PKG-INFO` & `pythoncoin-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythoncoin
-Version: 1.0.2
+Version: 1.0.3
 Summary: a packege to make some algorithmic trading analyses easy.
 Home-page: https://github.com/hadif1999/pycoin
 Author: Hadi Fathipour
 Author-email: hadi9628983@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -28,15 +28,18 @@
 Note: many of the functions in this package works with standard column names, standard column names are:
 "open", "close", "high", "low", "volume", "datetime", "timestamp". 
 so it's better to change your market dataframe column names if they are not as the above format.
 you can also change your column name using some methods that will be discussed in examples.
 
 Note: row indexes of your input dataframe must be integer not datetime or timestamp format.
 instead you must have a column named "datetime" that keeps time index of each row. 
-
+## Installation
+```bash
+pip install pythoncoin
+```
 ## Quick start
 
 after cloning the repo you can use these commands to make a market processing object:
 
 ```python 
 
 from pycoin.market_data_gathering.market_processing import Market_Processing
```

### Comparing `pythoncoin-1.0.2/README.md` & `pythoncoin-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 Note: many of the functions in this package works with standard column names, standard column names are:
 "open", "close", "high", "low", "volume", "datetime", "timestamp". 
 so it's better to change your market dataframe column names if they are not as the above format.
 you can also change your column name using some methods that will be discussed in examples.
 
 Note: row indexes of your input dataframe must be integer not datetime or timestamp format.
 instead you must have a column named "datetime" that keeps time index of each row. 
-
+## Installation
+```bash
+pip install pythoncoin
+```
 ## Quick start
 
 after cloning the repo you can use these commands to make a market processing object:
 
 ```python 
 
 from pycoin.market_data_gathering.market_processing import Market_Processing
```

### Comparing `pythoncoin-1.0.2/pycoin/market_data_gathering/market_processing.py` & `pythoncoin-1.0.3/pycoin/market_data_gathering/market_processing.py`

 * *Files identical despite different names*

### Comparing `pythoncoin-1.0.2/pycoin/market_data_gathering/trend_filters.py` & `pythoncoin-1.0.3/pycoin/market_data_gathering/trend_filters.py`

 * *Files identical despite different names*

### Comparing `pythoncoin-1.0.2/pycoin/market_data_kline_plots/market_plotter.py` & `pythoncoin-1.0.3/pycoin/market_data_kline_plots/market_plotter.py`

 * *Files identical despite different names*

### Comparing `pythoncoin-1.0.2/pythoncoin.egg-info/PKG-INFO` & `pythoncoin-1.0.3/pythoncoin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythoncoin
-Version: 1.0.2
+Version: 1.0.3
 Summary: a packege to make some algorithmic trading analyses easy.
 Home-page: https://github.com/hadif1999/pycoin
 Author: Hadi Fathipour
 Author-email: hadi9628983@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -28,15 +28,18 @@
 Note: many of the functions in this package works with standard column names, standard column names are:
 "open", "close", "high", "low", "volume", "datetime", "timestamp". 
 so it's better to change your market dataframe column names if they are not as the above format.
 you can also change your column name using some methods that will be discussed in examples.
 
 Note: row indexes of your input dataframe must be integer not datetime or timestamp format.
 instead you must have a column named "datetime" that keeps time index of each row. 
-
+## Installation
+```bash
+pip install pythoncoin
+```
 ## Quick start
 
 after cloning the repo you can use these commands to make a market processing object:
 
 ```python 
 
 from pycoin.market_data_gathering.market_processing import Market_Processing
```

### Comparing `pythoncoin-1.0.2/setup.py` & `pythoncoin-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name='pythoncoin',
-    version='v1.0.02',
+    version='v1.0.03',
     packages=['pycoin', 'pycoin/market_data_gathering', 'pycoin/market_data_kline_plots'],
     license="MIT",
     author='Hadi Fathipour',
     author_email="hadi9628983@gmail.com",
     url='https://github.com/hadif1999/pycoin',
     description="a packege to make some algorithmic trading analyses easy.",
     install_requires=['plotly', 'pandas', 'numpy', 'kucoin-python'],
```

