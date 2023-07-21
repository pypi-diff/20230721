# Comparing `tmp/fedex-sdk-0.0.3.tar.gz` & `tmp/fedex-sdk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedex-sdk-0.0.3.tar", last modified: Fri Jul 21 13:40:39 2023, max compression
+gzip compressed data, was "fedex-sdk-0.0.4.tar", last modified: Fri Jul 21 14:09:21 2023, max compression
```

## Comparing `fedex-sdk-0.0.3.tar` & `fedex-sdk-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 13:40:39.228057 fedex-sdk-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-07-21 13:40:39.143358 fedex-sdk-0.0.3/FedexSDK/
--rw-rw-rw-   0        0        0     3240 2023-07-21 13:40:15.000000 fedex-sdk-0.0.3/FedexSDK/FedExSDK.py
--rw-rw-rw-   0        0        0       55 2023-07-21 13:40:24.000000 fedex-sdk-0.0.3/FedexSDK/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:40:39.205853 fedex-sdk-0.0.3/FedexSDK/models/
--rw-rw-rw-   0        0        0       79 2023-07-20 14:07:03.000000 fedex-sdk-0.0.3/FedexSDK/models/AccountNumber.py
--rw-rw-rw-   0        0        0     1400 2023-07-20 14:15:22.000000 fedex-sdk-0.0.3/FedexSDK/models/Address.py
--rw-rw-rw-   0        0        0     2163 2023-07-20 13:11:54.000000 fedex-sdk-0.0.3/FedexSDK/models/Contact.py
--rw-rw-rw-   0        0        0      297 2023-07-20 14:00:52.000000 fedex-sdk-0.0.3/FedexSDK/models/Recipient.py
--rw-rw-rw-   0        0        0     1345 2023-07-20 14:16:51.000000 fedex-sdk-0.0.3/FedexSDK/models/Request.py
--rw-rw-rw-   0        0        0     6754 2023-07-21 08:19:24.000000 fedex-sdk-0.0.3/FedexSDK/models/RequestedShipment.py
--rw-rw-rw-   0        0        0      263 2023-07-20 13:49:03.000000 fedex-sdk-0.0.3/FedexSDK/models/Shipper.py
--rw-rw-rw-   0        0        0      316 2023-07-20 14:00:05.000000 fedex-sdk-0.0.3/FedexSDK/models/SoldTo.py
--rw-rw-rw-   0        0        0      581 2023-07-20 13:08:42.000000 fedex-sdk-0.0.3/FedexSDK/models/Tin.py
--rw-rw-rw-   0        0        0      300 2023-07-20 13:07:32.000000 fedex-sdk-0.0.3/FedexSDK/models/TotalDeclaredValue.py
--rw-rw-rw-   0        0        0      969 2023-07-21 08:43:43.000000 fedex-sdk-0.0.3/FedexSDK/models/__init__.py
--rw-rw-rw-   0        0        0      326 2023-07-21 13:40:39.228057 fedex-sdk-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-21 13:40:39.228057 fedex-sdk-0.0.3/fedex_sdk.egg-info/
--rw-rw-rw-   0        0        0      326 2023-07-21 13:40:38.000000 fedex-sdk-0.0.3/fedex_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-07-21 13:40:39.000000 fedex-sdk-0.0.3/fedex_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 13:40:38.000000 fedex-sdk-0.0.3/fedex_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-21 13:40:38.000000 fedex-sdk-0.0.3/fedex_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 13:40:39.228057 fedex-sdk-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      559 2023-07-21 08:44:20.000000 fedex-sdk-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 14:09:21.165813 fedex-sdk-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-07-21 14:09:21.118943 fedex-sdk-0.0.4/FedexSDK/
+-rw-rw-rw-   0        0        0     3231 2023-07-21 14:09:04.000000 fedex-sdk-0.0.4/FedexSDK/FedExSDK.py
+-rw-rw-rw-   0        0        0       55 2023-07-21 14:09:11.000000 fedex-sdk-0.0.4/FedexSDK/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 14:09:21.134566 fedex-sdk-0.0.4/FedexSDK/models/
+-rw-rw-rw-   0        0        0       79 2023-07-20 14:07:03.000000 fedex-sdk-0.0.4/FedexSDK/models/AccountNumber.py
+-rw-rw-rw-   0        0        0     1400 2023-07-20 14:15:22.000000 fedex-sdk-0.0.4/FedexSDK/models/Address.py
+-rw-rw-rw-   0        0        0     2163 2023-07-20 13:11:54.000000 fedex-sdk-0.0.4/FedexSDK/models/Contact.py
+-rw-rw-rw-   0        0        0      297 2023-07-20 14:00:52.000000 fedex-sdk-0.0.4/FedexSDK/models/Recipient.py
+-rw-rw-rw-   0        0        0     1345 2023-07-20 14:16:51.000000 fedex-sdk-0.0.4/FedexSDK/models/Request.py
+-rw-rw-rw-   0        0        0     6754 2023-07-21 08:19:24.000000 fedex-sdk-0.0.4/FedexSDK/models/RequestedShipment.py
+-rw-rw-rw-   0        0        0      263 2023-07-20 13:49:03.000000 fedex-sdk-0.0.4/FedexSDK/models/Shipper.py
+-rw-rw-rw-   0        0        0      316 2023-07-20 14:00:05.000000 fedex-sdk-0.0.4/FedexSDK/models/SoldTo.py
+-rw-rw-rw-   0        0        0      581 2023-07-20 13:08:42.000000 fedex-sdk-0.0.4/FedexSDK/models/Tin.py
+-rw-rw-rw-   0        0        0      300 2023-07-20 13:07:32.000000 fedex-sdk-0.0.4/FedexSDK/models/TotalDeclaredValue.py
+-rw-rw-rw-   0        0        0      969 2023-07-21 08:43:43.000000 fedex-sdk-0.0.4/FedexSDK/models/__init__.py
+-rw-rw-rw-   0        0        0      326 2023-07-21 14:09:21.150191 fedex-sdk-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-21 14:09:21.150191 fedex-sdk-0.0.4/fedex_sdk.egg-info/
+-rw-rw-rw-   0        0        0      326 2023-07-21 14:09:20.000000 fedex-sdk-0.0.4/fedex_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-07-21 14:09:21.000000 fedex-sdk-0.0.4/fedex_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 14:09:20.000000 fedex-sdk-0.0.4/fedex_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-21 14:09:20.000000 fedex-sdk-0.0.4/fedex_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 14:09:21.165813 fedex-sdk-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      559 2023-07-21 08:44:20.000000 fedex-sdk-0.0.4/setup.py
```

### Comparing `fedex-sdk-0.0.3/FedexSDK/FedExSDK.py` & `fedex-sdk-0.0.4/FedexSDK/FedExSDK.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         url = "https://apis.fedex.com/ship/v1/shipments"
 
         res = self.session.post(url, json=request.dict(), headers=self.headers)
         
         now_date = datetime.datetime.now()
         with open(f"{now_date.strftime('%d_%m_%Y_tracking_numbers.txt')}", "a") as f:
             f.write(
-                f"{res.json()['output']['transactionShipments'][0]['shipmentDocuments'][0]['trackingNumber']}:{data['requestedShipment']['recipients'][0]['contact']['personName']}\n"
+                f"{res.json()['output']['transactionShipments'][0]['shipmentDocuments'][0]['trackingNumber']}:{request.requestedShipment.recipients[0].contact.personName}\n"
             )
         
         json.dump(res.json(), open(output_json_path, "w", encoding="utf-8"), ensure_ascii=False)
 
     
     def add_image(self, reference_id: str, image_name: str, image_index: str, image_type: ImageType, image_path: str):
         name, ext = os.path.splitext(image_path)
```

### Comparing `fedex-sdk-0.0.3/FedexSDK/models/Address.py` & `fedex-sdk-0.0.4/FedexSDK/models/Address.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.3/FedexSDK/models/Contact.py` & `fedex-sdk-0.0.4/FedexSDK/models/Contact.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.3/FedexSDK/models/Request.py` & `fedex-sdk-0.0.4/FedexSDK/models/Request.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.3/FedexSDK/models/RequestedShipment.py` & `fedex-sdk-0.0.4/FedexSDK/models/RequestedShipment.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.3/FedexSDK/models/Tin.py` & `fedex-sdk-0.0.4/FedexSDK/models/Tin.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.3/FedexSDK/models/__init__.py` & `fedex-sdk-0.0.4/FedexSDK/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.3/setup.py` & `fedex-sdk-0.0.4/setup.py`

 * *Files identical despite different names*

