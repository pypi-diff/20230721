# Comparing `tmp/rst2dep-1.0.0.0.tar.gz` & `tmp/rst2dep-1.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rst2dep-1.0.0.0.tar", last modified: Wed Jul  5 18:00:34 2023, max compression
+gzip compressed data, was "dist\rst2dep-1.0.0.1.tar", last modified: Fri Jul 21 17:08:21 2023, max compression
```

## Comparing `rst2dep-1.0.0.0.tar` & `rst2dep-1.0.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 18:00:34.689212 rst2dep-1.0.0.0/
--rw-rw-rw-   0        0        0    10763 2023-06-30 21:19:28.000000 rst2dep-1.0.0.0/LICENSE
--rw-rw-rw-   0        0        0      780 2023-07-05 18:00:34.689212 rst2dep-1.0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     6121 2023-07-05 13:26:15.000000 rst2dep-1.0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 18:00:34.679179 rst2dep-1.0.0.0/rst2dep/
--rw-rw-rw-   0        0        0      127 2023-07-05 13:43:17.000000 rst2dep-1.0.0.0/rst2dep/__init__.py
--rw-rw-rw-   0        0        0     2704 2023-07-03 14:28:12.000000 rst2dep-1.0.0.0/rst2dep/__main__.py
--rw-rw-rw-   0        0        0    23648 2023-07-05 14:04:48.000000 rst2dep-1.0.0.0/rst2dep/classes.py
--rw-rw-rw-   0        0        0    16339 2023-07-05 13:43:13.000000 rst2dep-1.0.0.0/rst2dep/dep2rst.py
--rw-rw-rw-   0        0        0    13395 2021-10-21 19:46:30.000000 rst2dep-1.0.0.0/rst2dep/example.conllu
--rw-rw-rw-   0        0        0     2902 2021-10-21 20:26:06.000000 rst2dep-1.0.0.0/rst2dep/example.rs3
--rw-rw-rw-   0        0        0     1368 2021-10-21 20:24:03.000000 rst2dep-1.0.0.0/rst2dep/example.rsd
--rw-rw-rw-   0        0        0     3234 2023-07-05 14:04:58.000000 rst2dep-1.0.0.0/rst2dep/feature_extraction.py
--rw-rw-rw-   0        0        0    13374 2023-07-05 14:05:12.000000 rst2dep-1.0.0.0/rst2dep/rst2dep.py
--rw-rw-rw-   0        0        0      497 2023-06-30 21:52:58.000000 rst2dep-1.0.0.0/rst2dep/run_tests.py
-drwxrwxrwx   0        0        0        0 2023-07-05 18:00:34.689212 rst2dep-1.0.0.0/rst2dep.egg-info/
--rw-rw-rw-   0        0        0      780 2023-07-05 18:00:34.000000 rst2dep-1.0.0.0/rst2dep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-07-05 18:00:34.000000 rst2dep-1.0.0.0/rst2dep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 18:00:34.000000 rst2dep-1.0.0.0/rst2dep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-05 18:00:34.000000 rst2dep-1.0.0.0/rst2dep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 18:00:34.689212 rst2dep-1.0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-07-05 18:00:30.000000 rst2dep-1.0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 17:08:21.586852 rst2dep-1.0.0.1/
+-rw-rw-rw-   0        0        0    10763 2023-06-30 21:19:28.000000 rst2dep-1.0.0.1/LICENSE
+-rw-rw-rw-   0        0        0      780 2023-07-21 17:08:21.586852 rst2dep-1.0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6121 2023-07-05 13:26:15.000000 rst2dep-1.0.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 17:08:21.576701 rst2dep-1.0.0.1/rst2dep/
+-rw-rw-rw-   0        0        0      127 2023-07-05 13:43:17.000000 rst2dep-1.0.0.1/rst2dep/__init__.py
+-rw-rw-rw-   0        0        0     2704 2023-07-03 14:28:12.000000 rst2dep-1.0.0.1/rst2dep/__main__.py
+-rw-rw-rw-   0        0        0    23657 2023-07-19 15:24:54.000000 rst2dep-1.0.0.1/rst2dep/classes.py
+-rw-rw-rw-   0        0        0    16339 2023-07-05 13:43:13.000000 rst2dep-1.0.0.1/rst2dep/dep2rst.py
+-rw-rw-rw-   0        0        0    13395 2021-10-21 19:46:30.000000 rst2dep-1.0.0.1/rst2dep/example.conllu
+-rw-rw-rw-   0        0        0     2902 2021-10-21 20:26:06.000000 rst2dep-1.0.0.1/rst2dep/example.rs3
+-rw-rw-rw-   0        0        0     1368 2021-10-21 20:24:03.000000 rst2dep-1.0.0.1/rst2dep/example.rsd
+-rw-rw-rw-   0        0        0     3234 2023-07-05 14:04:58.000000 rst2dep-1.0.0.1/rst2dep/feature_extraction.py
+-rw-rw-rw-   0        0        0    13374 2023-07-05 14:05:12.000000 rst2dep-1.0.0.1/rst2dep/rst2dep.py
+-rw-rw-rw-   0        0        0      497 2023-06-30 21:52:58.000000 rst2dep-1.0.0.1/rst2dep/run_tests.py
+drwxrwxrwx   0        0        0        0 2023-07-21 17:08:21.584776 rst2dep-1.0.0.1/rst2dep.egg-info/
+-rw-rw-rw-   0        0        0      780 2023-07-21 17:08:21.000000 rst2dep-1.0.0.1/rst2dep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-07-21 17:08:21.000000 rst2dep-1.0.0.1/rst2dep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 17:08:21.000000 rst2dep-1.0.0.1/rst2dep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-21 17:08:21.000000 rst2dep-1.0.0.1/rst2dep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 17:08:21.586852 rst2dep-1.0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-07-21 17:07:25.000000 rst2dep-1.0.0.1/setup.py
```

### Comparing `rst2dep-1.0.0.0/LICENSE` & `rst2dep-1.0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rst2dep-1.0.0.0/PKG-INFO` & `rst2dep-1.0.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: rst2dep
-Version: 1.0.0.0
+Version: 1.0.0.1
 Summary: RST (Rhetorical Structure Theory) constituent and dependency converter for discourse parses
 Home-page: https://github.com/amir-zeldes/rst2dep
 Author: Amir Zeldes
 Author-email: amir.zeldes@georgetown.edu
 License: Apache License, Version 2.0
