# Comparing `tmp/opstool-0.8.2.tar.gz` & `tmp/opstool-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opstool-0.8.2.tar", last modified: Sat May 27 08:34:15 2023, max compression
+gzip compressed data, was "opstool-0.8.3.tar", last modified: Fri Jul 21 16:43:36 2023, max compression
```

## Comparing `opstool-0.8.2.tar` & `opstool-0.8.3.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 08:34:15.546811 opstool-0.8.2/
--rw-rw-rw-   0        0        0    34817 2022-12-02 05:00:10.000000 opstool-0.8.2/LICENCE.txt
--rw-rw-rw-   0        0        0     6424 2023-05-27 08:34:15.545965 opstool-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     6005 2023-03-31 11:53:22.000000 opstool-0.8.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-27 08:34:15.546811 opstool-0.8.2/setup.cfg
--rw-rw-rw-   0        0        0     1013 2023-05-07 06:04:08.000000 opstool-0.8.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:34:15.509348 opstool-0.8.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-27 08:34:15.514176 opstool-0.8.2/src/opstool/
--rw-rw-rw-   0        0        0       23 2023-05-27 08:32:31.000000 opstool-0.8.2/src/opstool/__about__.py
--rw-rw-rw-   0        0        0      673 2023-05-25 13:37:11.000000 opstool-0.8.2/src/opstool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:34:15.518009 opstool-0.8.2/src/opstool/analysis/
--rw-rw-rw-   0        0        0      147 2023-03-10 09:13:36.000000 opstool-0.8.2/src/opstool/analysis/__init__.py
--rw-rw-rw-   0        0        0    13408 2023-05-02 13:56:05.000000 opstool-0.8.2/src/opstool/analysis/_sec_analysis.py
--rw-rw-rw-   0        0        0    35206 2023-05-02 13:57:14.000000 opstool-0.8.2/src/opstool/analysis/_smart_analyze.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:34:15.530550 opstool-0.8.2/src/opstool/examples/
--rw-rw-rw-   0        0        0   365987 2022-12-25 13:36:57.000000 opstool-0.8.2/src/opstool/examples/ArchBridge.py
--rw-rw-rw-   0        0        0    96069 2023-01-06 03:19:00.000000 opstool-0.8.2/src/opstool/examples/ArchBridge2.py
--rw-rw-rw-   0        0        0   697240 2022-12-25 13:38:38.000000 opstool-0.8.2/src/opstool/examples/CableStayedBridge.py
--rw-rw-rw-   0        0        0   289022 2022-12-25 13:39:18.000000 opstool-0.8.2/src/opstool/examples/Dam.py
--rw-rw-rw-   0        0        0     1699 2022-12-25 13:39:55.000000 opstool-0.8.2/src/opstool/examples/DamBreak.py
--rw-rw-rw-   0        0        0   241484 2022-12-25 13:40:30.000000 opstool-0.8.2/src/opstool/examples/Frame3D.py
--rw-rw-rw-   0        0        0    15435 2023-05-06 11:58:20.000000 opstool-0.8.2/src/opstool/examples/Frame3D2.py
--rw-rw-rw-   0        0        0    54201 2023-05-06 11:47:25.000000 opstool-0.8.2/src/opstool/examples/GridFrame.py
--rw-rw-rw-   0        0        0   901646 2022-12-25 13:41:16.000000 opstool-0.8.2/src/opstool/examples/Igloo.py
--rw-rw-rw-   0        0        0     2102 2022-12-25 13:41:50.000000 opstool-0.8.2/src/opstool/examples/Pier.py
--rw-rw-rw-   0        0        0     1813 2022-12-25 13:42:23.000000 opstool-0.8.2/src/opstool/examples/SDOF.py
--rw-rw-rw-   0        0        0   110248 2022-12-25 13:43:18.000000 opstool-0.8.2/src/opstool/examples/SuspensionBridge.py
--rw-rw-rw-   0        0        0        2 2022-12-02 13:20:45.000000 opstool-0.8.2/src/opstool/examples/__init__.py
--rw-rw-rw-   0        0        0    16275 2023-05-06 19:15:36.000000 opstool-0.8.2/src/opstool/examples/shell3D.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:34:15.533314 opstool-0.8.2/src/opstool/preprocessing/
--rw-rw-rw-   0        0        0      838 2023-04-02 12:08:20.000000 opstool-0.8.2/src/opstool/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     2876 2023-05-09 04:18:48.000000 opstool-0.8.2/src/opstool/preprocessing/geom_transf.py
--rw-rw-rw-   0        0        0     2266 2023-05-02 14:30:35.000000 opstool-0.8.2/src/opstool/preprocessing/load.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:34:15.535704 opstool-0.8.2/src/opstool/preprocessing/section/
--rw-rw-rw-   0        0        0      554 2023-04-02 12:05:56.000000 opstool-0.8.2/src/opstool/preprocessing/section/__init__.py
--rw-rw-rw-   0        0        0     1417 2023-05-02 13:57:22.000000 opstool-0.8.2/src/opstool/preprocessing/section/lib_sec_mesh.py
--rw-rw-rw-   0        0        0    60702 2023-05-23 16:16:51.000000 opstool-0.8.2/src/opstool/preprocessing/section/sec_mesh.py
--rw-rw-rw-   0        0        0    26107 2023-05-02 13:57:35.000000 opstool-0.8.2/src/opstool/preprocessing/section/var_sec_mesh.py
--rw-rw-rw-   0        0        0    53581 2023-05-26 07:18:07.000000 opstool-0.8.2/src/opstool/preprocessing/tcl2py.py
--rw-rw-rw-   0        0        0     5490 2023-03-30 08:58:00.000000 opstool-0.8.2/src/opstool/preprocessing/unit_system.py
--rw-rw-rw-   0        0        0     8237 2023-05-25 13:58:46.000000 opstool-0.8.2/src/opstool/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:34:15.542641 opstool-0.8.2/src/opstool/vis/
--rw-rw-rw-   0        0        0      494 2023-05-04 17:23:00.000000 opstool-0.8.2/src/opstool/vis/__init__.py
--rw-rw-rw-   0        0        0    32555 2023-05-23 03:42:47.000000 opstool-0.8.2/src/opstool/vis/_get_model_base.py
--rw-rw-rw-   0        0        0   106783 2023-05-24 15:15:18.000000 opstool-0.8.2/src/opstool/vis/_plotly_base.py
--rw-rw-rw-   0        0        0    66174 2023-05-15 10:48:39.000000 opstool-0.8.2/src/opstool/vis/_pyvista_base.py
--rw-rw-rw-   0        0        0    23046 2023-05-04 17:23:18.000000 opstool-0.8.2/src/opstool/vis/fiber_sec_vis.py
--rw-rw-rw-   0        0        0    32015 2023-05-23 03:43:37.000000 opstool-0.8.2/src/opstool/vis/get_model_data.py
--rw-rw-rw-   0        0        0    28645 2023-05-25 15:40:29.000000 opstool-0.8.2/src/opstool/vis/ops_vis_2d.py
--rw-rw-rw-   0        0        0    25267 2023-05-09 06:37:32.000000 opstool-0.8.2/src/opstool/vis/ops_vis_plotly.py
--rw-rw-rw-   0        0        0    24060 2023-05-15 10:10:38.000000 opstool-0.8.2/src/opstool/vis/ops_vis_pyvista.py
--rw-rw-rw-   0        0        0    10494 2023-05-25 15:43:46.000000 opstool-0.8.2/src/opstool/vis/quick_plot.py
--rw-rw-rw-   0        0        0    14099 2023-05-09 07:53:13.000000 opstool-0.8.2/src/opstool/vis/save_tikz.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:34:15.515729 opstool-0.8.2/src/opstool.egg-info/
--rw-rw-rw-   0        0        0     6424 2023-05-27 08:34:15.000000 opstool-0.8.2/src/opstool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1730 2023-05-27 08:34:15.000000 opstool-0.8.2/src/opstool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 08:34:15.000000 opstool-0.8.2/src/opstool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-05-27 08:34:15.000000 opstool-0.8.2/src/opstool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-27 08:34:15.000000 opstool-0.8.2/src/opstool.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 08:34:15.545965 opstool-0.8.2/tests/
--rw-rw-rw-   0        0        0     2002 2023-01-18 14:49:51.000000 opstool-0.8.2/tests/test_dambreak.py
--rw-rw-rw-   0        0        0     1705 2023-03-27 03:00:39.000000 opstool-0.8.2/tests/test_fiber_sec_vis.py
--rw-rw-rw-   0        0        0     2981 2023-05-25 15:47:16.000000 opstool-0.8.2/tests/test_model_vis.py
--rw-rw-rw-   0        0        0     2261 2023-03-29 06:45:30.000000 opstool-0.8.2/tests/test_sec_analysis.py
--rw-rw-rw-   0        0        0    10302 2023-04-03 08:29:31.000000 opstool-0.8.2/tests/test_sec_mesh.py
--rw-rw-rw-   0        0        0      954 2023-05-09 13:39:18.000000 opstool-0.8.2/tests/test_temp.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:43:36.210731 opstool-0.8.3/
+-rw-rw-rw-   0        0        0    34817 2022-12-02 05:00:10.000000 opstool-0.8.3/LICENCE.txt
+-rw-rw-rw-   0        0        0     6424 2023-07-21 16:43:36.210731 opstool-0.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6005 2023-03-31 11:53:22.000000 opstool-0.8.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-21 16:43:36.210731 opstool-0.8.3/setup.cfg
+-rw-rw-rw-   0        0        0     1013 2023-05-07 06:04:08.000000 opstool-0.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:43:36.175592 opstool-0.8.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-21 16:43:36.179481 opstool-0.8.3/src/opstool/
+-rw-rw-rw-   0        0        0     8995 2023-06-17 04:24:19.000000 opstool-0.8.3/src/opstool/EleClassTags.py
+-rw-rw-rw-   0        0        0       23 2023-07-21 16:41:10.000000 opstool-0.8.3/src/opstool/__about__.py
+-rw-rw-rw-   0        0        0      673 2023-05-25 13:37:11.000000 opstool-0.8.3/src/opstool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:43:36.179481 opstool-0.8.3/src/opstool/analysis/
+-rw-rw-rw-   0        0        0      147 2023-03-10 09:13:36.000000 opstool-0.8.3/src/opstool/analysis/__init__.py
+-rw-rw-rw-   0        0        0    13409 2023-06-01 06:34:16.000000 opstool-0.8.3/src/opstool/analysis/_sec_analysis.py
+-rw-rw-rw-   0        0        0    35206 2023-05-02 13:57:14.000000 opstool-0.8.3/src/opstool/analysis/_smart_analyze.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:43:36.195114 opstool-0.8.3/src/opstool/examples/
+-rw-rw-rw-   0        0        0   365987 2022-12-25 13:36:57.000000 opstool-0.8.3/src/opstool/examples/ArchBridge.py
+-rw-rw-rw-   0        0        0    96069 2023-01-06 03:19:00.000000 opstool-0.8.3/src/opstool/examples/ArchBridge2.py
+-rw-rw-rw-   0        0        0   697240 2022-12-25 13:38:38.000000 opstool-0.8.3/src/opstool/examples/CableStayedBridge.py
+-rw-rw-rw-   0        0        0   289022 2022-12-25 13:39:18.000000 opstool-0.8.3/src/opstool/examples/Dam.py
+-rw-rw-rw-   0        0        0     1699 2022-12-25 13:39:55.000000 opstool-0.8.3/src/opstool/examples/DamBreak.py
+-rw-rw-rw-   0        0        0   241484 2022-12-25 13:40:30.000000 opstool-0.8.3/src/opstool/examples/Frame3D.py
+-rw-rw-rw-   0        0        0    15435 2023-05-06 11:58:20.000000 opstool-0.8.3/src/opstool/examples/Frame3D2.py
+-rw-rw-rw-   0        0        0    54201 2023-05-06 11:47:25.000000 opstool-0.8.3/src/opstool/examples/GridFrame.py
+-rw-rw-rw-   0        0        0   901646 2022-12-25 13:41:16.000000 opstool-0.8.3/src/opstool/examples/Igloo.py
+-rw-rw-rw-   0        0        0     2102 2022-12-25 13:41:50.000000 opstool-0.8.3/src/opstool/examples/Pier.py
+-rw-rw-rw-   0        0        0     1813 2022-12-25 13:42:23.000000 opstool-0.8.3/src/opstool/examples/SDOF.py
+-rw-rw-rw-   0        0        0   110248 2022-12-25 13:43:18.000000 opstool-0.8.3/src/opstool/examples/SuspensionBridge.py
+-rw-rw-rw-   0        0        0        2 2022-12-02 13:20:45.000000 opstool-0.8.3/src/opstool/examples/__init__.py
+-rw-rw-rw-   0        0        0    16275 2023-05-06 19:15:36.000000 opstool-0.8.3/src/opstool/examples/shell3D.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:43:36.195114 opstool-0.8.3/src/opstool/preprocessing/
+-rw-rw-rw-   0        0        0      838 2023-04-02 12:08:20.000000 opstool-0.8.3/src/opstool/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2876 2023-05-09 04:18:48.000000 opstool-0.8.3/src/opstool/preprocessing/geom_transf.py
+-rw-rw-rw-   0        0        0     2266 2023-05-02 14:30:35.000000 opstool-0.8.3/src/opstool/preprocessing/load.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:43:36.195114 opstool-0.8.3/src/opstool/preprocessing/section/
+-rw-rw-rw-   0        0        0      554 2023-04-02 12:05:56.000000 opstool-0.8.3/src/opstool/preprocessing/section/__init__.py
+-rw-rw-rw-   0        0        0     1417 2023-05-02 13:57:22.000000 opstool-0.8.3/src/opstool/preprocessing/section/lib_sec_mesh.py
+-rw-rw-rw-   0        0        0    60702 2023-05-23 16:16:51.000000 opstool-0.8.3/src/opstool/preprocessing/section/sec_mesh.py
+-rw-rw-rw-   0        0        0    26107 2023-05-02 13:57:35.000000 opstool-0.8.3/src/opstool/preprocessing/section/var_sec_mesh.py
+-rw-rw-rw-   0        0        0    53581 2023-05-26 07:18:07.000000 opstool-0.8.3/src/opstool/preprocessing/tcl2py.py
+-rw-rw-rw-   0        0        0     5490 2023-03-30 08:58:00.000000 opstool-0.8.3/src/opstool/preprocessing/unit_system.py
+-rw-rw-rw-   0        0        0     6679 2023-06-17 05:03:00.000000 opstool-0.8.3/src/opstool/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:43:36.210731 opstool-0.8.3/src/opstool/vis/
+-rw-rw-rw-   0        0        0      494 2023-05-04 17:23:00.000000 opstool-0.8.3/src/opstool/vis/__init__.py
+-rw-rw-rw-   0        0        0    32837 2023-06-17 08:35:28.000000 opstool-0.8.3/src/opstool/vis/_get_model_base.py
+-rw-rw-rw-   0        0        0   108776 2023-07-21 16:38:13.000000 opstool-0.8.3/src/opstool/vis/_plotly_base.py
+-rw-rw-rw-   0        0        0    68932 2023-06-23 14:36:55.000000 opstool-0.8.3/src/opstool/vis/_pyvista_base.py
+-rw-rw-rw-   0        0        0    23046 2023-05-04 17:23:18.000000 opstool-0.8.3/src/opstool/vis/fiber_sec_vis.py
+-rw-rw-rw-   0        0        0    33077 2023-06-17 09:08:01.000000 opstool-0.8.3/src/opstool/vis/get_model_data.py
+-rw-rw-rw-   0        0        0    28645 2023-05-25 15:40:29.000000 opstool-0.8.3/src/opstool/vis/ops_vis_2d.py
+-rw-rw-rw-   0        0        0    26569 2023-07-21 16:39:02.000000 opstool-0.8.3/src/opstool/vis/ops_vis_plotly.py
+-rw-rw-rw-   0        0        0    26362 2023-06-19 07:13:16.000000 opstool-0.8.3/src/opstool/vis/ops_vis_pyvista.py
+-rw-rw-rw-   0        0        0    10367 2023-06-17 09:08:55.000000 opstool-0.8.3/src/opstool/vis/quick_plot.py
+-rw-rw-rw-   0        0        0    14099 2023-05-09 07:53:13.000000 opstool-0.8.3/src/opstool/vis/save_tikz.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:43:36.179481 opstool-0.8.3/src/opstool.egg-info/
+-rw-rw-rw-   0        0        0     6424 2023-07-21 16:43:36.000000 opstool-0.8.3/src/opstool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1758 2023-07-21 16:43:36.000000 opstool-0.8.3/src/opstool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 16:43:36.000000 opstool-0.8.3/src/opstool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-07-21 16:43:36.000000 opstool-0.8.3/src/opstool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-21 16:43:36.000000 opstool-0.8.3/src/opstool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 16:43:36.210731 opstool-0.8.3/tests/
+-rw-rw-rw-   0        0        0     2002 2023-01-18 14:49:51.000000 opstool-0.8.3/tests/test_dambreak.py
+-rw-rw-rw-   0        0        0     1705 2023-03-27 03:00:39.000000 opstool-0.8.3/tests/test_fiber_sec_vis.py
+-rw-rw-rw-   0        0        0     2995 2023-06-17 05:06:14.000000 opstool-0.8.3/tests/test_model_vis.py
+-rw-rw-rw-   0        0        0     2261 2023-03-29 06:45:30.000000 opstool-0.8.3/tests/test_sec_analysis.py
+-rw-rw-rw-   0        0        0    10302 2023-04-03 08:29:31.000000 opstool-0.8.3/tests/test_sec_mesh.py
+-rw-rw-rw-   0        0        0      954 2023-05-09 13:39:18.000000 opstool-0.8.3/tests/test_temp.py
```

### Comparing `opstool-0.8.2/LICENCE.txt` & `opstool-0.8.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/PKG-INFO` & `opstool-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opstool
-Version: 0.8.2
+Version: 0.8.3
 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992
 Author: Yexiang Yan
 Author-email: yexiang_yan@outlook.com
 License: GPL Licence
 Keywords: OpenSees Visualization Seismic Simulation
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opstool Version: 0.8.2 Summary: openseespy toolbox
+Metadata-Version: 2.1 Name: opstool Version: 0.8.3 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992 Author: Yexiang Yan Author-email:
 yexiang_yan@outlook.com License: GPL Licence Keywords: OpenSees Visualization
 Seismic Simulation Platform: any Classifier: Programming Language :: Python ::
 3 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENCE.txt
                                     opstool
            modelling, visualization, post-processing for OpenSeesPy.
