# Comparing `tmp/isogrids-0.0.3.tar.gz` & `tmp/isogrids-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isogrids-0.0.3.tar", last modified: Thu Jul 20 23:27:05 2023, max compression
+gzip compressed data, was "isogrids-0.0.4.tar", last modified: Fri Jul 21 01:17:43 2023, max compression
```

## Comparing `isogrids-0.0.3.tar` & `isogrids-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 23:27:05.810647 isogrids-0.0.3/
--rw-rw-r--   0 isaac     (1001) isaac     (1001)     1067 2023-07-20 21:36:59.000000 isogrids-0.0.3/LICENSE
--rw-rw-r--   0 isaac     (1001) isaac     (1001)      760 2023-07-20 23:27:05.810647 isogrids-0.0.3/PKG-INFO
--rw-rw-r--   0 isaac     (1001) isaac     (1001)      167 2023-07-20 22:21:00.000000 isogrids-0.0.3/README.md
--rw-rw-r--   0 isaac     (1001) isaac     (1001)      665 2023-07-20 23:26:59.000000 isogrids-0.0.3/pyproject.toml
--rw-rw-r--   0 isaac     (1001) isaac     (1001)       38 2023-07-20 23:27:05.810647 isogrids-0.0.3/setup.cfg
-drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 23:27:05.806647 isogrids-0.0.3/src/
-drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 23:27:05.806647 isogrids-0.0.3/src/isogrids/
--rw-rw-r--   0 isaac     (1001) isaac     (1001)       26 2023-07-20 23:19:08.000000 isogrids-0.0.3/src/isogrids/__init__.py
--rw-rw-r--   0 isaac     (1001) isaac     (1001)       47 2023-07-13 20:48:01.000000 isogrids-0.0.3/src/isogrids/env.py
-drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 23:27:05.806647 isogrids-0.0.3/src/isogrids/environments/
--rw-rw-r--   0 isaac     (1001) isaac     (1001)       24 2023-07-20 23:20:18.000000 isogrids-0.0.3/src/isogrids/environments/__init__.py
-drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 23:27:05.806647 isogrids-0.0.3/src/isogrids/environments/house_env/
--rw-rw-r--   0 isaac     (1001) isaac     (1001)       23 2023-07-20 23:21:02.000000 isogrids-0.0.3/src/isogrids/environments/house_env/__init__.py
--rw-rw-r--   0 isaac     (1001) isaac     (1001)      936 2023-07-20 20:10:36.000000 isogrids-0.0.3/src/isogrids/environments/house_env/build_houses.py
--rw-rw-r--   0 isaac     (1001) isaac     (1001)     1607 2023-07-20 16:34:31.000000 isogrids-0.0.3/src/isogrids/environments/house_env/house_furniture.py
--rw-rw-r--   0 isaac     (1001) isaac     (1001)    17489 2023-07-20 23:24:11.000000 isogrids-0.0.3/src/isogrids/environments/house_env/house_gen.py
--rw-rw-r--   0 isaac     (1001) isaac     (1001)      703 2023-07-20 19:29:52.000000 isogrids-0.0.3/src/isogrids/environments/house_env/house_gen_timeout.py
--rw-rw-r--   0 isaac     (1001) isaac     (1001)     3221 2023-07-20 17:44:12.000000 isogrids-0.0.3/src/isogrids/environments/house_env/house_rooms.py
--rw-rw-r--   0 isaac     (1001) isaac     (1001)     2446 2023-07-20 19:14:35.000000 isogrids-0.0.3/src/isogrids/environments/house_env/plot_house_graph.py
-drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 23:27:05.806647 isogrids-0.0.3/src/isogrids.egg-info/
--rw-rw-r--   0 isaac     (1001) isaac     (1001)      760 2023-07-20 23:27:05.000000 isogrids-0.0.3/src/isogrids.egg-info/PKG-INFO
--rw-rw-r--   0 isaac     (1001) isaac     (1001)      627 2023-07-20 23:27:05.000000 isogrids-0.0.3/src/isogrids.egg-info/SOURCES.txt
--rw-rw-r--   0 isaac     (1001) isaac     (1001)        1 2023-07-20 23:27:05.000000 isogrids-0.0.3/src/isogrids.egg-info/dependency_links.txt
--rw-rw-r--   0 isaac     (1001) isaac     (1001)        9 2023-07-20 23:27:05.000000 isogrids-0.0.3/src/isogrids.egg-info/top_level.txt
+drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-21 01:17:43.972943 isogrids-0.0.4/
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)     1067 2023-07-20 21:36:59.000000 isogrids-0.0.4/LICENSE
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)      760 2023-07-21 01:17:43.968943 isogrids-0.0.4/PKG-INFO
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)      167 2023-07-20 22:21:00.000000 isogrids-0.0.4/README.md
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)      665 2023-07-21 01:17:22.000000 isogrids-0.0.4/pyproject.toml
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)       38 2023-07-21 01:17:43.972943 isogrids-0.0.4/setup.cfg
+drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-21 01:17:43.968943 isogrids-0.0.4/src/
+drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-21 01:17:43.968943 isogrids-0.0.4/src/isogrids/
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)       26 2023-07-20 23:19:08.000000 isogrids-0.0.4/src/isogrids/__init__.py
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)       47 2023-07-13 20:48:01.000000 isogrids-0.0.4/src/isogrids/env.py
+drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-21 01:17:43.968943 isogrids-0.0.4/src/isogrids/environments/
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)       24 2023-07-20 23:20:18.000000 isogrids-0.0.4/src/isogrids/environments/__init__.py
+drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-21 01:17:43.968943 isogrids-0.0.4/src/isogrids/environments/house_env/
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)       50 2023-07-21 00:29:43.000000 isogrids-0.0.4/src/isogrids/environments/house_env/__init__.py
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)     2969 2023-07-21 01:13:47.000000 isogrids-0.0.4/src/isogrids/environments/house_env/build_houses.py
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)     1607 2023-07-20 16:34:31.000000 isogrids-0.0.4/src/isogrids/environments/house_env/house_furniture.py
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)    17739 2023-07-21 01:13:59.000000 isogrids-0.0.4/src/isogrids/environments/house_env/house_gen.py
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)      703 2023-07-20 19:29:52.000000 isogrids-0.0.4/src/isogrids/environments/house_env/house_gen_timeout.py
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)     3221 2023-07-20 17:44:12.000000 isogrids-0.0.4/src/isogrids/environments/house_env/house_rooms.py
+drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-21 01:17:43.968943 isogrids-0.0.4/src/isogrids.egg-info/
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)      760 2023-07-21 01:17:43.000000 isogrids-0.0.4/src/isogrids.egg-info/PKG-INFO
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)      571 2023-07-21 01:17:43.000000 isogrids-0.0.4/src/isogrids.egg-info/SOURCES.txt
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)        1 2023-07-21 01:17:43.000000 isogrids-0.0.4/src/isogrids.egg-info/dependency_links.txt
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)        9 2023-07-21 01:17:43.000000 isogrids-0.0.4/src/isogrids.egg-info/top_level.txt
```

### Comparing `isogrids-0.0.3/LICENSE` & `isogrids-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `isogrids-0.0.3/PKG-INFO` & `isogrids-0.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isogrids
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package that generates and visualizes simple simulation environments and their respective scene graphs for planning-algorithm development
 Author-email: Isaac Remy <iremy@uw.edu>
 Project-URL: Homepage, https://github.com/isremy/isogrids
 Project-URL: Bug Tracker, https://github.com/isremy/isogrids
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `isogrids-0.0.3/pyproject.toml` & `isogrids-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "isogrids"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Isaac Remy", email="iremy@uw.edu" },
 ]
 description = "A package that generates and visualizes simple simulation environments and their respective scene graphs for planning-algorithm development"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `isogrids-0.0.3/src/isogrids/environments/house_env/house_furniture.py` & `isogrids-0.0.4/src/isogrids/environments/house_env/house_furniture.py`

 * *Files identical despite different names*

