# Comparing `tmp/jampy-7.2.0.tar.gz` & `tmp/jampy-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jampy-7.2.0.tar", last modified: Thu Jul 20 18:41:23 2023, max compression
+gzip compressed data, was "jampy-7.2.1.tar", last modified: Fri Jul 21 09:33:44 2023, max compression
```

## Comparing `jampy-7.2.0.tar` & `jampy-7.2.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 18:41:23.656146 jampy-7.2.0/
--rw-rw-rw-   0        0        0    50553 2023-07-20 18:41:23.656146 jampy-7.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-20 18:41:23.598747 jampy-7.2.0/jampy/
--rw-rw-rw-   0        0        0    13168 2023-07-20 18:41:14.000000 jampy-7.2.0/jampy/CHANGELOG.rst
--rw-rw-rw-   0        0        0      398 2023-07-07 13:06:09.000000 jampy-7.2.0/jampy/LICENSE.txt
--rw-rw-rw-   0        0        0     3564 2022-10-02 22:25:04.000000 jampy-7.2.0/jampy/README.rst
--rw-rw-rw-   0        0        0       23 2023-07-20 18:40:10.000000 jampy-7.2.0/jampy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 18:41:23.656146 jampy-7.2.0/jampy/examples/
--rw-rw-rw-   0        0        0       36 2018-04-16 16:12:03.000000 jampy-7.2.0/jampy/examples/__init__.py
--rw-rw-rw-   0        0        0     1019 2022-02-07 11:29:21.000000 jampy-7.2.0/jampy/examples/cappellari2020_table1.txt
--rw-rw-rw-   0        0        0     3060 2023-06-15 16:06:10.000000 jampy-7.2.0/jampy/examples/jam_axi_intr_example.py
--rw-rw-rw-   0        0        0     4524 2023-07-16 14:17:21.000000 jampy-7.2.0/jampy/examples/jam_axi_proj_example.py
--rw-rw-rw-   0        0        0     6915 2023-06-05 17:03:23.000000 jampy-7.2.0/jampy/examples/jam_black_hole_bayes_example.py
--rw-rw-rw-   0        0        0    10298 2023-06-05 17:02:41.000000 jampy-7.2.0/jampy/examples/jam_dark_halo_bayes_example.py
--rw-rw-rw-   0        0        0    10196 2023-06-21 10:58:03.000000 jampy-7.2.0/jampy/examples/jam_hernquist_model_example.py
--rw-rw-rw-   0        0        0     8544 2018-05-01 13:45:20.000000 jampy-7.2.0/jampy/examples/jam_mock_kinematics_black_hole.txt
--rw-rw-rw-   0        0        0     8592 2021-12-21 19:35:32.000000 jampy-7.2.0/jampy/examples/jam_mock_kinematics_dark_halo.txt
--rw-rw-rw-   0        0        0     2592 2023-05-31 18:23:57.000000 jampy-7.2.0/jampy/examples/jam_sph_proj_example.py
--rw-rw-rw-   0        0        0     2195 2023-06-05 17:01:53.000000 jampy-7.2.0/jampy/examples/mge_vcirc_example.py
--rw-rw-rw-   0        0        0    35745 2023-06-21 12:51:09.000000 jampy-7.2.0/jampy/jam_axi_intr.py
--rw-rw-rw-   0        0        0    48705 2023-06-18 18:06:40.000000 jampy-7.2.0/jampy/jam_axi_proj.py
--rw-rw-rw-   0        0        0     5438 2023-07-05 09:54:32.000000 jampy-7.2.0/jampy/jam_axi_sersic_mass.py
--rw-rw-rw-   0        0        0     8141 2023-05-31 18:20:50.000000 jampy-7.2.0/jampy/jam_sph_intr.py
--rw-rw-rw-   0        0        0    29072 2023-05-31 18:20:50.000000 jampy-7.2.0/jampy/jam_sph_proj.py
--rw-rw-rw-   0        0        0     6547 2022-10-09 17:30:15.000000 jampy-7.2.0/jampy/mge_half_light_isophote.py
--rw-rw-rw-   0        0        0     3568 2019-10-24 18:03:59.000000 jampy-7.2.0/jampy/mge_radial_density.py
--rw-rw-rw-   0        0        0     3173 2019-06-12 10:26:52.000000 jampy-7.2.0/jampy/mge_radial_mass.py
--rw-rw-rw-   0        0        0     6845 2023-01-01 15:05:41.000000 jampy-7.2.0/jampy/mge_vcirc.py
--rw-rw-rw-   0        0        0    19470 2023-06-13 12:02:24.000000 jampy-7.2.0/jampy/quad1d.py
--rw-rw-rw-   0        0        0    13046 2023-06-18 17:52:36.000000 jampy-7.2.0/jampy/quad2d.py
-drwxrwxrwx   0        0        0        0 2023-07-20 18:41:23.630007 jampy-7.2.0/jampy.egg-info/
--rw-rw-rw-   0        0        0    50553 2023-07-20 18:41:23.000000 jampy-7.2.0/jampy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      962 2023-07-20 18:41:23.000000 jampy-7.2.0/jampy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 18:41:23.000000 jampy-7.2.0/jampy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-07-20 18:41:23.000000 jampy-7.2.0/jampy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-20 18:41:23.000000 jampy-7.2.0/jampy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-20 18:41:23.000000 jampy-7.2.0/jampy.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-07-20 18:41:23.656146 jampy-7.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1750 2021-06-24 13:30:54.000000 jampy-7.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:33:44.901323 jampy-7.2.1/
+-rw-rw-rw-   0        0        0    50985 2023-07-21 09:33:44.901323 jampy-7.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-21 09:33:44.752192 jampy-7.2.1/jampy/
+-rw-rw-rw-   0        0        0    13594 2023-07-21 09:32:52.000000 jampy-7.2.1/jampy/CHANGELOG.rst
+-rw-rw-rw-   0        0        0      398 2023-07-07 13:06:09.000000 jampy-7.2.1/jampy/LICENSE.txt
+-rw-rw-rw-   0        0        0     3564 2022-10-02 22:25:04.000000 jampy-7.2.1/jampy/README.rst
+-rw-rw-rw-   0        0        0       23 2023-07-21 09:33:33.000000 jampy-7.2.1/jampy/__init__.py
+-rw-rw-rw-   0        0        0     2749 2023-07-21 09:30:36.000000 jampy-7.2.1/jampy/cosmology_distance.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:33:44.901323 jampy-7.2.1/jampy/examples/
+-rw-rw-rw-   0        0        0       36 2018-04-16 16:12:03.000000 jampy-7.2.1/jampy/examples/__init__.py
+-rw-rw-rw-   0        0        0     1019 2022-02-07 11:29:21.000000 jampy-7.2.1/jampy/examples/cappellari2020_table1.txt
+-rw-rw-rw-   0        0        0     3060 2023-06-15 16:06:10.000000 jampy-7.2.1/jampy/examples/jam_axi_intr_example.py
+-rw-rw-rw-   0        0        0     4524 2023-07-16 14:17:21.000000 jampy-7.2.1/jampy/examples/jam_axi_proj_example.py
+-rw-rw-rw-   0        0        0     6915 2023-06-05 17:03:23.000000 jampy-7.2.1/jampy/examples/jam_black_hole_bayes_example.py
+-rw-rw-rw-   0        0        0    10298 2023-06-05 17:02:41.000000 jampy-7.2.1/jampy/examples/jam_dark_halo_bayes_example.py
+-rw-rw-rw-   0        0        0    10196 2023-06-21 10:58:03.000000 jampy-7.2.1/jampy/examples/jam_hernquist_model_example.py
+-rw-rw-rw-   0        0        0     8544 2018-05-01 13:45:20.000000 jampy-7.2.1/jampy/examples/jam_mock_kinematics_black_hole.txt
+-rw-rw-rw-   0        0        0     8592 2021-12-21 19:35:32.000000 jampy-7.2.1/jampy/examples/jam_mock_kinematics_dark_halo.txt
+-rw-rw-rw-   0        0        0     2592 2023-05-31 18:23:57.000000 jampy-7.2.1/jampy/examples/jam_sph_proj_example.py
+-rw-rw-rw-   0        0        0     2195 2023-06-05 17:01:53.000000 jampy-7.2.1/jampy/examples/mge_vcirc_example.py
+-rw-rw-rw-   0        0        0    35745 2023-06-21 12:51:09.000000 jampy-7.2.1/jampy/jam_axi_intr.py
+-rw-rw-rw-   0        0        0    48705 2023-06-18 18:06:40.000000 jampy-7.2.1/jampy/jam_axi_proj.py
+-rw-rw-rw-   0        0        0     6600 2023-07-21 09:08:07.000000 jampy-7.2.1/jampy/jam_axi_sersic_mass.py
+-rw-rw-rw-   0        0        0     8141 2023-05-31 18:20:50.000000 jampy-7.2.1/jampy/jam_sph_intr.py
+-rw-rw-rw-   0        0        0    29072 2023-05-31 18:20:50.000000 jampy-7.2.1/jampy/jam_sph_proj.py
+-rw-rw-rw-   0        0        0     6547 2022-10-09 17:30:15.000000 jampy-7.2.1/jampy/mge_half_light_isophote.py
+-rw-rw-rw-   0        0        0     3568 2019-10-24 18:03:59.000000 jampy-7.2.1/jampy/mge_radial_density.py
+-rw-rw-rw-   0        0        0     3173 2019-06-12 10:26:52.000000 jampy-7.2.1/jampy/mge_radial_mass.py
+-rw-rw-rw-   0        0        0     6845 2023-01-01 15:05:41.000000 jampy-7.2.1/jampy/mge_vcirc.py
+-rw-rw-rw-   0        0        0    19470 2023-06-13 12:02:24.000000 jampy-7.2.1/jampy/quad1d.py
+-rw-rw-rw-   0        0        0    13046 2023-06-18 17:52:36.000000 jampy-7.2.1/jampy/quad2d.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:33:44.791461 jampy-7.2.1/jampy.egg-info/
+-rw-rw-rw-   0        0        0    50985 2023-07-21 09:33:44.000000 jampy-7.2.1/jampy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2023-07-21 09:33:44.000000 jampy-7.2.1/jampy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 09:33:44.000000 jampy-7.2.1/jampy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-21 09:33:44.000000 jampy-7.2.1/jampy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-21 09:33:44.000000 jampy-7.2.1/jampy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-21 09:33:44.000000 jampy-7.2.1/jampy.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-07-21 09:33:44.901323 jampy-7.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1750 2021-06-24 13:30:54.000000 jampy-7.2.1/setup.py
```

### Comparing `jampy-7.2.0/PKG-INFO` & `jampy-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jampy
-Version: 7.2.0
+Version: 7.2.1
 Summary: JamPy: Jeans Anisotropic Models for Galactic Dynamics
 Home-page: https://purl.org/cappellari/software
 Author: Michele Cappellari
 Author-email: michele.cappellari@physics.ox.ac.uk
 License: Other/Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -799,20 +799,26 @@
 redistribute the code.
 
 ###########################################################################
 
 Changelog
 =========
 
