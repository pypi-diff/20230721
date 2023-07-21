# Comparing `tmp/string_grab-0.0.5.tar.gz` & `tmp/string_grab-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "string_grab-0.0.5.tar", last modified: Fri Jul 21 06:24:39 2023, max compression
+gzip compressed data, was "string_grab-0.0.6.tar", last modified: Fri Jul 21 06:41:33 2023, max compression
```

## Comparing `string_grab-0.0.5.tar` & `string_grab-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 06:24:39.195934 string_grab-0.0.5/
--rw-rw-r--   0 omega     (1000) omega     (1000)    18092 2023-07-20 11:00:34.000000 string_grab-0.0.5/LICENSE
--rw-rw-r--   0 omega     (1000) omega     (1000)     1013 2023-07-21 06:24:39.191934 string_grab-0.0.5/PKG-INFO
--rw-rw-r--   0 omega     (1000) omega     (1000)      624 2023-07-20 16:34:40.000000 string_grab-0.0.5/README.md
--rw-rw-r--   0 omega     (1000) omega     (1000)       38 2023-07-21 06:24:39.195934 string_grab-0.0.5/setup.cfg
--rw-rw-r--   0 omega     (1000) omega     (1000)      543 2023-07-21 06:22:15.000000 string_grab-0.0.5/setup.py
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 06:24:39.191934 string_grab-0.0.5/string_grab/
--rw-rw-r--   0 omega     (1000) omega     (1000)       64 2023-07-20 11:00:34.000000 string_grab-0.0.5/string_grab/__init__.py
--rwxrwxr-x   0 omega     (1000) omega     (1000)     2558 2023-07-21 06:19:23.000000 string_grab-0.0.5/string_grab/string_grab.py
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 06:24:39.191934 string_grab-0.0.5/string_grab.egg-info/
--rw-rw-r--   0 omega     (1000) omega     (1000)     1013 2023-07-21 06:24:39.000000 string_grab-0.0.5/string_grab.egg-info/PKG-INFO
--rw-rw-r--   0 omega     (1000) omega     (1000)      217 2023-07-21 06:24:39.000000 string_grab-0.0.5/string_grab.egg-info/SOURCES.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)        1 2023-07-21 06:24:39.000000 string_grab-0.0.5/string_grab.egg-info/dependency_links.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)       12 2023-07-21 06:24:39.000000 string_grab-0.0.5/string_grab.egg-info/top_level.txt
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 06:41:33.771049 string_grab-0.0.6/
+-rw-rw-r--   0 omega     (1000) omega     (1000)    18092 2023-07-20 11:00:34.000000 string_grab-0.0.6/LICENSE
+-rw-rw-r--   0 omega     (1000) omega     (1000)     1013 2023-07-21 06:41:33.771049 string_grab-0.0.6/PKG-INFO
+-rw-rw-r--   0 omega     (1000) omega     (1000)      624 2023-07-20 16:34:40.000000 string_grab-0.0.6/README.md
+-rw-rw-r--   0 omega     (1000) omega     (1000)       38 2023-07-21 06:41:33.771049 string_grab-0.0.6/setup.cfg
+-rw-rw-r--   0 omega     (1000) omega     (1000)      543 2023-07-21 06:40:44.000000 string_grab-0.0.6/setup.py
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 06:41:33.771049 string_grab-0.0.6/string_grab/
+-rw-rw-r--   0 omega     (1000) omega     (1000)       64 2023-07-20 11:00:34.000000 string_grab-0.0.6/string_grab/__init__.py
+-rwxrwxr-x   0 omega     (1000) omega     (1000)     2565 2023-07-21 06:37:05.000000 string_grab-0.0.6/string_grab/string_grab.py
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 06:41:33.771049 string_grab-0.0.6/string_grab.egg-info/
+-rw-rw-r--   0 omega     (1000) omega     (1000)     1013 2023-07-21 06:41:33.000000 string_grab-0.0.6/string_grab.egg-info/PKG-INFO
+-rw-rw-r--   0 omega     (1000) omega     (1000)      217 2023-07-21 06:41:33.000000 string_grab-0.0.6/string_grab.egg-info/SOURCES.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)        1 2023-07-21 06:41:33.000000 string_grab-0.0.6/string_grab.egg-info/dependency_links.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)       12 2023-07-21 06:41:33.000000 string_grab-0.0.6/string_grab.egg-info/top_level.txt
```

### Comparing `string_grab-0.0.5/LICENSE` & `string_grab-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `string_grab-0.0.5/PKG-INFO` & `string_grab-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string_grab
-Version: 0.0.5
+Version: 0.0.6
 Summary: Extract one or multiple substrings between two start and end strings.
 Home-page: https://github.com/Julynx/string_grab
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Maintainer: Julio Cabria
 Maintainer-email: juliocabria@tutanota.com
 License: GPLv2
```

### Comparing `string_grab-0.0.5/README.md` & `string_grab-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `string_grab-0.0.5/setup.py` & `string_grab-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="string_grab",
-    version="0.0.5",
+    version="0.0.6",
     author="Julio Cabria",
     author_email="juliocabria@tutanota.com",
     maintainer="Julio Cabria",
     maintainer_email="juliocabria@tutanota.com",
     url="https://github.com/Julynx/string_grab",
     description=("Extract one or multiple substrings "
                  "between two start and end strings."),
```

### Comparing `string_grab-0.0.5/string_grab/string_grab.py` & `string_grab-0.0.6/string_grab/string_grab.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,9 +86,9 @@
         TypeError: If any of the arguments is not of the expected type.
     """
     for arg_name, arg_value in args_dict.items():
 
         if isinstance(arg_value, expects):
             continue
 
-        raise TypeError(f"{func_name}() expected str for '{arg_name}', "
-                        f"got {type(arg_value).__name__} instead.")
+        raise TypeError(f"{func_name}() expected {expects.__name__} for "
+                        f"'{arg_name}', got {type(arg_value).__name__}.")
```

### Comparing `string_grab-0.0.5/string_grab.egg-info/PKG-INFO` & `string_grab-0.0.6/string_grab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string-grab
-Version: 0.0.5
+Version: 0.0.6
 Summary: Extract one or multiple substrings between two start and end strings.
 Home-page: https://github.com/Julynx/string_grab
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Maintainer: Julio Cabria
 Maintainer-email: juliocabria@tutanota.com
 License: GPLv2
```

