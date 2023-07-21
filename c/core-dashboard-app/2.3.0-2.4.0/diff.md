# Comparing `tmp/core_dashboard_app-2.3.0.tar.gz` & `tmp/core_dashboard_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_dashboard_app-2.3.0.tar", last modified: Tue May  2 19:36:09 2023, max compression
+gzip compressed data, was "core_dashboard_app-2.4.0.tar", last modified: Fri Jul 21 02:10:21 2023, max compression
```

## Comparing `core_dashboard_app-2.3.0.tar` & `core_dashboard_app-2.4.0.tar`

### file list

```diff
@@ -1,66 +1,69 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.755907 core_dashboard_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:36:06.000000 core_dashboard_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      144 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1080 2023-05-02 19:36:09.751021 core_dashboard_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      579 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.351952 core_dashboard_app-2.3.0/core_dashboard_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4595 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3262 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/menus.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      407 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.106711 core_dashboard_app-2.3.0/core_dashboard_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.130807 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.112427 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.445096 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/admin/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       93 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/admin/js/my_dashboard_tabs.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.125549 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.457693 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/common/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       74 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/common/css/my_dashboard_tabs.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.469998 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/common/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      605 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/common/js/my_dashboard_tabs.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.134062 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.481581 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/user/js/my_dashboard_tabs.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.143832 core_dashboard_app-2.3.0/core_dashboard_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.177462 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.509808 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      323 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/admin/my_dashboard_container.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1150 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/admin/my_dashboard_content.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.173389 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.536161 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/common/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1720 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/common/list/my_dashboard_tabs.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      176 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/common/list/my_dashboard_tabs_file_pagination.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.549138 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/common/pagination/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2681 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/common/pagination/pagination_tab.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.561730 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      343 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/user/my_dashboard_container.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3885 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.574128 core_dashboard_app-2.3.0/core_dashboard_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.605603 core_dashboard_app-2.3.0/core_dashboard_app/views/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/views/common/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10514 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/core_dashboard_app/views/common/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.430864 core_dashboard_app-2.3.0/core_dashboard_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1080 2023-05-02 19:36:08.000000 core_dashboard_app-2.3.0/core_dashboard_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1597 2023-05-02 19:36:09.000000 core_dashboard_app-2.3.0/core_dashboard_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:36:08.000000 core_dashboard_app-2.3.0/core_dashboard_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      111 2023-05-02 19:36:08.000000 core_dashboard_app-2.3.0/core_dashboard_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-05-02 19:36:08.000000 core_dashboard_app-2.3.0/core_dashboard_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.653544 core_dashboard_app-2.3.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11302 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       85 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:36:09.757864 core_dashboard_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1077 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.678652 core_dashboard_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1621 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.689576 core_dashboard_app-2.3.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.705675 core_dashboard_app-2.3.0/tests/views/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/tests/views/common/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:09.741517 core_dashboard_app-2.3.0/tests/views/common/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/tests/views/common/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4784 2023-05-02 19:36:07.000000 core_dashboard_app-2.3.0/tests/views/common/views/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:21.700297 core_dashboard_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      144 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1080 2023-07-21 02:10:21.695293 core_dashboard_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      579 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:21.262667 core_dashboard_app-2.4.0/core_dashboard_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/core_dashboard_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4595 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/core_dashboard_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3262 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/core_dashboard_app/menus.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      407 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/core_dashboard_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:20.981280 core_dashboard_app-2.4.0/core_dashboard_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:21.004920 core_dashboard_app-2.4.0/core_dashboard_app/static/core_dashboard_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:20.987574 core_dashboard_app-2.4.0/core_dashboard_app/static/core_dashboard_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:21.349721 core_dashboard_app-2.4.0/core_dashboard_app/static/core_dashboard_app/admin/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       93 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/core_dashboard_app/static/core_dashboard_app/admin/js/my_dashboard_tabs.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:20.999597 core_dashboard_app-2.4.0/core_dashboard_app/static/core_dashboard_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:21.362089 core_dashboard_app-2.4.0/core_dashboard_app/static/core_dashboard_app/common/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       74 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/core_dashboard_app/static/core_dashboard_app/common/css/my_dashboard_tabs.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:21.373650 core_dashboard_app-2.4.0/core_dashboard_app/static/core_dashboard_app/common/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      605 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/core_dashboard_app/static/core_dashboard_app/common/js/my_dashboard_tabs.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:21.007689 core_dashboard_app-2.4.0/core_dashboard_app/static/core_dashboard_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:21.384479 core_dashboard_app-2.4.0/core_dashboard_app/static/core_dashboard_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/core_dashboard_app/static/core_dashboard_app/user/js/my_dashboard_tabs.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:21.017394 core_dashboard_app-2.4.0/core_dashboard_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:21.055293 core_dashboard_app-2.4.0/core_dashboard_app/templates/core_dashboard_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:21.414758 core_dashboard_app-2.4.0/core_dashboard_app/templates/core_dashboard_app/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      323 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/core_dashboard_app/templates/core_dashboard_app/admin/my_dashboard_container.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1251 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/core_dashboard_app/templates/core_dashboard_app/admin/my_dashboard_content.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:21.051296 core_dashboard_app-2.4.0/core_dashboard_app/templates/core_dashboard_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:21.440613 core_dashboard_app-2.4.0/core_dashboard_app/templates/core_dashboard_app/common/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1720 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/core_dashboard_app/templates/core_dashboard_app/common/list/my_dashboard_tabs.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      176 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/core_dashboard_app/templates/core_dashboard_app/common/list/my_dashboard_tabs_file_pagination.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:21.453049 core_dashboard_app-2.4.0/core_dashboard_app/templates/core_dashboard_app/common/pagination/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2681 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/core_dashboard_app/templates/core_dashboard_app/common/pagination/pagination_tab.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:21.465613 core_dashboard_app-2.4.0/core_dashboard_app/templates/core_dashboard_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      438 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/core_dashboard_app/templates/core_dashboard_app/user/my_dashboard_container.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3488 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/core_dashboard_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:21.477365 core_dashboard_app-2.4.0/core_dashboard_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/core_dashboard_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:21.508017 core_dashboard_app-2.4.0/core_dashboard_app/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/core_dashboard_app/views/common/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13038 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/core_dashboard_app/views/common/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:21.333803 core_dashboard_app-2.4.0/core_dashboard_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1080 2023-07-21 02:10:20.000000 core_dashboard_app-2.4.0/core_dashboard_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1673 2023-07-21 02:10:20.000000 core_dashboard_app-2.4.0/core_dashboard_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:10:20.000000 core_dashboard_app-2.4.0/core_dashboard_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      111 2023-07-21 02:10:20.000000 core_dashboard_app-2.4.0/core_dashboard_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-07-21 02:10:20.000000 core_dashboard_app-2.4.0/core_dashboard_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:21.541302 core_dashboard_app-2.4.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11302 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       85 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:10:21.701834 core_dashboard_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1077 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:21.578854 core_dashboard_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1812 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      467 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:21.609705 core_dashboard_app-2.4.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:21.620061 core_dashboard_app-2.4.0/tests/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/tests/views/common/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:21.680853 core_dashboard_app-2.4.0/tests/views/common/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/tests/views/common/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1226 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/tests/views/common/views/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6501 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/tests/views/common/views/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1893 2023-07-21 02:10:19.000000 core_dashboard_app-2.4.0/tests/views/fixtures.py
```

### Comparing `core_dashboard_app-2.3.0/LICENSE.md` & `core_dashboard_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.3.0/PKG-INFO` & `core_dashboard_app-2.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_dashboard_app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Resource management via a dashboard for the curator core project
 Home-page: https://github.com/usnistgov/core_dashboard_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ==================
         Core Dashboard App
