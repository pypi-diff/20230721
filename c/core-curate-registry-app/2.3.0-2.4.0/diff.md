# Comparing `tmp/core_curate_registry_app-2.3.0.tar.gz` & `tmp/core_curate_registry_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_curate_registry_app-2.3.0.tar", last modified: Tue May  2 19:35:57 2023, max compression
+gzip compressed data, was "core_curate_registry_app-2.4.0.tar", last modified: Fri Jul 21 02:10:08 2023, max compression
```

## Comparing `core_curate_registry_app-2.3.0.tar` & `core_curate_registry_app-2.4.0.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.863752 core_curate_registry_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:35:54.000000 core_curate_registry_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-05-02 19:35:54.000000 core_curate_registry_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1180 2023-05-02 19:35:57.858855 core_curate_registry_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      644 2023-05-02 19:35:54.000000 core_curate_registry_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.227145 core_curate_registry_app-2.3.0/core_curate_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:54.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.347119 core_curate_registry_app-2.3.0/core_curate_registry_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:54.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.383341 core_curate_registry_app-2.3.0/core_curate_registry_app/components/curate_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:54.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/components/curate_data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      620 2023-05-02 19:35:54.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/components/curate_data_structure/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.409603 core_curate_registry_app-2.3.0/core_curate_registry_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:54.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/rest/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      332 2023-05-02 19:35:54.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      666 2023-05-02 19:35:54.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:56.951219 core_curate_registry_app-2.3.0/core_curate_registry_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:56.941708 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:56.944615 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.460381 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_app/user/js/select_template.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2059 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_app/user/js/view_data_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      181 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_app/user/js/view_data_registry.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:56.954510 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:56.971533 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.478550 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       61 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/css/index.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.563991 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      348 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/banner.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1076 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/enter_data_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       86 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/enter_data_registry.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      945 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/role.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      871 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/start_curate.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1158 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/title.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       45 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/title.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.024314 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:56.984846 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.599974 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1286 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/curate.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      547 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/curate_start.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.613671 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1704 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/enter_data.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.629148 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      740 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/modals/xml-valid-registry.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.641960 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/data-review/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.656349 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/data-review/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1218 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/data-review/modals/save-form-registry.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1047 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/data-review/view_data.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.034659 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.668982 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_registry_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      509 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_registry_app/user/index.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3665 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.700707 core_curate_registry_app-2.3.0/core_curate_registry_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      472 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/utils/jquery.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.715953 core_curate_registry_app-2.3.0/core_curate_registry_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.768465 core_curate_registry_app-2.3.0/core_curate_registry_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1463 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7985 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/core_curate_registry_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.332546 core_curate_registry_app-2.3.0/core_curate_registry_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1180 2023-05-02 19:35:56.000000 core_curate_registry_app-2.3.0/core_curate_registry_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2500 2023-05-02 19:35:56.000000 core_curate_registry_app-2.3.0/core_curate_registry_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:35:56.000000 core_curate_registry_app-2.3.0/core_curate_registry_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-05-02 19:35:56.000000 core_curate_registry_app-2.3.0/core_curate_registry_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       31 2023-05-02 19:35:56.000000 core_curate_registry_app-2.3.0/core_curate_registry_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       53 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:35:57.865853 core_curate_registry_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1480 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.804615 core_curate_registry_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1105 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:57.846053 core_curate_registry_app-2.3.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/tests/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1749 2023-05-02 19:35:55.000000 core_curate_registry_app-2.3.0/tests/utils/test_units.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:08.771091 core_curate_registry_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:10:05.000000 core_curate_registry_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-07-21 02:10:05.000000 core_curate_registry_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1180 2023-07-21 02:10:08.765765 core_curate_registry_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      644 2023-07-21 02:10:05.000000 core_curate_registry_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:08.233863 core_curate_registry_app-2.4.0/core_curate_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:05.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:08.329400 core_curate_registry_app-2.4.0/core_curate_registry_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:05.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:08.356234 core_curate_registry_app-2.4.0/core_curate_registry_app/components/curate_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:05.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/components/curate_data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      620 2023-07-21 02:10:05.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/components/curate_data_structure/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:08.381275 core_curate_registry_app-2.4.0/core_curate_registry_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:05.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/rest/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      332 2023-07-21 02:10:05.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      666 2023-07-21 02:10:05.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:07.934507 core_curate_registry_app-2.4.0/core_curate_registry_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:07.923278 core_curate_registry_app-2.4.0/core_curate_registry_app/static/core_curate_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:07.926933 core_curate_registry_app-2.4.0/core_curate_registry_app/static/core_curate_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:08.416877 core_curate_registry_app-2.4.0/core_curate_registry_app/static/core_curate_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/static/core_curate_app/user/js/select_template.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2047 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/static/core_curate_app/user/js/view_data_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      181 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/static/core_curate_app/user/js/view_data_registry.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:07.937667 core_curate_registry_app-2.4.0/core_curate_registry_app/static/core_curate_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:07.945828 core_curate_registry_app-2.4.0/core_curate_registry_app/static/core_curate_registry_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:08.428058 core_curate_registry_app-2.4.0/core_curate_registry_app/static/core_curate_registry_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       61 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/static/core_curate_registry_app/user/css/index.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:08.501254 core_curate_registry_app-2.4.0/core_curate_registry_app/static/core_curate_registry_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      348 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/static/core_curate_registry_app/user/js/banner.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1056 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/static/core_curate_registry_app/user/js/enter_data_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       86 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/static/core_curate_registry_app/user/js/enter_data_registry.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      945 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/static/core_curate_registry_app/user/js/role.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      871 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/static/core_curate_registry_app/user/js/start_curate.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1158 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/static/core_curate_registry_app/user/js/title.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       45 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/static/core_curate_registry_app/user/js/title.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:07.991094 core_curate_registry_app-2.4.0/core_curate_registry_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:07.959838 core_curate_registry_app-2.4.0/core_curate_registry_app/templates/core_curate_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:08.520751 core_curate_registry_app-2.4.0/core_curate_registry_app/templates/core_curate_app/user/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1762 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/templates/core_curate_app/user/curate.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      547 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/templates/core_curate_app/user/curate_start.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:08.546423 core_curate_registry_app-2.4.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2270 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/enter_data.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:08.557651 core_curate_registry_app-2.4.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      842 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/modals/xml-valid-registry.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:08.569666 core_curate_registry_app-2.4.0/core_curate_registry_app/templates/core_curate_app/user/data-review/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:08.580134 core_curate_registry_app-2.4.0/core_curate_registry_app/templates/core_curate_app/user/data-review/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1309 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/templates/core_curate_app/user/data-review/modals/save-form-registry.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1519 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/templates/core_curate_app/user/data-review/view_data.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:07.994405 core_curate_registry_app-2.4.0/core_curate_registry_app/templates/core_curate_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:08.592354 core_curate_registry_app-2.4.0/core_curate_registry_app/templates/core_curate_registry_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      509 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/templates/core_curate_registry_app/user/index.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3909 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:08.620144 core_curate_registry_app-2.4.0/core_curate_registry_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      472 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/utils/jquery.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:08.634300 core_curate_registry_app-2.4.0/core_curate_registry_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:08.680095 core_curate_registry_app-2.4.0/core_curate_registry_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1463 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7985 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/core_curate_registry_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:08.305531 core_curate_registry_app-2.4.0/core_curate_registry_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1180 2023-07-21 02:10:07.000000 core_curate_registry_app-2.4.0/core_curate_registry_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2530 2023-07-21 02:10:07.000000 core_curate_registry_app-2.4.0/core_curate_registry_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:10:07.000000 core_curate_registry_app-2.4.0/core_curate_registry_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-07-21 02:10:07.000000 core_curate_registry_app-2.4.0/core_curate_registry_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       31 2023-07-21 02:10:07.000000 core_curate_registry_app-2.4.0/core_curate_registry_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       53 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:10:08.789923 core_curate_registry_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1480 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:08.709276 core_curate_registry_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1322 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:08.753636 core_curate_registry_app-2.4.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/tests/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      563 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/tests/utils/test_unit_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1749 2023-07-21 02:10:06.000000 core_curate_registry_app-2.4.0/tests/utils/test_units.py
```

### Comparing `core_curate_registry_app-2.3.0/LICENSE.md` & `core_curate_registry_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.3.0/PKG-INFO` & `core_curate_registry_app-2.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_curate_registry_app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Curation functionalities specific to Registry applications for the curator core project
 Home-page: https://github.com/usnistgov/core_curate_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: Core Curate Registry App
         ========================