```

### Comparing `opstool-0.8.2/README.md` & `opstool-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/setup.py` & `opstool-0.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/__init__.py` & `opstool-0.8.3/src/opstool/__init__.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/analysis/_sec_analysis.py` & `opstool-0.8.3/src/opstool/analysis/_sec_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         )
 
     def plot_M_phi(self):
         """Plot the moment-curvature relationship."""
         _, ax = plt.subplots(1, 1, figsize=(10, 10 * 0.618))
         ax.plot(self.phi, self.M, lw=3, c="blue")
         ax.set_title(
-            "$M-\phi$",
+            "$M-\\phi$",
             fontsize=28,
         )
         ax.set_xlabel("$\phi$", fontsize=25)
         ax.set_ylabel("$M$", fontsize=25)
         plt.xticks(fontsize=15)
         plt.yticks(fontsize=15)
         ax.spines["bottom"].set_linewidth(1.2)
```

### Comparing `opstool-0.8.2/src/opstool/analysis/_smart_analyze.py` & `opstool-0.8.3/src/opstool/analysis/_smart_analyze.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/examples/ArchBridge.py` & `opstool-0.8.3/src/opstool/examples/ArchBridge.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/examples/ArchBridge2.py` & `opstool-0.8.3/src/opstool/examples/ArchBridge2.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/examples/CableStayedBridge.py` & `opstool-0.8.3/src/opstool/examples/CableStayedBridge.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/examples/Dam.py` & `opstool-0.8.3/src/opstool/examples/Dam.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/examples/DamBreak.py` & `opstool-0.8.3/src/opstool/examples/DamBreak.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/examples/Frame3D.py` & `opstool-0.8.3/src/opstool/examples/Frame3D.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/examples/Frame3D2.py` & `opstool-0.8.3/src/opstool/examples/Frame3D2.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/examples/GridFrame.py` & `opstool-0.8.3/src/opstool/examples/GridFrame.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/examples/Igloo.py` & `opstool-0.8.3/src/opstool/examples/Igloo.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/examples/Pier.py` & `opstool-0.8.3/src/opstool/examples/Pier.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/examples/SDOF.py` & `opstool-0.8.3/src/opstool/examples/SDOF.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/examples/SuspensionBridge.py` & `opstool-0.8.3/src/opstool/examples/SuspensionBridge.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/examples/shell3D.py` & `opstool-0.8.3/src/opstool/examples/shell3D.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/preprocessing/__init__.py` & `opstool-0.8.3/src/opstool/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/preprocessing/geom_transf.py` & `opstool-0.8.3/src/opstool/preprocessing/geom_transf.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/preprocessing/load.py` & `opstool-0.8.3/src/opstool/preprocessing/load.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/preprocessing/section/__init__.py` & `opstool-0.8.3/src/opstool/preprocessing/section/__init__.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/preprocessing/section/lib_sec_mesh.py` & `opstool-0.8.3/src/opstool/preprocessing/section/lib_sec_mesh.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/preprocessing/section/sec_mesh.py` & `opstool-0.8.3/src/opstool/preprocessing/section/sec_mesh.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/preprocessing/section/var_sec_mesh.py` & `opstool-0.8.3/src/opstool/preprocessing/section/var_sec_mesh.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/preprocessing/tcl2py.py` & `opstool-0.8.3/src/opstool/preprocessing/tcl2py.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/preprocessing/unit_system.py` & `opstool-0.8.3/src/opstool/preprocessing/unit_system.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/utils.py` & `opstool-0.8.3/src/opstool/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,186 +1,27 @@
 import sys
 import numpy as np
 from pathlib import Path
 from typing import Union
+from .EleClassTags import (EleTypeTags, ELE_TAG_Beam, ELE_TAG_Tetrahedron, ELE_TAG_Link,
+                           ELE_TAG_PFEM, ELE_TAG_Brick, ELE_TAG_Joint, ELE_TAG_Plane, ELE_TAG_Truss)
+
+
+class EleClassTags:
+    TypeTags = EleTypeTags
+    BeamTags = ELE_TAG_Beam
+    TetTags = ELE_TAG_Tetrahedron
+    LinkTags = ELE_TAG_Link
+    TrussTags = ELE_TAG_Truss
+    PFEMTags = ELE_TAG_PFEM
+    BrickTags = ELE_TAG_Brick
+    JointTags = ELE_TAG_Joint
+    PlaneTags = ELE_TAG_Plane
+
 