-Download-URL: https://github.com/amir-zeldes/rst2dep/releases/tag/v1.0.0.0
+Download-URL: https://github.com/amir-zeldes/rst2dep/releases/tag/v1.0.0.1
 Description: UNKNOWN
 Keywords: NLP,RST,discourse,dependencies,converter,conversion,Rhetorical Structure Theory,parsing
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `rst2dep-1.0.0.0/README.md` & `rst2dep-1.0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `rst2dep-1.0.0.0/rst2dep/__main__.py` & `rst2dep-1.0.0.1/rst2dep/__main__.py`

 * *Files identical despite different names*

### Comparing `rst2dep-1.0.0.0/rst2dep/classes.py` & `rst2dep-1.0.0.1/rst2dep/classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from xml.dom import minidom
 from xml.parsers.expat import ExpatError
-import re, collections
+import re, collections, sys, io
 
 
 class SIGNAL:
     def __init__(self, sigtype, sigsubtype, tokens):
         self.type = sigtype
         self.subtype = sigsubtype
         self.tokens = tokens
```

### Comparing `rst2dep-1.0.0.0/rst2dep/dep2rst.py` & `rst2dep-1.0.0.1/rst2dep/dep2rst.py`

 * *Files identical despite different names*

### Comparing `rst2dep-1.0.0.0/rst2dep/example.conllu` & `rst2dep-1.0.0.1/rst2dep/example.conllu`

 * *Files identical despite different names*

### Comparing `rst2dep-1.0.0.0/rst2dep/example.rs3` & `rst2dep-1.0.0.1/rst2dep/example.rs3`

 * *Files identical despite different names*

### Comparing `rst2dep-1.0.0.0/rst2dep/example.rsd` & `rst2dep-1.0.0.1/rst2dep/example.rsd`

 * *Files identical despite different names*

### Comparing `rst2dep-1.0.0.0/rst2dep/feature_extraction.py` & `rst2dep-1.0.0.1/rst2dep/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `rst2dep-1.0.0.0/rst2dep/rst2dep.py` & `rst2dep-1.0.0.1/rst2dep/rst2dep.py`

 * *Files identical despite different names*

### Comparing `rst2dep-1.0.0.0/rst2dep.egg-info/PKG-INFO` & `rst2dep-1.0.0.1/rst2dep.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: rst2dep
-Version: 1.0.0.0
+Version: 1.0.0.1
 Summary: RST (Rhetorical Structure Theory) constituent and dependency converter for discourse parses
 Home-page: https://github.com/amir-zeldes/rst2dep
 Author: Amir Zeldes
 Author-email: amir.zeldes@georgetown.edu
 License: Apache License, Version 2.0
-Download-URL: https://github.com/amir-zeldes/rst2dep/releases/tag/v1.0.0.0
+Download-URL: https://github.com/amir-zeldes/rst2dep/releases/tag/v1.0.0.1
 Description: UNKNOWN
 Keywords: NLP,RST,discourse,dependencies,converter,conversion,Rhetorical Structure Theory,parsing
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `rst2dep-1.0.0.0/setup.py` & `rst2dep-1.0.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'rst2dep',
   packages = find_packages(),
-  version = '1.0.0.0',
+  version = '1.0.0.1',
   description = 'RST (Rhetorical Structure Theory) constituent and dependency converter for discourse parses',
   author = 'Amir Zeldes',
   author_email = 'amir.zeldes@georgetown.edu',
   package_data = {'':['README.md','LICENSE','requirements.txt'],'rst2dep':['*']},
   install_requires=[],
   url = 'https://github.com/amir-zeldes/rst2dep',
   license='Apache License, Version 2.0',
-  download_url = 'https://github.com/amir-zeldes/rst2dep/releases/tag/v1.0.0.0',
+  download_url = 'https://github.com/amir-zeldes/rst2dep/releases/tag/v1.0.0.1',
   keywords = ['NLP', 'RST', 'discourse', 'dependencies', 'converter', 'conversion','Rhetorical Structure Theory','parsing'],
   classifiers = ['Programming Language :: Python',
 'Programming Language :: Python :: 2',
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: Apache Software License',
 'Operating System :: OS Independent'],
 )
```

