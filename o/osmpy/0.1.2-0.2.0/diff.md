# Comparing `tmp/osmpy-0.1.2.tar.gz` & `tmp/osmpy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osmpy-0.1.2.tar", max compression
+gzip compressed data, was "osmpy-0.2.0.tar", last modified: Tue Nov 24 16:50:57 2020, max compression
```

## Comparing `osmpy-0.1.2.tar` & `osmpy-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1303 2023-07-21 16:07:40.317026 osmpy-0.1.2/LICENSE.md
--rw-r--r--   0        0        0     3409 2023-07-21 16:09:01.716127 osmpy-0.1.2/README.md
--rw-r--r--   0        0        0       60 2023-07-21 16:09:01.716377 osmpy-0.1.2/osmpy/__init__.py
--rw-r--r--   0        0        0     5870 2023-07-21 18:04:57.849361 osmpy-0.1.2/osmpy/core.py
--rw-r--r--   0        0        0     2250 2023-07-21 18:04:54.744925 osmpy-0.1.2/osmpy/queries.py
--rw-r--r--   0        0        0     1145 2023-07-21 18:15:32.234547 osmpy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4548 1970-01-01 00:00:00.000000 osmpy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3050 2020-11-24 16:40:32.497158 osmpy-0.2.0/README.md
+-rw-r--r--   0        0        0       65 2020-11-24 15:38:18.308047 osmpy-0.2.0/osmpy/__init__.py
+-rw-r--r--   0        0        0     4846 2020-11-24 15:38:18.308047 osmpy-0.2.0/osmpy/core.py
+-rw-r--r--   0        0        0     1859 2020-11-24 16:47:37.843116 osmpy-0.2.0/osmpy/queries.py
+-rw-r--r--   0        0        0     1145 2020-11-24 16:50:43.079968 osmpy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4016 2020-11-24 16:50:57.479580 osmpy-0.2.0/setup.py
+-rw-r--r--   0        0        0     4087 2020-11-24 16:50:57.479941 osmpy-0.2.0/PKG-INFO
```

### Comparing `osmpy-0.1.2/README.md` & `osmpy-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,41 +4,40 @@
 pip install osmpy
 ```
 
 #### List precooked queries
 ```python
 osmpy.list_queries()
 
-            name                                          docstring
-0      Amenities           Location of amenities within a boundary 
-1  AmentiesCount    Number of amenities per type within a boundary 
-2           POIs   Location of Points of Interest within a bound...
-3     RoadLength      Length of road by roadtype within a boundary 
+            name                                         docstring
+0      Amenities          Location of amenities within a boundary 
+1  AmentiesCount   Number of amenities per type within a boundary 
+2     RoadLength     Length of road by roadtype within a boundary 
 ```
 
-#### Get all Points of Interest (POIs) within a boundary
+#### Get all amenities in a boundary
 ```python
 import osmpy
 from shapely import wkt
 
 boundary = wkt.loads('POLYGON((-46.63 -23.54,-46.6 -23.54,-46.62 -23.55,-46.63 -23.55,-46.63 -23.54))')
-osmpy.get('POIs', boundary)
+osmpy.get('Amenities', boundary)
 
