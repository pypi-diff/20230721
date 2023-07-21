# Comparing `tmp/centerline-width-1.0.0.tar.gz` & `tmp/centerline-width-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/centerline-width-1.0.0.tar", last modified: Sun Jul  9 22:03:56 2023, max compression
+gzip compressed data, was "dist/centerline-width-1.0.1.tar", last modified: Fri Jul 21 21:24:06 2023, max compression
```

## Comparing `centerline-width-1.0.0.tar` & `centerline-width-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-09 22:03:56.576991 centerline-width-1.0.0/
--rw-rw-r--   0 user      (1000) user      (1000)    42692 2023-07-09 22:03:56.572991 centerline-width-1.0.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    37006 2023-07-09 08:39:47.000000 centerline-width-1.0.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-09 22:03:56.552991 centerline-width-1.0.0/centerline_width/
--rw-rw-r--   0 user      (1000) user      (1000)     1632 2023-06-23 06:05:21.000000 centerline-width-1.0.0/centerline_width/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    26135 2023-06-26 21:50:27.000000 centerline-width-1.0.0/centerline_width/centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)    16829 2023-06-26 21:48:17.000000 centerline-width-1.0.0/centerline_width/error_handling.py
--rw-rw-r--   0 user      (1000) user      (1000)     1854 2023-05-18 02:15:59.000000 centerline-width-1.0.0/centerline_width/getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)     9280 2023-06-28 04:14:39.000000 centerline-width-1.0.0/centerline_width/plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     6759 2023-06-01 21:17:09.000000 centerline-width-1.0.0/centerline_width/preprocessing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-09 22:03:56.572991 centerline-width-1.0.0/centerline_width/pytests/
--rw-rw-r--   0 user      (1000) user      (1000)    13693 2023-06-26 21:49:08.000000 centerline-width-1.0.0/centerline_width/pytests/test_centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-05-24 19:31:02.000000 centerline-width-1.0.0/centerline_width/pytests/test_getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)    12990 2023-06-24 07:23:37.000000 centerline-width-1.0.0/centerline_width/pytests/test_plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-1.0.0/centerline_width/pytests/test_preprocessing.py
--rw-rw-r--   0 user      (1000) user      (1000)     5105 2023-06-24 07:13:29.000000 centerline-width-1.0.0/centerline_width/pytests/test_riverCenterlineClass.py
--rw-rw-r--   0 user      (1000) user      (1000)     6510 2023-06-26 21:49:56.000000 centerline-width-1.0.0/centerline_width/riverCenterlineClass.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-09 22:03:56.556991 centerline-width-1.0.0/centerline_width.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    42692 2023-07-09 22:03:56.000000 centerline-width-1.0.0/centerline_width.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      700 2023-07-09 22:03:56.000000 centerline-width-1.0.0/centerline_width.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-09 22:03:56.000000 centerline-width-1.0.0/centerline_width.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      160 2023-07-09 22:03:56.000000 centerline-width-1.0.0/centerline_width.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       17 2023-07-09 22:03:56.000000 centerline-width-1.0.0/centerline_width.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-09 22:03:56.576991 centerline-width-1.0.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1846 2023-07-09 22:02:40.000000 centerline-width-1.0.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-21 21:24:06.287201 centerline-width-1.0.1/
+-rw-rw-r--   0 user      (1000) user      (1000)    46218 2023-07-21 21:24:06.287201 centerline-width-1.0.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    40212 2023-07-13 19:32:57.000000 centerline-width-1.0.1/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-21 21:24:06.279201 centerline-width-1.0.1/centerline_width/
+-rw-rw-r--   0 user      (1000) user      (1000)     1632 2023-06-23 06:05:21.000000 centerline-width-1.0.1/centerline_width/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    26135 2023-06-26 21:50:27.000000 centerline-width-1.0.1/centerline_width/centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16829 2023-06-26 21:48:17.000000 centerline-width-1.0.1/centerline_width/error_handling.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1854 2023-05-18 02:15:59.000000 centerline-width-1.0.1/centerline_width/getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9312 2023-07-12 06:10:05.000000 centerline-width-1.0.1/centerline_width/plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6759 2023-06-01 21:17:09.000000 centerline-width-1.0.1/centerline_width/preprocessing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-21 21:24:06.287201 centerline-width-1.0.1/centerline_width/pytests/
+-rw-rw-r--   0 user      (1000) user      (1000)    13693 2023-06-26 21:49:08.000000 centerline-width-1.0.1/centerline_width/pytests/test_centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-05-24 19:31:02.000000 centerline-width-1.0.1/centerline_width/pytests/test_getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12990 2023-06-24 07:23:37.000000 centerline-width-1.0.1/centerline_width/pytests/test_plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-1.0.1/centerline_width/pytests/test_preprocessing.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5105 2023-06-24 07:13:29.000000 centerline-width-1.0.1/centerline_width/pytests/test_riverCenterlineClass.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6510 2023-06-26 21:49:56.000000 centerline-width-1.0.1/centerline_width/riverCenterlineClass.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-21 21:24:06.279201 centerline-width-1.0.1/centerline_width.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    46218 2023-07-21 21:24:06.000000 centerline-width-1.0.1/centerline_width.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      700 2023-07-21 21:24:06.000000 centerline-width-1.0.1/centerline_width.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-21 21:24:06.000000 centerline-width-1.0.1/centerline_width.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      160 2023-07-21 21:24:06.000000 centerline-width-1.0.1/centerline_width.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2023-07-21 21:24:06.000000 centerline-width-1.0.1/centerline_width.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-21 21:24:06.287201 centerline-width-1.0.1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1846 2023-07-21 21:22:06.000000 centerline-width-1.0.1/setup.py
```

### Comparing `centerline-width-1.0.0/PKG-INFO` & `centerline-width-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v1.0.0.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v1.0.1.tar.gz
 Description: # Centerline-Width
          <p align="center">
           <img src="https://raw.githubusercontent.com/cyschneck/centerline-width/main/assets/centerline_logo.jpg" />
         </p>
         
         ![PyPi](https://img.shields.io/pypi/v/centerline-width)
         ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
@@ -87,15 +87,33 @@
         ```python
         river.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
         ```
         ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
         
         For more details to fix unexpected behavior or error code: [Debugging, Error Handling, and Edge Cases](#debugging-error-handling-and-edge-cases)
         
+        For a complete example script to run centerline-width: [centerline_width_example_script.py](https://github.com/cyschneck/centerline-width/blob/main/data/example_script_outputs/centerline_width_example_script.py) with [example outputs](https://github.com/cyschneck/centerline-width/tree/main/data/example_script_outputs)
+        
         ## Preprocessing
+        ### Generating KML files from Google Earth Pro
+        Riverbanks can be defined here as the high-contrast boundary between active/recently-active flow and the surrounding landscape. We will be mapping the right and left bank separately
+        
+        **Step 1**
+        
+        Map the left bank using the path tool. You can zoom into the river using the scroll-wheel. Flatten the mapping projection by pressing `u`. Leave the pop-up window open while you are mapping. You can erase the last point placed in a path by left-clicking. To erase a different point on the path, select the point with a right-click and then erase with a left-click and then select the last point to continue mapping downstream. To move a point, select it with a right-click. The selected point is highlighted blue, other points in the current path are highlighted red. The mapped distance downstream is shown in the measurements tab in the path tool pop-up window. When done mapping the left bank, close the pop-up window for the path
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/generate_kml.png)
+        
+        **Step 2**
+        
+        Save the path to a .kml file by right clicking on the path in Places and selecting 'save as'. Be sure to save as a .kml and not .kmz file. It is generally good practice to do this for each new path to ensure that no work is lost if Google Earth Pro crashes
+        
+        **Step 3**
+        
+        Repeat (1) and (2) for the right bank by starting a new path
+        
         ### Convert KML files to Text File
         
         Convert two .kml files from Google Earth Pro (for the left and right bank) and export the coordinates into a text file
         
         ```
         extractPointsToTextFile(left_kml=None,
         			right_kml=None,
@@ -178,15 +196,25 @@
         * [OPTIONAL] optional_cutoff (int): Include only the first x number of the data to chart (useful for debugging)
         * [OPTIONAL] interpolate_data (boolean): Interpolate between existing data by adding additional points
         * [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
         * [OPTIONAL] interpolate_n_centerpoints (int): Number of points used to interpolate the Voronoi centerline, defaults to the the length of the data frame (df_len)
         * [OPTIONAL] equal_distance (int): Equal distance between points (in meters) used to interpolate the Voronoi centerline, defaults 10 meters
         * [OPTIONAL] ellipsoid (string): Ellipsoid definition of Earth to provide size and shape for built-in functions to convert degrees to meters, options include (is sensitive to case): ["GRS80", "airy", "bessel", "clrk66", "intl", "WGS60", "WGS66", "WGS72", "WGS84", "sphere"] for more details: ["Built-in ellipsoid defintions"](https://proj.org/en/9.2/usage/ellipsoids.html#built-in-ellipsoid-definitions), defaults to "WGS84"
         
-        **Solutions for sparse data:**
+        **Equal Distance - Equal linear distance between points**
+        
+        `equal_distance` will generate points along the centerline that are an equal linear distance from one another in meters. When `equal_distance=5` each point will be 5 meters apart
+        
+        | equal_distance=5 | equal_distance=20 |
+        | ------------- | ------------- |
+        | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/equal_distance_5_m.jpg) | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/equal_distance_20_m.jpg) |
+        
+        The red pins represent the equal distance centerline coordinates produced by centerline-width. The yellow line is the distance measured in Google Earth Pro between the points. The mapped river banks are in purple.
+        
+        **Interpolation - A solution for sparse data**
         
         `interpolate_data` is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps due to the combination of sparse data and a narrow river (See: Debugging, Error Handling, and Edge Cases - Fix Gaps and Jagged Centerlines). By default, `interpolate_data=True` will add 5 additional points between each existing point but can be increased or decreased by modifying the `interpolate_n` option
         
         `interpolate_n_centerpoints` is an option that can be used to increase the resolution (number of points) of the centerline found by the Voronoi vertices. By default, will evenly space out to the size of the dataframe. Can artificially increase the amount of width lines generated by increasing the number of center points. When `interpolate_n_centerpoints` increases, the number of width lines generated will increase (and visa versa)
         
         | interpolate_n_centerpoints=75 | interpolate_n_centerpoints=200 |
         | ------------- | ------------- |
@@ -224,25 +252,25 @@
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         ```
         
         ### Return Latitude/Longitude Coordinates of Centerline
-        Return the latitude/longitude coordinates of the centerline based on the left and right banks
+        Return the latitude/longitude coordinates in units of decimal-degrees of the centerline based on the left and right banks
         
         **Types of Centerlines**
         
         There are four types of centerline coordinates formed from the riverbank data
         
         - **Voronoi centerline**: centerline generated from where Voronoi vertices intersect within the river
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/voronoi_centerline.png)
-        - **Equal Distance Centerline**: centerline based on Voronoi centerline but each point is equally spaced out from the previous (in meters) and takes into account the radius of the Earth to convert degrees to meters
+        - **Equal Distance Centerline**: centerline based on Voronoi centerline but each point is equally spaced out from the previous (in meters) and takes into account the radius of the Earth to convert degrees to meters (example below: `equal_distance=10`)
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/equal_distance_centerline.png)
-        - **Evenly Spaced Centerline**: centerline based on Voronoi centerline but evenly spaced with a fixed number of points
+        - **Evenly Spaced Centerline**: centerline based on Voronoi centerline but evenly spaced with a fixed number of points (example: `interpolate_n_centerpoints=200`)
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/evenly_spaced_centerline.png)
         - **Smoothed Centerline**: centerline generated from the evenly spaced centerline but smoothed by a b-spline
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/smoothed_centerline.png)
         
         Centerline coordinates are formed by the Voronoi vertices
         ```
         river_object.centerlineVoronoi
@@ -262,21 +290,21 @@
         ```
         river_object.centerlineSmoothed
         ```
         
         Example:
         ```python
         import centerline_width
