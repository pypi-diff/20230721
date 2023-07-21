# Comparing `tmp/wam2layers-3.0.0b4.tar.gz` & `tmp/wam2layers-3.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wam2layers-3.0.0b4.tar", last modified: Fri Apr 21 15:34:58 2023, max compression
+gzip compressed data, was "wam2layers-3.0.0b5.tar", last modified: Fri Jul 21 14:39:21 2023, max compression
```

## Comparing `wam2layers-3.0.0b4.tar` & `wam2layers-3.0.0b5.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 rjvanderent  (1000) rjvanderent  (1000)        0 2023-04-21 15:34:58.606377 wam2layers-3.0.0b4/
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)    11357 2022-11-04 15:43:46.000000 wam2layers-3.0.0b4/LICENSE
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)     2844 2023-04-21 15:34:58.606377 wam2layers-3.0.0b4/PKG-INFO
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)     2048 2022-12-22 15:03:20.000000 wam2layers-3.0.0b4/README.md
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)     1481 2023-04-21 15:33:29.000000 wam2layers-3.0.0b4/pyproject.toml
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)       38 2023-04-21 15:34:58.608382 wam2layers-3.0.0b4/setup.cfg
-drwxr-xr-x   0 rjvanderent  (1000) rjvanderent  (1000)        0 2023-04-21 15:34:58.532774 wam2layers-3.0.0b4/src/
-drwxr-xr-x   0 rjvanderent  (1000) rjvanderent  (1000)        0 2023-04-21 15:34:58.557788 wam2layers-3.0.0b4/src/wam2layers/
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)        0 2022-11-04 15:43:46.000000 wam2layers-3.0.0b4/src/wam2layers/__init__.py
-drwxr-xr-x   0 rjvanderent  (1000) rjvanderent  (1000)        0 2023-04-21 15:34:58.579906 wam2layers-3.0.0b4/src/wam2layers/analysis/
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)        0 2022-11-04 15:43:46.000000 wam2layers-3.0.0b4/src/wam2layers/analysis/__init__.py
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)     5181 2022-12-22 15:03:20.000000 wam2layers-3.0.0b4/src/wam2layers/analysis/checks.py
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)     8351 2023-04-21 15:33:29.000000 wam2layers-3.0.0b4/src/wam2layers/analysis/visualization.py
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)      492 2023-04-21 10:14:03.000000 wam2layers-3.0.0b4/src/wam2layers/cli.py
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)     8589 2023-04-21 15:33:29.000000 wam2layers-3.0.0b4/src/wam2layers/config.py
-drwxr-xr-x   0 rjvanderent  (1000) rjvanderent  (1000)        0 2023-04-21 15:34:58.591905 wam2layers-3.0.0b4/src/wam2layers/preprocessing/
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)        0 2022-11-04 15:43:46.000000 wam2layers-3.0.0b4/src/wam2layers/preprocessing/__init__.py
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)      216 2022-12-22 15:03:20.000000 wam2layers-3.0.0b4/src/wam2layers/preprocessing/cli.py
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)    12555 2023-04-21 15:33:29.000000 wam2layers-3.0.0b4/src/wam2layers/preprocessing/era5.py
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)     9802 2022-12-22 15:03:20.000000 wam2layers-3.0.0b4/src/wam2layers/preprocessing/shared.py
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)    10385 2022-11-04 15:43:46.000000 wam2layers-3.0.0b4/src/wam2layers/preprocessing/tableERA5model_to_pressure.csv
-drwxr-xr-x   0 rjvanderent  (1000) rjvanderent  (1000)        0 2023-04-21 15:34:58.594671 wam2layers-3.0.0b4/src/wam2layers/tracking/
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)        0 2022-11-04 15:43:46.000000 wam2layers-3.0.0b4/src/wam2layers/tracking/__init__.py
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)    17248 2023-04-21 15:33:29.000000 wam2layers-3.0.0b4/src/wam2layers/tracking/backtrack.py
-drwxr-xr-x   0 rjvanderent  (1000) rjvanderent  (1000)        0 2023-04-21 15:34:58.603574 wam2layers-3.0.0b4/src/wam2layers/utils/
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)        0 2022-11-04 15:43:46.000000 wam2layers-3.0.0b4/src/wam2layers/utils/__init__.py
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)     2458 2022-12-22 15:03:20.000000 wam2layers-3.0.0b4/src/wam2layers/utils/profiling.py
-drwxr-xr-x   0 rjvanderent  (1000) rjvanderent  (1000)        0 2023-04-21 15:34:58.571311 wam2layers-3.0.0b4/src/wam2layers.egg-info/
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)     2844 2023-04-21 15:34:58.000000 wam2layers-3.0.0b4/src/wam2layers.egg-info/PKG-INFO
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)      821 2023-04-21 15:34:58.000000 wam2layers-3.0.0b4/src/wam2layers.egg-info/SOURCES.txt
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)        1 2023-04-21 15:34:58.000000 wam2layers-3.0.0b4/src/wam2layers.egg-info/dependency_links.txt
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)       50 2023-04-21 15:34:58.000000 wam2layers-3.0.0b4/src/wam2layers.egg-info/entry_points.txt
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)      238 2023-04-21 15:34:58.000000 wam2layers-3.0.0b4/src/wam2layers.egg-info/requires.txt
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)       11 2023-04-21 15:34:58.000000 wam2layers-3.0.0b4/src/wam2layers.egg-info/top_level.txt
-drwxr-xr-x   0 rjvanderent  (1000) rjvanderent  (1000)        0 2023-04-21 15:34:58.605362 wam2layers-3.0.0b4/tests/
--rw-r--r--   0 rjvanderent  (1000) rjvanderent  (1000)      442 2023-04-21 15:33:29.000000 wam2layers-3.0.0b4/tests/test_config.py
+drwxr-xr-x   0 benedicti (58930) benedicti (58450)        0 2023-07-21 14:39:21.071417 wam2layers-3.0.0b5/
+-rw-r--r--   0 benedicti (58930) benedicti (58450)    11357 2022-08-29 13:06:00.000000 wam2layers-3.0.0b5/LICENSE
+-rw-r--r--   0 benedicti (58930) benedicti (58450)     3430 2023-07-21 14:39:21.070751 wam2layers-3.0.0b5/PKG-INFO
+-rw-r--r--   0 benedicti (58930) benedicti (58450)     2640 2023-07-21 09:55:28.000000 wam2layers-3.0.0b5/README.md
+-rw-r--r--   0 benedicti (58930) benedicti (58450)     1422 2023-07-21 14:38:17.000000 wam2layers-3.0.0b5/pyproject.toml
+-rw-r--r--   0 benedicti (58930) benedicti (58450)       38 2023-07-21 14:39:21.071551 wam2layers-3.0.0b5/setup.cfg
+drwxr-xr-x   0 benedicti (58930) benedicti (58450)        0 2023-07-21 14:39:21.046168 wam2layers-3.0.0b5/src/
+drwxr-xr-x   0 benedicti (58930) benedicti (58450)        0 2023-07-21 14:39:21.052935 wam2layers-3.0.0b5/src/wam2layers/
+-rw-r--r--   0 benedicti (58930) benedicti (58450)        0 2022-09-20 13:04:20.000000 wam2layers-3.0.0b5/src/wam2layers/__init__.py
+drwxr-xr-x   0 benedicti (58930) benedicti (58450)        0 2023-07-21 14:39:21.059237 wam2layers-3.0.0b5/src/wam2layers/analysis/
+-rw-r--r--   0 benedicti (58930) benedicti (58450)        0 2022-09-20 13:04:20.000000 wam2layers-3.0.0b5/src/wam2layers/analysis/__init__.py
+-rw-rw----   0 benedicti (58930) benedicti (58450)     5181 2022-12-23 15:27:06.000000 wam2layers-3.0.0b5/src/wam2layers/analysis/checks.py
+-rw-r--r--   0 benedicti (58930) benedicti (58450)     8326 2023-07-21 14:38:17.000000 wam2layers-3.0.0b5/src/wam2layers/analysis/visualization.py
+-rw-rw----   0 benedicti (58930) benedicti (58450)      492 2022-12-23 15:27:06.000000 wam2layers-3.0.0b5/src/wam2layers/cli.py
+-rw-r--r--   0 benedicti (58930) benedicti (58450)     8578 2023-07-21 14:36:06.000000 wam2layers-3.0.0b5/src/wam2layers/config.py
+drwxr-xr-x   0 benedicti (58930) benedicti (58450)        0 2023-07-21 14:39:21.064039 wam2layers-3.0.0b5/src/wam2layers/preprocessing/
+-rw-r--r--   0 benedicti (58930) benedicti (58450)        0 2022-09-20 13:04:20.000000 wam2layers-3.0.0b5/src/wam2layers/preprocessing/__init__.py
+-rw-rw----   0 benedicti (58930) benedicti (58450)      216 2022-12-23 15:27:06.000000 wam2layers-3.0.0b5/src/wam2layers/preprocessing/cli.py
+-rw-r--r--   0 benedicti (58930) benedicti (58450)    12555 2023-07-21 14:38:17.000000 wam2layers-3.0.0b5/src/wam2layers/preprocessing/era5.py
+-rw-r--r--   0 benedicti (58930) benedicti (58450)     9801 2023-07-21 14:36:06.000000 wam2layers-3.0.0b5/src/wam2layers/preprocessing/shared.py
+-rw-r--r--   0 benedicti (58930) benedicti (58450)    10385 2022-09-20 13:04:20.000000 wam2layers-3.0.0b5/src/wam2layers/preprocessing/tableERA5model_to_pressure.csv
+drwxr-xr-x   0 benedicti (58930) benedicti (58450)        0 2023-07-21 14:39:21.065957 wam2layers-3.0.0b5/src/wam2layers/tracking/
+-rw-r--r--   0 benedicti (58930) benedicti (58450)        0 2022-09-20 13:04:20.000000 wam2layers-3.0.0b5/src/wam2layers/tracking/__init__.py
+-rw-r--r--   0 benedicti (58930) benedicti (58450)    17268 2023-07-21 09:55:28.000000 wam2layers-3.0.0b5/src/wam2layers/tracking/backtrack.py
+drwxr-xr-x   0 benedicti (58930) benedicti (58450)        0 2023-07-21 14:39:21.068892 wam2layers-3.0.0b5/src/wam2layers/utils/
+-rw-rw----   0 benedicti (58930) benedicti (58450)        0 2022-11-18 10:00:46.000000 wam2layers-3.0.0b5/src/wam2layers/utils/__init__.py
+-rw-rw----   0 benedicti (58930) benedicti (58450)     2458 2022-12-23 15:27:06.000000 wam2layers-3.0.0b5/src/wam2layers/utils/profiling.py
+-rw-r--r--   0 benedicti (58930) benedicti (58450)    11727 2023-07-21 14:36:06.000000 wam2layers-3.0.0b5/src/wam2layers/utils/source_region.py
+drwxr-xr-x   0 benedicti (58930) benedicti (58450)        0 2023-07-21 14:39:21.056499 wam2layers-3.0.0b5/src/wam2layers.egg-info/
+-rw-r--r--   0 benedicti (58930) benedicti (58450)     3430 2023-07-21 14:39:21.053706 wam2layers-3.0.0b5/src/wam2layers.egg-info/PKG-INFO
+-rw-r--r--   0 benedicti (58930) benedicti (58450)      859 2023-07-21 14:39:21.054161 wam2layers-3.0.0b5/src/wam2layers.egg-info/SOURCES.txt
+-rw-r--r--   0 benedicti (58930) benedicti (58450)        1 2023-07-21 14:39:21.054652 wam2layers-3.0.0b5/src/wam2layers.egg-info/dependency_links.txt
+-rw-r--r--   0 benedicti (58930) benedicti (58450)       50 2023-07-21 14:39:21.055310 wam2layers-3.0.0b5/src/wam2layers.egg-info/entry_points.txt
+-rw-r--r--   0 benedicti (58930) benedicti (58450)      208 2023-07-21 14:39:21.056002 wam2layers-3.0.0b5/src/wam2layers.egg-info/requires.txt
+-rw-r--r--   0 benedicti (58930) benedicti (58450)       11 2023-07-21 14:39:21.056619 wam2layers-3.0.0b5/src/wam2layers.egg-info/top_level.txt
+drwxr-xr-x   0 benedicti (58930) benedicti (58450)        0 2023-07-21 14:39:21.069981 wam2layers-3.0.0b5/tests/
+-rw-r--r--   0 benedicti (58930) benedicti (58450)      442 2023-07-21 09:36:37.000000 wam2layers-3.0.0b5/tests/test_config.py
```

### Comparing `wam2layers-3.0.0b4/LICENSE` & `wam2layers-3.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `wam2layers-3.0.0b4/PKG-INFO` & `wam2layers-3.0.0b5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,68 @@
 Metadata-Version: 2.1
 Name: wam2layers
-Version: 3.0.0b4
+Version: 3.0.0b5
 Summary: Atmospheric moisture tracking model
 License: Apache 2.0
 Project-URL: Documentation, https://wam2layers.readthedocs.io/en/latest
 Project-URL: Source code, https://github.com/WAM2layers/WAM2layers
 Keywords: atmospheric rivers,hydrological cycle,meteorology,moisture recycling,moisture tracking
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Hydrology
-Requires-Python: <3.10,>=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
 [![DOI](https://zenodo.org/badge/471007521.svg)](https://zenodo.org/badge/latestdoi/471007521)
 [![Documentation Status](https://readthedocs.org/projects/wam2layers/badge/?version=latest)](https://wam2layers.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/wam2layers)](https://pypi.org/project/wam2layers/)
 
 # Atmospheric moisture tracking
 
+https://user-images.githubusercontent.com/17080502/233834536-a82ca96d-e303-4592-a588-472097ebe6c5.mp4
+
 This repository contains the source code of the WAM2layers moisture tracking
-code. This code is currently developed by a core team:
+code. It can be used to determine where
+precipitation originally evaporated (backtracking), or where evaporated moisture
+eventually ends up (forward tracking). 
+
+The animation above illustrates the concept of backtracking: you first see the water 
+content and fluxes move forward in time (left panel). Midway through, the animation 
+reverses and the moisture from the "source region" is tracked backward in time (right panel).
+
+
+This code is currently developed by a core team:
 Ruud van der Ent (Delft University of Technology)
 Imme Benedict (Wageningen University)
 Chris Weijenborg (Wageningen University)
+Vincent de Feiter (Wageningen University)
 Peter Kalverla (Netherlands eScienceCenter)
 
-It can be used to determine where
-precipitation originally evaporated (backtracking), or where evaporated moisture
-eventually ends up (forward tracking).
-
 # How to use
-See the [documentation](http://wam2layers.rtfd.io/) for a more detailed description.
+See the [documentation](https://wam2layers.readthedocs.io/en/latest/) for a more detailed description. Still questions? Follow the flowchart below.
+
+![FlowChart GitHub](https://github.com/WAM2layers/WAM2layers/assets/123247866/f5cbcf8f-a45f-4e73-b304-00956b4e2ee5)
+
 
-## Other versions
+# Other versions
 
 This is the official codebase for the WAM-2layers moisture tracking model as of
 18/03/2022, but there are still several other older versions around:
 
 - [Original Python code for ERA-Interim by Ruud van der Ent](https://github.com/ruudvdent/WAM2layersPython)
 - [Adapted version for EC-Earth by Imme Benedict](https://github.com/Imme1992/moisture_tracking_mississippi)
 - [Adapted version for MERRA2 by Pat Keys](https://github.com/pkeys/WAM2layersPythonMerra2)
 - [Adapted version for ERA5 pressure levels by Mingzhong Xiao](https://zenodo.org/record/4796962#.Y25d1-TMIVA)
 
-## Reuse and acknowledgement
+# Reuse and acknowledgement
 
 We are actively developing the code at the moment, so it may be subject to
 change. We encourage anyone who is interested in re-using the code to get in
 touch. We may be able to help.
 
 If you use the code for a publication, please cite it using the [DOI of the
 appropriate release](https://doi.org/10.5281/zenodo.7010594) and the
```

