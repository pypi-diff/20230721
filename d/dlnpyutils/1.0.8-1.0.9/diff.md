# Comparing `tmp/dlnpyutils-1.0.8.tar.gz` & `tmp/dlnpyutils-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dlnpyutils-1.0.8.tar", last modified: Tue Nov 30 03:52:47 2021, max compression
+gzip compressed data, was "dist/dlnpyutils-1.0.9.tar", last modified: Tue Nov 30 03:56:39 2021, max compression
```

## Comparing `dlnpyutils-1.0.8.tar` & `dlnpyutils-1.0.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 nidever    (503) staff       (20)        0 2021-11-30 03:52:47.000000 dlnpyutils-1.0.8/
--rw-r--r--   0 nidever    (503) staff       (20)    18092 2021-07-11 02:58:32.000000 dlnpyutils-1.0.8/LICENSE
--rw-r--r--   0 nidever    (503) staff       (20)       32 2021-09-28 22:46:23.000000 dlnpyutils-1.0.8/MANIFEST.in
--rw-r--r--   0 nidever    (503) staff       (20)     1410 2021-11-30 03:52:47.000000 dlnpyutils-1.0.8/PKG-INFO
--rw-r--r--   0 nidever    (503) staff       (20)      758 2021-09-28 22:46:09.000000 dlnpyutils-1.0.8/README.rst
-drwxr-xr-x   0 nidever    (503) staff       (20)        0 2021-11-30 03:52:47.000000 dlnpyutils-1.0.8/bin/
--rwxr-xr-x   0 nidever    (503) staff       (20)     6942 2021-11-15 21:37:05.000000 dlnpyutils-1.0.8/bin/bump
--rwxr-xr-x   0 nidever    (503) staff       (20)     1903 2019-04-05 04:01:00.000000 dlnpyutils-1.0.8/bin/job_daemon
--rwxr-xr-x   0 nidever    (503) staff       (20)      903 2021-11-17 00:12:06.000000 dlnpyutils-1.0.8/bin/topypi
-drwxr-xr-x   0 nidever    (503) staff       (20)        0 2021-11-30 03:52:47.000000 dlnpyutils-1.0.8/dlnpyutils/
--rw-r--r--   0 nidever    (503) staff       (20)      197 2021-11-30 03:52:43.000000 dlnpyutils-1.0.8/dlnpyutils/__init__.py
--rw-r--r--   0 nidever    (503) staff       (20)    15033 2021-10-28 18:06:50.000000 dlnpyutils-1.0.8/dlnpyutils/astro.py
--rw-r--r--   0 nidever    (503) staff       (20)    31584 2021-06-05 20:19:46.000000 dlnpyutils-1.0.8/dlnpyutils/bindata.py
--rw-r--r--   0 nidever    (503) staff       (20)    21821 2021-10-28 18:06:59.000000 dlnpyutils-1.0.8/dlnpyutils/coords.py
--rw-r--r--   0 nidever    (503) staff       (20)     5024 2020-06-03 15:27:50.000000 dlnpyutils-1.0.8/dlnpyutils/db.py
--rw-r--r--   0 nidever    (503) staff       (20)    12214 2021-10-28 18:14:00.000000 dlnpyutils-1.0.8/dlnpyutils/galaxy_model.py
--rw-r--r--   0 nidever    (503) staff       (20)     1836 2019-07-19 20:15:09.000000 dlnpyutils-1.0.8/dlnpyutils/gaps.py
--rwxr-xr-x   0 nidever    (503) staff       (20)    24772 2021-10-28 18:07:44.000000 dlnpyutils-1.0.8/dlnpyutils/job_daemon.py
--rw-r--r--   0 nidever    (503) staff       (20)     5569 2021-10-28 18:06:38.000000 dlnpyutils-1.0.8/dlnpyutils/ladfit.py
--rw-r--r--   0 nidever    (503) staff       (20)    38335 2021-06-04 03:09:13.000000 dlnpyutils-1.0.8/dlnpyutils/least_squares.py
--rw-r--r--   0 nidever    (503) staff       (20)    34308 2021-02-16 19:34:42.000000 dlnpyutils-1.0.8/dlnpyutils/minpack.py
--rw-r--r--   0 nidever    (503) staff       (20)    20850 2021-02-16 19:31:23.000000 dlnpyutils-1.0.8/dlnpyutils/mpcommon.py
--rw-r--r--   0 nidever    (503) staff       (20)    13255 2021-10-28 18:08:00.000000 dlnpyutils-1.0.8/dlnpyutils/plotting.py
--rw-r--r--   0 nidever    (503) staff       (20)    20091 2021-07-11 02:54:57.000000 dlnpyutils-1.0.8/dlnpyutils/robust.py
--rw-r--r--   0 nidever    (503) staff       (20)     7050 2020-04-28 16:51:50.000000 dlnpyutils-1.0.8/dlnpyutils/spec.py
--rw-r--r--   0 nidever    (503) staff       (20)    19975 2021-06-04 03:08:48.000000 dlnpyutils-1.0.8/dlnpyutils/trf.py
--rw-r--r--   0 nidever    (503) staff       (20)    66677 2021-11-30 03:52:22.000000 dlnpyutils-1.0.8/dlnpyutils/utils.py
-drwxr-xr-x   0 nidever    (503) staff       (20)        0 2021-11-30 03:52:47.000000 dlnpyutils-1.0.8/dlnpyutils.egg-info/
--rw-r--r--   0 nidever    (503) staff       (20)     1410 2021-11-30 03:52:47.000000 dlnpyutils-1.0.8/dlnpyutils.egg-info/PKG-INFO
--rw-r--r--   0 nidever    (503) staff       (20)      890 2021-11-30 03:52:47.000000 dlnpyutils-1.0.8/dlnpyutils.egg-info/SOURCES.txt
--rw-r--r--   0 nidever    (503) staff       (20)        1 2021-11-30 03:52:47.000000 dlnpyutils-1.0.8/dlnpyutils.egg-info/dependency_links.txt
--rw-r--r--   0 nidever    (503) staff       (20)        1 2021-11-30 03:52:47.000000 dlnpyutils-1.0.8/dlnpyutils.egg-info/not-zip-safe
--rw-r--r--   0 nidever    (503) staff       (20)      133 2021-11-30 03:52:47.000000 dlnpyutils-1.0.8/dlnpyutils.egg-info/requires.txt
--rw-r--r--   0 nidever    (503) staff       (20)       11 2021-11-30 03:52:47.000000 dlnpyutils-1.0.8/dlnpyutils.egg-info/top_level.txt
-drwxr-xr-x   0 nidever    (503) staff       (20)        0 2021-11-30 03:52:47.000000 dlnpyutils-1.0.8/docs/
--rw-r--r--   0 nidever    (503) staff       (20)      634 2021-06-04 00:23:25.000000 dlnpyutils-1.0.8/docs/Makefile
-drwxr-xr-x   0 nidever    (503) staff       (20)        0 2021-11-30 03:52:47.000000 dlnpyutils-1.0.8/docs/_static/
--rw-r--r--   0 nidever    (503) staff       (20)      331 2021-06-04 00:24:28.000000 dlnpyutils-1.0.8/docs/_static/dlnpyutils.css
--rw-r--r--   0 nidever    (503) staff       (20)     8022 2021-09-29 20:43:04.000000 dlnpyutils-1.0.8/docs/conf.py
--rw-r--r--   0 nidever    (503) staff       (20)    10143 2021-10-07 22:16:13.000000 dlnpyutils-1.0.8/docs/description.rst
--rw-r--r--   0 nidever    (503) staff       (20)     2453 2021-09-28 22:55:14.000000 dlnpyutils-1.0.8/docs/dlnpyutils.rst
--rw-r--r--   0 nidever    (503) staff       (20)      583 2021-09-29 20:48:47.000000 dlnpyutils-1.0.8/docs/index.rst
--rw-r--r--   0 nidever    (503) staff       (20)      421 2021-09-28 22:49:46.000000 dlnpyutils-1.0.8/docs/install.rst
--rw-r--r--   0 nidever    (503) staff       (20)      795 2021-06-04 00:23:25.000000 dlnpyutils-1.0.8/docs/make.bat
--rw-r--r--   0 nidever    (503) staff       (20)       67 2021-09-28 22:55:14.000000 dlnpyutils-1.0.8/docs/modules.rst
--rw-r--r--   0 nidever    (503) staff       (20)       69 2021-06-04 00:23:25.000000 dlnpyutils-1.0.8/docs/requirements.txt
--rw-r--r--   0 nidever    (503) staff       (20)      149 2021-09-28 22:42:20.000000 dlnpyutils-1.0.8/environment.yml
--rw-r--r--   0 nidever    (503) staff       (20)       49 2021-09-28 22:42:25.000000 dlnpyutils-1.0.8/requirements-dev.txt
--rw-r--r--   0 nidever    (503) staff       (20)       31 2021-09-28 22:47:40.000000 dlnpyutils-1.0.8/requirements.txt
--rw-r--r--   0 nidever    (503) staff       (20)     1164 2021-11-30 03:52:47.000000 dlnpyutils-1.0.8/setup.cfg
--rw-r--r--   0 nidever    (503) staff       (20)      477 2021-11-30 03:52:46.000000 dlnpyutils-1.0.8/setup.py
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2021-11-30 03:56:39.000000 dlnpyutils-1.0.9/
+-rw-r--r--   0 nidever    (503) staff       (20)    18092 2021-07-11 02:58:32.000000 dlnpyutils-1.0.9/LICENSE
+-rw-r--r--   0 nidever    (503) staff       (20)       32 2021-09-28 22:46:23.000000 dlnpyutils-1.0.9/MANIFEST.in
+-rw-r--r--   0 nidever    (503) staff       (20)     1410 2021-11-30 03:56:39.000000 dlnpyutils-1.0.9/PKG-INFO
+-rw-r--r--   0 nidever    (503) staff       (20)      758 2021-09-28 22:46:09.000000 dlnpyutils-1.0.9/README.rst
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2021-11-30 03:56:39.000000 dlnpyutils-1.0.9/bin/
+-rwxr-xr-x   0 nidever    (503) staff       (20)     6942 2021-11-15 21:37:05.000000 dlnpyutils-1.0.9/bin/bump
+-rwxr-xr-x   0 nidever    (503) staff       (20)     1903 2019-04-05 04:01:00.000000 dlnpyutils-1.0.9/bin/job_daemon
+-rwxr-xr-x   0 nidever    (503) staff       (20)      903 2021-11-17 00:12:06.000000 dlnpyutils-1.0.9/bin/topypi
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2021-11-30 03:56:39.000000 dlnpyutils-1.0.9/dlnpyutils/
+-rw-r--r--   0 nidever    (503) staff       (20)      197 2021-11-30 03:56:32.000000 dlnpyutils-1.0.9/dlnpyutils/__init__.py
+-rw-r--r--   0 nidever    (503) staff       (20)    15033 2021-10-28 18:06:50.000000 dlnpyutils-1.0.9/dlnpyutils/astro.py
+-rw-r--r--   0 nidever    (503) staff       (20)    31584 2021-06-05 20:19:46.000000 dlnpyutils-1.0.9/dlnpyutils/bindata.py
+-rw-r--r--   0 nidever    (503) staff       (20)    21821 2021-10-28 18:06:59.000000 dlnpyutils-1.0.9/dlnpyutils/coords.py
+-rw-r--r--   0 nidever    (503) staff       (20)     5024 2020-06-03 15:27:50.000000 dlnpyutils-1.0.9/dlnpyutils/db.py
+-rw-r--r--   0 nidever    (503) staff       (20)    12214 2021-10-28 18:14:00.000000 dlnpyutils-1.0.9/dlnpyutils/galaxy_model.py
+-rw-r--r--   0 nidever    (503) staff       (20)     1836 2019-07-19 20:15:09.000000 dlnpyutils-1.0.9/dlnpyutils/gaps.py
+-rwxr-xr-x   0 nidever    (503) staff       (20)    24772 2021-10-28 18:07:44.000000 dlnpyutils-1.0.9/dlnpyutils/job_daemon.py
+-rw-r--r--   0 nidever    (503) staff       (20)     5569 2021-10-28 18:06:38.000000 dlnpyutils-1.0.9/dlnpyutils/ladfit.py
+-rw-r--r--   0 nidever    (503) staff       (20)    38335 2021-06-04 03:09:13.000000 dlnpyutils-1.0.9/dlnpyutils/least_squares.py
+-rw-r--r--   0 nidever    (503) staff       (20)    34308 2021-02-16 19:34:42.000000 dlnpyutils-1.0.9/dlnpyutils/minpack.py
+-rw-r--r--   0 nidever    (503) staff       (20)    20850 2021-02-16 19:31:23.000000 dlnpyutils-1.0.9/dlnpyutils/mpcommon.py
+-rw-r--r--   0 nidever    (503) staff       (20)    13255 2021-10-28 18:08:00.000000 dlnpyutils-1.0.9/dlnpyutils/plotting.py
+-rw-r--r--   0 nidever    (503) staff       (20)    20091 2021-07-11 02:54:57.000000 dlnpyutils-1.0.9/dlnpyutils/robust.py
+-rw-r--r--   0 nidever    (503) staff       (20)     7050 2020-04-28 16:51:50.000000 dlnpyutils-1.0.9/dlnpyutils/spec.py
+-rw-r--r--   0 nidever    (503) staff       (20)    19975 2021-06-04 03:08:48.000000 dlnpyutils-1.0.9/dlnpyutils/trf.py
+-rw-r--r--   0 nidever    (503) staff       (20)    66677 2021-11-30 03:54:25.000000 dlnpyutils-1.0.9/dlnpyutils/utils.py
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2021-11-30 03:56:39.000000 dlnpyutils-1.0.9/dlnpyutils.egg-info/
+-rw-r--r--   0 nidever    (503) staff       (20)     1410 2021-11-30 03:56:39.000000 dlnpyutils-1.0.9/dlnpyutils.egg-info/PKG-INFO
+-rw-r--r--   0 nidever    (503) staff       (20)      890 2021-11-30 03:56:39.000000 dlnpyutils-1.0.9/dlnpyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 nidever    (503) staff       (20)        1 2021-11-30 03:56:39.000000 dlnpyutils-1.0.9/dlnpyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 nidever    (503) staff       (20)        1 2021-11-30 03:56:39.000000 dlnpyutils-1.0.9/dlnpyutils.egg-info/not-zip-safe
+-rw-r--r--   0 nidever    (503) staff       (20)      133 2021-11-30 03:56:39.000000 dlnpyutils-1.0.9/dlnpyutils.egg-info/requires.txt
+-rw-r--r--   0 nidever    (503) staff       (20)       11 2021-11-30 03:56:39.000000 dlnpyutils-1.0.9/dlnpyutils.egg-info/top_level.txt
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2021-11-30 03:56:39.000000 dlnpyutils-1.0.9/docs/
+-rw-r--r--   0 nidever    (503) staff       (20)      634 2021-06-04 00:23:25.000000 dlnpyutils-1.0.9/docs/Makefile
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2021-11-30 03:56:39.000000 dlnpyutils-1.0.9/docs/_static/
+-rw-r--r--   0 nidever    (503) staff       (20)      331 2021-06-04 00:24:28.000000 dlnpyutils-1.0.9/docs/_static/dlnpyutils.css
+-rw-r--r--   0 nidever    (503) staff       (20)     8022 2021-09-29 20:43:04.000000 dlnpyutils-1.0.9/docs/conf.py
+-rw-r--r--   0 nidever    (503) staff       (20)    10143 2021-10-07 22:16:13.000000 dlnpyutils-1.0.9/docs/description.rst
+-rw-r--r--   0 nidever    (503) staff       (20)     2453 2021-09-28 22:55:14.000000 dlnpyutils-1.0.9/docs/dlnpyutils.rst
+-rw-r--r--   0 nidever    (503) staff       (20)      583 2021-09-29 20:48:47.000000 dlnpyutils-1.0.9/docs/index.rst
+-rw-r--r--   0 nidever    (503) staff       (20)      421 2021-09-28 22:49:46.000000 dlnpyutils-1.0.9/docs/install.rst
+-rw-r--r--   0 nidever    (503) staff       (20)      795 2021-06-04 00:23:25.000000 dlnpyutils-1.0.9/docs/make.bat
+-rw-r--r--   0 nidever    (503) staff       (20)       67 2021-09-28 22:55:14.000000 dlnpyutils-1.0.9/docs/modules.rst
+-rw-r--r--   0 nidever    (503) staff       (20)       69 2021-06-04 00:23:25.000000 dlnpyutils-1.0.9/docs/requirements.txt
+-rw-r--r--   0 nidever    (503) staff       (20)      149 2021-09-28 22:42:20.000000 dlnpyutils-1.0.9/environment.yml
+-rw-r--r--   0 nidever    (503) staff       (20)       49 2021-09-28 22:42:25.000000 dlnpyutils-1.0.9/requirements-dev.txt
+-rw-r--r--   0 nidever    (503) staff       (20)       31 2021-09-28 22:47:40.000000 dlnpyutils-1.0.9/requirements.txt
+-rw-r--r--   0 nidever    (503) staff       (20)     1164 2021-11-30 03:56:39.000000 dlnpyutils-1.0.9/setup.cfg
+-rw-r--r--   0 nidever    (503) staff       (20)      477 2021-11-30 03:56:38.000000 dlnpyutils-1.0.9/setup.py
```

### Comparing `dlnpyutils-1.0.8/LICENSE` & `dlnpyutils-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/PKG-INFO` & `dlnpyutils-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlnpyutils
-Version: 1.0.8
+Version: 1.0.9
 Summary: David Nidever Python Utility Functions
 Home-page: https://github.com/dnidever/dlnpyutils
 Author: David Nidever
 Author-email: dnidever@montana.edu
 License: GNU
 Description: 
         dlnpyutils
