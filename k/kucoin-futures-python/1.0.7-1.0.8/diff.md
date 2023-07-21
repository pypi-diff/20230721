# Comparing `tmp/kucoin-futures-python-1.0.7.tar.gz` & `tmp/kucoin-futures-python-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kucoin-futures-python-1.0.7.tar", last modified: Tue Jul  4 02:25:17 2023, max compression
+gzip compressed data, was "kucoin-futures-python-1.0.8.tar", last modified: Fri Jul 21 06:51:19 2023, max compression
```

## Comparing `kucoin-futures-python-1.0.7.tar` & `kucoin-futures-python-1.0.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 bernardong   (501) staff       (20)        0 2023-07-04 02:25:17.948233 kucoin-futures-python-1.0.7/
--rw-rw-r--   0 bernardong   (501) staff       (20)     1063 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/LICENSE
--rw-r--r--   0 bernardong   (501) staff       (20)      392 2023-07-04 02:25:17.947957 kucoin-futures-python-1.0.7/PKG-INFO
--rw-rw-r--   0 bernardong   (501) staff       (20)     3732 2023-07-04 02:24:30.000000 kucoin-futures-python-1.0.7/README.rst
-drwxr-xr-x   0 bernardong   (501) staff       (20)        0 2023-07-04 02:25:17.931737 kucoin-futures-python-1.0.7/kucoin_futures/
--rw-rw-r--   0 bernardong   (501) staff       (20)        0 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/__init__.py
-drwxr-xr-x   0 bernardong   (501) staff       (20)        0 2023-07-04 02:25:17.932503 kucoin-futures-python-1.0.7/kucoin_futures/base_request/
--rw-rw-r--   0 bernardong   (501) staff       (20)        0 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/base_request/__init__.py
--rw-rw-r--   0 bernardong   (501) staff       (20)     4299 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/base_request/base_request.py
--rw-rw-r--   0 bernardong   (501) staff       (20)      350 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/client.py
-drwxr-xr-x   0 bernardong   (501) staff       (20)        0 2023-07-04 02:25:17.933275 kucoin-futures-python-1.0.7/kucoin_futures/marke_data/
--rw-rw-r--   0 bernardong   (501) staff       (20)        0 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/marke_data/__init__.py
--rw-rw-r--   0 bernardong   (501) staff       (20)    22513 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/marke_data/market_data.py
-drwxr-xr-x   0 bernardong   (501) staff       (20)        0 2023-07-04 02:25:17.934050 kucoin-futures-python-1.0.7/kucoin_futures/trade/
--rw-rw-r--   0 bernardong   (501) staff       (20)        0 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/trade/__init__.py
--rw-rw-r--   0 bernardong   (501) staff       (20)    28743 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/trade/trade.py
-drwxr-xr-x   0 bernardong   (501) staff       (20)        0 2023-07-04 02:25:17.934894 kucoin-futures-python-1.0.7/kucoin_futures/user/
--rw-rw-r--   0 bernardong   (501) staff       (20)        0 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/user/__init__.py
--rw-rw-r--   0 bernardong   (501) staff       (20)    15637 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/user/user.py
-drwxr-xr-x   0 bernardong   (501) staff       (20)        0 2023-07-04 02:25:17.935616 kucoin-futures-python-1.0.7/kucoin_futures/websocket/
--rw-rw-r--   0 bernardong   (501) staff       (20)        0 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/websocket/__init__.py
--rw-rw-r--   0 bernardong   (501) staff       (20)     5633 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/websocket/websocket.py
--rw-rw-r--   0 bernardong   (501) staff       (20)     1620 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/ws_client.py
-drwxr-xr-x   0 bernardong   (501) staff       (20)        0 2023-07-04 02:25:17.936392 kucoin-futures-python-1.0.7/kucoin_futures/ws_token/
--rw-rw-r--   0 bernardong   (501) staff       (20)        0 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/ws_token/__init__.py
--rw-rw-r--   0 bernardong   (501) staff       (20)      480 2023-05-25 06:35:11.000000 kucoin-futures-python-1.0.7/kucoin_futures/ws_token/token.py
-drwxr-xr-x   0 bernardong   (501) staff       (20)        0 2023-07-04 02:25:17.947456 kucoin-futures-python-1.0.7/kucoin_futures_python.egg-info/
--rw-r--r--   0 bernardong   (501) staff       (20)      392 2023-07-04 02:25:17.000000 kucoin-futures-python-1.0.7/kucoin_futures_python.egg-info/PKG-INFO
--rw-r--r--   0 bernardong   (501) staff       (20)      761 2023-07-04 02:25:17.000000 kucoin-futures-python-1.0.7/kucoin_futures_python.egg-info/SOURCES.txt
--rw-r--r--   0 bernardong   (501) staff       (20)        1 2023-07-04 02:25:17.000000 kucoin-futures-python-1.0.7/kucoin_futures_python.egg-info/dependency_links.txt
--rw-r--r--   0 bernardong   (501) staff       (20)       20 2023-07-04 02:25:17.000000 kucoin-futures-python-1.0.7/kucoin_futures_python.egg-info/requires.txt
--rw-r--r--   0 bernardong   (501) staff       (20)      159 2023-07-04 02:25:17.000000 kucoin-futures-python-1.0.7/kucoin_futures_python.egg-info/top_level.txt
--rw-r--r--   0 bernardong   (501) staff       (20)       38 2023-07-04 02:25:17.948288 kucoin-futures-python-1.0.7/setup.cfg
--rw-rw-r--   0 bernardong   (501) staff       (20)      751 2023-07-04 02:24:03.000000 kucoin-futures-python-1.0.7/setup.py
+drwxr-xr-x   0 joysu      (501) staff       (20)        0 2023-07-21 06:51:19.378602 kucoin-futures-python-1.0.8/
+-rw-r--r--   0 joysu      (501) staff       (20)     1063 2023-07-17 09:50:20.000000 kucoin-futures-python-1.0.8/LICENSE
+-rw-r--r--   0 joysu      (501) staff       (20)      392 2023-07-21 06:51:19.378271 kucoin-futures-python-1.0.8/PKG-INFO
+-rw-r--r--   0 joysu      (501) staff       (20)     3732 2023-07-19 08:08:03.000000 kucoin-futures-python-1.0.8/README.rst
+drwxr-xr-x   0 joysu      (501) staff       (20)        0 2023-07-21 06:51:19.353959 kucoin-futures-python-1.0.8/kucoin_futures/
+-rw-r--r--   0 joysu      (501) staff       (20)        0 2023-07-17 09:50:20.000000 kucoin-futures-python-1.0.8/kucoin_futures/__init__.py
+drwxr-xr-x   0 joysu      (501) staff       (20)        0 2023-07-21 06:51:19.354796 kucoin-futures-python-1.0.8/kucoin_futures/base_request/
+-rw-r--r--   0 joysu      (501) staff       (20)        0 2023-07-17 09:50:20.000000 kucoin-futures-python-1.0.8/kucoin_futures/base_request/__init__.py
+-rw-r--r--   0 joysu      (501) staff       (20)     4299 2023-07-17 09:50:20.000000 kucoin-futures-python-1.0.8/kucoin_futures/base_request/base_request.py
+-rw-r--r--   0 joysu      (501) staff       (20)      350 2023-07-17 09:50:20.000000 kucoin-futures-python-1.0.8/kucoin_futures/client.py
+drwxr-xr-x   0 joysu      (501) staff       (20)        0 2023-07-21 06:51:19.360012 kucoin-futures-python-1.0.8/kucoin_futures/marke_data/
+-rw-r--r--   0 joysu      (501) staff       (20)        0 2023-07-17 09:50:20.000000 kucoin-futures-python-1.0.8/kucoin_futures/marke_data/__init__.py
+-rw-r--r--   0 joysu      (501) staff       (20)    22513 2023-07-17 09:50:20.000000 kucoin-futures-python-1.0.8/kucoin_futures/marke_data/market_data.py
+drwxr-xr-x   0 joysu      (501) staff       (20)        0 2023-07-21 06:51:19.364220 kucoin-futures-python-1.0.8/kucoin_futures/trade/
+-rw-r--r--   0 joysu      (501) staff       (20)        0 2023-07-17 09:50:20.000000 kucoin-futures-python-1.0.8/kucoin_futures/trade/__init__.py
+-rw-r--r--   0 joysu      (501) staff       (20)    28743 2023-07-17 09:50:20.000000 kucoin-futures-python-1.0.8/kucoin_futures/trade/trade.py
+drwxr-xr-x   0 joysu      (501) staff       (20)        0 2023-07-21 06:51:19.365159 kucoin-futures-python-1.0.8/kucoin_futures/user/
+-rw-r--r--   0 joysu      (501) staff       (20)        0 2023-07-17 09:50:20.000000 kucoin-futures-python-1.0.8/kucoin_futures/user/__init__.py
+-rw-r--r--   0 joysu      (501) staff       (20)    17593 2023-07-19 02:36:25.000000 kucoin-futures-python-1.0.8/kucoin_futures/user/user.py
+drwxr-xr-x   0 joysu      (501) staff       (20)        0 2023-07-21 06:51:19.369013 kucoin-futures-python-1.0.8/kucoin_futures/websocket/
+-rw-r--r--   0 joysu      (501) staff       (20)        0 2023-07-17 09:50:20.000000 kucoin-futures-python-1.0.8/kucoin_futures/websocket/__init__.py
+-rw-r--r--   0 joysu      (501) staff       (20)     5633 2023-07-17 09:50:20.000000 kucoin-futures-python-1.0.8/kucoin_futures/websocket/websocket.py
+-rw-r--r--   0 joysu      (501) staff       (20)     1620 2023-07-17 09:50:20.000000 kucoin-futures-python-1.0.8/kucoin_futures/ws_client.py
+drwxr-xr-x   0 joysu      (501) staff       (20)        0 2023-07-21 06:51:19.371653 kucoin-futures-python-1.0.8/kucoin_futures/ws_token/
+-rw-r--r--   0 joysu      (501) staff       (20)        0 2023-07-17 09:50:20.000000 kucoin-futures-python-1.0.8/kucoin_futures/ws_token/__init__.py
+-rw-r--r--   0 joysu      (501) staff       (20)      480 2023-07-17 09:50:20.000000 kucoin-futures-python-1.0.8/kucoin_futures/ws_token/token.py
+drwxr-xr-x   0 joysu      (501) staff       (20)        0 2023-07-21 06:51:19.377673 kucoin-futures-python-1.0.8/kucoin_futures_python.egg-info/
+-rw-r--r--   0 joysu      (501) staff       (20)      392 2023-07-21 06:51:19.000000 kucoin-futures-python-1.0.8/kucoin_futures_python.egg-info/PKG-INFO
+-rw-r--r--   0 joysu      (501) staff       (20)      761 2023-07-21 06:51:19.000000 kucoin-futures-python-1.0.8/kucoin_futures_python.egg-info/SOURCES.txt
+-rw-r--r--   0 joysu      (501) staff       (20)        1 2023-07-21 06:51:19.000000 kucoin-futures-python-1.0.8/kucoin_futures_python.egg-info/dependency_links.txt
+-rw-r--r--   0 joysu      (501) staff       (20)       20 2023-07-21 06:51:19.000000 kucoin-futures-python-1.0.8/kucoin_futures_python.egg-info/requires.txt
+-rw-r--r--   0 joysu      (501) staff       (20)      159 2023-07-21 06:51:19.000000 kucoin-futures-python-1.0.8/kucoin_futures_python.egg-info/top_level.txt
+-rw-r--r--   0 joysu      (501) staff       (20)       38 2023-07-21 06:51:19.378685 kucoin-futures-python-1.0.8/setup.cfg
+-rw-r--r--   0 joysu      (501) staff       (20)      751 2023-07-19 08:07:42.000000 kucoin-futures-python-1.0.8/setup.py
```

### Comparing `kucoin-futures-python-1.0.7/LICENSE` & `kucoin-futures-python-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kucoin-futures-python-1.0.7/README.rst` & `kucoin-futures-python-1.0.8/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 - Implementation of REST endpoints
 - Simple handling of authentication
 - Response exception handling
 - Implement websockets (note only python3.6+)
 
 update
 ----------
