# Comparing `tmp/solo_epd_loader-0.3.1.tar.gz` & `tmp/solo_epd_loader-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/gieseler/uni/solo/solo-epd-loader/dist/.tmp-akki_32u/solo_epd_loader-0.3.1.tar", last modified: Thu Jul 20 14:47:11 2023, max compression
+gzip compressed data, was "solo_epd_loader-0.3.2.tar", last modified: Fri Jul 21 13:23:54 2023, max compression
```

## Comparing `solo_epd_loader-0.3.1.tar` & `solo_epd_loader-0.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-20 14:47:11.864363 solo_epd_loader-0.3.1/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.3.1/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.1/MANIFEST.in
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16842 2023-07-20 14:47:11.864363 solo_epd_loader-0.3.1/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15894 2023-07-20 13:53:21.000000 solo_epd_loader-0.3.1/README.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.3.1/code_of_conduct.md
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-20 14:47:11.860363 solo_epd_loader-0.3.1/docs/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.1/docs/Makefile
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.1/docs/conf.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.3.1/docs/index.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.1/docs/make.bat
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-20 14:47:11.860363 solo_epd_loader-0.3.1/examples/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.3.1/examples/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.3.1/examples/ws2021_fig_2d.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.3.1/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.3.1/gh2021_fig_2a.png
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-20 14:47:11.864363 solo_epd_loader-0.3.1/licenses/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.3.1/licenses/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2023-07-05 12:35:18.000000 solo_epd_loader-0.3.1/licenses/SUNPY_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.1/licenses/TEMPLATE_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.1/pyproject.toml
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2302 2023-07-20 14:47:11.868363 solo_epd_loader-0.3.1/setup.cfg
--rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.1/setup.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-20 14:47:11.864363 solo_epd_loader-0.3.1/solo_epd_loader/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    77138 2023-07-20 13:47:58.000000 solo_epd_loader-0.3.1/solo_epd_loader/__init__.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-20 14:47:11.864363 solo_epd_loader-0.3.1/solo_epd_loader/tests/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.1/solo_epd_loader/tests/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-07-20 14:47:11.000000 solo_epd_loader-0.3.1/solo_epd_loader/version.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-20 14:47:11.864363 solo_epd_loader-0.3.1/solo_epd_loader.egg-info/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16842 2023-07-20 14:47:11.000000 solo_epd_loader-0.3.1/solo_epd_loader.egg-info/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      638 2023-07-20 14:47:11.000000 solo_epd_loader-0.3.1/solo_epd_loader.egg-info/SOURCES.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-07-20 14:47:11.000000 solo_epd_loader-0.3.1/solo_epd_loader.egg-info/dependency_links.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.3.1/solo_epd_loader.egg-info/not-zip-safe
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      188 2023-07-20 14:47:11.000000 solo_epd_loader-0.3.1/solo_epd_loader.egg-info/requires.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-07-20 14:47:11.000000 solo_epd_loader-0.3.1/solo_epd_loader.egg-info/top_level.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.3.1/tox.ini
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 13:23:54.226393 solo_epd_loader-0.3.2/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.3.2/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.2/MANIFEST.in
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16842 2023-07-21 13:23:54.226393 solo_epd_loader-0.3.2/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15894 2023-07-20 13:53:21.000000 solo_epd_loader-0.3.2/README.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.3.2/code_of_conduct.md
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 13:23:54.210393 solo_epd_loader-0.3.2/docs/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.2/docs/Makefile
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.2/docs/conf.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.3.2/docs/index.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.2/docs/make.bat
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 13:23:54.218393 solo_epd_loader-0.3.2/examples/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.3.2/examples/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.3.2/examples/ws2021_fig_2d.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.3.2/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.3.2/gh2021_fig_2a.png
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 13:23:54.222393 solo_epd_loader-0.3.2/licenses/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.3.2/licenses/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2023-07-05 12:35:18.000000 solo_epd_loader-0.3.2/licenses/SUNPY_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.2/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.2/pyproject.toml
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2309 2023-07-21 13:23:54.226393 solo_epd_loader-0.3.2/setup.cfg
+-rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.2/setup.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 13:23:54.222393 solo_epd_loader-0.3.2/solo_epd_loader/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    81329 2023-07-21 13:20:21.000000 solo_epd_loader-0.3.2/solo_epd_loader/__init__.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 13:23:54.226393 solo_epd_loader-0.3.2/solo_epd_loader/tests/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.2/solo_epd_loader/tests/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-07-21 13:23:54.000000 solo_epd_loader-0.3.2/solo_epd_loader/version.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-21 13:23:54.222393 solo_epd_loader-0.3.2/solo_epd_loader.egg-info/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16842 2023-07-21 13:23:54.000000 solo_epd_loader-0.3.2/solo_epd_loader.egg-info/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      638 2023-07-21 13:23:54.000000 solo_epd_loader-0.3.2/solo_epd_loader.egg-info/SOURCES.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-07-21 13:23:54.000000 solo_epd_loader-0.3.2/solo_epd_loader.egg-info/dependency_links.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.3.2/solo_epd_loader.egg-info/not-zip-safe
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      194 2023-07-21 13:23:54.000000 solo_epd_loader-0.3.2/solo_epd_loader.egg-info/requires.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-07-21 13:23:54.000000 solo_epd_loader-0.3.2/solo_epd_loader.egg-info/top_level.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.3.2/tox.ini
```

### Comparing `solo_epd_loader-0.3.1/LICENSE.rst` & `solo_epd_loader-0.3.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.1/PKG-INFO` & `solo_epd_loader-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo_epd_loader
-Version: 0.3.1
+Version: 0.3.2
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `solo_epd_loader-0.3.1/README.rst` & `solo_epd_loader-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.1/code_of_conduct.md` & `solo_epd_loader-0.3.2/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.1/docs/Makefile` & `solo_epd_loader-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.1/docs/conf.py` & `solo_epd_loader-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.1/docs/make.bat` & `solo_epd_loader-0.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.1/examples/gh2021_fig_2.png` & `solo_epd_loader-0.3.2/examples/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.1/examples/ws2021_fig_2d.png` & `solo_epd_loader-0.3.2/examples/ws2021_fig_2d.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.1/gh2021_fig_2.png` & `solo_epd_loader-0.3.2/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.1/gh2021_fig_2a.png` & `solo_epd_loader-0.3.2/gh2021_fig_2a.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.1/licenses/LICENSE.rst` & `solo_epd_loader-0.3.2/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.1/licenses/SUNPY_LICENSE.rst` & `solo_epd_loader-0.3.2/licenses/SUNPY_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.1/licenses/TEMPLATE_LICENSE.rst` & `solo_epd_loader-0.3.2/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.1/setup.cfg` & `solo_epd_loader-0.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 	drms
 	h5netcdf
 	lxml
 	matplotlib
 	numpy
 	pandas
 	requests
+	seppy
 	sunpy>=4.1.0
 	tqdm
 	zeep
 
 [options.extras_require]
 all = 
 test =
```

