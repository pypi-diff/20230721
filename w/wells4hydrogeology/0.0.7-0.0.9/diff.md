# Comparing `tmp/wells4hydrogeology-0.0.7.tar.gz` & `tmp/wells4hydrogeology-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wells4hydrogeology-0.0.7.tar", last modified: Wed Jul 19 22:07:44 2023, max compression
+gzip compressed data, was "wells4hydrogeology-0.0.9.tar", last modified: Thu Jul 20 20:18:13 2023, max compression
```

## Comparing `wells4hydrogeology-0.0.7.tar` & `wells4hydrogeology-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:07:44.082404 wells4hydrogeology-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-19 22:07:32.000000 wells4hydrogeology-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-07-19 22:07:44.082404 wells4hydrogeology-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-19 22:07:32.000000 wells4hydrogeology-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-19 22:07:32.000000 wells4hydrogeology-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 22:07:44.082404 wells4hydrogeology-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-19 22:07:32.000000 wells4hydrogeology-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:07:44.082404 wells4hydrogeology-0.0.7/w4h/
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-19 22:07:32.000000 wells4hydrogeology-0.0.7/w4h/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16301 2023-07-19 22:07:32.000000 wells4hydrogeology-0.0.7/w4h/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-07-19 22:07:32.000000 wells4hydrogeology-0.0.7/w4h/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    24888 2023-07-19 22:07:32.000000 wells4hydrogeology-0.0.7/w4h/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-07-19 22:07:32.000000 wells4hydrogeology-0.0.7/w4h/export.py
--rw-r--r--   0 runner    (1001) docker     (123)    25324 2023-07-19 22:07:32.000000 wells4hydrogeology-0.0.7/w4h/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    29779 2023-07-19 22:07:32.000000 wells4hydrogeology-0.0.7/w4h/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    30609 2023-07-19 22:07:32.000000 wells4hydrogeology-0.0.7/w4h/read.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:07:44.082404 wells4hydrogeology-0.0.7/wells4hydrogeology.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-07-19 22:07:44.000000 wells4hydrogeology-0.0.7/wells4hydrogeology.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-19 22:07:44.000000 wells4hydrogeology-0.0.7/wells4hydrogeology.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 22:07:44.000000 wells4hydrogeology-0.0.7/wells4hydrogeology.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-19 22:07:44.000000 wells4hydrogeology-0.0.7/wells4hydrogeology.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-19 22:07:44.000000 wells4hydrogeology-0.0.7/wells4hydrogeology.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:18:13.263711 wells4hydrogeology-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-20 20:17:57.000000 wells4hydrogeology-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-07-20 20:18:13.263711 wells4hydrogeology-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-20 20:17:57.000000 wells4hydrogeology-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-20 20:17:57.000000 wells4hydrogeology-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 20:18:13.263711 wells4hydrogeology-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-20 20:17:57.000000 wells4hydrogeology-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:18:13.263711 wells4hydrogeology-0.0.9/w4h/
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-20 20:17:57.000000 wells4hydrogeology-0.0.9/w4h/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16301 2023-07-20 20:17:57.000000 wells4hydrogeology-0.0.9/w4h/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-07-20 20:17:57.000000 wells4hydrogeology-0.0.9/w4h/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24888 2023-07-20 20:17:57.000000 wells4hydrogeology-0.0.9/w4h/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-07-20 20:17:57.000000 wells4hydrogeology-0.0.9/w4h/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25324 2023-07-20 20:17:57.000000 wells4hydrogeology-0.0.9/w4h/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30309 2023-07-20 20:17:57.000000 wells4hydrogeology-0.0.9/w4h/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30609 2023-07-20 20:17:57.000000 wells4hydrogeology-0.0.9/w4h/read.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:18:13.263711 wells4hydrogeology-0.0.9/w4h/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-20 20:17:57.000000 wells4hydrogeology-0.0.9/w4h/resources/resReadme.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:17:57.000000 wells4hydrogeology-0.0.9/w4h/resources/resource_home.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-07-20 20:17:57.000000 wells4hydrogeology-0.0.9/w4h/resources/temp4wiki.md
+-rw-r--r--   0 runner    (1001) docker     (123)    21040 2023-07-20 20:17:57.000000 wells4hydrogeology-0.0.9/w4h/resources/uniqueparameters.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:18:13.263711 wells4hydrogeology-0.0.9/wells4hydrogeology.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-07-20 20:18:13.000000 wells4hydrogeology-0.0.9/wells4hydrogeology.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-20 20:18:13.000000 wells4hydrogeology-0.0.9/wells4hydrogeology.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 20:18:13.000000 wells4hydrogeology-0.0.9/wells4hydrogeology.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-20 20:18:13.000000 wells4hydrogeology-0.0.9/wells4hydrogeology.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-20 20:18:13.000000 wells4hydrogeology-0.0.9/wells4hydrogeology.egg-info/top_level.txt
```

### Comparing `wells4hydrogeology-0.0.7/LICENSE` & `wells4hydrogeology-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wells4hydrogeology-0.0.7/PKG-INFO` & `wells4hydrogeology-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wells4hydrogeology
-Version: 0.0.7
+Version: 0.0.9
 Summary: A package to read in geology data from wells and create a layered, gridded hydrogeologic model of a study region, all within a python environment, automating and performing tasks often carried out in a dedicated GIS software.
 Author: Riley Balikian
 Author-email: balikian@illinois.edu
 License: MIT License
         
         Copyright (c) 2023 RJbalikian
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wells4hydrogeology Version: 0.0.7 Summary: A
+Metadata-Version: 2.1 Name: wells4hydrogeology Version: 0.0.9 Summary: A
 package to read in geology data from wells and create a layered, gridded
 hydrogeologic model of a study region, all within a python environment,
 automating and performing tasks often carried out in a dedicated GIS software.
 Author: Riley Balikian Author-email: balikian@illinois.edu License: MIT License
 Copyright (c) 2023 RJbalikian Permission is hereby granted, free of charge, to
 any person obtaining a copy of this software and associated documentation files
 (the "Software"), to deal in the Software without restriction, including