-        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=15)
+        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_centerline_coordinates = river_object.centerlineVoronoi
         ```
         Output is a list of tuples: (example) `[(-92.86788596499872, 30.03786596717931), (-92.86789573751797, 30.037834641974108), (-92.8679141386283, 30.037789636848878), (-92.8679251193248, 30.037756853899904), (-92.86796903819089, 30.03765423778148), (-92.86797335733262, 30.037643336049054), (-92.8679920356456, 30.037592224469797), (-92.86800576063828, 30.037555441489403), (-92.86800841510367, 30.037546512833107), (-92.8680119498663, 30.03753043193875)]`
         
         ### Save Centerline Coordinates to a .CSV File
-        Save the centerline coordinates to a csv file with columns for latitude and longitude
+        Save the centerline coordinates to a csv file with columns for latitude and longitude. This is the file format for a table of (latitude,longitude) pairs accepted to import back into Google Earth Pro.
         
         ```
         saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi")
         ```
         * **[REQUIRED]** save_to_csv (string): CSV filename, requires a .csv extension
         * [OPTIONAL] centerline_type (string): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
         * [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type> Centerline Latitude (Deg)`
@@ -315,15 +343,15 @@
         Return the length of the centerline found between the left and right bank generated by the Voronoi diagram
         ```
         river_object.centerlineLength
         ```
         Length returned in kilometers
         ```python
         import centerline_width
-        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=550)
+        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_centerline_length = river_object.centerlineLength
         ```
         The length of the river centerline returns `215.34700589636674` km
         
         ## Plot Centerline in Matplotlib
         Plot the centerline created from a list of right and left banks with Voronoi vertices
         
