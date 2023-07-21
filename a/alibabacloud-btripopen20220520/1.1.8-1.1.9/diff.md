# Comparing `tmp/alibabacloud_btripopen20220520-1.1.8.tar.gz` & `tmp/alibabacloud_btripopen20220520-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_btripopen20220520-1.1.8.tar", last modified: Thu Jul 13 05:55:44 2023, max compression
+gzip compressed data, was "dist/alibabacloud_btripopen20220520-1.1.9.tar", last modified: Fri Jul 21 04:04:48 2023, max compression
```

## Comparing `alibabacloud_btripopen20220520-1.1.8.tar` & `alibabacloud_btripopen20220520-1.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:55:44.000000 alibabacloud_btripopen20220520-1.1.8/
--rw-r--r--   0 root         (0) root         (0)     3654 2023-07-13 05:55:43.000000 alibabacloud_btripopen20220520-1.1.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-13 05:55:43.000000 alibabacloud_btripopen20220520-1.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-13 05:55:43.000000 alibabacloud_btripopen20220520-1.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2364 2023-07-13 05:55:44.000000 alibabacloud_btripopen20220520-1.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1040 2023-07-13 05:55:43.000000 alibabacloud_btripopen20220520-1.1.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2023-07-13 05:55:43.000000 alibabacloud_btripopen20220520-1.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:55:44.000000 alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-13 05:55:43.000000 alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520/__init__.py
--rw-r--r--   0 root         (0) root         (0)   525626 2023-07-13 05:55:43.000000 alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520/client.py
--rw-r--r--   0 root         (0) root         (0)  1985099 2023-07-13 05:55:43.000000 alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:55:44.000000 alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2364 2023-07-13 05:55:44.000000 alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2023-07-13 05:55:44.000000 alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 05:55:44.000000 alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-07-13 05:55:44.000000 alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-07-13 05:55:44.000000 alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-13 05:55:44.000000 alibabacloud_btripopen20220520-1.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2640 2023-07-13 05:55:43.000000 alibabacloud_btripopen20220520-1.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:04:48.000000 alibabacloud_btripopen20220520-1.1.9/
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-07-21 04:04:47.000000 alibabacloud_btripopen20220520-1.1.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-21 04:04:47.000000 alibabacloud_btripopen20220520-1.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-21 04:04:47.000000 alibabacloud_btripopen20220520-1.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-07-21 04:04:48.000000 alibabacloud_btripopen20220520-1.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-07-21 04:04:47.000000 alibabacloud_btripopen20220520-1.1.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-07-21 04:04:47.000000 alibabacloud_btripopen20220520-1.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:04:48.000000 alibabacloud_btripopen20220520-1.1.9/alibabacloud_btripopen20220520/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-21 04:04:47.000000 alibabacloud_btripopen20220520-1.1.9/alibabacloud_btripopen20220520/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   525626 2023-07-21 04:04:47.000000 alibabacloud_btripopen20220520-1.1.9/alibabacloud_btripopen20220520/client.py
+-rw-r--r--   0 root         (0) root         (0)  1985912 2023-07-21 04:04:47.000000 alibabacloud_btripopen20220520-1.1.9/alibabacloud_btripopen20220520/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:04:48.000000 alibabacloud_btripopen20220520-1.1.9/alibabacloud_btripopen20220520.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-07-21 04:04:48.000000 alibabacloud_btripopen20220520-1.1.9/alibabacloud_btripopen20220520.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2023-07-21 04:04:48.000000 alibabacloud_btripopen20220520-1.1.9/alibabacloud_btripopen20220520.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 04:04:48.000000 alibabacloud_btripopen20220520-1.1.9/alibabacloud_btripopen20220520.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-21 04:04:48.000000 alibabacloud_btripopen20220520-1.1.9/alibabacloud_btripopen20220520.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-21 04:04:48.000000 alibabacloud_btripopen20220520-1.1.9/alibabacloud_btripopen20220520.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-21 04:04:48.000000 alibabacloud_btripopen20220520-1.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-07-21 04:04:47.000000 alibabacloud_btripopen20220520-1.1.9/setup.py
```

### Comparing `alibabacloud_btripopen20220520-1.1.8/ChangeLog.md` & `alibabacloud_btripopen20220520-1.1.9/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07-13 Version: 1.1.8
+- Update.
+
 2023-07-04 Version: 1.1.7
 - Update.
 
 2023-06-26 Version: 1.1.6
 - Update.
 
 2023-06-16 Version: 1.1.5
```

### Comparing `alibabacloud_btripopen20220520-1.1.8/LICENSE` & `alibabacloud_btripopen20220520-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520-1.1.8/PKG-INFO` & `alibabacloud_btripopen20220520-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_btripopen20220520
-Version: 1.1.8
+Version: 1.1.9
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520-1.1.8/README-CN.md` & `alibabacloud_btripopen20220520-1.1.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520-1.1.8/README.md` & `alibabacloud_btripopen20220520-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520/client.py` & `alibabacloud_btripopen20220520-1.1.9/alibabacloud_btripopen20220520/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520/models.py` & `alibabacloud_btripopen20220520-1.1.9/alibabacloud_btripopen20220520/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8420,15 +8420,17 @@
 class CarOrderQueryResponseBodyModuleCarInfo(TeaModel):
     def __init__(
         self,
         business_category: str = None,
         cancel_time: int = None,
         car_info: str = None,
         car_level: int = None,
+        driver_card: str = None,
         driver_confirm_time: int = None,
+        driver_name: str = None,
         estimate_price: int = None,
         from_address: str = None,
         from_city_name: str = None,
         is_special: bool = None,
         memo: str = None,
         pay_time: int = None,
         publish_time: int = None,
@@ -8443,15 +8445,17 @@
         to_city_name: str = None,
         travel_distance: str = None,
     ):
         self.business_category = business_category
         self.cancel_time = cancel_time
         self.car_info = car_info
         self.car_level = car_level
