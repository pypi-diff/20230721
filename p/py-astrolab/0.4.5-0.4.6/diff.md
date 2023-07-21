# Comparing `tmp/py_astrolab-0.4.5.tar.gz` & `tmp/py_astrolab-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_astrolab-0.4.5.tar", max compression
+gzip compressed data, was "py_astrolab-0.4.6.tar", max compression
```

## Comparing `py_astrolab-0.4.5.tar` & `py_astrolab-0.4.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0       91 2023-06-17 10:19:25.525258 py_astrolab-0.4.5/README.md
--rwxr-xr-x   0        0        0     5017 2023-05-29 18:14:56.433552 py_astrolab-0.4.5/py_astrolab/__init__.py
--rwxr-xr-x   0        0        0    17259 2023-07-20 23:25:25.614869 py_astrolab-0.4.5/py_astrolab/aspects.py
--rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.4.5/py_astrolab/charts/__init__.py
--rwxr-xr-x   0        0        0    80480 2023-07-21 15:40:10.377947 py_astrolab-0.4.5/py_astrolab/charts/charts_svg.py
--rwxr-xr-x   0        0        0    60301 2023-07-20 23:19:16.299036 py_astrolab-0.4.5/py_astrolab/charts/templates/basic.xml
--rwxr-xr-x   0        0        0     2699 2023-07-19 10:01:30.109259 py_astrolab-0.4.5/py_astrolab/charts/templates/dark_true_moon.svg
--rwxr-xr-x   0        0        0    60570 2023-07-20 23:18:57.800498 py_astrolab-0.4.5/py_astrolab/charts/templates/extended.xml
--rwxr-xr-x   0        0        0    64946 2023-07-21 00:13:53.576513 py_astrolab-0.4.5/py_astrolab/charts/templates/minimal.xml
--rwxr-xr-x   0        0        0    73370 2023-07-09 16:34:16.735355 py_astrolab-0.4.5/py_astrolab/charts/wonderful_mistake.py
--rwxr-xr-x   0        0        0     5077 2023-05-29 18:14:56.449179 py_astrolab-0.4.5/py_astrolab/fetch_geonames.py
--rwxr-xr-x   0        0        0    12935 2023-07-18 22:44:12.768183 py_astrolab-0.4.5/py_astrolab/kr.config.json
--rwxr-xr-x   0        0        0    27551 2023-07-21 13:28:22.310722 py_astrolab-0.4.5/py_astrolab/main.py
--rwxr-xr-x   0        0        0     3149 2023-06-17 10:10:20.258711 py_astrolab-0.4.5/py_astrolab/print_all_data.py
--rwxr-xr-x   0        0        0     7785 2023-06-17 10:10:20.255187 py_astrolab-0.4.5/py_astrolab/relationship_score.py
--rwxr-xr-x   0        0        0     2361 2023-07-12 12:55:07.631989 py_astrolab-0.4.5/py_astrolab/report.py
--rwxr-xr-x   0        0        0     5239 2023-07-19 09:00:42.893119 py_astrolab-0.4.5/py_astrolab/types.py
--rwxr-xr-x   0        0        0     7271 2023-07-19 09:03:07.864665 py_astrolab-0.4.5/py_astrolab/utilities.py
--rwxr-xr-x   0        0        0      689 2023-07-21 15:40:37.676788 py_astrolab-0.4.5/pyproject.toml
--rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.4.5/PKG-INFO
+-rwxr-xr-x   0        0        0       91 2023-06-17 10:19:25.525258 py_astrolab-0.4.6/README.md
+-rwxr-xr-x   0        0        0     5017 2023-05-29 18:14:56.433552 py_astrolab-0.4.6/py_astrolab/__init__.py
+-rwxr-xr-x   0        0        0    17259 2023-07-20 23:25:25.614869 py_astrolab-0.4.6/py_astrolab/aspects.py
+-rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.4.6/py_astrolab/charts/__init__.py
+-rwxr-xr-x   0        0        0    80460 2023-07-21 15:49:05.720028 py_astrolab-0.4.6/py_astrolab/charts/charts_svg.py
+-rwxr-xr-x   0        0        0    60301 2023-07-20 23:19:16.299036 py_astrolab-0.4.6/py_astrolab/charts/templates/basic.xml
+-rwxr-xr-x   0        0        0     2699 2023-07-19 10:01:30.109259 py_astrolab-0.4.6/py_astrolab/charts/templates/dark_true_moon.svg
+-rwxr-xr-x   0        0        0    60570 2023-07-20 23:18:57.800498 py_astrolab-0.4.6/py_astrolab/charts/templates/extended.xml
+-rwxr-xr-x   0        0        0    64946 2023-07-21 00:13:53.576513 py_astrolab-0.4.6/py_astrolab/charts/templates/minimal.xml
+-rwxr-xr-x   0        0        0    73370 2023-07-09 16:34:16.735355 py_astrolab-0.4.6/py_astrolab/charts/wonderful_mistake.py
+-rwxr-xr-x   0        0        0     5077 2023-05-29 18:14:56.449179 py_astrolab-0.4.6/py_astrolab/fetch_geonames.py
+-rwxr-xr-x   0        0        0    12935 2023-07-18 22:44:12.768183 py_astrolab-0.4.6/py_astrolab/kr.config.json
+-rwxr-xr-x   0        0        0    27551 2023-07-21 13:28:22.310722 py_astrolab-0.4.6/py_astrolab/main.py
+-rwxr-xr-x   0        0        0     3149 2023-06-17 10:10:20.258711 py_astrolab-0.4.6/py_astrolab/print_all_data.py
+-rwxr-xr-x   0        0        0     7785 2023-06-17 10:10:20.255187 py_astrolab-0.4.6/py_astrolab/relationship_score.py
+-rwxr-xr-x   0        0        0     2361 2023-07-12 12:55:07.631989 py_astrolab-0.4.6/py_astrolab/report.py
+-rwxr-xr-x   0        0        0     5239 2023-07-19 09:00:42.893119 py_astrolab-0.4.6/py_astrolab/types.py
+-rwxr-xr-x   0        0        0     7271 2023-07-19 09:03:07.864665 py_astrolab-0.4.6/py_astrolab/utilities.py
+-rwxr-xr-x   0        0        0      689 2023-07-21 15:49:30.924294 py_astrolab-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.4.6/PKG-INFO
```

### Comparing `py_astrolab-0.4.5/py_astrolab/__init__.py` & `py_astrolab-0.4.6/py_astrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.4.5/py_astrolab/aspects.py` & `py_astrolab-0.4.6/py_astrolab/aspects.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.4.5/py_astrolab/charts/charts_svg.py` & `py_astrolab-0.4.6/py_astrolab/charts/charts_svg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1318,15 +1318,15 @@
                     aspect_dict = {
                         'p1_abs_pos': axis.abs_pos,
                         'p2_abs_pos': (axis.abs_pos + 180) % 360,
                         'color': axis_data['color'],
                     }
                     out += arrow_top + self.__drawAspect(r, ar, aspect_dict, axis_id, True)
                     offset = offset = (int(self.houses_degree_ut[6]) / -1) + int(aspect_dict['p1_abs_pos'])
