# Comparing `tmp/fedex-sdk-0.0.2.tar.gz` & `tmp/fedex-sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedex-sdk-0.0.2.tar", last modified: Fri Jul 21 08:46:28 2023, max compression
+gzip compressed data, was "fedex-sdk-0.0.3.tar", last modified: Fri Jul 21 13:40:39 2023, max compression
```

## Comparing `fedex-sdk-0.0.2.tar` & `fedex-sdk-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 08:46:28.234185 fedex-sdk-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-07-21 08:46:28.201410 fedex-sdk-0.0.2/FedexSDK/
--rw-rw-rw-   0        0        0     3241 2023-07-21 08:40:34.000000 fedex-sdk-0.0.2/FedexSDK/FedExSDK.py
--rw-rw-rw-   0        0        0       55 2023-07-21 08:46:24.000000 fedex-sdk-0.0.2/FedexSDK/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:46:28.213224 fedex-sdk-0.0.2/FedexSDK/models/
--rw-rw-rw-   0        0        0       79 2023-07-20 14:07:03.000000 fedex-sdk-0.0.2/FedexSDK/models/AccountNumber.py
--rw-rw-rw-   0        0        0     1400 2023-07-20 14:15:22.000000 fedex-sdk-0.0.2/FedexSDK/models/Address.py
--rw-rw-rw-   0        0        0     2163 2023-07-20 13:11:54.000000 fedex-sdk-0.0.2/FedexSDK/models/Contact.py
--rw-rw-rw-   0        0        0      297 2023-07-20 14:00:52.000000 fedex-sdk-0.0.2/FedexSDK/models/Recipient.py
--rw-rw-rw-   0        0        0     1345 2023-07-20 14:16:51.000000 fedex-sdk-0.0.2/FedexSDK/models/Request.py
--rw-rw-rw-   0        0        0     6754 2023-07-21 08:19:24.000000 fedex-sdk-0.0.2/FedexSDK/models/RequestedShipment.py
--rw-rw-rw-   0        0        0      263 2023-07-20 13:49:03.000000 fedex-sdk-0.0.2/FedexSDK/models/Shipper.py
--rw-rw-rw-   0        0        0      316 2023-07-20 14:00:05.000000 fedex-sdk-0.0.2/FedexSDK/models/SoldTo.py
--rw-rw-rw-   0        0        0      581 2023-07-20 13:08:42.000000 fedex-sdk-0.0.2/FedexSDK/models/Tin.py
--rw-rw-rw-   0        0        0      300 2023-07-20 13:07:32.000000 fedex-sdk-0.0.2/FedexSDK/models/TotalDeclaredValue.py
--rw-rw-rw-   0        0        0      969 2023-07-21 08:43:43.000000 fedex-sdk-0.0.2/FedexSDK/models/__init__.py
--rw-rw-rw-   0        0        0      326 2023-07-21 08:46:28.233184 fedex-sdk-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-21 08:46:28.232191 fedex-sdk-0.0.2/fedex_sdk.egg-info/
--rw-rw-rw-   0        0        0      326 2023-07-21 08:46:27.000000 fedex-sdk-0.0.2/fedex_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-07-21 08:46:28.000000 fedex-sdk-0.0.2/fedex_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 08:46:27.000000 fedex-sdk-0.0.2/fedex_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-21 08:46:27.000000 fedex-sdk-0.0.2/fedex_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 08:46:28.234185 fedex-sdk-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      559 2023-07-21 08:44:20.000000 fedex-sdk-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 13:40:39.228057 fedex-sdk-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-07-21 13:40:39.143358 fedex-sdk-0.0.3/FedexSDK/
+-rw-rw-rw-   0        0        0     3240 2023-07-21 13:40:15.000000 fedex-sdk-0.0.3/FedexSDK/FedExSDK.py
+-rw-rw-rw-   0        0        0       55 2023-07-21 13:40:24.000000 fedex-sdk-0.0.3/FedexSDK/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 13:40:39.205853 fedex-sdk-0.0.3/FedexSDK/models/
+-rw-rw-rw-   0        0        0       79 2023-07-20 14:07:03.000000 fedex-sdk-0.0.3/FedexSDK/models/AccountNumber.py
+-rw-rw-rw-   0        0        0     1400 2023-07-20 14:15:22.000000 fedex-sdk-0.0.3/FedexSDK/models/Address.py
+-rw-rw-rw-   0        0        0     2163 2023-07-20 13:11:54.000000 fedex-sdk-0.0.3/FedexSDK/models/Contact.py
+-rw-rw-rw-   0        0        0      297 2023-07-20 14:00:52.000000 fedex-sdk-0.0.3/FedexSDK/models/Recipient.py
+-rw-rw-rw-   0        0        0     1345 2023-07-20 14:16:51.000000 fedex-sdk-0.0.3/FedexSDK/models/Request.py
+-rw-rw-rw-   0        0        0     6754 2023-07-21 08:19:24.000000 fedex-sdk-0.0.3/FedexSDK/models/RequestedShipment.py
+-rw-rw-rw-   0        0        0      263 2023-07-20 13:49:03.000000 fedex-sdk-0.0.3/FedexSDK/models/Shipper.py
+-rw-rw-rw-   0        0        0      316 2023-07-20 14:00:05.000000 fedex-sdk-0.0.3/FedexSDK/models/SoldTo.py
+-rw-rw-rw-   0        0        0      581 2023-07-20 13:08:42.000000 fedex-sdk-0.0.3/FedexSDK/models/Tin.py
+-rw-rw-rw-   0        0        0      300 2023-07-20 13:07:32.000000 fedex-sdk-0.0.3/FedexSDK/models/TotalDeclaredValue.py
+-rw-rw-rw-   0        0        0      969 2023-07-21 08:43:43.000000 fedex-sdk-0.0.3/FedexSDK/models/__init__.py
+-rw-rw-rw-   0        0        0      326 2023-07-21 13:40:39.228057 fedex-sdk-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-21 13:40:39.228057 fedex-sdk-0.0.3/fedex_sdk.egg-info/
+-rw-rw-rw-   0        0        0      326 2023-07-21 13:40:38.000000 fedex-sdk-0.0.3/fedex_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-07-21 13:40:39.000000 fedex-sdk-0.0.3/fedex_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 13:40:38.000000 fedex-sdk-0.0.3/fedex_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-21 13:40:38.000000 fedex-sdk-0.0.3/fedex_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 13:40:39.228057 fedex-sdk-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      559 2023-07-21 08:44:20.000000 fedex-sdk-0.0.3/setup.py
```

### Comparing `fedex-sdk-0.0.2/FedexSDK/FedExSDK.py` & `fedex-sdk-0.0.3/FedexSDK/FedExSDK.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 import json
 import os
 from dataclasses import dataclass
 from requests_oauthlib import OAuth2Session
 import requests
