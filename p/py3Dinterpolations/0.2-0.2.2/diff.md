# Comparing `tmp/py3Dinterpolations-0.2.tar.gz` & `tmp/py3Dinterpolations-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3Dinterpolations-0.2.tar", last modified: Sat Jun 24 18:52:51 2023, max compression
+gzip compressed data, was "py3Dinterpolations-0.2.2.tar", last modified: Fri Jul 21 10:41:44 2023, max compression
```

## Comparing `py3Dinterpolations-0.2.tar` & `py3Dinterpolations-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:52:51.236297 py3Dinterpolations-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-24 18:52:41.000000 py3Dinterpolations-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-24 18:52:51.236297 py3Dinterpolations-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-24 18:52:41.000000 py3Dinterpolations-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:52:51.236297 py3Dinterpolations-0.2/py3Dinterpolations/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-24 18:52:41.000000 py3Dinterpolations-0.2/py3Dinterpolations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:52:51.236297 py3Dinterpolations-0.2/py3Dinterpolations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-24 18:52:51.000000 py3Dinterpolations-0.2/py3Dinterpolations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-24 18:52:51.000000 py3Dinterpolations-0.2/py3Dinterpolations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 18:52:51.000000 py3Dinterpolations-0.2/py3Dinterpolations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-24 18:52:51.000000 py3Dinterpolations-0.2/py3Dinterpolations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-24 18:52:51.000000 py3Dinterpolations-0.2/py3Dinterpolations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 18:52:51.236297 py3Dinterpolations-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-24 18:52:41.000000 py3Dinterpolations-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:41:44.926471 py3Dinterpolations-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-21 10:41:33.000000 py3Dinterpolations-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-21 10:41:44.926471 py3Dinterpolations-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-21 10:41:33.000000 py3Dinterpolations-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:41:44.926471 py3Dinterpolations-0.2.2/py3Dinterpolations/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-21 10:41:33.000000 py3Dinterpolations-0.2.2/py3Dinterpolations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:41:44.926471 py3Dinterpolations-0.2.2/py3Dinterpolations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-21 10:41:44.000000 py3Dinterpolations-0.2.2/py3Dinterpolations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-21 10:41:44.000000 py3Dinterpolations-0.2.2/py3Dinterpolations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:41:44.000000 py3Dinterpolations-0.2.2/py3Dinterpolations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-21 10:41:44.000000 py3Dinterpolations-0.2.2/py3Dinterpolations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 10:41:44.000000 py3Dinterpolations-0.2.2/py3Dinterpolations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 10:41:44.926471 py3Dinterpolations-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-21 10:41:33.000000 py3Dinterpolations-0.2.2/setup.py
```

### Comparing `py3Dinterpolations-0.2/LICENSE` & `py3Dinterpolations-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py3Dinterpolations-0.2/PKG-INFO` & `py3Dinterpolations-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: py3Dinterpolations
-Version: 0.2
+Version: 0.2.2
 Summary: quick 3D interpolation with python
 Home-page: https://github.com/giocaizzi/py3Dinterpolations
 Author: giocaizzi
 Author-email: giocaizzi@gmail.com
 License: MIT
