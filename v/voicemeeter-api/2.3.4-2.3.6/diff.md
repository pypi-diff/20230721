# Comparing `tmp/voicemeeter_api-2.3.4.tar.gz` & `tmp/voicemeeter_api-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicemeeter_api-2.3.4.tar", max compression
+gzip compressed data, was "voicemeeter_api-2.3.6.tar", max compression
```

## Comparing `voicemeeter_api-2.3.4.tar` & `voicemeeter_api-2.3.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter_api-2.3.4/LICENSE
--rw-r--r--   0        0        0     1102 2023-07-20 10:11:55.345129 voicemeeter_api-2.3.4/pyproject.toml
--rw-r--r--   0        0        0    18957 2023-07-13 07:54:12.378858 voicemeeter_api-2.3.4/README.md
--rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter_api-2.3.4/voicemeeterlib/__init__.py
--rw-r--r--   0        0        0     8226 2023-07-18 12:50:39.247222 voicemeeter_api-2.3.4/voicemeeterlib/bus.py
--rw-r--r--   0        0        0     4207 2023-07-10 19:16:03.423527 voicemeeter_api-2.3.4/voicemeeterlib/cbindings.py
--rw-r--r--   0        0        0     1194 2023-06-22 23:31:24.097081 voicemeeter_api-2.3.4/voicemeeterlib/command.py
--rw-r--r--   0        0        0     5819 2023-06-22 09:43:14.446510 voicemeeter_api-2.3.4/voicemeeterlib/config.py
--rw-r--r--   0        0        0     1748 2022-07-07 14:44:58.387087 voicemeeter_api-2.3.4/voicemeeterlib/device.py
--rw-r--r--   0        0        0      575 2023-07-10 12:27:38.707424 voicemeeter_api-2.3.4/voicemeeterlib/error.py
--rw-r--r--   0        0        0     2099 2023-06-22 08:38:58.271443 voicemeeter_api-2.3.4/voicemeeterlib/event.py
--rw-r--r--   0        0        0     7792 2023-06-29 15:52:06.128626 voicemeeter_api-2.3.4/voicemeeterlib/factory.py
--rw-r--r--   0        0        0     1091 2023-06-22 23:31:40.238138 voicemeeter_api-2.3.4/voicemeeterlib/inst.py
--rw-r--r--   0        0        0     1800 2023-06-23 20:52:02.185334 voicemeeter_api-2.3.4/voicemeeterlib/iremote.py
--rw-r--r--   0        0        0     2628 2023-07-18 13:00:26.971422 voicemeeter_api-2.3.4/voicemeeterlib/kinds.py
--rw-r--r--   0        0        0     1081 2023-07-14 11:53:50.976482 voicemeeter_api-2.3.4/voicemeeterlib/macrobutton.py
--rw-r--r--   0        0        0     1130 2023-06-21 12:24:03.433043 voicemeeter_api-2.3.4/voicemeeterlib/meta.py
--rw-r--r--   0        0        0     6485 2023-07-10 14:28:38.873267 voicemeeter_api-2.3.4/voicemeeterlib/misc.py
--rw-r--r--   0        0        0     6739 2023-07-01 18:30:01.004734 voicemeeter_api-2.3.4/voicemeeterlib/recorder.py
--rw-r--r--   0        0        0    12072 2023-07-18 13:15:47.727817 voicemeeter_api-2.3.4/voicemeeterlib/remote.py
--rw-r--r--   0        0        0    15352 2023-07-14 11:51:40.640708 voicemeeter_api-2.3.4/voicemeeterlib/strip.py
--rw-r--r--   0        0        0     2277 2023-06-23 16:22:05.659320 voicemeeter_api-2.3.4/voicemeeterlib/subject.py
--rw-r--r--   0        0        0     2930 2023-07-18 13:06:02.678934 voicemeeter_api-2.3.4/voicemeeterlib/updater.py
--rw-r--r--   0        0        0     2436 2023-07-18 13:03:59.421646 voicemeeter_api-2.3.4/voicemeeterlib/util.py
--rw-r--r--   0        0        0     6055 2023-07-20 10:04:33.726657 voicemeeter_api-2.3.4/voicemeeterlib/vban.py
--rw-r--r--   0        0        0    18745 1970-01-01 00:00:00.000000 voicemeeter_api-2.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter_api-2.3.6/LICENSE
+-rw-r--r--   0        0        0     1102 2023-07-21 11:56:04.546339 voicemeeter_api-2.3.6/pyproject.toml
+-rw-r--r--   0        0        0    18957 2023-07-13 07:54:12.378858 voicemeeter_api-2.3.6/README.md
+-rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter_api-2.3.6/voicemeeterlib/__init__.py
+-rw-r--r--   0        0        0     8226 2023-07-18 12:50:39.247222 voicemeeter_api-2.3.6/voicemeeterlib/bus.py
+-rw-r--r--   0        0        0     4618 2023-07-21 11:37:10.587298 voicemeeter_api-2.3.6/voicemeeterlib/cbindings.py
+-rw-r--r--   0        0        0     1194 2023-06-22 23:31:24.097081 voicemeeter_api-2.3.6/voicemeeterlib/command.py
+-rw-r--r--   0        0        0     5819 2023-06-22 09:43:14.446510 voicemeeter_api-2.3.6/voicemeeterlib/config.py
+-rw-r--r--   0        0        0     1748 2022-07-07 14:44:58.387087 voicemeeter_api-2.3.6/voicemeeterlib/device.py
+-rw-r--r--   0        0        0      575 2023-07-10 12:27:38.707424 voicemeeter_api-2.3.6/voicemeeterlib/error.py
+-rw-r--r--   0        0        0     2099 2023-06-22 08:38:58.271443 voicemeeter_api-2.3.6/voicemeeterlib/event.py
+-rw-r--r--   0        0        0     7792 2023-06-29 15:52:06.128626 voicemeeter_api-2.3.6/voicemeeterlib/factory.py
+-rw-r--r--   0        0        0     1091 2023-06-22 23:31:40.238138 voicemeeter_api-2.3.6/voicemeeterlib/inst.py
+-rw-r--r--   0        0        0     1800 2023-06-23 20:52:02.185334 voicemeeter_api-2.3.6/voicemeeterlib/iremote.py
+-rw-r--r--   0        0        0     2628 2023-07-18 13:00:26.971422 voicemeeter_api-2.3.6/voicemeeterlib/kinds.py
+-rw-r--r--   0        0        0     1512 2023-07-21 10:03:47.432342 voicemeeter_api-2.3.6/voicemeeterlib/macrobutton.py
+-rw-r--r--   0        0        0     1130 2023-06-21 12:24:03.433043 voicemeeter_api-2.3.6/voicemeeterlib/meta.py
+-rw-r--r--   0        0        0     6485 2023-07-10 14:28:38.873267 voicemeeter_api-2.3.6/voicemeeterlib/misc.py
+-rw-r--r--   0        0        0     6739 2023-07-01 18:30:01.004734 voicemeeter_api-2.3.6/voicemeeterlib/recorder.py
+-rw-r--r--   0        0        0    12341 2023-07-21 11:55:26.907178 voicemeeter_api-2.3.6/voicemeeterlib/remote.py
+-rw-r--r--   0        0        0    15352 2023-07-14 11:51:40.640708 voicemeeter_api-2.3.6/voicemeeterlib/strip.py
+-rw-r--r--   0        0        0     2277 2023-06-23 16:22:05.659320 voicemeeter_api-2.3.6/voicemeeterlib/subject.py
+-rw-r--r--   0        0        0     2930 2023-07-18 13:06:02.678934 voicemeeter_api-2.3.6/voicemeeterlib/updater.py
+-rw-r--r--   0        0        0     2436 2023-07-21 11:41:24.422287 voicemeeter_api-2.3.6/voicemeeterlib/util.py
+-rw-r--r--   0        0        0     6055 2023-07-20 10:04:33.726657 voicemeeter_api-2.3.6/voicemeeterlib/vban.py
+-rw-r--r--   0        0        0    18745 1970-01-01 00:00:00.000000 voicemeeter_api-2.3.6/PKG-INFO
```

### Comparing `voicemeeter_api-2.3.4/LICENSE` & `voicemeeter_api-2.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.4/pyproject.toml` & `voicemeeter_api-2.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voicemeeter-api"
-version = "2.3.4"
+version = "2.3.6"
 description = "A Python wrapper for the Voiceemeter API"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/voicemeeter-api-python"
 
 packages = [{ include = "voicemeeterlib" }]
