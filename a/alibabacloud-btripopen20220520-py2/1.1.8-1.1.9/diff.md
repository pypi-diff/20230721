# Comparing `tmp/alibabacloud_btripopen20220520_py2-1.1.8.tar.gz` & `tmp/alibabacloud_btripopen20220520_py2-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_btripopen20220520_py2-1.1.8.tar", last modified: Thu Jul 13 05:55:03 2023, max compression
+gzip compressed data, was "dist/alibabacloud_btripopen20220520_py2-1.1.9.tar", last modified: Fri Jul 21 04:04:16 2023, max compression
```

## Comparing `alibabacloud_btripopen20220520_py2-1.1.8.tar` & `alibabacloud_btripopen20220520_py2-1.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:55:03.000000 alibabacloud_btripopen20220520_py2-1.1.8/
--rw-r--r--   0 root         (0) root         (0)     3528 2023-07-13 05:55:03.000000 alibabacloud_btripopen20220520_py2-1.1.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-07-13 05:55:03.000000 alibabacloud_btripopen20220520_py2-1.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-13 05:55:03.000000 alibabacloud_btripopen20220520_py2-1.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2508 2023-07-13 05:55:03.000000 alibabacloud_btripopen20220520_py2-1.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1051 2023-07-13 05:55:03.000000 alibabacloud_btripopen20220520_py2-1.1.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1134 2023-07-13 05:55:03.000000 alibabacloud_btripopen20220520_py2-1.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:55:03.000000 alibabacloud_btripopen20220520_py2-1.1.8/alibabacloud_btripopen20220520/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-13 05:55:03.000000 alibabacloud_btripopen20220520_py2-1.1.8/alibabacloud_btripopen20220520/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223404 2023-07-13 05:55:03.000000 alibabacloud_btripopen20220520_py2-1.1.8/alibabacloud_btripopen20220520/client.py
--rw-r--r--   0 root         (0) root         (0)  2007177 2023-07-13 05:55:03.000000 alibabacloud_btripopen20220520_py2-1.1.8/alibabacloud_btripopen20220520/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:55:03.000000 alibabacloud_btripopen20220520_py2-1.1.8/alibabacloud_btripopen20220520_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2508 2023-07-13 05:55:03.000000 alibabacloud_btripopen20220520_py2-1.1.8/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      488 2023-07-13 05:55:03.000000 alibabacloud_btripopen20220520_py2-1.1.8/alibabacloud_btripopen20220520_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 05:55:03.000000 alibabacloud_btripopen20220520_py2-1.1.8/alibabacloud_btripopen20220520_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-07-13 05:55:03.000000 alibabacloud_btripopen20220520_py2-1.1.8/alibabacloud_btripopen20220520_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-07-13 05:55:03.000000 alibabacloud_btripopen20220520_py2-1.1.8/alibabacloud_btripopen20220520_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-13 05:55:03.000000 alibabacloud_btripopen20220520_py2-1.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2933 2023-07-13 05:55:03.000000 alibabacloud_btripopen20220520_py2-1.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:04:16.000000 alibabacloud_btripopen20220520_py2-1.1.9/
+-rw-r--r--   0 root         (0) root         (0)     3565 2023-07-21 04:04:16.000000 alibabacloud_btripopen20220520_py2-1.1.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-21 04:04:16.000000 alibabacloud_btripopen20220520_py2-1.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-21 04:04:16.000000 alibabacloud_btripopen20220520_py2-1.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-07-21 04:04:16.000000 alibabacloud_btripopen20220520_py2-1.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-07-21 04:04:16.000000 alibabacloud_btripopen20220520_py2-1.1.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-07-21 04:04:16.000000 alibabacloud_btripopen20220520_py2-1.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:04:16.000000 alibabacloud_btripopen20220520_py2-1.1.9/alibabacloud_btripopen20220520/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-21 04:04:16.000000 alibabacloud_btripopen20220520_py2-1.1.9/alibabacloud_btripopen20220520/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223404 2023-07-21 04:04:16.000000 alibabacloud_btripopen20220520_py2-1.1.9/alibabacloud_btripopen20220520/client.py
+-rw-r--r--   0 root         (0) root         (0)  2007984 2023-07-21 04:04:16.000000 alibabacloud_btripopen20220520_py2-1.1.9/alibabacloud_btripopen20220520/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:04:16.000000 alibabacloud_btripopen20220520_py2-1.1.9/alibabacloud_btripopen20220520_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-07-21 04:04:16.000000 alibabacloud_btripopen20220520_py2-1.1.9/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      488 2023-07-21 04:04:16.000000 alibabacloud_btripopen20220520_py2-1.1.9/alibabacloud_btripopen20220520_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 04:04:16.000000 alibabacloud_btripopen20220520_py2-1.1.9/alibabacloud_btripopen20220520_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-21 04:04:16.000000 alibabacloud_btripopen20220520_py2-1.1.9/alibabacloud_btripopen20220520_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-21 04:04:16.000000 alibabacloud_btripopen20220520_py2-1.1.9/alibabacloud_btripopen20220520_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-21 04:04:16.000000 alibabacloud_btripopen20220520_py2-1.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-07-21 04:04:16.000000 alibabacloud_btripopen20220520_py2-1.1.9/setup.py
```

### Comparing `alibabacloud_btripopen20220520_py2-1.1.8/ChangeLog.md` & `alibabacloud_btripopen20220520_py2-1.1.9/ChangeLog.md`

 * *Files 1% similar despite different names*

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

### Comparing `alibabacloud_btripopen20220520_py2-1.1.8/LICENSE` & `alibabacloud_btripopen20220520_py2-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.1.8/PKG-INFO` & `alibabacloud_btripopen20220520_py2-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_btripopen20220520_py2
-Version: 1.1.8
+Version: 1.1.9
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520_py2-1.1.8/README-CN.md` & `alibabacloud_btripopen20220520_py2-1.1.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.1.8/README.md` & `alibabacloud_btripopen20220520_py2-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.1.8/alibabacloud_btripopen20220520/client.py` & `alibabacloud_btripopen20220520_py2-1.1.9/alibabacloud_btripopen20220520/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.1.8/alibabacloud_btripopen20220520/models.py` & `alibabacloud_btripopen20220520_py2-1.1.9/alibabacloud_btripopen20220520/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7378,24 +7378,26 @@
             self.order_id = m.get('order_id')
         if m.get('sub_order_id') is not None:
             self.sub_order_id = m.get('sub_order_id')
         return self
 
 
 class CarOrderQueryResponseBodyModuleCarInfo(TeaModel):
