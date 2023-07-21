# Comparing `tmp/nextnanopy-0.1.7.tar.gz` & `tmp/nextnanopy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nextnanopy-0.1.7.tar", last modified: Thu Dec  3 14:49:45 2020, max compression
+gzip compressed data, was "dist\nextnanopy-0.1.9.tar", last modified: Wed Dec 16 16:48:56 2020, max compression
```

## Comparing `nextnanopy-0.1.7.tar` & `nextnanopy-0.1.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2020-12-03 14:49:45.990873 nextnanopy-0.1.7/
--rw-rw-rw-   0        0        0     8212 2020-12-03 14:49:45.990873 nextnanopy-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     6287 2020-12-03 14:47:47.000000 nextnanopy-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2020-12-03 14:49:45.953015 nextnanopy-0.1.7/nextnanopy/
--rw-rw-rw-   0        0        0      240 2020-11-13 14:31:03.000000 nextnanopy-0.1.7/nextnanopy/__init__.py
--rw-rw-rw-   0        0        0     2548 2020-12-02 15:31:28.000000 nextnanopy-0.1.7/nextnanopy/commands.py
--rw-rw-rw-   0        0        0     5472 2020-12-02 12:34:02.000000 nextnanopy-0.1.7/nextnanopy/defaults.py
--rw-rw-rw-   0        0        0    11298 2020-12-03 11:27:27.000000 nextnanopy-0.1.7/nextnanopy/inputs.py
-drwxrwxrwx   0        0        0        0 2020-12-03 14:49:45.975852 nextnanopy-0.1.7/nextnanopy/msb/
--rw-rw-rw-   0        0        0        0 2020-11-11 14:54:24.000000 nextnanopy-0.1.7/nextnanopy/msb/__init__.py
--rw-rw-rw-   0        0        0     1542 2020-11-29 16:45:20.000000 nextnanopy-0.1.7/nextnanopy/msb/defaults.py
--rw-rw-rw-   0        0        0      331 2020-11-29 16:45:20.000000 nextnanopy-0.1.7/nextnanopy/msb/inputs.py
--rw-rw-rw-   0        0        0     4109 2020-12-02 12:34:02.000000 nextnanopy-0.1.7/nextnanopy/msb/outputs.py
-drwxrwxrwx   0        0        0        0 2020-12-03 14:49:45.977846 nextnanopy-0.1.7/nextnanopy/negf/
--rw-rw-rw-   0        0        0        0 2020-11-11 14:54:24.000000 nextnanopy-0.1.7/nextnanopy/negf/__init__.py
--rw-rw-rw-   0        0        0     1483 2020-11-29 16:45:20.000000 nextnanopy-0.1.7/nextnanopy/negf/defaults.py
--rw-rw-rw-   0        0        0      335 2020-11-29 16:45:20.000000 nextnanopy-0.1.7/nextnanopy/negf/inputs.py
--rw-rw-rw-   0        0        0     5336 2020-12-02 12:34:02.000000 nextnanopy-0.1.7/nextnanopy/negf/outputs.py
-drwxrwxrwx   0        0        0        0 2020-12-03 14:49:45.980838 nextnanopy-0.1.7/nextnanopy/nn3/
--rw-rw-rw-   0        0        0        0 2020-11-11 14:54:24.000000 nextnanopy-0.1.7/nextnanopy/nn3/__init__.py
--rw-rw-rw-   0        0        0     2006 2020-11-29 16:45:20.000000 nextnanopy-0.1.7/nextnanopy/nn3/defaults.py
--rw-rw-rw-   0        0        0      846 2020-11-29 16:45:20.000000 nextnanopy-0.1.7/nextnanopy/nn3/inputs.py
--rw-rw-rw-   0        0        0     4820 2020-12-03 11:38:23.000000 nextnanopy-0.1.7/nextnanopy/nn3/outputs.py
-drwxrwxrwx   0        0        0        0 2020-12-03 14:49:45.984828 nextnanopy-0.1.7/nextnanopy/nnp/
--rw-rw-rw-   0        0        0        0 2020-11-11 14:54:24.000000 nextnanopy-0.1.7/nextnanopy/nnp/__init__.py
--rw-rw-rw-   0        0        0    18241 2020-11-11 14:54:24.000000 nextnanopy-0.1.7/nextnanopy/nnp/assistants.py
--rw-rw-rw-   0        0        0     1704 2020-11-29 16:45:20.000000 nextnanopy-0.1.7/nextnanopy/nnp/defaults.py
--rw-rw-rw-   0        0        0      847 2020-11-29 16:45:20.000000 nextnanopy-0.1.7/nextnanopy/nnp/inputs.py
--rw-rw-rw-   0        0        0     4821 2020-12-03 11:38:23.000000 nextnanopy-0.1.7/nextnanopy/nnp/outputs.py
--rw-rw-rw-   0        0        0     2683 2020-11-29 17:23:23.000000 nextnanopy-0.1.7/nextnanopy/nnp/shapes.py
--rw-rw-rw-   0        0        0    13105 2020-12-03 12:03:38.000000 nextnanopy-0.1.7/nextnanopy/outputs.py
--rw-rw-rw-   0        0        0     9434 2020-11-11 17:22:26.000000 nextnanopy-0.1.7/nextnanopy/shapes.py
-drwxrwxrwx   0        0        0        0 2020-12-03 14:49:45.990873 nextnanopy-0.1.7/nextnanopy/utils/
--rw-rw-rw-   0        0        0        0 2020-10-30 15:04:06.000000 nextnanopy-0.1.7/nextnanopy/utils/__init__.py
--rw-rw-rw-   0        0        0     4810 2020-12-03 11:58:51.000000 nextnanopy-0.1.7/nextnanopy/utils/config.py
--rw-rw-rw-   0        0        0     7880 2020-12-03 13:40:15.000000 nextnanopy-0.1.7/nextnanopy/utils/datasets.py
--rw-rw-rw-   0        0        0     4925 2020-12-02 12:34:02.000000 nextnanopy-0.1.7/nextnanopy/utils/formatting.py
--rw-rw-rw-   0        0        0     2956 2020-11-28 09:42:13.000000 nextnanopy-0.1.7/nextnanopy/utils/misc.py
--rw-rw-rw-   0        0        0     1625 2020-12-03 13:46:05.000000 nextnanopy-0.1.7/nextnanopy/utils/mycollections.py
--rw-rw-rw-   0        0        0      405 2020-11-03 15:04:37.000000 nextnanopy-0.1.7/nextnanopy/utils/timer.py
-drwxrwxrwx   0        0        0        0 2020-12-03 14:49:45.958067 nextnanopy-0.1.7/nextnanopy.egg-info/
--rw-rw-rw-   0        0        0     8212 2020-12-03 14:49:45.000000 nextnanopy-0.1.7/nextnanopy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      999 2020-12-03 14:49:45.000000 nextnanopy-0.1.7/nextnanopy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-12-03 14:49:45.000000 nextnanopy-0.1.7/nextnanopy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2020-12-03 14:49:45.000000 nextnanopy-0.1.7/nextnanopy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2020-12-03 14:49:45.000000 nextnanopy-0.1.7/nextnanopy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-12-03 14:49:45.990873 nextnanopy-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     3027 2020-12-03 12:05:13.000000 nextnanopy-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2020-12-16 16:48:56.822083 nextnanopy-0.1.9/
+-rw-rw-rw-   0        0        0     8398 2020-12-16 16:48:56.821085 nextnanopy-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6423 2020-12-16 16:48:23.000000 nextnanopy-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2020-12-16 16:48:56.701367 nextnanopy-0.1.9/nextnanopy/
+-rw-rw-rw-   0        0        0      240 2020-11-13 14:31:03.000000 nextnanopy-0.1.9/nextnanopy/__init__.py
+-rw-rw-rw-   0        0        0     2632 2020-12-16 16:48:23.000000 nextnanopy-0.1.9/nextnanopy/commands.py
+-rw-rw-rw-   0        0        0     5625 2020-12-16 16:48:23.000000 nextnanopy-0.1.9/nextnanopy/defaults.py
+-rw-rw-rw-   0        0        0    11790 2020-12-16 16:48:23.000000 nextnanopy-0.1.9/nextnanopy/inputs.py
+drwxrwxrwx   0        0        0        0 2020-12-16 16:48:56.747245 nextnanopy-0.1.9/nextnanopy/msb/
+-rw-rw-rw-   0        0        0        0 2020-11-11 14:54:24.000000 nextnanopy-0.1.9/nextnanopy/msb/__init__.py
+-rw-rw-rw-   0        0        0     1542 2020-11-29 16:45:20.000000 nextnanopy-0.1.9/nextnanopy/msb/defaults.py
+-rw-rw-rw-   0        0        0      331 2020-11-29 16:45:20.000000 nextnanopy-0.1.9/nextnanopy/msb/inputs.py
+-rw-rw-rw-   0        0        0     4109 2020-12-16 16:47:47.000000 nextnanopy-0.1.9/nextnanopy/msb/outputs.py
+drwxrwxrwx   0        0        0        0 2020-12-16 16:48:56.758216 nextnanopy-0.1.9/nextnanopy/negf/
+-rw-rw-rw-   0        0        0        0 2020-11-11 14:54:24.000000 nextnanopy-0.1.9/nextnanopy/negf/__init__.py
+-rw-rw-rw-   0        0        0     1483 2020-11-29 16:45:20.000000 nextnanopy-0.1.9/nextnanopy/negf/defaults.py
+-rw-rw-rw-   0        0        0      335 2020-11-29 16:45:20.000000 nextnanopy-0.1.9/nextnanopy/negf/inputs.py
+-rw-rw-rw-   0        0        0     5336 2020-12-16 16:47:47.000000 nextnanopy-0.1.9/nextnanopy/negf/outputs.py
+drwxrwxrwx   0        0        0        0 2020-12-16 16:48:56.769185 nextnanopy-0.1.9/nextnanopy/nn3/
+-rw-rw-rw-   0        0        0        0 2020-11-11 14:54:24.000000 nextnanopy-0.1.9/nextnanopy/nn3/__init__.py
+-rw-rw-rw-   0        0        0     2006 2020-11-29 16:45:20.000000 nextnanopy-0.1.9/nextnanopy/nn3/defaults.py
+-rw-rw-rw-   0        0        0      846 2020-11-29 16:45:20.000000 nextnanopy-0.1.9/nextnanopy/nn3/inputs.py
+-rw-rw-rw-   0        0        0     4820 2020-12-16 16:47:47.000000 nextnanopy-0.1.9/nextnanopy/nn3/outputs.py
+drwxrwxrwx   0        0        0        0 2020-12-16 16:48:56.807519 nextnanopy-0.1.9/nextnanopy/nnp/
+-rw-rw-rw-   0        0        0        0 2020-11-11 14:54:24.000000 nextnanopy-0.1.9/nextnanopy/nnp/__init__.py
+-rw-rw-rw-   0        0        0    18241 2020-11-11 14:54:24.000000 nextnanopy-0.1.9/nextnanopy/nnp/assistants.py
+-rw-rw-rw-   0        0        0     1704 2020-11-29 16:45:20.000000 nextnanopy-0.1.9/nextnanopy/nnp/defaults.py
+-rw-rw-rw-   0        0        0      847 2020-11-29 16:45:20.000000 nextnanopy-0.1.9/nextnanopy/nnp/inputs.py
+-rw-rw-rw-   0        0        0     4821 2020-12-16 16:47:47.000000 nextnanopy-0.1.9/nextnanopy/nnp/outputs.py
+-rw-rw-rw-   0        0        0     2683 2020-11-29 17:23:23.000000 nextnanopy-0.1.9/nextnanopy/nnp/shapes.py
+-rw-rw-rw-   0        0        0    13046 2020-12-16 16:48:23.000000 nextnanopy-0.1.9/nextnanopy/outputs.py
+-rw-rw-rw-   0        0        0     9205 2020-12-16 16:47:47.000000 nextnanopy-0.1.9/nextnanopy/shapes.py
+drwxrwxrwx   0        0        0        0 2020-12-16 16:48:56.820086 nextnanopy-0.1.9/nextnanopy/utils/
+-rw-rw-rw-   0        0        0        0 2020-10-30 15:04:06.000000 nextnanopy-0.1.9/nextnanopy/utils/__init__.py
+-rw-rw-rw-   0        0        0     4810 2020-12-16 16:47:47.000000 nextnanopy-0.1.9/nextnanopy/utils/config.py
+-rw-rw-rw-   0        0        0     7881 2020-12-16 16:47:47.000000 nextnanopy-0.1.9/nextnanopy/utils/datasets.py
+-rw-rw-rw-   0        0        0     4925 2020-12-16 16:47:47.000000 nextnanopy-0.1.9/nextnanopy/utils/formatting.py
+-rw-rw-rw-   0        0        0     3277 2020-12-16 16:48:23.000000 nextnanopy-0.1.9/nextnanopy/utils/misc.py
+-rw-rw-rw-   0        0        0     1625 2020-12-16 16:47:47.000000 nextnanopy-0.1.9/nextnanopy/utils/mycollections.py
+-rw-rw-rw-   0        0        0      405 2020-11-03 15:04:37.000000 nextnanopy-0.1.9/nextnanopy/utils/timer.py
+drwxrwxrwx   0        0        0        0 2020-12-16 16:48:56.720317 nextnanopy-0.1.9/nextnanopy.egg-info/
+-rw-rw-rw-   0        0        0     8398 2020-12-16 16:48:56.000000 nextnanopy-0.1.9/nextnanopy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      999 2020-12-16 16:48:56.000000 nextnanopy-0.1.9/nextnanopy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-12-16 16:48:56.000000 nextnanopy-0.1.9/nextnanopy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2020-12-16 16:48:56.000000 nextnanopy-0.1.9/nextnanopy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2020-12-16 16:48:56.000000 nextnanopy-0.1.9/nextnanopy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2020-12-16 16:48:56.822083 nextnanopy-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     3027 2020-12-16 16:48:23.000000 nextnanopy-0.1.9/setup.py
```

### Comparing `nextnanopy-0.1.7/PKG-INFO` & `nextnanopy-0.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,97 +1,103 @@
 Metadata-Version: 2.1
 Name: nextnanopy