```

### Comparing `voicemeeter_api-2.3.4/README.md` & `voicemeeter_api-2.3.6/README.md`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.4/voicemeeterlib/bus.py` & `voicemeeter_api-2.3.6/voicemeeterlib/bus.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.4/voicemeeterlib/command.py` & `voicemeeter_api-2.3.6/voicemeeterlib/command.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.4/voicemeeterlib/config.py` & `voicemeeter_api-2.3.6/voicemeeterlib/config.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.4/voicemeeterlib/device.py` & `voicemeeter_api-2.3.6/voicemeeterlib/device.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.4/voicemeeterlib/error.py` & `voicemeeter_api-2.3.6/voicemeeterlib/error.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.4/voicemeeterlib/event.py` & `voicemeeter_api-2.3.6/voicemeeterlib/event.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.4/voicemeeterlib/factory.py` & `voicemeeter_api-2.3.6/voicemeeterlib/factory.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.4/voicemeeterlib/inst.py` & `voicemeeter_api-2.3.6/voicemeeterlib/inst.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.4/voicemeeterlib/iremote.py` & `voicemeeter_api-2.3.6/voicemeeterlib/iremote.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.4/voicemeeterlib/kinds.py` & `voicemeeter_api-2.3.6/voicemeeterlib/kinds.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.4/voicemeeterlib/meta.py` & `voicemeeter_api-2.3.6/voicemeeterlib/meta.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.4/voicemeeterlib/misc.py` & `voicemeeter_api-2.3.6/voicemeeterlib/misc.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.4/voicemeeterlib/recorder.py` & `voicemeeter_api-2.3.6/voicemeeterlib/recorder.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.4/voicemeeterlib/remote.py` & `voicemeeter_api-2.3.6/voicemeeterlib/remote.py`

 * *Files 14% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         self.updater = Updater(self, queue)
         self.updater.start()
         self.producer = Producer(self, queue)
         self.producer.start()
 
     def login(self) -> NoReturn:
         """Login to the API, initialize dirty parameters"""
