# Comparing `tmp/bokehmol-0.1.0a1.tar.gz` & `tmp/bokehmol-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bokehmol-0.1.0a1.tar", last modified: Thu Jul 20 22:39:01 2023, max compression
+gzip compressed data, was "bokehmol-0.1.0a2.tar", last modified: Thu Jul 20 23:11:00 2023, max compression
```

## Comparing `bokehmol-0.1.0a1.tar` & `bokehmol-0.1.0a2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:39:01.767846 bokehmol-0.1.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-07-20 22:38:44.000000 bokehmol-0.1.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-20 22:38:44.000000 bokehmol-0.1.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-07-20 22:39:01.767846 bokehmol-0.1.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-20 22:38:44.000000 bokehmol-0.1.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:39:01.767846 bokehmol-0.1.0a1/bokehmol/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-20 22:38:44.000000 bokehmol-0.1.0a1/bokehmol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 22:38:44.000000 bokehmol-0.1.0a1/bokehmol/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-20 22:38:44.000000 bokehmol-0.1.0a1/bokehmol/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-20 22:38:44.000000 bokehmol-0.1.0a1/bokehmol/hover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:39:01.767846 bokehmol-0.1.0a1/bokehmol/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:38:44.000000 bokehmol-0.1.0a1/bokehmol/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-20 22:38:44.000000 bokehmol-0.1.0a1/bokehmol/models/base_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-20 22:38:44.000000 bokehmol-0.1.0a1/bokehmol/models/base_hover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-20 22:38:44.000000 bokehmol-0.1.0a1/bokehmol/models/rdkit_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-20 22:38:44.000000 bokehmol-0.1.0a1/bokehmol/models/rdkit_hover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-20 22:38:44.000000 bokehmol-0.1.0a1/bokehmol/models/smilesdrawer_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-20 22:38:44.000000 bokehmol-0.1.0a1/bokehmol/models/smilesdrawer_hover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-20 22:38:44.000000 bokehmol-0.1.0a1/bokehmol/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:39:01.767846 bokehmol-0.1.0a1/bokehmol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-07-20 22:39:01.000000 bokehmol-0.1.0a1/bokehmol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-20 22:39:01.000000 bokehmol-0.1.0a1/bokehmol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 22:39:01.000000 bokehmol-0.1.0a1/bokehmol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 22:39:01.000000 bokehmol-0.1.0a1/bokehmol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 22:39:01.000000 bokehmol-0.1.0a1/bokehmol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-20 22:38:44.000000 bokehmol-0.1.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 22:39:01.767846 bokehmol-0.1.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 22:38:44.000000 bokehmol-0.1.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:11:00.954417 bokehmol-0.1.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14558 2023-07-20 23:11:00.954417 bokehmol-0.1.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:11:00.950417 bokehmol-0.1.0a2/bokehmol/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/hover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:11:00.954417 bokehmol-0.1.0a2/bokehmol/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/models/base_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/models/base_hover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/models/rdkit_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/models/rdkit_hover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/models/smilesdrawer_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/models/smilesdrawer_hover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/bokehmol/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:11:00.950417 bokehmol-0.1.0a2/bokehmol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14558 2023-07-20 23:11:00.000000 bokehmol-0.1.0a2/bokehmol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-20 23:11:00.000000 bokehmol-0.1.0a2/bokehmol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 23:11:00.000000 bokehmol-0.1.0a2/bokehmol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 23:11:00.000000 bokehmol-0.1.0a2/bokehmol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 23:11:00.000000 bokehmol-0.1.0a2/bokehmol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 23:11:00.954417 bokehmol-0.1.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 23:10:44.000000 bokehmol-0.1.0a2/setup.py
```

### Comparing `bokehmol-0.1.0a1/LICENSE` & `bokehmol-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `bokehmol-0.1.0a1/PKG-INFO` & `bokehmol-0.1.0a2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bokehmol
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Tools for plotting molecules in Bokeh
 Author-email: Cédric Bouysset <cedric@bouysset.net>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -177,15 +177,15 @@
               defend, and hold each Contributor harmless for any liability
               incurred by, or claims asserted against, such Contributor by reason
               of your accepting any such warranty or additional liability.
         
            END OF TERMS AND CONDITIONS
         
 Project-URL: Homepage, https://github.com/cbouy/bokehmol
-Project-URL: Documentation, https://bokehmol.readthedocs.io/en/stable/
+Project-URL: Documentation, https://nbviewer.org/github/cbouy/bokehmol/blob/master/notebooks/quickstart.ipynb
 Project-URL: Discussions, https://github.com/cbouy/bokehmol/discussions
 Project-URL: Issues, https://github.com/cbouy/bokehmol/issues
 Project-URL: Changelog, https://github.com/cbouy/bokehmol/blob/master/CHANGELOG.md
 Keywords: science,chemistry,drug-design,cheminformatics,chemoinformatics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
@@ -194,7 +194,37 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# bokehmol, gotta plot them mol! ⌬
+
+[![Powered by RDKit.js](https://img.shields.io/badge/Powered%20by-RDKit.js-3838ff.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQBAMAAADt3eJSAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAFVBMVEXc3NwUFP8UPP9kZP+MjP+0tP////9ZXZotAAAAAXRSTlMAQObYZgAAAAFiS0dEBmFmuH0AAAAHdElNRQfmAwsPGi+MyC9RAAAAQElEQVQI12NgQABGQUEBMENISUkRLKBsbGwEEhIyBgJFsICLC0iIUdnExcUZwnANQWfApKCK4doRBsKtQFgKAQC5Ww1JEHSEkAAAACV0RVh0ZGF0ZTpjcmVhdGUAMjAyMi0wMy0xMVQxNToyNjo0NyswMDowMDzr2J4AAAAldEVYdGRhdGU6bW9kaWZ5ADIwMjItMDMtMTFUMTU6MjY6NDcrMDA6MDBNtmAiAAAAAElFTkSuQmCC)](https://www.rdkit.org/)
+
+**bokehmol** provides custom extensions that help plotting molecules with the
+[Bokeh](https://docs.bokeh.org/) library.
+
+It currently provides hover tools that can depict molecules **on-the-fly** using SMILES: no need to
+pre-generate the depictions and store them in memory anymore! Everything is rendered client-side in
+the browser so you don't even need to install rdkit in your Python environment.
+
+## [Installation](https://pypi.org/project/bokehmol/)
+
+Bokehmol only requires bokeh as a dependency. You can install it with:
+```
+pip install bokehmol
+```
+
+## [Notebooks](https://github.com/cbouy/bokehmol/tree/master/notebooks)
+
+Some examples on how to use the library [![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.org/github/cbouy/bokehmol/blob/master/notebooks/quickstart.ipynb)
+
+## [Discussions](https://github.com/cbouy/bokehmol/discussions)
+
+Feature requests or questions on how to use should be posted [here](https://github.com/cbouy/bokehmol/discussions)
+
+## [Issues](https://github.com/cbouy/bokehmol/issues)
+
+Bug [tracker](https://github.com/cbouy/bokehmol/issues) 🐞
```

