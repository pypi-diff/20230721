# Comparing `tmp/sctriangulate-0.9.1.tar.gz` & `tmp/sctriangulate-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sctriangulate-0.9.1.tar", last modified: Sun Oct 10 16:35:53 2021, max compression
+gzip compressed data, was "dist/sctriangulate-0.9.2.tar", last modified: Sun Oct 24 01:43:45 2021, max compression
```

## Comparing `sctriangulate-0.9.1.tar` & `sctriangulate-0.9.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2021-10-10 16:35:53.000000 sctriangulate-0.9.1/
--rw-r--r--   0 ligk2e     (503) staff       (20)     2220 2021-10-10 16:35:53.000000 sctriangulate-0.9.1/PKG-INFO
-drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2021-10-10 16:35:53.000000 sctriangulate-0.9.1/sctriangulate/
--rwx------   0 ligk2e     (503) staff       (20)    22805 2021-07-31 15:47:47.000000 sctriangulate-0.9.1/sctriangulate/metrics.py
--rwx------   0 ligk2e     (503) staff       (20)   522232 2021-05-14 15:17:38.000000 sctriangulate-0.9.1/sctriangulate/artifact_genes.txt
--rwx------   0 ligk2e     (503) staff       (20)     5712 2021-06-04 04:04:31.000000 sctriangulate-0.9.1/sctriangulate/viewer.py
--rwx------   0 ligk2e     (503) staff       (20)      141 2021-09-30 12:49:30.000000 sctriangulate-0.9.1/sctriangulate/__init__.py
--rwx------   0 ligk2e     (503) staff       (20)       27 2021-05-27 20:07:02.000000 sctriangulate-0.9.1/sctriangulate/logger.py
--rwx------   0 ligk2e     (503) staff       (20)   117192 2021-10-10 15:35:42.000000 sctriangulate-0.9.1/sctriangulate/main_class.py
-drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2021-10-10 16:35:53.000000 sctriangulate-0.9.1/sctriangulate/viewer/
--rwx------   0 ligk2e     (503) staff       (20)     1275 2021-05-20 05:05:11.000000 sctriangulate-0.9.1/sctriangulate/viewer/inspection.css
--rwx------   0 ligk2e     (503) staff       (20)     1557 2021-05-27 03:12:05.000000 sctriangulate-0.9.1/sctriangulate/viewer/viewer.js
--rwx------   0 ligk2e     (503) staff       (20)     1857 2021-05-21 16:07:58.000000 sctriangulate-0.9.1/sctriangulate/viewer/viewer.css
--rwx------   0 ligk2e     (503) staff       (20)      580 2021-06-11 02:07:46.000000 sctriangulate-0.9.1/sctriangulate/viewer/inspection.js
--rwx------   0 ligk2e     (503) staff       (20)    43963 2021-10-10 15:24:06.000000 sctriangulate-0.9.1/sctriangulate/preprocessing.py
--rwx------   0 ligk2e     (503) staff       (20)    11291 2021-10-09 01:14:01.000000 sctriangulate-0.9.1/sctriangulate/prune.py
--rwx------   0 ligk2e     (503) staff       (20)     5265 2021-06-12 02:16:32.000000 sctriangulate-0.9.1/sctriangulate/shapley.py
--rwx------   0 ligk2e     (503) staff       (20)    10475 2021-10-06 04:36:32.000000 sctriangulate-0.9.1/sctriangulate/colors.py
-drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2021-10-10 16:35:53.000000 sctriangulate-0.9.1/sctriangulate.egg-info/
--rw-r--r--   0 ligk2e     (503) staff       (20)     2220 2021-10-10 16:35:53.000000 sctriangulate-0.9.1/sctriangulate.egg-info/PKG-INFO
--rw-r--r--   0 ligk2e     (503) staff       (20)      599 2021-10-10 16:35:53.000000 sctriangulate-0.9.1/sctriangulate.egg-info/SOURCES.txt
--rw-r--r--   0 ligk2e     (503) staff       (20)      112 2021-10-10 16:35:53.000000 sctriangulate-0.9.1/sctriangulate.egg-info/requires.txt
--rw-r--r--   0 ligk2e     (503) staff       (20)       14 2021-10-10 16:35:53.000000 sctriangulate-0.9.1/sctriangulate.egg-info/top_level.txt
--rw-r--r--   0 ligk2e     (503) staff       (20)        1 2021-10-10 16:35:53.000000 sctriangulate-0.9.1/sctriangulate.egg-info/dependency_links.txt
--rw-rw-r--   0 ligk2e     (503) staff       (20)     1117 2021-10-05 22:15:06.000000 sctriangulate-0.9.1/README.md
--rw-r--r--   0 ligk2e     (503) staff       (20)     1467 2021-10-10 16:34:20.000000 sctriangulate-0.9.1/setup.py
--rw-r--r--   0 ligk2e     (503) staff       (20)       38 2021-10-10 16:35:53.000000 sctriangulate-0.9.1/setup.cfg
+drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2021-10-24 01:43:45.000000 sctriangulate-0.9.2/
+-rw-r--r--   0 ligk2e     (503) staff       (20)     3659 2021-10-24 01:43:45.000000 sctriangulate-0.9.2/PKG-INFO
+drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2021-10-24 01:43:45.000000 sctriangulate-0.9.2/sctriangulate/
+-rwx------   0 ligk2e     (503) staff       (20)    22805 2021-07-31 15:47:47.000000 sctriangulate-0.9.2/sctriangulate/metrics.py
+-rwx------   0 ligk2e     (503) staff       (20)   522232 2021-05-14 15:17:38.000000 sctriangulate-0.9.2/sctriangulate/artifact_genes.txt
+-rwx------   0 ligk2e     (503) staff       (20)     5712 2021-06-04 04:04:31.000000 sctriangulate-0.9.2/sctriangulate/viewer.py
+-rwx------   0 ligk2e     (503) staff       (20)      141 2021-09-30 12:49:30.000000 sctriangulate-0.9.2/sctriangulate/__init__.py
+-rwx------   0 ligk2e     (503) staff       (20)       27 2021-05-27 20:07:02.000000 sctriangulate-0.9.2/sctriangulate/logger.py
+-rwx------   0 ligk2e     (503) staff       (20)   117192 2021-10-10 15:35:42.000000 sctriangulate-0.9.2/sctriangulate/main_class.py
+drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2021-10-24 01:43:45.000000 sctriangulate-0.9.2/sctriangulate/viewer/
+-rwx------   0 ligk2e     (503) staff       (20)     1275 2021-05-20 05:05:11.000000 sctriangulate-0.9.2/sctriangulate/viewer/inspection.css
+-rwx------   0 ligk2e     (503) staff       (20)     1557 2021-05-27 03:12:05.000000 sctriangulate-0.9.2/sctriangulate/viewer/viewer.js
+-rwx------   0 ligk2e     (503) staff       (20)     1857 2021-05-21 16:07:58.000000 sctriangulate-0.9.2/sctriangulate/viewer/viewer.css
+-rwx------   0 ligk2e     (503) staff       (20)      580 2021-06-11 02:07:46.000000 sctriangulate-0.9.2/sctriangulate/viewer/inspection.js
+-rwx------   0 ligk2e     (503) staff       (20)    43963 2021-10-10 15:24:06.000000 sctriangulate-0.9.2/sctriangulate/preprocessing.py
+-rwx------   0 ligk2e     (503) staff       (20)    11291 2021-10-09 01:14:01.000000 sctriangulate-0.9.2/sctriangulate/prune.py
+-rwx------   0 ligk2e     (503) staff       (20)     5265 2021-06-12 02:16:32.000000 sctriangulate-0.9.2/sctriangulate/shapley.py
+-rwx------   0 ligk2e     (503) staff       (20)    13043 2021-10-24 01:41:22.000000 sctriangulate-0.9.2/sctriangulate/colors.py
+drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2021-10-24 01:43:45.000000 sctriangulate-0.9.2/sctriangulate.egg-info/
+-rw-r--r--   0 ligk2e     (503) staff       (20)     3659 2021-10-24 01:43:45.000000 sctriangulate-0.9.2/sctriangulate.egg-info/PKG-INFO
+-rw-r--r--   0 ligk2e     (503) staff       (20)      599 2021-10-24 01:43:45.000000 sctriangulate-0.9.2/sctriangulate.egg-info/SOURCES.txt
+-rw-r--r--   0 ligk2e     (503) staff       (20)      112 2021-10-24 01:43:45.000000 sctriangulate-0.9.2/sctriangulate.egg-info/requires.txt
+-rw-r--r--   0 ligk2e     (503) staff       (20)       14 2021-10-24 01:43:45.000000 sctriangulate-0.9.2/sctriangulate.egg-info/top_level.txt
+-rw-r--r--   0 ligk2e     (503) staff       (20)        1 2021-10-24 01:43:45.000000 sctriangulate-0.9.2/sctriangulate.egg-info/dependency_links.txt
+-rw-rw-r--   0 ligk2e     (503) staff       (20)     2500 2021-10-17 00:16:32.000000 sctriangulate-0.9.2/README.md
+-rw-r--r--   0 ligk2e     (503) staff       (20)     1467 2021-10-24 01:42:56.000000 sctriangulate-0.9.2/setup.py
+-rw-r--r--   0 ligk2e     (503) staff       (20)       38 2021-10-24 01:43:45.000000 sctriangulate-0.9.2/setup.cfg
```

### Comparing `sctriangulate-0.9.1/sctriangulate/metrics.py` & `sctriangulate-0.9.2/sctriangulate/metrics.py`

 * *Files identical despite different names*

### Comparing `sctriangulate-0.9.1/sctriangulate/artifact_genes.txt` & `sctriangulate-0.9.2/sctriangulate/artifact_genes.txt`

 * *Files identical despite different names*

### Comparing `sctriangulate-0.9.1/sctriangulate/viewer.py` & `sctriangulate-0.9.2/sctriangulate/viewer.py`

 * *Files identical despite different names*

### Comparing `sctriangulate-0.9.1/sctriangulate/main_class.py` & `sctriangulate-0.9.2/sctriangulate/main_class.py`

 * *Files identical despite different names*

### Comparing `sctriangulate-0.9.1/sctriangulate/viewer/inspection.css` & `sctriangulate-0.9.2/sctriangulate/viewer/inspection.css`

 * *Files identical despite different names*

### Comparing `sctriangulate-0.9.1/sctriangulate/viewer/viewer.js` & `sctriangulate-0.9.2/sctriangulate/viewer/viewer.js`

 * *Files identical despite different names*

### Comparing `sctriangulate-0.9.1/sctriangulate/viewer/viewer.css` & `sctriangulate-0.9.2/sctriangulate/viewer/viewer.css`

 * *Files identical despite different names*

### Comparing `sctriangulate-0.9.1/sctriangulate/viewer/inspection.js` & `sctriangulate-0.9.2/sctriangulate/viewer/inspection.js`

 * *Files identical despite different names*

### Comparing `sctriangulate-0.9.1/sctriangulate/preprocessing.py` & `sctriangulate-0.9.2/sctriangulate/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sctriangulate-0.9.1/sctriangulate/prune.py` & `sctriangulate-0.9.2/sctriangulate/prune.py`

 * *Files identical despite different names*

### Comparing `sctriangulate-0.9.1/sctriangulate/shapley.py` & `sctriangulate-0.9.2/sctriangulate/shapley.py`

 * *Files identical despite different names*

### Comparing `sctriangulate-0.9.1/sctriangulate/colors.py` & `sctriangulate-0.9.2/sctriangulate/colors.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from matplotlib import cm
 import pandas as pd
 import numpy as np
 from matplotlib.colors import LinearSegmentedColormap, to_hex, to_rgb
