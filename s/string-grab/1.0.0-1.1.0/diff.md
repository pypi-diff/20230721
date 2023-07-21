# Comparing `tmp/string_grab-1.0.0.tar.gz` & `tmp/string_grab-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "string_grab-1.0.0.tar", last modified: Fri Jul 21 12:02:04 2023, max compression
+gzip compressed data, was "string_grab-1.1.0.tar", last modified: Fri Jul 21 19:08:32 2023, max compression
```

## Comparing `string_grab-1.0.0.tar` & `string_grab-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 12:02:04.793213 string_grab-1.0.0/
--rw-rw-r--   0 omega     (1000) omega     (1000)    18092 2023-07-20 11:00:34.000000 string_grab-1.0.0/LICENSE
--rw-rw-r--   0 omega     (1000) omega     (1000)     1013 2023-07-21 12:02:04.793213 string_grab-1.0.0/PKG-INFO
--rw-rw-r--   0 omega     (1000) omega     (1000)      624 2023-07-20 16:34:40.000000 string_grab-1.0.0/README.md
--rw-rw-r--   0 omega     (1000) omega     (1000)       38 2023-07-21 12:02:04.793213 string_grab-1.0.0/setup.cfg
--rw-rw-r--   0 omega     (1000) omega     (1000)      543 2023-07-21 12:01:51.000000 string_grab-1.0.0/setup.py
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 12:02:04.793213 string_grab-1.0.0/string_grab/
--rw-rw-r--   0 omega     (1000) omega     (1000)       64 2023-07-20 11:00:34.000000 string_grab-1.0.0/string_grab/__init__.py
--rwxrwxr-x   0 omega     (1000) omega     (1000)     2508 2023-07-21 11:49:22.000000 string_grab-1.0.0/string_grab/string_grab.py
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 12:02:04.793213 string_grab-1.0.0/string_grab.egg-info/
--rw-rw-r--   0 omega     (1000) omega     (1000)     1013 2023-07-21 12:02:04.000000 string_grab-1.0.0/string_grab.egg-info/PKG-INFO
--rw-rw-r--   0 omega     (1000) omega     (1000)      217 2023-07-21 12:02:04.000000 string_grab-1.0.0/string_grab.egg-info/SOURCES.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)        1 2023-07-21 12:02:04.000000 string_grab-1.0.0/string_grab.egg-info/dependency_links.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)       12 2023-07-21 12:02:04.000000 string_grab-1.0.0/string_grab.egg-info/top_level.txt
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 19:08:32.087725 string_grab-1.1.0/
+-rw-rw-r--   0 omega     (1000) omega     (1000)    18092 2023-07-20 11:00:34.000000 string_grab-1.1.0/LICENSE
+-rw-rw-r--   0 omega     (1000) omega     (1000)     1013 2023-07-21 19:08:32.087725 string_grab-1.1.0/PKG-INFO
+-rw-rw-r--   0 omega     (1000) omega     (1000)      624 2023-07-20 16:34:40.000000 string_grab-1.1.0/README.md
+-rw-rw-r--   0 omega     (1000) omega     (1000)       38 2023-07-21 19:08:32.087725 string_grab-1.1.0/setup.cfg
+-rw-rw-r--   0 omega     (1000) omega     (1000)      543 2023-07-21 18:42:56.000000 string_grab-1.1.0/setup.py
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 19:08:32.087725 string_grab-1.1.0/string_grab/
+-rw-rw-r--   0 omega     (1000) omega     (1000)       96 2023-07-21 18:44:51.000000 string_grab-1.1.0/string_grab/__init__.py
+-rwxrwxr-x   0 omega     (1000) omega     (1000)     3465 2023-07-21 18:47:04.000000 string_grab-1.1.0/string_grab/string_grab.py
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-21 19:08:32.087725 string_grab-1.1.0/string_grab.egg-info/
+-rw-rw-r--   0 omega     (1000) omega     (1000)     1013 2023-07-21 19:08:32.000000 string_grab-1.1.0/string_grab.egg-info/PKG-INFO
+-rw-rw-r--   0 omega     (1000) omega     (1000)      217 2023-07-21 19:08:32.000000 string_grab-1.1.0/string_grab.egg-info/SOURCES.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)        1 2023-07-21 19:08:32.000000 string_grab-1.1.0/string_grab.egg-info/dependency_links.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)       12 2023-07-21 19:08:32.000000 string_grab-1.1.0/string_grab.egg-info/top_level.txt
```

### Comparing `string_grab-1.0.0/LICENSE` & `string_grab-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `string_grab-1.0.0/PKG-INFO` & `string_grab-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string_grab
-Version: 1.0.0
+Version: 1.1.0
 Summary: Extract one or multiple substrings between two start and end strings.
 Home-page: https://github.com/Julynx/string_grab
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Maintainer: Julio Cabria
 Maintainer-email: juliocabria@tutanota.com
 License: GPLv2
```

### Comparing `string_grab-1.0.0/README.md` & `string_grab-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `string_grab-1.0.0/setup.py` & `string_grab-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="string_grab",
-    version="1.0.0",
+    version="1.1.0",
     author="Julio Cabria",
     author_email="juliocabria@tutanota.com",
     maintainer="Julio Cabria",
     maintainer_email="juliocabria@tutanota.com",
     url="https://github.com/Julynx/string_grab",
     description=("Extract one or multiple substrings "
                  "between two start and end strings."),
```

### Comparing `string_grab-1.0.0/string_grab/string_grab.py` & `string_grab-1.1.0/string_grab/string_grab.py`

 * *Files 13% similar despite different names*

```diff
@@ -67,14 +67,43 @@
             _ = parts[1]  # Raises IndexError if 'end' not in 'text'.
             yield parts[0]
 
         except IndexError:
             return
 
 
+def inject(text, insert, *, start, end):
+    """
+    Inject 'insert' in 'text' between two 'start' and 'end' strings.
+
+    Args:
+        text (str): The base string.
+        insert (str): The string to be injected.
+        start (str): The string before the injection point.
+        end (str): The string after the injection point.
+
+    Returns:
+        str: The 'text' string with the 'insert' string injected.
+
+    Raises:
+        TypeError: If any of the arguments is not a string.
+        LookupError: If the 'start' or 'end' strings are not in 'text'.
+    """
+    _validate_args(func_name="inject", args_dict=locals(), expects=str)
+
+    try:
+        prev_parts = text.split(start, 1)
+        next_parts = prev_parts[1].split(end, 1)
+        return "".join((prev_parts[0], start, insert, end, next_parts[1]))
+
+    except IndexError as index_error:
+        raise LookupError("Could not find 'start' or 'end' in 'text'.") \
+            from index_error
+
+
 def _validate_args(*, func_name, args_dict, expects):
     """
     Raises a TypeError if any of the arguments is not of the expected type.
 
     Args:
         func_name (str): The name of the function.
         args_dict (dict): The arguments dictionary.
```

### Comparing `string_grab-1.0.0/string_grab.egg-info/PKG-INFO` & `string_grab-1.1.0/string_grab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string-grab
-Version: 1.0.0
+Version: 1.1.0
 Summary: Extract one or multiple substrings between two start and end strings.
 Home-page: https://github.com/Julynx/string_grab
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Maintainer: Julio Cabria
 Maintainer-email: juliocabria@tutanota.com
 License: GPLv2
```

