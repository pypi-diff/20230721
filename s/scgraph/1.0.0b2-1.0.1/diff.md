# Comparing `tmp/scgraph-1.0.0b2.tar.gz` & `tmp/scgraph-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scgraph-1.0.0b2.tar", last modified: Thu Jul 20 20:32:36 2023, max compression
+gzip compressed data, was "scgraph-1.0.1.tar", last modified: Fri Jul 21 17:52:23 2023, max compression
```

## Comparing `scgraph-1.0.0b2.tar` & `scgraph-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-20 20:32:36.815843 scgraph-1.0.0b2/
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     1072 2023-04-14 17:06:21.000000 scgraph-1.0.0b2/LICENSE
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     6749 2023-07-20 20:32:36.815843 scgraph-1.0.0b2/PKG-INFO
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     6084 2023-07-20 20:25:00.000000 scgraph-1.0.0b2/README.md
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      109 2023-07-20 20:25:00.000000 scgraph-1.0.0b2/pyproject.toml
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-20 20:32:36.815843 scgraph-1.0.0b2/scgraph/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       96 2023-07-20 20:25:00.000000 scgraph-1.0.0b2/scgraph/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    20565 2023-07-20 20:25:00.000000 scgraph-1.0.0b2/scgraph/core.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-20 20:32:36.815843 scgraph-1.0.0b2/scgraph/geographs/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        0 2023-07-20 20:28:13.000000 scgraph-1.0.0b2/scgraph/geographs/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)  1143458 2023-07-20 20:25:00.000000 scgraph-1.0.0b2/scgraph/geographs/marnet.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     2150 2023-07-20 20:25:00.000000 scgraph-1.0.0b2/scgraph/utils.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-20 20:32:36.815843 scgraph-1.0.0b2/scgraph.egg-info/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     6749 2023-07-20 20:32:36.000000 scgraph-1.0.0b2/scgraph.egg-info/PKG-INFO
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      286 2023-07-20 20:32:36.000000 scgraph-1.0.0b2/scgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-07-20 20:32:36.000000 scgraph-1.0.0b2/scgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        8 2023-07-20 20:32:36.000000 scgraph-1.0.0b2/scgraph.egg-info/top_level.txt
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)       79 2023-07-20 20:32:36.815843 scgraph-1.0.0b2/setup.cfg
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      953 2023-07-20 20:32:23.000000 scgraph-1.0.0b2/setup.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-21 17:52:23.692390 scgraph-1.0.1/
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     1072 2023-04-14 17:06:21.000000 scgraph-1.0.1/LICENSE
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     7171 2023-07-21 17:52:23.692390 scgraph-1.0.1/PKG-INFO
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     6510 2023-07-21 17:35:23.000000 scgraph-1.0.1/README.md
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      109 2023-07-20 20:25:00.000000 scgraph-1.0.1/pyproject.toml
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-21 17:52:23.688389 scgraph-1.0.1/scgraph/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       96 2023-07-20 20:39:03.000000 scgraph-1.0.1/scgraph/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    20565 2023-07-20 20:25:00.000000 scgraph-1.0.1/scgraph/core.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-21 17:52:23.692390 scgraph-1.0.1/scgraph/geographs/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        0 2023-07-20 20:28:13.000000 scgraph-1.0.1/scgraph/geographs/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)  1143458 2023-07-20 20:25:00.000000 scgraph-1.0.1/scgraph/geographs/marnet.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)   976597 2023-07-21 17:34:03.000000 scgraph-1.0.1/scgraph/geographs/oak_ridge_maritime.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     2150 2023-07-20 20:25:00.000000 scgraph-1.0.1/scgraph/utils.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-21 17:52:23.688389 scgraph-1.0.1/scgraph.egg-info/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     7171 2023-07-21 17:52:23.000000 scgraph-1.0.1/scgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      326 2023-07-21 17:52:23.000000 scgraph-1.0.1/scgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-07-21 17:52:23.000000 scgraph-1.0.1/scgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        8 2023-07-21 17:52:23.000000 scgraph-1.0.1/scgraph.egg-info/top_level.txt
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)       79 2023-07-21 17:52:23.692390 scgraph-1.0.1/setup.cfg
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      949 2023-07-21 17:51:34.000000 scgraph-1.0.1/setup.py
```

### Comparing `scgraph-1.0.0b2/LICENSE` & `scgraph-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scgraph-1.0.0b2/PKG-INFO` & `scgraph-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scgraph
-Version: 1.0.0b2
+Version: 1.0.1
 Summary: Determine an approximate route between two points on earth
 Home-page: https://github.com/connor-makowski/scgraph
