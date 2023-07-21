# Comparing `tmp/notip-0.1.5.tar.gz` & `tmp/notip-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notip-0.1.5.tar", last modified: Fri Jul 21 17:31:32 2023, max compression
+gzip compressed data, was "notip-0.1.6.tar", last modified: Fri Jul 21 19:50:32 2023, max compression
```

## Comparing `notip-0.1.5.tar` & `notip-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ablain   (666989) soda     (202037)        0 2023-07-21 17:31:32.474754 notip-0.1.5/
--rw-r--r--   0 ablain   (666989) soda     (202037)     1347 2023-07-21 17:31:32.474754 notip-0.1.5/PKG-INFO
--rw-r--r--   0 ablain   (666989) soda     (202037)      848 2023-05-08 21:35:42.000000 notip-0.1.5/README.md
-drwxr-xr-x   0 ablain   (666989) soda     (202037)        0 2023-07-21 17:31:32.474754 notip-0.1.5/notip/
--rw-r--r--   0 ablain   (666989) soda     (202037)        1 2023-05-08 21:35:42.000000 notip-0.1.5/notip/__init__.py
--rw-r--r--   0 ablain   (666989) soda     (202037)    45671 2023-06-21 12:32:40.000000 notip-0.1.5/notip/posthoc_fmri.py
-drwxr-xr-x   0 ablain   (666989) soda     (202037)        0 2023-07-21 17:31:32.474754 notip-0.1.5/notip.egg-info/
--rw-r--r--   0 ablain   (666989) soda     (202037)     1347 2023-07-21 17:31:32.000000 notip-0.1.5/notip.egg-info/PKG-INFO
--rw-r--r--   0 ablain   (666989) soda     (202037)      212 2023-07-21 17:31:32.000000 notip-0.1.5/notip.egg-info/SOURCES.txt
--rw-r--r--   0 ablain   (666989) soda     (202037)        1 2023-07-21 17:31:32.000000 notip-0.1.5/notip.egg-info/dependency_links.txt
--rw-r--r--   0 ablain   (666989) soda     (202037)      108 2023-07-21 17:31:32.000000 notip-0.1.5/notip.egg-info/requires.txt
--rw-r--r--   0 ablain   (666989) soda     (202037)        6 2023-07-21 17:31:32.000000 notip-0.1.5/notip.egg-info/top_level.txt
--rw-r--r--   0 ablain   (666989) soda     (202037)       79 2023-07-21 17:31:32.474754 notip-0.1.5/setup.cfg
--rw-r--r--   0 ablain   (666989) soda     (202037)      976 2023-07-21 17:31:05.000000 notip-0.1.5/setup.py
+drwxr-xr-x   0 ablain   (666989) soda     (202037)        0 2023-07-21 19:50:32.614580 notip-0.1.6/
+-rw-r--r--   0 ablain   (666989) soda     (202037)     1347 2023-07-21 19:50:32.614580 notip-0.1.6/PKG-INFO
+-rw-r--r--   0 ablain   (666989) soda     (202037)      848 2023-05-08 21:35:42.000000 notip-0.1.6/README.md
+drwxr-xr-x   0 ablain   (666989) soda     (202037)        0 2023-07-21 19:50:32.610580 notip-0.1.6/notip/
+-rw-r--r--   0 ablain   (666989) soda     (202037)        1 2023-05-08 21:35:42.000000 notip-0.1.6/notip/__init__.py
+-rw-r--r--   0 ablain   (666989) soda     (202037)    45671 2023-06-21 12:32:40.000000 notip-0.1.6/notip/posthoc_fmri.py
+drwxr-xr-x   0 ablain   (666989) soda     (202037)        0 2023-07-21 19:50:32.614580 notip-0.1.6/notip.egg-info/
+-rw-r--r--   0 ablain   (666989) soda     (202037)     1347 2023-07-21 19:50:32.000000 notip-0.1.6/notip.egg-info/PKG-INFO
+-rw-r--r--   0 ablain   (666989) soda     (202037)      212 2023-07-21 19:50:32.000000 notip-0.1.6/notip.egg-info/SOURCES.txt
+-rw-r--r--   0 ablain   (666989) soda     (202037)        1 2023-07-21 19:50:32.000000 notip-0.1.6/notip.egg-info/dependency_links.txt
+-rw-r--r--   0 ablain   (666989) soda     (202037)      123 2023-07-21 19:50:32.000000 notip-0.1.6/notip.egg-info/requires.txt
+-rw-r--r--   0 ablain   (666989) soda     (202037)        6 2023-07-21 19:50:32.000000 notip-0.1.6/notip.egg-info/top_level.txt
+-rw-r--r--   0 ablain   (666989) soda     (202037)       79 2023-07-21 19:50:32.614580 notip-0.1.6/setup.cfg
+-rw-r--r--   0 ablain   (666989) soda     (202037)     1008 2023-07-21 19:50:17.000000 notip-0.1.6/setup.py
```

### Comparing `notip-0.1.5/PKG-INFO` & `notip-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notip
-Version: 0.1.5
+Version: 0.1.6
 Summary: Nonparametric True Discovery Proportion control for brain imaging
 Home-page: https://github.com/alexblnn/Notip
 Download-URL: https://github.com/alexblnn/Notip/releases/download/Notip_OHBM_v2/notip-0.1.2.tar.gz
 Author: Alexandre Blain
 Author-email: alexandre.blain@inria.fr
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `notip-0.1.5/README.md` & `notip-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `notip-0.1.5/notip/posthoc_fmri.py` & `notip-0.1.6/notip/posthoc_fmri.py`

 * *Files identical despite different names*

### Comparing `notip-0.1.5/notip.egg-info/PKG-INFO` & `notip-0.1.6/notip.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notip
-Version: 0.1.5
+Version: 0.1.6
 Summary: Nonparametric True Discovery Proportion control for brain imaging
 Home-page: https://github.com/alexblnn/Notip
 Download-URL: https://github.com/alexblnn/Notip/releases/download/Notip_OHBM_v2/notip-0.1.2.tar.gz
 Author: Alexandre Blain
 Author-email: alexandre.blain@inria.fr
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `notip-0.1.5/setup.py` & `notip-0.1.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = ["numpy>=1.15.0", "scipy>=1.0.0",
                 "joblib>=1.0.1", "scikit-learn>=0.22",
-                "nilearn","sanssouci","matplotlib",
+                "nilearn>=0.10.0","matplotlib>=3.3.0",
+                "sanssouci",
                 "pandas", "joblib", "tqdm"]
 
 setup(
     name="notip",
-    version="0.1.5",
+    version="0.1.6",
     author="Alexandre Blain",
     author_email="alexandre.blain@inria.fr",
     description="Nonparametric True Discovery Proportion control for brain imaging",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/alexblnn/Notip",
     download_url="https://github.com/alexblnn/Notip/releases/download/Notip_OHBM_v2/notip-0.1.2.tar.gz",
```