@@ -417,15 +445,15 @@
         			apply_smoothing=True,
         			remove_intersections=False,
         			save_to_csv=None)
         ```
         * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
         * [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
         * [OPTIONAL] remove_intersections (boolean): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to True
-        * [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (<units specified>)`)
+        * [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (km)`)
         
         Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordinates may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_width_dict = river_object.riverWidthFromCenterline(transect_span_distance=3,
@@ -442,23 +470,26 @@
         
         ### Right and Left bank points are plotted (X-Axis for Latitude, Y-Axis for Longitude)
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example1.png)
         
         ### Generate a polygon to encapsulate the river between the right and left banks to define in and outside of river
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example2.png)
         
-        ### Generate a Voronoi based on the points along the riverbanks
+        ### Generate a Voronoi diagram based on the points along the riverbanks
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example3.png)
         
         ### Display Voronoi ridge vertices that lie within the polygon (within the riverbanks)
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example4.png)
         
-        ### Filter out any point pairs that only have one connection to filter out the short dead end paths and find the starting and ending node based on distance from the top and bottom of polygon
+        ### Filter out any point pairs that only have one connection to filter out the short dead end paths
         With the vertices removed, it is possible to form multiple unconnected graphs within the polygon. The largest subgraph is assumed to contain the centerline and the other subgraphs are filtered out
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example6.png)
+        
+        ### Find the starting and ending node based on distance from the top and bottom of polygon
+        The starting/ending node is defined by the vertice closest to the top/bottom of the polygon along the longest path
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example7.png)
         
         ### Find the shortest path from the starting node to the ending node ([Dijkstra's Algorithm](https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.shortest_paths.generic.shortest_path.html#networkx.algorithms.shortest_paths.generic.shortest_path))
         | Points on Riverbank | NetworkX Graph of Points on Riverbank |
         | ------------- | ------------- |
         | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example10.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example9.png) |
         
@@ -551,14 +582,23 @@
         
          <p align="center">
           <img src="https://user-images.githubusercontent.com/22159116/222872092-e0b579cc-4f84-4f49-aa53-397785fb9bf2.png" />
           <img src="https://user-images.githubusercontent.com/22159116/222872119-7c485ee2-4ffd-413a-9e4f-b043b122d2bb.png" />
           <img src="https://user-images.githubusercontent.com/22159116/222872019-12931138-9e10-4e51-aa1e-552e72d09af0.png" />
         </p>
         
+        ## Acknowledging Software 
+        Please acknowledge the use of this software in any publications:
+        
+        ```
+        "River centerline/width extraction software was provided by C. Y. Schneck and U. G. Schneck, and is available at URL: https://github.com/cyschneck/centerline-width."
+        ```
+        Please send a copy of such publications to: cyschneck@gmail.com and ugschneck@gmail.com
+        
+        
         This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not necessarily reflect the views of the National Science Foundation.
         
         ## Bug and Feature Request
         
         Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/cyschneck/centerline-width/issues) or to ugschneck@gmail.com/cyschneck@gmail.com
         
 Keywords: geophysics,python,voronoi,networkx,centerline,centerline-extraction,centerline-detection,rivers,river-bank-length,river-bank,limnology,hydrology
```

### Comparing `centerline-width-1.0.0/README.md` & `centerline-width-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -79,15 +79,33 @@
 ```python
 river.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
 ```
 ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
 
 For more details to fix unexpected behavior or error code: [Debugging, Error Handling, and Edge Cases](#debugging-error-handling-and-edge-cases)
 
+For a complete example script to run centerline-width: [centerline_width_example_script.py](https://github.com/cyschneck/centerline-width/blob/main/data/example_script_outputs/centerline_width_example_script.py) with [example outputs](https://github.com/cyschneck/centerline-width/tree/main/data/example_script_outputs)
+
 ## Preprocessing
+### Generating KML files from Google Earth Pro
+Riverbanks can be defined here as the high-contrast boundary between active/recently-active flow and the surrounding landscape. We will be mapping the right and left bank separately
+
+**Step 1**
+
+Map the left bank using the path tool. You can zoom into the river using the scroll-wheel. Flatten the mapping projection by pressing `u`. Leave the pop-up window open while you are mapping. You can erase the last point placed in a path by left-clicking. To erase a different point on the path, select the point with a right-click and then erase with a left-click and then select the last point to continue mapping downstream. To move a point, select it with a right-click. The selected point is highlighted blue, other points in the current path are highlighted red. The mapped distance downstream is shown in the measurements tab in the path tool pop-up window. When done mapping the left bank, close the pop-up window for the path
+![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/generate_kml.png)
+
+**Step 2**
+
+Save the path to a .kml file by right clicking on the path in Places and selecting 'save as'. Be sure to save as a .kml and not .kmz file. It is generally good practice to do this for each new path to ensure that no work is lost if Google Earth Pro crashes
+
+**Step 3**
+
+Repeat (1) and (2) for the right bank by starting a new path
+
 ### Convert KML files to Text File
 
 Convert two .kml files from Google Earth Pro (for the left and right bank) and export the coordinates into a text file
 
 ```
 extractPointsToTextFile(left_kml=None,
 			right_kml=None,
@@ -170,15 +188,25 @@
 * [OPTIONAL] optional_cutoff (int): Include only the first x number of the data to chart (useful for debugging)
 * [OPTIONAL] interpolate_data (boolean): Interpolate between existing data by adding additional points
 * [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
 * [OPTIONAL] interpolate_n_centerpoints (int): Number of points used to interpolate the Voronoi centerline, defaults to the the length of the data frame (df_len)
 * [OPTIONAL] equal_distance (int): Equal distance between points (in meters) used to interpolate the Voronoi centerline, defaults 10 meters
 * [OPTIONAL] ellipsoid (string): Ellipsoid definition of Earth to provide size and shape for built-in functions to convert degrees to meters, options include (is sensitive to case): ["GRS80", "airy", "bessel", "clrk66", "intl", "WGS60", "WGS66", "WGS72", "WGS84", "sphere"] for more details: ["Built-in ellipsoid defintions"](https://proj.org/en/9.2/usage/ellipsoids.html#built-in-ellipsoid-definitions), defaults to "WGS84"
 
-**Solutions for sparse data:**
+**Equal Distance - Equal linear distance between points**
+
+`equal_distance` will generate points along the centerline that are an equal linear distance from one another in meters. When `equal_distance=5` each point will be 5 meters apart
+
+| equal_distance=5 | equal_distance=20 |
+| ------------- | ------------- |
+| ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/equal_distance_5_m.jpg) | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/equal_distance_20_m.jpg) |
+
+The red pins represent the equal distance centerline coordinates produced by centerline-width. The yellow line is the distance measured in Google Earth Pro between the points. The mapped river banks are in purple.
+
+**Interpolation - A solution for sparse data**
 
 `interpolate_data` is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps due to the combination of sparse data and a narrow river (See: Debugging, Error Handling, and Edge Cases - Fix Gaps and Jagged Centerlines). By default, `interpolate_data=True` will add 5 additional points between each existing point but can be increased or decreased by modifying the `interpolate_n` option
 
 `interpolate_n_centerpoints` is an option that can be used to increase the resolution (number of points) of the centerline found by the Voronoi vertices. By default, will evenly space out to the size of the dataframe. Can artificially increase the amount of width lines generated by increasing the number of center points. When `interpolate_n_centerpoints` increases, the number of width lines generated will increase (and visa versa)
 
 | interpolate_n_centerpoints=75 | interpolate_n_centerpoints=200 |
 | ------------- | ------------- |
@@ -216,25 +244,25 @@
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 ```
 
 ### Return Latitude/Longitude Coordinates of Centerline
-Return the latitude/longitude coordinates of the centerline based on the left and right banks
+Return the latitude/longitude coordinates in units of decimal-degrees of the centerline based on the left and right banks
 
 **Types of Centerlines**
 
 There are four types of centerline coordinates formed from the riverbank data
 
 - **Voronoi centerline**: centerline generated from where Voronoi vertices intersect within the river
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/voronoi_centerline.png)
-- **Equal Distance Centerline**: centerline based on Voronoi centerline but each point is equally spaced out from the previous (in meters) and takes into account the radius of the Earth to convert degrees to meters
+- **Equal Distance Centerline**: centerline based on Voronoi centerline but each point is equally spaced out from the previous (in meters) and takes into account the radius of the Earth to convert degrees to meters (example below: `equal_distance=10`)
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/equal_distance_centerline.png)
-- **Evenly Spaced Centerline**: centerline based on Voronoi centerline but evenly spaced with a fixed number of points
+- **Evenly Spaced Centerline**: centerline based on Voronoi centerline but evenly spaced with a fixed number of points (example: `interpolate_n_centerpoints=200`)
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/evenly_spaced_centerline.png)
 - **Smoothed Centerline**: centerline generated from the evenly spaced centerline but smoothed by a b-spline
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/smoothed_centerline.png)
 
 Centerline coordinates are formed by the Voronoi vertices
 ```
 river_object.centerlineVoronoi
@@ -254,21 +282,21 @@
 ```
 river_object.centerlineSmoothed
 ```
 
 Example:
 ```python
 import centerline_width
