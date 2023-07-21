# Comparing `tmp/asyncoinpayments-0.0.7a0.tar.gz` & `tmp/asyncoinpayments-0.0.8a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncoinpayments-0.0.7a0.tar", last modified: Fri Jul 21 14:30:58 2023, max compression
+gzip compressed data, was "asyncoinpayments-0.0.8a0.tar", last modified: Fri Jul 21 14:53:02 2023, max compression
```

## Comparing `asyncoinpayments-0.0.7a0.tar` & `asyncoinpayments-0.0.8a0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-21 14:30:58.836369 asyncoinpayments-0.0.7a0/
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       58 2023-07-21 09:11:52.000000 asyncoinpayments-0.0.7a0/.gitignore
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)    11328 2023-07-08 21:40:35.000000 asyncoinpayments-0.0.7a0/LICENSE.txt
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)     1044 2023-07-21 14:30:58.836369 asyncoinpayments-0.0.7a0/PKG-INFO
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      432 2023-07-08 20:18:04.000000 asyncoinpayments-0.0.7a0/README.md
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      842 2023-07-21 14:30:49.000000 asyncoinpayments-0.0.7a0/pyproject.toml
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       38 2023-07-21 14:30:58.836369 asyncoinpayments-0.0.7a0/setup.cfg
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       68 2023-07-20 21:25:48.000000 asyncoinpayments-0.0.7a0/setup.py
-drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-21 14:30:58.832369 asyncoinpayments-0.0.7a0/src/
-drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-21 14:30:58.832369 asyncoinpayments-0.0.7a0/src/asyncoinpayments/
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       91 2023-07-21 09:53:35.000000 asyncoinpayments-0.0.7a0/src/asyncoinpayments/__init__.py
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)    21178 2023-07-21 14:29:55.000000 asyncoinpayments-0.0.7a0/src/asyncoinpayments/coinpayments.py
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      155 2023-07-08 15:55:02.000000 asyncoinpayments-0.0.7a0/src/asyncoinpayments/errors.py
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      643 2023-07-21 09:47:09.000000 asyncoinpayments-0.0.7a0/src/asyncoinpayments/utils.py
-drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-21 14:30:58.836369 asyncoinpayments-0.0.7a0/src/asyncoinpayments.egg-info/
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)     1044 2023-07-21 14:30:58.000000 asyncoinpayments-0.0.7a0/src/asyncoinpayments.egg-info/PKG-INFO
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      406 2023-07-21 14:30:58.000000 asyncoinpayments-0.0.7a0/src/asyncoinpayments.egg-info/SOURCES.txt
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)        1 2023-07-21 14:30:58.000000 asyncoinpayments-0.0.7a0/src/asyncoinpayments.egg-info/dependency_links.txt
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       17 2023-07-21 14:30:58.000000 asyncoinpayments-0.0.7a0/src/asyncoinpayments.egg-info/requires.txt
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       17 2023-07-21 14:30:58.000000 asyncoinpayments-0.0.7a0/src/asyncoinpayments.egg-info/top_level.txt
+drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-21 14:53:02.087797 asyncoinpayments-0.0.8a0/
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       58 2023-07-21 09:11:52.000000 asyncoinpayments-0.0.8a0/.gitignore
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)    11328 2023-07-08 21:40:35.000000 asyncoinpayments-0.0.8a0/LICENSE.txt
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)     1044 2023-07-21 14:53:02.087797 asyncoinpayments-0.0.8a0/PKG-INFO
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      432 2023-07-08 20:18:04.000000 asyncoinpayments-0.0.8a0/README.md
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      842 2023-07-21 14:38:12.000000 asyncoinpayments-0.0.8a0/pyproject.toml
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       38 2023-07-21 14:53:02.087797 asyncoinpayments-0.0.8a0/setup.cfg
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       68 2023-07-20 21:25:48.000000 asyncoinpayments-0.0.8a0/setup.py
+drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-21 14:53:02.087797 asyncoinpayments-0.0.8a0/src/
+drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-21 14:53:02.087797 asyncoinpayments-0.0.8a0/src/asyncoinpayments/
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       91 2023-07-21 09:53:35.000000 asyncoinpayments-0.0.8a0/src/asyncoinpayments/__init__.py
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)    21268 2023-07-21 14:50:04.000000 asyncoinpayments-0.0.8a0/src/asyncoinpayments/coinpayments.py
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      155 2023-07-08 15:55:02.000000 asyncoinpayments-0.0.8a0/src/asyncoinpayments/errors.py
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      643 2023-07-21 09:47:09.000000 asyncoinpayments-0.0.8a0/src/asyncoinpayments/utils.py
+drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-21 14:53:02.087797 asyncoinpayments-0.0.8a0/src/asyncoinpayments.egg-info/
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)     1044 2023-07-21 14:53:02.000000 asyncoinpayments-0.0.8a0/src/asyncoinpayments.egg-info/PKG-INFO
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      406 2023-07-21 14:53:02.000000 asyncoinpayments-0.0.8a0/src/asyncoinpayments.egg-info/SOURCES.txt
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)        1 2023-07-21 14:53:02.000000 asyncoinpayments-0.0.8a0/src/asyncoinpayments.egg-info/dependency_links.txt
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       17 2023-07-21 14:53:02.000000 asyncoinpayments-0.0.8a0/src/asyncoinpayments.egg-info/requires.txt
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       17 2023-07-21 14:53:02.000000 asyncoinpayments-0.0.8a0/src/asyncoinpayments.egg-info/top_level.txt
```

### Comparing `asyncoinpayments-0.0.7a0/LICENSE.txt` & `asyncoinpayments-0.0.8a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `asyncoinpayments-0.0.7a0/PKG-INFO` & `asyncoinpayments-0.0.8a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncoinpayments
-Version: 0.0.7a0
+Version: 0.0.8a0
 Summary: Python Asynchronous Wrapper of the CoinPayments API
 Author-email: flalugli <flalugli.dev@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/flalugli/asyncoinpayments
 Keywords: python,crypto,cryptocurrency,payment gateway,async,aiohttp
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `asyncoinpayments-0.0.7a0/pyproject.toml` & `asyncoinpayments-0.0.8a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asyncoinpayments"
-version = "0.0.7a"
+version = "0.0.8a"
 description = "Python Asynchronous Wrapper of the CoinPayments API"
 authors = [
   { name="flalugli", email="flalugli.dev@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ['python', 'crypto', 'cryptocurrency', 'payment gateway', 'async', 'aiohttp']
```

### Comparing `asyncoinpayments-0.0.7a0/src/asyncoinpayments/coinpayments.py` & `asyncoinpayments-0.0.8a0/src/asyncoinpayments/coinpayments.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
             'currency' : currency,
             'merchant' : merchant_id,
             'auto_confirm' : auto_confirm
         }
 
         return await self.api_call(cmd, **necessary_params, **params)
 
-    async def create_withdrawal(self, amount:float, receive_currency:str, base_currency:str = None, address:str = None, ipn_url: str = None, auto_confirm:bool = False, **params) -> Union[JsonResponse, str]:
+    async def create_withdrawal(self, amount:float, receive_currency:str, base_currency:str = "USD", address:str = None, ipn_url: str = None, auto_confirm:bool = False, **params) -> Union[JsonResponse, str]:
         """
         create a withdrawal and send or transfer your funds to others
 
         Parameters
         ----------
         amount : float
             amount of base_currency to send
@@ -651,18 +651,19 @@
         Returns
         -------
         dict
             A dictionary containing the merchant's coin balances converted in the base currency
         """
 
         new_balances = {}
-
-        balances = self.result(await self.balances(all_coins = all_coins))
+        balances_api_response = await self.balances(all_coins = all_coins)
+        balances = balances_api_response.result
         #we call this function once and cache the result
-        rates = self.result(await self.rates(only_accepted = only_accepted))
+        rates_api_response = await self.rates(only_accepted = only_accepted)
+        rates = rates_api_response.result
 
         for coin in rates:
             
             try:
                 exchangerate = await self.conversion_fiat(coin1 = coin, base_currency = base_currency, from_data = rates)
                 coin_balance = float(balances[coin]['balancef'])
             except KeyError:
```

### Comparing `asyncoinpayments-0.0.7a0/src/asyncoinpayments/utils.py` & `asyncoinpayments-0.0.8a0/src/asyncoinpayments/utils.py`

 * *Files identical despite different names*

### Comparing `asyncoinpayments-0.0.7a0/src/asyncoinpayments.egg-info/PKG-INFO` & `asyncoinpayments-0.0.8a0/src/asyncoinpayments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncoinpayments
-Version: 0.0.7a0
+Version: 0.0.8a0
 Summary: Python Asynchronous Wrapper of the CoinPayments API
 Author-email: flalugli <flalugli.dev@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/flalugli/asyncoinpayments
 Keywords: python,crypto,cryptocurrency,payment gateway,async,aiohttp
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