-V7.2.0: MC, Oxford, 20 July 2023
+V7.2.1: MC, Oxford, 21 July 2023
     - ``jam_axi_intr``: Integrate all velocity components at the same time with
       a single call to the updated ``quad1d`` and ``quad2d``. Significant speedup.
     - ``quad1d``, ``quad2d``: Allow for integration of vector functions.
       All components are integrated over the same set of evaluation points.
     - ``jam_axi_proj``: Updated verbose output with more information.
+    - New procedure ``jam_axi_sersic_mass`` to efficiently compute dynamical
+      masses of axisymmetric galaxies described by Sersic profiles, while
+      allowing for seeing and aperture effects and assuming a given intrinsic
+      axial ratio. This is meant to be a simple and quick replacement for the
+      similar but less accurate virial estimators.
+    - New utility function ``cosmology_distance`` used in examples.
 
 V7.1.0: MC, Oxford, 5 June 2023
     - Separated computation for the black hole kinematics for both the
       cylindrically and spherically-aligned solutions. In both cases this
       removed one numerical quadrature. This is useful in extreme situations,
       when the minimum radius one wants to model around the black hole is orders
       of magnitude smaller than the smallest MGE Gaussian. This change
```

### Comparing `jampy-7.2.0/jampy/CHANGELOG.rst` & `jampy-7.2.1/jampy/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 
 Changelog
 =========
 
