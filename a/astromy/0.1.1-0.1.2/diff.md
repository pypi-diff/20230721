# Comparing `tmp/astromy-0.1.1.tar.gz` & `tmp/astromy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astromy-0.1.1.tar", last modified: Mon Feb 27 13:18:33 2023, max compression
+gzip compressed data, was "astromy-0.1.2.tar", last modified: Fri Jul 21 18:12:48 2023, max compression
```

## Comparing `astromy-0.1.1.tar` & `astromy-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 mingyu     (501) staff       (20)        0 2023-02-27 13:18:33.020991 astromy-0.1.1/
--rw-r--r--   0 mingyu     (501) staff       (20)     1060 2022-10-12 11:37:53.000000 astromy-0.1.1/LICENSE
--rw-r--r--   0 mingyu     (501) staff       (20)       26 2022-10-12 11:37:53.000000 astromy-0.1.1/MANIFEST.in
--rw-r--r--   0 mingyu     (501) staff       (20)      670 2023-02-27 13:18:33.020828 astromy-0.1.1/PKG-INFO
--rw-r--r--   0 mingyu     (501) staff       (20)       43 2023-02-27 13:08:05.000000 astromy-0.1.1/README.md
-drwxr-xr-x   0 mingyu     (501) staff       (20)        0 2023-02-27 13:18:33.020016 astromy-0.1.1/astromy/
--rw-r--r--   0 mingyu     (501) staff       (20)      544 2023-02-27 13:12:12.000000 astromy-0.1.1/astromy/__init__.py
--rw-r--r--   0 mingyu     (501) staff       (20)      389 2023-02-27 13:15:14.000000 astromy-0.1.1/astromy/__version__.py
--rw-r--r--   0 mingyu     (501) staff       (20)     8475 2023-02-27 13:07:02.000000 astromy-0.1.1/astromy/astromatic.py
--rw-r--r--   0 mingyu     (501) staff       (20)     1049 2022-10-12 11:37:53.000000 astromy-0.1.1/astromy/catalog.py
--rw-r--r--   0 mingyu     (501) staff       (20)     1264 2022-10-12 14:36:25.000000 astromy-0.1.1/astromy/cube.py
--rw-r--r--   0 mingyu     (501) staff       (20)     7096 2023-02-27 13:14:31.000000 astromy-0.1.1/astromy/image.py
--rw-r--r--   0 mingyu     (501) staff       (20)     2211 2022-11-17 15:28:44.000000 astromy-0.1.1/astromy/wcs.py
-drwxr-xr-x   0 mingyu     (501) staff       (20)        0 2023-02-27 13:18:33.020628 astromy-0.1.1/astromy.egg-info/
--rw-r--r--   0 mingyu     (501) staff       (20)      670 2023-02-27 13:18:32.000000 astromy-0.1.1/astromy.egg-info/PKG-INFO
--rw-r--r--   0 mingyu     (501) staff       (20)      324 2023-02-27 13:18:32.000000 astromy-0.1.1/astromy.egg-info/SOURCES.txt
--rw-r--r--   0 mingyu     (501) staff       (20)        1 2023-02-27 13:18:32.000000 astromy-0.1.1/astromy.egg-info/dependency_links.txt
--rw-r--r--   0 mingyu     (501) staff       (20)       78 2023-02-27 13:18:32.000000 astromy-0.1.1/astromy.egg-info/requires.txt
--rw-r--r--   0 mingyu     (501) staff       (20)        8 2023-02-27 13:18:32.000000 astromy-0.1.1/astromy.egg-info/top_level.txt
--rw-r--r--   0 mingyu     (501) staff       (20)       38 2023-02-27 13:18:33.021042 astromy-0.1.1/setup.cfg
--rw-r--r--   0 mingyu     (501) staff       (20)     3883 2023-02-27 13:18:08.000000 astromy-0.1.1/setup.py
+drwxr-xr-x   0 mingyu     (501) staff       (20)        0 2023-07-21 18:12:48.134799 astromy-0.1.2/
+-rw-r--r--   0 mingyu     (501) staff       (20)     1060 2022-10-12 11:37:53.000000 astromy-0.1.2/LICENSE
+-rw-r--r--   0 mingyu     (501) staff       (20)       26 2022-10-12 11:37:53.000000 astromy-0.1.2/MANIFEST.in
+-rw-r--r--   0 mingyu     (501) staff       (20)      670 2023-07-21 18:12:48.134618 astromy-0.1.2/PKG-INFO
+-rw-r--r--   0 mingyu     (501) staff       (20)       43 2023-02-27 13:08:05.000000 astromy-0.1.2/README.md
+drwxr-xr-x   0 mingyu     (501) staff       (20)        0 2023-07-21 18:12:48.133604 astromy-0.1.2/astromy/
+-rw-r--r--   0 mingyu     (501) staff       (20)      544 2023-03-25 08:53:36.000000 astromy-0.1.2/astromy/__init__.py
+-rw-r--r--   0 mingyu     (501) staff       (20)      389 2023-07-21 18:12:14.000000 astromy-0.1.2/astromy/__version__.py
+-rw-r--r--   0 mingyu     (501) staff       (20)     8475 2023-02-27 13:07:02.000000 astromy-0.1.2/astromy/astromatic.py
+-rw-r--r--   0 mingyu     (501) staff       (20)     1049 2022-10-12 11:37:53.000000 astromy-0.1.2/astromy/catalog.py
+-rw-r--r--   0 mingyu     (501) staff       (20)     1946 2023-03-08 13:31:58.000000 astromy-0.1.2/astromy/cube.py
+-rw-r--r--   0 mingyu     (501) staff       (20)     9535 2023-05-31 13:05:01.000000 astromy-0.1.2/astromy/image.py
+-rw-r--r--   0 mingyu     (501) staff       (20)     3314 2023-02-27 16:43:41.000000 astromy-0.1.2/astromy/line.py
+-rw-r--r--   0 mingyu     (501) staff       (20)     5557 2023-03-07 11:56:19.000000 astromy-0.1.2/astromy/mygrizli.py
+-rw-r--r--   0 mingyu     (501) staff       (20)     2851 2023-03-07 11:56:19.000000 astromy-0.1.2/astromy/spec1d.py
+-rw-r--r--   0 mingyu     (501) staff       (20)        0 2023-02-27 16:43:41.000000 astromy-0.1.2/astromy/spec2d.py
+-rw-r--r--   0 mingyu     (501) staff       (20)     2211 2022-11-17 15:28:44.000000 astromy-0.1.2/astromy/wcs.py
+drwxr-xr-x   0 mingyu     (501) staff       (20)        0 2023-07-21 18:12:48.134395 astromy-0.1.2/astromy.egg-info/
+-rw-r--r--   0 mingyu     (501) staff       (20)      670 2023-07-21 18:12:48.000000 astromy-0.1.2/astromy.egg-info/PKG-INFO
+-rw-r--r--   0 mingyu     (501) staff       (20)      396 2023-07-21 18:12:48.000000 astromy-0.1.2/astromy.egg-info/SOURCES.txt
+-rw-r--r--   0 mingyu     (501) staff       (20)        1 2023-07-21 18:12:48.000000 astromy-0.1.2/astromy.egg-info/dependency_links.txt
+-rw-r--r--   0 mingyu     (501) staff       (20)       78 2023-07-21 18:12:48.000000 astromy-0.1.2/astromy.egg-info/requires.txt
+-rw-r--r--   0 mingyu     (501) staff       (20)        8 2023-07-21 18:12:48.000000 astromy-0.1.2/astromy.egg-info/top_level.txt
+-rw-r--r--   0 mingyu     (501) staff       (20)       38 2023-07-21 18:12:48.134856 astromy-0.1.2/setup.cfg
+-rw-r--r--   0 mingyu     (501) staff       (20)     3877 2023-02-27 13:19:12.000000 astromy-0.1.2/setup.py
```

### Comparing `astromy-0.1.1/LICENSE` & `astromy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `astromy-0.1.1/PKG-INFO` & `astromy-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Astronomy data analysis package.
 Home-page: https://github.com/lmytime/astromy
 Author: Mingyu Li
 Author-email: lmytime@hotmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `astromy-0.1.1/astromy/__init__.py` & `astromy-0.1.2/astromy/__init__.py`

 * *Files identical despite different names*

### Comparing `astromy-0.1.1/astromy/astromatic.py` & `astromy-0.1.2/astromy/astromatic.py`

 * *Files identical despite different names*

### Comparing `astromy-0.1.1/astromy/catalog.py` & `astromy-0.1.2/astromy/catalog.py`

 * *Files identical despite different names*

### Comparing `astromy-0.1.1/astromy/image.py` & `astromy-0.1.2/astromy/image.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,29 +7,39 @@
 from astropy import units as u
 from astropy.coordinates import SkyCoord
 from astropy.io import fits
 from astropy.nddata.utils import Cutout2D
 from astropy.wcs import WCS
 from astropy.wcs.utils import proj_plane_pixel_scales
 from reproject import reproject_adaptive, reproject_exact, reproject_interp