-river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=15)
+river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_centerline_coordinates = river_object.centerlineVoronoi
 ```
 Output is a list of tuples: (example) `[(-92.86788596499872, 30.03786596717931), (-92.86789573751797, 30.037834641974108), (-92.8679141386283, 30.037789636848878), (-92.8679251193248, 30.037756853899904), (-92.86796903819089, 30.03765423778148), (-92.86797335733262, 30.037643336049054), (-92.8679920356456, 30.037592224469797), (-92.86800576063828, 30.037555441489403), (-92.86800841510367, 30.037546512833107), (-92.8680119498663, 30.03753043193875)]`
 
 ### Save Centerline Coordinates to a .CSV File
-Save the centerline coordinates to a csv file with columns for latitude and longitude
+Save the centerline coordinates to a csv file with columns for latitude and longitude. This is the file format for a table of (latitude,longitude) pairs accepted to import back into Google Earth Pro.
 
 ```
 saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi")
 ```
 * **[REQUIRED]** save_to_csv (string): CSV filename, requires a .csv extension
 * [OPTIONAL] centerline_type (string): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
 * [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type> Centerline Latitude (Deg)`
@@ -307,15 +335,15 @@
 Return the length of the centerline found between the left and right bank generated by the Voronoi diagram
 ```
 river_object.centerlineLength
 ```
 Length returned in kilometers
 ```python
 import centerline_width
-river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=550)
+river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_centerline_length = river_object.centerlineLength
 ```
 The length of the river centerline returns `215.34700589636674` km
 
 ## Plot Centerline in Matplotlib
 Plot the centerline created from a list of right and left banks with Voronoi vertices
 
