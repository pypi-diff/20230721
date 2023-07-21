# Comparing `tmp/afmformats-0.8.0.tar.gz` & `tmp/afmformats-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/afmformats-0.8.0.tar", last modified: Tue Feb  4 07:39:45 2020, max compression
+gzip compressed data, was "dist/afmformats-0.9.0.tar", last modified: Fri Feb 14 09:58:15 2020, max compression
```

## Comparing `afmformats-0.8.0.tar` & `afmformats-0.9.0.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-04 07:39:45.000000 afmformats-0.8.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)      112 2020-02-04 07:39:20.000000 afmformats-0.8.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2058 2020-02-04 07:39:45.000000 afmformats-0.8.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)       98 2020-02-04 07:39:45.000000 afmformats-0.8.0/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-04 07:39:45.000000 afmformats-0.8.0/afmformats.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2058 2020-02-04 07:39:45.000000 afmformats-0.8.0/afmformats.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-02-04 07:39:45.000000 afmformats-0.8.0/afmformats.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2020-02-04 07:39:45.000000 afmformats-0.8.0/afmformats.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      958 2020-02-04 07:39:45.000000 afmformats-0.8.0/afmformats.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       26 2020-02-04 07:39:45.000000 afmformats-0.8.0/afmformats.egg-info/requires.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-04 07:39:45.000000 afmformats-0.8.0/afmformats/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9010 2020-02-04 07:39:20.000000 afmformats-0.8.0/afmformats/afm_data.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-04 07:39:45.000000 afmformats-0.8.0/afmformats/fmt_jpk/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10869 2020-02-04 07:39:20.000000 afmformats-0.8.0/afmformats/fmt_jpk/read_jpk_meta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18985 2020-02-04 07:39:20.000000 afmformats-0.8.0/afmformats/fmt_jpk/read_jpk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1709 2020-02-04 07:39:20.000000 afmformats-0.8.0/afmformats/fmt_jpk/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7095 2020-02-04 07:39:20.000000 afmformats-0.8.0/afmformats/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1175 2020-02-04 07:39:20.000000 afmformats-0.8.0/afmformats/parse_funcs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1952 2020-02-04 07:39:20.000000 afmformats-0.8.0/afmformats/formats.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2558 2020-02-04 07:39:20.000000 afmformats-0.8.0/afmformats/fmt_tab.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5033 2020-02-04 07:39:20.000000 afmformats-0.8.0/afmformats/meta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      243 2020-02-04 07:39:20.000000 afmformats-0.8.0/afmformats/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2045 2020-02-04 07:39:20.000000 afmformats-0.8.0/afmformats/afm_fdist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      293 2020-02-04 07:39:20.000000 afmformats-0.8.0/afmformats/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       82 2020-02-04 07:39:24.000000 afmformats-0.8.0/afmformats/_version_save.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3771 2020-02-04 07:39:20.000000 afmformats-0.8.0/afmformats/fmt_hdf5.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2020-02-04 07:39:20.000000 afmformats-0.8.0/CHANGELOG
--rw-rw-r--   0 travis    (2000) travis    (2000)     1069 2020-02-04 07:39:20.000000 afmformats-0.8.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1249 2020-02-04 07:39:20.000000 afmformats-0.8.0/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1397 2020-02-04 07:39:20.000000 afmformats-0.8.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-04 07:39:45.000000 afmformats-0.8.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1102 2020-02-04 07:39:20.000000 afmformats-0.8.0/tests/test_fmt_hdf5_load.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3161 2020-02-04 07:39:20.000000 afmformats-0.8.0/tests/test_fmt_jpk_single.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-04 07:39:45.000000 afmformats-0.8.0/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)   407527 2020-02-04 07:39:20.000000 afmformats-0.8.0/tests/data/map0d_extracted.jpk-force-map
--rwxrwxr-x   0 travis    (2000) travis    (2000)    68411 2020-02-04 07:39:20.000000 afmformats-0.8.0/tests/data/calibration_force-save-2015.02.04-11.25.21.294.jpk-force
--rw-rw-r--   0 travis    (2000) travis    (2000)    22266 2020-02-04 07:39:20.000000 afmformats-0.8.0/tests/data/spot3-0192.jpk-force
--rw-rw-r--   0 travis    (2000) travis    (2000)   953060 2020-02-04 07:39:20.000000 afmformats-0.8.0/tests/data/map2x2_extracted.jpk-force-map
--rw-rw-r--   0 travis    (2000) travis    (2000)     2349 2020-02-04 07:39:20.000000 afmformats-0.8.0/tests/test_fmt_jpk_jproperties.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1874 2020-02-04 07:39:20.000000 afmformats-0.8.0/tests/test_fmt_tab_load.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1707 2020-02-04 07:39:20.000000 afmformats-0.8.0/tests/test_fmt_jpk_map.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1004 2020-02-04 07:39:20.000000 afmformats-0.8.0/tests/test_afm_fdist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1509 2020-02-04 07:39:20.000000 afmformats-0.8.0/tests/test_fmt_jpk_load.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 09:58:15.000000 afmformats-0.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      112 2020-02-14 09:57:42.000000 afmformats-0.9.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2058 2020-02-14 09:58:15.000000 afmformats-0.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)       98 2020-02-14 09:58:15.000000 afmformats-0.9.0/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 09:58:15.000000 afmformats-0.9.0/afmformats.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2058 2020-02-14 09:58:15.000000 afmformats-0.9.0/afmformats.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-02-14 09:58:15.000000 afmformats-0.9.0/afmformats.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       11 2020-02-14 09:58:15.000000 afmformats-0.9.0/afmformats.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1009 2020-02-14 09:58:15.000000 afmformats-0.9.0/afmformats.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       31 2020-02-14 09:58:15.000000 afmformats-0.9.0/afmformats.egg-info/requires.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 09:58:15.000000 afmformats-0.9.0/afmformats/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9010 2020-02-14 09:57:42.000000 afmformats-0.9.0/afmformats/afm_data.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 09:58:15.000000 afmformats-0.9.0/afmformats/fmt_jpk/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10855 2020-02-14 09:57:42.000000 afmformats-0.9.0/afmformats/fmt_jpk/read_jpk_meta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18985 2020-02-14 09:57:42.000000 afmformats-0.9.0/afmformats/fmt_jpk/read_jpk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1834 2020-02-14 09:57:42.000000 afmformats-0.9.0/afmformats/fmt_jpk/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7095 2020-02-14 09:57:42.000000 afmformats-0.9.0/afmformats/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1175 2020-02-14 09:57:42.000000 afmformats-0.9.0/afmformats/parse_funcs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2001 2020-02-14 09:57:42.000000 afmformats-0.9.0/afmformats/formats.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3411 2020-02-14 09:57:42.000000 afmformats-0.9.0/afmformats/fmt_igor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2595 2020-02-14 09:57:42.000000 afmformats-0.9.0/afmformats/fmt_tab.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5025 2020-02-14 09:57:42.000000 afmformats-0.9.0/afmformats/meta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      243 2020-02-14 09:57:42.000000 afmformats-0.9.0/afmformats/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2045 2020-02-14 09:57:42.000000 afmformats-0.9.0/afmformats/afm_fdist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      347 2020-02-14 09:57:42.000000 afmformats-0.9.0/afmformats/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       82 2020-02-14 09:57:48.000000 afmformats-0.9.0/afmformats/_version_save.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3798 2020-02-14 09:57:42.000000 afmformats-0.9.0/afmformats/fmt_hdf5.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1923 2020-02-14 09:57:42.000000 afmformats-0.9.0/CHANGELOG
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1069 2020-02-14 09:57:42.000000 afmformats-0.9.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1249 2020-02-14 09:57:42.000000 afmformats-0.9.0/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1463 2020-02-14 09:57:42.000000 afmformats-0.9.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 09:58:15.000000 afmformats-0.9.0/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1102 2020-02-14 09:57:42.000000 afmformats-0.9.0/tests/test_fmt_hdf5_load.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3161 2020-02-14 09:57:42.000000 afmformats-0.9.0/tests/test_fmt_jpk_single.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-14 09:58:15.000000 afmformats-0.9.0/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   407527 2020-02-14 09:57:42.000000 afmformats-0.9.0/tests/data/map0d_extracted.jpk-force-map
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    68411 2020-02-14 09:57:42.000000 afmformats-0.9.0/tests/data/calibration_force-save-2015.02.04-11.25.21.294.jpk-force
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22266 2020-02-14 09:57:42.000000 afmformats-0.9.0/tests/data/spot3-0192.jpk-force
+-rw-rw-r--   0 travis    (2000) travis    (2000)   953060 2020-02-14 09:57:42.000000 afmformats-0.9.0/tests/data/map2x2_extracted.jpk-force-map
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2349 2020-02-14 09:57:42.000000 afmformats-0.9.0/tests/test_fmt_jpk_jproperties.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1028 2020-02-14 09:57:42.000000 afmformats-0.9.0/tests/test_fmt_igor_load.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1874 2020-02-14 09:57:42.000000 afmformats-0.9.0/tests/test_fmt_tab_load.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1707 2020-02-14 09:57:42.000000 afmformats-0.9.0/tests/test_fmt_jpk_map.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1004 2020-02-14 09:57:42.000000 afmformats-0.9.0/tests/test_afm_fdist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1509 2020-02-14 09:57:42.000000 afmformats-0.9.0/tests/test_fmt_jpk_load.py
```

### Comparing `afmformats-0.8.0/PKG-INFO` & `afmformats-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: afmformats
-Version: 0.8.0
+Version: 0.9.0
 Summary: reading common AFM file formats
 Home-page: https://github.com/AFM-analysis/afmformats
 Author: Paul Müller
 Author-email: dev@craban.de
 License: MIT
 Description: afmformats
         ==========
