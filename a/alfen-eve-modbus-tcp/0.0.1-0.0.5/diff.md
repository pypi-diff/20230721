# Comparing `tmp/alfen_eve_modbus_tcp-0.0.1.tar.gz` & `tmp/alfen_eve_modbus_tcp-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfen_eve_modbus_tcp-0.0.1.tar", last modified: Sun Jul 16 14:15:04 2023, max compression
+gzip compressed data, was "alfen_eve_modbus_tcp-0.0.5.tar", last modified: Fri Jul 21 21:03:37 2023, max compression
```

## Comparing `alfen_eve_modbus_tcp-0.0.1.tar` & `alfen_eve_modbus_tcp-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-16 14:15:04.502103 alfen_eve_modbus_tcp-0.0.1/
--rw-rw-r--   0 luc       (1000) luc       (1000)     1063 2023-07-14 13:22:32.000000 alfen_eve_modbus_tcp-0.0.1/LICENSE
--rw-rw-r--   0 luc       (1000) luc       (1000)    12403 2023-07-16 14:15:04.502103 alfen_eve_modbus_tcp-0.0.1/PKG-INFO
--rw-rw-r--   0 luc       (1000) luc       (1000)    11717 2023-07-15 21:37:45.000000 alfen_eve_modbus_tcp-0.0.1/README.md
--rw-rw-r--   0 luc       (1000) luc       (1000)      861 2023-07-16 14:15:04.502103 alfen_eve_modbus_tcp-0.0.1/setup.cfg
--rwxrwxr-x   0 luc       (1000) luc       (1000)       38 2023-07-14 13:22:32.000000 alfen_eve_modbus_tcp-0.0.1/setup.py
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-16 14:15:04.502103 alfen_eve_modbus_tcp-0.0.1/src/
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-16 14:15:04.502103 alfen_eve_modbus_tcp-0.0.1/src/alfen_eve_modbus_tcp/
--rw-rw-r--   0 luc       (1000) luc       (1000)    22838 2023-07-16 12:34:44.000000 alfen_eve_modbus_tcp-0.0.1/src/alfen_eve_modbus_tcp/__init__.py
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-16 14:15:04.502103 alfen_eve_modbus_tcp-0.0.1/src/alfen_eve_modbus_tcp.egg-info/
--rw-rw-r--   0 luc       (1000) luc       (1000)    12403 2023-07-16 14:15:04.000000 alfen_eve_modbus_tcp-0.0.1/src/alfen_eve_modbus_tcp.egg-info/PKG-INFO
--rw-rw-r--   0 luc       (1000) luc       (1000)      312 2023-07-16 14:15:04.000000 alfen_eve_modbus_tcp-0.0.1/src/alfen_eve_modbus_tcp.egg-info/SOURCES.txt
--rw-rw-r--   0 luc       (1000) luc       (1000)        1 2023-07-16 14:15:04.000000 alfen_eve_modbus_tcp-0.0.1/src/alfen_eve_modbus_tcp.egg-info/dependency_links.txt
--rw-rw-r--   0 luc       (1000) luc       (1000)       40 2023-07-16 14:15:04.000000 alfen_eve_modbus_tcp-0.0.1/src/alfen_eve_modbus_tcp.egg-info/requires.txt
--rw-rw-r--   0 luc       (1000) luc       (1000)       21 2023-07-16 14:15:04.000000 alfen_eve_modbus_tcp-0.0.1/src/alfen_eve_modbus_tcp.egg-info/top_level.txt
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-21 21:03:37.978254 alfen_eve_modbus_tcp-0.0.5/
+-rw-rw-r--   0 luc       (1000) luc       (1000)     1063 2023-07-14 13:22:32.000000 alfen_eve_modbus_tcp-0.0.5/LICENSE
+-rw-rw-r--   0 luc       (1000) luc       (1000)    12403 2023-07-21 21:03:37.978254 alfen_eve_modbus_tcp-0.0.5/PKG-INFO
+-rw-rw-r--   0 luc       (1000) luc       (1000)    11717 2023-07-16 19:44:24.000000 alfen_eve_modbus_tcp-0.0.5/README.md
+-rw-rw-r--   0 luc       (1000) luc       (1000)      861 2023-07-21 21:03:37.978254 alfen_eve_modbus_tcp-0.0.5/setup.cfg
+-rwxrwxr-x   0 luc       (1000) luc       (1000)       38 2023-07-14 13:22:32.000000 alfen_eve_modbus_tcp-0.0.5/setup.py
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-21 21:03:37.978254 alfen_eve_modbus_tcp-0.0.5/src/
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-21 21:03:37.978254 alfen_eve_modbus_tcp-0.0.5/src/alfen_eve_modbus_tcp/
+-rw-rw-r--   0 luc       (1000) luc       (1000)    24155 2023-07-21 20:57:35.000000 alfen_eve_modbus_tcp-0.0.5/src/alfen_eve_modbus_tcp/__init__.py
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-07-21 21:03:37.978254 alfen_eve_modbus_tcp-0.0.5/src/alfen_eve_modbus_tcp.egg-info/
+-rw-rw-r--   0 luc       (1000) luc       (1000)    12403 2023-07-21 21:03:37.000000 alfen_eve_modbus_tcp-0.0.5/src/alfen_eve_modbus_tcp.egg-info/PKG-INFO
+-rw-rw-r--   0 luc       (1000) luc       (1000)      312 2023-07-21 21:03:37.000000 alfen_eve_modbus_tcp-0.0.5/src/alfen_eve_modbus_tcp.egg-info/SOURCES.txt
+-rw-rw-r--   0 luc       (1000) luc       (1000)        1 2023-07-21 21:03:37.000000 alfen_eve_modbus_tcp-0.0.5/src/alfen_eve_modbus_tcp.egg-info/dependency_links.txt
+-rw-rw-r--   0 luc       (1000) luc       (1000)       40 2023-07-21 21:03:37.000000 alfen_eve_modbus_tcp-0.0.5/src/alfen_eve_modbus_tcp.egg-info/requires.txt
+-rw-rw-r--   0 luc       (1000) luc       (1000)       21 2023-07-21 21:03:37.000000 alfen_eve_modbus_tcp-0.0.5/src/alfen_eve_modbus_tcp.egg-info/top_level.txt
```

### Comparing `alfen_eve_modbus_tcp-0.0.1/LICENSE` & `alfen_eve_modbus_tcp-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alfen_eve_modbus_tcp-0.0.1/PKG-INFO` & `alfen_eve_modbus_tcp-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfen_eve_modbus_tcp
-Version: 0.0.1
+Version: 0.0.5
 Summary: Alfen Eve Car Charger parser library
 Home-page: https://github.com/nessnaj/alfen_eve_modbus_tcp
 Author: nessnaj
 License: MIT License
 Project-URL: Issue Tracker, https://github.com/nessnaj/alfen_eve_modbus_tcp/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
