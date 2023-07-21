# Comparing `tmp/core_file_preview_app-2.3.0.tar.gz` & `tmp/core_file_preview_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_file_preview_app-2.3.0.tar", last modified: Tue May  2 19:39:08 2023, max compression
+gzip compressed data, was "core_file_preview_app-2.4.0.tar", last modified: Fri Jul 21 02:12:56 2023, max compression
```

## Comparing `core_file_preview_app-2.3.0.tar` & `core_file_preview_app-2.4.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:08.934504 core_file_preview_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:39:07.000000 core_file_preview_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      175 2023-05-02 19:39:07.000000 core_file_preview_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1117 2023-05-02 19:39:08.929399 core_file_preview_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      617 2023-05-02 19:39:07.000000 core_file_preview_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:08.733811 core_file_preview_app-2.3.0/core_file_preview_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:07.000000 core_file_preview_app-2.3.0/core_file_preview_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:08.587298 core_file_preview_app-2.3.0/core_file_preview_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:08.590514 core_file_preview_app-2.3.0/core_file_preview_app/static/core_file_preview_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:08.597410 core_file_preview_app-2.3.0/core_file_preview_app/static/core_file_preview_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:08.825765 core_file_preview_app-2.3.0/core_file_preview_app/static/core_file_preview_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      432 2023-05-02 19:39:07.000000 core_file_preview_app-2.3.0/core_file_preview_app/static/core_file_preview_app/user/css/file_preview.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:08.846369 core_file_preview_app-2.3.0/core_file_preview_app/static/core_file_preview_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5773 2023-05-02 19:39:07.000000 core_file_preview_app-2.3.0/core_file_preview_app/static/core_file_preview_app/user/js/file_preview.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2023-05-02 19:39:07.000000 core_file_preview_app-2.3.0/core_file_preview_app/static/core_file_preview_app/user/js/file_preview.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:08.607434 core_file_preview_app-2.3.0/core_file_preview_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:08.610445 core_file_preview_app-2.3.0/core_file_preview_app/templates/core_file_preview_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:08.856323 core_file_preview_app-2.3.0/core_file_preview_app/templates/core_file_preview_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      618 2023-05-02 19:39:07.000000 core_file_preview_app-2.3.0/core_file_preview_app/templates/core_file_preview_app/user/file_preview_modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      295 2023-05-02 19:39:07.000000 core_file_preview_app-2.3.0/core_file_preview_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:08.866508 core_file_preview_app-2.3.0/core_file_preview_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:07.000000 core_file_preview_app-2.3.0/core_file_preview_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:08.894430 core_file_preview_app-2.3.0/core_file_preview_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:07.000000 core_file_preview_app-2.3.0/core_file_preview_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2735 2023-05-02 19:39:07.000000 core_file_preview_app-2.3.0/core_file_preview_app/views/user/ajax.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:08.810135 core_file_preview_app-2.3.0/core_file_preview_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1117 2023-05-02 19:39:08.000000 core_file_preview_app-2.3.0/core_file_preview_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      865 2023-05-02 19:39:08.000000 core_file_preview_app-2.3.0/core_file_preview_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:39:08.000000 core_file_preview_app-2.3.0/core_file_preview_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       67 2023-05-02 19:39:08.000000 core_file_preview_app-2.3.0/core_file_preview_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       28 2023-05-02 19:39:08.000000 core_file_preview_app-2.3.0/core_file_preview_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:39:07.000000 core_file_preview_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2023-05-02 19:39:07.000000 core_file_preview_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       46 2023-05-02 19:39:07.000000 core_file_preview_app-2.3.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:39:08.936449 core_file_preview_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1411 2023-05-02 19:39:07.000000 core_file_preview_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:08.920067 core_file_preview_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:07.000000 core_file_preview_app-2.3.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      259 2023-05-02 19:39:07.000000 core_file_preview_app-2.3.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:56.774859 core_file_preview_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:12:54.000000 core_file_preview_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      175 2023-07-21 02:12:55.000000 core_file_preview_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1117 2023-07-21 02:12:56.770147 core_file_preview_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      617 2023-07-21 02:12:55.000000 core_file_preview_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:56.574704 core_file_preview_app-2.4.0/core_file_preview_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:55.000000 core_file_preview_app-2.4.0/core_file_preview_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:56.422053 core_file_preview_app-2.4.0/core_file_preview_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:56.425927 core_file_preview_app-2.4.0/core_file_preview_app/static/core_file_preview_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:56.434451 core_file_preview_app-2.4.0/core_file_preview_app/static/core_file_preview_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:56.661332 core_file_preview_app-2.4.0/core_file_preview_app/static/core_file_preview_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      432 2023-07-21 02:12:55.000000 core_file_preview_app-2.4.0/core_file_preview_app/static/core_file_preview_app/user/css/file_preview.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:56.683441 core_file_preview_app-2.4.0/core_file_preview_app/static/core_file_preview_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5773 2023-07-21 02:12:55.000000 core_file_preview_app-2.4.0/core_file_preview_app/static/core_file_preview_app/user/js/file_preview.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2023-07-21 02:12:55.000000 core_file_preview_app-2.4.0/core_file_preview_app/static/core_file_preview_app/user/js/file_preview.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:56.444737 core_file_preview_app-2.4.0/core_file_preview_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:56.448071 core_file_preview_app-2.4.0/core_file_preview_app/templates/core_file_preview_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:56.694949 core_file_preview_app-2.4.0/core_file_preview_app/templates/core_file_preview_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      712 2023-07-21 02:12:55.000000 core_file_preview_app-2.4.0/core_file_preview_app/templates/core_file_preview_app/user/file_preview_modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      295 2023-07-21 02:12:55.000000 core_file_preview_app-2.4.0/core_file_preview_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:56.705753 core_file_preview_app-2.4.0/core_file_preview_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:55.000000 core_file_preview_app-2.4.0/core_file_preview_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:56.733248 core_file_preview_app-2.4.0/core_file_preview_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:55.000000 core_file_preview_app-2.4.0/core_file_preview_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2735 2023-07-21 02:12:55.000000 core_file_preview_app-2.4.0/core_file_preview_app/views/user/ajax.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:56.647326 core_file_preview_app-2.4.0/core_file_preview_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1117 2023-07-21 02:12:56.000000 core_file_preview_app-2.4.0/core_file_preview_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      865 2023-07-21 02:12:56.000000 core_file_preview_app-2.4.0/core_file_preview_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:12:56.000000 core_file_preview_app-2.4.0/core_file_preview_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       67 2023-07-21 02:12:56.000000 core_file_preview_app-2.4.0/core_file_preview_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       28 2023-07-21 02:12:56.000000 core_file_preview_app-2.4.0/core_file_preview_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:12:55.000000 core_file_preview_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2023-07-21 02:12:55.000000 core_file_preview_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       46 2023-07-21 02:12:55.000000 core_file_preview_app-2.4.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:12:56.776618 core_file_preview_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1411 2023-07-21 02:12:55.000000 core_file_preview_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:56.760024 core_file_preview_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:55.000000 core_file_preview_app-2.4.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      259 2023-07-21 02:12:55.000000 core_file_preview_app-2.4.0/tests/test_settings.py
```

### Comparing `core_file_preview_app-2.3.0/LICENSE.md` & `core_file_preview_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_file_preview_app-2.3.0/PKG-INFO` & `core_file_preview_app-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_file_preview_app
-Version: 2.3.0
+Version: 2.4.0
 Summary: File preview functionalities for the curator core project
 Home-page: https://github.com/usnistgov/core_main_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =====================
         Core File Preview App