+import getpass
+import time
 
 from .wcs import transform_wcs
 
 
-def zscale(img):
+def zscale(img, vmin=None, vmax=None):
     """
     Normalization of zscale.
     Input is a 2D numpy array.
 
     Return a Normalization class to be used with Matplotlib.
     """
     from astropy.visualization import (ImageNormalize, LinearStretch,
                                        ZScaleInterval)
-    norm = ImageNormalize(img, interval=ZScaleInterval(),
-                          stretch=LinearStretch())
+    if vmin is None:
+        if vmax is None:
+            norm = ImageNormalize(img, interval=ZScaleInterval(), stretch=LinearStretch())
+        else:
+            norm = ImageNormalize(img, interval=ZScaleInterval(), stretch=LinearStretch(), vmax=vmax)
+    else:
+        if vmax is None:
+            norm = ImageNormalize(img, interval=ZScaleInterval(), stretch=LinearStretch(), vmin=vmin)
+        else:
+            norm = ImageNormalize(img, interval=ZScaleInterval(), stretch=LinearStretch(), vmin=vmin, vmax=vmax)
     return norm
 
 def gamma_correction(colorbar, gamma=1.0):
     '''
     Gamma correction for colorbar.
     Input is a colormap instance.
 
@@ -74,17 +84,56 @@
     ax.add_artist(mpatches.Ellipse(xy=xy, width=BMIN, height=BMAJ, angle=-BPA, facecolor="none", color='white',linewidth=3))
 
 
 
 class AstroImage:
     def __init__(self, data, header):
         self.data = data
+        self.__fix_data__()
         self.header = header
+        self.__fix_header__()
         self.wcs = WCS(self.header)
 
+    def __fix_data__(self):
+        # fix the data for axes with length 1
+        self.data = np.squeeze(self.data)
+
+
+    def __fix_header__(self):
+        """Fix the header for empty axes. Adapted from Qubefit."""
+        # update the NAXIS keywords
+        axes = ['NAXIS1', 'NAXIS2', 'NAXIS3', 'NAXIS4']
+        for cnt, axis in enumerate(axes):
+            if cnt >= self.data.ndim:
+                break
+            if (self.header.get(axis, default=-1) !=
+                    self.data.shape[self.data.ndim-cnt-1]):
+                self.header[axis] = self.data.shape[self.data.ndim-cnt-1]
+        self.header['NAXIS'] = self.data.ndim
+
+        # remove the fourth dimension if not needed
+        if self.data.ndim <= 3:
+            keys = ['PC04_01', 'PC04_02', 'PC04_03', 'PC04_04',
+                    'PC01_04', 'PC02_04', 'PC03_04', 'CTYPE4',
+                    'CRVAL4', 'CDELT4', 'CRPIX4', 'CUNIT4',
+                    'CROTA4', 'NAXIS4', 'CNAME4', 'PC4_1',
+                    'PC4_2', 'PC4_3', 'PC1_4', 'PC2_4', 'PC3_4', 'PC4_4']
+            for key in keys:
+                self.header.remove(key, ignore_missing=True)
+
+        # remove the third dimension if not needed
+        if self.data.ndim <= 2:
+            keys = ['PC03_01', 'PC03_02', 'PC03_03', 'PC01_03',
+                    'PC02_03', 'CTYPE3', 'CRVAL3', 'CDELT3',
+                    'CRPIX3', 'CUNIT3', 'CROTA3', 'NAXIS3', 'CNAME3',
+                    'CD3_3', 'PC3_1', 'PC3_2', 'PC3_3', 'PC1_3',
+                    'PC2_3']
+            for key in keys:
+                self.header.remove(key, ignore_missing=True)
+
     @classmethod
     def read(cls, url, ext=0):
         with fits.open(url) as hdulist:
             data = hdulist[ext].data
             header = hdulist[ext].header
         return cls(data, header)
 
@@ -157,15 +206,21 @@
         if(size_unit == u.arcsec):
             size = size * size_unit
         elif(size_unit == 'pixel'):
             size = size
         hdu_crop = Cutout2D(self.data, position=coord, size=size,
                             wcs=self.wcs, mode=mode)
         wcs_crop = hdu_crop.wcs
-        return AstroImage(data=hdu_crop.data, header=wcs_crop.to_header())
+        header = self.header.copy()
+        header.update(wcs_crop.to_header())
+        header['history'] = f"Image cropped with AstroMy by {getpass.getuser()} on {time.strftime('%Y/%m/%d %H:%m', time.localtime())}"
+        header['coord'] = f"{coord.ra.value:.6f}, {coord.dec.value:.6f}"
+        header['size'] = f"{size} {size.unit}"
+
+        return AstroImage(data=hdu_crop.data, header=header)
 
     def rotate(self, angle, algorithm='interpolation'):
         input_wcs = deepcopy(self.wcs)
         input_wcs.wcs.crpix = self.pixcenter
         input_wcs.wcs.crval = self.skycenter
         output_wcs = transform_wcs(input_wcs, rotation=np.deg2rad(angle))
         if(algorithm == 'interpolation'):
```

### Comparing `astromy-0.1.1/astromy/wcs.py` & `astromy-0.1.2/astromy/wcs.py`

 * *Files identical despite different names*

### Comparing `astromy-0.1.1/astromy.egg-info/PKG-INFO` & `astromy-0.1.2/astromy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Astronomy data analysis package.
 Home-page: https://github.com/lmytime/astromy
 Author: Mingyu Li
 Author-email: lmytime@hotmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `astromy-0.1.1/setup.py` & `astromy-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Package meta-data.
 NAME = 'astromy'
 DESCRIPTION = 'Astronomy data analysis package.'
 URL = 'https://github.com/lmytime/astromy'
 EMAIL = 'lmytime@hotmail.com'
 AUTHOR = 'Mingyu Li'
 REQUIRES_PYTHON = '>=3.6.0'
-# VERSION read from __version__.py
-VERSION = False
+# VERSION from __version__.py
+VERSION = None
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'astropy', 'numpy', 'matplotlib', 'pandas', 'regions', 'getpass', 'spectral_cube', 'scipy', 'reproject'
 ]
 
 # What packages are optional?
```

