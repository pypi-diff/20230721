# Comparing `tmp/bitcoin_qrreader-0.1.2.tar.gz` & `tmp/bitcoin_qrreader-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitcoin_qrreader-0.1.2.tar", last modified: Thu Jul 20 18:02:14 2023, max compression
+gzip compressed data, was "bitcoin_qrreader-0.2.1.tar", last modified: Fri Jul 21 18:04:58 2023, max compression
```

## Comparing `bitcoin_qrreader-0.1.2.tar` & `bitcoin_qrreader-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,53 @@
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-20 18:02:14.117302 bitcoin_qrreader-0.1.2/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    35149 2023-06-09 17:54:40.000000 bitcoin_qrreader-0.1.2/LICENSE
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1128 2023-07-20 18:02:14.117302 bitcoin_qrreader-0.1.2/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      646 2023-07-20 17:59:03.000000 bitcoin_qrreader-0.1.2/README.md
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-20 18:02:14.117302 bitcoin_qrreader-0.1.2/bitcoin_qrreader/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        0 2023-07-20 11:25:47.000000 bitcoin_qrreader-0.1.2/bitcoin_qrreader/__init__.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    15502 2023-07-20 11:27:13.000000 bitcoin_qrreader-0.1.2/bitcoin_qrreader/bitcoin_qr.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1239 2023-07-20 11:32:56.000000 bitcoin_qrreader-0.1.2/bitcoin_qrreader/bitcoin_qr_gui.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     3689 2023-07-19 13:09:39.000000 bitcoin_qrreader-0.1.2/bitcoin_qrreader/qr_qui.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-20 18:02:14.117302 bitcoin_qrreader-0.1.2/bitcoin_qrreader.egg-info/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1128 2023-07-20 18:02:14.000000 bitcoin_qrreader-0.1.2/bitcoin_qrreader.egg-info/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      347 2023-07-20 18:02:14.000000 bitcoin_qrreader-0.1.2/bitcoin_qrreader.egg-info/SOURCES.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2023-07-20 18:02:14.000000 bitcoin_qrreader-0.1.2/bitcoin_qrreader.egg-info/dependency_links.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       47 2023-07-20 18:02:14.000000 bitcoin_qrreader-0.1.2/bitcoin_qrreader.egg-info/requires.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       17 2023-07-20 18:02:14.000000 bitcoin_qrreader-0.1.2/bitcoin_qrreader.egg-info/top_level.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2023-07-20 18:02:14.117302 bitcoin_qrreader-0.1.2/setup.cfg
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1077 2023-07-20 18:01:39.000000 bitcoin_qrreader-0.1.2/setup.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-21 18:04:58.463288 bitcoin_qrreader-0.2.1/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    35149 2023-06-09 17:54:40.000000 bitcoin_qrreader-0.2.1/LICENSE
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2854 2023-07-21 11:50:05.000000 bitcoin_qrreader-0.2.1/LICENSE_UR
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1291 2023-07-21 18:04:58.463288 bitcoin_qrreader-0.2.1/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      784 2023-07-21 17:29:28.000000 bitcoin_qrreader-0.2.1/README.md
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-21 18:04:58.455288 bitcoin_qrreader-0.2.1/bitcoin_qrreader/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        0 2023-07-20 11:25:47.000000 bitcoin_qrreader-0.2.1/bitcoin_qrreader/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    21558 2023-07-21 17:53:15.000000 bitcoin_qrreader-0.2.1/bitcoin_qrreader/bitcoin_qr.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1366 2023-07-21 11:27:49.000000 bitcoin_qrreader-0.2.1/bitcoin_qrreader/bitcoin_qr_gui.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     3691 2023-07-21 14:47:36.000000 bitcoin_qrreader-0.2.1/bitcoin_qrreader/qr_qui.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-21 18:04:58.455288 bitcoin_qrreader-0.2.1/bitcoin_qrreader.egg-info/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1291 2023-07-21 18:04:58.000000 bitcoin_qrreader-0.2.1/bitcoin_qrreader.egg-info/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1001 2023-07-21 18:04:58.000000 bitcoin_qrreader-0.2.1/bitcoin_qrreader.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2023-07-21 18:04:58.000000 bitcoin_qrreader-0.2.1/bitcoin_qrreader.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       47 2023-07-21 18:04:58.000000 bitcoin_qrreader-0.2.1/bitcoin_qrreader.egg-info/requires.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       28 2023-07-21 18:04:58.000000 bitcoin_qrreader-0.2.1/bitcoin_qrreader.egg-info/top_level.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2023-07-21 18:04:58.463288 bitcoin_qrreader-0.2.1/setup.cfg
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1075 2023-07-21 18:04:12.000000 bitcoin_qrreader-0.2.1/setup.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-21 18:04:58.459288 bitcoin_qrreader-0.2.1/ur/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        0 2023-07-21 11:50:05.000000 bitcoin_qrreader-0.2.1/ur/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     4940 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.1/ur/bytewords.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    11377 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.1/ur/cbor_lite.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      179 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.1/ur/constants.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      729 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.1/ur/crc32.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     9669 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.1/ur/fountain_decoder.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     4978 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.1/ur/fountain_encoder.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1603 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.1/ur/fountain_utils.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1568 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.1/ur/random_sampler.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      491 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.1/ur/ur.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     5115 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.1/ur/ur_decoder.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2038 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.1/ur/ur_encoder.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1638 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.1/ur/utils.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     4440 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.1/ur/xoshiro256.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-21 18:04:58.459288 bitcoin_qrreader-0.2.1/urtypes/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1157 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.1/urtypes/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1580 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.1/urtypes/bytes.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-21 18:04:58.459288 bitcoin_qrreader-0.2.1/urtypes/cbor/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1247 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.1/urtypes/cbor/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2213 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.1/urtypes/cbor/data.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     6660 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.1/urtypes/cbor/decoder.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     4937 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.1/urtypes/cbor/encoder.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-21 18:04:58.463288 bitcoin_qrreader-0.2.1/urtypes/crypto/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1315 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.1/urtypes/crypto/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2370 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.1/urtypes/crypto/account.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1842 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.1/urtypes/crypto/bip39.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1951 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.1/urtypes/crypto/coin_info.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2238 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.1/urtypes/crypto/ec_key.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     9315 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.1/urtypes/crypto/hd_key.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     3747 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.1/urtypes/crypto/keypath.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2467 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.1/urtypes/crypto/multi_key.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     6360 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.1/urtypes/crypto/output.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1293 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.1/urtypes/crypto/psbt.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2288 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.1/urtypes/registry.py
```

### Comparing `bitcoin_qrreader-0.1.2/LICENSE` & `bitcoin_qrreader-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.1.2/PKG-INFO` & `bitcoin_qrreader-0.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: bitcoin_qrreader
-Version: 0.1.2
+Version: 0.2.1
 Summary: Bitcoin qr reader
 Home-page: https://github.com/andreasgriffin/bitcoin-qrreader
 Author: Andreas Griffin
 Author-email: andreasgriffin@proton.me
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7,<4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: LICENSE_UR
 
 # A python bitcoin qr reader
 
 * Recognizes (and classifies)
   * Addresses  (also BIP21 with amount)
   * Transactions (also base43 electrum encoding)
   * PSBT
   * Xpub
   * Descriptor
   * Partial descriptors (Specter DIY) ( finger print , derivation, xpub)
   * TxId
