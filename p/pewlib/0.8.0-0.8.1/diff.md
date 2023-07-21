# Comparing `tmp/pewlib-0.8.0.tar.gz` & `tmp/pewlib-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pewlib-0.8.0.tar", last modified: Tue Jul 18 06:13:28 2023, max compression
+gzip compressed data, was "pewlib-0.8.1.tar", last modified: Fri Jul 21 07:18:40 2023, max compression
```

## Comparing `pewlib-0.8.0.tar` & `pewlib-0.8.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:13:28.666656 pewlib-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-18 06:13:08.000000 pewlib-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-18 06:13:28.666656 pewlib-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-18 06:13:08.000000 pewlib-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:13:28.658655 pewlib-0.8.0/pewlib/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:13:28.658655 pewlib-0.8.0/pewlib/io/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/io/agilent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/io/npz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/io/perkinelmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/io/textimage.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/io/thermo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/io/vtk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/laser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:13:28.662655 pewlib-0.8.0/pewlib/process/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/process/calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/process/colocal.py
--rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/process/convolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/process/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14654 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/process/peakfinding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/process/register.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/process/threshold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:13:28.662655 pewlib-0.8.0/pewlib/srr/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/srr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/srr/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/srr/srr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:13:28.658655 pewlib-0.8.0/pewlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-18 06:13:28.000000 pewlib-0.8.0/pewlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 06:13:28.000000 pewlib-0.8.0/pewlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 06:13:28.000000 pewlib-0.8.0/pewlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-18 06:13:28.000000 pewlib-0.8.0/pewlib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 06:13:28.000000 pewlib-0.8.0/pewlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 06:13:28.000000 pewlib-0.8.0/pewlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 06:13:28.666656 pewlib-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-18 06:13:08.000000 pewlib-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:13:28.662655 pewlib-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_colocal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_convolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_io_agilent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_io_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_io_thermo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_laser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_peakfinding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_srr.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:18:40.528747 pewlib-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 07:18:25.000000 pewlib-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-21 07:18:40.528747 pewlib-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-21 07:18:25.000000 pewlib-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:18:40.508747 pewlib-0.8.1/pewlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:18:40.516747 pewlib-0.8.1/pewlib/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/io/agilent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/io/npz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/io/perkinelmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/io/textimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/io/thermo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/io/vtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/laser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:18:40.520747 pewlib-0.8.1/pewlib/process/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/process/calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/process/colocal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/process/convolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/process/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14654 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/process/peakfinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/process/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/process/threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:18:40.520747 pewlib-0.8.1/pewlib/srr/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/srr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/srr/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/srr/srr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:18:40.512747 pewlib-0.8.1/pewlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-21 07:18:40.000000 pewlib-0.8.1/pewlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-21 07:18:40.000000 pewlib-0.8.1/pewlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:18:40.000000 pewlib-0.8.1/pewlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-21 07:18:40.000000 pewlib-0.8.1/pewlib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 07:18:40.000000 pewlib-0.8.1/pewlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-21 07:18:40.000000 pewlib-0.8.1/pewlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 07:18:40.528747 pewlib-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-21 07:18:25.000000 pewlib-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:18:40.528747 pewlib-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_colocal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_convolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_io_agilent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_io_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_io_thermo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_laser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_peakfinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_srr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_threshold.py
```

### Comparing `pewlib-0.8.0/LICENSE` & `pewlib-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/PKG-INFO` & `pewlib-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pewlib
-Version: 0.8.0
+Version: 0.8.1
 Summary: Import, processing and export library for LA-ICP-MS data.
 Home-page: https://github.com/djdt/pewlib
 Author: T. Lockwood
 Author-email: thomas.lockwood@uts.edu.au
 Project-URL: Documentation, https://djdt.github.io/pewlib
 Project-URL: Source, https://gtihub.com/djdt/pewlib
 Description-Content-Type: text/markdown
