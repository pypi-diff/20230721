# Comparing `tmp/amfiprot-0.1.1.tar.gz` & `tmp/amfiprot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amfiprot-0.1.1.tar", last modified: Wed Apr  5 07:33:49 2023, max compression
+gzip compressed data, was "amfiprot-0.1.2.tar", last modified: Fri Jul 21 06:55:16 2023, max compression
```

## Comparing `amfiprot-0.1.1.tar` & `amfiprot-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 07:33:49.565587 amfiprot-0.1.1/
--rw-rw-rw-   0        0        0     1057 2023-02-24 09:52:55.000000 amfiprot-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     6026 2023-04-05 07:33:49.565587 amfiprot-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5614 2023-02-24 09:52:55.000000 amfiprot-0.1.1/README.md
--rw-rw-rw-   0        0        0      110 2023-02-24 09:52:55.000000 amfiprot-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      650 2023-04-05 07:33:49.570588 amfiprot-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-05 07:33:49.539582 amfiprot-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-05 07:33:49.551584 amfiprot-0.1.1/src/amfiprot/
--rw-rw-rw-   0        0        0      351 2023-04-05 07:33:28.000000 amfiprot-0.1.1/src/amfiprot/__init__.py
--rw-rw-rw-   0        0        0    30466 2023-04-05 07:01:28.000000 amfiprot-0.1.1/src/amfiprot/common_payload.py
--rw-rw-rw-   0        0        0     4566 2023-02-24 09:52:55.000000 amfiprot-0.1.1/src/amfiprot/configurator.py
--rw-rw-rw-   0        0        0     1227 2023-02-24 09:52:55.000000 amfiprot-0.1.1/src/amfiprot/connection.py
--rw-rw-rw-   0        0        0     5293 2023-02-24 09:52:55.000000 amfiprot-0.1.1/src/amfiprot/device.py
--rw-rw-rw-   0        0        0     2253 2023-02-24 09:52:55.000000 amfiprot-0.1.1/src/amfiprot/node.py
--rw-rw-rw-   0        0        0     5960 2023-02-24 09:52:55.000000 amfiprot-0.1.1/src/amfiprot/packet.py
--rw-rw-rw-   0        0        0     1728 2023-02-24 09:52:55.000000 amfiprot-0.1.1/src/amfiprot/payload.py
--rw-rw-rw-   0        0        0     1593 2023-02-24 09:52:55.000000 amfiprot-0.1.1/src/amfiprot/response_payload.py
--rw-rw-rw-   0        0        0    15567 2023-02-24 09:52:55.000000 amfiprot-0.1.1/src/amfiprot/usb_connection.py
-drwxrwxrwx   0        0        0        0 2023-04-05 07:33:49.564587 amfiprot-0.1.1/src/amfiprot.egg-info/
--rw-rw-rw-   0        0        0     6026 2023-04-05 07:33:49.000000 amfiprot-0.1.1/src/amfiprot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      488 2023-04-05 07:33:49.000000 amfiprot-0.1.1/src/amfiprot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 07:33:49.000000 amfiprot-0.1.1/src/amfiprot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-05 07:33:49.000000 amfiprot-0.1.1/src/amfiprot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-05 07:33:49.000000 amfiprot-0.1.1/src/amfiprot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 06:55:16.861455 amfiprot-0.1.2/
+-rw-rw-rw-   0        0        0     1057 2023-07-21 06:35:46.000000 amfiprot-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     6026 2023-07-21 06:55:16.861455 amfiprot-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5614 2023-07-21 06:40:05.000000 amfiprot-0.1.2/README.md
+-rw-rw-rw-   0        0        0      110 2023-07-21 06:35:46.000000 amfiprot-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      650 2023-07-21 06:55:16.862456 amfiprot-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-21 06:55:16.804833 amfiprot-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-21 06:55:16.833353 amfiprot-0.1.2/src/amfiprot/
+-rw-rw-rw-   0        0        0      351 2023-07-21 06:41:10.000000 amfiprot-0.1.2/src/amfiprot/__init__.py
+-rw-rw-rw-   0        0        0    31174 2023-07-21 06:35:46.000000 amfiprot-0.1.2/src/amfiprot/common_payload.py
+-rw-rw-rw-   0        0        0     4566 2023-07-21 06:35:46.000000 amfiprot-0.1.2/src/amfiprot/configurator.py
+-rw-rw-rw-   0        0        0     1227 2023-07-21 06:35:46.000000 amfiprot-0.1.2/src/amfiprot/connection.py
+-rw-rw-rw-   0        0        0     5293 2023-07-21 06:35:46.000000 amfiprot-0.1.2/src/amfiprot/device.py
+-rw-rw-rw-   0        0        0     2253 2023-07-21 06:35:46.000000 amfiprot-0.1.2/src/amfiprot/node.py
+-rw-rw-rw-   0        0        0     5960 2023-07-21 06:35:46.000000 amfiprot-0.1.2/src/amfiprot/packet.py
+-rw-rw-rw-   0        0        0     1728 2023-07-21 06:35:46.000000 amfiprot-0.1.2/src/amfiprot/payload.py
+-rw-rw-rw-   0        0        0     1593 2023-07-21 06:35:46.000000 amfiprot-0.1.2/src/amfiprot/response_payload.py
+-rw-rw-rw-   0        0        0    15567 2023-07-21 06:35:46.000000 amfiprot-0.1.2/src/amfiprot/usb_connection.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:55:16.860462 amfiprot-0.1.2/src/amfiprot.egg-info/
+-rw-rw-rw-   0        0        0     6026 2023-07-21 06:55:16.000000 amfiprot-0.1.2/src/amfiprot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      488 2023-07-21 06:55:16.000000 amfiprot-0.1.2/src/amfiprot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 06:55:16.000000 amfiprot-0.1.2/src/amfiprot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-21 06:55:16.000000 amfiprot-0.1.2/src/amfiprot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-21 06:55:16.000000 amfiprot-0.1.2/src/amfiprot.egg-info/top_level.txt
```

### Comparing `amfiprot-0.1.1/LICENSE` & `amfiprot-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `amfiprot-0.1.1/PKG-INFO` & `amfiprot-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amfiprot
-Version: 0.1.1
+Version: 0.1.2
 Summary: Core library for Amfiprot
 Author: Kristian Klein-Wengel
 Author-email: kkw@amfitech.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Requires-Python: >=3.7
@@ -82,15 +82,15 @@
 ```python
 import amfiprot
 
 VENDOR_ID = 0xC17
 PRODUCT_ID = 0xD12
 
 if __name__ == "__main__":
