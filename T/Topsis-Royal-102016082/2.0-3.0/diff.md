# Comparing `tmp/Topsis-Royal-102016082-2.0.tar.gz` & `tmp/Topsis-Royal-102016082-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Topsis-Royal-102016082-2.0.tar", last modified: Fri Feb 10 21:18:46 2023, max compression
+gzip compressed data, was "Topsis-Royal-102016082-3.0.tar", last modified: Fri Jul 21 16:58:17 2023, max compression
```

## Comparing `Topsis-Royal-102016082-2.0.tar` & `Topsis-Royal-102016082-3.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxr-x   0 royal     (1000) royal     (1000)        0 2023-02-10 21:18:46.350876 Topsis-Royal-102016082-2.0/
--rw-rw-r--   0 royal     (1000) royal     (1000)      360 2023-02-10 21:18:46.350876 Topsis-Royal-102016082-2.0/PKG-INFO
-drwxrwxr-x   0 royal     (1000) royal     (1000)        0 2023-02-10 21:18:46.350876 Topsis-Royal-102016082-2.0/Topsis_Royal_102016082.egg-info/
--rw-rw-r--   0 royal     (1000) royal     (1000)      360 2023-02-10 21:18:46.000000 Topsis-Royal-102016082-2.0/Topsis_Royal_102016082.egg-info/PKG-INFO
--rw-rw-r--   0 royal     (1000) royal     (1000)      301 2023-02-10 21:18:46.000000 Topsis-Royal-102016082-2.0/Topsis_Royal_102016082.egg-info/SOURCES.txt
--rw-rw-r--   0 royal     (1000) royal     (1000)        1 2023-02-10 21:18:46.000000 Topsis-Royal-102016082-2.0/Topsis_Royal_102016082.egg-info/dependency_links.txt
--rw-rw-r--   0 royal     (1000) royal     (1000)       59 2023-02-10 21:18:46.000000 Topsis-Royal-102016082-2.0/Topsis_Royal_102016082.egg-info/entry_points.txt
--rw-rw-r--   0 royal     (1000) royal     (1000)       18 2023-02-10 21:18:46.000000 Topsis-Royal-102016082-2.0/Topsis_Royal_102016082.egg-info/top_level.txt
--rw-rw-r--   0 royal     (1000) royal     (1000)       38 2023-02-10 21:18:46.350876 Topsis-Royal-102016082-2.0/setup.cfg
--rw-rw-r--   0 royal     (1000) royal     (1000)      992 2023-02-10 21:18:24.000000 Topsis-Royal-102016082-2.0/setup.py
-drwxrwxr-x   0 royal     (1000) royal     (1000)        0 2023-02-10 21:18:46.350876 Topsis-Royal-102016082-2.0/topsis_assignment/
--rw-rw-r--   0 royal     (1000) royal     (1000)       17 2023-02-10 21:18:28.000000 Topsis-Royal-102016082-2.0/topsis_assignment/__init__.py
--rw-rw-r--   0 royal     (1000) royal     (1000)     2924 2023-02-10 21:15:22.000000 Topsis-Royal-102016082-2.0/topsis_assignment/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:58:17.536733 Topsis-Royal-102016082-3.0/
+-rw-rw-rw-   0        0        0     1067 2023-07-21 16:38:52.000000 Topsis-Royal-102016082-3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2048 2023-07-21 16:58:17.536733 Topsis-Royal-102016082-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1504 2023-07-21 16:52:50.000000 Topsis-Royal-102016082-3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 16:58:17.536733 Topsis-Royal-102016082-3.0/Topsis_Royal_102016082.egg-info/
+-rw-rw-rw-   0        0        0     2048 2023-07-21 16:58:17.000000 Topsis-Royal-102016082-3.0/Topsis_Royal_102016082.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-07-21 16:58:17.000000 Topsis-Royal-102016082-3.0/Topsis_Royal_102016082.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 16:58:17.000000 Topsis-Royal-102016082-3.0/Topsis_Royal_102016082.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-21 16:58:17.000000 Topsis-Royal-102016082-3.0/Topsis_Royal_102016082.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2023-07-21 16:58:17.000000 Topsis-Royal-102016082-3.0/Topsis_Royal_102016082.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-21 16:58:17.000000 Topsis-Royal-102016082-3.0/Topsis_Royal_102016082.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-21 16:58:17.544758 Topsis-Royal-102016082-3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1126 2023-07-21 16:58:12.000000 Topsis-Royal-102016082-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:58:17.536733 Topsis-Royal-102016082-3.0/topsis_assignment/
+-rw-rw-rw-   0        0        0       17 2023-07-21 16:28:00.000000 Topsis-Royal-102016082-3.0/topsis_assignment/__init__.py
+-rw-rw-rw-   0        0        0     2789 2023-07-21 16:33:51.000000 Topsis-Royal-102016082-3.0/topsis_assignment/__main__.py
```

### Comparing `Topsis-Royal-102016082-2.0/setup.py` & `Topsis-Royal-102016082-3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import pathlib
 from setuptools import setup
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
-#README = (HERE / "README.md").read_text()
+README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="Topsis-Royal-102016082",
-    version="2.0",
+    version="3.0",
     description="Topsis Assignment",
-    #long_description=README,
-    #long_description_content_type="text/markdown",
-    #url="https://github.com/uditvashisht/saral-square",
+    long_description=README,
+    long_description_content_type="text/markdown",
+    url="https://github.com/RGarg2002/Topsis-Royal-102016082",
     author="Royal Garg",
     author_email="royalgarg36@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
     ],
     packages=["topsis_assignment"],
     include_package_data=True,
-    install_requires=[],
+    install_requires=['pandas',
+                      'math',
+                      'numpy',
+                      'sys',
+                      'logging'],
     entry_points={
         "console_scripts": [
             "topsis=topsis_assignment.__main__:main",
         ]
     },
 )
```

### Comparing `Topsis-Royal-102016082-2.0/topsis_assignment/__main__.py` & `Topsis-Royal-102016082-3.0/topsis_assignment/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 import pandas as pd
 import math
 import numpy as np
-from pathlib import Path
-import os
 import sys
 import logging
 
-#data_folder = Path(os.getcwd())
-#file_to_open = data_folder / sys.argv[1]
-#f = open(file_to_open)
-
 def main():  
   if (len(sys.argv) != 5):
     logging.warning("Usages: python <program.py> <InputDataFile> <Weights> <Impacts> <ResultFileName>")
     exit()
   try:
       data = pd.DataFrame(pd.read_csv(str(sys.argv[1])))
   except FileNotFoundError:
```