@@ -409,15 +437,15 @@
 			apply_smoothing=True,
 			remove_intersections=False,
 			save_to_csv=None)
 ```
 * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
 * [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
 * [OPTIONAL] remove_intersections (boolean): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to True
-* [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (<units specified>)`)
+* [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (km)`)
 
 Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordinates may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_width_dict = river_object.riverWidthFromCenterline(transect_span_distance=3,
@@ -434,23 +462,26 @@
 
 ### Right and Left bank points are plotted (X-Axis for Latitude, Y-Axis for Longitude)
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example1.png)
 
 ### Generate a polygon to encapsulate the river between the right and left banks to define in and outside of river
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example2.png)
 
-### Generate a Voronoi based on the points along the riverbanks
+### Generate a Voronoi diagram based on the points along the riverbanks
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example3.png)
 
 ### Display Voronoi ridge vertices that lie within the polygon (within the riverbanks)
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example4.png)
 
-### Filter out any point pairs that only have one connection to filter out the short dead end paths and find the starting and ending node based on distance from the top and bottom of polygon
+### Filter out any point pairs that only have one connection to filter out the short dead end paths
 With the vertices removed, it is possible to form multiple unconnected graphs within the polygon. The largest subgraph is assumed to contain the centerline and the other subgraphs are filtered out
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example6.png)
+
+### Find the starting and ending node based on distance from the top and bottom of polygon
+The starting/ending node is defined by the vertice closest to the top/bottom of the polygon along the longest path
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example7.png)
 
 ### Find the shortest path from the starting node to the ending node ([Dijkstra's Algorithm](https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.shortest_paths.generic.shortest_path.html#networkx.algorithms.shortest_paths.generic.shortest_path))
 | Points on Riverbank | NetworkX Graph of Points on Riverbank |
 | ------------- | ------------- |
 | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example10.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example9.png) |
 
@@ -543,12 +574,21 @@
 
  <p align="center">
   <img src="https://user-images.githubusercontent.com/22159116/222872092-e0b579cc-4f84-4f49-aa53-397785fb9bf2.png" />
   <img src="https://user-images.githubusercontent.com/22159116/222872119-7c485ee2-4ffd-413a-9e4f-b043b122d2bb.png" />
   <img src="https://user-images.githubusercontent.com/22159116/222872019-12931138-9e10-4e51-aa1e-552e72d09af0.png" />
 </p>
 
+## Acknowledging Software 
+Please acknowledge the use of this software in any publications:
+
+```
+"River centerline/width extraction software was provided by C. Y. Schneck and U. G. Schneck, and is available at URL: https://github.com/cyschneck/centerline-width."
+```
+Please send a copy of such publications to: cyschneck@gmail.com and ugschneck@gmail.com
+
+
 This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not necessarily reflect the views of the National Science Foundation.
 
 ## Bug and Feature Request
 
 Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/cyschneck/centerline-width/issues) or to ugschneck@gmail.com/cyschneck@gmail.com
```

### Comparing `centerline-width-1.0.0/centerline_width/__init__.py` & `centerline-width-1.0.1/centerline_width/__init__.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.0.0/centerline_width/centerline.py` & `centerline-width-1.0.1/centerline_width/centerline.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.0.0/centerline_width/error_handling.py` & `centerline-width-1.0.1/centerline_width/error_handling.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.0.0/centerline_width/getCoordinatesKML.py` & `centerline-width-1.0.1/centerline_width/getCoordinatesKML.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.0.0/centerline_width/plotDiagrams.py` & `centerline-width-1.0.1/centerline_width/plotDiagrams.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,22 +62,22 @@
 		centerline_coordinates_by_type = river_object.centerlineSmoothed
 		centerline_legend = "Smoothed Centerlined Coordiantes"
 
 	if centerline_coordinates_by_type:
 		valid_path_through = True
 		if display_true_centerline:
 			if marker_type == "Line":
-				plt.plot(*zip(*centerline_coordinates_by_type), c=centerline_color, label=centerline_legend)
+				plt.plot(*zip(*centerline_coordinates_by_type), c=centerline_color, label=centerline_legend, zorder=10)
 			if marker_type == "Scatter":
 				x = []
 				y = []
 				for k, v in centerline_coordinates_by_type:
 					x.append(k)
 					y.append(v)
-				plt.scatter(x, y, c=centerline_color, label=centerline_legend, s=8)
+				plt.scatter(x, y, c=centerline_color, label=centerline_legend, s=8, zorder=10)
 
 	# Dynamically assign the starting and ending
 	if river_object.starting_node is not None: # error handling for when data is too small to generate centerline coordiantes
 		plt.scatter(river_object.starting_node[0], river_object.starting_node[1], c="green", label="Starting Node", s=45)
 		plt.scatter(river_object.ending_node[0], river_object.ending_node[1], c="red", label="Ending Node", s=45)
 
 	return fig, ax, valid_path_through
@@ -109,15 +109,15 @@
 	# Display the Voronoi Diagram
 	if display_voronoi:
 		voronoi_plot_2d(river_object.bank_voronoi, show_points=True, point_size=1, ax=ax)
 
 	# Plot all possible paths with text for positions
 	if display_all_possible_paths:
 		for i in range(len(river_object.x_voronoi_ridge_point)):
-			plt.plot(river_object.x_voronoi_ridge_point[i], river_object.y_voronoi_ridge_point[i], 'cyan', linewidth=1)
+			plt.plot(river_object.x_voronoi_ridge_point[i], river_object.y_voronoi_ridge_point[i], 'cyan', linewidth=1, zorder=1)
 
 	# Plot Title, Legends, and Axis Labels
 	if not plot_title:
 		plt.title("River Coordinates: Valid Centerline = {0}, Valid Polygon = {1}, Interpolated = {2}".format(valid_path_through, river_object.bank_polygon.is_valid, river_object.interpolate_data))
 	else:
 		plt.title(plot_title)
 	plt.xlabel("Longitude (°)")
```

### Comparing `centerline-width-1.0.0/centerline_width/preprocessing.py` & `centerline-width-1.0.1/centerline_width/preprocessing.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.0.0/centerline_width/pytests/test_centerline.py` & `centerline-width-1.0.1/centerline_width/pytests/test_centerline.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.0.0/centerline_width/pytests/test_getCoordinatesKML.py` & `centerline-width-1.0.1/centerline_width/pytests/test_getCoordinatesKML.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.0.0/centerline_width/pytests/test_plotDiagrams.py` & `centerline-width-1.0.1/centerline_width/pytests/test_plotDiagrams.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.0.0/centerline_width/pytests/test_preprocessing.py` & `centerline-width-1.0.1/centerline_width/pytests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.0.0/centerline_width/pytests/test_riverCenterlineClass.py` & `centerline-width-1.0.1/centerline_width/pytests/test_riverCenterlineClass.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.0.0/centerline_width/riverCenterlineClass.py` & `centerline-width-1.0.1/centerline_width/riverCenterlineClass.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.0.0/centerline_width.egg-info/PKG-INFO` & `centerline-width-1.0.1/centerline_width.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v1.0.0.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v1.0.1.tar.gz
 Description: # Centerline-Width
          <p align="center">
           <img src="https://raw.githubusercontent.com/cyschneck/centerline-width/main/assets/centerline_logo.jpg" />
         </p>
         
         ![PyPi](https://img.shields.io/pypi/v/centerline-width)
         ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
@@ -87,15 +87,33 @@
         ```python
         river.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
         ```
         ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
         
         For more details to fix unexpected behavior or error code: [Debugging, Error Handling, and Edge Cases](#debugging-error-handling-and-edge-cases)
         
+        For a complete example script to run centerline-width: [centerline_width_example_script.py](https://github.com/cyschneck/centerline-width/blob/main/data/example_script_outputs/centerline_width_example_script.py) with [example outputs](https://github.com/cyschneck/centerline-width/tree/main/data/example_script_outputs)
+        
         ## Preprocessing
+        ### Generating KML files from Google Earth Pro
+        Riverbanks can be defined here as the high-contrast boundary between active/recently-active flow and the surrounding landscape. We will be mapping the right and left bank separately
+        
+        **Step 1**
+        
+        Map the left bank using the path tool. You can zoom into the river using the scroll-wheel. Flatten the mapping projection by pressing `u`. Leave the pop-up window open while you are mapping. You can erase the last point placed in a path by left-clicking. To erase a different point on the path, select the point with a right-click and then erase with a left-click and then select the last point to continue mapping downstream. To move a point, select it with a right-click. The selected point is highlighted blue, other points in the current path are highlighted red. The mapped distance downstream is shown in the measurements tab in the path tool pop-up window. When done mapping the left bank, close the pop-up window for the path
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/generate_kml.png)
+        
+        **Step 2**
+        
+        Save the path to a .kml file by right clicking on the path in Places and selecting 'save as'. Be sure to save as a .kml and not .kmz file. It is generally good practice to do this for each new path to ensure that no work is lost if Google Earth Pro crashes
+        
+        **Step 3**
+        
+        Repeat (1) and (2) for the right bank by starting a new path
+        
         ### Convert KML files to Text File
         
         Convert two .kml files from Google Earth Pro (for the left and right bank) and export the coordinates into a text file
         
         ```
         extractPointsToTextFile(left_kml=None,
         			right_kml=None,
@@ -178,15 +196,25 @@
         * [OPTIONAL] optional_cutoff (int): Include only the first x number of the data to chart (useful for debugging)
         * [OPTIONAL] interpolate_data (boolean): Interpolate between existing data by adding additional points
         * [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
         * [OPTIONAL] interpolate_n_centerpoints (int): Number of points used to interpolate the Voronoi centerline, defaults to the the length of the data frame (df_len)
         * [OPTIONAL] equal_distance (int): Equal distance between points (in meters) used to interpolate the Voronoi centerline, defaults 10 meters
         * [OPTIONAL] ellipsoid (string): Ellipsoid definition of Earth to provide size and shape for built-in functions to convert degrees to meters, options include (is sensitive to case): ["GRS80", "airy", "bessel", "clrk66", "intl", "WGS60", "WGS66", "WGS72", "WGS84", "sphere"] for more details: ["Built-in ellipsoid defintions"](https://proj.org/en/9.2/usage/ellipsoids.html#built-in-ellipsoid-definitions), defaults to "WGS84"
         
-        **Solutions for sparse data:**
+        **Equal Distance - Equal linear distance between points**
+        
+        `equal_distance` will generate points along the centerline that are an equal linear distance from one another in meters. When `equal_distance=5` each point will be 5 meters apart
+        
+        | equal_distance=5 | equal_distance=20 |
+        | ------------- | ------------- |
+        | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/equal_distance_5_m.jpg) | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/equal_distance_20_m.jpg) |
+        
+        The red pins represent the equal distance centerline coordinates produced by centerline-width. The yellow line is the distance measured in Google Earth Pro between the points. The mapped river banks are in purple.
+        
+        **Interpolation - A solution for sparse data**
         
         `interpolate_data` is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps due to the combination of sparse data and a narrow river (See: Debugging, Error Handling, and Edge Cases - Fix Gaps and Jagged Centerlines). By default, `interpolate_data=True` will add 5 additional points between each existing point but can be increased or decreased by modifying the `interpolate_n` option
         
         `interpolate_n_centerpoints` is an option that can be used to increase the resolution (number of points) of the centerline found by the Voronoi vertices. By default, will evenly space out to the size of the dataframe. Can artificially increase the amount of width lines generated by increasing the number of center points. When `interpolate_n_centerpoints` increases, the number of width lines generated will increase (and visa versa)
         
         | interpolate_n_centerpoints=75 | interpolate_n_centerpoints=200 |
         | ------------- | ------------- |
@@ -224,25 +252,25 @@
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         ```
         
         ### Return Latitude/Longitude Coordinates of Centerline
-        Return the latitude/longitude coordinates of the centerline based on the left and right banks
+        Return the latitude/longitude coordinates in units of decimal-degrees of the centerline based on the left and right banks
         
         **Types of Centerlines**
         
         There are four types of centerline coordinates formed from the riverbank data
         
         - **Voronoi centerline**: centerline generated from where Voronoi vertices intersect within the river
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/voronoi_centerline.png)
-        - **Equal Distance Centerline**: centerline based on Voronoi centerline but each point is equally spaced out from the previous (in meters) and takes into account the radius of the Earth to convert degrees to meters
+        - **Equal Distance Centerline**: centerline based on Voronoi centerline but each point is equally spaced out from the previous (in meters) and takes into account the radius of the Earth to convert degrees to meters (example below: `equal_distance=10`)
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/equal_distance_centerline.png)
-        - **Evenly Spaced Centerline**: centerline based on Voronoi centerline but evenly spaced with a fixed number of points
+        - **Evenly Spaced Centerline**: centerline based on Voronoi centerline but evenly spaced with a fixed number of points (example: `interpolate_n_centerpoints=200`)
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/evenly_spaced_centerline.png)
         - **Smoothed Centerline**: centerline generated from the evenly spaced centerline but smoothed by a b-spline
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/smoothed_centerline.png)
         
         Centerline coordinates are formed by the Voronoi vertices
         ```
         river_object.centerlineVoronoi
@@ -262,21 +290,21 @@
         ```
         river_object.centerlineSmoothed
         ```
         
         Example:
         ```python
         import centerline_width
