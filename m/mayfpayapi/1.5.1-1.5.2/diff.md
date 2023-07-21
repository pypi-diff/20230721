# Comparing `tmp/mayfpayapi-1.5.1.tar.gz` & `tmp/mayfpayapi-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mayfpayapi-1.5.1.tar", last modified: Wed Jul 19 07:11:08 2023, max compression
+gzip compressed data, was "mayfpayapi-1.5.2.tar", last modified: Fri Jul 21 10:13:15 2023, max compression
```

## Comparing `mayfpayapi-1.5.1.tar` & `mayfpayapi-1.5.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dimamayfeed   (502) staff       (20)        0 2023-07-19 07:11:08.720821 mayfpayapi-1.5.1/
--rw-r--r--   0 dimamayfeed   (502) staff       (20)     1794 2023-07-19 07:11:08.720634 mayfpayapi-1.5.1/PKG-INFO
--rw-r--r--   0 dimamayfeed   (502) staff       (20)     1241 2023-07-19 07:07:33.000000 mayfpayapi-1.5.1/README.md
-drwxr-xr-x   0 dimamayfeed   (502) staff       (20)        0 2023-07-19 07:11:08.719176 mayfpayapi-1.5.1/mayfpayapi/
--rw-r--r--   0 dimamayfeed   (502) staff       (20)       26 2023-04-10 18:23:23.000000 mayfpayapi-1.5.1/mayfpayapi/__init__.py
--rw-r--r--   0 dimamayfeed   (502) staff       (20)     2646 2023-07-19 07:06:17.000000 mayfpayapi-1.5.1/mayfpayapi/mayfpayapi.py
-drwxr-xr-x   0 dimamayfeed   (502) staff       (20)        0 2023-07-19 07:11:08.720363 mayfpayapi-1.5.1/mayfpayapi.egg-info/
--rw-r--r--   0 dimamayfeed   (502) staff       (20)     1794 2023-07-19 07:11:08.000000 mayfpayapi-1.5.1/mayfpayapi.egg-info/PKG-INFO
--rw-r--r--   0 dimamayfeed   (502) staff       (20)      235 2023-07-19 07:11:08.000000 mayfpayapi-1.5.1/mayfpayapi.egg-info/SOURCES.txt
--rw-r--r--   0 dimamayfeed   (502) staff       (20)        1 2023-07-19 07:11:08.000000 mayfpayapi-1.5.1/mayfpayapi.egg-info/dependency_links.txt
--rw-r--r--   0 dimamayfeed   (502) staff       (20)        9 2023-07-19 07:11:08.000000 mayfpayapi-1.5.1/mayfpayapi.egg-info/requires.txt
--rw-r--r--   0 dimamayfeed   (502) staff       (20)       11 2023-07-19 07:11:08.000000 mayfpayapi-1.5.1/mayfpayapi.egg-info/top_level.txt
--rw-r--r--   0 dimamayfeed   (502) staff       (20)       38 2023-07-19 07:11:08.720900 mayfpayapi-1.5.1/setup.cfg
--rw-r--r--   0 dimamayfeed   (502) staff       (20)      892 2023-07-19 07:08:49.000000 mayfpayapi-1.5.1/setup.py
+drwxr-xr-x   0 dimamayfeed   (502) staff       (20)        0 2023-07-21 10:13:15.572627 mayfpayapi-1.5.2/
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)     1794 2023-07-21 10:13:15.572437 mayfpayapi-1.5.2/PKG-INFO
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)     1241 2023-07-19 07:07:33.000000 mayfpayapi-1.5.2/README.md
+drwxr-xr-x   0 dimamayfeed   (502) staff       (20)        0 2023-07-21 10:13:15.570907 mayfpayapi-1.5.2/mayfpayapi/
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)       26 2023-04-10 18:23:23.000000 mayfpayapi-1.5.2/mayfpayapi/__init__.py
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)     2667 2023-07-21 10:07:33.000000 mayfpayapi-1.5.2/mayfpayapi/mayfpayapi.py
+drwxr-xr-x   0 dimamayfeed   (502) staff       (20)        0 2023-07-21 10:13:15.572152 mayfpayapi-1.5.2/mayfpayapi.egg-info/
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)     1794 2023-07-21 10:13:15.000000 mayfpayapi-1.5.2/mayfpayapi.egg-info/PKG-INFO
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)      235 2023-07-21 10:13:15.000000 mayfpayapi-1.5.2/mayfpayapi.egg-info/SOURCES.txt
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)        1 2023-07-21 10:13:15.000000 mayfpayapi-1.5.2/mayfpayapi.egg-info/dependency_links.txt
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)        9 2023-07-21 10:13:15.000000 mayfpayapi-1.5.2/mayfpayapi.egg-info/requires.txt
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)       11 2023-07-21 10:13:15.000000 mayfpayapi-1.5.2/mayfpayapi.egg-info/top_level.txt
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)       38 2023-07-21 10:13:15.572688 mayfpayapi-1.5.2/setup.cfg
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)      892 2023-07-21 10:05:50.000000 mayfpayapi-1.5.2/setup.py
```

### Comparing `mayfpayapi-1.5.1/PKG-INFO` & `mayfpayapi-1.5.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayfpayapi
-Version: 1.5.1
+Version: 1.5.2
 Summary: MayfPayApi is a Python library for interacting with the MayfPay payment system API. It provides methods for retrieving kassa balances, creating and checking invoices.
 Home-page: https://github.com/MAYFPAY/MayfPayApi
 Author: MayfPay
 Author-email: support@mayfpay.top
 Project-URL: Source, https://github.com/MAYFPAY/MayfPayApi
 Project-URL: Documentation, https://mayfpay.top/docs
 Project-URL: Bug Reports, https://github.com/MAYFPAY/MayfPayApi/issues