```

### Comparing `wells4hydrogeology-0.0.7/README.md` & `wells4hydrogeology-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `wells4hydrogeology-0.0.7/pyproject.toml` & `wells4hydrogeology-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wells4hydrogeology"
 dynamic = ["readme"]
 license = {file = "LICENSE"}
-version="0.0.7"
+version="0.0.9"
 description = "A package to read in geology data from wells and create a layered, gridded hydrogeologic model of a study region, all within a python environment, automating and performing tasks often carried out in a dedicated GIS software."
 keywords = ["hydrogeology", "modflow", "water wells", "geology", 'water', 'geotechnical']
 requires-python = "<3.13, >=3.9"
 dependencies =  ["geopandas", "rioxarray", "owslib", "scipy", "matplotlib", "pandas", "numpy"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Intended Audience :: Science/Research",
```

### Comparing `wells4hydrogeology-0.0.7/setup.py` & `wells4hydrogeology-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,13 +4,14 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="wells4hydrogeology",
     author= "Riley Balikian",
     author_email = "balikian@illinois.edu",
-    version="0.0.7",
+    version="0.0.9",
     install_requires=["geopandas", "rioxarray", "owslib", "scipy", "matplotlib", "pandas", "numpy"],
     long_description = long_description,
     long_description_content_type="text/markdown",
-    description="A package to read in geology data from wells and create a layered, gridded hydrogeologic model of a study region, all within a python environment, automating and performing tasks often carried out in a dedicated GIS software."
+    description="A package to read in geology data from wells and create a layered, gridded hydrogeologic model of a study region, all within a python environment, automating and performing tasks often carried out in a dedicated GIS software.",
+    package_data={'w4h': ['resources/*']}
     )