-    conn = amfiprot.UsbConnection(VENDOR_ID, PRODUCT_ID)
+    conn = amfiprot.USBConnection(VENDOR_ID, PRODUCT_ID)
     nodes = conn.find_nodes()
 
     print(f"Found {len(nodes)} node(s).")
     for node in nodes:
         print(f"[{node.tx_id}] {node.name}")
 
     dev = amfiprot.Device(nodes[0])
@@ -106,24 +106,24 @@
 The following sections provide a more in-depth explanation.
 
 ## Discovering and connecting to a root node
 
 After attaching a device to your host machine, you can scan for connected devices (e.g. connected via USB) with:
 
 ```python
-phys_devs = amfiprot.UsbConnection.discover()
+phys_devs = amfiprot.USBConnection.discover()
 
 for dev in phys_devs:
     print(dev)
 ```
 
 A connection can then be created using a specific physical device:
 
 ```python
-conn = amfiprot.UsbConnection(dev['vid'], dev['pid'], dev['serial_number'])
+conn = amfiprot.USBConnection(dev['vid'], dev['pid'], dev['serial_number'])
 ```
 
 Using `serial_number` is optional. If none is given, the first device matching the given vendor and product ID is used.
 
 ## Finding nodes
 
 After creating a connection, we can search for nodes that are connected to the root node (e.g. via RF or UART):
