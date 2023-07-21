# Comparing `tmp/xmask-0.3.2.tar.gz` & `tmp/xmask-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmask-0.3.2.tar", last modified: Sun Jun 11 06:15:52 2023, max compression
+gzip compressed data, was "xmask-0.3.3.tar", last modified: Fri Jul 21 09:09:39 2023, max compression
```

## Comparing `xmask-0.3.2.tar` & `xmask-0.3.3.tar`

### file list

```diff
@@ -1,30 +1,26 @@
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-11 06:15:52.516300 xmask-0.3.2/
--rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:05:06.000000 xmask-0.3.2/LICENSE
--rw-r--r--   0 giadarol   (503) staff       (20)      237 2023-03-23 11:05:06.000000 xmask-0.3.2/MANIFEST.in
--rw-r--r--   0 giadarol   (503) staff       (20)      520 2023-06-11 06:15:52.516153 xmask-0.3.2/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)      115 2023-03-23 11:05:06.000000 xmask-0.3.2/pyproject.toml
--rw-r--r--   0 giadarol   (503) staff       (20)       38 2023-06-11 06:15:52.516344 xmask-0.3.2/setup.cfg
--rw-r--r--   0 giadarol   (503) staff       (20)     1433 2023-03-23 11:05:06.000000 xmask-0.3.2/setup.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-11 06:15:52.507410 xmask-0.3.2/tests/
--rw-r--r--   0 giadarol   (503) staff       (20)    71861 2023-06-11 06:15:17.000000 xmask-0.3.2/tests/test_hllhc14.py
--rw-r--r--   0 giadarol   (503) staff       (20)    21540 2023-05-30 19:22:48.000000 xmask-0.3.2/tests/test_hllhc14_b1_only.py
--rw-r--r--   0 giadarol   (503) staff       (20)    29755 2023-05-30 19:22:48.000000 xmask-0.3.2/tests/test_lhc_ion.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-11 06:15:52.509580 xmask-0.3.2/xmask/
--rw-r--r--   0 giadarol   (503) staff       (20)      233 2023-03-23 11:05:06.000000 xmask-0.3.2/xmask/__init__.py
--rw-r--r--   0 giadarol   (503) staff       (20)       22 2023-06-11 06:15:35.000000 xmask-0.3.2/xmask/_version.py
--rw-r--r--   0 giadarol   (503) staff       (20)      225 2023-03-23 11:05:06.000000 xmask-0.3.2/xmask/env_and_links.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-11 06:15:52.515808 xmask-0.3.2/xmask/lhc/
--rw-r--r--   0 giadarol   (503) staff       (20)      432 2023-05-07 06:53:44.000000 xmask-0.3.2/xmask/lhc/__init__.py
--rw-r--r--   0 giadarol   (503) staff       (20)     5652 2023-05-07 06:53:44.000000 xmask-0.3.2/xmask/lhc/build_madx_and_xsuite_models.py
--rw-r--r--   0 giadarol   (503) staff       (20)     3553 2023-03-23 11:05:06.000000 xmask-0.3.2/xmask/lhc/errors.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2423 2023-05-30 19:22:48.000000 xmask-0.3.2/xmask/lhc/knob_manipulations.py
--rw-r--r--   0 giadarol   (503) staff       (20)     3231 2023-05-28 15:35:42.000000 xmask-0.3.2/xmask/lhc/leveling.py
--rw-r--r--   0 giadarol   (503) staff       (20)    12355 2023-05-07 06:53:44.000000 xmask-0.3.2/xmask/madx_model.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2883 2023-05-07 06:53:44.000000 xmask-0.3.2/xmask/tuning.py
--rw-r--r--   0 giadarol   (503) staff       (20)      728 2023-03-23 11:05:06.000000 xmask-0.3.2/xmask/yaml.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-11 06:15:52.514365 xmask-0.3.2/xmask.egg-info/
--rw-r--r--   0 giadarol   (503) staff       (20)      520 2023-06-11 06:15:52.000000 xmask-0.3.2/xmask.egg-info/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)      508 2023-06-11 06:15:52.000000 xmask-0.3.2/xmask.egg-info/SOURCES.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        1 2023-06-11 06:15:52.000000 xmask-0.3.2/xmask.egg-info/dependency_links.txt
--rw-r--r--   0 giadarol   (503) staff       (20)       49 2023-06-11 06:15:52.000000 xmask-0.3.2/xmask.egg-info/requires.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        6 2023-06-11 06:15:52.000000 xmask-0.3.2/xmask.egg-info/top_level.txt
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-07-21 09:09:39.378224 xmask-0.3.3/
+-rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:05:06.000000 xmask-0.3.3/LICENSE
+-rw-r--r--   0 giadarol   (503) staff       (20)      237 2023-03-23 11:05:06.000000 xmask-0.3.3/MANIFEST.in
+-rw-r--r--   0 giadarol   (503) staff       (20)      520 2023-07-21 09:09:39.378053 xmask-0.3.3/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)      115 2023-03-23 11:05:06.000000 xmask-0.3.3/pyproject.toml
+-rw-r--r--   0 giadarol   (503) staff       (20)       38 2023-07-21 09:09:39.378274 xmask-0.3.3/setup.cfg
+-rw-r--r--   0 giadarol   (503) staff       (20)     1433 2023-03-23 11:05:06.000000 xmask-0.3.3/setup.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-07-21 09:09:39.374970 xmask-0.3.3/xmask/
+-rw-r--r--   0 giadarol   (503) staff       (20)      233 2023-03-23 11:05:06.000000 xmask-0.3.3/xmask/__init__.py
+-rw-r--r--   0 giadarol   (503) staff       (20)       22 2023-07-21 09:09:22.000000 xmask-0.3.3/xmask/_version.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      225 2023-03-23 11:05:06.000000 xmask-0.3.3/xmask/env_and_links.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-07-21 09:09:39.377811 xmask-0.3.3/xmask/lhc/
+-rw-r--r--   0 giadarol   (503) staff       (20)      432 2023-05-07 06:53:44.000000 xmask-0.3.3/xmask/lhc/__init__.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     5652 2023-05-07 06:53:44.000000 xmask-0.3.3/xmask/lhc/build_madx_and_xsuite_models.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     3553 2023-03-23 11:05:06.000000 xmask-0.3.3/xmask/lhc/errors.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2423 2023-05-30 19:22:48.000000 xmask-0.3.3/xmask/lhc/knob_manipulations.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     3542 2023-07-21 09:09:07.000000 xmask-0.3.3/xmask/lhc/leveling.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    12388 2023-07-21 09:09:07.000000 xmask-0.3.3/xmask/madx_model.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2883 2023-05-07 06:53:44.000000 xmask-0.3.3/xmask/tuning.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      728 2023-03-23 11:05:06.000000 xmask-0.3.3/xmask/yaml.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-07-21 09:09:39.376418 xmask-0.3.3/xmask.egg-info/
+-rw-r--r--   0 giadarol   (503) staff       (20)      520 2023-07-21 09:09:39.000000 xmask-0.3.3/xmask.egg-info/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)      434 2023-07-21 09:09:39.000000 xmask-0.3.3/xmask.egg-info/SOURCES.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        1 2023-07-21 09:09:39.000000 xmask-0.3.3/xmask.egg-info/dependency_links.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)       49 2023-07-21 09:09:39.000000 xmask-0.3.3/xmask.egg-info/requires.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        6 2023-07-21 09:09:39.000000 xmask-0.3.3/xmask.egg-info/top_level.txt
```

### Comparing `xmask-0.3.2/LICENSE` & `xmask-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xmask-0.3.2/PKG-INFO` & `xmask-0.3.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmask
-Version: 0.3.2
+Version: 0.3.3
 Summary: Configuration of tracking simulations for the LHC and other accelerators
 Home-page: https://github.com/xsuite/xsuite/issues
 Download-URL: https://pypi.python.org/pypi/xmask
 Author: G. Iadarola et al.
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
 Project-URL: Source Code, https://github.com/xsuite/xmask/
