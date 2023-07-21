# Comparing `tmp/hcam_widgets-1.0.3.tar.gz` & `tmp/hcam_widgets-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcam_widgets-1.0.3.tar", last modified: Mon Sep 13 09:39:25 2021, max compression
+gzip compressed data, was "hcam_widgets-1.1.0.tar", last modified: Fri Jul 21 10:49:41 2023, max compression
```

## Comparing `hcam_widgets-1.0.3.tar` & `hcam_widgets-1.1.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2021-09-13 09:39:25.407786 hcam_widgets-1.0.3/
--rw-r--r--   0 sl         (501) staff       (20)      166 2017-11-13 13:48:04.000000 hcam_widgets-1.0.3/AUTHORS.rst
--rw-r--r--   0 sl         (501) staff       (20)     3303 2017-11-13 15:08:00.000000 hcam_widgets-1.0.3/CONTRIBUTING.rst
--rw-r--r--   0 sl         (501) staff       (20)       89 2017-11-13 13:48:04.000000 hcam_widgets-1.0.3/HISTORY.rst
--rw-r--r--   0 sl         (501) staff       (20)     1077 2017-11-13 13:48:08.000000 hcam_widgets-1.0.3/LICENSE
--rw-r--r--   0 sl         (501) staff       (20)      303 2021-05-26 10:14:11.000000 hcam_widgets-1.0.3/MANIFEST.in
--rw-r--r--   0 sl         (501) staff       (20)     3326 2021-09-13 09:39:25.407861 hcam_widgets-1.0.3/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)     2299 2018-02-15 16:29:54.000000 hcam_widgets-1.0.3/README.rst
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2021-09-13 09:39:25.405660 hcam_widgets-1.0.3/hcam_widgets/
--rw-r--r--   0 sl         (501) staff       (20)      246 2021-09-13 09:39:15.000000 hcam_widgets-1.0.3/hcam_widgets/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     8880 2021-05-26 10:14:11.000000 hcam_widgets-1.0.3/hcam_widgets/astro.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2021-09-13 09:39:25.406842 hcam_widgets-1.0.3/hcam_widgets/compo/
--rw-r--r--   0 sl         (501) staff       (20)        0 2021-05-26 10:14:11.000000 hcam_widgets-1.0.3/hcam_widgets/compo/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)    13914 2021-05-26 10:14:11.000000 hcam_widgets-1.0.3/hcam_widgets/compo/utils.py
--rw-r--r--   0 sl         (501) staff       (20)    12244 2021-05-26 10:14:11.000000 hcam_widgets-1.0.3/hcam_widgets/compo/widgets.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2021-09-13 09:39:25.406962 hcam_widgets-1.0.3/hcam_widgets/data/
--rw-r--r--   0 sl         (501) staff       (20)     1704 2021-05-26 10:14:11.000000 hcam_widgets-1.0.3/hcam_widgets/data/compo_lens_offset.csv
--rw-r--r--   0 sl         (501) staff       (20)     7024 2021-05-26 10:14:11.000000 hcam_widgets-1.0.3/hcam_widgets/globals.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2021-09-13 09:39:25.407575 hcam_widgets-1.0.3/hcam_widgets/hardware/
--rw-r--r--   0 sl         (501) staff       (20)    17450 2021-05-26 10:14:11.000000 hcam_widgets-1.0.3/hcam_widgets/hardware/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     6312 2021-05-26 10:14:11.000000 hcam_widgets-1.0.3/hcam_widgets/hardware/alarms.py
--rw-r--r--   0 sl         (501) staff       (20)     4581 2021-06-14 10:34:27.000000 hcam_widgets-1.0.3/hcam_widgets/hardware/ccds.py
--rw-r--r--   0 sl         (501) staff       (20)     8392 2021-06-14 10:34:38.000000 hcam_widgets-1.0.3/hcam_widgets/hardware/slide.py
--rw-r--r--   0 sl         (501) staff       (20)    68828 2021-09-13 09:35:16.000000 hcam_widgets-1.0.3/hcam_widgets/hcam.py
--rw-r--r--   0 sl         (501) staff       (20)     4036 2018-02-15 16:29:54.000000 hcam_widgets-1.0.3/hcam_widgets/logs.py
--rw-r--r--   0 sl         (501) staff       (20)      370 2021-05-26 10:14:11.000000 hcam_widgets-1.0.3/hcam_widgets/mimic.py
--rw-r--r--   0 sl         (501) staff       (20)    20068 2021-09-13 09:33:55.000000 hcam_widgets-1.0.3/hcam_widgets/misc.py
--rw-r--r--   0 sl         (501) staff       (20)     2087 2021-05-26 10:14:11.000000 hcam_widgets-1.0.3/hcam_widgets/tcs.py
--rw-r--r--   0 sl         (501) staff       (20)     1880 2017-11-22 14:17:48.000000 hcam_widgets-1.0.3/hcam_widgets/tkutils.py
--rw-r--r--   0 sl         (501) staff       (20)    22334 2021-05-26 10:14:11.000000 hcam_widgets-1.0.3/hcam_widgets/ucam.py
--rw-r--r--   0 sl         (501) staff       (20)    36505 2021-05-26 10:14:11.000000 hcam_widgets-1.0.3/hcam_widgets/uspec.py
--rw-r--r--   0 sl         (501) staff       (20)   146303 2021-09-13 09:33:55.000000 hcam_widgets-1.0.3/hcam_widgets/widgets.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2021-09-13 09:39:25.406556 hcam_widgets-1.0.3/hcam_widgets.egg-info/
--rw-r--r--   0 sl         (501) staff       (20)     3326 2021-09-13 09:39:25.000000 hcam_widgets-1.0.3/hcam_widgets.egg-info/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)      827 2021-09-13 09:39:25.000000 hcam_widgets-1.0.3/hcam_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2021-09-13 09:39:25.000000 hcam_widgets-1.0.3/hcam_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2021-09-13 09:39:25.000000 hcam_widgets-1.0.3/hcam_widgets.egg-info/not-zip-safe
--rw-r--r--   0 sl         (501) staff       (20)       71 2021-09-13 09:39:25.000000 hcam_widgets-1.0.3/hcam_widgets.egg-info/requires.txt
--rw-r--r--   0 sl         (501) staff       (20)       13 2021-09-13 09:39:25.000000 hcam_widgets-1.0.3/hcam_widgets.egg-info/top_level.txt
--rw-r--r--   0 sl         (501) staff       (20)      313 2021-09-13 09:39:25.408136 hcam_widgets-1.0.3/setup.cfg
--rw-r--r--   0 sl         (501) staff       (20)     1931 2021-09-13 09:39:15.000000 hcam_widgets-1.0.3/setup.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:49:41.676451 hcam_widgets-1.1.0/
+-rw-r--r--   0 sl         (501) staff       (20)      166 2017-11-13 13:48:04.000000 hcam_widgets-1.1.0/AUTHORS.rst
+-rw-r--r--   0 sl         (501) staff       (20)     3303 2017-11-13 15:08:00.000000 hcam_widgets-1.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 sl         (501) staff       (20)       89 2017-11-13 13:48:04.000000 hcam_widgets-1.1.0/HISTORY.rst
+-rw-r--r--   0 sl         (501) staff       (20)     1077 2017-11-13 13:48:08.000000 hcam_widgets-1.1.0/LICENSE
+-rw-r--r--   0 sl         (501) staff       (20)      303 2021-05-26 10:14:11.000000 hcam_widgets-1.1.0/MANIFEST.in
+-rw-r--r--   0 sl         (501) staff       (20)     3306 2023-07-21 10:49:41.676524 hcam_widgets-1.1.0/PKG-INFO
+-rw-r--r--   0 sl         (501) staff       (20)     2299 2018-02-15 16:29:54.000000 hcam_widgets-1.1.0/README.rst
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:49:41.672860 hcam_widgets-1.1.0/hcam_widgets/
+-rw-r--r--   0 sl         (501) staff       (20)      246 2023-07-21 10:48:53.000000 hcam_widgets-1.1.0/hcam_widgets/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     8880 2021-05-26 10:14:11.000000 hcam_widgets-1.1.0/hcam_widgets/astro.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:49:41.674804 hcam_widgets-1.1.0/hcam_widgets/compo/
+-rw-r--r--   0 sl         (501) staff       (20)        0 2021-05-26 10:14:11.000000 hcam_widgets-1.1.0/hcam_widgets/compo/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)    15062 2023-05-30 12:10:48.000000 hcam_widgets-1.1.0/hcam_widgets/compo/utils.py
+-rw-r--r--   0 sl         (501) staff       (20)    27122 2023-05-17 10:15:42.000000 hcam_widgets-1.1.0/hcam_widgets/compo/widgets.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:49:41.675176 hcam_widgets-1.1.0/hcam_widgets/data/
+-rw-r--r--   0 sl         (501) staff       (20)     1704 2021-05-26 10:14:11.000000 hcam_widgets-1.1.0/hcam_widgets/data/compo_lens_offset.csv
+-rw-r--r--   0 sl         (501) staff       (20)     7024 2021-05-26 10:14:11.000000 hcam_widgets-1.1.0/hcam_widgets/globals.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:49:41.676172 hcam_widgets-1.1.0/hcam_widgets/hardware/
+-rw-r--r--   0 sl         (501) staff       (20)    17450 2021-05-26 10:14:11.000000 hcam_widgets-1.1.0/hcam_widgets/hardware/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     6312 2021-05-26 10:14:11.000000 hcam_widgets-1.1.0/hcam_widgets/hardware/alarms.py
+-rw-r--r--   0 sl         (501) staff       (20)     4751 2023-05-10 10:21:39.000000 hcam_widgets-1.1.0/hcam_widgets/hardware/ccds.py
+-rw-r--r--   0 sl         (501) staff       (20)     9157 2023-05-15 10:45:53.000000 hcam_widgets-1.1.0/hcam_widgets/hardware/slide.py
+-rw-r--r--   0 sl         (501) staff       (20)    70117 2023-05-04 13:39:14.000000 hcam_widgets-1.1.0/hcam_widgets/hcam.py
+-rw-r--r--   0 sl         (501) staff       (20)     4036 2018-02-15 16:29:54.000000 hcam_widgets-1.1.0/hcam_widgets/logs.py
+-rw-r--r--   0 sl         (501) staff       (20)      370 2021-05-26 10:14:11.000000 hcam_widgets-1.1.0/hcam_widgets/mimic.py
+-rw-r--r--   0 sl         (501) staff       (20)    20068 2021-09-13 09:33:55.000000 hcam_widgets-1.1.0/hcam_widgets/misc.py
+-rw-r--r--   0 sl         (501) staff       (20)     2087 2021-05-26 10:14:11.000000 hcam_widgets-1.1.0/hcam_widgets/tcs.py
+-rw-r--r--   0 sl         (501) staff       (20)     1880 2017-11-22 14:17:48.000000 hcam_widgets-1.1.0/hcam_widgets/tkutils.py
+-rw-r--r--   0 sl         (501) staff       (20)    22334 2021-05-26 10:14:11.000000 hcam_widgets-1.1.0/hcam_widgets/ucam.py
+-rw-r--r--   0 sl         (501) staff       (20)    36505 2021-05-26 10:14:11.000000 hcam_widgets-1.1.0/hcam_widgets/uspec.py
+-rw-r--r--   0 sl         (501) staff       (20)   149251 2023-05-12 19:12:14.000000 hcam_widgets-1.1.0/hcam_widgets/widgets.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:49:41.674206 hcam_widgets-1.1.0/hcam_widgets.egg-info/
+-rw-r--r--   0 sl         (501) staff       (20)     3306 2023-07-21 10:49:41.000000 hcam_widgets-1.1.0/hcam_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 sl         (501) staff       (20)      827 2023-07-21 10:49:41.000000 hcam_widgets-1.1.0/hcam_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-21 10:49:41.000000 hcam_widgets-1.1.0/hcam_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-21 10:49:41.000000 hcam_widgets-1.1.0/hcam_widgets.egg-info/not-zip-safe
+-rw-r--r--   0 sl         (501) staff       (20)       71 2023-07-21 10:49:41.000000 hcam_widgets-1.1.0/hcam_widgets.egg-info/requires.txt
+-rw-r--r--   0 sl         (501) staff       (20)       13 2023-07-21 10:49:41.000000 hcam_widgets-1.1.0/hcam_widgets.egg-info/top_level.txt
+-rw-r--r--   0 sl         (501) staff       (20)      313 2023-07-21 10:49:41.676766 hcam_widgets-1.1.0/setup.cfg
+-rw-r--r--   0 sl         (501) staff       (20)     1909 2023-07-21 10:48:53.000000 hcam_widgets-1.1.0/setup.py
```

### Comparing `hcam_widgets-1.0.3/CONTRIBUTING.rst` & `hcam_widgets-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.0.3/LICENSE` & `hcam_widgets-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.0.3/PKG-INFO` & `hcam_widgets-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: hcam_widgets
-Version: 1.0.3
+Version: 1.1.0
 Summary: Common Tkinter widgets for HiPerCAM
 Home-page: https://github.com/HiPERCAM/hcam_widgets
+Download-URL: https://github.com/HiPERCAM/hcam_widgets/archive/v1.1.0.tar.gz
 Author: Stuart Littlefair
 Author-email: s.littlefair@shef.ac.uk
 License: MIT license
-Download-URL: https://github.com/HiPERCAM/hcam_widgets/archive/v1.0.3.tar.gz
 Keywords: hcam_widgets
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
@@ -87,9 +86,7 @@
 History
 =======
 
 0.1.0 (2017-02-11)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `hcam_widgets-1.0.3/README.rst` & `hcam_widgets-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.0.3/hcam_widgets/astro.py` & `hcam_widgets-1.1.0/hcam_widgets/astro.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.0.3/hcam_widgets/compo/utils.py` & `hcam_widgets-1.1.0/hcam_widgets/compo/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,88 +13,136 @@
 from matplotlib.collections import PatchCollection
 
 # optional
 try:
     from ginga import trcalc
     from ginga.util import wcs
     import ginga.canvas.types.all as ginga_types
+
     has_ginga = True
 except Exception:
     has_ginga = False
 
-flip_y = np.array([[1, 0, 0], [0, -1, 0], [0, 0, 1]])
+flip = np.array([[-1, 0, 0], [0, -1, 0], [0, 0, 1]])
 
 # COMPO is only available on GTC, so these values are well-known
 pixel_scale = 0.08086 * u.arcsec / u.pix
 focal_plane_scale = 1.214 * u.arcsec / u.mm
 gtc_focalplane_equivalencies = [
-    (u.mm, u.arcsec, lambda x: x*1.214, lambda x: x/1.214),
-    (u.pix, u.arcsec, lambda x: x/0.08086, lambda x: x*0.08086),
-    (u.mm, u.pix, lambda x: x*1.214/0.08086, lambda x: x*0.08086/1.214)
+    (u.mm, u.arcsec, lambda x: x * 1.214, lambda x: x / 1.214),
+    (u.pix, u.arcsec, lambda x: x / 0.08086, lambda x: x * 0.08086),
+    (u.mm, u.pix, lambda x: x * 1.214 / 0.08086, lambda x: x * 0.08086 / 1.214),
 ]
 
 # predicted position of pick-off pupil from FoV centre
 # from Zeemax simulations
-THETA = u.Quantity([0, 5, 10, 15, 20, 25, 30,
-                    35, 40, 45, 50, 55, 60, 65], unit=u.deg)
-X = u.Quantity([0.0, 0.476, 0.949, 1.414, 1.868, 2.309, 2.731, 3.133,
-                3.511, 3.863, 4.185, 4.475, 4.731, 4.951], unit=u.arcmin)
-Y = u.Quantity([0.0, 0.021, 0.083, 0.186, 0.329, 0.512, 0.732, 0.988,
-                1.278, 1.600, 1.951, 2.329, 2.731, 3.154], unit=u.arcmin)
-
-# Vital statistics from FDR
-PARK_POSITION = -60*u.deg
-MAX_ANGLE = 55*u.deg
-PICKOFF_SIZE = 26.73*u.arcsec  # 330 pixels
-MIRROR_SIZE = 24.3*u.arcsec  # 20 mm
-SHADOW_X = 40*u.mm  # extent of vignetting by injector arm
-SHADOW_Y = 49*u.mm  # extent of vignetting by injector arm (~739 pix)
-INJECTOR_THETA = 13.04*u.deg  # angle of injector arm when in position
-LENS_REF_POSITION = 20 * u.mm  # TODO: this is made up, replace with true value
+THETA = u.Quantity([0, 5, 10, 15, 20, 25, 30, 35, 40, 45, 50, 55, 60, 65], unit=u.deg)
+X = u.Quantity(
+    [
+        0.0,
+        0.476,
+        0.949,
+        1.414,
+        1.868,
+        2.309,
+        2.731,
+        3.133,
+        3.511,
+        3.863,
+        4.185,
+        4.475,
+        4.731,
+        4.951,
+    ],
+    unit=u.arcmin,
+)
+Y = u.Quantity(
+    [
+        0.0,
+        0.021,
+        0.083,
+        0.186,
+        0.329,
+        0.512,
+        0.732,
+        0.988,
+        1.278,
+        1.600,
+        1.951,
+        2.329,
+        2.731,
+        3.154,
+    ],
+    unit=u.arcmin,
+)
+
+# Vital statistics for COMPO (from FDR and commissioning)
+PARK_POSITION = -66.4 * u.deg
+MAX_ANGLE = 55 * u.deg
+PICKOFF_SIZE = 26.73 * u.arcsec  # 330 pixels
+MIRROR_SIZE = 24.3 * u.arcsec  # 20 mm
+SHADOW_X = 40 * u.mm  # extent of vignetting by injector arm
+SHADOW_Y = 49 * u.mm  # extent of vignetting by injector arm (~739 pix)
+INJECTOR_THETA = 13.04 * u.deg  # angle of injector arm when in position
+GUIDE_THETA = -66.4 * u.deg  # angle of injector arm when guiding
+LENS_REF_POSITION = 0 * u.mm  # TODO: this is made up, replace with true value
+NOMINAL_INJECTOR_ZERO = -0.1583 * u.deg  # value of stage encoder when arm centred
+NOMINAL_PICKOFF_ZERO = 0.34 * u.deg  # value of stage encoder when arm centred
+MAX_ANGLE = 67 * u.deg  # hard stops at (67.79, -67.55) for PO, (67.4, -67.8) for IA
 
 # interpolated functions for X and Y positions - not unit aware
-x_func = interp1d(THETA, X, kind='cubic', bounds_error=False, fill_value='extrapolate')
-y_func = interp1d(THETA, Y, kind='cubic', bounds_error=False, fill_value='extrapolate')
+x_func = interp1d(THETA, X, kind="cubic", bounds_error=False, fill_value="extrapolate")
+y_func = interp1d(THETA, Y, kind="cubic", bounds_error=False, fill_value="extrapolate")
 
 # interpolated functions for lens offset
-lens_data_file = pkg_resources.resource_filename('hcam_widgets', 'data/compo_lens_offset.csv')
-_, po_theta, lens_off = np.loadtxt(lens_data_file, delimiter=',', skiprows=1).T
-_g = interp1d(po_theta, lens_off, bounds_error=False, fill_value='extrapolate')
+lens_data_file = pkg_resources.resource_filename(
+    "hcam_widgets", "data/compo_lens_offset.csv"
+)
+_, po_theta, lens_off = np.loadtxt(lens_data_file, delimiter=",", skiprows=1).T
+_g = interp1d(po_theta, lens_off, bounds_error=False, fill_value="extrapolate")
 
 
 @u.quantity_input(pickoff_theta=u.deg)
 def target_lens_position(pickoff_theta, guiding=False):
     """
     Find the correct position for the corrector lens
     """
+    # TODO: find correct value for guiding!
     offset = _g(abs(pickoff_theta.to_value(u.deg))) * u.mm
     return LENS_REF_POSITION + offset
 
 
 @u.quantity_input(theta=u.deg)
 def field_stop_centre(theta):
     """
     Where does the field stop of the injector arm fall in the focal plane?
 
     This is based on Zeemax simulations that include distortions
     and the curvature of the plane.
     """
+    # make a simple float or numpy array
     theta = theta.to_value(u.deg)
-    return x_func(theta)*u.arcmin, y_func(theta)*u.arcmin
+
+    # flip the sign of the x-position if we have a -ve angle
+    xmul = xmul = np.where(theta < 0, -1.0, 1.0)
+
+    # interpolate
+    theta = np.fabs(theta)
+    return xmul * x_func(theta) * u.arcmin, y_func(theta) * u.arcmin
 
 
 def focal_plane_units(unit):
     return unit in (u.deg, u.arcmin, u.arcsec, u.rad)
 
 
 def focal_plane_to_sky(cartrep):
     """
     Convert physical position in focal plane to sky offset from FoV
     """
-    cartrep = cartrep.transform(flip_y)
+    cartrep = cartrep.transform(flip)
     with u.set_enabled_equivalencies(gtc_focalplane_equivalencies):
         return CartesianRepresentation(cartrep.xyz.to(u.arcsec))
 
 
 @u.quantity_input(pickoff_angle=u.deg)
 @u.quantity_input(injection_angle=u.deg)
 def plot_compo(pickoff_angle, injection_angle, axis=None):
@@ -102,61 +150,62 @@
         fig, axis = plt.subplots()
     c = Chip().to_patches()
     poa = PickoffArm().to_patches(pickoff_angle)
     ia = InjectionArm().to_patches(injection_angle)
     # todo set colors with pc.set_array
     cmap = colors.ListedColormap(
         [
-            '#BFD7EA',  # Chip (blue)
-            '#59C9A5',  # POA arc
-            '#56E39F',  # POA Baffle
-            '#3A3042',  # POA FOV
-            '#FF8C42',  # Inj Baffle
-            '#3A3042',  # Inj Fov
+            "#BFD7EA",  # Chip (blue)
+            "#59C9A5",  # POA arc
+            "#56E39F",  # POA Baffle
+            "#3A3042",  # POA FOV
+            "#FF8C42",  # Inj Baffle
+            "#3A3042",  # Inj Fov
         ]
     )
-    pc = PatchCollection(c+poa+ia, alpha=0.8, cmap=cmap)
+    pc = PatchCollection(c + poa + ia, alpha=0.8, cmap=cmap)
     pc.set_array(np.array([0, 1, 2, 3, 4, 5]))
     axis.add_collection(pc)
     axis.set_xlim(-300, 300)
     axis.set_ylim(-50, 150)
-    axis.set_aspect('equal')
+    axis.set_aspect("equal")
     return axis
 
 
 class Chip:
     """
     Representing the Chip
     """
+
     with u.set_enabled_equivalencies(gtc_focalplane_equivalencies):
         NX = (2048 * u.pix).to(u.mm)
         NY = (1024 * u.pix).to(u.mm)
 
     @lazyproperty
     def vertices(self):
         return CartesianRepresentation(
-            [-self.NX/2, self.NX/2, self.NX/2, -self.NX/2],
-            [-self.NY/2, -self.NY/2, self.NY/2, self.NY/2],
-            0*u.mm
+            [-self.NX / 2, self.NX / 2, self.NX / 2, -self.NX / 2],
+            [-self.NY / 2, -self.NY / 2, self.NY / 2, self.NY / 2],
+            0 * u.mm,
         )
 
     def to_patches(self, unit=u.mm):
         with u.set_enabled_equivalencies(gtc_focalplane_equivalencies):
-            ll = ((-self.NX/2).to_value(unit), (-self.NY/2).to_value(unit))
+            ll = ((-self.NX / 2).to_value(unit), (-self.NY / 2).to_value(unit))
             width = self.NX.to_value(unit)
             height = self.NY.to_value(unit)
             rect = patches.Rectangle(ll, width, height)
         return [rect]
 
     def contains(self, repr):
         with u.set_enabled_equivalencies(gtc_focalplane_equivalencies):
             x = repr.x.to(u.mm)
             y = repr.y.to(u.mm)
         inchip = False
-        if (-self.NX/2 < x < self.NX/2) and (-self.NY/2 < y < self.NY/2):
+        if (-self.NX / 2 < x < self.NX / 2) and (-self.NY / 2 < y < self.NY / 2):
             inchip = True
         return inchip
 
     def clip_shape(self, vertices):
         """
         Clip a shape defined as a CartesianRepresentation of points by the chip edges
 
@@ -178,197 +227,225 @@
             new vertices, after clipping
         """
         # enforce pixel space
         try:
             with u.set_enabled_equivalencies(gtc_focalplane_equivalencies):
                 xyz = vertices.xyz.to(u.mm)
         except u.UnitConversionError:
-            raise ValueError('vertices are not in units of physical length')
+            raise ValueError("vertices are not in units of physical length")
 
         # drop Z axis and reshape to (N, 2)
         xy = xyz[:2].T
         poly = path.Path(xy, closed=True)
-        clip_rect = transforms.Bbox([[-self.NX.value/2, -self.NY.value/2],
-                                    [self.NX.value/2, self.NY.value/2]])
+        clip_rect = transforms.Bbox(
+            [
+                [-self.NX.value / 2, -self.NY.value / 2],
+                [self.NX.value / 2, self.NY.value / 2],
+            ]
+        )
         poly_clipped = poly.clip_to_bbox(clip_rect).to_polygons()[0]
         if np.all(poly_clipped[0] == poly_clipped[-1]):
             poly_clipped = poly_clipped[:-1]
 
-        return CartesianRepresentation(*u.Quantity(poly_clipped, unit=u.mm).T, vertices.z)
+        return CartesianRepresentation(
+            *u.Quantity(poly_clipped, unit=u.mm).T, vertices.z
+        )
 
 
 class Baffle:
     """
     The Baffle present on both arms
     """
+
     BAFFLE_X = SHADOW_X
     BAFFLE_Y = SHADOW_Y
-    INJECTION_ROTATION_RIGHT = rotation_matrix(-INJECTOR_THETA, 'z')
-    INJECTION_ROTATION_LEFT = rotation_matrix(INJECTOR_THETA, 'z')
-    INJECTION_TRANSLATION_RIGHT = CartesianRepresentation(57.5*u.mm, 23.2*u.mm, 0*u.mm)
-    INJECTION_TRANSLATION_LEFT = CartesianRepresentation(-57.5*u.mm, 23.2*u.mm, 0*u.mm)
+    INJECTION_ROTATION_RIGHT = rotation_matrix(-INJECTOR_THETA, "z")
+    INJECTION_ROTATION_LEFT = rotation_matrix(INJECTOR_THETA, "z")
+    INJECTION_TRANSLATION_RIGHT = CartesianRepresentation(
+        57.5 * u.mm, 23.2 * u.mm, 0 * u.mm
+    )
+    INJECTION_TRANSLATION_LEFT = CartesianRepresentation(
+        -57.5 * u.mm, 23.2 * u.mm, 0 * u.mm
+    )
 
     @lazyproperty
     def vertices(self):
         return CartesianRepresentation(
-            [-self.BAFFLE_X/2, self.BAFFLE_X/2, self.BAFFLE_X/2, -self.BAFFLE_X/2],
-            [-self.BAFFLE_Y/2, -self.BAFFLE_Y/2, self.BAFFLE_Y/2, self.BAFFLE_Y/2],
-            0*u.mm
+            [
+                -self.BAFFLE_X / 2,
+                self.BAFFLE_X / 2,
+                self.BAFFLE_X / 2,
+                -self.BAFFLE_X / 2,
+            ],
+            [
+                -self.BAFFLE_Y / 2,
+                -self.BAFFLE_Y / 2,
+                self.BAFFLE_Y / 2,
+                self.BAFFLE_Y / 2,
+            ],
+            0 * u.mm,
         )
 
 
 class InjectionArm:
-
     @u.quantity_input(theta=u.deg)
     def position(self, theta):
         """
         Position of pupil stop centre in focal plane (mm)
 
         Uses approximate formula which agrees with Zeemax calculations inc distortion to 1pix
         """
         r = 254.72 * u.mm  # length of injection arm
         off = 270 * u.mm  # dist from rotation axis to FoV centre
         d = off - r
-        x = r * np.sin(theta)
-        y = d + r * (1-np.cos(theta))
-        return CartesianRepresentation(x, y, 0*u.mm)
+        x = r * np.sin(-theta)
+        y = d + r * (1 - np.cos(-theta))
+        return CartesianRepresentation(x, y, 0 * u.mm)
 
     @u.quantity_input(theta=u.deg)
     def to_patches(self, theta, unit=u.mm):
         with u.set_enabled_equivalencies(gtc_focalplane_equivalencies):
             centre = self.position(theta)
             fov = patches.Circle(
                 tuple(centre.xyz[:2].to_value(unit)),
-                radius=MIRROR_SIZE.to_value(unit)/2
+                radius=MIRROR_SIZE.to_value(unit) / 2,
             )
 
             baffle_cart = Baffle().vertices
-            baffle_cart = baffle_cart.transform(rotation_matrix(-theta))
+            baffle_cart = baffle_cart.transform(rotation_matrix(theta))
             baffle_cart += centre
             c = Chip()
             if c.contains(centre):
                 baffle_cart = c.clip_shape(baffle_cart)
             baffle_xy = baffle_cart.xyz[:2].T.to_value(unit)
             baffle = patches.Polygon(baffle_xy, closed=True)
 
         return [baffle, fov]
 
     @u.quantity_input(theta=u.deg)
     @u.quantity_input(ra_cen=u.deg)
     @u.quantity_input(dec_cen=u.deg)
     def to_ginga_object(self, theta, ra_cen, dec_cen, **params):
         if not has_ginga:
-            raise RuntimeError('ginga not installed, cannot create Ginga object')
+            raise RuntimeError("ginga not installed, cannot create Ginga object")
 
         with u.set_enabled_equivalencies(gtc_focalplane_equivalencies):
             # centre w.r.t FoV
             centre = self.position(theta)
+
             # now Baffle
             baffle_cart = Baffle().vertices
-            baffle_cart = baffle_cart.transform(rotation_matrix(-theta))
+            baffle_cart = baffle_cart.transform(rotation_matrix(theta))
             baffle_cart += centre
             c = Chip()
             if c.contains(centre):
                 baffle_cart = c.clip_shape(baffle_cart)
 
             # convert to sky plane
             centre = focal_plane_to_sky(centre)
             baffle_cart = focal_plane_to_sky(baffle_cart)
 
             # add centre of pointing
-            x, y = wcs.add_offset_radec(ra_cen.to_value(u.deg),
-                                        dec_cen.to_value(u.deg),
-                                        *centre.xyz[:2].to_value(u.deg))
+            x, y = wcs.add_offset_radec(
+                ra_cen.to_value(u.deg),
+                dec_cen.to_value(u.deg),
+                *centre.xyz[:2].to_value(u.deg)
+            )
             fov = ginga_types.Circle(
-                x, y, MIRROR_SIZE.to_value(u.deg)/2, coord='wcs', **params
+                x, y, MIRROR_SIZE.to_value(u.deg) / 2, coord="wcs", **params
             )
             # add vignetting by baffle
             corners = [
-                wcs.add_offset_radec(ra_cen.to_value(u.deg),
-                                     dec_cen.to_value(u.deg),
-                                     *p.xyz[:2].to_value(u.deg))
+                wcs.add_offset_radec(
+                    ra_cen.to_value(u.deg),
+                    dec_cen.to_value(u.deg),
+                    *p.xyz[:2].to_value(u.deg)
+                )
                 for p in baffle_cart
             ]
-            vignetting = ginga_types.Polygon(corners, coord='wcs', **params)
+            vignetting = ginga_types.Polygon(corners, coord="wcs", **params)
             return ginga_types.CompoundObject(vignetting, fov)
 
 
 class PickoffArm:
-
     @u.quantity_input(theta=u.deg)
     def position(self, theta):
         """
         Position of pupil stop centre in focal plane (mm)
 
         Uses approximate formula which agrees with Zeemax calculations inc distortion to 1pix
         """
-        r = 270*u.mm
+        r = 270 * u.mm
+        # stage for pickoff arm rotates in opposite sense to coordinate axes
         x = r * np.sin(theta)
         y = r * (1 - np.cos(theta))
         # actually not in focal plane, but assuming it is is OK
-        return CartesianRepresentation(x, y, 0*u.mm)
+        return CartesianRepresentation(x, y, 0 * u.mm)
 
     @u.quantity_input(theta=u.deg)
     def to_patches(self, theta, unit=u.mm):
         with u.set_enabled_equivalencies(gtc_focalplane_equivalencies):
             centre = self.position(theta)
-            patrol_arc_centre = (0, (270*u.mm).to_value(unit))
-            radius = (270*u.mm + 0.5*MIRROR_SIZE).to_value(unit)
+            patrol_arc_centre = (0, (270 * u.mm).to_value(unit))
+            radius = (270 * u.mm + 0.5 * MIRROR_SIZE).to_value(unit)
             arc = patches.Wedge(
-                patrol_arc_centre, radius,
+                patrol_arc_centre,
+                radius,
                 # mpl, 0 is along x axis. COMPO, 0 is along -y
-                PARK_POSITION.to_value(u.deg) - 90, MAX_ANGLE.to_value(u.deg) - 90,
-                width=MIRROR_SIZE.to_value(unit)
+                PARK_POSITION.to_value(u.deg) - 90,
+                MAX_ANGLE.to_value(u.deg) - 90,
+                width=MIRROR_SIZE.to_value(unit),
             )
             pickoff = patches.Circle(
                 tuple(centre.xyz[:2].to_value(unit)),
-                radius=MIRROR_SIZE.to_value(unit)/2
+                radius=MIRROR_SIZE.to_value(unit) / 2,
             )
             baffle_cart = Baffle().vertices
             baffle_cart = baffle_cart.transform(rotation_matrix(-theta))
             baffle_cart += centre
             baffle_xy = baffle_cart.xyz[:2].T.to_value(unit)
             baffle = patches.Polygon(baffle_xy, closed=True)
 
         return [arc, baffle, pickoff]
 
     @u.quantity_input(theta=u.deg)
     @u.quantity_input(ra_cen=u.deg)
     @u.quantity_input(dec_cen=u.deg)
     def to_ginga_object(self, theta, ra_cen, dec_cen, **params):
         if not has_ginga:
-            raise RuntimeError('ginga not installed, cannot create Ginga object')
+            raise RuntimeError("ginga not installed, cannot create Ginga object")
 
         with u.set_enabled_equivalencies(gtc_focalplane_equivalencies):
             # centre w.r.t FoV
             centre = self.position(theta)
 
             # now Baffle
             baffle_cart = Baffle().vertices
             baffle_cart = baffle_cart.transform(rotation_matrix(-theta))
             baffle_cart += centre
-            c = Chip()
-            if c.contains(centre):
-                baffle_cart = c.clip_shape(baffle_cart)
 
             # convert to sky plane
             centre = focal_plane_to_sky(centre)
             baffle_cart = focal_plane_to_sky(baffle_cart)
 
             # create Pickoff circle
-            x, y = wcs.add_offset_radec(ra_cen.to_value(u.deg),
-                                        dec_cen.to_value(u.deg),
-                                        *centre.xyz[:2].to_value(u.deg))
+            x, y = wcs.add_offset_radec(
+                ra_cen.to_value(u.deg),
+                dec_cen.to_value(u.deg),
+                *centre.xyz[:2].to_value(u.deg)
+            )
             fov = ginga_types.Circle(
-                x, y, MIRROR_SIZE.to_value(u.deg)/2, coord='wcs', **params
+                x, y, MIRROR_SIZE.to_value(u.deg) / 2, coord="wcs", **params
             )
             # create vignetting by baffle
             corners = [
-                wcs.add_offset_radec(ra_cen.to_value(u.deg),
-                                     dec_cen.to_value(u.deg),
-                                     *p.xyz[:2].to_value(u.deg))
+                wcs.add_offset_radec(
+                    ra_cen.to_value(u.deg),
+                    dec_cen.to_value(u.deg),
+                    *p.xyz[:2].to_value(u.deg)
+                )
                 for p in baffle_cart
             ]
-            vignetting = ginga_types.Polygon(corners, coord='wcs', **params)
+            vignetting = ginga_types.Polygon(corners, coord="wcs", **params)
 
             # TODO patrol arc.
             return ginga_types.CompoundObject(vignetting, fov)
```

### Comparing `hcam_widgets-1.0.3/hcam_widgets/data/compo_lens_offset.csv` & `hcam_widgets-1.1.0/hcam_widgets/data/compo_lens_offset.csv`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.0.3/hcam_widgets/globals.py` & `hcam_widgets-1.1.0/hcam_widgets/globals.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.0.3/hcam_widgets/hardware/__init__.py` & `hcam_widgets-1.1.0/hcam_widgets/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.0.3/hcam_widgets/hardware/alarms.py` & `hcam_widgets-1.1.0/hcam_widgets/hardware/alarms.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.0.3/hcam_widgets/hardware/ccds.py` & `hcam_widgets-1.1.0/hcam_widgets/hardware/ccds.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,110 +15,120 @@
     import tkinter as tk
 
 
 class CCDTempFrame(tk.LabelFrame):
     """
     Self-contained widget to control CCD temps and reset TECS.
     """
+
     def __init__(self, master):
-        tk.LabelFrame.__init__(
-            self, master, text='CCD TECs', padx=10, pady=4
-        )
+        tk.LabelFrame.__init__(self, master, text="CCD TECs", padx=10, pady=4)
         # Top for table of buttons
         top = tk.Frame(self)
 
-        tk.Label(top, text='CCD1').grid(row=0, column=0)
-        tk.Label(top, text='CCD2').grid(row=0, column=1)
-        tk.Label(top, text='CCD3').grid(row=0, column=2)
-        tk.Label(top, text='CCD4').grid(row=0, column=3)
-        tk.Label(top, text='CCD5').grid(row=0, column=4)
+        tk.Label(top, text="CCD1").grid(row=0, column=0)
+        tk.Label(top, text="CCD2").grid(row=0, column=1)
+        tk.Label(top, text="CCD3").grid(row=0, column=2)
+        tk.Label(top, text="CCD4").grid(row=0, column=3)
+        tk.Label(top, text="CCD5").grid(row=0, column=4)
 
         # maps ccd number to meerstetter, meerstetter address
-        self.mapping = {
-            1: (1, 1), 2: (1, 2), 3: (1, 3),
-            4: (2, 1), 5: (2, 2)
-        }
+        self.mapping = {1: (1, 1), 2: (1, 2), 3: (1, 3), 4: (2, 1), 5: (2, 2)}
 
         self.temp_entry_widgets = {}
         self.setpoint_displays = {}
         self.reset_buttons = {}
         width = 8
         for i in range(1, 6):
             ival = 5
             self.temp_entry_widgets[i] = RangedInt(
                 top, ival, -100, 20, None, True, width=width
             )
-            self.temp_entry_widgets[i].grid(row=1, column=i-1)
-            self.setpoint_displays[i] = tk.Label(top, text='nan', width=width)
-            self.setpoint_displays[i].grid(row=2, column=i-1)
+            self.temp_entry_widgets[i].grid(row=1, column=i - 1)
+            self.setpoint_displays[i] = tk.Label(top, text="nan", width=width)
+            self.setpoint_displays[i].grid(row=2, column=i - 1)
             self.reset_buttons[i] = tk.Button(
-                top, fg='black', width=width, text='Reset',
-                command=lambda ccd=i: self.reset(ccd))
-            self.reset_buttons[i].grid(row=3, column=i-1)
+                top,
+                fg="black",
+                width=width,
+                text="Reset",
+                command=lambda ccd=i: self.reset(ccd),
+            )
+            self.reset_buttons[i].grid(row=3, column=i - 1)
 
         # bind enter to set value routine
         for i in range(1, 6):
             widget = self.temp_entry_widgets[i]
-            widget.unbind('<Return>')
-            widget.bind('<Return>', lambda event, ccd=i: self.update(ccd))
+            widget.unbind("<Return>")
+            widget.bind("<Return>", lambda event, ccd=i: self.update(ccd))
 
         top.pack(pady=2)
         addStyle(self)
 
         self.telemetry_topics = [
-            ('hipercam.meerstetter1.telemetry', lambda data: self.on_telemetry(1, data)),
-            ('hipercam.meerstetter2.telemetry', lambda data: self.on_telemetry(2, data))
+            (
+                "hipercam.meerstetter1.telemetry",
+                lambda data: self.on_telemetry(1, data),
+            ),
+            (
+                "hipercam.meerstetter2.telemetry",
+                lambda data: self.on_telemetry(2, data),
+            ),
         ]
 
     def on_telemetry(self, ms, data):
         g = get_root(self).globals
         try:
             telemetry = pickle.loads(data)
         except Exception as err:
-            wrn = 'cannot parse telemetry from Meerstetter {}: {}'
+            wrn = "cannot parse telemetry from Meerstetter {}: {}"
             g.clog.warn(wrn.format(ms, str(err)))
         else:
             if ms == 1:
                 widget_numbers = (1, 2, 3)
             else:
                 widget_numbers = (4, 5)
             for i, num in enumerate(widget_numbers):
-                key = 'target_temperature{}'.format(i+1)
+                key = "target_temperature{}".format(i + 1)
                 setpoint = telemetry[key].value
                 widget = self.setpoint_displays[num]
                 widget.configure(text=str(setpoint))
 
     @inlineCallbacks
     def update(self, ccd):
         g = get_root(self).globals
-        if not g.cpars['ccd_temp_monitoring_on']:
-            g.clog.warn('Temperature monitoring disabled. Will not update CCD{}'.format(ccd))
+        if not g.cpars["ccd_temp_monitoring_on"]:
+            g.clog.warn(
+                "Temperature monitoring disabled. Will not update CCD{}".format(ccd)
+            )
             return
-        g.clog.info('Updating CCD{}'.format(ccd))
+        g.clog.info("Updating CCD{}".format(ccd))
         widget = self.temp_entry_widgets[ccd]
         val = widget.value()
-        g.clog.info('desired setpoint ' + str(val))
+        g.clog.info("desired setpoint " + str(val))
 
         try:
             session = get_root(self).globals.session
-            topic = 'hipercam.ccd{}.setpoint'.format(ccd)
-            g.clog.info('publishing to topic ' + topic)
+            topic = "hipercam.ccd{}.setpoint".format(ccd)
+            g.clog.info("publishing to topic " + topic)
             yield session.publish(topic, float(val))
         except Exception:
-            g.clog.warn('Unable to update setpoint for CCD{}'.format(ccd))
+            g.clog.warn("Unable to update setpoint for CCD{}".format(ccd))
 
     @inlineCallbacks
     def reset(self, ccd):
         g = get_root(self).globals
-        if not g.cpars['ccd_temp_monitoring_on']:
-            g.clog.warn('Temperature monitoring disabled. Will not reset CCD{}'.format(ccd))
+        if not g.cpars["ccd_temp_monitoring_on"]:
+            g.clog.warn(
+                "Temperature monitoring disabled. Will not reset CCD{}".format(ccd)
+            )
             return
-        g.clog.info('Resetting TEC on CCD{}'.format(ccd))
-        ms, address = self.mapping(ccd)
+        g.clog.info("Resetting TEC on CCD{}".format(ccd))
+        ms, address = self.mapping[ccd]
         try:
-            rpc = 'hipercam.meerstetter{}.rpc.reset'.format(ms)
+            rpc = "hipercam.meerstetter{}.rpc.reset".format(ms)
             session = get_root(self).globals.session
             yield session.call(rpc, address)
         except Exception as err:
-            g.clog.warn('Unable to reset TEC {}'.format(ccd))
-            msg = err.error_message() if hasattr(err, 'error_message') else str(err)
+            g.clog.warn("Unable to reset TEC {}".format(ccd))
+            msg = err.error_message() if hasattr(err, "error_message") else str(err)
             g.clog.warn(msg)
```

### Comparing `hcam_widgets-1.0.3/hcam_widgets/hardware/slide.py` & `hcam_widgets-1.1.0/hcam_widgets/hardware/slide.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from __future__ import absolute_import, division, print_function
 
 import pickle
 
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 from matplotlib import patches
 
@@ -11,73 +10,125 @@
 
 from autobahn.wamp.exception import SerializationError
 
 from hcam_widgets.tkutils import get_root
 from hcam_widgets.widgets import IntegerEntry
 from hcam_widgets.mimic import Mimic
 from hcam_devices.models.slide import BLOCK_POS, UNBLOCK_POS
+from hcam_widgets.misc import async_sleep
 
 from twisted.internet.defer import inlineCallbacks
 
 if not six.PY3:
     import Tkinter as tk
 else:
     import tkinter as tk
 
 
+SLEEP_BEFORE_MOVE = 0.5
+
+
 class SlideFrame(tk.LabelFrame, Mimic):
     """
     Self-contained widget to deal with the focal plane slide
     """
 
     def __init__(self, master, show_mimic=True):
         """
         master  : containing widget
         """
         Mimic.__init__(self, height=200, width=100)
-        tk.LabelFrame.__init__(
-            self, master, text='Focal plane slide', padx=10, pady=4)
+        tk.LabelFrame.__init__(self, master, text="Focal plane slide", padx=10, pady=4)
 
         # Top for table of buttons
         top = tk.Frame(self)
 
         # Define the buttons
         width = 8
-        self.connect = tk.Button(top, fg='black', text='conn', width=width,
-                                 command=lambda: self.action('connection.connect'))
-
-        self.home = tk.Button(top, fg='black', text='home', width=width,
-                              command=lambda: self.action('stage.home'))
-
-        self.block = tk.Button(top, fg='black', text='block', width=width,
-                               command=lambda: self.action('block'))
-
-        self.unblock = tk.Button(top, fg='black', text='unblock', width=width,
-                                 command=lambda: self.action('unblock'))
+        self.connect = tk.Button(
+            top,
+            fg="black",
+            text="conn",
+            width=width,
+            command=lambda: self.action("connection.connect"),
+        )
+
+        self.home = tk.Button(
+            top,
+            fg="black",
+            text="home",
+            width=width,
+            command=lambda: self.action("stage.home"),
+        )
+
+        self.block = tk.Button(
+            top,
+            fg="black",
+            text="block",
+            width=width,
+            command=lambda: self.action("block"),
+        )
+
+        self.unblock = tk.Button(
+            top,
+            fg="black",
+            text="unblock",
+            width=width,
+            command=lambda: self.action("unblock"),
+        )
 
         self.gval = IntegerEntry(top, UNBLOCK_POS, None, True, width=4)
 
-        self.goto = tk.Button(top, fg='black', text='goto', width=width,
-                              command=lambda: self.action('goto',
-                                                          self.gval.value()))
-
-        self.reset = tk.Button(top, fg='black', text='reset', width=width,
-                               command=lambda: self.action('reset'))
-
-        self.stop = tk.Button(top, fg='black', text='stop', width=width,
-                              command=lambda: self.action('stage.stop'))
-
-        self.enable = tk.Button(top, fg='black', text='enable', width=width,
-                                command=lambda: self.action('enable'))
-
-        self.disable = tk.Button(top, fg='black', text='disable', width=width,
-                                 command=lambda: self.action('disable'))
-
-        self.restore = tk.Button(top, fg='black', text='restore', width=width,
-                                 command=lambda: self.action('restore'))
+        self.goto = tk.Button(
+            top,
+            fg="black",
+            text="goto",
+            width=width,
+            command=lambda: self.action("goto", self.gval.value()),
+        )
+
+        self.reset = tk.Button(
+            top,
+            fg="black",
+            text="reset",
+            width=width,
+            command=lambda: self.action("reset"),
+        )
+
+        self.stop = tk.Button(
+            top,
+            fg="black",
+            text="stop",
+            width=width,
+            command=lambda: self.action("stage.stop"),
+        )
+
+        self.enable = tk.Button(
+            top,
+            fg="black",
+            text="enable",
+            width=width,
+            command=lambda: self.action("enable"),
+        )
+
+        self.disable = tk.Button(
+            top,
+            fg="black",
+            text="disable",
+            width=width,
+            command=lambda: self.action("disable"),
+        )
+
+        self.restore = tk.Button(
+            top,
+            fg="black",
+            text="restore",
+            width=width,
+            command=lambda: self.action("restore"),
+        )
 
         # arrange the permanent ones
         self.connect.grid(row=0, column=0)
         self.home.grid(row=0, column=1)
         self.block.grid(row=0, column=2)
         self.unblock.grid(row=1, column=2)
         self.goto.grid(row=1, column=0)
@@ -85,15 +136,15 @@
 
         # set others according to expertlevel
         self.setExpertLevel()
 
         g = get_root(self).globals
 
         # widget for messages
-        self.label = tk.Text(top, height=4, width=30, bg=g.COL['log'])
+        self.label = tk.Text(top, height=4, width=30, bg=g.COL["log"])
         self.label.configure(state=tk.NORMAL, font=g.ENTRY_FONT)
         self.label.grid(row=4, column=0, columnspan=3)
 
         # mimic
         self.showing_mimic = show_mimic
         if show_mimic:
             self.canvas = FigureCanvasTkAgg(self.figure, top)
@@ -105,58 +156,65 @@
         """
         Use current telemetry to update Mimic of the slide
         """
         if not telemetry or not self.showing_mimic:
             return
 
         try:
-            pos = telemetry['position']['current'].value
+            pos = telemetry["position"]["current"].value
         except Exception:
-            pos = telemetry['position']['current']
+            pos = telemetry["position"]["current"]
 
-        state = telemetry['state']
-        connection_state = state['connection']
-        stage_state = state['stage']
-
-        ccd_color, slide_color = ('b', 'k')  # chip slide (stopped)
-        if ('error' in connection_state or 'offline' in connection_state
-                or 'homed' not in stage_state):
-            slide_color = 'r'
-        elif 'moving' in stage_state:
-            slide_color = 'y'
+        state = telemetry["state"]
+        connection_state = state["connection"]
+        stage_state = state["stage"]
+
+        ccd_color, slide_color = ("b", "k")  # chip slide (stopped)
+        if (
+            "error" in connection_state
+            or "offline" in connection_state
+            or "homed" not in stage_state
+        ):
+            slide_color = "r"
+        elif "moving" in stage_state:
+            slide_color = "y"
 
         ll = (0, 0)
         width = 2048
         height = 1024
         ccd = patches.Rectangle(ll, width, height, color=ccd_color, fill=False)
         slide_origin = 3500
-        slide_corners = np.array([
-            ((-50, slide_origin + 50)),  # top left
-            (-50, pos),  # bottom left
-            (2048+50, pos),  # bottom right
-            (2048+50, slide_origin + 50)  # top right
-        ])
-        slide = patches.Polygon(slide_corners, closed=False, alpha=0.8, color=slide_color)
+        slide_corners = np.array(
+            [
+                ((-50, slide_origin + 50)),  # top left
+                (-50, pos),  # bottom left
+                (2048 + 50, pos),  # bottom right
+                (2048 + 50, slide_origin + 50),  # top right
+            ]
+        )
+        slide = patches.Polygon(
+            slide_corners, closed=False, alpha=0.8, color=slide_color
+        )
         self.ax.clear()
         self.ax.add_patch(ccd)
         self.ax.add_patch(slide)
         self.ax.set_xlim(-80, 2048 + 80)
         self.ax.set_ylim(-200, slide_origin + 100)
-        self.ax.set_aspect('equal')
+        self.ax.set_aspect("equal")
         self.ax.set_axis_off()
         self.canvas.draw()
 
     def setExpertLevel(self):
         """
         Modifies widget according to expertise level, which in this
         case is just matter of hiding or revealing the LED option
         and changing the lower limit on the exposure button.
         """
         g = get_root(self).globals
-        level = g.cpars['expert_level']
+        level = g.cpars["expert_level"]
         if level == 0:
             self.reset.grid_forget()
             self.enable.grid_forget()
             self.disable.grid_forget()
             self.restore.grid_forget()
             self.stop.grid_forget()
         else:
@@ -169,71 +227,76 @@
     @inlineCallbacks
     def action(self, *comm):
         """
         Send a command to the focal plane slide
         """
         session = get_root(self).globals.session
         if not session:
-            self.print_message('no session')
+            self.print_message("no session")
             return
 
-        if comm[0] == 'block':
+        if comm[0] == "block":
             topic = "hipercam.slide.rpc.stage.move"
             self.set_slide_target_position(BLOCK_POS)
-        elif comm[0] == 'unblock':
+            # allow time for statemachines to step forward
+            # this means we state is updated to out of position before moving
+            yield async_sleep(SLEEP_BEFORE_MOVE)
+        elif comm[0] == "unblock":
             topic = "hipercam.slide.rpc.stage.move"
             self.set_slide_target_position(UNBLOCK_POS)
-        elif comm[0] == 'goto':
+            yield async_sleep(SLEEP_BEFORE_MOVE)
+        elif comm[0] == "goto":
             topic = "hipercam.slide.rpc.stage.move"
             self.set_slide_target_position(int(comm[1]))
+            yield async_sleep(SLEEP_BEFORE_MOVE)
         else:
             topic = f"hipercam.slide.rpc.{comm[0]}"
 
         try:
             yield session.call(topic)
         except SerializationError:
             pass
         except Exception as err:
             g = get_root(self).globals
-            msg = err.error_message() if hasattr(err, 'error_message') else str(err)
-            g.clog.warn('error in slide command:' + msg)
+            msg = err.error_message() if hasattr(err, "error_message") else str(err)
+            g.clog.warn("error in slide command:" + msg)
 
     def set_slide_target_position(self, pos):
         topic = "hipercam.slide.target_position"
         session = get_root(self).globals.session
         if session:
             session.publish(topic, pos)
 
     def send_message(self, topic, msg):
         session = get_root(self).globals.session
         if session:
             session.publish(topic, msg)
 
     def print_message(self, msg):
         self.label.delete(1.0, tk.END)
-        self.label.insert(tk.END, msg+'\n')
+        self.label.insert(tk.END, msg + "\n")
 
     def on_telemetry(self, package_data):
         telemetry = pickle.loads(package_data)
 
         try:
-            pos = telemetry['position']['current'].value
-            targ = telemetry['position']['target'].value
+            pos = telemetry["position"]["current"].value
+            targ = telemetry["position"]["target"].value
         except Exception:
-            pos = telemetry['position']['current']
-            targ = telemetry['position']['target']
+            pos = telemetry["position"]["current"]
+            targ = telemetry["position"]["target"]
 
-        state = telemetry['state']
-        if 'error' in state['connection'] or 'offline' in state['connection']:
+        state = telemetry["state"]
+        if "error" in state["connection"] or "offline" in state["connection"]:
             self.connect.config(
-                command=lambda: self.action('connection.connect'),
-                text='conn')
+                command=lambda: self.action("connection.connect"), text="conn"
+            )
         else:
             self.connect.config(
-                command=lambda: self.action('connection.disconnect'),
-                text='disconn')
+                command=lambda: self.action("connection.disconnect"), text="disconn"
+            )
 
-        str = f"{telemetry['timestamp'].iso}:\n"
-        status = "/".join(state['stage'][4:])
+        str = f"{telemetry['timestamp']}:\n"
+        status = "/".join(state["stage"][4:])
         str += f"pos: curr={pos:.0f}, targ={targ:.0f}\n{status}\n\n"
         self.update_mimic(telemetry)
         self.print_message(str)
```

### Comparing `hcam_widgets-1.0.3/hcam_widgets/hcam.py` & `hcam_widgets-1.1.0/hcam_widgets/hcam.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,25 @@
 import numpy as np
 from twisted.internet.defer import inlineCallbacks, returnValue
 
 # internal imports
 from . import widgets as w
 from . import DriverError
 from .tkutils import get_root
-from .misc import (createJSON, isPoweredOn, saveJSON, postJSON, startNodding,
-                   execCommand, isRunActive, jsonFromFits, ReadNGCTelemetry)
+from .misc import (
+    createJSON,
+    isPoweredOn,
+    saveJSON,
+    postJSON,
+    startNodding,
+    execCommand,
+    isRunActive,
+    jsonFromFits,
+    ReadNGCTelemetry,
+)
 
 if not six.PY3:
     import Tkinter as tk
     import tkFileDialog as filedialog
     import tkMessageBox as messagebox
 else:
     import tkinter as tk
@@ -43,25 +52,27 @@
 GAIN_SLOW = 1.1
 RNO_FAST = 5.0  # e- / pixel
 RNO_SLOW = 4.5
 DARK_E = 0.02  # e/pix/s
 
 
 FFX = 1024  # X pixels per output
-FFY = 520   # Y pixels per output
+FFY = 520  # Y pixels per output
 PRSCX = 50  # number of pre-scan pixels
 
 
 class ExposureMultiplier(tk.LabelFrame):
     """
     Top to bottom group of RangedInt entry items to specify Nblue etc. Has a max
     number of rows after which it will jump to the left of next column and start over.
     """
-    def __init__(self, master, labels, ivals, imins, imaxs,
-                 nrmax, checker, blank, **kw):
+
+    def __init__(
+        self, master, labels, ivals, imins, imaxs, nrmax, checker, blank, **kw
+    ):
         """
         Parameters
         ----------
         master : tk.widget
             enclosing widget
         labels : iterable
             labels for entry items
@@ -81,27 +92,30 @@
             allowed, even if it is technically invalid
         kw : dict
             keyword arguments
 
         """
         tk.LabelFrame.__init__(self, master, bd=0)
         nitems = len(labels)
-        if (len(ivals) != nitems or len(imins) != nitems or
-                len(imaxs) != nitems):
-            raise DriverError('ExposureMultiplier.__init__ values and options ' +
-                              'must have same length')
+        if len(ivals) != nitems or len(imins) != nitems or len(imaxs) != nitems:
+            raise DriverError(
+                "ExposureMultiplier.__init__ values and options "
+                + "must have same length"
+            )
         self.nitems = nitems
         self.labels = labels
-        self.widgets = [w.RangedInt(self, ival, imin, imax, checker, blank, **kw) for
-                        ival, imin, imax in zip(ivals, imins, imaxs)]
+        self.widgets = [
+            w.RangedInt(self, ival, imin, imax, checker, blank, **kw)
+            for ival, imin, imax in zip(ivals, imins, imaxs)
+        ]
         row = 0
         col = 0
         for nw, widget in enumerate(self.widgets):
             tk.Label(self, text=labels[nw]).grid(row=row, column=col, sticky=tk.W)
-            widget.grid(row=row, column=col+1, sticky=tk.W)
+            widget.grid(row=row, column=col + 1, sticky=tk.W)
             row += 1
             if row == nrmax:
                 col += 1
                 row = 0
 
     def value(self, index):
         return self.widgets[index].value()
@@ -114,113 +128,118 @@
 
     def setall(self, nums):
         for index, val in enumerate(nums):
             self.set(index, val)
 
     def disable(self):
         for widget in self.widgets:
-            widget.configure(state='disable')
+            widget.configure(state="disable")
             widget.set_unbind()
 
     def enable(self):
         for widget in self.widgets:
-            widget.configure(state='normal')
+            widget.configure(state="normal")
             widget.set_bind()
 
 
 class InstPars(tk.LabelFrame):
     """
     Instrument parameters block.
 
     This widget block contains the meat of hdriver. Window settings, readout speed
     etc.
     """
+
     def __init__(self, master):
         """
         master : enclosing widget
         """
         tk.LabelFrame.__init__(self, master)
 
         # left hand side
         lhs = tk.Frame(self)
         rhs = tk.Frame(self)
 
         # Application (mode)
-        tk.Label(lhs, text='Mode').grid(row=0, column=0, sticky=tk.W)
-        self.app = w.Radio(lhs, ('Full', 'Wins', 'Drift'), 3, self.check,
-                           ('FullFrame', 'Windows', 'Drift'))
+        tk.Label(lhs, text="Mode").grid(row=0, column=0, sticky=tk.W)
+        self.app = w.Radio(
+            lhs,
+            ("Full", "Wins", "Drift"),
+            3,
+            self.check,
+            ("FullFrame", "Windows", "Drift"),
+        )
         self.app.grid(row=0, column=1, columnspan=2, sticky=tk.W)
 
         # Clear enabled
-        self.clearLab = tk.Label(lhs, text='Clear')
+        self.clearLab = tk.Label(lhs, text="Clear")
         self.clearLab.grid(row=1, column=0, sticky=tk.W)
         self.clear = w.OnOff(lhs, False, self.check)
         self.clear.grid(row=1, column=1, columnspan=2, sticky=tk.W)
 
         # nod telescope
-        self.nodLab = tk.Label(lhs, text='Dithering')
+        self.nodLab = tk.Label(lhs, text="Dithering")
         self.nodLab.grid(row=2, column=0, sticky=tk.W)
         self.nod = w.OnOff(lhs, False, self.setupNodding)
         self.nod.grid(row=2, column=1, columnspan=2, sticky=tk.W)
         self.nodPattern = {}
 
         # Overscan in x enabled
-        self.oscanLab = tk.Label(lhs, text='Overscan')
+        self.oscanLab = tk.Label(lhs, text="Overscan")
         self.oscanLab.grid(row=3, column=0, sticky=tk.W)
         self.oscan = w.OnOff(lhs, False, self.check)
         self.oscany = w.OnOff(lhs, False, self.check)
         self.oscan.grid(row=3, column=1, sticky=tk.W)
         self.oscany.grid(row=3, column=2, sticky=tk.W)
 
         # led on (expert mode only)
-        self.ledLab = tk.Label(lhs, text='LED setting')
+        self.ledLab = tk.Label(lhs, text="LED setting")
         self.ledLab.grid(row=4, column=0, sticky=tk.W)
         self.led = w.OnOff(lhs, False, None)
         self.led.grid(row=4, column=1, columnspan=2, pady=2, sticky=tk.W)
 
         # dummy mode enabled (expert mode only)
-        self.dummyLab = tk.Label(lhs, text='Dummy Output')
+        self.dummyLab = tk.Label(lhs, text="Dummy Output")
         self.dummyLab.grid(row=5, column=0, sticky=tk.W)
         self.dummy = w.OnOff(lhs, True, self.check)
         self.dummy.grid(row=5, column=1, columnspan=2, pady=2, sticky=tk.W)
 
         # Faster Clock speed enabled
-        self.fastClkLab = tk.Label(lhs, text='Fast Clocks')
+        self.fastClkLab = tk.Label(lhs, text="Fast Clocks")
         self.fastClkLab.grid(row=6, column=0, sticky=tk.W)
         self.fastClk = w.OnOff(lhs, False, self.check)
         self.fastClk.grid(row=6, column=1, columnspan=2, pady=2, sticky=tk.W)
 
         # Readout speed
-        tk.Label(lhs, text='Readout speed').grid(row=7, column=0, sticky=tk.W)
-        self.readSpeed = w.Select(lhs, 1, ('Fast', 'Slow'), self.check)
+        tk.Label(lhs, text="Readout speed").grid(row=7, column=0, sticky=tk.W)
+        self.readSpeed = w.Select(lhs, 1, ("Fast", "Slow"), self.check)
         self.readSpeed.grid(row=7, column=1, columnspan=2, pady=2, sticky=tk.W)
 
         # Exp delay
-        tk.Label(lhs, text='Exposure delay (s)').grid(row=8, column=0,
-                                                      sticky=tk.W)
-        self.expose = w.Expose(lhs, 0.1, 0.00001, 1677.7207,
-                               self.check, width=7)
+        tk.Label(lhs, text="Exposure delay (s)").grid(row=8, column=0, sticky=tk.W)
+        self.expose = w.Expose(lhs, 0.1, 0.00001, 1677.7207, self.check, width=7)
         self.expose.grid(row=8, column=1, columnspan=2, pady=2, sticky=tk.W)
 
         # num exp
-        tk.Label(lhs, text='Num. exposures  ').grid(row=9, column=0,  sticky=tk.W)
+        tk.Label(lhs, text="Num. exposures  ").grid(row=9, column=0, sticky=tk.W)
         self.number = w.PosInt(lhs, 0, None, False, width=7)
         self.number.grid(row=9, column=1, columnspan=2, pady=2, sticky=tk.W)
 
         # nb, ng, nr etc
-        labels = ('nu', 'ng', 'nr', 'ni', 'nz')
+        labels = ("nu", "ng", "nr", "ni", "nz")
         ivals = (1, 1, 1, 1, 1)
         imins = (1, 1, 1, 1, 1)
         imaxs = (500, 500, 500, 500, 500)
-        self.nmult = ExposureMultiplier(rhs, labels, ivals, imins, imaxs,
-                                        5, self.check, False, width=4)
+        self.nmult = ExposureMultiplier(
+            rhs, labels, ivals, imins, imaxs, 5, self.check, False, width=4
+        )
         # grid (on RHS)
         self.nmult.grid(row=0, column=0, columnspan=2, pady=2, sticky=tk.E + tk.S)
 
-        tk.Label(rhs, text='COMPO  ').grid(row=1, column=0)
+        tk.Label(rhs, text="COMPO  ").grid(row=1, column=0)
         self.compo = w.OnOff(rhs, False, self.check)
         self.compo.grid(row=1, column=1, pady=2, sticky=tk.W)
 
         # We have two possible window frames. A single pair for
         # drift mode, or a 2-quad frame for window mode.
 
         # drift frame
@@ -238,19 +257,31 @@
         ysmaxs = (512,)
         # sizes of windows (start at FF)
         nxs = (100,)
         nys = (100,)
         # allowed binning factors
         xbfac = tuple(range(1, 21))
         ybfac = tuple(range(1, 21))
-        self.drift_frame = w.WinPairs(lhs, xsls, xslmins, xslmaxs,
-                                      xsrs, xsrmins, xsrmaxs,
-                                      yss, ysmins, ysmaxs,
-                                      nxs, nys, xbfac, ybfac,
-                                      self.check)
+        self.drift_frame = w.WinPairs(
+            lhs,
+            xsls,
+            xslmins,
+            xslmaxs,
+            xsrs,
+            xsrmins,
+            xsrmaxs,
+            yss,
+            ysmins,
+            ysmaxs,
+            nxs,
+            nys,
+            xbfac,
+            ybfac,
+            self.check,
+        )
 
         # window frame for quads
         # xstart on LHS
         xsll = xsul = (1, 1)
         xsllmin = xsulmin = (1, 1)
         xsllmax = xsulmax = (1024, 1024)
         # xstart on RHS
@@ -260,23 +291,39 @@
         # ystart
         ys = (1, 1)
         ysmin = (1, 1)
         ysmax = (512, 512)
         # sizes (start at FF)
         nx = (1024, 1024)
         ny = (512, 512)
-        self.quad_frame = w.WinQuads(lhs, xsll, xsllmin, xsllmax,
-                                     xsul, xsulmin, xsulmax,
-                                     xslr, xslrmin, xslrmax,
-                                     xsur, xsurmin, xsurmax,
-                                     ys, ysmin, ysmax, nx, ny,
-                                     xbfac, ybfac, self.check)
+        self.quad_frame = w.WinQuads(
+            lhs,
+            xsll,
+            xsllmin,
+            xsllmax,
+            xsul,
+            xsulmin,
+            xsulmax,
+            xslr,
+            xslrmin,
+            xslrmax,
+            xsur,
+            xsurmin,
+            xsurmax,
+            ys,
+            ysmin,
+            ysmax,
+            nx,
+            ny,
+            xbfac,
+            ybfac,
+            self.check,
+        )
 
-        self.quad_frame.grid(row=10, column=0, columnspan=3,
-                             sticky=tk.W+tk.N)
+        self.quad_frame.grid(row=10, column=0, columnspan=3, sticky=tk.W + tk.N)
 
         # Pack two halfs
         lhs.pack(side=tk.LEFT, anchor=tk.N, padx=5)
         rhs.pack(side=tk.LEFT, anchor=tk.N, padx=5)
 
         # Store freeze state
         self.frozen = False
@@ -302,114 +349,115 @@
 
             # clear existing nod pattern
             self.nodPattern = {}
             self.check()
             return
 
         # Do nothing if we're not at the GTC
-        if g.cpars['telins_name'] != 'GTC':
-            messagebox.showerror('Error', 'Cannot dither WHT')
+        if g.cpars["telins_name"] != "GTC":
+            messagebox.showerror("Error", "Cannot dither WHT")
             self.nod.set(False)
             self.nodPattern = {}
             return
 
         # check for drift mode and bomb out
         if self.isDrift():
-            messagebox.showerror('Error', 'Cannot dither telescope in drift mode')
+            messagebox.showerror("Error", "Cannot dither telescope in drift mode")
             self.nod.set(False)
             self.nodPattern = {}
             return
 
         # check for clear not enabled and warn
         if not self.clear():
-            if not messagebox.askokcancel('Warning',
-                                          'Dithering telescope will enable clear mode. Continue?'):
+            if not messagebox.askokcancel(
+                "Warning", "Dithering telescope will enable clear mode. Continue?"
+            ):
                 self.nod.set(False)
                 self.nodPattern = {}
                 return
 
         # Ask for nod pattern
         try:
-            home = expanduser('~')
+            home = expanduser("~")
             fname = filedialog.askopenfilename(
-                title='Open offsets text file',
-                defaultextension='.txt',
-                filetypes=[('text files', '.txt')],
-                initialdir=home)
+                title="Open offsets text file",
+                defaultextension=".txt",
+                filetypes=[("text files", ".txt")],
+                initialdir=home,
+            )
 
             if not fname:
-                g.clog.warn('Aborted load from disk')
+                g.clog.warn("Aborted load from disk")
                 raise ValueError
 
             ra, dec = np.loadtxt(fname).T
             if len(ra) != len(dec):
-                g.clog.warn('Mismatched lengths of RA and Dec offsets')
+                g.clog.warn("Mismatched lengths of RA and Dec offsets")
                 raise ValueError
 
-            data = dict(
-                ra=ra.tolist(),
-                dec=dec.tolist()
-            )
+            data = dict(ra=ra.tolist(), dec=dec.tolist())
         except Exception:
-            g.clog.warn('Setting dither pattern failed. Disabling dithering')
+            g.clog.warn("Setting dither pattern failed. Disabling dithering")
             self.nod.set(False)
             self.nodPattern = {}
             return
 
         # store nodding on ipars object
         self.nodPattern = data
         # enable clear mode
         self.clear.set(True)
         # update
         self.check()
 
     def setExpertLevel(self):
         g = get_root(self).globals
-        level = g.cpars['expert_level']
+        level = g.cpars["expert_level"]
         if level == 0:
             self.ledLab.grid_forget()
             self.led.grid_forget()
             self.led.set(0)
 
-            self.oscanLab.config(text='Overscan')
+            self.oscanLab.config(text="Overscan")
             self.oscany.grid_forget()
             self.remember_oscany = self.oscany()
             self.oscany.set(0)
 
             self.dummyLab.grid_forget()
             self.dummy.grid_forget()
         else:
             self.ledLab.grid(row=4, column=0, sticky=tk.W)
             self.led.grid(row=4, column=1, columnspan=2, pady=2, sticky=tk.W)
 
-            self.oscanLab.config(text='Overscan (x, y)')
+            self.oscanLab.config(text="Overscan (x, y)")
             self.oscany.grid(row=3, column=2, sticky=tk.W)
-            if hasattr(self, 'remember_oscany'):
+            if hasattr(self, "remember_oscany"):
                 self.oscany.set(self.remember_oscany)
 
             self.dummyLab.grid(row=5, column=0, sticky=tk.W)
             self.dummy.grid(row=5, column=1, columnspan=2, pady=2, sticky=tk.W)
 
     def isDrift(self):
-        if self.app.value() == 'Drift':
+        if self.app.value() == "Drift":
             return True
-        elif self.app.value() in ['FullFrame', 'Windows']:
+        elif self.app.value() in ["FullFrame", "Windows"]:
             return False
         else:
-            raise DriverError('InstPars.isDrift: application ' +
-                              self.app.value() + ' not recognised')
+            raise DriverError(
+                "InstPars.isDrift: application " + self.app.value() + " not recognised"
+            )
 
     def isFF(self):
-        if self.app.value() == 'FullFrame':
+        if self.app.value() == "FullFrame":
             return True
-        elif self.app.value() in ['Drift', 'Windows']:
+        elif self.app.value() in ["Drift", "Windows"]:
             return False
         else:
-            raise DriverError('InstPars.isDrift: application ' +
-                              self.app.value() + ' not recognised')
+            raise DriverError(
+                "InstPars.isDrift: application " + self.app.value() + " not recognised"
+            )
 
     def dumpJSON(self):
         """
         Encodes current parameters to JSON compatible dictionary
         """
         numexp = self.number.get()
         expTime, _, _, _, _ = self.timing()
@@ -426,139 +474,155 @@
             dwell=self.expose.value(),
             exptime=expTime,
             oscan=self.oscan(),
             oscany=self.oscany(),
             xbin=self.wframe.xbin.value(),
             ybin=self.wframe.ybin.value(),
             multipliers=self.nmult.getall(),
-            clear=self.clear()
+            clear=self.clear(),
         )
 
         # only allow nodding in clear mode, even if GUI has got confused
-        if data['clear'] and self.nodPattern:
-            data['nodpattern'] = self.nodPattern
+        if data["clear"] and self.nodPattern:
+            data["nodpattern"] = self.nodPattern
 
         # no mixing clear and multipliers, no matter what GUI says
-        if data['clear']:
-            data['multipliers'] = [1 for i in self.nmult.getall()]
+        if data["clear"]:
+            data["multipliers"] = [1 for i in self.nmult.getall()]
 
         # add window mode
         if not self.isFF():
             if self.isDrift():
                 # no clear, multipliers or oscan in drift
-                for setting in ('clear', 'oscan', 'oscany'):
+                for setting in ("clear", "oscan", "oscany"):
                     data[setting] = 0
-                data['multipliers'] = [1 for i in self.nmult.getall()]
+                data["multipliers"] = [1 for i in self.nmult.getall()]
 
                 for iw, (xsl, xsr, ys, nx, ny) in enumerate(self.wframe):
-                    data['x{}start_left'.format(iw+1)] = xsl
-                    data['x{}start_right'.format(iw+1)] = xsr
-                    data['y{}start'.format(iw+1)] = ys
-                    data['y{}size'.format(iw+1)] = ny
-                    data['x{}size'.format(iw+1)] = nx
+                    data["x{}start_left".format(iw + 1)] = xsl
+                    data["x{}start_right".format(iw + 1)] = xsr
+                    data["y{}start".format(iw + 1)] = ys
+                    data["y{}size".format(iw + 1)] = ny
+                    data["x{}size".format(iw + 1)] = nx
             else:
                 # no oscany in window mode
-                data['oscany'] = 0
+                data["oscany"] = 0
 
                 for iw, (xsll, xsul, xslr, xsur, ys, nx, ny) in enumerate(self.wframe):
-                    data['x{}start_upperleft'.format(iw+1)] = xsul
-                    data['x{}start_lowerleft'.format(iw+1)] = xsll
-                    data['x{}start_upperright'.format(iw+1)] = xsur
-                    data['x{}start_lowerright'.format(iw+1)] = xslr
-                    data['y{}start'.format(iw+1)] = ys
-                    data['x{}size'.format(iw+1)] = nx
-                    data['y{}size'.format(iw+1)] = ny
+                    data["x{}start_upperleft".format(iw + 1)] = xsul
+                    data["x{}start_lowerleft".format(iw + 1)] = xsll
+                    data["x{}start_upperright".format(iw + 1)] = xsur
+                    data["x{}start_lowerright".format(iw + 1)] = xslr
+                    data["y{}start".format(iw + 1)] = ys
+                    data["x{}size".format(iw + 1)] = nx
+                    data["y{}size".format(iw + 1)] = ny
         return data
 
     def loadJSON(self, json_string):
         """
         Loads in an application saved in JSON format.
         """
         g = get_root(self).globals
-        data = json.loads(json_string)['appdata']
+
+        # enable COMPO if present in JSON
+        if "compo" in json.loads(json_string):
+            self.compo.set(1)
+        else:
+            self.compo.set(0)
+
+        data = json.loads(json_string)["appdata"]
         # first set the parameters which change regardless of mode
         # number of exposures
-        numexp = data.get('numexp', 0)
+        numexp = data.get("numexp", 0)
         if numexp == -1:
             numexp = 0
         self.number.set(numexp)
         # Overscan (x, y)
-        if 'oscan' in data:
-            self.oscan.set(data['oscan'])
-        if 'oscany' in data:
-            self.oscan.set(data['oscany'])
+        if "oscan" in data:
+            self.oscan.set(data["oscan"])
+        if "oscany" in data:
+            self.oscan.set(data["oscany"])
         # LED setting
-        self.led.set(data.get('led_flsh', 0))
+        self.led.set(data.get("led_flsh", 0))
         # Dummy output enabled
-        self.dummy.set(data.get('dummy_out', 1))
+        self.dummy.set(data.get("dummy_out", 1))
         # Fast clocking option?
-        self.fastClk.set(data.get('fast_clks', 0))
+        self.fastClk.set(data.get("fast_clks", 0))
         # readout speed
-        self.readSpeed.set(data.get('readout', 'Slow'))
+        self.readSpeed.set(data.get("readout", "Slow"))
         # dwell
-        dwell = data.get('dwell', 0)
+        dwell = data.get("dwell", 0)
         self.expose.set(str(float(dwell)))
 
         # multipliers
-        mult_values = data.get('multipliers',
-                               (1, 1, 1, 1, 1))
+        mult_values = data.get("multipliers", (1, 1, 1, 1, 1))
         self.nmult.setall(mult_values)
 
         # look for nodpattern in data
-        nodPattern = data.get('nodpattern', {})
-        if nodPattern and g.cpars['telins_name'] == 'GTC':
+        nodPattern = data.get("nodpattern", {})
+        if nodPattern and g.cpars["telins_name"] == "GTC":
             self.nodPattern = nodPattern
             self.nod.set(True)
             self.clear.set(True)
         else:
             self.nodPattern = {}
             self.nod.set(False)
 
         # binning
-        self.quad_frame.xbin.set(data.get('xbin', 1))
-        self.quad_frame.ybin.set(data.get('ybin', 1))
-        self.drift_frame.xbin.set(data.get('xbin', 1))
-        self.drift_frame.ybin.set(data.get('ybin', 1))
+        self.quad_frame.xbin.set(data.get("xbin", 1))
+        self.quad_frame.ybin.set(data.get("ybin", 1))
+        self.drift_frame.xbin.set(data.get("xbin", 1))
+        self.drift_frame.ybin.set(data.get("ybin", 1))
 
         # now for the behaviour which depends on mode
-        if 'app' in data:
-            self.app.set(data['app'])
-            app = data['app']
+        if "app" in data:
+            self.app.set(data["app"])
+            app = data["app"]
 
-            if app == 'Drift':
+            if app == "Drift":
                 # disable clear mode in drift
                 self.clear.set(0)
                 # only one pair allowed
                 self.wframe.npair.set(1)
 
                 # set the window pair values
-                labels = ('x1start_left', 'y1start',
-                          'x1start_right', 'x1size',
-                          'y1size')
+                labels = (
+                    "x1start_left",
+                    "y1start",
+                    "x1start_right",
+                    "x1size",
+                    "y1size",
+                )
                 if not all(label in data for label in labels):
-                    raise DriverError('Drift mode application missing window params')
+                    raise DriverError("Drift mode application missing window params")
                 # now actually set them
-                self.wframe.xsl[0].set(data['x1start_left'])
-                self.wframe.xsr[0].set(data['x1start_right'])
-                self.wframe.ys[0].set(data['y1start'])
-                self.wframe.nx[0].set(data['x1size'])
-                self.wframe.ny[0].set(data['y1size'])
+                self.wframe.xsl[0].set(data["x1start_left"])
+                self.wframe.xsr[0].set(data["x1start_right"])
+                self.wframe.ys[0].set(data["y1start"])
+                self.wframe.nx[0].set(data["x1size"])
+                self.wframe.ny[0].set(data["y1size"])
                 self.wframe.check()
 
-            elif app == 'FullFrame':
+            elif app == "FullFrame":
                 # enable clear mode if set
-                self.clear.set(data.get('clear', 0))
+                self.clear.set(data.get("clear", 0))
 
-            elif app == 'Windows':
+            elif app == "Windows":
                 # enable clear mode if set
-                self.clear.set(data.get('clear', 0))
+                self.clear.set(data.get("clear", 0))
                 nquad = 0
                 for nw in range(2):
-                    labels = ('x{0}start_lowerleft y{0}start x{0}start_upperleft x{0}start_upperright ' +
-                              'x{0}start_lowerright x{0}size y{0}size').format(nw+1).split()
+                    labels = (
+                        (
+                            "x{0}start_lowerleft y{0}start x{0}start_upperleft x{0}start_upperright "
+                            + "x{0}start_lowerright x{0}size y{0}size"
+                        )
+                        .format(nw + 1)
+                        .split()
+                    )
                     if all(label in data for label in labels):
                         xsll = data[labels[0]]
                         xslr = data[labels[4]]
                         xsul = data[labels[2]]
                         xsur = data[labels[3]]
                         ys = data[labels[1]]
                         nx = data[labels[5]]
@@ -595,142 +659,148 @@
             True or False according to whether the settings are OK.
         """
         status = True
         g = get_root(self).globals
 
         # if we've just enabled COMPO, then raise window if exists
         if self.compo():
-            compo_hw_widget = getattr(g, 'compo_hw', None)
+            compo_hw_widget = getattr(g, "compo_hw", None)
             if compo_hw_widget is not None:
                 compo_hw_widget.deiconify()
 
         # clear errors on binning (may be set later if FF)
         xbinw, ybinw = self.wframe.xbin, self.wframe.ybin
-        xbinw.config(bg=g.COL['main'])
-        ybinw.config(bg=g.COL['main'])
+        xbinw.config(bg=g.COL["main"])
+        ybinw.config(bg=g.COL["main"])
 
         # keep binning factors of drift mode and windowed mode up to date
-        oframe, aframe = ((self.quad_frame, self.drift_frame) if self.drift_frame.winfo_ismapped()
-                          else (self.drift_frame, self.quad_frame))
+        oframe, aframe = (
+            (self.quad_frame, self.drift_frame)
+            if self.drift_frame.winfo_ismapped()
+            else (self.drift_frame, self.quad_frame)
+        )
         xbin, ybin = aframe.xbin.value(), aframe.ybin.value()
         oframe.xbin.set(xbin)
         oframe.ybin.set(ybin)
 
         if not self.frozen:
             if self.clear() or self.isDrift():
                 # disable nmult in clear or drift mode
                 self.nmult.disable()
             else:
                 self.nmult.enable()
 
         if self.isDrift():
-            self.clearLab.config(state='disable')
-            self.nodLab.config(state='disable')
+            self.clearLab.config(state="disable")
+            self.nodLab.config(state="disable")
             if not self.drift_frame.winfo_ismapped():
                 self.quad_frame.grid_forget()
-                self.drift_frame.grid(row=10, column=0, columnspan=3,
-                                      sticky=tk.W+tk.N)
+                self.drift_frame.grid(
+                    row=10, column=0, columnspan=3, sticky=tk.W + tk.N
+                )
 
             if not self.frozen:
-                self.oscany.config(state='disable')
-                self.oscan.config(state='disable')
-                self.clear.config(state='disable')
-                self.nod.config(state='disable')
+                self.oscany.config(state="disable")
+                self.oscan.config(state="disable")
+                self.clear.config(state="disable")
+                self.nod.config(state="disable")
                 self.wframe.enable()
                 status = self.wframe.check()
 
         elif self.isFF():
             # special case check of binning from window frame
             if 1024 % xbin != 0:
                 status = False
-                xbinw.config(bg=g.COL['error'])
+                xbinw.config(bg=g.COL["error"])
             elif (1024 // xbin) % 4 != 0:
                 status = False
-                xbinw.config(bg=g.COL['error'])
+                xbinw.config(bg=g.COL["error"])
             if 512 % ybin != 0:
                 status = False
-                ybinw.config(bg=g.COL['error'])
+                ybinw.config(bg=g.COL["error"])
 
             if not self.quad_frame.winfo_ismapped():
                 self.drift_frame.grid_forget()
-                self.quad_frame.grid(row=10, column=0, columnspan=3,
-                                     sticky=tk.W+tk.N)
+                self.quad_frame.grid(row=10, column=0, columnspan=3, sticky=tk.W + tk.N)
 
-            self.clearLab.config(state='normal')
-            if g.cpars['telins_name'] == 'GTC':
-                self.nodLab.config(state='normal')
+            self.clearLab.config(state="normal")
+            if g.cpars["telins_name"] == "GTC":
+                self.nodLab.config(state="normal")
             else:
-                self.nodLab.config(state='disable')
+                self.nodLab.config(state="disable")
             if not self.frozen:
-                self.oscany.config(state='normal')
-                self.oscan.config(state='normal')
-                self.clear.config(state='normal')
-                if g.cpars['telins_name'] == 'GTC':
-                    self.nod.config(state='normal')
+                self.oscany.config(state="normal")
+                self.oscan.config(state="normal")
+                self.clear.config(state="normal")
+                if g.cpars["telins_name"] == "GTC":
+                    self.nod.config(state="normal")
                 else:
-                    self.nod.config(state='disable')
+                    self.nod.config(state="disable")
                 self.wframe.disable()
 
         else:
-            self.clearLab.config(state='normal')
-            if g.cpars['telins_name'] == 'GTC':
-                self.nodLab.config(state='normal')
+            self.clearLab.config(state="normal")
+            if g.cpars["telins_name"] == "GTC":
+                self.nodLab.config(state="normal")
             else:
-                self.nodLab.config(state='disable')
+                self.nodLab.config(state="disable")
             if not self.quad_frame.winfo_ismapped():
                 self.drift_frame.grid_forget()
-                self.quad_frame.grid(row=10, column=0, columnspan=3,
-                                     sticky=tk.W+tk.N)
+                self.quad_frame.grid(row=10, column=0, columnspan=3, sticky=tk.W + tk.N)
 
             if not self.frozen:
-                self.oscany.config(state='disable')
-                self.oscan.config(state='normal')
-                self.clear.config(state='normal')
-                if g.cpars['telins_name'] == 'GTC':
-                    self.nod.config(state='normal')
+                self.oscany.config(state="disable")
+                self.oscan.config(state="normal")
+                self.clear.config(state="normal")
+                if g.cpars["telins_name"] == "GTC":
+                    self.nod.config(state="normal")
                 else:
-                    self.nod.config(state='disable')
+                    self.nod.config(state="disable")
                 self.wframe.enable()
                 status = self.wframe.check()
 
         # exposure delay
         if self.expose.ok():
-            self.expose.config(bg=g.COL['main'])
+            self.expose.config(bg=g.COL["main"])
         else:
-            self.expose.config(bg=g.COL['warn'])
+            self.expose.config(bg=g.COL["warn"])
             status = False
 
         # don't allow binning other than 1, 2 in overscan or prescan mode
         if self.oscan() or self.oscany():
             if xbin not in (1, 2):
                 status = False
-                xbinw.config(bg=g.COL['error'])
+                xbinw.config(bg=g.COL["error"])
             if ybin not in (1, 2):
                 status = False
-                ybinw.config(bg=g.COL['error'])
+                ybinw.config(bg=g.COL["error"])
 
         # disable clear if nodding enabled. re-enable if not drift
         if not self.frozen:
             if self.nod() or self.nodPattern:
-                self.clear.config(state='disabled')
-                self.clearLab.config(state='disabled')
+                self.clear.config(state="disabled")
+                self.clearLab.config(state="disabled")
             elif not self.isDrift():
-                self.clear.config(state='normal')
-                self.clearLab.config(state='normal')
+                self.clear.config(state="normal")
+                self.clearLab.config(state="normal")
 
         # allow posting if parameters are OK. update count and SN estimates too
         if status:
             try:
                 run_active = yield isRunActive(g)
                 powered_on = yield isPoweredOn(g)
             except Exception as err:
                 g.clog.warn(str(err))
-            if (g.cpars['hcam_server_on'] and g.cpars['eso_server_online'] and
-                    g.observe.start['state'] == 'disabled' and
-                    not run_active and powered_on):
+            if (
+                g.cpars["hcam_server_on"]
+                and g.cpars["eso_server_online"]
+                and g.observe.start["state"] == "disabled"
+                and not run_active
+                and powered_on
+            ):
                 g.observe.start.enable()
             g.count.update()
         else:
             g.observe.start.disable()
 
         returnValue(status)
 
@@ -763,60 +833,52 @@
         self.expose.enable()
         self.number.enable()
         self.wframe.enable()
         self.nmult.enable()
         self.frozen = False
 
     def getRtplotWins(self):
-        """"
+        """ "
         Returns a string suitable to sending off to rtplot when
         it asks for window parameters. Returns null string '' if
         the windows are not OK. This operates on the basis of
         trying to send something back, even if it might not be
         OK as a window setup. Note that we have to take care
         here not to update any GUI components because this is
         called outside of the main thread.
         """
         try:
             if self.isFF():
-                return 'fullframe\r\n'
+                return "fullframe\r\n"
             elif self.isDrift():
                 xbin = self.wframe.xbin.value()
                 ybin = self.wframe.ybin.value()
-                nwin = 2*self.wframe.npair.value()
-                ret = str(xbin) + ' ' + str(ybin) + ' ' + str(nwin) + '\r\n'
+                nwin = 2 * self.wframe.npair.value()
+                ret = str(xbin) + " " + str(ybin) + " " + str(nwin) + "\r\n"
                 for xsl, xsr, ys, nx, ny in self.wframe:
-                    ret += '{:d} {:d} {:d} {:d}\r\n'.format(
-                        xsl, ys, nx, ny
-                    )
-                    ret += '{:d} {:d} {:d} {:d}'.format(
-                        xsr, ys, nx, ny
-                    )
+                    ret += "{:d} {:d} {:d} {:d}\r\n".format(xsl, ys, nx, ny)
+                    ret += "{:d} {:d} {:d} {:d}".format(xsr, ys, nx, ny)
                 return ret
             else:
                 xbin = self.wframe.xbin.value()
                 ybin = self.wframe.ybin.value()
-                nwin = 4*self.wframe.nquad.value()
-                ret = str(xbin) + ' ' + str(ybin) + ' ' + str(nwin) + '\r\n'
+                nwin = 4 * self.wframe.nquad.value()
+                ret = str(xbin) + " " + str(ybin) + " " + str(nwin) + "\r\n"
                 for xsll, xsul, xslr, xsur, ys, nx, ny in self.wframe:
-                    ret += '{:d} {:d} {:d} {:d}\r\n'.format(
-                        xsll, ys, nx, ny
-                    )
-                    ret += '{:d} {:d} {:d} {:d}\r\n'.format(
+                    ret += "{:d} {:d} {:d} {:d}\r\n".format(xsll, ys, nx, ny)
+                    ret += "{:d} {:d} {:d} {:d}\r\n".format(
                         xsul, 1025 - ys - ny, nx, ny
                     )
-                    ret += '{:d} {:d} {:d} {:d}\r\n'.format(
-                        xslr, ys, nx, ny
-                    )
-                    ret += '{:d} {:d} {:d} {:d}\r\n'.format(
+                    ret += "{:d} {:d} {:d} {:d}\r\n".format(xslr, ys, nx, ny)
+                    ret += "{:d} {:d} {:d} {:d}\r\n".format(
                         xsur, 1025 - ys - ny, nx, ny
                     )
                 return ret
         except Exception:
-            return ''
+            return ""
 
     def timing(self):
         """
         Estimates timing information for the current setup. You should
         run a check on the instrument parameters before calling this.
 
         Returns: (expTime, deadTime, cycleTime, dutyCycle)
@@ -831,23 +893,24 @@
         isDriftMode = self.isDrift()
         # FF y/n?
         isFF = self.isFF()
 
         # Set the readout speed
         readSpeed = self.readSpeed()
 
-        if readSpeed == 'Fast' and self.dummy():
+        if readSpeed == "Fast" and self.dummy():
             video = VIDEO_FAST
-        elif readSpeed == 'Slow' and self.dummy():
+        elif readSpeed == "Slow" and self.dummy():
             video = VIDEO_SLOW
         elif not self.dummy():
             video = VIDEO_SLOW_SE
         else:
-            raise DriverError('InstPars.timing: readout speed = ' +
-                              readSpeed + ' not recognised.')
+            raise DriverError(
+                "InstPars.timing: readout speed = " + readSpeed + " not recognised."
+            )
 
         if self.fastClk():
             DUMP_TIME = DUMP_TIME_FAST
             VCLOCK_FRAME = VCLOCK_FAST
             VCLOCK_STORAGE = VCLOCK_FAST
             HCLOCK = HCLOCK_FAST
         else:
@@ -874,194 +937,215 @@
             dys = self.wframe.ys[0].value() - 1
             dnx = self.wframe.nx[0].value()
             dny = self.wframe.ny[0].value()
             dxsl = self.wframe.xsl[0].value()
             dxsr = self.wframe.xsr[0].value()
             # differential shift needed to line both
             # windows up with the edge of the chip
-            diffshift = abs(dxsl - 1 - (2*FFX - dxsr - dnx + 1))
+            diffshift = abs(dxsl - 1 - (2 * FFX - dxsr - dnx + 1))
         elif isFF:
             nwin = 1
             ys, nx, ny = [0], [1024], [512]
         else:
             ys, nx, ny = [], [], []
             xse, xsf, xsg, xsh = [], [], [], []
             nwin = self.wframe.nquad.value()
             for xsll, xsul, xslr, xsur, ysv, nxv, nyv in self.wframe:
                 xse.append(xsll - 1)
                 xsf.append(2049 - xslr - nxv)
                 xsg.append(2049 - xsur - nxv)
                 xsh.append(xsul - 1)
-                ys.append(ysv-1)
+                ys.append(ysv - 1)
                 nx.append(nxv)
                 ny.append(nyv)
 
         # convert timing parameters to seconds
         expose_delay = expose
 
         # clear chip by VCLOCK-ing the image and area and dumping storage area (x5)
         if lclear:
-            clear_time = 5*(FFY*VCLOCK_FRAME + FFY*DUMP_TIME)
+            clear_time = 5 * (FFY * VCLOCK_FRAME + FFY * DUMP_TIME)
         else:
             clear_time = 0.0
 
         if isDriftMode:
             # for drift mode, we need the number of windows in the pipeline
             # and the pipeshift
             nrows = FFY  # number of rows in storage area
-            pnwin = int(((nrows / dny) + 1)/2)
-            pshift = nrows - (2*pnwin-1)*dny
-            frame_transfer = (dny+dys)*VCLOCK_FRAME
+            pnwin = int(((nrows / dny) + 1) / 2)
+            pshift = nrows - (2 * pnwin - 1) * dny
+            frame_transfer = (dny + dys) * VCLOCK_FRAME
 
-            yshift = [dys*VCLOCK_STORAGE]
+            yshift = [dys * VCLOCK_STORAGE]
 
             # After placing the window adjacent to the serial register, the
             # register must be cleared by clocking out the entire register,
             # taking FFX hclocks.
-            line_clear = [0.]
+            line_clear = [0.0]
             if yshift[0] != 0:
                 line_clear[0] = DUMP_TIME
 
             # to calculate number of HCLOCKS needed to read a line in
             # drift mode we have to account for the diff shifts and dumping.
             # first perform diff shifts
             # for now we need this *2 (for quadrants E, H or F, G)
-            numhclocks = 2*diffshift
+            numhclocks = 2 * diffshift
             # now add the amount of clocks needed to get
             # both windows to edge of chip
-            if dxsl - 1 > 2*FFX - dxsr - dnx + 1:
+            if dxsl - 1 > 2 * FFX - dxsr - dnx + 1:
                 # it was the left window that got the diff shift,
                 # so the number of hclocks increases by the amount
                 # needed to get the RH window to the edge
-                numhclocks += 2*FFX - dxsr - dnx + 1
+                numhclocks += 2 * FFX - dxsr - dnx + 1
             else:
                 # vice versa
                 numhclocks += dxsl - 1
             # now we actually clock the windows themselves
             numhclocks += dnx
             # finally, we need to hclock the additional pre-scan pixels
-            numhclocks += 2*PRSCX
+            numhclocks += 2 * PRSCX
 
             # here is the total time to read the whole line
-            line_read = [VCLOCK_STORAGE*ybin + numhclocks*HCLOCK +
-                         video*dnx/xbin + DUMP_TIME + 2*SETUP_READ]
+            line_read = [
+                VCLOCK_STORAGE * ybin
+                + numhclocks * HCLOCK
+                + video * dnx / xbin
+                + DUMP_TIME
+                + 2 * SETUP_READ
+            ]
 
-            readout = [(dny/ybin) * line_read[0]]
+            readout = [(dny / ybin) * line_read[0]]
         elif isFF:
             # move entire image into storage area
-            frame_transfer = FFY*VCLOCK_FRAME + DUMP_TIME
+            frame_transfer = FFY * VCLOCK_FRAME + DUMP_TIME
 
             yshift = [0]
             line_clear = [0]
 
             numhclocks = FFX + PRSCX
-            line_read = [VCLOCK_STORAGE*ybin + numhclocks*HCLOCK +
-                         video*nx[0]/xbin + SETUP_READ]
+            line_read = [
+                VCLOCK_STORAGE * ybin
+                + numhclocks * HCLOCK
+                + video * nx[0] / xbin
+                + SETUP_READ
+            ]
             if oscan:
-                line_read[0] += video*PRSCX/xbin
-            nlines = ny[0]/ybin if not oscany else (ny[0] + 8/ybin)
-            readout = [nlines*line_read[0]]
+                line_read[0] += video * PRSCX / xbin
+            nlines = ny[0] / ybin if not oscany else (ny[0] + 8 / ybin)
+            readout = [nlines * line_read[0]]
         else:
             # windowed mode
             # move entire image into storage area
-            frame_transfer = FFY*VCLOCK_FRAME + DUMP_TIME
+            frame_transfer = FFY * VCLOCK_FRAME + DUMP_TIME
 
             # dump rows in storage area up to start of the window without changing the
             # image area.
-            yshift = nwin*[0.]
-            yshift[0] = ys[0]*DUMP_TIME
+            yshift = nwin * [0.0]
+            yshift[0] = ys[0] * DUMP_TIME
             for nw in range(1, nwin):
-                yshift[nw] = (ys[nw]-ys[nw-1]-ny[nw-1])*DUMP_TIME
+                yshift[nw] = (ys[nw] - ys[nw - 1] - ny[nw - 1]) * DUMP_TIME
 
-            line_clear = nwin*[0.]
+            line_clear = nwin * [0.0]
             # Naidu always dumps the serial register, in windowed mode
             # regardless of whether we need to or not
             for nw in range(nwin):
                 line_clear[nw] = DUMP_TIME
 
             # calculate how long it takes to shift one row into the serial
             # register shift along serial register and then read out the data.
             # total number of hclocks needs to account for diff shifts of
             # windows, carried out in serial
-            numhclocks = nwin*[0]
+            numhclocks = nwin * [0]
             for nw in range(nwin):
                 common_shift = min(xse[nw], xsf[nw], xsg[nw], xsh[nw])
-                diffshifts = sum((xs-common_shift for xs in (xse[nw], xsf[nw], xsg[nw], xsh[nw])))
-                numhclocks[nw] = 2*PRSCX + common_shift + diffshifts + nx[nw]
+                diffshifts = sum(
+                    (xs - common_shift for xs in (xse[nw], xsf[nw], xsg[nw], xsh[nw]))
+                )
+                numhclocks[nw] = 2 * PRSCX + common_shift + diffshifts + nx[nw]
 
-            line_read = nwin*[0.]
+            line_read = nwin * [0.0]
             # line read includes vclocking a row, all the hclocks, digitising pixels and dumping serial register
             # when windows are read out.
             for nw in range(nwin):
-                line_read[nw] = (VCLOCK_STORAGE*ybin + numhclocks[nw]*HCLOCK +
-                                 video*nx[nw]/xbin + 2*SETUP_READ + DUMP_TIME)
+                line_read[nw] = (
+                    VCLOCK_STORAGE * ybin
+                    + numhclocks[nw] * HCLOCK
+                    + video * nx[nw] / xbin
+                    + 2 * SETUP_READ
+                    + DUMP_TIME
+                )
                 if oscan:
-                    line_read[nw] += video*PRSCX/xbin
+                    line_read[nw] += video * PRSCX / xbin
 
             # multiply time to shift one row into serial register by
             # number of rows for total readout time
-            readout = nwin*[0.]
+            readout = nwin * [0.0]
             for nw in range(nwin):
-                nlines = ny[nw]/ybin if not oscany else (ny[nw] + 8/ybin)
+                nlines = ny[nw] / ybin if not oscany else (ny[nw] + 8 / ybin)
                 readout[nw] = nlines * line_read[nw]
 
         # now get the total time to read out one exposure.
         cycleTime = expose_delay + clear_time + frame_transfer
         if isDriftMode:
-            cycleTime += pshift*VCLOCK_STORAGE + yshift[0] + line_clear[0] + readout[0]
+            cycleTime += (
+                pshift * VCLOCK_STORAGE + yshift[0] + line_clear[0] + readout[0]
+            )
         else:
             for nw in range(nwin):
                 cycleTime += yshift[nw] + line_clear[nw] + readout[nw]
 
         # use 5sec estimate for nod time
         # TODO: replace with accurate estimate
         if self.nod() and lclear:
             cycleTime += 5
         elif self.nod():
             g = get_root(self).globals
-            g.clog.warn('ERR: dithering enabled with clear mode off')
+            g.clog.warn("ERR: dithering enabled with clear mode off")
 
-        frameRate = 1.0/cycleTime
+        frameRate = 1.0 / cycleTime
         expTime = expose_delay if lclear else cycleTime - frame_transfer
         deadTime = cycleTime - expTime
-        dutyCycle = 100.0*expTime/cycleTime
+        dutyCycle = 100.0 * expTime / cycleTime
         return (expTime, deadTime, cycleTime, dutyCycle, frameRate)
 
 
 class RunPars(tk.LabelFrame):
     """
     Run parameters
     """
+
     def __init__(self, master):
-        tk.LabelFrame.__init__(self, master, text='Next run parameters',
-                               padx=10, pady=10)
+        tk.LabelFrame.__init__(
+            self, master, text="Next run parameters", padx=10, pady=10
+        )
 
         row = 0
         column = 0
-        tk.Label(self, text='Target name').grid(row=row, column=column, sticky=tk.W)
+        tk.Label(self, text="Target name").grid(row=row, column=column, sticky=tk.W)
 
         row += 1
-        tk.Label(self, text='Filters').grid(row=row, column=column, sticky=tk.W)
+        tk.Label(self, text="Filters").grid(row=row, column=column, sticky=tk.W)
 
         row += 1
-        tk.Label(self, text='Programme ID/OB').grid(row=row, column=column, sticky=tk.W)
+        tk.Label(self, text="Programme ID/OB").grid(row=row, column=column, sticky=tk.W)
 
         row += 1
-        tk.Label(self, text='Principal Investigator').grid(row=row,
-                                                           column=column, sticky=tk.W)
+        tk.Label(self, text="Principal Investigator").grid(
+            row=row, column=column, sticky=tk.W
+        )
 
         row += 1
-        tk.Label(self, text='Observer(s)').grid(row=row, column=column, sticky=tk.W)
+        tk.Label(self, text="Observer(s)").grid(row=row, column=column, sticky=tk.W)
 
         row += 1
-        tk.Label(self, text='Pre-run comment').grid(row=row, column=column, sticky=tk.W)
+        tk.Label(self, text="Pre-run comment").grid(row=row, column=column, sticky=tk.W)
 
         # spacer
         column += 1
-        tk.Label(self, text=' ').grid(row=0, column=column)
+        tk.Label(self, text=" ").grid(row=0, column=column)
 
         # target
         row = 0
         column += 1
         self.target = w.Target(self, self.check)
         self.target.grid(row=row, column=column, sticky=tk.W)
 
@@ -1091,342 +1175,348 @@
         self.comment.grid(row=row, column=column, sticky=tk.W)
 
     def loadJSON(self, json_string):
         """
         Sets the values of the run parameters given an JSON string
         """
         g = get_root(self).globals
-        user = json.loads(json_string)['user']
+        user = json.loads(json_string)["user"]
 
         def setField(widget, field):
             val = user.get(field)
             if val is not None:
                 widget.set(val)
 
-        setField(self.prog_ob.obid, 'OB')
-        setField(self.target, 'target')
-        setField(self.prog_ob.progid, 'ID')
-        setField(self.pi, 'PI')
-        setField(self.observers, 'Observers')
-        setField(self.comment, 'comment')
-        setField(self.filter, 'filters')
-        setField(g.observe.rtype, 'flags')
+        setField(self.prog_ob.obid, "OB")
+        setField(self.target, "target")
+        setField(self.prog_ob.progid, "ID")
+        setField(self.pi, "PI")
+        setField(self.observers, "Observers")
+        setField(self.comment, "comment")
+        setField(self.filter, "filters")
+        setField(g.observe.rtype, "flags")
 
     def dumpJSON(self):
         """
         Encodes current parameters to JSON compatible dictionary
         """
         g = get_root(self).globals
         dtype = g.observe.rtype()
-        if dtype == 'bias':
-            target = 'BIAS'
-        elif dtype == 'flat':
-            target = 'FLAT'
-        elif dtype == 'dark':
-            target = 'DARK'
+        if dtype == "bias":
+            target = "BIAS"
+        elif dtype == "flat":
+            target = "FLAT"
+        elif dtype == "dark":
+            target = "DARK"
         else:
             target = self.target.value()
 
         return dict(
             target=target,
             ID=self.prog_ob.progid.value(),
             PI=self.pi.value(),
-            OB='{:04d}'.format(self.prog_ob.obid.value()),
+            OB="{:04d}".format(self.prog_ob.obid.value()),
             Observers=self.observers.value(),
             comment=self.comment.value(),
             flags=dtype,
-            filters=self.filter.value()
+            filters=self.filter.value(),
         )
 
     def check(self, *args):
         """
         Checks the validity of the run parameters. Returns
         flag (True = OK), and a message which indicates the
         nature of the problem if the flag is False.
         """
 
         ok = True
-        msg = ''
+        msg = ""
         g = get_root(self).globals
         dtype = g.observe.rtype()
-        expert = g.cpars['expert_level'] > 0
+        expert = g.cpars["expert_level"] > 0
 
-        if dtype == 'bias' or dtype == 'flat' or dtype == 'dark':
-            self.pi.configure(state='disable')
-            self.prog_ob.configure(state='disable')
+        if dtype == "bias" or dtype == "flat" or dtype == "dark":
+            self.pi.configure(state="disable")
+            self.prog_ob.configure(state="disable")
             self.target.disable()
         else:
             if expert:
-                self.pi.configure(state='normal')
-                self.prog_ob.configure(state='normal')
+                self.pi.configure(state="normal")
+                self.prog_ob.configure(state="normal")
                 self.prog_ob.enable()
             else:
-                self.prog_ob.configure(state='disable')
-                self.pi.configure(state='disable')
+                self.prog_ob.configure(state="disable")
+                self.pi.configure(state="disable")
                 self.prog_ob.disable()
             self.target.enable()
 
-        if g.cpars['require_run_params']:
+        if g.cpars["require_run_params"]:
             if self.target.ok():
-                self.target.entry.config(bg=g.COL['main'])
+                self.target.entry.config(bg=g.COL["main"])
             else:
-                self.target.entry.config(bg=g.COL['error'])
+                self.target.entry.config(bg=g.COL["error"])
                 ok = False
-                msg += 'Target name field cannot be blank\n'
-
-            if dtype == 'acquisition' or \
-               dtype == 'data' or dtype == 'technical':
+                msg += "Target name field cannot be blank\n"
 
+            if dtype == "acquisition" or dtype == "data" or dtype == "technical":
                 if self.prog_ob.ok():
-                    self.prog_ob.config(bg=g.COL['main'])
+                    self.prog_ob.config(bg=g.COL["main"])
                 else:
-                    self.prog_ob.config(bg=g.COL['error'])
+                    self.prog_ob.config(bg=g.COL["error"])
                     ok = False
-                    msg += 'Programme or OB ID field cannot be blank\n'
+                    msg += "Programme or OB ID field cannot be blank\n"
 
                 if self.pi.ok():
-                    self.pi.config(bg=g.COL['main'])
+                    self.pi.config(bg=g.COL["main"])
                 else:
-                    self.pi.config(bg=g.COL['error'])
+                    self.pi.config(bg=g.COL["error"])
                     ok = False
-                    msg += 'Principal Investigator field cannot be blank\n'
+                    msg += "Principal Investigator field cannot be blank\n"
 
             if self.observers.ok():
-                self.observers.config(bg=g.COL['main'])
+                self.observers.config(bg=g.COL["main"])
             else:
-                self.observers.config(bg=g.COL['error'])
+                self.observers.config(bg=g.COL["error"])
                 ok = False
-                msg += 'Observers field cannot be blank'
+                msg += "Observers field cannot be blank"
         return (ok, msg)
 
     def setExpertLevel(self):
         g = get_root(self).globals
-        expert = g.cpars['expert_level'] > 0
+        expert = g.cpars["expert_level"] > 0
         if expert:
-            self.pi.configure(state='normal')
-            self.prog_ob.configure(state='normal')
+            self.pi.configure(state="normal")
+            self.prog_ob.configure(state="normal")
             self.prog_ob.enable()
         else:
-            self.prog_ob.configure(state='disable')
-            self.pi.configure(state='disable')
+            self.prog_ob.configure(state="disable")
+            self.pi.configure(state="disable")
             self.prog_ob.disable()
 
     def freeze(self):
         """
         Freeze all settings so that they can't be altered
         """
         self.target.disable()
-        self.filter.configure(state='disable')
-        self.prog_ob.configure(state='disable')
-        self.pi.configure(state='disable')
-        self.observers.configure(state='disable')
-        self.comment.configure(state='disable')
+        self.filter.configure(state="disable")
+        self.prog_ob.configure(state="disable")
+        self.pi.configure(state="disable")
+        self.observers.configure(state="disable")
+        self.comment.configure(state="disable")
 
     def unfreeze(self):
         """
         Unfreeze all settings so that they can be altered
         """
         g = get_root(self).globals
-        self.filter.configure(state='normal')
+        self.filter.configure(state="normal")
         dtype = g.observe.rtype()
-        if dtype == 'acquisition' or dtype == 'data' or dtype == 'technical':
-            self.prog_ob.configure(state='normal')
-            self.pi.configure(state='normal')
+        if dtype == "acquisition" or dtype == "data" or dtype == "technical":
+            self.prog_ob.configure(state="normal")
+            self.pi.configure(state="normal")
             self.target.enable()
-        self.observers.configure(state='normal')
-        self.comment.configure(state='normal')
+        self.observers.configure(state="normal")
+        self.comment.configure(state="normal")
 
 
 class CountsFrame(tk.LabelFrame):
     """
     Frame for count rate estimates
     """
+
     def __init__(self, master):
         """
         master : enclosing widget
         """
-        tk.LabelFrame.__init__(self, master, pady=2,
-                               text='Count & S-to-N estimator')
+        tk.LabelFrame.__init__(self, master, pady=2, text="Count & S-to-N estimator")
 
         # divide into left and right frames
         lframe = tk.Frame(self, padx=2)
         rframe = tk.Frame(self, padx=2)
 
         # entries
-        self.filter = w.Radio(lframe,
-                              ('u', 'g', 'r', 'i', 'z'), 3,
-                              self.checkUpdate, initial=1)
-        self.mag = w.RangedFloat(lframe, 18., 0., 30.,
-                                 self.checkUpdate, True, width=5,
-                                 nplaces=2)
-        self.seeing = w.RangedFloat(lframe, 1.0, 0.2, 20.,
-                                    self.checkUpdate, True, True,
-                                    width=5, nplaces=1)
-        self.airmass = w.RangedFloat(lframe, 1.5, 1.0, 5.0,
-                                     self.checkUpdate, True, width=5,
-                                     nplaces=2)
-        self.moon = w.Radio(lframe, ('d', 'g', 'b'),  3, self.checkUpdate)
+        self.filter = w.Radio(
+            lframe, ("u", "g", "r", "i", "z"), 3, self.checkUpdate, initial=1
+        )
+        self.mag = w.RangedFloat(
+            lframe, 18.0, 0.0, 30.0, self.checkUpdate, True, width=5, nplaces=2
+        )
+        self.seeing = w.RangedFloat(
+            lframe, 1.0, 0.2, 20.0, self.checkUpdate, True, True, width=5, nplaces=1
+        )
+        self.airmass = w.RangedFloat(
+            lframe, 1.5, 1.0, 5.0, self.checkUpdate, True, width=5, nplaces=2
+        )
+        self.moon = w.Radio(lframe, ("d", "g", "b"), 3, self.checkUpdate)
 
         # results
-        self.cadence = w.Ilabel(rframe, text='UNDEF', width=10, anchor=tk.W)
-        self.exposure = w.Ilabel(rframe, text='UNDEF', width=10, anchor=tk.W)
-        self.duty = w.Ilabel(rframe, text='UNDEF', width=10, anchor=tk.W)
-        self.peak = w.Ilabel(rframe, text='UNDEF', width=10, anchor=tk.W)
-        self.total = w.Ilabel(rframe, text='UNDEF', width=10, anchor=tk.W)
-        self.ston = w.Ilabel(rframe, text='UNDEF', width=10, anchor=tk.W)
-        self.ston3 = w.Ilabel(rframe, text='UNDEF', width=10, anchor=tk.W)
+        self.cadence = w.Ilabel(rframe, text="UNDEF", width=10, anchor=tk.W)
+        self.exposure = w.Ilabel(rframe, text="UNDEF", width=10, anchor=tk.W)
+        self.duty = w.Ilabel(rframe, text="UNDEF", width=10, anchor=tk.W)
+        self.peak = w.Ilabel(rframe, text="UNDEF", width=10, anchor=tk.W)
+        self.total = w.Ilabel(rframe, text="UNDEF", width=10, anchor=tk.W)
+        self.ston = w.Ilabel(rframe, text="UNDEF", width=10, anchor=tk.W)
+        self.ston3 = w.Ilabel(rframe, text="UNDEF", width=10, anchor=tk.W)
 
         # layout
         # left
-        tk.Label(lframe, text='Filter:').grid(row=0, column=0,
-                                              padx=5, pady=3, sticky=tk.W+tk.N)
+        tk.Label(lframe, text="Filter:").grid(
+            row=0, column=0, padx=5, pady=3, sticky=tk.W + tk.N
+        )
         self.filter.grid(row=0, column=1, padx=5, pady=3, sticky=tk.W)
 
-        tk.Label(lframe, text='Mag:').grid(row=1, column=0, padx=5,
-                                           pady=3, sticky=tk.W)
+        tk.Label(lframe, text="Mag:").grid(row=1, column=0, padx=5, pady=3, sticky=tk.W)
         self.mag.grid(row=1, column=1, padx=5, pady=3, sticky=tk.W)
 
-        tk.Label(lframe, text='Seeing:').grid(row=2, column=0, padx=5,
-                                              pady=3, sticky=tk.W)
+        tk.Label(lframe, text="Seeing:").grid(
+            row=2, column=0, padx=5, pady=3, sticky=tk.W
+        )
         self.seeing.grid(row=2, column=1, padx=5, pady=3, sticky=tk.W)
 
-        tk.Label(lframe, text='Airmass:').grid(row=3, column=0, padx=5,
-                                               pady=3, sticky=tk.W)
+        tk.Label(lframe, text="Airmass:").grid(
+            row=3, column=0, padx=5, pady=3, sticky=tk.W
+        )
         self.airmass.grid(row=3, column=1, padx=5, pady=3, sticky=tk.W)
 
-        tk.Label(lframe, text='Moon:').grid(row=4, column=0, padx=5,
-                                            pady=3, sticky=tk.W)
+        tk.Label(lframe, text="Moon:").grid(
+            row=4, column=0, padx=5, pady=3, sticky=tk.W
+        )
         self.moon.grid(row=4, column=1, padx=5, pady=3, sticky=tk.W)
 
         # right
-        tk.Label(rframe, text='Cadence:').grid(row=0, column=0, padx=5,
-                                               pady=3, sticky=tk.W)
+        tk.Label(rframe, text="Cadence:").grid(
+            row=0, column=0, padx=5, pady=3, sticky=tk.W
+        )
         self.cadence.grid(row=0, column=1, padx=5, pady=3, sticky=tk.W)
 
-        tk.Label(rframe, text='Exposure:').grid(row=1, column=0, padx=5,
-                                                pady=3, sticky=tk.W)
+        tk.Label(rframe, text="Exposure:").grid(
+            row=1, column=0, padx=5, pady=3, sticky=tk.W
+        )
         self.exposure.grid(row=1, column=1, padx=5, pady=3, sticky=tk.W)
 
-        tk.Label(rframe, text='Duty cycle:').grid(row=2, column=0, padx=5,
-                                                  pady=3, sticky=tk.W)
+        tk.Label(rframe, text="Duty cycle:").grid(
+            row=2, column=0, padx=5, pady=3, sticky=tk.W
+        )
         self.duty.grid(row=2, column=1, padx=5, pady=3, sticky=tk.W)
 
-        tk.Label(rframe, text='Peak:').grid(row=3, column=0, padx=5, pady=3,
-                                            sticky=tk.W)
+        tk.Label(rframe, text="Peak:").grid(
+            row=3, column=0, padx=5, pady=3, sticky=tk.W
+        )
         self.peak.grid(row=3, column=1, padx=5, pady=3, sticky=tk.W)
 
-        tk.Label(rframe, text='Total:').grid(row=4, column=0, padx=5,
-                                             pady=3, sticky=tk.W)
+        tk.Label(rframe, text="Total:").grid(
+            row=4, column=0, padx=5, pady=3, sticky=tk.W
+        )
         self.total.grid(row=4, column=1, padx=5, pady=3, sticky=tk.W)
 
-        tk.Label(rframe, text='S/N:').grid(row=5, column=0, padx=5, pady=3, sticky=tk.W)
+        tk.Label(rframe, text="S/N:").grid(row=5, column=0, padx=5, pady=3, sticky=tk.W)
         self.ston.grid(row=5, column=1, padx=5, pady=3, sticky=tk.W)
 
-        tk.Label(rframe, text='S/N (3h):').grid(row=6, column=0, padx=5,
-                                                pady=3, sticky=tk.W)
+        tk.Label(rframe, text="S/N (3h):").grid(
+            row=6, column=0, padx=5, pady=3, sticky=tk.W
+        )
         self.ston3.grid(row=6, column=1, padx=5, pady=3, sticky=tk.W)
 
         # slot frames in
-        lframe.grid(row=0, column=0, sticky=tk.W+tk.N)
-        rframe.grid(row=0, column=1, sticky=tk.W+tk.N)
+        lframe.grid(row=0, column=0, sticky=tk.W + tk.N)
+        rframe.grid(row=0, column=1, sticky=tk.W + tk.N)
 
     def checkUpdate(self, *args):
         """
         Updates values after first checking instrument parameters are OK.
         This is not integrated within update to prevent ifinite recursion
         since update gets called from ipars.
         """
         g = get_root(self).globals
         if not self.check():
-            g.clog.warn('Current observing parameters are not valid.')
+            g.clog.warn("Current observing parameters are not valid.")
             return False
 
         if not g.ipars.check():
-            g.clog.warn('Current instrument parameters are not valid.')
+            g.clog.warn("Current instrument parameters are not valid.")
             return False
 
     def check(self):
         """
         Checks values
         """
         status = True
         g = get_root(self).globals
         if self.mag.ok():
-            self.mag.config(bg=g.COL['main'])
+            self.mag.config(bg=g.COL["main"])
         else:
-            self.mag.config(bg=g.COL['warn'])
+            self.mag.config(bg=g.COL["warn"])
             status = False
 
         if self.airmass.ok():
-            self.airmass.config(bg=g.COL['main'])
+            self.airmass.config(bg=g.COL["main"])
         else:
-            self.airmass.config(bg=g.COL['warn'])
+            self.airmass.config(bg=g.COL["warn"])
             status = False
 
         if self.seeing.ok():
-            self.seeing.config(bg=g.COL['main'])
+            self.seeing.config(bg=g.COL["main"])
         else:
-            self.seeing.config(bg=g.COL['warn'])
+            self.seeing.config(bg=g.COL["warn"])
             status = False
 
         return status
 
     def update(self, *args):
         """
         Updates values. You should run a check on the instrument and
         target parameters before calling this.
         """
         g = get_root(self).globals
         expTime, deadTime, cycleTime, dutyCycle, frameRate = g.ipars.timing()
 
-        total, peak, peakSat, peakWarn, ston, ston3 = \
-            self.counts(expTime, cycleTime)
+        total, peak, peakSat, peakWarn, ston, ston3 = self.counts(expTime, cycleTime)
 
         if cycleTime < 0.01:
-            self.cadence.config(text='{0:7.5f} s'.format(cycleTime))
+            self.cadence.config(text="{0:7.5f} s".format(cycleTime))
         elif cycleTime < 0.1:
-            self.cadence.config(text='{0:6.4f} s'.format(cycleTime))
-        elif cycleTime < 1.:
-            self.cadence.config(text='{0:5.3f} s'.format(cycleTime))
-        elif cycleTime < 10.:
-            self.cadence.config(text='{0:4.2f} s'.format(cycleTime))
-        elif cycleTime < 100.:
-            self.cadence.config(text='{0:4.1f} s'.format(cycleTime))
-        elif cycleTime < 1000.:
-            self.cadence.config(text='{0:4.0f} s'.format(cycleTime))
+            self.cadence.config(text="{0:6.4f} s".format(cycleTime))
+        elif cycleTime < 1.0:
+            self.cadence.config(text="{0:5.3f} s".format(cycleTime))
+        elif cycleTime < 10.0:
+            self.cadence.config(text="{0:4.2f} s".format(cycleTime))
+        elif cycleTime < 100.0:
+            self.cadence.config(text="{0:4.1f} s".format(cycleTime))
+        elif cycleTime < 1000.0:
+            self.cadence.config(text="{0:4.0f} s".format(cycleTime))
         else:
-            self.cadence.config(text='{0:5.0f} s'.format(cycleTime))
+            self.cadence.config(text="{0:5.0f} s".format(cycleTime))
 
         if expTime < 0.01:
-            self.exposure.config(text='{0:7.5f} s'.format(expTime))
+            self.exposure.config(text="{0:7.5f} s".format(expTime))
         elif expTime < 0.1:
-            self.exposure.config(text='{0:6.4f} s'.format(expTime))
-        elif expTime < 1.:
-            self.exposure.config(text='{0:5.3f} s'.format(expTime))
-        elif expTime < 10.:
-            self.exposure.config(text='{0:4.2f} s'.format(expTime))
-        elif expTime < 100.:
-            self.exposure.config(text='{0:4.1f} s'.format(expTime))
-        elif expTime < 1000.:
-            self.exposure.config(text='{0:4.0f} s'.format(expTime))
+            self.exposure.config(text="{0:6.4f} s".format(expTime))
+        elif expTime < 1.0:
+            self.exposure.config(text="{0:5.3f} s".format(expTime))
+        elif expTime < 10.0:
+            self.exposure.config(text="{0:4.2f} s".format(expTime))
+        elif expTime < 100.0:
+            self.exposure.config(text="{0:4.1f} s".format(expTime))
+        elif expTime < 1000.0:
+            self.exposure.config(text="{0:4.0f} s".format(expTime))
         else:
-            self.exposure.config(text='{0:5.0f} s'.format(expTime))
+            self.exposure.config(text="{0:5.0f} s".format(expTime))
 
-        self.duty.config(text='{0:4.1f} %'.format(dutyCycle))
-        self.peak.config(text='{0:d} cts'.format(int(round(peak))))
+        self.duty.config(text="{0:4.1f} %".format(dutyCycle))
+        self.peak.config(text="{0:d} cts".format(int(round(peak))))
         if peakSat:
-            self.peak.config(bg=g.COL['error'])
+            self.peak.config(bg=g.COL["error"])
         elif peakWarn:
-            self.peak.config(bg=g.COL['warn'])
+            self.peak.config(bg=g.COL["warn"])
         else:
-            self.peak.config(bg=g.COL['main'])
+            self.peak.config(bg=g.COL["main"])
 
-        self.total.config(text='{0:d} cts'.format(int(round(total))))
-        self.ston.config(text='{0:.1f}'.format(ston))
-        self.ston3.config(text='{0:.1f}'.format(ston3))
+        self.total.config(text="{0:d} cts".format(int(round(total))))
+        self.ston.config(text="{0:.1f}".format(ston))
+        self.ston3.config(text="{0:.1f}".format(ston3))
 
     def counts(self, expTime, cycleTime, ap_scale=1.6, ndiv=5):
         """
         Computes counts per pixel, total counts, sky counts
         etc given current magnitude, seeing etc. You should
         run a check on the instrument parameters before calling
         this.
@@ -1446,105 +1536,107 @@
         """
 
         # code directly translated from Java equivalent.
         g = get_root(self).globals
 
         # Set the readout speed
         readSpeed = g.ipars.readSpeed()
-        if readSpeed == 'Fast':
+        if readSpeed == "Fast":
             gain = GAIN_FAST
             read = RNO_FAST
-        elif readSpeed == 'Slow':
+        elif readSpeed == "Slow":
             gain = GAIN_SLOW
             read = RNO_SLOW
         else:
-            raise DriverError('CountsFrame.counts: readout speed = ' +
-                              readSpeed + ' not recognised.')
+            raise DriverError(
+                "CountsFrame.counts: readout speed = " + readSpeed + " not recognised."
+            )
 
         xbin, ybin = g.ipars.wframe.xbin.value(), g.ipars.wframe.ybin.value()
 
         # calculate SN info.
-        zero, sky, skyTot, darkTot = 0., 0., 0., 0.
-        total, peak, correct, signal, readTot, seeing = 0., 0., 0., 0., 0., 0.
-        noise, narcsec, npix, signalToNoise3 = 1., 0., 0., 0.
+        zero, sky, skyTot, darkTot = 0.0, 0.0, 0.0, 0.0
+        total, peak, correct, signal, readTot, seeing = 0.0, 0.0, 0.0, 0.0, 0.0, 0.0
+        noise, narcsec, npix, signalToNoise3 = 1.0, 0.0, 0.0, 0.0
 
-        tinfo = g.TINS[g.cpars['telins_name']]
+        tinfo = g.TINS[g.cpars["telins_name"]]
         filtnam = self.filter.value()
 
-        zero = tinfo['zerop'][filtnam]
+        zero = tinfo["zerop"][filtnam]
         mag = self.mag.value()
         seeing = self.seeing.value()
         sky = g.SKY[self.moon.value()][filtnam]
         airmass = self.airmass.value()
-        plateScale = tinfo['plateScale']
+        plateScale = tinfo["plateScale"]
 
         # calculate expected electrons
-        total = 10.**((zero-mag-airmass*g.EXTINCTION[filtnam])/2.5)*expTime
+        total = 10.0 ** ((zero - mag - airmass * g.EXTINCTION[filtnam]) / 2.5) * expTime
 
         # compute fraction that fall in central pixel
         # assuming target exactly at its centre. Do this
         # by splitting each pixel of the central (potentially
         # binned) pixel into ndiv * ndiv points at
         # which the seeing profile is added. sigma is the
         # RMS seeing in terms of pixels.
-        sigma = seeing/g.EFAC/plateScale
+        sigma = seeing / g.EFAC / plateScale
 
-        sum = 0.
+        sum = 0.0
         for iyp in range(ybin):
-            yoff = -ybin/2.+iyp
+            yoff = -ybin / 2.0 + iyp
             for ixp in range(xbin):
-                xoff = -xbin/2.+ixp
+                xoff = -xbin / 2.0 + ixp
                 for iys in range(ndiv):
-                    y = (yoff + (iys+0.5)/ndiv)/sigma
+                    y = (yoff + (iys + 0.5) / ndiv) / sigma
                     for ixs in range(ndiv):
-                        x = (xoff + (ixs+0.5)/ndiv)/sigma
-                        sum += math.exp(-(x*x+y*y)/2.)
-        peak = total*sum/(2.*math.pi*sigma**2*ndiv**2)
+                        x = (xoff + (ixs + 0.5) / ndiv) / sigma
+                        sum += math.exp(-(x * x + y * y) / 2.0)
+        peak = total * sum / (2.0 * math.pi * sigma**2 * ndiv**2)
 
         # Work out fraction of flux in aperture with radius AP_SCALE*seeing
-        correct = 1. - math.exp(-(g.EFAC*ap_scale)**2/2.)
+        correct = 1.0 - math.exp(-((g.EFAC * ap_scale) ** 2) / 2.0)
 
         # expected sky e- per arcsec
-        skyPerArcsec = 10.**((zero-sky)/2.5)*expTime
+        skyPerArcsec = 10.0 ** ((zero - sky) / 2.5) * expTime
         # skyPerPixel = skyPerArcsec*plateScale**2*xbin*ybin
-        narcsec = math.pi*(ap_scale*seeing)**2
-        skyTot = skyPerArcsec*narcsec
-        npix = math.pi*(ap_scale*seeing/plateScale)**2/xbin/ybin
-
-        signal = correct*total  # in electrons
-        darkTot = npix*DARK_E*expTime  # in electrons
-        readTot = npix*read**2  # in electrons
+        narcsec = math.pi * (ap_scale * seeing) ** 2
+        skyTot = skyPerArcsec * narcsec
+        npix = math.pi * (ap_scale * seeing / plateScale) ** 2 / xbin / ybin
+
+        signal = correct * total  # in electrons
+        darkTot = npix * DARK_E * expTime  # in electrons
+        readTot = npix * read**2  # in electrons
 
         # noise, in electrons
         noise = math.sqrt(readTot + darkTot + skyTot + signal)
 
         # Now compute signal-to-noise in 3 hour seconds run
-        signalToNoise3 = signal/noise*math.sqrt(3*3600./cycleTime)
+        signalToNoise3 = signal / noise * math.sqrt(3 * 3600.0 / cycleTime)
 
         # convert from electrons to counts
         total /= gain
         peak /= gain
 
         warn = 25000
         sat = 60000
 
         peakSat = peak > sat
         peakWarn = peak > warn
 
-        return (total, peak, peakSat, peakWarn, signal/noise, signalToNoise3)
+        return (total, peak, peakSat, peakWarn, signal / noise, signalToNoise3)
 
 
 class RunType(w.Select):
     """
     Dropdown box to select run type.
 
     Start button should be disabled until an option is made from this dropdown.
     """
-    DTYPES = ('', 'data', 'acquire', 'bias', 'flat', 'dark', 'tech')
-    DVALS = ('', 'data', 'acquisition', 'bias', 'flat', 'dark', 'technical')
+
+    DTYPES = ("", "data", "acquire", "bias", "flat", "dark", "tech")
+    DVALS = ("", "data", "acquisition", "bias", "flat", "dark", "technical")
 
     def __init__(self, master, start_button, checker=None):
         w.Select.__init__(self, master, 0, RunType.DTYPES, self.check)
         self.start_button = start_button
         self._checker = checker
 
     def __call__(self):
@@ -1555,28 +1647,32 @@
         index = RunType.DVALS.index(value)
         w.Select.set(self, RunType.DTYPES[index])
 
     @inlineCallbacks
     def check(self, *args):
         if self._checker is not None:
             self._checker()
-        if self.val.get() == '':
+        if self.val.get() == "":
             self.start_button.run_type_set = False
             self.start_button.disable()
         else:
             self.start_button.run_type_set = True
             g = get_root(self).globals
             try:
                 run_active = yield isRunActive(g)
                 powered_on = yield isPoweredOn(g)
             except Exception as err:
                 g.clog.warn(str(err))
-            if (g.cpars['hcam_server_on'] and g.cpars['eso_server_online'] and
-                    g.observe.start['state'] == 'disabled' 
-                    and not run_active and powered_on):
+            if (
+                g.cpars["hcam_server_on"]
+                and g.cpars["eso_server_online"]
+                and g.observe.start["state"] == "disabled"
+                and not run_active
+                and powered_on
+            ):
                 self.start_button.enable()
             g.rpars.check()
 
 
 class Start(w.ActButton):
     """
     Button to start a run.
@@ -1586,57 +1682,58 @@
     -- check the instrument and run parameters are OK
     -- optionally, hassle the user if the target changes
     -- post the run settings to the ESO NGC control server
     -- start the run
     -- update the button status
     -- start the exposure timer
     """
+
     def __init__(self, master, width):
         """
         Parameters
         ----------
         master : tk
             containing widget
         width : int
             width of button
         """
-        w.ActButton.__init__(self, master, width, text='Start')
+        w.ActButton.__init__(self, master, width, text="Start")
         g = get_root(self).globals
-        self.config(bg=g.COL['start'])
+        self.config(bg=g.COL["start"])
         self.target = None
         self.run_type_set = False
 
     def enable(self):
         """
         Enable the button
         """
         if self.run_type_set:
             w.ActButton.enable(self)
             g = get_root(self).globals
-            self.config(bg=g.COL['start'])
+            self.config(bg=g.COL["start"])
 
     def disable(self):
         """
         Disable the button, if in non-expert mode.
         """
         w.ActButton.disable(self)
         g = get_root(self).globals
         if self._expert:
-            self.config(bg=g.COL['start'])
+            self.config(bg=g.COL["start"])
         else:
-            self.config(bg=g.COL['startD'])
+            self.config(bg=g.COL["startD"])
 
     def setExpert(self):
         """
         Turns on 'expert' status whereby the button is always enabled,
         regardless of its activity status.
         """
         w.ActButton.setExpert(self)
         g = get_root(self).globals
-        self.config(bg=g.COL['start'])
+        self.config(bg=g.COL["start"])
 
     def setNonExpert(self):
         """
         Turns off 'expert' status whereby to allow a button to be disabled
         """
         self._expert = False
         if self._active and self.run_type_set:
@@ -1646,24 +1743,24 @@
 
     @inlineCallbacks
     def on_telemetry(self, package):
         """
         This is run every time a telemetry packet comes in from NGC.
 
         It is the responsibility of an implementing GUI to subscribe to the
-        NGC telemetry topic with this function as the callback. 
+        NGC telemetry topic with this function as the callback.
         """
         telemetry = pickle.loads(package)
         res = ReadNGCTelemetry(telemetry)
         if not res.ok:
-            raise DriverError('cannot read NGC telemetry: ' + str(res.err))
-        if res.clocks != 'enabled':
+            raise DriverError("cannot read NGC telemetry: " + str(res.err))
+        if res.clocks != "enabled":
             # NGC voltages are not powered on, cannot start runs
             self.disable()
-        elif res.state == 'active':
+        elif res.state == "active":
             # run is underway - cannot start runs
             self.disable()
         else:
             self.enable()
 
     @inlineCallbacks
     def act(self):
@@ -1678,54 +1775,76 @@
         region. Some columns will contain a
         mix of o/scan and data.
 
         Click OK if you wish to continue."""
         if g.ipars.oscan():
             xbin, ybin = g.ipars.wframe.xbin.value(), g.ipars.wframe.ybin.value()
             if xbin not in (1, 2, 5, 10) or ybin not in (1, 2, 5, 10):
-                if not messagebox.askokcancel('Binning alert', msg):
-                    return False
+                if not messagebox.askokcancel("Binning alert", msg):
+                    returnValue(False)
 
         # Check instrument pars are OK
         if not g.ipars.check():
-            g.clog.warn('Invalid instrument parameters; save failed.')
+            g.clog.warn("Invalid instrument parameters; start failed.")
             returnValue(False)
 
         # create JSON to post
         data = yield createJSON(g)
 
+        # check if COMPO is in position
+        # Do this regardless if enabled or not, as we might need to park
+        if not g.compo_hw.ok_to_start_run:
+            msg = """
+            COMPO is reporting that it is not ready to start a run.
+            Please check the state of COMPO.
+            
+            Click OK if you wish to continue anyway."""
+            if not messagebox.askokcancel("COMPO alert", msg):
+                returnValue(False)
+
+        # check autoguiding is started if we are guiding with COMPO
+        if g.ipars.compo() and g.compo_hw.setup_frame.injection_side.value() == "G":
+            msg = """
+            COMPO setup implies you will be guiding with COMPO.
+            Check that autoguiding is set up and running.
+            
+            Click OK when you wish to continue and start run.
+            Click Cancel to abort run."""
+            if not messagebox.askokcancel("Guiding alert", msg):
+                returnValue(False)
+
         # POST
         try:
             success = yield postJSON(g, data)
             if not success:
-                raise Exception('postJSON returned False')
+                raise Exception("postJSON returned False")
         except Exception as err:
             g.clog.warn("Failed to post data to servers")
             g.clog.warn(str(err))
             returnValue(False)
 
         # START
         try:
-            success = yield execCommand(g, 'start')
+            success = yield execCommand(g, "start")
             if not success:
                 raise Exception("Start command failed: check server response")
         except Exception as err:
-            g.clog.warn('Failed to start run')
+            g.clog.warn("Failed to start run")
             g.clog.warn(str(err))
             returnValue(False)
 
         # Is nod enabled? Should we start GTC offsetter?
         try:
             success = yield startNodding(g, data)
             if not success:
-                raise Exception('Failed to start dither: response was false')
+                raise Exception("Failed to start dither: response was false")
         except Exception as err:
             g.clog.warn("Failed to start GTC offsetter")
             g.clog.warn(str(err))
-            g.clog.warn('Run may be paused indefinitely')
+            g.clog.warn("Run may be paused indefinitely")
             g.clog.warn('use "ngcbCmd seq start" to fix')
             returnValue(False)
 
         # Run successfully started.
         # enable stop button, disable Start
         # also make inactive until RunType select box makes active again
         # start run timer
@@ -1745,74 +1864,79 @@
     """
 
     def __init__(self, master, width):
         """
         master  : containing widget
         width   : width of button
         """
-        w.ActButton.__init__(self, master, width, text='Load')
+        w.ActButton.__init__(self, master, width, text="Load")
 
     def act(self):
         """
         Carries out the action associated with the Load button
         """
         g = get_root(self).globals
         fname = filedialog.askopenfilename(
-            defaultextension='.json',
-            filetypes=[('json files', '.json'), ('fits files', '.fits')],
-            initialdir=g.cpars['app_directory'])
+            defaultextension=".json",
+            filetypes=[("json files", ".json"), ("fits files", ".fits")],
+            initialdir=g.cpars["app_directory"],
+        )
         if not fname:
-            g.clog.warn('Aborted load from disk')
+            g.clog.warn("Aborted load from disk")
             return False
 
         # load json
-        if fname.endswith('.json'):
+        if fname.endswith(".json"):
             with open(fname) as ifname:
                 json_string = ifname.read()
         else:
             json_string = jsonFromFits(fname)
 
         # load up the instrument settings
         g.ipars.loadJSON(json_string)
 
         # load up the run parameters
         g.rpars.loadJSON(json_string)
 
+        # load the COMPO setup
+        g.compo_hw.loadJSON(json_string)
+
         return True
 
 
 class Save(w.ActButton):
     """
     Class defining the 'Save' button's operation. This saves the
     current configuration to disk.
     """
+
     def __init__(self, master, width):
         """
         master  : containing widget
         width   : width of button
         """
-        w.ActButton.__init__(self, master, width, text='Save')
+        w.ActButton.__init__(self, master, width, text="Save")
 
     @inlineCallbacks
     def act(self):
         """
         Carries out the action associated with the Save button
         """
         g = get_root(self).globals
-        g.clog.info('\nSaving current application to disk')
+        g.clog.info("\nSaving current application to disk")
 
         # check instrument parameters
         if not g.ipars.check():
-            g.clog.warn('Invalid instrument parameters; save failed.')
+            g.clog.warn("Invalid instrument parameters; save failed.")
             returnValue(False)
 
         # check run parameters
         rok, msg = g.rpars.check()
         if not rok:
-            g.clog.warn('Invalid run parameters; save failed.')
+            g.clog.warn("Invalid run parameters; save failed.")
             g.clog.warn(msg)
             returnValue(False)
 
         # Get data to save
         data = yield createJSON(g, full=False)
 
         # Save to disk
@@ -1829,20 +1953,21 @@
             returnValue(False)
 
 
 class Unfreeze(w.ActButton):
     """
     Class defining the 'Unfreeze' button's operation.
     """
+
     def __init__(self, master, width):
         """
         master  : containing widget
         width   : width of button
         """
-        w.ActButton.__init__(self, master, width, text='Unfreeze')
+        w.ActButton.__init__(self, master, width, text="Unfreeze")
 
     def act(self):
         """
         Carries out the action associated with the Unfreeze button
         """
         g = get_root(self).globals
         g.ipars.unfreeze()
@@ -1851,14 +1976,15 @@
         self.disable()
 
 
 class Observe(tk.LabelFrame):
     """
     Observe widget. Collects together all the buttons needed for observing.
     """
+
     def __init__(self, master):
         tk.LabelFrame.__init__(self, master, padx=10, pady=10)
 
         width = 10
         self.load = Load(self, width)
         self.save = Save(self, width)
         self.unfreeze = Unfreeze(self, width)
@@ -1877,28 +2003,26 @@
         # Define initial status
         self.start.disable()
         self.stop.disable()
         self.unfreeze.disable()
 
         # Implement expert level
         self.setExpertLevel()
-        self.telemetry_topics = [
-            ('hipercam.ngc.telemetry', self.on_telemetry)
-        ]
+        self.telemetry_topics = [("hipercam.ngc.telemetry", self.on_telemetry)]
 
     def on_telemetry(self, package):
         self.stop.on_telemetry(package)
         self.start.on_telemetry(package)
 
     def setExpertLevel(self):
         """
         Set expert level
         """
         g = get_root(self).globals
-        level = g.cpars['expert_level']
+        level = g.cpars["expert_level"]
 
         # now set whether buttons are permanently enabled or not
         if level == 0 or level == 1:
             self.load.setNonExpert()
             self.save.setNonExpert()
             self.unfreeze.setNonExpert()
             self.start.setNonExpert()
```

### Comparing `hcam_widgets-1.0.3/hcam_widgets/logs.py` & `hcam_widgets-1.1.0/hcam_widgets/logs.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.0.3/hcam_widgets/misc.py` & `hcam_widgets-1.1.0/hcam_widgets/misc.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.0.3/hcam_widgets/tcs.py` & `hcam_widgets-1.1.0/hcam_widgets/tcs.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.0.3/hcam_widgets/tkutils.py` & `hcam_widgets-1.1.0/hcam_widgets/tkutils.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.0.3/hcam_widgets/ucam.py` & `hcam_widgets-1.1.0/hcam_widgets/ucam.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.0.3/hcam_widgets/uspec.py` & `hcam_widgets-1.1.0/hcam_widgets/uspec.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.0.3/hcam_widgets/widgets.py` & `hcam_widgets-1.1.0/hcam_widgets/widgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # general purpose widgets
 from __future__ import print_function, unicode_literals, absolute_import, division
 from six.moves import urllib
+from functools import partial
 import time
 import socket
 from functools import reduce
 import numpy as np
 import six
 import pickle
 import subprocess
@@ -14,25 +15,34 @@
 from astropy import units as u
 from astropy.time import Time
 
 # twisted and async support
 from twisted.internet.defer import inlineCallbacks, returnValue
 from twisted.internet.task import LoopingCall
 
-from hcam_devices.gtc.headers import (create_gtc_header_table,
-                                      add_gtc_header_table_row)
+from hcam_devices.gtc.headers import create_gtc_header_table, add_gtc_header_table_row
 
 # internal
 from . import DriverError
 from .tkutils import get_root
 from .logs import Logger, GuiHandler
 from .astro import calc_riseset
-from .misc import (execCommand, checkSimbad, isOnline, isRunActive, stopNodding,
-                   getRunNumber, postJSON, insertFITSHDU,
-                   isPoweredOn, ReadNGCTelemetry, async_sleep)
+from .misc import (
+    execCommand,
+    checkSimbad,
+    isOnline,
+    isRunActive,
+    stopNodding,
+    getRunNumber,
+    postJSON,
+    insertFITSHDU,
+    isPoweredOn,
+    ReadNGCTelemetry,
+    async_sleep,
+)
 
 if not six.PY3:
     import Tkinter as tk
 else:
     import tkinter as tk
 
 
@@ -41,22 +51,23 @@
     """
     Defines an object representing one of the boolean configuration
     parameters to allow it to be interfaced with the menubar easily.
 
     If defined, callback is run with the new value of the flag as its
     argument
     """
+
     def __init__(self, master, flag, callback=None):
         tk.IntVar.__init__(self)
         self.master = master
         # get globals from root
         g = get_root(master).globals
 
         self.set(g.cpars[flag])
-        self.trace('w', self._update)
+        self.trace("w", self._update)
         self.flag = flag
         self.callback = callback
 
     def _update(self, *args):
         # get globals from root
         g = get_root(self.master).globals
         if self.get():
@@ -174,19 +185,19 @@
         try:
             int(self._value)
             return True
         except ValueError:
             return False
 
     def enable(self):
-        self.configure(state='normal')
+        self.configure(state="normal")
         self.set_bind()
 
     def disable(self):
-        self.configure(state='disable')
+        self.configure(state="disable")
         self.set_unbind()
 
     def on_key_release(self, *dummy):
         self.has_prev_key_release = None
         if self.checker:
             self.checker(dummy)
 
@@ -203,58 +214,58 @@
         if self.has_prev_key_release:
             # stop the key release callback being called yet
             self.after_cancel(self.has_prev_key_release)
             # set prev_key_release to None, so next key release will reactivate
             self.has_prev_key_release = None
         # increment the value
         increment = 1
-        if 'Shift' in keysym:
+        if "Shift" in keysym:
             increment = 10
-        elif 'Control' in keysym:
+        elif "Control" in keysym:
             increment = 100
-        if 'Up' in keysym:
+        if "Up" in keysym:
             self.add(increment)
-        elif 'Down' in keysym:
+        elif "Down" in keysym:
             self.sub(increment)
 
     def set_bind(self):
         """
         Sets key bindings.
         """
         # Arrow keys and enter
-        self.bind('<Up>', lambda e: self.on_key_press_repeat('Up'))
-        self.bind('<Down>', lambda e: self.on_key_press_repeat('Down'))
-        self.bind('<Shift-Up>', lambda e: self.on_key_press_repeat('Shift-Up'))
-        self.bind('<Shift-Down>', lambda e: self.on_key_press_repeat('Shift-Down'))
-        self.bind('<Control-Up>', lambda e: self.on_key_press_repeat('Control-Up'))
-        self.bind('<Control-Down>', lambda e: self.on_key_press_repeat('Control-Down'))
-        self.bind('<KeyRelease>', lambda e: self.on_key_release_repeat())
+        self.bind("<Up>", lambda e: self.on_key_press_repeat("Up"))
+        self.bind("<Down>", lambda e: self.on_key_press_repeat("Down"))
+        self.bind("<Shift-Up>", lambda e: self.on_key_press_repeat("Shift-Up"))
+        self.bind("<Shift-Down>", lambda e: self.on_key_press_repeat("Shift-Down"))
+        self.bind("<Control-Up>", lambda e: self.on_key_press_repeat("Control-Up"))
+        self.bind("<Control-Down>", lambda e: self.on_key_press_repeat("Control-Down"))
+        self.bind("<KeyRelease>", lambda e: self.on_key_release_repeat())
 
         # Mouse buttons: bit complex since they don't automatically
         # run in continuous mode like the arrow keys
-        self.bind('<ButtonPress-1>', self._leftMouseDown)
-        self.bind('<ButtonRelease-1>', self._leftMouseUp)
-        self.bind('<Shift-ButtonPress-1>', self._shiftLeftMouseDown)
-        self.bind('<Shift-ButtonRelease-1>', self._shiftLeftMouseUp)
-        self.bind('<Control-Button-1>', lambda e: self.add(100))
-
-        self.bind('<ButtonPress-3>', self._rightMouseDown)
-        self.bind('<ButtonRelease-3>', self._rightMouseUp)
-        self.bind('<Shift-ButtonPress-3>', self._shiftRightMouseDown)
-        self.bind('<Shift-ButtonRelease-3>', self._shiftRightMouseUp)
-        self.bind('<Control-Button-3>', lambda e: self.sub(100))
-
-        self.bind('<Double-Button-1>', self._dadd1)
-        self.bind('<Double-Button-3>', self._dsub1)
-        self.bind('<Shift-Double-Button-1>', self._dadd10)
-        self.bind('<Shift-Double-Button-3>', self._dsub10)
-        self.bind('<Control-Double-Button-1>', self._dadd100)
-        self.bind('<Control-Double-Button-3>', self._dsub100)
+        self.bind("<ButtonPress-1>", self._leftMouseDown)
+        self.bind("<ButtonRelease-1>", self._leftMouseUp)
+        self.bind("<Shift-ButtonPress-1>", self._shiftLeftMouseDown)
+        self.bind("<Shift-ButtonRelease-1>", self._shiftLeftMouseUp)
+        self.bind("<Control-Button-1>", lambda e: self.add(100))
+
+        self.bind("<ButtonPress-3>", self._rightMouseDown)
+        self.bind("<ButtonRelease-3>", self._rightMouseUp)
+        self.bind("<Shift-ButtonPress-3>", self._shiftRightMouseDown)
+        self.bind("<Shift-ButtonRelease-3>", self._shiftRightMouseUp)
+        self.bind("<Control-Button-3>", lambda e: self.sub(100))
+
+        self.bind("<Double-Button-1>", self._dadd1)
+        self.bind("<Double-Button-3>", self._dsub1)
+        self.bind("<Shift-Double-Button-1>", self._dadd10)
+        self.bind("<Shift-Double-Button-3>", self._dsub10)
+        self.bind("<Control-Double-Button-1>", self._dadd100)
+        self.bind("<Control-Double-Button-3>", self._dsub100)
 
-        self.bind('<Enter>', self._enter)
+        self.bind("<Enter>", self._enter)
 
     def _leftMouseDown(self, event):
         self._leftMousePressed = True
         self._mouseJustPressed = True
         self._pollMouse()
 
     def _leftMouseUp(self, event):
@@ -327,36 +338,36 @@
             self.sub(10)
             self.after_id = self.after(delay, self._pollMouse)
 
     def set_unbind(self):
         """
         Unsets key bindings.
         """
-        self.unbind('<Up>')
-        self.unbind('<Down>')
-        self.unbind('<Shift-Up>')
-        self.unbind('<Shift-Down>')
-        self.unbind('<Control-Up>')
-        self.unbind('<Control-Down>')
-
-        self.unbind('<Shift-Button-1>')
-        self.unbind('<Shift-Button-3>')
-        self.unbind('<Control-Button-1>')
-        self.unbind('<Control-Button-3>')
-        self.unbind('<ButtonPress-1>')
-        self.unbind('<ButtonRelease-1>')
-        self.unbind('<ButtonPress-3>')
-        self.unbind('<ButtonRelease-3>')
-        self.unbind('<Double-Button-1>')
-        self.unbind('<Double-Button-3>')
-        self.unbind('<Shift-Double-Button-1>')
-        self.unbind('<shiftDouble-Button-3>')
-        self.unbind('<Control-Double-Button-1>')
-        self.unbind('<Control-Double-Button-3>')
-        self.unbind('<Enter>')
+        self.unbind("<Up>")
+        self.unbind("<Down>")
+        self.unbind("<Shift-Up>")
+        self.unbind("<Shift-Down>")
+        self.unbind("<Control-Up>")
+        self.unbind("<Control-Down>")
+
+        self.unbind("<Shift-Button-1>")
+        self.unbind("<Shift-Button-3>")
+        self.unbind("<Control-Button-1>")
+        self.unbind("<Control-Button-3>")
+        self.unbind("<ButtonPress-1>")
+        self.unbind("<ButtonRelease-1>")
+        self.unbind("<ButtonPress-3>")
+        self.unbind("<ButtonRelease-3>")
+        self.unbind("<Double-Button-1>")
+        self.unbind("<Double-Button-3>")
+        self.unbind("<Shift-Double-Button-1>")
+        self.unbind("<shiftDouble-Button-3>")
+        self.unbind("<Control-Double-Button-1>")
+        self.unbind("<Control-Double-Button-3>")
+        self.unbind("<Enter>")
 
     def _callback(self, *dummy):
         """
         This gets called on any attempt to change the value
         """
         # retrieve the value from the Entry
         value = self._variable.get()
@@ -377,60 +388,60 @@
         else:
             # Store new value
             self._value = value
 
     # following are callbacks for bindings
     def _dadd1(self, event):
         self.add(1)
-        return 'break'
+        return "break"
 
     def _dsub1(self, event):
         self.sub(1)
-        return 'break'
+        return "break"
 
     def _dadd10(self, event):
         self.add(10)
-        return 'break'
+        return "break"
 
     def _dsub10(self, event):
         self.sub(10)
-        return 'break'
+        return "break"
 
     def _dadd100(self, event):
         self.add(100)
-        return 'break'
+        return "break"
 
     def _dsub100(self, event):
         self.sub(100)
-        return 'break'
+        return "break"
 
     def _enter(self, event):
         self.focus()
         self.icursor(tk.END)
 
 
-class PosInt (IntegerEntry):
+class PosInt(IntegerEntry):
     """
     Provide positive or 0 integer input. Basically
     an IntegerEntry with one or two extras.
     """
 
     def set_bind(self):
         """
         Sets key bindings -- we need this more than once
         """
         IntegerEntry.set_bind(self)
-        self.bind('<Next>', lambda e: self.set(0))
+        self.bind("<Next>", lambda e: self.set(0))
 
     def set_unbind(self):
         """
         Unsets key bindings -- we need this more than once
         """
         IntegerEntry.set_unbind(self)
-        self.unbind('<Next>')
+        self.unbind("<Next>")
 
     def validate(self, value):
         """
         Applies the validation criteria.
         Returns value, new value, or None if invalid.
 
         Overload this in derived classes.
@@ -479,14 +490,15 @@
             return False
 
 
 class RangedInt(IntegerEntry):
     """
     Provides range-checked integer input.
     """
+
     def __init__(self, master, ival, imin, imax, checker, blank, **kw):
         """
         master  -- enclosing widget
         ival    -- initial integer value
         imin    -- minimum value
         imax    -- maximum value
         checker -- command that is run on any change to the entry
@@ -495,32 +507,32 @@
                    a blank field is allowed, even if it is technically
                    invalid.
         kw      -- keyword arguments
         """
         self.imin = imin
         self.imax = imax
         IntegerEntry.__init__(self, master, ival, checker, blank, **kw)
-        self.bind('<Next>', lambda e: self.set(self.imin))
-        self.bind('<Prior>', lambda e: self.set(self.imax))
+        self.bind("<Next>", lambda e: self.set(self.imin))
+        self.bind("<Prior>", lambda e: self.set(self.imax))
 
     def set_bind(self):
         """
         Sets key bindings -- we need this more than once
         """
         IntegerEntry.set_bind(self)
-        self.bind('<Next>', lambda e: self.set(self.imin))
-        self.bind('<Prior>', lambda e: self.set(self.imax))
+        self.bind("<Next>", lambda e: self.set(self.imin))
+        self.bind("<Prior>", lambda e: self.set(self.imax))
 
     def set_unbind(self):
         """
         Unsets key bindings -- we need this more than once
         """
         IntegerEntry.set_unbind(self)
-        self.unbind('<Next>')
-        self.unbind('<Prior>')
+        self.unbind("<Next>")
+        self.unbind("<Prior>")
 
     def validate(self, value):
         """
         Applies the validation criteria.
         Returns value, new value, or None if invalid.
 
         Overload this in derived classes.
@@ -576,55 +588,54 @@
 
     def __init__(self, master, ival, imin, imax, mfac, checker, blank, **kw):
         """
         mfac must be class that support 'value()' to return an integer value.
         to allow it to be updated
         """
         self.mfac = mfac
-        RangedInt.__init__(self, master, ival, imin,
-                           imax, checker, blank, **kw)
-        self.unbind('<Next>')
-        self.unbind('<Prior>')
-        self.bind('<Next>', lambda e: self.set(self._min()))
-        self.bind('<Prior>', lambda e: self.set(self._max()))
+        RangedInt.__init__(self, master, ival, imin, imax, checker, blank, **kw)
+        self.unbind("<Next>")
+        self.unbind("<Prior>")
+        self.bind("<Next>", lambda e: self.set(self._min()))
+        self.bind("<Prior>", lambda e: self.set(self._max()))
 
     def set_bind(self):
         """
         Sets key bindings -- we need this more than once
         """
         RangedInt.set_bind(self)
-        self.unbind('<Next>')
-        self.unbind('<Prior>')
-        self.bind('<Next>', lambda e: self.set(self._min()))
-        self.bind('<Prior>', lambda e: self.set(self._max()))
+        self.unbind("<Next>")
+        self.unbind("<Prior>")
+        self.bind("<Next>", lambda e: self.set(self._min()))
+        self.bind("<Prior>", lambda e: self.set(self._max()))
 
     def set_unbind(self):
         """
         Sets key bindings -- we need this more than once
         """
         RangedInt.set_unbind(self)
-        self.unbind('<Next>')
-        self.unbind('<Prior>')
+        self.unbind("<Next>")
+        self.unbind("<Prior>")
 
     def add(self, num):
         """
         Adds num to the current value, jumping up the next
         multiple of mfac if the result is not a multiple already
         """
         try:
             val = self.value() + num
         except Exception:
             val = num
 
         chunk = self.mfac.value()
         if val % chunk > 0:
             if num > 0:
-                val = chunk*(val // chunk + 1)
+                val = chunk * (val // chunk + 1)
             elif num < 0:
-                val = chunk*(val // chunk)
+                val = chunk * (val // chunk)
 
         val = max(self._min(), min(self._max(), val))
         self.set(val)
 
     def sub(self, num):
         """
         Subtracts num from the current value, forcing the result to be within
@@ -634,17 +645,17 @@
             val = self.value() - num
         except Exception:
             val = -num
 
         chunk = self.mfac.value()
         if val % chunk > 0:
             if num > 0:
-                val = chunk*(val // chunk)
+                val = chunk * (val // chunk)
             elif num < 0:
-                val = chunk*(val // chunk + 1)
+                val = chunk * (val // chunk + 1)
 
         val = max(self._min(), min(self._max(), val))
         self.set(val)
 
     def ok(self):
         """
         Returns True if OK to use, else False
@@ -670,71 +681,76 @@
 
 
 class ListInt(IntegerEntry):
     """
     Provides integer input allowing only a finite list of integers.
     Needed for the binning factors.
     """
+
     def __init__(self, master, ival, allowed, checker, **kw):
         """
         master  -- enclosing widget
         ival    -- initial integer value
         allowed -- list of allowed values. Will be checked for uniqueness
         checker -- command that is run on any change to the entry
         kw      -- keyword arguments
         """
         if ival not in allowed:
-            raise DriverError('utils.widgets.ListInt: value = ' + str(ival) +
-                              ' not in list of allowed values.')
+            raise DriverError(
+                "utils.widgets.ListInt: value = "
+                + str(ival)
+                + " not in list of allowed values."
+            )
         if len(set(allowed)) != len(allowed):
-            raise DriverError('utils.widgets.ListInt: not all values unique' +
-                              ' in allowed list.')
+            raise DriverError(
+                "utils.widgets.ListInt: not all values unique" + " in allowed list."
+            )
 
         # we need to maintain an index of which integer has been selected
         self.allowed = allowed
         self.index = allowed.index(ival)
         IntegerEntry.__init__(self, master, ival, checker, False, **kw)
         self.set_bind()
 
     def set_bind(self):
         """
         Sets key bindings -- we need this more than once
         """
         IntegerEntry.set_bind(self)
-        self.unbind('<Shift-Up>')
-        self.unbind('<Shift-Down>')
-        self.unbind('<Control-Up>')
-        self.unbind('<Control-Down>')
-        self.unbind('<Double-Button-1>')
-        self.unbind('<Double-Button-3>')
-        self.unbind('<Shift-Button-1>')
-        self.unbind('<Shift-Button-3>')
-        self.unbind('<Control-Button-1>')
-        self.unbind('<Control-Button-3>')
-
-        self.bind('<Button-1>', lambda e: self.add(1))
-        self.bind('<Button-3>', lambda e: self.sub(1))
-        self.bind('<Up>', lambda e: self.add(1))
-        self.bind('<Down>', lambda e: self.sub(1))
-        self.bind('<Enter>', self._enter)
-        self.bind('<Next>', lambda e: self.set(self.allowed[0]))
-        self.bind('<Prior>', lambda e: self.set(self.allowed[-1]))
+        self.unbind("<Shift-Up>")
+        self.unbind("<Shift-Down>")
+        self.unbind("<Control-Up>")
+        self.unbind("<Control-Down>")
+        self.unbind("<Double-Button-1>")
+        self.unbind("<Double-Button-3>")
+        self.unbind("<Shift-Button-1>")
+        self.unbind("<Shift-Button-3>")
+        self.unbind("<Control-Button-1>")
+        self.unbind("<Control-Button-3>")
+
+        self.bind("<Button-1>", lambda e: self.add(1))
+        self.bind("<Button-3>", lambda e: self.sub(1))
+        self.bind("<Up>", lambda e: self.add(1))
+        self.bind("<Down>", lambda e: self.sub(1))
+        self.bind("<Enter>", self._enter)
+        self.bind("<Next>", lambda e: self.set(self.allowed[0]))
+        self.bind("<Prior>", lambda e: self.set(self.allowed[-1]))
 
     def set_unbind(self):
         """
         Unsets key bindings -- we need this more than once
         """
         IntegerEntry.set_unbind(self)
-        self.unbind('<Button-1>')
-        self.unbind('<Button-3>')
-        self.unbind('<Up>')
-        self.unbind('<Down>')
-        self.unbind('<Enter>')
-        self.unbind('<Next>')
-        self.unbind('<Prior>')
+        self.unbind("<Button-1>")
+        self.unbind("<Button-3>")
+        self.unbind("<Up>")
+        self.unbind("<Down>")
+        self.unbind("<Enter>")
+        self.unbind("<Next>")
+        self.unbind("<Prior>")
 
     def validate(self, value):
         """
         Applies the validation criteria.
         Returns value, new value, or None if invalid.
 
         Overload this in derived classes.
@@ -755,22 +771,22 @@
             self.index = self.allowed.index(num)
         IntegerEntry.set(self, num)
 
     def add(self, num):
         """
         Adds num to the current value
         """
-        self.index = max(0, min(len(self.allowed)-1, self.index+num))
+        self.index = max(0, min(len(self.allowed) - 1, self.index + num))
         self.set(self.allowed[self.index])
 
     def sub(self, num):
         """
         Subtracts num from the current value
         """
-        self.index = max(0, min(len(self.allowed)-1, self.index-num))
+        self.index = max(0, min(len(self.allowed) - 1, self.index - num))
         self.set(self.allowed[self.index])
 
     def ok(self):
         """
         Returns True if OK to use, else False
         """
         return True
@@ -792,15 +808,15 @@
                    invalid (the latter case requires some other checking)
         kw      -- optional keyword arguments that can be used for
                    an Entry. If 'nplaces' argument is set, precision
                    of FloatEntry will be limited to nplaces decimal places.
         """
         # important to set the value of _variable before tracing it
         # to avoid immediate run of _callback.
-        np = kw.pop('nplaces', 8)
+        np = kw.pop("nplaces", 8)
         tk.Entry.__init__(self, master, **kw)
         self._variable = tk.StringVar()
         self.nplaces = np
         self._value = str(round(float(fval), self.nplaces))
         self._variable.set(self._value)
         self._variable.trace("w", self._callback)
         self.config(textvariable=self._variable)
@@ -866,60 +882,60 @@
         try:
             float(self._value)
             return True
         except Exception:
             return False
 
     def enable(self):
-        self.configure(state='normal')
+        self.configure(state="normal")
         self.set_bind()
 
     def disable(self):
-        self.configure(state='disable')
+        self.configure(state="disable")
         self.set_unbind()
 
     def set_bind(self):
         """
         Sets key bindings.
         """
-        self.bind('<Button-1>', lambda e: self.add(0.1))
-        self.bind('<Button-3>', lambda e: self.sub(0.1))
-        self.bind('<Up>', lambda e: self.add(0.1))
-        self.bind('<Down>', lambda e: self.sub(0.1))
-        self.bind('<Shift-Up>', lambda e: self.add(1))
-        self.bind('<Shift-Down>', lambda e: self.sub(1))
-        self.bind('<Control-Up>', lambda e: self.add(10))
-        self.bind('<Control-Down>', lambda e: self.sub(10))
-        self.bind('<Double-Button-1>', self._dadd)
-        self.bind('<Double-Button-3>', self._dsub)
-        self.bind('<Shift-Button-1>', lambda e: self.add(1))
-        self.bind('<Shift-Button-3>', lambda e: self.sub(1))
-        self.bind('<Control-Button-1>', lambda e: self.add(10))
-        self.bind('<Control-Button-3>', lambda e: self.sub(10))
-        self.bind('<Enter>', self._enter)
+        self.bind("<Button-1>", lambda e: self.add(0.1))
+        self.bind("<Button-3>", lambda e: self.sub(0.1))
+        self.bind("<Up>", lambda e: self.add(0.1))
+        self.bind("<Down>", lambda e: self.sub(0.1))
+        self.bind("<Shift-Up>", lambda e: self.add(1))
+        self.bind("<Shift-Down>", lambda e: self.sub(1))
+        self.bind("<Control-Up>", lambda e: self.add(10))
+        self.bind("<Control-Down>", lambda e: self.sub(10))
+        self.bind("<Double-Button-1>", self._dadd)
+        self.bind("<Double-Button-3>", self._dsub)
+        self.bind("<Shift-Button-1>", lambda e: self.add(1))
+        self.bind("<Shift-Button-3>", lambda e: self.sub(1))
+        self.bind("<Control-Button-1>", lambda e: self.add(10))
+        self.bind("<Control-Button-3>", lambda e: self.sub(10))
+        self.bind("<Enter>", self._enter)
 
     def set_unbind(self):
         """
         Unsets key bindings.
         """
-        self.unbind('<Button-1>')
-        self.unbind('<Button-3>')
-        self.unbind('<Up>')
-        self.unbind('<Down>')
-        self.unbind('<Shift-Up>')
-        self.unbind('<Shift-Down>')
-        self.unbind('<Control-Up>')
-        self.unbind('<Control-Down>')
-        self.unbind('<Double-Button-1>')
-        self.unbind('<Double-Button-3>')
-        self.unbind('<Shift-Button-1>')
-        self.unbind('<Shift-Button-3>')
-        self.unbind('<Control-Button-1>')
-        self.unbind('<Control-Button-3>')
-        self.unbind('<Enter>')
+        self.unbind("<Button-1>")
+        self.unbind("<Button-3>")
+        self.unbind("<Up>")
+        self.unbind("<Down>")
+        self.unbind("<Shift-Up>")
+        self.unbind("<Shift-Down>")
+        self.unbind("<Control-Up>")
+        self.unbind("<Control-Down>")
+        self.unbind("<Double-Button-1>")
+        self.unbind("<Double-Button-3>")
+        self.unbind("<Shift-Button-1>")
+        self.unbind("<Shift-Button-3>")
+        self.unbind("<Control-Button-1>")
+        self.unbind("<Control-Button-3>")
+        self.unbind("<Enter>")
 
     def _callback(self, *dummy):
         """
         This gets called on any attempt to change the value
         """
         # retrieve the value from the Entry
         value = self._variable.get()
@@ -944,31 +960,31 @@
             self._value = value
             if self.checker:
                 self.checker(*dummy)
 
     # following are callbacks for bindings
     def _dadd(self, event):
         self.add(0.1)
-        return 'break'
+        return "break"
 
     def _dsub(self, event):
         self.sub(0.1)
-        return 'break'
+        return "break"
 
     def _enter(self, event):
         self.focus()
         self.icursor(tk.END)
 
 
 class RangedFloat(FloatEntry):
     """
     Provides range-checked float input.
     """
-    def __init__(self, master, fval, fmin, fmax, checker,
-                 blank, allowzero=False, **kw):
+
+    def __init__(self, master, fval, fmin, fmax, checker, blank, allowzero=False, **kw):
         """
         master    -- enclosing widget
         fval      -- initial float value
         fmin      -- minimum value
         fmax      -- maximum value
         checker   -- command that is run on any change to the entry
         blank     -- controls whether the field is allowed to be
@@ -979,47 +995,50 @@
                      can be difficult unless 0 is allowed even though it is
                      an invalid value.
         kw        -- keyword arguments
         """
         self.fmin = fmin
         self.fmax = fmax
         FloatEntry.__init__(self, master, fval, checker, blank, **kw)
-        self.bind('<Next>', lambda e: self.set(self.fmin))
-        self.bind('<Prior>', lambda e: self.set(self.fmax))
+        self.bind("<Next>", lambda e: self.set(self.fmin))
+        self.bind("<Prior>", lambda e: self.set(self.fmax))
         self.allowzero = allowzero
 
     def set_bind(self):
         """
         Sets key bindings -- we need this more than once
         """
         FloatEntry.set_bind(self)
-        self.bind('<Next>', lambda e: self.set(self.fmin))
-        self.bind('<Prior>', lambda e: self.set(self.fmax))
+        self.bind("<Next>", lambda e: self.set(self.fmin))
+        self.bind("<Prior>", lambda e: self.set(self.fmax))
 
     def set_unbind(self):
         """
         Unsets key bindings -- we need this more than once
         """
         FloatEntry.set_unbind(self)
-        self.unbind('<Next>')
-        self.unbind('<Prior>')
+        self.unbind("<Next>")
+        self.unbind("<Prior>")
 
     def validate(self, value):
         """
         Applies the validation criteria.
         Returns value, new value, or None if invalid.
 
         Overload this in derived classes.
         """
         try:
             # trap blank fields here
             if not self.blank or value:
                 v = float(value)
-                if (self.allowzero and v != 0 and v < self.fmin) or \
-                        (not self.allowzero and v < self.fmin) or v > self.fmax:
+                if (
+                    (self.allowzero and v != 0 and v < self.fmin)
+                    or (not self.allowzero and v < self.fmin)
+                    or v > self.fmax
+                ):
                     return None
             return value
         except ValueError:
             return None
 
     def add(self, num):
         """
@@ -1057,56 +1076,53 @@
 
 class TextEntry(tk.Entry):
     """
     Sub-class of Entry for basic text input. Not a lot to
     it but it keeps things neater and it has a check for
     blank entries.
     """
+
     def __init__(self, master, width, callback=None):
         """
         master  : the widget this gets placed inside
-        """        # Define a StringVar, connect it to the callback, if there is one
+        """  # Define a StringVar, connect it to the callback, if there is one
         self.val = tk.StringVar()
         if callback is not None:
-            self.val.trace('w', callback)
-        tk.Entry.__init__(
-            self,
-            master,
-            textvariable=self.val,
-            width=width
-        )
+            self.val.trace("w", callback)
+        tk.Entry.__init__(self, master, textvariable=self.val, width=width)
         # get globals
         g = get_root(self).globals
-        self.config(fg=g.COL['text'], bg=g.COL['main'])
+        self.config(fg=g.COL["text"], bg=g.COL["main"])
         # Control input behaviour.
-        self.bind('<Enter>', lambda e: self.focus())
+        self.bind("<Enter>", lambda e: self.focus())
 
     def value(self):
         """
         Returns value.
         """
         return self.val.get()
 
     def set(self, text):
         """
         Returns value.
         """
         return self.val.set(text)
 
     def ok(self):
-        if self.value() == '' or self.value().isspace():
+        if self.value() == "" or self.value().isspace():
             return False
         else:
             return True
 
 
 class Choice(tk.OptionMenu):
     """
     Menu choice class.
     """
+
     def __init__(self, master, options, initial=None, width=0, checker=None):
         """
         master  : containing widget
         options : list of strings
         initial : the initial one to select. If None will default to the first.
         width   : minimum character width to use. Width set will be large
                   enough for longest option.
@@ -1120,28 +1136,38 @@
             self.val.set(initial)
         tk.OptionMenu.__init__(self, master, self.val, *options)
         width = max(width, reduce(max, [len(s) for s in options]))
         g = get_root(self).globals
         self.config(width=width, font=g.ENTRY_FONT)
         self.checker = checker
         if self.checker is not None:
-            self.val.trace('w', self.checker)
+            self.val.trace("w", self.checker)
         self.options = options
 
+    def update(self, new_options):
+        """
+        Update option list with new options
+        """
+        menu = self["menu"]
+        # clear the menu
+        menu.delete(0, "end")
+        for option in new_options:
+            menu.add_command(label=option, command=partial(self.val.set, option))
+
     def value(self):
         return self.val.get()
 
     def set(self, choice):
         return self.val.set(choice)
 
     def disable(self):
-        self.configure(state='disable')
+        self.configure(state="disable")
 
     def enable(self):
-        self.configure(state='normal')
+        self.configure(state="normal")
 
     def getIndex(self):
         """
         Returns the index of the selected choice,
         Throws a ValueError if the set value is not
         one of the options.
         """
@@ -1149,225 +1175,248 @@
 
 
 class Expose(RangedFloat):
     """
     Special entry field for exposure times designed to return
     an integer number of 0.01ms increments.
     """
+
     def __init__(self, master, fval, fmin, fmax, checker, **kw):
         """
         master  -- enclosing widget
         fval    -- initial value, seconds
         fmin    -- minimum value, seconds
         fmax    -- maximum value, seconds
         checker -- command that is run on any change to the entry
 
         fval, fmin and fmax must be multiples of 0.00001
         """
-        if abs(round(100000*fval)-100000*fval) > 1.e-12:
+        if abs(round(100000 * fval) - 100000 * fval) > 1.0e-12:
             raise DriverError(
-                'utils.widgets.Expose.__init__: fval must be a multiple of 0.00001')
-        if abs(round(100000*fmin)-100000*fmin) > 1.e-12:
+                "utils.widgets.Expose.__init__: fval must be a multiple of 0.00001"
+            )
+        if abs(round(100000 * fmin) - 100000 * fmin) > 1.0e-12:
             raise DriverError(
-                'utils.widgets.Expose.__init__: fmin must be a multiple of 0.00001')
-        if abs(round(100000*fmax)-100000*fmax) > 1.e-12:
+                "utils.widgets.Expose.__init__: fmin must be a multiple of 0.00001"
+            )
+        if abs(round(100000 * fmax) - 100000 * fmax) > 1.0e-12:
             raise DriverError(
-                'utils.widgets.Expose.__init__: fmax must be a multiple of 0.00001')
-        kw['nplaces'] = 5
+                "utils.widgets.Expose.__init__: fmax must be a multiple of 0.00001"
+            )
+        kw["nplaces"] = 5
         RangedFloat.__init__(self, master, fval, fmin, fmax, checker, True, **kw)
 
     def validate(self, value):
         """
         This prevents setting any value more precise than 0.00001
         """
         try:
             # trap blank fields here
             if value:
                 v = float(value)
                 if (v != 0 and v < self.fmin) or v > self.fmax:
                     return None
-                if abs(round(100000*v)-100000*v) > 1.e-12:
+                if abs(round(100000 * v) - 100000 * v) > 1.0e-12:
                     return None
             return value
         except ValueError:
             return None
 
     def ivalue(self):
         """
         Returns integer value in units of 0.01ms, if possible, None if not.
         """
         try:
-            return int(round(100000*float(self._value)))
+            return int(round(100000 * float(self._value)))
         except Exception:
             return None
 
     def set_min(self, fmin):
         """
         Updates minimum value
         """
-        if round(100000*fmin) != 100000*fmin:
-            raise DriverError('utils.widgets.Expose.set_min: ' +
-                              'fmin must be a multiple of 0.00001')
+        if round(100000 * fmin) != 100000 * fmin:
+            raise DriverError(
+                "utils.widgets.Expose.set_min: " + "fmin must be a multiple of 0.00001"
+            )
         self.fmin = fmin
         self.set(self.fmin)
 
 
 class Radio(tk.Frame):
     """
     Left-to-right radio button class. Lays out buttons in a grid
     from left-to-right. Has a max number of columns after which it
     will jump to left of next row and start over.
     """
-    def __init__(self, master, options, ncmax, checker=None,
-                 values=None, initial=0):
+
+    def __init__(self, master, options, ncmax, checker=None, values=None, initial=0):
         """
         master : containing widget
         options : array of option strings, in order. These are the choices
         presented to the user.
         ncmax : max number of columns (flows onto next row if need be)
         checker : callback to be run after any change
         values : array of string values used by the code internally.
         If 'None', the value from 'options' will be used.
         initial : index of initial value to set.
         """
         tk.Frame.__init__(self, master)
         # get globals from root widget
         g = get_root(self).globals
         if values is not None and len(values) != len(options):
-            raise DriverError('utils.widgets.Radio.__init__: values and ' +
-                              'options must have same length')
+            raise DriverError(
+                "utils.widgets.Radio.__init__: values and "
+                + "options must have same length"
+            )
 
         self.val = tk.StringVar()
         if values is None:
             self.val.set(options[initial])
         else:
             self.val.set(values[initial])
 
         row = 0
         col = 0
         self.buttons = []
         for nopt, option in enumerate(options):
             if values is None:
                 self.buttons.append(
-                    tk.Radiobutton(self, text=option, variable=self.val,
-                                   font=g.ENTRY_FONT, value=option))
+                    tk.Radiobutton(
+                        self,
+                        text=option,
+                        variable=self.val,
+                        font=g.ENTRY_FONT,
+                        value=option,
+                    )
+                )
                 self.buttons[-1].grid(row=row, column=col, sticky=tk.W)
             else:
                 self.buttons.append(
-                    tk.Radiobutton(self, text=option, variable=self.val,
-                                   font=g.ENTRY_FONT, value=values[nopt]))
+                    tk.Radiobutton(
+                        self,
+                        text=option,
+                        variable=self.val,
+                        font=g.ENTRY_FONT,
+                        value=values[nopt],
+                    )
+                )
                 self.buttons[-1].grid(row=row, column=col, sticky=tk.W)
             col += 1
             if col == ncmax:
                 row += 1
                 col = 0
 
         self.checker = checker
         if self.checker is not None:
-            self.val.trace('w', self.checker)
+            self.val.trace("w", self.checker)
         self.options = options
 
     def value(self):
         return self.val.get()
 
     def set(self, choice):
         self.val.set(choice)
 
     def disable(self):
         for b in self.buttons:
-            b.configure(state='disable')
+            b.configure(state="disable")
 
     def enable(self):
         for b in self.buttons:
-            b.configure(state='normal')
+            b.configure(state="normal")
 
     def getIndex(self):
         """
         Returns the index of the selected choice,
         Throws a ValueError if the set value is not
         one of the options.
         """
         return self.options.index(self.val.get())
 
 
 class OnOff(tk.Checkbutton):
     """
     On or Off choice
     """
+
     def __init__(self, master, value, checker=None):
         self.val = tk.IntVar()
         self.val.set(value)
-        tk.Checkbutton.__init__(self, master, variable=self.val,
-                                command=checker)
+        tk.Checkbutton.__init__(self, master, variable=self.val, command=checker)
 
     def __call__(self):
         return self.val.get()
 
     def disable(self):
-        self.configure(state='disable')
+        self.configure(state="disable")
 
     def enable(self):
-        self.configure(state='normal')
+        self.configure(state="normal")
 
     def set(self, state):
         self.val.set(state)
 
 
 class Select(tk.OptionMenu):
     """
     Dropdown box menu for selection
     """
+
     def __init__(self, master, initial_index, options, checker=None):
         self.val = tk.StringVar()
         self.options = options
         self.val.set(options[initial_index])
-        tk.OptionMenu.__init__(self, master, self.val, *options,
-                               command=checker)
+        tk.OptionMenu.__init__(self, master, self.val, *options, command=checker)
 
     def __call__(self):
         return self.val.get()
 
     def disable(self):
-        self.configure(state='disable')
+        self.configure(state="disable")
 
     def enable(self):
-        self.configure(state='normal')
+        self.configure(state="normal")
 
     def set(self, value):
         if value not in self.options:
-            raise ValueError('{0} not one of the possible options: {1!r}'.format(
-                value, self.options
-            ))
+            raise ValueError(
+                "{0} not one of the possible options: {1!r}".format(value, self.options)
+            )
         self.val.set(value)
 
 
 class GuiLogger(Logger, tk.Frame):
     """
     Defines a GUI logger, a combination of Logger and a Frame
 
      logname : unique name for logger
      root    : the root widget the LabelFrame descends from
      height  : height in pixels
      width   : width in pixels
 
     """
-    def __init__(self, logname, root, height, width):
 
+    def __init__(self, logname, root, height, width):
         # configure the Logger
         Logger.__init__(self, logname)
 
         # configure the LabelFrame
         tk.Frame.__init__(self, root)
 
         g = get_root(self).globals
         scrollbar = tk.Scrollbar(self)
         scrollbar.pack(side=tk.RIGHT, fill=tk.Y)
         twidget = tk.Text(
-            self, height=height, width=width, bg=g.COL['log'],
-            yscrollcommand=scrollbar.set)
+            self,
+            height=height,
+            width=width,
+            bg=g.COL["log"],
+            yscrollcommand=scrollbar.set,
+        )
         twidget.configure(state=tk.DISABLED)
         twidget.pack(side=tk.LEFT)
         scrollbar.config(command=twidget.yview)
 
         # create and add a handler for the GUI
         self._log.addHandler(GuiHandler(twidget))
 
@@ -1381,27 +1430,30 @@
      height  : height in pixels
      width   : width in pixels
      label   : label for the LabelFrame
 
     """
 
     def __init__(self, logname, root, height, width, label):
-
         # configure the Logger
         Logger.__init__(self, logname)
 
         # configure the LabelFrame
         tk.LabelFrame.__init__(self, root, text=label)
 
         g = get_root(self).globals
         scrollbar = tk.Scrollbar(self)
         scrollbar.pack(side=tk.RIGHT, fill=tk.Y)
         twidget = tk.Text(
-            self, height=height, width=width, bg=g.COL['log'],
-            yscrollcommand=scrollbar.set)
+            self,
+            height=height,
+            width=width,
+            bg=g.COL["log"],
+            yscrollcommand=scrollbar.set,
+        )
         twidget.configure(state=tk.DISABLED)
         twidget.pack(side=tk.LEFT)
         scrollbar.config(command=twidget.yview)
 
         # create and add a handler for the GUI
         self._log.addHandler(GuiHandler(twidget))
 
@@ -1421,48 +1473,49 @@
         """
         master   : containing widget
         width    : width in characters of the button
         callback : function that is called when button is pressed
         bg       : background colour
         kwargs   : keyword arguments
         """
-        tk.Button.__init__(self, master, fg='black', width=width,
-                           command=self.act, **kwargs)
+        tk.Button.__init__(
+            self, master, fg="black", width=width, command=self.act, **kwargs
+        )
 
         # store some attributes. other anc calbback are obvious.
         # _active indicates whether the button should be enabled or disabled
         # _expert indicates whether the activity state should be overridden so
         #         that the button is enabled in any case (if set True)
         self.callback = callback
         self._active = True
         self._expert = False
 
     def enable(self):
         """
         Enable the button, set its activity flag.
         """
-        self.config(state='normal')
+        self.config(state="normal")
         self._active = True
 
     def disable(self):
         """
         Disable the button, if in non-expert mode;
         unset its activity flag come-what-may.
         """
         if not self._expert:
-            self.config(state='disable')
+            self.config(state="disable")
         self._active = False
 
     def setExpert(self):
         """
         Turns on 'expert' status whereby the button is always enabled,
         regardless of its activity status.
         """
         self._expert = True
-        self.configure(state='normal')
+        self.configure(state="normal")
 
     def setNonExpert(self):
         """
         Turns off 'expert' status whereby to allow a button to be disabled
         """
         self._expert = False
         if self._active:
@@ -1479,36 +1532,39 @@
 
 
 class Ilabel(tk.Label):
     """
     Class to define an information label which uses the same font
     as the entry fields rather than the default font
     """
+
     def __init__(self, master, **kw):
         tk.Label.__init__(self, master, **kw)
         g = get_root(self).globals
         self.config(font=g.ENTRY_FONT)
 
 
 class PABox(RangedFloat):
     """
     A float that wraps at 360 deg
     """
+
     def set(self, value):
-        new_val = coord.Longitude(value*u.deg).deg
+        new_val = coord.Longitude(value * u.deg).deg
         RangedFloat.set(self, new_val)
 
 
 class Sexagesimal(tk.Entry):
     """
     Widget for coordinate entry
     """
-    def __init__(self, master, ival=0, callback=None, unit='hms', **kw):
+
+    def __init__(self, master, ival=0, callback=None, unit="hms", **kw):
         tk.Entry.__init__(self, master, **kw)
-        if unit == 'hms':
+        if unit == "hms":
             self.unit = u.hourangle
         else:
             self.unit = u.deg
         # variable is the thing that's shown in the widget
         self._variable = tk.StringVar()
         # value is the thing that tracks the value, and has a unit
         self._value = coord.Angle(ival, unit=u.deg)
@@ -1517,17 +1573,19 @@
         self.config(textvariable=self._variable)
         self.checker = callback
         self.set_unbind()
         self.set_bind()
 
     def as_string(self):
         if self.unit == u.hourangle:
-            return self._value.to_string(unit=self.unit, sep=':', precision=2)
+            return self._value.to_string(unit=self.unit, sep=":", precision=2)
         else:
-            return self._value.to_string(unit=self.unit, sep=':', precision=1, alwayssign=True)
+            return self._value.to_string(
+                unit=self.unit, sep=":", precision=1, alwayssign=True
+            )
 
     def validate(self, value):
         """
         Applies the validation criteria.
         Returns value, new value, or None if invalid.
         """
         try:
@@ -1575,60 +1633,60 @@
         try:
             coord.Angle(self._value, unit=u.deg)
             return True
         except ValueError:
             return False
 
     def enable(self):
-        self.configure(state='normal')
+        self.configure(state="normal")
         self.set_bind()
 
     def disable(self):
-        self.configure(state='disable')
+        self.configure(state="disable")
         self.set_unbind()
 
     def set_bind(self):
         """
         Sets key bindings.
         """
-        self.bind('<Button-1>', lambda e: self.add(0.1*u.arcsec))
-        self.bind('<Button-3>', lambda e: self.sub(0.1*u.arcsec))
-        self.bind('<Up>', lambda e: self.add(0.1*u.arcsec))
-        self.bind('<Down>', lambda e: self.sub(0.1*u.arcsec))
-        self.bind('<Shift-Up>', lambda e: self.add(1*u.arcsec))
-        self.bind('<Shift-Down>', lambda e: self.sub(1*u.arcsec))
-        self.bind('<Control-Up>', lambda e: self.add(10*u.arcsec))
-        self.bind('<Control-Down>', lambda e: self.sub(10*u.arcsec))
-        self.bind('<Double-Button-1>', self._dadd)
-        self.bind('<Double-Button-3>', self._dsub)
-        self.bind('<Shift-Button-1>', lambda e: self.add(1*u.arcsec))
-        self.bind('<Shift-Button-3>', lambda e: self.sub(1*u.arcsec))
-        self.bind('<Control-Button-1>', lambda e: self.add(10*u.arcsec))
-        self.bind('<Control-Button-3>', lambda e: self.sub(10*u.arcsec))
-        self.bind('<Enter>', self._enter)
+        self.bind("<Button-1>", lambda e: self.add(0.1 * u.arcsec))
+        self.bind("<Button-3>", lambda e: self.sub(0.1 * u.arcsec))
+        self.bind("<Up>", lambda e: self.add(0.1 * u.arcsec))
+        self.bind("<Down>", lambda e: self.sub(0.1 * u.arcsec))
+        self.bind("<Shift-Up>", lambda e: self.add(1 * u.arcsec))
+        self.bind("<Shift-Down>", lambda e: self.sub(1 * u.arcsec))
+        self.bind("<Control-Up>", lambda e: self.add(10 * u.arcsec))
+        self.bind("<Control-Down>", lambda e: self.sub(10 * u.arcsec))
+        self.bind("<Double-Button-1>", self._dadd)
+        self.bind("<Double-Button-3>", self._dsub)
+        self.bind("<Shift-Button-1>", lambda e: self.add(1 * u.arcsec))
+        self.bind("<Shift-Button-3>", lambda e: self.sub(1 * u.arcsec))
+        self.bind("<Control-Button-1>", lambda e: self.add(10 * u.arcsec))
+        self.bind("<Control-Button-3>", lambda e: self.sub(10 * u.arcsec))
+        self.bind("<Enter>", self._enter)
 
     def set_unbind(self):
         """
         Unsets key bindings.
         """
-        self.unbind('<Button-1>')
-        self.unbind('<Button-3>')
-        self.unbind('<Up>')
-        self.unbind('<Down>')
-        self.unbind('<Shift-Up>')
-        self.unbind('<Shift-Down>')
-        self.unbind('<Control-Up>')
-        self.unbind('<Control-Down>')
-        self.unbind('<Double-Button-1>')
-        self.unbind('<Double-Button-3>')
-        self.unbind('<Shift-Button-1>')
-        self.unbind('<Shift-Button-3>')
-        self.unbind('<Control-Button-1>')
-        self.unbind('<Control-Button-3>')
-        self.unbind('<Enter>')
+        self.unbind("<Button-1>")
+        self.unbind("<Button-3>")
+        self.unbind("<Up>")
+        self.unbind("<Down>")
+        self.unbind("<Shift-Up>")
+        self.unbind("<Shift-Down>")
+        self.unbind("<Control-Up>")
+        self.unbind("<Control-Down>")
+        self.unbind("<Double-Button-1>")
+        self.unbind("<Double-Button-3>")
+        self.unbind("<Shift-Button-1>")
+        self.unbind("<Shift-Button-3>")
+        self.unbind("<Control-Button-1>")
+        self.unbind("<Control-Button-3>")
+        self.unbind("<Enter>")
 
     def _callback(self, *dummy):
         """
         This gets called on any attempt to change the value
         """
         # retrieve the value from the Entry
         value = self._variable.get()
@@ -1642,20 +1700,20 @@
             # Store new value
             self._value = coord.Angle(value, unit=self.unit)
             if self.checker:
                 self.checker(*dummy)
 
     # following are callbacks for bindings
     def _dadd(self, event):
-        self.add(0.1*u.arcsec)
-        return 'break'
+        self.add(0.1 * u.arcsec)
+        return "break"
 
     def _dsub(self, event):
-        self.sub(0.1*u.arcsec)
-        return 'break'
+        self.sub(0.1 * u.arcsec)
+        return "break"
 
     def _enter(self, event):
         self.focus()
         self.icursor(tk.END)
 
 
 #
@@ -1667,48 +1725,48 @@
     """
 
     def __init__(self, master, width):
         """
         master   : containing widget
         width    : width of button
         """
-        ActButton.__init__(self, master, width, text='Stop')
+        ActButton.__init__(self, master, width, text="Stop")
         g = get_root(self).globals
-        self.config(bg=g.COL['stop'])
+        self.config(bg=g.COL["stop"])
 
         # flags to help with stopping in background
         self.stopping = False
 
     def enable(self):
         """
         Enable the button.
         """
         ActButton.enable(self)
         g = get_root(self).globals
-        self.config(bg=g.COL['stop'])
+        self.config(bg=g.COL["stop"])
 
     def disable(self):
         """
         Disable the button, if in non-expert mode.
         """
         ActButton.disable(self)
         g = get_root(self).globals
         if self._expert:
-            self.config(bg=g.COL['stop'])
+            self.config(bg=g.COL["stop"])
         else:
-            self.config(bg=g.COL['stopD'])
+            self.config(bg=g.COL["stopD"])
 
     def setExpert(self):
         """
         Turns on 'expert' status whereby the button is always enabled,
         regardless of its activity status.
         """
         ActButton.setExpert(self)
         g = get_root(self).globals
-        self.config(bg=g.COL['stop'])
+        self.config(bg=g.COL["stop"])
 
     def setNonExpert(self):
         """
         Turns off 'expert' status whereby to allow a button to be disabled
         """
         self._expert = False
         if self._active:
@@ -1718,27 +1776,27 @@
 
     @inlineCallbacks
     def act(self):
         """
         Carries out the action associated with Stop button
         """
         g = get_root(self).globals
-        g.clog.info('Stop pressed')
+        g.clog.info("Stop pressed")
 
         # Stop exposure meter
         # do this first, so timer doesn't also try to enable idle mode
         g.info.timer.stop()
 
         try:
             session = get_root(self).globals.session
-            yield session.call('hipercam.ngc.rpc.abort')
+            yield session.call("hipercam.ngc.rpc.abort")
             self.stopping = True
         except Exception as err:
-            msg = err.error_message() if hasattr(err, 'error_message') else str(err)
-            g.clog.warn('Run stop failed. Error = ' + msg)
+            msg = err.error_message() if hasattr(err, "error_message") else str(err)
+            g.clog.warn("Run stop failed. Error = " + msg)
             self.stopping = False
 
     @inlineCallbacks
     def on_telemetry(self, package):
         """
         Checks the status of the stop exposure command
         This is run every time a telemetry packet comes in from NGC.
@@ -1746,93 +1804,94 @@
         It is the responsibility of an implementing GUI to subscribe to the
         NGC telemetry topic with this function as the callback.
         """
         telemetry = pickle.loads(package)
 
         g = get_root(self).globals
         res = ReadNGCTelemetry(telemetry)
-        stopped = res.state == 'idle'
+        stopped = res.state == "idle"
 
         if stopped and self.stopping:
             # Exposure stopped OK; modify buttons
             self.disable()
 
             # try and write FITS table before enabling start button, otherwise
             # a new start will clear table
             try:
                 yield insertFITSHDU(g)
             except Exception as err:
-                g.clog.warn('Could not add FITS Table to run')
+                g.clog.warn("Could not add FITS Table to run")
                 g.clog.warn(str(err))
 
             g.observe.start.enable()
             g.setup.powerOn.disable()
             g.setup.powerOff.enable()
             self.disable()
 
             # Report that run has stopped
-            g.clog.info('Run stopped')
+            g.clog.info("Run stopped")
             self.stopping = False
 
             # enable idle mode now run has stopped
-            g.clog.info('Setting chips to idle')
-            idle = {'appdata': {'app': 'Idle'}}
+            g.clog.info("Setting chips to idle")
+            idle = {"appdata": {"app": "Idle"}}
             try:
                 success = yield postJSON(g, idle)
                 if not success:
-                    raise Exception('postJSON returned false')
+                    raise Exception("postJSON returned false")
             except Exception as err:
-                g.clog.warn('Failed to enable idle mode')
+                g.clog.warn("Failed to enable idle mode")
                 g.clog.warn(str(err))
 
-            g.clog.info('Stopping offsets (if running')
+            g.clog.info("Stopping offsets (if running")
             try:
                 success = yield stopNodding(g)
                 if not success:
-                    raise Exception('Failed to stop dithering: response was false')
+                    raise Exception("Failed to stop dithering: response was false")
             except Exception as err:
-                g.clog.warn('Failed to stop GTC offset script')
+                g.clog.warn("Failed to stop GTC offset script")
                 g.clog.warn(str(err))
 
             returnValue(True)
         elif stopped and not self.stopping:
             # exposure is not running, but we haven't been pressed
             g.observe.start.enable()
             self.disable()
         elif self.stopping:
             # Exposure in process of stopping
             # Disable lots of buttons
             self.disable()
             g.observe.start.disable()
             g.setup.powerOn.disable()
             g.setup.powerOff.disable()
-        elif res.state == 'active':
+        elif res.state == "active":
             # exposure is underway
             self.enable()
             g.observe.start.disable()
             g.setup.powerOn.disable()
             g.setup.powerOff.disable()
 
 
 class ProgramID(tk.Frame):
     """
     Class to combine the ProgramID and OB number.
 
     This is a text entry field and a PosInt widget bound together.
     The point of this widget is simply to get a nice layout.
     """
+
     def __init__(self, master):
         tk.Frame.__init__(self, master)
         self.master = master
-        check = master.check if hasattr(master, 'check') else None
+        check = master.check if hasattr(master, "check") else None
         self.progid = TextEntry(self, 20, check)
         self.obid = PosInt(self, 1, check, True, width=4)
 
         self.progid.pack(side=tk.LEFT, anchor=tk.W)
-        tk.Label(self, text='/').pack(side=tk.LEFT, anchor=tk.W, padx=2)
+        tk.Label(self, text="/").pack(side=tk.LEFT, anchor=tk.W, padx=2)
         self.obid.pack(side=tk.LEFT, anchor=tk.W, padx=2)
 
     def disable(self):
         self.obid.disable()
 
     def enable(self):
         self.obid.enable()
@@ -1849,36 +1908,37 @@
     """
     Class wrapping up what is needed for a target name which
     is an entry field and a verification button. The verification
     button checks for simbad recognition and goes green or red
     according to the results. If no check has been made, it has
     a default colour.
     """
+
     def __init__(self, master, callback=None):
         tk.Frame.__init__(self, master)
 
         g = get_root(self).globals
 
         # Entry field, linked to a StringVar which is traced for
         # any modification
         self.val = tk.StringVar()
-        self.val.trace('w', self.modver)
+        self.val.trace("w", self.modver)
         self.entry = tk.Entry(
-            self, textvariable=self.val, fg=g.COL['text'],
-            bg=g.COL['main'], width=25)
-        self.entry.bind('<Enter>', lambda e: self.entry.focus())
+            self, textvariable=self.val, fg=g.COL["text"], bg=g.COL["main"], width=25
+        )
+        self.entry.bind("<Enter>", lambda e: self.entry.focus())
 
         # Verification button which accesses simbad to see if
         # the target is recognised.
         self.verify = tk.Button(
-            self, fg='black', width=8, text='Verify',
-            bg=g.COL['main'], command=self.act)
+            self, fg="black", width=8, text="Verify", bg=g.COL["main"], command=self.act
+        )
         self.entry.pack(side=tk.LEFT, anchor=tk.W)
         self.verify.pack(side=tk.LEFT, anchor=tk.W, padx=5)
-        self.verify.config(state='disable')
+        self.verify.config(state="disable")
         # track successed and failures
         self.successes = []
         self.failures = []
         self.callback = callback
 
     def value(self):
         """
@@ -1889,139 +1949,140 @@
     def set(self, text):
         """
         Sets value.
         """
         return self.val.set(text)
 
     def disable(self):
-        self.entry.configure(state='disable')
+        self.entry.configure(state="disable")
         g = get_root(self).globals
         if self.ok():
             tname = self.val.get()
             if tname in self.successes:
                 # known to be in simbad
-                self.verify.config(bg=g.COL['startD'])
+                self.verify.config(bg=g.COL["startD"])
             elif tname in self.failures:
                 # known not to be in simbad
-                self.verify.config(bg=g.COL['stopD'])
+                self.verify.config(bg=g.COL["stopD"])
             else:
                 # not known whether in simbad
-                self.verify.config(bg=g.COL['main'])
+                self.verify.config(bg=g.COL["main"])
         else:
-            self.verify.config(bg=g.COL['main'])
-        self.verify.config(state='disable')
+            self.verify.config(bg=g.COL["main"])
+        self.verify.config(state="disable")
 
     def enable(self):
-        self.entry.configure(state='normal')
+        self.entry.configure(state="normal")
         g = get_root(self).globals
         if self.ok():
             tname = self.val.get()
             if tname in self.successes:
                 # known to be in simbad
-                self.verify.config(bg=g.COL['start'])
+                self.verify.config(bg=g.COL["start"])
             elif tname in self.failures:
                 # known not to be in simbad
-                self.verify.config(bg=g.COL['stop'])
+                self.verify.config(bg=g.COL["stop"])
             else:
                 # not known whether in simbad
-                self.verify.config(bg=g.COL['main'])
+                self.verify.config(bg=g.COL["main"])
         else:
-            self.verify.config(bg=g.COL['main'])
-        self.verify.config(state='normal')
+            self.verify.config(bg=g.COL["main"])
+        self.verify.config(state="normal")
 
     def ok(self):
-        if self.val.get() == '' or self.val.get().isspace():
+        if self.val.get() == "" or self.val.get().isspace():
             return False
         else:
             return True
 
     def modver(self, *args):
         """
         Switches colour of verify button
         """
         g = get_root(self).globals
         if self.ok():
             tname = self.val.get()
             if tname in self.successes:
                 # known to be in simbad
-                self.verify.config(bg=g.COL['start'])
+                self.verify.config(bg=g.COL["start"])
             elif tname in self.failures:
                 # known not to be in simbad
-                self.verify.config(bg=g.COL['stop'])
+                self.verify.config(bg=g.COL["stop"])
             else:
                 # not known whether in simbad
-                self.verify.config(bg=g.COL['main'])
-            self.verify.config(state='normal')
+                self.verify.config(bg=g.COL["main"])
+            self.verify.config(state="normal")
         else:
-            self.verify.config(bg=g.COL['main'])
-            self.verify.config(state='disable')
+            self.verify.config(bg=g.COL["main"])
+            self.verify.config(state="disable")
 
         if self.callback is not None:
             self.callback()
 
     def act(self):
         """
         Carries out the action associated with Verify button
         """
         tname = self.val.get()
         g = get_root(self).globals
-        g.clog.info('Checking ' + tname + ' in simbad')
+        g.clog.info("Checking " + tname + " in simbad")
         try:
             ret = checkSimbad(g, tname)
             if len(ret) == 0:
-                self.verify.config(bg=g.COL['stop'])
+                self.verify.config(bg=g.COL["stop"])
                 g.clog.warn('No matches to "' + tname + '" found.')
                 if tname not in self.failures:
                     self.failures.append(tname)
             elif len(ret) == 1:
-                self.verify.config(bg=g.COL['start'])
-                g.clog.info(tname + ' verified OK in simbad')
-                g.clog.info('Primary simbad name = ' + ret[0]['Name'])
+                self.verify.config(bg=g.COL["start"])
+                g.clog.info(tname + " verified OK in simbad")
+                g.clog.info("Primary simbad name = " + ret[0]["Name"])
                 if tname not in self.successes:
                     self.successes.append(tname)
             else:
                 g.clog.warn('More than one match to "' + tname + '" found')
-                self.verify.config(bg=g.COL['stop'])
+                self.verify.config(bg=g.COL["stop"])
                 if tname not in self.failures:
                     self.failures.append(tname)
         except urllib.error.URLError:
-            g.clog.warn('Simbad lookup timed out')
+            g.clog.warn("Simbad lookup timed out")
         except socket.timeout:
-            g.clog.warn('Simbad lookup timed out')
+            g.clog.warn("Simbad lookup timed out")
 
 
 class NGCReset(ActButton):
     """
     Class defining the 'NGC Reset' button
     """
+
     def __init__(self, master, width):
         """
         master   : containing widget
         width    : width of button
         """
-        ActButton.__init__(self, master, width, text='NGC Reset')
+        ActButton.__init__(self, master, width, text="NGC Reset")
 
     @inlineCallbacks
     def act(self):
         """
         Carries out the action associated with the System Reset
         """
         root = get_root(self)
         g = root.globals
-        g.clog.debug('NGC Reset pressed')
+        g.clog.debug("NGC Reset pressed")
         session = root.globals.session
         try:
-            msg, ok = yield session.call('hipercam.ngc.rpc.reset')
+            msg, ok = yield session.call("hipercam.ngc.rpc.reset")
             if not ok:
-                raise RuntimeError('reset command failed: ' + msg)
+                raise RuntimeError("reset command failed: " + msg)
         except Exception:
-            g.clog.warn('NGC Reset failed')
+            g.clog.warn("NGC Reset failed")
             returnValue(False)
         else:
-            g.clog.info('NGC Reset succeeded')
+            g.clog.info("NGC Reset succeeded")
 
             # alter buttons here
             g.observe.start.disable()
             g.observe.stop.disable()
             g.setup.cldcOn.disable()
             g.setup.cldcOff.disable()
             returnValue(True)
@@ -2030,34 +2091,35 @@
 class NGCStandby(ActButton):
     """
     Class defining the standby button.
 
     In standby, the NGC server will respond to commands, but processes (sequencer) etc are
     halted, and power is off to controller.
     """
+
     def __init__(self, master, width):
         """
         master   : containing widget
         width    : width of button
         """
-        ActButton.__init__(self, master, width, text='NGC Standby')
+        ActButton.__init__(self, master, width, text="NGC Standby")
 
     @inlineCallbacks
     def act(self):
         root = get_root(self)
         g = root.globals
-        g.clog.debug('NGC Standby pressed')
+        g.clog.debug("NGC Standby pressed")
         session = root.globals.session
         try:
-            yield session.call('hipercam.ngc.rpc.standby')
+            yield session.call("hipercam.ngc.rpc.standby")
         except Exception as err:
-            g.clog.warn('NGC Standby failed: ' + str(err))
+            g.clog.warn("NGC Standby failed: " + str(err))
             returnValue(False)
         else:
-            g.clog.info('Standby command successful')
+            g.clog.info("Standby command successful")
             # alter buttons here
             g.observe.start.disable()
             g.observe.stop.disable()
             g.setup.cldcOn.disable()
             g.setup.cldcOff.disable()
             returnValue(True)
 
@@ -2066,35 +2128,36 @@
     """
     Class defining the online button.
 
     In online, the NGC server will respond to commands, but processes (e.g sequencer)
     are autostarted if autostart is enabled, as are any clocks. You can turn clocks on
     and off in this state.
     """
+
     def __init__(self, master, width):
         """
         master   : containing widget
         width    : width of button
         """
-        ActButton.__init__(self, master, width, text='NGC Online')
+        ActButton.__init__(self, master, width, text="NGC Online")
 
     @inlineCallbacks
     def act(self):
         root = get_root(self)
         g = root.globals
-        g.clog.debug('NGC Online pressed')
+        g.clog.debug("NGC Online pressed")
         session = root.globals.session
         try:
-            yield session.call('hipercam.ngc.rpc.online')
+            yield session.call("hipercam.ngc.rpc.online")
         except Exception as err:
-            msg = err.error_message() if hasattr(err, 'error_message') else str(err)
+            msg = err.error_message() if hasattr(err, "error_message") else str(err)
             g.clog.warn("NGC Online failed: " + msg)
             returnValue(False)
         else:
-            g.clog.info('Online command successful')
+            g.clog.info("Online command successful")
             # alter buttons here
             g.observe.start.disable()
             g.observe.stop.disable()
             g.setup.cldcOn.enable()
             g.setup.cldcOff.disable()
             returnValue(True)
 
@@ -2105,194 +2168,199 @@
 
     In the off (loaded) state, the NGC server will respond to commands, but no-subprocesses
     are launched, and the controller electronics configuration and detector configuration
     is not applied.
 
     The server initialises in this state.
     """
+
     def __init__(self, master, width):
         """
         master   : containing widget
         width    : width of button
         """
-        ActButton.__init__(self, master, width, text='NGC Off')
+        ActButton.__init__(self, master, width, text="NGC Off")
 
     @inlineCallbacks
     def act(self):
         root = get_root(self)
         g = root.globals
-        g.clog.debug('NGC Off pressed')
+        g.clog.debug("NGC Off pressed")
         session = root.globals.session
         try:
-            yield session.call('hipercam.ngc.rpc.offline')
+            yield session.call("hipercam.ngc.rpc.offline")
         except Exception as err:
-            msg = err.error_message() if hasattr(err, 'error_message') else str(err)
+            msg = err.error_message() if hasattr(err, "error_message") else str(err)
             g.clog.warn("NGC Off failed: " + msg)
             returnValue(False)
         else:
-            g.clog.info('off command successful; server in loaded state')
+            g.clog.info("off command successful; server in loaded state")
 
             # alter buttons here
             g.observe.start.disable()
             g.observe.stop.disable()
             g.setup.cldcOn.disable()
             g.setup.cldcOff.disable()
             returnValue(True)
 
 
 class SeqStart(ActButton):
     """
     Class defining the button to start sequencers.
     """
+
     def __init__(self, master, width):
         """
         master   : containing widget
         width    : width of button
         """
-        ActButton.__init__(self, master, width, text='Seq Start')
+        ActButton.__init__(self, master, width, text="Seq Start")
         self.disable()
 
     @inlineCallbacks
     def act(self):
         root = get_root(self)
         g = root.globals
-        g.clog.debug('Seq Start pressed')
+        g.clog.debug("Seq Start pressed")
         session = root.globals.session
 
         try:
-            msg, ok = yield session.call('hipercam.ngc.rpc.seq_start')
+            msg, ok = yield session.call("hipercam.ngc.rpc.seq_start")
             if not ok:
-                raise RuntimeError('could not start sequencer: ' + msg)
+                raise RuntimeError("could not start sequencer: " + msg)
         except Exception as err:
-            msg = err.error_message() if hasattr(err, 'error_message') else str(err)
+            msg = err.error_message() if hasattr(err, "error_message") else str(err)
             g.clog.warn("Seq Start failed: " + msg)
             returnValue(False)
         else:
-            g.clog.info('seq start command successful; clocks powered on')
+            g.clog.info("seq start command successful; clocks powered on")
             # alter buttons here
             g.observe.start.enable()
             g.observe.stop.enable()
             g.setup.seqStop.enable()
             self.disable()
             returnValue(True)
 
 
 class SeqStop(ActButton):
     """
     Class defining the button to stop sequencers.
     """
+
     def __init__(self, master, width):
         """
         master   : containing widget
         width    : width of button
         """
-        ActButton.__init__(self, master, width, text='Seq Stop')
+        ActButton.__init__(self, master, width, text="Seq Stop")
         self.disable()
 
     @inlineCallbacks
     def act(self):
         root = get_root(self)
         g = root.globals
-        g.clog.debug('Seq Stop pressed')
+        g.clog.debug("Seq Stop pressed")
         session = root.globals.session
 
         try:
-            msg, ok = yield session.call('hipercam.ngc.rpc.seq_stop')
+            msg, ok = yield session.call("hipercam.ngc.rpc.seq_stop")
             if not ok:
-                raise RuntimeError('could not stop sequencer: ' + msg)
+                raise RuntimeError("could not stop sequencer: " + msg)
         except Exception as err:
-            msg = err.error_message() if hasattr(err, 'error_message') else str(err)
+            msg = err.error_message() if hasattr(err, "error_message") else str(err)
             g.clog.warn("Seq Stop failed: " + msg)
             returnValue(False)
         else:
-            g.clog.info('seq stop command successful')
+            g.clog.info("seq stop command successful")
             # alter buttons here
             g.observe.start.disable()
             g.observe.stop.disable()
             g.setup.seqStart.enable()
             self.disable()
             returnValue(True)
 
 
 class CLDCOn(ActButton):
     """
     Class defining the button to turn on clocks.
     """
+
     def __init__(self, master, width):
         """
         master   : containing widget
         width    : width of button
         """
-        ActButton.__init__(self, master, width, text='CLDC On')
+        ActButton.__init__(self, master, width, text="CLDC On")
         self.disable()
 
     @inlineCallbacks
     def act(self):
         root = get_root(self)
         g = root.globals
-        g.clog.debug('CLDC On pressed')
+        g.clog.debug("CLDC On pressed")
         session = root.globals.session
         try:
             powered_on = yield isPoweredOn(g)
         except Exception as err:
             g.clog.warn(str(err))
             returnValue(False)
 
         if powered_on:
-            g.clog.info('clocks already on')
+            g.clog.info("clocks already on")
             returnValue(True)
 
         try:
-            msg, ok = yield session.call('hipercam.ngc.rpc.pon')
+            msg, ok = yield session.call("hipercam.ngc.rpc.pon")
             if not ok:
-                raise RuntimeError('could not power on clocks')
+                raise RuntimeError("could not power on clocks")
         except Exception as err:
-            msg = err.error_message() if hasattr(err, 'error_message') else str(err)
+            msg = err.error_message() if hasattr(err, "error_message") else str(err)
             g.clog.warn("CLDC On failed: " + msg)
             returnValue(False)
         else:
-            g.clog.info('CLDC on command successful; clocks powered on')
+            g.clog.info("CLDC on command successful; clocks powered on")
             # alter buttons here
             g.observe.start.enable()
             g.observe.stop.enable()
             g.setup.cldcOff.enable()
             g.setup.seqStart.enable()
             self.disable()
             returnValue(True)
 
 
 class CLDCOff(ActButton):
     """
     Class defining the button to turn off clocks.
     """
+
     def __init__(self, master, width):
         """
         master   : containing widget
         width    : width of button
         """
-        ActButton.__init__(self, master, width, text='CLDC Off')
+        ActButton.__init__(self, master, width, text="CLDC Off")
         self.disable()
 
     @inlineCallbacks
     def act(self):
         root = get_root(self)
         g = root.globals
-        g.clog.debug('CLDC Off pressed')
+        g.clog.debug("CLDC Off pressed")
         session = root.globals.session
 
         try:
-            msg, ok = yield session.call('hipercam.ngc.rpc.poff')
+            msg, ok = yield session.call("hipercam.ngc.rpc.poff")
             if not ok:
-                raise RuntimeError('could not power off clocks')
+                raise RuntimeError("could not power off clocks")
         except Exception as err:
-            msg = err.error_message() if hasattr(err, 'error_message') else str(err)
+            msg = err.error_message() if hasattr(err, "error_message") else str(err)
             g.clog.warn("CLDC Off failed: " + msg)
             returnValue(False)
         else:
-            g.clog.info('CLDC off command successful; clocks powered off')
+            g.clog.info("CLDC off command successful; clocks powered off")
 
             # alter buttons here
             g.observe.start.disable()
             g.observe.stop.disable()
             g.setup.cldcOn.enable()
             self.disable()
             returnValue(True)
@@ -2304,61 +2372,61 @@
     """
 
     def __init__(self, master, width):
         """
         master  : containing widget
         width   : width of button
         """
-        ActButton.__init__(self, master, width, text='Power on')
+        ActButton.__init__(self, master, width, text="Power on")
 
     @inlineCallbacks
     def act(self):
         """
         Power on action
         """
         root = get_root(self)
         g = root.globals
-        g.clog.debug('Power on pressed')
+        g.clog.debug("Power on pressed")
         try:
             session = root.globals.session
-            msg, ok = yield session.call('hipercam.ngc.rpc.online')
+            msg, ok = yield session.call("hipercam.ngc.rpc.online")
             if not ok:
                 raise RuntimeError(msg)
         except Exception as err:
-            msg = err.error_message() if hasattr(err, 'error_message') else str(err)
-            g.clog.warn('Failed to bring server online: ' + msg)
+            msg = err.error_message() if hasattr(err, "error_message") else str(err)
+            g.clog.warn("Failed to bring server online: " + msg)
             return False
         else:
-            g.clog.info('ESO server online')
-            g.cpars['eso_server_online'] = True
+            g.clog.info("ESO server online")
+            g.cpars["eso_server_online"] = True
             try:
                 powered_on = yield isPoweredOn(g)
             except Exception as err:
-                g.clog.warn('cannot determine if CLDC is already on')
-                msg = err.error_message() if hasattr(err, 'error_message') else str(err)
+                g.clog.warn("cannot determine if CLDC is already on")
+                msg = err.error_message() if hasattr(err, "error_message") else str(err)
                 g.clog.warn(msg)
                 returnValue(False)
 
             if not powered_on:
-                success = yield execCommand(g, 'pon')
+                success = yield execCommand(g, "pon")
                 if not success:
-                    g.clog.warn('Unable to power on CLDC')
+                    g.clog.warn("Unable to power on CLDC")
                     returnValue(False)
 
-            success = yield execCommand(g, 'seq_start')
+            success = yield execCommand(g, "seq_start")
             if not success:
-                g.clog.warn('Failed to start sequencer after Power On.')
+                g.clog.warn("Failed to start sequencer after Power On.")
 
             try:
                 run = yield getRunNumber(g)
-                g.info.run.configure(text='{0:03d}'.format(run))
+                g.info.run.configure(text="{0:03d}".format(run))
             except Exception as err:
-                g.clog.warn('Failed to determine run number at start of run')
+                g.clog.warn("Failed to determine run number at start of run")
                 g.clog.warn(str(err))
-                g.info.run.configure(text='UNDEF')
+                g.info.run.configure(text="UNDEF")
 
             # change other buttons
             self.disable()
             g.observe.start.enable()
             g.observe.stop.disable()
             g.setup.powerOff.enable()
             returnValue(True)
@@ -2370,57 +2438,56 @@
     """
 
     def __init__(self, master, width):
         """
         master  : containing widget
         width   : width of button
         """
-        ActButton.__init__(self, master, width, text='Power off')
+        ActButton.__init__(self, master, width, text="Power off")
         self.disable()
 
     @inlineCallbacks
     def act(self):
         """
         Power off action
         """
         g = get_root(self).globals
-        g.clog.debug('Power off pressed')
+        g.clog.debug("Power off pressed")
 
-        success = yield execCommand(g, 'poff')
+        success = yield execCommand(g, "poff")
         if not success:
-            g.clog.warn('Unable to power off CLDC')
+            g.clog.warn("Unable to power off CLDC")
             returnValue(False)
 
-        success = yield execCommand(g, 'offline')
+        success = yield execCommand(g, "offline")
         if success:
-            g.clog.info('ESO server idle')
-            g.cpars['eso_server_online'] = False
+            g.clog.info("ESO server idle")
+            g.cpars["eso_server_online"] = False
 
             # alter buttons
             self.disable()
             g.observe.start.disable()
             g.observe.stop.disable()
             g.setup.powerOn.enable()
             returnValue(True)
         else:
-            g.clog.warn('Power off failed')
+            g.clog.warn("Power off failed")
             returnValue(False)
 
 
 class InstSetup(tk.LabelFrame):
     """
     Instrument setup frame.
     """
 
     def __init__(self, master):
         """
         master -- containing widget
         """
-        tk.LabelFrame.__init__(self, master, text='Instrument setup',
-                               padx=10, pady=10)
+        tk.LabelFrame.__init__(self, master, text="Instrument setup", padx=10, pady=10)
 
         # Define all buttons
         width = 17
         # expert
         self.ngcReset = NGCReset(self, width)
         self.ngcStandby = NGCStandby(self, width)
         self.ngcOnline = NGCOnline(self, width)
@@ -2428,54 +2495,60 @@
         self.cldcOff = CLDCOff(self, width)
         self.cldcOn = CLDCOn(self, width)
         self.seqStart = SeqStart(self, width)
         self.seqStop = SeqStop(self, width)
         # non-expert
         self.powerOn = PowerOn(self, width)
         self.powerOff = PowerOff(self, width)
-        self.all_buttons = [self.ngcReset, self.ngcStandby, self.ngcOnline,
-                            self.ngcOff, self.cldcOn, self.cldcOff,
-                            self.powerOn, self.powerOff, self.seqStart, self.seqStop]
+        self.all_buttons = [
+            self.ngcReset,
+            self.ngcStandby,
+            self.ngcOnline,
+            self.ngcOff,
+            self.cldcOn,
+            self.cldcOff,
+            self.powerOn,
+            self.powerOff,
+            self.seqStart,
+            self.seqStop,
+        ]
         # set which buttons are presented and where they go
         self.setExpertLevel()
-        self.telemetry_topics = [
-            ('hipercam.ngc.telemetry', self.on_telemetry)
-        ]
+        self.telemetry_topics = [("hipercam.ngc.telemetry", self.on_telemetry)]
 
     def on_telemetry(self, package):
         g = get_root(self).globals
         try:
             telemetry = pickle.loads(package)
-            ngc_status = telemetry.get('system.stateName', 'unknown')
+            ngc_status = telemetry.get("system.stateName", "unknown")
             res = ReadNGCTelemetry(telemetry)
             # clocks
-            if res.clocks == 'enabled':
+            if res.clocks == "enabled":
                 self.cldcOn.disable()
                 self.cldcOff.enable()
                 self.seqStart.enable()
             else:
                 self.cldcOn.enable()
                 self.cldcOff.disable()
             # power on/off
-            if (res.clocks == 'enabled'
-                    and ngc_status.lower() == 'online'):
+            if res.clocks == "enabled" and ngc_status.lower() == "online":
                 self.powerOff.enable()
                 self.powerOn.disable()
             else:
                 self.powerOn.enable()
                 self.powerOff.disable()
         except Exception:
-            g.clog.warn('could not decode NGC telemetry')
+            g.clog.warn("could not decode NGC telemetry")
 
     def setExpertLevel(self):
         """
         Set expert level
         """
         g = get_root(self).globals
-        level = g.cpars['expert_level']
+        level = g.cpars["expert_level"]
 
         # first define which buttons are visible
         if level == 0:
             # simple layout
             for button in self.all_buttons:
                 button.grid_forget()
 
@@ -2510,155 +2583,166 @@
 
 class Switch(tk.Frame):
     """
     Frame sub-class to switch between setup, focal plane slide
     and observing frames. Provides radio buttons and hides / shows
     respective frames
     """
+
     def __init__(self, master):
         """
         master : containing widget
         """
         tk.Frame.__init__(self, master)
 
         self.val = tk.StringVar()
-        self.val.set('Setup')
-        self.val.trace('w', self._changed)
+        self.val.set("Setup")
+        self.val.trace("w", self._changed)
 
         g = get_root(self).globals
-        tk.Radiobutton(self, text='Setup', variable=self.val,
-                       font=g.ENTRY_FONT,
-                       value='Setup').grid(row=0, column=0, sticky=tk.W)
-        tk.Radiobutton(self, text='Observe', variable=self.val,
-                       font=g.ENTRY_FONT,
-                       value='Observe').grid(row=0, column=1, sticky=tk.W)
-        tk.Radiobutton(self, text='Focal plane slide', variable=self.val,
-                       font=g.ENTRY_FONT,
-                       value='Focal plane slide').grid(row=0, column=2,
-                                                       sticky=tk.W)
-        self.tecs = tk.Radiobutton(self, text='CCD TECs', variable=self.val,
-                                   font=g.ENTRY_FONT, value='CCD TECs')
+        tk.Radiobutton(
+            self, text="Setup", variable=self.val, font=g.ENTRY_FONT, value="Setup"
+        ).grid(row=0, column=0, sticky=tk.W)
+        tk.Radiobutton(
+            self, text="Observe", variable=self.val, font=g.ENTRY_FONT, value="Observe"
+        ).grid(row=0, column=1, sticky=tk.W)
+        tk.Radiobutton(
+            self,
+            text="Focal plane slide",
+            variable=self.val,
+            font=g.ENTRY_FONT,
+            value="Focal plane slide",
+        ).grid(row=0, column=2, sticky=tk.W)
+        self.tecs = tk.Radiobutton(
+            self,
+            text="CCD TECs",
+            variable=self.val,
+            font=g.ENTRY_FONT,
+            value="CCD TECs",
+        )
         self.tecs.grid(row=0, column=3, sticky=tk.W)
 
         self.setExpertLevel()
 
     def _changed(self, *args):
         g = get_root(self).globals
-        if self.val.get() == 'Setup':
+        if self.val.get() == "Setup":
             g.setup.pack(anchor=tk.W, pady=10)
             g.fpslide.pack_forget()
             g.observe.pack_forget()
             g.tecs.pack_forget()
 
-        elif self.val.get() == 'Focal plane slide':
+        elif self.val.get() == "Focal plane slide":
             g.setup.pack_forget()
             g.fpslide.pack(anchor=tk.W, pady=10)
             g.observe.pack_forget()
             g.tecs.pack_forget()
 
-        elif self.val.get() == 'Observe':
+        elif self.val.get() == "Observe":
             g.setup.pack_forget()
             g.fpslide.pack_forget()
             g.observe.pack(anchor=tk.W, pady=10)
             g.tecs.pack_forget()
 
-        elif self.val.get() == 'CCD TECs':
+        elif self.val.get() == "CCD TECs":
             g.setup.pack_forget()
             g.fpslide.pack_forget()
             g.observe.pack_forget()
             g.tecs.pack(anchor=tk.W, pady=10)
 
         else:
-            raise DriverError('Unrecognised Switch value')
+            raise DriverError("Unrecognised Switch value")
 
     def setExpertLevel(self):
         """
         Modifies widget according to expertise level, which in this
         case is just matter of hiding or revealing the button to
         set CCD temps
         """
         g = get_root(self).globals
-        level = g.cpars['expert_level']
+        level = g.cpars["expert_level"]
         if level == 0:
-            if self.val.get() == 'CCD TECs':
-                self.val.set('Observe')
+            if self.val.get() == "CCD TECs":
+                self.val.set("Observe")
                 self._changed()
             self.tecs.grid_forget()
         else:
             self.tecs.grid(row=0, column=3, sticky=tk.W)
 
 
 class TelChooser(tk.Menu):
     """
     Provides a menu to choose the telescope.
 
     The telescope setting affects the signal/noise calculations
     and routines for pulling RA/Dec etc from the TCS.
     """
+
     def __init__(self, master, *args):
         """
         Parameters
         ----------
         master : tk.Widget
             the containing widget, .e.g toolbar menu
         """
         tk.Menu.__init__(self, master, tearoff=0)
         g = get_root(self).globals
 
         self.val = tk.StringVar()
-        tel = g.cpars.get('telins_name', list(g.TINS)[0])
+        tel = g.cpars.get("telins_name", list(g.TINS)[0])
         self.val.set(tel)
-        self.val.trace('w', self._change)
+        self.val.trace("w", self._change)
         for tel_name in g.TINS.keys():
             self.add_radiobutton(label=tel_name, value=tel_name, variable=self.val)
         self.args = args
         self.root = master
 
     def _change(self, *args):
         g = get_root(self).globals
-        g.cpars['telins_name'] = self.val.get()
+        g.cpars["telins_name"] = self.val.get()
         g.count.update()
         g.ipars.check()
 
 
 class ExpertMenu(tk.Menu):
     """
     Provides a menu to select the level of expertise wanted
     when interacting with a control GUI. This setting might
     be used to hide buttons for instance according to
     the status of others, etc. Use ExpertMenu.indices
     to pass a set of indices of the master menu which get
     enabled or disabled according to the expert level (disabled
     at level 0, otherwise enabled)
     """
+
     def __init__(self, master, *args):
         """
         master   -- the containing widget, e.g. toolbar menu
         args     -- other objects that have a 'setExpertLevel()' method.
         """
         tk.Menu.__init__(self, master, tearoff=0)
         g = get_root(self).globals
 
         self.val = tk.IntVar()
-        self.val.set(g.cpars['expert_level'])
-        self.val.trace('w', self._change)
-        self.add_radiobutton(label='Level 0', value=0, variable=self.val)
-        self.add_radiobutton(label='Level 1', value=1, variable=self.val)
-        self.add_radiobutton(label='Level 2', value=2, variable=self.val)
+        self.val.set(g.cpars["expert_level"])
+        self.val.trace("w", self._change)
+        self.add_radiobutton(label="Level 0", value=0, variable=self.val)
+        self.add_radiobutton(label="Level 1", value=1, variable=self.val)
+        self.add_radiobutton(label="Level 2", value=2, variable=self.val)
         self.args = args
         self.root = master
         self.indices = []
 
     def _change(self, *args):
         g = get_root(self).globals
-        g.cpars['expert_level'] = self.val.get()
+        g.cpars["expert_level"] = self.val.get()
         for arg in self.args:
             arg.setExpertLevel()
         for index in self.indices:
-            if g.cpars['expert_level']:
+            if g.cpars["expert_level"]:
                 self.root.entryconfig(index, state=tk.NORMAL)
             else:
                 self.root.entryconfig(index, state=tk.DISABLED)
 
 
 class Timer(tk.Label):
     """
@@ -2666,220 +2750,223 @@
 
     Responsible for monitoring a started run. If a run reaches the end without
     Stop being pressed, this class will make sure that button statuses are
     updated and Idle mode is engaged.
 
     Updates @10Hz, checks run status @1Hz.
     """
+
     def __init__(self, master):
-        tk.Label.__init__(self, master, text='{0:<d} s'.format(0))
+        tk.Label.__init__(self, master, text="{0:<d} s".format(0))
         g = get_root(self).globals
         self.config(font=g.ENTRY_FONT)
         self._loop = None
         self.count = 0
 
     def start(self):
         """
         Starts the timer from zero
         """
         self.startTime = time.time()
-        self.configure(text='{0:<d} s'.format(0))
+        self.configure(text="{0:<d} s".format(0))
         self._loop = LoopingCall(self.tick)
         self._loop.start(0.1)
 
     @inlineCallbacks
     def tick(self):
         """
         Updates @ 10Hz to give smooth running clock, checks
         run status @0.2Hz to reduce load on servers.
         """
         g = get_root(self).globals
         try:
             self.count += 1
             delta = int(round(time.time() - self.startTime))
-            self.configure(text='{0:<d} s'.format(delta))
+            self.configure(text="{0:<d} s".format(delta))
 
             if self.count % 50 == 0:
                 try:
                     run_active = yield isRunActive(g)
                 except Exception as err:
                     g.clog.warn(str(err))
                 if not run_active:
-
                     # try and write FITS table before enabling start button, otherwise
                     # a new start will clear table
                     try:
                         yield insertFITSHDU(g)
                     except Exception as err:
-                        g.clog.warn('Could not add FITS Table to run')
+                        g.clog.warn("Could not add FITS Table to run")
                         g.clog.warn(str(err))
 
                     g.observe.start.enable()
                     g.observe.stop.disable()
                     g.setup.ngcReset.enable()
                     g.setup.powerOn.disable()
                     g.setup.powerOff.enable()
-                    g.clog.info('Timer detected stopped run')
+                    g.clog.info("Timer detected stopped run")
 
-                    warn_cmd = '/usr/bin/ssh observer@192.168.1.1 spd-say "\'exposure finished\'"'
+                    warn_cmd = "/usr/bin/ssh observer@192.168.1.1 spd-say \"'exposure finished'\""
                     try:
-                        subprocess.check_output(warn_cmd, shell=True, stderr=subprocess.PIPE)
+                        subprocess.check_output(
+                            warn_cmd, shell=True, stderr=subprocess.PIPE
+                        )
                     except Exception:
                         pass
 
                     # enable idle mode now run has stopped
-                    g.clog.info('Setting chips to idle')
-                    idle = {'appdata': {'app': 'Idle'}}
+                    g.clog.info("Setting chips to idle")
+                    idle = {"appdata": {"app": "Idle"}}
                     try:
                         success = yield postJSON(g, idle)
                         if not success:
-                            raise Exception('postJSON returned false')
+                            raise Exception("postJSON returned false")
                     except Exception as err:
-                        g.clog.warn('Failed to enable idle mode')
+                        g.clog.warn("Failed to enable idle mode")
                         g.clog.warn(str(err))
 
-                    g.clog.info('Stopping offsets (if running')
+                    g.clog.info("Stopping offsets (if running")
                     try:
                         success = yield stopNodding(g)
                         if not success:
-                            raise Exception('failed to stop dithering')
+                            raise Exception("failed to stop dithering")
                     except Exception as err:
-                        g.clog.warn('Failed to stop GTC offset script')
+                        g.clog.warn("Failed to stop GTC offset script")
                         g.clog.warn(str(err))
 
                     self.stop()
 
         except Exception as err:
             if self.count % 100 == 0:
-                g.clog.warn('Timer.update: error = ' + str(err))
+                g.clog.warn("Timer.update: error = " + str(err))
 
     def stop(self):
-        if hasattr(self, '_loop') and self._loop is not None:
+        if hasattr(self, "_loop") and self._loop is not None:
             self._loop.stop()
         self._loop = None
 
 
 class InfoFrame(tk.LabelFrame):
     """
     Information frame: run number, exposure time, etc.
     """
+
     def __init__(self, master):
-        tk.LabelFrame.__init__(self, master,
-                               text='Current run & telescope status', padx=4, pady=4)
+        tk.LabelFrame.__init__(
+            self, master, text="Current run & telescope status", padx=4, pady=4
+        )
 
-        self.run = Ilabel(self, text='UNDEF')
-        self.frame = Ilabel(self, text='UNDEF')
+        self.run = Ilabel(self, text="UNDEF")
+        self.frame = Ilabel(self, text="UNDEF")
         self.timer = Timer(self)
-        self.cadence = Ilabel(self, text='UNDEF')
-        self.duty = Ilabel(self, text='UNDEF')
-        self.ra = Ilabel(self, text='UNDEF')
-        self.dec = Ilabel(self, text='UNDEF')
-        self.alt = Ilabel(self, text='UNDEF')
-        self.az = Ilabel(self, text='UNDEF')
-        self.airmass = Ilabel(self, text='UNDEF')
-        self.ha = Ilabel(self, text='UNDEF')
-        self.pa = Ilabel(self, text='UNDEF')
-        self.focus = Ilabel(self, text='UNDEF')
-        self.mdist = Ilabel(self, text='UNDEF')
-        self.fpslide = Ilabel(self, text='UNDEF')
-        self.ccd_temps = Ilabel(self, text='UNDEF')
+        self.cadence = Ilabel(self, text="UNDEF")
+        self.duty = Ilabel(self, text="UNDEF")
+        self.ra = Ilabel(self, text="UNDEF")
+        self.dec = Ilabel(self, text="UNDEF")
+        self.alt = Ilabel(self, text="UNDEF")
+        self.az = Ilabel(self, text="UNDEF")
+        self.airmass = Ilabel(self, text="UNDEF")
+        self.ha = Ilabel(self, text="UNDEF")
+        self.pa = Ilabel(self, text="UNDEF")
+        self.focus = Ilabel(self, text="UNDEF")
+        self.mdist = Ilabel(self, text="UNDEF")
+        self.fpslide = Ilabel(self, text="UNDEF")
+        self.ccd_temps = Ilabel(self, text="UNDEF")
 
         # left-hand side
-        tk.Label(self, text='Run:').grid(row=0, column=0, padx=5, sticky=tk.W)
+        tk.Label(self, text="Run:").grid(row=0, column=0, padx=5, sticky=tk.W)
         self.run.grid(row=0, column=1, padx=5, sticky=tk.W)
 
-        tk.Label(self, text='Frame:').grid(row=1, column=0, padx=5, sticky=tk.W)
+        tk.Label(self, text="Frame:").grid(row=1, column=0, padx=5, sticky=tk.W)
         self.frame.grid(row=1, column=1, padx=5, sticky=tk.W)
 
-        tk.Label(self, text='Exposure:').grid(row=2, column=0, padx=5, sticky=tk.W)
+        tk.Label(self, text="Exposure:").grid(row=2, column=0, padx=5, sticky=tk.W)
         self.timer.grid(row=2, column=1, padx=5, sticky=tk.W)
 
-        tk.Label(self, text='Cadence:').grid(row=3, column=0, padx=5, sticky=tk.W)
+        tk.Label(self, text="Cadence:").grid(row=3, column=0, padx=5, sticky=tk.W)
         self.cadence.grid(row=3, column=1, padx=5, sticky=tk.W)
 
-        tk.Label(self, text='Duty cycle:').grid(row=4, column=0, padx=5,
-                                                sticky=tk.W)
+        tk.Label(self, text="Duty cycle:").grid(row=4, column=0, padx=5, sticky=tk.W)
         self.duty.grid(row=4, column=1, padx=5, sticky=tk.W)
 
         # middle
-        tk.Label(self, text='RA:').grid(row=0, column=3, padx=5, sticky=tk.W)
+        tk.Label(self, text="RA:").grid(row=0, column=3, padx=5, sticky=tk.W)
         self.ra.grid(row=0, column=4, padx=5, sticky=tk.W)
 
-        tk.Label(self, text='Dec:').grid(row=1, column=3, padx=5, sticky=tk.W)
+        tk.Label(self, text="Dec:").grid(row=1, column=3, padx=5, sticky=tk.W)
         self.dec.grid(row=1, column=4, padx=5, sticky=tk.W)
 
-        tk.Label(self, text='Alt:').grid(row=2, column=3, padx=5, sticky=tk.W)
+        tk.Label(self, text="Alt:").grid(row=2, column=3, padx=5, sticky=tk.W)
         self.alt.grid(row=2, column=4, padx=5, sticky=tk.W)
 
-        tk.Label(self, text='Az:').grid(row=3, column=3, padx=5, sticky=tk.W)
+        tk.Label(self, text="Az:").grid(row=3, column=3, padx=5, sticky=tk.W)
         self.az.grid(row=3, column=4, padx=5, sticky=tk.W)
 
-        tk.Label(self, text='Airm:').grid(row=4, column=3, padx=5, sticky=tk.W)
+        tk.Label(self, text="Airm:").grid(row=4, column=3, padx=5, sticky=tk.W)
         self.airmass.grid(row=4, column=4, padx=5, sticky=tk.W)
 
-        tk.Label(self, text='HA:').grid(row=5, column=3, padx=5, sticky=tk.W)
+        tk.Label(self, text="HA:").grid(row=5, column=3, padx=5, sticky=tk.W)
         self.ha.grid(row=5, column=4, padx=5, sticky=tk.W)
 
         # right-hand side
-        tk.Label(self, text='PA:').grid(row=0, column=6, padx=5, sticky=tk.W)
+        tk.Label(self, text="PA:").grid(row=0, column=6, padx=5, sticky=tk.W)
         self.pa.grid(row=0, column=7, padx=5, sticky=tk.W)
 
-        tk.Label(self, text='Focus:').grid(row=1, column=6, padx=5, sticky=tk.W)
+        tk.Label(self, text="Focus:").grid(row=1, column=6, padx=5, sticky=tk.W)
         self.focus.grid(row=1, column=7, padx=5, sticky=tk.W)
 
-        tk.Label(self, text='Mdist:').grid(row=2, column=6, padx=5, sticky=tk.W)
+        tk.Label(self, text="Mdist:").grid(row=2, column=6, padx=5, sticky=tk.W)
         self.mdist.grid(row=2, column=7, padx=5, sticky=tk.W)
 
-        tk.Label(self, text='FP slide:').grid(row=3, column=6, padx=5, sticky=tk.W)
+        tk.Label(self, text="FP slide:").grid(row=3, column=6, padx=5, sticky=tk.W)
         self.fpslide.grid(row=3, column=7, padx=5, sticky=tk.W)
 
-        tk.Label(self, text='CCD temps:').grid(row=4, column=6, padx=5, sticky=tk.W)
+        tk.Label(self, text="CCD temps:").grid(row=4, column=6, padx=5, sticky=tk.W)
         self.ccd_temps.grid(row=4, column=7, padx=5, sticky=tk.W)
 
         # add a FITS table to record TCS info
         self.tcs_table = create_gtc_header_table()
 
         # start
         self.count = 0
         self.update()
 
         # an implementing GUI must subscribe this widget to the
         # following topics, with the given callbacks
         self.telemetry_topics = [
-            ('hipercam.slide.telemetry', self.update_slidepos),
-            ('hipercam.gtc.telemetry', self.update_tcs),
-            ('hipercam.ccd1.telemetry', self.update_ccd),
-            ('hipercam.ccd2.telemetry', self.update_ccd),
-            ('hipercam.ccd3.telemetry', self.update_ccd),
-            ('hipercam.ccd4.telemetry', self.update_ccd),
-            ('hipercam.ccd5.telemetry', self.update_ccd),
-            ('hipercam.ngc.telemetry', self.update_runstatus)
+            ("hipercam.slide.telemetry", self.update_slidepos),
+            ("hipercam.gtc.telemetry", self.update_tcs),
+            ("hipercam.ccd1.telemetry", self.update_ccd),
+            ("hipercam.ccd2.telemetry", self.update_ccd),
+            ("hipercam.ccd3.telemetry", self.update_ccd),
+            ("hipercam.ccd4.telemetry", self.update_ccd),
+            ("hipercam.ccd5.telemetry", self.update_ccd),
+            ("hipercam.ngc.telemetry", self.update_runstatus),
         ]
 
         self._update_tcs_table_loop = LoopingCall(self.update_tcs_table)
         self._update_tcs_table_loop.start(60)
 
     def _getVal(self, widg):
-        return -99.0 if widg['text'] == 'UNDEF' else float(widg['text'])
+        return -99.0 if widg["text"] == "UNDEF" else float(widg["text"])
 
     def dumpJSON(self):
         """
         Return dictionary of data for FITS headers.
         """
         g = get_root(self).globals
         return dict(
-            RA=self.ra['text'],
-            DEC=self.dec['text'],
-            tel=g.cpars['telins_name'],
+            RA=self.ra["text"],
+            DEC=self.dec["text"],
+            tel=g.cpars["telins_name"],
             alt=self._getVal(self.alt),
             az=self._getVal(self.az),
             secz=self._getVal(self.airmass),
             pa=self._getVal(self.pa),
             foc=self._getVal(self.focus),
-            mdist=self._getVal(self.mdist)
+            mdist=self._getVal(self.mdist),
         )
 
     def clear_tcs_table(self):
         """
         Create a new table from scratch - should be cleared for each run.
         """
         self.tcs_table = create_gtc_header_table()
@@ -2889,23 +2976,25 @@
         """
         Periodically update a table of info from the TCS.
 
         Only works at GTC. Called every 60s.
         """
         root = get_root(self)
         g = root.globals
-        if not g.cpars['tcs_on'] or not g.cpars['telins_name'].lower() == 'gtc':
+        if not g.cpars["tcs_on"] or not g.cpars["telins_name"].lower() == "gtc":
             return
         try:
             session = root.globals.session
-            telpars = yield session.call('hipercam.gtc.rpc.get_telescope_pars')
+            telpars = yield session.call("hipercam.gtc.rpc.get_telescope_pars")
+            if telpars is None:
+                raise RuntimeError("no telescope parameters returned from server")
             add_gtc_header_table_row(self.tcs_table, telpars)
         except Exception as err:
-            msg = err.error_message() if hasattr(err, 'error_message') else str(err)
-            g.clog.warn('Could not update table of TCS info: ' + msg)
+            msg = err.error_message() if hasattr(err, "error_message") else str(err)
+            g.clog.warn("Could not update table of TCS info: " + msg)
 
     def update_tcs(self, packet):
         """
         Update TCS data.
 
         This is a callback to be used with subscription to the GTC telemetry
         topic.
@@ -2914,63 +3003,62 @@
         ----------
         packet: bytes
             a pickled serialisation of the telemetry packet
         """
         g = get_root(self).globals
         try:
             telemetry = pickle.loads(packet)
-            header = telemetry['telpars']
+            header = telemetry["telpars"]
         except Exception as err:
-            g.clog.warn('Could not parse telemetry from TCS: ' + str(err))
+            g.clog.warn("Could not parse telemetry from TCS: " + str(err))
         else:
-            ra = float(header['RADEG'])
-            dec = float(header['DECDEG'])
-            pa = float(header['INSTRPA'])
-            focus = float(header['M2UZ'])
+            ra = float(header["RADEG"])
+            dec = float(header["DECDEG"])
+            pa = float(header["INSTRPA"])
+            focus = float(header["M2UZ"])
             # format ra, dec as HMS
             coo = coord.SkyCoord(ra, dec, unit=(u.deg, u.deg))
-            ratxt = coo.ra.to_string(sep=':', unit=u.hour, precision=0)
-            dectxt = coo.dec.to_string(sep=':', unit=u.deg,
-                                       alwayssign=True,
-                                       precision=0)
+            ratxt = coo.ra.to_string(sep=":", unit=u.hour, precision=0)
+            dectxt = coo.dec.to_string(
+                sep=":", unit=u.deg, alwayssign=True, precision=0
+            )
             self.ra.configure(text=ratxt)
             self.dec.configure(text=dectxt)
 
             # wrap pa from 0 to 360
-            pa = coord.Longitude(pa*u.deg)
-            self.pa.configure(text='{0:6.2f}'.format(pa.value))
+            pa = coord.Longitude(pa * u.deg)
+            self.pa.configure(text="{0:6.2f}".format(pa.value))
 
             # set focus
-            self.focus.configure(text='{0:+5.2f}'.format(focus))
+            self.focus.configure(text="{0:+5.2f}".format(focus))
 
             # Calculate most of the
             # stuff that we don't get from the telescope
             now = Time.now()
             lon = g.astro.obs.lon
-            lst = now.sidereal_time(kind='mean',
-                                    longitude=lon)
-            ha = lst - coo.ra.hourangle*u.hourangle
-            hatxt = ha.wrap_at(12*u.hourangle).to_string(sep=':', precision=0)
+            lst = now.sidereal_time(kind="mean", longitude=lon)
+            ha = lst - coo.ra.hourangle * u.hourangle
+            hatxt = ha.wrap_at(12 * u.hourangle).to_string(sep=":", precision=0)
             self.ha.configure(text=hatxt)
 
             altaz_frame = coord.AltAz(obstime=now, location=g.astro.obs)
             altaz = coo.transform_to(altaz_frame)
-            self.alt.configure(text='{0:<4.1f}'.format(altaz.alt.value))
-            self.az.configure(text='{0:<5.1f}'.format(altaz.az.value))
+            self.alt.configure(text="{0:<4.1f}".format(altaz.alt.value))
+            self.az.configure(text="{0:<5.1f}".format(altaz.az.value))
             # set airmass
-            self.airmass.configure(text='{0:<4.2f}'.format(altaz.secz))
+            self.airmass.configure(text="{0:<4.2f}".format(altaz.secz))
 
             # distance to the moon. Warn if too close
             # (configurable) to it.
             md = coord.get_moon(now, g.astro.obs).separation(coo)
-            self.mdist.configure(text='{0:<7.2f}'.format(md.value))
-            if md < g.cpars['mdist_warn']*u.deg:
-                self.mdist.configure(bg=g.COL['warn'])
+            self.mdist.configure(text="{0:<7.2f}".format(md.value))
+            if md < g.cpars["mdist_warn"] * u.deg:
+                self.mdist.configure(bg=g.COL["warn"])
             else:
-                self.mdist.configure(bg=g.COL['main'])
+                self.mdist.configure(bg=g.COL["main"])
 
     def update_ccd(self, packet):
         """
         Update the CCD label.
 
         This routine is a callback to be called whenever a telemetry message
         from a CCD is received.
@@ -2980,100 +3068,100 @@
         packet: bytes
             a pickled serialisation of the telemetry packet
         """
         g = get_root(self).globals
         try:
             telemetry = pickle.loads(packet)
         except Exception as err:
-            g.clog.warn('could not decode CCD telemetry: ' + str(err))
-            self.ccd_temps.configure(text='UNDEF')
-            self.ccd_temps.configure(bg=g.COL['warn'])
+            g.clog.warn("could not decode CCD telemetry: " + str(err))
+            self.ccd_temps.configure(text="UNDEF")
+            self.ccd_temps.configure(bg=g.COL["warn"])
         else:
-            if telemetry['state'] == 'OK':
-                self.ccd_temps.configure(text='OK')
-                self.ccd_temps.configure(bg=g.COL['main'])
+            if telemetry["state"] == "OK":
+                self.ccd_temps.configure(text="OK")
+                self.ccd_temps.configure(bg=g.COL["main"])
             else:
-                self.ccd_temps.configure(text='ERR')
-                self.ccd_temps.configure(bg=g.COL['warn'])
+                self.ccd_temps.configure(text="ERR")
+                self.ccd_temps.configure(bg=g.COL["warn"])
 
     def update_slidepos(self, packet):
         """
         Update the slide position.
 
         This routine is a callback to be called whenever a telemetry message
         from the slide is received.
 
         Parameters
         ----------
         packet: bytes
             a pickled serialisation of the telemetry packet
         """
         g = get_root(self).globals
-        if not g.cpars['focal_plane_slide_on']:
+        if not g.cpars["focal_plane_slide_on"]:
             return
 
         try:
             telemetry = pickle.loads(packet)
         except Exception as err:
-            g.clog.warn('could not decode slide telemetry: ' + str(err))
+            g.clog.warn("could not decode slide telemetry: " + str(err))
         else:
             # get positions, dealing with the fact that sometimes it has units
             try:
-                pos = telemetry['position']['current']
-                targ = telemetry['position']['target']
-                pos = pos.value if hasattr(pos, 'value') else pos
-                targ = targ.value if hasattr(targ, 'value') else targ
-                state = telemetry['state']
-                if 'error' in state['connection'] or 'offline' in state['connection']:
-                    self.fpslide.configure(bg=g.COL['warn'])
-                    g.clog.warn('slide in error state')
-
-                self.fpslide.configure(text='{0:d}'.format(
-                        int(round(pos))))
-                if pos < 1050. or abs(pos-targ) > 3:
-                    self.fpslide.configure(bg=g.COL['warn'])
+                pos = telemetry["position"]["current"]
+                targ = telemetry["position"]["target"]
+                pos = pos.value if hasattr(pos, "value") else pos
+                targ = targ.value if hasattr(targ, "value") else targ
+                state = telemetry["state"]
+                if "error" in state["connection"] or "offline" in state["connection"]:
+                    self.fpslide.configure(bg=g.COL["warn"])
+                    g.clog.warn("slide in error state")
+
+                self.fpslide.configure(text="{0:d}".format(int(round(pos))))
+                if pos < 1050.0 or abs(pos - targ) > 3:
+                    self.fpslide.configure(bg=g.COL["warn"])
                 else:
-                    self.fpslide.configure(bg=g.COL['main'])
+                    self.fpslide.configure(bg=g.COL["main"])
             except Exception as err:
-                g.clog.warn('unable to process slide telemetry: ') + str(err)
+                g.clog.warn("unable to process slide telemetry: ") + str(err)
 
     def update_runstatus(self, packet):
         """
         Updates run status widgets.
 
         This routine is a callback to be called whenever a telemetry message
         from the NGC is received.
 
         Parameters
         ----------
         packet: bytes
             a pickled serialisation of the telemetry packet
         """
         g = get_root(self).globals
-        if not (g.cpars['hcam_server_on'] and g.cpars['eso_server_online']):
+        if not (g.cpars["hcam_server_on"] and g.cpars["eso_server_online"]):
             return
 
         try:
             telemetry = pickle.loads(packet)
             status = ReadNGCTelemetry(telemetry)
             run = status.run
-            frame_no = int(telemetry['exposure.frame'])
+            frame_no = int(telemetry["exposure.frame"])
         except Exception as err:
-            g.clog.warn('failed to parse NGC telemetry: ' + str(err))
+            g.clog.warn("failed to parse NGC telemetry: " + str(err))
         else:
-            self.run.configure(text='{0:03d}'.format(run))
-            self.frame.configure(text='{0:04d}'.format(frame_no))
+            self.run.configure(text="{0:03d}".format(run))
+            self.frame.configure(text="{0:04d}".format(frame_no))
 
 
 class AstroFrame(tk.LabelFrame):
     """
     Astronomical information frame
     """
+
     def __init__(self, master):
-        tk.LabelFrame.__init__(self, master, padx=2, pady=2, text='Time & Sky')
+        tk.LabelFrame.__init__(self, master, padx=2, pady=2, text="Time & Sky")
 
         # times
         self.mjd = Ilabel(self)
         self.utc = Ilabel(self, width=9, anchor=tk.W)
         self.lst = Ilabel(self)
 
         # sun info
@@ -3086,64 +3174,55 @@
         self.moonra = Ilabel(self)
         self.moondec = Ilabel(self)
         self.moonalt = Ilabel(self)
         self.moonphase = Ilabel(self)
 
         # observatory info
         g = get_root(self).globals
-        tins = g.TINS[g.cpars['telins_name']]
-        lat = tins['latitude']
-        lon = tins['longitude']
-        elevation = tins['elevation']
+        tins = g.TINS[g.cpars["telins_name"]]
+        lat = tins["latitude"]
+        lon = tins["longitude"]
+        elevation = tins["elevation"]
         self.obs = coord.EarthLocation.from_geodetic(
-            lon*u.deg,
-            lat*u.deg,
-            elevation*u.m
+            lon * u.deg, lat * u.deg, elevation * u.m
         )
         # report back to the user
-        g.clog.info('Tel/ins = ' + g.cpars['telins_name'])
-        g.clog.info('Longitude = ' + str(tins['longitude']) + ' E')
-        g.clog.info('Latitude = ' + str(tins['latitude']) + ' N')
-        g.clog.info('Elevation = ' + str(tins['elevation']) + ' m')
+        g.clog.info("Tel/ins = " + g.cpars["telins_name"])
+        g.clog.info("Longitude = " + str(tins["longitude"]) + " E")
+        g.clog.info("Latitude = " + str(tins["latitude"]) + " N")
+        g.clog.info("Elevation = " + str(tins["elevation"]) + " m")
 
         # arrange time info
-        tk.Label(self, text='MJD:').grid(
-            row=0, column=0, padx=2, pady=3, sticky=tk.W)
+        tk.Label(self, text="MJD:").grid(row=0, column=0, padx=2, pady=3, sticky=tk.W)
         self.mjd.grid(row=0, column=1, columnspan=2, padx=2, pady=3, sticky=tk.W)
-        tk.Label(self, text='UTC:').grid(
-            row=0, column=3, padx=2, pady=3, sticky=tk.W)
+        tk.Label(self, text="UTC:").grid(row=0, column=3, padx=2, pady=3, sticky=tk.W)
         self.utc.grid(row=0, column=4, padx=2, pady=3, sticky=tk.W)
-        tk.Label(self, text='LST:').grid(
-            row=0, column=5, padx=2, pady=3, sticky=tk.W)
+        tk.Label(self, text="LST:").grid(row=0, column=5, padx=2, pady=3, sticky=tk.W)
         self.lst.grid(row=0, column=6, padx=2, pady=3, sticky=tk.W)
 
         # arrange solar info
-        tk.Label(self, text='Sun:').grid(
-            row=1, column=0, padx=2, pady=3, sticky=tk.W)
-        tk.Label(self, text='Alt:').grid(
-            row=1, column=1, padx=2, pady=3, sticky=tk.W)
+        tk.Label(self, text="Sun:").grid(row=1, column=0, padx=2, pady=3, sticky=tk.W)
+        tk.Label(self, text="Alt:").grid(row=1, column=1, padx=2, pady=3, sticky=tk.W)
         self.sunalt.grid(row=1, column=2, padx=2, pady=3, sticky=tk.W)
         self.lriset.grid(row=1, column=3, padx=2, pady=3, sticky=tk.W)
         self.riset.grid(row=1, column=4, padx=2, pady=3, sticky=tk.W)
-        tk.Label(self, text='At -18:').grid(
-            row=1, column=5, padx=2, pady=3, sticky=tk.W)
+        tk.Label(self, text="At -18:").grid(
+            row=1, column=5, padx=2, pady=3, sticky=tk.W
+        )
         self.astro.grid(row=1, column=6, padx=2, pady=3, sticky=tk.W)
 
         # arrange moon info
-        tk.Label(self, text='Moon:').grid(
-            row=2, column=0, padx=2, pady=3, sticky=tk.W)
-        tk.Label(self, text='RA:').grid(
-            row=2, column=1, padx=2, pady=3, sticky=tk.W)
+        tk.Label(self, text="Moon:").grid(row=2, column=0, padx=2, pady=3, sticky=tk.W)
+        tk.Label(self, text="RA:").grid(row=2, column=1, padx=2, pady=3, sticky=tk.W)
         self.moonra.grid(row=2, column=2, padx=2, pady=3, sticky=tk.W)
-        tk.Label(self, text='Dec:').grid(row=3, column=1, padx=2, sticky=tk.W)
+        tk.Label(self, text="Dec:").grid(row=3, column=1, padx=2, sticky=tk.W)
         self.moondec.grid(row=3, column=2, padx=2, sticky=tk.W)
-        tk.Label(self, text='Alt:').grid(
-            row=2, column=3, padx=2, pady=3, sticky=tk.W)
+        tk.Label(self, text="Alt:").grid(row=2, column=3, padx=2, pady=3, sticky=tk.W)
         self.moonalt.grid(row=2, column=4, padx=2, pady=3, sticky=tk.W)
-        tk.Label(self, text='Phase:').grid(row=3, column=3, padx=2, sticky=tk.W)
+        tk.Label(self, text="Phase:").grid(row=3, column=3, padx=2, sticky=tk.W)
         self.moonphase.grid(row=3, column=4, padx=2, sticky=tk.W)
 
         # parameters used to reduce re-calculation of sun rise etc, and
         # to provide info for other widgets
         self.lastRiset = Time.now()
         self.lastAstro = Time.now()
         self.counter = 0
@@ -3160,120 +3239,146 @@
             self.counter += 1
             g = get_root(self).globals
 
             # current time
             now = Time.now()
 
             # configure times
-            self.utc.configure(text=now.datetime.strftime('%H:%M:%S'))
-            self.mjd.configure(text='{0:11.5f}'.format(now.mjd))
+            self.utc.configure(text=now.datetime.strftime("%H:%M:%S"))
+            self.mjd.configure(text="{0:11.5f}".format(now.mjd))
             lon = self.obs.lon
-            lst = now.sidereal_time(kind='mean', longitude=lon)
-            self.lst.configure(text=lst.to_string(sep=':', precision=0))
+            lst = now.sidereal_time(kind="mean", longitude=lon)
+            self.lst.configure(text=lst.to_string(sep=":", precision=0))
 
             if self.counter % 600 == 1:
                 # only re-compute Sun & Moon info once every 600 calls
                 altaz_frame = coord.AltAz(obstime=now, location=self.obs)
                 sun = coord.get_sun(now)
                 sun_aa = sun.transform_to(altaz_frame)
                 moon = coord.get_moon(now, self.obs)
                 moon_aa = moon.transform_to(altaz_frame)
                 elongation = sun.separation(moon)
-                moon_phase_angle = np.arctan2(sun.distance*np.sin(elongation),
-                                              moon.distance - sun.distance*np.cos(elongation))
-                moon_phase = (1 + np.cos(moon_phase_angle))/2.0
-
-                self.sunalt.configure(
-                    text='{0:+03d} deg'.format(int(sun_aa.alt.deg))
+                moon_phase_angle = np.arctan2(
+                    sun.distance * np.sin(elongation),
+                    moon.distance - sun.distance * np.cos(elongation),
                 )
+                moon_phase = (1 + np.cos(moon_phase_angle)) / 2.0
+
+                self.sunalt.configure(text="{0:+03d} deg".format(int(sun_aa.alt.deg)))
                 self.moonra.configure(
-                    text=moon.ra.to_string(unit='hour', sep=':', precision=0)
+                    text=moon.ra.to_string(unit="hour", sep=":", precision=0)
                 )
                 self.moondec.configure(
-                    text=moon.dec.to_string(unit='deg', sep=':', precision=0)
+                    text=moon.dec.to_string(unit="deg", sep=":", precision=0)
+                )
+                self.moonalt.configure(text="{0:+03d} deg".format(int(moon_aa.alt.deg)))
+                self.moonphase.configure(
+                    text="{0:02d} %".format(int(100.0 * moon_phase.value))
                 )
-                self.moonalt.configure(text='{0:+03d} deg'.format(
-                        int(moon_aa.alt.deg)
-                ))
-                self.moonphase.configure(text='{0:02d} %'.format(
-                        int(100.*moon_phase.value)
-                ))
 
-                if (now > self.lastRiset and now > self.lastAstro):
+                if now > self.lastRiset and now > self.lastAstro:
                     # Only re-compute rise and setting times when necessary,
                     # and only re-compute when both rise/set and astro
                     # twilight times have gone by
 
                     # For sunrise and set we set the horizon down to match a
                     # standard amount of refraction at the horizon and subtract size of disc
-                    horizon = -64*u.arcmin
-                    sunset = calc_riseset(now, 'sun', self.obs, 'next', 'setting', horizon)
-                    sunrise = calc_riseset(now, 'sun', self.obs, 'next', 'rising', horizon)
+                    horizon = -64 * u.arcmin
+                    sunset = calc_riseset(
+                        now, "sun", self.obs, "next", "setting", horizon
+                    )
+                    sunrise = calc_riseset(
+                        now, "sun", self.obs, "next", "rising", horizon
+                    )
 
                     # Astro twilight: geometric centre at -18 deg
-                    horizon = -18*u.deg
-                    astroset = calc_riseset(now, 'sun', self.obs, 'next', 'setting', horizon)
-                    astrorise = calc_riseset(now, 'sun', self.obs, 'next', 'rising', horizon)
+                    horizon = -18 * u.deg
+                    astroset = calc_riseset(
+                        now, "sun", self.obs, "next", "setting", horizon
+                    )
+                    astrorise = calc_riseset(
+                        now, "sun", self.obs, "next", "rising", horizon
+                    )
 
                     if sunrise > sunset:
                         # In the day time we report the upcoming sunset and
                         # end of evening twilight
-                        self.lriset.configure(text='Sets:', font=g.DEFAULT_FONT)
+                        self.lriset.configure(text="Sets:", font=g.DEFAULT_FONT)
                         self.lastRiset = sunset
                         self.lastAstro = astroset
 
                     elif astrorise > astroset and astrorise < sunrise:
                         # During evening twilight, we report the sunset just
                         # passed and end of evening twilight
-                        self.lriset.configure(text='Sets:', font=g.DEFAULT_FONT)
-                        horizon = -64*u.arcmin
-                        self.lastRiset = calc_riseset(now, 'sun', self.obs, 'previous', 'setting', horizon)
+                        self.lriset.configure(text="Sets:", font=g.DEFAULT_FONT)
+                        horizon = -64 * u.arcmin
+                        self.lastRiset = calc_riseset(
+                            now, "sun", self.obs, "previous", "setting", horizon
+                        )
                         self.lastAstro = astroset
 
                     elif astrorise > astroset and astrorise < sunrise:
                         # During night, report upcoming start of morning
                         # twilight and sunrise
-                        self.lriset.configure(text='Rises:',
-                                              font=g.DEFAULT_FONT)
-                        horizon = -64*u.arcmin
+                        self.lriset.configure(text="Rises:", font=g.DEFAULT_FONT)
+                        horizon = -64 * u.arcmin
                         self.lastRiset = sunrise
                         self.lastAstro = astrorise
 
                     else:
                         # During morning twilight report start of twilight
                         # just passed and upcoming sunrise
-                        self.lriset.configure(text='Rises:',
-                                              font=g.DEFAULT_FONT)
-                        horizon = -18*u.deg
+                        self.lriset.configure(text="Rises:", font=g.DEFAULT_FONT)
+                        horizon = -18 * u.deg
                         self.lastRiset = sunrise
-                        self.lastAstro = calc_riseset(now, 'sun', self.obs, 'previous', 'rising', horizon)
+                        self.lastAstro = calc_riseset(
+                            now, "sun", self.obs, "previous", "rising", horizon
+                        )
 
                     # Configure the corresponding text fields
                     self.riset.configure(
                         text=self.lastRiset.datetime.strftime("%H:%M:%S")
                     )
                     self.astro.configure(
                         text=self.lastAstro.datetime.strftime("%H:%M:%S")
                     )
 
         except Exception as err:
             # catchall
-            g.clog.warn('AstroFrame.update: error = ' + str(err))
+            g.clog.warn("AstroFrame.update: error = " + str(err))
 
         # run again after 100 milli-seconds
         self.after_id = self.after(100, self.update)
 
 
 class WinPairs(tk.Frame):
     """
     Class to define a frame of multiple window pairs,
     contained within a gridded block that can be easily position.
     """
-    def __init__(self, master, xsls, xslmins, xslmaxs, xsrs, xsrmins, xsrmaxs,
-                 yss, ysmins, ysmaxs, nxs, nys, xbfac, ybfac, checker, hcam=True):
+
+    def __init__(
+        self,
+        master,
+        xsls,
+        xslmins,
+        xslmaxs,
+        xsrs,
+        xsrmins,
+        xsrmaxs,
+        yss,
+        ysmins,
+        ysmaxs,
+        nxs,
+        nys,
+        xbfac,
+        ybfac,
+        checker,
+        hcam=True,
+    ):
         """
         Arguments:
 
           master :
             container widget
 
           xsls, xslmins, xslmaxs :
@@ -3307,102 +3412,133 @@
             to any changes made to the values stored in a Window. Can be None.
 
         It is assumed that the maximum X dimension is the same for both left
         and right windows and equal to xslmax-xslmin+1.
         """
         self.is_hcam = hcam
         npair = len(xsls)
-        checks = (xsls, xslmins, xslmaxs, xsrs, xsrmins, xsrmaxs,
-                  yss, ysmins, ysmaxs, nxs, nys)
+        checks = (
+            xsls,
+            xslmins,
+            xslmaxs,
+            xsrs,
+            xsrmins,
+            xsrmaxs,
+            yss,
+            ysmins,
+            ysmaxs,
+            nxs,
+            nys,
+        )
         for check in checks:
             if npair != len(check):
                 raise DriverError(
-                    'drivers.WindowPairs.__init__:' +
-                    ' conflict array lengths amonst inputs')
+                    "drivers.WindowPairs.__init__:"
+                    + " conflict array lengths amonst inputs"
+                )
 
         tk.Frame.__init__(self, master)
 
         # top part contains the binning factors and
         # the number of active windows
         top = tk.Frame(self)
         top.pack(anchor=tk.W)
 
-        tk.Label(top, text='Binning factors (X x Y): ').grid(
-            row=0, column=0, sticky=tk.W)
+        tk.Label(top, text="Binning factors (X x Y): ").grid(
+            row=0, column=0, sticky=tk.W
+        )
 
         xyframe = tk.Frame(top)
         self.xbin = ListInt(xyframe, xbfac[0], xbfac, checker, width=2)
         self.xbin.pack(side=tk.LEFT)
-        tk.Label(xyframe, text=' x ').pack(side=tk.LEFT)
+        tk.Label(xyframe, text=" x ").pack(side=tk.LEFT)
         self.ybin = ListInt(xyframe, ybfac[0], ybfac, checker, width=2)
         self.ybin.pack(side=tk.LEFT)
         xyframe.grid(row=0, column=1, sticky=tk.W)
 
         row = 1
         allowed_pairs = (1, 2, 3)
         ap = [pairnum for pairnum in allowed_pairs if pairnum <= npair]
         self.npair = ListInt(top, ap[0], ap, checker, width=2)
         if npair > 1:
             # Second row: number of windows
-            tk.Label(top, text='Number of window pairs').grid(
-                row=1, column=0, sticky=tk.W)
+            tk.Label(top, text="Number of window pairs").grid(
+                row=1, column=0, sticky=tk.W
+            )
             self.npair.grid(row=row, column=1, sticky=tk.W, pady=2)
             row += 1
 
         # bottom part contains the window settings
         bottom = tk.Frame(self)
         bottom.pack(anchor=tk.W)
 
         # top row
-        tk.Label(bottom, text='xsl').grid(row=row, column=1, ipady=5, sticky=tk.S)
-        tk.Label(bottom, text='xsr').grid(row=row, column=2, ipady=5, sticky=tk.S)
-        tk.Label(bottom, text='ys').grid(row=row, column=3, ipady=5, sticky=tk.S)
-        tk.Label(bottom, text='nx').grid(row=row, column=4, ipady=5, sticky=tk.S)
-        tk.Label(bottom, text='ny').grid(row=row, column=5, ipady=5, sticky=tk.S)
+        tk.Label(bottom, text="xsl").grid(row=row, column=1, ipady=5, sticky=tk.S)
+        tk.Label(bottom, text="xsr").grid(row=row, column=2, ipady=5, sticky=tk.S)
+        tk.Label(bottom, text="ys").grid(row=row, column=3, ipady=5, sticky=tk.S)
+        tk.Label(bottom, text="nx").grid(row=row, column=4, ipady=5, sticky=tk.S)
+        tk.Label(bottom, text="ny").grid(row=row, column=5, ipady=5, sticky=tk.S)
 
         row += 1
-        (self.label, self.xsl, self.xsr,
-         self.ys, self.nx, self.ny) = [], [], [], [], [], []
+        (self.label, self.xsl, self.xsr, self.ys, self.nx, self.ny) = (
+            [],
+            [],
+            [],
+            [],
+            [],
+            [],
+        )
         nr = 0
-        for (xsl, xslmin, xslmax, xsr, xsrmin,
-             xsrmax, ys, ysmin, ysmax, nx, ny) in zip(*checks):
-
+        for xsl, xslmin, xslmax, xsr, xsrmin, xsrmax, ys, ysmin, ysmax, nx, ny in zip(
+            *checks
+        ):
             # create
             if npair == 1:
-                self.label.append(tk.Label(bottom, text='Pair: '))
+                self.label.append(tk.Label(bottom, text="Pair: "))
             else:
-                self.label.append(
-                    tk.Label(bottom, text='Pair ' + str(nr) + ': '))
+                self.label.append(tk.Label(bottom, text="Pair " + str(nr) + ": "))
 
             self.xsl.append(
-                RangedInt(bottom, xsl, xslmin, xslmax, checker, True, width=4))
+                RangedInt(bottom, xsl, xslmin, xslmax, checker, True, width=4)
+            )
             self.xsr.append(
-                RangedInt(bottom, xsr, xsrmin, xsrmax, checker, True, width=4))
-            self.ys.append(
-                RangedInt(bottom, ys, ysmin, ysmax, checker, True, width=4))
+                RangedInt(bottom, xsr, xsrmin, xsrmax, checker, True, width=4)
+            )
+            self.ys.append(RangedInt(bottom, ys, ysmin, ysmax, checker, True, width=4))
             self.nx.append(
-                RangedMint(bottom, nx, 1, xslmax-xslmin+1, self.xbin,
-                           checker, True, width=4))
+                RangedMint(
+                    bottom,
+                    nx,
+                    1,
+                    xslmax - xslmin + 1,
+                    self.xbin,
+                    checker,
+                    True,
+                    width=4,
+                )
+            )
             self.ny.append(
-                RangedMint(bottom, ny, 1, ysmax-ysmin+1, self.ybin,
-                           checker, True, width=4))
+                RangedMint(
+                    bottom, ny, 1, ysmax - ysmin + 1, self.ybin, checker, True, width=4
+                )
+            )
 
             # arrange
             self.label[-1].grid(row=row, column=0)
             self.xsl[-1].grid(row=row, column=1)
             self.xsr[-1].grid(row=row, column=2)
             self.ys[-1].grid(row=row, column=3)
             self.nx[-1].grid(row=row, column=4)
             self.ny[-1].grid(row=row, column=5)
 
             row += 1
             nr += 1
 
         # syncing button
-        self.sbutt = ActButton(bottom, 5, self.sync, text='Sync')
+        self.sbutt = ActButton(bottom, 5, self.sync, text="Sync")
         self.sbutt.grid(row=row, column=0, columnspan=5, pady=10, sticky=tk.W)
         self.frozen = False
 
     def check(self):
         """
         Checks the values of the window pairs. If any problems are found, it
         flags them by changing the background colour.
@@ -3418,105 +3554,111 @@
 
         xbin = self.xbin.value()
         ybin = self.ybin.value()
         npair = self.npair.value()
 
         g = get_root(self).globals
         # individual pair checks
-        for xslw, xsrw, ysw, nxw, nyw in zip(self.xsl[:npair], self.xsr[:npair],
-                                             self.ys[:npair], self.nx[:npair],
-                                             self.ny[:npair]):
-            xslw.config(bg=g.COL['main'])
-            xsrw.config(bg=g.COL['main'])
-            ysw.config(bg=g.COL['main'])
-            nxw.config(bg=g.COL['main'])
-            nyw.config(bg=g.COL['main'])
+        for xslw, xsrw, ysw, nxw, nyw in zip(
+            self.xsl[:npair],
+            self.xsr[:npair],
+            self.ys[:npair],
+            self.nx[:npair],
+            self.ny[:npair],
+        ):
+            xslw.config(bg=g.COL["main"])
+            xsrw.config(bg=g.COL["main"])
+            ysw.config(bg=g.COL["main"])
+            nxw.config(bg=g.COL["main"])
+            nyw.config(bg=g.COL["main"])
             status = status if xslw.ok() else False
             status = status if xsrw.ok() else False
             status = status if ysw.ok() else False
             status = status if nxw.ok() else False
             status = status if nyw.ok() else False
             xsl = xslw.value()
             xsr = xsrw.value()
             ys = ysw.value()
             nx = nxw.value()
             ny = nyw.value()
 
             # Are unbinned dimensions consistent with binning factors?
             if nx is None or nx % xbin != 0:
-                nxw.config(bg=g.COL['error'])
+                nxw.config(bg=g.COL["error"])
                 status = False
             elif self.is_hcam and (nx // xbin) % 4 != 0:
                 """
                 The NGC collects pixel data in chunks before transmission.
                 As a result, to avoid loss of data from frames, the binned
                 x-size must be a multiple of 4.
                 """
-                nxw.config(bg=g.COL['error'])
+                nxw.config(bg=g.COL["error"])
                 status = False
 
             if ny is None or ny % ybin != 0:
-                nyw.config(bg=g.COL['error'])
+                nyw.config(bg=g.COL["error"])
                 status = False
 
             # overlap checks
             if xsl is None or xsr is None or xsl >= xsr:
-                xsrw.config(bg=g.COL['error'])
+                xsrw.config(bg=g.COL["error"])
                 status = False
 
             if xsl is None or xsr is None or nx is None or xsl + nx > xsr:
-                xsrw.config(bg=g.COL['error'])
+                xsrw.config(bg=g.COL["error"])
                 status = False
 
             # Are the windows synchronised? This means that they would
             # be consistent with the pixels generated were the whole CCD
             # to be binned by the same factors. If relevant values are not
             # set, we count that as "synced" because the purpose of this is
             # to enable / disable the sync button and we don't want it to be
             # enabled just because xs or ys are not set.
             perform_check = all([param is not None for param in (xsl, xsr, ys, nx, ny)])
-            if (perform_check and
-                ((xsl - 1) % xbin != 0 or (xsr - 1025) % xbin != 0 or
-                 (ys - 1) % ybin != 0)):
+            if perform_check and (
+                (xsl - 1) % xbin != 0
+                or (xsr - 1025) % xbin != 0
+                or (ys - 1) % ybin != 0
+            ):
                 synced = False
 
             # Range checks
             if xsl is None or nx is None or xsl + nx - 1 > xslw.imax:
-                xslw.config(bg=g.COL['error'])
+                xslw.config(bg=g.COL["error"])
                 status = False
 
             if xsr is None or nx is None or xsr + nx - 1 > xsrw.imax:
-                xsrw.config(bg=g.COL['error'])
+                xsrw.config(bg=g.COL["error"])
                 status = False
 
             if ys is None or ny is None or ys + ny - 1 > ysw.imax:
-                ysw.config(bg=g.COL['error'])
+                ysw.config(bg=g.COL["error"])
                 status = False
 
         # Pair overlap checks. Compare one pair with the next one in the
         # same quadrant (if there is one). Only bother if we have survived
         # so far, which saves a lot of checks
         if status:
-            for index in range(npair-2):
+            for index in range(npair - 2):
                 ys1 = self.ys[index].value()
                 ny1 = self.ny[index].value()
 
-                ysw2 = self.ys[index+2]
+                ysw2 = self.ys[index + 2]
                 ys2 = ysw2.value()
                 if ys1 + ny1 > ys2:
-                    ysw2.config(bg=g.COL['error'])
+                    ysw2.config(bg=g.COL["error"])
                     status = False
 
         if synced:
-            self.sbutt.config(bg=g.COL['main'])
+            self.sbutt.config(bg=g.COL["main"])
             self.sbutt.disable()
         else:
             if not self.frozen:
                 self.sbutt.enable()
-            self.sbutt.config(bg=g.COL['warn'])
+            self.sbutt.config(bg=g.COL["warn"])
 
         return status
 
     def sync(self):
         """
         Synchronise the settings. This means that the pixel start
         values are shifted downwards so that they are synchronised
@@ -3526,35 +3668,33 @@
 
         # needs some mods for ultracam ??
         xbin = self.xbin.value()
         ybin = self.ybin.value()
         n = 0
         for xsl, xsr, ys, nx, ny in self:
             if xbin > 1:
-                xsl = xbin*((xsl-1)//xbin)+1
+                xsl = xbin * ((xsl - 1) // xbin) + 1
                 self.xsl[n].set(xsl)
-                xsr = xbin*((xsr-1025)//xbin)+1025
+                xsr = xbin * ((xsr - 1025) // xbin) + 1025
                 self.xsr[n].set(xsr)
 
             if ybin > 1:
-                ys = ybin*((ys-1)//ybin)+1
+                ys = ybin * ((ys - 1) // ybin) + 1
                 self.ys[n].set(ys)
 
             n += 1
         g = get_root(self).globals
-        self.sbutt.config(bg=g.COL['main'])
-        self.sbutt.config(state='disable')
+        self.sbutt.config(bg=g.COL["main"])
+        self.sbutt.config(state="disable")
 
     def freeze(self):
         """
         Freeze (disable) all settings so they can't be altered
         """
-        for xsl, xsr, ys, nx, ny in \
-                zip(self.xsl, self.xsr,
-                    self.ys, self.nx, self.ny):
+        for xsl, xsr, ys, nx, ny in zip(self.xsl, self.xsr, self.ys, self.nx, self.ny):
             xsl.disable()
             xsr.disable()
             ys.disable()
             nx.disable()
             ny.disable()
         self.npair.disable()
         self.xbin.disable()
@@ -3586,28 +3726,38 @@
         self.frozen = False
 
     def enable(self):
         """
         Enables WinPair settings
         """
         npair = self.npair.value()
-        for label, xsl, xsr, ys, nx, ny in \
-                zip(self.label[:npair], self.xsl[:npair], self.xsr[:npair],
-                    self.ys[:npair], self.nx[:npair], self.ny[:npair]):
-            label.config(state='normal')
+        for label, xsl, xsr, ys, nx, ny in zip(
+            self.label[:npair],
+            self.xsl[:npair],
+            self.xsr[:npair],
+            self.ys[:npair],
+            self.nx[:npair],
+            self.ny[:npair],
+        ):
+            label.config(state="normal")
             xsl.enable()
             xsr.enable()
             ys.enable()
             nx.enable()
             ny.enable()
 
-        for label, xsl, xsr, ys, nx, ny in \
-                zip(self.label[npair:], self.xsl[npair:], self.xsr[npair:],
-                    self.ys[npair:], self.nx[npair:], self.ny[npair:]):
-            label.config(state='disable')
+        for label, xsl, xsr, ys, nx, ny in zip(
+            self.label[npair:],
+            self.xsl[npair:],
+            self.xsr[npair:],
+            self.ys[npair:],
+            self.nx[npair:],
+            self.ny[npair:],
+        ):
+            label.config(state="disable")
             xsl.disable()
             xsr.disable()
             ys.disable()
             nx.disable()
             ny.disable()
 
         self.npair.enable()
@@ -3615,40 +3765,70 @@
         self.ybin.enable()
         self.sbutt.enable()
 
     def params(self, n):
         """
         return xsl, xsr, ys, nx, ny for this pair
         """
-        return (self.xsl[n].value(), self.xsr[n].value(),
-                self.ys[n].value(), self.nx[n].value(), self.ny[n].value())
+        return (
+            self.xsl[n].value(),
+            self.xsr[n].value(),
+            self.ys[n].value(),
+            self.nx[n].value(),
+            self.ny[n].value(),
+        )
 
     def __iter__(self):
         """
         Generator to allow looping through through the window pairs.
         Successive calls return xsl, xsr, ys, nx, ny for each pair
         """
         n = 0
         npair = self.npair.value()
         while n < npair:
-            yield (self.xsl[n].value(), self.xsr[n].value(),
-                   self.ys[n].value(), self.nx[n].value(), self.ny[n].value())
+            yield (
+                self.xsl[n].value(),
+                self.xsr[n].value(),
+                self.ys[n].value(),
+                self.nx[n].value(),
+                self.ny[n].value(),
+            )
             n += 1
 
 
 class WinQuads(tk.Frame):
     """
     Class to define a frame of multiple window quads,
     contained within a gridded block that can be easily postioned.
     """
 
-    def __init__(self, master,
-                 xsll, xsllmin, xsllmax, xsul, xsulmin, xsulmax,
-                 xslr, xslrmin, xslrmax, xsur, xsurmin, xsurmax,
-                 ys, ysmin, ysmax, nx, ny, xbfac, ybfac, checker):
+    def __init__(
+        self,
+        master,
+        xsll,
+        xsllmin,
+        xsllmax,
+        xsul,
+        xsulmin,
+        xsulmax,
+        xslr,
+        xslrmin,
+        xslrmax,
+        xsur,
+        xsurmin,
+        xsurmax,
+        ys,
+        ysmin,
+        ysmax,
+        nx,
+        ny,
+        xbfac,
+        ybfac,
+        checker,
+    ):
         """
         Arguments:
 
             master:
                 container widget
 
             xsll, xsllmin, xsllmax: float or container of floats
@@ -3688,95 +3868,150 @@
                 to any changes made to the values stored in a Window. Can be None.
 
         It is assumed that the maximum X dimension is the same for all windows in the quad
         and is equal to xsllmax - xsllmin + 1.
         """
         # check we have a consistent number of quads in all parameters
         nquad = len(xsll)
-        checks = (xsll, xsllmin, xsllmax, xslr, xslrmin, xslrmax,
-                  xsul, xsulmin, xsulmax, xsur, xsurmin, xsurmax,
-                  ys, ysmin, ysmax, nx, ny)
+        checks = (
+            xsll,
+            xsllmin,
+            xsllmax,
+            xslr,
+            xslrmin,
+            xslrmax,
+            xsul,
+            xsulmin,
+            xsulmax,
+            xsur,
+            xsurmin,
+            xsurmax,
+            ys,
+            ysmin,
+            ysmax,
+            nx,
+            ny,
+        )
         for check in checks:
             if nquad != len(check):
-                raise DriverError('drivers.WinQuads.__init__:' +
-                                  ' conflicting array lengths amongst inputs')
+                raise DriverError(
+                    "drivers.WinQuads.__init__:"
+                    + " conflicting array lengths amongst inputs"
+                )
 
         tk.Frame.__init__(self, master)
 
         # top part contains binning factors and number of quads
         top = tk.Frame(self)
         top.pack(anchor=tk.W)
 
-        tk.Label(top, text='Binning factors (X x Y): ').grid(
-            row=0, column=0, sticky=tk.W)
+        tk.Label(top, text="Binning factors (X x Y): ").grid(
+            row=0, column=0, sticky=tk.W
+        )
 
         xyframe = tk.Frame(top)
         self.xbin = ListInt(xyframe, xbfac[0], xbfac, checker, width=2)
         self.xbin.pack(side=tk.LEFT)
-        tk.Label(xyframe, text=' x ').pack(side=tk.LEFT)
+        tk.Label(xyframe, text=" x ").pack(side=tk.LEFT)
         self.ybin = ListInt(xyframe, ybfac[0], ybfac, checker, width=2)
         self.ybin.pack(side=tk.LEFT)
         xyframe.grid(row=0, column=1, sticky=tk.W)
 
         row = 1
         allowed_quads = (1, 2)
         aq = [quadnum for quadnum in allowed_quads if quadnum <= nquad]
         self.nquad = ListInt(top, aq[0], aq, checker, width=2)
         if nquad > 1:
             # Second row: number of quads selector
-            tk.Label(top, text='Number of window quads: ').grid(
-                row=1, column=0, sticky=tk.W)
+            tk.Label(top, text="Number of window quads: ").grid(
+                row=1, column=0, sticky=tk.W
+            )
             self.nquad.grid(row=row, column=1, sticky=tk.W, pady=2)
             row += 1
 
         # bottom part of the frame contains the window settings
         bottom = tk.Frame(self)
         bottom.pack(anchor=tk.W)
 
         # top row - labels
-        tk.Label(bottom, text='xsll').grid(row=row, column=1, ipady=5, sticky=tk.S)
-        tk.Label(bottom, text='xslr').grid(row=row, column=2, ipady=5, sticky=tk.S)
-        tk.Label(bottom, text='xsul').grid(row=row, column=3, ipady=5, sticky=tk.S)
-        tk.Label(bottom, text='xsur').grid(row=row, column=4, ipady=5, sticky=tk.S)
-        tk.Label(bottom, text='ys').grid(row=row, column=5, ipady=5, sticky=tk.S)
-        tk.Label(bottom, text='nx').grid(row=row, column=6, ipady=5, sticky=tk.S)
-        tk.Label(bottom, text='ny').grid(row=row, column=7, ipady=5, sticky=tk.S)
+        tk.Label(bottom, text="xsll").grid(row=row, column=1, ipady=5, sticky=tk.S)
+        tk.Label(bottom, text="xslr").grid(row=row, column=2, ipady=5, sticky=tk.S)
+        tk.Label(bottom, text="xsul").grid(row=row, column=3, ipady=5, sticky=tk.S)
+        tk.Label(bottom, text="xsur").grid(row=row, column=4, ipady=5, sticky=tk.S)
+        tk.Label(bottom, text="ys").grid(row=row, column=5, ipady=5, sticky=tk.S)
+        tk.Label(bottom, text="nx").grid(row=row, column=6, ipady=5, sticky=tk.S)
+        tk.Label(bottom, text="ny").grid(row=row, column=7, ipady=5, sticky=tk.S)
 
         row += 1
-        (self.label, self.xsll, self.xsul, self.xslr, self.xsur,
-         self.ys, self.nx, self.ny) = [], [], [], [], [], [], [], []
+        (
+            self.label,
+            self.xsll,
+            self.xsul,
+            self.xslr,
+            self.xsur,
+            self.ys,
+            self.nx,
+            self.ny,
+        ) = ([], [], [], [], [], [], [], [])
         nr = 0
-        for (xsll, xsllmin, xsllmax, xslr, xslrmin, xslrmax,
-             xsul, xsulmin, xsulmax, xsur, xsurmin, xsurmax,
-             ys, ysmin, ysmax, nx, ny) in zip(*checks):
-
+        for (
+            xsll,
+            xsllmin,
+            xsllmax,
+            xslr,
+            xslrmin,
+            xslrmax,
+            xsul,
+            xsulmin,
+            xsulmax,
+            xsur,
+            xsurmin,
+            xsurmax,
+            ys,
+            ysmin,
+            ysmax,
+            nx,
+            ny,
+        ) in zip(*checks):
             # create
             if nquad == 1:
-                self.label.append(tk.Label(bottom, text='Quad: '))
+                self.label.append(tk.Label(bottom, text="Quad: "))
             else:
-                self.label.append(
-                    tk.Label(bottom, text='Quad ' + str(nr + 1) + ': ')
-                )
+                self.label.append(tk.Label(bottom, text="Quad " + str(nr + 1) + ": "))
 
             self.xsll.append(
-                RangedInt(bottom, xsll, xsllmin, xsllmax, checker, True, width=4))
+                RangedInt(bottom, xsll, xsllmin, xsllmax, checker, True, width=4)
+            )
             self.xsul.append(
-                RangedInt(bottom, xsul, xsulmin, xsulmax, checker, True, width=4))
+                RangedInt(bottom, xsul, xsulmin, xsulmax, checker, True, width=4)
+            )
             self.xslr.append(
-                RangedInt(bottom, xslr, xslrmin, xslrmax, checker, True, width=4))
+                RangedInt(bottom, xslr, xslrmin, xslrmax, checker, True, width=4)
+            )
             self.xsur.append(
-                RangedInt(bottom, xsur, xsurmin, xsurmax, checker, True, width=4))
-            self.ys.append(
-                RangedInt(bottom, ys, ysmin, ysmax, checker, True, width=4))
+                RangedInt(bottom, xsur, xsurmin, xsurmax, checker, True, width=4)
+            )
+            self.ys.append(RangedInt(bottom, ys, ysmin, ysmax, checker, True, width=4))
             self.nx.append(
-                RangedMint(bottom, nx, 1, xsulmax-xsulmin+1, self.xbin,
-                           checker, True, width=4))
+                RangedMint(
+                    bottom,
+                    nx,
+                    1,
+                    xsulmax - xsulmin + 1,
+                    self.xbin,
+                    checker,
+                    True,
+                    width=4,
+                )
+            )
             self.ny.append(
-                RangedMint(bottom, ny, 1, ysmax-ysmin+1, self.ybin,
-                           checker, True, width=4))
+                RangedMint(
+                    bottom, ny, 1, ysmax - ysmin + 1, self.ybin, checker, True, width=4
+                )
+            )
 
             # arrange
             self.label[-1].grid(row=row, column=0)
             self.xsll[-1].grid(row=row, column=1)
             self.xslr[-1].grid(row=row, column=2)
             self.xsul[-1].grid(row=row, column=3)
             self.xsur[-1].grid(row=row, column=4)
@@ -3784,15 +4019,15 @@
             self.nx[-1].grid(row=row, column=6)
             self.ny[-1].grid(row=row, column=7)
 
             row += 1
             nr += 1
 
         # sync button
-        self.sbutt = ActButton(bottom, 5, self.sync, text='Sync')
+        self.sbutt = ActButton(bottom, 5, self.sync, text="Sync")
         self.sbutt.grid(row=row, column=0, columnspan=7, pady=10, sticky=tk.W)
         self.frozen = False
 
     def check(self):
         """
         Checks the values of the window quads. If any problems are found it
         flags the offending window by changing the background colour.
@@ -3804,158 +4039,173 @@
 
         xbin = self.xbin.value()
         ybin = self.ybin.value()
         nquad = self.nquad.value()
 
         g = get_root(self).globals
         # individual window checks
-        for (xsllw, xsulw, xslrw, xsurw, ysw, nxw, nyw) in zip(
-             self.xsll[:nquad],
-             self.xsul[:nquad], self.xslr[:nquad],
-             self.xsur[:nquad], self.ys[:nquad], self.nx[:nquad], self.ny[:nquad]):
-
+        for xsllw, xsulw, xslrw, xsurw, ysw, nxw, nyw in zip(
+            self.xsll[:nquad],
+            self.xsul[:nquad],
+            self.xslr[:nquad],
+            self.xsur[:nquad],
+            self.ys[:nquad],
+            self.nx[:nquad],
+            self.ny[:nquad],
+        ):
             all_fields = (xsllw, xsulw, xslrw, xsurw, ysw, nxw, nyw)
             for field in all_fields:
-                field.config(bg=g.COL['main'])
+                field.config(bg=g.COL["main"])
                 status = status if field.ok() else False
 
             xsll = xsllw.value()
             xsul = xsulw.value()
             xslr = xslrw.value()
             xsur = xsurw.value()
             ys = ysw.value()
             nx = nxw.value()
             ny = nyw.value()
 
             # Are unbinned dimensions consistent with binning factors?
             if nx is None or nx % xbin != 0:
-                nxw.config(bg=g.COL['error'])
+                nxw.config(bg=g.COL["error"])
                 status = False
             elif (nx // xbin) % 4 != 0:
                 """
                 The NGC collects pixel data in chunks before transmission.
                 As a result, to avoid loss of data from frames, the binned
                 x-size must be a multiple of 4.
                 """
-                nxw.config(bg=g.COL['error'])
+                nxw.config(bg=g.COL["error"])
                 status = False
 
             if ny is None or ny % ybin != 0:
-                nyw.config(bg=g.COL['error'])
+                nyw.config(bg=g.COL["error"])
                 status = False
 
             # overlap checks in x direction
             if xsll is None or xslr is None or xsll >= xslr:
-                xslrw.config(bg=g.COL['error'])
+                xslrw.config(bg=g.COL["error"])
                 status = False
             if xsul is None or xsur is None or xsul >= xsur:
-                xsurw.config(bg=g.COL['error'])
+                xsurw.config(bg=g.COL["error"])
                 status = False
             if nx is None or xsll is None or xsll + nx > xslr:
-                xslrw.config(bg=g.COL['error'])
+                xslrw.config(bg=g.COL["error"])
                 status = False
             if xsul is None or nx is None or xsul + nx > xsur:
-                xsurw.config(bg=g.COL['error'])
+                xsurw.config(bg=g.COL["error"])
                 status = False
 
             # Are the windows synchronised? This means that they would
             # be consistent with the pixels generated were the whole CCD
             # to be binned by the same factors. If relevant values are not
             # set, we count that as "synced" because the purpose of this is
             # to enable / disable the sync button and we don't want it to be
             # enabled just because xs or ys are not set.
-            perform_check = all([param is not None for param in (
-                xsll, xslr, ys, nx, ny
-            )])
-            if (perform_check and ((xsll - 1) % xbin != 0 or (xslr - 1025) % xbin != 0 or
-                                   (ys - 1) % ybin != 0)):
+            perform_check = all(
+                [param is not None for param in (xsll, xslr, ys, nx, ny)]
+            )
+            if perform_check and (
+                (xsll - 1) % xbin != 0
+                or (xslr - 1025) % xbin != 0
+                or (ys - 1) % ybin != 0
+            ):
                 synced = False
 
-            perform_check = all([param is not None for param in (
-                xsul, xsur, ys, nx, ny
-            )])
-            if (perform_check and ((xsul - 1) % xbin != 0 or (xsur - 1025) % xbin != 0 or
-                                   (ys - 1) % ybin != 0)):
+            perform_check = all(
+                [param is not None for param in (xsul, xsur, ys, nx, ny)]
+            )
+            if perform_check and (
+                (xsul - 1) % xbin != 0
+                or (xsur - 1025) % xbin != 0
+                or (ys - 1) % ybin != 0
+            ):
                 synced = False
 
             # Range checks
-            rchecks = ((xsll, nx, xsllw), (xslr, nx, xslrw),
-                       (xsul, nx, xsulw), (xsur, nx, xsurw),
-                       (ys, ny, ysw))
+            rchecks = (
+                (xsll, nx, xsllw),
+                (xslr, nx, xslrw),
+                (xsul, nx, xsulw),
+                (xsur, nx, xsurw),
+                (ys, ny, ysw),
+            )
             for check in rchecks:
                 val, size, widg = check
                 if val is None or size is None or val + size - 1 > widg.imax:
-                    widg.config(bg=g.COL['error'])
+                    widg.config(bg=g.COL["error"])
                     status = False
 
         # Quad overlap checks. Compare one quad with the next one
         # in the same quadrant if there is one. Only bother if we
         # have survived so far, which saves a lot of checks.
         if status:
-            for index in range(nquad-1):
+            for index in range(nquad - 1):
                 ys1 = self.ys[index].value()
                 ny1 = self.ny[index].value()
-                ysw2 = self.ys[index+1]
+                ysw2 = self.ys[index + 1]
                 ys2 = ysw2.value()
                 if any([thing is None for thing in (ys1, ny1, ys2)]) or ys1 + ny1 > ys2:
-                    ysw2.config(bg=g.COL['error'])
+                    ysw2.config(bg=g.COL["error"])
                     status = False
 
         if synced:
-            self.sbutt.config(bg=g.COL['main'])
+            self.sbutt.config(bg=g.COL["main"])
             self.sbutt.disable()
         else:
             if not self.frozen:
                 self.sbutt.enable()
-            self.sbutt.config(bg=g.COL['warn'])
+            self.sbutt.config(bg=g.COL["warn"])
         return status
 
     def sync(self):
         """
         Synchronise the settings.
 
         This routine changes the window settings so that the pixel start
         values are shifted downwards until they are synchronised with a
         full-frame binned version. This does nothing if the binning factor
         is 1.
         """
         xbin = self.xbin.value()
         ybin = self.ybin.value()
         if xbin == 1 and ybin == 1:
-            self.sbutt.config(state='disable')
+            self.sbutt.config(state="disable")
             return
 
         for n, (xsll, xsul, xslr, xsur, ys, nx, ny) in enumerate(self):
-            if (xsll-1) % xbin != 0:
-                xsll = xbin * ((xsll-1)//xbin)+1
+            if (xsll - 1) % xbin != 0:
+                xsll = xbin * ((xsll - 1) // xbin) + 1
                 self.xsll[n].set(xsll)
-            if (xsul-1) % xbin != 0:
-                xsul = xbin * ((xsul-1)//xbin)+1
+            if (xsul - 1) % xbin != 0:
+                xsul = xbin * ((xsul - 1) // xbin) + 1
                 self.xsul[n].set(xsul)
-            if (xslr-1025) % xbin != 0:
-                xslr = xbin * ((xslr-1025)//xbin)+1025
+            if (xslr - 1025) % xbin != 0:
+                xslr = xbin * ((xslr - 1025) // xbin) + 1025
                 self.xslr[n].set(xslr)
-            if (xsur-1025) % xbin != 0:
-                xsur = xbin * ((xsur-1025)//xbin)+1025
+            if (xsur - 1025) % xbin != 0:
+                xsur = xbin * ((xsur - 1025) // xbin) + 1025
                 self.xsur[n].set(xsur)
 
-            if ybin > 1 and (ys-1) % ybin != 0:
-                ys = ybin*((ys-1)//ybin)+1
+            if ybin > 1 and (ys - 1) % ybin != 0:
+                ys = ybin * ((ys - 1) // ybin) + 1
                 self.ys[n].set(ys)
 
         g = get_root(self).globals
-        self.sbutt.config(bg=g.COL['main'])
-        self.sbutt.config(state='disable')
+        self.sbutt.config(bg=g.COL["main"])
+        self.sbutt.config(state="disable")
 
     def freeze(self):
         """
         Freeze (disable) all settings
         """
-        for fields in zip(self.xsll, self.xsul, self.xslr, self.xsur,
-                          self.ys, self.nx, self.ny):
+        for fields in zip(
+            self.xsll, self.xsul, self.xslr, self.xsur, self.ys, self.nx, self.ny
+        ):
             for field in fields:
                 field.disable()
         self.nquad.disable()
         self.xbin.disable()
         self.ybin.disable()
         self.sbutt.disable()
         self.frozen = True
@@ -3984,27 +4234,39 @@
         self.frozen = False
 
     def enable(self):
         """
         Enables WinQuad setting
         """
         nquad = self.nquad.value()
-        for label, xsll, xsul, xslr, xsur, ys, nx, ny in \
-                zip(self.label[:nquad], self.xsll[:nquad], self.xsul[:nquad],
-                    self.xslr[:nquad], self.xsur[:nquad], self.ys[:nquad],
-                    self.nx[:nquad], self.ny[:nquad]):
-            label.config(state='normal')
+        for label, xsll, xsul, xslr, xsur, ys, nx, ny in zip(
+            self.label[:nquad],
+            self.xsll[:nquad],
+            self.xsul[:nquad],
+            self.xslr[:nquad],
+            self.xsur[:nquad],
+            self.ys[:nquad],
+            self.nx[:nquad],
+            self.ny[:nquad],
+        ):
+            label.config(state="normal")
             for thing in (xsll, xsul, xslr, xsur, ys, nx, ny):
                 thing.enable()
 
-        for label, xsll, xsul, xslr, xsur, ys, nx, ny in \
-                zip(self.label[nquad:], self.xsll[nquad:], self.xsul[nquad:],
-                    self.xslr[nquad:], self.xsur[nquad:], self.ys[nquad:],
-                    self.nx[nquad:], self.ny[nquad:]):
-            label.config(state='disable')
+        for label, xsll, xsul, xslr, xsur, ys, nx, ny in zip(
+            self.label[nquad:],
+            self.xsll[nquad:],
+            self.xsul[nquad:],
+            self.xslr[nquad:],
+            self.xsur[nquad:],
+            self.ys[nquad:],
+            self.nx[nquad:],
+            self.ny[nquad:],
+        ):
+            label.config(state="disable")
             for thing in (xsll, xsul, xslr, xsur, ys, nx, ny):
                 thing.disable()
 
         self.nquad.enable()
         self.xbin.enable()
         self.ybin.enable()
         self.sbutt.enable()
@@ -4016,30 +4278,47 @@
         Successive calls return xsll, xsul, xslr, xsur, ys, nx, ny
         for each quad.
         """
         n = 0
         nquad = self.nquad.value()
         while n < nquad:
             yield (
-                self.xsll[n].value(), self.xsul[n].value(),
-                self.xslr[n].value(), self.xsur[n].value(),
-                self.ys[n].value(), self.nx[n].value(), self.ny[n].value()
+                self.xsll[n].value(),
+                self.xsul[n].value(),
+                self.xslr[n].value(),
+                self.xsur[n].value(),
+                self.ys[n].value(),
+                self.nx[n].value(),
+                self.ny[n].value(),
             )
             n += 1
 
 
 class Windows(tk.Frame):
     """
     Class to define a frame of multiple windows as a gridded
     block that can be placed easily within a container widget.
     Also defines binning factors and the number of active windows.
     """
 
-    def __init__(self, master, xss, xsmins, xsmaxs, yss, ysmins, ysmaxs,
-                 nxs, nys, xbfac, ybfac, checker):
+    def __init__(
+        self,
+        master,
+        xss,
+        xsmins,
+        xsmaxs,
+        yss,
+        ysmins,
+        ysmaxs,
+        nxs,
+        nys,
+        xbfac,
+        ybfac,
+        checker,
+    ):
         """
         Arguments:
 
           master :
             container widget
 
           xss, xsmins, xsmaxs :
@@ -4069,88 +4348,90 @@
             to any changes made to the values stored in a Window. Can be None.
         """
 
         nwin = len(xss)
         checks = (xss, xsmins, xsmaxs, yss, ysmins, ysmaxs, nxs, nys)
         for check in checks:
             if nwin != len(check):
-                raise DriverError('drivers.Windows.__init__: ' +
-                                  'conflict array lengths amonst inputs')
+                raise DriverError(
+                    "drivers.Windows.__init__: "
+                    + "conflict array lengths amonst inputs"
+                )
 
         tk.Frame.__init__(self, master)
 
         # top part contains the binning factors and the number
         # of active windows
         top = tk.Frame(self)
         top.pack(anchor=tk.W)
 
-        tk.Label(top, text='Binning factors (X x Y): ').grid(
-            row=0, column=0, sticky=tk.W)
+        tk.Label(top, text="Binning factors (X x Y): ").grid(
+            row=0, column=0, sticky=tk.W
+        )
 
         xyframe = tk.Frame(top)
         self.xbin = ListInt(xyframe, xbfac[0], xbfac, checker, width=2)
         self.xbin.pack(side=tk.LEFT)
-        tk.Label(xyframe, text=' x ').pack(side=tk.LEFT)
+        tk.Label(xyframe, text=" x ").pack(side=tk.LEFT)
         self.ybin = ListInt(xyframe, ybfac[0], ybfac, checker, width=2)
         self.ybin.pack(side=tk.LEFT)
         xyframe.grid(row=0, column=1, sticky=tk.W)
 
         # Second row: number of windows
         self.nwin = RangedInt(top, 1, 1, nwin, checker, False, width=2)
         row = 1
         if nwin > 1:
-            tk.Label(top, text='Number of windows').grid(row=row, column=0,
-                                                         sticky=tk.W)
+            tk.Label(top, text="Number of windows").grid(row=row, column=0, sticky=tk.W)
             self.nwin.grid(row=1, column=1, sticky=tk.W, pady=2)
             row += 1
 
         # bottom part contains the window settings
         bottom = tk.Frame(self)
         bottom.pack(anchor=tk.W)
 
         # top row
-        tk.Label(bottom, text='xs').grid(row=row, column=1, ipady=5, sticky=tk.S)
-        tk.Label(bottom, text='ys').grid(row=row, column=2, ipady=5, sticky=tk.S)
-        tk.Label(bottom, text='nx').grid(row=row, column=3, ipady=5, sticky=tk.S)
-        tk.Label(bottom, text='ny').grid(row=row, column=4, ipady=5, sticky=tk.S)
+        tk.Label(bottom, text="xs").grid(row=row, column=1, ipady=5, sticky=tk.S)
+        tk.Label(bottom, text="ys").grid(row=row, column=2, ipady=5, sticky=tk.S)
+        tk.Label(bottom, text="nx").grid(row=row, column=3, ipady=5, sticky=tk.S)
+        tk.Label(bottom, text="ny").grid(row=row, column=4, ipady=5, sticky=tk.S)
 
         self.label, self.xs, self.ys, self.nx, self.ny = [], [], [], [], []
         nr = 0
         row += 1
         for xs, xsmin, xsmax, ys, ysmin, ysmax, nx, ny in zip(*checks):
-
             # create
             if nwin == 1:
-                self.label.append(tk.Label(bottom, text='Window: '))
+                self.label.append(tk.Label(bottom, text="Window: "))
             else:
-                self.label.append(
-                    tk.Label(bottom, text='Window ' + str(nr+1) + ': '))
+                self.label.append(tk.Label(bottom, text="Window " + str(nr + 1) + ": "))
 
-            self.xs.append(
-                RangedInt(bottom, xs, xsmin, xsmax, checker, True, width=4))
-            self.ys.append(
-                RangedInt(bottom, ys, ysmin, ysmax, checker, True, width=4))
+            self.xs.append(RangedInt(bottom, xs, xsmin, xsmax, checker, True, width=4))
+            self.ys.append(RangedInt(bottom, ys, ysmin, ysmax, checker, True, width=4))
             self.nx.append(
-                RangedMint(bottom, nx, 1, xsmax-xsmin+1,
-                           self.xbin, checker, True, width=4))
+                RangedMint(
+                    bottom, nx, 1, xsmax - xsmin + 1, self.xbin, checker, True, width=4
+                )
+            )
             self.ny.append(
-                RangedMint(bottom, ny, 1, ysmax-ysmin+1,
-                           self.ybin, checker, True, width=4))
+                RangedMint(
+                    bottom, ny, 1, ysmax - ysmin + 1, self.ybin, checker, True, width=4
+                )
+            )
 
             # arrange
             self.label[-1].grid(row=row, column=0)
             self.xs[-1].grid(row=row, column=1)
             self.ys[-1].grid(row=row, column=2)
             self.nx[-1].grid(row=row, column=3)
             self.ny[-1].grid(row=row, column=4)
 
             row += 1
             nr += 1
 
-        self.sbutt = ActButton(bottom, 5, self.sync, text='Sync')
+        self.sbutt = ActButton(bottom, 5, self.sync, text="Sync")
         self.sbutt.grid(row=row, column=0, columnspan=5, pady=6, sticky=tk.W)
         self.frozen = False
 
     def check(self):
         """
         Checks the values of the windows. If any problems are found,
         it flags them by changing the background colour. Only active
@@ -4164,86 +4445,87 @@
 
         xbin = self.xbin.value()
         ybin = self.ybin.value()
         nwin = self.nwin.value()
 
         # individual window checks
         g = get_root(self).globals
-        for xsw, ysw, nxw, nyw in \
-                zip(self.xs[:nwin], self.ys[:nwin],
-                    self.nx[:nwin], self.ny[:nwin]):
-
-            xsw.config(bg=g.COL['main'])
-            ysw.config(bg=g.COL['main'])
-            nxw.config(bg=g.COL['main'])
-            nyw.config(bg=g.COL['main'])
+        for xsw, ysw, nxw, nyw in zip(
+            self.xs[:nwin], self.ys[:nwin], self.nx[:nwin], self.ny[:nwin]
+        ):
+            xsw.config(bg=g.COL["main"])
+            ysw.config(bg=g.COL["main"])
+            nxw.config(bg=g.COL["main"])
+            nyw.config(bg=g.COL["main"])
             status = status if xsw.ok() else False
             status = status if ysw.ok() else False
             status = status if nxw.ok() else False
             status = status if nyw.ok() else False
             xs = xsw.value()
             ys = ysw.value()
             nx = nxw.value()
             ny = nyw.value()
 
             # Are unbinned dimensions consistent with binning factors?
             if nx is None or nx % xbin != 0:
-                nxw.config(bg=g.COL['error'])
+                nxw.config(bg=g.COL["error"])
                 status = False
 
             if ny is None or ny % ybin != 0:
-                nyw.config(bg=g.COL['error'])
+                nyw.config(bg=g.COL["error"])
                 status = False
 
             # Are the windows synchronised? This means that they
             # would be consistent with the pixels generated were
             # the whole CCD to be binned by the same factors
             # If relevant values are not set, we count that as
             # "synced" because the purpose of this is to enable
             # / disable the sync button and we don't want it to be
             # enabled just because xs or ys are not set.
-            if (xs is not None and ys is not None and nx is not None and ny is not None):
-                if (xs < 1025 and ((xs - 1) % xbin != 0 or (ys - 1) % ybin != 0)
-                        or ((xs-1025) % xbin != 0 or (ys - 1) % ybin != 0)):
+            if xs is not None and ys is not None and nx is not None and ny is not None:
+                if (
+                    xs < 1025
+                    and ((xs - 1) % xbin != 0 or (ys - 1) % ybin != 0)
+                    or ((xs - 1025) % xbin != 0 or (ys - 1) % ybin != 0)
+                ):
                     synced = False
 
             # Range checks
             if xs is None or nx is None or xs + nx - 1 > xsw.imax:
-                xsw.config(bg=g.COL['error'])
+                xsw.config(bg=g.COL["error"])
                 status = False
 
             if ys is None or ny is None or ys + ny - 1 > ysw.imax:
-                ysw.config(bg=g.COL['error'])
+                ysw.config(bg=g.COL["error"])
                 status = False
 
         # Overlap checks. Compare each window with the next one, requiring
         # no y overlap and that the second is higher than the first
         if status:
             n1 = 0
-            for ysw1, nyw1 in zip(self.ys[:nwin-1], self.ny[:nwin-1]):
-
+            for ysw1, nyw1 in zip(self.ys[: nwin - 1], self.ny[: nwin - 1]):
                 ys1 = ysw1.value()
                 ny1 = nyw1.value()
 
                 n1 += 1
                 ysw2 = self.ys[n1]
 
                 ys2 = ysw2.value()
 
                 if ys2 < ys1 + ny1:
-                    ysw2.config(bg=g.COL['error'])
+                    ysw2.config(bg=g.COL["error"])
                     status = False
 
         if synced:
-            self.sbutt.config(bg=g.COL['main'])
+            self.sbutt.config(bg=g.COL["main"])
             self.sbutt.disable()
         else:
             if not self.frozen:
                 self.sbutt.enable()
-            self.sbutt.config(bg=g.COL['warn'])
+            self.sbutt.config(bg=g.COL["warn"])
 
         return status
 
     def sync(self, *args):
         """
         Synchronise the settings. This means that the pixel start
         values are shifted downwards so that they are synchronised
@@ -4252,35 +4534,34 @@
         """
         xbin = self.xbin.value()
         ybin = self.ybin.value()
         n = 0
         for xs, ys, nx, ny in self:
             if xbin > 1 and xs % xbin != 1:
                 if xs < 1025:
-                    xs = xbin*((xs-1)//xbin)+1
+                    xs = xbin * ((xs - 1) // xbin) + 1
                 else:
-                    xs = xbin*((xs-1025)//xbin)+1025
+                    xs = xbin * ((xs - 1025) // xbin) + 1025
                 self.xs[n].set(xs)
 
             if ybin > 1 and ys % ybin != 1:
-                ys = ybin*((ys-1)//ybin)+1
+                ys = ybin * ((ys - 1) // ybin) + 1
                 self.ys[n].set(ys)
 
             n += 1
 
         g = get_root(self).globals
-        self.sbutt.config(bg=g.COL['main'])
-        self.sbutt.config(state='disable')
+        self.sbutt.config(bg=g.COL["main"])
+        self.sbutt.config(state="disable")
 
     def freeze(self):
         """
         Freeze all settings so they can't be altered
         """
-        for xs, ys, nx, ny in \
-                zip(self.xs, self.ys, self.nx, self.ny):
+        for xs, ys, nx, ny in zip(self.xs, self.ys, self.nx, self.ny):
             xs.disable()
             ys.disable()
             nx.disable()
             ny.disable()
         self.nwin.disable()
         self.xbin.disable()
         self.ybin.disable()
@@ -4296,27 +4577,35 @@
         self.check()
 
     def enable(self):
         """
         Enables all settings
         """
         nwin = self.nwin.value()
-        for label, xs, ys, nx, ny in \
-                zip(self.label[:nwin], self.xs[:nwin], self.ys[:nwin],
-                    self.nx[:nwin], self.ny[:nwin]):
-            label.config(state='normal')
+        for label, xs, ys, nx, ny in zip(
+            self.label[:nwin],
+            self.xs[:nwin],
+            self.ys[:nwin],
+            self.nx[:nwin],
+            self.ny[:nwin],
+        ):
+            label.config(state="normal")
             xs.enable()
             ys.enable()
             nx.enable()
             ny.enable()
 
-        for label, xs, ys, nx, ny in \
-                zip(self.label[nwin:], self.xs[nwin:], self.ys[nwin:],
-                    self.nx[nwin:], self.ny[nwin:]):
-            label.config(state='disable')
+        for label, xs, ys, nx, ny in zip(
+            self.label[nwin:],
+            self.xs[nwin:],
+            self.ys[nwin:],
+            self.nx[nwin:],
+            self.ny[nwin:],
+        ):
+            label.config(state="disable")
             xs.disable()
             ys.disable()
             nx.disable()
             ny.disable()
 
         self.nwin.enable()
         self.xbin.enable()
@@ -4327,10 +4616,14 @@
         """
         Generator to allow looping through through the window values.
         Successive calls return xs, ys, nx, ny for each window
         """
         n = 0
         nwin = self.nwin.value()
         while n < nwin:
-            yield (self.xs[n].value(), self.ys[n].value(),
-                   self.nx[n].value(), self.ny[n].value())
+            yield (
+                self.xs[n].value(),
+                self.ys[n].value(),
+                self.nx[n].value(),
+                self.ny[n].value(),
+            )
             n += 1
```

### Comparing `hcam_widgets-1.0.3/hcam_widgets.egg-info/PKG-INFO` & `hcam_widgets-1.1.0/hcam_widgets.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: hcam-widgets
-Version: 1.0.3
+Version: 1.1.0
 Summary: Common Tkinter widgets for HiPerCAM
 Home-page: https://github.com/HiPERCAM/hcam_widgets
+Download-URL: https://github.com/HiPERCAM/hcam_widgets/archive/v1.1.0.tar.gz
 Author: Stuart Littlefair
 Author-email: s.littlefair@shef.ac.uk
 License: MIT license
-Download-URL: https://github.com/HiPERCAM/hcam_widgets/archive/v1.0.3.tar.gz
 Keywords: hcam_widgets
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
@@ -87,9 +86,7 @@
 History
 =======
 
 0.1.0 (2017-02-11)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `hcam_widgets-1.0.3/hcam_widgets.egg-info/SOURCES.txt` & `hcam_widgets-1.1.0/hcam_widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.0.3/setup.py` & `hcam_widgets-1.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,66 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 import glob
 import os
 
-with open('README.rst') as readme_file:
+with open("README.rst") as readme_file:
     readme = readme_file.read()
 
-with open('HISTORY.rst') as history_file:
+with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
 requirements = [
-    'astropy', 'requests', 'twisted', 'hcam_devices>=0.3.0', 'matplotlib',
-    'scipy', 'autobahn'
+    "astropy",
+    "requests",
+    "twisted",
+    "hcam_devices>=1.0.0",
+    "matplotlib",
+    "scipy",
+    "autobahn",
 ]
 
 test_requirements = [
     # TODO: put package test requirements here
 ]
 
 # Treat everything in scripts except README.rst as a script to be installed
-scripts = [fname for fname in glob.glob(os.path.join('scripts', '*'))
-           if os.path.basename(fname) != 'README.rst']
+scripts = [
+    fname
+    for fname in glob.glob(os.path.join("scripts", "*"))
+    if os.path.basename(fname) != "README.rst"
+]
 
 setup(
-    name='hcam_widgets',
-    version='1.0.3',
+    name="hcam_widgets",
+    version="1.1.0",
     description="Common Tkinter widgets for HiPerCAM",
-    long_description=readme + '\n\n' + history,
+    long_description=readme + "\n\n" + history,
     author="Stuart Littlefair",
-    author_email='s.littlefair@shef.ac.uk',
-    url='https://github.com/HiPERCAM/hcam_widgets',
-    download_url='https://github.com/HiPERCAM/hcam_widgets/archive/v1.0.3.tar.gz',
-    packages=[
-        'hcam_widgets',
-        'hcam_widgets.compo',
-        'hcam_widgets.hardware'
-    ],
-    package_dir={'hcam_widgets':
-                 'hcam_widgets'},
+    author_email="s.littlefair@shef.ac.uk",
+    url="https://github.com/HiPERCAM/hcam_widgets",
+    download_url="https://github.com/HiPERCAM/hcam_widgets/archive/v1.1.0.tar.gz",
+    packages=["hcam_widgets", "hcam_widgets.compo", "hcam_widgets.hardware"],
+    package_dir={"hcam_widgets": "hcam_widgets"},
     include_package_data=True,
     install_requires=requirements,
     license="MIT license",
     zip_safe=False,
-    keywords='hcam_widgets',
+    keywords="hcam_widgets",
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
+        "Development Status :: 2 - Pre-Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Natural Language :: English",
         "Programming Language :: Python :: 2",
-        'Programming Language :: Python :: 2.6',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
+        "Programming Language :: Python :: 2.6",
+        "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.3",
+        "Programming Language :: Python :: 3.4",
+        "Programming Language :: Python :: 3.5",
     ],
-    test_suite='tests',
-    tests_require=test_requirements
+    test_suite="tests",
+    tests_require=test_requirements,
 )
```