-V7.2.0: MC, Oxford, 20 July 2023
+V7.2.1: MC, Oxford, 21 July 2023
     - ``jam_axi_intr``: Integrate all velocity components at the same time with
       a single call to the updated ``quad1d`` and ``quad2d``. Significant speedup.
     - ``quad1d``, ``quad2d``: Allow for integration of vector functions.
       All components are integrated over the same set of evaluation points.
     - ``jam_axi_proj``: Updated verbose output with more information.
+    - New procedure ``jam_axi_sersic_mass`` to efficiently compute dynamical
+      masses of axisymmetric galaxies described by Sersic profiles, while
+      allowing for seeing and aperture effects and assuming a given intrinsic
+      axial ratio. This is meant to be a simple and quick replacement for the
+      similar but less accurate virial estimators.
+    - New utility function ``cosmology_distance`` used in examples.
 
 V7.1.0: MC, Oxford, 5 June 2023
     - Separated computation for the black hole kinematics for both the
       cylindrically and spherically-aligned solutions. In both cases this
       removed one numerical quadrature. This is useful in extreme situations,
       when the minimum radius one wants to model around the black hole is orders
       of magnitude smaller than the smallest MGE Gaussian. This change
```

### Comparing `jampy-7.2.0/jampy/README.rst` & `jampy-7.2.1/jampy/README.rst`

 * *Files identical despite different names*

### Comparing `jampy-7.2.0/jampy/examples/cappellari2020_table1.txt` & `jampy-7.2.1/jampy/examples/cappellari2020_table1.txt`

 * *Files identical despite different names*

### Comparing `jampy-7.2.0/jampy/examples/jam_axi_intr_example.py` & `jampy-7.2.1/jampy/examples/jam_axi_intr_example.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.0/jampy/examples/jam_axi_proj_example.py` & `jampy-7.2.1/jampy/examples/jam_axi_proj_example.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.0/jampy/examples/jam_black_hole_bayes_example.py` & `jampy-7.2.1/jampy/examples/jam_black_hole_bayes_example.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.0/jampy/examples/jam_dark_halo_bayes_example.py` & `jampy-7.2.1/jampy/examples/jam_dark_halo_bayes_example.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.0/jampy/examples/jam_hernquist_model_example.py` & `jampy-7.2.1/jampy/examples/jam_hernquist_model_example.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.0/jampy/examples/jam_mock_kinematics_black_hole.txt` & `jampy-7.2.1/jampy/examples/jam_mock_kinematics_black_hole.txt`

 * *Files identical despite different names*

### Comparing `jampy-7.2.0/jampy/examples/jam_mock_kinematics_dark_halo.txt` & `jampy-7.2.1/jampy/examples/jam_mock_kinematics_dark_halo.txt`

 * *Files identical despite different names*

### Comparing `jampy-7.2.0/jampy/examples/jam_sph_proj_example.py` & `jampy-7.2.1/jampy/examples/jam_sph_proj_example.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.0/jampy/examples/mge_vcirc_example.py` & `jampy-7.2.1/jampy/examples/mge_vcirc_example.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.0/jampy/jam_axi_intr.py` & `jampy-7.2.1/jampy/jam_axi_intr.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.0/jampy/jam_axi_proj.py` & `jampy-7.2.1/jampy/jam_axi_proj.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.0/jampy/jam_axi_sersic_mass.py` & `jampy-7.2.1/jampy/jam_axi_sersic_mass.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 """
-    Michele Cappellari, Oxford, 17 January 2022
-    Test for the paper on the virial coefficient by van der Wel and LEGA-C
-    https://ui.adsabs.harvard.edu/abs/2022ApJ...936....9V
+    Copyright (C) 2022-2023, Michele Cappellari
 
-    Modified 25 May 2022 for the paper by Jordan N Runco+22
-    https://ui.adsabs.harvard.edu/abs/2022MNRAS.517.4405R
+    E-mail: michele.cappellari_at_physics.ox.ac.uk
 
-    Made it a general procedure. MC, Oxford, 19 May 2023
+    Updated versions of the software are available from my web page
+    https://purl.org/cappellari/software
+
+    This software is provided as is without any warranty whatsoever.
+    Permission to use, for non-commercial purposes is granted.
+    Permission to modify for personal or internal use is granted,
+    provided this copyright and disclaimer are included unchanged
+    at the beginning of the file. All other rights are reserved.
+    In particular, redistribution of the code is not allowed.
+
+Changelog
+---------
+
+V1.0.0: Michele Cappellari, Oxford, 17 January 2022
+  - Written and tested as a separate procedure.
+Vx.x.x: Additional changes are documented in the CHANGELOG of the JamPy package.
 
 """
 
 import numpy as np
 import matplotlib.pyplot as plt
 
 from mgefit.mge_fit_1d import mge_fit_1d
 from jampy.jam_axi_proj import jam_axi_proj
