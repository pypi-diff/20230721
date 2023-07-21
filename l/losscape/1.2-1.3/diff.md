# Comparing `tmp/losscape-1.2.tar.gz` & `tmp/losscape-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "losscape-1.2.tar", last modified: Fri Jul 21 07:21:56 2023, max compression
+gzip compressed data, was "losscape-1.3.tar", last modified: Fri Jul 21 07:28:30 2023, max compression
```

## Comparing `losscape-1.2.tar` & `losscape-1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 07:21:56.211571 losscape-1.2/
--rw-rw-r--   0 alex      (1000) alex      (1000)      230 2023-07-21 07:21:56.211571 losscape-1.2/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3020 2023-07-18 21:38:11.000000 losscape-1.2/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 07:21:56.211571 losscape-1.2/losscape/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-18 12:39:49.000000 losscape-1.2/losscape/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1380 2023-07-18 10:08:58.000000 losscape-1.2/losscape/compute_loss.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1816 2023-07-18 09:41:21.000000 losscape-1.2/losscape/create_directions.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    15690 2023-07-21 07:21:10.000000 losscape-1.2/losscape/create_landscape.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2099 2023-07-21 07:07:54.000000 losscape-1.2/losscape/train.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 07:21:56.211571 losscape-1.2/losscape.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)      230 2023-07-21 07:21:56.000000 losscape-1.2/losscape.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      300 2023-07-21 07:21:56.000000 losscape-1.2/losscape.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-21 07:21:56.000000 losscape-1.2/losscape.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       36 2023-07-21 07:21:56.000000 losscape-1.2/losscape.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-21 07:21:56.000000 losscape-1.2/losscape.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-21 07:21:56.211571 losscape-1.2/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)      399 2023-07-21 07:21:29.000000 losscape-1.2/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 07:28:30.832615 losscape-1.3/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      230 2023-07-21 07:28:30.832615 losscape-1.3/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3020 2023-07-18 21:38:11.000000 losscape-1.3/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 07:28:30.832615 losscape-1.3/losscape/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-18 12:39:49.000000 losscape-1.3/losscape/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1380 2023-07-18 10:08:58.000000 losscape-1.3/losscape/compute_loss.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1816 2023-07-18 09:41:21.000000 losscape-1.3/losscape/create_directions.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15961 2023-07-21 07:27:43.000000 losscape-1.3/losscape/create_landscape.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2099 2023-07-21 07:07:54.000000 losscape-1.3/losscape/train.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 07:28:30.832615 losscape-1.3/losscape.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      230 2023-07-21 07:28:30.000000 losscape-1.3/losscape.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      300 2023-07-21 07:28:30.000000 losscape-1.3/losscape.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-21 07:28:30.000000 losscape-1.3/losscape.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       36 2023-07-21 07:28:30.000000 losscape-1.3/losscape.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-21 07:28:30.000000 losscape-1.3/losscape.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-21 07:28:30.832615 losscape-1.3/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)      399 2023-07-21 07:28:15.000000 losscape-1.3/setup.py
```

### Comparing `losscape-1.2/README.md` & `losscape-1.3/README.md`

 * *Files identical despite different names*

### Comparing `losscape-1.2/losscape/compute_loss.py` & `losscape-1.3/losscape/compute_loss.py`

 * *Files identical despite different names*

### Comparing `losscape-1.2/losscape/create_directions.py` & `losscape-1.3/losscape/create_directions.py`

 * *Files identical despite different names*

### Comparing `losscape-1.2/losscape/create_landscape.py` & `losscape-1.3/losscape/create_landscape.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import torch
 
 import math
 import numpy as np
 from scipy import interpolate
 import matplotlib.pyplot as plt
+import h5py
 
 from losscape.compute_loss import compute_loss
 from losscape.create_directions import create_random_direction, create_random_directions
 
 #todo : plot anim la traj d'une optim avec PCA
 #todo : losscape avec le test loss
 #todo pour la lib : possiblité de tout foutre dans un fichier, et il fait les exps automatiquement ? (genre on met model + dataloader + optim + loss et il loop sur les models + optims)
@@ -127,14 +128,20 @@
         plt.show()
     
     plt.clf()
 
     if output_vtp:
         _create_vtp(X, Y, losses, log=log_vtp)
 
+    if output_h5:
+        with h5py.File('data.h5', 'w') as hf:
+            hf.create_dataset("X", data=X)
+            hf.create_dataset("Y", data=Y)
+            hf.create_dataset("losses", data=losses)
+
     return X, Y, losses
 
 def _set_weights(model, weights, directions, step):
     if len(directions) == 2:
         dx = directions[0]
         dy = directions[1]
         changes = [d0*step[0] + d1*step[1] for (d0, d1) in zip(dx, dy)]
@@ -145,14 +152,15 @@
     for (p, w, d) in zip(model.parameters(), weights, changes):
         p.data = w + d
 
 def _reset_weights(model, weights):
     for (p, w) in zip(model.parameters(), weights):
         p.data.copy_(w.type(type(p.data)))
 
+# as in https://github.com/tomgoldstein/loss-landscape
 def _create_vtp(X, Y, losses, log=False, zmax=-1, interp=-1):
     #set this to True to generate points
     show_points = False
     #set this to True to generate polygons
     show_polys = True
 
     xcoordinates = X
```

### Comparing `losscape-1.2/losscape/train.py` & `losscape-1.3/losscape/train.py`

 * *Files identical despite different names*

