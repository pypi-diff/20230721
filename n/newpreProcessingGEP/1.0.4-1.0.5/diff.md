# Comparing `tmp/newpreProcessingGEP-1.0.4.tar.gz` & `tmp/newpreProcessingGEP-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newpreProcessingGEP-1.0.4.tar", last modified: Fri Jul 21 10:21:11 2023, max compression
+gzip compressed data, was "newpreProcessingGEP-1.0.5.tar", last modified: Fri Jul 21 10:49:15 2023, max compression
```

## Comparing `newpreProcessingGEP-1.0.4.tar` & `newpreProcessingGEP-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 10:21:11.498415 newpreProcessingGEP-1.0.4/
--rw-rw-rw-   0        0        0       11 2023-07-04 12:45:21.000000 newpreProcessingGEP-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     2668 2023-07-21 10:21:11.495417 newpreProcessingGEP-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2189 2023-07-21 10:17:03.000000 newpreProcessingGEP-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 10:21:11.430104 newpreProcessingGEP-1.0.4/newpreProcessingGEP/
--rw-rw-rw-   0        0        0      210 2023-07-21 10:03:14.000000 newpreProcessingGEP-1.0.4/newpreProcessingGEP/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:21:11.492415 newpreProcessingGEP-1.0.4/newpreProcessingGEP.egg-info/
--rw-rw-rw-   0        0        0     2668 2023-07-21 10:21:11.000000 newpreProcessingGEP-1.0.4/newpreProcessingGEP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-07-21 10:21:11.000000 newpreProcessingGEP-1.0.4/newpreProcessingGEP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 10:21:11.000000 newpreProcessingGEP-1.0.4/newpreProcessingGEP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-21 10:21:11.000000 newpreProcessingGEP-1.0.4/newpreProcessingGEP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 10:21:11.500416 newpreProcessingGEP-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      698 2023-07-21 10:18:24.000000 newpreProcessingGEP-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 10:49:15.210419 newpreProcessingGEP-1.0.5/
+-rw-rw-rw-   0        0        0       11 2023-07-04 12:45:21.000000 newpreProcessingGEP-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2688 2023-07-21 10:49:15.208397 newpreProcessingGEP-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2209 2023-07-21 10:48:32.000000 newpreProcessingGEP-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 10:49:15.172378 newpreProcessingGEP-1.0.5/newpreProcessingGEP/
+-rw-rw-rw-   0        0        0      210 2023-07-21 10:48:34.000000 newpreProcessingGEP-1.0.5/newpreProcessingGEP/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 10:49:15.206385 newpreProcessingGEP-1.0.5/newpreProcessingGEP.egg-info/
+-rw-rw-rw-   0        0        0     2688 2023-07-21 10:49:14.000000 newpreProcessingGEP-1.0.5/newpreProcessingGEP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-07-21 10:49:15.000000 newpreProcessingGEP-1.0.5/newpreProcessingGEP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 10:49:14.000000 newpreProcessingGEP-1.0.5/newpreProcessingGEP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-21 10:49:14.000000 newpreProcessingGEP-1.0.5/newpreProcessingGEP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 10:49:15.212394 newpreProcessingGEP-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      698 2023-07-21 10:45:56.000000 newpreProcessingGEP-1.0.5/setup.py
```

### Comparing `newpreProcessingGEP-1.0.4/PKG-INFO` & `newpreProcessingGEP-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newpreProcessingGEP
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package for preprocessing text
 Home-page: https://github.com/vanshajsingla03/newpreProcessingGEP
 Author: Vanshaj Singla
 Author-email: vanshaj.singla@gep.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,25 +16,35 @@
 
 You can access following functions:
 
 The provided package is a collection of functions for text preprocessing and cleaning. Here is a brief explanation of each function :
 
 FOR SUPPLIER:
 
+
 supplier_name_cleaning
+
 supplier_norm_name_cleaning
+
 supplier_name_normalization_bkp
 
 
 FOR KEYWORD:
+
+
 removestopwords
+
 lemmatization
+
 removespecialchars
+
 RemoveNonEngWords
+
 SeparateNumStrings
+
 stemming
 
 
 FOR ITEM:
 
 _en_stopwords: Returns a list of English stopwords.
```

### Comparing `newpreProcessingGEP-1.0.4/README.md` & `newpreProcessingGEP-1.0.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,35 @@
 
 You can access following functions:
 
 The provided package is a collection of functions for text preprocessing and cleaning. Here is a brief explanation of each function :
 
 FOR SUPPLIER:
 
+
 supplier_name_cleaning
+
 supplier_norm_name_cleaning
+
 supplier_name_normalization_bkp
 
 
 FOR KEYWORD:
+
+
 removestopwords
+
 lemmatization
+
 removespecialchars
+
 RemoveNonEngWords
+
 SeparateNumStrings
+
 stemming
 
 
 FOR ITEM:
 
 _en_stopwords: Returns a list of English stopwords.
```

### Comparing `newpreProcessingGEP-1.0.4/newpreProcessingGEP.egg-info/PKG-INFO` & `newpreProcessingGEP-1.0.5/newpreProcessingGEP.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newpreProcessingGEP
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package for preprocessing text
 Home-page: https://github.com/vanshajsingla03/newpreProcessingGEP
 Author: Vanshaj Singla
 Author-email: vanshaj.singla@gep.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,25 +16,35 @@
 
 You can access following functions:
 
 The provided package is a collection of functions for text preprocessing and cleaning. Here is a brief explanation of each function :
 
 FOR SUPPLIER:
 
+
 supplier_name_cleaning
+
 supplier_norm_name_cleaning
+
 supplier_name_normalization_bkp
 
 
 FOR KEYWORD:
+
+
 removestopwords
+
 lemmatization
+
 removespecialchars
+
 RemoveNonEngWords
+
 SeparateNumStrings
+
 stemming
 
 
 FOR ITEM:
 
 _en_stopwords: Returns a list of English stopwords.
```

### Comparing `newpreProcessingGEP-1.0.4/setup.py` & `newpreProcessingGEP-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="newpreProcessingGEP",
-    version="1.0.4",
+    version="1.0.5",
     author="Vanshaj Singla",
     author_email="vanshaj.singla@gep.com",
     description="A package for preprocessing text",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/vanshajsingla03/newpreProcessingGEP",
     packages=["newpreProcessingGEP"],
```