```

### Comparing `mayfpayapi-1.5.1/README.md` & `mayfpayapi-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `mayfpayapi-1.5.1/mayfpayapi/mayfpayapi.py` & `mayfpayapi-1.5.2/mayfpayapi/mayfpayapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             "kassa_id": self.kassa_id,
         }
         headers = self._generate_auth_headers(payload)  # Pass payload as an argument
         response = requests.get(url, headers=headers, json=payload)
         response_json = response.json()
         return response_json
 
-    def create_invoice(self, amount: float, order_id: str, expire_invoice: int, payment_method: str, comment: str, data: dict, en: bool = False, SubPayMethodId: str = None, successUrl: str = None, failUrl: str = None):
+    def create_invoice(self, amount: float, order_id: str, payment_method: str, expire_invoice: int = None, comment: str = None, data: dict = None, en: bool = False, SubPayMethodId: str = None, successUrl: str = None, failUrl: str = None):
         url = f"{self.base_url}/kassa/invoice/create"
         payload = {
             "api_token": self.api_token,
             "kassa_id": self.kassa_id,
             "amount": amount,
             "order_id": order_id,
             "expire_invoice": expire_invoice,
```

### Comparing `mayfpayapi-1.5.1/mayfpayapi.egg-info/PKG-INFO` & `mayfpayapi-1.5.2/mayfpayapi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayfpayapi
-Version: 1.5.1
+Version: 1.5.2
 Summary: MayfPayApi is a Python library for interacting with the MayfPay payment system API. It provides methods for retrieving kassa balances, creating and checking invoices.
 Home-page: https://github.com/MAYFPAY/MayfPayApi
 Author: MayfPay
 Author-email: support@mayfpay.top
 Project-URL: Source, https://github.com/MAYFPAY/MayfPayApi
 Project-URL: Documentation, https://mayfpay.top/docs
 Project-URL: Bug Reports, https://github.com/MAYFPAY/MayfPayApi/issues
```

### Comparing `mayfpayapi-1.5.1/setup.py` & `mayfpayapi-1.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='mayfpayapi',
-    version='1.5.1',
+    version='1.5.2',
     author='MayfPay',
     author_email='support@mayfpay.top',
     description='MayfPayApi is a Python library for interacting with the MayfPay payment system API. It provides methods for retrieving kassa balances, creating and checking invoices.',
     url='https://github.com/MAYFPAY/MayfPayApi',
     packages=find_packages(),
     py_modules=['mayfpayapi'],
     project_urls={
```