```

### Comparing `afmformats-0.8.0/afmformats.egg-info/PKG-INFO` & `afmformats-0.9.0/afmformats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: afmformats
-Version: 0.8.0
+Version: 0.9.0
 Summary: reading common AFM file formats
 Home-page: https://github.com/AFM-analysis/afmformats
 Author: Paul Müller
 Author-email: dev@craban.de
 License: MIT
 Description: afmformats
         ==========
```

### Comparing `afmformats-0.8.0/afmformats.egg-info/SOURCES.txt` & `afmformats-0.9.0/afmformats.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,28 +7,30 @@
 afmformats/__init__.py
 afmformats/_version.py
 afmformats/_version_save.py
 afmformats/afm_data.py
 afmformats/afm_fdist.py
 afmformats/errors.py
 afmformats/fmt_hdf5.py
+afmformats/fmt_igor.py
 afmformats/fmt_tab.py
 afmformats/formats.py
 afmformats/meta.py
 afmformats/parse_funcs.py
 afmformats.egg-info/PKG-INFO
 afmformats.egg-info/SOURCES.txt
 afmformats.egg-info/dependency_links.txt
 afmformats.egg-info/requires.txt
 afmformats.egg-info/top_level.txt
 afmformats/fmt_jpk/__init__.py
 afmformats/fmt_jpk/read_jpk.py
 afmformats/fmt_jpk/read_jpk_meta.py
 tests/test_afm_fdist.py
 tests/test_fmt_hdf5_load.py
