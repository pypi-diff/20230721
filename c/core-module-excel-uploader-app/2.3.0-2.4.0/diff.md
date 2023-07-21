# Comparing `tmp/core_module_excel_uploader_app-2.3.0.tar.gz` & `tmp/core_module_excel_uploader_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_module_excel_uploader_app-2.3.0.tar", last modified: Tue May  2 19:45:53 2023, max compression
+gzip compressed data, was "core_module_excel_uploader_app-2.4.0.tar", last modified: Fri Jul 21 02:15:07 2023, max compression
```

## Comparing `core_module_excel_uploader_app-2.3.0.tar` & `core_module_excel_uploader_app-2.4.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:53.004203 core_module_excel_uploader_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      193 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1160 2023-05-02 19:45:52.999256 core_module_excel_uploader_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      666 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:52.782479 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:52.631703 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:52.644435 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:52.872592 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      426 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/css/excel_uploader.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:52.884409 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      310 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/js/excel_uploader.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:52.896551 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/xls/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    25600 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/xls/data.xls
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:52.653899 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:52.909402 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/templates/core_module_excel_uploader_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      161 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/templates/core_module_excel_uploader_app/excel_uploader.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      318 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:52.951185 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      178 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/views/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7529 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/views/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:52.858525 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1160 2023-05-02 19:45:52.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      985 2023-05-02 19:45:52.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:45:52.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-05-02 19:45:52.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2023-05-02 19:45:52.000000 core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       41 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       19 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:45:53.006231 core_module_excel_uploader_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:52.989626 core_module_excel_uploader_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2023-05-02 19:45:51.000000 core_module_excel_uploader_app-2.3.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:07.840495 core_module_excel_uploader_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:15:06.000000 core_module_excel_uploader_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      193 2023-07-21 02:15:06.000000 core_module_excel_uploader_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1160 2023-07-21 02:15:07.836892 core_module_excel_uploader_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      666 2023-07-21 02:15:06.000000 core_module_excel_uploader_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:07.674077 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:06.000000 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:07.521826 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:07.542072 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:07.746457 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      426 2023-07-21 02:15:06.000000 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/css/excel_uploader.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:07.756665 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      310 2023-07-21 02:15:06.000000 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/js/excel_uploader.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:07.766529 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/xls/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    25600 2023-07-21 02:15:06.000000 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/xls/data.xls
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:07.550580 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:07.776104 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app/templates/core_module_excel_uploader_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      161 2023-07-21 02:15:06.000000 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app/templates/core_module_excel_uploader_app/excel_uploader.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      318 2023-07-21 02:15:06.000000 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:07.807140 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:06.000000 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      178 2023-07-21 02:15:06.000000 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app/views/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7529 2023-07-21 02:15:06.000000 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app/views/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:07.734454 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1160 2023-07-21 02:15:07.000000 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      985 2023-07-21 02:15:07.000000 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:15:07.000000 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-07-21 02:15:07.000000 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2023-07-21 02:15:07.000000 core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:15:06.000000 core_module_excel_uploader_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       41 2023-07-21 02:15:06.000000 core_module_excel_uploader_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       19 2023-07-21 02:15:06.000000 core_module_excel_uploader_app-2.4.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:15:07.842115 core_module_excel_uploader_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2023-07-21 02:15:06.000000 core_module_excel_uploader_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:07.828703 core_module_excel_uploader_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:15:06.000000 core_module_excel_uploader_app-2.4.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2023-07-21 02:15:06.000000 core_module_excel_uploader_app-2.4.0/tests/test_settings.py
```

### Comparing `core_module_excel_uploader_app-2.3.0/LICENSE.md` & `core_module_excel_uploader_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_module_excel_uploader_app-2.3.0/PKG-INFO` & `core_module_excel_uploader_app-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_module_excel_uploader_app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Excel Uploader module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_excel_uploader_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_excel_uploader_app
         ==============================
```

### Comparing `core_module_excel_uploader_app-2.3.0/README.rst` & `core_module_excel_uploader_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/xls/data.xls` & `core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/xls/data.xls`

 * *Files identical despite different names*

### Comparing `core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app/views/views.py` & `core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app/views/views.py`

 * *Files identical despite different names*

### Comparing `core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app.egg-info/PKG-INFO` & `core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-module-excel-uploader-app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Excel Uploader module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_excel_uploader_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_excel_uploader_app
         ==============================
```

### Comparing `core_module_excel_uploader_app-2.3.0/core_module_excel_uploader_app.egg-info/SOURCES.txt` & `core_module_excel_uploader_app-2.4.0/core_module_excel_uploader_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_module_excel_uploader_app-2.3.0/setup.py` & `core_module_excel_uploader_app-2.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_excel_uploader_app",
-    version="2.3.0",
+    version="2.4.0",
     description="Excel Uploader module for the parser core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_excel_uploader_app",
     packages=find_packages(),
     include_package_data=True,
```

