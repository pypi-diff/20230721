# Comparing `tmp/qtmetabolabpy-0.9.2.tar.gz` & `tmp/qtmetabolabpy-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtmetabolabpy-0.9.2.tar", last modified: Wed Jul 19 23:19:30 2023, max compression
+gzip compressed data, was "qtmetabolabpy-0.9.4.tar", last modified: Fri Jul 21 11:28:53 2023, max compression
```

## Comparing `qtmetabolabpy-0.9.2.tar` & `qtmetabolabpy-0.9.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-19 23:19:30.482126 qtmetabolabpy-0.9.2/
--rw-r--r--   0 ludwigc  (1699341573) 1311385079    35149 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.2/LICENSE
--rw-r--r--   0 ludwigc  (1699341573) 1311385079      364 2023-07-11 15:01:39.000000 qtmetabolabpy-0.9.2/MANIFEST.in
--rw-r--r--   0 ludwigc  (1699341573) 1311385079     3745 2023-07-19 23:19:30.481941 qtmetabolabpy-0.9.2/PKG-INFO
--rw-r--r--   0 ludwigc  (1699341573) 1311385079     2977 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.2/README.rst
-drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-19 23:19:30.479137 qtmetabolabpy-0.9.2/qtmetabolabpy/
--rw-r--r--   0 ludwigc  (1699341573) 1311385079      210 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.2/qtmetabolabpy/__init__.py
--rwxr-xr-x   0 ludwigc  (1699341573) 1311385079     5014 2023-07-16 19:58:28.000000 qtmetabolabpy-0.9.2/qtmetabolabpy/__main__.py
-drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-19 23:19:30.480232 qtmetabolabpy-0.9.2/qtmetabolabpy/bash/
--rwxr-xr-x   0 ludwigc  (1699341573) 1311385079      556 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.2/qtmetabolabpy/bash/fix_pyside2
-drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-19 23:19:30.480481 qtmetabolabpy-0.9.2/qtmetabolabpy/mlStarter/
-drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-19 23:19:30.480802 qtmetabolabpy-0.9.2/qtmetabolabpy/mlStarter/Contents/
--rw-r--r--   0 ludwigc  (1699341573) 1311385079      884 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.2/qtmetabolabpy/mlStarter/Contents/Info.plist
--rw-r--r--   0 ludwigc  (1699341573) 1311385079        9 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.2/qtmetabolabpy/mlStarter/Contents/PkgInfo
-drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-19 23:19:30.481018 qtmetabolabpy-0.9.2/qtmetabolabpy/mlStarter/Contents/Resources/
--rw-r--r--   0 ludwigc  (1699341573) 1311385079   173336 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.2/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns
--rw-r--r--   0 ludwigc  (1699341573) 1311385079        0 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.2/qtmetabolabpy/mlStarter/Icon
--rwxr-xr-x   0 ludwigc  (1699341573) 1311385079   376370 2023-07-19 23:16:47.000000 qtmetabolabpy-0.9.2/qtmetabolabpy/qtMetaboLabPy.py
-drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-19 23:19:30.481405 qtmetabolabpy-0.9.2/qtmetabolabpy/ui/
--rw-r--r--   0 ludwigc  (1699341573) 1311385079   243075 2023-07-19 20:57:45.000000 qtmetabolabpy-0.9.2/qtmetabolabpy/ui/metabolabpy_mainwindow.ui
-drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-19 23:19:30.480114 qtmetabolabpy-0.9.2/qtmetabolabpy.egg-info/
--rw-r--r--   0 ludwigc  (1699341573) 1311385079     3745 2023-07-19 23:19:30.000000 qtmetabolabpy-0.9.2/qtmetabolabpy.egg-info/PKG-INFO
--rw-r--r--   0 ludwigc  (1699341573) 1311385079      607 2023-07-19 23:19:30.000000 qtmetabolabpy-0.9.2/qtmetabolabpy.egg-info/SOURCES.txt
--rw-r--r--   0 ludwigc  (1699341573) 1311385079        1 2023-07-19 23:19:30.000000 qtmetabolabpy-0.9.2/qtmetabolabpy.egg-info/dependency_links.txt
--rw-r--r--   0 ludwigc  (1699341573) 1311385079       62 2023-07-19 23:19:30.000000 qtmetabolabpy-0.9.2/qtmetabolabpy.egg-info/entry_points.txt
--rw-r--r--   0 ludwigc  (1699341573) 1311385079      119 2023-07-19 23:19:30.000000 qtmetabolabpy-0.9.2/qtmetabolabpy.egg-info/requires.txt
--rw-r--r--   0 ludwigc  (1699341573) 1311385079       14 2023-07-19 23:19:30.000000 qtmetabolabpy-0.9.2/qtmetabolabpy.egg-info/top_level.txt
--rw-r--r--   0 ludwigc  (1699341573) 1311385079      321 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.2/requirements.txt
--rw-r--r--   0 ludwigc  (1699341573) 1311385079       38 2023-07-19 23:19:30.482166 qtmetabolabpy-0.9.2/setup.cfg
--rw-r--r--   0 ludwigc  (1699341573) 1311385079     3912 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.2/setup.py
+drwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        0 2023-07-21 11:28:53.014507 qtmetabolabpy-0.9.4/
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)    35149 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.4/LICENSE
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)      364 2023-07-11 15:01:39.000000 qtmetabolabpy-0.9.4/MANIFEST.in
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)     3745 2023-07-21 11:28:53.014277 qtmetabolabpy-0.9.4/PKG-INFO
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)     2977 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.4/README.rst
+drwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        0 2023-07-21 11:28:53.011184 qtmetabolabpy-0.9.4/qtmetabolabpy/
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)      195 2023-07-21 11:28:48.000000 qtmetabolabpy-0.9.4/qtmetabolabpy/__init__.py
+-rwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)     5014 2023-07-16 19:58:28.000000 qtmetabolabpy-0.9.4/qtmetabolabpy/__main__.py
+drwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        0 2023-07-21 11:28:53.012653 qtmetabolabpy-0.9.4/qtmetabolabpy/bash/
+-rwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)      556 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.4/qtmetabolabpy/bash/fix_pyside2
+drwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        0 2023-07-21 11:28:53.012975 qtmetabolabpy-0.9.4/qtmetabolabpy/mlStarter/
+drwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        0 2023-07-21 11:28:53.013289 qtmetabolabpy-0.9.4/qtmetabolabpy/mlStarter/Contents/
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)      884 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.4/qtmetabolabpy/mlStarter/Contents/Info.plist
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        9 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.4/qtmetabolabpy/mlStarter/Contents/PkgInfo
+drwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        0 2023-07-21 11:28:53.013455 qtmetabolabpy-0.9.4/qtmetabolabpy/mlStarter/Contents/Resources/
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)   173336 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.4/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        0 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.4/qtmetabolabpy/mlStarter/Icon
+-rwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)   376412 2023-07-21 11:25:55.000000 qtmetabolabpy-0.9.4/qtmetabolabpy/qtMetaboLabPy.py
+drwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        0 2023-07-21 11:28:53.013712 qtmetabolabpy-0.9.4/qtmetabolabpy/ui/
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)   243075 2023-07-19 20:57:45.000000 qtmetabolabpy-0.9.4/qtmetabolabpy/ui/metabolabpy_mainwindow.ui
+drwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        0 2023-07-21 11:28:53.012506 qtmetabolabpy-0.9.4/qtmetabolabpy.egg-info/
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)     3745 2023-07-21 11:28:52.000000 qtmetabolabpy-0.9.4/qtmetabolabpy.egg-info/PKG-INFO
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)      607 2023-07-21 11:28:52.000000 qtmetabolabpy-0.9.4/qtmetabolabpy.egg-info/SOURCES.txt
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        1 2023-07-21 11:28:52.000000 qtmetabolabpy-0.9.4/qtmetabolabpy.egg-info/dependency_links.txt
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)       62 2023-07-21 11:28:52.000000 qtmetabolabpy-0.9.4/qtmetabolabpy.egg-info/entry_points.txt
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)       97 2023-07-21 11:28:52.000000 qtmetabolabpy-0.9.4/qtmetabolabpy.egg-info/requires.txt
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)       14 2023-07-21 11:28:52.000000 qtmetabolabpy-0.9.4/qtmetabolabpy.egg-info/top_level.txt
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)      323 2023-07-21 11:26:22.000000 qtmetabolabpy-0.9.4/requirements.txt
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)       38 2023-07-21 11:28:53.014546 qtmetabolabpy-0.9.4/setup.cfg
+-rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)     3912 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.4/setup.py
```

### Comparing `qtmetabolabpy-0.9.2/LICENSE` & `qtmetabolabpy-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.2/PKG-INFO` & `qtmetabolabpy-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmetabolabpy
-Version: 0.9.2
+Version: 0.9.4
 Summary: Python package for data processing of NMR 1D and 2D metabolomics and metabolism tracing data
 Home-page: https://github.com/ludwigc/qtmetabolabpy
 Author: Christian Ludwig
 Author-email: C.Ludwig@bham.ac.uk 
 License: GPLv3
 Keywords: Metabolomics,Tracing,NMR,Data Processing,13C
 Platform: MacOS, Windows, UNIX
