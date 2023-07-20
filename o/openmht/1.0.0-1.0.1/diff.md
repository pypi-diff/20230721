# Comparing `tmp/openmht-1.0.0.tar.gz` & `tmp/openmht-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\openmht-1.0.0.tar", last modified: Tue Jun  6 00:47:58 2023, max compression
+gzip compressed data, was "dist\openmht-1.0.1.tar", last modified: Thu Jul 20 22:55:16 2023, max compression
```

## Comparing `openmht-1.0.0.tar` & `openmht-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 00:47:58.000000 openmht-1.0.0/
--rw-rw-rw-   0        0        0      569 2023-06-06 00:47:58.000000 openmht-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2126 2023-06-06 00:37:53.000000 openmht-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 00:47:58.000000 openmht-1.0.0/openmht/
--rw-rw-rw-   0        0        0        0 2020-02-08 03:31:14.000000 openmht-1.0.0/openmht/__init__.py
--rw-rw-rw-   0        0        0      117 2023-06-06 00:37:53.000000 openmht-1.0.0/openmht/__main__.py
--rw-rw-rw-   0        0        0     5209 2023-06-06 00:39:25.000000 openmht-1.0.0/openmht/cli.py
--rw-rw-rw-   0        0        0     3675 2020-02-08 06:06:47.000000 openmht-1.0.0/openmht/graph.py
--rw-rw-rw-   0        0        0     2476 2023-06-06 00:37:53.000000 openmht-1.0.0/openmht/kalman_filter.py
--rw-rw-rw-   0        0        0     5396 2023-06-06 00:37:53.000000 openmht-1.0.0/openmht/mht.py
--rw-rw-rw-   0        0        0     3328 2023-06-06 00:40:47.000000 openmht-1.0.0/openmht/weighted_graph.py
-drwxrwxrwx   0        0        0        0 2023-06-06 00:47:58.000000 openmht-1.0.0/openmht.egg-info/
--rw-rw-rw-   0        0        0      569 2023-06-06 00:47:58.000000 openmht-1.0.0/openmht.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-06-06 00:47:58.000000 openmht-1.0.0/openmht.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 00:47:58.000000 openmht-1.0.0/openmht.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-06 00:47:58.000000 openmht-1.0.0/openmht.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-06-06 00:47:58.000000 openmht-1.0.0/openmht.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 00:47:58.000000 openmht-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      868 2023-06-06 00:45:54.000000 openmht-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 22:55:16.000000 openmht-1.0.1/
+-rw-rw-rw-   0        0        0      569 2023-07-20 22:55:16.000000 openmht-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2126 2023-06-06 00:37:53.000000 openmht-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 22:55:16.000000 openmht-1.0.1/openmht/
+-rw-rw-rw-   0        0        0        0 2020-02-08 03:31:14.000000 openmht-1.0.1/openmht/__init__.py
+-rw-rw-rw-   0        0        0      117 2023-07-20 22:15:04.000000 openmht-1.0.1/openmht/__main__.py
+-rw-rw-rw-   0        0        0     5122 2023-07-20 22:41:09.000000 openmht-1.0.1/openmht/cli.py
+-rw-rw-rw-   0        0        0     3675 2020-02-08 06:06:47.000000 openmht-1.0.1/openmht/graph.py
+-rw-rw-rw-   0        0        0     2476 2023-06-06 00:37:53.000000 openmht-1.0.1/openmht/kalman_filter.py
+-rw-rw-rw-   0        0        0     5396 2023-06-06 00:37:53.000000 openmht-1.0.1/openmht/mht.py
+-rw-rw-rw-   0        0        0     3857 2023-07-20 22:41:09.000000 openmht-1.0.1/openmht/weighted_graph.py
+drwxrwxrwx   0        0        0        0 2023-07-20 22:55:16.000000 openmht-1.0.1/openmht.egg-info/
+-rw-rw-rw-   0        0        0      569 2023-07-20 22:55:16.000000 openmht-1.0.1/openmht.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-07-20 22:55:16.000000 openmht-1.0.1/openmht.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 22:55:16.000000 openmht-1.0.1/openmht.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-20 22:55:16.000000 openmht-1.0.1/openmht.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-07-20 22:55:16.000000 openmht-1.0.1/openmht.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 22:55:16.000000 openmht-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      868 2023-07-20 22:46:37.000000 openmht-1.0.1/setup.py
```

### Comparing `openmht-1.0.0/PKG-INFO` & `openmht-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmht
-Version: 1.0.0
+Version: 1.0.1
 Summary: OpenMHT
 Home-page: https://github.com/jonperdomo/openmht
 Author: Jonathan Elliot Perdomo
 Author-email: jonperdomodb@gmail.com
 License: UNKNOWN
 Description: An implementation of the multiple hypothesis tracking algorithm for data association.
 Platform: UNKNOWN