```

### Comparing `core_dashboard_app-2.3.0/README.rst` & `core_dashboard_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.3.0/core_dashboard_app/admin.py` & `core_dashboard_app-2.4.0/core_dashboard_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.3.0/core_dashboard_app/menus.py` & `core_dashboard_app-2.4.0/core_dashboard_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.3.0/core_dashboard_app/static/core_dashboard_app/common/js/my_dashboard_tabs.js` & `core_dashboard_app-2.4.0/core_dashboard_app/static/core_dashboard_app/common/js/my_dashboard_tabs.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/admin/my_dashboard_content.html` & `core_dashboard_app-2.4.0/core_dashboard_app/templates/core_dashboard_app/admin/my_dashboard_content.html`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
          <i class="fas fa-arrow-left"></i> Previous page
     </a>
 {% endblock %}
 
 {% block box_body %}
     {% if data.menu and not data.title %}
         <div class="dropdown" id="id_actions" style="display:none">
-            <button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenu1" data-toggle="dropdown" aria-haspopup="true" aria-expanded="true">
+            <button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenu1" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-toggle{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-toggle{% endif %}="dropdown" aria-haspopup="true" aria-expanded="true">
                 Choose action
                 <span class="caret"></span>
             </button>
             <ul class="dropdown-menu">
                 {% for value, text in data.action_form.fields.actions.choices %}
                     <li style="cursor:  pointer;" onclick="action_dashboard({{value}});">{{text}}</li>
                 {% endfor %}
```