### Comparing `wam2layers-3.0.0b4/README.md` & `wam2layers-3.0.0b5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,49 @@
 [![DOI](https://zenodo.org/badge/471007521.svg)](https://zenodo.org/badge/latestdoi/471007521)
 [![Documentation Status](https://readthedocs.org/projects/wam2layers/badge/?version=latest)](https://wam2layers.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/wam2layers)](https://pypi.org/project/wam2layers/)
 
 # Atmospheric moisture tracking
 
+https://user-images.githubusercontent.com/17080502/233834536-a82ca96d-e303-4592-a588-472097ebe6c5.mp4
+
 This repository contains the source code of the WAM2layers moisture tracking
-code. This code is currently developed by a core team:
+code. It can be used to determine where
+precipitation originally evaporated (backtracking), or where evaporated moisture
+eventually ends up (forward tracking). 
+
+The animation above illustrates the concept of backtracking: you first see the water 
+content and fluxes move forward in time (left panel). Midway through, the animation 
+reverses and the moisture from the "source region" is tracked backward in time (right panel).
+
+
+This code is currently developed by a core team:
 Ruud van der Ent (Delft University of Technology)
 Imme Benedict (Wageningen University)
 Chris Weijenborg (Wageningen University)
+Vincent de Feiter (Wageningen University)
 Peter Kalverla (Netherlands eScienceCenter)
 
-It can be used to determine where
-precipitation originally evaporated (backtracking), or where evaporated moisture
-eventually ends up (forward tracking).
-
 # How to use
-See the [documentation](http://wam2layers.rtfd.io/) for a more detailed description.
+See the [documentation](https://wam2layers.readthedocs.io/en/latest/) for a more detailed description. Still questions? Follow the flowchart below.
+
+![FlowChart GitHub](https://github.com/WAM2layers/WAM2layers/assets/123247866/f5cbcf8f-a45f-4e73-b304-00956b4e2ee5)
+
 
-## Other versions
+# Other versions
 
 This is the official codebase for the WAM-2layers moisture tracking model as of
 18/03/2022, but there are still several other older versions around:
 
 - [Original Python code for ERA-Interim by Ruud van der Ent](https://github.com/ruudvdent/WAM2layersPython)
 - [Adapted version for EC-Earth by Imme Benedict](https://github.com/Imme1992/moisture_tracking_mississippi)
 - [Adapted version for MERRA2 by Pat Keys](https://github.com/pkeys/WAM2layersPythonMerra2)
 - [Adapted version for ERA5 pressure levels by Mingzhong Xiao](https://zenodo.org/record/4796962#.Y25d1-TMIVA)
 
-## Reuse and acknowledgement
+# Reuse and acknowledgement
 
 We are actively developing the code at the moment, so it may be subject to
 change. We encourage anyone who is interested in re-using the code to get in
 touch. We may be able to help.
 
 If you use the code for a publication, please cite it using the [DOI of the
 appropriate release](https://doi.org/10.5281/zenodo.7010594) and the
```

### Comparing `wam2layers-3.0.0b4/pyproject.toml` & `wam2layers-3.0.0b5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wam2layers"
 description = "Atmospheric moisture tracking model"
-version = "3.0.0-beta.4"
+version = "3.0.0-beta.5"
 readme = "README.md"
 license = { text = "Apache 2.0" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
@@ -19,41 +19,42 @@
 keywords = [
   "atmospheric rivers",
   "hydrological cycle",
   "meteorology",
   "moisture recycling",
   "moisture tracking",
 ]
-requires-python = ">=3.8,<3.10"
+requires-python = ">=3.8"
 dependencies = [
     "numpy",
     "pyyaml",
     "scipy",
-    "pandas>=1.4.0",
-    "xarray", # or xarray[io,parallel,complete,...]
+    "pandas",
+    "xarray",
     "netcdf4",
     "scipy",
     "click",
     "pydantic",
-    "dask>=2022.11",
-    "distributed>=2022.11",
+    "dask",
+    "distributed",
     "psutil",
     "matplotlib",
     "cmocean",
+    "regionmask",
 ]
 
 [project.optional-dependencies]
 develop = [
     "black",
     "cffconvert",
     "isort",
     "myst-nb",
     "sphinx_rtd_theme",
     "sphinx",
-    "myst-nb==0.16.0",
+    "myst-nb",
     "pytest",
     "flake8",
     "build",
     "twine",
 ]
 
 [project.urls]
```

### Comparing `wam2layers-3.0.0b4/src/wam2layers/analysis/checks.py` & `wam2layers-3.0.0b5/src/wam2layers/analysis/checks.py`

 * *Files identical despite different names*

### Comparing `wam2layers-3.0.0b4/src/wam2layers/analysis/visualization.py` & `wam2layers-3.0.0b5/src/wam2layers/analysis/visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,15 @@
     # Load config and some usful stuf.
     region = load_region(config)
 
     # Load data
     dates = pd.date_range(
         start=config.preprocess_start_date,
         end=config.preprocess_end_date,
-        freq=config[
-            "output_frequency"
-        ],  # Should be output frequency, since this is used to save the data
+        freq=config.output_frequency,  # Should be output frequency, since this is used to save the data
         inclusive="left",
     )
 
     input_files = []
     for date in dates:
         input_files.append(input_path(date, config))
```

### Comparing `wam2layers-3.0.0b4/src/wam2layers/config.py` & `wam2layers-3.0.0b5/src/wam2layers/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from pydantic import BaseModel, FilePath, validator, root_validator
-import yaml
 from datetime import datetime
 from pathlib import Path
-from typing import Literal, Union
+from typing import Dict, List, Literal, Optional, Union
 
 import yaml
-from pydantic import BaseModel, FilePath, validator
+from pydantic import BaseModel, ConfigDict, FilePath, field_validator, model_validator
 
 
 class Config(BaseModel):
+    # Pydantic configuration
+    model_config = ConfigDict(validate_assignment=True)
+
+    # Configuration settings
     filename_template: str
     """The filename pattern of the raw input data.
 
     Used to find the input files during preprocessing. The pattern will be
     interpreted during execution of the model to find the input data for each
     date and variable.
 
@@ -210,15 +212,15 @@
 
     .. code-block:: yaml
 
         level_type: model_levels
 
     """
 
-    levels: "Union[list[int], Literal['All']]"
+    levels: "Union[List[int], Literal['All']]"
     """Which levels to use from the raw input data.
 
     A list of integers corresponding to the levels in the input data, or a
     subset thereof. Shorthand `"all"` will attempt to use all 137 ERA5 levels.
 
     For example:
 
@@ -272,15 +274,15 @@
 
     .. code-block:: yaml
 
         kvf: 3
 
     """
 
-    chunks: "Union[None, dict[str, int]]"
+    chunks: Optional[Dict[str, int]]
     """Whether to use dask.
 
     Using dask can help process large datasets without memory issues, but its
     performance is quite sensitive to the chunk configuration.
 
     Some examples:
 
@@ -315,40 +317,34 @@
 
         """
         with open(config_file) as f:
             settings = yaml.safe_load(f)
 
         return cls(**settings)
 
-    @validator("preprocessed_data_folder", "region", "output_folder")
+    @field_validator("preprocessed_data_folder", "region", "output_folder")
+    @classmethod
     def _expanduser(cls, path):
         """Resolve ~ in input paths."""
         return path.expanduser()
 
-    @validator("preprocessed_data_folder", "output_folder")
+    @field_validator("preprocessed_data_folder", "output_folder")
+    @classmethod
     def _make_dir(cls, path):
         """Create output dirs if they don't exist yet."""
         if not path.exists():
             print(f"Creating output folder {path}")
             path.mkdir(parents=True)
         return path
 
-    @root_validator
-    def check_date_order(cls, values):
-        for date_field in ['track', 'event', 'preprocess']:
-            start = values.get(f'{date_field}_start_date')
-            end = values.get(f'{date_field}_end_date')
-
-            if not start < end:
-                raise ValueError("End date should be later than start date.")
-
-        return values
-
-    class Config:
-        """This is the config of the **Pydantic** class, not the wam2layers config.
-
-        Note: this will change in v2
-        https://docs.pydantic.dev/blog/pydantic-v2-alpha/#changes-to-config
-        """
-        # Also force validation when new value is set on existing config
-        validate_assignment = True
+    @model_validator(mode="after")
+    def check_date_order(self):
+        if self.track_start_date > self.track_end_date:
+            raise ValueError("track_end_date should be later than track_start_date")
+        if self.event_start_date > self.event_end_date:
+            raise ValueError("event_end_date should be later than event_start_date")
+        if self.preprocess_start_date > self.preprocess_end_date:
+            raise ValueError(
+                "preprocess_end_date should be later than preprocess_start_date"
+            )
 
+        return self
```

### Comparing `wam2layers-3.0.0b4/src/wam2layers/preprocessing/era5.py` & `wam2layers-3.0.0b5/src/wam2layers/preprocessing/era5.py`

 * *Files identical despite different names*

### Comparing `wam2layers-3.0.0b4/src/wam2layers/preprocessing/shared.py` & `wam2layers-3.0.0b5/src/wam2layers/preprocessing/shared.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,14 @@
     new_var = np.zeros_like(new_pressure_levels)
 
     ntime, _, nlat, nlon = old_var.shape
 
     for t in range(ntime):
         for i in range(nlat):
             for j in range(nlon):
-
                 pressure_1d = old_pressure_levels[t, :, i, j]
                 var_1d = old_var[t, :, i, j]
 
                 pressure_1d = pressure_1d[~pressure_1d.mask]
                 var_1d = var_1d[~var_1d.mask]
 
                 f_q = interp1d(pressure_1d, var_1d, type)
```

### Comparing `wam2layers-3.0.0b4/src/wam2layers/preprocessing/tableERA5model_to_pressure.csv` & `wam2layers-3.0.0b5/src/wam2layers/preprocessing/tableERA5model_to_pressure.csv`

 * *Files identical despite different names*

### Comparing `wam2layers-3.0.0b4/src/wam2layers/tracking/backtrack.py` & `wam2layers-3.0.0b5/src/wam2layers/tracking/backtrack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from functools import lru_cache
-from pathlib import Path
 
 import click
 import numpy as np
 import pandas as pd
 import xarray as xr
-import yaml
 
 from wam2layers.config import Config
 from wam2layers.preprocessing.shared import get_grid_info
-from wam2layers.utils.profiling import Profiler, ProgressTracker
+from wam2layers.utils.profiling import ProgressTracker
 
 
 def get_tracking_dates(config):
     """Dates for tracking."""
     # E.g. if data from 00:00 to 23:00
     # Using target freq directly would end at 23:45 or so
     input_dates = pd.date_range(
@@ -33,15 +31,15 @@
 def input_path(date, config):
     input_dir = config.preprocessed_data_folder
     return f"{input_dir}/{date.strftime('%Y-%m-%d')}_fluxes_storages.nc"
 
 
 def output_path(date, config):
     output_dir = config.output_folder
-    return f"{output_dir}/{date.strftime('%Y-%m-%d')}_s_track.nc"
+    return f"{output_dir}/backtrack_{date.strftime('%Y-%m-%dT%H:%M')}.nc"
 
 
 # LRU Cache keeps the file open so we save a bit on I/O
 @lru_cache(maxsize=2)
 def read_data_at_date(d):
     """Load input data for given date."""
     file = input_path(d, config)
@@ -279,15 +277,14 @@
 def backtrack(
     fluxes,
     states_prev,
     states_next,
     region,
     output,
 ):
-
     # Unpack input data
     fx_upper = fluxes["fx_upper"].values
     fy_upper = fluxes["fy_upper"].values
     fx_lower = fluxes["fx_lower"].values
     fy_lower = fluxes["fy_lower"].values
     evap = fluxes["evap"].values
     precip = fluxes["precip"].values
@@ -466,15 +463,14 @@
 
     config, region, output = initialize(config_file)
 
     tracking_dates = get_tracking_dates(config)
 
     progress_tracker = ProgressTracker(output)
     for t in reversed(tracking_dates):
-
         fluxes = load_fluxes(t)
         states_prev, states_next = load_states(t)
 
         # Convert data to volumes
         change_units(states_prev, config.target_frequency)
         change_units(states_next, config.target_frequency)
         change_units(fluxes, config.target_frequency)
@@ -501,19 +497,21 @@
             states_prev,
             states_next,
             region,
             output,
         )
 
         # Daily output
-        if t == t.floor(config.output_frequency):
+        if t == t.floor(config.output_frequency) or t == tracking_dates[0]:
             progress_tracker.print_progress(t, output)
             progress_tracker.store_intermediate_states(output)
             write_output(output, t)
 
+    print("Experiment complete.")
+
 
 ###########################################################################
 # The code below makes it possible to run wam2layers from the command line:
 # >>> python backtrack.py path/to/cases/era5_2021.yaml
 # or even:
 # >>> wam2layers backtrack path/to/cases/era5_2021.yaml
 ###########################################################################
```

### Comparing `wam2layers-3.0.0b4/src/wam2layers/utils/profiling.py` & `wam2layers-3.0.0b5/src/wam2layers/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `wam2layers-3.0.0b4/src/wam2layers.egg-info/PKG-INFO` & `wam2layers-3.0.0b5/src/wam2layers.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,68 @@
 Metadata-Version: 2.1
 Name: wam2layers
-Version: 3.0.0b4
+Version: 3.0.0b5
 Summary: Atmospheric moisture tracking model
 License: Apache 2.0
 Project-URL: Documentation, https://wam2layers.readthedocs.io/en/latest
 Project-URL: Source code, https://github.com/WAM2layers/WAM2layers
 Keywords: atmospheric rivers,hydrological cycle,meteorology,moisture recycling,moisture tracking
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Hydrology
-Requires-Python: <3.10,>=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
 [![DOI](https://zenodo.org/badge/471007521.svg)](https://zenodo.org/badge/latestdoi/471007521)
 [![Documentation Status](https://readthedocs.org/projects/wam2layers/badge/?version=latest)](https://wam2layers.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/wam2layers)](https://pypi.org/project/wam2layers/)
 
 # Atmospheric moisture tracking
 
+https://user-images.githubusercontent.com/17080502/233834536-a82ca96d-e303-4592-a588-472097ebe6c5.mp4
+
 This repository contains the source code of the WAM2layers moisture tracking
-code. This code is currently developed by a core team:
+code. It can be used to determine where
+precipitation originally evaporated (backtracking), or where evaporated moisture
+eventually ends up (forward tracking). 
+
+The animation above illustrates the concept of backtracking: you first see the water 
+content and fluxes move forward in time (left panel). Midway through, the animation 
+reverses and the moisture from the "source region" is tracked backward in time (right panel).
+
+
+This code is currently developed by a core team:
 Ruud van der Ent (Delft University of Technology)
 Imme Benedict (Wageningen University)
 Chris Weijenborg (Wageningen University)
+Vincent de Feiter (Wageningen University)
 Peter Kalverla (Netherlands eScienceCenter)
 
-It can be used to determine where
-precipitation originally evaporated (backtracking), or where evaporated moisture
-eventually ends up (forward tracking).
-
 # How to use
-See the [documentation](http://wam2layers.rtfd.io/) for a more detailed description.
+See the [documentation](https://wam2layers.readthedocs.io/en/latest/) for a more detailed description. Still questions? Follow the flowchart below.
+
+![FlowChart GitHub](https://github.com/WAM2layers/WAM2layers/assets/123247866/f5cbcf8f-a45f-4e73-b304-00956b4e2ee5)
+
 
-## Other versions
+# Other versions
 
 This is the official codebase for the WAM-2layers moisture tracking model as of
 18/03/2022, but there are still several other older versions around:
 
 - [Original Python code for ERA-Interim by Ruud van der Ent](https://github.com/ruudvdent/WAM2layersPython)
 - [Adapted version for EC-Earth by Imme Benedict](https://github.com/Imme1992/moisture_tracking_mississippi)
 - [Adapted version for MERRA2 by Pat Keys](https://github.com/pkeys/WAM2layersPythonMerra2)
 - [Adapted version for ERA5 pressure levels by Mingzhong Xiao](https://zenodo.org/record/4796962#.Y25d1-TMIVA)
 
-## Reuse and acknowledgement
+# Reuse and acknowledgement
 
 We are actively developing the code at the moment, so it may be subject to
 change. We encourage anyone who is interested in re-using the code to get in
 touch. We may be able to help.
 
 If you use the code for a publication, please cite it using the [DOI of the
 appropriate release](https://doi.org/10.5281/zenodo.7010594) and the
```

### Comparing `wam2layers-3.0.0b4/src/wam2layers.egg-info/SOURCES.txt` & `wam2layers-3.0.0b5/src/wam2layers.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 src/wam2layers/preprocessing/era5.py
 src/wam2layers/preprocessing/shared.py
 src/wam2layers/preprocessing/tableERA5model_to_pressure.csv
 src/wam2layers/tracking/__init__.py
 src/wam2layers/tracking/backtrack.py
 src/wam2layers/utils/__init__.py
 src/wam2layers/utils/profiling.py
+src/wam2layers/utils/source_region.py
 tests/test_config.py
```

