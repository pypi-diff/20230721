# Comparing `tmp/meer_tec-0.0.3.tar.gz` & `tmp/meer_tec-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meer_tec-0.0.3.tar", last modified: Thu Apr 21 13:48:27 2022, max compression
+gzip compressed data, was "meer_tec-0.0.4.tar", last modified: Fri Jul 21 13:50:28 2023, max compression
```

## Comparing `meer_tec-0.0.3.tar` & `meer_tec-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 13:48:27.182025 meer_tec-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-04-21 13:48:12.000000 meer_tec-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-04-21 13:48:12.000000 meer_tec-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2911 2022-04-21 13:48:27.182025 meer_tec-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2285 2022-04-21 13:48:12.000000 meer_tec-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 13:48:27.182025 meer_tec-0.0.3/meer_tec/
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-04-21 13:48:12.000000 meer_tec-0.0.3/meer_tec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-04-21 13:48:27.182025 meer_tec-0.0.3/meer_tec/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    11433 2022-04-21 13:48:12.000000 meer_tec-0.0.3/meer_tec/meer_tec.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 13:48:27.182025 meer_tec-0.0.3/meer_tec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2911 2022-04-21 13:48:27.000000 meer_tec-0.0.3/meer_tec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-04-21 13:48:27.000000 meer_tec-0.0.3/meer_tec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-21 13:48:27.000000 meer_tec-0.0.3/meer_tec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-04-21 13:48:27.000000 meer_tec-0.0.3/meer_tec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-04-21 13:48:27.000000 meer_tec-0.0.3/meer_tec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      672 2022-04-21 13:48:12.000000 meer_tec-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1013 2022-04-21 13:48:27.182025 meer_tec-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-04-21 13:48:12.000000 meer_tec-0.0.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68626 2022-04-21 13:48:12.000000 meer_tec-0.0.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:50:28.272042 meer_tec-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-21 13:50:18.000000 meer_tec-0.0.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:50:28.272042 meer_tec-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:50:28.272042 meer_tec-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-21 13:50:18.000000 meer_tec-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-21 13:50:18.000000 meer_tec-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-21 13:50:18.000000 meer_tec-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 13:50:18.000000 meer_tec-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43437 2023-07-21 13:50:28.272042 meer_tec-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-21 13:50:18.000000 meer_tec-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:50:28.272042 meer_tec-0.0.4/meer_tec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:50:18.000000 meer_tec-0.0.4/meer_tec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-21 13:50:28.000000 meer_tec-0.0.4/meer_tec/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-07-21 13:50:18.000000 meer_tec-0.0.4/meer_tec/meer_tec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:50:28.272042 meer_tec-0.0.4/meer_tec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43437 2023-07-21 13:50:28.000000 meer_tec-0.0.4/meer_tec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-21 13:50:28.000000 meer_tec-0.0.4/meer_tec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:50:28.000000 meer_tec-0.0.4/meer_tec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-21 13:50:28.000000 meer_tec-0.0.4/meer_tec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 13:50:28.000000 meer_tec-0.0.4/meer_tec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-21 13:50:18.000000 meer_tec-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 13:50:28.272042 meer_tec-0.0.4/setup.cfg
```

### Comparing `meer_tec-0.0.3/LICENSE` & `meer_tec-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `meer_tec-0.0.3/README.md` & `meer_tec-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,14 @@
 
 -   Bastian Leykauf (<https://github.com/bleykauf>)
 
 ## License
 
 MeerTEC -- Python implemenation of the MeCom interface for Meerstetter TECs.
 
-Copyright © 2020 B. Leykauf
+Copyright © 2020-2023 B. Leykauf
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
```

### Comparing `meer_tec-0.0.3/meer_tec/meer_tec.py` & `meer_tec-0.0.4/meer_tec/meer_tec.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,46 +24,48 @@
 
 def _calc_checksum(string: str) -> str:
     """Calculate CRC checksum."""
     return "{:04X}".format(CRC().calculate(string))
 
 
 class XPort(socket.socket):
-    def __init__(self, ip, port=10001):
+    def __init__(self, ip: str, port: int = 10001) -> None:
         super().__init__(socket.AF_INET, socket.SOCK_STREAM)
         self.settimeout(0.2)
         self.ip = ip
         self.port = port
         self.connect()
 
     def connect(self):
         super().connect((self.ip, self.port))
 
 
 class TEC:
-    def __init__(self, xport, addr):
+    def __init__(self, xport: XPort, addr: int) -> None:
         self.xport = xport
         self.addr = str(addr)
 
-    def _tcpip_query(self, request):
+    def _tcpip_query(self, request: "Request") -> str:
         self.xport.send(request.encode("ascii"))
         time.sleep(0.01)
         return self.xport.recv(128).decode("ascii")
 
-    def clear_buffer(self):
+    def clear_buffer(self) -> None:
         _ = self.xport.recv(128)
 
-    def get_parameter(self, cmd_id: int, value_type, request_number=None, instance=1):
+    def get_parameter(
+        self, cmd_id: int, value_type, request_number=None, instance: int = 1
+    ):
         cmd = "?VR" + _id_to_hex(cmd_id) + "{:02X}".format(instance)
         request = Request(cmd, self.addr, request_number=request_number)
         reponse = Response(self._tcpip_query(request), request, value_type=value_type)
         return reponse.value
 
     def set_parameter(
-        self, cmd_id: int, value, value_type, request_number=None, instance=1
+        self, cmd_id: int, value, value_type, request_number=None, instance: int = 1
     ):
         cmd = "VS" + _id_to_hex(cmd_id) + "{:02X}".format(instance)
         if value_type is float:
             cmd += _float_to_hex(value)
         elif value_type is int:
             cmd += _int_to_hex(value)
         request = Request(cmd, self.addr, request_number=request_number)
```