```

### Comparing `amfiprot-0.1.1/README.md` & `amfiprot-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 ```python
 import amfiprot
 
 VENDOR_ID = 0xC17
 PRODUCT_ID = 0xD12
 
 if __name__ == "__main__":
-    conn = amfiprot.UsbConnection(VENDOR_ID, PRODUCT_ID)
+    conn = amfiprot.USBConnection(VENDOR_ID, PRODUCT_ID)
     nodes = conn.find_nodes()
 
     print(f"Found {len(nodes)} node(s).")
     for node in nodes:
         print(f"[{node.tx_id}] {node.name}")
 
     dev = amfiprot.Device(nodes[0])
@@ -93,24 +93,24 @@
 The following sections provide a more in-depth explanation.
 
 ## Discovering and connecting to a root node
 
 After attaching a device to your host machine, you can scan for connected devices (e.g. connected via USB) with:
 
 ```python
-phys_devs = amfiprot.UsbConnection.discover()
+phys_devs = amfiprot.USBConnection.discover()
 
 for dev in phys_devs:
     print(dev)
 ```
 
 A connection can then be created using a specific physical device:
 
 ```python
-conn = amfiprot.UsbConnection(dev['vid'], dev['pid'], dev['serial_number'])
+conn = amfiprot.USBConnection(dev['vid'], dev['pid'], dev['serial_number'])
 ```
 
 Using `serial_number` is optional. If none is given, the first device matching the given vendor and product ID is used.
 
 ## Finding nodes
 
 After creating a connection, we can search for nodes that are connected to the root node (e.g. via RF or UART):
```

### Comparing `amfiprot-0.1.1/setup.cfg` & `amfiprot-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `amfiprot-0.1.1/src/amfiprot/common_payload.py` & `amfiprot-0.1.2/src/amfiprot/common_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     REPLY_CONFIGURATION_VALUE_COUNT = 0x19
     REQUEST_CATEGORY_COUNT = 0x1A
     REPLY_CATEGORY_COUNT = 0x1B
     REQUEST_FIRMWARE_VERSION_PER_ID = 0x1C
     REPLY_FIRMWARE_VERSION_PER_ID = 0x1D
     DEBUG_OUTPUT = 0x20
     REBOOT = 0x21
+    RESET_PARAMETER = 0x24
 
 
 class ConfigValueType(enum.IntEnum):
     BOOL = 0
     CHAR = 1
     INT8 = 2
     UINT8 = 3
@@ -349,14 +350,34 @@
         return self.data
 
     def to_dict(self):
         return {
             'payload_id': self.data[0]
         }
 
+class ResetParameterPayload(CommonPayload):
+    def __init__(self, ResetParameter: int = 0):
+        self.data = array.array('B', [CommonPayloadId.RESET_PARAMETER, ResetParameter])
+
+    @classmethod
+    def from_bytes(cls, data):
+        ResetParameter = data[1]
+        return RequestFirmwareVersionPerIdPayload(ResetParameter)
+
+    def __len__(self):
+        return len(self.data)
+
+    def to_bytes(self):
+        return self.data
+
+    def to_dict(self):
+        return {
+            'payload_id': CommonPayloadId.RESET_PARAMETER,
+            'resetParameter_id': self.data[1]
+        }
 
 class RequestCategoryCountPayload(CommonPayload):
     def __init__(self):
         self.data = array.array('B', [CommonPayloadId.REQUEST_CATEGORY_COUNT])
 
     @classmethod
     def from_bytes(cls, data):
@@ -681,15 +702,15 @@
     def to_dict(self):
         return {
             'payload_id': CommonPayloadId.LOAD_DEFAULT
         }
 
 class SaveAsDefaultConfigurationPayload(CommonPayload):
     def __init__(self):
-        self.data = array.array('B', CommonPayloadId.SAVE_AS_DEFAULT)
+        self.data = array.array('B', [CommonPayloadId.SAVE_AS_DEFAULT])
 
     @classmethod
     def from_bytes(cls, data):
         return SaveAsDefaultConfigurationPayload()
 
     def __len__(self):
         return len(self.data)
@@ -894,15 +915,16 @@
             CommonPayloadId.LOAD_DEFAULT: LoadDefaultConfigurationPayload,
             CommonPayloadId.SET_CONFIGURATION_VALUE_UID: SetConfigurationValueUidPayload,
             CommonPayloadId.SAVE_AS_DEFAULT: SaveAsDefaultConfigurationPayload,
             CommonPayloadId.FIRMWARE_START: FirmwareStartPayload,
             CommonPayloadId.FIRMWARE_DATA:FirmwareDataPayload,
             CommonPayloadId.FIRMWARE_END: FirmwareEndPayload,
             CommonPayloadId.REQUEST_FIRMWARE_VERSION_PER_ID: RequestFirmwareVersionPerIdPayload,
