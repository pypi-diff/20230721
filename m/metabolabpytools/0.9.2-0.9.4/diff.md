# Comparing `tmp/metabolabpytools-0.9.2.tar.gz` & `tmp/metabolabpytools-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabolabpytools-0.9.2.tar", last modified: Wed Jul 19 23:20:03 2023, max compression
+gzip compressed data, was "metabolabpytools-0.9.4.tar", last modified: Fri Jul 21 11:29:36 2023, max compression
```

## Comparing `metabolabpytools-0.9.2.tar` & `metabolabpytools-0.9.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-19 23:20:03.703395 metabolabpytools-0.9.2/
--rw-r--r--   0 ludwigc  (1699341573) 1311385079    35149 2023-06-29 16:08:10.000000 metabolabpytools-0.9.2/LICENSE
--rw-r--r--   0 ludwigc  (1699341573) 1311385079       78 2023-06-29 16:08:10.000000 metabolabpytools-0.9.2/MANIFEST.in
--rw-r--r--   0 ludwigc  (1699341573) 1311385079     3709 2023-07-19 23:20:03.703211 metabolabpytools-0.9.2/PKG-INFO
--rw-r--r--   0 ludwigc  (1699341573) 1311385079       67 2023-06-29 16:08:10.000000 metabolabpytools-0.9.2/README.md
--rw-r--r--   0 ludwigc  (1699341573) 1311385079     2977 2023-06-29 16:08:10.000000 metabolabpytools-0.9.2/README.rst
-drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-19 23:20:03.702098 metabolabpytools-0.9.2/metabolabpytools/
--rw-r--r--   0 ludwigc  (1699341573) 1311385079      153 2023-07-19 23:17:38.000000 metabolabpytools-0.9.2/metabolabpytools/__init__.py
--rw-r--r--   0 ludwigc  (1699341573) 1311385079     1893 2023-06-29 16:08:10.000000 metabolabpytools-0.9.2/metabolabpytools/analysis.py
--rw-r--r--   0 ludwigc  (1699341573) 1311385079    25753 2023-07-16 14:50:21.000000 metabolabpytools-0.9.2/metabolabpytools/isotopomerAnalysis.py
-drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-19 23:20:03.703030 metabolabpytools-0.9.2/metabolabpytools.egg-info/
--rw-r--r--   0 ludwigc  (1699341573) 1311385079     3709 2023-07-19 23:20:03.000000 metabolabpytools-0.9.2/metabolabpytools.egg-info/PKG-INFO
--rw-r--r--   0 ludwigc  (1699341573) 1311385079      362 2023-07-19 23:20:03.000000 metabolabpytools-0.9.2/metabolabpytools.egg-info/SOURCES.txt
--rw-r--r--   0 ludwigc  (1699341573) 1311385079        1 2023-07-19 23:20:03.000000 metabolabpytools-0.9.2/metabolabpytools.egg-info/dependency_links.txt
--rw-r--r--   0 ludwigc  (1699341573) 1311385079       19 2023-07-19 23:20:03.000000 metabolabpytools-0.9.2/metabolabpytools.egg-info/requires.txt
--rw-r--r--   0 ludwigc  (1699341573) 1311385079       17 2023-07-19 23:20:03.000000 metabolabpytools-0.9.2/metabolabpytools.egg-info/top_level.txt
--rw-r--r--   0 ludwigc  (1699341573) 1311385079       19 2023-06-29 16:08:10.000000 metabolabpytools-0.9.2/requirements.txt
--rw-r--r--   0 ludwigc  (1699341573) 1311385079       38 2023-07-19 23:20:03.703440 metabolabpytools-0.9.2/setup.cfg
--rw-r--r--   0 ludwigc  (1699341573) 1311385079     1507 2023-06-29 16:08:10.000000 metabolabpytools-0.9.2/setup.py
+drwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        0 2023-07-21 11:29:36.919814 metabolabpytools-0.9.4/
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)    35149 2023-06-29 16:08:10.000000 metabolabpytools-0.9.4/LICENSE
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)       78 2023-06-29 16:08:10.000000 metabolabpytools-0.9.4/MANIFEST.in
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)     3709 2023-07-21 11:29:36.919611 metabolabpytools-0.9.4/PKG-INFO
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)       67 2023-06-29 16:08:10.000000 metabolabpytools-0.9.4/README.md
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)     2977 2023-06-29 16:08:10.000000 metabolabpytools-0.9.4/README.rst
+drwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        0 2023-07-21 11:29:36.918425 metabolabpytools-0.9.4/metabolabpytools/
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)      153 2023-07-21 11:29:30.000000 metabolabpytools-0.9.4/metabolabpytools/__init__.py
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)     1893 2023-06-29 16:08:10.000000 metabolabpytools-0.9.4/metabolabpytools/analysis.py
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)    25753 2023-07-16 14:50:21.000000 metabolabpytools-0.9.4/metabolabpytools/isotopomerAnalysis.py
+drwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        0 2023-07-21 11:29:36.919436 metabolabpytools-0.9.4/metabolabpytools.egg-info/
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)     3709 2023-07-21 11:29:36.000000 metabolabpytools-0.9.4/metabolabpytools.egg-info/PKG-INFO
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)      362 2023-07-21 11:29:36.000000 metabolabpytools-0.9.4/metabolabpytools.egg-info/SOURCES.txt
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        1 2023-07-21 11:29:36.000000 metabolabpytools-0.9.4/metabolabpytools.egg-info/dependency_links.txt
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)       19 2023-07-21 11:29:36.000000 metabolabpytools-0.9.4/metabolabpytools.egg-info/requires.txt
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)       17 2023-07-21 11:29:36.000000 metabolabpytools-0.9.4/metabolabpytools.egg-info/top_level.txt
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)       19 2023-06-29 16:08:10.000000 metabolabpytools-0.9.4/requirements.txt
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)       38 2023-07-21 11:29:36.919854 metabolabpytools-0.9.4/setup.cfg
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)     1507 2023-06-29 16:08:10.000000 metabolabpytools-0.9.4/setup.py
```

### Comparing `metabolabpytools-0.9.2/LICENSE` & `metabolabpytools-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `metabolabpytools-0.9.2/PKG-INFO` & `metabolabpytools-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabolabpytools
-Version: 0.9.2
+Version: 0.9.4
 Summary: Tools for metabolomics and metabolism tracing data
 Home-page: https://github.com/ludwigc/metabolabpytools
 Author: Christian Ludwig
 Author-email: C.Ludwig@bham.ac.uk 
 License: GPLv3
 Keywords: Metabolomics,Tracing,NMR,Data Processing,13C
 Platform: MacOS, Windows, UNIX
```

### Comparing `metabolabpytools-0.9.2/README.rst` & `metabolabpytools-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `metabolabpytools-0.9.2/metabolabpytools/analysis.py` & `metabolabpytools-0.9.4/metabolabpytools/analysis.py`

 * *Files identical despite different names*

### Comparing `metabolabpytools-0.9.2/metabolabpytools/isotopomerAnalysis.py` & `metabolabpytools-0.9.4/metabolabpytools/isotopomerAnalysis.py`

 * *Files identical despite different names*

### Comparing `metabolabpytools-0.9.2/metabolabpytools.egg-info/PKG-INFO` & `metabolabpytools-0.9.4/metabolabpytools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabolabpytools
-Version: 0.9.2
+Version: 0.9.4
 Summary: Tools for metabolomics and metabolism tracing data
 Home-page: https://github.com/ludwigc/metabolabpytools
 Author: Christian Ludwig
 Author-email: C.Ludwig@bham.ac.uk 
 License: GPLv3
 Keywords: Metabolomics,Tracing,NMR,Data Processing,13C
 Platform: MacOS, Windows, UNIX
```

### Comparing `metabolabpytools-0.9.2/setup.py` & `metabolabpytools-0.9.4/setup.py`

 * *Files identical despite different names*