-Download-URL: https://github.com/connor-makowski/scgraph/dist/scgraph-1.0.0b2.tar.gz
+Download-URL: https://github.com/connor-makowski/scgraph/dist/scgraph-1.0.1.tar.gz
 Author: Connor Makowski
 Author-email: connor.m.makowski@gmail.com
 License: MIT
 Keywords: scgraph
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -195,13 +195,18 @@
 # }
 ```
 
 
 ## Included GeoGraphs
 
 - marnet_geograph:
-    - What: A maritime network data set
+    - What: A maritime network data set from searoute
     - Use: `from scgraph.geographs.marnet import marnet_geograph`
+    - Attribution: [searoute](https://github.com/genthalili/searoute-py)
+- oak_ridge_maritime_geograph:
+    - What: A maritime data set from the Oak Ridge National Laboratory campus
+    - Use: `from scgraph.geographs.oak_ridge_maritime import oak_ridge_maritime_geograph`
+    - Attribution: [Oak Ridge National Laboratory](https://www.ornl.gov/) with data from [Geocommons](http://geocommons.com/datasets?id=25)
 - More to follow
 
 ## Attributions and Thanks
 Originally inspired by [searoute](https://github.com/genthalili/searoute-py) including the use of one of their [datasets](https://github.com/genthalili/searoute-py/blob/main/searoute/data/marnet_densified_v2_old.geojson) that has been modified to work properly with this package.
```

### Comparing `scgraph-1.0.0b2/README.md` & `scgraph-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -177,13 +177,18 @@
 # }
 ```
 
 
 ## Included GeoGraphs
 
 - marnet_geograph:
-    - What: A maritime network data set
+    - What: A maritime network data set from searoute
     - Use: `from scgraph.geographs.marnet import marnet_geograph`
+    - Attribution: [searoute](https://github.com/genthalili/searoute-py)
+- oak_ridge_maritime_geograph:
+    - What: A maritime data set from the Oak Ridge National Laboratory campus
+    - Use: `from scgraph.geographs.oak_ridge_maritime import oak_ridge_maritime_geograph`
+    - Attribution: [Oak Ridge National Laboratory](https://www.ornl.gov/) with data from [Geocommons](http://geocommons.com/datasets?id=25)
 - More to follow
 
 ## Attributions and Thanks
 Originally inspired by [searoute](https://github.com/genthalili/searoute-py) including the use of one of their [datasets](https://github.com/genthalili/searoute-py/blob/main/searoute/data/marnet_densified_v2_old.geojson) that has been modified to work properly with this package.
```

### Comparing `scgraph-1.0.0b2/scgraph/core.py` & `scgraph-1.0.1/scgraph/core.py`

 * *Files identical despite different names*

### Comparing `scgraph-1.0.0b2/scgraph/geographs/marnet.py` & `scgraph-1.0.1/scgraph/geographs/marnet.py`

 * *Files identical despite different names*

### Comparing `scgraph-1.0.0b2/scgraph/utils.py` & `scgraph-1.0.1/scgraph/utils.py`

 * *Files identical despite different names*

### Comparing `scgraph-1.0.0b2/scgraph.egg-info/PKG-INFO` & `scgraph-1.0.1/scgraph.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scgraph
-Version: 1.0.0b2
+Version: 1.0.1
 Summary: Determine an approximate route between two points on earth
 Home-page: https://github.com/connor-makowski/scgraph
-Download-URL: https://github.com/connor-makowski/scgraph/dist/scgraph-1.0.0b2.tar.gz
+Download-URL: https://github.com/connor-makowski/scgraph/dist/scgraph-1.0.1.tar.gz
 Author: Connor Makowski
 Author-email: connor.m.makowski@gmail.com
 License: MIT
 Keywords: scgraph
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -195,13 +195,18 @@
 # }
 ```
 
 
 ## Included GeoGraphs
 
 - marnet_geograph:
-    - What: A maritime network data set
+    - What: A maritime network data set from searoute
     - Use: `from scgraph.geographs.marnet import marnet_geograph`
+    - Attribution: [searoute](https://github.com/genthalili/searoute-py)
+- oak_ridge_maritime_geograph:
+    - What: A maritime data set from the Oak Ridge National Laboratory campus
+    - Use: `from scgraph.geographs.oak_ridge_maritime import oak_ridge_maritime_geograph`
+    - Attribution: [Oak Ridge National Laboratory](https://www.ornl.gov/) with data from [Geocommons](http://geocommons.com/datasets?id=25)
 - More to follow
 
 ## Attributions and Thanks
 Originally inspired by [searoute](https://github.com/genthalili/searoute-py) including the use of one of their [datasets](https://github.com/genthalili/searoute-py/blob/main/searoute/data/marnet_densified_v2_old.geojson) that has been modified to work properly with this package.
```

### Comparing `scgraph-1.0.0b2/setup.py` & `scgraph-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'scgraph',
   packages = ['scgraph', 'scgraph.geographs'],
-  version = '1.0.0b2',
+  version = '1.0.1',
   license='MIT',
   description = 'Determine an approximate route between two points on earth',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Connor Makowski',
   author_email = 'connor.m.makowski@gmail.com',
   url = 'https://github.com/connor-makowski/scgraph',
-  download_url = 'https://github.com/connor-makowski/scgraph/dist/scgraph-1.0.0b2.tar.gz',
+  download_url = 'https://github.com/connor-makowski/scgraph/dist/scgraph-1.0.1.tar.gz',
   keywords = ['scgraph'],
   install_requires=[],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
```

