# Comparing `tmp/string_grab-0.0.6.tar.gz` & `tmp/string_grab-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "string_grab-0.0.6.tar", last modified: Fri Jul 21 06:41:33 2023, max compression
+gzip compressed data, was "string_grab-1.0.0.tar", last modified: Fri Jul 21 12:02:04 2023, max compression
```

## Comparing `string_grab-0.0.6.tar` & `string_grab-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 06:41:33.771049 string_grab-0.0.6/
--rw-rw-r--   0 omega     (1000) omega     (1000)    18092 2023-07-20 11:00:34.000000 string_grab-0.0.6/LICENSE
--rw-rw-r--   0 omega     (1000) omega     (1000)     1013 2023-07-21 06:41:33.771049 string_grab-0.0.6/PKG-INFO
--rw-rw-r--   0 omega     (1000) omega     (1000)      624 2023-07-20 16:34:40.000000 string_grab-0.0.6/README.md
--rw-rw-r--   0 omega     (1000) omega     (1000)       38 2023-07-21 06:41:33.771049 string_grab-0.0.6/setup.cfg
--rw-rw-r--   0 omega     (1000) omega     (1000)      543 2023-07-21 06:40:44.000000 string_grab-0.0.6/setup.py
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 06:41:33.771049 string_grab-0.0.6/string_grab/
--rw-rw-r--   0 omega     (1000) omega     (1000)       64 2023-07-20 11:00:34.000000 string_grab-0.0.6/string_grab/__init__.py
--rwxrwxr-x   0 omega     (1000) omega     (1000)     2565 2023-07-21 06:37:05.000000 string_grab-0.0.6/string_grab/string_grab.py
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 06:41:33.771049 string_grab-0.0.6/string_grab.egg-info/
--rw-rw-r--   0 omega     (1000) omega     (1000)     1013 2023-07-21 06:41:33.000000 string_grab-0.0.6/string_grab.egg-info/PKG-INFO
--rw-rw-r--   0 omega     (1000) omega     (1000)      217 2023-07-21 06:41:33.000000 string_grab-0.0.6/string_grab.egg-info/SOURCES.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)        1 2023-07-21 06:41:33.000000 string_grab-0.0.6/string_grab.egg-info/dependency_links.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)       12 2023-07-21 06:41:33.000000 string_grab-0.0.6/string_grab.egg-info/top_level.txt
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 12:02:04.793213 string_grab-1.0.0/
+-rw-rw-r--   0 omega     (1000) omega     (1000)    18092 2023-07-20 11:00:34.000000 string_grab-1.0.0/LICENSE
+-rw-rw-r--   0 omega     (1000) omega     (1000)     1013 2023-07-21 12:02:04.793213 string_grab-1.0.0/PKG-INFO
+-rw-rw-r--   0 omega     (1000) omega     (1000)      624 2023-07-20 16:34:40.000000 string_grab-1.0.0/README.md
+-rw-rw-r--   0 omega     (1000) omega     (1000)       38 2023-07-21 12:02:04.793213 string_grab-1.0.0/setup.cfg
+-rw-rw-r--   0 omega     (1000) omega     (1000)      543 2023-07-21 12:01:51.000000 string_grab-1.0.0/setup.py
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 12:02:04.793213 string_grab-1.0.0/string_grab/
+-rw-rw-r--   0 omega     (1000) omega     (1000)       64 2023-07-20 11:00:34.000000 string_grab-1.0.0/string_grab/__init__.py
+-rwxrwxr-x   0 omega     (1000) omega     (1000)     2508 2023-07-21 11:49:22.000000 string_grab-1.0.0/string_grab/string_grab.py
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 12:02:04.793213 string_grab-1.0.0/string_grab.egg-info/
+-rw-rw-r--   0 omega     (1000) omega     (1000)     1013 2023-07-21 12:02:04.000000 string_grab-1.0.0/string_grab.egg-info/PKG-INFO
+-rw-rw-r--   0 omega     (1000) omega     (1000)      217 2023-07-21 12:02:04.000000 string_grab-1.0.0/string_grab.egg-info/SOURCES.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)        1 2023-07-21 12:02:04.000000 string_grab-1.0.0/string_grab.egg-info/dependency_links.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)       12 2023-07-21 12:02:04.000000 string_grab-1.0.0/string_grab.egg-info/top_level.txt
```

### Comparing `string_grab-0.0.6/LICENSE` & `string_grab-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `string_grab-0.0.6/PKG-INFO` & `string_grab-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string_grab
-Version: 0.0.6
+Version: 1.0.0
 Summary: Extract one or multiple substrings between two start and end strings.
 Home-page: https://github.com/Julynx/string_grab
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Maintainer: Julio Cabria
 Maintainer-email: juliocabria@tutanota.com
 License: GPLv2
```