-Version: 0.1.7
+Version: 0.1.9
 Summary: Useful tools to interface the nextnano software (https://www.nextnano.com/)
 Home-page: https://github.com/nextnanopy/nextnanopy
 Author: nextnano GmbH
 Author-email: python@nextnano.com
 License: BSD-3-Clause
 Description: # NEXTNANOPY README
         
         [![BSD-3-Clause](https://img.shields.io/github/license/nextnanopy/nextnanopy)](https://opensource.org/licenses/BSD-3-Clause)
         [![Downloads](https://img.shields.io/github/downloads/nextnanopy/nextnanopy/total)](https://github.com/nextnanopy/nextnanopy/releases)
         
         nextnanopy is a Python module to interface the [nextnano](https://www.nextnano.com/) software. This package includes features for:
-        * **Output files**: user-friendly method to load the datafiles which allows easy and flexible post-processing. 
-        * **Input files:** load input files, set variables, save by finding unused name, execute the file, write input files, etc.
-        * **Configuration**: setup default nextnano configuration (path to executables, databases, licenses, etc).
-        * **Import from GDS files**: load polygons from GDS files and user-friendly methods to generate raw text of nextnano shapes (beta).
+        * **Output files**: User-friendly method to load the datafiles which allows easy and flexible post-processing. 
+        * **Input files:** Load input files, set variables, save by finding unused name, execute the file, write input files, etc.
+        * **Configuration**: Setup default nextnano configuration (path to executables, databases, licenses, etc).
+        * **Import from GDS files**: Load polygons from GDS files and user-friendly methods to generate raw text of nextnano shapes (beta).
         
-        **Note:** the license is not compulsory for the general use of nextnanopy, unless you would like to execute input files via Python.
+        **Note:** A valid license for the nextnano software is not compulsory for the general use of nextnanopy, unless you would like to execute input files via Python.
         
         ## Future of nextnanopy
-        Currently, nextnanopy has basic features for [nextnano products](https://www.nextnano.com/products/products.php) nextnano++, nextnano3, nextnano.NEGF and nextnano/MSB. The goal is to extend the functionalities to nextnano.MSB in future releases.
+        Currently, nextnanopy has basic features for [nextnano products](https://www.nextnano.com/products/products.php) nextnano++, nextnanoÂ³, nextnano.NEGF and nextnano.MSB.
         
         In future releases, we would like to implement:
         
-        * **Common post-processing methods**: like loading and plotting together bandedges, eigenenergies and eigenlevels, colormap of potential landscape with GDS polygons on top, etc.
-        * **Support for any nextnano.NEGF datafiles**: in the current release, it is only implemented the loading of .dat files (most of them).
-        * **Support for any nextnano.MSB datafiles**: not loading routines are implemented yet.
-        * **User-friendly input file creation/modification**: the idea is to load any input file and it would detect all the different blocks so the user can easily modify parameters like 'boundary conditions' or 'region material'. Similarly, it should be user-friendly to create any input file from scratch via Python.
-        * **Feedback loops**: a routine that allows the user to optimize any figure of merit of a device with a given set of input variables. The user can set a post-processing routine to get the figure of merit from the simulated data and later, a new set of input variables will be generated and executed. This feedback loop will repeat until a set of conditions are satisfied.
-        * **Improve documentation**: we will add an extensive documentation in the website as well as in the source code.
-        * **Guidelines for contributors**: set of rules if you want to contribute to the project.
+        * **Common post-processing methods**: Like loading and plotting together bandedges, eigenenergies and eigenlevels, colormap of potential landscape with GDS polygons on top, etc.
+        * **Improved support for specific nextnano.NEGF and nextnano.MSB datafiles**
+        * **User-friendly input file creation/modification**: The idea is to load any input file and it would detect all the different blocks so the user can easily modify parameters like 'boundary conditions' or 'region material'. Similarly, it should be user-friendly to create any input file from scratch via Python.
+        * **Feedback loops**: A routine that allows the user to optimize any figure of merit of a device with a given set of input variables. The user can set a post-processing routine to get the figure of merit from the simulated data and later, a new set of input variables will be generated and executed. This feedback loop will repeat until a set of conditions are satisfied.
+        * **Improve documentation**: We will add an extensive documentation in the website as well as in the source code.
+        * **Guidelines for contributors**: Set of rules if you want to contribute to the project.
          
         ## Installation
         
         ### Requirements
         
-        You need a working python 3.x installation to be able to use nextnanopy. We highly recommend installing [Anaconda](https://www.anaconda.com/), which takes care of installing Python and managing packages. 
-        Make sure to download the latest version with python 3.8.
+        You need a working Python 3.8 installation to be able to use nextnanopy. We highly recommend installing [Anaconda](https://www.anaconda.com/), which takes care of installing Python and managing packages. 
+        Make sure to download the latest version with Python 3.8.
         
         ### Dependencies:
         
         * [Python](https://www.python.org/) (tested with 3.8)
-        * [Numpy](http://numpy.scipy.org/)
+        * [NumPy](http://numpy.scipy.org/)
         * [PyVista](https://www.pyvista.org/) (For loading VTK files)
         * [Gdspy](https://gdspy.readthedocs.io/) (optional: to import gds files)
         * [Shapely](https://shapely.readthedocs.io/) (optional: to manipulate polygons from gds files)
         * [Matplotlib](https://matplotlib.org/) (optional: to visualize imported polygons)
-        * [Cylcer](https://pypi.org/project/Cycler/) (optional: to visualize imported polygons)
+        * [Cycler](https://pypi.org/project/Cycler/) (optional: to visualize imported polygons)
         
         ### Linux / OS X / Windows
         
         #### Option 1: Using [pip](https://docs.python.org/3/installing/)
         
-        Simply open anaconda prompt and type:
+        Simply open Anaconda prompt and type:
         
         ```sh
         pip install nextnanopy
         ```
         or if you want to upgrade:
         ```sh
         pip install --upgrade nextnanopy
         ```
         
-        #### Option 2: from the source code
+        #### Option 2: From the source code
         
         1. Download the source from [github](https://github.com/nextnanopy/nextnanopy)
-        2. Open anaconda prompt
+        2. Open Anaconda prompt
         3. Go to the directory of the nextnanopy project
         4. Build/install by typing:
         
         ```sh
         python setup.py install
         ```
         
-        For more information, please, see the documents in docs folder.
+        For more information, please see the documents in docs/ folder.
         
         ## Documentation
         
-        Currently, the complete documentation is not available yet. However, there are few examples located in docs/examples that will help you to start playing with nextnanopy.
+        Currently, the complete documentation is not available yet. However, there are few examples located in templates/ and docs/examples that will help you to start playing with nextnanopy.
         
         
         ## Support
         
         Do you want to help nextnanopy? Please, send an email to [python@nextnano.com](mailto:python@nextnano.com). 
         
         
         ## History of changes
         
+        ### Version 0.1.9 (Dec 14th, 2020)
+        * Feature: InputFile.execute has now show_log (True or False) to turn on/off the log. Note: the log file is always saved. 
+        * Removed default messages when saving an input file
+        
+        ### Version 0.1.8 (Dec 14th, 2020)
+        * Buf fix: find unused name when saving input file
+        
         ### Version 0.1.7 (Dec 3rd, 2020)
         * docstring for inputs.py, outputs.py, config.py, mycollections.py, datasets.py
         * Updated examples in docs/examples/
         
         ### Version 0.1.6 (Dec 2nd, 2020)
         * Feature: [DataFile] access with index to coordinates and to variables
         ```python
@@ -106,41 +112,41 @@
         df['xmax'] # same as df.variables['xmax']
         ```
         * Feature: [InputFile] is loopable as well as .coords and .variables
         * Feature: [InputFile] extra attributes
         ```python
         df = nextnanopy.InputFile(...)
         df.folder_output # returns the output folder if it was executed, otherwise it raises an error
-        df.filename # settable
+        df.filename      # settable
         df.filename_only # settable
-        df.folder_input # settable
+        df.folder_input  # settable
         ```
-        * Feature: user-friendly information for DataFile, InputFile, Variable, Coord and InputVariable.
+        * Feature: User-friendly information for DataFile, InputFile, Variable, Coord and InputVariable
         * Bug fix: .vtr dataset reshape method
         
         ### Version 0.1.5 (Dec 2nd, 2020)
-        * Feature: support .vtr data files
-        * Feature: if unit is not found, default value is 'a.u'
-        * Bug fix: better methods to find correctly name and unit from data file headers
+        * Feature: Support of .vtr data files
+        * Feature: If unit is not found, default value is 'a.u.'.
+        * Bug fix: Better methods to find correctly name and unit from data file headers
         
         ### Version 0.1.4 (Nov 29th, 2020)
-        * Feature: create an empty input file and set the raw text with the attribute text.
+        * Feature: Create an empty input file and set the raw text with the attribute text.
         
         ### Version 0.1.3 (Nov 28th, 2020)
-        * Bug fix: find unused name when save input files
-        * Feature: default label for Variables and Coords. The attribute label returns "name (unit)". 
+        * Bug fix: Find unused name when save input files.
+        * Feature: Default label for Variables and Coords. The attribute label returns "name (unit)". 
         
         ### Version 0.1.2 (Nov 20th, 2020)
-        * Bug fix: Raw text of input variables without comment was generated incorrectly
+        * Bug fix: Raw text of input variables without comment was generated incorrectly.
         
         ### Version 0.1.1 (Nov 18th, 2020)
-        * Bug fix: find the home path for OSX and Linux. 
+        * Bug fix: Find the home path for OSX and Linux.
         
         ### Version 0.1.0 (Nov 13th, 2020)
-        * Initial release.
+        * Initial release
         
 Keywords: nextnano
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Customer Service
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nextnanopy-0.1.7/README.md` & `nextnanopy-0.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,89 +1,95 @@
 # NEXTNANOPY README
 
 [![BSD-3-Clause](https://img.shields.io/github/license/nextnanopy/nextnanopy)](https://opensource.org/licenses/BSD-3-Clause)
 [![Downloads](https://img.shields.io/github/downloads/nextnanopy/nextnanopy/total)](https://github.com/nextnanopy/nextnanopy/releases)
 
 nextnanopy is a Python module to interface the [nextnano](https://www.nextnano.com/) software. This package includes features for:
-* **Output files**: user-friendly method to load the datafiles which allows easy and flexible post-processing. 
-* **Input files:** load input files, set variables, save by finding unused name, execute the file, write input files, etc.
-* **Configuration**: setup default nextnano configuration (path to executables, databases, licenses, etc).
-* **Import from GDS files**: load polygons from GDS files and user-friendly methods to generate raw text of nextnano shapes (beta).
+* **Output files**: User-friendly method to load the datafiles which allows easy and flexible post-processing. 
+* **Input files:** Load input files, set variables, save by finding unused name, execute the file, write input files, etc.
+* **Configuration**: Setup default nextnano configuration (path to executables, databases, licenses, etc).
+* **Import from GDS files**: Load polygons from GDS files and user-friendly methods to generate raw text of nextnano shapes (beta).
 
-**Note:** the license is not compulsory for the general use of nextnanopy, unless you would like to execute input files via Python.
+**Note:** A valid license for the nextnano software is not compulsory for the general use of nextnanopy, unless you would like to execute input files via Python.
 
 ## Future of nextnanopy
-Currently, nextnanopy has basic features for [nextnano products](https://www.nextnano.com/products/products.php) nextnano++, nextnano3, nextnano.NEGF and nextnano/MSB. The goal is to extend the functionalities to nextnano.MSB in future releases.
+Currently, nextnanopy has basic features for [nextnano products](https://www.nextnano.com/products/products.php) nextnano++, nextnano³, nextnano.NEGF and nextnano.MSB.
 
 In future releases, we would like to implement:
 
-* **Common post-processing methods**: like loading and plotting together bandedges, eigenenergies and eigenlevels, colormap of potential landscape with GDS polygons on top, etc.
-* **Support for any nextnano.NEGF datafiles**: in the current release, it is only implemented the loading of .dat files (most of them).
-* **Support for any nextnano.MSB datafiles**: not loading routines are implemented yet.
-* **User-friendly input file creation/modification**: the idea is to load any input file and it would detect all the different blocks so the user can easily modify parameters like 'boundary conditions' or 'region material'. Similarly, it should be user-friendly to create any input file from scratch via Python.
-* **Feedback loops**: a routine that allows the user to optimize any figure of merit of a device with a given set of input variables. The user can set a post-processing routine to get the figure of merit from the simulated data and later, a new set of input variables will be generated and executed. This feedback loop will repeat until a set of conditions are satisfied.
-* **Improve documentation**: we will add an extensive documentation in the website as well as in the source code.
-* **Guidelines for contributors**: set of rules if you want to contribute to the project.
+* **Common post-processing methods**: Like loading and plotting together bandedges, eigenenergies and eigenlevels, colormap of potential landscape with GDS polygons on top, etc.
+* **Improved support for specific nextnano.NEGF and nextnano.MSB datafiles**
+* **User-friendly input file creation/modification**: The idea is to load any input file and it would detect all the different blocks so the user can easily modify parameters like 'boundary conditions' or 'region material'. Similarly, it should be user-friendly to create any input file from scratch via Python.
+* **Feedback loops**: A routine that allows the user to optimize any figure of merit of a device with a given set of input variables. The user can set a post-processing routine to get the figure of merit from the simulated data and later, a new set of input variables will be generated and executed. This feedback loop will repeat until a set of conditions are satisfied.
+* **Improve documentation**: We will add an extensive documentation in the website as well as in the source code.
+* **Guidelines for contributors**: Set of rules if you want to contribute to the project.
  
 ## Installation
 
 ### Requirements
 
-You need a working python 3.x installation to be able to use nextnanopy. We highly recommend installing [Anaconda](https://www.anaconda.com/), which takes care of installing Python and managing packages. 
-Make sure to download the latest version with python 3.8.
+You need a working Python 3.8 installation to be able to use nextnanopy. We highly recommend installing [Anaconda](https://www.anaconda.com/), which takes care of installing Python and managing packages. 
+Make sure to download the latest version with Python 3.8.
 
 ### Dependencies:
 
 * [Python](https://www.python.org/) (tested with 3.8)
-* [Numpy](http://numpy.scipy.org/)
+* [NumPy](http://numpy.scipy.org/)
 * [PyVista](https://www.pyvista.org/) (For loading VTK files)
 * [Gdspy](https://gdspy.readthedocs.io/) (optional: to import gds files)
 * [Shapely](https://shapely.readthedocs.io/) (optional: to manipulate polygons from gds files)
 * [Matplotlib](https://matplotlib.org/) (optional: to visualize imported polygons)
-* [Cylcer](https://pypi.org/project/Cycler/) (optional: to visualize imported polygons)
+* [Cycler](https://pypi.org/project/Cycler/) (optional: to visualize imported polygons)
 
 ### Linux / OS X / Windows
 
 #### Option 1: Using [pip](https://docs.python.org/3/installing/)
 
-Simply open anaconda prompt and type:
+Simply open Anaconda prompt and type:
 
 ```sh
 pip install nextnanopy
 ```
 or if you want to upgrade:
 ```sh
 pip install --upgrade nextnanopy
 ```
 
-#### Option 2: from the source code
+#### Option 2: From the source code
 
 1. Download the source from [github](https://github.com/nextnanopy/nextnanopy)
-2. Open anaconda prompt
+2. Open Anaconda prompt
 3. Go to the directory of the nextnanopy project
 4. Build/install by typing:
 
 ```sh
 python setup.py install
 ```
 
-For more information, please, see the documents in docs folder.
+For more information, please see the documents in docs/ folder.
 
 ## Documentation
 
-Currently, the complete documentation is not available yet. However, there are few examples located in docs/examples that will help you to start playing with nextnanopy.
+Currently, the complete documentation is not available yet. However, there are few examples located in templates/ and docs/examples that will help you to start playing with nextnanopy.
 
 
 ## Support
 
 Do you want to help nextnanopy? Please, send an email to [python@nextnano.com](mailto:python@nextnano.com). 
 
 
 ## History of changes
 
+### Version 0.1.9 (Dec 14th, 2020)
+* Feature: InputFile.execute has now show_log (True or False) to turn on/off the log. Note: the log file is always saved. 
+* Removed default messages when saving an input file
+
+### Version 0.1.8 (Dec 14th, 2020)
+* Buf fix: find unused name when saving input file
+
 ### Version 0.1.7 (Dec 3rd, 2020)
 * docstring for inputs.py, outputs.py, config.py, mycollections.py, datasets.py
 * Updated examples in docs/examples/
 
 ### Version 0.1.6 (Dec 2nd, 2020)
 * Feature: [DataFile] access with index to coordinates and to variables
 ```python
@@ -98,34 +104,34 @@
 df['xmax'] # same as df.variables['xmax']
 ```
 * Feature: [InputFile] is loopable as well as .coords and .variables
 * Feature: [InputFile] extra attributes
 ```python
 df = nextnanopy.InputFile(...)
 df.folder_output # returns the output folder if it was executed, otherwise it raises an error
-df.filename # settable
+df.filename      # settable
 df.filename_only # settable
-df.folder_input # settable
+df.folder_input  # settable
 ```
-* Feature: user-friendly information for DataFile, InputFile, Variable, Coord and InputVariable.
+* Feature: User-friendly information for DataFile, InputFile, Variable, Coord and InputVariable
 * Bug fix: .vtr dataset reshape method
 
 ### Version 0.1.5 (Dec 2nd, 2020)
-* Feature: support .vtr data files
-* Feature: if unit is not found, default value is 'a.u'
-* Bug fix: better methods to find correctly name and unit from data file headers
+* Feature: Support of .vtr data files
+* Feature: If unit is not found, default value is 'a.u.'.
+* Bug fix: Better methods to find correctly name and unit from data file headers
 
 ### Version 0.1.4 (Nov 29th, 2020)
-* Feature: create an empty input file and set the raw text with the attribute text.
+* Feature: Create an empty input file and set the raw text with the attribute text.
 
 ### Version 0.1.3 (Nov 28th, 2020)
-* Bug fix: find unused name when save input files
-* Feature: default label for Variables and Coords. The attribute label returns "name (unit)". 
+* Bug fix: Find unused name when save input files.
+* Feature: Default label for Variables and Coords. The attribute label returns "name (unit)". 
 
 ### Version 0.1.2 (Nov 20th, 2020)
-* Bug fix: Raw text of input variables without comment was generated incorrectly
+* Bug fix: Raw text of input variables without comment was generated incorrectly.
 
 ### Version 0.1.1 (Nov 18th, 2020)
-* Bug fix: find the home path for OSX and Linux. 
+* Bug fix: Find the home path for OSX and Linux.
 
 ### Version 0.1.0 (Nov 13th, 2020)
-* Initial release.
+* Initial release
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nextnanopy-0.1.7/nextnanopy/commands.py` & `nextnanopy-0.1.9/nextnanopy/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,31 +35,32 @@
 def read_output(pipe, funcs):
     for line in iter(pipe.readline, b''):
         for func in funcs:
             func(line)
     pipe.close()
 
 
-def write_output(get, filepath):
+def write_output(get, filepath, show=True):
     f = open(filepath, 'w', newline='')
     for line in iter(get, None):
         line = str(line, 'utf-8', errors='ignore')
-        sys.stdout.write(line)
+        if show:
+            sys.stdout.write(line)
         f.write(line)
     f.close()
 
 
-def start_log(process, filepath):
+def start_log(process, filepath, show=True):
     q = queue.Queue()
     out, err = [], []
     tout = threading.Thread(
         target=read_output, args=(process.stdout, [q.put, out.append]))
     terr = threading.Thread(
         target=read_output, args=(process.stderr, [q.put, err.append]))
-    twrite = threading.Thread(target=write_output, args=(q.get, filepath))
+    twrite = threading.Thread(target=write_output, args=(q.get, filepath, show))
     for t in (tout, terr, twrite):
         t.daemon = False
         t.start()
     process.wait()
     for t in (tout, terr):
         t.join()
     q.put(None)
@@ -67,26 +68,27 @@
 
 def execute(
         inputfile,
         exe,
         license,
         database,
         outputdirectory,
+        show_log=True,
         **kwargs,
 ):
     filename = get_filename(inputfile, ext=False)
     outputdirectory = os.path.join(outputdirectory, filename)
     mkdir_if_not_exist(outputdirectory)
     logfile = os.path.join(outputdirectory, f'{filename}.log')
     cmd = command(inputfile, exe, license, database, outputdirectory, **kwargs)
     cwd = os.getcwd()
     wdir = os.path.split(exe)[0]  # nn3 assumes wdir at one folder upper than the executable
     os.chdir(wdir)
     process = send(cmd)
-    start_log(process, logfile)
+    start_log(process, logfile, show_log)
     os.chdir(cwd)
     info = {
         'process': process,
         'outputdirectory': outputdirectory,
         'filename': filename,
         'logfile': logfile,
         'cmd': cmd,
```

### Comparing `nextnanopy-0.1.7/nextnanopy/defaults.py` & `nextnanopy-0.1.9/nextnanopy/defaults.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 import os
 from pathlib import Path
 from nextnanopy.utils.config import Config
 
 products = ['nextnano++', 'nextnano3', 'nextnano.NEGF', 'nextnano.MSB']
 default_folder = str(Path.home())
 config_default_path = os.path.join(default_folder, '.nextnanopy-config')
+messages = {
+    'load_input': [None, None],
+    'save_input': [None, None],
+    'execute_input': [None, None],
+    'load_output': [None, None],
+}
 
 
 def get_InputFile(product):
     if product == 'nextnano++':
         from nextnanopy.nnp.inputs import InputFile
     elif product == 'nextnano3':
         from nextnanopy.nn3.inputs import InputFile
```

### Comparing `nextnanopy-0.1.7/nextnanopy/inputs.py` & `nextnanopy-0.1.9/nextnanopy/inputs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 import os
 from nextnanopy.utils.formatting import text_to_lines, lines_to_text
 from nextnanopy.utils.mycollections import DictList
-from nextnanopy.utils.misc import savetxt, get_filename, get_folder, get_file_extension
+from nextnanopy.utils.misc import savetxt, get_filename, get_folder, get_file_extension, message_decorator
 from nextnanopy.commands import execute as cmd_execute
 from nextnanopy import defaults
 
+_msgs = defaults.messages['load_input']
+load_message = lambda method: message_decorator(method, init_msg=_msgs[0], end_msg=_msgs[1])
+_msgs = defaults.messages['save_input']
+save_message = lambda method: message_decorator(method, init_msg=_msgs[0], end_msg=_msgs[1])
+_msgs = defaults.messages['execute_input']
+execute_message = lambda method: message_decorator(method, init_msg=_msgs[0], end_msg=_msgs[1])
+
 
 class InputFileTemplate(object):
     """
         This class stores and manipulates any kind of nextnano input files.
         For each nextnano product, the syntax is different but the core information
         is very similar like the variables that can be changed.
         This class contains useful methods such as to get a preview of the file or
@@ -166,14 +173,15 @@
         """
         for i, line in enumerate(self.lines):
             if nums:
                 print(f'{i} {line}')
             else:
                 print(f'{line}')
 
+    @load_message
     def load(self, fullpath):
         """
         The steps are the following:
             1. clear the current information
             2. load the raw text (update .fullpath and .raw_lines)
             3. find the nextnano product (update .product)
             4. validate the input file
@@ -195,14 +203,15 @@
         self.product = defaults.input_text_type(self.text)
         return self.product
 
     def validate(self):
         if self.product not in defaults.products:
             raise ValueError(f'Not valid input file')
 
+    @save_message
     def save(self, fullpath=None, overwrite=False, automkdir=True):
         """
         Save the current information into a file.
 
         Parameters
         ----------
         fullpath : str, optional
@@ -218,14 +227,15 @@
         if fullpath is None:
             if self.fullpath is None:
                 raise ValueError('Please, specify a fullpath')
             fullpath = self.fullpath
         self.fullpath = savetxt(fullpath=fullpath, text=self.text, overwrite=overwrite, automkdir=automkdir)
         return self.fullpath
 
+    @execute_message
     def execute(self, **kwargs):
         """
         Execute the input file located at .fullpath
         Individual kwargs can be passed like 'license' or 'database'
         If no kwargs is specified, it will use the default values in .config
 
         Parameters
```

### Comparing `nextnanopy-0.1.7/nextnanopy/msb/defaults.py` & `nextnanopy-0.1.9/nextnanopy/msb/defaults.py`

 * *Files identical despite different names*

### Comparing `nextnanopy-0.1.7/nextnanopy/msb/outputs.py` & `nextnanopy-0.1.9/nextnanopy/msb/outputs.py`

 * *Files identical despite different names*

### Comparing `nextnanopy-0.1.7/nextnanopy/negf/defaults.py` & `nextnanopy-0.1.9/nextnanopy/negf/defaults.py`

 * *Files identical despite different names*

### Comparing `nextnanopy-0.1.7/nextnanopy/negf/outputs.py` & `nextnanopy-0.1.9/nextnanopy/negf/outputs.py`

 * *Files identical despite different names*

### Comparing `nextnanopy-0.1.7/nextnanopy/nn3/defaults.py` & `nextnanopy-0.1.9/nextnanopy/nn3/defaults.py`

 * *Files identical despite different names*

### Comparing `nextnanopy-0.1.7/nextnanopy/nn3/inputs.py` & `nextnanopy-0.1.9/nextnanopy/nn3/inputs.py`

 * *Files identical despite different names*

### Comparing `nextnanopy-0.1.7/nextnanopy/nn3/outputs.py` & `nextnanopy-0.1.9/nextnanopy/nn3/outputs.py`

 * *Files identical despite different names*

### Comparing `nextnanopy-0.1.7/nextnanopy/nnp/assistants.py` & `nextnanopy-0.1.9/nextnanopy/nnp/assistants.py`

 * *Files identical despite different names*

### Comparing `nextnanopy-0.1.7/nextnanopy/nnp/defaults.py` & `nextnanopy-0.1.9/nextnanopy/nnp/defaults.py`

 * *Files identical despite different names*

### Comparing `nextnanopy-0.1.7/nextnanopy/nnp/inputs.py` & `nextnanopy-0.1.9/nextnanopy/nnp/inputs.py`

 * *Files identical despite different names*

### Comparing `nextnanopy-0.1.7/nextnanopy/nnp/outputs.py` & `nextnanopy-0.1.9/nextnanopy/nnp/outputs.py`

 * *Files identical despite different names*

### Comparing `nextnanopy-0.1.7/nextnanopy/nnp/shapes.py` & `nextnanopy-0.1.9/nextnanopy/nnp/shapes.py`

 * *Files identical despite different names*

### Comparing `nextnanopy-0.1.7/nextnanopy/outputs.py` & `nextnanopy-0.1.9/nextnanopy/outputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 import os
 from itertools import islice
 import numpy as np
 
 from nextnanopy.utils.datasets import Variable, Coord
 from nextnanopy.utils.mycollections import DictList
 from nextnanopy.utils.formatting import best_str_to_name_unit
-from nextnanopy.utils.misc import savetxt, get_filename, get_folder, get_file_extension
+from nextnanopy.utils.misc import get_filename, message_decorator
 from nextnanopy import defaults
 
 import pyvista as pv
 
-
-def load_message(method):
-    def f(*args, **kwargs):
-        # print('Loading...')
-        result = method(*args, **kwargs)
-        # print('Done!')
-
-    return f
+_msgs = defaults.messages['load_output']
+load_message = lambda method: message_decorator(method, init_msg=_msgs[0], end_msg=_msgs[1])
 
 
 class Output(object):
 
     def __init__(self, fullpath):
         self.fullpath = fullpath
         self.metadata = {}
```

### Comparing `nextnanopy-0.1.7/nextnanopy/shapes.py` & `nextnanopy-0.1.9/nextnanopy/shapes.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,16 +90,14 @@
             fig, ax = plt.subplots(1)
         if cmap:
             colormap = plt.get_cmap(cmap)
             colors = [colormap(i) for i in np.linspace(0, 1, self.nb_polygons)]
             ax.set_prop_cycle(cycler('color', colors))
         ax.set_xlabel(f'x {self.unit}')
         ax.set_ylabel(f'y {self.unit}')
-        ax.figure.tight_layout()
-        plt.show()
         return ax
 
     def show_all(self, ax=None, cmap='nipy_spectral', fill_kw={}):
         ax = self._prepare_ax(ax, cmap)
         for xy, label in zip(self.xy, self.labels):
             x, y = xy
             ax.fill(x, y, label=label, **fill_kw)
@@ -123,24 +121,22 @@
         return ax
 
     def show(self, ax=None, cmap='nipy_spectral', fill_kw={}, onebyone=False):
         if onebyone:
             ax = self.show_onebyone(ax, cmap, fill_kw)
         else:
             ax = self.show_all(ax, cmap, fill_kw)
-        ax.figure.tight_layout()
         return ax
 
     def show_slices(self, ax=None, fill_kw={}):
         ax = self._prepare_ax(ax, cmap=None)
         for spol in self.slices:
             for pol in spol.slices:
                 x, y = pol.boundary.xy
                 ax.fill(x, y, **fill_kw)
-        ax.figure.tight_layout()
         return ax
 
 
 class SlicedPolygon(shapely.geometry.Polygon):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._slices = []
@@ -299,19 +295,15 @@
             y = p_follow
         elif self.slice_axis == 'y':
             y = p_sorted
             x = p_follow
         return x, y
 
     def show_slices(self, ax=None, fill_kw={}):
-        plt.ion()
         if not ax:
             fig, ax = plt.subplots(1)
         ax.set_xlabel(f'x')
         ax.set_ylabel(f'y')
-        ax.figure.tight_layout()
-        plt.show()
         for pol in self.slices:
             x, y = pol.boundary.xy
             ax.fill(x, y, **fill_kw)
-        ax.figure.tight_layout()
         return ax
```

### Comparing `nextnanopy-0.1.7/nextnanopy/utils/config.py` & `nextnanopy-0.1.9/nextnanopy/utils/config.py`

 * *Files identical despite different names*

### Comparing `nextnanopy-0.1.7/nextnanopy/utils/datasets.py` & `nextnanopy-0.1.9/nextnanopy/utils/datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from copy import deepcopy
 import numpy as np
 
-default_unit = 'a.u'
+default_unit = 'a.u.'
 
 
 class Data(object):
     """
     This class stores any kind of information from nextnano files (input files, data files).
     This is a template class for datasets like Variables, Coords, InputVariables, etc.
```

### Comparing `nextnanopy-0.1.7/nextnanopy/utils/formatting.py` & `nextnanopy-0.1.9/nextnanopy/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `nextnanopy-0.1.7/nextnanopy/utils/misc.py` & `nextnanopy-0.1.9/nextnanopy/utils/misc.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,29 +46,29 @@
 
 
 def find_unused_name(name, list_names, extension, max_idx=True):
     if extension[0] != '.':
         extension = f'.{extension}'
     if extension not in name:
         name += extension
-    only_name = get_file_prefix(name)
-    lnames = list(filter(lambda ln: extension in ln and only_name in ln, list_names))
+    prefix = get_file_prefix(name)
+    lnames = list(filter(lambda ln: extension in ln and prefix in ln, list_names))
+
     if len(lnames) == 0:
         max_idx = 0
     if max_idx:
         idxs = [get_file_idx(name) for name in lnames]
         idxs.sort()
         max_idx = idxs[-1]
-        idx = max_idx + 1
-        unused_name = f'{only_name}_{max_idx + 1}{extension}'
+        unused_name = f'{prefix}_{max_idx + 1}{extension}'
     else:
         idx = 0
-        unused_name = f'{only_name}_{idx}{extension}'
+        unused_name = f'{prefix}_{idx}{extension}'
         while unused_name in list_names:
-            unused_name = f'{only_name}_{idx}{extension}'
+            unused_name = f'{prefix}_{idx}{extension}'
             idx += 1
     return unused_name
 
 
 def find_unused_in_folder(fullpath, overwrite=False):
     folder, name = os.path.split(fullpath)
     ext = get_file_extension(name)
@@ -79,31 +79,50 @@
 
 
 def savetxt(fullpath, text, overwrite=False, automkdir=True):
     if automkdir:
         mkdir_if_not_exist(get_folder(fullpath))
     fullpath = find_unused_in_folder(fullpath, overwrite)
     with open(fullpath, 'w+') as file:
-        print(f'Saving {fullpath}...')
         file.write(text)
-    print('Done!')
     return fullpath
 
 
 def get_file_prefix(file):
     prefix, ext = os.path.splitext(file)
     idx = get_file_idx(prefix)
     if idx > -1:
-        prefix = prefix.split(f'_{idx}')[0]
+        prefix = '_'.join(prefix.split('_')[0:-1])
     return prefix
 
 
 def get_file_idx(file):
     prefix, ext = os.path.splitext(file)
     idx = -1
     if '_' in prefix:
         end = prefix.split('_')[-1]
         try:
             idx = int(end)
         except:
             pass
     return idx
+
+
+def message_decorator(method, init_msg=None, end_msg=None):
+    def f(*args, **kwargs):
+        show_message(init_msg)
+        result = method(*args, **kwargs)
+        show_message(end_msg)
+        return result
+
+    return f
+
+
+def show_message(msg):
+    if msg is None:
+        return
+    if type(msg) == str:
+        print(msg)
+    elif callable(msg):
+        msg()
+    else:
+        pass
```

### Comparing `nextnanopy-0.1.7/nextnanopy/utils/mycollections.py` & `nextnanopy-0.1.9/nextnanopy/utils/mycollections.py`

 * *Files identical despite different names*

### Comparing `nextnanopy-0.1.7/nextnanopy.egg-info/PKG-INFO` & `nextnanopy-0.1.9/nextnanopy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,97 +1,103 @@
 Metadata-Version: 2.1
 Name: nextnanopy
-Version: 0.1.7
+Version: 0.1.9
 Summary: Useful tools to interface the nextnano software (https://www.nextnano.com/)
 Home-page: https://github.com/nextnanopy/nextnanopy
 Author: nextnano GmbH
 Author-email: python@nextnano.com
 License: BSD-3-Clause
 Description: # NEXTNANOPY README
         
         [![BSD-3-Clause](https://img.shields.io/github/license/nextnanopy/nextnanopy)](https://opensource.org/licenses/BSD-3-Clause)
         [![Downloads](https://img.shields.io/github/downloads/nextnanopy/nextnanopy/total)](https://github.com/nextnanopy/nextnanopy/releases)
         
         nextnanopy is a Python module to interface the [nextnano](https://www.nextnano.com/) software. This package includes features for:
-        * **Output files**: user-friendly method to load the datafiles which allows easy and flexible post-processing. 
-        * **Input files:** load input files, set variables, save by finding unused name, execute the file, write input files, etc.
-        * **Configuration**: setup default nextnano configuration (path to executables, databases, licenses, etc).
-        * **Import from GDS files**: load polygons from GDS files and user-friendly methods to generate raw text of nextnano shapes (beta).
+        * **Output files**: User-friendly method to load the datafiles which allows easy and flexible post-processing. 
+        * **Input files:** Load input files, set variables, save by finding unused name, execute the file, write input files, etc.
+        * **Configuration**: Setup default nextnano configuration (path to executables, databases, licenses, etc).
+        * **Import from GDS files**: Load polygons from GDS files and user-friendly methods to generate raw text of nextnano shapes (beta).
         
-        **Note:** the license is not compulsory for the general use of nextnanopy, unless you would like to execute input files via Python.
+        **Note:** A valid license for the nextnano software is not compulsory for the general use of nextnanopy, unless you would like to execute input files via Python.
         
         ## Future of nextnanopy
-        Currently, nextnanopy has basic features for [nextnano products](https://www.nextnano.com/products/products.php) nextnano++, nextnano3, nextnano.NEGF and nextnano/MSB. The goal is to extend the functionalities to nextnano.MSB in future releases.
+        Currently, nextnanopy has basic features for [nextnano products](https://www.nextnano.com/products/products.php) nextnano++, nextnanoÂ³, nextnano.NEGF and nextnano.MSB.
         
         In future releases, we would like to implement:
         
-        * **Common post-processing methods**: like loading and plotting together bandedges, eigenenergies and eigenlevels, colormap of potential landscape with GDS polygons on top, etc.
-        * **Support for any nextnano.NEGF datafiles**: in the current release, it is only implemented the loading of .dat files (most of them).
-        * **Support for any nextnano.MSB datafiles**: not loading routines are implemented yet.
-        * **User-friendly input file creation/modification**: the idea is to load any input file and it would detect all the different blocks so the user can easily modify parameters like 'boundary conditions' or 'region material'. Similarly, it should be user-friendly to create any input file from scratch via Python.
-        * **Feedback loops**: a routine that allows the user to optimize any figure of merit of a device with a given set of input variables. The user can set a post-processing routine to get the figure of merit from the simulated data and later, a new set of input variables will be generated and executed. This feedback loop will repeat until a set of conditions are satisfied.
-        * **Improve documentation**: we will add an extensive documentation in the website as well as in the source code.
-        * **Guidelines for contributors**: set of rules if you want to contribute to the project.
+        * **Common post-processing methods**: Like loading and plotting together bandedges, eigenenergies and eigenlevels, colormap of potential landscape with GDS polygons on top, etc.
+        * **Improved support for specific nextnano.NEGF and nextnano.MSB datafiles**
+        * **User-friendly input file creation/modification**: The idea is to load any input file and it would detect all the different blocks so the user can easily modify parameters like 'boundary conditions' or 'region material'. Similarly, it should be user-friendly to create any input file from scratch via Python.
+        * **Feedback loops**: A routine that allows the user to optimize any figure of merit of a device with a given set of input variables. The user can set a post-processing routine to get the figure of merit from the simulated data and later, a new set of input variables will be generated and executed. This feedback loop will repeat until a set of conditions are satisfied.
+        * **Improve documentation**: We will add an extensive documentation in the website as well as in the source code.
+        * **Guidelines for contributors**: Set of rules if you want to contribute to the project.
          
         ## Installation
         
         ### Requirements
         
-        You need a working python 3.x installation to be able to use nextnanopy. We highly recommend installing [Anaconda](https://www.anaconda.com/), which takes care of installing Python and managing packages. 
-        Make sure to download the latest version with python 3.8.
+        You need a working Python 3.8 installation to be able to use nextnanopy. We highly recommend installing [Anaconda](https://www.anaconda.com/), which takes care of installing Python and managing packages. 
+        Make sure to download the latest version with Python 3.8.
         
         ### Dependencies:
         
         * [Python](https://www.python.org/) (tested with 3.8)
-        * [Numpy](http://numpy.scipy.org/)
+        * [NumPy](http://numpy.scipy.org/)
         * [PyVista](https://www.pyvista.org/) (For loading VTK files)
         * [Gdspy](https://gdspy.readthedocs.io/) (optional: to import gds files)
         * [Shapely](https://shapely.readthedocs.io/) (optional: to manipulate polygons from gds files)
         * [Matplotlib](https://matplotlib.org/) (optional: to visualize imported polygons)
-        * [Cylcer](https://pypi.org/project/Cycler/) (optional: to visualize imported polygons)
+        * [Cycler](https://pypi.org/project/Cycler/) (optional: to visualize imported polygons)
         
         ### Linux / OS X / Windows
         
         #### Option 1: Using [pip](https://docs.python.org/3/installing/)
         
-        Simply open anaconda prompt and type:
+        Simply open Anaconda prompt and type:
         
         ```sh
         pip install nextnanopy
         ```
         or if you want to upgrade:
         ```sh
         pip install --upgrade nextnanopy
         ```
         
-        #### Option 2: from the source code
+        #### Option 2: From the source code
         
         1. Download the source from [github](https://github.com/nextnanopy/nextnanopy)
-        2. Open anaconda prompt
+        2. Open Anaconda prompt
         3. Go to the directory of the nextnanopy project
         4. Build/install by typing:
         
         ```sh
         python setup.py install
         ```
         
-        For more information, please, see the documents in docs folder.
+        For more information, please see the documents in docs/ folder.
         
         ## Documentation
         
-        Currently, the complete documentation is not available yet. However, there are few examples located in docs/examples that will help you to start playing with nextnanopy.
+        Currently, the complete documentation is not available yet. However, there are few examples located in templates/ and docs/examples that will help you to start playing with nextnanopy.
         
         
         ## Support
         
         Do you want to help nextnanopy? Please, send an email to [python@nextnano.com](mailto:python@nextnano.com). 
         
         
         ## History of changes
         
+        ### Version 0.1.9 (Dec 14th, 2020)
+        * Feature: InputFile.execute has now show_log (True or False) to turn on/off the log. Note: the log file is always saved. 
+        * Removed default messages when saving an input file
+        
+        ### Version 0.1.8 (Dec 14th, 2020)
+        * Buf fix: find unused name when saving input file
+        
         ### Version 0.1.7 (Dec 3rd, 2020)
         * docstring for inputs.py, outputs.py, config.py, mycollections.py, datasets.py
         * Updated examples in docs/examples/
         
         ### Version 0.1.6 (Dec 2nd, 2020)
         * Feature: [DataFile] access with index to coordinates and to variables
         ```python
@@ -106,41 +112,41 @@
         df['xmax'] # same as df.variables['xmax']
         ```
         * Feature: [InputFile] is loopable as well as .coords and .variables
         * Feature: [InputFile] extra attributes
         ```python
         df = nextnanopy.InputFile(...)
         df.folder_output # returns the output folder if it was executed, otherwise it raises an error
-        df.filename # settable
+        df.filename      # settable
         df.filename_only # settable
-        df.folder_input # settable
+        df.folder_input  # settable
         ```
-        * Feature: user-friendly information for DataFile, InputFile, Variable, Coord and InputVariable.
+        * Feature: User-friendly information for DataFile, InputFile, Variable, Coord and InputVariable
         * Bug fix: .vtr dataset reshape method
         
         ### Version 0.1.5 (Dec 2nd, 2020)
-        * Feature: support .vtr data files
-        * Feature: if unit is not found, default value is 'a.u'
-        * Bug fix: better methods to find correctly name and unit from data file headers
+        * Feature: Support of .vtr data files
+        * Feature: If unit is not found, default value is 'a.u.'.
+        * Bug fix: Better methods to find correctly name and unit from data file headers
         
         ### Version 0.1.4 (Nov 29th, 2020)
-        * Feature: create an empty input file and set the raw text with the attribute text.
+        * Feature: Create an empty input file and set the raw text with the attribute text.
         
         ### Version 0.1.3 (Nov 28th, 2020)
-        * Bug fix: find unused name when save input files
-        * Feature: default label for Variables and Coords. The attribute label returns "name (unit)". 
+        * Bug fix: Find unused name when save input files.
+        * Feature: Default label for Variables and Coords. The attribute label returns "name (unit)". 
         
         ### Version 0.1.2 (Nov 20th, 2020)
-        * Bug fix: Raw text of input variables without comment was generated incorrectly
+        * Bug fix: Raw text of input variables without comment was generated incorrectly.
         
         ### Version 0.1.1 (Nov 18th, 2020)
-        * Bug fix: find the home path for OSX and Linux. 
+        * Bug fix: Find the home path for OSX and Linux.
         
         ### Version 0.1.0 (Nov 13th, 2020)
-        * Initial release.
+        * Initial release
         
 Keywords: nextnano
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Customer Service
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nextnanopy-0.1.7/nextnanopy.egg-info/SOURCES.txt` & `nextnanopy-0.1.9/nextnanopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nextnanopy-0.1.7/setup.py` & `nextnanopy-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 install_requires = [
     'numpy>=1.18',
     'pyvista>=0.27',
 ]
 
 setuptools.setup(
     name="nextnanopy",
-    version="0.1.7",
+    version="0.1.9",
     author="nextnano GmbH",
     author_email="python@nextnano.com",
     license='BSD-3-Clause',
     description="Useful tools to interface the nextnano software (https://www.nextnano.com/)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="nextnano",
```