-                    out += self.drawTick(r, self.axes_settings[0]["name"], offset)
+                    out += self.drawTick(r, axis.name, offset)
         return out
 
     def drawTick(self, r, id, offset) -> str:
         out = ''
         for c in [self.c2, self.c3]:
             # Calculate the start and end points of the tick mark
             tick_start_x = self.__sliceToX(0, r-c, offset) + c
```

### Comparing `py_astrolab-0.4.5/py_astrolab/charts/templates/basic.xml` & `py_astrolab-0.4.6/py_astrolab/charts/templates/basic.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.4.5/py_astrolab/charts/templates/dark_true_moon.svg` & `py_astrolab-0.4.6/py_astrolab/charts/templates/dark_true_moon.svg`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.4.5/py_astrolab/charts/templates/extended.xml` & `py_astrolab-0.4.6/py_astrolab/charts/templates/extended.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.4.5/py_astrolab/charts/templates/minimal.xml` & `py_astrolab-0.4.6/py_astrolab/charts/templates/minimal.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.4.5/py_astrolab/charts/wonderful_mistake.py` & `py_astrolab-0.4.6/py_astrolab/charts/wonderful_mistake.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.4.5/py_astrolab/fetch_geonames.py` & `py_astrolab-0.4.6/py_astrolab/fetch_geonames.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.4.5/py_astrolab/kr.config.json` & `py_astrolab-0.4.6/py_astrolab/kr.config.json`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.4.5/py_astrolab/main.py` & `py_astrolab-0.4.6/py_astrolab/main.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.4.5/py_astrolab/print_all_data.py` & `py_astrolab-0.4.6/py_astrolab/print_all_data.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.4.5/py_astrolab/relationship_score.py` & `py_astrolab-0.4.6/py_astrolab/relationship_score.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.4.5/py_astrolab/report.py` & `py_astrolab-0.4.6/py_astrolab/report.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.4.5/py_astrolab/types.py` & `py_astrolab-0.4.6/py_astrolab/types.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.4.5/py_astrolab/utilities.py` & `py_astrolab-0.4.6/py_astrolab/utilities.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.4.5/pyproject.toml` & `py_astrolab-0.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-astrolab"
-version = "0.4.5"
+version = "0.4.6"
 description = "A Python interface on Swiss Ephemeris to perform astrological calculations"
 authors = ["Giacomo Battaglia <battaglia.giacomo@yahoo.it>", "Arcangelo Massari <arcangelomas@gmail.com>"]
 license = "GNU General Public License (GPL)"
 readme = "README.md"
 packages = [{include = "py_astrolab"}]
 
 [tool.poetry.dependencies]
```

### Comparing `py_astrolab-0.4.5/PKG-INFO` & `py_astrolab-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-astrolab
-Version: 0.4.5
+Version: 0.4.6
 Summary: A Python interface on Swiss Ephemeris to perform astrological calculations
 License: GNU General Public License (GPL)
 Author: Giacomo Battaglia
 Author-email: battaglia.giacomo@yahoo.it
 Requires-Python: >=3.9,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

