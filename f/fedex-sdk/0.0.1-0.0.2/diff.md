# Comparing `tmp/fedex-sdk-0.0.1.tar.gz` & `tmp/fedex-sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedex-sdk-0.0.1.tar", last modified: Fri Jul 21 08:44:23 2023, max compression
+gzip compressed data, was "fedex-sdk-0.0.2.tar", last modified: Fri Jul 21 08:46:28 2023, max compression
```

## Comparing `fedex-sdk-0.0.1.tar` & `fedex-sdk-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 08:44:23.673225 fedex-sdk-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-07-21 08:44:23.633225 fedex-sdk-0.0.1/FedexSDK/
--rw-rw-rw-   0        0        0     3241 2023-07-21 08:40:34.000000 fedex-sdk-0.0.1/FedexSDK/FedExSDK.py
--rw-rw-rw-   0        0        0       21 2023-07-21 08:38:31.000000 fedex-sdk-0.0.1/FedexSDK/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:44:23.647225 fedex-sdk-0.0.1/FedexSDK/models/
--rw-rw-rw-   0        0        0       79 2023-07-20 14:07:03.000000 fedex-sdk-0.0.1/FedexSDK/models/AccountNumber.py
--rw-rw-rw-   0        0        0     1400 2023-07-20 14:15:22.000000 fedex-sdk-0.0.1/FedexSDK/models/Address.py
--rw-rw-rw-   0        0        0     2163 2023-07-20 13:11:54.000000 fedex-sdk-0.0.1/FedexSDK/models/Contact.py
--rw-rw-rw-   0        0        0      297 2023-07-20 14:00:52.000000 fedex-sdk-0.0.1/FedexSDK/models/Recipient.py
--rw-rw-rw-   0        0        0     1345 2023-07-20 14:16:51.000000 fedex-sdk-0.0.1/FedexSDK/models/Request.py
--rw-rw-rw-   0        0        0     6754 2023-07-21 08:19:24.000000 fedex-sdk-0.0.1/FedexSDK/models/RequestedShipment.py
--rw-rw-rw-   0        0        0      263 2023-07-20 13:49:03.000000 fedex-sdk-0.0.1/FedexSDK/models/Shipper.py
--rw-rw-rw-   0        0        0      316 2023-07-20 14:00:05.000000 fedex-sdk-0.0.1/FedexSDK/models/SoldTo.py
--rw-rw-rw-   0        0        0      581 2023-07-20 13:08:42.000000 fedex-sdk-0.0.1/FedexSDK/models/Tin.py
--rw-rw-rw-   0        0        0      300 2023-07-20 13:07:32.000000 fedex-sdk-0.0.1/FedexSDK/models/TotalDeclaredValue.py
--rw-rw-rw-   0        0        0      969 2023-07-21 08:43:43.000000 fedex-sdk-0.0.1/FedexSDK/models/__init__.py
--rw-rw-rw-   0        0        0      326 2023-07-21 08:44:23.672224 fedex-sdk-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-21 08:44:23.670230 fedex-sdk-0.0.1/fedex_sdk.egg-info/
--rw-rw-rw-   0        0        0      326 2023-07-21 08:44:23.000000 fedex-sdk-0.0.1/fedex_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-07-21 08:44:23.000000 fedex-sdk-0.0.1/fedex_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 08:44:23.000000 fedex-sdk-0.0.1/fedex_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-21 08:44:23.000000 fedex-sdk-0.0.1/fedex_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 08:44:23.673225 fedex-sdk-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      559 2023-07-21 08:44:20.000000 fedex-sdk-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:46:28.234185 fedex-sdk-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-07-21 08:46:28.201410 fedex-sdk-0.0.2/FedexSDK/
+-rw-rw-rw-   0        0        0     3241 2023-07-21 08:40:34.000000 fedex-sdk-0.0.2/FedexSDK/FedExSDK.py
+-rw-rw-rw-   0        0        0       55 2023-07-21 08:46:24.000000 fedex-sdk-0.0.2/FedexSDK/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:46:28.213224 fedex-sdk-0.0.2/FedexSDK/models/
+-rw-rw-rw-   0        0        0       79 2023-07-20 14:07:03.000000 fedex-sdk-0.0.2/FedexSDK/models/AccountNumber.py
+-rw-rw-rw-   0        0        0     1400 2023-07-20 14:15:22.000000 fedex-sdk-0.0.2/FedexSDK/models/Address.py
+-rw-rw-rw-   0        0        0     2163 2023-07-20 13:11:54.000000 fedex-sdk-0.0.2/FedexSDK/models/Contact.py
+-rw-rw-rw-   0        0        0      297 2023-07-20 14:00:52.000000 fedex-sdk-0.0.2/FedexSDK/models/Recipient.py
+-rw-rw-rw-   0        0        0     1345 2023-07-20 14:16:51.000000 fedex-sdk-0.0.2/FedexSDK/models/Request.py
+-rw-rw-rw-   0        0        0     6754 2023-07-21 08:19:24.000000 fedex-sdk-0.0.2/FedexSDK/models/RequestedShipment.py
+-rw-rw-rw-   0        0        0      263 2023-07-20 13:49:03.000000 fedex-sdk-0.0.2/FedexSDK/models/Shipper.py
+-rw-rw-rw-   0        0        0      316 2023-07-20 14:00:05.000000 fedex-sdk-0.0.2/FedexSDK/models/SoldTo.py
+-rw-rw-rw-   0        0        0      581 2023-07-20 13:08:42.000000 fedex-sdk-0.0.2/FedexSDK/models/Tin.py
+-rw-rw-rw-   0        0        0      300 2023-07-20 13:07:32.000000 fedex-sdk-0.0.2/FedexSDK/models/TotalDeclaredValue.py
+-rw-rw-rw-   0        0        0      969 2023-07-21 08:43:43.000000 fedex-sdk-0.0.2/FedexSDK/models/__init__.py
+-rw-rw-rw-   0        0        0      326 2023-07-21 08:46:28.233184 fedex-sdk-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-21 08:46:28.232191 fedex-sdk-0.0.2/fedex_sdk.egg-info/
+-rw-rw-rw-   0        0        0      326 2023-07-21 08:46:27.000000 fedex-sdk-0.0.2/fedex_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-07-21 08:46:28.000000 fedex-sdk-0.0.2/fedex_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 08:46:27.000000 fedex-sdk-0.0.2/fedex_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-21 08:46:27.000000 fedex-sdk-0.0.2/fedex_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 08:46:28.234185 fedex-sdk-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      559 2023-07-21 08:44:20.000000 fedex-sdk-0.0.2/setup.py
```

### Comparing `fedex-sdk-0.0.1/FedexSDK/FedExSDK.py` & `fedex-sdk-0.0.2/FedexSDK/FedExSDK.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.1/FedexSDK/models/Address.py` & `fedex-sdk-0.0.2/FedexSDK/models/Address.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.1/FedexSDK/models/Contact.py` & `fedex-sdk-0.0.2/FedexSDK/models/Contact.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.1/FedexSDK/models/Request.py` & `fedex-sdk-0.0.2/FedexSDK/models/Request.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.1/FedexSDK/models/RequestedShipment.py` & `fedex-sdk-0.0.2/FedexSDK/models/RequestedShipment.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.1/FedexSDK/models/Tin.py` & `fedex-sdk-0.0.2/FedexSDK/models/Tin.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.1/FedexSDK/models/__init__.py` & `fedex-sdk-0.0.2/FedexSDK/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.1/setup.py` & `fedex-sdk-0.0.2/setup.py`

 * *Files identical despite different names*

