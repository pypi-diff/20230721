# Comparing `tmp/odhpy-0.0.8.tar.gz` & `tmp/odhpy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odhpy-0.0.8.tar", last modified: Wed Dec 14 04:25:46 2022, max compression
+gzip compressed data, was "odhpy-0.0.9.tar", last modified: Wed Dec 14 05:40:54 2022, max compression
```

## Comparing `odhpy-0.0.8.tar` & `odhpy-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2022-12-14 04:25:46.021606 odhpy-0.0.8/
--rw-rw-rw-   0        0        0     1448 2022-12-14 04:25:46.020609 odhpy-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      961 2022-12-11 06:47:55.000000 odhpy-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2022-12-14 04:25:46.021606 odhpy-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      740 2022-12-04 07:28:14.000000 odhpy-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-14 04:25:45.982735 odhpy-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-12-14 04:25:45.989712 odhpy-0.0.8/src/odhpy/
--rw-rw-rw-   0        0        0       73 2022-12-11 07:33:10.000000 odhpy-0.0.8/src/odhpy/__init__.py
--rw-rw-rw-   0        0        0      123 2022-12-11 07:25:35.000000 odhpy-0.0.8/src/odhpy/demo.py
-drwxrwxrwx   0        0        0        0 2022-12-14 04:25:46.008648 odhpy-0.0.8/src/odhpy/io/
--rw-rw-rw-   0        0        0       17 2022-12-13 06:20:10.000000 odhpy-0.0.8/src/odhpy/io/__init__.py
--rw-rw-rw-   0        0        0      588 2022-12-14 01:05:59.000000 odhpy-0.0.8/src/odhpy/io/io.py
-drwxrwxrwx   0        0        0        0 2022-12-14 04:25:46.011639 odhpy-0.0.8/src/odhpy/plots/
--rw-rw-rw-   0        0        0       30 2022-12-11 12:34:43.000000 odhpy-0.0.8/src/odhpy/plots/__init__.py
--rw-rw-rw-   0        0        0     1988 2022-12-12 12:31:36.000000 odhpy-0.0.8/src/odhpy/plots/plot_functions.py
--rw-rw-rw-   0        0        0        0 2022-12-12 22:38:32.000000 odhpy-0.0.8/src/odhpy/plots/plotly_helpers.py
-drwxrwxrwx   0        0        0        0 2022-12-14 04:25:46.013632 odhpy-0.0.8/src/odhpy/stoch/
--rw-rw-rw-   0        0        0       23 2022-12-14 04:17:45.000000 odhpy-0.0.8/src/odhpy/stoch/__init__.py
--rw-rw-rw-   0        0        0        0 2022-12-11 07:35:57.000000 odhpy-0.0.8/src/odhpy/stoch/analyse.py
--rw-rw-rw-   0        0        0     2867 2022-12-14 04:11:12.000000 odhpy-0.0.8/src/odhpy/stoch/generate.py
-drwxrwxrwx   0        0        0        0 2022-12-14 04:25:46.015626 odhpy-0.0.8/src/odhpy/trans/
--rw-rw-rw-   0        0        0       27 2022-12-08 21:34:03.000000 odhpy-0.0.8/src/odhpy/trans/__init__.py
--rw-rw-rw-   0        0        0     3237 2022-12-11 07:57:56.000000 odhpy-0.0.8/src/odhpy/trans/transformers.py
-drwxrwxrwx   0        0        0        0 2022-12-14 04:25:46.019612 odhpy-0.0.8/src/odhpy/utils/
--rw-rw-rw-   0        0        0       69 2022-12-13 04:10:17.000000 odhpy-0.0.8/src/odhpy/utils/__init__.py
--rw-rw-rw-   0        0        0     1475 2022-12-14 01:01:28.000000 odhpy-0.0.8/src/odhpy/utils/dataframe_functions.py
--rw-rw-rw-   0        0        0     1885 2022-12-11 07:43:28.000000 odhpy-0.0.8/src/odhpy/utils/datetime_functions.py
--rw-rw-rw-   0        0        0      205 2022-12-14 04:25:33.000000 odhpy-0.0.8/src/odhpy/version.py
-drwxrwxrwx   0        0        0        0 2022-12-14 04:25:46.006656 odhpy-0.0.8/src/odhpy.egg-info/
--rw-rw-rw-   0        0        0     1448 2022-12-14 04:25:45.000000 odhpy-0.0.8/src/odhpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      599 2022-12-14 04:25:45.000000 odhpy-0.0.8/src/odhpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-14 04:25:45.000000 odhpy-0.0.8/src/odhpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2022-12-14 04:25:45.000000 odhpy-0.0.8/src/odhpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-12-14 05:40:54.007897 odhpy-0.0.9/
+-rw-rw-rw-   0        0        0     1448 2022-12-14 05:40:54.007897 odhpy-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      961 2022-12-11 06:47:55.000000 odhpy-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-12-14 05:40:54.007897 odhpy-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      740 2022-12-04 07:28:14.000000 odhpy-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-14 05:40:53.977632 odhpy-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2022-12-14 05:40:53.983612 odhpy-0.0.9/src/odhpy/
+-rw-rw-rw-   0        0        0       73 2022-12-11 07:33:10.000000 odhpy-0.0.9/src/odhpy/__init__.py
+-rw-rw-rw-   0        0        0      123 2022-12-11 07:25:35.000000 odhpy-0.0.9/src/odhpy/demo.py
+drwxrwxrwx   0        0        0        0 2022-12-14 05:40:53.995936 odhpy-0.0.9/src/odhpy/io/
+-rw-rw-rw-   0        0        0       17 2022-12-13 06:20:10.000000 odhpy-0.0.9/src/odhpy/io/__init__.py
+-rw-rw-rw-   0        0        0      983 2022-12-14 05:40:31.000000 odhpy-0.0.9/src/odhpy/io/io.py
+drwxrwxrwx   0        0        0        0 2022-12-14 05:40:53.998927 odhpy-0.0.9/src/odhpy/plots/
+-rw-rw-rw-   0        0        0       30 2022-12-11 12:34:43.000000 odhpy-0.0.9/src/odhpy/plots/__init__.py
+-rw-rw-rw-   0        0        0     1988 2022-12-12 12:31:36.000000 odhpy-0.0.9/src/odhpy/plots/plot_functions.py
+-rw-rw-rw-   0        0        0        0 2022-12-12 22:38:32.000000 odhpy-0.0.9/src/odhpy/plots/plotly_helpers.py
+drwxrwxrwx   0        0        0        0 2022-12-14 05:40:54.001917 odhpy-0.0.9/src/odhpy/stoch/
+-rw-rw-rw-   0        0        0       23 2022-12-14 04:17:45.000000 odhpy-0.0.9/src/odhpy/stoch/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-12-11 07:35:57.000000 odhpy-0.0.9/src/odhpy/stoch/analyse.py
+-rw-rw-rw-   0        0        0     2867 2022-12-14 04:11:12.000000 odhpy-0.0.9/src/odhpy/stoch/generate.py
+drwxrwxrwx   0        0        0        0 2022-12-14 05:40:54.003910 odhpy-0.0.9/src/odhpy/trans/
+-rw-rw-rw-   0        0        0       27 2022-12-08 21:34:03.000000 odhpy-0.0.9/src/odhpy/trans/__init__.py
+-rw-rw-rw-   0        0        0     3237 2022-12-11 07:57:56.000000 odhpy-0.0.9/src/odhpy/trans/transformers.py
+drwxrwxrwx   0        0        0        0 2022-12-14 05:40:54.006900 odhpy-0.0.9/src/odhpy/utils/
+-rw-rw-rw-   0        0        0       69 2022-12-13 04:10:17.000000 odhpy-0.0.9/src/odhpy/utils/__init__.py
+-rw-rw-rw-   0        0        0     1475 2022-12-14 01:01:28.000000 odhpy-0.0.9/src/odhpy/utils/dataframe_functions.py
+-rw-rw-rw-   0        0        0     1885 2022-12-11 07:43:28.000000 odhpy-0.0.9/src/odhpy/utils/datetime_functions.py
+-rw-rw-rw-   0        0        0      205 2022-12-14 05:40:45.000000 odhpy-0.0.9/src/odhpy/version.py
+drwxrwxrwx   0        0        0        0 2022-12-14 05:40:53.993943 odhpy-0.0.9/src/odhpy.egg-info/
+-rw-rw-rw-   0        0        0     1448 2022-12-14 05:40:53.000000 odhpy-0.0.9/src/odhpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      599 2022-12-14 05:40:53.000000 odhpy-0.0.9/src/odhpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-14 05:40:53.000000 odhpy-0.0.9/src/odhpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2022-12-14 05:40:53.000000 odhpy-0.0.9/src/odhpy.egg-info/top_level.txt
```

### Comparing `odhpy-0.0.8/PKG-INFO` & `odhpy-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odhpy
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of splashings to master that which has no form and count that which is uncountable.
 Home-page: https://bitbucket.org/odhydrology/odhpy.git
 Author: Chas Egan
 Author-email: chas@odhydrology.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `odhpy-0.0.8/README.md` & `odhpy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `odhpy-0.0.8/setup.py` & `odhpy-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.0.8/src/odhpy/io/io.py` & `odhpy-0.0.9/src/odhpy/io/io.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 import pandas as pd
 from odhpy import utils
 
