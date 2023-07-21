# Comparing `tmp/mapel-roommates-2.0.8.tar.gz` & `tmp/mapel-roommates-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-roommates-2.0.8.tar", last modified: Tue Jul 18 07:11:39 2023, max compression
+gzip compressed data, was "mapel-roommates-2.0.9.tar", last modified: Fri Jul 21 15:02:07 2023, max compression
```

## Comparing `mapel-roommates-2.0.8.tar` & `mapel-roommates-2.0.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:39.673060 mapel-roommates-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-18 07:11:39.673060 mapel-roommates-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 07:11:39.673060 mapel-roommates-2.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:39.669060 mapel-roommates-2.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:39.669060 mapel-roommates-2.0.8/src/mapel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:39.669060 mapel-roommates-2.0.8/src/mapel/roommates/
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:39.669060 mapel-roommates-2.0.8/src/mapel/roommates/cultures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/cultures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/cultures/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/cultures/euclidean.py
--rw-r--r--   0 runner    (1001) docker     (123)    18776 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/cultures/group_separable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/cultures/impartial.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/cultures/mallows.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/cultures/urn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/cultures_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:39.673060 mapel-roommates-2.0.8/src/mapel/roommates/distances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/distances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/distances/main_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/distances_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:39.673060 mapel-roommates-2.0.8/src/mapel/roommates/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/features/basic_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/features/distance_to_stability_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/features_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:39.673060 mapel-roommates-2.0.8/src/mapel/roommates/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/objects/Roommates.py
--rw-r--r--   0 runner    (1001) docker     (123)    18351 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/objects/RoommatesExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/objects/RoommatesFamily.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:39.673060 mapel-roommates-2.0.8/src/mapel/roommates/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/persistence/instance_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/persistence/instance_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:39.673060 mapel-roommates-2.0.8/src/mapel_roommates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-18 07:11:39.000000 mapel-roommates-2.0.8/src/mapel_roommates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-18 07:11:39.000000 mapel-roommates-2.0.8/src/mapel_roommates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 07:11:39.000000 mapel-roommates-2.0.8/src/mapel_roommates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-18 07:11:39.000000 mapel-roommates-2.0.8/src/mapel_roommates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 07:11:39.000000 mapel-roommates-2.0.8/src/mapel_roommates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:02:07.265889 mapel-roommates-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-21 15:02:07.265889 mapel-roommates-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:02:07.269888 mapel-roommates-2.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:02:07.261888 mapel-roommates-2.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:02:07.261888 mapel-roommates-2.0.9/src/mapel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:02:07.265889 mapel-roommates-2.0.9/src/mapel/roommates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/src/mapel/roommates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:02:07.265889 mapel-roommates-2.0.9/src/mapel/roommates/cultures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/src/mapel/roommates/cultures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/src/mapel/roommates/cultures/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/src/mapel/roommates/cultures/euclidean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18776 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/src/mapel/roommates/cultures/group_separable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/src/mapel/roommates/cultures/impartial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/src/mapel/roommates/cultures/mallows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/src/mapel/roommates/cultures/urn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/src/mapel/roommates/cultures_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:02:07.265889 mapel-roommates-2.0.9/src/mapel/roommates/distances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/src/mapel/roommates/distances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/src/mapel/roommates/distances/main_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/src/mapel/roommates/distances_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:02:07.265889 mapel-roommates-2.0.9/src/mapel/roommates/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/src/mapel/roommates/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/src/mapel/roommates/features/basic_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/src/mapel/roommates/features/distance_to_stability_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/src/mapel/roommates/features_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:02:07.265889 mapel-roommates-2.0.9/src/mapel/roommates/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/src/mapel/roommates/objects/Roommates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18351 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/src/mapel/roommates/objects/RoommatesExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/src/mapel/roommates/objects/RoommatesFamily.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/src/mapel/roommates/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:02:07.265889 mapel-roommates-2.0.9/src/mapel/roommates/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/src/mapel/roommates/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/src/mapel/roommates/persistence/instance_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-21 15:01:36.000000 mapel-roommates-2.0.9/src/mapel/roommates/persistence/instance_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:02:07.265889 mapel-roommates-2.0.9/src/mapel_roommates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-21 15:02:07.000000 mapel-roommates-2.0.9/src/mapel_roommates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-21 15:02:07.000000 mapel-roommates-2.0.9/src/mapel_roommates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:02:07.000000 mapel-roommates-2.0.9/src/mapel_roommates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 15:02:07.000000 mapel-roommates-2.0.9/src/mapel_roommates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 15:02:07.000000 mapel-roommates-2.0.9/src/mapel_roommates.egg-info/top_level.txt
```

### Comparing `mapel-roommates-2.0.8/LICENSE.txt` & `mapel-roommates-2.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.8/PKG-INFO` & `mapel-roommates-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-roommates
-Version: 2.0.8
+Version: 2.0.9
 Summary: Map of Roommates
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-roommates-2.0.8/README.md` & `mapel-roommates-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.8/pyproject.toml` & `mapel-roommates-2.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel", "pybind11>=2.6.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapel-roommates"
-version = "2.0.8"
+version = "2.0.9"
 authors = [
  {name = "Stanislaw Szufa", email = "s.szufa@gmail.com"},
  {name = "Niclas Boehmer", email = "niclas.boehmer@tu-berlin.de"},
 ]
 description = "Map of Roommates"
 classifiers=[
     "Programming Language :: Python :: 3",
```

### Comparing `mapel-roommates-2.0.8/src/mapel/roommates/__init__.py` & `mapel-roommates-2.0.9/src/mapel/roommates/__init__.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.8/src/mapel/roommates/cultures/euclidean.py` & `mapel-roommates-2.0.9/src/mapel/roommates/cultures/euclidean.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.8/src/mapel/roommates/cultures/group_separable.py` & `mapel-roommates-2.0.9/src/mapel/roommates/cultures/group_separable.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.8/src/mapel/roommates/cultures/impartial.py` & `mapel-roommates-2.0.9/src/mapel/roommates/cultures/impartial.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.8/src/mapel/roommates/cultures/mallows.py` & `mapel-roommates-2.0.9/src/mapel/roommates/cultures/mallows.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.8/src/mapel/roommates/cultures/urn.py` & `mapel-roommates-2.0.9/src/mapel/roommates/cultures/urn.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.8/src/mapel/roommates/cultures_.py` & `mapel-roommates-2.0.9/src/mapel/roommates/cultures_.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.8/src/mapel/roommates/distances/main_distances.py` & `mapel-roommates-2.0.9/src/mapel/roommates/distances/main_distances.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.8/src/mapel/roommates/distances_.py` & `mapel-roommates-2.0.9/src/mapel/roommates/distances_.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.8/src/mapel/roommates/features/basic_features.py` & `mapel-roommates-2.0.9/src/mapel/roommates/features/basic_features.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.8/src/mapel/roommates/features/distance_to_stability_features.py` & `mapel-roommates-2.0.9/src/mapel/roommates/features/distance_to_stability_features.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.8/src/mapel/roommates/features_.py` & `mapel-roommates-2.0.9/src/mapel/roommates/features_.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.8/src/mapel/roommates/objects/Roommates.py` & `mapel-roommates-2.0.9/src/mapel/roommates/objects/Roommates.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.8/src/mapel/roommates/objects/RoommatesExperiment.py` & `mapel-roommates-2.0.9/src/mapel/roommates/objects/RoommatesExperiment.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.8/src/mapel/roommates/objects/RoommatesFamily.py` & `mapel-roommates-2.0.9/src/mapel/roommates/objects/RoommatesFamily.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.8/src/mapel/roommates/persistence/instance_exports.py` & `mapel-roommates-2.0.9/src/mapel/roommates/persistence/instance_exports.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.8/src/mapel/roommates/persistence/instance_imports.py` & `mapel-roommates-2.0.9/src/mapel/roommates/persistence/instance_imports.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.8/src/mapel_roommates.egg-info/PKG-INFO` & `mapel-roommates-2.0.9/src/mapel_roommates.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-roommates
-Version: 2.0.8
+Version: 2.0.9
 Summary: Map of Roommates
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-roommates-2.0.8/src/mapel_roommates.egg-info/SOURCES.txt` & `mapel-roommates-2.0.9/src/mapel_roommates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