-- 2023 07/04
+- 2023 07/19
 
 Quick Start
 -----------
 
 Register an account with `KuCoin_Futures <https://futures.kucoin.com/signup?utm=api_github>`_.
 
 To test on the Sandbox  with `KuCoin_Futures Sandbox <https://sandbox-futures.kucoin.com>`_.
```

### Comparing `kucoin-futures-python-1.0.7/kucoin_futures/base_request/base_request.py` & `kucoin-futures-python-1.0.8/kucoin_futures/base_request/base_request.py`

 * *Files identical despite different names*

### Comparing `kucoin-futures-python-1.0.7/kucoin_futures/marke_data/market_data.py` & `kucoin-futures-python-1.0.8/kucoin_futures/marke_data/market_data.py`

 * *Files identical despite different names*

### Comparing `kucoin-futures-python-1.0.7/kucoin_futures/trade/trade.py` & `kucoin-futures-python-1.0.8/kucoin_futures/trade/trade.py`

 * *Files identical despite different names*

### Comparing `kucoin-futures-python-1.0.7/kucoin_futures/user/user.py` & `kucoin-futures-python-1.0.8/kucoin_futures/user/user.py`

 * *Files 10% similar despite different names*

```diff
@@ -407,7 +407,61 @@
         params = {
             'subName': sub_name,
             'passphrase': passphrase,
             'apiKey': api_key
         }
 
         return self._request('DELETE', '/api/v1/sub/api-key', params=params)