+tests/test_fmt_igor_load.py
 tests/test_fmt_jpk_jproperties.py
 tests/test_fmt_jpk_load.py
 tests/test_fmt_jpk_map.py
 tests/test_fmt_jpk_single.py
 tests/test_fmt_tab_load.py
 tests/data/calibration_force-save-2015.02.04-11.25.21.294.jpk-force
 tests/data/map0d_extracted.jpk-force-map
```

### Comparing `afmformats-0.8.0/afmformats/afm_data.py` & `afmformats-0.9.0/afmformats/afm_data.py`

 * *Files identical despite different names*

### Comparing `afmformats-0.8.0/afmformats/fmt_jpk/read_jpk_meta.py` & `afmformats-0.9.0/afmformats/fmt_jpk/read_jpk_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,16 +149,16 @@
 
     md["curve id"] = "{}:{:g}".format(md["session id"], mdi["position index"])
 
     md["setpoint"] = md_im["setpoint [V]"] * \
         md["spring constant"]*md["sensitivity"]
 
     md["rate " + curseg] = md["point count"]/md["duration"]
-    md["z range"] = abs(md_im["z start"] - md_im["z end"])
-    md["speed " + curseg] = md["z range"]/md["duration"]
+    zrange = abs(md_im["z start"] - md_im["z end"])
+    md["speed " + curseg] = zrange/md["duration"]
     if "position x [m]" in md_im:
         md["position x"] = md_im["position x [m]"]
     if "position y [m]" in md_im:
         md["position y"] = md_im["position y [m]"]
     if "grid size x [m]" in md_im:
         md["grid size x"] = md_im["grid size x [m]"]
     if "grid size y [m]" in md_im:
```

### Comparing `afmformats-0.8.0/afmformats/fmt_jpk/read_jpk.py` & `afmformats-0.9.0/afmformats/fmt_jpk/read_jpk.py`

 * *Files identical despite different names*

### Comparing `afmformats-0.8.0/afmformats/fmt_jpk/__init__.py` & `afmformats-0.9.0/afmformats/fmt_jpk/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,28 +28,31 @@
         # join segments
         lenapp = len(app[list(app.keys())[0]])
         lenret = len(ret[list(ret.keys())[0]])
         ret["time"] += metadata["duration"]
         data = {}
         for key in app.keys():
             data[key] = np.concatenate((app[key], ret[key]))
+        metadata["z range"] = np.ptp(data["height (piezo)"])
         data["segment"] = np.concatenate((np.zeros(lenapp, dtype=bool),
                                           np.ones(lenret, dtype=bool)))
         dataset.append({"data": data,
                         "metadata": metadata,
                         })
     return dataset
 
 
 recipe_jpk_force = {
+    "descr": "binary FD data",
     "loader": load_jpk,
     "suffix": ".jpk-force",
     "mode": "force-distance",
     "maker": "JPK Instruments",
 }
 
 recipe_jpk_force_map = {
+    "descr": "binary QMap data",
     "loader": load_jpk,
     "suffix": ".jpk-force-map",
     "mode": "force-distance",
     "maker": "JPK Instruments",
 }
```

### Comparing `afmformats-0.8.0/afmformats/_version.py` & `afmformats-0.9.0/afmformats/_version.py`

 * *Files identical despite different names*

### Comparing `afmformats-0.8.0/afmformats/parse_funcs.py` & `afmformats-0.9.0/afmformats/parse_funcs.py`

 * *Files identical despite different names*

### Comparing `afmformats-0.8.0/afmformats/formats.py` & `afmformats-0.9.0/afmformats/formats.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pathlib
 
 from .fmt_hdf5 import recipe_hdf5
+from .fmt_igor import recipe_ibw
 from .fmt_jpk import recipe_jpk_force, recipe_jpk_force_map
 from .fmt_tab import recipe_tab
 from .afm_fdist import AFMForceDistance
 
 
 __all__ = ["load_data", "formats_available", "formats_by_suffix",
            "formats_by_mode", "supported_extensions"]
@@ -31,14 +32,15 @@
         raise ValueError("Unsupported file extension: '{}'!".format(path))
     return afmdata
 
 
 #: available/supported file formats
 formats_available = [
     recipe_hdf5,
+    recipe_ibw,
     recipe_jpk_force,
     recipe_jpk_force_map,
     recipe_tab,
 ]
 #: available file formats in a dictionary with suffix keys
 formats_by_suffix = {}
 # Populate list of available fit models
```

### Comparing `afmformats-0.8.0/afmformats/fmt_tab.py` & `afmformats-0.9.0/afmformats/fmt_tab.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,12 +81,13 @@
     elif dtype in [float, int]:
         return dtype(astring)
     else:
         raise ValueError("No conversion rule for dtype '{}'!".format(dtype))
 
 
 recipe_tab = {
+    "descr": "tab-separated values",
     "loader": load_tab,
     "suffix": ".tab",
     "mode": "force-distance",
     "maker": "afmformats",
 }
```

### Comparing `afmformats-0.8.0/afmformats/meta.py` & `afmformats-0.9.0/afmformats/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,23 +28,23 @@
             "force-distance",
         ])],
         "rate approach": ["Sampling rate (approach)", "Hz", float],
         "rate retract": ["Sampling rate (retract)", "Hz", float],
         "sensitivity": ["Sensitivity", "m/V", float],
         "setpoint": ["Active feedback loop setpoint", "N", float],
         "spring constant": ["Cantilever spring constant", "N/m", float],