-def read_ts_csv(filename, date_format=r"%d/%m/%Y", **kwargs):
+def read_ts_csv(filename, date_format=r"%d/%m/%Y", df=None, colprefix="", **kwargs):
     """Reads a daily timeseries csv into a DataFrame, and sets the index to the Date.
     Assumed there is a column named "Date"
 
     Args:
         filename (_type_): _description_
         date_format (str, optional): defaults to "%d/%m/%Y" as per Fors. Other common formats include "%Y-%m-%d", "%Y/%m/%d".
 
     Returns:
         _type_: _description_
     """
-    df = pd.read_csv(filename, **kwargs)
-    df = utils.set_index_dt(df, format=date_format)
+    if df == None:
+        df = pd.DataFrame()
+    temp = pd.read_csv(filename, **kwargs)
+    temp = utils.set_index_dt(temp, format=date_format)
+    if colprefix is not None:
+        for c in temp.columns:
+            temp.rename(columns = {c:f"{colprefix}{c}"}, inplace = True)        
+    df = df.join(temp, how="outer").sort_index()
+    # TODO: THERE IS NO GUARANTEE THAT THE DATES OVERLAP, THEREFORE WE MAY END UP WITH A DATAFRAME WITH INCOMPLETE DATES
     return df
```

### Comparing `odhpy-0.0.8/src/odhpy/plots/plot_functions.py` & `odhpy-0.0.9/src/odhpy/plots/plot_functions.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.0.8/src/odhpy/stoch/generate.py` & `odhpy-0.0.9/src/odhpy/stoch/generate.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.0.8/src/odhpy/trans/transformers.py` & `odhpy-0.0.9/src/odhpy/trans/transformers.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.0.8/src/odhpy/utils/dataframe_functions.py` & `odhpy-0.0.9/src/odhpy/utils/dataframe_functions.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.0.8/src/odhpy/utils/datetime_functions.py` & `odhpy-0.0.9/src/odhpy/utils/datetime_functions.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.0.8/src/odhpy.egg-info/PKG-INFO` & `odhpy-0.0.9/src/odhpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odhpy
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of splashings to master that which has no form and count that which is uncountable.
 Home-page: https://bitbucket.org/odhydrology/odhpy.git
 Author: Chas Egan
 Author-email: chas@odhydrology.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `odhpy-0.0.8/src/odhpy.egg-info/SOURCES.txt` & `odhpy-0.0.9/src/odhpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

