# Comparing `tmp/mcu-geo-utils-0.3.tar.gz` & `tmp/mcu-geo-utils-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcu-geo-utils-0.3.tar", last modified: Thu Jul 20 20:05:17 2023, max compression
+gzip compressed data, was "mcu-geo-utils-0.4.tar", last modified: Fri Jul 21 19:27:14 2023, max compression
```

## Comparing `mcu-geo-utils-0.3.tar` & `mcu-geo-utils-0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 martincontreras   (501) staff       (20)        0 2023-07-20 20:05:17.270346 mcu-geo-utils-0.3/
--rw-r--r--   0 martincontreras   (501) staff       (20)     1075 2023-07-20 16:07:16.000000 mcu-geo-utils-0.3/LICENSE
--rw-r--r--   0 martincontreras   (501) staff       (20)       32 2023-07-19 20:10:43.000000 mcu-geo-utils-0.3/MANIFEST.in
--rw-r--r--   0 martincontreras   (501) staff       (20)      427 2023-07-20 20:05:17.270219 mcu-geo-utils-0.3/PKG-INFO
--rw-r--r--   0 martincontreras   (501) staff       (20)      144 2023-07-20 20:03:40.000000 mcu-geo-utils-0.3/README.md
-drwxr-xr-x   0 martincontreras   (501) staff       (20)        0 2023-07-20 20:05:17.269444 mcu-geo-utils-0.3/mcu_geo_utils/
--rw-r--r--   0 martincontreras   (501) staff       (20)     2045 2023-07-20 19:24:45.000000 mcu-geo-utils-0.3/mcu_geo_utils/OSM.py
--rw-r--r--   0 martincontreras   (501) staff       (20)      191 2023-07-19 19:51:00.000000 mcu-geo-utils-0.3/mcu_geo_utils/__init__.py
--rw-r--r--   0 martincontreras   (501) staff       (20)     3621 2023-07-20 15:51:36.000000 mcu-geo-utils-0.3/mcu_geo_utils/census.py
-drwxr-xr-x   0 martincontreras   (501) staff       (20)        0 2023-07-20 20:05:17.270049 mcu-geo-utils-0.3/mcu_geo_utils.egg-info/
--rw-r--r--   0 martincontreras   (501) staff       (20)      427 2023-07-20 20:05:17.000000 mcu-geo-utils-0.3/mcu_geo_utils.egg-info/PKG-INFO
--rw-r--r--   0 martincontreras   (501) staff       (20)      293 2023-07-20 20:05:17.000000 mcu-geo-utils-0.3/mcu_geo_utils.egg-info/SOURCES.txt
--rw-r--r--   0 martincontreras   (501) staff       (20)        1 2023-07-20 20:05:17.000000 mcu-geo-utils-0.3/mcu_geo_utils.egg-info/dependency_links.txt
--rw-r--r--   0 martincontreras   (501) staff       (20)       58 2023-07-20 20:05:17.000000 mcu-geo-utils-0.3/mcu_geo_utils.egg-info/requires.txt
--rw-r--r--   0 martincontreras   (501) staff       (20)       14 2023-07-20 20:05:17.000000 mcu-geo-utils-0.3/mcu_geo_utils.egg-info/top_level.txt
--rw-r--r--   0 martincontreras   (501) staff       (20)       38 2023-07-20 20:05:17.270389 mcu-geo-utils-0.3/setup.cfg
--rw-r--r--   0 martincontreras   (501) staff       (20)      562 2023-07-20 20:03:13.000000 mcu-geo-utils-0.3/setup.py
+drwxr-xr-x   0 martincontreras   (501) staff       (20)        0 2023-07-21 19:27:14.237670 mcu-geo-utils-0.4/
+-rw-r--r--   0 martincontreras   (501) staff       (20)     1075 2023-07-20 16:07:16.000000 mcu-geo-utils-0.4/LICENSE
+-rw-r--r--   0 martincontreras   (501) staff       (20)       32 2023-07-19 20:10:43.000000 mcu-geo-utils-0.4/MANIFEST.in
+-rw-r--r--   0 martincontreras   (501) staff       (20)      427 2023-07-21 19:27:14.237541 mcu-geo-utils-0.4/PKG-INFO
+-rw-r--r--   0 martincontreras   (501) staff       (20)      144 2023-07-20 20:03:40.000000 mcu-geo-utils-0.4/README.md
+drwxr-xr-x   0 martincontreras   (501) staff       (20)        0 2023-07-21 19:27:14.236766 mcu-geo-utils-0.4/mcu_geo_utils/
+-rw-r--r--   0 martincontreras   (501) staff       (20)     2045 2023-07-20 19:24:45.000000 mcu-geo-utils-0.4/mcu_geo_utils/OSM.py
+-rw-r--r--   0 martincontreras   (501) staff       (20)      191 2023-07-19 19:51:00.000000 mcu-geo-utils-0.4/mcu_geo_utils/__init__.py
+-rw-r--r--   0 martincontreras   (501) staff       (20)     3637 2023-07-21 19:25:05.000000 mcu-geo-utils-0.4/mcu_geo_utils/census.py
+drwxr-xr-x   0 martincontreras   (501) staff       (20)        0 2023-07-21 19:27:14.237364 mcu-geo-utils-0.4/mcu_geo_utils.egg-info/
+-rw-r--r--   0 martincontreras   (501) staff       (20)      427 2023-07-21 19:27:14.000000 mcu-geo-utils-0.4/mcu_geo_utils.egg-info/PKG-INFO
+-rw-r--r--   0 martincontreras   (501) staff       (20)      293 2023-07-21 19:27:14.000000 mcu-geo-utils-0.4/mcu_geo_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 martincontreras   (501) staff       (20)        1 2023-07-21 19:27:14.000000 mcu-geo-utils-0.4/mcu_geo_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 martincontreras   (501) staff       (20)       58 2023-07-21 19:27:14.000000 mcu-geo-utils-0.4/mcu_geo_utils.egg-info/requires.txt
+-rw-r--r--   0 martincontreras   (501) staff       (20)       14 2023-07-21 19:27:14.000000 mcu-geo-utils-0.4/mcu_geo_utils.egg-info/top_level.txt
+-rw-r--r--   0 martincontreras   (501) staff       (20)       38 2023-07-21 19:27:14.237713 mcu-geo-utils-0.4/setup.cfg
+-rw-r--r--   0 martincontreras   (501) staff       (20)      562 2023-07-21 19:27:01.000000 mcu-geo-utils-0.4/setup.py
```

### Comparing `mcu-geo-utils-0.3/LICENSE` & `mcu-geo-utils-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mcu-geo-utils-0.3/mcu_geo_utils/OSM.py` & `mcu-geo-utils-0.4/mcu_geo_utils/OSM.py`

 * *Files identical despite different names*

### Comparing `mcu-geo-utils-0.3/mcu_geo_utils/census.py` & `mcu-geo-utils-0.4/mcu_geo_utils/census.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 # TODO:
 # 1: CHECK IF 18S OR 19S SHOULD APPLY
 
 
 def get_census_dataset() -> gpd.GeoDataFrame:
     os.makedirs("data", exist_ok=True)