@@ -25,15 +25,15 @@
 
 To install, either clone this project and install using `setuptools`:
 
 ```python3 setup.py install```
 
 or install the package from PyPi:
 
-```pip3 install alfen_eve_modbus_tcp```
+```pip3 install alfen-eve-modbus-tcp```
 
 ## Usage
 
 The script `example.py` provides a minimal example of connecting to and displaying all registers from an Alfen Eve Car Charger over Modbus TCP.
 
 ```
 usage: example.py [-h] [--timeout TIMEOUT] [--json] host port
```

### Comparing `alfen_eve_modbus_tcp-0.0.1/README.md` & `alfen_eve_modbus_tcp-0.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 To install, either clone this project and install using `setuptools`:
 
 ```python3 setup.py install```
 
 or install the package from PyPi:
 
-```pip3 install alfen_eve_modbus_tcp```
+```pip3 install alfen-eve-modbus-tcp```
 
 ## Usage
 
 The script `example.py` provides a minimal example of connecting to and displaying all registers from an Alfen Eve Car Charger over Modbus TCP.
 
 ```
 usage: example.py [-h] [--timeout TIMEOUT] [--json] host port
```

### Comparing `alfen_eve_modbus_tcp-0.0.1/setup.cfg` & `alfen_eve_modbus_tcp-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = alfen_eve_modbus_tcp
-version = 0.0.1
+version = 0.0.5
 author = nessnaj
 description = Alfen Eve Car Charger parser library
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
 url = https://github.com/nessnaj/alfen_eve_modbus_tcp
 project_urls =