```

### Comparing `core_curate_registry_app-2.3.0/README.rst` & `core_curate_registry_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.3.0/core_curate_registry_app/components/curate_data_structure/api.py` & `core_curate_registry_app-2.4.0/core_curate_registry_app/components/curate_data_structure/api.py`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.3.0/core_curate_registry_app/settings.py` & `core_curate_registry_app-2.4.0/core_curate_registry_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_app/user/js/view_data_registry.js` & `core_curate_registry_app-2.4.0/core_curate_registry_app/static/core_curate_app/user/js/view_data_registry.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -75,13 +75,11 @@
         },
         success: function(data) {
             window.location = curateIndexUrl;
         },
         error: function(data) {
             hideSpinner($("publish > i"), icon)
             var myArr = JSON.parse(data.responseText);
-            $.notify(myArr.message, {
-                style: myArr.tags
-            });
+            $.notify(myArr.message, "danger");
         }
     });
 }
```

### Comparing `core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/enter_data_registry.js` & `core_curate_registry_app-2.4.0/core_curate_registry_app/static/core_curate_registry_app/user/js/enter_data_registry.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -12,31 +12,27 @@
         url: saveFormUrl,
         type: 'POST',
         data: {
             'id': objectID
         },
         dataType: 'json',
         success: function(data) {
-            $.notify(data.message, {
-                style: data.tags
-            });
+            $.notify(data.message, "success");
         },
     }).always(function(data) {
         // get old button icon
         hideSpinner($(".save-form-registry > i"), icon);
     });
 };
 
 /**
  * Notify the download
  */
 var downloadMessage = function() {
-    $.notify("Download in progress", {
-        style: "info"
-    });
+    $.notify("Download in progress", "info");
 };
 
 /**
  * Shows the review data dialog
  */
 var reviewDataDialog = function() {
     $("#xml-valid-registry-modal").modal("show");
```

### Comparing `core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/role.js` & `core_curate_registry_app-2.4.0/core_curate_registry_app/static/core_curate_registry_app/user/js/role.js`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/start_curate.js` & `core_curate_registry_app-2.4.0/core_curate_registry_app/static/core_curate_registry_app/user/js/start_curate.js`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.3.0/core_curate_registry_app/static/core_curate_registry_app/user/js/title.js` & `core_curate_registry_app-2.4.0/core_curate_registry_app/static/core_curate_registry_app/user/js/title.js`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/curate.html` & `core_curate_registry_app-2.4.0/core_curate_registry_app/templates/core_curate_app/user/curate.html`

 * *Files 23% similar despite different names*

```diff
@@ -22,60 +22,90 @@
 00000150: 6e65 3b22 3e0a 2020 2020 7b7b 6461 7461  ne;">.    {{data
 00000160: 2e63 7573 746f 6d5f 7265 736f 7572 6365  .custom_resource
 00000170: 2e74 6974 6c65 7d7d 0a3c 2f64 6976 3e0a  .title}}.</div>.
 00000180: 3c64 6976 2063 6c61 7373 3d22 616c 6572  <div class="aler
 00000190: 7420 616c 6572 742d 6461 6e67 6572 2220  t alert-danger" 
 000001a0: 6964 3d22 6261 6e6e 6572 5f65 7272 6f72  id="banner_error
 000001b0: 7322 2073 7479 6c65 3d22 6469 7370 6c61  s" style="displa
-000001c0: 793a 206e 6f6e 653b 223e 0a20 2020 2020  y: none;">.     
-000001d0: 2020 203c 6120 6872 6566 3d22 2322 2063     <a href="#" c
-000001e0: 6c61 7373 3d22 636c 6f73 6522 2064 6174  lass="close" dat
-000001f0: 612d 6869 6465 3d22 616c 6572 7422 2061  a-hide="alert" a
-00000200: 7269 612d 6c61 6265 6c3d 2263 6c6f 7365  ria-label="close
-00000210: 223e 2674 696d 6573 3b3c 2f61 3e0a 2020  ">&times;</a>.  
-00000220: 2020 2009 3c68 343e 3c69 2063 6c61 7373     .<h4><i class
-00000230: 3d22 6661 7320 6661 2d65 7863 6c61 6d61  ="fas fa-exclama
-00000240: 7469 6f6e 2d63 6972 636c 6522 3e3c 2f69  tion-circle"></i
-00000250: 3e20 4572 726f 723c 2f68 343e 0a20 2020  > Error</h4>.   
-00000260: 2020 2020 203c 6469 7620 6964 3d22 666f       <div id="fo
-00000270: 726d 5f73 7461 7274 5f65 7272 6f72 7322  rm_start_errors"
-00000280: 3e0a 3c2f 6469 763e 0a3c 2f64 6976 3e0a  >.</div>.</div>.
-00000290: 0a50 6c65 6173 6520 7365 6c65 6374 206f  .Please select o
-000002a0: 6e65 206f 6620 7468 6520 666f 6c6c 6f77  ne of the follow
-000002b0: 696e 6720 6f70 7469 6f6e 7320 746f 2041  ing options to A
-000002c0: 6464 2079 6f75 7220 5265 736f 7572 6365  dd your Resource
-000002d0: 2e20 596f 7520 6361 6e20 6372 6561 7465  . You can create
-000002e0: 2061 206e 6577 2072 6573 6f75 7263 652c   a new resource,
-000002f0: 206f 7220 7570 6c6f 6164 2061 6e20 584d   or upload an XM
-00000300: 4c20 6669 6c65 2e0a 0a3c 6272 2f3e 3c62  L file...<br/><b
-00000310: 722f 3e0a 3c64 6976 2069 643d 2266 6f72  r/>.<div id="for
-00000320: 6d5f 7374 6172 745f 636f 6e74 656e 7422  m_start_content"
-00000330: 3e0a 3c2f 6469 763e 0a3c 6469 7620 6964  >.</div>.<div id
-00000340: 3d22 7465 6d70 6c61 7465 5f69 6422 2063  ="template_id" c
-00000350: 6c61 7373 3d22 6869 6464 656e 223e 7b7b  lass="hidden">{{
-00000360: 2064 6174 612e 7465 6d70 6c61 7465 5f69   data.template_i
-00000370: 6420 7d7d 3c2f 6469 763e 0a3c 6272 2f3e  d }}</div>.<br/>
-00000380: 3c62 722f 3e0a 0a3c 6275 7474 6f6e 2069  <br/>..<button i
-00000390: 643d 2262 746e 2d73 6176 652d 6461 7461  d="btn-save-data
-000003a0: 2220 636c 6173 733d 2262 746e 2062 746e  " class="btn btn
-000003b0: 2d70 7269 6d61 7279 2220 6869 6464 656e  -primary" hidden
-000003c0: 3d22 223e 3c69 2063 6c61 7373 3d22 6661  =""><i class="fa
-000003d0: 7320 6661 2d73 6176 6522 3e3c 2f69 3e20  s fa-save"></i> 
-000003e0: 5361 7665 2077 6974 686f 7574 2065 6469  Save without edi
-000003f0: 7469 6e67 3c2f 6275 7474 6f6e 3e0a 3c62  ting</button>.<b
-00000400: 7574 746f 6e20 6964 3d22 6274 6e2d 6f70  utton id="btn-op
-00000410: 656e 2d64 6174 6122 2063 6c61 7373 3d22  en-data" class="
-00000420: 6274 6e20 6274 6e2d 7072 696d 6172 7922  btn btn-primary"
-00000430: 3e3c 6920 636c 6173 733d 2266 6173 2066  ><i class="fas f
-00000440: 612d 636f 6465 223e 3c2f 693e 204f 7065  a-code"></i> Ope
-00000450: 6e20 696e 2054 6578 7420 6564 6974 6f72  n in Text editor
-00000460: 3c2f 6275 7474 6f6e 3e0a 3c62 7574 746f  </button>.<butto
-00000470: 6e20 6964 3d22 6274 6e2d 6469 7370 6c61  n id="btn-displa
-00000480: 792d 6461 7461 2220 636c 6173 733d 2262  y-data" class="b
-00000490: 746e 2062 746e 2d70 7269 6d61 7279 223e  tn btn-primary">
-000004a0: 3c69 2063 6c61 7373 3d22 6661 7320 6661  <i class="fas fa
-000004b0: 2d70 6c61 7922 3e3c 2f69 3e20 5374 6172  -play"></i> Star
-000004c0: 7420 6564 6974 696e 673c 2f62 7574 746f  t editing</butto
-000004d0: 6e3e 0a3c 6469 7620 6964 3d22 726f 6c65  n>.<div id="role
-000004e0: 2220 636c 6173 733d 2268 6964 6465 6e22  " class="hidden"
-000004f0: 3e7b 7b20 6461 7461 2e72 6f6c 6520 7d7d  >{{ data.role }}
-00000500: 3c2f 6469 763e                           </div>
+000001c0: 793a 206e 6f6e 653b 223e 0a20 2020 203c  y: none;">.    <
+000001d0: 6275 7474 6f6e 2074 7970 653d 2262 7574  button type="but
+000001e0: 746f 6e22 2061 7269 612d 6c61 6265 6c3d  ton" aria-label=
+000001f0: 2243 6c6f 7365 220a 2020 2020 2020 2020  "Close".        
+00000200: 2020 2020 7b25 2069 6620 424f 4f54 5354      {% if BOOTST
+00000210: 5241 505f 5645 5253 494f 4e20 3d3d 2022  RAP_VERSION == "
+00000220: 342e 362e 3222 2025 7d63 6c61 7373 3d22  4.6.2" %}class="
+00000230: 636c 6f73 6522 0a20 2020 2020 2020 2020  close".         
+00000240: 2020 207b 2520 656c 6966 2042 4f4f 5453     {% elif BOOTS
+00000250: 5452 4150 5f56 4552 5349 4f4e 203d 3d20  TRAP_VERSION == 
+00000260: 2235 2e31 2e33 2220 257d 636c 6173 733d  "5.1.3" %}class=
+00000270: 2262 746e 2d63 6c6f 7365 2066 6c6f 6174  "btn-close float
+00000280: 2d65 6e64 220a 2020 2020 2020 2020 2020  -end".          
+00000290: 2020 7b25 2065 6e64 6966 2025 7d0a 2020    {% endif %}.  
+000002a0: 2020 2020 2020 2020 2020 7b25 2069 6620            {% if 
+000002b0: 424f 4f54 5354 5241 505f 5645 5253 494f  BOOTSTRAP_VERSIO
+000002c0: 4e20 3d3d 2022 342e 362e 3222 2025 7d64  N == "4.6.2" %}d
+000002d0: 6174 612d 6469 736d 6973 733d 2261 6c65  ata-dismiss="ale
+000002e0: 7274 220a 2020 2020 2020 2020 2020 2020  rt".            
+000002f0: 7b25 2065 6c69 6620 424f 4f54 5354 5241  {% elif BOOTSTRA
+00000300: 505f 5645 5253 494f 4e20 3d3d 2022 352e  P_VERSION == "5.
+00000310: 312e 3322 2025 7d64 6174 612d 6273 2d64  1.3" %}data-bs-d
+00000320: 6973 6d69 7373 3d22 616c 6572 7422 0a20  ismiss="alert". 
+00000330: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
+00000340: 6469 6620 257d 0a20 2020 203e 0a20 2020  dif %}.    >.   
+00000350: 2020 2020 207b 2520 6966 2042 4f4f 5453       {% if BOOTS
+00000360: 5452 4150 5f56 4552 5349 4f4e 203d 3d20  TRAP_VERSION == 
+00000370: 2234 2e36 2e32 2220 257d 0a20 2020 2020  "4.6.2" %}.     
+00000380: 2020 2020 2020 203c 7370 616e 2061 7269         <span ari
+00000390: 612d 6869 6464 656e 3d22 7472 7565 223e  a-hidden="true">
+000003a0: 2674 696d 6573 3b3c 2f73 7061 6e3e 0a20  &times;</span>. 
+000003b0: 2020 2020 2020 207b 2520 656c 6966 2042         {% elif B
+000003c0: 4f4f 5453 5452 4150 5f56 4552 5349 4f4e  OOTSTRAP_VERSION
+000003d0: 203d 3d20 2235 2e31 2e33 2220 257d 0a20   == "5.1.3" %}. 
+000003e0: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
+000003f0: 257d 0a20 2020 203c 2f62 7574 746f 6e3e  %}.    </button>
+00000400: 0a20 2020 203c 6834 3e3c 6920 636c 6173  .    <h4><i clas
+00000410: 733d 2266 6173 2066 612d 6578 636c 616d  s="fas fa-exclam
+00000420: 6174 696f 6e2d 6369 7263 6c65 223e 3c2f  ation-circle"></
+00000430: 693e 2045 7272 6f72 3c2f 6834 3e0a 2020  i> Error</h4>.  
+00000440: 2020 3c64 6976 2069 643d 2266 6f72 6d5f    <div id="form_
+00000450: 7374 6172 745f 6572 726f 7273 223e 3c2f  start_errors"></
+00000460: 6469 763e 0a3c 2f64 6976 3e0a 0a50 6c65  div>.</div>..Ple
+00000470: 6173 6520 7365 6c65 6374 206f 6e65 206f  ase select one o
+00000480: 6620 7468 6520 666f 6c6c 6f77 696e 6720  f the following 
+00000490: 6f70 7469 6f6e 7320 746f 2041 6464 2079  options to Add y
+000004a0: 6f75 7220 5265 736f 7572 6365 2e20 596f  our Resource. Yo
+000004b0: 7520 6361 6e20 6372 6561 7465 2061 206e  u can create a n
+000004c0: 6577 2072 6573 6f75 7263 652c 206f 7220  ew resource, or 
+000004d0: 7570 6c6f 6164 2061 6e20 584d 4c20 6669  upload an XML fi
+000004e0: 6c65 2e0a 0a3c 6272 2f3e 3c62 722f 3e0a  le...<br/><br/>.
+000004f0: 3c64 6976 2069 643d 2266 6f72 6d5f 7374  <div id="form_st
+00000500: 6172 745f 636f 6e74 656e 7422 3e0a 3c2f  art_content">.</
+00000510: 6469 763e 0a3c 6469 7620 6964 3d22 7465  div>.<div id="te
+00000520: 6d70 6c61 7465 5f69 6422 2063 6c61 7373  mplate_id" class
+00000530: 3d22 6869 6464 656e 223e 7b7b 2064 6174  ="hidden">{{ dat
+00000540: 612e 7465 6d70 6c61 7465 5f69 6420 7d7d  a.template_id }}
+00000550: 3c2f 6469 763e 0a3c 6272 2f3e 3c62 722f  </div>.<br/><br/
+00000560: 3e0a 0a3c 6275 7474 6f6e 2069 643d 2262  >..<button id="b
+00000570: 746e 2d73 6176 652d 6461 7461 2220 636c  tn-save-data" cl
+00000580: 6173 733d 2262 746e 2062 746e 2d70 7269  ass="btn btn-pri
+00000590: 6d61 7279 2220 6869 6464 656e 3d22 223e  mary" hidden="">
+000005a0: 3c69 2063 6c61 7373 3d22 6661 7320 6661  <i class="fas fa
+000005b0: 2d73 6176 6522 3e3c 2f69 3e20 5361 7665  -save"></i> Save
+000005c0: 2077 6974 686f 7574 2065 6469 7469 6e67   without editing
+000005d0: 3c2f 6275 7474 6f6e 3e0a 3c62 7574 746f  </button>.<butto
+000005e0: 6e20 6964 3d22 6274 6e2d 6f70 656e 2d64  n id="btn-open-d
+000005f0: 6174 6122 2063 6c61 7373 3d22 6274 6e20  ata" class="btn 
+00000600: 6274 6e2d 7072 696d 6172 7922 3e3c 6920  btn-primary"><i 
+00000610: 636c 6173 733d 2266 6173 2066 612d 636f  class="fas fa-co
+00000620: 6465 223e 3c2f 693e 204f 7065 6e20 696e  de"></i> Open in
+00000630: 2054 6578 7420 6564 6974 6f72 3c2f 6275   Text editor</bu
+00000640: 7474 6f6e 3e0a 3c62 7574 746f 6e20 6964  tton>.<button id
+00000650: 3d22 6274 6e2d 6469 7370 6c61 792d 6461  ="btn-display-da
+00000660: 7461 2220 636c 6173 733d 2262 746e 2062  ta" class="btn b
+00000670: 746e 2d70 7269 6d61 7279 223e 3c69 2063  tn-primary"><i c
+00000680: 6c61 7373 3d22 6661 7320 6661 2d70 6c61  lass="fas fa-pla
+00000690: 7922 3e3c 2f69 3e20 5374 6172 7420 6564  y"></i> Start ed
+000006a0: 6974 696e 673c 2f62 7574 746f 6e3e 0a3c  iting</button>.<
+000006b0: 6469 7620 6964 3d22 726f 6c65 2220 636c  div id="role" cl
+000006c0: 6173 733d 2268 6964 6465 6e22 3e7b 7b20  ass="hidden">{{ 
+000006d0: 6461 7461 2e72 6f6c 6520 7d7d 3c2f 6469  data.role }}</di
+000006e0: 763e                                     v>
```

### Comparing `core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/curate_start.html` & `core_curate_registry_app-2.4.0/core_curate_registry_app/templates/core_curate_app/user/curate_start.html`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/enter_data.html` & `core_curate_registry_app-2.4.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/enter_data.html`

 * *Files 26% similar despite different names*

```diff
@@ -8,20 +8,20 @@
         {% else %}
         {% if data.edit %}Edit{% else %}Add new{% endif %} Resource
         {% endif %}
     </h3>
 </div>
 
 <div class="toolbar">
-	<div class="float-right">
-		<button class="btn btn-danger clear-fields mr-auto"><i class="fas fa-eraser"></i> Clear Fields </button>
-        <button class="btn btn-danger cancel-changes mr-auto"><i class="fas fa-sync"></i> Cancel Changes </button>
-        <button class="btn btn-danger cancel-form mr-auto"><i class="fas fa-trash"></i> Delete {% trans "form_label"|title %} </button>
-    	<button class="btn btn-secondary save-form-registry mr-auto"><i class="fas fa-save"></i> Save {% trans "form_label"|title %} </button>
-        <a href= "{% url 'core_curate_download_xml' data.data_structure.id %}" class="btn btn-secondary download-registry mr-auto"><i class="fas fa-download"></i> Download </a>
+	<div class="{% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}">
+		<button class="btn btn-danger clear-fields {% if BOOTSTRAP_VERSION == "4.6.2" %}mr-auto{% elif BOOTSTRAP_VERSION == "5.1.3" %}me-auto{% endif %}"><i class="fas fa-eraser"></i> Clear Fields </button>
+        <button class="btn btn-danger cancel-changes {% if BOOTSTRAP_VERSION == "4.6.2" %}mr-auto{% elif BOOTSTRAP_VERSION == "5.1.3" %}me-auto{% endif %}"><i class="fas fa-sync"></i> Cancel Changes </button>
+        <button class="btn btn-danger cancel-form {% if BOOTSTRAP_VERSION == "4.6.2" %}mr-auto{% elif BOOTSTRAP_VERSION == "5.1.3" %}me-auto{% endif %}"><i class="fas fa-trash"></i> Delete {% trans "form_label"|title %} </button>
+    	<button class="btn btn-secondary save-form-registry {% if BOOTSTRAP_VERSION == "4.6.2" %}mr-auto{% elif BOOTSTRAP_VERSION == "5.1.3" %}me-auto{% endif %}"><i class="fas fa-save"></i> Save {% trans "form_label"|title %} </button>
+        <a href= "{% url 'core_curate_download_xml' data.data_structure.id %}" class="btn btn-secondary download-registry {% if BOOTSTRAP_VERSION == "4.6.2" %}mr-auto{% elif BOOTSTRAP_VERSION == "5.1.3" %}me-auto{% endif %}"><i class="fas fa-download"></i> Download </a>
         <button class="btn btn-primary validate"><i class="fas fa-check-square"></i> Validate &rarr; Review </button>
 
 	</div>
     <br/><br/>
 
     <span>Title: {{data.data_structure.name}}</span>
     <div id = "data_title" class = "hidden" >
```

#### html2text {}

```diff
@@ -1,14 +1,23 @@
 {% load i18n %}
 {% if data.role_choice %}  {% if data.edit %}Edit{% else %}Add a new{% endif %}
 {{data.role_choice}} {% else %} {% if data.edit %}Edit{% else %}Add new{% endif
 %} Resource {% endif %}
- Clear Fields   Cancel Changes   Delete {% trans "form_label"|title %}   Save
+.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif
+%}">
+.6.2" %}mr-auto{% elif BOOTSTRAP_VERSION == "5.1.3" %}me-auto{% endif %}">
+Clear Fields
+.6.2" %}mr-auto{% elif BOOTSTRAP_VERSION == "5.1.3" %}me-auto{% endif %}">
+Cancel Changes
+.6.2" %}mr-auto{% elif BOOTSTRAP_VERSION == "5.1.3" %}me-auto{% endif %}">
+Delete {% trans "form_label"|title %}
+.6.2" %}mr-auto{% elif BOOTSTRAP_VERSION == "5.1.3" %}me-auto{% endif %}"> Save
 {% trans "form_label"|title %}
- Download
+.6.2" %}mr-auto{% elif BOOTSTRAP_VERSION == "5.1.3" %}me-auto{% endif %}">
+Download
   Validate → Review
 
 
 Title: {{data.data_structure.name}}
 {{data.data_structure.name}}
 {{data.xsd_form|safe}}
 {{ data.data_structure.id }}
```

### Comparing `core_curate_registry_app-2.3.0/core_curate_registry_app/templates/core_curate_app/user/data-review/modals/save-form-registry.html` & `core_curate_registry_app-2.4.0/core_curate_registry_app/templates/core_curate_app/user/data-review/modals/save-form-registry.html`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 {% endblock %}
 
 {% block modal_footer %}
     <div class="container">
         <div class="row">
             <div class="col-8">
                 <div class="d-flex justify-content-start">
-                    <a class="btn btn-danger mr-1" href="{% url 'core_curate_index' %}">
+                    <a class="btn btn-danger {% if BOOTSTRAP_VERSION == "4.6.2" %}mr-1{% elif BOOTSTRAP_VERSION == "5.1.3" %}me-1{% endif %}" href="{% url 'core_curate_index' %}">
                         <i class="fas fa-home"></i> No, go to curate page
                     </a>
                     <a class="btn btn-danger" href="{% url 'core_dashboard_records' %}">
                         <i class="fas fa-home"></i> No, go to resource page
                     </a>
                 </div>
             </div>
```

### Comparing `core_curate_registry_app-2.3.0/core_curate_registry_app/urls.py` & `core_curate_registry_app-2.4.0/core_curate_registry_app/urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """ Url router for the curate application
 """
+from core_curate_app.rest.curate_data_structure.views import (
+    CurateDataStructureDetail,
+)
 from django.conf.urls import include
 from django.urls import re_path
 
 import core_curate_app.views.user.ajax as user_ajax
 import core_curate_app.views.user.views as user_views
 import core_curate_registry_app.views.user.ajax as user_registry_ajax
 import core_curate_registry_app.views.user.views as user_registry_views
@@ -97,9 +100,14 @@
         r"^xml-editor/form",
         permission_required(
             content_type=rights.CURATE_CONTENT_TYPE,
             permission=rights.CURATE_DATA_STRUCTURE_ACCESS,
         )(common_views.DraftContentEditor.as_view()),
         name="core_curate_app_xml_text_editor_view",
     ),
