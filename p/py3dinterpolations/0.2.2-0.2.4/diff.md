# Comparing `tmp/py3Dinterpolations-0.2.2.tar.gz` & `tmp/py3dinterpolations-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3Dinterpolations-0.2.2.tar", last modified: Fri Jul 21 10:41:44 2023, max compression
+gzip compressed data, was "py3dinterpolations-0.2.4.tar", last modified: Fri Jul 21 12:01:09 2023, max compression
```

## Comparing `py3Dinterpolations-0.2.2.tar` & `py3dinterpolations-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:41:44.926471 py3Dinterpolations-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-21 10:41:33.000000 py3Dinterpolations-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-21 10:41:44.926471 py3Dinterpolations-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-21 10:41:33.000000 py3Dinterpolations-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:41:44.926471 py3Dinterpolations-0.2.2/py3Dinterpolations/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-21 10:41:33.000000 py3Dinterpolations-0.2.2/py3Dinterpolations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:41:44.926471 py3Dinterpolations-0.2.2/py3Dinterpolations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-21 10:41:44.000000 py3Dinterpolations-0.2.2/py3Dinterpolations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-21 10:41:44.000000 py3Dinterpolations-0.2.2/py3Dinterpolations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:41:44.000000 py3Dinterpolations-0.2.2/py3Dinterpolations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-21 10:41:44.000000 py3Dinterpolations-0.2.2/py3Dinterpolations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 10:41:44.000000 py3Dinterpolations-0.2.2/py3Dinterpolations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 10:41:44.926471 py3Dinterpolations-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-21 10:41:33.000000 py3Dinterpolations-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:01:09.675067 py3dinterpolations-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-21 12:01:00.000000 py3dinterpolations-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-21 12:01:09.675067 py3dinterpolations-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-21 12:01:00.000000 py3dinterpolations-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:01:09.675067 py3dinterpolations-0.2.4/py3dinterpolations/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-21 12:01:00.000000 py3dinterpolations-0.2.4/py3dinterpolations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:01:09.675067 py3dinterpolations-0.2.4/py3dinterpolations/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-21 12:01:00.000000 py3dinterpolations-0.2.4/py3dinterpolations/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-21 12:01:00.000000 py3dinterpolations-0.2.4/py3dinterpolations/core/grid3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-21 12:01:00.000000 py3dinterpolations-0.2.4/py3dinterpolations/core/griddata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:01:09.675067 py3dinterpolations-0.2.4/py3dinterpolations/modelling/
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-21 12:01:00.000000 py3dinterpolations-0.2.4/py3dinterpolations/modelling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-21 12:01:00.000000 py3dinterpolations-0.2.4/py3dinterpolations/modelling/modeler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:01:09.675067 py3dinterpolations-0.2.4/py3dinterpolations/modelling/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-21 12:01:00.000000 py3dinterpolations-0.2.4/py3dinterpolations/modelling/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-21 12:01:00.000000 py3dinterpolations-0.2.4/py3dinterpolations/modelling/models/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-07-21 12:01:00.000000 py3dinterpolations-0.2.4/py3dinterpolations/modelling/models/idw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-07-21 12:01:00.000000 py3dinterpolations-0.2.4/py3dinterpolations/modelling/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:01:09.675067 py3dinterpolations-0.2.4/py3dinterpolations/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:01:00.000000 py3dinterpolations-0.2.4/py3dinterpolations/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-21 12:01:00.000000 py3dinterpolations-0.2.4/py3dinterpolations/plotting/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:01:09.675067 py3dinterpolations-0.2.4/py3dinterpolations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-21 12:01:09.000000 py3dinterpolations-0.2.4/py3dinterpolations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-21 12:01:09.000000 py3dinterpolations-0.2.4/py3dinterpolations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:01:09.000000 py3dinterpolations-0.2.4/py3dinterpolations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-21 12:01:09.000000 py3dinterpolations-0.2.4/py3dinterpolations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 12:01:09.000000 py3dinterpolations-0.2.4/py3dinterpolations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 12:01:09.675067 py3dinterpolations-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-21 12:01:00.000000 py3dinterpolations-0.2.4/setup.py
```

### Comparing `py3Dinterpolations-0.2.2/LICENSE` & `py3dinterpolations-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py3Dinterpolations-0.2.2/PKG-INFO` & `py3dinterpolations-0.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: py3Dinterpolations
-Version: 0.2.2
+Name: py3dinterpolations
+Version: 0.2.4
 Summary: quick 3D interpolation with python
