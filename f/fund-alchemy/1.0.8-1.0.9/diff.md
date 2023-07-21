# Comparing `tmp/fund_alchemy-1.0.8.tar.gz` & `tmp/fund_alchemy-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\fund_alchemy-1.0.8.tar", last modified: Wed Jun 29 07:42:26 2022, max compression
+gzip compressed data, was "dist\fund_alchemy-1.0.9.tar", last modified: Wed Jun 29 08:55:08 2022, max compression
```

## Comparing `fund_alchemy-1.0.8.tar` & `fund_alchemy-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-06-29 07:42:26.480000 fund_alchemy-1.0.8/
--rw-rw-rw-   0        0        0     1079 2021-12-20 13:51:28.000000 fund_alchemy-1.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0      727 2022-06-29 07:42:28.000000 fund_alchemy-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      265 2022-06-29 07:12:50.000000 fund_alchemy-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-06-29 07:42:26.530000 fund_alchemy-1.0.8/fund_alchemy/
--rw-rw-rw-   0        0        0       58 2022-06-29 02:57:12.000000 fund_alchemy-1.0.8/fund_alchemy/__init__.py
--rw-rw-rw-   0        0        0   123318 2022-06-29 06:32:46.000000 fund_alchemy-1.0.8/fund_alchemy/config.py
--rw-rw-rw-   0        0        0    18095 2022-06-29 06:36:24.000000 fund_alchemy-1.0.8/fund_alchemy/custodian_table.py
--rw-rw-rw-   0        0        0     9330 2022-06-29 06:34:16.000000 fund_alchemy-1.0.8/fund_alchemy/figure.py
--rw-rw-rw-   0        0        0    24182 2022-03-03 12:34:30.000000 fund_alchemy-1.0.8/fund_alchemy/general_tools.py
--rw-rw-rw-   0        0        0    14423 2022-03-17 10:54:14.000000 fund_alchemy-1.0.8/fund_alchemy/mysql_tools.py
-drwxrwxrwx   0        0        0        0 2022-06-29 07:42:26.590000 fund_alchemy-1.0.8/fund_alchemy.egg-info/
--rw-rw-rw-   0        0        0      727 2022-06-29 07:42:28.000000 fund_alchemy-1.0.8/fund_alchemy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2022-06-29 07:42:28.000000 fund_alchemy-1.0.8/fund_alchemy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-29 07:42:28.000000 fund_alchemy-1.0.8/fund_alchemy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2022-06-29 07:42:28.000000 fund_alchemy-1.0.8/fund_alchemy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-06-29 07:42:28.000000 fund_alchemy-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      677 2022-06-29 07:42:16.000000 fund_alchemy-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-06-29 08:55:08.520000 fund_alchemy-1.0.9/
+-rw-rw-rw-   0        0        0     1079 2021-12-20 13:51:28.000000 fund_alchemy-1.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      727 2022-06-29 08:55:10.000000 fund_alchemy-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2022-06-29 07:12:50.000000 fund_alchemy-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-06-29 08:55:08.560000 fund_alchemy-1.0.9/fund_alchemy/
+-rw-rw-rw-   0        0        0       58 2022-06-29 02:57:12.000000 fund_alchemy-1.0.9/fund_alchemy/__init__.py
+-rw-rw-rw-   0        0        0   123318 2022-06-29 06:32:46.000000 fund_alchemy-1.0.9/fund_alchemy/config.py
+-rw-rw-rw-   0        0        0    18128 2022-06-29 08:54:32.000000 fund_alchemy-1.0.9/fund_alchemy/custodian_table.py
+-rw-rw-rw-   0        0        0     9343 2022-06-29 08:53:28.000000 fund_alchemy-1.0.9/fund_alchemy/figure.py
+-rw-rw-rw-   0        0        0    24182 2022-03-03 12:34:30.000000 fund_alchemy-1.0.9/fund_alchemy/general_tools.py
+-rw-rw-rw-   0        0        0    14423 2022-03-17 10:54:14.000000 fund_alchemy-1.0.9/fund_alchemy/mysql_tools.py
+drwxrwxrwx   0        0        0        0 2022-06-29 08:55:08.610000 fund_alchemy-1.0.9/fund_alchemy.egg-info/
+-rw-rw-rw-   0        0        0      727 2022-06-29 08:55:10.000000 fund_alchemy-1.0.9/fund_alchemy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2022-06-29 08:55:10.000000 fund_alchemy-1.0.9/fund_alchemy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-06-29 08:55:10.000000 fund_alchemy-1.0.9/fund_alchemy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2022-06-29 08:55:10.000000 fund_alchemy-1.0.9/fund_alchemy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-06-29 08:55:10.000000 fund_alchemy-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      677 2022-06-29 08:55:02.000000 fund_alchemy-1.0.9/setup.py
```

### Comparing `fund_alchemy-1.0.8/LICENSE.txt` & `fund_alchemy-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fund_alchemy-1.0.8/PKG-INFO` & `fund_alchemy-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fund_alchemy
-Version: 1.0.8
+Version: 1.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/ShoesFly/fund_alchemy
 Author: xxf
 Author-email: shoesflying@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fund_alchemy-1.0.8/fund_alchemy/config.py` & `fund_alchemy-1.0.9/fund_alchemy/config.py`

 * *Files identical despite different names*

### Comparing `fund_alchemy-1.0.8/fund_alchemy/custodian_table.py` & `fund_alchemy-1.0.9/fund_alchemy/custodian_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 import datetime as dt
 import pickle