-# The element class Tag in OpenSees, which is used to determine the element type
-# see ...\SRC\classTags.h
-ELE_TAG_Truss = [
-    12,
-    13,
-    14,
-    15,
-    16,
-    17,
-    18,
-    138,
-    139,
-    155,
-    169,
-    218,
-]  # 169 is CatenaryCable
-ELE_TAG_Link = [
-    19,
-    20,
-    21,
-    22,
-    23,
-    24,
-    25,
-    26,
-    260,
-    27,  # zeroLength
-    86,  # 86-twoNodeLink
-    84,
-    85,
-    87,
-    88,
-    89,
-    90,
-    91,
-    92,
-    93,
-    94,
-    95,
-    96,
-    97,
-    98,
-    99,
-    100,
-    101,
-    102,
-    103,
-    104,
-    105,
-    106,
-    107,
-    108,
-    109,
-    130,
-    131,
-    132,
-    147,
-    148,
-    149,
-    150,
-    151,
-    152,
-    153,
-    158,
-    159,
-    160,
-    161,
-    165,
-    166,
-]  # Bearing
-ELE_TAG_Beam = [
-    3,
-    4,
-    5,
-    5001,
-    6,
-    7,
-    8,
-    9,
-    10,
-    11,
-    28,
-    29,
-    30,
-    34,
-    35,
-    62,
-    621,
-    63,
-    64,
-    640,
-    641,
-    642,
-    65,
-    66,
-    67,
-    68,
-    69,
-    70,
-    71,
-    72,
-    73,
-    731,
-    74,
-    75,
-    751,
-    76,
-    77,
-    78,
-    30766,
-    30765,
-    30767,
-    79,
-    128,
-]
-ELE_TAG_Plane = [
-    31,
-    32,
-    33,
-    40,
-    47,
-    50,
-    52,
-    53,
-    54,
-    55,
-    59,
-    60,
-    61,
-    116,
-    119,
-    120,
-    126,
-    134,
-    142,
-    143,
-    156,
-    157,
-    167,
-    168,
-    173,
-    174,
-    175,
-    180,
-    203,
-    204,
-    207,
-    208,
-    209,
-]
-ELE_TAG_Joint = [71, 72, 81, 8181, 82, 83]
-ELE_TAG_Tetrahedron = [179, 256, 189]  # four, ten, 189-FEMBubble
-ELE_TAG_Brick = [
-    36,
-    37,
-    38,
-    39,
-    41,
-    42,
-    43,
-    44,
-    45,
-    46,
-    48,
-    49,
-    51,
-    56,
-    57,
-    58,
-    121,
-    122,
-    127,
-]
-ELE_TAG_PFEM = [133, 141, 142, 143, 144, 164, 187, 189, 199, 200, 255]
 # shape dict used to subplots
 shape_dict = {
     1: (1, 1),
     2: (1, 2),
     3: (1, 3),
     4: (2, 2),
     5: (2, 3),
@@ -271,73 +112,73 @@
         "DamBreak", "GridFrame", "Shell3D".
 
     Returns:
     --------
     None
     """
     if name.lower() == "archbridge":
-        from opstool.examples.ArchBridge import ArchBridge
+        from .examples.ArchBridge import ArchBridge
 
         ArchBridge()
         # exec("from opstool.examples.ArchBridge import *")
     elif name.lower() == "archbridge2":
-        from opstool.examples.ArchBridge2 import ArchBridge2
+        from .examples.ArchBridge2 import ArchBridge2
 
         ArchBridge2()
         # exec("from opstool.examples.ArchBridge2 import *")
     elif name.lower() == "cablestayedbridge":
-        from opstool.examples.CableStayedBridge import CableStayedBridge
+        from .examples.CableStayedBridge import CableStayedBridge
 
         CableStayedBridge()
         # exec("from opstool.examples.CableStayedBridge import *")
     elif name.lower() == "dam":
-        from opstool.examples.Dam import Dam
+        from .examples.Dam import Dam
 
         Dam()
         # exec("from opstool.examples.Dam import *")
     elif name.lower() == "frame3d":
-        from opstool.examples.Frame3D import Frame3D
+        from .examples.Frame3D import Frame3D
 
         Frame3D()
         # exec("from opstool.examples.Frame3D import *")
     elif name.lower() == "frame3d2":
-        from opstool.examples.Frame3D2 import Frame3D2
+        from .examples.Frame3D2 import Frame3D2
 
         Frame3D2()
     elif name.lower() == "igloo":
-        from opstool.examples.Igloo import Igloo
+        from .examples.Igloo import Igloo
 
         Igloo()
         # exec("from opstool.examples.Igloo import *")
     elif name.lower() == "pier":
-        from opstool.examples.Pier import Pier
+        from .examples.Pier import Pier
 
         Pier()
         # exec("from opstool.examples.Pier import *")
     elif name.lower() == "suspensionbridge":
-        from opstool.examples.SuspensionBridge import SuspensionBridge
+        from .examples.SuspensionBridge import SuspensionBridge
 
         SuspensionBridge()
         # exec("from opstool.examples.SuspensionBridge import *")
     elif name.lower() == "sdof":
-        from opstool.examples.SDOF import SDOF
+        from .examples.SDOF import SDOF
 
         SDOF()
         # exec("from opstool.examples.SDOF import *")
     elif name.lower() == "dambreak":
-        from opstool.examples.DamBreak import DamBreak
+        from .examples.DamBreak import DamBreak
 
         DamBreak()
         # exec("from opstool.examples.DamBreak import *")
     elif name.lower() == "gridframe":
-        from opstool.examples.GridFrame import GridFrame
+        from .examples.GridFrame import GridFrame
 
         GridFrame()
     elif name.lower() == "shell3d":
-        from opstool.examples.shell3D import Shell3D
+        from .examples.shell3D import Shell3D
 
         Shell3D()
     else:
         print(f"Not supported example {name}!")
         print(f"Now try treating {name} as your own model file and run it!")
         run_model(name)
 
@@ -373,18 +214,20 @@
         import openseespymac.opensees as ops
         tar_file = Path(ops.__file__).resolve().parent / "opensees.pyi"
     else:
         raise RuntimeError(sys.platform + ' is not supported yet')
     tar_file.write_text(src_file.read_text(encoding="utf-8"), encoding="utf-8")
     print(f"opstool:: opensees.pyi file has been created to {tar_file}!")
 
+
 def print_version():
     from .__about__ import __version__
     print(__version__)
 
+
 def _get_random_color():
     colors = [
         "#00aeff",
         "#3369e7",
         "#8e43e7",
         "#b84592",
         "#ff4f81",
```

### Comparing `opstool-0.8.2/src/opstool/vis/_get_model_base.py` & `opstool-0.8.3/src/opstool/vis/_get_model_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -498,14 +498,20 @@
     ele_midpoints = []
     for i, ele in enumerate(ele_tags):
         ele_nodes = ops.eleNodes(ele)
         idxs = [node_index[tag_] for tag_ in ele_nodes]
         ele_midpoints.append(np.mean(node_coords[idxs], axis=0))
     return np.array(ele_midpoints)
 
+def get_ele_class_tags():
+    ele_class_tags = ops.getEleClassTags()
+    # for ele in ele_tags:
+    #     ele_class_tags.append(ops.getEleClassTags(ele)[0])
+    return ele_class_tags
+
 
 def get_bounds(node_coords):
     min_node = np.min(node_coords, axis=0)
     max_node = np.max(node_coords, axis=0)
     space = (max_node - min_node) / 12
     min_node = min_node - space
     max_node = max_node + space
@@ -562,14 +568,15 @@
     all_lines_cells, all_lines_cells_tags = get_all_line_info(ele_tags, node_index)
     plane_cells, plane_cells_tags = get_plane_info(ele_tags, node_index)
     tetrahedron_cells, tetrahedron_cells_tags = get_tet_info(ele_tags, node_index)
     brick_cells, brick_cells_tags = get_bri_info(ele_tags, node_index)
     all_faces_cells = plane_cells + tetrahedron_cells + brick_cells
     all_faces_cells_tags = plane_cells_tags + tetrahedron_cells_tags + brick_cells_tags
     ele_midpoints = get_ele_mid(ele_tags, node_coords, node_index)
+    ele_class_tags = get_ele_class_tags()
     bounds, max_bound, min_bound = get_bounds(node_coords)
     node_load_info, node_load_data = get_node_load(node_index)
     ele_load_info, ele_load_data, ele_load_locals = get_ele_load(node_index)
     model_info = dict()
     model_info["coord_no_deform"] = node_coords
     model_info["coord_ele_midpoints"] = ele_midpoints
     model_info["bound"] = bounds
@@ -582,14 +589,15 @@
     model_info["FixNodeDofs"] = fixed_dofs
     model_info["FixNodeCoords"] = fixed_coords
     model_info["ConstrainedCoords"] = ctra_coords
     model_info["ConstrainedMidCoords"] = ctra_midcoords
     model_info["ConstrainedDofs"] = ctra_dofs
     model_info["ConstrainedCells"] = ctra_cells
     model_info["EleTags"] = ele_tags
+    model_info["EleClassTags"] = ele_class_tags
     model_info["model_dims"] = model_dims
     model_info["coord_ele_midpoints"] = ele_midpoints
     model_info["beam_midpoints"] = beam_midpoints
     model_info["beam_lengths"] = beam_lengths
     model_info["beam_xlocal"] = beam_xlocal
     model_info["beam_ylocal"] = beam_ylocal
     model_info["beam_zlocal"] = beam_zlocal
```

### Comparing `opstool-0.8.2/src/opstool/vis/_plotly_base.py` & `opstool-0.8.3/src/opstool/vis/_plotly_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             vecj.append(len(face_points) + 5)
             veck.append(len(face_points) + 7)
         face_line_points.extend(list(data))
         face_points.extend(list(data0))
     face_line_points = np.array(face_line_points)
     face_points = np.array(face_points)
     face_mid_points = np.array(face_mid_points)
-    return (face_points, face_line_points, face_mid_points, veci, vecj, veck)
+    return face_points, face_line_points, face_mid_points, veci, vecj, veck
 
 
 def _make_lines(points, cells):
     line_points = []
     line_mid_points = []
     for cell in cells:
         data0 = points[cell[1:], :]
@@ -367,15 +367,15 @@
         template=obj.theme,
         autosize=True,
         showlegend=False,
         scene=scene,
         title=dict(
             font=dict(family="courier", color="black", size=25),
             text=(
-                "<b>OpenSeesPy 3D View</b> <br>"
+                "<b>OPSTOOL:: OpenSeesPy 3D Viewer</b> <br>"
                 f"Num. of Node: {model_info['num_node']} || Num. of Ele:{model_info['num_ele']}"
             ),
         ),
     )
     if not show_outline:
         fig.update_layout(
             scene=dict(
@@ -923,18 +923,17 @@
         idx = np.abs(new_ptags - ptag) < 1e-3
         coords = new_points[idx]
         for i in range(3):
             data = np.ravel(load_data[idx, i])
             lengths = np.abs(data) * alpha_
             arrow_heights = [0.4 * ll for ll in lengths]
             arrow_widths = [0.6 * h for h in arrow_heights]
-            new_locals[idx, 3 * i : 3 * i + 3]
-            xaxis = new_locals[idx, idxs[idxsidx[i][0]]]
-            yaxis = new_locals[idx, idxs[idxsidx[i][1]]]
-            zaxis = new_locals[idx, idxs[idxsidx[i][2]]]
+            xaxis = new_locals[np.ix_(idx, idxs[idxsidx[i][0]])]
+            yaxis = new_locals[np.ix_(idx, idxs[idxsidx[i][1]])]
+            zaxis = new_locals[np.ix_(idx, idxs[idxsidx[i][2]])]
             new_coords = np.zeros_like(coords)
             for j in range(len(xaxis)):
                 xaxis[j] *= np.sign(data[j])
                 new_coords[j] = coords[j] - 1.4 * lengths[j] * xaxis[j]
             labels = [f"{d:.2e}" for d in data]
             plotter.extend(
                 _make_lines_arrows(
@@ -1007,25 +1006,25 @@
     with h5py.File(filename, "r") as f:
         grp = f["EigenInfo"]
         for name, value in grp.items():
             eigen_data[name] = value[...]
     eigen_data["all_lines"] = _reshape_cell(eigen_data["all_lines"])
     eigen_data["all_faces"] = _reshape_cell(eigen_data["all_faces"])
 
-    f = eigen_data["f"]
+    f = eigen_data["eigenFrequency"]
     eigenvector = eigen_data["eigenvector"]
     num_mode_tag = len(f)
     modei, modej = mode_tags
     modei, modej = int(modei), int(modej)
     if modej > num_mode_tag:
         raise ValueError(f"Insufficient number of modes in eigen file {filename}!")
 
     fig = go.Figure()
     title = dict(
-        font=dict(family="courier", color="black", size=25),
+        font=dict(family="courier", color="black", size=label_size),
         text="<b>OpenSeesPy Eigen 3D View</b>",
     )
     if show_outline:
         off_axis = {"showgrid": True, "zeroline": True, "visible": True}
     else:
         off_axis = {"showgrid": False, "zeroline": False, "visible": False}
 
@@ -1169,15 +1168,16 @@
             if i == 0:
                 n_data = len(fig.data)
         for i in range(n_data, len(fig.data)):
             fig.data[i].visible = False
         # Create and add slider
         steps = []
         for i, idx in enumerate(range(modei, modej + 1)):
-            txt = "Mode {}: T = {:.3f} s".format(idx, 1 / f[idx - 1])
+            # txt = "Mode {}: T = {:.3f} s".format(idx, 1 / f[idx - 1])
+            txt = _make_eigen_txt(eigen_data, idx-1)
             step = dict(
                 method="update",
                 args=[
                     {"visible": [False] * len(fig.data)},
                     {"title": txt},
                 ],  # layout attribute
                 label=str(idx),
@@ -1232,14 +1232,50 @@
     if save_html:
         if not save_html.endswith(".html"):
             save_html += ".html"
         pio.write_html(fig, file=save_html, auto_open=True)
     return fig
 
 
+def _make_eigen_txt(eigen_data, step):
+    fi = eigen_data["eigenFrequency"][step]
+    txt = f"<b>Mode {step + 1}</b><br>period: {1 / fi:.6f} s; freq: {fi:.6f} Hz\n"
+    if np.max(eigen_data["model_dims"]) <= 2:
+        txt += "<br>modal participation mass ratios (%)"
+        mx = eigen_data["partiMassRatiosMX"][step]
+        my = eigen_data["partiMassRatiosMY"][step]
+        rmz = eigen_data["partiMassRatiosRMZ"][step]
+        txt += f"<br>{mx:7.3f} {my:7.3f} {rmz:7.3f}"
+        txt += "<br>cumulative modal participation mass ratios (%)"
+        mx = eigen_data["partiMassRatiosCumuMX"][step]
+        my = eigen_data["partiMassRatiosCumuMY"][step]
+        rmz = eigen_data["partiMassRatiosCumuRMZ"][step]
+        txt += f"<br>{mx:7.3f} {my:7.3f} {rmz:7.3f}"
+        txt += "<br>{:>7} {:>7} {:>7}".format("X", "Y", "RZ")
+    else:
+        txt += "<br>modal participation mass ratios (%)"
+        mx = eigen_data["partiMassRatiosMX"][step]
+        my = eigen_data["partiMassRatiosMY"][step]
+        mz = eigen_data["partiMassRatiosMZ"][step]
+        rmx = eigen_data["partiMassRatiosRMX"][step]
+        rmy = eigen_data["partiMassRatiosRMY"][step]
+        rmz = eigen_data["partiMassRatiosRMZ"][step]
+        txt += f"<br>{mx:7.3f} {my:7.3f} {mz:7.3f} {rmx:7.3f} {rmy:7.3f} {rmz:7.3f}"
+        txt += "<br>cumulative modal participation mass ratios (%)"
+        mx = eigen_data["partiMassRatiosCumuMX"][step]
+        my = eigen_data["partiMassRatiosCumuMY"][step]
+        mz = eigen_data["partiMassRatiosCumuMZ"][step]
+        rmx = eigen_data["partiMassRatiosCumuRMX"][step]
+        rmy = eigen_data["partiMassRatiosCumuRMY"][step]
+        rmz = eigen_data["partiMassRatiosCumuRMZ"][step]
+        txt += f"<br>{mx:7.3f} {my:7.3f} {mz:7.3f} {rmx:7.3f} {rmy:7.3f} {rmz:7.3f}"
+        txt += "<br>{:>7} {:>7} {:>7} {:>7} {:>7} {:>7}".format("X", "Y", "Z", "RX", "RY", "RZ")
+    return txt
+
+
 def _eigen_anim(
     obj,
     mode_tag: int = 1,
     input_file: str = "EigenData.hdf5",
     n_cycle: int = 5,
     alpha: float = 1.0,
     show_outline: bool = False,
```

### Comparing `opstool-0.8.2/src/opstool/vis/_pyvista_base.py` & `opstool-0.8.3/src/opstool/vis/_pyvista_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,32 +3,33 @@
 import h5py
 import numpy as np
 import matplotlib.pyplot as plt
 import pyvista as pv
 
 from ..utils import check_file, shape_dict
 
+
 def _model_vis(
-    obj,
-    input_file: str = "ModelData.hdf5",
-    show_node_label: bool = False,
-    show_ele_label: bool = False,
-    label_size: float = 10,
-    show_local_crd: bool = False,
-    local_crd_alpha: float = 1.0,
-    show_fix_node: bool = True,
-    fix_node_alpha: float = 1.0,
-    show_load: bool = False,
-    load_alpha: float = 1.0,
-    show_constrain_dof: bool = False,
-    show_beam_sec: bool = False,
-    beam_sec_paras: dict = None,
-    show_outline: bool = True,
-    opacity: float = 1.0,
-    save_fig: str = "ModelVis.svg",
+        obj,
+        input_file: str = "ModelData.hdf5",
+        show_node_label: bool = False,
+        show_ele_label: bool = False,
+        label_size: float = 10,
+        show_local_crd: bool = False,
+        local_crd_alpha: float = 1.0,
+        show_fix_node: bool = True,
+        fix_node_alpha: float = 1.0,
+        show_load: bool = False,
+        load_alpha: float = 1.0,
+        show_constrain_dof: bool = False,
+        show_beam_sec: bool = False,
+        beam_sec_paras: dict = None,
+        show_outline: bool = True,
+        opacity: float = 1.0,
+        save_fig: str = "ModelVis.svg",
 ):
     filename = obj.out_dir + "/" + input_file
     model_info = dict()
     cells = dict()
     with h5py.File(filename, "r") as f:
         grp1 = f["ModelInfo"]
         for name in grp1.keys():
@@ -36,16 +37,16 @@
         grp2 = f["Cell"]
         for name in grp2.keys():
             cells[name] = grp2[name][...]
 
     plotter = pv.Plotter(notebook=obj.notebook, line_smoothing=True)
     _plot_model(obj, plotter, model_info, cells, opacity)
 
-    txt = f"OpenSees 3D View\nNum. of Node:{model_info['num_node']}\nNum. of Ele:{model_info['num_ele']}"
-    plotter.add_text(txt, position="upper_right", font_size=12, font="courier")
+    txt = f"OPSTOOL:: Num. Node: {model_info['num_node']} Num. Ele: {model_info['num_ele']}"
+    plotter.add_text(txt, position="lower_right", font_size=8, font="courier")
     if show_outline:
         show_zaxis = False if np.max(model_info["model_dims"]) <= 2 else True
         plotter.show_bounds(
             grid=False,
             location="outer",
             bounds=model_info["bound"],
             show_zaxis=show_zaxis,
@@ -94,17 +95,17 @@
     if show_load:
         _show_node_load(plotter, model_info, load_alpha)
         _show_ele_load(plotter, model_info, load_alpha)
     plotter.add_axes()
     plotter.view_isometric()
     if np.max(model_info["model_dims"]) <= 2:
         plotter.view_xy(negative=False)
+    plotter.enable_anti_aliasing("msaa")
     if save_fig:
         plotter.save_graphic(save_fig)
-    plotter.enable_anti_aliasing("msaa")
     plotter.show(title=obj.title)
     plotter.close()
 
 
 def _show_mp_constraint(obj, plotter, model_info, show_dofs):
     points = model_info["ConstrainedCoords"]
     cells = model_info["ConstrainedCells"]
@@ -184,15 +185,15 @@
     node_load_data = np.array(model_info["node_load_data"])
     if len(node_load_info) == 0:
         return None
     loc, load_data = 0, []
     for info in node_load_info:
         ndm = info[2]
         ndf = info[3]
-        data = node_load_data[loc : loc + ndf]
+        data = node_load_data[loc: loc + ndf]
         if ndm <= 2 and ndf <= 3:
             load_data.append([data[0], data[1], 0])  # x, y
         else:
             load_data.append([data[0], data[1], data[2]])  # x, y, z
         loc += ndf
     load_data = np.array(load_data)
     maxdata = np.max(np.abs(load_data))
@@ -239,48 +240,48 @@
     load_data = []
     loc = 0
     for i, info in enumerate(ele_load_info):
         ptag, _, classtag, nidx1, nidx2 = info
         coord1, coord2 = points[nidx1], points[nidx2]
         local_axis = ele_load_locals[i]
         if classtag == 3:  # beamUniform2D, Wya <Wxa>
-            wy, wx = ele_load_data[loc : loc + 2]
+            wy, wx = ele_load_data[loc: loc + 2]
             wz = 0.0
             n = 11
             xl = np.linspace(0, 1, n)
             wx, wy, wz = [wx] * n, [wy] * n, [wz] * n
             localaxis = [local_axis] * n
             new_ptags.extend([ptag] * n)
             loc += 2
         elif classtag == 12:  # beamUniform2D, Wya <Wxa> <aL> <bL> <Wyb> <Wxb>
-            wya, wyb, wxa, wxb, al, bl = ele_load_data[loc : loc + 6]
+            wya, wyb, wxa, wxb, al, bl = ele_load_data[loc: loc + 6]
             n = int((bl - al) / 0.1) + 1
             xl = np.linspace(al, bl, n)
             wy = np.interp(xl, [0, 1], [wya, wyb])
             wx = np.interp(xl, [0, 1], [wxa, wxb])
             wz = wy * 0
             localaxis = [local_axis] * n
             new_ptags.extend([ptag] * n)
             loc += 6
         elif classtag == 5:  # beamUniform3D wy, wz, wx
-            wy, wz, wx = ele_load_data[loc : loc + 3]
+            wy, wz, wx = ele_load_data[loc: loc + 3]
             n = 11
             xl = np.linspace(0, 1, n)
             wx, wy, wz = [wx] * n, [wy] * n, [wz] * n
             localaxis = [local_axis] * n
             new_ptags.extend([ptag] * n)
             loc += 3
         elif classtag == 4:  # beamPoint2D, Py xL <Px>
-            wy, wx, xl = ele_load_data[loc : loc + 3]
+            wy, wx, xl = ele_load_data[loc: loc + 3]
             wz = 0
             localaxis = [local_axis]
             new_ptags.append(ptag)
             loc += 3
         elif classtag == 6:  # beamPoint3D, Py, Pz, x, N
-            wy, wz, wx, xl = ele_load_data[loc : loc + 4]
+            wy, wz, wx, xl = ele_load_data[loc: loc + 4]
             localaxis = [local_axis]
             new_ptags.append(ptag)
             loc += 4
         else:
             warnings.warn(
                 "Currently load visualization only supports-->"
                 "<beamUniform2D,beamUniform3D,beamPoint2D,beamPoint3D>!"
@@ -310,25 +311,25 @@
     for p, ptag in enumerate(patterntags):
         idx = np.abs(new_ptags - ptag) < 1e-3
         coords = new_points[idx]
         for i in range(3):
             ply = pv.PolyData(coords)
             data = np.ravel(load_data[idx, i])
             ply["scalars"] = np.abs(data)
-            ply["vectors"] = new_locals[idx, 3 * i : 3 * i + 3]
+            ply["vectors"] = new_locals[idx, 3 * i: 3 * i + 3]
             for j in range(len(ply["vectors"])):
                 ply["vectors"][j] *= np.sign(data[j])
             glyphs = ply.glyph(
                 orient="vectors", scale="scalars", factor=alpha_, geom=geom
             )
             plotter.add_mesh(glyphs, show_scalar_bar=False, color=colors[p])
 
 
 def _show_beam_local_axes(
-    plotter, model_info, alpha: float = 1.0, label_size: float = 10
+        plotter, model_info, alpha: float = 1.0, label_size: float = 10
 ):
     beam_xlocal = model_info["beam_xlocal"]
     beam_ylocal = model_info["beam_ylocal"]
     beam_zlocal = model_info["beam_zlocal"]
     beam_midpoints = model_info["beam_midpoints"]
     beam_lengths = model_info["beam_lengths"]
     if len(beam_lengths) > 0:
@@ -370,15 +371,15 @@
             always_visible=True,
         )
     else:
         warnings.warn("Model has no frame elements when show_local_crd=True!")
 
 
 def _show_link_local_axes(
-    plotter, model_info, alpha: float = 1.0, label_size: float = 10
+        plotter, model_info, alpha: float = 1.0, label_size: float = 10
 ):
     link_xlocal = model_info["link_xlocal"]
     link_ylocal = model_info["link_ylocal"]
     link_zlocal = model_info["link_zlocal"]
     link_midpoints = model_info["link_midpoints"]
     link_lengths = model_info["link_lengths"]
     if len(link_midpoints) > 0:
@@ -537,17 +538,17 @@
         length = np.sqrt(np.sum((coord2 - coord1) ** 2))
         if np.abs(length) < 1e-8:
             points_zero.append(coord1)
         else:
             xaxis = np.array(coord2 - coord1)
             global_z = [0.0, 0.0, 1.0]
             cos_angle = xaxis.dot(global_z) / (
-                np.linalg.norm(xaxis) * np.linalg.norm(global_z)
+                    np.linalg.norm(xaxis) * np.linalg.norm(global_z)
             )
-            if np.abs(1 - cos_angle**2) < 1e-10:
+            if np.abs(1 - cos_angle ** 2) < 1e-10:
                 yaxis = np.cross([-1.0, 0.0, 0.0], xaxis)
             else:
                 yaxis = np.cross(global_z, xaxis)
             xaxis = xaxis / np.linalg.norm(xaxis)
             yaxis = yaxis / np.linalg.norm(yaxis)
             idx = len(points_nonzero)
             for i in range(5):
@@ -656,56 +657,59 @@
         )
         plotter.add_mesh(
             bri_plot, color=obj.color_solid, show_edges=True, opacity=opacity
         )
 
 
 def _eigen_vis(
-    obj,
-    mode_tags: list,
-    input_file: str = "EigenData.hdf5",
-    subplots: bool = False,
-    link_views: bool = True,
-    alpha: float = 1.0,
-    show_outline: bool = False,
-    show_origin: bool = False,
-    label_size: float = 15,
-    opacity: float = 1.0,
-    show_face_line: bool = True,
-    save_fig: str = "EigenVis.svg",
+        obj,
+        mode_tags: list,
+        input_file: str = "EigenData.hdf5",
+        subplots: bool = False,
+        link_views: bool = True,
+        alpha: float = 1.0,
+        show_outline: bool = False,
+        show_origin: bool = False,
+        label_size: float = 15,
+        opacity: float = 1.0,
+        show_face_line: bool = True,
+        save_fig: str = "EigenVis.svg",
 ):
     filename = obj.out_dir + "/" + input_file
     eigen_data = dict()
     with h5py.File(filename, "r") as f:
         grp = f["EigenInfo"]
         for name, value in grp.items():
             eigen_data[name] = value[...]
 
-    f = eigen_data["f"]
+    f = eigen_data["eigenFrequency"]
+    # T = eigen_data["eigenPeriod"]
     eigenvector = eigen_data["eigenvector"]
     show_zaxis = False if np.max(eigen_data["model_dims"]) <= 2 else True
     num_mode_tag = len(f)
     modei, modej = mode_tags
     modei, modej = int(modei), int(modej)
     if modej > num_mode_tag:
         raise ValueError(f"Insufficient number of modes in eigen file {filename}!")
 
     # -----------------------------------------------------------------------
     def create_mesh(idx, idxi=None, idxj=None):
         if idxi is not None and idxj is not None:
             plotter.subplot(idxi, idxj)
+            subplots = True
         else:
             plotter.clear_actors()
+            subplots = False
         step = int(round(idx)) - 1
         eigen_vec = eigenvector[step]
-        value_ = np.max(np.sqrt(np.sum(eigen_vec**2, axis=1)))
+        value_ = np.max(np.sqrt(np.sum(eigen_vec ** 2, axis=1)))
         alpha_ = eigen_data["max_bound"] / obj.bound_fact / value_
         alpha_ = alpha_ * alpha if alpha else alpha_
         eigen_points = eigen_data["coord_no_deform"] + eigen_vec * alpha_
-        scalars = np.sqrt(np.sum(eigen_vec**2, axis=1))
+        scalars = np.sqrt(np.sum(eigen_vec ** 2, axis=1))
         _ = _generate_all_mesh(
             plotter,
             eigen_points,
             scalars,
             opacity,
             obj.color_map,
             eigen_data["all_lines"],
@@ -714,18 +718,24 @@
             points_origin=eigen_data["coord_no_deform"],
             point_size=obj.point_size,
             line_width=obj.line_width,
             show_face_line=show_face_line,
         )
         # plotter.add_scalar_bar(fmt="%.3e", n_labels=10, label_font_size=12)
         # txt = 'Mode {}\nf = {:.3f} Hz\nT = {:.3f} s'.format(mode_tag, f_, 1 / f_)
-        txt = "Mode {}\nT = {:.3f} s".format(step + 1, 1 / f[step])
-        plotter.add_text(
-            txt, position="upper_left", font_size=label_size, font="courier"
-        )
+        if not subplots:
+            txt = _make_eigen_txt(eigen_data, step)
+            plotter.add_text(
+                txt, position="lower_right", font_size=label_size - 3, font="courier"
+            )
+        else:
+            txt = "Mode {}\nT = {:.3f} s".format(step + 1, 1 / f[step])
+            plotter.add_text(
+                txt, position="upper_left", font_size=label_size, font="courier"
+            )
         if show_outline:
             plotter.show_bounds(
                 grid=False,
                 location="outer",
                 bounds=eigen_data["bound"],
                 show_zaxis=show_zaxis,
                 # color="black",
@@ -762,31 +772,67 @@
             tube_width=0.01,
         )
     plotter.view_isometric()
     if np.max(eigen_data["model_dims"]) <= 2:
         plotter.view_xy(negative=False)
     if save_fig:
         plotter.save_graphic(save_fig)
-    plotter.enable_anti_aliasing("msaa")
+    plotter.enable_anti_aliasing(obj.anti_aliasing)
     plotter.show(title=obj.title)
     plotter.close()
 
 
+def _make_eigen_txt(eigen_data, step):
+    fi = eigen_data["eigenFrequency"][step]
+    txt = f"Mode {step + 1}\nperiod: {1 / fi:.6f} s; freq: {fi:.6f} Hz\n"
+    if np.max(eigen_data["model_dims"]) <= 2:
+        txt += "modal participation mass ratios (%)\n"
+        mx = eigen_data["partiMassRatiosMX"][step]
+        my = eigen_data["partiMassRatiosMY"][step]
+        rmz = eigen_data["partiMassRatiosRMZ"][step]
+        txt += f"{mx:7.3f} {my:7.3f} {rmz:7.3f}\n"
+        txt += "cumulative modal participation mass ratios (%)\n"
+        mx = eigen_data["partiMassRatiosCumuMX"][step]
+        my = eigen_data["partiMassRatiosCumuMY"][step]
+        rmz = eigen_data["partiMassRatiosCumuRMZ"][step]
+        txt += f"{mx:7.3f} {my:7.3f} {rmz:7.3f}\n"
+        txt += "{:>7} {:>7} {:>7}\n".format("X", "Y", "RZ")
+    else:
+        txt += "modal participation mass ratios (%)\n"
+        mx = eigen_data["partiMassRatiosMX"][step]
+        my = eigen_data["partiMassRatiosMY"][step]
+        mz = eigen_data["partiMassRatiosMZ"][step]
+        rmx = eigen_data["partiMassRatiosRMX"][step]
+        rmy = eigen_data["partiMassRatiosRMY"][step]
+        rmz = eigen_data["partiMassRatiosRMZ"][step]
+        txt += f"{mx:7.3f} {my:7.3f} {mz:7.3f} {rmx:7.3f} {rmy:7.3f} {rmz:7.3f}\n"
+        txt += "cumulative modal participation mass ratios (%)\n"
+        mx = eigen_data["partiMassRatiosCumuMX"][step]
+        my = eigen_data["partiMassRatiosCumuMY"][step]
+        mz = eigen_data["partiMassRatiosCumuMZ"][step]
+        rmx = eigen_data["partiMassRatiosCumuRMX"][step]
+        rmy = eigen_data["partiMassRatiosCumuRMY"][step]
+        rmz = eigen_data["partiMassRatiosCumuRMZ"][step]
+        txt += f"{mx:7.3f} {my:7.3f} {mz:7.3f} {rmx:7.3f} {rmy:7.3f} {rmz:7.3f}\n"
+        txt += "{:>7} {:>7} {:>7} {:>7} {:>7} {:>7}\n".format("X", "Y", "Z", "RX", "RY", "RZ")
+    return txt
+
+
 def _eigen_anim(
-    obj,
-    mode_tag: int = 1,
-    input_file: str = "EigenData.hdf5",
-    n_cycle: int = 5,
-    label_size: float = 15,
-    alpha: float = None,
-    show_outline: bool = False,
-    opacity: float = 1,
-    framerate: int = 3,
-    show_face_line: bool = True,
-    save_fig: str = "EigenAnimation.gif",
+        obj,
+        mode_tag: int = 1,
+        input_file: str = "EigenData.hdf5",
+        n_cycle: int = 5,
+        label_size: float = 15,
+        alpha: float = None,
+        show_outline: bool = False,
+        opacity: float = 1,
+        framerate: int = 3,
+        show_face_line: bool = True,
+        save_fig: str = "EigenAnimation.gif",
 ):
     filename = obj.out_dir + "/" + input_file
     eigen_data = dict()
     with h5py.File(filename, "r") as f:
         grp = f["EigenInfo"]
         for name, value in grp.items():
             eigen_data[name] = value[...]
@@ -794,31 +840,31 @@
     f = eigen_data["f"]
     eigenvector = eigen_data["eigenvector"]
     num_mode_tag = len(f)
     if mode_tag > num_mode_tag:
         raise ValueError("Insufficient number of modes in open file")
     eigen_vec = eigenvector[mode_tag - 1]
     f_ = f[mode_tag - 1]
-    value_ = np.max(np.sqrt(np.sum(eigen_vec**2, axis=1)))
+    value_ = np.max(np.sqrt(np.sum(eigen_vec ** 2, axis=1)))
     alpha_ = eigen_data["max_bound"] / obj.bound_fact / value_
     alpha_ = alpha_ * alpha if alpha else alpha_
     eigen_points = eigen_data["coord_no_deform"] + eigen_vec * alpha_
     anti_eigen_points = eigen_data["coord_no_deform"] - eigen_vec * alpha_
-    scalars = np.sqrt(np.sum(eigen_vec**2, axis=1))
+    scalars = np.sqrt(np.sum(eigen_vec ** 2, axis=1))
     plt_points = [anti_eigen_points, eigen_data["coord_no_deform"], eigen_points]
     # -----------------------------------------------------------------------------
     # start plot
     plotter = pv.Plotter(notebook=obj.notebook, line_smoothing=True)
 
-    value_ = np.max(np.sqrt(np.sum(eigen_vec**2, axis=1)))
+    value_ = np.max(np.sqrt(np.sum(eigen_vec ** 2, axis=1)))
     alpha_ = eigen_data["max_bound"] / obj.bound_fact / value_
     alpha_ = alpha_ * alpha if alpha else alpha_
     eigen_points = eigen_data["coord_no_deform"] + eigen_vec * alpha_
     anti_eigen_points = eigen_data["coord_no_deform"] - eigen_vec * alpha_
-    scalars = np.sqrt(np.sum(eigen_vec**2, axis=1))
+    scalars = np.sqrt(np.sum(eigen_vec ** 2, axis=1))
     point_plot, line_plot, face_plot = _generate_all_mesh(
         plotter,
         eigen_data["coord_no_deform"],
         scalars * 0,
         opacity,
         obj.color_map,
         eigen_data["all_lines"],
@@ -863,42 +909,42 @@
     plt_points = [anti_eigen_points, eigen_data["coord_no_deform"], eigen_points]
     render = False
     index = [2, 0] * n_cycle
     plotter.write_frame()  # write initial data
     for idx in index:
         points = plt_points[idx]
         xyz = (eigen_data["coord_no_deform"] - points) / alpha_
-        xyz_eigen = np.sqrt(np.sum(xyz**2, axis=1))
+        xyz_eigen = np.sqrt(np.sum(xyz ** 2, axis=1))
         if point_plot:
             plotter.update_coordinates(points, mesh=point_plot, render=render)
             plotter.update_scalars(scalars=xyz_eigen, mesh=point_plot, render=render)
         if line_plot:
             plotter.update_scalars(scalars=xyz_eigen, mesh=line_plot, render=render)
             plotter.update_coordinates(points, mesh=line_plot, render=render)
         if face_plot:
             plotter.update_scalars(scalars=xyz_eigen, mesh=face_plot, render=render)
             plotter.update_coordinates(points, mesh=face_plot, render=render)
         plotter.update_scalar_bar_range(
             clim=[np.min(xyz_eigen), np.max(xyz_eigen)], name=None
         )
         plotter.write_frame()
     # ----------------------------------------------------------------------------------
-    plotter.enable_anti_aliasing("msaa")
+    plotter.enable_anti_aliasing(obj.anti_aliasing)
     plotter.show(title=obj.title)
     plotter.close()
 
 
 def _react_vis(
-    obj,
-    input_file: str = "NodeReactionStepData-1.hdf5",
-    slider: bool = False,
-    direction: str = "Fz",
-    show_values: bool = True,
-    show_outline: bool = False,
-    save_fig: str = "ReactionVis.svg",
+        obj,
+        input_file: str = "NodeReactionStepData-1.hdf5",
+        slider: bool = False,
+        direction: str = "Fz",
+        show_values: bool = True,
+        show_outline: bool = False,
+        save_fig: str = "ReactionVis.svg",
 ):
     direct = direction.lower()
     if direct not in ["fx", "fy", "fz", "mx", "my", "mz"]:
         raise ValueError(
             "response must be one of ['Fx', 'Fy', 'Fz', 'Mx', 'My', 'Mz']!"
         )
     filename = obj.out_dir + "/" + input_file
@@ -1034,31 +1080,31 @@
         )
         create_mesh(idx + 1)
     plotter.view_isometric()
     if D2:
         plotter.view_xy(negative=False)
     if save_fig:
         plotter.save_graphic(save_fig)
-    plotter.enable_anti_aliasing("msaa")
+    plotter.enable_anti_aliasing(obj.anti_aliasing)
     plotter.show(title=obj.title)
     plotter.close()
 
 
 def _deform_vis(
-    obj,
-    input_file: str = "NodeRespStepData-1.hdf5",
-    slider: bool = False,
-    response: str = "disp",
-    alpha: float = 1.0,
-    show_outline: bool = False,
-    show_origin: bool = False,
-    show_face_line: bool = True,
-    opacity: float = 1,
-    save_fig: str = "DefoVis.svg",
-    model_update: bool = False,
+        obj,
+        input_file: str = "NodeRespStepData-1.hdf5",
+        slider: bool = False,
+        response: str = "disp",
+        alpha: float = 1.0,
+        show_outline: bool = False,
+        show_origin: bool = False,
+        show_face_line: bool = True,
+        opacity: float = 1,
+        save_fig: str = "DefoVis.svg",
+        model_update: bool = False,
 ):
     resp_type = response.lower()
     if resp_type not in ["disp", "vel", "accel"]:
         raise ValueError("response must be 'disp', 'vel', or 'accel'!")
 
     filename = obj.out_dir + "/" + input_file
     model_info_steps = dict()
@@ -1089,33 +1135,33 @@
             temp = []
             for i in range(n):
                 temp.append(value_[f"step{i + 1}"][...])
             node_resp_steps[name] = temp
     num_steps = len(node_resp_steps["disp"])
     # ! max response
     max_resps = [
-        np.max(np.sqrt(np.sum(resp_**2, axis=1)))
+        np.max(np.sqrt(np.sum(resp_ ** 2, axis=1)))
         for resp_ in node_resp_steps[resp_type]
     ]
     max_step = np.argmax(max_resps)
     max_node_resp = node_resp_steps[resp_type][max_step]
-    scalars = np.sqrt(np.sum(max_node_resp**2, axis=1))
+    scalars = np.sqrt(np.sum(max_node_resp ** 2, axis=1))
     cmin, cmax = np.min(scalars), np.max(scalars)
     if model_update:
         bounds = model_info_steps["bound"][0]
         model_dims = model_info_steps["model_dims"][0]
     else:
         bounds = model_info_steps["bound"]
         model_dims = model_info_steps["model_dims"]
     # scale factor
     if resp_type == "disp":
         max_bound = np.max(
             [bounds[1] - bounds[0], bounds[3] - bounds[2], bounds[5] - bounds[4]]
         )
-        value = np.max(np.sqrt(np.sum(max_node_resp**2, axis=1)))
+        value = np.max(np.sqrt(np.sum(max_node_resp ** 2, axis=1)))
         alpha_ = max_bound / obj.bound_fact / value
         alpha_ = alpha_ * alpha if alpha else alpha_
     else:
         alpha_ = 0
     # ------------------------------------------------------------------------
     # Start plot
     # -------------------------------------------------------------------------
@@ -1131,16 +1177,16 @@
         else:
             node_nodeform_coords = model_info_steps["coord_no_deform"]
             bounds = model_info_steps["bound"]
             lines_cells = cell_steps["all_lines"]
             faces_cells = cell_steps["all_faces"]
         node_resp = node_resp_steps[resp_type][step]
         node_deform_coords = alpha_ * node_resp + node_nodeform_coords
-        scalars = np.sqrt(np.sum(node_resp**2, axis=1))
-        plotter.clear_actors()  # !!!!!!
+        scalars = np.sqrt(np.sum(node_resp ** 2, axis=1))
+        plotter.clear_actors()  # ! clear
         _ = _generate_all_mesh(
             plotter,
             node_deform_coords,
             scalars,
             opacity,
             obj.color_map,
             lines_cells=lines_cells,
@@ -1213,29 +1259,29 @@
     else:  # plot a single step
         create_mesh(max_step + 1)
     plotter.view_isometric()
     if np.max(model_dims) <= 2:
         plotter.view_xy(negative=False)
     if save_fig:
         plotter.save_graphic(save_fig)
-    plotter.enable_anti_aliasing("msaa")
+    plotter.enable_anti_aliasing(obj.anti_aliasing)
     plotter.show(title=obj.title)
     plotter.close()
 
 
 def _deform_peak_vis(
-    obj,
-    input_file: str = "NodeRespStepData-1.hdf5",
-    response: str = "disp",
-    alpha: float = 1.0,
-    show_outline: bool = False,
-    show_origin: bool = False,
-    show_face_line: bool = True,
-    opacity: float = 1,
-    save_fig: str = "DefoVis.svg",
+        obj,
+        input_file: str = "NodeRespStepData-1.hdf5",
+        response: str = "disp",
+        alpha: float = 1.0,
+        show_outline: bool = False,
+        show_origin: bool = False,
+        show_face_line: bool = True,
+        opacity: float = 1,
+        save_fig: str = "DefoVis.svg",
 ):
     resp_type = response.lower()
     if resp_type not in ["disp", "vel", "accel"]:
         raise ValueError("response must be 'disp', 'vel', or 'accel'!")
 
     filename = obj.out_dir + "/" + input_file
     model_info_steps = dict()
@@ -1258,15 +1304,15 @@
     # ! max response
     idxs = np.argmax(np.abs(node_resp_steps[resp_type]), axis=0)
     node_resp = np.zeros_like(idxs, dtype=float)
     for i in range(idxs.shape[0]):
         for j in range(idxs.shape[1]):
             node_resp[i, j] = node_resp_steps[resp_type][idxs[i, j]][i, j]
     max_resps = np.amax(np.abs(node_resp_steps[resp_type]), axis=0)
-    scalars = np.sqrt(np.sum(max_resps**2, axis=1))
+    scalars = np.sqrt(np.sum(max_resps ** 2, axis=1))
     cmin, cmax = np.min(scalars), np.max(scalars)
     bounds = model_info_steps["bound"]
     model_dims = model_info_steps["model_dims"]
     # scale factor
     if resp_type == "disp":
         max_bound = np.max(
             [bounds[1] - bounds[0], bounds[3] - bounds[2], bounds[5] - bounds[4]]
@@ -1340,30 +1386,30 @@
         )
     plotter.add_axes()
     plotter.view_isometric()
     if np.max(model_dims) <= 2:
         plotter.view_xy(negative=False)
     if save_fig:
         plotter.save_graphic(save_fig)
-    plotter.enable_anti_aliasing("msaa")
+    plotter.enable_anti_aliasing(obj.anti_aliasing)
     plotter.show(title=obj.title)
     plotter.close()
 
 
 def _deform_anim(
-    obj,
-    input_file: str = "NodeRespStepData-1.hdf5",
-    response: str = "disp",
-    alpha: float = 1.0,
-    show_outline: bool = False,
-    opacity: float = 1,
-    framerate: int = 24,
-    show_face_line: bool = True,
-    save_fig: str = "DefoAnimation.gif",
-    model_update: bool = False,
+        obj,
+        input_file: str = "NodeRespStepData-1.hdf5",
+        response: str = "disp",
+        alpha: float = 1.0,
+        show_outline: bool = False,
+        opacity: float = 1,
+        framerate: int = 24,
+        show_face_line: bool = True,
+        save_fig: str = "DefoAnimation.gif",
+        model_update: bool = False,
 ):
     resp_type = response.lower()
     if resp_type not in ["disp", "vel", "accel"]:
         raise ValueError("response must be 'disp', 'vel', or 'accel'!")
 
     filename = obj.out_dir + "/" + input_file
     model_info_steps = dict()
@@ -1396,33 +1442,33 @@
                 temp.append(value_[f"step{i + 1}"][...])
             node_resp_steps[name] = temp
 
     num_steps = len(node_resp_steps["disp"])
 
     # ! max response
     max_resps = [
-        np.max(np.sqrt(np.sum(resp_**2, axis=1)))
+        np.max(np.sqrt(np.sum(resp_ ** 2, axis=1)))
         for resp_ in node_resp_steps[resp_type]
     ]
     max_step = np.argmax(max_resps)
     max_node_resp = node_resp_steps[resp_type][max_step]
-    scalars = np.sqrt(np.sum(max_node_resp**2, axis=1))
+    scalars = np.sqrt(np.sum(max_node_resp ** 2, axis=1))
     cmin, cmax = np.min(scalars), np.max(scalars)
     if model_update:
         bounds = model_info_steps["bound"][0]
         model_dims = model_info_steps["model_dims"][0]
     else:
         bounds = model_info_steps["bound"]
         model_dims = model_info_steps["model_dims"]
     # scale factor
     if resp_type == "disp":
         max_bound = np.max(
             [bounds[1] - bounds[0], bounds[3] - bounds[2], bounds[5] - bounds[4]]
         )
-        value = np.max(np.sqrt(np.sum(max_node_resp**2, axis=1)))
+        value = np.max(np.sqrt(np.sum(max_node_resp ** 2, axis=1)))
         alpha_ = max_bound / obj.bound_fact / value
         alpha_ = alpha_ * alpha if alpha else alpha_
     else:
         alpha_ = 0
     # -----------------------------------------------------------------------------
     # start plot
     plotter = pv.Plotter(notebook=obj.notebook, line_smoothing=True)
@@ -1436,15 +1482,15 @@
         else:
             node_nodeform_coords = model_info_steps["coord_no_deform"]
             bounds = model_info_steps["bound"]
             lines_cells = cell_steps["all_lines"]
             faces_cells = cell_steps["all_faces"]
         node_resp = node_resp_steps[resp_type][step]
         node_deform_coords = alpha_ * node_resp + node_nodeform_coords
-        scalars = np.sqrt(np.sum(node_resp**2, axis=1))
+        scalars = np.sqrt(np.sum(node_resp ** 2, axis=1))
         plotter.clear_actors()  # !!!!!!
         point_plot, line_plot, face_plot = _generate_all_mesh(
             plotter,
             node_deform_coords,
             scalars,
             opacity,
             obj.color_map,
@@ -1501,29 +1547,29 @@
         plotter.open_movie(save_fig, framerate=framerate)
     # plotter.write_frame()  # write initial data
     for step in range(num_steps):
         _ = creat_mesh(step)
         plotter.write_frame()
 
     # ----------------------------------------------------------------------------------
-    plotter.enable_anti_aliasing("msaa")
+    plotter.enable_anti_aliasing(obj.anti_aliasing)
     plotter.show(title=obj.title)
     plotter.close()
 
 
 def _frame_resp_vis(
-    obj,
-    input_file: str = "BeamRespStepData-1.hdf5",
-    ele_tags: list = None,
-    slider: bool = False,
-    response: str = "Mz",
-    show_values=True,
-    alpha: float = 1.0,
-    opacity: float = 1,
-    save_fig: str = "FrameRespVis.svg",
+        obj,
+        input_file: str = "BeamRespStepData-1.hdf5",
+        ele_tags: list = None,
+        slider: bool = False,
+        response: str = "Mz",
+        show_values=True,
+        alpha: float = 1.0,
+        opacity: float = 1,
+        save_fig: str = "FrameRespVis.svg",
 ):
     check_file(save_fig, [".svg", ".eps", ".ps", "pdf", ".tex"])
     filename = obj.out_dir + "/" + input_file
     beam_infos = dict()
     beam_resp_step = dict()
     with h5py.File(filename, "r") as f:
         n = int(f["Nsteps"][...])
@@ -1734,15 +1780,15 @@
     else:  # plot a single step
         create_mesh(maxstep + 1)
     plotter.view_isometric()
     if np.max(np.abs(beam_node_coords[:, -1])) < 1e-5:
         plotter.view_xy(negative=False)
     if save_fig:
         plotter.save_graphic(save_fig)
-    plotter.enable_anti_aliasing("msaa")
+    plotter.enable_anti_aliasing(obj.anti_aliasing)
     plotter.show(title=obj.title)
     plotter.close()
 
 
 def _generate_mesh(points, cells, kind="line"):
     """
     generate the mesh from the points and cells
@@ -1757,28 +1803,28 @@
         pltr.faces = cells
     else:
         raise ValueError(f"not supported {kind}!")
     return pltr
 
 
 def _generate_all_mesh(
-    plotter,
-    points,
-    scalars,
-    opacity,
-    colormap,
-    lines_cells,
-    face_cells,
-    show_origin=False,
-    points_origin=None,
-    show_scalar_bar=False,
-    point_size=1,
-    line_width=1,
-    show_face_line=True,
-    clim=None,
+        plotter,
+        points,
+        scalars,
+        opacity,
+        colormap,
+        lines_cells,
+        face_cells,
+        show_origin=False,
+        points_origin=None,
+        show_scalar_bar=False,
+        point_size=1,
+        line_width=1,
+        show_face_line=True,
+        clim=None,
 ):
     """
     Auxiliary function for generating all meshes
     """
     if clim is None:
         clim = [np.min(scalars), np.max(scalars)]
     sargs = dict(
```

### Comparing `opstool-0.8.2/src/opstool/vis/fiber_sec_vis.py` & `opstool-0.8.3/src/opstool/vis/fiber_sec_vis.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/vis/get_model_data.py` & `opstool-0.8.3/src/opstool/vis/get_model_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Union
 
 import h5py
 import numpy as np
 import openseespy.opensees as ops
 from rich import print
 
-from ..utils import check_file
+from ..utils import check_file, EleTypeTags
 from ._get_model_base import (
     get_beam_info2,
     get_beam_resp,
     get_model_info,
     get_node_coords,
     get_node_react,
     get_node_resp,
@@ -150,16 +150,19 @@
         self._reset_fiber_step()
         self.resp_step_track = 0
 
         # Truss Element Analysis Step Response Data
 
         # Beam Element Analysis Step Response Data
 
-    def get_model_data(
-        self, beam_sec: dict = None, save_file: Union[str, bool] = "ModelData.hdf5"
+    def get_model_data(self,
+                       beam_sec: dict = None,
+                       save_file: Union[str, bool] = "ModelData.hdf5",
+                       print_model_info: bool = True
+
     ):
         """Get data from the current model domain.
         The data will saved to file ``results_dir`` + ``save_file`` in hdf5 style.
 
         Parameters
         -----------
         beam_sec: dict, default=None
@@ -169,36 +172,53 @@
         save_file: str, default="ModelData.hdf5"
             The file name that data saved.
             If None of False, the data will not be saved.
 
             .. warning::
                 Be careful not to include any path, only filename,
                 the file will be saved to the directory ``results_dir``.
+        print_model_info: bool, default=True
+            If True, print the model information.
 
         """
         if save_file:
             check_file(save_file, [".hdf5", ".h5", ".he5"])
         # --------------------------------
         model_info, cells = get_model_info(sec_mesh=beam_sec)
         self.model_info.update(model_info)
         self.cells.update(cells)
         self.get_model_data_finished = True
+        if print_model_info:
+            self._print_model_info(model_info)
         if save_file:
             output_filename = self.out_dir + "/" + save_file
             with h5py.File(output_filename, "w") as f:
                 grp1 = f.create_group("ModelInfo")
                 for name, value in self.model_info.items():
                     grp1.create_dataset(name, data=value)
                 grp2 = f.create_group("Cell")
                 for name, value in self.cells.items():
                     grp2.create_dataset(name, data=value)
             print(
                 f"Model data saved in [bold {next(self.colors_cycle)}]{output_filename}[/]!"
             )
 
+    @staticmethod
+    def _print_model_info(model_info):
+        print("\n***** Model Information *****")
+        print(f"Number of nodes: {model_info['num_node']}")
+        print(f"Number of elements: {model_info['num_ele']}")
+        bounds = np.array(model_info["bound"])
+        bounds = np.round(bounds, 6)
+        print(f"The boundary size: X --> {bounds[:2]}; Y --> {bounds[2:4]}; Z --> {bounds[4:]}")
+        ele_types = [EleTypeTags[ele] for ele in model_info["EleClassTags"]]
+        ele_types = set(ele_types)
+        print(f"Element types: {ele_types}")
+        print("***** END *****\n")
+
     def get_eigen_data(
         self,
         mode_tag: int = 1,
         solver: str = "-genBandArpack",
         save_file: str = "EigenData.hdf5",
     ):
         """Get eigenvalue Analysis Data.
@@ -222,22 +242,23 @@
         Returns
         -------
         None
         """
         # ----------------------------------
         if save_file:
             check_file(save_file, [".hdf5", ".h5", ".he5"])
-        self.get_model_data(save_file=False)
+        self.get_model_data(save_file=False, print_model_info=False)
         self.reset_eigen_state()
         # ----------------------------------
         ops.wipeAnalysis()
         if mode_tag == 1:
             eigen_values = ops.eigen(solver, 2)[:1]
         else:
             eigen_values = ops.eigen(solver, mode_tag)
+        modalProps = ops.modalProperties('-return')
         omega = np.sqrt(eigen_values)
         f = omega / (2 * np.pi)
         self.eigen["f"] = f
         eigenvectors = []
         for mode_tag in range(1, mode_tag + 1):
             eigen_vector = np.zeros((self.model_info["num_node"], 3))
             for i, Tag in enumerate(self.model_info["NodeTags"]):
@@ -257,14 +278,15 @@
                     eigen = eigen[:3]
                 eigen_vector[i] = np.array(eigen)
             eigenvectors.append(eigen_vector)
         self.eigen["eigenvector"] = eigenvectors
 
         self.eigen.update(self.model_info)
         self.eigen.update(self.cells)
+        self.eigen.update(modalProps)
         # ----------------------------------------------------------------
         if save_file:
             output_filename = self.out_dir + "/" + save_file
             with h5py.File(output_filename, "w") as f:
                 grp = f.create_group("EigenInfo")
                 for name, value in self.eigen.items():
                     grp.create_dataset(name, data=value)
@@ -402,18 +424,18 @@
         Returns
         -------
         None
         """
         if save_file:
             check_file(save_file, [".hdf5", ".h5", ".he5"])
         if model_update:
-            self.get_model_data(save_file=False)
+            self.get_model_data(save_file=False, print_model_info=False)
         else:
             if not self.get_model_data_finished:
-                self.get_model_data(save_file=False)
+                self.get_model_data(save_file=False, print_model_info=False)
 
         node_tags = self.model_info["NodeTags"]
         (node_disp, node_vel, node_accel, node_deform_coord) = get_node_resp(node_tags)
 
         self.node_resp_steps["disp"].append(node_disp)
         self.node_resp_steps["vel"].append(node_vel)
         self.node_resp_steps["accel"].append(node_accel)
```

### Comparing `opstool-0.8.2/src/opstool/vis/ops_vis_2d.py` & `opstool-0.8.3/src/opstool/vis/ops_vis_2d.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool/vis/ops_vis_plotly.py` & `opstool-0.8.3/src/opstool/vis/ops_vis_plotly.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         color_map: str = "jet",
         on_notebook: bool = False,
         results_dir: str = "opstool_output",
     ):
         # ------------------------------
         self.point_size = point_size
         self.line_width = line_width
-        self.title = "OpenSeesVispy"
+        self.title = "opstool"
         colors = dict(
             point="#580f41",
             line="#0504aa",
             face="#00c16e",
             solid="#0cb9c1",
             truss="#7552cc",
             link="#01ff07",
@@ -85,14 +85,45 @@
         self.color_constraint = colors["constraint"]
         self.theme = theme
         self.color_map = color_map
         self.notebook = on_notebook
         self.out_dir = results_dir
         self.bound_fact = 30
 
+    def set_color(self, point: str = "#580f41", line: str = "#0504aa",
+                  face: str = "#00c16e", solid: str = "#0cb9c1",
+                  truss: str = "#7552cc", link: str = "#01ff07",
+                  constraint: str = "#00ffff"):
+        """Set the color for various element types.
+
+        Paramaters
+        -----------
+        point: str, default="#580f41"
+            Nodal color.
+        line: str, default="#0504aa"
+            Line element color, including beams.
+        face: str, default="#00c16e"
+            The color of planar elements, including 2D solid elements, plate and shell elements.
+        solid: str, default="#0cb9c1"
+            The color of solid elements.
+        truss: str, default="#7552cc"
+            Truss color.
+        link: str, default="#01ff07"
+            The color of link and bearing elements.
+        constraint: str, default="#00ffff"
+            The color of multi-point constraint.
+        """
+        self.color_point = point
+        self.color_line = line
+        self.color_face = face
+        self.color_solid = solid
+        self.color_truss = truss
+        self.color_link = link
+        self.color_constraint = constraint
+
     def write_html(self, fig, filepath, **kwargs):
         """Write a figure to an HTML file representation.
 
         .. note::
             Added since v0.8.0.
             The purpose is to replace the argument ``save_html`` in various visualization method.
 
@@ -187,29 +218,29 @@
             If you want to further control the size, you can use `load_alpha`.
             Currently only supported beam element load types include
             <beamUniform2D, beamUniform3D, beamPoint2D, beamPoint3D>.
 
             .. note::
                 Please make sure that all dofs (or directions) have values
                 when adding the ``load`` or ``eleLoad`` command,
-                even if the value is 0.
+                even if the value is 0.0.
 
         load_alpha: float, default = 1.0
             On existing displays, the scaling factor for the load arrow sizes.
         show_constrain_dof: bool, default=False
             Whether to display labels for constrained degrees of freedom.
         show_beam_sec: bool default = False
             Whether to render the 3d section of beam or truss elements.
             If True, the Arg `beam_sec` in :py:meth:`opstool.vis.GetFEMdata.get_model_data`
             must be assigned in advance.
         beam_sec_paras: dict defalut = None,
             A dict to control beam section render, optional key: color, opacity.
             Note that the backend plotly does not currently support texture.
         label_size: float, default=8
-            The foontsize of node and ele label.
+            The fontsize of node and ele label.
         show_outline: bool, default=True
             Whether to show the axis frame.
         opacity: float, default=1.0
             Plane and solid element transparency.
         save_html: str, default=None
             The html file name to output. If False, the html file will not be generated.
 
@@ -274,14 +305,16 @@
             If True, subplots in a figure. If False, plot in a slide style.
         alpha: float, default=1.0
             Model scaling factor, scale further on existing display.
         show_outline: bool, default=True
             Whether to display the axes.
         show_origin: bool, default=False
             Whether to show undeformed shape.
+        label_size: float, default=15
+            The fontsize of text labels.
         opacity: float, default=1.0
             Plane and solid element transparency.
         show_face_line: bool, default=True
             If True, the edges of plate and solid elements will be displayed.
         save_html: str, default=None
             The html file name to output. If False, the html file will not be generated.
```

### Comparing `opstool-0.8.2/src/opstool/vis/ops_vis_pyvista.py` & `opstool-0.8.3/src/opstool/vis/ops_vis_pyvista.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,22 +43,22 @@
 
     Returns
     --------
     None
     """
 
     def __init__(
-        self,
-        point_size: float = 1,
-        line_width: float = 3,
-        colors_dict: dict = None,
-        theme: str = "document",
-        color_map: str = "jet",
-        on_notebook: bool = False,
-        results_dir: str = "opstool_output",
+            self,
+            point_size: float = 1,
+            line_width: float = 3,
+            colors_dict: dict = None,
+            theme: str = "document",
+            color_map: str = "jet",
+            on_notebook: bool = False,
+            results_dir: str = "opstool_output",
     ):
         # ------------------------------
         self.point_size = point_size
         self.line_width = line_width
         self.title = "opstool"
         # Initialize the color dict
         colors = dict(
@@ -84,34 +84,83 @@
         self.theme = theme
         pv.set_plot_theme(theme)
         self.color_map = color_map
         self.notebook = on_notebook
         # -------------------------------------------------
         self.out_dir = results_dir
         # -------------------------------------------------
-        self.bound_fact = 20
+        self.bound_fact = 30
+        self.anti_aliasing = "msaa"
+
+    def set_color(
+        self, point: str = "#580f41", line: str = "#0504aa",
+        face: str = "#00c16e", solid: str = "#0cb9c1",
+        truss: str = "#7552cc", link: str = "#01ff07",
+        constraint: str = "#00ffff"
+    ):
+        """Set the color for various element types.
+
+        Paramaters
+        -----------
+        point: str, default="#580f41"
+            Nodal color.
+        line: str, default="#0504aa"
+            Line element color, including beams.
+        face: str, default="#00c16e"
+            The color of planar elements, including 2D solid elements, plate and shell elements.
+        solid: str, default="#0cb9c1"
+            The color of solid elements.
+        truss: str, default="#7552cc"
+            Truss color.
+        link: str, default="#01ff07"
+            The color of link and bearing elements.
+        constraint: str, default="#00ffff"
+            The color of multi-point constraint.
+        """
+        self.color_point = point
+        self.color_line = line
+        self.color_face = face
+        self.color_solid = solid
+        self.color_truss = truss
+        self.color_link = link
+        self.color_constraint = constraint
+
+    def set_anti_aliasing(self, aa_type: str = "msaa"):
+        """
+        Make edges (lines) appear softer and less pixelated.
+
+        Parameters
+        -----------
+        aa_type: str, default = "msaa"
+            Anti-aliasing type. See the notes below. One of the following:
+
+            * ``"ssaa"`` - Super-Sample Anti-Aliasing
+            * ``"msaa"`` - Multi-Sample Anti-Aliasing
+            * ``"fxaa"`` - Fast Approximate Anti-Aliasing
+        """
+        self.anti_aliasing = aa_type
 
     def model_vis(
-        self,
-        input_file: str = "ModelData.hdf5",
-        show_node_label: bool = False,
-        show_ele_label: bool = False,
-        label_size: float = 10,
-        show_local_crd: bool = False,
-        local_crd_alpha: float = 1.0,
-        show_fix_node: bool = True,
-        fix_node_alpha: float = 1.0,
-        show_load: bool = False,
-        load_alpha: float = 1.0,
-        show_constrain_dof: bool = False,
-        show_beam_sec: bool = False,
-        beam_sec_paras: dict = None,
-        show_outline: bool = True,
-        opacity: float = 1.0,
-        save_fig: str = "ModelVis.svg",
+            self,
+            input_file: str = "ModelData.hdf5",
+            show_node_label: bool = False,
+            show_ele_label: bool = False,
+            label_size: float = 10,
+            show_local_crd: bool = False,
+            local_crd_alpha: float = 1.0,
+            show_fix_node: bool = True,
+            fix_node_alpha: float = 1.0,
+            show_load: bool = False,
+            load_alpha: float = 1.0,
+            show_constrain_dof: bool = False,
+            show_beam_sec: bool = False,
+            beam_sec_paras: dict = None,
+            show_outline: bool = True,
+            opacity: float = 1.0,
+            save_fig: str = "ModelVis.svg",
     ):
         """
         Visualize the model in the current domain.
 
         Parameters
         ----------
         input_file: str, default = "ModelData.hdf5",
@@ -196,26 +245,26 @@
             label_size=label_size,
             show_outline=show_outline,
             opacity=opacity,
             save_fig=save_fig,
         )
 
     def eigen_vis(
-        self,
-        mode_tags: list,
-        input_file: str = "EigenData.hdf5",
-        subplots: bool = False,
-        link_views: bool = True,
-        alpha: float = 1.0,
-        show_outline: bool = False,
-        show_origin: bool = False,
-        label_size: float = 15,
-        opacity: float = 1.0,
-        show_face_line: bool = True,
-        save_fig: str = "EigenVis.svg",
+            self,
+            mode_tags: list,
+            input_file: str = "EigenData.hdf5",
+            subplots: bool = False,
+            link_views: bool = True,
+            alpha: float = 1.0,
+            show_outline: bool = False,
+            show_origin: bool = False,
+            label_size: float = 15,
+            opacity: float = 1.0,
+            show_face_line: bool = True,
+            save_fig: str = "EigenVis.svg",
     ):
         """Eigenvalue Analysis Visualization.
 
         Parameters
         ----------
         mode_tags: list[int], or tuple[int]
             Mode tags to be shown, if list or tuple [mode1, mode2], display the multiple modes from mode1 to mode2.
@@ -233,14 +282,16 @@
             If True, link the views’ cameras, only usefuly when subplots is True.
         alpha: float, default=1.0
             Model scaling factor, scale further on existing display.
         show_outline: bool, default=True
             Whether to display the axes.
         show_origin: bool, default=False
             Whether to show undeformed shape.
+        label_size: float, default=15
+            The fontsize of text labels.
         opacity: float, default=1.0
             Plane and solid element transparency.
         show_face_line: bool, default=True
             If True, the edges of plate and solid elements will be displayed.
         save_fig: str, default='EigenVis.svg'
             The file name to output. If False or None, the file will not be generated.
             The supported formats are:
@@ -268,25 +319,25 @@
             label_size=label_size,
             opacity=opacity,
             show_face_line=show_face_line,
             save_fig=save_fig,
         )
 
     def eigen_anim(
-        self,
-        mode_tag: int = 1,
-        input_file: str = "EigenData.hdf5",
-        n_cycle: int = 5,
-        alpha: float = 1.0,
-        show_outline: bool = False,
-        label_size: float = 15,
-        opacity: float = 1,
-        framerate: int = 3,
-        show_face_line: bool = True,
-        save_fig: str = "EigenAnimation.gif",
+            self,
+            mode_tag: int = 1,
+            input_file: str = "EigenData.hdf5",
+            n_cycle: int = 5,
+            alpha: float = 1.0,
+            show_outline: bool = False,
+            label_size: float = 15,
+            opacity: float = 1,
+            framerate: int = 3,
+            show_face_line: bool = True,
+            save_fig: str = "EigenAnimation.gif",
     ):
         """Animation of Modal Analysis.
 
         Parameters
         ----------
         mode_tag: int
             The mode tag.
@@ -300,14 +351,16 @@
 
         n_cycle: int, default = 5,
             The number of cycles in the positive and negative directions of the modal deformation.
         alpha: float, default=1.0
             Scaling factor, scale further on existing display.
         show_outline: bool, default=False
             Whether to display the axes.
+        label_size: float, default=15
+            The fontsize of text labels.
         opacity: float, default=1.0
             Plane and solid element transparency.
         framerate: int
             The number of frames per second.
         show_face_line: bool, default=True
             If True, the edges of plate and solid elements will be displayed.
         save_fig: str, default='EigenAnimation.gif'
@@ -330,21 +383,21 @@
             opacity=opacity,
             framerate=framerate,
             show_face_line=show_face_line,
             save_fig=save_fig,
         )
 
     def react_vis(
-        self,
-        input_file: str = "NodeReactionStepData-1.hdf5",
-        slider: bool = False,
-        direction: str = "Fz",
-        show_values: bool = True,
-        show_outline: bool = False,
-        save_fig: str = "ReactionVis.svg",
+            self,
+            input_file: str = "NodeReactionStepData-1.hdf5",
+            slider: bool = False,
+            direction: str = "Fz",
+            show_values: bool = True,
+            show_outline: bool = False,
+            save_fig: str = "ReactionVis.svg",
     ):
         """Plot the node reactions.
 
         Parameters
         ----------
         input_file : str, optional, default="NodeReactionStepData-1.hdf5"
             The filename that eigen data saved by
@@ -376,25 +429,25 @@
             direction=direction,
             show_values=show_values,
             show_outline=show_outline,
             save_fig=save_fig,
         )
 
     def deform_vis(
-        self,
-        input_file: str = "NodeRespStepData-1.hdf5",
-        slider: bool = False,
-        response: str = "disp",
-        alpha: float = 1.0,
-        show_outline: bool = False,
-        show_origin: bool = False,
-        show_face_line: bool = True,
-        opacity: float = 1,
-        save_fig: str = "DefoVis.svg",
-        model_update: bool = False,
+            self,
+            input_file: str = "NodeRespStepData-1.hdf5",
+            slider: bool = False,
+            response: str = "disp",
+            alpha: float = 1.0,
+            show_outline: bool = False,
+            show_origin: bool = False,
+            show_face_line: bool = True,
+            opacity: float = 1,
+            save_fig: str = "DefoVis.svg",
+            model_update: bool = False,
     ):
         """Visualize the deformation of the model at a certain analysis step.
 
         Parameters
         ----------
         input_file: str, default = "NodeRespStepData-1.hdf5",
             The filename that node responses data saved by
@@ -451,24 +504,24 @@
             show_face_line=show_face_line,
             opacity=opacity,
             save_fig=save_fig,
             model_update=model_update,
         )
 
     def deform_anim(
-        self,
-        input_file: str = "NodeRespStepData-1.hdf5",
-        response: str = "disp",
-        alpha: float = 1.0,
-        show_outline: bool = False,
-        opacity: float = 1,
-        framerate: int = 24,
-        show_face_line: bool = True,
-        save_fig: str = "DefoAnimation.gif",
-        model_update: bool = False,
+            self,
+            input_file: str = "NodeRespStepData-1.hdf5",
+            response: str = "disp",
+            alpha: float = 1.0,
+            show_outline: bool = False,
+            opacity: float = 1,
+            framerate: int = 24,
+            show_face_line: bool = True,
+            save_fig: str = "DefoAnimation.gif",
+            model_update: bool = False,
     ):
         """Deformation animation of the model.
 
         Parameters
         ----------
         input_file: str, default = "NodeRespStepData-1.hdf5",
             The filename that node responses data saved by
@@ -514,23 +567,23 @@
             framerate=framerate,
             show_face_line=show_face_line,
             save_fig=save_fig,
             model_update=model_update,
         )
 
     def deform_peak_vis(
-        self,
-        input_file: str = "NodeRespStepData-1.hdf5",
-        response: str = "disp",
-        alpha: float = 1.0,
-        show_outline: bool = False,
-        show_origin: bool = False,
-        show_face_line: bool = True,
-        opacity: float = 1,
-        save_fig: str = "DefoVis.svg"
+            self,
+            input_file: str = "NodeRespStepData-1.hdf5",
+            response: str = "disp",
+            alpha: float = 1.0,
+            show_outline: bool = False,
+            show_origin: bool = False,
+            show_face_line: bool = True,
+            opacity: float = 1,
+            save_fig: str = "DefoVis.svg"
     ):
         """Visualize the node peak responses of the model at all analysis steps.
         That is to say, the response of each node in each direction is the absolute maximum
         value in all its time steps.
 
         .. note::
             This method does not support the arg `model_update`,
@@ -581,23 +634,23 @@
             show_origin=show_origin,
             show_face_line=show_face_line,
             opacity=opacity,
             save_fig=save_fig
         )
 
     def frame_resp_vis(
-        self,
-        input_file: str = "BeamRespStepData-1.hdf5",
-        ele_tags: list = None,
-        slider: bool = False,
-        response: str = "Mz",
-        show_values=True,
-        alpha: float = 1.0,
-        opacity: float = 1,
-        save_fig: str = "FrameRespVis.svg",
+            self,
+            input_file: str = "BeamRespStepData-1.hdf5",
+            ele_tags: list = None,
+            slider: bool = False,
+            response: str = "Mz",
+            show_values=True,
+            alpha: float = 1.0,
+            opacity: float = 1,
+            save_fig: str = "FrameRespVis.svg",
     ):
         """
         Display the force response of frame elements.
 
         Parameters
         ----------
         input_file: str, default = "BeamRespStepData-1.hdf5",
```

### Comparing `opstool-0.8.2/src/opstool/vis/quick_plot.py` & `opstool-0.8.3/src/opstool/vis/quick_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         The foontsize of node and ele label.
     show_outline: bool, default=True
         Whether to show the axis frame.
     opacity: float, default=1.0
         Plane and solid element transparency.
     """
     ModelData = GetFEMdata(results_dir="opstool_output")
