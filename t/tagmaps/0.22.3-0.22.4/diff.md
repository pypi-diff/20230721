# Comparing `tmp/tagmaps-0.22.3.tar.gz` & `tmp/tagmaps-0.22.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tagmaps-0.22.3.tar", last modified: Mon Jul 17 11:24:34 2023, max compression
+gzip compressed data, was "tagmaps-0.22.4.tar", last modified: Fri Jul 21 09:31:09 2023, max compression
```

## Comparing `tagmaps-0.22.3.tar` & `tagmaps-0.22.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 11:24:34.908782 tagmaps-0.22.3/
--rw-r--r--   0 alex      (1000) alex      (1000)     8701 2023-07-17 11:23:47.000000 tagmaps-0.22.3/CHANGELOG.md
--rwxrwxrwx   0 alex      (1000) alex      (1000)    34940 2019-01-29 10:06:07.000000 tagmaps-0.22.3/LICENSE.md
--rw-r--r--   0 alex      (1000) alex      (1000)      164 2023-05-16 10:04:37.000000 tagmaps-0.22.3/MANIFEST.in
--rw-r--r--   0 alex      (1000) alex      (1000)    12288 2023-07-17 11:24:34.898678 tagmaps-0.22.3/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)    12137 2023-05-16 10:05:32.000000 tagmaps-0.22.3/README.md
--rw-r--r--   0 alex      (1000) alex      (1000)     2195 2023-05-16 10:04:38.000000 tagmaps-0.22.3/pyproject.toml
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-07-17 11:24:34.908782 tagmaps-0.22.3/setup.cfg
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 11:24:34.491994 tagmaps-0.22.3/src/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 11:24:34.652163 tagmaps-0.22.3/src/tagmaps/
--rw-r--r--   0 alex      (1000) alex      (1000)      620 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     5914 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/__main__.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 11:24:34.825741 tagmaps-0.22.3/src/tagmaps/classes/
--rw-r--r--   0 alex      (1000) alex      (1000)       33 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/classes/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)    17470 2023-07-17 11:20:03.000000 tagmaps-0.22.3/src/tagmaps/classes/alpha_shapes.py
--rw-r--r--   0 alex      (1000) alex      (1000)    41054 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/classes/cluster.py
--rw-r--r--   0 alex      (1000) alex      (1000)    17232 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/classes/compile_output.py
--rw-r--r--   0 alex      (1000) alex      (1000)    23633 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/classes/interface.py
--rw-r--r--   0 alex      (1000) alex      (1000)    17745 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/classes/load_data.py
--rw-r--r--   0 alex      (1000) alex      (1000)    10479 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/classes/plotting.py
--rw-r--r--   0 alex      (1000) alex      (1000)    32505 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/classes/prepare_data.py
--rw-r--r--   0 alex      (1000) alex      (1000)     9578 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/classes/shared_structure.py
--rw-r--r--   0 alex      (1000) alex      (1000)    21911 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/classes/utils.py
--rw-r--r--   0 alex      (1000) alex      (1000)       75 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/classes/write_output.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 11:24:34.844908 tagmaps-0.22.3/src/tagmaps/config/
--rw-r--r--   0 alex      (1000) alex      (1000)       39 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/config/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)    26041 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/config/config.py
--rw-r--r--   0 alex      (1000) alex      (1000)    31972 2023-05-16 10:04:39.000000 tagmaps-0.22.3/src/tagmaps/matplotlibrc
--rw-r--r--   0 alex      (1000) alex      (1000)    19100 2023-05-16 10:04:39.000000 tagmaps-0.22.3/src/tagmaps/tagmaps_.py
--rw-r--r--   0 alex      (1000) alex      (1000)       46 2023-07-17 11:23:47.000000 tagmaps-0.22.3/src/tagmaps/version.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 11:24:34.679425 tagmaps-0.22.3/src/tagmaps.egg-info/
--rwxrwxrwx   0 alex      (1000) alex      (1000)    12288 2023-07-17 11:24:34.000000 tagmaps-0.22.3/src/tagmaps.egg-info/PKG-INFO
--rwxrwxrwx   0 alex      (1000) alex      (1000)      885 2023-07-17 11:24:34.000000 tagmaps-0.22.3/src/tagmaps.egg-info/SOURCES.txt
--rwxrwxrwx   0 alex      (1000) alex      (1000)        1 2023-07-17 11:24:34.000000 tagmaps-0.22.3/src/tagmaps.egg-info/dependency_links.txt
--rwxrwxrwx   0 alex      (1000) alex      (1000)       50 2023-07-17 11:24:34.000000 tagmaps-0.22.3/src/tagmaps.egg-info/entry_points.txt
--rwxrwxrwx   0 alex      (1000) alex      (1000)      110 2023-07-17 11:24:34.000000 tagmaps-0.22.3/src/tagmaps.egg-info/requires.txt
--rwxrwxrwx   0 alex      (1000) alex      (1000)        8 2023-07-17 11:24:34.000000 tagmaps-0.22.3/src/tagmaps.egg-info/top_level.txt
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 11:24:34.886654 tagmaps-0.22.3/tests/
--rw-r--r--   0 alex      (1000) alex      (1000)      627 2023-05-16 10:04:39.000000 tagmaps-0.22.3/tests/test_all.py
--rwxrwxrwx   0 alex      (1000) alex      (1000)     3271 2019-02-22 14:26:36.000000 tagmaps-0.22.3/tests/test_emoji.py
--rwxrwxrwx   0 alex      (1000) alex      (1000)      934 2019-01-29 10:06:07.000000 tagmaps-0.22.3/tests/test_post.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 09:31:09.745502 tagmaps-0.22.4/
+-rw-r--r--   0 alex      (1000) alex      (1000)     9421 2023-07-21 09:30:35.000000 tagmaps-0.22.4/CHANGELOG.md
+-rwxrwxrwx   0 alex      (1000) alex      (1000)    34940 2019-01-29 10:06:07.000000 tagmaps-0.22.4/LICENSE.md
+-rw-r--r--   0 alex      (1000) alex      (1000)      164 2023-05-16 10:04:37.000000 tagmaps-0.22.4/MANIFEST.in
+-rw-r--r--   0 alex      (1000) alex      (1000)    12288 2023-07-21 09:31:09.729434 tagmaps-0.22.4/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)    12137 2023-05-16 10:05:32.000000 tagmaps-0.22.4/README.md
+-rw-r--r--   0 alex      (1000) alex      (1000)     2195 2023-07-21 09:30:11.000000 tagmaps-0.22.4/pyproject.toml
+-rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-07-21 09:31:09.746506 tagmaps-0.22.4/setup.cfg
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 09:31:09.268733 tagmaps-0.22.4/src/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 09:31:09.421664 tagmaps-0.22.4/src/tagmaps/
+-rw-r--r--   0 alex      (1000) alex      (1000)      620 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     5914 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/__main__.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 09:31:09.660687 tagmaps-0.22.4/src/tagmaps/classes/
+-rw-r--r--   0 alex      (1000) alex      (1000)       33 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/classes/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    17470 2023-07-17 11:20:03.000000 tagmaps-0.22.4/src/tagmaps/classes/alpha_shapes.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    41054 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/classes/cluster.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    17232 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/classes/compile_output.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    23633 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/classes/interface.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    17745 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/classes/load_data.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    10479 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/classes/plotting.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    32505 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/classes/prepare_data.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     9578 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/classes/shared_structure.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    21911 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/classes/utils.py
+-rw-r--r--   0 alex      (1000) alex      (1000)       75 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/classes/write_output.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 09:31:09.674243 tagmaps-0.22.4/src/tagmaps/config/
+-rw-r--r--   0 alex      (1000) alex      (1000)       39 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/config/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    26041 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/config/config.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    31972 2023-05-16 10:04:39.000000 tagmaps-0.22.4/src/tagmaps/matplotlibrc
+-rw-r--r--   0 alex      (1000) alex      (1000)    19100 2023-05-16 10:04:39.000000 tagmaps-0.22.4/src/tagmaps/tagmaps_.py
+-rw-r--r--   0 alex      (1000) alex      (1000)       46 2023-07-21 09:30:35.000000 tagmaps-0.22.4/src/tagmaps/version.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 09:31:09.464716 tagmaps-0.22.4/src/tagmaps.egg-info/
+-rwxrwxrwx   0 alex      (1000) alex      (1000)    12288 2023-07-21 09:31:09.000000 tagmaps-0.22.4/src/tagmaps.egg-info/PKG-INFO
+-rwxrwxrwx   0 alex      (1000) alex      (1000)      885 2023-07-21 09:31:09.000000 tagmaps-0.22.4/src/tagmaps.egg-info/SOURCES.txt
+-rwxrwxrwx   0 alex      (1000) alex      (1000)        1 2023-07-21 09:31:09.000000 tagmaps-0.22.4/src/tagmaps.egg-info/dependency_links.txt
+-rwxrwxrwx   0 alex      (1000) alex      (1000)       50 2023-07-21 09:31:09.000000 tagmaps-0.22.4/src/tagmaps.egg-info/entry_points.txt
+-rwxrwxrwx   0 alex      (1000) alex      (1000)      110 2023-07-21 09:31:09.000000 tagmaps-0.22.4/src/tagmaps.egg-info/requires.txt
+-rwxrwxrwx   0 alex      (1000) alex      (1000)        8 2023-07-21 09:31:09.000000 tagmaps-0.22.4/src/tagmaps.egg-info/top_level.txt
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 09:31:09.726434 tagmaps-0.22.4/tests/
+-rw-r--r--   0 alex      (1000) alex      (1000)      627 2023-05-16 10:04:39.000000 tagmaps-0.22.4/tests/test_all.py
+-rwxrwxrwx   0 alex      (1000) alex      (1000)     3271 2019-02-22 14:26:36.000000 tagmaps-0.22.4/tests/test_emoji.py
+-rwxrwxrwx   0 alex      (1000) alex      (1000)      934 2019-01-29 10:06:07.000000 tagmaps-0.22.4/tests/test_post.py
```

### Comparing `tagmaps-0.22.3/CHANGELOG.md` & `tagmaps-0.22.4/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.22.4 (2023-07-21)
+### Fix
+* Requirements.txt containing misspelled and missing dependencies ([`54fa4c1`](https://github.com/Sieboldianus/TagMaps/commit/54fa4c122c75ea580bbe136864815dd1ee265dc5))
+* HDBSCAN TypeError: 'numpy.float64', [1] ([`4f9a652`](https://github.com/Sieboldianus/TagMaps/commit/4f9a652111d1fa28e393051df64e8a7e9f179cca))
+
+### Documentation
+* Add instructions to install on Linux and from requirements.txt ([`07cc618`](https://github.com/Sieboldianus/TagMaps/commit/07cc618175f6cfa9b0da1abf26d9932af752283e))
+* Add instructions to use conda together with no-dependencies and --editable flags ([`d8143db`](https://github.com/Sieboldianus/TagMaps/commit/d8143db52c19b5867c7e981618b847076a1f9190))
+
 ## v0.22.3 (2023-07-17)
 ### Fix
 * Tri.vertices - Delaunay object has no attribute vertices ([`621b267`](https://github.com/Sieboldianus/TagMaps/commit/621b2673e34cec61c35c625a512b73b9937d6497))
 
 ## v0.22.2 (2023-05-16)
```

### Comparing `tagmaps-0.22.3/LICENSE.md` & `tagmaps-0.22.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.3/PKG-INFO` & `tagmaps-0.22.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tagmaps
-Version: 0.22.3
+Version: 0.22.4
 Summary: Tag Clustering for Tag Maps
 Author-email: Alexander Dunkel <alexander.dunkel@tu-dresden.de>
 License: GNU GPLv3 or any higher
 Project-URL: Homepage, https://github.com/Sieboldianus/TagMaps
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `tagmaps-0.22.3/README.md` & `tagmaps-0.22.4/README.md`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.3/pyproject.toml` & `tagmaps-0.22.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "fiona",
     "shapely",
     "pandas>=0.24.2",
     "pyproj>=2.0.0",
     "numpy",
     "matplotlib>=3.0.0",
     "emoji>=2.0.0",
-    "hdbscan>=0.8.20",
+    "hdbscan>=0.8.31",
     "seaborn",
     "scipy",
 ]
 dynamic = ["version"]
 
 [project.readme]
 file = "README.md"
```

### Comparing `tagmaps-0.22.3/src/tagmaps/__init__.py` & `tagmaps-0.22.4/src/tagmaps/__init__.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.3/src/tagmaps/__main__.py` & `tagmaps-0.22.4/src/tagmaps/__main__.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.3/src/tagmaps/classes/alpha_shapes.py` & `tagmaps-0.22.4/src/tagmaps/classes/alpha_shapes.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.3/src/tagmaps/classes/cluster.py` & `tagmaps-0.22.4/src/tagmaps/classes/cluster.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.3/src/tagmaps/classes/compile_output.py` & `tagmaps-0.22.4/src/tagmaps/classes/compile_output.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.3/src/tagmaps/classes/interface.py` & `tagmaps-0.22.4/src/tagmaps/classes/interface.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.3/src/tagmaps/classes/load_data.py` & `tagmaps-0.22.4/src/tagmaps/classes/load_data.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.3/src/tagmaps/classes/plotting.py` & `tagmaps-0.22.4/src/tagmaps/classes/plotting.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.3/src/tagmaps/classes/prepare_data.py` & `tagmaps-0.22.4/src/tagmaps/classes/prepare_data.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.3/src/tagmaps/classes/shared_structure.py` & `tagmaps-0.22.4/src/tagmaps/classes/shared_structure.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.3/src/tagmaps/classes/utils.py` & `tagmaps-0.22.4/src/tagmaps/classes/utils.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.3/src/tagmaps/config/config.py` & `tagmaps-0.22.4/src/tagmaps/config/config.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.3/src/tagmaps/matplotlibrc` & `tagmaps-0.22.4/src/tagmaps/matplotlibrc`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.3/src/tagmaps/tagmaps_.py` & `tagmaps-0.22.4/src/tagmaps/tagmaps_.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.3/src/tagmaps.egg-info/PKG-INFO` & `tagmaps-0.22.4/src/tagmaps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tagmaps
-Version: 0.22.3
+Version: 0.22.4
 Summary: Tag Clustering for Tag Maps
 Author-email: Alexander Dunkel <alexander.dunkel@tu-dresden.de>
 License: GNU GPLv3 or any higher
 Project-URL: Homepage, https://github.com/Sieboldianus/TagMaps
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `tagmaps-0.22.3/src/tagmaps.egg-info/SOURCES.txt` & `tagmaps-0.22.4/src/tagmaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.3/tests/test_all.py` & `tagmaps-0.22.4/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.3/tests/test_emoji.py` & `tagmaps-0.22.4/tests/test_emoji.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.3/tests/test_post.py` & `tagmaps-0.22.4/tests/test_post.py`

 * *Files identical despite different names*

