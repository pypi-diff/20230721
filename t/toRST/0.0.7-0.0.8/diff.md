# Comparing `tmp/toRST-0.0.7.tar.gz` & `tmp/toRST-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toRST-0.0.7.tar", last modified: Fri Jul 21 02:32:32 2023, max compression
+gzip compressed data, was "toRST-0.0.8.tar", last modified: Fri Jul 21 03:16:50 2023, max compression
```

## Comparing `toRST-0.0.7.tar` & `toRST-0.0.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 02:32:32.002007 toRST-0.0.7/
--rw-r--r--   0 jreyno     (501) staff       (20)     1085 2023-07-18 19:42:12.000000 toRST-0.0.7/LICENSE
--rw-r--r--   0 jreyno     (501) staff       (20)     2617 2023-07-21 02:32:32.002060 toRST-0.0.7/PKG-INFO
--rw-r--r--   0 jreyno     (501) staff       (20)     1222 2023-07-21 02:00:59.000000 toRST-0.0.7/README.md
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 02:32:31.999413 toRST-0.0.7/csv2rst/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.7/csv2rst/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)      488 2023-07-18 16:07:34.000000 toRST-0.0.7/csv2rst/csv2rst.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 02:32:32.000092 toRST-0.0.7/funcs/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.7/funcs/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)     1179 2023-07-18 16:07:34.000000 toRST-0.0.7/funcs/command.py
--rw-r--r--   0 jreyno     (501) staff       (20)       76 2023-07-18 16:07:34.000000 toRST-0.0.7/funcs/funcs.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 02:32:32.000398 toRST-0.0.7/json2rst/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.7/json2rst/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)      385 2023-07-18 16:07:34.000000 toRST-0.0.7/json2rst/json2rst.py
--rw-r--r--   0 jreyno     (501) staff       (20)      103 2023-07-18 20:40:47.000000 toRST-0.0.7/pyproject.toml
--rw-r--r--   0 jreyno     (501) staff       (20)      678 2023-07-21 02:32:32.002292 toRST-0.0.7/setup.cfg
--rw-r--r--   0 jreyno     (501) staff       (20)     1535 2023-07-21 02:24:31.000000 toRST-0.0.7/setup.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 02:32:32.000557 toRST-0.0.7/tests/
--rw-r--r--   0 jreyno     (501) staff       (20)      790 2023-07-18 16:07:34.000000 toRST-0.0.7/tests/test_toRST_toRST.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 02:32:32.001008 toRST-0.0.7/toRST/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.7/toRST/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)     2954 2023-07-21 02:32:05.000000 toRST-0.0.7/toRST/toRST.py
--rw-r--r--   0 jreyno     (501) staff       (20)      332 2023-07-21 01:49:45.000000 toRST-0.0.7/toRST/write.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 02:32:32.001885 toRST-0.0.7/toRST.egg-info/
--rw-r--r--   0 jreyno     (501) staff       (20)     2617 2023-07-21 02:32:31.000000 toRST-0.0.7/toRST.egg-info/PKG-INFO
--rw-r--r--   0 jreyno     (501) staff       (20)      404 2023-07-21 02:32:31.000000 toRST-0.0.7/toRST.egg-info/SOURCES.txt
--rw-r--r--   0 jreyno     (501) staff       (20)        1 2023-07-21 02:32:31.000000 toRST-0.0.7/toRST.egg-info/dependency_links.txt
--rw-r--r--   0 jreyno     (501) staff       (20)       44 2023-07-21 02:32:31.000000 toRST-0.0.7/toRST.egg-info/entry_points.txt
--rw-r--r--   0 jreyno     (501) staff       (20)       29 2023-07-21 02:32:31.000000 toRST-0.0.7/toRST.egg-info/top_level.txt
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 03:16:50.984797 toRST-0.0.8/
+-rw-r--r--   0 jreyno     (501) staff       (20)     1085 2023-07-18 19:42:12.000000 toRST-0.0.8/LICENSE
+-rw-r--r--   0 jreyno     (501) staff       (20)     2617 2023-07-21 03:16:50.984857 toRST-0.0.8/PKG-INFO
+-rw-r--r--   0 jreyno     (501) staff       (20)     1222 2023-07-21 02:00:59.000000 toRST-0.0.8/README.md
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 03:16:50.981690 toRST-0.0.8/csv2rst/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.8/csv2rst/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      836 2023-07-21 03:11:50.000000 toRST-0.0.8/csv2rst/csv2rst.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 03:16:50.982472 toRST-0.0.8/funcs/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.8/funcs/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)     1179 2023-07-18 16:07:34.000000 toRST-0.0.8/funcs/command.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      434 2023-07-21 03:14:42.000000 toRST-0.0.8/funcs/funcs.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 03:16:50.982872 toRST-0.0.8/json2rst/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.8/json2rst/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      385 2023-07-18 16:07:34.000000 toRST-0.0.8/json2rst/json2rst.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      103 2023-07-18 20:40:47.000000 toRST-0.0.8/pyproject.toml
+-rw-r--r--   0 jreyno     (501) staff       (20)      678 2023-07-21 03:16:50.985086 toRST-0.0.8/setup.cfg
+-rw-r--r--   0 jreyno     (501) staff       (20)     1535 2023-07-21 03:16:09.000000 toRST-0.0.8/setup.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 03:16:50.983142 toRST-0.0.8/tests/
+-rw-r--r--   0 jreyno     (501) staff       (20)      790 2023-07-18 16:07:34.000000 toRST-0.0.8/tests/test_toRST_toRST.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 03:16:50.983840 toRST-0.0.8/toRST/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.8/toRST/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)     2606 2023-07-21 03:15:29.000000 toRST-0.0.8/toRST/toRST.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      332 2023-07-21 01:49:45.000000 toRST-0.0.8/toRST/write.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 03:16:50.984678 toRST-0.0.8/toRST.egg-info/
+-rw-r--r--   0 jreyno     (501) staff       (20)     2617 2023-07-21 03:16:50.000000 toRST-0.0.8/toRST.egg-info/PKG-INFO
+-rw-r--r--   0 jreyno     (501) staff       (20)      404 2023-07-21 03:16:50.000000 toRST-0.0.8/toRST.egg-info/SOURCES.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)        1 2023-07-21 03:16:50.000000 toRST-0.0.8/toRST.egg-info/dependency_links.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)       44 2023-07-21 03:16:50.000000 toRST-0.0.8/toRST.egg-info/entry_points.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)       29 2023-07-21 03:16:50.000000 toRST-0.0.8/toRST.egg-info/top_level.txt
```

### Comparing `toRST-0.0.7/LICENSE` & `toRST-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `toRST-0.0.7/PKG-INFO` & `toRST-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toRST
-Version: 0.0.7
+Version: 0.0.8
 Summary: Command line tool for converting CSV and JSON files into reStructuredText Tables.
 Home-page: https://github.com/jrey999/toRST
 Author: John Reynolds
 Author-email: reynoldsjohngreg@gmail.com
 License: The MIT License (MIT)
         Copyright © 2023 John Reynolds
```

