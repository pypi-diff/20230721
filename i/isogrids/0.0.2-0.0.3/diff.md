# Comparing `tmp/isogrids-0.0.2.tar.gz` & `tmp/isogrids-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isogrids-0.0.2.tar", last modified: Thu Jul 20 22:36:31 2023, max compression
+gzip compressed data, was "isogrids-0.0.3.tar", last modified: Thu Jul 20 23:27:05 2023, max compression
```

## Comparing `isogrids-0.0.2.tar` & `isogrids-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 22:36:31.720440 isogrids-0.0.2/
--rw-rw-r--   0 isaac     (1001) isaac     (1001)     1067 2023-07-20 21:36:59.000000 isogrids-0.0.2/LICENSE
--rw-rw-r--   0 isaac     (1001) isaac     (1001)      760 2023-07-20 22:36:31.720440 isogrids-0.0.2/PKG-INFO
--rw-rw-r--   0 isaac     (1001) isaac     (1001)      167 2023-07-20 22:21:00.000000 isogrids-0.0.2/README.md
--rw-rw-r--   0 isaac     (1001) isaac     (1001)      665 2023-07-20 22:36:08.000000 isogrids-0.0.2/pyproject.toml
--rw-rw-r--   0 isaac     (1001) isaac     (1001)       38 2023-07-20 22:36:31.720440 isogrids-0.0.2/setup.cfg
-drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 22:36:31.720440 isogrids-0.0.2/src/
-drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 22:36:31.720440 isogrids-0.0.2/src/isogrids/
--rw-rw-r--   0 isaac     (1001) isaac     (1001)        0 2023-07-20 21:51:46.000000 isogrids-0.0.2/src/isogrids/__init__.py
--rw-rw-r--   0 isaac     (1001) isaac     (1001)       47 2023-07-13 20:48:01.000000 isogrids-0.0.2/src/isogrids/env.py
-drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 22:36:31.720440 isogrids-0.0.2/src/isogrids/environments/
-drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 22:36:31.720440 isogrids-0.0.2/src/isogrids/environments/house_env/
--rw-rw-r--   0 isaac     (1001) isaac     (1001)      936 2023-07-20 20:10:36.000000 isogrids-0.0.2/src/isogrids/environments/house_env/build_houses.py
--rw-rw-r--   0 isaac     (1001) isaac     (1001)     1607 2023-07-20 16:34:31.000000 isogrids-0.0.2/src/isogrids/environments/house_env/house_furniture.py
--rw-rw-r--   0 isaac     (1001) isaac     (1001)    17828 2023-07-20 20:10:23.000000 isogrids-0.0.2/src/isogrids/environments/house_env/house_gen.py
--rw-rw-r--   0 isaac     (1001) isaac     (1001)      703 2023-07-20 19:29:52.000000 isogrids-0.0.2/src/isogrids/environments/house_env/house_gen_timeout.py
--rw-rw-r--   0 isaac     (1001) isaac     (1001)     3221 2023-07-20 17:44:12.000000 isogrids-0.0.2/src/isogrids/environments/house_env/house_rooms.py
--rw-rw-r--   0 isaac     (1001) isaac     (1001)     2446 2023-07-20 19:14:35.000000 isogrids-0.0.2/src/isogrids/environments/house_env/plot_house_graph.py
-drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 22:36:31.720440 isogrids-0.0.2/src/isogrids.egg-info/
--rw-rw-r--   0 isaac     (1001) isaac     (1001)      760 2023-07-20 22:36:31.000000 isogrids-0.0.2/src/isogrids.egg-info/PKG-INFO
--rw-rw-r--   0 isaac     (1001) isaac     (1001)      541 2023-07-20 22:36:31.000000 isogrids-0.0.2/src/isogrids.egg-info/SOURCES.txt
--rw-rw-r--   0 isaac     (1001) isaac     (1001)        1 2023-07-20 22:36:31.000000 isogrids-0.0.2/src/isogrids.egg-info/dependency_links.txt
--rw-rw-r--   0 isaac     (1001) isaac     (1001)        9 2023-07-20 22:36:31.000000 isogrids-0.0.2/src/isogrids.egg-info/top_level.txt
+drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 23:27:05.810647 isogrids-0.0.3/
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)     1067 2023-07-20 21:36:59.000000 isogrids-0.0.3/LICENSE
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)      760 2023-07-20 23:27:05.810647 isogrids-0.0.3/PKG-INFO
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)      167 2023-07-20 22:21:00.000000 isogrids-0.0.3/README.md
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)      665 2023-07-20 23:26:59.000000 isogrids-0.0.3/pyproject.toml
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)       38 2023-07-20 23:27:05.810647 isogrids-0.0.3/setup.cfg
+drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 23:27:05.806647 isogrids-0.0.3/src/
+drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 23:27:05.806647 isogrids-0.0.3/src/isogrids/
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)       26 2023-07-20 23:19:08.000000 isogrids-0.0.3/src/isogrids/__init__.py
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)       47 2023-07-13 20:48:01.000000 isogrids-0.0.3/src/isogrids/env.py
+drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 23:27:05.806647 isogrids-0.0.3/src/isogrids/environments/
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)       24 2023-07-20 23:20:18.000000 isogrids-0.0.3/src/isogrids/environments/__init__.py
+drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 23:27:05.806647 isogrids-0.0.3/src/isogrids/environments/house_env/
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)       23 2023-07-20 23:21:02.000000 isogrids-0.0.3/src/isogrids/environments/house_env/__init__.py
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)      936 2023-07-20 20:10:36.000000 isogrids-0.0.3/src/isogrids/environments/house_env/build_houses.py
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)     1607 2023-07-20 16:34:31.000000 isogrids-0.0.3/src/isogrids/environments/house_env/house_furniture.py
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)    17489 2023-07-20 23:24:11.000000 isogrids-0.0.3/src/isogrids/environments/house_env/house_gen.py
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)      703 2023-07-20 19:29:52.000000 isogrids-0.0.3/src/isogrids/environments/house_env/house_gen_timeout.py
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)     3221 2023-07-20 17:44:12.000000 isogrids-0.0.3/src/isogrids/environments/house_env/house_rooms.py
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)     2446 2023-07-20 19:14:35.000000 isogrids-0.0.3/src/isogrids/environments/house_env/plot_house_graph.py
+drwxrwxr-x   0 isaac     (1001) isaac     (1001)        0 2023-07-20 23:27:05.806647 isogrids-0.0.3/src/isogrids.egg-info/
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)      760 2023-07-20 23:27:05.000000 isogrids-0.0.3/src/isogrids.egg-info/PKG-INFO
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)      627 2023-07-20 23:27:05.000000 isogrids-0.0.3/src/isogrids.egg-info/SOURCES.txt
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)        1 2023-07-20 23:27:05.000000 isogrids-0.0.3/src/isogrids.egg-info/dependency_links.txt
+-rw-rw-r--   0 isaac     (1001) isaac     (1001)        9 2023-07-20 23:27:05.000000 isogrids-0.0.3/src/isogrids.egg-info/top_level.txt
```

### Comparing `isogrids-0.0.2/LICENSE` & `isogrids-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `isogrids-0.0.2/PKG-INFO` & `isogrids-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isogrids
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package that generates and visualizes simple simulation environments and their respective scene graphs for planning-algorithm development
 Author-email: Isaac Remy <iremy@uw.edu>
 Project-URL: Homepage, https://github.com/isremy/isogrids
 Project-URL: Bug Tracker, https://github.com/isremy/isogrids
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `isogrids-0.0.2/pyproject.toml` & `isogrids-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "isogrids"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Isaac Remy", email="iremy@uw.edu" },
 ]
 description = "A package that generates and visualizes simple simulation environments and their respective scene graphs for planning-algorithm development"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `isogrids-0.0.2/src/isogrids/environments/house_env/build_houses.py` & `isogrids-0.0.3/src/isogrids/environments/house_env/build_houses.py`

 * *Files identical despite different names*