```

### Comparing `xmask-0.3.2/setup.py` & `xmask-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.2/xmask/lhc/build_madx_and_xsuite_models.py` & `xmask-0.3.3/xmask/lhc/build_madx_and_xsuite_models.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.2/xmask/lhc/errors.py` & `xmask-0.3.3/xmask/lhc/errors.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.2/xmask/lhc/knob_manipulations.py` & `xmask-0.3.3/xmask/lhc/knob_manipulations.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.2/xmask/lhc/leveling.py` & `xmask-0.3.3/xmask/lhc/leveling.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,20 +21,21 @@
         targets=[]
         vary=[]
 
         if 'luminosity' in config_this_ip.keys():
             targets.append(
                 xt.TargetLuminosity(
                     ip_name=ip_name, luminosity=config_this_ip['luminosity'], crab=False,
-                    tol=0.01 * config_this_ip['luminosity'],
+                    tol=0.001 * config_this_ip['luminosity'],
                     f_rev=f_rev, num_colliding_bunches=config_this_ip['num_colliding_bunches'],
                     num_particles_per_bunch=config_beambeam['num_particles_per_bunch'],
                     sigma_z=config_beambeam['sigma_z'],
                     nemitt_x=config_beambeam['nemitt_x'],
-                    nemitt_y=config_beambeam['nemitt_y'])
+                    nemitt_y=config_beambeam['nemitt_y'],
+                    log=True)
             )
         elif 'separation_in_sigmas' in config_this_ip.keys():
             targets.append(
                 xt.TargetSeparation(
                     ip_name=ip_name,
                     separation_norm=config_this_ip['separation_in_sigmas'],
                     tol=1e-4, # in sigmas
@@ -44,31 +45,39 @@
             )
         else:
             raise ValueError('Either `luminosity` or `separation_in_sigmas` must be specified')
 
         if config_this_ip['impose_separation_orthogonal_to_crossing']:
             targets.append(
                 xt.TargetSeparationOrthogonalToCrossing(ip_name='ip8'))
-        vary.append(
-            xt.VaryList(config_this_ip['knobs'], step=1e-4))
+        for knob_name in config_this_ip['knobs']:
+            vv = collider.vars[knob_name]._value
+            # Preserve knob sign
+            if vv >= 0:
+                ll = (0, 1e200)
+            else:
+                ll = (-1e200, 0)
+            vary.append(xt.Vary(name=knob_name, step=1e-7, limits=ll))
 
         # Target and knobs to rematch the crossing angles and close the bumps
         for line_name in ['lhcb1', 'lhcb2']:
             targets += [
                 # Preserve crossing angle
                 xt.TargetList(['px', 'py'], at=ip_name, line=line_name, value='preserve', tol=1e-7, scale=1e3),
                 # Close the bumps
                 xt.TargetList(['x', 'y'], at=bump_range[line_name][-1], line=line_name, value='preserve', tol=1e-5, scale=1),
                 xt.TargetList(['px', 'py'], at=bump_range[line_name][-1], line=line_name, value='preserve', tol=1e-5, scale=1e3),
             ]
 
         vary.append(xt.VaryList(config_this_ip['corrector_knob_names'], step=1e-7))
 
         # Match
-        collider.match(
+        opt = collider.match(
             lines=['lhcb1', 'lhcb2'],
             ele_start=[bump_range['lhcb1'][0], bump_range['lhcb2'][0]],
             ele_stop=[bump_range['lhcb1'][-1], bump_range['lhcb2'][-1]],
             twiss_init='preserve',
             targets=targets,
-            vary=vary
+            vary=vary,
+            solve=False,
         )
+        opt.solve()
```

### Comparing `xmask-0.3.2/xmask/madx_model.py` & `xmask-0.3.3/xmask/madx_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
             print(f'Warning: b4 indep {nn}={b4_indep[nn]} is not in b2.')
 
     b2_dep=var_dicts_b2['dependent_variables_expr']
     b4_dep=var_dicts_b4['dependent_variables_expr']
     for nn in b2_dep.keys():
         if str(nn) in list(update_globals.keys()):
             continue
-        assert str(b4_dep[nn]) == str(b2_dep[nn])
+        assert str(b4_dep[nn]).replace(" ","") == str(b2_dep[nn]).replace(" ","")
 
     for nn in b4_dep.keys():
         if nn not in b2_dep.keys():
             print(f'Warning: b4 dep {nn}={str(b4_dep[nn])} is not in b2.')
 
 def _get_variables_dicts(mad, expressions_as_str=True):
         variables_df = _get_variables_dataframes(mad)
@@ -348,8 +348,8 @@
             'floor',
             'ceil',
             'round',
             'frac',
             'ranf',
             'gauss',
             'tgauss']))
-        return my_list
+        return my_list
```

### Comparing `xmask-0.3.2/xmask/tuning.py` & `xmask-0.3.3/xmask/tuning.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.2/xmask/yaml.py` & `xmask-0.3.3/xmask/yaml.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.2/xmask.egg-info/PKG-INFO` & `xmask-0.3.3/xmask.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmask
-Version: 0.3.2
+Version: 0.3.3
 Summary: Configuration of tracking simulations for the LHC and other accelerators
 Home-page: https://github.com/xsuite/xsuite/issues
 Download-URL: https://pypi.python.org/pypi/xmask
 Author: G. Iadarola et al.
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
 Project-URL: Source Code, https://github.com/xsuite/xmask/
```

