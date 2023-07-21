# Comparing `tmp/toRST-0.0.5.tar.gz` & `tmp/toRST-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toRST-0.0.5.tar", last modified: Fri Jul 21 01:58:21 2023, max compression
+gzip compressed data, was "toRST-0.0.6.tar", last modified: Fri Jul 21 02:14:04 2023, max compression
```

## Comparing `toRST-0.0.5.tar` & `toRST-0.0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 01:58:21.649288 toRST-0.0.5/
--rw-r--r--   0 jreyno     (501) staff       (20)     1085 2023-07-18 19:42:12.000000 toRST-0.0.5/LICENSE
--rw-r--r--   0 jreyno     (501) staff       (20)     2617 2023-07-21 01:58:21.649350 toRST-0.0.5/PKG-INFO
--rw-r--r--   0 jreyno     (501) staff       (20)     1223 2023-07-21 01:54:42.000000 toRST-0.0.5/README.md
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 01:58:21.646714 toRST-0.0.5/csv2rst/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.5/csv2rst/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)      488 2023-07-18 16:07:34.000000 toRST-0.0.5/csv2rst/csv2rst.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 01:58:21.647468 toRST-0.0.5/funcs/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.5/funcs/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)     1179 2023-07-18 16:07:34.000000 toRST-0.0.5/funcs/command.py
--rw-r--r--   0 jreyno     (501) staff       (20)       76 2023-07-18 16:07:34.000000 toRST-0.0.5/funcs/funcs.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 01:58:21.647829 toRST-0.0.5/json2rst/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.5/json2rst/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)      385 2023-07-18 16:07:34.000000 toRST-0.0.5/json2rst/json2rst.py
--rw-r--r--   0 jreyno     (501) staff       (20)      103 2023-07-18 20:40:47.000000 toRST-0.0.5/pyproject.toml
--rw-r--r--   0 jreyno     (501) staff       (20)      678 2023-07-21 01:58:21.649577 toRST-0.0.5/setup.cfg
--rw-r--r--   0 jreyno     (501) staff       (20)     1535 2023-07-21 01:56:49.000000 toRST-0.0.5/setup.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 01:58:21.648005 toRST-0.0.5/tests/
--rw-r--r--   0 jreyno     (501) staff       (20)      790 2023-07-18 16:07:34.000000 toRST-0.0.5/tests/test_toRST_toRST.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 01:58:21.648440 toRST-0.0.5/toRST/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.5/toRST/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)     2976 2023-07-21 01:48:55.000000 toRST-0.0.5/toRST/toRST.py
--rw-r--r--   0 jreyno     (501) staff       (20)      332 2023-07-21 01:49:45.000000 toRST-0.0.5/toRST/write.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 01:58:21.649175 toRST-0.0.5/toRST.egg-info/
--rw-r--r--   0 jreyno     (501) staff       (20)     2617 2023-07-21 01:58:21.000000 toRST-0.0.5/toRST.egg-info/PKG-INFO
--rw-r--r--   0 jreyno     (501) staff       (20)      404 2023-07-21 01:58:21.000000 toRST-0.0.5/toRST.egg-info/SOURCES.txt
--rw-r--r--   0 jreyno     (501) staff       (20)        1 2023-07-21 01:58:21.000000 toRST-0.0.5/toRST.egg-info/dependency_links.txt
--rw-r--r--   0 jreyno     (501) staff       (20)       44 2023-07-21 01:58:21.000000 toRST-0.0.5/toRST.egg-info/entry_points.txt
--rw-r--r--   0 jreyno     (501) staff       (20)       29 2023-07-21 01:58:21.000000 toRST-0.0.5/toRST.egg-info/top_level.txt
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 02:14:04.029287 toRST-0.0.6/
+-rw-r--r--   0 jreyno     (501) staff       (20)     1085 2023-07-18 19:42:12.000000 toRST-0.0.6/LICENSE
+-rw-r--r--   0 jreyno     (501) staff       (20)     2617 2023-07-21 02:14:04.029411 toRST-0.0.6/PKG-INFO
+-rw-r--r--   0 jreyno     (501) staff       (20)     1222 2023-07-21 02:00:59.000000 toRST-0.0.6/README.md
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 02:14:04.017607 toRST-0.0.6/csv2rst/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.6/csv2rst/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      488 2023-07-18 16:07:34.000000 toRST-0.0.6/csv2rst/csv2rst.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 02:14:04.018625 toRST-0.0.6/funcs/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.6/funcs/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)     1179 2023-07-18 16:07:34.000000 toRST-0.0.6/funcs/command.py
+-rw-r--r--   0 jreyno     (501) staff       (20)       76 2023-07-18 16:07:34.000000 toRST-0.0.6/funcs/funcs.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 02:14:04.019005 toRST-0.0.6/json2rst/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.6/json2rst/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      385 2023-07-18 16:07:34.000000 toRST-0.0.6/json2rst/json2rst.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      103 2023-07-18 20:40:47.000000 toRST-0.0.6/pyproject.toml
+-rw-r--r--   0 jreyno     (501) staff       (20)      678 2023-07-21 02:14:04.029743 toRST-0.0.6/setup.cfg
+-rw-r--r--   0 jreyno     (501) staff       (20)     1535 2023-07-21 02:00:14.000000 toRST-0.0.6/setup.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 02:14:04.019270 toRST-0.0.6/tests/
+-rw-r--r--   0 jreyno     (501) staff       (20)      790 2023-07-18 16:07:34.000000 toRST-0.0.6/tests/test_toRST_toRST.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 02:14:04.024310 toRST-0.0.6/toRST/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.6/toRST/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)     2984 2023-07-21 02:09:04.000000 toRST-0.0.6/toRST/toRST.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      332 2023-07-21 01:49:45.000000 toRST-0.0.6/toRST/write.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 02:14:04.027052 toRST-0.0.6/toRST.egg-info/
+-rw-r--r--   0 jreyno     (501) staff       (20)     2617 2023-07-21 02:14:04.000000 toRST-0.0.6/toRST.egg-info/PKG-INFO
+-rw-r--r--   0 jreyno     (501) staff       (20)      404 2023-07-21 02:14:04.000000 toRST-0.0.6/toRST.egg-info/SOURCES.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)        1 2023-07-21 02:14:04.000000 toRST-0.0.6/toRST.egg-info/dependency_links.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)       44 2023-07-21 02:14:04.000000 toRST-0.0.6/toRST.egg-info/entry_points.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)       29 2023-07-21 02:14:04.000000 toRST-0.0.6/toRST.egg-info/top_level.txt
```

### Comparing `toRST-0.0.5/LICENSE` & `toRST-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `toRST-0.0.5/PKG-INFO` & `toRST-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toRST
-Version: 0.0.5
+Version: 0.0.6
 Summary: Command line tool for converting CSV and JSON files into reStructuredText Tables.
 Home-page: https://github.com/jrey999/toRST
 Author: John Reynolds
 Author-email: reynoldsjohngreg@gmail.com
 License: The MIT License (MIT)
         Copyright © 2023 John Reynolds
         
@@ -47,33 +47,33 @@
 -------------
 example<br>
   Convert file1.csv and file2.json into RST
 ```bash
 torst file1.csv file2.json -o ./outputfolder
 ```
 
-**Python Usage**
--------------
-example<br>
-  
-Import Table class
-```python
-from toRST.toRST import Table
-```
-Convert file1.csv into RST string
-```python
-rst_table = Table('file1').build_table()
-```
-
 **Positional Arguments**:
 ------------------------
 
 inputs
   One or more input files to convert to RST. Currently only CSV and JSON files are 
   supported, but additional formats will be added.
 
 **Optional Arguments**:
 ---------------------- 
 
 -o, --output_dir
   Output directory for generated RST files. Defaults to the current 
   working directory if not provided.
+
+**Python Usage**
+-------------
+example<br>
+  
+Import Table class
+```python
+from toRST.toRST import Table
+```
+Convert file1.csv into RST string
+```python
+rst_table = Table('file1').build_table()
+```
```