### Comparing `toRST-0.0.7/README.md` & `toRST-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `toRST-0.0.7/funcs/command.py` & `toRST-0.0.8/funcs/command.py`

 * *Files identical despite different names*

### Comparing `toRST-0.0.7/setup.cfg` & `toRST-0.0.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = torst
-version = 0.0.7
+version = 0.0.8
 author = John Reynolds
 author_email = reynoldsjohngreg@gmail.com
 description = Convert various data formats to reStructuredText tables.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jrey999/toRST
 project_urls =
```

### Comparing `toRST-0.0.7/setup.py` & `toRST-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 ```
 """.strip()
 
 with open('LICENSE') as f:
     license = f.read()
 setup(
     name='toRST',
-    version='0.0.7',
+    version='0.0.8',
     description='Command line tool for converting CSV and JSON files into reStructuredText Tables.',
     long_description=readme,
     author='John Reynolds',
     author_email='reynoldsjohngreg@gmail.com',
     url='https://github.com/jrey999/toRST',
     license=license,
     packages=find_packages(exclude=('tests',)),
```

### Comparing `toRST-0.0.7/tests/test_toRST_toRST.py` & `toRST-0.0.8/tests/test_toRST_toRST.py`

 * *Files identical despite different names*

### Comparing `toRST-0.0.7/toRST/toRST.py` & `toRST-0.0.8/toRST/toRST.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,19 @@
-from funcs.funcs import get_extension
-from csv2rst.csv2rst import from_csv
-from json2rst.json2rst import from_json
+from funcs.funcs import get_extension, handle_file
 
 
-def handle_file(file: str) -> list[list]:
-
-    extension = get_extension(file)
-    if extension == "csv":
-        return from_csv(file)
-    elif extension == "json":
-        return from_json(file)
-    else:
-        raise ValueError(f"{extension} files not currently supported")
 class Table:
 
     def __init__(self, file) -> None:
         
         self.data = handle_file(file)
         self.headers = self.data[0]
         self.column_widths = self.get_column_widths()
         self.page_info = self.get_page_info()
 
-    
-
     def get_column_widths(self) -> dict[int, int]:
         """
         Get the maximum width for each column.
         
         This determines the column widths needed to properly 
         format the reStructuredText grid by finding the max
         string length in each column of data.
```

### Comparing `toRST-0.0.7/toRST.egg-info/PKG-INFO` & `toRST-0.0.8/toRST.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toRST
-Version: 0.0.7
+Version: 0.0.8
 Summary: Command line tool for converting CSV and JSON files into reStructuredText Tables.
 Home-page: https://github.com/jrey999/toRST
 Author: John Reynolds
 Author-email: reynoldsjohngreg@gmail.com
 License: The MIT License (MIT)
         Copyright © 2023 John Reynolds
```