```

### Comparing `openmht-1.0.0/README.md` & `openmht-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `openmht-1.0.0/openmht/cli.py` & `openmht-1.0.1/openmht/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python
 """CLI"""
 
-
 from .mht import MHT
+from pathlib import Path
 
-import os
 import sys
 import argparse
 import time
 import csv
 
 import logging
 logging.basicConfig(level=logging.INFO,
@@ -119,19 +118,19 @@
     # Parse arguments
     input_file = args.ifile
     output_file = args.ofile
     param_file = args.pfile
 
     # Verify CSV file formats
     try:
-        assert os.path.isfile(input_file), "Input file does not exist: {}".format(input_file)
-        assert os.path.isfile(param_file), "Parameter file does not exist: {}".format(param_file)
-        assert os.path.splitext(input_file)[-1].lower() == '.csv', "Input file is not CSV: {}".format(input_file)
-        assert os.path.splitext(output_file)[-1].lower() == '.csv', "Output file is not CSV: {}".format(output_file)
-        assert os.path.splitext(param_file)[-1].lower() == '.txt', "Parameter file is not TXT: {}".format(param_file)
+        assert Path(input_file).is_file(), f"Input file does not exist: {input_file}"
+        assert Path(param_file).is_file(), f"Parameter file does not exist: {param_file}"
+        assert Path(input_file).suffix == '.csv', f"Input file is not CSV: {input_file}"
+        assert Path(output_file).suffix == '.csv', f"Output file is not CSV: {output_file}"
+        assert Path(param_file).suffix == '.txt', f"Parameter file is not TXT: {param_file}"
 
     except AssertionError as e:
         print(e)
         sys.exit(2)
 
     logging.info(f"Input file is: {input_file}")
     logging.info(f"Output file is: {output_file}")
@@ -150,8 +149,8 @@
     detections = read_uv_csv(input_file)
     start = time.time()
     mht = MHT(detections, params)
     solution_coordinates = mht.run()
     write_uv_csv(output_file, solution_coordinates)
     end = time.time()
     elapsed_seconds = end - start
-    logging.info("Elapsed time (seconds): {0:.3f}".format(elapsed_seconds))
+    logging.info(f"Elapsed time (seconds): {elapsed_seconds:.3f}")
```

### Comparing `openmht-1.0.0/openmht/graph.py` & `openmht-1.0.1/openmht/graph.py`

 * *Files identical despite different names*

### Comparing `openmht-1.0.0/openmht/kalman_filter.py` & `openmht-1.0.1/openmht/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `openmht-1.0.0/openmht/mht.py` & `openmht-1.0.1/openmht/mht.py`

 * *Files identical despite different names*

### Comparing `openmht-1.0.0/openmht/weighted_graph.py` & `openmht-1.0.1/openmht/weighted_graph.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,100 +1,112 @@
 #!/usr/bin/env python
 """Weighted Graph"""
 
 import operator
-import random
+import numpy as np
 
 from .graph import Graph
 
 __author__ = "Jon Perdomo"
 __license__ = "GPL-3.0"
 __version__ = "0.1.0"
 
 
 class WeightedGraph(Graph):
-    """
-    A graph with weighted vertices.
-    """
+    """A graph with weighted vertices."""
+
     def __init__(self, graph_dict=None):
         Graph.__init__(self, graph_dict)
         self.__weights = {}
 
     def mwis(self):
         """Determine the maximum weighted independent set."""
 
         # Find all maximal independent sets
         complement = self.complement()
         ind_sets = []
         self.____bron_kerbosch3(complement, ind_sets)
 
         # Find the maximum weighted set