+from matplotlib import colors
 import copy
 import matplotlib.pyplot as plt
 import matplotlib as mpl
 
 mpl.rcParams['pdf.fonttype'] = 42
 mpl.rcParams['ps.fonttype'] = 42
 mpl.rcParams['font.family'] = 'Arial'
@@ -95,14 +96,18 @@
     for i in range(hex2.shape[0]):
         for j in range(hex2.shape[1]):
             hex_ = hex2[i][j]
             rgb_ = to_rgb(hex_)
             rgb3[i,j,:] = rgb_ 
     return rgb3
 
+# 256 to [0,1]
+def inter_from_256(x):
+    return np.interp(x=x,xp=[0,255],fp=[0,1])
+
 # choose colors
 def retrieve_pretty_colors(name):
     '''
     retrieve pretty customized colors (discrete)
 
     :param name: string, valid value 'icgs2', 'shap'
 
@@ -211,14 +216,78 @@
 
     '''
     length = len(setlist)
     _colors = pick_n_colors(n=length)
     cmap = pd.Series(index=setlist,data=_colors).to_dict()
     return cmap
 
+
+def build_custom_continuous_cmap(*rgb_list):
+    '''
+    Generating any custom continuous colormap, user should supply a list of (R,G,B) color taking the value from [0,255], because this is
+    the format the adobe color will output for you. 
+
+    Examples::
+
+        test_cmap = build_custom_continuous_cmap([64,57,144],[112,198,162],[230,241,146],[253,219,127],[244,109,69],[169,23,69])
+        fig,ax = plt.subplots()
+        fig.colorbar(cm.ScalarMappable(norm=colors.Normalize(),cmap=diverge_cmap),ax=ax)
+
+    .. image:: ./_static/custom_continuous_cmap.png
+        :height: 400px
+        :width: 550px
+        :align: center
+        :target: target     
+
+    '''
+    all_red = []
+    all_green = []
+    all_blue = []
+    for rgb in rgb_list:
+        all_red.append(rgb[0])
+        all_green.append(rgb[1])
+        all_blue.append(rgb[2])
+    # build each section
+    n_section = len(all_red) - 1
+    red = tuple([(1/n_section*i,inter_from_256(v),inter_from_256(v)) for i,v in enumerate(all_red)])
+    green = tuple([(1/n_section*i,inter_from_256(v),inter_from_256(v)) for i,v in enumerate(all_green)])
+    blue = tuple([(1/n_section*i,inter_from_256(v),inter_from_256(v)) for i,v in enumerate(all_blue)])
+    cdict = {'red':red,'green':green,'blue':blue}
+    new_cmap = colors.LinearSegmentedColormap('new_cmap',segmentdata=cdict)
+    return new_cmap
+
+def build_custom_divergent_cmap(hex_left,hex_right):
+    '''
+    User supplies two arbitrary hex code for the vmin and vmax color values, then it will build a divergent cmap centers at pure white.
+
+    Examples::
+
+        diverge_cmap = build_custom_divergent_cmap('#21EBDB','#F0AA5F')
+        fig,ax = plt.subplots()
+        fig.colorbar(cm.ScalarMappable(norm=colors.Normalize(),cmap=diverge_cmap),ax=ax)
+
+    .. image:: ./_static/custom_divergent_cmap.png
+        :height: 400px
+        :width: 550px
+        :align: center
+        :target: target        
+
+    '''
+    left_rgb = colors.to_rgb(hex_left)
+    right_rgb = colors.to_rgb(hex_right)
+    # build each section
+    n_section = 2
+    red = ((0,left_rgb[0],left_rgb[0]),(0.5,1,1),(1,right_rgb[0],right_rgb[0]))
+    green = ((0,left_rgb[1],left_rgb[1]), (0.5, 1, 1), (1, right_rgb[1], right_rgb[1]))
+    blue = ((0,left_rgb[2],left_rgb[2]), (0.5, 1, 1), (1, right_rgb[2], right_rgb[2]))
+    cdict = {'red':red,'green':green,'blue':blue}
+    new_cmap = colors.LinearSegmentedColormap('new_cmap',segmentdata=cdict)
+    return new_cmap
+
+
 # zeileis_28 was taken from scanpy: https://github.com/theislab/scanpy/blob/master/scanpy/plotting/palettes.py
 # and they noted the original source as below:
 # https://graphicdesign.stackexchange.com/questions/3682/where-can-i-find-a-large-palette-set-of-contrasting-colors-for-coloring-many-d
 # update 1
 # orig reference http://epub.wu.ac.at/1692/1/document.pdf
```

### Comparing `sctriangulate-0.9.1/sctriangulate.egg-info/SOURCES.txt` & `sctriangulate-0.9.2/sctriangulate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sctriangulate-0.9.1/setup.py` & `sctriangulate-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     'numpy ==1.19.5',
     'pandas ==1.1.5',
     'leidenalg',
 ]
 
 setup(
       name = 'sctriangulate',
-      version = '0.9.1',
+      version = '0.9.2',
       description= 'A Python package to mix-and-match conflicting clustering results in single cell analysis, and generate reconciled clustering solutions.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Guangyuan(Frank) Li',
       author_email='li2g2@mail.uc.edu',
       maintainer='Guangyuan(Frank) Li',
       maintainer_email='li2g2@mail.uc.edu',
```

