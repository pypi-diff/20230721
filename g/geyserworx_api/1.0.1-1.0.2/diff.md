# Comparing `tmp/geyserworx_api-1.0.1.tar.gz` & `tmp/geyserworx_api-1.0.2.tar.gz`

## Comparing `geyserworx_api-1.0.1.tar` & `geyserworx_api-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 geyserworx_api-1.0.1/src/geyserworx_api/__init__.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 geyserworx_api-1.0.1/src/geyserworx_api/geyserworx_api.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 geyserworx_api-1.0.1/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 geyserworx_api-1.0.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geyserworx_api-1.0.1/README.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 geyserworx_api-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 geyserworx_api-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 geyserworx_api-1.0.2/src/geyserworx_api/__init__.py
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 geyserworx_api-1.0.2/src/geyserworx_api/geyserworx_api.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 geyserworx_api-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 geyserworx_api-1.0.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geyserworx_api-1.0.2/README.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 geyserworx_api-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 geyserworx_api-1.0.2/PKG-INFO
```

### Comparing `geyserworx_api-1.0.1/src/geyserworx_api/geyserworx_api.py` & `geyserworx_api-1.0.2/src/geyserworx_api/geyserworx_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-from enum import Enum
-import json
-
-from aiohttp import ClientSession
-
-
-class PowerType(Enum):
-    AC = 'ACM'
-    AC_BOOST = 'ACO'
-    PV = 'PVM'
-
-
-class TemperatureType(Enum):
-    AC = 'ACT'
-    AC_BOOST = 'ACOT'
-    PV = 'PVT'
-
-
-class GeyserworxAPI:
-    __API_BASE__ = 'gwa'
-    __TOPIC_BASE_GET__ = 'GWA'
-    __TOPIC_BASE_SET__ = 'GWR'
-
-    def __init__(
-            self,
-            session: ClientSession,
-            geyser_serial_number: str,
-            geyser_number: int = 1,
-            base_url: str = "http://192.168.4.1"
-    ):
-        self.geyser_serial_number = geyser_serial_number
-        self.geyser_number = geyser_number
-        self.base_url_get = f'{base_url}/{self.__API_BASE__}?topic={self.__TOPIC_BASE_GET__}/{self.geyser_serial_number}/{self.geyser_number}/'
-        self.base_url_set = f'{base_url}/{self.__API_BASE__}?topic={self.__TOPIC_BASE_SET__}/{self.geyser_serial_number}/{self.geyser_number}/'
-        self.session = session
-
-    async def get_current_temperature(self) -> float:
-        url = f'{self.base_url_get}A'
-        response = await self.session.get(url)
-        response_json: dict = await response.json()
-        return response_json['T']['G']
-
-    async def get_settings(self) -> dict:
-        url = f'{self.base_url_get}SET'
-        response = await self.session.get(url)
-        response_json: dict = await response.json()
-        return {
-            'POWER': {
-                'AC': True if response_json['O']['ACM'] == 1 else False,
-                'AC_BOOST': True if response_json['O']['ACO'] == 1 else False,
-                'PV': True if response_json['O']['PVM'] == 1 else False
-            },
-            'TEMP': {
-                'AC': response_json['S']['ACT'],
-                'AC_BOOST': response_json['S']['ACOT'],
-                'PV': response_json['S']['PVT']
-            }
-        }
-
-    async def get_power_status(self) -> dict[str, bool]:
-        url = f'{self.base_url_get}STS'
-        response = await self.session.get(url)
-        response_json: dict = await response.json()
-        return {
-            'AC': True if response_json['O']['AC'] == 1 else False,
-            'PV': True if response_json['O']['PV'] == 1 else False
-        }
-
-    async def set_power(self, power_type: PowerType, on: bool) -> bool:
-        payload = {
-            'O': {
-                power_type.value: 1 if on else 0
-            }
-        }
-        url = f'{self.base_url_set}STS/O&payload={json.dumps(payload)}'
-        response = await self.session.get(url)
-        response_json: dict = await response.json()
-        return response_json['O'][power_type.value] == 1
-
-    async def set_temp(self, temperature_type: TemperatureType, temperature: int) -> int:
-        payload = {
-            'S': {
-                temperature_type.value: temperature
-            }
-        }
-        url = f'{self.base_url_set}STS/S&payload={json.dumps(payload)}'
-        response = await self.session.get(url)
-        response_json: dict = await response.json()
-        return response_json['S'][temperature_type.value]
+from enum import Enum
+import json
+
+from aiohttp import ClientSession
+
+
+class PowerType(Enum):
+    AC = 'ACM'
+    AC_BOOST = 'ACO'
+    PV = 'PVM'
+
+
+class TemperatureType(Enum):
+    AC = 'ACT'
+    AC_BOOST = 'ACOT'
+    PV = 'PVT'
+
+
+class GeyserworxAPI:
+    __API_BASE__ = 'gwa'
+    __TOPIC_BASE_GET__ = 'GWA'
+    __TOPIC_BASE_SET__ = 'GWR'
+
+    def __init__(
+            self,
+            session: ClientSession,
+            geyser_serial_number: str,
+            geyser_number: int = 1,
+            base_url: str = "http://192.168.4.1"
+    ):
+        self.geyser_serial_number = geyser_serial_number
+        self.geyser_number = geyser_number
+        self.base_url_get = f'{base_url}/{self.__API_BASE__}?topic={self.__TOPIC_BASE_GET__}/{self.geyser_serial_number}/{self.geyser_number}/'
+        self.base_url_set = f'{base_url}/{self.__API_BASE__}?topic={self.__TOPIC_BASE_SET__}/{self.geyser_serial_number}/{self.geyser_number}/'
+        self.session = session
+
+    async def get_current_temperature(self) -> float:
+        url = f'{self.base_url_get}A'
+        response = await self.session.get(url)
+        response_json: dict = await response.json(content_type=None)
+        return response_json['T']['G']
+
+    async def get_settings(self) -> dict:
+        url = f'{self.base_url_get}SET'
+        response = await self.session.get(url)
+        response_json: dict = await response.json(content_type=None)
+        return {
+            'POWER': {
+                'AC': True if response_json['O']['ACM'] == 1 else False,
+                'AC_BOOST': True if response_json['O']['ACO'] == 1 else False,
+                'PV': True if response_json['O']['PVM'] == 1 else False
+            },
+            'TEMP': {
+                'AC': response_json['S']['ACT'],
+                'AC_BOOST': response_json['S']['ACOT'],
+                'PV': response_json['S']['PVT']
+            }
+        }
+
+    async def get_power_status(self) -> dict[str, bool]:
+        url = f'{self.base_url_get}STS'
+        response = await self.session.get(url)
+        response_json: dict = await response.json(content_type=None)
+        return {
+            'AC': True if response_json['O']['AC'] == 1 else False,
+            'PV': True if response_json['O']['PV'] == 1 else False
+        }
+
+    async def set_power(self, power_type: PowerType, on: bool) -> bool:
+        payload = {
+            'O': {
+                power_type.value: 1 if on else 0
+            }
+        }
+        url = f'{self.base_url_set}STS/O&payload={json.dumps(payload)}'
+        response = await self.session.get(url)
+        response_json: dict = await response.json(content_type=None)
+        return response_json['O'][power_type.value] == 1
+
+    async def set_temp(self, temperature_type: TemperatureType, temperature: int) -> int:
+        payload = {
+            'S': {
+                temperature_type.value: temperature
+            }
+        }
+        url = f'{self.base_url_set}STS/S&payload={json.dumps(payload)}'
+        response = await self.session.get(url)
+        response_json: dict = await response.json(content_type=None)
+        return response_json['S'][temperature_type.value]
```

### Comparing `geyserworx_api-1.0.1/LICENSE` & `geyserworx_api-1.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Dovi Joel
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Dovi Joel
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `geyserworx_api-1.0.1/PKG-INFO` & `geyserworx_api-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: geyserworx_api
-Version: 1.0.1
-Summary: An SDK interface to read and set Geyserworx geysers without using the app.
+Version: 1.0.2
+Summary: An API interface to read and set Geyserworx geysers without using the app.
 Project-URL: Homepage, https://github.com/dovijoel/GeyserworxAPI
 Project-URL: Bug Tracker, https://github.com/dovijoel/GeyserworxAPI/issues
 Author-email: Dovi Joel <dovi@debuggingmadejoyful.tech>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