-        # NOTE: The maximum total weight of any subset of nodes in this graph cannot be less than the additive
-        # inverse of the total magnitude of all node weights, subtract 1. Use this value as the initial maximum weight.
+        # NOTE: The maximum total weight of any subset of nodes in this graph
+        # cannot be less than the additive inverse of the total magnitude of all
+        # node weights, subtract 1. Use this value as the initial maximum
+        # weight.
         max_weight = -sum(map(abs, self.__weights.values()))-1
         mwis = []
         for ind_set in ind_sets:
             set_weight = sum([self.__weights[str(i)] for i in ind_set])
             if set_weight > max_weight:
                 max_weight = set_weight
                 mwis = ind_set
 
         return mwis
 
-    def ____bron_kerbosch3(self, g, results):
+    def ____bron_kerbosch3(self, g: np.ndarray, results: list):
         """With vertex ordering."""
         P = set(range(len(self.vertices())))
         R, X = set(), set()
         deg_ord = self.__degeneracy_ordering(g)
 
         for v in deg_ord:
             N_v = self.__n(v, g)
             self.____bron_kerbosch2(R | {v}, P & N_v, X & N_v, g, results)
 
             P = P - {v}
             X = X | {v}
 
-    def ____bron_kerbosch2(self, R, P, X, g, results):
+    def ____bron_kerbosch2(self, R: set, P: set, X: set, g: np.ndarray,
+                           results: list):
         """With pivoting."""
         if not any((P, X)):
             results.append(R)
             return
 
-        u = random.choice(tuple(P | X))
-        for v in P - self.__n(u, g):
+        # Choose pivot point u that maximizes size of N(u). This is chosen to
+        # minimize the size of P - N(u), thus minimizing recursion branches.
+        u_max = -1
+        size_max = 0
+        for u in P | X:
+            size_N = len(self.__n(u, g))
+            if size_N > size_max:
+                u_max = u
+                size_max = size_N
+
+        for v in P - self.__n(u_max, g):
             N_v = self.__n(v, g)
-            self.__bron_kerbosch(R | {v}, P & N_v, X & N_v, g, results)
+            self.____bron_kerbosch2(R | {v}, P & N_v, X & N_v, g, results)
 
             P = P - {v}
             X = X | {v}
 
-    def __bron_kerbosch(self, R, P, X, g, results):
+    def __bron_kerbosch(self, R: set, P: set, X: set, g: np.ndarray,
+                        results: list):
         """Without pivoting."""
         if not any((P, X)):
             results.append(R)
 
         for v in set(P):
             N_v = self.__n(v, g)
             self.__bron_kerbosch(R | {v}, P & N_v, X & N_v, g, results)
 
             P = P - {v}
             X = X | {v}
 
-    def __degeneracy_ordering(self, g):
+    def __degeneracy_ordering(self, g: np.ndarray) -> list:
         """Order such that each vertex has d or fewer neighbors that come later in the ordering."""
         v_ordered = []
         degrees = list(enumerate(self.vertex_degrees(g)))
         while degrees:
             min_index, min_value = min(degrees, key=operator.itemgetter(1))
             v_ordered.append(min_index)
             degrees.remove((min_index, min_value))
 
         return v_ordered
 
-    def __n(self, v, g):
+    def __n(self, v: int, g: np.ndarray) -> set:
         return set([i for i, n_v in enumerate(g[v]) if n_v])
 
     def add_weighted_vertex(self, vertex, weight):
         """
         Add a weighted vertex to the graph.
         """
         self.add_vertex(vertex)
```

### Comparing `openmht-1.0.0/openmht.egg-info/PKG-INFO` & `openmht-1.0.1/openmht.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmht
-Version: 1.0.0
+Version: 1.0.1
 Summary: OpenMHT
 Home-page: https://github.com/jonperdomo/openmht
 Author: Jonathan Elliot Perdomo
 Author-email: jonperdomodb@gmail.com
 License: UNKNOWN
 Description: An implementation of the multiple hypothesis tracking algorithm for data association.
 Platform: UNKNOWN
```

### Comparing `openmht-1.0.0/setup.py` & `openmht-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="openmht",
-    version="1.0.0",
+    version="1.0.1",
     author="Jonathan Elliot Perdomo",
     author_email="jonperdomodb@gmail.com",
     description="OpenMHT",
     long_description="An implementation of the multiple hypothesis tracking algorithm for data association.",
     long_description_content_type="text/markdown",
     url="https://github.com/jonperdomo/openmht",
     packages=setuptools.find_packages(),
```