-            CommonPayloadId.REPLY_FIRMWARE_VERSION_PER_ID: ReplyFirmwareVersionPerIdPayload
+            CommonPayloadId.REPLY_FIRMWARE_VERSION_PER_ID: ReplyFirmwareVersionPerIdPayload,
+            CommonPayloadId.RESET_PARAMETER: ResetParameterPayload
         }
 
 
 def create_common_payload(data) -> Payload:
     payload_id = data[0]
     if payload_id in payload_ids:
         return payload_ids[payload_id].from_bytes(data)  # type: ignore
```

### Comparing `amfiprot-0.1.1/src/amfiprot/configurator.py` & `amfiprot-0.1.2/src/amfiprot/configurator.py`

 * *Files identical despite different names*

### Comparing `amfiprot-0.1.1/src/amfiprot/connection.py` & `amfiprot-0.1.2/src/amfiprot/connection.py`

 * *Files identical despite different names*

### Comparing `amfiprot-0.1.1/src/amfiprot/device.py` & `amfiprot-0.1.2/src/amfiprot/device.py`

 * *Files identical despite different names*

### Comparing `amfiprot-0.1.1/src/amfiprot/node.py` & `amfiprot-0.1.2/src/amfiprot/node.py`

 * *Files identical despite different names*

### Comparing `amfiprot-0.1.1/src/amfiprot/packet.py` & `amfiprot-0.1.2/src/amfiprot/packet.py`

 * *Files identical despite different names*

### Comparing `amfiprot-0.1.1/src/amfiprot/payload.py` & `amfiprot-0.1.2/src/amfiprot/payload.py`

 * *Files identical despite different names*

### Comparing `amfiprot-0.1.1/src/amfiprot/response_payload.py` & `amfiprot-0.1.2/src/amfiprot/response_payload.py`

 * *Files identical despite different names*

### Comparing `amfiprot-0.1.1/src/amfiprot/usb_connection.py` & `amfiprot-0.1.2/src/amfiprot/usb_connection.py`

 * *Files identical despite different names*

### Comparing `amfiprot-0.1.1/src/amfiprot.egg-info/PKG-INFO` & `amfiprot-0.1.2/src/amfiprot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amfiprot
-Version: 0.1.1
+Version: 0.1.2
 Summary: Core library for Amfiprot
 Author: Kristian Klein-Wengel
 Author-email: kkw@amfitech.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Requires-Python: >=3.7
@@ -82,15 +82,15 @@
 ```python
 import amfiprot
 
 VENDOR_ID = 0xC17
 PRODUCT_ID = 0xD12
 
 if __name__ == "__main__":
-    conn = amfiprot.UsbConnection(VENDOR_ID, PRODUCT_ID)
+    conn = amfiprot.USBConnection(VENDOR_ID, PRODUCT_ID)
     nodes = conn.find_nodes()
 
     print(f"Found {len(nodes)} node(s).")
     for node in nodes:
         print(f"[{node.tx_id}] {node.name}")
 
     dev = amfiprot.Device(nodes[0])
@@ -106,24 +106,24 @@
 The following sections provide a more in-depth explanation.
 
 ## Discovering and connecting to a root node
 
 After attaching a device to your host machine, you can scan for connected devices (e.g. connected via USB) with:
 
 ```python
-phys_devs = amfiprot.UsbConnection.discover()
+phys_devs = amfiprot.USBConnection.discover()
 
 for dev in phys_devs:
     print(dev)
 ```
 
 A connection can then be created using a specific physical device:
 
 ```python
-conn = amfiprot.UsbConnection(dev['vid'], dev['pid'], dev['serial_number'])
+conn = amfiprot.USBConnection(dev['vid'], dev['pid'], dev['serial_number'])
 ```
 
 Using `serial_number` is optional. If none is given, the first device matching the given vendor and product ID is used.
 
 ## Finding nodes
 
 After creating a connection, we can search for nodes that are connected to the root node (e.g. via RF or UART):
```