+from jampy.cosmology_distance import angular_diameter_distance
 from plotbin.plot_velfield import plot_velfield
-from cosmology_distance import comoving_distance
 
 ###############################################################################
 
 def sersic_profile(n, rad):
     """ Sersic profile with rad=R/Re """
 
     # This has a maximum absolute error of 5.6e-4 in the interval n = [0.2, 16]
@@ -47,16 +59,16 @@
         plt.clf()
 
     return surf, sigma
 
 ###############################################################################
 
 def jam_axi_sersic_mass(re_maj_ser, n_ser, qobs, qintr, sigma_ap, sigma_ap_err,
-                        dxy_ap, sigma_psf, distance, beta=0, ngauss=16,
-                        lg_rmax=2, plot=True, quiet=False):
+                        dxy_ap, sigma_psf, distance, beta=0., ngauss=16,
+                        lg_rmax=2., plot=True, quiet=False):
     """
     Compute the mass M_Ser and uncertainty of a mass-follow-light Sersic model,
     at the given distance, that produces a given second moment of the stellar
     velocity sigma_ap inside a rectangular aperture of sides dxy_ap, assuming an
     intrinsic axial ratio qintr.
     Ideally, the Sersic model should be fitted to the photometry in a band close
     to the wavelength of the spectroscopic observations used to extract sigma_ap.
@@ -66,14 +78,17 @@
 
         (M/L)_e = M_Ser/L_Ser
 
     closely approximates the average mass-to-light ratio in the same band,
     within a sphere of radius R_e equal to the projected hal-light radius.
     (see Cappellari+13 https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C)
 
+    This procedure is meant as a simple replacement for the less accurate virial
+    mass estimators.
+
     """
     assert qintr <= qobs, "Must be `qintr <= qobs`"
     inc = np.degrees(np.arctan2(np.sqrt(1 - qobs**2), np.sqrt(qobs**2 - qintr**2)))
 
     # Adopt as reference an arbitrary galaxy mass and find how much I need to
     # scale it to match the observed sigma
     mass = 1e11