-    def __init__(self, business_category=None, cancel_time=None, car_info=None, car_level=None,
-                 driver_confirm_time=None, estimate_price=None, from_address=None, from_city_name=None, is_special=None, memo=None,
-                 pay_time=None, publish_time=None, real_from_address=None, real_from_city_name=None, real_to_address=None,
-                 real_to_city_name=None, service_type=None, special_types=None, taken_time=None, to_address=None, to_city_name=None,
-                 travel_distance=None):
+    def __init__(self, business_category=None, cancel_time=None, car_info=None, car_level=None, driver_card=None,
+                 driver_confirm_time=None, driver_name=None, estimate_price=None, from_address=None, from_city_name=None,
+                 is_special=None, memo=None, pay_time=None, publish_time=None, real_from_address=None,
+                 real_from_city_name=None, real_to_address=None, real_to_city_name=None, service_type=None, special_types=None,
+                 taken_time=None, to_address=None, to_city_name=None, travel_distance=None):
         self.business_category = business_category  # type: str
         self.cancel_time = cancel_time  # type: long
         self.car_info = car_info  # type: str
         self.car_level = car_level  # type: int
+        self.driver_card = driver_card  # type: str
         self.driver_confirm_time = driver_confirm_time  # type: long
+        self.driver_name = driver_name  # type: str
         self.estimate_price = estimate_price  # type: long
         self.from_address = from_address  # type: str
         self.from_city_name = from_city_name  # type: str
         self.is_special = is_special  # type: bool
         self.memo = memo  # type: str
         self.pay_time = pay_time  # type: long
         self.publish_time = publish_time  # type: long
@@ -7423,16 +7425,20 @@
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
@@ -7471,16 +7477,20 @@
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
@@ -38367,16 +38377,17 @@
         m = m or dict()
         if m.get('bill_month') is not None:
             self.bill_month = m.get('bill_month')
         return self
 
 
 class MonthBillGetResponseBodyModuleMonthAccountBillDetail(TeaModel):
-    def __init__(self, car_amount=None, damage_amount=None, flight_amount=None, fu_point=None, hotel_amount=None,
-                 ie_flight_amount=None, mail_bill_date=None, service_amount=None, train_amount=None):
+    def __init__(self, bill_confirmed=None, car_amount=None, damage_amount=None, flight_amount=None, fu_point=None,
+                 hotel_amount=None, ie_flight_amount=None, mail_bill_date=None, service_amount=None, train_amount=None):
+        self.bill_confirmed = bill_confirmed  # type: int
         # 用车金额（单位：元）
         self.car_amount = car_amount  # type: float
         # 违约金金额（单位：元）
         self.damage_amount = damage_amount  # type: float
         # 机票金额（单位：元）
         self.flight_amount = flight_amount  # type: float
         # 福豆金额（单位：元）
@@ -38397,14 +38408,16 @@
 
     def to_map(self):
         _map = super(MonthBillGetResponseBodyModuleMonthAccountBillDetail, self).to_map()
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
@@ -38419,14 +38432,16 @@
             result['serviceAmount'] = self.service_amount
         if self.train_amount is not None:
             result['trainAmount'] = self.train_amount
         return result
 
     def from_map(self, m=None):
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

### Comparing `alibabacloud_btripopen20220520_py2-1.1.8/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO` & `alibabacloud_btripopen20220520_py2-1.1.9/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-btripopen20220520-py2
-Version: 1.1.8
+Version: 1.1.9
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520_py2-1.1.8/setup.py` & `alibabacloud_btripopen20220520_py2-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_btripopen20220520_py2.
 
-Created on 13/07/2023
+Created on 21/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_btripopen20220520"
 NAME = "alibabacloud_btripopen20220520_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud btripOpen (20220520) SDK Library for Python2"
```

