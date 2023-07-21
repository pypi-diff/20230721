# Comparing `tmp/TDCRPy-0.0.8.tar.gz` & `tmp/TDCRPy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TDCRPy-0.0.8.tar", last modified: Tue Jul 18 11:26:37 2023, max compression
+gzip compressed data, was "dist\TDCRPy-0.0.9.tar", last modified: Wed Jul 19 08:14:14 2023, max compression
```

## Comparing `TDCRPy-0.0.8.tar` & `TDCRPy-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 11:26:37.000000 TDCRPy-0.0.8/
-drwxrwxrwx   0        0        0        0 2023-07-18 11:26:37.000000 TDCRPy-0.0.8/Code/
--rw-rw-rw-   0        0        0    11530 2023-07-05 06:46:32.000000 TDCRPy-0.0.8/Code/Activity_TDCR.py
--rw-rw-rw-   0        0        0     4829 2023-07-05 09:18:15.000000 TDCRPy-0.0.8/Code/EfficiencyProfils.py
--rw-rw-rw-   0        0        0    23214 2023-07-18 11:21:15.000000 TDCRPy-0.0.8/Code/TDCRPy.py
--rw-rw-rw-   0        0        0    79829 2023-07-18 09:23:02.000000 TDCRPy-0.0.8/Code/TDCR_model_lib.py
--rw-rw-rw-   0        0        0     3171 2023-07-13 14:12:55.000000 TDCRPy-0.0.8/Code/TDCRoptimize.py
--rw-rw-rw-   0        0        0       93 2023-07-14 12:49:39.000000 TDCRPy-0.0.8/Code/__init__.py
--rw-rw-rw-   0        0        0      817 2023-05-23 08:42:51.000000 TDCRPy-0.0.8/Code/decay.py
--rw-rw-rw-   0        0        0      292 2023-07-18 09:45:23.000000 TDCRPy-0.0.8/Code/test.py
--rw-rw-rw-   0        0        0     3250 2023-05-23 08:42:51.000000 TDCRPy-0.0.8/Code/test1.py
--rw-rw-rw-   0        0        0     1086 2023-07-14 13:43:17.000000 TDCRPy-0.0.8/LICENCE.md
--rw-rw-rw-   0        0        0     5610 2023-07-18 11:26:37.000000 TDCRPy-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4737 2023-05-23 08:42:51.000000 TDCRPy-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 11:26:37.000000 TDCRPy-0.0.8/TDCRPy.egg-info/
--rw-rw-rw-   0        0        0     5610 2023-07-18 11:26:36.000000 TDCRPy-0.0.8/TDCRPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-07-18 11:26:37.000000 TDCRPy-0.0.8/TDCRPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 11:26:36.000000 TDCRPy-0.0.8/TDCRPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-18 11:26:36.000000 TDCRPy-0.0.8/TDCRPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-18 11:26:36.000000 TDCRPy-0.0.8/TDCRPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 11:26:37.000000 TDCRPy-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1188 2023-07-18 11:26:19.000000 TDCRPy-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 08:14:14.000000 TDCRPy-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-07-19 08:14:14.000000 TDCRPy-0.0.9/Code/
+-rw-rw-rw-   0        0        0    11530 2023-07-05 06:46:32.000000 TDCRPy-0.0.9/Code/Activity_TDCR.py
+-rw-rw-rw-   0        0        0     4829 2023-07-05 09:18:15.000000 TDCRPy-0.0.9/Code/EfficiencyProfils.py
+-rw-rw-rw-   0        0        0    23233 2023-07-18 11:35:16.000000 TDCRPy-0.0.9/Code/TDCRPy.py
+-rw-rw-rw-   0        0        0    79829 2023-07-18 09:23:02.000000 TDCRPy-0.0.9/Code/TDCR_model_lib.py
+-rw-rw-rw-   0        0        0     3171 2023-07-13 14:12:55.000000 TDCRPy-0.0.9/Code/TDCRoptimize.py
+-rw-rw-rw-   0        0        0       57 2023-07-19 08:13:43.000000 TDCRPy-0.0.9/Code/__init__.py
+-rw-rw-rw-   0        0        0      817 2023-05-23 08:42:51.000000 TDCRPy-0.0.9/Code/decay.py
+-rw-rw-rw-   0        0        0      292 2023-07-18 09:45:23.000000 TDCRPy-0.0.9/Code/test.py
+-rw-rw-rw-   0        0        0     3250 2023-05-23 08:42:51.000000 TDCRPy-0.0.9/Code/test1.py
+-rw-rw-rw-   0        0        0     1086 2023-07-14 13:43:17.000000 TDCRPy-0.0.9/LICENCE.md
+-rw-rw-rw-   0        0        0     5610 2023-07-19 08:14:14.000000 TDCRPy-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4737 2023-05-23 08:42:51.000000 TDCRPy-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 08:14:14.000000 TDCRPy-0.0.9/TDCRPy.egg-info/
+-rw-rw-rw-   0        0        0     5610 2023-07-19 08:14:13.000000 TDCRPy-0.0.9/TDCRPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-07-19 08:14:13.000000 TDCRPy-0.0.9/TDCRPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 08:14:13.000000 TDCRPy-0.0.9/TDCRPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-19 08:14:13.000000 TDCRPy-0.0.9/TDCRPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-19 08:14:13.000000 TDCRPy-0.0.9/TDCRPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 08:14:14.000000 TDCRPy-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1188 2023-07-19 08:14:05.000000 TDCRPy-0.0.9/setup.py
```

### Comparing `TDCRPy-0.0.8/Code/Activity_TDCR.py` & `TDCRPy-0.0.9/Code/Activity_TDCR.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.8/Code/EfficiencyProfils.py` & `TDCRPy-0.0.9/Code/EfficiencyProfils.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.8/Code/TDCRPy.py` & `TDCRPy-0.0.9/Code/TDCRPy.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,15 +285,15 @@
                 energy_vec[i] = tl.energie_dep_beta(energy_vec[i])
 
             if p == "beta+":
                 e_b,p_b = tl.readBetaShape(rad_i,"beta+",level_before_trans)
                 index_beta_energy = tl.sampling(p_b)
                 particle_vec[i] = "positron"
                 energy_vec[i] = e_b[index_beta_energy]