```

### Comparing `qtmetabolabpy-0.9.2/README.rst` & `qtmetabolabpy-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.2/qtmetabolabpy/__main__.py` & `qtmetabolabpy-0.9.4/qtmetabolabpy/__main__.py`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.2/qtmetabolabpy/bash/fix_pyside2` & `qtmetabolabpy-0.9.4/qtmetabolabpy/bash/fix_pyside2`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.2/qtmetabolabpy/mlStarter/Contents/Info.plist` & `qtmetabolabpy-0.9.4/qtmetabolabpy/mlStarter/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.2/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns` & `qtmetabolabpy-0.9.4/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.2/qtmetabolabpy/qtMetaboLabPy.py` & `qtmetabolabpy-0.9.4/qtmetabolabpy/qtMetaboLabPy.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 ## matplotlib.rc('ytick', labelsize=8)
 import platform  # pragma: no cover
 import os  # pragma: no cover
 
 
 
 try:
-    v = 0.9.2
     from PySide2.QtUiTools import QUiLoader  # pragma: no cover
     from PySide2.QtCore import QFile  # pragma: no cover
     from PySide2.QtCore import QCoreApplication  # pragma: no cover
     from PySide2.QtWidgets import *  # pragma: no cover
     from PySide2 import QtWidgets  # pragma: no cover
     from PySide2.QtGui import *  # pragma: no cover
     from PySide2 import QtGui  # pragma: no cover