+  * Animated QR Codes ([UR](https://github.com/BlockchainCommons/Research/blob/master/papers/bcr-2020-005-ur.md)) (Transactions and Descriptors)
+  * Animated QR Codes (Specter)
 * **blazingly fast** recognition
-* bdkpython as only bitcoin dependency
 * SLIP132 -> to BIP32 conversion
 
 ### Demo
 
 Run the demo with
 
 ```
```

### Comparing `bitcoin_qrreader-0.1.2/README.md` & `bitcoin_qrreader-0.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,17 @@
   * Addresses  (also BIP21 with amount)
   * Transactions (also base43 electrum encoding)
   * PSBT
   * Xpub
   * Descriptor
   * Partial descriptors (Specter DIY) ( finger print , derivation, xpub)
   * TxId
+  * Animated QR Codes ([UR](https://github.com/BlockchainCommons/Research/blob/master/papers/bcr-2020-005-ur.md)) (Transactions and Descriptors)
+  * Animated QR Codes (Specter)
 * **blazingly fast** recognition
-* bdkpython as only bitcoin dependency
 * SLIP132 -> to BIP32 conversion
 
 ### Demo
 
 Run the demo with
 
 ```
```

### Comparing `bitcoin_qrreader-0.1.2/bitcoin_qrreader/bitcoin_qr.py` & `bitcoin_qrreader-0.2.1/bitcoin_qrreader/bitcoin_qr.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import re, urllib
-from typing import List, Callable, Union, Optional
+from typing import List, Callable, Union, Optional, Tuple, Dict
 from decimal import Decimal
 import bdkpython as bdk
-import base64
+import base64, json
+from urtypes.crypto import PSBT as UR_PSBT
+from urtypes.crypto import Output as US_OUTPUT
+from ur.ur_decoder import URDecoder
+from urtypes.bytes import Bytes as UR_BYTES
 
 
 def is_bitcoin_address(s):
     if re.search(r"^bitcoin\:.*", s, re.IGNORECASE):
         return True
     elif re.search(r"^((bc1|tb1|bcr|[123]|[mn])[a-zA-HJ-NP-Z0-9]{25,62})$", s):
         # TODO: Handle regtest bcrt?
@@ -394,20 +398,29 @@
                 return Data(convert_slip132_to_bip32(s), DataType.Xpub)
             return Data(s, DataType.Xpub)
 
         # try descriptor
         descriptor = None
         try:
             descriptor = bdk.Descriptor(s, network)
+            if descriptor:
+                print("detected descriptor")
+                return Data(descriptor, DataType.Descriptor)
         except:
             pass
 
-        if descriptor:
-            print("detected descriptor")
-            return Data(descriptor, DataType.Descriptor)
+        # try if it is a dict containing a descriptor
+        try:
+            specter_dict = json.loads(s)
+            if "descriptor" in specter_dict:
+                descriptor = bdk.Descriptor(specter_dict["descriptor"], network)
+                print("detected descriptor")
+                return Data(descriptor, DataType.Descriptor)
+        except:
+            pass
 
         # try txid
         if is_valid_bitcoin_hash(s):
             return Data(s, DataType.Txid)
 
         # try txid
         if is_valid_wallet_fingerprint(s):
@@ -463,15 +476,15 @@
                         )
 
                     # Check if decoded string starts with the magic bytes for PSBT
                     return Data(bdk.Transaction(tx_bytes), DataType.Tx)
                 except:
                     pass
 
-        # try specter partial descriptor
+        # try specter DIY partial descriptor
         keystore_info = None
         try:
             keystore_info = extract_keystore(s)
         except:
             pass
 
         if keystore_info:
@@ -479,9 +492,189 @@
 
             if is_slip132(keystore_info.get("xpub")):
                 keystore_info["xpub"] = convert_slip132_to_bip32(
                     keystore_info.get("xpub")
                 )
             return Data(keystore_info, DataType.KeyStoreInfo)
 
-        raise Exception("Could not be decoded")
+        # tries to use json to decode and recognize keystore infos
+        # used by cobo vault
+        # s = """{"xfp":"7cf42c8e","xpub":"tpubDE5U4jVviWBZ9iXA7ZEpYR8FM1oce2N2Pv16mfVjr7q9WRR2DJva6co8acMLAmhm8kkMJsFMRmaHL8v6rzc81hsvgcVzc3MTSfnrtwYZMMy","path":"m\/48'\/0'\/0'\/2'"}"""
+        try:
+            cobo_dict = json.loads(s)
+            keystore_info = {}
+            key_map = {"fingerprint": "xfp", "derivation_path": "path", "xpub": "xpub"}
+            for key, cobo_key in key_map.items():
+                if cobo_key in cobo_dict:
+                    keystore_info[key] = cobo_dict[cobo_key]
+                if key in cobo_dict:
+                    keystore_info[key] = cobo_dict[key]
+            if keystore_info:
+                return Data(keystore_info, DataType.KeyStoreInfo)
+        except:
+            pass
+
+        raise Exception(f"{s} Could not be decoded")
+
+
+class BaseCollector:
+    def __init__(self, network) -> None:
+        self.data: Data = None
+        self.network = network
+
+    def is_correct_data_format(self, s):
+        pass
+
+    def is_complete(self) -> bool:
+        pass
+
+    def get_complete_data(self) -> Data:
+        pass
+
+    def add(self, s: str):
+        pass
+
+    def clear(self):
+        self.data = None
+
+
+class SinglePassCollector(BaseCollector):
+    def is_correct_data_format(self, s):
+        return True
+
+    def is_complete(self) -> bool:
+        return True
+
+    def get_complete_data(self) -> Data:
+        return self.data
+
+    def add(self, s: str):
+        self.data = Data.from_str(s, network=self.network)
+        return self.data
+
+
+class SpecterDIYCollector(BaseCollector):
+    def __init__(self, network) -> None:
+        super().__init__(network)
+        self.clear()
+
+    def is_correct_data_format(self, s):
+        return self.extract_specter_diy_qr_part(s) is not None
+
+    def is_complete(self) -> bool:
+        return len(self.parts) == self.total_parts
+
+    def get_complete_data(self) -> Data:
+        if not self.is_complete():
+            return None
+
+        total_s = ""
+        for i in range(1, self.total_parts + 1):
+            total_s += self.parts[i]
+        return Data.from_str(total_s, network=self.network)
+
+    def extract_specter_diy_qr_part(self, s) -> Tuple[int, int, str]:
+        "pMofM something  ->  (M,N,something)"
+        pattern = r"^p(\d+)of(\d+)\s(.*)"
+        match = re.match(pattern, s)
+        if match:
+            return int(match.group(1)), int(match.group(2)), match.group(3)
+        else:
+            return None
+
+    def add(self, s: str):
+        m, n, data = self.extract_specter_diy_qr_part(s)
+        if self.total_parts is None:
+            self.total_parts = n
+        else:
+            assert n == self.total_parts
+
+        self.parts[m] = data
+        return data
+
+    def clear(self):
+        super().clear()
+        self.parts: Dict[int, str] = {}
+        self.total_parts = None
+
+
+class URCollector(BaseCollector):
+    def __init__(self, network) -> None:
+        super().__init__(network)
+        self.clear()
+
+    def is_psbt(self, s: str):
+        return re.search("^UR:CRYPTO-PSBT/", s, re.IGNORECASE)
+
+    def is_descriptor(self, s: str):
+        return re.search("^UR:CRYPTO-OUTPUT/", s, re.IGNORECASE)
+
+    def is_descriptor(self, s: str):
+        return re.search("^UR:CRYPTO-OUTPUT/", s, re.IGNORECASE)
+
+    def is_bytes(self, s: str):
+        return re.search("^UR:BYTES/", s, re.IGNORECASE)
+
+    def is_correct_data_format(self, s):
+        if self.is_psbt(s):
+            return True
+        if self.is_descriptor(s):
+            return True
+        if self.is_bytes(s):
+            return True
+
+        return False
+
+    def is_complete(self) -> bool:
+        return self.decoder.is_complete()
 
+    def get_complete_data(self) -> Data:
+        if self.decoder.result.type == "crypto-psbt":
+            qr_content = UR_PSBT.from_cbor(self.decoder.result.cbor).data
+            s = base64.b64encode(qr_content).decode("utf-8")
+        if self.decoder.result.type == "crypto-output":
+            s = US_OUTPUT.from_cbor(self.decoder.result.cbor).descriptor()
+        if self.decoder.result.type == "bytes":
+            raw = UR_BYTES.from_cbor(self.decoder.result.cbor).data
+            s = raw.hex()
+
+        return Data.from_str(s, network=self.network)
+
+    def add(self, s: str):
+        self.decoder.receive_part(s)
+        print(f"{round(self.decoder.estimated_percent_complete()*100)}% complete")
+        return s
+
+    def clear(self):
+        super().clear()
+        self.decoder = URDecoder()
+
+
+class MetaDataHandler:
+    "Unified class to handle animated and static qr codes"
+
+    def __init__(self, network) -> None:
+        self.network = network
+        # SinglePassCollector must be the last one
+        self.collectors: List[BaseCollector] = [
+            URCollector(self.network),
+            SpecterDIYCollector(self.network),
+            SinglePassCollector(self.network),
+        ]
+        self.last_used_collector = None
+
+    def get_collector(self, s: str):
+        for collector in self.collectors:
+            if collector.is_correct_data_format(s):
+                return collector
+
+    def add(self, s: str):
+        self.last_used_collector = self.get_collector(s)
+        return self.last_used_collector.add(s)
+
+    def is_complete(self) -> bool:
+        return self.last_used_collector.is_complete()
+
+    def get_complete_data(self) -> Data:
+        data = self.last_used_collector.get_complete_data()
+        self.last_used_collector.clear()
+        return data
```

### Comparing `bitcoin_qrreader-0.1.2/bitcoin_qrreader/bitcoin_qr_gui.py` & `bitcoin_qrreader-0.2.1/bitcoin_qrreader/bitcoin_qr_gui.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 from .qr_qui import VideoWidget
 from .bitcoin_qr import *
 from PySide2 import QtWidgets
+from typing import Dict
 
 
 class BitcoinVideoWidget(VideoWidget):
     def __init__(
         self,
         result_callback=None,
         close_on_result=True,
         parent=None,
         network=bdk.Network.REGTEST,
     ):
         super().__init__(qr_data_callback=self.qr_data_callback, parent=parent)
 
         self.network = network
-        self.data = None
         self.result_callback = result_callback
         self.close_on_result = close_on_result
+        
+        self.meta_data_handler = MetaDataHandler(self.network)
+        
 
     def qr_data_callback(self, qr_data):
-        data = Data.from_str(qr_data.decode("utf-8"), network=self.network)
+        self.meta_data_handler.add(qr_data.decode("utf-8"))
+            
+        if self.meta_data_handler.is_complete():
+            if self.close_on_result:
+                self.close()
+            if self.result_callback:
+                self.result_callback(self.meta_data_handler.get_complete_data())
 
-        if not data:
-            return
-
-        self.data = data
-        if self.close_on_result:
-            self.close()
-        if self.result_callback:
-            self.result_callback(data)
+            
 
 
 
 
 class DemoBitcoinVideoWidget(BitcoinVideoWidget):
     def __init__(self, parent=None, close_on_result=False,):
         super().__init__(result_callback=self.result_callback, parent=parent, close_on_result=close_on_result)
```

### Comparing `bitcoin_qrreader-0.1.2/bitcoin_qrreader/qr_qui.py` & `bitcoin_qrreader-0.2.1/bitcoin_qrreader/qr_qui.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         self.qr_data_callback = qr_data_callback
         self.signal_qr_data_callback.connect(qr_data_callback)
 
         pygame.camera.init()
         self.cameras = self.get_valid_cameras()
         self.combo_cameras = QtWidgets.QComboBox()
         self.combo_cameras.addItems(self.cameras)
-        self.combo_cameras.currentIndexChanged.connect(qr_data_callback)
+        self.combo_cameras.currentIndexChanged.connect(self.switch_camera)
 
         layout = QtWidgets.QVBoxLayout()
         layout.addWidget(self.label_image)
         layout.addWidget(self.combo_cameras)
 
         self.setLayout(layout)
```

### Comparing `bitcoin_qrreader-0.1.2/bitcoin_qrreader.egg-info/PKG-INFO` & `bitcoin_qrreader-0.2.1/bitcoin_qrreader.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: bitcoin-qrreader
-Version: 0.1.2
+Version: 0.2.1
 Summary: Bitcoin qr reader
 Home-page: https://github.com/andreasgriffin/bitcoin-qrreader
 Author: Andreas Griffin
 Author-email: andreasgriffin@proton.me
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7,<4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: LICENSE_UR
 
 # A python bitcoin qr reader
 
 * Recognizes (and classifies)
   * Addresses  (also BIP21 with amount)
   * Transactions (also base43 electrum encoding)
   * PSBT
   * Xpub
   * Descriptor
   * Partial descriptors (Specter DIY) ( finger print , derivation, xpub)
   * TxId
+  * Animated QR Codes ([UR](https://github.com/BlockchainCommons/Research/blob/master/papers/bcr-2020-005-ur.md)) (Transactions and Descriptors)
+  * Animated QR Codes (Specter)
 * **blazingly fast** recognition
-* bdkpython as only bitcoin dependency
 * SLIP132 -> to BIP32 conversion
 
 ### Demo
 
 Run the demo with
 
 ```
```

### Comparing `bitcoin_qrreader-0.1.2/setup.py` & `bitcoin_qrreader-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from setuptools import setup,  find_namespace_packages, find_packages
-
+from setuptools import setup, find_namespace_packages, find_packages
 
 
 with open("requirements.txt") as f:
     install_reqs = f.read().strip().split("\n")
 
 # Filter out comments/hashes
 reqs = []
@@ -15,15 +14,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="bitcoin_qrreader",
-    version="0.1.2",
+    version="0.2.1",
     author="Andreas Griffin",
     author_email="andreasgriffin@proton.me",
     description="Bitcoin qr reader",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/andreasgriffin/bitcoin-qrreader",
     packages=find_packages(),
```

