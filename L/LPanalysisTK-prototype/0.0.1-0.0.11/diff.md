# Comparing `tmp/LPanalysisTK_prototype-0.0.1.tar.gz` & `tmp/LPanalysisTK_prototype-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LPanalysisTK_prototype-0.0.1.tar", last modified: Thu Jul 20 18:59:01 2023, max compression
+gzip compressed data, was "LPanalysisTK_prototype-0.0.11.tar", last modified: Fri Jul 21 12:59:19 2023, max compression
```

## Comparing `LPanalysisTK_prototype-0.0.1.tar` & `LPanalysisTK_prototype-0.0.11.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 18:59:01.047574 LPanalysisTK_prototype-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-07-18 16:56:25.000000 LPanalysisTK_prototype-0.0.1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-20 18:59:00.991304 LPanalysisTK_prototype-0.0.1/LPAnalysisTK_prototype/
--rw-rw-rw-   0        0        0      137 2023-07-20 18:51:48.000000 LPanalysisTK_prototype-0.0.1/LPAnalysisTK_prototype/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 18:59:01.045213 LPanalysisTK_prototype-0.0.1/LPanalysisTK_prototype.egg-info/
--rw-rw-rw-   0        0        0      791 2023-07-20 18:59:00.000000 LPanalysisTK_prototype-0.0.1/LPanalysisTK_prototype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-07-20 18:59:00.000000 LPanalysisTK_prototype-0.0.1/LPanalysisTK_prototype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 18:59:00.000000 LPanalysisTK_prototype-0.0.1/LPanalysisTK_prototype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-20 18:59:00.000000 LPanalysisTK_prototype-0.0.1/LPanalysisTK_prototype.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-20 18:59:00.000000 LPanalysisTK_prototype-0.0.1/LPanalysisTK_prototype.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      791 2023-07-20 18:59:01.047574 LPanalysisTK_prototype-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      136 2023-07-18 20:33:07.000000 LPanalysisTK_prototype-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-20 18:59:01.048671 LPanalysisTK_prototype-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1233 2023-07-20 18:58:55.000000 LPanalysisTK_prototype-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:59:19.936581 LPanalysisTK_prototype-0.0.11/
+-rw-rw-rw-   0        0        0     1091 2023-07-18 16:56:25.000000 LPanalysisTK_prototype-0.0.11/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-21 12:59:19.906567 LPanalysisTK_prototype-0.0.11/LPAnalysisTK_prototype/
+-rw-rw-rw-   0        0        0       91 2023-07-21 12:51:48.000000 LPanalysisTK_prototype-0.0.11/LPAnalysisTK_prototype/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:59:19.933591 LPanalysisTK_prototype-0.0.11/LPanalysisTK_prototype.egg-info/
+-rw-rw-rw-   0        0        0      792 2023-07-21 12:59:19.000000 LPanalysisTK_prototype-0.0.11/LPanalysisTK_prototype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-07-21 12:59:19.000000 LPanalysisTK_prototype-0.0.11/LPanalysisTK_prototype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 12:59:19.000000 LPanalysisTK_prototype-0.0.11/LPanalysisTK_prototype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-21 12:59:19.000000 LPanalysisTK_prototype-0.0.11/LPanalysisTK_prototype.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-21 12:59:19.000000 LPanalysisTK_prototype-0.0.11/LPanalysisTK_prototype.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      792 2023-07-21 12:59:19.935584 LPanalysisTK_prototype-0.0.11/PKG-INFO
+-rw-rw-rw-   0        0        0      136 2023-07-18 20:33:07.000000 LPanalysisTK_prototype-0.0.11/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-21 12:59:19.936581 LPanalysisTK_prototype-0.0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1234 2023-07-21 12:58:44.000000 LPanalysisTK_prototype-0.0.11/setup.py
```

### Comparing `LPanalysisTK_prototype-0.0.1/LICENSE` & `LPanalysisTK_prototype-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `LPanalysisTK_prototype-0.0.1/LPanalysisTK_prototype.egg-info/PKG-INFO` & `LPanalysisTK_prototype-0.0.11/LPanalysisTK_prototype.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LPanalysisTK-prototype
-Version: 0.0.1
+Version: 0.0.11
 Summary: A protoype of a new package in python for Laplacefintools analysis
 Author: Nabil Benjaa
 Author-email: nabil.benjaa@laplaceinsights.com
 Keywords: Analysis,Fintools
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `LPanalysisTK_prototype-0.0.1/PKG-INFO` & `LPanalysisTK_prototype-0.0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LPanalysisTK_prototype
-Version: 0.0.1
+Version: 0.0.11
 Summary: A protoype of a new package in python for Laplacefintools analysis
 Author: Nabil Benjaa
 Author-email: nabil.benjaa@laplaceinsights.com
 Keywords: Analysis,Fintools
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `LPanalysisTK_prototype-0.0.1/setup.py` & `LPanalysisTK_prototype-0.0.11/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.11'
 DESCRIPTION = "A protoype of a new package in python for Laplacefintools analysis"
 LONG_DESCRIPTION = "A protoype of a new package in python for Laplacefintools analysis"
 
 # Setting up
 setup(
     name="LPanalysisTK_prototype",
     version=VERSION,
```

