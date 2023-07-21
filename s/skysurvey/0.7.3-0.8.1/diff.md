# Comparing `tmp/skysurvey-0.7.3.tar.gz` & `tmp/skysurvey-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skysurvey-0.7.3.tar", last modified: Mon Jul  3 08:29:37 2023, max compression
+gzip compressed data, was "skysurvey-0.8.1.tar", last modified: Fri Jul 21 08:19:27 2023, max compression
```

## Comparing `skysurvey-0.7.3.tar` & `skysurvey-0.8.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-03 08:29:37.184815 skysurvey-0.7.3/
--rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-08-10 14:40:58.000000 skysurvey-0.7.3/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      747 2023-07-03 08:29:37.184872 skysurvey-0.7.3/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)     2136 2023-06-30 08:24:06.000000 skysurvey-0.7.3/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)     1205 2023-07-03 08:29:37.185190 skysurvey-0.7.3/setup.cfg
--rw-r--r--   0 rigault   (2358) staff       (20)       37 2023-06-12 09:49:45.000000 skysurvey-0.7.3/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-03 08:29:37.181020 skysurvey-0.7.3/skysurvey/
--rw-r--r--   0 rigault   (2358) staff       (20)       90 2023-07-03 08:25:02.000000 skysurvey-0.7.3/skysurvey/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)      524 2023-06-27 13:24:20.000000 skysurvey-0.7.3/skysurvey/config.py
--rw-r--r--   0 rigault   (2358) staff       (20)    27899 2023-06-29 09:38:43.000000 skysurvey-0.7.3/skysurvey/dataset.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-03 08:29:37.182258 skysurvey-0.7.3/skysurvey/examples/
--rw-r--r--   0 rigault   (2358) staff       (20)       26 2023-06-29 14:59:14.000000 skysurvey-0.7.3/skysurvey/examples/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2233 2023-06-29 14:59:29.000000 skysurvey-0.7.3/skysurvey/examples/mocksurvey.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-03 08:29:37.183129 skysurvey-0.7.3/skysurvey/survey/
--rw-r--r--   0 rigault   (2358) staff       (20)      125 2023-06-28 15:34:39.000000 skysurvey-0.7.3/skysurvey/survey/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)     9538 2023-06-29 14:45:35.000000 skysurvey-0.7.3/skysurvey/survey/core.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2849 2023-06-29 07:52:19.000000 skysurvey-0.7.3/skysurvey/survey/des.py
--rw-r--r--   0 rigault   (2358) staff       (20)    15609 2023-06-29 13:44:29.000000 skysurvey-0.7.3/skysurvey/survey/healpix.py
--rw-r--r--   0 rigault   (2358) staff       (20)      976 2023-06-30 08:20:21.000000 skysurvey-0.7.3/skysurvey/survey/lsst.py
--rw-r--r--   0 rigault   (2358) staff       (20)    13238 2023-06-29 13:35:29.000000 skysurvey-0.7.3/skysurvey/survey/polygon.py
--rw-r--r--   0 rigault   (2358) staff       (20)     8955 2023-06-29 09:16:04.000000 skysurvey-0.7.3/skysurvey/survey/survey.py
--rw-r--r--   0 rigault   (2358) staff       (20)     1938 2023-06-29 13:30:27.000000 skysurvey-0.7.3/skysurvey/survey/ztf.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-03 08:29:37.184407 skysurvey-0.7.3/skysurvey/target/
--rw-r--r--   0 rigault   (2358) staff       (20)      113 2023-05-05 08:46:40.000000 skysurvey-0.7.3/skysurvey/target/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)    12064 2023-06-30 12:09:56.000000 skysurvey-0.7.3/skysurvey/target/collection.py
--rw-r--r--   0 rigault   (2358) staff       (20)    33561 2023-07-03 07:33:19.000000 skysurvey-0.7.3/skysurvey/target/core.py
--rw-r--r--   0 rigault   (2358) staff       (20)      391 2022-10-06 08:31:16.000000 skysurvey-0.7.3/skysurvey/target/environments.py
--rw-r--r--   0 rigault   (2358) staff       (20)      165 2022-09-17 13:52:22.000000 skysurvey-0.7.3/skysurvey/target/kilonova.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2341 2023-06-09 12:22:54.000000 skysurvey-0.7.3/skysurvey/target/sncc.py
--rw-r--r--   0 rigault   (2358) staff       (20)    10038 2023-07-03 07:59:46.000000 skysurvey-0.7.3/skysurvey/target/snia.py
--rw-r--r--   0 rigault   (2358) staff       (20)      681 2023-06-02 09:01:21.000000 skysurvey-0.7.3/skysurvey/target/stars.py
--rw-r--r--   0 rigault   (2358) staff       (20)     7268 2023-07-03 07:59:22.000000 skysurvey-0.7.3/skysurvey/target/timeserie.py
--rw-r--r--   0 rigault   (2358) staff       (20)    16507 2023-05-26 07:31:27.000000 skysurvey-0.7.3/skysurvey/template.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-03 08:29:37.184724 skysurvey-0.7.3/skysurvey/tools/
--rw-r--r--   0 rigault   (2358) staff       (20)       64 2023-06-29 10:12:11.000000 skysurvey-0.7.3/skysurvey/tools/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2301 2023-06-27 14:26:14.000000 skysurvey-0.7.3/skysurvey/tools/snana.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2762 2023-06-27 08:23:39.000000 skysurvey-0.7.3/skysurvey/tools/utils.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-03 08:29:37.182030 skysurvey-0.7.3/skysurvey.egg-info/
--rw-r--r--   0 rigault   (2358) staff       (20)      747 2023-07-03 08:29:37.000000 skysurvey-0.7.3/skysurvey.egg-info/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)      922 2023-07-03 08:29:37.000000 skysurvey-0.7.3/skysurvey.egg-info/SOURCES.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-07-03 08:29:37.000000 skysurvey-0.7.3/skysurvey.egg-info/dependency_links.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-06-12 09:47:03.000000 skysurvey-0.7.3/skysurvey.egg-info/not-zip-safe
--rw-r--r--   0 rigault   (2358) staff       (20)      194 2023-07-03 08:29:37.000000 skysurvey-0.7.3/skysurvey.egg-info/requires.txt
--rw-r--r--   0 rigault   (2358) staff       (20)       10 2023-07-03 08:29:37.000000 skysurvey-0.7.3/skysurvey.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-21 08:19:27.372113 skysurvey-0.8.1/
+-rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-08-10 14:40:58.000000 skysurvey-0.8.1/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      747 2023-07-21 08:19:27.372190 skysurvey-0.8.1/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)     2136 2023-06-30 08:24:06.000000 skysurvey-0.8.1/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)     1205 2023-07-21 08:19:27.372532 skysurvey-0.8.1/setup.cfg
+-rw-r--r--   0 rigault   (2358) staff       (20)       37 2023-06-12 09:49:45.000000 skysurvey-0.8.1/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-21 08:19:27.350787 skysurvey-0.8.1/skysurvey/
+-rw-r--r--   0 rigault   (2358) staff       (20)       90 2023-07-21 08:19:03.000000 skysurvey-0.8.1/skysurvey/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      524 2023-06-27 13:24:20.000000 skysurvey-0.8.1/skysurvey/config.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    27899 2023-06-29 09:38:43.000000 skysurvey-0.8.1/skysurvey/dataset.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-21 08:19:27.352294 skysurvey-0.8.1/skysurvey/examples/
+-rw-r--r--   0 rigault   (2358) staff       (20)       26 2023-06-29 14:59:14.000000 skysurvey-0.8.1/skysurvey/examples/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2233 2023-06-29 14:59:29.000000 skysurvey-0.8.1/skysurvey/examples/mocksurvey.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-21 08:19:27.354362 skysurvey-0.8.1/skysurvey/survey/
+-rw-r--r--   0 rigault   (2358) staff       (20)      125 2023-06-28 15:34:39.000000 skysurvey-0.8.1/skysurvey/survey/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     9538 2023-06-29 14:45:35.000000 skysurvey-0.8.1/skysurvey/survey/core.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2849 2023-06-29 07:52:19.000000 skysurvey-0.8.1/skysurvey/survey/des.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    15609 2023-06-29 13:44:29.000000 skysurvey-0.8.1/skysurvey/survey/healpix.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      976 2023-06-30 08:20:21.000000 skysurvey-0.8.1/skysurvey/survey/lsst.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    13238 2023-06-29 13:35:29.000000 skysurvey-0.8.1/skysurvey/survey/polygon.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     8955 2023-06-29 09:16:04.000000 skysurvey-0.8.1/skysurvey/survey/survey.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     1938 2023-07-19 09:47:02.000000 skysurvey-0.8.1/skysurvey/survey/ztf.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-21 08:19:27.367826 skysurvey-0.8.1/skysurvey/target/
+-rw-r--r--   0 rigault   (2358) staff       (20)      113 2023-05-05 08:46:40.000000 skysurvey-0.8.1/skysurvey/target/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    12064 2023-06-30 12:09:56.000000 skysurvey-0.8.1/skysurvey/target/collection.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    36619 2023-07-21 08:14:03.000000 skysurvey-0.8.1/skysurvey/target/core.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      391 2022-10-06 08:31:16.000000 skysurvey-0.8.1/skysurvey/target/environments.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     3394 2023-07-20 21:35:56.000000 skysurvey-0.8.1/skysurvey/target/host.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      165 2022-09-17 13:52:22.000000 skysurvey-0.8.1/skysurvey/target/kilonova.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2341 2023-06-09 12:22:54.000000 skysurvey-0.8.1/skysurvey/target/sncc.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    17405 2023-07-20 21:35:56.000000 skysurvey-0.8.1/skysurvey/target/snia.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      681 2023-06-02 09:01:21.000000 skysurvey-0.8.1/skysurvey/target/stars.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     7268 2023-07-03 07:59:22.000000 skysurvey-0.8.1/skysurvey/target/timeserie.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    16507 2023-05-26 07:31:27.000000 skysurvey-0.8.1/skysurvey/template.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-21 08:19:27.371698 skysurvey-0.8.1/skysurvey/tools/
+-rw-r--r--   0 rigault   (2358) staff       (20)       64 2023-06-29 10:12:11.000000 skysurvey-0.8.1/skysurvey/tools/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2301 2023-06-27 14:26:14.000000 skysurvey-0.8.1/skysurvey/tools/snana.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2762 2023-06-27 08:23:39.000000 skysurvey-0.8.1/skysurvey/tools/utils.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-21 08:19:27.351842 skysurvey-0.8.1/skysurvey.egg-info/
+-rw-r--r--   0 rigault   (2358) staff       (20)      747 2023-07-21 08:19:27.000000 skysurvey-0.8.1/skysurvey.egg-info/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)      947 2023-07-21 08:19:27.000000 skysurvey-0.8.1/skysurvey.egg-info/SOURCES.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-07-21 08:19:27.000000 skysurvey-0.8.1/skysurvey.egg-info/dependency_links.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-06-12 09:47:03.000000 skysurvey-0.8.1/skysurvey.egg-info/not-zip-safe
+-rw-r--r--   0 rigault   (2358) staff       (20)      194 2023-07-21 08:19:27.000000 skysurvey-0.8.1/skysurvey.egg-info/requires.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)       10 2023-07-21 08:19:27.000000 skysurvey-0.8.1/skysurvey.egg-info/top_level.txt
```

### Comparing `skysurvey-0.7.3/LICENSE` & `skysurvey-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.3/PKG-INFO` & `skysurvey-0.8.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skysurvey
-Version: 0.7.3
+Version: 0.8.1
 Summary: Simulating Transient in the sky and how to observe them
 Home-page: https://github.com/MickaelRigault/skysurvey
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: Apache Software License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `skysurvey-0.7.3/README.md` & `skysurvey-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.3/setup.cfg` & `skysurvey-0.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.3/skysurvey/config.py` & `skysurvey-0.8.1/skysurvey/config.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.3/skysurvey/dataset.py` & `skysurvey-0.8.1/skysurvey/dataset.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.3/skysurvey/examples/mocksurvey.py` & `skysurvey-0.8.1/skysurvey/examples/mocksurvey.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.3/skysurvey/survey/core.py` & `skysurvey-0.8.1/skysurvey/survey/core.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.3/skysurvey/survey/des.py` & `skysurvey-0.8.1/skysurvey/survey/des.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.3/skysurvey/survey/healpix.py` & `skysurvey-0.8.1/skysurvey/survey/healpix.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.3/skysurvey/survey/lsst.py` & `skysurvey-0.8.1/skysurvey/survey/lsst.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.3/skysurvey/survey/polygon.py` & `skysurvey-0.8.1/skysurvey/survey/polygon.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.3/skysurvey/survey/survey.py` & `skysurvey-0.8.1/skysurvey/survey/survey.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.3/skysurvey/survey/ztf.py` & `skysurvey-0.8.1/skysurvey/survey/ztf.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.3/skysurvey/target/collection.py` & `skysurvey-0.8.1/skysurvey/target/collection.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.3/skysurvey/target/core.py` & `skysurvey-0.8.1/skysurvey/target/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import warnings
 import numpy as np
 import pandas
-import inspect
 from astropy import cosmology, time
 from astropy.utils.decorators import classproperty
 
 
 from ..template import Template
 from ..tools.utils import parse_skyarea, surface_of_skyarea
 
@@ -98,27 +97,28 @@
         return this
         
     @classmethod
     def from_draw(cls, size=None, model=None, template=None,
                       zmax=None, tstart=None, tstop=None,
                       zmin=0, nyears=None,
                       skyarea=None,
+                      funcs={},
                       **kwargs):
         """ loads the instance from a random draw of targets given the model 
 
         Parameters
         ----------
         size: int, None
             number of target you want to sample
             size=None as in numpy. Usually means 1.
             = ignored if nyears given =
 
         model: dict, None
             defines how  template parameters to draw and how they are connected
-            See "target model documentation"
+            model will update the default cls._MODEL if any
             = leave to None if unsure, cls._MODEL used as default = 
 
         template_source: str, None
             name of the template (sncosmo.Model(source)). 
             = leave to None if unsure, cls._TEMPLATE used as default =
 
         zmax: float
@@ -164,25 +164,26 @@
 
         See also
         --------
         from_setting:  loads an instance given model parameters (dict)            
         """
         this = cls()
         if model is not None:
-            this.set_model(model)
+            this.update_model(**model) # will update any model entry.
 
         if template is not None:
             this.set_template(template)
             
-        _ = this.draw(size=size,
-                        zmin=zmin, zmax=zmax,
-                        tstart=tstart, tstop=tstop,
-                        nyears=nyears,
-                        skyarea=skyarea,
-                          **kwargs)
+        _ = this.draw( size=size,
+                       zmin=zmin, zmax=zmax,
+                       tstart=tstart, tstop=tstop,
+                       nyears=nyears,
+                       skyarea=skyarea,
+                       inplace=True, # creates self.data
+                       **kwargs)
         return this
         
     # ------------- # 
     #   Template    #
     # ------------- #
     def set_template(self, template):
         """ set the template 
@@ -263,15 +264,15 @@
         See also
         --------
         get_template: get a template instance (sncosmo.Model)
         get_template_parameters: get the template parameters for the given target
 
         """
         return self.get_template(index=index, **kwargs)
-
+    
     def get_target_flux(self, index, band, phase, zp=None, zpsys=None):
         """ Flux through the given bandpass(es) at the given time(s).
 
         Default return value is flux in photons / s / cm^2. If zp and zpsys
         are given, flux(es) are scaled to the requested zeropoints.
 
         Parameters
@@ -301,15 +302,14 @@
             given, in which case flux is scaled so that it corresponds
             to the requested zeropoint. Return value is `float` if all
             input parameters are scalars, `~numpy.ndarray` otherwise.
         """
         sncosmo_model = self.get_target_template(index).sncosmo_model
         return sncosmo_model.bandflux(band, sncosmo_model.get('t0')+phase, zp=zp, zpsys=zpsys)
 
-
     def clone_target_change_entry(self, index, name, values, as_dataframe=False):
         """ get a clone of the given target at the given redshifts.
         This: 
         (1) copies the index entries, 
         (2) sets the `name` to the input `values`
         (3) redraw the model starting from `name` (creating a new dataframe)
         (4, optional) sets a new instance with the updated dataframe
@@ -559,14 +559,65 @@
             if self.template is None:
                 templatename = "unknown"
             else:
                 templatename = self.template_source.name
             data["template"] = templatename
 
         self._data = data
+
+    def get_noisy_data(self, errmodel):
+        """ get a copy of the data with error applied on it.
+        
+
+        Parameters
+        ----------
+        errmodel: dict or ModelDAG
+            error model for self.data entries. 
+            It follows the ModelDAG format (if dict: {key: {"func": {}, "kwarg":{}}, }).
+            a dataframe with the same size as self.data will be created 
+            and each entry of the errmodel will affect the corresponding entry in the data. 
+            if "key_err" is given in the model, this entry will be passed to data.
+            = warning: no error on the error implemented yet. =
+            
+        Returns
+        -------
+        pandas.DataFrame
+            a copy of self.data affected by errors.
+
+        Example
+        -------
+        creating a random gaussian error with a scale of 2. 
+        The error also has error, and will not be given perfectly 2 but a random error of 0.01.
+        ```python
+        errmodel = {"a": {"func":np.random.normal, "kwargs":{"loc":0, "scale":2 }},
+                   "a_err": {"func":np.random.normal, "kwargs":{"loc":2, "scale":0.01 }},
+                   }
+        datanoisy = self.get_noisy_data(errmodel)
+        ```
+    
+        """
+
+        if type(errmodel) is dict:
+            from modeldag import ModelDAG
+            errmodel = ModelDAG(errmodel)
+
+
+        data_err=  errmodel.draw( len(self.data) )
+        column_to_noisify = data_err.columns
+
+
+        datanoisy = self.data.copy()
+        for k in column_to_noisify:
+            datanoisy[k] = datanoisy[k] + data_err[k]
+            if f"{k}_err" in data_err.columns:
+                datanoisy[f"{k}_err"] = data_err[f"{k}_err"].abs() # abs in case
+            else:
+                warnings.warn(f"no error given for {k}_err entry.")
+
+        return datanoisy
         
     def get_model(self, **kwargs):
         """ get a copy of the model (dict) 
 
         You can change the model you get (not the current model)
         using the kwargs. 
 
@@ -581,55 +632,73 @@
         -------
         dict
            a copy of the model (with param potentially updated)
            
            
         See also
         --------
-        change_model_parameter: change the current model (not just the one you get)
+        update_model: change the current model (not just the one you get)
         get_model_parameter: access the model parameters.
         """
-        self.model.get_model(**kwargs)
+        return self.model.get_model(**kwargs)
 
-    def get_model_parameter(self, entry, key, default=None):
+    def get_model_parameter(self, entry, key, default=None, model=None):
         """ access a parameter of the model.
 
         Parameters
         ----------
         entry: str
             name of the variable as given by the model dict
 
         key: str
             name of the parameters
 
         default: 
             value returned if the parameter is not found.
 
+        model: modelDAG
+            get the parameter of this model instead of self.model
+            = use with caution =
+
         Returns
         -------
         value of the entry parameter
         
         Example
         -------
         >>> self.get_model_parameter('redshift', 'zmax', None)
 
         """
-        return self.model.model[entry]["kwargs"].get(key, default)
+        if model is None:
+            model = self.model
+            
+        return model.model[entry]["kwargs"].get(key, default)
+
 
-    def change_model_parameter(self, **kwargs):
-        """ Change the model parameters
+    def update_model_parameter(self, **kwargs):
+        """ change the kwargs entry of a model. """
 
-        **kwargs will update any model entry parameters (i.e., the "param", e.g. t0["param"]).
+        for k, v in kwargs.items():
+            self.model.model[k]["kwargs"] = {**self.model.model[k]["kwargs"], **v}
+            
+    def update_model(self, **kwargs):
+        """ Change the given entries of the model.
+
+        **kwargs will update any model entry (or create a new one at the end).
 
         Example
         -------
-        Change the maximum redshift to 1.
-        >>> self.change_model_parameter(redshift={"zmax":1})
+        Changing the b entry function and make it depends on "a"
+        >>> self.update_model( b={"func":np.random.normal, "kwargs":{"loc":"@a", "scale":1}})
         """
-        _ = self.model.change_model(**kwargs)
+        new_model = {**self.model.model, **kwargs}
+        if not new_model.keys() == self.model.model.keys():
+            warnings.warn("updating the model has changed the model entries")
+
+        _ = self.set_model(new_model)
         
     # -------------- #
     #   Plotter      #
     # -------------- #
     def show_scatter(self, xkey, ykey, ckey=None, ax=None, fig=None, 
                          index=None, data=None, colorbar=True,
                          **kwargs):
@@ -667,15 +736,17 @@
     # =============== #
     #   Draw Methods  #
     # =============== #
     def draw(self, size=None,
                  zmax=None, zmin=0,
                  tstart=None, tstop=None, nyears=None,
                  skyarea=None,
-                 inplace=True, **kwargs):
+                 inplace=False,
+                 model=None,
+                 **kwargs):
         """ draws the parameter model (using self.model.draw()) 
 
         Parameters
         ----------
         size: int
             = ignored is nyears is not None =
             number of target you want to draw.
@@ -712,14 +783,24 @@
 
         Returns
         -------
         DataFrame
             the simulated dataframe.
 
         """
+        #
+        # Drawn model
+        # 
+        if model is None:
+            drawn_model = self.model # a modelDAG
+        else:
+            from modeldag import ModelDAG
+            current_model_dict = self.model.model
+            drawn_model = ModelDAG( {**current_model_dict, **model}, obj=self)
+            
         # => tstart, tstop format
         if type(tstart) is str:
             tstart = time.Time(tstart).mjd
         elif type(tstart) is time.Time:
             tstart = tstart.mjd
 
         if type(tstop) is str:
@@ -747,21 +828,22 @@
         # Redshift
         #
         # zmax
         if zmax is not None:
             kwargs.setdefault("redshift",{}).update({"zmax": zmax})
             
         elif nyears is not None:
-            zmax = self.get_model_parameter("redshift", "zmax", None)
+            zmax = self.get_model_parameter("redshift", "zmax", None, model=drawn_model)
+            
         # zmin
         if zmin is not None and "redshift" in self.model.model:
             kwargs.setdefault("redshift",{}).update({"zmin": zmin})
             
         elif nyears is not None:
-            zmin = self.get_model_parameter("redshift", "zmin", None)
+            zmin = self.get_model_parameter("redshift", "zmin", None, model=drawn_model)
 
         if tstop is not None:
             if type( tstop ) is str:
                 tstop = time.Time(tstop).mjd
 
             kwargs.setdefault("t0",{}).update({"high": tstop})
 
@@ -771,27 +853,29 @@
         if tstart is not None:
             if type( tstart ) is str:
                 tstart = time.Time(tstart).mjd
                 
             kwargs.setdefault("t0",{}).update({"low": tstart})
             if tstop is None and nyears is None: # do 1 year by default
                 kwargs.setdefault("t0",{}).update({"high": tstart+365.25})
+                
         # tstart is None, then what ?
         elif tstop is not None and nyears is not None:
-            tstart = tstop - 365.25*nyears # fixed later            
+            tstart = tstop - 365.25*nyears # fixed later
+            
         elif nyears is not None:
-            tstart = self.get_model_parameter("t0", "low", None)
+            tstart = self.get_model_parameter("t0", "low", None, model=drawn_model)
 
         #
         # Sky area
         #
         skyarea = parse_skyarea(skyarea) # shapely.geometry or skyarea
         if skyarea is not None:
-            param_affected = [k for k, v in self.model.get_func_parameters().items() if "skyarea" in v]
-            if "radec" in self.model.model.keys() and "radec" not in param_affected:
+            param_affected = [k for k, v in drawn_model.get_func_parameters().items() if "skyarea" in v]
+            if "radec" in drawn_model.model.keys() and "radec" not in param_affected:
                 warnings.warn("radec in model, skyarea given, but the radec func does not accept skyarea.")
                 
             for k in param_affected:
                 kwargs.setdefault(k,{}).update({"skyarea": skyarea})
                 
 
         #
@@ -800,15 +884,15 @@
         # skyarea affect get_rate
         if nyears is not None:
             rate_min = self.get_rate(zmin, skyarea=skyarea) if (zmin is not None and zmin >0) else 0
             kwargs.setdefault("t0",{}).update({"low": tstart, "high": tstart + 365.25*nyears})
             size = int((self.get_rate(zmax, skyarea=skyarea)-rate_min) * nyears)
             
         # actually draw the data
-        data = self.model.draw(size=size, **kwargs)
+        data = drawn_model.draw(size=size, **kwargs)
         if inplace:
             # lower precision
             data = data.astype( {k: str(v).replace("64","32") for k, v in data.dtypes.to_dict().items()})
             self.set_data(data)
             
         return data
```