### Comparing `isogrids-0.0.2/src/isogrids/environments/house_env/house_furniture.py` & `isogrids-0.0.3/src/isogrids/environments/house_env/house_furniture.py`

 * *Files identical despite different names*

### Comparing `isogrids-0.0.2/src/isogrids/environments/house_env/house_gen.py` & `isogrids-0.0.3/src/isogrids/environments/house_env/house_gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import house_rooms, house_furniture
+from . import house_rooms, house_furniture
 import networkx as nx
 import random as rd
 import numpy as np
 import math
 import cv2
 from copy import deepcopy
 import time
-from house_gen_timeout import timeout
+from .house_gen_timeout import timeout
 
 SCALE_X = 700
 SCALE_Y = 700
 NUM_REGIONS = 6
 BLUR_KERNEL = 37
 DOORWAY_WIDTH = 70
 TIMEOUT = 15
@@ -181,45 +181,42 @@
 			queue = [start_node]
 			visited.add(start_node)
 			occurances_dict = {room_dict[start_node]["name"]: 1}
 			self.__graph.add_edge("house", room_dict[start_node]["name"])
 
 			while queue:
 				node = queue.pop(0)
-				# print(room_dict[node]["name"], " --> ", str(node))
 				neighbors = room_dict[node]["edges"]
 				adj_rooms, adj_room_scores = zip(*getattr(house_rooms, room_dict[node]["name"][:-1]).room_associations.items())
 
 				for neighbor in neighbors:
 					if neighbor not in visited:
 						room_name = rd.choices(adj_rooms, adj_room_scores)[0] + "0"
 
 						duplicate = getattr(house_rooms, room_name[:-1]).duplicate
 						again = 0
 						while(self.__graph.has_edge("house", room_name) and again == 0):
 							duplicate = getattr(house_rooms, room_name[:-1]).duplicate
 							if duplicate > 0.01:
 								again = np.random.binomial(1, duplicate ** occurances_dict[room_name[:-1]])
 								if again == 1:
-									# print("here")
 									room_name = room_name[:-1] + str(occurances_dict[room_name[:-1]])
 							else:
 								room_name = rd.choices(adj_rooms, adj_room_scores)[0]
 								room_name += "0"
 
 						self.__graph.add_edge("house", room_name)
 						self.__graph.add_edge(room_dict[node]["name"], room_name)
 						room_dict[neighbor]["name"] = room_name
 						
 						if room_name[:-1] not in  occurances_dict.keys():
 							occurances_dict[room_name[:-1]] = 1
 						else:
 							occurances_dict[room_name[:-1]] += 1
 
-						# print(room_name, " --> ", str(neighbor))
 						visited.add(neighbor)
 						queue.append(neighbor)
 					else:
 						self.__graph.add_edge(room_dict[node]["name"], room_dict[neighbor]["name"])
 
 		dfs(graph_obj_dict, max_room_id)
 
@@ -279,16 +276,14 @@
 					graph_obj_dict[room_id]["edges"] += (f_id,)
 					self.__graph.add_edge(graph_obj_dict[room_id]["name"], f_name)
 					cv2.circle(color_image, point, 5, (255, 0, 0), -1)
 				max_id += num_pieces
 
 
 		for obj in graph_obj_dict:
-			# fill_color = getattr(house_rooms, graph_obj_dict[room]["name"][:-1]).color
-			# cv2.fillPoly(color_image, [graph_obj_dict[room]["contour"]], fill_color)
 			text = graph_obj_dict[obj]["name"]
 			font = cv2.FONT_HERSHEY_SIMPLEX
 			font_scale = 0.5
 			font_color = (0, 0, 0)  # black color in BGR format
 			line_thickness = 2
 			text_size, _ = cv2.getTextSize(text, font, font_scale, line_thickness)
 			position = graph_obj_dict[obj]["centroid"]
@@ -478,15 +473,14 @@
 		end = time.time()
 		print("Generation time: ", str(end-start))
 
 		sorted_keys = sorted(size_img_dict, key=lambda k: size_img_dict[k], reverse=True)
 
 		black_image = np.zeros((len(img_list[0]), len(img_list[0][0]), 3), dtype=np.uint8)
 		for idx in sorted_keys:
-			# draw_bounds(rects_list[idx])
 			curr_img = rects_list[idx]
 			for i in range(len(curr_img)):
 				for j in range(len(curr_img[0])):
 					if curr_img[i][j].any():
 						black_image[i][j] = curr_img[i][j]
 
 		gray = cv2.cvtColor(black_image, cv2.COLOR_BGR2GRAY)
@@ -524,11 +518,8 @@
 				# Calculate the x and y coordinates of the centroid
 				centroid_x = int(M["m10"] / M["m00"])
 				centroid_y = int(M["m01"] / M["m00"])
 
 				# Append the centroid coordinates to the list
 				centroids.append((centroid_x, centroid_y))
 
-		return inverted_image, contours, centroids
-
-# h=House()
-# h.gen()
+		return inverted_image, contours, centroids
```

### Comparing `isogrids-0.0.2/src/isogrids/environments/house_env/house_gen_timeout.py` & `isogrids-0.0.3/src/isogrids/environments/house_env/house_gen_timeout.py`

 * *Files identical despite different names*

### Comparing `isogrids-0.0.2/src/isogrids/environments/house_env/house_rooms.py` & `isogrids-0.0.3/src/isogrids/environments/house_env/house_rooms.py`

 * *Files identical despite different names*

### Comparing `isogrids-0.0.2/src/isogrids/environments/house_env/plot_house_graph.py` & `isogrids-0.0.3/src/isogrids/environments/house_env/plot_house_graph.py`

 * *Files identical despite different names*

### Comparing `isogrids-0.0.2/src/isogrids.egg-info/PKG-INFO` & `isogrids-0.0.3/src/isogrids.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isogrids
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package that generates and visualizes simple simulation environments and their respective scene graphs for planning-algorithm development
 Author-email: Isaac Remy <iremy@uw.edu>
 Project-URL: Homepage, https://github.com/isremy/isogrids
 Project-URL: Bug Tracker, https://github.com/isremy/isogrids
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `isogrids-0.0.2/src/isogrids.egg-info/SOURCES.txt` & `isogrids-0.0.3/src/isogrids.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -3,13 +3,15 @@
 pyproject.toml
 src/isogrids/__init__.py
 src/isogrids/env.py
 src/isogrids.egg-info/PKG-INFO
 src/isogrids.egg-info/SOURCES.txt
 src/isogrids.egg-info/dependency_links.txt
 src/isogrids.egg-info/top_level.txt
+src/isogrids/environments/__init__.py
+src/isogrids/environments/house_env/__init__.py
 src/isogrids/environments/house_env/build_houses.py
 src/isogrids/environments/house_env/house_furniture.py
 src/isogrids/environments/house_env/house_gen.py
 src/isogrids/environments/house_env/house_gen_timeout.py
 src/isogrids/environments/house_env/house_rooms.py
 src/isogrids/environments/house_env/plot_house_graph.py
```