-    ModelData.get_model_data(save_file="ModelData.hdf5")
+    ModelData.get_model_data(save_file="ModelData.hdf5", print_model_info=False)
     if backend.lower() == "pyvista":
         opsvis = OpsVisPyvista(
             point_size=point_size,
             line_width=line_width,
             colors_dict=colors_dict,
             theme="document",
             color_map="jet",
@@ -161,14 +161,15 @@
     line_width: float = 3,
     on_notebook: bool = False,
     subplots: bool = False,
     link_views: bool = True,
     alpha: float = 1.0,
     show_outline: bool = False,
     show_origin: bool = False,
+    label_size: float = 15.0,
     opacity: float = 1.0,
     show_face_line: bool = True,
     show_cmap: bool = True,
 ):
     """Fast eigen visualization.
 
     Parameters
@@ -193,14 +194,16 @@
         If True, link the views’ cameras, only usefuly when subplots is True, and backend='pyvista'.
     alpha: float, default=1.0
         Model scaling factor on existing display.
     show_outline: bool, default=True
         Whether to display the axes.
     show_origin: bool, default=False
         Whether to show undeformed shape.
+    label_size: float, default=15
+            The fontsize of text labels.
     opacity: float, default=1.0
         Plane and solid element transparency.
     show_face_line: bool, default=True
         If True, the edges of plate and solid elements will be displayed.
     show_cmap: bool, default=True
         If True, display the cloud plot, else only the deformation with single color.
         Only supported for `backend="matplotlib"`.
@@ -221,14 +224,15 @@
         opsvis.eigen_vis(
             input_file="EigenData.hdf5",
             mode_tags=mode_tags,
             subplots=subplots,
             alpha=alpha,
             show_outline=show_outline,
             show_origin=show_origin,
+            label_size=label_size,
             opacity=opacity,
             show_face_line=show_face_line,
             link_views=link_views,
             save_fig=None,
         )
     elif backend.lower() == "plotly":
         opsvis = OpsVisPlotly(
@@ -241,14 +245,15 @@
         )
         opsvis.eigen_vis(
             input_file="EigenData.hdf5",
             mode_tags=mode_tags,
             subplots=subplots,
             alpha=alpha,
             show_outline=show_outline,
+            label_size=label_size,
             show_origin=show_origin,
             opacity=opacity,
             show_face_line=show_face_line,
             save_html="EigenVis.html",
         )
     elif backend.lower().startswith("m"):
         opsvis = OpsVis2D(
@@ -266,16 +271,7 @@
             show_origin=show_origin,
             opacity=opacity,
             show_face_line=show_face_line,
             show_cmap=show_cmap,
         )
     else:
         raise ValueError("Arg backend must be one of ['pyvista', 'plotly', 'mpl']!")
-
-
-# def plot_node_resp(disp_file, dof_num, ):
-#     ModelData = GetFEMdata(results_dir="opstool_output")
-#     ModelData.get_model_data(save_file="ModelData.hdf5")
-#     disp_data = np.loadtxt(disp_file)
-#     step_num = disp_data.shape[0]
-#     for i in range(step_num):
-#         np.reshape(disp_data[i], (-1, dof_num))
```

### Comparing `opstool-0.8.2/src/opstool/vis/save_tikz.py` & `opstool-0.8.3/src/opstool/vis/save_tikz.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/src/opstool.egg-info/PKG-INFO` & `opstool-0.8.3/src/opstool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opstool
-Version: 0.8.2
+Version: 0.8.3
 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992
 Author: Yexiang Yan
 Author-email: yexiang_yan@outlook.com
 License: GPL Licence
 Keywords: OpenSees Visualization Seismic Simulation
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opstool Version: 0.8.2 Summary: openseespy toolbox
+Metadata-Version: 2.1 Name: opstool Version: 0.8.3 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992 Author: Yexiang Yan Author-email:
 yexiang_yan@outlook.com License: GPL Licence Keywords: OpenSees Visualization
 Seismic Simulation Platform: any Classifier: Programming Language :: Python ::
 3 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENCE.txt
                                     opstool
            modelling, visualization, post-processing for OpenSeesPy.
```

### Comparing `opstool-0.8.2/src/opstool.egg-info/SOURCES.txt` & `opstool-0.8.3/src/opstool.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENCE.txt
 README.md
 setup.py
+src/opstool/EleClassTags.py
 src/opstool/__about__.py
 src/opstool/__init__.py
 src/opstool/utils.py
 src/opstool.egg-info/PKG-INFO
 src/opstool.egg-info/SOURCES.txt
 src/opstool.egg-info/dependency_links.txt
 src/opstool.egg-info/requires.txt
```

### Comparing `opstool-0.8.2/tests/test_dambreak.py` & `opstool-0.8.3/tests/test_dambreak.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/tests/test_fiber_sec_vis.py` & `opstool-0.8.3/tests/test_fiber_sec_vis.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/tests/test_model_vis.py` & `opstool-0.8.3/tests/test_model_vis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# %%
+
 import openseespy.opensees as ops
 import opstool as opst
 
 #
-opst.load_ops_examples("ArchBridge")
-# opst.load_ops_examples("CableStayedBridge")
+# opst.load_ops_examples("ArchBridge")
+opst.load_ops_examples("CableStayedBridge")
 # opst.load_ops_examples("Dam")
 # opst.load_ops_examples("Frame3D")
 # opst.load_ops_examples("Igloo")
 # opst.load_ops_examples("Pier")
 # opst.load_ops_examples("SuspensionBridge")
 # opst.plot_model(backend="pyvista")    # or backend="plotly"
 # opst.plot_eigen(mode_tags=[1, 12], backend="pyvista", subplots=True)   # or backend="plotly"
 # opst.gen_grav_load(ts_tag=1, pattern_tag=1, factor=-9.81, direction="Z")
 ModelData = opst.GetFEMdata()
 ModelData.get_model_data()
 ModelData.get_eigen_data(mode_tag=15)
 opsv = opst.OpsVisPlotly(
-    point_size=4,
-    line_width=4,
+    point_size=0.1,
+    line_width=2,
     colors_dict=None,
     color_map="jet",
     on_notebook=False,
     results_dir="opstool_output",
 )
 fig = opsv.model_vis(
     show_node_label=False,
@@ -35,24 +35,24 @@
     show_outline=True,
     opacity=1.0,
 )
 fig.show()
 # fig.write_html("ModelVis.html", auto_open=True)
 # %%
 opst.save_tikz("opstool_output/ModelData.hdf5")
-opsv.eigen_vis(
+fig = opsv.eigen_vis(
     mode_tags=[1, 12],
     subplots=True,
     alpha=1.0,
     show_outline=False,
     show_origin=False,
     opacity=1.0,
     show_face_line=False,
 )
-
+fig.show()
 opsv.eigen_anim(
     mode_tag=4,
     alpha=1.0,
     show_outline=False,
     opacity=1,
     framerate=3,
     show_face_line=True,
```

### Comparing `opstool-0.8.2/tests/test_sec_analysis.py` & `opstool-0.8.3/tests/test_sec_analysis.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/tests/test_sec_mesh.py` & `opstool-0.8.3/tests/test_sec_mesh.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.2/tests/test_temp.py` & `opstool-0.8.3/tests/test_temp.py`

 * *Files identical despite different names*