-import fund_alchemy as f
-from config import custodian_config
+import fund_alchemy.general_tools as gt
+from fund_alchemy.config import custodian_config
 
 
 class standard_custodian_table:
     """将各托管估值表数据标准化.
 
     Parameters:
     ----------
@@ -157,15 +157,15 @@
 
         return data
 
     def mode2(self, filepath):
         xls = pd.read_excel(filepath, header=None)
         data = {}
         data['fund_name'] = xls.loc[0, 0].split("_")[1]
-        data['inner_date'] = f.find_date(xls.loc[0, 0])
+        data['inner_date'] = gt.find_date(xls.loc[0, 0])
 
         header1 = xls.loc[4, :]
         header2 = xls.loc[5, :]
         header = []
         for i in range(len(header1)):
             if header1[i] == header2[i]:
                 header.append(header1[i])
@@ -215,15 +215,15 @@
 
         return data
 
     def mode3(self, filepath):
         xls = pd.read_excel(filepath, header=None)
         data = {}
         data['fund_name'] = xls.loc[1, 0].split("___")[1]
-        data['inner_date'] = f.find_date(xls.loc[2, 7])
+        data['inner_date'] = gt.find_date(xls.loc[2, 7])
 
         header = xls.loc[3, :]
         last_idx = (xls.isnull().sum(axis=1) == xls.shape[1])\
             .loc[lambda x: x == True].index[0]  # noqa: E712
         df = xls[4:last_idx].copy().reset_index(drop=True)
         df.columns = header
         m = self.MODEs["mode3"]
@@ -264,15 +264,15 @@
 
         return data
 
     def mode4(self, filepath):
         xls = pd.read_excel(filepath, header=None)
         data = {}
         data['fund_name'] = xls.loc[1, 0].split("___")[1]
-        data['inner_date'] = f.find_date(xls.loc[2, 0])
+        data['inner_date'] = gt.find_date(xls.loc[2, 0])
 
         header = xls.loc[3, :]
 
         df = xls[4:].copy().reset_index(drop=True)
         last_idx = (xls.isnull().sum(axis=1) == xls.shape[1])\
             .loc[lambda x: x == True].index[0]  # noqa: E712
         df = xls[4:last_idx].copy().reset_index(drop=True)
@@ -317,15 +317,15 @@
 
         return data
 
     def mode5(self, filepath):
         xls = pd.read_excel(filepath, header=None)
         data = {}
         data['fund_name'] = xls.loc[2, 0].split("_")[-2]
-        data['inner_date'] = f.find_date(xls.loc[0, 0])
+        data['inner_date'] = gt.find_date(xls.loc[0, 0])
 
         header1 = xls.loc[4, :]
         header2 = xls.loc[5, :]
         header = []
         for i in range(len(header1)):
             if header1[i] == header2[i]:
                 header.append(header1[i])
@@ -375,15 +375,15 @@
 
         return data
 
     def mode6(self, filepath):
         xls = pd.read_excel(filepath, header=None)
         data = {}
         data['fund_name'] = xls.loc[2, 0].split("__")[-2]
-        data['inner_date'] = f.find_date(xls.loc[0, 0])
+        data['inner_date'] = gt.find_date(xls.loc[0, 0])
 
         header = xls.loc[4, :]
 
         last_idx = (xls[0].loc[lambda x: x == "证券投资合计"]).index[0] - 1
 
         df = xls[7:last_idx].copy().reset_index(drop=True)
         df.columns = header
```

### Comparing `fund_alchemy-1.0.8/fund_alchemy/figure.py` & `fund_alchemy-1.0.9/fund_alchemy/figure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib.gridspec import GridSpec
 import colorsys
 import fund_alchemy.general_tools as gt
-from config import matplotlib_custom_style
+from fund_alchemy.config import matplotlib_custom_style
 plt.style.use(matplotlib_custom_style)
 
 
 def comprehensive_analysis(series, rf=0.03):
     """计算基于净值序列的分析指标.
 
     parameters:
```

### Comparing `fund_alchemy-1.0.8/fund_alchemy/general_tools.py` & `fund_alchemy-1.0.9/fund_alchemy/general_tools.py`

 * *Files identical despite different names*

### Comparing `fund_alchemy-1.0.8/fund_alchemy/mysql_tools.py` & `fund_alchemy-1.0.9/fund_alchemy/mysql_tools.py`

 * *Files identical despite different names*

### Comparing `fund_alchemy-1.0.8/fund_alchemy.egg-info/PKG-INFO` & `fund_alchemy-1.0.9/fund_alchemy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fund-alchemy
-Version: 1.0.8
+Version: 1.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/ShoesFly/fund_alchemy
 Author: xxf
 Author-email: shoesflying@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fund_alchemy-1.0.8/setup.py` & `fund_alchemy-1.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fund_alchemy",
-    version="1.0.8",
+    version="1.0.9",
     author="xxf",
     author_email="shoesflying@163.com",
     descroption="A fund analysis platform.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ShoesFly/fund_alchemy",
     packages=setuptools.find_packages(),
```