+Project-URL: Documentation, https://giocaizzi.github.io/py3Dinterpolations/
 Project-URL: Bug Reports, https://github.com/giocaizzi/py3Dinterpolations/issues
 Project-URL: Source, https://github.com/giocaizzi/py3Dinterpolations
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -20,21 +21,23 @@
 
 # py3Dinterpolations
 
 |  |  |
 | --- | --- |
 | Distribution | ![PyPI](https://img.shields.io/pypi/v/py3Dinterpolations?color=blue) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py3Dinterpolations) |
 | Testing | [![Tests](https://github.com/giocaizzi/py3Dinterpolations/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/giocaizzi/py3Dinterpolations/actions/workflows/tests.yml) [![codecov](https://codecov.io/gh/giocaizzi/py3Dinterpolations/branch/main/graph/badge.svg?token=8COIITUR2I)](https://codecov.io/gh/giocaizzi/py3Dinterpolations) |
+|Code style|![Black](https://img.shields.io/badge/code%20style-black-black) [![Flake8 Linting](https://github.com/giocaizzi/py3Dinterpolations/actions/workflows/linting.yml/badge.svg?branch=main)](https://github.com/giocaizzi/py3Dinterpolations/actions/workflows/linting.yml)|
 | Documentation | [![Documentation](https://github.com/giocaizzi/py3Dinterpolations/actions/workflows/documentation.yml/badge.svg?branch=gh-pages)](https://github.com/giocaizzi/py3Dinterpolations/actions/workflows/documentation.yml) |
 
 
 This is a python package to compute **quick 3D interpolations of spatial data**.
 
 Supports the **following interpolation** methods:
 - *Ordinary 3D Kriging* : [`pykrige`](https://github.com/GeoStat-Framework/PyKrige)
+- *Inverse Distance Weighting (IDW)*
 
 Supports **preprocessing** of data:
 - *Downsampling*
 - *Normalization* of X,Y,Z coordinates
 - *Standardization* of signal 
 
 **Visualizations**
```

### Comparing `py3Dinterpolations-0.2/README.md` & `py3Dinterpolations-0.2.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # py3Dinterpolations
 
 |  |  |
 | --- | --- |
 | Distribution | ![PyPI](https://img.shields.io/pypi/v/py3Dinterpolations?color=blue) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py3Dinterpolations) |
 | Testing | [![Tests](https://github.com/giocaizzi/py3Dinterpolations/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/giocaizzi/py3Dinterpolations/actions/workflows/tests.yml) [![codecov](https://codecov.io/gh/giocaizzi/py3Dinterpolations/branch/main/graph/badge.svg?token=8COIITUR2I)](https://codecov.io/gh/giocaizzi/py3Dinterpolations) |
+|Code style|![Black](https://img.shields.io/badge/code%20style-black-black) [![Flake8 Linting](https://github.com/giocaizzi/py3Dinterpolations/actions/workflows/linting.yml/badge.svg?branch=main)](https://github.com/giocaizzi/py3Dinterpolations/actions/workflows/linting.yml)|
 | Documentation | [![Documentation](https://github.com/giocaizzi/py3Dinterpolations/actions/workflows/documentation.yml/badge.svg?branch=gh-pages)](https://github.com/giocaizzi/py3Dinterpolations/actions/workflows/documentation.yml) |
 
 
 This is a python package to compute **quick 3D interpolations of spatial data**.
 
 Supports the **following interpolation** methods:
 - *Ordinary 3D Kriging* : [`pykrige`](https://github.com/GeoStat-Framework/PyKrige)
+- *Inverse Distance Weighting (IDW)*
 
 Supports **preprocessing** of data:
 - *Downsampling*
 - *Normalization* of X,Y,Z coordinates
 - *Standardization* of signal 
 
 **Visualizations**
```

### Comparing `py3Dinterpolations-0.2/py3Dinterpolations.egg-info/PKG-INFO` & `py3Dinterpolations-0.2.2/py3Dinterpolations.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: py3Dinterpolations
-Version: 0.2
+Version: 0.2.2
 Summary: quick 3D interpolation with python
 Home-page: https://github.com/giocaizzi/py3Dinterpolations
 Author: giocaizzi
 Author-email: giocaizzi@gmail.com
 License: MIT
+Project-URL: Documentation, https://giocaizzi.github.io/py3Dinterpolations/
 Project-URL: Bug Reports, https://github.com/giocaizzi/py3Dinterpolations/issues
 Project-URL: Source, https://github.com/giocaizzi/py3Dinterpolations
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -20,21 +21,23 @@
 
 # py3Dinterpolations
 
 |  |  |
 | --- | --- |
 | Distribution | ![PyPI](https://img.shields.io/pypi/v/py3Dinterpolations?color=blue) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py3Dinterpolations) |
 | Testing | [![Tests](https://github.com/giocaizzi/py3Dinterpolations/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/giocaizzi/py3Dinterpolations/actions/workflows/tests.yml) [![codecov](https://codecov.io/gh/giocaizzi/py3Dinterpolations/branch/main/graph/badge.svg?token=8COIITUR2I)](https://codecov.io/gh/giocaizzi/py3Dinterpolations) |
+|Code style|![Black](https://img.shields.io/badge/code%20style-black-black) [![Flake8 Linting](https://github.com/giocaizzi/py3Dinterpolations/actions/workflows/linting.yml/badge.svg?branch=main)](https://github.com/giocaizzi/py3Dinterpolations/actions/workflows/linting.yml)|
 | Documentation | [![Documentation](https://github.com/giocaizzi/py3Dinterpolations/actions/workflows/documentation.yml/badge.svg?branch=gh-pages)](https://github.com/giocaizzi/py3Dinterpolations/actions/workflows/documentation.yml) |
 
 
 This is a python package to compute **quick 3D interpolations of spatial data**.
 
 Supports the **following interpolation** methods:
 - *Ordinary 3D Kriging* : [`pykrige`](https://github.com/GeoStat-Framework/PyKrige)
+- *Inverse Distance Weighting (IDW)*
 
 Supports **preprocessing** of data:
 - *Downsampling*
 - *Normalization* of X,Y,Z coordinates
 - *Standardization* of signal 
 
 **Visualizations**
```

### Comparing `py3Dinterpolations-0.2/setup.py` & `py3Dinterpolations-0.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="py3Dinterpolations",
-    version="0.2",
+    version="0.2.2",
     description="quick 3D interpolation with python",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://github.com/giocaizzi/py3Dinterpolations",
     author="giocaizzi",
     author_email="giocaizzi@gmail.com",
     license="MIT",
@@ -34,12 +34,12 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     project_urls={
-        # "Documentation": "https://giocaizzi.github.io/py3Dinterpolations/",
+        "Documentation": "https://giocaizzi.github.io/py3Dinterpolations/",
         "Bug Reports": "https://github.com/giocaizzi/py3Dinterpolations/issues",
         "Source": "https://github.com/giocaizzi/py3Dinterpolations",
     },
 )
```