```

### Comparing `wells4hydrogeology-0.0.7/w4h/__init__.py` & `wells4hydrogeology-0.0.9/w4h/__init__.py`

 * *Files identical despite different names*

### Comparing `wells4hydrogeology-0.0.7/w4h/classify.py` & `wells4hydrogeology-0.0.9/w4h/classify.py`

 * *Files identical despite different names*

### Comparing `wells4hydrogeology-0.0.7/w4h/clean.py` & `wells4hydrogeology-0.0.9/w4h/clean.py`

 * *Files identical despite different names*

### Comparing `wells4hydrogeology-0.0.7/w4h/core.py` & `wells4hydrogeology-0.0.9/w4h/core.py`

 * *Files identical despite different names*

### Comparing `wells4hydrogeology-0.0.7/w4h/export.py` & `wells4hydrogeology-0.0.9/w4h/export.py`

 * *Files identical despite different names*

### Comparing `wells4hydrogeology-0.0.7/w4h/layers.py` & `wells4hydrogeology-0.0.9/w4h/layers.py`

 * *Files identical despite different names*

### Comparing `wells4hydrogeology-0.0.7/w4h/mapping.py` & `wells4hydrogeology-0.0.9/w4h/mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -528,25 +528,32 @@
         Data array containing model grid
     """
     logger_function(log, locals(), inspect.currentframe().f_code.co_name)
     
     if read_grid and model_grid_path is not None:
         modelGridIN = rxr.open_rasterio(model_grid_path)
 
-        file = w4h.read.__get_resource_path('isws_crs.txt')
-        iswsCRS = w4h.read_dict(file, keytype=None)
-
         if grid_crs is None:
             try:
                 grid_crs=modelGridIN.spatial_ref.crs_wkt
             except:
-                modelGridIN.rio.write_crs(iswsCRS)
-        elif grid_crs.lower()=='isws':
-            modelGridIN.rio.write_crs(iswsCRS)
-        
+                file = w4h.read.__get_resource_path('isws_crs.txt')
+                iswsCRS = w4h.read_dict(file, keytype=None)
+                grid_crs = iswsCRS              
+                modelGridIN.rio.write_crs(grid_crs)
+        elif isinstance(grid_crs, str) and grid_crs.lower()=='isws':
+            file = w4h.read.__get_resource_path('isws_crs.txt')
+            iswsCRS = w4h.read_dict(file, keytype=None)            
+            grid_crs = iswsCRS              
+            modelGridIN.rio.write_crs(grid_crs)
+        elif isinstance(grid_crs, pathlib.PurePath) or (isinstance(grid_crs, str) and pathlib.Path(grid_crs).exists()):
+            file = grid_crs
+            grid_crs = w4h.read_dict(file, keytype=None)            
+            modelGridIN.rio.write_crs(grid_crs)
+
         if study_area is not None:                
             if study_area_crs is None:
                 study_area_crs=study_area.crs
             study_area = study_area.to_crs(grid_crs)
             study_area_crs=study_area.crs            
             modelGrid = grid2study_area(study_area=study_area, grid=modelGridIN, study_area_crs=study_area_crs, grid_crs=grid_crs)
         else:
```

### Comparing `wells4hydrogeology-0.0.7/w4h/read.py` & `wells4hydrogeology-0.0.9/w4h/read.py`

 * *Files identical despite different names*

### Comparing `wells4hydrogeology-0.0.7/wells4hydrogeology.egg-info/PKG-INFO` & `wells4hydrogeology-0.0.9/wells4hydrogeology.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wells4hydrogeology
-Version: 0.0.7
+Version: 0.0.9
 Summary: A package to read in geology data from wells and create a layered, gridded hydrogeologic model of a study region, all within a python environment, automating and performing tasks often carried out in a dedicated GIS software.
 Author: Riley Balikian
 Author-email: balikian@illinois.edu
 License: MIT License
         
         Copyright (c) 2023 RJbalikian
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wells4hydrogeology Version: 0.0.7 Summary: A
+Metadata-Version: 2.1 Name: wells4hydrogeology Version: 0.0.9 Summary: A
 package to read in geology data from wells and create a layered, gridded
 hydrogeologic model of a study region, all within a python environment,
 automating and performing tasks often carried out in a dedicated GIS software.
 Author: Riley Balikian Author-email: balikian@illinois.edu License: MIT License
 Copyright (c) 2023 RJbalikian Permission is hereby granted, free of charge, to
 any person obtaining a copy of this software and associated documentation files
 (the "Software"), to deal in the Software without restriction, including
```