+    re_path(
+        r"^draft/(?P<pk>\w+)/$",
+        CurateDataStructureDetail.as_view(),
+        name="core_curate_app_rest_draft_detail",
+    ),
     re_path(r"^rest/", include("core_curate_registry_app.rest.urls")),
 ]
```

### Comparing `core_curate_registry_app-2.3.0/core_curate_registry_app/views/user/ajax.py` & `core_curate_registry_app-2.4.0/core_curate_registry_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.3.0/core_curate_registry_app/views/user/views.py` & `core_curate_registry_app-2.4.0/core_curate_registry_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.3.0/core_curate_registry_app.egg-info/PKG-INFO` & `core_curate_registry_app-2.4.0/core_curate_registry_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-curate-registry-app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Curation functionalities specific to Registry applications for the curator core project
 Home-page: https://github.com/usnistgov/core_curate_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: Core Curate Registry App
         ========================
```

### Comparing `core_curate_registry_app-2.3.0/core_curate_registry_app.egg-info/SOURCES.txt` & `core_curate_registry_app-2.4.0/core_curate_registry_app.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,8 +40,9 @@
 core_curate_registry_app/views/__init__.py
 core_curate_registry_app/views/user/__init__.py
 core_curate_registry_app/views/user/ajax.py
 core_curate_registry_app/views/user/views.py
 tests/__init__.py
 tests/test_settings.py
 tests/utils/__init__.py