+        self.driver_card = driver_card
         self.driver_confirm_time = driver_confirm_time
+        self.driver_name = driver_name
         self.estimate_price = estimate_price
         self.from_address = from_address
         self.from_city_name = from_city_name
         self.is_special = is_special
         self.memo = memo
         self.pay_time = pay_time
         self.publish_time = publish_time
@@ -8479,16 +8483,20 @@
             result['business_category'] = self.business_category
         if self.cancel_time is not None:
             result['cancel_time'] = self.cancel_time
         if self.car_info is not None:
             result['car_info'] = self.car_info
         if self.car_level is not None:
             result['car_level'] = self.car_level
+        if self.driver_card is not None:
+            result['driver_card'] = self.driver_card
         if self.driver_confirm_time is not None:
             result['driver_confirm_time'] = self.driver_confirm_time
+        if self.driver_name is not None:
+            result['driver_name'] = self.driver_name
         if self.estimate_price is not None:
             result['estimate_price'] = self.estimate_price
         if self.from_address is not None:
             result['from_address'] = self.from_address
         if self.from_city_name is not None:
             result['from_city_name'] = self.from_city_name
         if self.is_special is not None:
@@ -8527,16 +8535,20 @@
             self.business_category = m.get('business_category')
         if m.get('cancel_time') is not None:
             self.cancel_time = m.get('cancel_time')
         if m.get('car_info') is not None:
             self.car_info = m.get('car_info')
         if m.get('car_level') is not None:
             self.car_level = m.get('car_level')
+        if m.get('driver_card') is not None:
+            self.driver_card = m.get('driver_card')
         if m.get('driver_confirm_time') is not None:
             self.driver_confirm_time = m.get('driver_confirm_time')
+        if m.get('driver_name') is not None:
+            self.driver_name = m.get('driver_name')
         if m.get('estimate_price') is not None:
             self.estimate_price = m.get('estimate_price')
         if m.get('from_address') is not None:
             self.from_address = m.get('from_address')
         if m.get('from_city_name') is not None:
             self.from_city_name = m.get('from_city_name')
         if m.get('is_special') is not None:
@@ -43727,24 +43739,26 @@
             self.bill_month = m.get('bill_month')
         return self
 
 
 class MonthBillGetResponseBodyModuleMonthAccountBillDetail(TeaModel):
     def __init__(
         self,
+        bill_confirmed: int = None,
         car_amount: float = None,
         damage_amount: float = None,
         flight_amount: float = None,
         fu_point: float = None,
         hotel_amount: float = None,
         ie_flight_amount: float = None,
         mail_bill_date: int = None,
         service_amount: float = None,
         train_amount: float = None,
     ):
+        self.bill_confirmed = bill_confirmed
         # 用车金额（单位：元）
         self.car_amount = car_amount
         # 违约金金额（单位：元）
         self.damage_amount = damage_amount
         # 机票金额（单位：元）
         self.flight_amount = flight_amount
         # 福豆金额（单位：元）
@@ -43765,14 +43779,16 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.bill_confirmed is not None:
+            result['billConfirmed'] = self.bill_confirmed
         if self.car_amount is not None:
             result['carAmount'] = self.car_amount
         if self.damage_amount is not None:
             result['damageAmount'] = self.damage_amount
         if self.flight_amount is not None:
             result['flightAmount'] = self.flight_amount
         if self.fu_point is not None:
@@ -43787,14 +43803,16 @@
             result['serviceAmount'] = self.service_amount
         if self.train_amount is not None:
             result['trainAmount'] = self.train_amount
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('billConfirmed') is not None:
+            self.bill_confirmed = m.get('billConfirmed')
         if m.get('carAmount') is not None:
             self.car_amount = m.get('carAmount')
         if m.get('damageAmount') is not None:
             self.damage_amount = m.get('damageAmount')
         if m.get('flightAmount') is not None:
             self.flight_amount = m.get('flightAmount')
         if m.get('fuPoint') is not None:
```

### Comparing `alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520.egg-info/PKG-INFO` & `alibabacloud_btripopen20220520-1.1.9/alibabacloud_btripopen20220520.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-btripopen20220520
-Version: 1.1.8
+Version: 1.1.9
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520-1.1.8/setup.py` & `alibabacloud_btripopen20220520-1.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_btripopen20220520.
 
-Created on 13/07/2023
+Created on 21/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_btripopen20220520"
 NAME = "alibabacloud_btripopen20220520" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud btripOpen (20220520) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.9, <1.0.0",
+    "alibabacloud_tea_util>=0.3.10, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