@@ -112,23 +127,32 @@
         plt.title("JAM $V_{\\rm rms}$")
         plt.pause(1)
 
     return lg_mjam, d_lg_mjam
 
 ###############################################################################
 
-if __name__ == '__main__':
+def jam_axi_sersic_mass_example():
+    """Usage example for jam_axi_sersic_mass"""
 
+    # Input parameters
     dxy_ap = [1.1, 0.7]     # sides of rectangular aperture in arcsec
-    n_ser = 2.57
-    qobs = 0.656
+    n_ser = 2.57            # Sersic exponent (e.g. n = 4 --> de Vaucouleurs)
+    qobs = 0.656            # Observed axial ratio of the fitted Seric model
     qintr = 0.4             # assumed intrinsic axial ratio
-    beta = 0.2
-    re_maj_ser = 0.67       # arcsec
-    sigma_psf = 0.5/2.355
+    beta = 0.2              # anisotropy beta = 1 - (sig_z/sig_R)^2
+    re_maj_ser = 0.67       # arcsec. Semimajor axis half-light ellipse of Sersic model
+    sigma_psf = 0.5/2.355   # dispersion of the PSF in arcsec
     redshift = 0.8          # galaxy redshift
-    comdist = comoving_distance(redshift)
-    dist_ang = comdist/(1 + redshift)  # D_A angular size distance
-    sigma_ap = 166  # km/s
-    sigma_ap_err = 19
+    sigma_ap = 166          # km/s. Observed second velocity moment (sigma)
+    sigma_ap_err = 19       # km/s. 1sigma uncertainty on sigma_ap
+
+    # Computation
+    dist_ang = angular_diameter_distance(redshift)  # D_A angular diameter distance
     lg_mjam = jam_axi_sersic_mass(re_maj_ser, n_ser, qobs, qintr, sigma_ap,
                                   sigma_ap_err, dxy_ap, sigma_psf, dist_ang, beta=beta)
