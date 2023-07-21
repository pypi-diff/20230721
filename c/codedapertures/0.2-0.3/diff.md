# Comparing `tmp/codedapertures-0.2.tar.gz` & `tmp/codedapertures-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedapertures-0.2.tar", last modified: Thu Jul 20 03:46:32 2023, max compression
+gzip compressed data, was "codedapertures-0.3.tar", last modified: Fri Jul 21 01:51:54 2023, max compression
```

## Comparing `codedapertures-0.2.tar` & `codedapertures-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-20 03:46:32.311574 codedapertures-0.2/
--rw-r--r--   0 bbudden    (501) staff       (20)     1062 2023-01-26 02:12:38.000000 codedapertures-0.2/LICENSE
--rw-r--r--   0 bbudden    (501) staff       (20)      697 2023-07-20 03:46:32.311473 codedapertures-0.2/PKG-INFO
--rw-r--r--   0 bbudden    (501) staff       (20)     1355 2023-07-06 00:57:20.000000 codedapertures-0.2/README.md
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-20 03:46:32.310525 codedapertures-0.2/codedapertures/
--rw-r--r--   0 bbudden    (501) staff       (20)       30 2023-01-26 02:12:38.000000 codedapertures-0.2/codedapertures/__init__.py
--rw-r--r--   0 bbudden    (501) staff       (20)    10021 2023-07-20 03:43:02.000000 codedapertures-0.2/codedapertures/codedapertures.py
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-20 03:46:32.311344 codedapertures-0.2/codedapertures.egg-info/
--rw-r--r--   0 bbudden    (501) staff       (20)      697 2023-07-20 03:46:32.000000 codedapertures-0.2/codedapertures.egg-info/PKG-INFO
--rw-r--r--   0 bbudden    (501) staff       (20)      312 2023-07-20 03:46:32.000000 codedapertures-0.2/codedapertures.egg-info/SOURCES.txt
--rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-20 03:46:32.000000 codedapertures-0.2/codedapertures.egg-info/dependency_links.txt
--rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-06 00:30:22.000000 codedapertures-0.2/codedapertures.egg-info/not-zip-safe
--rw-r--r--   0 bbudden    (501) staff       (20)       26 2023-07-20 03:46:32.000000 codedapertures-0.2/codedapertures.egg-info/requires.txt
--rw-r--r--   0 bbudden    (501) staff       (20)       15 2023-07-20 03:46:32.000000 codedapertures-0.2/codedapertures.egg-info/top_level.txt
--rw-r--r--   0 bbudden    (501) staff       (20)       38 2023-07-20 03:46:32.311602 codedapertures-0.2/setup.cfg
--rw-r--r--   0 bbudden    (501) staff       (20)      868 2023-07-20 03:44:16.000000 codedapertures-0.2/setup.py
+drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-21 01:51:54.842318 codedapertures-0.3/
+-rw-r--r--   0 bbudden    (501) staff       (20)     1062 2023-01-26 02:12:38.000000 codedapertures-0.3/LICENSE
+-rw-r--r--   0 bbudden    (501) staff       (20)      697 2023-07-21 01:51:54.842213 codedapertures-0.3/PKG-INFO
+-rw-r--r--   0 bbudden    (501) staff       (20)     1530 2023-07-20 04:15:05.000000 codedapertures-0.3/README.md
+drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-21 01:51:54.841362 codedapertures-0.3/codedapertures/
+-rw-r--r--   0 bbudden    (501) staff       (20)       30 2023-01-26 02:12:38.000000 codedapertures-0.3/codedapertures/__init__.py
+-rw-r--r--   0 bbudden    (501) staff       (20)    13570 2023-07-21 01:46:46.000000 codedapertures-0.3/codedapertures/codedapertures.py
+drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-21 01:51:54.842062 codedapertures-0.3/codedapertures.egg-info/
+-rw-r--r--   0 bbudden    (501) staff       (20)      697 2023-07-21 01:51:54.000000 codedapertures-0.3/codedapertures.egg-info/PKG-INFO
+-rw-r--r--   0 bbudden    (501) staff       (20)      312 2023-07-21 01:51:54.000000 codedapertures-0.3/codedapertures.egg-info/SOURCES.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-21 01:51:54.000000 codedapertures-0.3/codedapertures.egg-info/dependency_links.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-06 00:30:22.000000 codedapertures-0.3/codedapertures.egg-info/not-zip-safe
+-rw-r--r--   0 bbudden    (501) staff       (20)       26 2023-07-21 01:51:54.000000 codedapertures-0.3/codedapertures.egg-info/requires.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)       15 2023-07-21 01:51:54.000000 codedapertures-0.3/codedapertures.egg-info/top_level.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)       38 2023-07-21 01:51:54.842347 codedapertures-0.3/setup.cfg
+-rw-r--r--   0 bbudden    (501) staff       (20)      868 2023-07-21 01:51:45.000000 codedapertures-0.3/setup.py
```

### Comparing `codedapertures-0.2/LICENSE` & `codedapertures-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `codedapertures-0.2/PKG-INFO` & `codedapertures-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedapertures
-Version: 0.2
+Version: 0.3
 Summary: Coded Aperture Production in PYthon (CAPPY)
 Home-page: https://github.com/bpops/cappy
 Author: bpops
 License: MIT
 License-File: LICENSE
 
 CAPPY is a python module that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.
```