#### html2text {}

```diff
@@ -1,11 +1,13 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% block
 box_title %}{{data.title}}{% endblock %} {% block box_tools %}
  Previous_page
  {% endblock %} {% block box_body %} {% if data.menu and not data.title %}
- Choose action
+% if BOOTSTRAP_VERSION == "4.6.2" %}data-toggle{% elif BOOTSTRAP_VERSION ==
+"5.1.3" %}data-bs-toggle{% endif %}="dropdown" aria-haspopup="true" aria-
+expanded="true"> Choose action
     * {% for value, text in data.action_form.fields.actions.choices %}
     * {{text}}
     * {% endfor %}
 {% endif %}
 {% include data.template with objects=data.user_data group='user' %}
 {% endblock %}
```

### Comparing `core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/common/list/my_dashboard_tabs.html` & `core_dashboard_app-2.4.0/core_dashboard_app/templates/core_dashboard_app/common/list/my_dashboard_tabs.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.3.0/core_dashboard_app/templates/core_dashboard_app/common/pagination/pagination_tab.html` & `core_dashboard_app-2.4.0/core_dashboard_app/templates/core_dashboard_app/common/pagination/pagination_tab.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.3.0/core_dashboard_app/urls.py` & `core_dashboard_app-2.4.0/core_dashboard_app/urls.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 from django.urls import reverse_lazy
 
 from core_dashboard_app.views.common import views as dashboard_app_common_views
 from core_dashboard_common_app.views.common import (
     ajax,
     views as dashboard_common_app_common_views,
 )