@@ -125,18 +124,18 @@
 import shutil  # pragma: no cover
 import scipy.io  # pragma: no cover
 #import inspect
 from io import StringIO
 import contextlib
 import zipfile
 from collections import defaultdict
-from notebook import notebookapp
+#from notebook import notebookapp
 import multiprocess
 import subprocess
-import jupyterthemes
+#import jupyterthemes
 import itertools
 import xlsxwriter
 from string import ascii_uppercase
 import metabolabpy.nmr.nmrHsqc as nmrHsqc
 
 try:
     # ------------------ MplWidget ------------------
@@ -359,16 +358,16 @@
         self.w.invertMatrix_2.stateChanged.connect(self.set_invert)
         self.w.exportFileName.textChanged.connect(self.set_export_file_name)
         self.w.exportDelimiterTab.toggled.connect(self.set_export_delimiter_tab)
         self.w.exportCharacter.textChanged.connect(self.set_export_character)
         self.w.titleFile.textChanged.connect(self.change_title_file)
         self.w.samplesInComboBox.currentIndexChanged.connect(self.set_samples_in_combo_box)
         self.w.openWeb.activated.connect(self.open_metabolite_web)
-        self.w.startNotebookButton.clicked.connect(self.start_notebook)
-        self.w.stopNotebookButton.clicked.connect(self.stop_notebook)
+        #self.w.startNotebookButton.clicked.connect(self.start_notebook)
+        #self.w.stopNotebookButton.clicked.connect(self.stop_notebook)
         self.w.runPreProcessingButton.clicked.connect(self.data_pre_processing)
         self.w.resetPreProcessingButton.clicked.connect(self.reset_data_pre_processing)
         self.w.avoidNegValues.stateChanged.connect(self.set_avoid_neg_values)
         self.w.excludeRegion.stateChanged.connect(self.set_exclude_region)
         self.w.segmentalAlignment.stateChanged.connect(self.set_segmental_alignment)
         self.w.compressBuckets.stateChanged.connect(self.set_compress_buckets)
         self.w.noiseFiltering.stateChanged.connect(self.set_noise_filtering)
@@ -599,16 +598,16 @@
         self.w.iSpc_p4.textChanged.connect(self.get_i_spc_p4)
         self.w.iSpc_p5.textChanged.connect(self.get_i_spc_p5)
         self.w.iSpc_p6.textChanged.connect(self.get_i_spc_p6)
         self.set_font_size()
         self.w.MplWidget.toolbar.setVisible(False)
         self.w.hsqcMultiplet.toolbar.setVisible(False)
         self.w.hsqcPeak.toolbar.setVisible(False)
-        self.w.startNotebookButton.setVisible(False)
-        self.w.stopNotebookButton.setVisible(False)
+        #self.w.startNotebookButton.setVisible(False)
+        #self.w.stopNotebookButton.setVisible(False)
         # self.w.isotopomerHsqcPeak.toolbar.setVisible(False)
         # self.w.isotopomerMultiplet.toolbar.setVisible(False)
         self.w.MplWidget.setFocus()
         self.set_zoom()
         self.w.pickRowColPhCorr2d.clicked.connect(self.pick_col_row)
         self.w.emptyRowColPhCorr2d.clicked.connect(self.empty_col_row)
         self.w.removeRowColPhCorr2d.clicked.connect(self.remove_last_col_row)
@@ -7870,53 +7869,53 @@
         for i in range(max_range):
             # Simulate something that takes time
             time.sleep(max_time / float(max_range))
 
         splash.close()
         # end splash
 