```

### Comparing `core_file_preview_app-2.3.0/README.rst` & `core_file_preview_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_file_preview_app-2.3.0/core_file_preview_app/static/core_file_preview_app/user/js/file_preview.js` & `core_file_preview_app-2.4.0/core_file_preview_app/static/core_file_preview_app/user/js/file_preview.js`

 * *Files identical despite different names*

### Comparing `core_file_preview_app-2.3.0/core_file_preview_app/templates/core_file_preview_app/user/file_preview_modal.html` & `core_file_preview_app-2.4.0/core_file_preview_app/templates/core_file_preview_app/user/file_preview_modal.html`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 {% block modal_body %}
     <div id="fileImageDisplayArea"></div>
     <pre id="fileTextDisplayArea"></pre>
     <div class="alert alert-info alert-preview" id="errorArea"></div>
 {% endblock %}
 
 {% block modal_footer %}
-    <div class="ml-auto">
+    <div class="{% if BOOTSTRAP_VERSION == "4.6.2" %}ml-auto{% elif BOOTSTRAP_VERSION == "5.1.3" %}ms-auto{% endif %}">
         <a id="btn-file-preview-download"
            class="btn btn-primary"
            href="#">
             <i class="fas fa-download"></i>
             Download
         </a>
     </div>
```

### Comparing `core_file_preview_app-2.3.0/core_file_preview_app/views/user/ajax.py` & `core_file_preview_app-2.4.0/core_file_preview_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_file_preview_app-2.3.0/core_file_preview_app.egg-info/PKG-INFO` & `core_file_preview_app-2.4.0/core_file_preview_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-file-preview-app
-Version: 2.3.0
+Version: 2.4.0
 Summary: File preview functionalities for the curator core project
 Home-page: https://github.com/usnistgov/core_main_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =====================
         Core File Preview App
```

### Comparing `core_file_preview_app-2.3.0/core_file_preview_app.egg-info/SOURCES.txt` & `core_file_preview_app-2.4.0/core_file_preview_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_file_preview_app-2.3.0/setup.py` & `core_file_preview_app-2.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_file_preview_app",
-    version="2.3.0",
+    version="2.4.0",
     description="File preview functionalities for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_main_app",
     packages=find_packages(),
     include_package_data=True,
```

