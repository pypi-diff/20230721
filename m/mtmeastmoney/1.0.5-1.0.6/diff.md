# Comparing `tmp/mtmeastmoney-1.0.5.tar.gz` & `tmp/mtmeastmoney-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtmeastmoney-1.0.5.tar", last modified: Wed Jul 19 13:14:39 2023, max compression
+gzip compressed data, was "mtmeastmoney-1.0.6.tar", last modified: Fri Jul 21 07:17:32 2023, max compression
```

## Comparing `mtmeastmoney-1.0.5.tar` & `mtmeastmoney-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 13:14:39.861837 mtmeastmoney-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-07-19 13:14:28.000000 mtmeastmoney-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      631 2023-07-19 13:14:39.861837 mtmeastmoney-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-19 13:14:28.000000 mtmeastmoney-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-19 13:14:39.861837 mtmeastmoney-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2127 2023-07-19 13:14:28.000000 mtmeastmoney-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 13:14:39.857837 mtmeastmoney-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 13:14:39.861837 mtmeastmoney-1.0.5/src/mtmeastmoney/
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-07-19 13:14:28.000000 mtmeastmoney-1.0.5/src/mtmeastmoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-19 13:14:28.000000 mtmeastmoney-1.0.5/src/mtmeastmoney/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     2314 2023-07-19 13:14:28.000000 mtmeastmoney-1.0.5/src/mtmeastmoney/dbaccount.py
--rw-r--r--   0 runner    (1001) docker     (122)     8454 2023-07-19 13:14:28.000000 mtmeastmoney-1.0.5/src/mtmeastmoney/eastmoney.py
--rw-r--r--   0 runner    (1001) docker     (122)     3279 2023-07-19 13:14:28.000000 mtmeastmoney-1.0.5/src/mtmeastmoney/jointquant.py
--rw-r--r--   0 runner    (1001) docker     (122)      458 2023-07-19 13:14:28.000000 mtmeastmoney-1.0.5/src/mtmeastmoney/ocr.py
--rw-r--r--   0 runner    (1001) docker     (122)     2564 2023-07-19 13:14:28.000000 mtmeastmoney-1.0.5/src/mtmeastmoney/tiantianfund.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 13:14:39.861837 mtmeastmoney-1.0.5/src/mtmeastmoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      631 2023-07-19 13:14:39.000000 mtmeastmoney-1.0.5/src/mtmeastmoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      468 2023-07-19 13:14:39.000000 mtmeastmoney-1.0.5/src/mtmeastmoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 13:14:39.000000 mtmeastmoney-1.0.5/src/mtmeastmoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 13:14:39.000000 mtmeastmoney-1.0.5/src/mtmeastmoney.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-19 13:14:39.000000 mtmeastmoney-1.0.5/src/mtmeastmoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-19 13:14:39.000000 mtmeastmoney-1.0.5/src/mtmeastmoney.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 07:17:32.858523 mtmeastmoney-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-07-21 07:17:24.000000 mtmeastmoney-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      631 2023-07-21 07:17:32.858523 mtmeastmoney-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-21 07:17:24.000000 mtmeastmoney-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-21 07:17:32.858523 mtmeastmoney-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2127 2023-07-21 07:17:24.000000 mtmeastmoney-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 07:17:32.854523 mtmeastmoney-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 07:17:32.858523 mtmeastmoney-1.0.6/src/mtmeastmoney/
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-07-21 07:17:24.000000 mtmeastmoney-1.0.6/src/mtmeastmoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-21 07:17:24.000000 mtmeastmoney-1.0.6/src/mtmeastmoney/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2314 2023-07-21 07:17:24.000000 mtmeastmoney-1.0.6/src/mtmeastmoney/dbaccount.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9584 2023-07-21 07:17:24.000000 mtmeastmoney-1.0.6/src/mtmeastmoney/eastmoney.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3279 2023-07-21 07:17:24.000000 mtmeastmoney-1.0.6/src/mtmeastmoney/jointquant.py
+-rw-r--r--   0 runner    (1001) docker     (122)      458 2023-07-21 07:17:24.000000 mtmeastmoney-1.0.6/src/mtmeastmoney/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2564 2023-07-21 07:17:24.000000 mtmeastmoney-1.0.6/src/mtmeastmoney/tiantianfund.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 07:17:32.858523 mtmeastmoney-1.0.6/src/mtmeastmoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      631 2023-07-21 07:17:32.000000 mtmeastmoney-1.0.6/src/mtmeastmoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      468 2023-07-21 07:17:32.000000 mtmeastmoney-1.0.6/src/mtmeastmoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 07:17:32.000000 mtmeastmoney-1.0.6/src/mtmeastmoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 07:17:32.000000 mtmeastmoney-1.0.6/src/mtmeastmoney.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-21 07:17:32.000000 mtmeastmoney-1.0.6/src/mtmeastmoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-21 07:17:32.000000 mtmeastmoney-1.0.6/src/mtmeastmoney.egg-info/top_level.txt
```

### Comparing `mtmeastmoney-1.0.5/LICENSE` & `mtmeastmoney-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mtmeastmoney-1.0.5/PKG-INFO` & `mtmeastmoney-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmeastmoney
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Personal Eastmoney Library
 Home-page: https://github.com/imutum/imutum_eastmoney_library
 Author: imutum
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Developers
```

### Comparing `mtmeastmoney-1.0.5/setup.py` & `mtmeastmoney-1.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os, shutil, sys, glob
 
 package_name = 'imutum_eastmoney_library'
 abbreviation_name = "mtmeastmoney"
 description = "A Personal Eastmoney Library"
