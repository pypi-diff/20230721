# Comparing `tmp/pythonquerylanguage-0.1.5.tar.gz` & `tmp/PythonQueryLanguage-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonquerylanguage-0.1.5.tar", max compression
+gzip compressed data, was "PythonQueryLanguage-0.1.6.tar", max compression
```

## Comparing `pythonquerylanguage-0.1.5.tar` & `PythonQueryLanguage-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0        0 2023-07-21 12:05:56.004611 pythonquerylanguage-0.1.5/PythonQueryLanguage/__init__.py
--rw-r--r--   0        0        0    23068 2023-07-21 12:05:56.008611 pythonquerylanguage-0.1.5/PythonQueryLanguage/pql.py
--rw-r--r--   0        0        0      508 2023-07-21 12:21:10.595368 pythonquerylanguage-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2866 2023-07-21 12:05:56.008611 pythonquerylanguage-0.1.5/readme.md
--rw-r--r--   0        0        0     3569 1970-01-01 00:00:00.000000 pythonquerylanguage-0.1.5/PKG-INFO
+-rwxr-xr-x   0        0        0      455 2022-08-22 12:31:00.049547 PythonQueryLanguage-0.1.6/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2022-08-22 12:22:59.796524 PythonQueryLanguage-0.1.6/pythonquerylanguage/__init__.py
+-rwxr-xr-x   0        0        0    23085 2022-08-22 12:25:16.313928 PythonQueryLanguage-0.1.6/pythonquerylanguage/pql.py
+-rwxr-xr-x   0        0        0     2866 2022-02-25 14:04:00.907483 PythonQueryLanguage-0.1.6/readme.md
+-rw-r--r--   0        0        0     3736 2022-08-22 12:31:04.311988 PythonQueryLanguage-0.1.6/setup.py
+-rw-r--r--   0        0        0     3528 2022-08-22 12:31:04.312703 PythonQueryLanguage-0.1.6/PKG-INFO
```

### Comparing `pythonquerylanguage-0.1.5/PythonQueryLanguage/pql.py` & `PythonQueryLanguage-0.1.6/pythonquerylanguage/pql.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 from sqlalchemy import create_engine
-from IPython.display import display
+#from IPython.display import display
 import pandas as pd
 import numpy as np
 import difflib
 
 # develop insert mode (only_print, print_and_ask_confirm, ask_confirm, nothing)
 # think show table to insert or statement? hum..
 
@@ -470,15 +470,16 @@
     def required_confirmation(table=None, table_name='', ask_usr=True, _display=True):
         """
         Ask for a text confirmation when required
         """
         if ask_usr:
             print("--Select/Insert/update: " + table_name)
             if _display:
-                display(table)
+                print(table)
+		#display(table)
             confirmation = input("Are you sure you want to perform this operation?")
             if confirmation in ["yes", 'y', 'YES', 'Yes']:
                 print("Operation accepted")
                 return True
             else:
                 print("Operation cancelled by user")
                 return False
```

### Comparing `pythonquerylanguage-0.1.5/readme.md` & `PythonQueryLanguage-0.1.6/readme.md`

 * *Files identical despite different names*

### Comparing `pythonquerylanguage-0.1.5/PKG-INFO` & `PythonQueryLanguage-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: pythonquerylanguage
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python SQL wrapper based on pandas and SQLalchemy
 License: MIT
 Author: Pablo Ruiz
 Author-email: pablo.r.c@live.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: SQLAlchemy (>=1.4.31,<2.0.0)
-Requires-Dist: ipython (>=8.0.1,<9.0.0)
+Requires-Dist: ipython (==8.0.1)
 Requires-Dist: numpy (>=1.22.2,<2.0.0)
-Requires-Dist: pandas
+Requires-Dist: pandas (>=1.4.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 
 # <b>Python Query Language PQL</b>
 
 <b>PQL</b> is a python wrapper of the sql sintax based in SQLalchemy and pandas, this code introduces a new syntax to use 
 in your code when calling a database table.
```

