# Comparing `tmp/pythoncoin-1.0.1.tar.gz` & `tmp/pythoncoin-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoncoin-1.0.1.tar", last modified: Fri Jul 21 09:37:50 2023, max compression
+gzip compressed data, was "pythoncoin-1.0.2.tar", last modified: Fri Jul 21 10:14:37 2023, max compression
```

## Comparing `pythoncoin-1.0.1.tar` & `pythoncoin-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 hadi      (1000) hadi      (1000)        0 2023-07-21 09:37:50.355508 pythoncoin-1.0.1/
--rw-rw-r--   0 hadi      (1000) hadi      (1000)      386 2023-07-21 09:37:50.355508 pythoncoin-1.0.1/PKG-INFO
--rw-rw-r--   0 hadi      (1000) hadi      (1000)     5556 2023-07-10 10:37:32.000000 pythoncoin-1.0.1/README.md
-drwxrwxr-x   0 hadi      (1000) hadi      (1000)        0 2023-07-21 09:37:50.343508 pythoncoin-1.0.1/pycoin/
--rw-rw-r--   0 hadi      (1000) hadi      (1000)        0 2023-07-10 10:37:32.000000 pythoncoin-1.0.1/pycoin/__init__.py
-drwxrwxr-x   0 hadi      (1000) hadi      (1000)        0 2023-07-21 09:37:50.343508 pythoncoin-1.0.1/pycoin/market_data_gathering/
--rw-rw-r--   0 hadi      (1000) hadi      (1000)        0 2023-07-10 10:37:32.000000 pythoncoin-1.0.1/pycoin/market_data_gathering/__init__.py
--rw-rw-r--   0 hadi      (1000) hadi      (1000)    28063 2023-07-10 10:37:32.000000 pythoncoin-1.0.1/pycoin/market_data_gathering/market_processing.py
--rw-rw-r--   0 hadi      (1000) hadi      (1000)     6267 2023-07-10 10:37:32.000000 pythoncoin-1.0.1/pycoin/market_data_gathering/trend_filters.py
-drwxrwxr-x   0 hadi      (1000) hadi      (1000)        0 2023-07-21 09:37:50.347508 pythoncoin-1.0.1/pycoin/market_data_kline_plots/
--rw-rw-r--   0 hadi      (1000) hadi      (1000)        0 2023-07-10 10:37:32.000000 pythoncoin-1.0.1/pycoin/market_data_kline_plots/__init__.py
--rw-rw-r--   0 hadi      (1000) hadi      (1000)    23253 2023-07-10 10:37:32.000000 pythoncoin-1.0.1/pycoin/market_data_kline_plots/market_plotter.py
-drwxrwxr-x   0 hadi      (1000) hadi      (1000)        0 2023-07-21 09:37:50.355508 pythoncoin-1.0.1/pythoncoin.egg-info/
--rw-rw-r--   0 hadi      (1000) hadi      (1000)      386 2023-07-21 09:37:50.000000 pythoncoin-1.0.1/pythoncoin.egg-info/PKG-INFO
--rw-rw-r--   0 hadi      (1000) hadi      (1000)      435 2023-07-21 09:37:50.000000 pythoncoin-1.0.1/pythoncoin.egg-info/SOURCES.txt
--rw-rw-r--   0 hadi      (1000) hadi      (1000)        1 2023-07-21 09:37:50.000000 pythoncoin-1.0.1/pythoncoin.egg-info/dependency_links.txt
--rw-rw-r--   0 hadi      (1000) hadi      (1000)       34 2023-07-21 09:37:50.000000 pythoncoin-1.0.1/pythoncoin.egg-info/requires.txt
--rw-rw-r--   0 hadi      (1000) hadi      (1000)       67 2023-07-21 09:37:50.000000 pythoncoin-1.0.1/pythoncoin.egg-info/top_level.txt
--rw-rw-r--   0 hadi      (1000) hadi      (1000)       38 2023-07-21 09:37:50.355508 pythoncoin-1.0.1/setup.cfg
--rw-rw-r--   0 hadi      (1000) hadi      (1000)      671 2023-07-21 09:36:30.000000 pythoncoin-1.0.1/setup.py
+drwxrwxr-x   0 hadi      (1000) hadi      (1000)        0 2023-07-21 10:14:37.241416 pythoncoin-1.0.2/
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)     5983 2023-07-21 10:14:37.241416 pythoncoin-1.0.2/PKG-INFO
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)     5556 2023-07-10 10:37:32.000000 pythoncoin-1.0.2/README.md
+drwxrwxr-x   0 hadi      (1000) hadi      (1000)        0 2023-07-21 10:14:37.229416 pythoncoin-1.0.2/pycoin/
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)        0 2023-07-10 10:37:32.000000 pythoncoin-1.0.2/pycoin/__init__.py
+drwxrwxr-x   0 hadi      (1000) hadi      (1000)        0 2023-07-21 10:14:37.233416 pythoncoin-1.0.2/pycoin/market_data_gathering/
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)        0 2023-07-10 10:37:32.000000 pythoncoin-1.0.2/pycoin/market_data_gathering/__init__.py
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)    28063 2023-07-10 10:37:32.000000 pythoncoin-1.0.2/pycoin/market_data_gathering/market_processing.py
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)     6267 2023-07-10 10:37:32.000000 pythoncoin-1.0.2/pycoin/market_data_gathering/trend_filters.py
+drwxrwxr-x   0 hadi      (1000) hadi      (1000)        0 2023-07-21 10:14:37.233416 pythoncoin-1.0.2/pycoin/market_data_kline_plots/
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)        0 2023-07-10 10:37:32.000000 pythoncoin-1.0.2/pycoin/market_data_kline_plots/__init__.py
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)    23253 2023-07-10 10:37:32.000000 pythoncoin-1.0.2/pycoin/market_data_kline_plots/market_plotter.py
+drwxrwxr-x   0 hadi      (1000) hadi      (1000)        0 2023-07-21 10:14:37.241416 pythoncoin-1.0.2/pythoncoin.egg-info/
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)     5983 2023-07-21 10:14:37.000000 pythoncoin-1.0.2/pythoncoin.egg-info/PKG-INFO
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)      435 2023-07-21 10:14:37.000000 pythoncoin-1.0.2/pythoncoin.egg-info/SOURCES.txt
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)        1 2023-07-21 10:14:37.000000 pythoncoin-1.0.2/pythoncoin.egg-info/dependency_links.txt
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)       34 2023-07-21 10:14:37.000000 pythoncoin-1.0.2/pythoncoin.egg-info/requires.txt
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)       67 2023-07-21 10:14:37.000000 pythoncoin-1.0.2/pythoncoin.egg-info/top_level.txt
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)       38 2023-07-21 10:14:37.241416 pythoncoin-1.0.2/setup.cfg
+-rw-rw-r--   0 hadi      (1000) hadi      (1000)      888 2023-07-21 10:13:15.000000 pythoncoin-1.0.2/setup.py
```

### Comparing `pythoncoin-1.0.1/README.md` & `pythoncoin-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pythoncoin-1.0.1/pycoin/market_data_gathering/market_processing.py` & `pythoncoin-1.0.2/pycoin/market_data_gathering/market_processing.py`

 * *Files identical despite different names*

### Comparing `pythoncoin-1.0.1/pycoin/market_data_gathering/trend_filters.py` & `pythoncoin-1.0.2/pycoin/market_data_gathering/trend_filters.py`

 * *Files identical despite different names*

### Comparing `pythoncoin-1.0.1/pycoin/market_data_kline_plots/market_plotter.py` & `pythoncoin-1.0.2/pycoin/market_data_kline_plots/market_plotter.py`

 * *Files identical despite different names*

### Comparing `pythoncoin-1.0.1/setup.py` & `pythoncoin-1.0.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 #!/usr/bin/python3
 # -*- coding:utf-8 -*-
 
 from setuptools import setup
 
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
 
 setup(
     name='pythoncoin',
-    version='v1.0.01',
+    version='v1.0.02',
     packages=['pycoin', 'pycoin/market_data_gathering', 'pycoin/market_data_kline_plots'],
     license="MIT",
     author='Hadi Fathipour',
     author_email="hadi9628983@gmail.com",
     url='https://github.com/hadif1999/pycoin',
     description="a packege to make some algorithmic trading analyses easy.",
     install_requires=['plotly', 'pandas', 'numpy', 'kucoin-python'],
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