### Comparing `solo_epd_loader-0.3.1/setup.py` & `solo_epd_loader-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.1/solo_epd_loader/__init__.py` & `solo_epd_loader-0.3.2/solo_epd_loader/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pkg_resources import DistributionNotFound, get_distribution
 
 try:
     __version__ = get_distribution(__name__).version
 except DistributionNotFound:
     pass  # package is not installed
 
+import copy
 import datetime as dt
 import glob
 import itertools
 import os
 import re
 import sunpy
 import urllib.request
@@ -18,14 +19,15 @@
 from packaging.version import Version
 from pathlib import Path
 
 import cdflib
 import numpy as np
 import pandas as pd
 from astropy.io.votable import parse_single_table
+from seppy.tools import resample_df
 from tqdm import tqdm
 
 if hasattr(sunpy, "__version__") and Version(sunpy.__version__) >= Version("5.0.0"):
     from sunpy.io._cdf import read_cdf, _known_units
 else:
     from sunpy.io.cdf import read_cdf, _known_units
 from sunpy.timeseries import TimeSeries
@@ -551,15 +553,15 @@
     if sensor.lower() == 'ept' or sensor.lower() == 'het':
         if viewing is None:
             raise Exception("EPT and HET need a telescope 'viewing' " +
                             "direction! No data read!")
             df_epd_p = []
             df_epd_e = []
             energies_dict = []
-        elif viewing is 'omni':
+        elif viewing == 'omni':
             all_df_epd_p = {}
             all_df_epd_e = {}
             for view in ['sun', 'asun', 'north', 'south']:
                 df_epd_p, df_epd_e, energies_dict = \
                     _read_epd_cdf(sensor=sensor, viewing=view, level=level, startdate=startdate, enddate=enddate,
                                   path=path, autodownload=autodownload)
                 all_df_epd_p[view] = df_epd_p
@@ -1455,14 +1457,111 @@
     index = pd.MultiIndex.from_tuples(tuples)
 
     df = pd.DataFrame(df.values, index=df.index, columns=index)
     #  df.index.names = ['Time']
     return df
 
 