-Home-page: https://github.com/giocaizzi/py3Dinterpolations
+Home-page: https://github.com/giocaizzi/py3dinterpolations
 Author: giocaizzi
 Author-email: giocaizzi@gmail.com
 License: MIT
-Project-URL: Documentation, https://giocaizzi.github.io/py3Dinterpolations/
-Project-URL: Bug Reports, https://github.com/giocaizzi/py3Dinterpolations/issues
-Project-URL: Source, https://github.com/giocaizzi/py3Dinterpolations
+Project-URL: Documentation, https://giocaizzi.github.io/py3dinterpolations/
+Project-URL: Bug Reports, https://github.com/giocaizzi/py3dinterpolations/issues
+Project-URL: Source, https://github.com/giocaizzi/py3dinterpolations
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: docs
```

### Comparing `py3Dinterpolations-0.2.2/README.md` & `py3dinterpolations-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `py3Dinterpolations-0.2.2/py3Dinterpolations.egg-info/PKG-INFO` & `py3dinterpolations-0.2.4/py3dinterpolations.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: py3Dinterpolations
-Version: 0.2.2
+Name: py3dinterpolations
+Version: 0.2.4
 Summary: quick 3D interpolation with python
-Home-page: https://github.com/giocaizzi/py3Dinterpolations
+Home-page: https://github.com/giocaizzi/py3dinterpolations
 Author: giocaizzi
 Author-email: giocaizzi@gmail.com
 License: MIT
-Project-URL: Documentation, https://giocaizzi.github.io/py3Dinterpolations/
-Project-URL: Bug Reports, https://github.com/giocaizzi/py3Dinterpolations/issues
-Project-URL: Source, https://github.com/giocaizzi/py3Dinterpolations
+Project-URL: Documentation, https://giocaizzi.github.io/py3dinterpolations/
+Project-URL: Bug Reports, https://github.com/giocaizzi/py3dinterpolations/issues
+Project-URL: Source, https://github.com/giocaizzi/py3dinterpolations
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: docs
```

### Comparing `py3Dinterpolations-0.2.2/setup.py` & `py3dinterpolations-0.2.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # read the contents of your README file
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
-    name="py3Dinterpolations",
-    version="0.2.2",
+    name="py3dinterpolations",
+    version="0.2.4",
     description="quick 3D interpolation with python",
     long_description_content_type="text/markdown",
     long_description=long_description,
-    url="https://github.com/giocaizzi/py3Dinterpolations",
+    url="https://github.com/giocaizzi/py3dinterpolations",
     author="giocaizzi",
     author_email="giocaizzi@gmail.com",
     license="MIT",
-    packages=find_packages(include=["py3Dinterpolations", "py3Dinterpolations/*"]),
+    packages=find_packages(include=["py3dinterpolations", "py3dinterpolations.*"]),
     setup_requires=[],
     tests_require=[],
     install_requires=[
         "pandas",
         "numpy",
         "matplotlib",
         "pykrige",
@@ -34,12 +34,12 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     project_urls={
-        "Documentation": "https://giocaizzi.github.io/py3Dinterpolations/",
-        "Bug Reports": "https://github.com/giocaizzi/py3Dinterpolations/issues",
-        "Source": "https://github.com/giocaizzi/py3Dinterpolations",
+        "Documentation": "https://giocaizzi.github.io/py3dinterpolations/",
+        "Bug Reports": "https://github.com/giocaizzi/py3dinterpolations/issues",
+        "Source": "https://github.com/giocaizzi/py3dinterpolations",
     },
 )
```