### Comparing `skysurvey-0.7.3/skysurvey/target/sncc.py` & `skysurvey-0.8.1/skysurvey/target/sncc.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.3/skysurvey/target/stars.py` & `skysurvey-0.8.1/skysurvey/target/stars.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.3/skysurvey/target/timeserie.py` & `skysurvey-0.8.1/skysurvey/target/timeserie.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.3/skysurvey/template.py` & `skysurvey-0.8.1/skysurvey/template.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.3/skysurvey/tools/snana.py` & `skysurvey-0.8.1/skysurvey/tools/snana.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.3/skysurvey/tools/utils.py` & `skysurvey-0.8.1/skysurvey/tools/utils.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.7.3/skysurvey.egg-info/PKG-INFO` & `skysurvey-0.8.1/skysurvey.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skysurvey
-Version: 0.7.3
+Version: 0.8.1
 Summary: Simulating Transient in the sky and how to observe them
 Home-page: https://github.com/MickaelRigault/skysurvey
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: Apache Software License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `skysurvey-0.7.3/skysurvey.egg-info/SOURCES.txt` & `skysurvey-0.8.1/skysurvey.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 skysurvey/survey/polygon.py
 skysurvey/survey/survey.py
 skysurvey/survey/ztf.py
 skysurvey/target/__init__.py
 skysurvey/target/collection.py
 skysurvey/target/core.py
 skysurvey/target/environments.py
+skysurvey/target/host.py
 skysurvey/target/kilonova.py
 skysurvey/target/sncc.py
 skysurvey/target/snia.py
 skysurvey/target/stars.py
 skysurvey/target/timeserie.py
 skysurvey/tools/__init__.py
 skysurvey/tools/snana.py
```