+from FedexSDK.models import Request
 
 @dataclass
 class APIType:
     Production: str = "Production"
     Test: str = "Test"
 
 @dataclass
@@ -23,27 +24,26 @@
         
         self.session = session
         self.headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {session.access_token}"
         }
 
-    def create_shipment(self, data: dict):
+    def create_shipment(self, request: Request, output_json_path: str):
         url = "https://apis.fedex.com/ship/v1/shipments"
 
-        res = self.session.post(url, json=data, headers=self.headers)
+        res = self.session.post(url, json=request.dict(), headers=self.headers)
         
         now_date = datetime.datetime.now()
-        print(res.json())
         with open(f"{now_date.strftime('%d_%m_%Y_tracking_numbers.txt')}", "a") as f:
             f.write(
                 f"{res.json()['output']['transactionShipments'][0]['shipmentDocuments'][0]['trackingNumber']}:{data['requestedShipment']['recipients'][0]['contact']['personName']}\n"
             )
         
-        json.dump(res.json(), open("data.json", "w", encoding="utf-8"), ensure_ascii=False)
+        json.dump(res.json(), open(output_json_path, "w", encoding="utf-8"), ensure_ascii=False)
 
     
     def add_image(self, reference_id: str, image_name: str, image_index: str, image_type: ImageType, image_path: str):
         name, ext = os.path.splitext(image_path)
         data = {
             "document": {
                 "referenceId": reference_id,
@@ -63,16 +63,15 @@
         }
         url = "https://documentapi.prod.fedex.com/documents/v1/lhsimages/upload"
         
         headers = self.headers
         headers["Content-Type"] = "multipart/form-data"
         
         res = self.session.post(url, data=data, headers=headers, files=files)
-        print(res.json())
-    
+        
     @classmethod
     def authorize(cls, client_id: str, client_secret: str, api_type: APIType = APIType.Test) -> OAuth2Session:
         if api_type == APIType.Production:
             url = "https://apis.fedex.com/oauth/token"
         elif api_type == APIType.Test:
             url = "https://apis.sandbox.fedex.com/oauth/token"
         else:
@@ -84,11 +83,10 @@
         data = {
             "grant_type": "client_credentials",
             "client_id": client_id,
             "client_secret": client_secret
         }
 
         response = requests.request("POST", url, data=data, headers=headers)
-        print(response.json())
         return OAuth2Session(client_id=client_id, token=response.json())
```

### Comparing `fedex-sdk-0.0.2/FedexSDK/models/Address.py` & `fedex-sdk-0.0.3/FedexSDK/models/Address.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.2/FedexSDK/models/Contact.py` & `fedex-sdk-0.0.3/FedexSDK/models/Contact.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.2/FedexSDK/models/Request.py` & `fedex-sdk-0.0.3/FedexSDK/models/Request.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.2/FedexSDK/models/RequestedShipment.py` & `fedex-sdk-0.0.3/FedexSDK/models/RequestedShipment.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.2/FedexSDK/models/Tin.py` & `fedex-sdk-0.0.3/FedexSDK/models/Tin.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.2/FedexSDK/models/__init__.py` & `fedex-sdk-0.0.3/FedexSDK/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.2/setup.py` & `fedex-sdk-0.0.3/setup.py`

 * *Files identical despite different names*

