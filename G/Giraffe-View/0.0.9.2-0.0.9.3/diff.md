# Comparing `tmp/Giraffe_View-0.0.9.2.tar.gz` & `tmp/Giraffe_View-0.0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Giraffe_View-0.0.9.2.tar", last modified: Fri Jul 21 06:38:23 2023, max compression
+gzip compressed data, was "Giraffe_View-0.0.9.3.tar", last modified: Fri Jul 21 10:04:50 2023, max compression
```

## Comparing `Giraffe_View-0.0.9.2.tar` & `Giraffe_View-0.0.9.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-21 06:38:23.269874 Giraffe_View-0.0.9.2/
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-21 06:38:23.265874 Giraffe_View-0.0.9.2/Giraffe_View/
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       57 2023-07-18 11:47:04.000000 Giraffe_View-0.0.9.2/Giraffe_View/__init__.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2835 2023-07-18 10:42:50.000000 Giraffe_View-0.0.9.2/Giraffe_View/estimated_read_accuracy.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4539 2023-07-18 10:42:50.000000 Giraffe_View-0.0.9.2/Giraffe_View/function.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3288 2023-07-18 11:57:08.000000 Giraffe_View-0.0.9.2/Giraffe_View/gc_bias.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4357 2023-07-21 06:37:43.000000 Giraffe_View-0.0.9.2/Giraffe_View/giraffe
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4721 2023-07-18 12:03:26.000000 Giraffe_View-0.0.9.2/Giraffe_View/homopolymer.py
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     2944 2023-07-18 10:42:50.000000 Giraffe_View-0.0.9.2/Giraffe_View/observed_read_accuracy.py
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     5505 2023-07-21 05:59:39.000000 Giraffe_View-0.0.9.2/Giraffe_View/plot.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2156 2023-07-18 10:42:50.000000 Giraffe_View-0.0.9.2/Giraffe_View/regional_modification.py
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-21 06:38:23.269874 Giraffe_View-0.0.9.2/Giraffe_View.egg-info/
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5057 2023-07-21 06:38:23.000000 Giraffe_View-0.0.9.2/Giraffe_View.egg-info/PKG-INFO
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)      466 2023-07-21 06:38:23.000000 Giraffe_View-0.0.9.2/Giraffe_View.egg-info/SOURCES.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2023-07-21 06:38:23.000000 Giraffe_View-0.0.9.2/Giraffe_View.egg-info/dependency_links.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       64 2023-07-21 06:38:23.000000 Giraffe_View-0.0.9.2/Giraffe_View.egg-info/requires.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       13 2023-07-21 06:38:23.000000 Giraffe_View-0.0.9.2/Giraffe_View.egg-info/top_level.txt
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     1064 2023-07-18 10:44:57.000000 Giraffe_View-0.0.9.2/LICENSE
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5057 2023-07-21 06:38:23.269874 Giraffe_View-0.0.9.2/PKG-INFO
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     4662 2023-07-21 06:12:03.000000 Giraffe_View-0.0.9.2/README.md
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       38 2023-07-21 06:38:23.269874 Giraffe_View-0.0.9.2/setup.cfg
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)      931 2023-07-21 06:18:35.000000 Giraffe_View-0.0.9.2/setup.py
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-21 10:04:50.670559 Giraffe_View-0.0.9.3/
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-21 10:04:50.670559 Giraffe_View-0.0.9.3/Giraffe_View/
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       57 2023-07-21 09:58:31.000000 Giraffe_View-0.0.9.3/Giraffe_View/__init__.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2835 2023-07-21 09:58:31.000000 Giraffe_View-0.0.9.3/Giraffe_View/estimated_read_accuracy.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4539 2023-07-21 09:58:31.000000 Giraffe_View-0.0.9.3/Giraffe_View/function.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3288 2023-07-21 09:58:31.000000 Giraffe_View-0.0.9.3/Giraffe_View/gc_bias.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4357 2023-07-21 09:58:31.000000 Giraffe_View-0.0.9.3/Giraffe_View/giraffe
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4721 2023-07-21 09:58:31.000000 Giraffe_View-0.0.9.3/Giraffe_View/homopolymer.py
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     2944 2023-07-21 09:58:31.000000 Giraffe_View-0.0.9.3/Giraffe_View/observed_read_accuracy.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4591 2023-07-21 09:57:39.000000 Giraffe_View-0.0.9.3/Giraffe_View/plot.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2156 2023-07-21 09:58:31.000000 Giraffe_View-0.0.9.3/Giraffe_View/regional_modification.py
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-21 10:04:50.670559 Giraffe_View-0.0.9.3/Giraffe_View.egg-info/
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5057 2023-07-21 10:04:50.000000 Giraffe_View-0.0.9.3/Giraffe_View.egg-info/PKG-INFO
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)      466 2023-07-21 10:04:50.000000 Giraffe_View-0.0.9.3/Giraffe_View.egg-info/SOURCES.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2023-07-21 10:04:50.000000 Giraffe_View-0.0.9.3/Giraffe_View.egg-info/dependency_links.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       71 2023-07-21 10:04:50.000000 Giraffe_View-0.0.9.3/Giraffe_View.egg-info/requires.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       13 2023-07-21 10:04:50.000000 Giraffe_View-0.0.9.3/Giraffe_View.egg-info/top_level.txt
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     1064 2023-07-21 09:58:42.000000 Giraffe_View-0.0.9.3/LICENSE
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5057 2023-07-21 10:04:50.670559 Giraffe_View-0.0.9.3/PKG-INFO
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     4662 2023-07-21 09:58:42.000000 Giraffe_View-0.0.9.3/README.md
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       38 2023-07-21 10:04:50.670559 Giraffe_View-0.0.9.3/setup.cfg
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)      940 2023-07-21 09:59:40.000000 Giraffe_View-0.0.9.3/setup.py
```

### Comparing `Giraffe_View-0.0.9.2/Giraffe_View/estimated_read_accuracy.py` & `Giraffe_View-0.0.9.3/Giraffe_View/estimated_read_accuracy.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.2/Giraffe_View/function.py` & `Giraffe_View-0.0.9.3/Giraffe_View/function.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.2/Giraffe_View/gc_bias.py` & `Giraffe_View-0.0.9.3/Giraffe_View/gc_bias.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.2/Giraffe_View/giraffe` & `Giraffe_View-0.0.9.3/Giraffe_View/giraffe`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.2/Giraffe_View/homopolymer.py` & `Giraffe_View-0.0.9.3/Giraffe_View/homopolymer.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.2/Giraffe_View/observed_read_accuracy.py` & `Giraffe_View-0.0.9.3/Giraffe_View/observed_read_accuracy.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.2/Giraffe_View/regional_modification.py` & `Giraffe_View-0.0.9.3/Giraffe_View/regional_modification.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.2/Giraffe_View.egg-info/PKG-INFO` & `Giraffe_View-0.0.9.3/Giraffe_View.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Giraffe-View
-Version: 0.0.9.2
+Version: 0.0.9.3
 Summary: A small tool help assess and visualize the accuracy of a sequencing dataset,   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.
 Home-page: https://github.com/lxd98/Giraffe_View
 Author: Xudong Liu
 Author-email: xudongliu98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Giraffe_View-0.0.9.2/LICENSE` & `Giraffe_View-0.0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.2/PKG-INFO` & `Giraffe_View-0.0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Giraffe_View
-Version: 0.0.9.2
+Version: 0.0.9.3
 Summary: A small tool help assess and visualize the accuracy of a sequencing dataset,   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.
 Home-page: https://github.com/lxd98/Giraffe_View
 Author: Xudong Liu
 Author-email: xudongliu98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Giraffe_View-0.0.9.2/README.md` & `Giraffe_View-0.0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.2/setup.py` & `Giraffe_View-0.0.9.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="Giraffe_View",
-  version="0.0.9.2",
+  version="0.0.9.3",
   author="Xudong Liu",
   author_email="xudongliu98@gmail.com",
   description="A small tool help assess and visualize the accuracy of a sequencing dataset, \
   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/lxd98/Giraffe_View",
@@ -18,14 +18,14 @@
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   ],
   python_requires = '>=3.7, <=3.10',
   install_requires=[
   'pysam >= 0.17.0',
-  'rpy2==3.0',
+  'plotnine >= 0.12.1',
   'numpy >= 1.7.0',
   'pandas >= 1.5.0',
   'tqdm == 4.64.0'
   ],
   scripts = ["Giraffe_View/giraffe"]
 )
```

