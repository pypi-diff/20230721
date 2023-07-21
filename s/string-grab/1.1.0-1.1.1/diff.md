# Comparing `tmp/string_grab-1.1.0.tar.gz` & `tmp/string_grab-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "string_grab-1.1.0.tar", last modified: Fri Jul 21 19:08:32 2023, max compression
+gzip compressed data, was "string_grab-1.1.1.tar", last modified: Fri Jul 21 19:36:53 2023, max compression
```

## Comparing `string_grab-1.1.0.tar` & `string_grab-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 19:08:32.087725 string_grab-1.1.0/
--rw-rw-r--   0 omega     (1000) omega     (1000)    18092 2023-07-20 11:00:34.000000 string_grab-1.1.0/LICENSE
--rw-rw-r--   0 omega     (1000) omega     (1000)     1013 2023-07-21 19:08:32.087725 string_grab-1.1.0/PKG-INFO
--rw-rw-r--   0 omega     (1000) omega     (1000)      624 2023-07-20 16:34:40.000000 string_grab-1.1.0/README.md
--rw-rw-r--   0 omega     (1000) omega     (1000)       38 2023-07-21 19:08:32.087725 string_grab-1.1.0/setup.cfg
--rw-rw-r--   0 omega     (1000) omega     (1000)      543 2023-07-21 18:42:56.000000 string_grab-1.1.0/setup.py
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 19:08:32.087725 string_grab-1.1.0/string_grab/
--rw-rw-r--   0 omega     (1000) omega     (1000)       96 2023-07-21 18:44:51.000000 string_grab-1.1.0/string_grab/__init__.py
--rwxrwxr-x   0 omega     (1000) omega     (1000)     3465 2023-07-21 18:47:04.000000 string_grab-1.1.0/string_grab/string_grab.py
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 19:08:32.087725 string_grab-1.1.0/string_grab.egg-info/
--rw-rw-r--   0 omega     (1000) omega     (1000)     1013 2023-07-21 19:08:32.000000 string_grab-1.1.0/string_grab.egg-info/PKG-INFO
--rw-rw-r--   0 omega     (1000) omega     (1000)      217 2023-07-21 19:08:32.000000 string_grab-1.1.0/string_grab.egg-info/SOURCES.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)        1 2023-07-21 19:08:32.000000 string_grab-1.1.0/string_grab.egg-info/dependency_links.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)       12 2023-07-21 19:08:32.000000 string_grab-1.1.0/string_grab.egg-info/top_level.txt
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 19:36:53.636788 string_grab-1.1.1/
+-rw-rw-r--   0 omega     (1000) omega     (1000)    18092 2023-07-20 11:00:34.000000 string_grab-1.1.1/LICENSE
+-rw-rw-r--   0 omega     (1000) omega     (1000)     1330 2023-07-21 19:36:53.632788 string_grab-1.1.1/PKG-INFO
+-rw-rw-r--   0 omega     (1000) omega     (1000)      941 2023-07-21 19:36:16.000000 string_grab-1.1.1/README.md
+-rw-rw-r--   0 omega     (1000) omega     (1000)       38 2023-07-21 19:36:53.636788 string_grab-1.1.1/setup.cfg
+-rw-rw-r--   0 omega     (1000) omega     (1000)      543 2023-07-21 19:32:57.000000 string_grab-1.1.1/setup.py
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 19:36:53.632788 string_grab-1.1.1/string_grab/
+-rw-rw-r--   0 omega     (1000) omega     (1000)       96 2023-07-21 18:44:51.000000 string_grab-1.1.1/string_grab/__init__.py
+-rwxrwxr-x   0 omega     (1000) omega     (1000)     3465 2023-07-21 18:47:04.000000 string_grab-1.1.1/string_grab/string_grab.py
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 19:36:53.632788 string_grab-1.1.1/string_grab.egg-info/
+-rw-rw-r--   0 omega     (1000) omega     (1000)     1330 2023-07-21 19:36:53.000000 string_grab-1.1.1/string_grab.egg-info/PKG-INFO
+-rw-rw-r--   0 omega     (1000) omega     (1000)      217 2023-07-21 19:36:53.000000 string_grab-1.1.1/string_grab.egg-info/SOURCES.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)        1 2023-07-21 19:36:53.000000 string_grab-1.1.1/string_grab.egg-info/dependency_links.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)       12 2023-07-21 19:36:53.000000 string_grab-1.1.1/string_grab.egg-info/top_level.txt
```

### Comparing `string_grab-1.1.0/LICENSE` & `string_grab-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `string_grab-1.1.0/PKG-INFO` & `string_grab-1.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string_grab
-Version: 1.1.0
+Version: 1.1.1
 Summary: Extract one or multiple substrings between two start and end strings.
 Home-page: https://github.com/Julynx/string_grab
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Maintainer: Julio Cabria
 Maintainer-email: juliocabria@tutanota.com
 License: GPLv2
@@ -35,7 +35,20 @@
 
 for number in grab_all(text, start="Mobile: ", end="\n"):
     print(number)
 
 >> "715-523-1076"
 >> "715-563-3967"
 ```
+```python
+from string_grab import inject
+
+inject(text, "611 Waterwheel Ln", start="Street: ", end="\n")
+
+>> """Gender: female
+   Race: White
+   Birthday: 3/23/1973 (50 years old)
+   Mobile: 715-523-1076
+   Mobile: 715-563-3967
+   Street: 611 Waterwheel Ln
+   City, State, Zip: Eau Claire, Wisconsin(WI), 54701"""
+```
```

### Comparing `string_grab-1.1.0/setup.py` & `string_grab-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="string_grab",
-    version="1.1.0",
+    version="1.1.1",
     author="Julio Cabria",
     author_email="juliocabria@tutanota.com",
     maintainer="Julio Cabria",
     maintainer_email="juliocabria@tutanota.com",
     url="https://github.com/Julynx/string_grab",
     description=("Extract one or multiple substrings "
                  "between two start and end strings."),
```

### Comparing `string_grab-1.1.0/string_grab/string_grab.py` & `string_grab-1.1.1/string_grab/string_grab.py`

 * *Files identical despite different names*

### Comparing `string_grab-1.1.0/string_grab.egg-info/PKG-INFO` & `string_grab-1.1.1/string_grab.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string-grab
-Version: 1.1.0
+Version: 1.1.1
 Summary: Extract one or multiple substrings between two start and end strings.
 Home-page: https://github.com/Julynx/string_grab
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Maintainer: Julio Cabria
 Maintainer-email: juliocabria@tutanota.com
 License: GPLv2
@@ -35,7 +35,20 @@
 
 for number in grab_all(text, start="Mobile: ", end="\n"):
     print(number)
 
 >> "715-523-1076"
 >> "715-563-3967"
 ```
+```python
+from string_grab import inject
+
+inject(text, "611 Waterwheel Ln", start="Street: ", end="\n")
+
+>> """Gender: female
+   Race: White
+   Birthday: 3/23/1973 (50 years old)
+   Mobile: 715-523-1076
+   Mobile: 715-563-3967
+   Street: 611 Waterwheel Ln
+   City, State, Zip: Eau Claire, Wisconsin(WI), 54701"""
+```
```