### Comparing `bokehmol-0.1.0a1/README.md` & `bokehmol-0.1.0a2/README.md`

 * *Files identical despite different names*

### Comparing `bokehmol-0.1.0a1/bokehmol/config.py` & `bokehmol-0.1.0a2/bokehmol/config.py`

 * *Files identical despite different names*

### Comparing `bokehmol-0.1.0a1/bokehmol/hover.py` & `bokehmol-0.1.0a2/bokehmol/hover.py`

 * *Files identical despite different names*

### Comparing `bokehmol-0.1.0a1/bokehmol/models/rdkit_formatter.py` & `bokehmol-0.1.0a2/bokehmol/models/rdkit_formatter.py`

 * *Files identical despite different names*

### Comparing `bokehmol-0.1.0a1/bokehmol/models/smilesdrawer_formatter.py` & `bokehmol-0.1.0a2/bokehmol/models/smilesdrawer_formatter.py`

 * *Files identical despite different names*

### Comparing `bokehmol-0.1.0a1/bokehmol/utils.py` & `bokehmol-0.1.0a2/bokehmol/utils.py`

 * *Files identical despite different names*

### Comparing `bokehmol-0.1.0a1/bokehmol.egg-info/PKG-INFO` & `bokehmol-0.1.0a2/bokehmol.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bokehmol
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Tools for plotting molecules in Bokeh
 Author-email: Cédric Bouysset <cedric@bouysset.net>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -177,15 +177,15 @@
               defend, and hold each Contributor harmless for any liability
               incurred by, or claims asserted against, such Contributor by reason
               of your accepting any such warranty or additional liability.
         
            END OF TERMS AND CONDITIONS
         
 Project-URL: Homepage, https://github.com/cbouy/bokehmol