-                energy_vec[i] = tl.energie_dep_beta(energy_vec[i])
+                energy_vec[i] = tl.energie_dep_beta(energy_vec[i]) # treated as beta-
                 particle_vec.append("gamma")
                 particle_vec.append("gamma")
                 energy_vec.append(511)
                 energy_vec.append(511)
 
             if p == "gamma" or p == "XKA" or p == "XKB" or p == "XL":
                 energy_vec[i] = tl.energie_dep_gamma(energy_vec[i],v=10)          # sampling energy free from photon
```

### Comparing `TDCRPy-0.0.8/Code/TDCR_model_lib.py` & `TDCRPy-0.0.9/Code/TDCR_model_lib.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.8/Code/TDCRoptimize.py` & `TDCRPy-0.0.9/Code/TDCRoptimize.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.8/Code/decay.py` & `TDCRPy-0.0.9/Code/decay.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.8/Code/test1.py` & `TDCRPy-0.0.9/Code/test1.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.8/LICENCE.md` & `TDCRPy-0.0.9/LICENCE.md`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.8/PKG-INFO` & `TDCRPy-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDCRPy
-Version: 0.0.8
+Version: 0.0.9
 Summary: TDCR model
 Home-page: https://github.com/RomainCoulon/TDCRPy
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 License: UNKNOWN
 Keywords: python,TDCR,Monte-Carlo,radionuclide,scintillation,counting
 Platform: UNKNOWN
```

### Comparing `TDCRPy-0.0.8/README.md` & `TDCRPy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.8/TDCRPy.egg-info/PKG-INFO` & `TDCRPy-0.0.9/TDCRPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDCRPy
-Version: 0.0.8
+Version: 0.0.9
 Summary: TDCR model
 Home-page: https://github.com/RomainCoulon/TDCRPy
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 License: UNKNOWN
 Keywords: python,TDCR,Monte-Carlo,radionuclide,scintillation,counting
 Platform: UNKNOWN
```

### Comparing `TDCRPy-0.0.8/setup.py` & `TDCRPy-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 DESCRIPTION = "TDCR model"
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name = "TDCRPy",
```