-        "z range": ["Axial piezo range covered", "m", float],
     },
     # dataset parameters
     "dataset": {
         "duration": ["Duration", "s", float],
         "enum": ["Dataset index within the experiment", "", fint],
         "point count": ["Size of the dataset in points", "", fint],
         "speed approach": ["Piezo speed (approach)", "m/s", float],
         "speed retract": ["Piezo speed (retract)", "m/s", float],
+        "z range": ["Axial piezo range", "m", float],
     },
     # QMap related dataset metadata
     "qmap": {
         "grid center x": ["Horizontal center of grid", "m", float],
         "grid center y": ["Vertical center of grid", "m", float],
         "grid index x": ["Horizontal grid position index", "", fint],
         "grid index y": ["Vertical grid position index", "", fint],
```

### Comparing `afmformats-0.8.0/afmformats/afm_fdist.py` & `afmformats-0.9.0/afmformats/afm_fdist.py`

 * *Files identical despite different names*

### Comparing `afmformats-0.8.0/afmformats/fmt_hdf5.py` & `afmformats-0.9.0/afmformats/fmt_hdf5.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,12 +106,13 @@
                        "metadata": metadata})
     if close:
         h5.close()
     return fdlist
 
 
 recipe_hdf5 = {
+    "descr": "HDF5-based",
     "loader": load_hdf5,
     "suffix": ".h5",
     "mode": "force-distance",
     "maker": "afmformats",
 }
```

### Comparing `afmformats-0.8.0/CHANGELOG` & `afmformats-0.9.0/CHANGELOG`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+0.9.0
+ - feat: support new file format from Asylum Research, Igor (.ibw)
+ - ref: always compute piezo range metadata instead of taking it from
+   the set value in the acquisition settings (JKP format) 
 0.8.0
  - enh: do not export "index" column to HDF5 files to save disk space
  - enh: save column units when exporting to HDF5
  - ref: moved class methods and constants from "afm_fdist" to "afm_data"
  - docs: add code reference, basic usage, and list of file formats
 0.7.1
  - fix: exporting to HDF5 did not work when a h5py.Group was used
```

### Comparing `afmformats-0.8.0/LICENSE` & `afmformats-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `afmformats-0.8.0/README.rst` & `afmformats-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `afmformats-0.8.0/setup.py` & `afmformats-0.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     packages=find_packages(),
     package_dir={name: name},
     include_package_data=True,
     license="MIT",
     description=description,
     long_description=open('README.rst').read() if exists('README.rst') else '',
     install_requires=["h5py",
+                      "igor",  # Asylum Research .ibw file format
                       "jprops",  # JPK file format
                       "numpy>=1.14.0",
                       ],
     setup_requires=["pytest-runner"],
     tests_require=["pytest"],
     python_requires='>=3.6, <4',
     keywords=["atomic force microscopy",
```

### Comparing `afmformats-0.8.0/tests/test_fmt_hdf5_load.py` & `afmformats-0.9.0/tests/test_fmt_hdf5_load.py`

 * *Files identical despite different names*

### Comparing `afmformats-0.8.0/tests/test_fmt_jpk_single.py` & `afmformats-0.9.0/tests/test_fmt_jpk_single.py`

 * *Files identical despite different names*

### Comparing `afmformats-0.8.0/tests/data/map0d_extracted.jpk-force-map` & `afmformats-0.9.0/tests/data/map0d_extracted.jpk-force-map`

 * *Files identical despite different names*

### Comparing `afmformats-0.8.0/tests/data/calibration_force-save-2015.02.04-11.25.21.294.jpk-force` & `afmformats-0.9.0/tests/data/calibration_force-save-2015.02.04-11.25.21.294.jpk-force`

 * *Files identical despite different names*

### Comparing `afmformats-0.8.0/tests/data/spot3-0192.jpk-force` & `afmformats-0.9.0/tests/data/spot3-0192.jpk-force`

 * *Files identical despite different names*

### Comparing `afmformats-0.8.0/tests/data/map2x2_extracted.jpk-force-map` & `afmformats-0.9.0/tests/data/map2x2_extracted.jpk-force-map`

 * *Files identical despite different names*

### Comparing `afmformats-0.8.0/tests/test_fmt_jpk_jproperties.py` & `afmformats-0.9.0/tests/test_fmt_jpk_jproperties.py`

 * *Files identical despite different names*

### Comparing `afmformats-0.8.0/tests/test_fmt_tab_load.py` & `afmformats-0.9.0/tests/test_fmt_tab_load.py`

 * *Files identical despite different names*

### Comparing `afmformats-0.8.0/tests/test_fmt_jpk_map.py` & `afmformats-0.9.0/tests/test_fmt_jpk_map.py`

 * *Files identical despite different names*

### Comparing `afmformats-0.8.0/tests/test_afm_fdist.py` & `afmformats-0.9.0/tests/test_afm_fdist.py`

 * *Files identical despite different names*

### Comparing `afmformats-0.8.0/tests/test_fmt_jpk_load.py` & `afmformats-0.9.0/tests/test_fmt_jpk_load.py`

 * *Files identical despite different names*