+
+###############################################################################
+
+if __name__ == '__main__':
+
+    jam_axi_sersic_mass_example()
```

### Comparing `jampy-7.2.0/jampy/jam_sph_intr.py` & `jampy-7.2.1/jampy/jam_sph_intr.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.0/jampy/jam_sph_proj.py` & `jampy-7.2.1/jampy/jam_sph_proj.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.0/jampy/mge_half_light_isophote.py` & `jampy-7.2.1/jampy/mge_half_light_isophote.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.0/jampy/mge_radial_density.py` & `jampy-7.2.1/jampy/mge_radial_density.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.0/jampy/mge_radial_mass.py` & `jampy-7.2.1/jampy/mge_radial_mass.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.0/jampy/mge_vcirc.py` & `jampy-7.2.1/jampy/mge_vcirc.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.0/jampy/quad1d.py` & `jampy-7.2.1/jampy/quad1d.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.0/jampy/quad2d.py` & `jampy-7.2.1/jampy/quad2d.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.0/jampy.egg-info/PKG-INFO` & `jampy-7.2.1/jampy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jampy
-Version: 7.2.0
+Version: 7.2.1
 Summary: JamPy: Jeans Anisotropic Models for Galactic Dynamics
 Home-page: https://purl.org/cappellari/software
 Author: Michele Cappellari
 Author-email: michele.cappellari@physics.ox.ac.uk
 License: Other/Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -799,20 +799,26 @@
 redistribute the code.
 
 ###########################################################################
 
 Changelog
 =========
 
-V7.2.0: MC, Oxford, 20 July 2023
+V7.2.1: MC, Oxford, 21 July 2023
     - ``jam_axi_intr``: Integrate all velocity components at the same time with
       a single call to the updated ``quad1d`` and ``quad2d``. Significant speedup.
     - ``quad1d``, ``quad2d``: Allow for integration of vector functions.
       All components are integrated over the same set of evaluation points.
     - ``jam_axi_proj``: Updated verbose output with more information.
+    - New procedure ``jam_axi_sersic_mass`` to efficiently compute dynamical
+      masses of axisymmetric galaxies described by Sersic profiles, while
+      allowing for seeing and aperture effects and assuming a given intrinsic
+      axial ratio. This is meant to be a simple and quick replacement for the
+      similar but less accurate virial estimators.
+    - New utility function ``cosmology_distance`` used in examples.
 
 V7.1.0: MC, Oxford, 5 June 2023
     - Separated computation for the black hole kinematics for both the
       cylindrically and spherically-aligned solutions. In both cases this
       removed one numerical quadrature. This is useful in extreme situations,
       when the minimum radius one wants to model around the black hole is orders
       of magnitude smaller than the smallest MGE Gaussian. This change
```

### Comparing `jampy-7.2.0/jampy.egg-info/SOURCES.txt` & `jampy-7.2.1/jampy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 setup.py
 jampy/CHANGELOG.rst
 jampy/LICENSE.txt
 jampy/README.rst
 jampy/__init__.py
+jampy/cosmology_distance.py
 jampy/jam_axi_intr.py
 jampy/jam_axi_proj.py
 jampy/jam_axi_sersic_mass.py
 jampy/jam_sph_intr.py
 jampy/jam_sph_proj.py
 jampy/mge_half_light_isophote.py
 jampy/mge_radial_density.py
```

### Comparing `jampy-7.2.0/setup.py` & `jampy-7.2.1/setup.py`

 * *Files identical despite different names*