### Comparing `isogrids-0.0.3/src/isogrids/environments/house_env/house_gen.py` & `isogrids-0.0.4/src/isogrids/environments/house_env/house_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from . import house_rooms, house_furniture
+# import house_rooms, house_furniture
 import networkx as nx
 import random as rd
 import numpy as np
 import math
 import cv2
 from copy import deepcopy
 import time
 from .house_gen_timeout import timeout
+# from house_gen_timeout import timeout
 
 SCALE_X = 700
 SCALE_Y = 700
 NUM_REGIONS = 6
 BLUR_KERNEL = 37
 DOORWAY_WIDTH = 70
 TIMEOUT = 15
@@ -260,26 +262,29 @@
 
 		for room_id in rooms:
 			if room_id != 0:
 				f_pieces = tuple()
 				room_f_dict = getattr(house_rooms, graph_obj_dict[room_id]["name"][:-1]).furniture_associations.keys()
 				num_pieces = len(room_f_dict)
 				for f_id, f in enumerate(room_f_dict, max_id + 1):
-					if f not in furniture_nums.keys():
-						furniture_nums[f] = 0
-					else:
-						furniture_nums[f] += 1
-					f_name = f + str(furniture_nums[f])
-					contour = graph_obj_dict[room_id]["contour"]
-					point = rand_contour_point(contour, 30, 5, graph_obj_dict[room_id]["doorways"], f_pieces)
-					f_pieces += (point,)
-					graph_obj_dict[f_id] = {"name":f_name, "centroid":point, "edges": (room_id), "contour":(), "class":"furniture"}
-					graph_obj_dict[room_id]["edges"] += (f_id,)
-					self.__graph.add_edge(graph_obj_dict[room_id]["name"], f_name)
-					cv2.circle(color_image, point, 5, (255, 0, 0), -1)
+					prob = getattr(house_rooms, graph_obj_dict[room_id]["name"][:-1]).furniture_associations[f]
+					placed = np.random.binomial(1, prob)
+					if placed == 1:
+						if f not in furniture_nums.keys():
+							furniture_nums[f] = 0
+						else:
+							furniture_nums[f] += 1
+						f_name = f + str(furniture_nums[f])
+						contour = graph_obj_dict[room_id]["contour"]
+						point = rand_contour_point(contour, 30, 5, graph_obj_dict[room_id]["doorways"], f_pieces)
+						f_pieces += (point,)
+						graph_obj_dict[f_id] = {"name":f_name, "centroid":point, "edges": (room_id), "contour":(), "class":"furniture"}
+						graph_obj_dict[room_id]["edges"] += (f_id,)
+						self.__graph.add_edge(graph_obj_dict[room_id]["name"], f_name)
+						cv2.circle(color_image, point, 5, (255, 0, 0), -1)
 				max_id += num_pieces
 
 
 		for obj in graph_obj_dict:
 			text = graph_obj_dict[obj]["name"]
 			font = cv2.FONT_HERSHEY_SIMPLEX
 			font_scale = 0.5