-        self.gui.launched = self.call(self.vm_login, ok=(0, 1)) == 0
+        self.gui.launched = self.call(self.bind_login, ok=(0, 1)) == 0
         if not self.gui.launched:
             self.logger.info(
                 "Voicemeeter engine running but GUI not launched. Launching the GUI now."
             )
             self.run_voicemeeter(self.kind.name)
         self.logger.info(
             f"{type(self).__name__}: Successfully logged into {self} version {self.version}"
@@ -78,46 +78,46 @@
     def run_voicemeeter(self, kind_id: str) -> NoReturn:
         if kind_id not in (kind.name.lower() for kind in KindId):
             raise VMError(f"Unexpected Voicemeeter type: '{kind_id}'")
         if kind_id == "potato" and bits == 8:
             value = KindId[kind_id.upper()].value + 3
         else:
             value = KindId[kind_id.upper()].value
-        self.call(self.vm_runvm, value)
+        self.call(self.bind_run_voicemeeter, value)
         time.sleep(1)
 
     @property
     def type(self) -> str:
         """Returns the type of Voicemeeter installation (basic, banana, potato)."""
         type_ = ct.c_long()
-        self.call(self.vm_get_type, ct.byref(type_))
+        self.call(self.bind_get_voicemeeter_type, ct.byref(type_))
         return KindId(type_.value).name.lower()
 
     @property
     def version(self) -> str:
         """Returns Voicemeeter's version as a string"""
         ver = ct.c_long()
-        self.call(self.vm_get_version, ct.byref(ver))
+        self.call(self.bind_get_voicemeeter_version, ct.byref(ver))
         return "{}.{}.{}.{}".format(
             (ver.value & 0xFF000000) >> 24,
             (ver.value & 0x00FF0000) >> 16,
             (ver.value & 0x0000FF00) >> 8,
             ver.value & 0x000000FF,
         )
 
     @property
     def pdirty(self) -> bool:
         """True iff UI parameters have been updated."""
-        return self.call(self.vm_pdirty, ok=(0, 1)) == 1
+        return self.call(self.bind_is_parameters_dirty, ok=(0, 1)) == 1
 
     @property
     def mdirty(self) -> bool:
         """True iff MB parameters have been updated."""
         try:
-            return self.call(self.vm_mdirty, ok=(0, 1)) == 1
+            return self.call(self.bind_macro_button_is_dirty, ok=(0, 1)) == 1
         except AttributeError as e:
             self.logger.exception(f"{type(e).__name__}: {e}")
             ERR_MSG = (
                 "no bind for VBVMR_MacroButton_IsDirty.",
                 "are you using an old version of the API?",
             )
             raise CAPIError(
@@ -145,99 +145,108 @@
                 pass
 
     @polling
     def get(self, param: str, is_string: Optional[bool] = False) -> Union[str, float]:
         """Gets a string or float parameter"""
         if is_string:
             buf = ct.create_unicode_buffer(512)
-            self.call(self.vm_get_parameter_string, param.encode(), ct.byref(buf))
+            self.call(self.bind_get_parameter_string_w, param.encode(), ct.byref(buf))
         else:
             buf = ct.c_float()
-            self.call(self.vm_get_parameter_float, param.encode(), ct.byref(buf))
+            self.call(self.bind_get_parameter_float, param.encode(), ct.byref(buf))
         return buf.value
 
     def set(self, param: str, val: Union[str, float]) -> NoReturn:
         """Sets a string or float parameter. Caches value"""
         if isinstance(val, str):
             if len(val) >= 512:
                 raise VMError("String is too long")
-            self.call(self.vm_set_parameter_string, param.encode(), ct.c_wchar_p(val))
+            self.call(
+                self.bind_set_parameter_string_w, param.encode(), ct.c_wchar_p(val)
+            )
         else:
             self.call(
-                self.vm_set_parameter_float, param.encode(), ct.c_float(float(val))
+                self.bind_set_parameter_float, param.encode(), ct.c_float(float(val))
             )
         self.cache[param] = val
 
     @polling
-    def get_buttonstatus(self, id: int, mode: int) -> int:
+    def get_buttonstatus(self, id_: int, mode: int) -> int:
         """Gets a macrobutton parameter"""
-        state = ct.c_float()
+        c_state = ct.c_float()
         try:
             self.call(
-                self.vm_get_buttonstatus,
-                ct.c_long(id),
-                ct.byref(state),
+                self.bind_macro_button_get_status,
+                ct.c_long(id_),
+                ct.byref(c_state),
                 ct.c_long(mode),
             )
         except AttributeError as e:
             self.logger.exception(f"{type(e).__name__}: {e}")
             ERR_MSG = (
                 "no bind for VBVMR_MacroButton_GetStatus.",
                 "are you using an old version of the API?",
             )
             raise CAPIError(
                 "VBVMR_MacroButton_GetStatus", -9, msg=" ".join(ERR_MSG)
             ) from e
-        return int(state.value)
+        return int(c_state.value)
 
-    def set_buttonstatus(self, id: int, state: int, mode: int) -> NoReturn:
+    def set_buttonstatus(self, id_: int, val: int, mode: int) -> NoReturn:
         """Sets a macrobutton parameter. Caches value"""
-        c_state = ct.c_float(float(state))
+        c_state = ct.c_float(float(val))
         try:
-            self.call(self.vm_set_buttonstatus, ct.c_long(id), c_state, ct.c_long(mode))
+            self.call(
+                self.bind_macro_button_set_status,
+                ct.c_long(id_),
+                c_state,
+                ct.c_long(mode),
+            )
         except AttributeError as e:
             self.logger.exception(f"{type(e).__name__}: {e}")
             ERR_MSG = (
                 "no bind for VBVMR_MacroButton_SetStatus.",
                 "are you using an old version of the API?",
             )
             raise CAPIError(
                 "VBVMR_MacroButton_SetStatus", -9, msg=" ".join(ERR_MSG)
             ) from e
-        self.cache[f"mb_{id}_{mode}"] = int(c_state.value)
+        self.cache[f"mb_{id_}_{mode}"] = int(c_state.value)
 
     def get_num_devices(self, direction: str = None) -> int:
         """Retrieves number of physical devices connected"""
         if direction not in ("in", "out"):
             raise VMError("Expected a direction: in or out")
-        func = getattr(self, f"vm_get_num_{direction}devices")
+        func = getattr(self, f"bind_{direction}put_get_device_number")
         res = self.call(func, ok_exp=lambda r: r >= 0)
         return res
 
     def get_device_description(self, index: int, direction: str = None) -> tuple:
         """Returns a tuple of device parameters"""
         if direction not in ("in", "out"):
             raise VMError("Expected a direction: in or out")
         type_ = ct.c_long()
         name = ct.create_unicode_buffer(256)
         hwid = ct.create_unicode_buffer(256)
-        func = getattr(self, f"vm_get_desc_{direction}devices")
+        func = getattr(self, f"bind_{direction}put_get_device_desc_w")
         self.call(
             func,
             ct.c_long(index),
             ct.byref(type_),
             ct.byref(name),
             ct.byref(hwid),
         )
         return (name.value, type_.value, hwid.value)
 
     def get_level(self, type_: int, index: int) -> float:
         """Retrieves a single level value"""
         val = ct.c_float()
-        self.call(self.vm_get_level, ct.c_long(type_), ct.c_long(index), ct.byref(val))
+        self.call(
+            self.bind_get_level, ct.c_long(type_), ct.c_long(index), ct.byref(val)
+        )
         return val.value
 
     def _get_levels(self) -> Iterable:
         """
         returns both level arrays (strip_levels, bus_levels) BEFORE math conversion
         """
         return (
@@ -248,15 +257,15 @@
             tuple(self.get_level(3, i) for i in range(self.kind.num_bus_levels)),
         )
 
     def get_midi_message(self):
         n = ct.c_long(1024)
         buf = ct.create_string_buffer(1024)
         res = self.call(
-            self.vm_get_midi_message,
+            self.bind_get_midi_message,
             ct.byref(buf),
             n,
             ok=(-5, -6),  # no data received from midi device
             ok_exp=lambda r: r >= 0,
         )
         if res > 0:
             vals = tuple(
@@ -271,15 +280,15 @@
             return True
 
     @script
     def sendtext(self, script: str):
         """Sets many parameters from a script"""
         if len(script) > 48000:
             raise ValueError("Script too large, max size 48kB")
-        self.call(self.vm_set_parameter_multi, script.encode())
+        self.call(self.bind_set_parameters, script.encode())
         time.sleep(self.DELAY * 5)
 
     def apply(self, data: dict):
         """
         Sets all parameters of a dict
 
         minor delay between each recursion
@@ -324,14 +333,14 @@
     def end_thread(self):
         self.logger.debug("events thread shutdown started")
         self.running = False
 
     def logout(self) -> NoReturn:
         """Logout of the API"""
         time.sleep(0.1)
-        self.call(self.vm_logout)
+        self.call(self.bind_logout)
         self.logger.info(f"{type(self).__name__}: Successfully logged out of {self}")
 
     def __exit__(self, exc_type, exc_value, exc_traceback) -> NoReturn:
         """teardown procedures"""
         self.end_thread()
         self.logout()
```

### Comparing `voicemeeter_api-2.3.4/voicemeeterlib/strip.py` & `voicemeeter_api-2.3.6/voicemeeterlib/strip.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.4/voicemeeterlib/subject.py` & `voicemeeter_api-2.3.6/voicemeeterlib/subject.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.4/voicemeeterlib/updater.py` & `voicemeeter_api-2.3.6/voicemeeterlib/updater.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.4/voicemeeterlib/util.py` & `voicemeeter_api-2.3.6/voicemeeterlib/util.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.4/voicemeeterlib/vban.py` & `voicemeeter_api-2.3.6/voicemeeterlib/vban.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.4/PKG-INFO` & `voicemeeter_api-2.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicemeeter-api
-Version: 2.3.4
+Version: 2.3.6
 Summary: A Python wrapper for the Voiceemeter API
 Home-page: https://github.com/onyx-and-iris/voicemeeter-api-python
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