-    def start_notebook(self):
-        try:
-            self.p.terminate()
-            sleep(2)
-        except:
-            pass
-
-        if self.cf.mode == 'dark' or (self.cf.mode == 'system' and darkdetect.isDark()):
-            jupyterthemes.install_theme('chesterish')
-        else:
-            jupyterthemes.install_theme('grade3')
-
-        nmr_dir = os.path.split(inspect.getmodule(nmrDataSet).__file__)[0]
-        base_dir = os.path.split(nmr_dir)[0]
-        jupyter_path = os.path.join(base_dir, "nmr", "jupyter")
-        jobs = []
-        print("-----------------")
-        self.process = multiprocess.Process(target=notebookapp.main,args=([jupyter_path, '--ip=127.0.0.1', '--port=9997'],))
-        #self.process = multiprocess.Process(target=notebookapp.main,args=([jupyter_path, '--no-browser', '--ip=127.0.0.1', '--port=9997', '--NotebookApp.token=''', '--NotebookApp.password='''],))
-        print('=======================')
-        jobs.append(self.process)
-        print('#########################')
-        self.process.start()
-        print('//////////////////////////')
-        sleep(2)
-        print('__________________________')
-        self.w.helpView.setUrl('http://127.0.0.1:9997')
-        self.w.nmrSpectrum.setCurrentIndex(12)
-        # end startNotebook
-
-    def stop_notebook(self):
-        try:
-            self.process.terminate()
-            sleep(2)
-        except:
-            pass
-
-        self.reset_help()
-        # end stop_notebook
+    #def start_notebook(self):
+    #    try:
+    #        self.p.terminate()
+    #        sleep(2)
+    #    except:
+    #        pass
+    #
+    #    if self.cf.mode == 'dark' or (self.cf.mode == 'system' and darkdetect.isDark()):
+    #        jupyterthemes.install_theme('chesterish')
+    #    else:
+    #        jupyterthemes.install_theme('grade3')
+    #
+    #    nmr_dir = os.path.split(inspect.getmodule(nmrDataSet).__file__)[0]
+    #    base_dir = os.path.split(nmr_dir)[0]
+    #    jupyter_path = os.path.join(base_dir, "nmr", "jupyter")
+    #    jobs = []
+    #    print("-----------------")
+    #    self.process = multiprocess.Process(target=notebookapp.main,args=([jupyter_path, '--ip=127.0.0.1', '--port=9997'],))
+    #    #self.process = multiprocess.Process(target=notebookapp.main,args=([jupyter_path, '--no-browser', '--ip=127.0.0.1', '--port=9997', '--NotebookApp.token=''', '--NotebookApp.password='''],))
+    #    print('=======================')
+    #    jobs.append(self.process)
+    #    print('#########################')
+    #    self.process.start()
+    #    print('//////////////////////////')
+    #    sleep(2)
+    #    print('__________________________')
+    #    self.w.helpView.setUrl('http://127.0.0.1:9997')
+    #    self.w.nmrSpectrum.setCurrentIndex(12)
+    #    # end startNotebook
+
+    #def stop_notebook(self):
+    #    try:
+    #        self.process.terminate()
+    #        sleep(2)
+    #    except:
+    #        pass
+    #
+    #    self.reset_help()
+    #    # end stop_notebook
 
     def start_stop_ph_corr(self):
         s = self.nd.s
         e = self.nd.e
         if self.nd.nmrdat[s][e].projected_j_res:
             if self.cf.mode == 'dark' or (self.cf.mode == 'system' and darkdetect.isDark()):
                 txt_col = QColor.fromRgbF(1.0, 1.0, 1.0, 1.0)
```

### Comparing `qtmetabolabpy-0.9.2/qtmetabolabpy/ui/metabolabpy_mainwindow.ui` & `qtmetabolabpy-0.9.4/qtmetabolabpy/ui/metabolabpy_mainwindow.ui`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.2/qtmetabolabpy.egg-info/PKG-INFO` & `qtmetabolabpy-0.9.4/qtmetabolabpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmetabolabpy
-Version: 0.9.2
+Version: 0.9.4
 Summary: Python package for data processing of NMR 1D and 2D metabolomics and metabolism tracing data
 Home-page: https://github.com/ludwigc/qtmetabolabpy
 Author: Christian Ludwig
 Author-email: C.Ludwig@bham.ac.uk 
 License: GPLv3
 Keywords: Metabolomics,Tracing,NMR,Data Processing,13C
 Platform: MacOS, Windows, UNIX
```

### Comparing `qtmetabolabpy-0.9.2/qtmetabolabpy.egg-info/SOURCES.txt` & `qtmetabolabpy-0.9.4/qtmetabolabpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.2/setup.py` & `qtmetabolabpy-0.9.4/setup.py`

 * *Files identical despite different names*