```

### Comparing `pewlib-0.8.0/pewlib/__main__.py` & `pewlib-0.8.1/pewlib/__main__.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/pewlib/calibration.py` & `pewlib-0.8.1/pewlib/calibration.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/pewlib/config.py` & `pewlib-0.8.1/pewlib/config.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/pewlib/io/agilent.py` & `pewlib-0.8.1/pewlib/io/agilent.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/pewlib/io/csv.py` & `pewlib-0.8.1/pewlib/io/csv.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/pewlib/io/npz.py` & `pewlib-0.8.1/pewlib/io/npz.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/pewlib/io/perkinelmer.py` & `pewlib-0.8.1/pewlib/io/perkinelmer.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/pewlib/io/textimage.py` & `pewlib-0.8.1/pewlib/io/textimage.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/pewlib/io/thermo.py` & `pewlib-0.8.1/pewlib/io/thermo.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/pewlib/io/vtk.py` & `pewlib-0.8.1/pewlib/io/vtk.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/pewlib/laser.py` & `pewlib-0.8.1/pewlib/laser.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/pewlib/process/calc.py` & `pewlib-0.8.1/pewlib/process/calc.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/pewlib/process/colocal.py` & `pewlib-0.8.1/pewlib/process/colocal.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/pewlib/process/convolve.py` & `pewlib-0.8.1/pewlib/process/convolve.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/pewlib/process/filters.py` & `pewlib-0.8.1/pewlib/process/filters.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/pewlib/process/peakfinding.py` & `pewlib-0.8.1/pewlib/process/peakfinding.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/pewlib/process/register.py` & `pewlib-0.8.1/pewlib/process/register.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Module for registering and merging images."""
 
-import numpy as np
+from typing import Iterable, List, Tuple
 
-from typing import Iterable, Tuple
+import numpy as np
+import numpy.lib.recfunctions as rfn
 
 
 def anchor_offset(a: np.ndarray, b: np.ndarray, anchor: str) -> Tuple[int, int]:
     """Return offset of `b` from `a` given a common achor point.
 
     Both `a` and `b` must be 2d arrays.
     Valid anchors are 'top left', 'top right', 'bottom left', 'bottom right' or 'center'.
@@ -55,156 +56,118 @@
     xcorr = np.fft.irfftn(np.fft.rfftn(a) * np.fft.rfftn(b).conj())
     xcorr = np.fft.fftshift(xcorr)
 
     return np.unravel_index(np.argmax(xcorr), xcorr.shape) - np.array(xcorr.shape) // 2
 
 
 def overlap_arrays(
-    a: np.ndarray,
-    b: np.ndarray,
-    offset: Iterable[int],
+    arrays: List[np.ndarray],
+    offsets: List[Iterable[int]],
     fill: float = np.nan,
     mode: str = "replace",
 ) -> np.ndarray:
     """Merges two arrays by enlarging.
 
-    Coordinates (0, 0) of array `b` will be at `offset` in the new array.
-    Non-overlapping areas are filled with `fill`.
-    Overlapped values are calculated using `mode`. Mode 'replace' will use values in `b`,
-    'mean' and 'sum' uses the mean and sum of `a` and `b` respectively.
+    Creates a new array from `arrays` by positioning each array at its respective,
+    simplified offset from `offsets`. Non-overlapping areas are filled with `fill`.
+    Overlapped values are calculated using `mode`. Mode 'replace' will replace
+    values with those last in `array`, 'mean' and 'sum' uses the mean and sum of
+    `arrays` respectively.
 
     Args:
-        a: ndim array
-        b: ndim array
-        offset: offset for 'b', any int
+        arrays: list of arrays
+        offsets: offset for each array
         fill: value for non-overlapping areas
         mode: value for overlapped areas, {'replace', 'mean', 'sum'}
 
     Returns:
-        new overlapped array, same dtype as 'a'
+        new overlapped array, same dtype as arrays[0]
 
     Example
     -------
 
     >>> import numpy as np
     >>> from pewlib.process import register
     >>> a = np.arange(9.0).reshape(3, 3)
     >>> b = np.arange(9.0).reshape(3, 3)
-    >>> c = register.overlap_arrays(a, b, fill=0, mode="sum")
+    >>> c = register.overlap_arrays([a, b], [(0, 0), (2, 2)], fill=0, mode="sum")
 
 
     .. plot::
 
         import numpy as np
         from pewlib.process import register
         import matplotlib.pyplot as plt
-        c = register.overlap_arrays(np.arange(9.0).reshape(3, 3), np.arange(9.0).reshape(3, 3), fill=0, mode="sum")
+        c = register.overlap_arrays(
+            [np.arange(9.0).reshape(3, 3), np.arange(9.0).reshape(3, 3)],
+            [(0, 0), (2, 2)], fill=0, mode="sum"
+        )
 
         plt.imshow(c)
         plt.show()
     """
 
