# Comparing `tmp/core_module_chemical_composition_simple_app-2.3.0.tar.gz` & `tmp/core_module_chemical_composition_simple_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_module_chemical_composition_simple_app-2.3.0.tar", last modified: Tue May  2 19:45:22 2023, max compression
+gzip compressed data, was "core_module_chemical_composition_simple_app-2.4.0.tar", last modified: Fri Jul 21 02:15:01 2023, max compression
```

## Comparing `core_module_chemical_composition_simple_app-2.3.0.tar` & `core_module_chemical_composition_simple_app-2.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:22.780586 core_module_chemical_composition_simple_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:45:21.000000 core_module_chemical_composition_simple_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      189 2023-05-02 19:45:21.000000 core_module_chemical_composition_simple_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1277 2023-05-02 19:45:22.775426 core_module_chemical_composition_simple_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      736 2023-05-02 19:45:21.000000 core_module_chemical_composition_simple_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:22.618981 core_module_chemical_composition_simple_app-2.3.0/core_module_chemical_composition_simple_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:21.000000 core_module_chemical_composition_simple_app-2.3.0/core_module_chemical_composition_simple_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:22.491086 core_module_chemical_composition_simple_app-2.3.0/core_module_chemical_composition_simple_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:22.493879 core_module_chemical_composition_simple_app-2.3.0/core_module_chemical_composition_simple_app/static/core_module_chemical_composition_simple_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:22.733710 core_module_chemical_composition_simple_app-2.3.0/core_module_chemical_composition_simple_app/static/core_module_chemical_composition_simple_app/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1374 2023-05-02 19:45:21.000000 core_module_chemical_composition_simple_app-2.3.0/core_module_chemical_composition_simple_app/static/core_module_chemical_composition_simple_app/js/chemical_element_composition_simple.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      392 2023-05-02 19:45:21.000000 core_module_chemical_composition_simple_app-2.3.0/core_module_chemical_composition_simple_app/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3023 2023-05-02 19:45:21.000000 core_module_chemical_composition_simple_app-2.3.0/core_module_chemical_composition_simple_app/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:22.718046 core_module_chemical_composition_simple_app-2.3.0/core_module_chemical_composition_simple_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1277 2023-05-02 19:45:22.000000 core_module_chemical_composition_simple_app-2.3.0/core_module_chemical_composition_simple_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      747 2023-05-02 19:45:22.000000 core_module_chemical_composition_simple_app-2.3.0/core_module_chemical_composition_simple_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:45:22.000000 core_module_chemical_composition_simple_app-2.3.0/core_module_chemical_composition_simple_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-05-02 19:45:22.000000 core_module_chemical_composition_simple_app-2.3.0/core_module_chemical_composition_simple_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       50 2023-05-02 19:45:22.000000 core_module_chemical_composition_simple_app-2.3.0/core_module_chemical_composition_simple_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:45:21.000000 core_module_chemical_composition_simple_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-05-02 19:45:21.000000 core_module_chemical_composition_simple_app-2.3.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:45:22.782514 core_module_chemical_composition_simple_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      990 2023-05-02 19:45:21.000000 core_module_chemical_composition_simple_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:22.764969 core_module_chemical_composition_simple_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:21.000000 core_module_chemical_composition_simple_app-2.3.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2023-05-02 19:45:21.000000 core_module_chemical_composition_simple_app-2.3.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:01.223152 core_module_chemical_composition_simple_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:14:57.000000 core_module_chemical_composition_simple_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      189 2023-07-21 02:14:57.000000 core_module_chemical_composition_simple_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1277 2023-07-21 02:15:01.218086 core_module_chemical_composition_simple_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      736 2023-07-21 02:14:57.000000 core_module_chemical_composition_simple_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:01.080886 core_module_chemical_composition_simple_app-2.4.0/core_module_chemical_composition_simple_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:57.000000 core_module_chemical_composition_simple_app-2.4.0/core_module_chemical_composition_simple_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:00.625640 core_module_chemical_composition_simple_app-2.4.0/core_module_chemical_composition_simple_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:00.983350 core_module_chemical_composition_simple_app-2.4.0/core_module_chemical_composition_simple_app/static/core_module_chemical_composition_simple_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:01.166947 core_module_chemical_composition_simple_app-2.4.0/core_module_chemical_composition_simple_app/static/core_module_chemical_composition_simple_app/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1374 2023-07-21 02:14:57.000000 core_module_chemical_composition_simple_app-2.4.0/core_module_chemical_composition_simple_app/static/core_module_chemical_composition_simple_app/js/chemical_element_composition_simple.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      392 2023-07-21 02:14:57.000000 core_module_chemical_composition_simple_app-2.4.0/core_module_chemical_composition_simple_app/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3023 2023-07-21 02:14:57.000000 core_module_chemical_composition_simple_app-2.4.0/core_module_chemical_composition_simple_app/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:01.154114 core_module_chemical_composition_simple_app-2.4.0/core_module_chemical_composition_simple_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1277 2023-07-21 02:15:00.000000 core_module_chemical_composition_simple_app-2.4.0/core_module_chemical_composition_simple_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      747 2023-07-21 02:15:00.000000 core_module_chemical_composition_simple_app-2.4.0/core_module_chemical_composition_simple_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:15:00.000000 core_module_chemical_composition_simple_app-2.4.0/core_module_chemical_composition_simple_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-07-21 02:15:00.000000 core_module_chemical_composition_simple_app-2.4.0/core_module_chemical_composition_simple_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       50 2023-07-21 02:15:00.000000 core_module_chemical_composition_simple_app-2.4.0/core_module_chemical_composition_simple_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:14:57.000000 core_module_chemical_composition_simple_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2023-07-21 02:14:57.000000 core_module_chemical_composition_simple_app-2.4.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:15:01.251020 core_module_chemical_composition_simple_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      990 2023-07-21 02:14:57.000000 core_module_chemical_composition_simple_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:01.189971 core_module_chemical_composition_simple_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:57.000000 core_module_chemical_composition_simple_app-2.4.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2023-07-21 02:14:57.000000 core_module_chemical_composition_simple_app-2.4.0/tests/test_settings.py
```

### Comparing `core_module_chemical_composition_simple_app-2.3.0/LICENSE.md` & `core_module_chemical_composition_simple_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_simple_app-2.3.0/PKG-INFO` & `core_module_chemical_composition_simple_app-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_module_chemical_composition_simple_app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Chemical composition simple module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_chemical_composition_simple_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_chemical_composition_simple_app
         ===========================================
```

### Comparing `core_module_chemical_composition_simple_app-2.3.0/README.rst` & `core_module_chemical_composition_simple_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_simple_app-2.3.0/core_module_chemical_composition_simple_app/static/core_module_chemical_composition_simple_app/js/chemical_element_composition_simple.js` & `core_module_chemical_composition_simple_app-2.4.0/core_module_chemical_composition_simple_app/static/core_module_chemical_composition_simple_app/js/chemical_element_composition_simple.js`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_simple_app-2.3.0/core_module_chemical_composition_simple_app/views.py` & `core_module_chemical_composition_simple_app-2.4.0/core_module_chemical_composition_simple_app/views.py`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_simple_app-2.3.0/core_module_chemical_composition_simple_app.egg-info/PKG-INFO` & `core_module_chemical_composition_simple_app-2.4.0/core_module_chemical_composition_simple_app.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-module-chemical-composition-simple-app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Chemical composition simple module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_chemical_composition_simple_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_chemical_composition_simple_app
         ===========================================
```

### Comparing `core_module_chemical_composition_simple_app-2.3.0/core_module_chemical_composition_simple_app.egg-info/SOURCES.txt` & `core_module_chemical_composition_simple_app-2.4.0/core_module_chemical_composition_simple_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

