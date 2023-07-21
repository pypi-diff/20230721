# Comparing `tmp/toRST-0.0.4.tar.gz` & `tmp/toRST-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toRST-0.0.4.tar", last modified: Fri Jul 21 00:52:18 2023, max compression
+gzip compressed data, was "toRST-0.0.5.tar", last modified: Fri Jul 21 01:58:21 2023, max compression
```

## Comparing `toRST-0.0.4.tar` & `toRST-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 00:52:18.438896 toRST-0.0.4/
--rw-r--r--   0 jreyno     (501) staff       (20)     1085 2023-07-18 19:42:12.000000 toRST-0.0.4/LICENSE
--rw-r--r--   0 jreyno     (501) staff       (20)     2468 2023-07-21 00:52:18.438955 toRST-0.0.4/PKG-INFO
--rw-r--r--   0 jreyno     (501) staff       (20)     1024 2023-07-19 15:18:01.000000 toRST-0.0.4/README.md
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 00:52:18.436188 toRST-0.0.4/csv2rst/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.4/csv2rst/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)      488 2023-07-18 16:07:34.000000 toRST-0.0.4/csv2rst/csv2rst.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 00:52:18.437023 toRST-0.0.4/funcs/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.4/funcs/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)     1179 2023-07-18 16:07:34.000000 toRST-0.0.4/funcs/command.py
--rw-r--r--   0 jreyno     (501) staff       (20)       76 2023-07-18 16:07:34.000000 toRST-0.0.4/funcs/funcs.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 00:52:18.437345 toRST-0.0.4/json2rst/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.4/json2rst/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)      385 2023-07-18 16:07:34.000000 toRST-0.0.4/json2rst/json2rst.py
--rw-r--r--   0 jreyno     (501) staff       (20)      103 2023-07-18 20:40:47.000000 toRST-0.0.4/pyproject.toml
--rw-r--r--   0 jreyno     (501) staff       (20)      678 2023-07-21 00:52:18.439214 toRST-0.0.4/setup.cfg
--rw-r--r--   0 jreyno     (501) staff       (20)     1386 2023-07-21 00:51:16.000000 toRST-0.0.4/setup.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 00:52:18.437496 toRST-0.0.4/tests/
--rw-r--r--   0 jreyno     (501) staff       (20)      790 2023-07-18 16:07:34.000000 toRST-0.0.4/tests/test_toRST_toRST.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 00:52:18.437985 toRST-0.0.4/toRST/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.4/toRST/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)     2965 2023-07-19 13:36:13.000000 toRST-0.0.4/toRST/toRST.py
--rw-r--r--   0 jreyno     (501) staff       (20)      374 2023-07-19 13:36:13.000000 toRST-0.0.4/toRST/write.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 00:52:18.438785 toRST-0.0.4/toRST.egg-info/
--rw-r--r--   0 jreyno     (501) staff       (20)     2468 2023-07-21 00:52:18.000000 toRST-0.0.4/toRST.egg-info/PKG-INFO
--rw-r--r--   0 jreyno     (501) staff       (20)      404 2023-07-21 00:52:18.000000 toRST-0.0.4/toRST.egg-info/SOURCES.txt
--rw-r--r--   0 jreyno     (501) staff       (20)        1 2023-07-21 00:52:18.000000 toRST-0.0.4/toRST.egg-info/dependency_links.txt
--rw-r--r--   0 jreyno     (501) staff       (20)       44 2023-07-21 00:52:18.000000 toRST-0.0.4/toRST.egg-info/entry_points.txt
--rw-r--r--   0 jreyno     (501) staff       (20)       29 2023-07-21 00:52:18.000000 toRST-0.0.4/toRST.egg-info/top_level.txt
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 01:58:21.649288 toRST-0.0.5/
+-rw-r--r--   0 jreyno     (501) staff       (20)     1085 2023-07-18 19:42:12.000000 toRST-0.0.5/LICENSE
+-rw-r--r--   0 jreyno     (501) staff       (20)     2617 2023-07-21 01:58:21.649350 toRST-0.0.5/PKG-INFO
+-rw-r--r--   0 jreyno     (501) staff       (20)     1223 2023-07-21 01:54:42.000000 toRST-0.0.5/README.md
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 01:58:21.646714 toRST-0.0.5/csv2rst/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.5/csv2rst/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      488 2023-07-18 16:07:34.000000 toRST-0.0.5/csv2rst/csv2rst.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 01:58:21.647468 toRST-0.0.5/funcs/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.5/funcs/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)     1179 2023-07-18 16:07:34.000000 toRST-0.0.5/funcs/command.py
+-rw-r--r--   0 jreyno     (501) staff       (20)       76 2023-07-18 16:07:34.000000 toRST-0.0.5/funcs/funcs.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 01:58:21.647829 toRST-0.0.5/json2rst/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.5/json2rst/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      385 2023-07-18 16:07:34.000000 toRST-0.0.5/json2rst/json2rst.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      103 2023-07-18 20:40:47.000000 toRST-0.0.5/pyproject.toml
+-rw-r--r--   0 jreyno     (501) staff       (20)      678 2023-07-21 01:58:21.649577 toRST-0.0.5/setup.cfg
+-rw-r--r--   0 jreyno     (501) staff       (20)     1535 2023-07-21 01:56:49.000000 toRST-0.0.5/setup.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 01:58:21.648005 toRST-0.0.5/tests/
+-rw-r--r--   0 jreyno     (501) staff       (20)      790 2023-07-18 16:07:34.000000 toRST-0.0.5/tests/test_toRST_toRST.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 01:58:21.648440 toRST-0.0.5/toRST/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.5/toRST/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)     2976 2023-07-21 01:48:55.000000 toRST-0.0.5/toRST/toRST.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      332 2023-07-21 01:49:45.000000 toRST-0.0.5/toRST/write.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 01:58:21.649175 toRST-0.0.5/toRST.egg-info/
+-rw-r--r--   0 jreyno     (501) staff       (20)     2617 2023-07-21 01:58:21.000000 toRST-0.0.5/toRST.egg-info/PKG-INFO
+-rw-r--r--   0 jreyno     (501) staff       (20)      404 2023-07-21 01:58:21.000000 toRST-0.0.5/toRST.egg-info/SOURCES.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)        1 2023-07-21 01:58:21.000000 toRST-0.0.5/toRST.egg-info/dependency_links.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)       44 2023-07-21 01:58:21.000000 toRST-0.0.5/toRST.egg-info/entry_points.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)       29 2023-07-21 01:58:21.000000 toRST-0.0.5/toRST.egg-info/top_level.txt
```

### Comparing `toRST-0.0.4/LICENSE` & `toRST-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `toRST-0.0.4/PKG-INFO` & `toRST-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toRST
-Version: 0.0.4
+Version: 0.0.5
 Summary: Command line tool for converting CSV and JSON files into reStructuredText Tables.
 Home-page: https://github.com/jrey999/toRST
 Author: John Reynolds
 Author-email: reynoldsjohngreg@gmail.com
 License: The MIT License (MIT)
         Copyright © 2023 John Reynolds
         
@@ -34,28 +34,40 @@
 
 **Planned formats**:
 
 
 - Excel<br><br>
 
 **installation**
-[PyPI](https://pypi.org/project/toRST/0.0.1/)<br>
 ```bash
 pip install toRST
 ```
 <br>
 
-**Usage Cli**
+**CLI Usage**
 -------------
 example<br>
   Convert file1.csv and file2.json into RST
 ```bash
 torst file1.csv file2.json -o ./outputfolder
 ```
 
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
 **Positional Arguments**:
 ------------------------
 
 inputs
   One or more input files to convert to RST. Currently only CSV and JSON files are 
   supported, but additional formats will be added.
```