+tests/utils/test_unit_urls.py
 tests/utils/test_units.py
```

### Comparing `core_curate_registry_app-2.3.0/setup.py` & `core_curate_registry_app-2.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 chdir(normpath(join(abspath(__file__), pardir)))
 
 dep_links = [r for r in required if r.startswith("https://")]
 required = [req_link(r) if r.startswith("https://") else r for r in required]
 
 setup(
     name="core_curate_registry_app",
-    version="2.3.0",
+    version="2.4.0",
     description="Curation functionalities specific to Registry applications for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_curate_registry_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_curate_registry_app-2.3.0/tests/test_settings.py` & `core_curate_registry_app-2.4.0/tests/test_settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,18 @@
     "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.sites",
     # Local apps
+    "core_main_app",
+    "core_main_registry_app",
+    "core_parser_app",
+    "core_curate_app",
     "tests",
 ]
 
 MIDDLEWARE = (
     "django.contrib.auth.middleware.AuthenticationMiddleware",
     "django.contrib.messages.middleware.MessageMiddleware",
     "django.contrib.sessions.middleware.SessionMiddleware",
@@ -33,9 +37,11 @@
                 "django.contrib.auth.context_processors.auth",
                 "django.contrib.messages.context_processors.messages",
                 "django.template.context_processors.i18n",
             ],
         },
     },
 ]
+ROOT_URLCONF = "core_curate_registry_app.urls"
 MONGODB_INDEXING = False
 MONGODB_ASYNC_SAVE = False
+CELERYBEAT_SCHEDULER = "django_celery_beat.schedulers:DatabaseScheduler"
```

### Comparing `core_curate_registry_app-2.3.0/tests/utils/test_units.py` & `core_curate_registry_app-2.4.0/tests/utils/test_units.py`

 * *Files identical despite different names*

