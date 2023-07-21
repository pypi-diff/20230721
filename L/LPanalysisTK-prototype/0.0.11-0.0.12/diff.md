# Comparing `tmp/LPanalysisTK_prototype-0.0.11.tar.gz` & `tmp/LPanalysisTK_prototype-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LPanalysisTK_prototype-0.0.11.tar", last modified: Fri Jul 21 12:59:19 2023, max compression
+gzip compressed data, was "LPanalysisTK_prototype-0.0.12.tar", last modified: Fri Jul 21 13:46:49 2023, max compression
```

## Comparing `LPanalysisTK_prototype-0.0.11.tar` & `LPanalysisTK_prototype-0.0.12.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 12:59:19.936581 LPanalysisTK_prototype-0.0.11/
--rw-rw-rw-   0        0        0     1091 2023-07-18 16:56:25.000000 LPanalysisTK_prototype-0.0.11/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-21 12:59:19.906567 LPanalysisTK_prototype-0.0.11/LPAnalysisTK_prototype/
--rw-rw-rw-   0        0        0       91 2023-07-21 12:51:48.000000 LPanalysisTK_prototype-0.0.11/LPAnalysisTK_prototype/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 12:59:19.933591 LPanalysisTK_prototype-0.0.11/LPanalysisTK_prototype.egg-info/
--rw-rw-rw-   0        0        0      792 2023-07-21 12:59:19.000000 LPanalysisTK_prototype-0.0.11/LPanalysisTK_prototype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-07-21 12:59:19.000000 LPanalysisTK_prototype-0.0.11/LPanalysisTK_prototype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 12:59:19.000000 LPanalysisTK_prototype-0.0.11/LPanalysisTK_prototype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-21 12:59:19.000000 LPanalysisTK_prototype-0.0.11/LPanalysisTK_prototype.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-21 12:59:19.000000 LPanalysisTK_prototype-0.0.11/LPanalysisTK_prototype.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      792 2023-07-21 12:59:19.935584 LPanalysisTK_prototype-0.0.11/PKG-INFO
--rw-rw-rw-   0        0        0      136 2023-07-18 20:33:07.000000 LPanalysisTK_prototype-0.0.11/README.md
--rw-rw-rw-   0        0        0       42 2023-07-21 12:59:19.936581 LPanalysisTK_prototype-0.0.11/setup.cfg
--rw-rw-rw-   0        0        0     1234 2023-07-21 12:58:44.000000 LPanalysisTK_prototype-0.0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 13:46:49.636075 LPanalysisTK_prototype-0.0.12/
+-rw-rw-rw-   0        0        0     1091 2023-07-18 16:56:25.000000 LPanalysisTK_prototype-0.0.12/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-21 13:46:49.579017 LPanalysisTK_prototype-0.0.12/LPAnalysisTK_prototype/
+-rw-rw-rw-   0        0        0      139 2023-07-21 13:46:26.000000 LPanalysisTK_prototype-0.0.12/LPAnalysisTK_prototype/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 13:46:49.630588 LPanalysisTK_prototype-0.0.12/LPanalysisTK_prototype.egg-info/
+-rw-rw-rw-   0        0        0      792 2023-07-21 13:46:49.000000 LPanalysisTK_prototype-0.0.12/LPanalysisTK_prototype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-07-21 13:46:49.000000 LPanalysisTK_prototype-0.0.12/LPanalysisTK_prototype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 13:46:49.000000 LPanalysisTK_prototype-0.0.12/LPanalysisTK_prototype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-21 13:46:49.000000 LPanalysisTK_prototype-0.0.12/LPanalysisTK_prototype.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-21 13:46:49.000000 LPanalysisTK_prototype-0.0.12/LPanalysisTK_prototype.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      792 2023-07-21 13:46:49.633584 LPanalysisTK_prototype-0.0.12/PKG-INFO
+-rw-rw-rw-   0        0        0      136 2023-07-18 20:33:07.000000 LPanalysisTK_prototype-0.0.12/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-21 13:46:49.636075 LPanalysisTK_prototype-0.0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1232 2023-07-21 13:46:09.000000 LPanalysisTK_prototype-0.0.12/setup.py
```

### Comparing `LPanalysisTK_prototype-0.0.11/LICENSE` & `LPanalysisTK_prototype-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `LPanalysisTK_prototype-0.0.11/LPanalysisTK_prototype.egg-info/PKG-INFO` & `LPanalysisTK_prototype-0.0.12/LPanalysisTK_prototype.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LPanalysisTK-prototype
-Version: 0.0.11
+Version: 0.0.12
 Summary: A protoype of a new package in python for Laplacefintools analysis
 Author: Nabil Benjaa
 Author-email: nabil.benjaa@laplaceinsights.com
 Keywords: Analysis,Fintools
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `LPanalysisTK_prototype-0.0.11/PKG-INFO` & `LPanalysisTK_prototype-0.0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LPanalysisTK_prototype
-Version: 0.0.11
+Version: 0.0.12
 Summary: A protoype of a new package in python for Laplacefintools analysis
 Author: Nabil Benjaa
 Author-email: nabil.benjaa@laplaceinsights.com
 Keywords: Analysis,Fintools
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `LPanalysisTK_prototype-0.0.11/setup.py` & `LPanalysisTK_prototype-0.0.12/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.11'
+VERSION = '0.0.12'
 DESCRIPTION = "A protoype of a new package in python for Laplacefintools analysis"
 LONG_DESCRIPTION = "A protoype of a new package in python for Laplacefintools analysis"
 
 # Setting up
 setup(
     name="LPanalysisTK_prototype",
     version=VERSION,
@@ -19,15 +19,15 @@
     author_email="nabil.benjaa@laplaceinsights.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     setup_requires=['wheel'],
     install_requires=["pandas","numpy"],
-    keywords = ["Analysis", "Fintools"],
+    keywords=["Analysis", "Fintools"],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: Microsoft :: Windows",
         "License :: OSI Approved :: MIT License",
```