-version = "1.0.5"
+version = "1.0.6"
 
 
 def check_requires(requires: list):
     pip_file = "pip.exe" if "win" in sys.platform else "pip"
     pip_paths = [
         os.path.join(os.path.dirname(sys.executable), "Scripts", pip_file),
         os.path.join(os.path.dirname(sys.executable), pip_file),
```

### Comparing `mtmeastmoney-1.0.5/src/mtmeastmoney/common.py` & `mtmeastmoney-1.0.6/src/mtmeastmoney/common.py`

 * *Files identical despite different names*

### Comparing `mtmeastmoney-1.0.5/src/mtmeastmoney/dbaccount.py` & `mtmeastmoney-1.0.6/src/mtmeastmoney/dbaccount.py`

 * *Files identical despite different names*

### Comparing `mtmeastmoney-1.0.5/src/mtmeastmoney/eastmoney.py` & `mtmeastmoney-1.0.6/src/mtmeastmoney/eastmoney.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,14 +161,53 @@
         resp = self.session.get(url)
         result = re.search(today_str, resp.text)
         if result is not None:
             return True
         else:
             return False
 
+    def order_(self, stock_code:str, amount:int, trade_type:str, price:float=None) -> dict: 
+        """下单固定的数量
+
+        Parameters
+        ----------
+        stock_code : str
+            股票代码
+        amount : int
+            股票交易数量
+        trade_type : str
+            股票交易类型\  
+
+        price : float, optional
+            股票价格，限价需要, by default None
+
+        交易类型可选: \ 
+        0i 最优五档剩余撤销，卖出; \ 
+        0d 最优五档剩余撤销，买入; \ 
+        S 限价委托卖出; \ 
+        B 限价委托买入; \ 
+
+        Returns
+        -------
+        dict
+            委托发送信息
+        """
+
+        url = self.url_add_validate_key("/Trade/SubmitTradeV2")
+        if price is None:
+            price = self.query_stock_current_info(stock_code)["最新价"]
+        data = {
+            "stockCode": stock_code,
+            "price": "{:.2f}".format(price/100),
+            "amount": int(amount),
+            "tradeType": trade_type,
+        }
+        message = post_order(self.session, url, data)
+        return message
+
     def scripts_buy_today_convertible_bonds(self):
         json_data = self.query_market_convertible_bonds_list()
         json_data = [bond for bond in json_data if bond["PURCHASEDATE"] == datetime.now().strftime("%Y%m%d")]
         if not len(json_data):
             return "今日无可买可转债"
         data = [{
             "StockCode": bond["SUBCODE"],
```

### Comparing `mtmeastmoney-1.0.5/src/mtmeastmoney/jointquant.py` & `mtmeastmoney-1.0.6/src/mtmeastmoney/jointquant.py`

 * *Files identical despite different names*

### Comparing `mtmeastmoney-1.0.5/src/mtmeastmoney/tiantianfund.py` & `mtmeastmoney-1.0.6/src/mtmeastmoney/tiantianfund.py`

 * *Files identical despite different names*

### Comparing `mtmeastmoney-1.0.5/src/mtmeastmoney.egg-info/PKG-INFO` & `mtmeastmoney-1.0.6/src/mtmeastmoney.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmeastmoney
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Personal Eastmoney Library
 Home-page: https://github.com/imutum/imutum_eastmoney_library
 Author: imutum
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Developers
```