-from core_dashboard_common_app.views.common.views import (
-    UserDashboardPasswordChangeFormView,
-)
 from core_main_app.settings import INSTALLED_APPS
 from core_main_app.views.common.ajax import EditTemplateVersionManagerView
 
 urlpatterns = [
     # Common
     re_path(
         r"^$",
@@ -30,22 +27,14 @@
     ),
     re_path(
         r"^my-profile/edit$",
         dashboard_common_app_common_views.my_profile_edit,
         name="core_dashboard_profile_edit",
     ),
     re_path(
-        r"^my-profile/change-password",
-        UserDashboardPasswordChangeFormView.as_view(
-            template_name="core_dashboard_common_app/my_profile_change_password.html",
-            success_url="/",
-        ),
-        name="core_dashboard_profile_change_password",
-    ),
-    re_path(
         r"^delete-document",
         ajax.delete_document,
         name="core_dashboard_delete_document",
     ),
     re_path(
         r"^change-owner",
         ajax.change_owner_document,
```

### Comparing `core_dashboard_app-2.3.0/core_dashboard_app/views/common/views.py` & `core_dashboard_app-2.4.0/core_dashboard_app/views/common/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 """ User Views
 """
 import copy
 
+from core_main_app.components.workspace.api import (
+    check_if_workspace_can_be_changed,
+)
+
 from django.core.exceptions import ObjectDoesNotExist
 from django.urls import reverse
-
+from core_dashboard_common_app import settings as dashboard_settings
 from core_dashboard_common_app import constants as dashboard_constants
-from core_dashboard_common_app import settings
 from core_dashboard_common_app.views.common.forms import UserForm
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.commons import exceptions
+from core_main_app.commons.exceptions import DoesNotExist
 from core_main_app.components.blob import api as workspace_blob_api
 from core_main_app.components.blob import utils as blob_utils
 from core_main_app.components.data import api as workspace_data_api
 from core_main_app.components.user import api as user_api
 from core_main_app.components.workspace import api as workspace_api
-from core_main_app.settings import INSTALLED_APPS
+from django.conf import settings
 from core_main_app.utils.pagination.django_paginator.results_paginator import (
     ResultsPaginator,
 )
 from core_main_app.views.common.views import CommonView
 
+if "core_curate_app" in settings.INSTALLED_APPS:
+    import core_curate_app.components.curate_data_structure.api as curate_data_structure_api
+
 
 class DashboardWorkspaceTabs(CommonView):
     """Workspace Tab Page"""
 
     template = "core_dashboard_app/user/my_dashboard_container.html"
     data_template = "core_dashboard_app/common/list/my_dashboard_tabs.html"
 
@@ -93,15 +100,17 @@
         user_can_write = workspace_api.can_user_write_workspace(
             workspace, request.user
         )
 
         # Paginator
         page = request.GET.get("page", 1)
         results_paginator = ResultsPaginator.get_results(
-            items_to_render, page, settings.RECORD_PER_PAGE_PAGINATION
+            items_to_render,
+            page,
+            dashboard_settings.RECORD_PER_PAGE_PAGINATION,
         )
 
         # Data context
         results_paginator.object_list = self._format_document_context(
             request,
             results_paginator.object_list,
             user_can_read,
@@ -122,14 +131,16 @@
                 "username_list": user_api.get_id_username_dict(
                     user_api.get_all_users()
                 ),
                 "tab": tab_selected,
                 "title": workspace.title,
                 "number_total_data": data_count,
                 "number_total_files": files_count,
+                "share_pid_button": "core_linked_records_app"
+                in settings.INSTALLED_APPS,
             }
         )
 
         if self.administration and workspace.owner:
             context.update(
                 {
                     "owner": user_api.get_user_by_id(workspace.owner).username,
@@ -144,32 +155,54 @@
             (str(x.id), x.username) for x in user_api.get_all_users()
         )
         context.update({"usernames": user_names})
 
         modals = [
             dashboard_constants.MODALS_COMMON_CHANGE_OWNER,
             dashboard_constants.MODALS_COMMON_DELETE,
+            "core_main_app/user/workspaces/list/modals/assign_workspace.html",
         ]
 
         assets = self._get_assets()
 
-        if "core_file_preview_app" in INSTALLED_APPS:
+        if "core_file_preview_app" in settings.INSTALLED_APPS:
             assets["js"].extend(
                 [
                     {
                         "path": "core_file_preview_app/user/js/file_preview.js",
                         "is_raw": False,
                     }
                 ]
             )
             assets["css"].append(
                 "core_file_preview_app/user/css/file_preview.css"
             )
             modals.append("core_file_preview_app/user/file_preview_modal.html")
 
+        if context["share_pid_button"]:
+            modals.append(
+                "core_linked_records_app/user/sharing/data_detail/modal.html"
+            )
+            assets["css"].append("core_main_app/common/css/share_link.css"),
+
+            assets["js"] += [
+                {
+                    "path": "core_main_app/user/js/sharing_modal.js",
+                    "is_raw": False,
+                },
+                {
+                    "path": "core_linked_records_app/user/js/sharing/common_list.js",
+                    "is_raw": False,
+                },
+                {
+                    "path": "core_linked_records_app/user/js/sharing/data_list.js",
+                    "is_raw": False,
+                },
+            ]
+
         # Set page title
         context.update({"page_title": "Dashboard"})
         return self.common_render(
             request,
             self.template,
             context=context,
             assets=assets,
@@ -189,49 +222,78 @@
         for document in document_list:
             is_owner = (
                 str(document.user_id) == str(user.id) or self.administration
             )
             document_context = {
                 "can_read": user_can_read or is_owner,
                 "can_write": user_can_write or is_owner,
+                "can_change_workspace": check_if_workspace_can_be_changed(
+                    document
+                ),
+                "is_owner": is_owner,
             }
             if tab_selected == "data":
+                forms_count = (
+                    len(
+                        curate_data_structure_api.get_all_curate_data_structures_by_data(
+                            document, user
+                        )
+                    )
+                    if self.administration
+                    else 0
+                )
                 document_context.update(
-                    {"data": document, "is_owner": is_owner}
+                    {
+                        "data": document,
+                        "form_id": self._get_form(document, user),
+                        "forms_count": forms_count,
+                    }
                 )
             elif tab_selected == "file":
                 try:
                     username = user_api.get_user_by_id(
                         document.user_id
                     ).username
                 except ObjectDoesNotExist:
                     username = "None"
                 document_context.update(
                     {
                         "file": document,
-                        "url": blob_utils.get_blob_download_uri(
+                        "url": f"{reverse('core_main_app_blob_detail')}?id={document.id}",
+                        "download_url": blob_utils.get_blob_download_uri(
                             document, request
                         ),
                         "user": username,
                         "date": document.creation_date,
-                        "is_owner": is_owner,
                     }
                 )
             detailed_documents.append(document_context)
         return detailed_documents
 
+    def _get_form(self, data, user):
+        try:
+            return curate_data_structure_api.get_by_data_id_and_user(
+                data.id, user
+            ).id
+        except DoesNotExist:
+            return None
+
     def _get_assets(self):
         assets = {
             "css": copy.deepcopy(dashboard_constants.CSS_COMMON),
             "js": [
                 {
                     "path": "core_main_app/user/js/workspaces/list/modals/assign_workspace.js",
                     "is_raw": False,
                 },
                 {
+                    "path": "core_main_app/user/js/workspaces/list/modals/assign_data_workspace.raw.js",
+                    "is_raw": True,
+                },
+                {
                     "path": dashboard_constants.USER_VIEW_RECORD_RAW,
                     "is_raw": True,
                 },
                 {"path": dashboard_constants.JS_EDIT_RECORD, "is_raw": False},
                 {
                     "path": dashboard_constants.JS_USER_SELECTED_ELEMENT,
                     "is_raw": False,
@@ -261,14 +323,18 @@
                     "path": dashboard_constants.JS_COMMON_FUNCTION_DELETE,
                     "is_raw": False,
                 },
                 {
                     "path": "core_dashboard_app/common/js/my_dashboard_tabs.js",
                     "is_raw": False,
                 },
+                {
+                    "path": "core_dashboard_common_app/common/js/list/delete_data_draft.js",
+                    "is_raw": False,
+                },
             ],
         }
 
         assets["css"].append(
             "core_dashboard_app/common/css/my_dashboard_tabs.css"
         )
```

### Comparing `core_dashboard_app-2.3.0/core_dashboard_app.egg-info/PKG-INFO` & `core_dashboard_app-2.4.0/core_dashboard_app.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-dashboard-app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Resource management via a dashboard for the curator core project
 Home-page: https://github.com/usnistgov/core_dashboard_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ==================
         Core Dashboard App
```

### Comparing `core_dashboard_app-2.3.0/core_dashboard_app.egg-info/SOURCES.txt` & `core_dashboard_app-2.4.0/core_dashboard_app.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -28,11 +28,14 @@
 core_dashboard_app/views/common/__init__.py
 core_dashboard_app/views/common/views.py
 docs/__init__.py
 docs/conf.py
 docs/conf_urls.py
 tests/__init__.py
 tests/test_settings.py
+tests/urls.py
 tests/views/__init__.py
+tests/views/fixtures.py
 tests/views/common/__init__.py
 tests/views/common/views/__init__.py
+tests/views/common/views/tests_int.py
 tests/views/common/views/tests_unit.py
```

### Comparing `core_dashboard_app-2.3.0/docs/conf.py` & `core_dashboard_app-2.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.3.0/setup.py` & `core_dashboard_app-2.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_dashboard_app",
-    version="2.3.0",
+    version="2.4.0",
     description="Resource management via a dashboard for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_dashboard_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_dashboard_app-2.3.0/tests/test_settings.py` & `core_dashboard_app-2.4.0/tests/test_settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,16 +7,23 @@
     # Django apps
     "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.sites",
+    # Extra apps
+    "django_celery_beat",
     # Local apps
     "core_main_app",
+    "core_dashboard_common_app",
+    "core_dashboard_app",
+    "core_parser_app",
+    "core_curate_app",
+    "core_explore_common_app",
     "tests",
 ]
 
 # IN-MEMORY TEST DATABASE
 DATABASES = {
     "default": {
         "ENGINE": "django.db.backends.sqlite3",
@@ -28,15 +35,14 @@
     },
 }
 
 MIDDLEWARE = (
     "django.contrib.auth.middleware.AuthenticationMiddleware",
     "django.contrib.messages.middleware.MessageMiddleware",
     "django.contrib.sessions.middleware.SessionMiddleware",
-    "tz_detect.middleware.TimezoneMiddleware",
 )
 
 TEMPLATES = [
     {
         "BACKEND": "django.template.backends.django.DjangoTemplates",
         "DIRS": ["templates"],
         "APP_DIRS": True,
@@ -54,9 +60,10 @@
 ]
 
 CELERYBEAT_SCHEDULER = "django_celery_beat.schedulers:DatabaseScheduler"
 CUSTOM_NAME = "Curator"
 
 MONGODB_INDEXING = False
 MONGODB_ASYNC_SAVE = False
-
+ROOT_URLCONF = "tests.urls"
 ENABLE_SAML2_SSO_AUTH = False
+RECORD_PER_PAGE_PAGINATION = 10
```

### Comparing `core_dashboard_app-2.3.0/tests/views/common/views/tests_unit.py` & `core_dashboard_app-2.4.0/tests/views/common/views/tests_unit.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """ Unit tests on common dashboard views.
 """
 from unittest import TestCase
 from unittest.mock import patch
 
+from django.test import override_settings
+
 from core_dashboard_app.views.common import views as common_views
 from core_main_app.commons import exceptions
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 from core_main_app.components.workspace import api as workspace_api
 from core_main_app.components.data import api as data_api
 from core_main_app.components.blob import api as blob_api
@@ -119,7 +121,52 @@
             self.workspace_records_view.as_view(),
             self.user,
             param={"workspace_id": 42},
         )
 
         self.assertIn("owner", response.keys())
         self.assertIn("owner_change_url", response.keys())
+
+    @patch.object(workspace_api, "get_by_id")
+    @patch.object(data_api, "get_all_by_workspace")
+    @patch.object(blob_api, "get_all_by_workspace")
+    @patch.object(workspace_api, "can_user_read_workspace")
+    @patch.object(workspace_api, "can_user_write_workspace")
+    @patch.object(common_views, "ResultsPaginator")
+    @patch.object(common_views, "UserForm")
+    @patch.object(user_api, "get_id_username_dict")
+    @patch.object(user_api, "get_all_users")
+    @patch.object(user_api, "get_user_by_id")
+    @patch.object(common_views.DashboardWorkspaceTabs, "common_render")
+    @override_settings(
+        INSTALLED_APPS=[
+            "core_main_app",
+            "core_dashboard_common_app",
+            "core_linked_records_app",
+        ]
+    )
+    def test_user_side_context_has_share_pid_btn(
+        self,
+        mock_common_render,
+        mock_get_user_by_id,
+        mock_get_all_users,
+        mock_get_id_username_dict,
+        mock_user_form,
+        mock_results_paginator,
+        mock_can_user_write_workspace,
+        mock_can_user_read_workspace,
+        mock_get_all_blob_by_workspace,
+        mock_get_all_data_by_workspace,
+        mock_workspace_get_by_id,
+    ):
+        """test_user_side_context_has_share_pid_btn"""
+        mock_common_render.side_effect = self.mock_render_only_context
+
+        self.workspace_records_view.administration = False
+        response = RequestMock.do_request_get(
+            self.workspace_records_view.as_view(),
+            self.user,
+            param={"workspace_id": 42},
+        )
+
+        self.assertIn("share_pid_button", response.keys())
+        self.assertEquals(response["share_pid_button"], True)
```

