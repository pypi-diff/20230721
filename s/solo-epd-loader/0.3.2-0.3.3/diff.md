# Comparing `tmp/solo_epd_loader-0.3.2.tar.gz` & `tmp/solo_epd_loader-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solo_epd_loader-0.3.2.tar", last modified: Fri Jul 21 13:23:54 2023, max compression
+gzip compressed data, was "solo_epd_loader-0.3.3.tar", last modified: Fri Jul 21 14:04:30 2023, max compression
```

## Comparing `solo_epd_loader-0.3.2.tar` & `solo_epd_loader-0.3.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 13:23:54.226393 solo_epd_loader-0.3.2/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.3.2/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.2/MANIFEST.in
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16842 2023-07-21 13:23:54.226393 solo_epd_loader-0.3.2/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15894 2023-07-20 13:53:21.000000 solo_epd_loader-0.3.2/README.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.3.2/code_of_conduct.md
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 13:23:54.210393 solo_epd_loader-0.3.2/docs/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.2/docs/Makefile
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.2/docs/conf.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.3.2/docs/index.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.2/docs/make.bat
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 13:23:54.218393 solo_epd_loader-0.3.2/examples/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.3.2/examples/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.3.2/examples/ws2021_fig_2d.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.3.2/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.3.2/gh2021_fig_2a.png
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 13:23:54.222393 solo_epd_loader-0.3.2/licenses/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.3.2/licenses/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2023-07-05 12:35:18.000000 solo_epd_loader-0.3.2/licenses/SUNPY_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.2/licenses/TEMPLATE_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.2/pyproject.toml
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2309 2023-07-21 13:23:54.226393 solo_epd_loader-0.3.2/setup.cfg
--rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.2/setup.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 13:23:54.222393 solo_epd_loader-0.3.2/solo_epd_loader/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    81329 2023-07-21 13:20:21.000000 solo_epd_loader-0.3.2/solo_epd_loader/__init__.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 13:23:54.226393 solo_epd_loader-0.3.2/solo_epd_loader/tests/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.2/solo_epd_loader/tests/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-07-21 13:23:54.000000 solo_epd_loader-0.3.2/solo_epd_loader/version.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 13:23:54.222393 solo_epd_loader-0.3.2/solo_epd_loader.egg-info/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16842 2023-07-21 13:23:54.000000 solo_epd_loader-0.3.2/solo_epd_loader.egg-info/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      638 2023-07-21 13:23:54.000000 solo_epd_loader-0.3.2/solo_epd_loader.egg-info/SOURCES.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-07-21 13:23:54.000000 solo_epd_loader-0.3.2/solo_epd_loader.egg-info/dependency_links.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.3.2/solo_epd_loader.egg-info/not-zip-safe
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      194 2023-07-21 13:23:54.000000 solo_epd_loader-0.3.2/solo_epd_loader.egg-info/requires.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-07-21 13:23:54.000000 solo_epd_loader-0.3.2/solo_epd_loader.egg-info/top_level.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.3.2/tox.ini
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 14:04:30.466758 solo_epd_loader-0.3.3/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.3.3/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.3/MANIFEST.in
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16842 2023-07-21 14:04:30.466758 solo_epd_loader-0.3.3/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15894 2023-07-20 13:53:21.000000 solo_epd_loader-0.3.3/README.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.3.3/code_of_conduct.md
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 14:04:30.462758 solo_epd_loader-0.3.3/docs/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.3/docs/Makefile
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.3/docs/conf.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.3.3/docs/index.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.3/docs/make.bat
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 14:04:30.466758 solo_epd_loader-0.3.3/examples/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.3.3/examples/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.3.3/examples/ws2021_fig_2d.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.3.3/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.3.3/gh2021_fig_2a.png
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 14:04:30.466758 solo_epd_loader-0.3.3/licenses/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.3.3/licenses/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2023-07-05 12:35:18.000000 solo_epd_loader-0.3.3/licenses/SUNPY_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.3/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.3/pyproject.toml
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2309 2023-07-21 14:04:30.466758 solo_epd_loader-0.3.3/setup.cfg
+-rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.3/setup.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 14:04:30.466758 solo_epd_loader-0.3.3/solo_epd_loader/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    81547 2023-07-21 14:00:54.000000 solo_epd_loader-0.3.3/solo_epd_loader/__init__.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 14:04:30.466758 solo_epd_loader-0.3.3/solo_epd_loader/tests/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.3/solo_epd_loader/tests/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-07-21 14:04:30.000000 solo_epd_loader-0.3.3/solo_epd_loader/version.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 14:04:30.466758 solo_epd_loader-0.3.3/solo_epd_loader.egg-info/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16842 2023-07-21 14:04:30.000000 solo_epd_loader-0.3.3/solo_epd_loader.egg-info/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      638 2023-07-21 14:04:30.000000 solo_epd_loader-0.3.3/solo_epd_loader.egg-info/SOURCES.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-07-21 14:04:30.000000 solo_epd_loader-0.3.3/solo_epd_loader.egg-info/dependency_links.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.3.3/solo_epd_loader.egg-info/not-zip-safe
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      194 2023-07-21 14:04:30.000000 solo_epd_loader-0.3.3/solo_epd_loader.egg-info/requires.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-07-21 14:04:30.000000 solo_epd_loader-0.3.3/solo_epd_loader.egg-info/top_level.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.3.3/tox.ini
```

### Comparing `solo_epd_loader-0.3.2/LICENSE.rst` & `solo_epd_loader-0.3.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.2/PKG-INFO` & `solo_epd_loader-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo_epd_loader
-Version: 0.3.2
+Version: 0.3.3
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `solo_epd_loader-0.3.2/README.rst` & `solo_epd_loader-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.2/code_of_conduct.md` & `solo_epd_loader-0.3.3/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.2/docs/Makefile` & `solo_epd_loader-0.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.2/docs/conf.py` & `solo_epd_loader-0.3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.2/docs/make.bat` & `solo_epd_loader-0.3.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.2/examples/gh2021_fig_2.png` & `solo_epd_loader-0.3.3/examples/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.2/examples/ws2021_fig_2d.png` & `solo_epd_loader-0.3.3/examples/ws2021_fig_2d.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.2/gh2021_fig_2.png` & `solo_epd_loader-0.3.3/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.2/gh2021_fig_2a.png` & `solo_epd_loader-0.3.3/gh2021_fig_2a.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.2/licenses/LICENSE.rst` & `solo_epd_loader-0.3.3/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.2/licenses/SUNPY_LICENSE.rst` & `solo_epd_loader-0.3.3/licenses/SUNPY_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.2/licenses/TEMPLATE_LICENSE.rst` & `solo_epd_loader-0.3.3/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.2/setup.cfg` & `solo_epd_loader-0.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.2/setup.py` & `solo_epd_loader-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.2/solo_epd_loader/__init__.py` & `solo_epd_loader-0.3.3/solo_epd_loader/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from packaging.version import Version
 from pathlib import Path
 
 import cdflib
 import numpy as np
 import pandas as pd
 from astropy.io.votable import parse_single_table
-from seppy.tools import resample_df
 from tqdm import tqdm
 
 if hasattr(sunpy, "__version__") and Version(sunpy.__version__) >= Version("5.0.0"):
     from sunpy.io._cdf import read_cdf, _known_units
 else:
     from sunpy.io.cdf import read_cdf, _known_units
 from sunpy.timeseries import TimeSeries
@@ -1459,25 +1458,25 @@
     df = pd.DataFrame(df.values, index=df.index, columns=index)
     #  df.index.names = ['Time']
     return df
 
 
 def combine_channels(df, energies, en_channel, sensor):
     """
-    Average the fluxes of several adjascent energy channels of one sensor into
+    Average the fluxes of several adjacent energy channels of one sensor into
     a combined energy channel.
 
     Parameters
     ----------
     df : pd.DataFrame
         DataFrame containing electron or proton/ion data of the sensor
     energies : dict
         Energy/meta dictionary returned from epd_load (last returned object)
     en_channel : list of 2 integers
-        Range of adjascent energy channels to be used, e.g. [3, 5] for
+        Range of adjacent energy channels to be used, e.g. [3, 5] for
         combining 4th, 5th, and 6th channels (counting starts with 0).
     sensor : string
         'ept' or 'het'
 
     Returns
     -------
     pd.DataFrame
@@ -1554,14 +1553,20 @@
         en_channel_string = en_str[en_channel][0]
     return flux_out, en_channel_string
 
 
 calc_av_en_flux = copy.copy(combine_channels)  # define old name of the function for compatibility
 
 
+# import here to avoid circular import with seppy
+def resample_df(df, resample, pos_timestamp='center', origin='start'):
+    from seppy.tools import resample_df
+    return resample_df(df=df, resample=resample, pos_timestamp=pos_timestamp, origin=origin)
+
+
 """
 Modification of sunpy's read_cdf function to allow skipping of reading variables from a cdf file.
 This function is copied from sunpy under the terms of the BSD 2-Clause licence. See licenses/SUNPY_LICENSE.rst
 """
 
 
 def _read_cdf_mod(fname, ignore_vars=[]):
```

### Comparing `solo_epd_loader-0.3.2/solo_epd_loader.egg-info/PKG-INFO` & `solo_epd_loader-0.3.3/solo_epd_loader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo-epd-loader
-Version: 0.3.2
+Version: 0.3.3
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `solo_epd_loader-0.3.2/solo_epd_loader.egg-info/SOURCES.txt` & `solo_epd_loader-0.3.3/solo_epd_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.2/tox.ini` & `solo_epd_loader-0.3.3/tox.ini`

 * *Files identical despite different names*

