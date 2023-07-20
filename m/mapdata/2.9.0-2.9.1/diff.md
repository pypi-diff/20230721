# Comparing `tmp/mapdata-2.9.0.tar.gz` & `tmp/mapdata-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapdata-2.9.0.tar", last modified: Wed Jul 12 03:55:14 2023, max compression
+gzip compressed data, was "mapdata-2.9.1.tar", last modified: Wed Jul 12 11:32:03 2023, max compression
```

## Comparing `mapdata-2.9.0.tar` & `mapdata-2.9.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-07-12 03:55:14.317345 mapdata-2.9.0/
--rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-2.9.0/LICENSE.txt
--rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-2.9.0/MANIFEST.in
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     4115 2023-07-12 03:55:14.317345 mapdata-2.9.0/PKG-INFO
--rw-r--r--   0 dreas     (1000) dreas     (1000)     2870 2023-06-28 13:59:57.000000 mapdata-2.9.0/README.md
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-07-12 03:55:14.317345 mapdata-2.9.0/mapdata/
--rwxrwxr-x   0 dreas     (1000) dreas     (1000)   341285 2023-07-12 03:39:29.000000 mapdata-2.9.0/mapdata/mapdata.py
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-07-12 03:55:14.317345 mapdata-2.9.0/mapdata.egg-info/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     4115 2023-07-12 03:55:14.000000 mapdata-2.9.0/mapdata.egg-info/PKG-INFO
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-07-12 03:55:14.000000 mapdata-2.9.0/mapdata.egg-info/SOURCES.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-07-12 03:55:14.000000 mapdata-2.9.0/mapdata.egg-info/dependency_links.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-07-12 03:55:14.000000 mapdata-2.9.0/mapdata.egg-info/top_level.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-07-12 03:55:14.317345 mapdata-2.9.0/setup.cfg
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     1366 2023-07-12 03:40:02.000000 mapdata-2.9.0/setup.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-07-12 11:32:03.382956 mapdata-2.9.1/
+-rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-2.9.1/LICENSE.txt
+-rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-2.9.1/MANIFEST.in
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     4115 2023-07-12 11:32:03.382956 mapdata-2.9.1/PKG-INFO
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     2870 2023-06-28 13:59:57.000000 mapdata-2.9.1/README.md
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-07-12 11:32:03.378956 mapdata-2.9.1/mapdata/
+-rwxrwxr-x   0 dreas     (1000) dreas     (1000)   341240 2023-07-12 11:30:33.000000 mapdata-2.9.1/mapdata/mapdata.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-07-12 11:32:03.378956 mapdata-2.9.1/mapdata.egg-info/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     4115 2023-07-12 11:32:03.000000 mapdata-2.9.1/mapdata.egg-info/PKG-INFO
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-07-12 11:32:03.000000 mapdata-2.9.1/mapdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-07-12 11:32:03.000000 mapdata-2.9.1/mapdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-07-12 11:32:03.000000 mapdata-2.9.1/mapdata.egg-info/top_level.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-07-12 11:32:03.382956 mapdata-2.9.1/setup.cfg
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     1366 2023-07-12 11:30:58.000000 mapdata-2.9.1/setup.py
```

### Comparing `mapdata-2.9.0/LICENSE.txt` & `mapdata-2.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapdata-2.9.0/PKG-INFO` & `mapdata-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 2.9.0
+Version: 2.9.1
 Summary: An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,Spreadsheet,Database,PNG,JPG,Postscript
 Platform: UNKNOWN