+def combine_channels(df, energies, en_channel, sensor):
+    """
+    Average the fluxes of several adjascent energy channels of one sensor into
+    a combined energy channel.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        DataFrame containing electron or proton/ion data of the sensor
+    energies : dict
+        Energy/meta dictionary returned from epd_load (last returned object)
+    en_channel : list of 2 integers
+        Range of adjascent energy channels to be used, e.g. [3, 5] for
+        combining 4th, 5th, and 6th channels (counting starts with 0).
+    sensor : string
+        'ept' or 'het'
+
+    Returns
+    -------
+    pd.DataFrame
+        flux_out : contains channel-averaged flux
+    string
+        en_channel_string : describes the energry range of combined channel
+
+    Raises
+    ------
+    Exception
+        - Sensor 'step' not supported yet.
+        - Lowest EPT channels not supported because of overlapping energies.
+
+    Examples
+    --------
+    Load EPT sun viewing direction level 2 data for Aug 20 to Aug 21, 2020, and
+    combine electron channels 9 to 12 (i.e., 10th to 13th).
+
+    >>> df_p, df_e, meta = epd_load('ept', 20200820, 20200821, 'l2', 'sun')
+    >>> df_new, chan_new = combine_channels(df_p, meta, [9, 12], 'ept')
+    """
+    if sensor.lower() == 'step':
+        raise Exception('STEP data not supported yet!')
+        return pd.DataFrame(), ''
+    # if species.lower() in ['e', 'electrons']:
+    if 'Electron_Flux' in df.keys():
+        en_str = energies['Electron_Bins_Text']
+        bins_width = 'Electron_Bins_Width'
+        flux_key = 'Electron_Flux'
+    # if species.lower() in ['p', 'protons', 'i', 'ions', 'h']:
+    else:
+        if sensor.lower() == 'het':
+            en_str = energies['H_Bins_Text']
+            bins_width = 'H_Bins_Width'
+            flux_key = 'H_Flux'
+        if sensor.lower() == 'ept':
+            en_str = energies['Ion_Bins_Text']
+            bins_width = 'Ion_Bins_Width'
+            flux_key = 'Ion_Flux'
+    if type(en_channel) == list:
+        energy_low = en_str[en_channel[0]][0].split('-')[0]
+        energy_up = en_str[en_channel[-1]][0].split('-')[-1]
+        en_channel_string = energy_low + '-' + energy_up
+
+        if len(en_channel) > 2:
+            raise Exception('en_channel must have 2 elements: start channel and end channel, e.g. [1,3]!')
+        if len(en_channel) == 2:
+            # catch overlapping EPT energy channels and cancel calculation:
+            if sensor.lower() == 'ept' and 'Electron_Flux' in df.keys() and en_channel[0] < 4:
+                raise Exception('Lowest 4 EPT e channels not supported because of overlapping energies!')
+                return pd.DataFrame(), ''
+            if sensor.lower() == 'ept' and 'Electron_Flux' not in df.keys() and en_channel[0] < 9:
+                raise Exception('Lowest 9 EPT ion channels not supported because of overlapping energies!')
+                return pd.DataFrame(), ''
+            # try to convert multi-index dataframe to normal one. if this is already the case, just continue
+            try:
+                df = df[flux_key]
+            except (AttributeError, KeyError):
+                None
+            DE = energies[bins_width]
+            for bins in np.arange(en_channel[0], en_channel[-1]+1):
+                if bins == en_channel[0]:
+                    I_all = df[f'{flux_key}_{bins}'] * DE[bins]
+                else:
+                    I_all = I_all + df[f'{flux_key}_{bins}'] * DE[bins]
+            DE_total = np.sum(DE[(en_channel[0]):(en_channel[-1]+1)])
+            flux_out = pd.DataFrame({'flux': I_all/DE_total}, index=df.index)
+        else:
+            en_channel = en_channel[0]
+            flux_out = pd.DataFrame({'flux': df[flux_key][f'{flux_key}_{en_channel}']}, index=df.index)
+            en_channel_string = en_str[en_channel][0]
+    else:
+        flux_out = pd.DataFrame({'flux': df[flux_key][f'{flux_key}_{en_channel}']}, index=df.index)
+        en_channel_string = en_str[en_channel][0]
+    return flux_out, en_channel_string
+
+
+calc_av_en_flux = copy.copy(combine_channels)  # define old name of the function for compatibility
+
+
 """
 Modification of sunpy's read_cdf function to allow skipping of reading variables from a cdf file.
 This function is copied from sunpy under the terms of the BSD 2-Clause licence. See licenses/SUNPY_LICENSE.rst
 """
 
 
 def _read_cdf_mod(fname, ignore_vars=[]):
```

### Comparing `solo_epd_loader-0.3.1/solo_epd_loader.egg-info/PKG-INFO` & `solo_epd_loader-0.3.2/solo_epd_loader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo-epd-loader
-Version: 0.3.1
+Version: 0.3.2
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `solo_epd_loader-0.3.1/solo_epd_loader.egg-info/SOURCES.txt` & `solo_epd_loader-0.3.2/solo_epd_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.1/tox.ini` & `solo_epd_loader-0.3.2/tox.ini`

 * *Files identical despite different names*