-    file = wget.download("https://github.com/martin-conur/geo_utils/blob/main/geo_utils/data/info_manzanas_censo2017.feather?raw=True", out="data/info_manzanas_censo2017.feather")
+    file = wget.download("https://github.com/martin-conur/mcu_geo_utils/blob/main/mcu_geo_utils/data/info_manzanas_censo2017.feather?raw=True", out="data/info_manzanas_censo2017.feather")
     return gpd.read_feather(file)
 
 
 def get_ismt_dataset() -> gpd.GeoDataFrame:
     os.makedirs("data", exist_ok=True)
-    file = wget.download("https://github.com/martin-conur/geo_utils/blob/main/geo_utils/data/ISMT_2022_actualizado_simplificado.feather?raw=True", out="data/ISMT_2022_actualizado_simplificado.feather")
+    file = wget.download("https://github.com/martin-conur/mcu_geo_utils/blob/main/mcu_geo_utils/data/ISMT_2022_actualizado_simplificado.feather?raw=True", out="data/ISMT_2022_actualizado_simplificado.feather")
     return gpd.read_feather(file)
 
 
 def get_coverture_percentage(df, other):
     return (
         df
         .assign(
```

### Comparing `mcu-geo-utils-0.3/setup.py` & `mcu-geo-utils-0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 setup(
     name='mcu-geo-utils',
-    version='0.3',
+    version='0.4',
     author='Martin Conur',
     author_email='martincontrerasur@gmail.com',
     packages=['mcu_geo_utils'],
     scripts=[],
     url='https://pypi.org/project/mcu-geo-utils/',
     license='MIT',
     description='variaty of geo-related tools',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     install_requires=[
         "pandas >= 1.0",
-        "geopandas == 0.12.1",
+        "geopandas == 0.10.1",
         "shapely == 2.0.1",
         "osmnx == 1.5.1"
     ],
 )
```

