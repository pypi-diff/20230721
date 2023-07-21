# Comparing `tmp/AllyInvestPy-1.0.8.tar.gz` & `tmp/AllyInvestPy-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\AllyInvestPy-1.0.8.tar", last modified: Sat Mar 11 22:22:37 2023, max compression
+gzip compressed data, was "dist\AllyInvestPy-1.0.9.tar", last modified: Sat Mar 11 22:24:24 2023, max compression
```

## Comparing `AllyInvestPy-1.0.8.tar` & `AllyInvestPy-1.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-03-11 22:22:37.000000 AllyInvestPy-1.0.8/
-drwxrwxrwx   0        0        0        0 2023-03-11 22:22:37.000000 AllyInvestPy-1.0.8/AllyInvestPy.egg-info/
--rw-rw-rw-   0        0        0     3515 2023-03-11 22:22:37.000000 AllyInvestPy-1.0.8/AllyInvestPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      947 2023-03-11 22:22:37.000000 AllyInvestPy-1.0.8/AllyInvestPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-11 22:22:37.000000 AllyInvestPy-1.0.8/AllyInvestPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-03-11 22:22:37.000000 AllyInvestPy-1.0.8/AllyInvestPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-11 22:22:37.000000 AllyInvestPy-1.0.8/AllyInvestPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1077 2020-07-01 21:08:34.000000 AllyInvestPy-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     3515 2023-03-11 22:22:37.000000 AllyInvestPy-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3143 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-11 22:22:37.000000 AllyInvestPy-1.0.8/ally/
--rw-rw-rw-   0        0        0     9387 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.8/ally/URLs.py
--rw-rw-rw-   0        0        0      189 2021-08-18 19:31:09.000000 AllyInvestPy-1.0.8/ally/__init__.py
--rw-rw-rw-   0        0        0    22370 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.8/ally/ally.py
-drwxrwxrwx   0        0        0        0 2023-03-11 22:22:37.000000 AllyInvestPy-1.0.8/ally/requests/
--rw-rw-rw-   0        0        0      176 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.8/ally/requests/__init__.py
--rw-rw-rw-   0        0        0      415 2019-12-04 02:38:07.000000 AllyInvestPy-1.0.8/ally/requests/account_balances.py
--rw-rw-rw-   0        0        0      415 2019-12-11 16:20:36.000000 AllyInvestPy-1.0.8/ally/requests/account_holdings.py
--rw-rw-rw-   0        0        0      337 2019-12-04 02:39:53.000000 AllyInvestPy-1.0.8/ally/requests/accounts_balances.py
--rw-rw-rw-   0        0        0      522 2021-03-04 03:02:56.000000 AllyInvestPy-1.0.8/ally/requests/option_quote.py
--rw-rw-rw-   0        0        0      377 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.8/ally/requests/orders.py
--rw-rw-rw-   0        0        0     1142 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.8/ally/requests/post_order.py
--rw-rw-rw-   0        0        0     1205 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.8/ally/requests/post_order_preview.py
--rw-rw-rw-   0        0        0      625 2020-07-04 06:07:09.000000 AllyInvestPy-1.0.8/ally/requests/quotes.py
--rw-rw-rw-   0        0        0      148 2019-12-04 02:35:18.000000 AllyInvestPy-1.0.8/ally/requests/request.py
-drwxrwxrwx   0        0        0        0 2023-03-11 22:22:37.000000 AllyInvestPy-1.0.8/ally/responses/
--rw-rw-rw-   0        0        0      288 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.8/ally/responses/__init__.py
--rw-rw-rw-   0        0        0        0 2019-12-03 23:55:35.000000 AllyInvestPy-1.0.8/ally/responses/account.py
--rw-rw-rw-   0        0        0      317 2019-12-04 02:38:01.000000 AllyInvestPy-1.0.8/ally/responses/account_balances.py
--rw-rw-rw-   0        0        0      982 2019-12-17 23:44:34.000000 AllyInvestPy-1.0.8/ally/responses/account_holdings.py
--rw-rw-rw-   0        0        0        0 2019-12-03 23:55:35.000000 AllyInvestPy-1.0.8/ally/responses/accounts.py
--rw-rw-rw-   0        0        0      962 2019-12-04 03:01:13.000000 AllyInvestPy-1.0.8/ally/responses/accounts_balances.py
--rw-rw-rw-   0        0        0     2073 2023-03-11 22:20:46.000000 AllyInvestPy-1.0.8/ally/responses/holding.py
--rw-rw-rw-   0        0        0    11037 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.8/ally/responses/order.py
--rw-rw-rw-   0        0        0      973 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.8/ally/responses/orders.py
--rw-rw-rw-   0        0        0      518 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.8/ally/responses/post_order.py
--rw-rw-rw-   0        0        0      525 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.8/ally/responses/post_order_preview.py
--rw-rw-rw-   0        0        0     7150 2020-07-01 21:08:34.000000 AllyInvestPy-1.0.8/ally/responses/quote.py
--rw-rw-rw-   0        0        0      935 2020-07-01 21:08:34.000000 AllyInvestPy-1.0.8/ally/responses/quotes.py
--rw-rw-rw-   0        0        0      489 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.8/ally/responses/response.py
--rw-rw-rw-   0        0        0       42 2023-03-11 22:22:37.000000 AllyInvestPy-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      635 2023-03-11 22:22:29.000000 AllyInvestPy-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-11 22:24:24.000000 AllyInvestPy-1.0.9/
+drwxrwxrwx   0        0        0        0 2023-03-11 22:24:24.000000 AllyInvestPy-1.0.9/AllyInvestPy.egg-info/
+-rw-rw-rw-   0        0        0     3515 2023-03-11 22:24:24.000000 AllyInvestPy-1.0.9/AllyInvestPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      947 2023-03-11 22:24:24.000000 AllyInvestPy-1.0.9/AllyInvestPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-11 22:24:24.000000 AllyInvestPy-1.0.9/AllyInvestPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-03-11 22:24:24.000000 AllyInvestPy-1.0.9/AllyInvestPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-03-11 22:24:24.000000 AllyInvestPy-1.0.9/AllyInvestPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1077 2020-07-01 21:08:34.000000 AllyInvestPy-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3515 2023-03-11 22:24:24.000000 AllyInvestPy-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3143 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-11 22:24:24.000000 AllyInvestPy-1.0.9/ally/
+-rw-rw-rw-   0        0        0     9387 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.9/ally/URLs.py
+-rw-rw-rw-   0        0        0      189 2021-08-18 19:31:09.000000 AllyInvestPy-1.0.9/ally/__init__.py
+-rw-rw-rw-   0        0        0    22370 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.9/ally/ally.py
+drwxrwxrwx   0        0        0        0 2023-03-11 22:24:24.000000 AllyInvestPy-1.0.9/ally/requests/
+-rw-rw-rw-   0        0        0      176 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.9/ally/requests/__init__.py
+-rw-rw-rw-   0        0        0      415 2019-12-04 02:38:07.000000 AllyInvestPy-1.0.9/ally/requests/account_balances.py
+-rw-rw-rw-   0        0        0      415 2019-12-11 16:20:36.000000 AllyInvestPy-1.0.9/ally/requests/account_holdings.py
+-rw-rw-rw-   0        0        0      337 2019-12-04 02:39:53.000000 AllyInvestPy-1.0.9/ally/requests/accounts_balances.py
+-rw-rw-rw-   0        0        0      522 2021-03-04 03:02:56.000000 AllyInvestPy-1.0.9/ally/requests/option_quote.py
+-rw-rw-rw-   0        0        0      377 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.9/ally/requests/orders.py
+-rw-rw-rw-   0        0        0     1142 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.9/ally/requests/post_order.py
+-rw-rw-rw-   0        0        0     1205 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.9/ally/requests/post_order_preview.py
+-rw-rw-rw-   0        0        0      625 2020-07-04 06:07:09.000000 AllyInvestPy-1.0.9/ally/requests/quotes.py
+-rw-rw-rw-   0        0        0      148 2019-12-04 02:35:18.000000 AllyInvestPy-1.0.9/ally/requests/request.py
+drwxrwxrwx   0        0        0        0 2023-03-11 22:24:24.000000 AllyInvestPy-1.0.9/ally/responses/
+-rw-rw-rw-   0        0        0      288 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.9/ally/responses/__init__.py
+-rw-rw-rw-   0        0        0        0 2019-12-03 23:55:35.000000 AllyInvestPy-1.0.9/ally/responses/account.py
+-rw-rw-rw-   0        0        0      317 2019-12-04 02:38:01.000000 AllyInvestPy-1.0.9/ally/responses/account_balances.py
+-rw-rw-rw-   0        0        0      982 2019-12-17 23:44:34.000000 AllyInvestPy-1.0.9/ally/responses/account_holdings.py
+-rw-rw-rw-   0        0        0        0 2019-12-03 23:55:35.000000 AllyInvestPy-1.0.9/ally/responses/accounts.py
+-rw-rw-rw-   0        0        0      962 2019-12-04 03:01:13.000000 AllyInvestPy-1.0.9/ally/responses/accounts_balances.py
+-rw-rw-rw-   0        0        0     2245 2023-03-11 22:24:14.000000 AllyInvestPy-1.0.9/ally/responses/holding.py
+-rw-rw-rw-   0        0        0    11037 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.9/ally/responses/order.py
+-rw-rw-rw-   0        0        0      973 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.9/ally/responses/orders.py
+-rw-rw-rw-   0        0        0      518 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.9/ally/responses/post_order.py
+-rw-rw-rw-   0        0        0      525 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.9/ally/responses/post_order_preview.py
+-rw-rw-rw-   0        0        0     7150 2020-07-01 21:08:34.000000 AllyInvestPy-1.0.9/ally/responses/quote.py
+-rw-rw-rw-   0        0        0      935 2020-07-01 21:08:34.000000 AllyInvestPy-1.0.9/ally/responses/quotes.py
+-rw-rw-rw-   0        0        0      489 2023-03-11 22:01:18.000000 AllyInvestPy-1.0.9/ally/responses/response.py
+-rw-rw-rw-   0        0        0       42 2023-03-11 22:24:24.000000 AllyInvestPy-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      635 2023-03-11 22:24:21.000000 AllyInvestPy-1.0.9/setup.py
```

### Comparing `AllyInvestPy-1.0.8/AllyInvestPy.egg-info/PKG-INFO` & `AllyInvestPy-1.0.9/AllyInvestPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AllyInvestPy
-Version: 1.0.8
+Version: 1.0.9
 Summary: A blackbox Ally Invest/TradeKing API interface for application developers.
 Home-page: https://github.com/anthonymorast/AllyInvest.py
 Author: Anthony Morast
 Author-email: anthony.a.morast@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `AllyInvestPy-1.0.8/AllyInvestPy.egg-info/SOURCES.txt` & `AllyInvestPy-1.0.9/AllyInvestPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AllyInvestPy-1.0.8/LICENSE` & `AllyInvestPy-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `AllyInvestPy-1.0.8/PKG-INFO` & `AllyInvestPy-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AllyInvestPy