-        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=15)
+        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_centerline_coordinates = river_object.centerlineVoronoi
         ```
         Output is a list of tuples: (example) `[(-92.86788596499872, 30.03786596717931), (-92.86789573751797, 30.037834641974108), (-92.8679141386283, 30.037789636848878), (-92.8679251193248, 30.037756853899904), (-92.86796903819089, 30.03765423778148), (-92.86797335733262, 30.037643336049054), (-92.8679920356456, 30.037592224469797), (-92.86800576063828, 30.037555441489403), (-92.86800841510367, 30.037546512833107), (-92.8680119498663, 30.03753043193875)]`
         
         ### Save Centerline Coordinates to a .CSV File
-        Save the centerline coordinates to a csv file with columns for latitude and longitude
+        Save the centerline coordinates to a csv file with columns for latitude and longitude. This is the file format for a table of (latitude,longitude) pairs accepted to import back into Google Earth Pro.
         
         ```
         saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi")
         ```
         * **[REQUIRED]** save_to_csv (string): CSV filename, requires a .csv extension
         * [OPTIONAL] centerline_type (string): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
         * [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type> Centerline Latitude (Deg)`
@@ -315,15 +343,15 @@
         Return the length of the centerline found between the left and right bank generated by the Voronoi diagram
         ```
         river_object.centerlineLength
         ```
         Length returned in kilometers
         ```python
         import centerline_width
-        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=550)
+        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_centerline_length = river_object.centerlineLength
         ```
         The length of the river centerline returns `215.34700589636674` km
         
         ## Plot Centerline in Matplotlib
         Plot the centerline created from a list of right and left banks with Voronoi vertices
         