+
+    def get_account_overview_all(self, currency="XBT"):
+        """
+        https://www.kucoin.com/zh-hant/docs/rest/funding/funding-overview/get-all-sub-accounts-balance-futures
+        :param currency: string Currecny ,including XBT,USDT,Default XBT
+        :return:
+          {
+            "success": true,
+            "code": "200",
+            "msg": "success",
+            "retry": false,
+            "data": {
+                "summary": {
+                    "accountEquityTotal": 9.99,
+                    "unrealisedPNLTotal": 0,
+                    "marginBalanceTotal": 9.99,
+                    "positionMarginTotal": 0,
+                    "orderMarginTotal": 0,
+                    "frozenFundsTotal": 0,
+                    "availableBalanceTotal": 9.99,
+                    "currency": "USDT"
+                },
+                "accounts": [
+                    {
+                        "accountName": "main",
+                        "accountEquity": 9.99,
+                        "unrealisedPNL": 0,
+                        "marginBalance": 9.99,
+                        "positionMargin": 0,
+                        "orderMargin": 0,
+                        "frozenFunds": 0,
+                        "availableBalance": 9.99,
+                        "currency": "USDT"
+                    },
+                    {
+                        "accountName": "subacct",
+                        "accountEquity": 0,
+                        "unrealisedPNL": 0,
+                        "marginBalance": 0,
+                        "positionMargin": 0,
+                        "orderMargin": 0,
+                        "frozenFunds": 0,
+                        "availableBalance": 0,
+                        "currency": "USDT"
+                    }
+                ]
+            }
+        }
+        """
+        params = {
+            'currency': currency
+        }
+
+        return self._request('GET', '/api/v1/account-overview-all', params=params)
```

### Comparing `kucoin-futures-python-1.0.7/kucoin_futures/websocket/websocket.py` & `kucoin-futures-python-1.0.8/kucoin_futures/websocket/websocket.py`

 * *Files identical despite different names*

### Comparing `kucoin-futures-python-1.0.7/kucoin_futures/ws_client.py` & `kucoin-futures-python-1.0.8/kucoin_futures/ws_client.py`

 * *Files identical despite different names*

### Comparing `kucoin-futures-python-1.0.7/kucoin_futures_python.egg-info/SOURCES.txt` & `kucoin-futures-python-1.0.8/kucoin_futures_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kucoin-futures-python-1.0.7/setup.py` & `kucoin-futures-python-1.0.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:utf-8 -*-
 
 from setuptools import setup
 
 
 setup(
     name='kucoin-futures-python',
-    version='v1.0.7',
+    version='v1.0.8',
     packages=['kucoin_futures', 'kucoin_futures/base_request', 'kucoin_futures/marke_data', 'kucoin_futures/trade', 'kucoin_futures/user',
               'kucoin_futures/websocket', 'kucoin_futures/ws_token'],
     license="MIT",
     author='Grape',
     author_email="grape.zhang@kucoin.com",
     url='https://github.com/Kucoin/kucoin-futures-python-sdk',
     description="kucoin-futures-api-sdk",
```