```

### Comparing `dlnpyutils-1.0.8/README.rst` & `dlnpyutils-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/bin/bump` & `dlnpyutils-1.0.9/bin/bump`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/bin/job_daemon` & `dlnpyutils-1.0.9/bin/job_daemon`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/bin/topypi` & `dlnpyutils-1.0.9/bin/topypi`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/dlnpyutils/astro.py` & `dlnpyutils-1.0.9/dlnpyutils/astro.py`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/dlnpyutils/bindata.py` & `dlnpyutils-1.0.9/dlnpyutils/bindata.py`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/dlnpyutils/coords.py` & `dlnpyutils-1.0.9/dlnpyutils/coords.py`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/dlnpyutils/db.py` & `dlnpyutils-1.0.9/dlnpyutils/db.py`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/dlnpyutils/galaxy_model.py` & `dlnpyutils-1.0.9/dlnpyutils/galaxy_model.py`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/dlnpyutils/gaps.py` & `dlnpyutils-1.0.9/dlnpyutils/gaps.py`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/dlnpyutils/job_daemon.py` & `dlnpyutils-1.0.9/dlnpyutils/job_daemon.py`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/dlnpyutils/ladfit.py` & `dlnpyutils-1.0.9/dlnpyutils/ladfit.py`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/dlnpyutils/least_squares.py` & `dlnpyutils-1.0.9/dlnpyutils/least_squares.py`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/dlnpyutils/minpack.py` & `dlnpyutils-1.0.9/dlnpyutils/minpack.py`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/dlnpyutils/mpcommon.py` & `dlnpyutils-1.0.9/dlnpyutils/mpcommon.py`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/dlnpyutils/plotting.py` & `dlnpyutils-1.0.9/dlnpyutils/plotting.py`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/dlnpyutils/robust.py` & `dlnpyutils-1.0.9/dlnpyutils/robust.py`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/dlnpyutils/spec.py` & `dlnpyutils-1.0.9/dlnpyutils/spec.py`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/dlnpyutils/trf.py` & `dlnpyutils-1.0.9/dlnpyutils/trf.py`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/dlnpyutils/utils.py` & `dlnpyutils-1.0.9/dlnpyutils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -933,15 +933,15 @@
     x1 = np.median(xx[si[0:nq]])
     y1 = np.median(yy[si[0:nq]])
     slp34 = (yy[si[nh:]]-y1)/(xx[si[nh:]]-x1)
     # Fourth quartile median X/Y values    
     x4 = np.median(xx[si[-nq:]])
     y4 = np.median(yy[si[-nq:]])
     slp12 = (yy[si[0:nh]]-y4)/(xx[si[0:nh]]-x4)