-Version: 1.0.8
+Version: 1.0.9
 Summary: A blackbox Ally Invest/TradeKing API interface for application developers.
 Home-page: https://github.com/anthonymorast/AllyInvest.py
 Author: Anthony Morast
 Author-email: anthony.a.morast@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `AllyInvestPy-1.0.8/README.md` & `AllyInvestPy-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `AllyInvestPy-1.0.8/ally/URLs.py` & `AllyInvestPy-1.0.9/ally/URLs.py`

 * *Files identical despite different names*

### Comparing `AllyInvestPy-1.0.8/ally/ally.py` & `AllyInvestPy-1.0.9/ally/ally.py`

 * *Files identical despite different names*

### Comparing `AllyInvestPy-1.0.8/ally/requests/option_quote.py` & `AllyInvestPy-1.0.9/ally/requests/option_quote.py`

 * *Files identical despite different names*

### Comparing `AllyInvestPy-1.0.8/ally/requests/post_order.py` & `AllyInvestPy-1.0.9/ally/requests/post_order.py`

 * *Files identical despite different names*

### Comparing `AllyInvestPy-1.0.8/ally/requests/post_order_preview.py` & `AllyInvestPy-1.0.9/ally/requests/post_order_preview.py`

 * *Files identical despite different names*

### Comparing `AllyInvestPy-1.0.8/ally/requests/quotes.py` & `AllyInvestPy-1.0.9/ally/requests/quotes.py`

 * *Files identical despite different names*

### Comparing `AllyInvestPy-1.0.8/ally/responses/account_holdings.py` & `AllyInvestPy-1.0.9/ally/responses/account_holdings.py`

 * *Files identical despite different names*

### Comparing `AllyInvestPy-1.0.8/ally/responses/accounts_balances.py` & `AllyInvestPy-1.0.9/ally/responses/accounts_balances.py`

 * *Files identical despite different names*

### Comparing `AllyInvestPy-1.0.8/ally/responses/holding.py` & `AllyInvestPy-1.0.9/ally/responses/holding.py`

 * *Files 24% similar despite different names*

```diff
@@ -27,16 +27,18 @@
         	self.gainloss = json['gainloss']
         if 'lastprice' in json['quote']:
         	self.lastprice = json['quote']['lastprice']
         if 'marketvalue' in json:
         	self.marketvalue = json['marketvalue']
         if 'marketvaluechange' in json:
         	self.marketvaluechange = json['marketvaluechange']