```

### Comparing `mapdata-2.9.0/README.md` & `mapdata-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `mapdata-2.9.0/mapdata/mapdata.py` & `mapdata-2.9.1/mapdata/mapdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 # 	The GNU General Public License is available at <http://www.gnu.org/licenses/>
 #
 # AUTHOR
 #	Dreas Nielsen (RDN)
 #
 # ==================================================================
 
-version = "2.9.0"
-vdate = "2023-07-11"
+version = "2.9.1"
+vdate = "2023-07-12"
 
 copyright = "2023"
 
 
 import sys
 import os.path
 import io
@@ -3052,15 +3052,14 @@
 			if plot_type == "Category counts":
 				# Count of values for each X, ordered by X
 				counter = collections.Counter(self.dataset[0])
 				x_vals = list(counter.keys())
 				x_vals.sort()
 				x_counts = [counter[k] for k in x_vals]
 				self.plot_data = [x_vals, x_counts]
-				#self.plot_data_labels = [self.x_var.get(), "Count"]
 				self.plot_data_labels = [self.data_labels[0], "Count"]
 			elif plot_type == "Box plot":
 				# A list of Y values for each X value
 				x_vals = list(set(self.dataset[0]))
 				ds = list(zip(self.dataset[0], self.dataset[1]))
 				plot_data = []
 				for x in x_vals:
@@ -3070,24 +3069,24 @@
 			elif plot_type == "Empirical CDF":
 				# Y is the fraction of data points below each X value
 				x_counts = np.unique(self.dataset[0], return_counts=True)
 				y_vals = list(np.cumsum(x_counts[1]/np.sum(x_counts[1])))
 				self.plot_data = [list(x_counts[0]), y_vals]
 				self.plot_data_labels = [self.data_labels[0], "Cumulative frequency"]
 			elif plot_type == "Normal Q-Q plot":
-				x_vals = list(set(self.dataset[0]))
+				x_vals = copy.copy(self.dataset[0])
 				x_vals.sort()
 				x_mean = statistics.mean(x_vals)
 				x_sd = statistics.stdev(x_vals)
 				x_quantiles = [(x - x_mean)/x_sd for x in x_vals]
 				x_len = len(x_vals)
 				q = [(i + 0.5)/x_len for i in range(x_len)]
 				norm_quantiles = [qnorm(p) for p in q]
 				self.plot_data = [x_vals, x_quantiles, norm_quantiles]
-				self.plot_data_labels = [self.x_var.get(), "Sample quantiles", "Theoretical quantiles"]
+				self.plot_data_labels = [self.data_labels[0], "Sample quantiles", "Theoretical quantiles"]
 			elif plot_type == "Y range plot":
 				# Min and max Y for each X
 				x_vals = list(set(self.dataset[0]))
 				x_vals.sort()
 				y_vals = [[None, None]] * len(x_vals)
 				plotdata = dict(zip(x_vals, y_vals))
 				for i in range(len(self.dataset[0])):
@@ -3097,15 +3096,15 @@
 					if y_vals[0] is None or y < y_vals[0]:
 						plotdata[x][0] = y
 					if y_vals[1] is None or y > y_vals[1]:
 						plotdata[x][1] = y
 				y1 = [plotdata[x][0] for x in x_vals]
 				y2 = [plotdata[x][1] for x in x_vals]
 				self.plot_data = [x_vals, y1, y2]
-				self.plot_data_labels = [self.x_var.get(), self.y_var.get() + " min", self.y_var.get() + " max"]
+				self.plot_data_labels = [self.data_labels[0], self.data_labels[1] + " min", self.data_labels[1] + " max"]
 			elif plot_type == "Line plot":
 				# Sort by X
 				ds = list(zip(self.dataset[0], self.dataset[1]))
 				ds.sort()
 				ds2 = list(zip(*ds))
 				self.plot_data = [list(ds2[0]), list(ds2[1])]
 				self.plot_data_labels = self.data_labels
```

### Comparing `mapdata-2.9.0/mapdata.egg-info/PKG-INFO` & `mapdata-2.9.1/mapdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 2.9.0
+Version: 2.9.1
 Summary: An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,Spreadsheet,Database,PNG,JPG,Postscript
 Platform: UNKNOWN
```

### Comparing `mapdata-2.9.0/setup.py` & `mapdata-2.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 import io
 
 with io.open('README.md', encoding='utf-8') as f:
 	long_description = f.read()
 
 setuptools.setup(name='mapdata',
-	version='2.9.0',
+	version='2.9.1',
 	description="An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database",
 	author='Dreas Nielsen',
 	author_email='dreas.nielsen@gmail.com',
     url='https://osdn.net/project/mapdata/',
 	scripts=['mapdata/mapdata.py'],
     license='GPL',
 	requires=['tkintermapview', 'pyproj', 'odfpy', 'openpyxl', 'xlrd', 'matplotlib'],
```