### Comparing `codedapertures-0.2/README.md` & `codedapertures-0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -19,8 +19,10 @@
 See [demo.ipynb](https://github.com/bpops/cappy/blob/master/demo.ipynb) for examples of use.
 
 
 ### Credits
 
 URA pattern: E. E. Fenimore and T. M. Cannon, "Coded aperture imaging with uniformly redundant arrays," Appl. Opt. 17, 337-347 (1978).
 
-MURA pattern:  E.E. Fenimore and S. R. Gottesman, "New family of binary arrays for coded aperture imaging" Appl. Opt. 28 (20): 4344-4352 (1989).
+MURA pattern:  E.E. Fenimore and S. R. Gottesman, "New family of binary arrays for coded aperture imaging" Appl. Opt. 28 (20): 4344-4352 (1989).
+
+SHURA and HURA pattern: M.H. Finger and T.A. Prince, "Hexagonal Uniformly Redundant Arrays for Coded-Aperture Imaging," Proc. 19th Int. Cosmic Ray Conf., 3: 295-298 (1985).
```

### Comparing `codedapertures-0.2/codedapertures/codedapertures.py` & `codedapertures-0.3/codedapertures/codedapertures.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 #                                                                                 
 #                Coded Aperture Production in PYthon                                                                              
 #
 #                           MIT license
 #                  https://github.com/bpops/cappy
 #
 
-import numpy             as np
-import matplotlib.pyplot as plt
+import numpy              as     np
+import matplotlib.pyplot  as     plt
+from   matplotlib.patches import RegularPolygon
 import pyprimes
 import random
 
 
 class mask():
     """
     Mask
@@ -336,15 +337,14 @@
                 A_ij[i,j] = A_IJ[i%r,j%s]
         self.A_ij = A_ij
 
         # get width/height
         self.width = self.A_ij.shape[0]
         self.height = self.A_ij.shape[1]
 
-
         if not quiet: self.report()
         
     def report(self):
         """
         Report on the mask information
         """
         print("Modified Uniformly Redundant Array")
@@ -367,8 +367,126 @@
         while True:
             L = 4*m + 1
             if pyprimes.isprime(L):
                 this_rank += 1
             if this_rank == rank:
                 break
             m += 1
-        return L
+        return L
+    
+class shura(mask):
+    """
+    Skew-Hadamard Uniformly Redundant Array
+
+    Parameters
+    ----------
+    n : int
+        determines the order, v, where v=4n-1 (default 6)
+    r : int
+        feeds into pattern (default 5)
+    mult : int
+        multiplier (default 10)
+    quiet : bool
+        if True, will print information about the array upon creation
+    """
+
+    def __init__(self, n=6, r=5, mult=4, quiet=False):
+        self.n    = n
+        self.r    = r
+        self.mult = mult
+        
+        # calculate intermediates
+        self.v   = 4*n-1
+        self.k   = 2*n-1
+        self.lam = n-1
+
+        # construct cyclic difference set D
+        self.D = np.zeros((int((self.v-1)/2)), dtype=np.int32)
+        for i in range(len(self.D)):
+            self.D[i] = ((i+1)**2) % self.v
+
+        # determine labels
+        rx = r*mult
+        self.l = np.zeros((rx,rx))
+        for i in range(rx):
+            for j in range(rx):
+                self.l[i,j] = (i + r*j) % self.v
+
+        # calculate mask
+        self.mask = np.zeros(self.l.shape)
+        for i in range(self.mask.shape[0]):
+            for j in range(self.mask.shape[1]):
+                if self.l[i,j] in self.D:
+                    self.mask[i,j] = 1
+
+        if not quiet: self.report()
+
+    def report(self):
+        """
+        Report the array info
+        """
+        print("Skew-Hadamard Uniformly Redundant Array")
+        print(f"n: {self.n}")
+        print(f"order (v): {self.v}")
+        print(f"k: {self.k}")
+        print(f"lambda: {self.lam}")
+        print(f"r: {self.r}")
+        print(f"multiplier: {self.mult}")
+
+    def show(self):
+        """
+        Plot the mask
+        """
+
+        # determine open/closed pixels
+        pix_close  = np.where(self.mask == 1)
+        pix_open   = np.where(self.mask == 0)
+        
+        # determine open/closed pixels
+        x_closed = pix_close[0]
+        y_closed = pix_close[1]
+        x_opened = pix_open[0]
+        y_opened = pix_open[1]
+
+        hex_vert = 1/(np.sqrt(3)/2)
+        hex_radius = (hex_vert)/2.0
+
+        fig, ax = plt.subplots(1)
+        ax.set_aspect('equal')
+
+        # closed pixels
+        for x, y in zip (x_closed, y_closed):
+
+            # determine patch origin
+            x += y * 0.5
+            y *= np.sqrt(3)/2
+
+            # recenter
+            x -= (self.mask.shape[0] + self.mask.shape[1]/2.0)/2.0
+            y -= (self.mask.shape[1] * 1/hex_vert)/2.0
+
+            # add hexagon
+            hex = RegularPolygon((x, y), numVertices=6, radius=hex_radius, 
+                                    orientation=np.radians(60), 
+                                    facecolor='k', alpha=0.5, edgecolor='k')
+            ax.add_patch(hex)
+
+        # open pixels
+        for x, y in zip (x_opened, y_opened):
+
+            # determine patch origin
+            x += y * 0.5
+            y *= np.sqrt(3)/2
+
+            # recenter
+            x -= (self.mask.shape[0] + self.mask.shape[1]/2.0)/2.0
+            y -= (self.mask.shape[1] * 1/hex_vert)/2.0
+
+            # add hexagon
+            hex = RegularPolygon((x, y), numVertices=6, radius=hex_radius, 
+                                    orientation=np.radians(60), 
+                                    facecolor='w', alpha=0.2, edgecolor='k')
+            ax.add_patch(hex)
+
+        plt.xlim(-self.mask.shape[0]/3.0,self.mask.shape[0]/3.0)
+        plt.ylim(-self.mask.shape[0]/3.0,self.mask.shape[1]/3.0)
+        plt.title(f"SHURA [o:{self.v}, r:{self.r}, x:{self.mult}]")
```

### Comparing `codedapertures-0.2/codedapertures.egg-info/PKG-INFO` & `codedapertures-0.3/codedapertures.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedapertures
-Version: 0.2
+Version: 0.3
 Summary: Coded Aperture Production in PYthon (CAPPY)
 Home-page: https://github.com/bpops/cappy
 Author: bpops
 License: MIT
 License-File: LICENSE
 
 CAPPY is a python module that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.
```

### Comparing `codedapertures-0.2/setup.py` & `codedapertures-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 setuptools.setup(name='codedapertures',
-      version='0.2',
+      version='0.3',
       description='Coded Aperture Production in PYthon (CAPPY)',
       long_description='CAPPY is a python module that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.',
       url='https://github.com/bpops/cappy',
       author='bpops',
       license='MIT',
       install_requires=['pyprimes',
                 'numpy',
```