```

### Comparing `isogrids-0.0.3/src/isogrids/environments/house_env/house_gen_timeout.py` & `isogrids-0.0.4/src/isogrids/environments/house_env/house_gen_timeout.py`

 * *Files identical despite different names*

### Comparing `isogrids-0.0.3/src/isogrids/environments/house_env/house_rooms.py` & `isogrids-0.0.4/src/isogrids/environments/house_env/house_rooms.py`

 * *Files identical despite different names*

### Comparing `isogrids-0.0.3/src/isogrids.egg-info/PKG-INFO` & `isogrids-0.0.4/src/isogrids.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isogrids
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package that generates and visualizes simple simulation environments and their respective scene graphs for planning-algorithm development
 Author-email: Isaac Remy <iremy@uw.edu>
 Project-URL: Homepage, https://github.com/isremy/isogrids
 Project-URL: Bug Tracker, https://github.com/isremy/isogrids
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `isogrids-0.0.3/src/isogrids.egg-info/SOURCES.txt` & `isogrids-0.0.4/src/isogrids.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 src/isogrids.egg-info/top_level.txt
 src/isogrids/environments/__init__.py
 src/isogrids/environments/house_env/__init__.py
 src/isogrids/environments/house_env/build_houses.py
 src/isogrids/environments/house_env/house_furniture.py
 src/isogrids/environments/house_env/house_gen.py
 src/isogrids/environments/house_env/house_gen_timeout.py
-src/isogrids/environments/house_env/house_rooms.py
-src/isogrids/environments/house_env/plot_house_graph.py
+src/isogrids/environments/house_env/house_rooms.py
```