### Comparing `toRST-0.0.4/funcs/command.py` & `toRST-0.0.5/funcs/command.py`

 * *Files identical despite different names*

### Comparing `toRST-0.0.4/setup.cfg` & `toRST-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = torst
-version = 0.0.3
+version = 0.0.5
 author = John Reynolds
 author_email = reynoldsjohngreg@gmail.com
 description = Convert various data formats to reStructuredText tables.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jrey999/toRST
 project_urls =
```

### Comparing `toRST-0.0.4/setup.py` & `toRST-0.0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,28 +16,40 @@
 
 **Planned formats**:
 
 
 - Excel<br><br>
 
 **installation**
-[PyPI](https://pypi.org/project/toRST/0.0.1/)<br>
 ```bash
 pip install toRST
 ```
 <br>
 
-**Usage Cli**
+**CLI Usage**
 -------------
 example<br>
   Convert file1.csv and file2.json into RST
 ```bash
 torst file1.csv file2.json -o ./outputfolder
 ```
 
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
 **Positional Arguments**:
 ------------------------
 
 inputs
   One or more input files to convert to RST. Currently only CSV and JSON files are 
   supported, but additional formats will be added.
 
@@ -49,15 +61,15 @@
   working directory if not provided.
 """.strip()
 
 with open('LICENSE') as f:
     license = f.read()
 setup(
     name='toRST',
-    version='0.0.4',
+    version='0.0.5',
     description='Command line tool for converting CSV and JSON files into reStructuredText Tables.',
     long_description=readme,
     author='John Reynolds',
     author_email='reynoldsjohngreg@gmail.com',
     url='https://github.com/jrey999/toRST',
     license=license,
     packages=find_packages(exclude=('tests',)),
```

### Comparing `toRST-0.0.4/tests/test_toRST_toRST.py` & `toRST-0.0.5/tests/test_toRST_toRST.py`

 * *Files identical despite different names*

### Comparing `toRST-0.0.4/toRST/toRST.py` & `toRST-0.0.5/toRST/toRST.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,8 +79,8 @@
         for row in self.data[1:]:
             
             rst_row=""
             for index, cell in enumerate(row):
                 column_width = self.column_widths[index]
                 rst_row += "|" + (str(cell) + " " * (column_width - len(str(cell))))
             table += [rst_row + "|"] + [self.page_info["new_line"]]
-        return table
+        return "\n".join(table)
```

### Comparing `toRST-0.0.4/toRST.egg-info/PKG-INFO` & `toRST-0.0.5/toRST.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toRST
-Version: 0.0.4
+Version: 0.0.5
 Summary: Command line tool for converting CSV and JSON files into reStructuredText Tables.
 Home-page: https://github.com/jrey999/toRST
 Author: John Reynolds
 Author-email: reynoldsjohngreg@gmail.com
 License: The MIT License (MIT)
         Copyright © 2023 John Reynolds
         
@@ -34,28 +34,40 @@
 
 **Planned formats**:
 
 
 - Excel<br><br>
 
 **installation**
-[PyPI](https://pypi.org/project/toRST/0.0.1/)<br>
 ```bash
 pip install toRST
 ```
 <br>
 
-**Usage Cli**
+**CLI Usage**
 -------------
 example<br>
   Convert file1.csv and file2.json into RST
 ```bash
 torst file1.csv file2.json -o ./outputfolder
 ```
 
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
 **Positional Arguments**:
 ------------------------
 
 inputs
   One or more input files to convert to RST. Currently only CSV and JSON files are 
   supported, but additional formats will be added.
```