-        if 'matdt' in json:
-        	self.matdt = json['matdt']
+        if 'matdt' in json['instrument']:   # simplex options use matdt
+        	self.matdt = json['instrument']['matdt']
+        if 'mat' in json['instrument']:     # multilegs use mat
+        	self.matdt = json['instrument']['mat']
         if 'mmy' in json:
         	self.mmy = json['mmy']
         if 'mult' in json:
         	self.mult = json['mult']
         if 'price' in json:
         	self.price = json['price']
         if 'purchaseprice' in json:
```

### Comparing `AllyInvestPy-1.0.8/ally/responses/order.py` & `AllyInvestPy-1.0.9/ally/responses/order.py`

 * *Files identical despite different names*

### Comparing `AllyInvestPy-1.0.8/ally/responses/orders.py` & `AllyInvestPy-1.0.9/ally/responses/orders.py`

 * *Files identical despite different names*

### Comparing `AllyInvestPy-1.0.8/ally/responses/post_order.py` & `AllyInvestPy-1.0.9/ally/responses/post_order.py`

 * *Files identical despite different names*

### Comparing `AllyInvestPy-1.0.8/ally/responses/post_order_preview.py` & `AllyInvestPy-1.0.9/ally/responses/post_order_preview.py`

 * *Files identical despite different names*

### Comparing `AllyInvestPy-1.0.8/ally/responses/quote.py` & `AllyInvestPy-1.0.9/ally/responses/quote.py`

 * *Files identical despite different names*

### Comparing `AllyInvestPy-1.0.8/ally/responses/quotes.py` & `AllyInvestPy-1.0.9/ally/responses/quotes.py`

 * *Files identical despite different names*

### Comparing `AllyInvestPy-1.0.8/setup.py` & `AllyInvestPy-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='AllyInvestPy',
-    version='1.0.8',
+    version='1.0.9',
     description='A blackbox Ally Invest/TradeKing API interface for application developers.',
     url='https://github.com/anthonymorast/AllyInvest.py',
     author='Anthony Morast',
     author_email='anthony.a.morast@gmail.com',
     license='MIT',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