```

### Comparing `alfen_eve_modbus_tcp-0.0.1/src/alfen_eve_modbus_tcp/__init__.py` & `alfen_eve_modbus_tcp-0.0.5/src/alfen_eve_modbus_tcp/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -473,7 +473,38 @@
             "remaining_valid_time_max_current_phase_l2": (0xc8, 0x591, 2, registerType.HOLDING, registerDataType.UINT32, int, "Max current valid time", "1s", 8),
             "remaining_valid_time_max_current_phase_l3": (0xc8, 0x593, 2, registerType.HOLDING, registerDataType.UINT32, int, "Max current valid time", "1s", 8),
             "scn_safe_current": (0xc8, 0x595, 2, registerType.HOLDING, registerDataType.FLOAT32, float, "Configured SCN safe current", "1A", 8),
             "scn_modbus_slave_max_current_enable": (0xc8, 0x597, 1, registerType.HOLDING, registerDataType.UINT16, int, "1: Enabled; 0: Disabled", "1A",
             8)
 
         }
+
+    def pause_charging(self):
+        PAUSE_CURRENT = 5
+        print(f"Stop Charging...")
+        value = self.read('modbus_slave_max_current')
+        current = value['modbus_slave_max_current']
+        print(f"\tCurrent usage in A: {current}")
+        if current > 5.5:
+            print(f"\tPausing...")
+            self.set_current(PAUSE_CURRENT)
+            print(f"\tPaused...")
+        else:
+            print(f"\tAlready paused charging...")
+
+    def switch_phase(self, phases):
+        if (phases == 1 or phases == 3):
+            current_phases = self.read('charge_using_1_or_3_phases')['charge_using_1_or_3_phases']
+            if current_phases == phases:
+                print(f"No need to switch, already at {phases} phase...")
+            else:
+                print(f"Switch to {phases} phase(s)...")
+                print(f"\tCurrent phase(s): {current_phases}")
+                self.write('charge_using_1_or_3_phases', phases)
+                print(f"\tSwitched...")
+                current_phases = self.read('charge_using_1_or_3_phases')['charge_using_1_or_3_phases']
+                print(f"\tCurrent phase(s): {current_phases}")
+        else:
+            print(f"\tInvalid # of phases: {phases}...")
+
+    def set_current(self, current):
+        self.write('modbus_slave_max_current', current)
```

### Comparing `alfen_eve_modbus_tcp-0.0.1/src/alfen_eve_modbus_tcp.egg-info/PKG-INFO` & `alfen_eve_modbus_tcp-0.0.5/src/alfen_eve_modbus_tcp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfen-eve-modbus-tcp
-Version: 0.0.1
+Version: 0.0.5
 Summary: Alfen Eve Car Charger parser library
 Home-page: https://github.com/nessnaj/alfen_eve_modbus_tcp
 Author: nessnaj
 License: MIT License
 Project-URL: Issue Tracker, https://github.com/nessnaj/alfen_eve_modbus_tcp/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
@@ -25,15 +25,15 @@
 
 To install, either clone this project and install using `setuptools`:
 
 ```python3 setup.py install```
 
 or install the package from PyPi:
 
-```pip3 install alfen_eve_modbus_tcp```
+```pip3 install alfen-eve-modbus-tcp```
 
 ## Usage
 
 The script `example.py` provides a minimal example of connecting to and displaying all registers from an Alfen Eve Car Charger over Modbus TCP.
 
 ```
 usage: example.py [-h] [--timeout TIMEOUT] [--json] host port
```

