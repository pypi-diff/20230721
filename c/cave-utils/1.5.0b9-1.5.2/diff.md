# Comparing `tmp/cave_utils-1.5.0b9.tar.gz` & `tmp/cave_utils-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cave_utils-1.5.0b9.tar", last modified: Tue Jun 27 13:55:57 2023, max compression
+gzip compressed data, was "cave_utils-1.5.2.tar", last modified: Fri Jul 21 14:24:22 2023, max compression
```

## Comparing `cave_utils-1.5.0b9.tar` & `cave_utils-1.5.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-27 13:55:57.724303 cave_utils-1.5.0b9/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    11357 2023-06-13 15:21:54.000000 cave_utils-1.5.0b9/LICENSE
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      631 2023-06-13 15:22:15.000000 cave_utils-1.5.0b9/NOTICE.md
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1606 2023-06-27 13:55:57.724303 cave_utils-1.5.0b9/PKG-INFO
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      927 2023-06-13 20:25:36.000000 cave_utils-1.5.0b9/README.md
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-27 13:55:57.724303 cave_utils-1.5.0b9/cave_utils/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      131 2023-06-22 13:25:50.000000 cave_utils-1.5.0b9/cave_utils/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1798 2023-06-27 13:54:10.000000 cave_utils-1.5.0b9/cave_utils/arguments.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1325 2023-06-16 14:30:37.000000 cave_utils-1.5.0b9/cave_utils/log.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      257 2023-06-16 14:28:26.000000 cave_utils-1.5.0b9/cave_utils/socket.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    54678 2023-06-16 14:30:37.000000 cave_utils-1.5.0b9/cave_utils/validator.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-27 13:55:57.724303 cave_utils-1.5.0b9/cave_utils.egg-info/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1606 2023-06-27 13:55:57.000000 cave_utils-1.5.0b9/cave_utils.egg-info/PKG-INFO
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      383 2023-06-27 13:55:57.000000 cave_utils-1.5.0b9/cave_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-06-27 13:55:57.000000 cave_utils-1.5.0b9/cave_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       13 2023-06-27 13:55:57.000000 cave_utils-1.5.0b9/cave_utils.egg-info/requires.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       11 2023-06-27 13:55:57.000000 cave_utils-1.5.0b9/cave_utils.egg-info/top_level.txt
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      101 2023-06-13 14:42:48.000000 cave_utils-1.5.0b9/pyproject.toml
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)       79 2023-06-27 13:55:57.724303 cave_utils-1.5.0b9/setup.cfg
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      997 2023-06-27 13:55:30.000000 cave_utils-1.5.0b9/setup.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-27 13:55:57.724303 cave_utils-1.5.0b9/test/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      305 2023-06-27 13:54:32.000000 cave_utils-1.5.0b9/test/test_arguments.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       39 2023-06-22 13:14:02.000000 cave_utils-1.5.0b9/test/test_import.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-21 14:24:22.186586 cave_utils-1.5.2/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    11357 2023-06-13 15:21:54.000000 cave_utils-1.5.2/LICENSE
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      631 2023-06-13 15:22:15.000000 cave_utils-1.5.2/NOTICE.md
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1602 2023-07-21 14:24:22.186586 cave_utils-1.5.2/PKG-INFO
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      927 2023-06-13 20:25:36.000000 cave_utils-1.5.2/README.md
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-21 14:24:22.186586 cave_utils-1.5.2/cave_utils/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      131 2023-06-22 13:25:50.000000 cave_utils-1.5.2/cave_utils/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1798 2023-06-27 13:54:10.000000 cave_utils-1.5.2/cave_utils/arguments.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1325 2023-06-16 14:30:37.000000 cave_utils-1.5.2/cave_utils/log.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      257 2023-06-16 14:28:26.000000 cave_utils-1.5.2/cave_utils/socket.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    57226 2023-07-21 14:23:54.000000 cave_utils-1.5.2/cave_utils/validator.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-21 14:24:22.186586 cave_utils-1.5.2/cave_utils.egg-info/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1602 2023-07-21 14:24:22.000000 cave_utils-1.5.2/cave_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      383 2023-07-21 14:24:22.000000 cave_utils-1.5.2/cave_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-07-21 14:24:22.000000 cave_utils-1.5.2/cave_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       13 2023-07-21 14:24:22.000000 cave_utils-1.5.2/cave_utils.egg-info/requires.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       11 2023-07-21 14:24:22.000000 cave_utils-1.5.2/cave_utils.egg-info/top_level.txt
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      101 2023-06-13 14:42:48.000000 cave_utils-1.5.2/pyproject.toml
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)       79 2023-07-21 14:24:22.190586 cave_utils-1.5.2/setup.cfg
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      993 2023-07-21 14:18:24.000000 cave_utils-1.5.2/setup.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-21 14:24:22.186586 cave_utils-1.5.2/test/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      305 2023-06-27 13:54:32.000000 cave_utils-1.5.2/test/test_arguments.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       39 2023-06-22 13:14:02.000000 cave_utils-1.5.2/test/test_import.py
```

### Comparing `cave_utils-1.5.0b9/LICENSE` & `cave_utils-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.0b9/NOTICE.md` & `cave_utils-1.5.2/NOTICE.md`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.0b9/PKG-INFO` & `cave_utils-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cave_utils
-Version: 1.5.0b9
+Version: 1.5.2
 Summary: Cave utilities for the CAVE App at the MIT
 Home-page: https://github.com/mit-cave/cave_utils
-Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b9.tar.gz
+Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.2.tar.gz
 Author: Connor Makowski
 Author-email: connor.m.makowski@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cave_utils-1.5.0b9/README.md` & `cave_utils-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.0b9/cave_utils/arguments.py` & `cave_utils-1.5.2/cave_utils/arguments.py`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.0b9/cave_utils/log.py` & `cave_utils-1.5.2/cave_utils/log.py`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.0b9/cave_utils/validator.py` & `cave_utils-1.5.2/cave_utils/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,36 +34,36 @@
                 check_value = value
                 if isinstance(value, dict):
                     check_value = list(value.keys())
                 value_diff = pamda.difference(check_value, accepted_values)
                 if len(value_diff) > 0:
                     self.log.add(
                         path=[field],
-                        msg=f"Invalid values ({value_diff}): Acceptable values are: {accepted_values}",
+                        msg=f"Invalid values ('{value_diff}'): Acceptable values are: {accepted_values}",
                     )
                     continue
             else:
                 if accepted_values is not None and value not in accepted_values:
                     self.log.add(
                         path=[field],
-                        msg=f"Invalid value ({value}): Acceptable values are: {accepted_values}",
+                        msg=f"Invalid value ('{value}'): Acceptable values are: {accepted_values}",
                     )
                     continue
             if field not in self.required_fields + self.optional_fields:
                 self.log.add(
                     path=[field],
-                    msg=f"Unknown field ({field}): Acceptable fields are: {self.required_fields + self.optional_fields}",
+                    msg=f"Unknown field ('{field}'): Acceptable fields are: {self.required_fields + self.optional_fields}",
                     level="warning",
                 )
                 continue
             acceptable_types = self.field_types.get(field, type(None))
             if not isinstance(value, acceptable_types):
                 self.log.add(
                     path=[field],
-                    msg=f"Invalid type ({type(value)}): Acceptable types are: {acceptable_types}",
+                    msg=f"Invalid type ('{type(value)}'): Acceptable types are: {acceptable_types}",
                 )
 
         # Run additional Validations
         try:
             self.additional_validations(**kwargs)
         except Exception as e:
             self.log.add(
@@ -146,14 +146,24 @@
             return False
         return True
 
     def validate_coord_path(self, coord_path: list, prepend_path: list = []):
         if not self.is_coord_path_valid(coord_path):
             self.log.add(path=prepend_path, msg=f"Invalid coordinate path")
 
+    def validate_list(self, data: list, types: tuple, prepend_path: str):
+        if not isinstance(types, tuple):
+            types = (types,)
+        for item in data:
+            if not isinstance(item, types):
+                self.log.add(
+                    path=prepend_path, msg=f"Invalid list type. Item {item} is not of type {types}"
+                )
+                break
+
 
 class NumericDictValidator(CoreValidator):
     def populate_data(self, **kwargs):
         self.field_types = {i: (int, float) for i in self.data.keys()}
         self.required_fields = list(self.data.keys())
         self.optional_fields = []
         self.accepted_values = {}
@@ -186,14 +196,35 @@
             "locale": str,
         }
         self.required_fields = []
         self.optional_fields = list(self.field_types.keys())
         self.accepted_values = {}
 
 
+class legendOverrideValidator(CoreValidator):
+    def populate_data(self, **kwargs):
+        self.field_types = {
+            "scientificPrecision": int,
+            "useScientificFormat": bool,
+            "minLabel": (
+                str,
+                int,
+                float,
+            ),
+            "maxLabel": (
+                str,
+                int,
+                float,
+            ),
+        }
+        self.required_fields = []
+        self.optional_fields = list(self.field_types.keys())
+        self.accepted_values = {}
+
+
 class ColorByOptionValidator(CoreValidator):
     def is_categorical(self):
         if self.data == {}:
             return False
         expected_keys = ["min", "max", "startGradientColor", "endGradientColor"]
         return len(pamda.intersection(expected_keys, list(self.data.keys()))) == 0
 
@@ -276,28 +307,30 @@
             "options": dict,
             "maxValue": (int, float),
             "minValue": (int, float),
             "maxRows": int,
             "minRows": int,
             "rows": int,
             "numberFormat": dict,
+            "legendOverride": dict,
         }
 
         self.allowed_variants = {
             "head": ["column", "row"],
             "text": ["textarea"],
             "num": ["slider"],
             "selector": [
                 "dropdown",
                 "checkbox",
                 "radio",
                 "combobox",
                 "hstepper",
                 "vstepper",
                 "hradio",
+                "nested",
             ],
             "date": ["date", "time", "datetime"],
             "media": ["picture", "video"],
         }
 
         self.accepted_values = {
             "type": ["head", "num", "toggle", "button", "text", "selector", "date", "media"],
@@ -326,39 +359,42 @@
                 "enabled",
                 "variant",
                 "apiCommand",
                 "apiCommandKeys",
                 "maxValue",
                 "minValue",
                 "numberFormat",
+                "legendOverride",
             ],
             "toggle": ["help", "enabled", "apiCommand", "apiCommandKeys"],
             "button": ["help", "enabled", "apiCommand", "apiCommandKeys"],
+            "media": ["help", "variant"],
             "selector": [
                 "help",
                 "enabled",
                 "variant",
                 "apiCommand",
                 "apiCommandKeys",
                 "placeholder",
             ],
             "date": ["help", "enabled", "variant", "apiCommand", "apiCommandKeys", "views"],
-        }.get(validation_type, list(self.field_types.keys()))
+        }.get(validation_type, [])
 
         # Custom code to handle semi-required fields
         # If the prop is a types prop, then these fields are optional
         # Otherwise, they are required
         semi_required_fields = {
             "head": ["name"],
             "text": ["name", "value"],
             "num": ["name", "value"],
             "toggle": ["name", "value"],
             "button": ["name", "value"],
             "selector": ["name", "value", "options"],
             "date": ["name", "value"],
+            "media": ["name", "value"],
         }.get(validation_type, [])
 
         if is_types_prop:
             self.optional_fields += semi_required_fields
         else:
             self.required_fields += semi_required_fields
 
@@ -384,20 +420,51 @@
 
         if validation_type == "num":
             number_format = self.data.get("numberFormat")
             if number_format:
                 NumberFormatValidator(
                     data=number_format, log=self.log, prepend_path=["numberFormat"]
                 )
+            legendOverride = self.data.get("legendOverride")
+            if legendOverride:
+                legendOverrideValidator(
+                    data=legendOverride, log=self.log, prepend_path=["legendOverride"]
+                )
 
         elif validation_type == "selector":
-            if self.data.get("variant") != "checkbox" and len(self.data.get("value", [])) > 1:
+            variant = self.data.get("variant")
+            value = self.data.get("value", [])
+            if variant not in ["checkbox", "nested"] and len(value) > 1:
                 self.error(
                     "Only one value can be selected for this variant.", prepend_path=["value"]
                 )
+            CustomKeyValidator(
+                data=self.data.get("options", {}),
+                log=self.log,
+                prepend_path=["options"],
+                validator=SelectorOptionsValidator,
+                variant=variant,
+                **kwargs,
+            )
+
+
+class SelectorOptionsValidator(CoreValidator):
+    def populate_data(self, **kwargs):
+        self.field_types = {
+            "name": str,
+            "path": list,
+        }
+        self.required_fields = ["name"]
+        self.optional_fields = []
+        self.accepted_values = {}
+        if kwargs.get("variant") == "nested":
+            self.required_fields += ["path"]
+
+    def additional_validations(self, **kwargs):
+        self.validate_list(data=self.data.get("path", []), types=(str,), prepend_path=["path"])
 
 
 class LayoutValidator(CoreValidator):
     def populate_data(self, **kwargs):
         layout_type = self.data.get("type", None)
 
         self.field_types = {
@@ -1202,16 +1269,36 @@
             "groupMatchCategoryLevel": str,
             "order": int,
         }
 
         self.accepted_values = {
             "sizeBy": prop_options,
             "colorBy": prop_options,
-            "groupCalcByColor": ["count", "sum", "mean", "median", "mode", "min", "max"],
-            "groupCalcBySize": ["count", "sum", "mean", "median", "mode", "min", "max"],
+            "groupCalcByColor": [
+                "count",
+                "sum",
+                "mean",
+                "median",
+                "mode",
+                "min",
+                "max",
+                "and",
+                "or",
+            ],
+            "groupCalcBySize": [
+                "count",
+                "sum",
+                "mean",
+                "median",
+                "mode",
+                "min",
+                "max",
+                "and",
+                "or",
+            ],
             "groupMatchCategory": list(categories.keys()),
             "groupMatchCategoryLevel": categories.get(self.data.get("groupMatchCategory"), []),
         }
 
         self.required_fields = ["value", "colorBy"]
 
         self.optional_fields = ["order"]
```

### Comparing `cave_utils-1.5.0b9/cave_utils.egg-info/PKG-INFO` & `cave_utils-1.5.2/cave_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cave-utils
-Version: 1.5.0b9
+Version: 1.5.2
 Summary: Cave utilities for the CAVE App at the MIT
 Home-page: https://github.com/mit-cave/cave_utils
-Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b9.tar.gz
+Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.2.tar.gz
 Author: Connor Makowski
 Author-email: connor.m.makowski@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cave_utils-1.5.0b9/setup.py` & `cave_utils-1.5.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'cave_utils',
   packages=['cave_utils'],
-  version = '1.5.0b9',
+  version = '1.5.2',
   license='MIT',
   description = 'Cave utilities for the CAVE App at the MIT',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Connor Makowski',
   author_email = 'connor.m.makowski@gmail.com',
   url = 'https://github.com/mit-cave/cave_utils',
-  download_url = 'https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b9.tar.gz',
+  download_url = 'https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.2.tar.gz',
   keywords = [],
   install_requires=[
     'pamda>=2.1.2',
   ],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

