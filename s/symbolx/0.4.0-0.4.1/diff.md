# Comparing `tmp/symbolx-0.4.0.tar.gz` & `tmp/symbolx-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbolx-0.4.0.tar", last modified: Fri Jul 21 21:35:25 2023, max compression
+gzip compressed data, was "symbolx-0.4.1.tar", last modified: Fri Jul 21 21:37:51 2023, max compression
```

## Comparing `symbolx-0.4.0.tar` & `symbolx-0.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 cgaete    (1000) cgaete    (1000)        0 2023-07-21 21:35:25.527325 symbolx-0.4.0/
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     1069 2023-05-23 09:10:57.000000 symbolx-0.4.0/LICENSE
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     3090 2023-07-21 21:35:25.527325 symbolx-0.4.0/PKG-INFO
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     2227 2023-07-21 21:27:01.000000 symbolx-0.4.0/README.md
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)       38 2023-07-21 21:35:25.527325 symbolx-0.4.0/setup.cfg
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     1610 2023-07-21 21:32:42.000000 symbolx-0.4.0/setup.py
-drwxrwxr-x   0 cgaete    (1000) cgaete    (1000)        0 2023-07-21 21:35:25.527325 symbolx-0.4.0/symbolx/
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)      586 2023-05-23 09:10:57.000000 symbolx-0.4.0/symbolx/__init__.py
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)    12238 2023-05-23 09:10:57.000000 symbolx-0.4.0/symbolx/handler.py
-drwxrwxr-x   0 cgaete    (1000) cgaete    (1000)        0 2023-07-21 21:35:25.527325 symbolx-0.4.0/symbolx/parsers/
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)        0 2023-05-23 09:10:57.000000 symbolx-0.4.0/symbolx/parsers/__init__.py
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     4615 2023-05-23 09:10:57.000000 symbolx-0.4.0/symbolx/parsers/parser_csv.py
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     3395 2023-05-23 09:10:57.000000 symbolx-0.4.0/symbolx/parsers/parser_feather.py
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)    12426 2023-07-21 21:25:07.000000 symbolx-0.4.0/symbolx/parsers/parser_gdx.py
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     1388 2023-05-23 09:10:57.000000 symbolx-0.4.0/symbolx/settings.py
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)    54620 2023-05-23 09:10:57.000000 symbolx-0.4.0/symbolx/symbols.py
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     6725 2023-05-23 09:10:57.000000 symbolx-0.4.0/symbolx/utils.py
-drwxrwxr-x   0 cgaete    (1000) cgaete    (1000)        0 2023-07-21 21:35:25.527325 symbolx-0.4.0/symbolx.egg-info/
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     3090 2023-07-21 21:35:25.000000 symbolx-0.4.0/symbolx.egg-info/PKG-INFO
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)      410 2023-07-21 21:35:25.000000 symbolx-0.4.0/symbolx.egg-info/SOURCES.txt
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)        1 2023-07-21 21:35:25.000000 symbolx-0.4.0/symbolx.egg-info/dependency_links.txt
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)       35 2023-07-21 21:35:25.000000 symbolx-0.4.0/symbolx.egg-info/requires.txt
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)        8 2023-07-21 21:35:25.000000 symbolx-0.4.0/symbolx.egg-info/top_level.txt
-drwxrwxr-x   0 cgaete    (1000) cgaete    (1000)        0 2023-07-21 21:35:25.527325 symbolx-0.4.0/test/
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     3559 2023-06-16 18:52:39.000000 symbolx-0.4.0/test/test.py
+drwxrwxr-x   0 cgaete    (1000) cgaete    (1000)        0 2023-07-21 21:37:51.232957 symbolx-0.4.1/
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     1069 2023-05-23 09:10:57.000000 symbolx-0.4.1/LICENSE
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     3090 2023-07-21 21:37:51.232957 symbolx-0.4.1/PKG-INFO
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     2227 2023-07-21 21:27:01.000000 symbolx-0.4.1/README.md
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)       38 2023-07-21 21:37:51.232957 symbolx-0.4.1/setup.cfg
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     1610 2023-07-21 21:36:48.000000 symbolx-0.4.1/setup.py
+drwxrwxr-x   0 cgaete    (1000) cgaete    (1000)        0 2023-07-21 21:37:51.232957 symbolx-0.4.1/symbolx/
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)      586 2023-07-21 21:37:08.000000 symbolx-0.4.1/symbolx/__init__.py
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)    12238 2023-05-23 09:10:57.000000 symbolx-0.4.1/symbolx/handler.py
+drwxrwxr-x   0 cgaete    (1000) cgaete    (1000)        0 2023-07-21 21:37:51.232957 symbolx-0.4.1/symbolx/parsers/
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)        0 2023-05-23 09:10:57.000000 symbolx-0.4.1/symbolx/parsers/__init__.py
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     4615 2023-05-23 09:10:57.000000 symbolx-0.4.1/symbolx/parsers/parser_csv.py
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     3395 2023-05-23 09:10:57.000000 symbolx-0.4.1/symbolx/parsers/parser_feather.py
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)    12426 2023-07-21 21:25:07.000000 symbolx-0.4.1/symbolx/parsers/parser_gdx.py
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     1388 2023-05-23 09:10:57.000000 symbolx-0.4.1/symbolx/settings.py
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)    54620 2023-05-23 09:10:57.000000 symbolx-0.4.1/symbolx/symbols.py
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     6725 2023-05-23 09:10:57.000000 symbolx-0.4.1/symbolx/utils.py
+drwxrwxr-x   0 cgaete    (1000) cgaete    (1000)        0 2023-07-21 21:37:51.232957 symbolx-0.4.1/symbolx.egg-info/
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     3090 2023-07-21 21:37:51.000000 symbolx-0.4.1/symbolx.egg-info/PKG-INFO
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)      410 2023-07-21 21:37:51.000000 symbolx-0.4.1/symbolx.egg-info/SOURCES.txt
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)        1 2023-07-21 21:37:51.000000 symbolx-0.4.1/symbolx.egg-info/dependency_links.txt
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)       35 2023-07-21 21:37:51.000000 symbolx-0.4.1/symbolx.egg-info/requires.txt
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)        8 2023-07-21 21:37:51.000000 symbolx-0.4.1/symbolx.egg-info/top_level.txt
+drwxrwxr-x   0 cgaete    (1000) cgaete    (1000)        0 2023-07-21 21:37:51.232957 symbolx-0.4.1/test/
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     3559 2023-06-16 18:52:39.000000 symbolx-0.4.1/test/test.py
```

### Comparing `symbolx-0.4.0/LICENSE` & `symbolx-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `symbolx-0.4.0/PKG-INFO` & `symbolx-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbolx
-Version: 0.4.0
+Version: 0.4.1
 Summary:  Symbolx helps collecting several scenarios data such as multidimentional variables and parameters for reporting and visualization wiht help of karray
 Author: Carlos Gaete-Morales
 Author-email: cdgaete@gmail.com
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `symbolx-0.4.0/README.md` & `symbolx-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `symbolx-0.4.0/setup.py` & `symbolx-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         pkg = dirpath.replace(os.path.sep, ".")
         if os.path.altsep:
             pkg = pkg.replace(os.path.altsep, ".")
         packages.append(pkg)
 
 setup(
     name="symbolx",
-    version="0.4.0",
+    version="0.4.1",
     packages=packages,
     author="Carlos Gaete-Morales",
     author_email="cdgaete@gmail.com",
     install_requires=[
         "numpy",
         "pandas",
         "pyarrow",
```