### Comparing `toRST-0.0.5/README.md` & `toRST-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,39 +25,38 @@
 **CLI Usage**
 -------------
 example<br>
   Convert file1.csv and file2.json into RST
 ```bash
 torst file1.csv file2.json -o ./outputfolder
 ```
-
-**Python Usage**
--------------
-example<br>
-  
-Import Table class
-```python
-from toRST.toRST import Table
-```
-Convert file1.csv into RST string
-```python
-rst_table = Table('file1').build_table()
-```
-
 **Positional Arguments**:
 ------------------------
 
 inputs
   One or more input files to convert to RST. Currently only CSV and JSON files are 
   supported, but additional formats will be added.
 
 **Optional Arguments**:
 ---------------------- 
 
 -o, --output_dir
   Output directory for generated RST files. Defaults to the current 
   working directory if not provided.
 
+**Python Usage**
+-------------
+example<br>
+  
+Import Table class
+```python
+from toRST.toRST import Table
+```
+Convert file1.csv into RST string
+```python
+rst_table = Table('file1').build_table()
+```
+
 **What toRST was built for**
 ----------------------------
 
 While building [mlb-positive-ev](https://github.com/jrey999/mlb-positive-ev), I wanted a quick and readable output of a SQLite query and couldn't find anything suitable.
```

### Comparing `toRST-0.0.5/funcs/command.py` & `toRST-0.0.6/funcs/command.py`

 * *Files identical despite different names*

### Comparing `toRST-0.0.5/setup.cfg` & `toRST-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = torst
-version = 0.0.5
+version = 0.0.6
 author = John Reynolds
 author_email = reynoldsjohngreg@gmail.com
 description = Convert various data formats to reStructuredText tables.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jrey999/toRST
 project_urls =
```

### Comparing `toRST-0.0.5/setup.py` & `toRST-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,47 +29,47 @@
 -------------
 example<br>
   Convert file1.csv and file2.json into RST
 ```bash
 torst file1.csv file2.json -o ./outputfolder
 ```
 
-**Python Usage**
--------------
-example<br>
-  
-Import Table class
-```python
-from toRST.toRST import Table
-```
-Convert file1.csv into RST string
-```python
-rst_table = Table('file1').build_table()
-```
-
 **Positional Arguments**:
 ------------------------
 
 inputs
   One or more input files to convert to RST. Currently only CSV and JSON files are 
   supported, but additional formats will be added.
 
 **Optional Arguments**:
 ---------------------- 
 
 -o, --output_dir
   Output directory for generated RST files. Defaults to the current 
   working directory if not provided.
+
+**Python Usage**
+-------------
+example<br>
+  
+Import Table class
+```python
+from toRST.toRST import Table
+```
+Convert file1.csv into RST string
+```python
+rst_table = Table('file1').build_table()
+```
 """.strip()
 
 with open('LICENSE') as f:
     license = f.read()
 setup(
     name='toRST',
-    version='0.0.5',
+    version='0.0.6',
     description='Command line tool for converting CSV and JSON files into reStructuredText Tables.',
     long_description=readme,
     author='John Reynolds',
     author_email='reynoldsjohngreg@gmail.com',
     url='https://github.com/jrey999/toRST',
     license=license,
     packages=find_packages(exclude=('tests',)),
```

### Comparing `toRST-0.0.5/tests/test_toRST_toRST.py` & `toRST-0.0.6/tests/test_toRST_toRST.py`

 * *Files identical despite different names*

### Comparing `toRST-0.0.5/toRST/toRST.py` & `toRST-0.0.6/toRST/toRST.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,16 +52,16 @@
 
         :returns: Dict with page formatting metadata
         :rtype: dict[str, int or str]
         """
         return {
             "num_columns": len(self.headers),
             "page_wdith": sum(self.column_widths.values()),
-            "header": "".join(["+" + column_width * "=" for column_width in self.column_widths.values()]) + "+",
-            "new_line": "".join(["+" + column_width * "-" for column_width in self.column_widths.values()]) + "+"
+            "header": "+{}+".format("+".join([column_width * "=" for column_width in self.column_widths.values()])),
+            "new_line": "+{}+".format("+".join([column_width * "-" for column_width in self.column_widths.values()]))
         }
     
     def build_table(self) -> list[str]:
         
         """
         Construct the reST grid table.
```

### Comparing `toRST-0.0.5/toRST.egg-info/PKG-INFO` & `toRST-0.0.6/toRST.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toRST
-Version: 0.0.5
+Version: 0.0.6
 Summary: Command line tool for converting CSV and JSON files into reStructuredText Tables.
 Home-page: https://github.com/jrey999/toRST
 Author: John Reynolds
 Author-email: reynoldsjohngreg@gmail.com
 License: The MIT License (MIT)
         Copyright © 2023 John Reynolds
         
@@ -47,33 +47,33 @@
 -------------
 example<br>
   Convert file1.csv and file2.json into RST
 ```bash
 torst file1.csv file2.json -o ./outputfolder
 ```
 
-**Python Usage**
--------------
-example<br>
-  
-Import Table class
-```python
-from toRST.toRST import Table
-```
-Convert file1.csv into RST string
-```python
-rst_table = Table('file1').build_table()
-```
-
 **Positional Arguments**:
 ------------------------
 
 inputs
   One or more input files to convert to RST. Currently only CSV and JSON files are 
   supported, but additional formats will be added.
 
 **Optional Arguments**:
 ---------------------- 
 
 -o, --output_dir
   Output directory for generated RST files. Defaults to the current 
   working directory if not provided.
+
+**Python Usage**
+-------------
+example<br>
+  
+Import Table class
+```python
+from toRST.toRST import Table
+```
+Convert file1.csv into RST string
+```python
+rst_table = Table('file1').build_table()
+```
```