-    if a.ndim != b.ndim:  # pragma: no cover
-        raise ValueError(
-            f"Arrays 'a' and 'b' must have the same dimensions, {a.ndim} != {b.ndim}."
-        )
+    if not all(a.ndim == arrays[0].ndim for a in arrays):  # pragma: no cover
+        raise ValueError("Arrays must have the same dimensions.")
 
-    offset = np.array(offset, dtype=int)
-    if offset.size != a.ndim:  # pragma: no cover
-        raise ValueError("Offset must have same dimensions as arrays.")
-
-    if mode not in ["replace", "mean", "sum"]:  # pragma: no cover
-        raise ValueError("'mode' must be 'replace', 'mean' or 'sum'.")
-
-    # find the max / min extents of the new array
-    new_shape = np.maximum(a.shape, offset + b.shape) - np.minimum(0, offset)
-    c = np.full(new_shape, fill, dtype=a.dtype)
-
-    # offsets for each array
-    aoffset = np.where(offset < 0, -offset, 0)
-    boffset = np.where(offset >= 0, offset, 0)
-    aslice = tuple(slice(o, o + s) for o, s in zip(aoffset, a.shape))
-    bslice = tuple(slice(o, o + s) for o, s in zip(boffset, b.shape))
-
-    # size and slice of overlapping area
-    abslice = tuple(
-        slice(max(a.start, b.start), min(a.stop, b.stop), None)
-        for a, b in zip(aslice, bslice)
+    min_offset = np.amin(offsets, axis=0)
+    offsets = [(offset - min_offset) for offset in offsets]
+    new_shape = np.amax(
+        [np.array(offset) + a.shape for offset, a in zip(offsets, arrays)], axis=0
     )
-    absize = tuple(s.stop - s.start for s in abslice)
-    hasoverlap = all(x > 0 for x in absize)
 
-    # sections of overlap from a, b
-    asec = tuple(slice(o, o + s) for o, s in zip(aoffset, absize))
-    bsec = tuple(slice(o, o + s) for o, s in zip(boffset, absize))
-
-    c[aslice] = a
-    c[bslice] = b
-
-    if mode == "replace":
-        pass
-    elif mode == "mean" and hasoverlap:
-        c[abslice] = np.nanmean([a[asec], b[bsec]], axis=0)
-    elif mode == "sum" and hasoverlap:
-        c[abslice] = np.nansum([a[asec], b[bsec]], axis=0)
+    overlap = np.full(new_shape, fill, dtype=arrays[0].dtype)
+    visits = np.zeros(new_shape, dtype=int)  # Track idx for mean calc
+    for i, (offset, array) in enumerate(zip(offsets, arrays)):
+        slice_idx = tuple(slice(o, o + s) for o, s in zip(offset, array.shape))
+        if mode == "replace":
+            nans = np.isnan(array)
+            overlap[slice_idx][~nans] = array[~nans]
+        elif mode == "mean" or mode == "sum":
+            overlap[slice_idx] = np.nansum([overlap[slice_idx], array], axis=0)
+        visits[slice_idx][~np.isnan(array)] += 1
 
-    return c
+    if mode == "mean":
+        overlap[visits > 1] /= visits[visits > 1]
+
+    return overlap
 
 
 def overlap_structured_arrays(
-    a: np.ndarray,
-    b: np.ndarray,
-    offset: Iterable[int],
+    arrays: List[np.ndarray],
+    offsets: List[Iterable[int]],
     fill: float = np.nan,
     mode: str = "replace",
 ) -> np.ndarray:
     """Merges two structured arrays by enlarging.
 
-    Coordinates (0, 0) of array `b` will be at `offset` in the new array.
-    Shared names in 'a' and 'b' are calculated using `mode` where overlap occurs.
+    Shared names in `arrays` are calculated using `mode` where overlap occurs.
 
     Args:
-        a: ndim array
-        b: ndim array
-        offset: offset for 'b'
+        arrays: list of arrays
+        offset: offset for each array
         fill: value for non-overlapping areas
         mode: value for overlapped areas, {'replace', 'mean', 'sum'}
 
     Returns:
         new overlapped array
 
     See Also:
         :func:`pewlib.process.register.overlap_arrays`
     """
-    offset = np.array(offset, dtype=int)
-    if offset.size != a.ndim:  # pragma: no cover
-        raise ValueError("Anchor must have same dimensions as arrays.")
-
-    # find the max / min extents of the new array
-    new_shape = np.maximum(a.shape, offset + b.shape) - np.minimum(0, offset)
-    new_dtype = list(a.dtype.descr)
-    new_dtype.extend([x for x in b.dtype.descr if x not in new_dtype])
+    min_offset = np.amin(offsets, axis=0)
+    offsets = [(offset - min_offset) for offset in offsets]
+    rfn.merge_arrays
+    new_shape = np.amax(
+        [np.array(offset) + a.shape for offset, a in zip(offsets, arrays)], axis=0
+    )
+    new_dtype = list(arrays[0].dtype.descr)
+    for array in arrays[1:]:
+        new_dtype.extend([x for x in array.dtype.descr if x not in new_dtype])
     c = np.empty(new_shape, dtype=new_dtype)
-
     for name in c.dtype.names:
-        if name not in b.dtype.names:
-            c[name] = overlap_arrays(
-                np.full(b.shape, fill),
-                a[name],
-                offset=-offset,
-                fill=fill,
-                mode="replace",
-            )
-        elif name not in a.dtype.names:
-            c[name] = overlap_arrays(
-                np.full(a.shape, fill),
-                b[name],
-                offset=offset,
-                fill=fill,
-                mode="replace",
-            )
-        else:
-            c[name] = overlap_arrays(
-                a[name], b[name], offset=offset, fill=fill, mode=mode
-            )
-
+        name_arrays = [
+            array[name] if name in array.dtype.names else np.full(array.shape, np.nan)
+            for array in arrays
+        ]
+        c[name] = overlap_arrays(name_arrays, offsets, fill=fill, mode=mode)
     return c
```

### Comparing `pewlib-0.8.0/pewlib/process/threshold.py` & `pewlib-0.8.1/pewlib/process/threshold.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/pewlib/srr/config.py` & `pewlib-0.8.1/pewlib/srr/config.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/pewlib/srr/srr.py` & `pewlib-0.8.1/pewlib/srr/srr.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/pewlib.egg-info/PKG-INFO` & `pewlib-0.8.1/pewlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pewlib
-Version: 0.8.0
+Version: 0.8.1
 Summary: Import, processing and export library for LA-ICP-MS data.
 Home-page: https://github.com/djdt/pewlib
 Author: T. Lockwood
 Author-email: thomas.lockwood@uts.edu.au
 Project-URL: Documentation, https://djdt.github.io/pewlib
 Project-URL: Source, https://gtihub.com/djdt/pewlib
 Description-Content-Type: text/markdown
```

### Comparing `pewlib-0.8.0/pewlib.egg-info/SOURCES.txt` & `pewlib-0.8.1/pewlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/setup.py` & `pewlib-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/tests/test_calc.py` & `pewlib-0.8.1/tests/test_calc.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/tests/test_calibration.py` & `pewlib-0.8.1/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/tests/test_colocal.py` & `pewlib-0.8.1/tests/test_colocal.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/tests/test_config.py` & `pewlib-0.8.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/tests/test_convolve.py` & `pewlib-0.8.1/tests/test_convolve.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/tests/test_filters.py` & `pewlib-0.8.1/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/tests/test_io.py` & `pewlib-0.8.1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/tests/test_io_agilent.py` & `pewlib-0.8.1/tests/test_io_agilent.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/tests/test_io_csv.py` & `pewlib-0.8.1/tests/test_io_csv.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/tests/test_io_thermo.py` & `pewlib-0.8.1/tests/test_io_thermo.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/tests/test_laser.py` & `pewlib-0.8.1/tests/test_laser.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/tests/test_peakfinding.py` & `pewlib-0.8.1/tests/test_peakfinding.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.0/tests/test_register.py` & `pewlib-0.8.1/tests/test_register.py`

 * *Files 26% similar despite different names*

```diff
@@ -45,60 +45,85 @@
     offset = register.fft_register_offset(a, b)
     assert np.all(offset == (-50, 0))
     offset = register.fft_register_offset(b, a)
     assert np.all(offset == (50, 0))
 
 
 def test_overlap_arrays():
-    a = np.arange(9.0).reshape(3, 3)
-    b = np.arange(9.0).reshape(3, 3)
+    a = np.ones((2, 2))
+    b = np.ones((2, 2)) * 2
+    c = np.ones((2, 2)) * 3
+
+    offsets = [(0, 0), (-1, 1), (0, 1)]
+    # _   b   b
+    # a   abc bc
+    # a   ac  c
 
     # Test overlap methods
-    c = register.overlap_arrays(a, b, offset=(1, 1), mode="replace")
-    assert c.shape == (4, 4)
-    assert np.isnan(c[0, 3])
-    assert np.isnan(c[3, 0])
-    assert np.all(c[~np.isnan(c)] == [0, 1, 2, 3, 0, 1, 2, 6, 3, 4, 5, 6, 7, 8])
-    c = register.overlap_arrays(a, b, offset=(1, 1), mode="mean")
-    assert np.all(c[~np.isnan(c)] == [0, 1, 2, 3, 2, 3, 2, 6, 5, 6, 5, 6, 7, 8])
-    c = register.overlap_arrays(a, b, offset=(1, 1), mode="sum")
-    assert np.all(c[~np.isnan(c)] == [0, 1, 2, 3, 4, 6, 2, 6, 10, 12, 5, 6, 7, 8])
-
-    # Test various offsets
-    for i in range(-5, 5):
-        for j in range(-5, 5):
-            c = register.overlap_arrays(a, b, offset=(i, j), mode="sum")
-            assert np.nansum(c) == 72.0
-
-    # Test non nan fill
-    c = register.overlap_arrays(a, b, offset=(-3, 0), fill=0.0, mode="replace")
-    assert np.all(c[:3] == b)
-    c = register.overlap_arrays(a, b, offset=(-3, 0), fill=0.0, mode="mean")
-    assert np.all(c[:3] == b)
-    c = register.overlap_arrays(a, b, offset=(-3, 0), fill=0.0, mode="sum")
-    assert np.all(c[:3] == b)
+    d = register.overlap_arrays([a, b, c], offsets=offsets, mode="replace")
+    assert d.shape == (3, 3)
+    assert np.isnan(d[0][0])
+    assert np.all(d[~np.isnan(d)] == [2, 2, 1, 3, 3, 1, 3, 3])
+
+    d = register.overlap_arrays([a, b, c], offsets=offsets, mode="mean")
+    assert np.all(d[~np.isnan(d)] == [2, 2, 1, 2, 2.5, 1, 2, 3])
+
+    d = register.overlap_arrays([a, b, c], offsets=offsets, mode="sum")
+    assert np.all(d[~np.isnan(d)] == [2, 2, 1, 6, 5, 1, 4, 3])
+
+    d = register.overlap_arrays([a, b, c], offsets=[(-1, -1), (2, 2), (-2, 2)], fill=10)
+    assert np.all(
+        d
+        == [
+            [10, 10, 10, 3, 3],
+            [1, 1, 10, 3, 3],
+            [1, 1, 10, 10, 10],
+            [10, 10, 10, 10, 10],
+            [10, 10, 10, 2, 2],
+            [10, 10, 10, 2, 2],
+        ]
+    )
+
+
+def test_overlap_arrays_nan():
+    a = np.ones((3, 3))
+    b = np.full_like(a, np.nan)
+
+    c = register.overlap_arrays([a, b], offsets=[(0, 0), (0, 0)])
+    assert np.all(c == 1.0)
+    c = register.overlap_arrays([a, b], offsets=[(0, 0), (0, 0)], mode="mean")
+    assert np.all(c == 1.0)
+    c = register.overlap_arrays([a, b], offsets=[(0, 0), (0, 0)], mode="sum")
+    assert np.all(c == 1.0)
 
 
 def test_overlap_structured_arrays():
-    a = np.empty((4, 4), dtype=[("a", float), ("c", float)])
-    a["a"].flat = np.arange(16.0)
-    a["c"].flat = np.arange(16.0)
-    b = np.empty((4, 4), dtype=[("b", float), ("c", float)])
-    b["b"].flat = np.arange(16.0)
-    b["c"] = 1.0
-
-    d = register.overlap_structured_arrays(a, b, offset=(2, 2), mode="replace")
-
-    # Test overlap methods
-    assert d.shape == (6, 6)
-    assert np.all(d["a"][:4, :4] == a["a"])
-    assert np.all(d["b"][2:, 2:] == b["b"])
-    assert np.all(d["c"][2:, 2:] == 1.0)
-    assert np.all(d["c"][:2, :2] == a["a"][:2, :2])
-
-    d = register.overlap_structured_arrays(a, b, offset=(2, 2), mode="mean")
-
-    # Test overlap methods
-    assert np.all(d["c"][2:4, 2:4] == np.mean([a["c"][:2, :2], b["c"][:2, :2]], axis=0))
-
-    d = register.overlap_structured_arrays(a, b, offset=(2, 2), mode="sum")
-    assert np.all(d["c"][2:4, 2:4] == np.sum([a["c"][:2, :2], b["c"][:2, :2]], axis=0))
+    a = np.empty((2, 2), dtype=[("a", float), ("c", float)])
+    b = np.empty((2, 2), dtype=[("b", float), ("c", float)])
+    a["a"] = 1
+    a["c"] = 2
+    b["b"] = 3
+    b["c"] = 4
+
+    c = register.overlap_structured_arrays([a, b], offsets=[(0, 0), (1, 1)])
+    assert c.shape == (3, 3)
+    assert c.dtype.names == ("a", "c", "b")
+
+    assert np.all(np.nan_to_num(c["a"]) == [[1, 1, 0], [1, 1, 0], [0, 0, 0]])
+    assert np.all(np.nan_to_num(c["b"]) == [[0, 0, 0], [0, 3, 3], [0, 3, 3]])
+    assert np.all(np.nan_to_num(c["c"]) == [[2, 2, 0], [2, 4, 4], [0, 4, 4]])
+
+    c = register.overlap_structured_arrays(
+        [a, b], offsets=[(0, 0), (1, 1)], mode="mean"
+    )
+
+    assert np.all(np.nan_to_num(c["a"]) == [[1, 1, 0], [1, 1, 0], [0, 0, 0]])
+    assert np.all(np.nan_to_num(c["b"]) == [[0, 0, 0], [0, 3, 3], [0, 3, 3]])
+    assert np.all(np.nan_to_num(c["c"]) == [[2, 2, 0], [2, 3, 4], [0, 4, 4]])
+
+    c = register.overlap_structured_arrays(
+        [a, b], offsets=[(0, 0), (1, 1)], mode="sum"
+    )
+
+    assert np.all(np.nan_to_num(c["a"]) == [[1, 1, 0], [1, 1, 0], [0, 0, 0]])
+    assert np.all(np.nan_to_num(c["b"]) == [[0, 0, 0], [0, 3, 3], [0, 3, 3]])
+    assert np.all(np.nan_to_num(c["c"]) == [[2, 2, 0], [2, 6, 4], [0, 4, 4]])
```

### Comparing `pewlib-0.8.0/tests/test_srr.py` & `pewlib-0.8.1/tests/test_srr.py`

 * *Files identical despite different names*