### Comparing `string_grab-0.0.6/README.md` & `string_grab-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `string_grab-0.0.6/setup.py` & `string_grab-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="string_grab",
-    version="0.0.6",
+    version="1.0.0",
     author="Julio Cabria",
     author_email="juliocabria@tutanota.com",
     maintainer="Julio Cabria",
     maintainer_email="juliocabria@tutanota.com",
     url="https://github.com/Julynx/string_grab",
     description=("Extract one or multiple substrings "
                  "between two start and end strings."),
```

### Comparing `string_grab-0.0.6/string_grab/string_grab.py` & `string_grab-1.0.0/string_grab/string_grab.py`

 * *Files 26% similar despite different names*

```diff
@@ -24,22 +24,22 @@
 
     Raises:
         TypeError: If the 'text', 'start' or 'end' arguments are not strings.
         LookupError: If the 'start' or 'end' strings are not in 'text'.
     """
     _validate_args(func_name="grab", args_dict=locals(), expects=str)
 
-    len_start = len(start)
-    start_index = text.find(start)
-    end_index = text.find(end, start_index + len_start)
-
-    if -1 in (start_index, end_index):
-        raise LookupError("Could not find 'start' or 'end' in 'text'.")
-
-    return text[start_index + len_start:end_index]
+    try:
+        parts = text.split(start, 1)[1].split(end, 1)
+        _ = parts[1]  # Raises IndexError if 'end' not in 'text'.
+        return parts[0]
+
+    except IndexError as index_error:
+        raise LookupError("Could not find 'start' or 'end' in 'text'.") \
+            from index_error
 
 
 def grab_all(text, *, start, end):
     """
     Yield all substrings from a string.
 
     Usage:
@@ -55,26 +55,24 @@
         str: The next substring between the 'start' and 'end' strings.
 
     Raises:
         TypeError: If the 'text', 'start' or 'end' arguments are not strings.
     """
     _validate_args(func_name="grab_all", args_dict=locals(), expects=str)
 
-    len_start = len(start)
-    len_end = len(end)
-
     while True:
-        start_index = text.find(start)
-        end_index = text.find(end, start_index + len_start)
 
-        if -1 in (start_index, end_index):
-            return
+        try:
+            text = text.split(start, 1)[1]
+            parts = text.split(end, 1)
+            _ = parts[1]  # Raises IndexError if 'end' not in 'text'.
+            yield parts[0]
 
-        yield text[start_index + len_start:end_index]
-        text = text[end_index + len_end:]
+        except IndexError:
+            return
 
 
 def _validate_args(*, func_name, args_dict, expects):
     """
     Raises a TypeError if any of the arguments is not of the expected type.
 
     Args:
```

### Comparing `string_grab-0.0.6/string_grab.egg-info/PKG-INFO` & `string_grab-1.0.0/string_grab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string-grab
-Version: 0.0.6
+Version: 1.0.0
 Summary: Extract one or multiple substrings between two start and end strings.
 Home-page: https://github.com/Julynx/string_grab
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Maintainer: Julio Cabria
 Maintainer-email: juliocabria@tutanota.com
 License: GPLv2
```

