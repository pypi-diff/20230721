# Comparing `tmp/element-miniscope-0.3.1.tar.gz` & `tmp/element-miniscope-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-miniscope-0.3.1.tar", last modified: Fri May 26 19:36:57 2023, max compression
+gzip compressed data, was "element-miniscope-0.3.2.tar", last modified: Thu Jul 20 22:29:14 2023, max compression
```

## Comparing `element-miniscope-0.3.1.tar` & `element-miniscope-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:36:57.175881 element-miniscope-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 19:36:54.000000 element-miniscope-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-26 19:36:57.175881 element-miniscope-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-26 19:36:54.000000 element-miniscope-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:36:57.171882 element-miniscope-0.3.1/element_miniscope/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:36:54.000000 element-miniscope-0.3.1/element_miniscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46341 2023-05-26 19:36:54.000000 element-miniscope-0.3.1/element_miniscope/miniscope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-26 19:36:54.000000 element-miniscope-0.3.1/element_miniscope/miniscope_report.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-26 19:36:54.000000 element-miniscope-0.3.1/element_miniscope/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:36:57.175881 element-miniscope-0.3.1/element_miniscope.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-26 19:36:57.000000 element-miniscope-0.3.1/element_miniscope.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-26 19:36:57.000000 element-miniscope-0.3.1/element_miniscope.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:36:57.000000 element-miniscope-0.3.1/element_miniscope.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 19:36:57.000000 element-miniscope-0.3.1/element_miniscope.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 19:36:57.000000 element-miniscope-0.3.1/element_miniscope.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 19:36:57.175881 element-miniscope-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-26 19:36:54.000000 element-miniscope-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:29:14.342312 element-miniscope-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-20 22:29:11.000000 element-miniscope-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-20 22:29:14.342312 element-miniscope-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-20 22:29:11.000000 element-miniscope-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:29:14.342312 element-miniscope-0.3.2/element_miniscope/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:29:11.000000 element-miniscope-0.3.2/element_miniscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46341 2023-07-20 22:29:11.000000 element-miniscope-0.3.2/element_miniscope/miniscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-20 22:29:11.000000 element-miniscope-0.3.2/element_miniscope/miniscope_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-20 22:29:11.000000 element-miniscope-0.3.2/element_miniscope/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:29:14.342312 element-miniscope-0.3.2/element_miniscope.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-20 22:29:14.000000 element-miniscope-0.3.2/element_miniscope.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-20 22:29:14.000000 element-miniscope-0.3.2/element_miniscope.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 22:29:14.000000 element-miniscope-0.3.2/element_miniscope.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-20 22:29:14.000000 element-miniscope-0.3.2/element_miniscope.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 22:29:14.000000 element-miniscope-0.3.2/element_miniscope.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 22:29:14.342312 element-miniscope-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-20 22:29:11.000000 element-miniscope-0.3.2/setup.py
```

### Comparing `element-miniscope-0.3.1/LICENSE` & `element-miniscope-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `element-miniscope-0.3.1/PKG-INFO` & `element-miniscope-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-miniscope
-Version: 0.3.1
+Version: 0.3.2
 Summary: Miniscope DataJoint Element
 Home-page: https://github.com/datajoint/element-miniscope
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience calcium-imaging science datajoint miniscope
 Platform: UNKNOWN
```

### Comparing `element-miniscope-0.3.1/README.md` & `element-miniscope-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `element-miniscope-0.3.1/element_miniscope/miniscope.py` & `element-miniscope-0.3.2/element_miniscope/miniscope.py`

 * *Files identical despite different names*

### Comparing `element-miniscope-0.3.1/element_miniscope/miniscope_report.py` & `element-miniscope-0.3.2/element_miniscope/miniscope_report.py`

 * *Files identical despite different names*

### Comparing `element-miniscope-0.3.1/element_miniscope.egg-info/PKG-INFO` & `element-miniscope-0.3.2/element_miniscope.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-miniscope
-Version: 0.3.1
+Version: 0.3.2
 Summary: Miniscope DataJoint Element
 Home-page: https://github.com/datajoint/element-miniscope
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience calcium-imaging science datajoint miniscope
 Platform: UNKNOWN
```

### Comparing `element-miniscope-0.3.1/setup.py` & `element-miniscope-0.3.2/setup.py`

 * *Files identical despite different names*