-    allslp = np.vstack((slp12,slp34))
+    allslp = np.hstack((slp12,slp34))
     slp = np.median(allslp)
     return slp    
 
     
 def iqrslope(x,y):
     """ Calculate robust slope using median X/Y values of first quartile
          and last quartile points."""
```

### Comparing `dlnpyutils-1.0.8/dlnpyutils.egg-info/PKG-INFO` & `dlnpyutils-1.0.9/dlnpyutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlnpyutils
-Version: 1.0.8
+Version: 1.0.9
 Summary: David Nidever Python Utility Functions
 Home-page: https://github.com/dnidever/dlnpyutils
 Author: David Nidever
 Author-email: dnidever@montana.edu
 License: GNU
 Description: 
         dlnpyutils
```

### Comparing `dlnpyutils-1.0.8/dlnpyutils.egg-info/SOURCES.txt` & `dlnpyutils-1.0.9/dlnpyutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/docs/Makefile` & `dlnpyutils-1.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/docs/conf.py` & `dlnpyutils-1.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/docs/description.rst` & `dlnpyutils-1.0.9/docs/description.rst`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/docs/dlnpyutils.rst` & `dlnpyutils-1.0.9/docs/dlnpyutils.rst`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/docs/index.rst` & `dlnpyutils-1.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/docs/make.bat` & `dlnpyutils-1.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dlnpyutils-1.0.8/setup.cfg` & `dlnpyutils-1.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 license_file = LICENSE
 url = https://github.com/dnidever/dlnpyutils
 description = A package of useful python utility functions.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 edit_on_github = False
 github_project = dnidever/dlnpyutils
-version = 1.0.8
+version = 1.0.9
 
 [options]
 zip_safe = False
 packages = find:
 python_requires = >=3.6
 setup_requires = 
 	setuptools_scm
```