-Project-URL: Documentation, https://bokehmol.readthedocs.io/en/stable/
+Project-URL: Documentation, https://nbviewer.org/github/cbouy/bokehmol/blob/master/notebooks/quickstart.ipynb
 Project-URL: Discussions, https://github.com/cbouy/bokehmol/discussions
 Project-URL: Issues, https://github.com/cbouy/bokehmol/issues
 Project-URL: Changelog, https://github.com/cbouy/bokehmol/blob/master/CHANGELOG.md
 Keywords: science,chemistry,drug-design,cheminformatics,chemoinformatics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
@@ -194,7 +194,37 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# bokehmol, gotta plot them mol! ⌬
+
+[![Powered by RDKit.js](https://img.shields.io/badge/Powered%20by-RDKit.js-3838ff.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQBAMAAADt3eJSAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAFVBMVEXc3NwUFP8UPP9kZP+MjP+0tP////9ZXZotAAAAAXRSTlMAQObYZgAAAAFiS0dEBmFmuH0AAAAHdElNRQfmAwsPGi+MyC9RAAAAQElEQVQI12NgQABGQUEBMENISUkRLKBsbGwEEhIyBgJFsICLC0iIUdnExcUZwnANQWfApKCK4doRBsKtQFgKAQC5Ww1JEHSEkAAAACV0RVh0ZGF0ZTpjcmVhdGUAMjAyMi0wMy0xMVQxNToyNjo0NyswMDowMDzr2J4AAAAldEVYdGRhdGU6bW9kaWZ5ADIwMjItMDMtMTFUMTU6MjY6NDcrMDA6MDBNtmAiAAAAAElFTkSuQmCC)](https://www.rdkit.org/)
+
+**bokehmol** provides custom extensions that help plotting molecules with the
+[Bokeh](https://docs.bokeh.org/) library.
+
+It currently provides hover tools that can depict molecules **on-the-fly** using SMILES: no need to
+pre-generate the depictions and store them in memory anymore! Everything is rendered client-side in
+the browser so you don't even need to install rdkit in your Python environment.
+
+## [Installation](https://pypi.org/project/bokehmol/)
+
+Bokehmol only requires bokeh as a dependency. You can install it with:
+```
+pip install bokehmol
+```
+
+## [Notebooks](https://github.com/cbouy/bokehmol/tree/master/notebooks)
+
+Some examples on how to use the library [![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.org/github/cbouy/bokehmol/blob/master/notebooks/quickstart.ipynb)
+
+## [Discussions](https://github.com/cbouy/bokehmol/discussions)
+
+Feature requests or questions on how to use should be posted [here](https://github.com/cbouy/bokehmol/discussions)
+
+## [Issues](https://github.com/cbouy/bokehmol/issues)
+
+Bug [tracker](https://github.com/cbouy/bokehmol/issues) 🐞
```

### Comparing `bokehmol-0.1.0a1/bokehmol.egg-info/SOURCES.txt` & `bokehmol-0.1.0a2/bokehmol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bokehmol-0.1.0a1/pyproject.toml` & `bokehmol-0.1.0a2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "bokehmol"
 description = "Tools for plotting molecules in Bokeh"
 authors = [
   { name = "Cédric Bouysset", email = "cedric@bouysset.net" },
 ]
-readme = "README.MD"
+readme = "README.md"
 requires-python = ">=3.8"
 dynamic = ["version"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
@@ -30,15 +30,15 @@
 ]
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/cbouy/bokehmol"
-Documentation = "https://bokehmol.readthedocs.io/en/stable/"
+Documentation = "https://nbviewer.org/github/cbouy/bokehmol/blob/master/notebooks/quickstart.ipynb"
 Discussions = "https://github.com/cbouy/bokehmol/discussions"
 Issues = "https://github.com/cbouy/bokehmol/issues"
 Changelog = "https://github.com/cbouy/bokehmol/blob/master/CHANGELOG.md"
 
 [tool.setuptools]
 include-package-data = true
```