-    type          id        lat        lon                                               tags                      poi
-0   node   661212030 -23.544739 -46.626160           {'amenity': 'fuel', 'name': 'Posto NGM'}             amenity:fuel
-1   node   661212089 -23.547450 -46.626073  {'amenity': 'fuel', 'name': 'Posto Maserati', ...             amenity:fuel
-2   node   745733280 -23.541411 -46.613930  {'addr:city': 'São Paulo', 'addr:housenumber':...             amenity:bank
-3   node   745733292 -23.542070 -46.614916  {'addr:city': 'São Paulo', 'addr:housenumber':...             amenity:bank
-4   node   889763809 -23.542558 -46.620360  {'addr:housenumber': '110/C9', 'addr:street': ...    amenity:social_centre
-..   ...         ...        ...        ...                                                ...                      ...
-82  node  5663737625 -23.540027 -46.605425  {'access': 'yes', 'addr:city': 'São Paulo', 'a...          amenity:parking
-83  node  5990269247 -23.540650 -46.607532  {'addr:city': 'São Paulo', 'addr:housenumber':...        amenity:fast_food
-84  node  6621564995 -23.543880 -46.626414  {'access': 'yes', 'addr:city': 'São Paulo', 'a...          amenity:parking
-85  node  6625433725 -23.546727 -46.623956  {'access': 'yes', 'addr:city': 'São Paulo', 'a...          amenity:parking
-86  node  6625433753 -23.547111 -46.624790  {'access': 'yes', 'addr:city': 'São Paulo', 'a...  amenity:bicycle_parking
+    type          id        lat        lon                                               tags
+0   node   661212030 -23.544739 -46.626160           {'amenity': 'fuel', 'name': 'Posto NGM'}
+1   node   661212089 -23.547450 -46.626073  {'amenity': 'fuel', 'name': 'Posto Maserati', ...
+2   node   745733280 -23.541411 -46.613930  {'addr:city': 'São Paulo', 'addr:housenumber':...
+3   node   745733292 -23.542070 -46.614916  {'addr:city': 'São Paulo', 'addr:housenumber':...
+4   node   889763809 -23.542558 -46.620360  {'addr:housenumber': '110/C9', 'addr:street': ...
+..   ...         ...        ...        ...                                                ...
+84  node  5663737625 -23.540027 -46.605425  {'access': 'yes', 'addr:city': 'São Paulo', 'a...
+85  node  5990269247 -23.540650 -46.607532  {'addr:city': 'São Paulo', 'addr:housenumber':...
+86  node  6621564995 -23.543880 -46.626414  {'access': 'yes', 'addr:city': 'São Paulo', 'a...
+87  node  6625433725 -23.546727 -46.623956  {'access': 'yes', 'addr:city': 'São Paulo', 'a...
+88  node  6625433753 -23.547111 -46.624790  {'access': 'yes', 'addr:city': 'São Paulo', 'a...
 ```
 
 #### Total road length by road type
 ```python
 osmpy.get('RoadLength', boundary)
 
                count     length
@@ -90,8 +89,10 @@
 osmpy.get(YourPrecookedQuery, boundary)
 ```
 
 :point_right: Leave an issue or PR if you want to add a new query to the package
 
 ## Credits
 
+Free software: MIT license
+
 Function `katana` from @snorfalorpagus_.
```

### Comparing `osmpy-0.1.2/osmpy/core.py` & `osmpy-0.2.0/osmpy/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 import pyproj
 import time
 import json
 from retry import retry
 import pandas as pd
 import warnings
 import re
-from .queries import *
+import osmpy.queries as qs
 import sys
-import inspect
 
 warnings.filterwarnings("ignore", category=FutureWarning)
 
 def simplify(s, delta=0.05):
     
     while not check_length(s):
         s = s.simplify(delta, False)
@@ -27,41 +26,38 @@
     return s
 
 def check_length(s, threshold=3000):
     
     return len(str(s)) < threshold
 
 def get_area(s):
-    """Get the area of a shapely polygon in sq km"""
     s = shape(s)
     proj = partial(
         pyproj.transform, pyproj.Proj(init="epsg:4326"), pyproj.Proj(init="epsg:3857")
     )
-    area = transform(proj, s).area / 1e6  # km
-    
-    return area
+
+    return transform(proj, s).area / 1e6  # km
 
 
 def threshold_func(g, value):
 
     return get_area(g) < value
 
 
-def katana(geometry, threshold_func, threshold_value, count=0, urllen_threshold=7648):
+def katana(geometry, threshold_func, threshold_value, count=0):
     """Split a Polygon into two parts across it's shortest dimension
     
     KUDOS https://snorfalorpagus.net/blog/2016/03/13/splitting-large-polygons-for-faster-intersections/
     """
     bounds = geometry.bounds
     width = bounds[2] - bounds[0]
     height = bounds[3] - bounds[1]
-    if (threshold_func(geometry, threshold_value) and (len(to_overpass_coords(geometry)) < urllen_threshold)) or (count == 250):
-        # either the polygon is smaller than the threshold
-        # AND the length of the expected url is short enough to avoid Error 414
-        # OR the maximum number of recursions has been reached
+    if threshold_func(geometry, threshold_value) or count == 250:
+        # either the polygon is smaller than the threshold, or the maximum
+        # number of recursions has been reached
         return [geometry]
     if height >= width:
         # split left to right
         a = box(bounds[0], bounds[1], bounds[2], bounds[1] + height / 2)
         b = box(bounds[0], bounds[1] + height / 2, bounds[2], bounds[3])
     else:
         # split top to bottom
@@ -73,15 +69,15 @@
         b,
     ):
         c = geometry.intersection(d)
         if not isinstance(c, GeometryCollection):
             c = [c]
         for e in c:
             if isinstance(e, (Polygon, MultiPolygon)):
-                result.extend(katana(e, threshold_func, threshold_value, count + 1, urllen_threshold=urllen_threshold))
+                result.extend(katana(e, threshold_func, threshold_value, count + 1))
     if count > 0:
         return result
     # convert multipart into singlepart
     final_result = []
     for g in result:
         if isinstance(g, MultiPolygon):
             final_result.extend(g)
@@ -125,77 +121,61 @@
     overpass_query = query.query.format(boundary=boundary)
 
     response = requests.get(overpass_url, params={"data": overpass_query}).json()
 
     return pd.DataFrame(response['elements'])
 
 
-def get(query, boundary, threshold_value=1000000, urllen_threshold=7648):
-    """Get Open Street Maps Turbo Query for a given boundary
+def get(query, boundary, threshold_value=1000000):
+    """Get Open Street Maps highways length in meters and object count for a given boundary
 
     It splits the regions to manage overpass turbo limits.
 
     For MultiPolygons, only the biggest polygon will be considered.
 
     Parameters
     ----------
     boundary : shapely.geometry
         A shapely polygon
     threshold_value : int, optional
         Maximum area in sq km to split the polygons, by default 1000000
-    urllen_threshold : int, optional
-        Maximum length of the url to send to Overpass API, by default 7648 (found experimentally)
 
     Returns
     -------
     pd.DataFrame
         Table indexed by highway with length sum in meters and observation count
     """
 
     if isinstance(query, str):
         if query in _get_queries_names():
             query_obj = getattr(sys.modules['osmpy.queries'], query)()
         else:
-            query_obj = QueryType()
+            query_obj = qs.QueryType()
             query_obj.query = query
     elif isinstance(query, type):
         query_obj = query()
 
-    boundaries = katana(boundary, threshold_func, threshold_value, urllen_threshold=urllen_threshold)
-    
-    # Looking for the boundaries which generate too long URLs resulting in Error 414.
-    # If found the boundaries will be processed again by `katana()`
-    while True:
-        for geo in boundaries:
-            urllen = len(to_overpass_coords(geo))
-            if urllen >= urllen_threshold:
-                boundaries.remove(geo)
-                boundaries.extend(katana(geo, threshold_func, threshold_value, urllen_threshold=urllen_threshold))
-                break
-        else:
-            break
+    boundaries = katana(boundary, threshold_func, threshold_value)
 
     responses = []
     for bound in boundaries:
 
         bound = to_overpass_coords(bound)
         responses.append(overpass_request(query_obj, bound))
 
     data = pd.concat([pd.DataFrame(d) for d in responses])
 
     data = query_obj.postprocess(data)
 
     return data
 
 def _get_queries_names():
-    query_classes = [c[0] for c in inspect.getmembers(sys.modules[__name__], inspect.isclass) if QueryType in c[1].__bases__]
-    return query_classes
+
+    return [t for t in dir(qs) if (t[0].isupper() and (t is not 'QueryType'))]
 
 def list_queries():
     
     return pd.DataFrame([
         {'name': t,
         'docstring': re.sub('\s+',' ',
                 getattr(sys.modules['osmpy.queries'], t)().docstring)}
-     for t in _get_queries_names()])
-
-
+     for t in _get_queries_names()])
```

### Comparing `osmpy-0.1.2/osmpy/queries.py` & `osmpy-0.2.0/osmpy/queries.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,16 +14,16 @@
         out body geom;
     """
 
     docstring = """
     Location of Points of Interest within a boundary. 
     Points of Interest being all shops and amenities.
     """
-    
-    def prep_pois(self, x):
+    @staticmethod
+    def prep_pois(x):
     
         if x.get('amenity'):
             return f'amenity:{x["amenity"]}'
         elif x.get('shop'):
             return f'shop:{x["shop"]}'
         else:
             return None
@@ -83,17 +83,8 @@
     }}"""
 
     docstring = """
     Length of road by roadtype within a boundary
     """
 
     def postprocess(self, df):
-        if 'tags' in df.columns:
-            return df['tags'].apply(pd.Series).astype({ # It seems API may generate dataframe with strings
-                'highway': 'str',
-                'count': 'int',
-                'length': 'float'
-            }).groupby('highway').sum()
-        else:
-            empty = pd.DataFrame(columns=['count', 'length']).astype({'count': 'int', 'length': 'float'})
-            empty.index.name = 'highway'
-            return empty
+        return df['tags'].apply(pd.Series).groupby('highway').sum()
```

### Comparing `osmpy-0.1.2/pyproject.toml` & `osmpy-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ]
 description = "Powerfull wrapper around OSM Overpass Turbo to query regions of any size and shape"
 homepage = "https://github.com/JoaoCarabetta/osmpy"
 license = "AM-331-A3 Licencia de Software"
 name = "osmpy"
 readme = "README.md"
 repository = "https://github.com/JoaoCarabetta/osmpy"
-version = "0.1.2"
+version = "0.2.0"
 
 [tool.poetry.dependencies]
 python = "^3.6"
 shapely = "1.7.0"
 geojson = "2.5.0"
 requests = "2.23.0"
 retry = "*"
```

### Comparing `osmpy-0.1.2/PKG-INFO` & `osmpy-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: osmpy
-Version: 0.1.2
+Version: 0.2.0
 Summary: Powerfull wrapper around OSM Overpass Turbo to query regions of any size and shape
 Home-page: https://github.com/JoaoCarabetta/osmpy
 License: AM-331-A3 Licencia de Software
 Author: Joao Carabetta
 Author-email: joao.carabetta@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: geojson (==2.5.0)
 Requires-Dist: pandas (>=1.0.0,<2.0.0)
 Requires-Dist: pyproj
 Requires-Dist: requests (==2.23.0)
 Requires-Dist: retry
@@ -32,41 +30,40 @@
 pip install osmpy
 ```
 
 #### List precooked queries
 ```python
 osmpy.list_queries()
 
-            name                                          docstring
-0      Amenities           Location of amenities within a boundary 
-1  AmentiesCount    Number of amenities per type within a boundary 
-2           POIs   Location of Points of Interest within a bound...
-3     RoadLength      Length of road by roadtype within a boundary 
+            name                                         docstring
+0      Amenities          Location of amenities within a boundary 
+1  AmentiesCount   Number of amenities per type within a boundary 
+2     RoadLength     Length of road by roadtype within a boundary 
 ```
 
-#### Get all Points of Interest (POIs) within a boundary
+#### Get all amenities in a boundary
 ```python
 import osmpy
 from shapely import wkt
 
 boundary = wkt.loads('POLYGON((-46.63 -23.54,-46.6 -23.54,-46.62 -23.55,-46.63 -23.55,-46.63 -23.54))')
-osmpy.get('POIs', boundary)
+osmpy.get('Amenities', boundary)
 
-    type          id        lat        lon                                               tags                      poi
-0   node   661212030 -23.544739 -46.626160           {'amenity': 'fuel', 'name': 'Posto NGM'}             amenity:fuel
-1   node   661212089 -23.547450 -46.626073  {'amenity': 'fuel', 'name': 'Posto Maserati', ...             amenity:fuel
-2   node   745733280 -23.541411 -46.613930  {'addr:city': 'São Paulo', 'addr:housenumber':...             amenity:bank
-3   node   745733292 -23.542070 -46.614916  {'addr:city': 'São Paulo', 'addr:housenumber':...             amenity:bank
-4   node   889763809 -23.542558 -46.620360  {'addr:housenumber': '110/C9', 'addr:street': ...    amenity:social_centre
-..   ...         ...        ...        ...                                                ...                      ...
-82  node  5663737625 -23.540027 -46.605425  {'access': 'yes', 'addr:city': 'São Paulo', 'a...          amenity:parking
-83  node  5990269247 -23.540650 -46.607532  {'addr:city': 'São Paulo', 'addr:housenumber':...        amenity:fast_food
-84  node  6621564995 -23.543880 -46.626414  {'access': 'yes', 'addr:city': 'São Paulo', 'a...          amenity:parking
-85  node  6625433725 -23.546727 -46.623956  {'access': 'yes', 'addr:city': 'São Paulo', 'a...          amenity:parking
-86  node  6625433753 -23.547111 -46.624790  {'access': 'yes', 'addr:city': 'São Paulo', 'a...  amenity:bicycle_parking
+    type          id        lat        lon                                               tags
+0   node   661212030 -23.544739 -46.626160           {'amenity': 'fuel', 'name': 'Posto NGM'}
+1   node   661212089 -23.547450 -46.626073  {'amenity': 'fuel', 'name': 'Posto Maserati', ...
+2   node   745733280 -23.541411 -46.613930  {'addr:city': 'São Paulo', 'addr:housenumber':...
+3   node   745733292 -23.542070 -46.614916  {'addr:city': 'São Paulo', 'addr:housenumber':...
+4   node   889763809 -23.542558 -46.620360  {'addr:housenumber': '110/C9', 'addr:street': ...
+..   ...         ...        ...        ...                                                ...
+84  node  5663737625 -23.540027 -46.605425  {'access': 'yes', 'addr:city': 'São Paulo', 'a...
+85  node  5990269247 -23.540650 -46.607532  {'addr:city': 'São Paulo', 'addr:housenumber':...
+86  node  6621564995 -23.543880 -46.626414  {'access': 'yes', 'addr:city': 'São Paulo', 'a...
+87  node  6625433725 -23.546727 -46.623956  {'access': 'yes', 'addr:city': 'São Paulo', 'a...
+88  node  6625433753 -23.547111 -46.624790  {'access': 'yes', 'addr:city': 'São Paulo', 'a...
 ```
 
 #### Total road length by road type
 ```python
 osmpy.get('RoadLength', boundary)
 
                count     length
@@ -118,9 +115,11 @@
 osmpy.get(YourPrecookedQuery, boundary)
 ```
 
 :point_right: Leave an issue or PR if you want to add a new query to the package
 
 ## Credits
 
+Free software: MIT license
+
 Function `katana` from @snorfalorpagus_.
```