@@ -417,15 +445,15 @@
         			apply_smoothing=True,
         			remove_intersections=False,
         			save_to_csv=None)
         ```
         * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
         * [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
         * [OPTIONAL] remove_intersections (boolean): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to True
-        * [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (<units specified>)`)
+        * [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (km)`)
         
         Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordinates may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_width_dict = river_object.riverWidthFromCenterline(transect_span_distance=3,
@@ -442,23 +470,26 @@
         
         ### Right and Left bank points are plotted (X-Axis for Latitude, Y-Axis for Longitude)
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example1.png)
         
         ### Generate a polygon to encapsulate the river between the right and left banks to define in and outside of river
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example2.png)
         
-        ### Generate a Voronoi based on the points along the riverbanks
+        ### Generate a Voronoi diagram based on the points along the riverbanks
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example3.png)
         
         ### Display Voronoi ridge vertices that lie within the polygon (within the riverbanks)
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example4.png)
         
-        ### Filter out any point pairs that only have one connection to filter out the short dead end paths and find the starting and ending node based on distance from the top and bottom of polygon
+        ### Filter out any point pairs that only have one connection to filter out the short dead end paths
         With the vertices removed, it is possible to form multiple unconnected graphs within the polygon. The largest subgraph is assumed to contain the centerline and the other subgraphs are filtered out
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example6.png)
+        
+        ### Find the starting and ending node based on distance from the top and bottom of polygon
+        The starting/ending node is defined by the vertice closest to the top/bottom of the polygon along the longest path
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example7.png)
         
         ### Find the shortest path from the starting node to the ending node ([Dijkstra's Algorithm](https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.shortest_paths.generic.shortest_path.html#networkx.algorithms.shortest_paths.generic.shortest_path))
         | Points on Riverbank | NetworkX Graph of Points on Riverbank |
         | ------------- | ------------- |
         | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example10.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/example9.png) |
         
@@ -551,14 +582,23 @@
         
          <p align="center">
           <img src="https://user-images.githubusercontent.com/22159116/222872092-e0b579cc-4f84-4f49-aa53-397785fb9bf2.png" />
           <img src="https://user-images.githubusercontent.com/22159116/222872119-7c485ee2-4ffd-413a-9e4f-b043b122d2bb.png" />
           <img src="https://user-images.githubusercontent.com/22159116/222872019-12931138-9e10-4e51-aa1e-552e72d09af0.png" />
         </p>
         
+        ## Acknowledging Software 
+        Please acknowledge the use of this software in any publications:
+        
+        ```
+        "River centerline/width extraction software was provided by C. Y. Schneck and U. G. Schneck, and is available at URL: https://github.com/cyschneck/centerline-width."
+        ```
+        Please send a copy of such publications to: cyschneck@gmail.com and ugschneck@gmail.com
+        
+        
         This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not necessarily reflect the views of the National Science Foundation.
         
         ## Bug and Feature Request
         
         Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/cyschneck/centerline-width/issues) or to ugschneck@gmail.com/cyschneck@gmail.com
         
 Keywords: geophysics,python,voronoi,networkx,centerline,centerline-extraction,centerline-detection,rivers,river-bank-length,river-bank,limnology,hydrology
```

### Comparing `centerline-width-1.0.0/centerline_width.egg-info/SOURCES.txt` & `centerline-width-1.0.1/centerline_width.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `centerline-width-1.0.0/setup.py` & `centerline-width-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 # Python Package Setup
 from setuptools import setup, find_namespace_packages
 
-VERSION="1.0.0"
+VERSION="1.0.1"
 DESCRIPTION="A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank"
 
 with open("README.md", "r") as f:
 	long_description_readme = f.read()
 
 setup(
 	name="centerline-width",
```

