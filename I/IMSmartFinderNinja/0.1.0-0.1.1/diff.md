# Comparing `tmp/IMSmartFinderNinja-0.1.0.tar.gz` & `tmp/IMSmartFinderNinja-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMSmartFinderNinja-0.1.0.tar", last modified: Mon Jul 17 10:33:49 2023, max compression
+gzip compressed data, was "IMSmartFinderNinja-0.1.1.tar", last modified: Fri Jul 21 09:17:51 2023, max compression
```

## Comparing `IMSmartFinderNinja-0.1.0.tar` & `IMSmartFinderNinja-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 10:33:49.971046 IMSmartFinderNinja-0.1.0/
--rw-rw-rw-   0        0        0        0 2023-07-12 22:27:16.000000 IMSmartFinderNinja-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      638 2023-07-17 10:33:49.971046 IMSmartFinderNinja-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      108 2023-07-12 22:50:02.000000 IMSmartFinderNinja-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      779 2023-07-17 10:33:49.974041 IMSmartFinderNinja-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-17 10:33:49.913875 IMSmartFinderNinja-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-17 10:33:49.954915 IMSmartFinderNinja-0.1.0/src/IMSmartFinderNinja.egg-info/
--rw-rw-rw-   0        0        0      638 2023-07-17 10:33:49.000000 IMSmartFinderNinja-0.1.0/src/IMSmartFinderNinja.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-07-17 10:33:49.000000 IMSmartFinderNinja-0.1.0/src/IMSmartFinderNinja.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 10:33:49.000000 IMSmartFinderNinja-0.1.0/src/IMSmartFinderNinja.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-17 10:33:49.000000 IMSmartFinderNinja-0.1.0/src/IMSmartFinderNinja.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-17 10:33:49.966757 IMSmartFinderNinja-0.1.0/src/Ninja/
--rw-rw-rw-   0        0        0    23527 2023-07-17 10:33:01.000000 IMSmartFinderNinja-0.1.0/src/Ninja/Ninja_Finder.py
--rw-rw-rw-   0        0        0        0 2023-07-12 22:27:17.000000 IMSmartFinderNinja-0.1.0/src/Ninja/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:17:50.992662 IMSmartFinderNinja-0.1.1/
+-rw-rw-rw-   0        0        0        0 2023-07-12 22:27:16.000000 IMSmartFinderNinja-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      638 2023-07-21 09:17:50.992764 IMSmartFinderNinja-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2023-07-12 22:50:02.000000 IMSmartFinderNinja-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      779 2023-07-21 09:17:50.994845 IMSmartFinderNinja-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-21 09:17:50.964661 IMSmartFinderNinja-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-21 09:17:50.982650 IMSmartFinderNinja-0.1.1/src/IMSmartFinderNinja.egg-info/
+-rw-rw-rw-   0        0        0      638 2023-07-21 09:17:50.000000 IMSmartFinderNinja-0.1.1/src/IMSmartFinderNinja.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-07-21 09:17:50.000000 IMSmartFinderNinja-0.1.1/src/IMSmartFinderNinja.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 09:17:50.000000 IMSmartFinderNinja-0.1.1/src/IMSmartFinderNinja.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-21 09:17:50.000000 IMSmartFinderNinja-0.1.1/src/IMSmartFinderNinja.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 09:17:50.990660 IMSmartFinderNinja-0.1.1/src/Ninja/
+-rw-rw-rw-   0        0        0    23711 2023-07-21 09:16:53.000000 IMSmartFinderNinja-0.1.1/src/Ninja/Ninja_Finder.py
+-rw-rw-rw-   0        0        0        0 2023-07-12 22:27:17.000000 IMSmartFinderNinja-0.1.1/src/Ninja/__init__.py
```

### Comparing `IMSmartFinderNinja-0.1.0/PKG-INFO` & `IMSmartFinderNinja-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMSmartFinderNinja
-Version: 0.1.0
+Version: 0.1.1
 Summary: this version is for smart solution for data quality Assuracne Engineering automation
 Home-page: https://github.com/Mohamed-ElhajAbdou/IMSmartFinderNinja
 Author: Mohamed Elhajabdou
 Author-email: mohamedelsayedmohammed.2020@gmail.com
 Project-URL: Bug Tracker, https://github.com/Mohamed-ElhajAbdou/IMSmartFinderNinja/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IMSmartFinderNinja-0.1.0/setup.cfg` & `IMSmartFinderNinja-0.1.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2049 4d53 6d61 7274 4669 6e64 6572   = IMSmartFinder
 00000020: 4e69 6e6a 610d 0a76 6572 7369 6f6e 203d  Ninja..version =
-00000030: 2030 2e31 2e30 0d0a 6175 7468 6f72 203d   0.1.0..author =
+00000030: 2030 2e31 2e31 0d0a 6175 7468 6f72 203d   0.1.1..author =
 00000040: 204d 6f68 616d 6564 2045 6c68 616a 6162   Mohamed Elhajab
 00000050: 646f 750d 0a61 7574 686f 725f 656d 6169  dou..author_emai
 00000060: 6c20 3d20 6d6f 6861 6d65 6465 6c73 6179  l = mohamedelsay
 00000070: 6564 6d6f 6861 6d6d 6564 2e32 3032 3040  edmohammed.2020@
 00000080: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000090: 6970 7469 6f6e 203d 2074 6869 7320 7665  iption = this ve
 000000a0: 7273 696f 6e20 6973 2066 6f72 2073 6d61  rsion is for sma
```

### Comparing `IMSmartFinderNinja-0.1.0/src/IMSmartFinderNinja.egg-info/PKG-INFO` & `IMSmartFinderNinja-0.1.1/src/IMSmartFinderNinja.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMSmartFinderNinja
-Version: 0.1.0
+Version: 0.1.1
 Summary: this version is for smart solution for data quality Assuracne Engineering automation
 Home-page: https://github.com/Mohamed-ElhajAbdou/IMSmartFinderNinja
 Author: Mohamed Elhajabdou
 Author-email: mohamedelsayedmohammed.2020@gmail.com
 Project-URL: Bug Tracker, https://github.com/Mohamed-ElhajAbdou/IMSmartFinderNinja/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IMSmartFinderNinja-0.1.0/src/Ninja/Ninja_Finder.py` & `IMSmartFinderNinja-0.1.1/src/Ninja/Ninja_Finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,18 +51,23 @@
 
     
     @staticmethod
     def convert_column_to_list(data_frame, column):
         column_values = list(data_frame[column])
         return column_values
     
-    def covert_list_lower_case(original_list):
-        
-        lowercase_list = [item.lower() for item in original_list]
 
+    def convert_to_lower_string(data):
+        if isinstance(data, str):
+            return data.lower()
+        else:
+            return str(data).lower()
+
+    def covert_list_lower_case(original_list):
+        lowercase_list = [DataProcessor.convert_to_lower_string(item) for item in original_list]
         return lowercase_list
 
     @staticmethod
     def get_unique_from_lists(original_list):
         unique_values = set(original_list)
         return unique_values
```