### Comparing `symbolx-0.4.0/symbolx/__init__.py` & `symbolx-0.4.1/symbolx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # symbolx
 # copyright 2022, Carlos Gaete-Morales, DIW-Berlin 
 """
     symbolx
     copyright 2022, Carlos Gaete-Morales, DIW-Berlin 
 """
-__version__ = (0, 3, 2)
+__version__ = (0, 4, 1)
 __author__ = 'Carlos Gaete-Morales'
 
 
 from .parsers.parser_csv import symbol_parser_csv, load_csv
 from .parsers.parser_feather import symbol_parser_feather, load_feather
 from .parsers.parser_gdx import symbol_parser_gdx, load_gdx
 from .handler import DataCollection
```

### Comparing `symbolx-0.4.0/symbolx/handler.py` & `symbolx-0.4.1/symbolx/handler.py`

 * *Files identical despite different names*

### Comparing `symbolx-0.4.0/symbolx/parsers/parser_csv.py` & `symbolx-0.4.1/symbolx/parsers/parser_csv.py`

 * *Files identical despite different names*

### Comparing `symbolx-0.4.0/symbolx/parsers/parser_feather.py` & `symbolx-0.4.1/symbolx/parsers/parser_feather.py`

 * *Files identical despite different names*

### Comparing `symbolx-0.4.0/symbolx/parsers/parser_gdx.py` & `symbolx-0.4.1/symbolx/parsers/parser_gdx.py`

 * *Files identical despite different names*

### Comparing `symbolx-0.4.0/symbolx/settings.py` & `symbolx-0.4.1/symbolx/settings.py`

 * *Files identical despite different names*

### Comparing `symbolx-0.4.0/symbolx/symbols.py` & `symbolx-0.4.1/symbolx/symbols.py`

 * *Files identical despite different names*

### Comparing `symbolx-0.4.0/symbolx/utils.py` & `symbolx-0.4.1/symbolx/utils.py`

 * *Files identical despite different names*

### Comparing `symbolx-0.4.0/symbolx.egg-info/PKG-INFO` & `symbolx-0.4.1/symbolx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbolx
-Version: 0.4.0
+Version: 0.4.1
 Summary:  Symbolx helps collecting several scenarios data such as multidimentional variables and parameters for reporting and visualization wiht help of karray
 Author: Carlos Gaete-Morales
 Author-email: cdgaete@gmail.com
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `symbolx-0.4.0/test/test.py` & `symbolx-0.4.1/test/test.py`

 * *Files identical despite different names*

