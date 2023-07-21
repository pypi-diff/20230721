# Comparing `tmp/core_dashboard_registry_app-2.3.0.tar.gz` & `tmp/core_dashboard_registry_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_dashboard_registry_app-2.3.0.tar", last modified: Tue May  2 19:36:38 2023, max compression
+gzip compressed data, was "core_dashboard_registry_app-2.4.0.tar", last modified: Fri Jul 21 02:10:42 2023, max compression
```

## Comparing `core_dashboard_registry_app-2.3.0.tar` & `core_dashboard_registry_app-2.4.0.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:38.191435 core_dashboard_registry_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      162 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1145 2023-05-02 19:36:38.185245 core_dashboard_registry_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      633 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.503217 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3446 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      661 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/constants.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2803 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/menus.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      415 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.231973 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.235153 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.248037 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.593119 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/home.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.605937 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1672 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/list/records.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.654413 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1056 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/get_url.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/get_url.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.724475 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/open_form.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      649 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/publish.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       72 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/publish.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1665 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/records.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/records.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1657 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/record_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      226 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/record_registry.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.270550 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.736823 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_common_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.780681 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2778 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4888 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table_pagination.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2960 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_common_app/my_dashboard.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.805457 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1180 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/home.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.861402 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1731 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_forms_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      192 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_forms_table_pagination.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5496 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_records_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_records_table_pagination.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3839 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.873824 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.889082 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/query/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.922689 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/query/django/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/query/django/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      622 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/query/django/prepare.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.954970 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/query/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/query/mongo/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      786 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/query/mongo/prepare.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.967110 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:38.037276 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/views/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/views/common/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3843 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/views/common/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      515 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/views/common/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17579 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/views/common/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:37.577747 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1145 2023-05-02 19:36:36.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3210 2023-05-02 19:36:37.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:36:36.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2023-05-02 19:36:36.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       34 2023-05-02 19:36:36.000000 core_dashboard_registry_app-2.3.0/core_dashboard_registry_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       94 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:36:38.193694 core_dashboard_registry_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1104 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:38.070918 core_dashboard_registry_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1809 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:38.097606 core_dashboard_registry_app-2.3.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/tests/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:38.134305 core_dashboard_registry_app-2.3.0/tests/utils/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/tests/utils/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3483 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/tests/utils/query/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:38.165993 core_dashboard_registry_app-2.3.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/tests/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14651 2023-05-02 19:36:35.000000 core_dashboard_registry_app-2.3.0/tests/views/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:42.274597 core_dashboard_registry_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      162 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1145 2023-07-21 02:10:42.270935 core_dashboard_registry_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      633 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:41.665719 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3446 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      661 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/constants.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2803 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/menus.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      415 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:41.401251 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:41.404312 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/static/core_dashboard_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:41.431678 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:41.729143 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/home.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:41.739862 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1722 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/list/records.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:41.784014 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1056 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/get_url.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/get_url.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:41.843745 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/open_form.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      637 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/publish.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       72 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/publish.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1732 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/records.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/records.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1657 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/record_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      226 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/record_registry.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:41.470425 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:41.855613 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/templates/core_dashboard_common_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:41.889663 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3453 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7272 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table_pagination.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3065 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/templates/core_dashboard_common_app/my_dashboard.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:41.900553 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1180 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/home.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:41.951611 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2121 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_forms_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      192 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_forms_table_pagination.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7145 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_records_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_records_table_pagination.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3442 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:41.998130 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:42.014189 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/utils/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/utils/query/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:42.043272 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/utils/query/django/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/utils/query/django/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      622 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/utils/query/django/prepare.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:42.068892 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/utils/query/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/utils/query/mongo/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      786 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/utils/query/mongo/prepare.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:42.082271 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:42.135122 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/views/common/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3843 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/views/common/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      515 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/views/common/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18759 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/views/common/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:41.717764 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1145 2023-07-21 02:10:41.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3224 2023-07-21 02:10:41.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:10:41.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2023-07-21 02:10:41.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       34 2023-07-21 02:10:41.000000 core_dashboard_registry_app-2.4.0/core_dashboard_registry_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       94 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:10:42.281171 core_dashboard_registry_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1104 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:42.179546 core_dashboard_registry_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1817 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      486 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:42.201187 core_dashboard_registry_app-2.4.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:39.000000 core_dashboard_registry_app-2.4.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:42.233047 core_dashboard_registry_app-2.4.0/tests/utils/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:40.000000 core_dashboard_registry_app-2.4.0/tests/utils/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3483 2023-07-21 02:10:40.000000 core_dashboard_registry_app-2.4.0/tests/utils/query/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:42.260914 core_dashboard_registry_app-2.4.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:40.000000 core_dashboard_registry_app-2.4.0/tests/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16201 2023-07-21 02:10:40.000000 core_dashboard_registry_app-2.4.0/tests/views/tests_unit.py
```

### Comparing `core_dashboard_registry_app-2.3.0/LICENSE.md` & `core_dashboard_registry_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.3.0/PKG-INFO` & `core_dashboard_registry_app-2.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_dashboard_registry_app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Resource management via a dashboard for the registry core project
 Home-page: https://github.com/usnistgov/core_dashboard_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: Core Dashboard Registry App
         ===========================
```

### Comparing `core_dashboard_registry_app-2.3.0/README.rst` & `core_dashboard_registry_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/admin.py` & `core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/constants.py` & `core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/constants.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/menus.py` & `core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/list/records.css` & `core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/list/records.css`

 * *Files 9% similar despite different names*

```diff
@@ -87,7 +87,11 @@
     max-width: 105px;
     width: 105px;
 }
 
 .label-status {
     padding-top: 12px;
 }
+
+.valign-top{
+    vertical-align:top !important;
+}
```

### Comparing `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/get_url.js` & `core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/get_url.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/records.js` & `core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/records.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -12,22 +12,22 @@
             data: {
                 "data_id": data_id,
                 "new_status": new_status
             },
             success: function(data) {
                 btn_element.attr('class', 'dropbtn status-' + new_status);
                 btn_element.attr('data-status', new_status);
-                btn_element.closest('td').children('span.label-status').attr('class', 'float-right label-status font-' + new_status);
-                btn_element.closest('td').children('span.label-status').text(new_status);
+                var labelStatus = btn_element.closest('td').children('span.label-status')
+                var floatClass = labelStatus.attr('class').split(' ')[0]
+                labelStatus.attr('class', floatClass + ' label-status font-' + new_status);
+                labelStatus.text(new_status);
             },
             error: function(data) {
                 var errors = $.parseJSON(data.responseText);
-                $.notify(errors.message, {
-                    style: 'error'
-                });
+                $.notify(errors.message, "danger");
             }
         });
     }
 }
 
 // called when the webpage is loaded
 $(document).ready(function() {
```

### Comparing `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/record_registry.js` & `core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/record_registry.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html` & `core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html`

 * *Files 13% similar despite different names*

```diff
@@ -31,36 +31,43 @@
                 <td>
                     {% with key=data_loaded.form.user %}
                       {{ data.usernames|get:key }}
                     {% endwith %}
                 </td>
                 {% endif %}
                 <td>
-                    {% if come_from_admin %}
-                        <a class="btn btn-secondary view-form-btn"
-                           href="{% url 'core-admin:core_curate_view_form' data_loaded.form.id %}">
-                            <i class="far fa-file-alt"></i> View
+                    <a class="btn btn-secondary dropdown-toggle" type="button" id="dropdownActions" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-toggle{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-toggle{% endif %}="dropdown" aria-haspopup="true" aria-expanded="false">
+                        <i class="fas fa-sliders"></i> Actions
+                    </a>
+                    <div class="dropdown-menu" aria-labelledby="dropdownActions">
+                        {% if come_from_admin %}
+                            <a class="dropdown-item view-form-btn"
+                               href="{% url 'core-admin:core_curate_view_form' data_loaded.form.id %}">
+                                <i class="far fa-file-alt"></i> View
+                            </a>
+                        {% else %}
+                            <a class="dropdown-item view-form-btn"
+                               href="{% url 'core_curate_view_form' data_loaded.form.id %}">
+                                <i class="far fa-file-alt"></i> View
+                            </a>
+                        {% endif %}
+                        <div class="dropdown-divider"></div>
+                        <a class="dropdown-item edit-form-btn" href="{% url 'core_curate_enter_data' data_loaded.form.id %}">
+                            <i class="fas fa-edit"></i> Edit
                         </a>
-                    {% else %}
-                        <a class="btn btn-secondary view-form-btn"
-                           href="{% url 'core_curate_view_form' data_loaded.form.id %}">
-                            <i class="far fa-file-alt"></i> View
+                        <a class="dropdown-item open-form-btn" href="#">
+                            <i class="fas fa-code"></i> Open
                         </a>
-                    {% endif %}
-                    <a class="btn btn-secondary edit-form-btn" href="{% url 'core_curate_enter_data' data_loaded.form.id %}">
-                        <i class="fas fa-edit"></i> Edit
-                    </a>
-                    <a class="btn btn-secondary open-form-btn">
-                        <i class="fas fa-code"></i> Open
-                    </a>
-                    <a class="btn btn-secondary change-owner-btn">
-                        <i class="fas fa-user-circle"></i> Change Owner
-                    </a>
-                    <button class="btn btn-danger delete-document-btn">
-                        <i class="fas fa-trash"></i> Delete
-                    </button>
+                        <a class="dropdown-item change-owner-btn" href="#">
+                            <i class="fas fa-user-circle"></i> Change Owner
+                        </a>
+                        <div class="dropdown-divider"></div>
+                        <a class="dropdown-item delete-document-btn" href="#">
+                            <i class="fas fa-trash"></i> Delete
+                        </a>
+                    </div>
                 </td>
             </tr>
         {% endfor %}
     </tbody>
 </table>
 {% include 'core_main_app/common/pagination/data_source_pagination.html' with pagination=data.pagination%}
```

#### html2text {}

```diff
@@ -1,16 +1,31 @@
 {% load dict_key_extras %}
-                                                                   {% if
+                                                                   % if
+                                                                   BOOTSTRAP_VERSION
+                                                                   == "4.6.2"
+                                                                   %}data-toggle{%
+                                                                   elif
+                                                                   BOOTSTRAP_VERSION
+                                                                   == "5.1.3"
+                                                                   %}data-bs-toggle
+                                                                   {% endif
+                                                                   %}="dropdown"
+                                                                   aria-
+                                                                   haspopup="true"
+  {                     {                {% with                   aria-
+�{                     {                key=data_loaded.form.user expanded="false">
+  data_loaded.form.name data_loaded.role %} {{ data.usernames|get: Actions
+  }}                    }}               key }} {% endwith %}      {% if
                                                                    come_from_admin
                                                                    %}
                                                                     View
-  {                     {                {% with                    {% else %}
-  {                     {                key=data_loaded.form.user  View
-�data_loaded.form.name data_loaded.role %} {{ data.usernames|get:  {% endif %}
-  }}                    }}               key }} {% endwith %}       Edit
+                                                                    {% else %}
+                                                                    View
+                                                                    {% endif %}
+                                                                    Edit
 
                                                                     Open
 
-                                                                    Change Owner
-                                                                      Delete
+                                                                    Change_Owner
+                                                                    Delete
 {% include 'core_main_app/common/pagination/data_source_pagination.html' with
 pagination=data.pagination%}
```

### Comparing `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_common_app/my_dashboard.html` & `core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/templates/core_dashboard_common_app/my_dashboard.html`

 * *Files 11% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     {% if data.user_data %}
         Total number of {{data.document|special_plural}}: {{ data.number_total }}
     {% endif %}
 
     {% if data.menu and not data.title %}
         <div class="dropdown" id="id_actions" style="display:none">
-            <button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenu1" data-toggle="dropdown"
+            <button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenu1" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-toggle{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-toggle{% endif %}="dropdown"
                     aria-haspopup="true" aria-expanded="true">
                 Choose action
                 <span class="caret"></span>
             </button>
             <ul class="dropdown-menu">
                 {% for value, text in data.action_form.fields.actions.choices %}
                     <li style="cursor:  pointer;" onclick="action_dashboard({{value}});">{{text}}</li>
@@ -47,24 +47,24 @@
         </div>
     {% endif %}
 
     {% if data.resources %}
         {% include 'core_main_registry_app/resource_banner/resource_banner.html' %}
         <ul class="nav nav-tabs">
             <li class="nav-item pointer">
-                <a class="nav-link {% if data.ispublished == 'all' %}active{% endif%}" onclick="get_url('all', '');">All</a>
+                <a class="nav-link {% if data.ispublished == 'all' %}active{% endif %}" onclick="get_url('all', '');">All</a>
             </li>
             <li class="nav-item pointer">
-                <a class="nav-link {% if data.ispublished == 'published' %}active{% endif%}" onclick="get_url('published', '');">Published</a>
+                <a class="nav-link {% if data.ispublished == 'published' %}active{% endif %}" onclick="get_url('published', '');">Published</a>
             </li>
             <li class="nav-item pointer">
-                <a class="nav-link {% if data.ispublished == 'unpublished' %}active{% endif%}" onclick="get_url('unpublished', '');">Not Published</a>
+                <a class="nav-link {% if data.ispublished == 'unpublished' %}active{% endif %}" onclick="get_url('unpublished', '');">Not Published</a>
             </li>
             <li id="draft" class="nav-item pointer">
-                <a class="nav-link {% if data.ispublished == 'draft' %}active{% endif%}" onclick="get_url('draft', '');">Drafts</a>
+                <a class="nav-link {% if data.ispublished == 'draft' %}active{% endif %}" onclick="get_url('draft', '');">Drafts</a>
             </li>
         </ul>
     {% endif %}
 
     <div class="tab-content">
         {% if data.user_data %}
             {% include data.template with objects=data.user_data group='user' %}
```

#### html2text {}

```diff
@@ -8,15 +8,17 @@
  Previous_page
  {% endif %} {% endblock %} {% block box_body %} {% if data.administration and
 data.owner %}
 Owner: {{_data.owner_}}
 {% endif %} {% if data.user_data %} Total number of {
 {data.document|special_plural}}: {{ data.number_total }} {% endif %} {% if
 data.menu and not data.title %}
- Choose action
+% if BOOTSTRAP_VERSION == "4.6.2" %}data-toggle{% elif BOOTSTRAP_VERSION ==
+"5.1.3" %}data-bs-toggle{% endif %}="dropdown" aria-haspopup="true" aria-
+expanded="true"> Choose action
     * {% for value, text in data.action_form.fields.actions.choices %}
     * {{text}}
     * {% endfor %}
 {% endif %} {% if data.resources %} {% include 'core_main_registry_app/
 resource_banner/resource_banner.html' %}
     * All
     * Published
```

### Comparing `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/home.html` & `core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/home.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_records_table.html` & `core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_records_table.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 {% load dict_key_extras %}
-{% load draft_extras %}
 {% load timestamptags %}
+{% load special_plural %}
+{% load tz %}
 
 
 {% for data_loaded in objects %}
 <table class="table table-borderless table-card">
     <tr objectid="{{data_loaded.data.id}}">
-        <td class="px-3 pull-left">
+        <td class="px-3 pull-left valign-top">
             {% if data_loaded.can_read %}
-                <a class="view-record-btn font-weight-bold pointer">{{ data_loaded.data.title }}</a> ({{ data_loaded.data_role }})
+                <a class="view-record-btn font-weight-bold pointer fw-bold">{{ data_loaded.data.title }}</a> ({{ data_loaded.data_role }})
             {% else %}
                 <span style="font-weight: bold;">{{ data_loaded.data.title }}</span> ({{ data_loaded.data_role }})
             {% endif %}
-            {% if data_loaded.data|has_draft:request.user%}, <text class="text-danger">&nbsp;Draft</text>{% endif %}
+            {% if data.administration and data_loaded.forms_count > 0  %}
+                ,<text class="text-danger"> Draft{{ data_loaded.forms_count|pluralize }} </text>
+            {% elif data_loaded.form_id %}
+                ,<text class="text-danger"> Draft </text>
+            {% endif %}
 
         </td>
         <td class="cell-dropdown">
-            <span class="float-right dropdown">
+            <span class="{% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %} dropdown">
                 {% if data_loaded.data_status == data_loaded.data_status_values.ACTIVE  %}
                     <span data-status="active" class="dropbtn status-active pointer"></span>
                 {% endif %}
                 {% if data_loaded.data_status == data_loaded.data_status_values.INACTIVE  %}
                     <span data-status="inactive" class="dropbtn status-inactive pointer"></span>
                 {% endif %}
                 {% if data_loaded.data_status == data_loaded.data_status_values.DELETED  %}
@@ -31,21 +36,21 @@
                   <a data-status="inactive" class="switch font-inactive">Inactive</a>
                     {% if data_loaded.data.workspace.is_public %}
                         <a data-status="deleted" class="switch font-deleted">Deleted</a>
                     {% endif %}
               </div>
             </span>
             {% if data_loaded.data_status == data_loaded.data_status_values.ACTIVE  %}
-                <span class="float-right label-status font-active">Active</span>
+                <span class="{% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %} label-status font-active">Active</span>
             {% endif %}
             {% if data_loaded.data_status == data_loaded.data_status_values.INACTIVE  %}
-                <span class="float-right label-status font-inactive">Inactive</span>
+                <span class="{% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %} label-status font-inactive">Inactive</span>
             {% endif %}
             {% if data_loaded.data_status == data_loaded.data_status_values.DELETED  %}
-                <span class="float-right label-status font-deleted">Deleted</span>
+                <span class="{% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %} label-status font-deleted">Deleted</span>
             {% endif %}
         </td>
     </tr>
     <tr>
         <td class="px-3">
             {% if data_loaded.data.workspace %}
                 <span style="background-color: #a5d1ed; padding:2px 10px 2px 10px;">
@@ -73,41 +78,56 @@
             {% if data_loaded.is_owner %}
                 <a class="btn btn-secondary change-owner-btn">
                     <i class="fas fa-user-circle"></i> Change owner
                 </a>
             {% endif %}
             {% if data_loaded.can_write %}
                 <a class="btn btn-secondary edit-record-btn">
-                    <i class="fas fa-edit"></i> {% if data_loaded.data|has_draft:request.user %} Edit draft {% else %} Create new version {% endif %}
+                    <i class="fas fa-edit"></i> {% if data_loaded.form_id %} Edit draft {% else %} Create new version {% endif %}
+                </a>
+                {% if data_loaded.form_id %}
+                <a class="btn btn-secondary" href="{% url 'core_curate_app_xml_text_editor_view'%}?id={{ data_loaded.form_id }}">
+                    <i class="fas fa-code"></i> Open Draft
                 </a>
-                <a class="btn btn-secondary open-record-btn">
+                {% else %}
+                <a class="btn btn-secondary open-record-btn" href="#">
                     <i class="fas fa-code"></i> Open
                 </a>
+                {% endif %}
             {% endif %}
             {% if data_loaded.can_write %}
                 {% if data.administration %}
                     {% url 'core-admin:core_dashboard_app_edit_data' data_loaded.data.id as edit_url %}
                 {% else %}
                     {% url 'core_dashboard_app_edit_data' data_loaded.data.id as edit_url %}
                 {% endif %}
                 {% include 'core_main_app/common/buttons/edit.html' with label="Edit Title" %}
                 {% if data.administration %}
                     {% with data_loaded.delete_url as delete_url %}
                     {% include 'core_main_app/common/buttons/delete.html' %}
                     {% endwith %}
                 {% endif %}
+                {% if data.administration and  data_loaded.forms_count > 0 %}
+                <a objectid="{{data_loaded.data.id}}" class="btn btn-danger delete-data-draft-list-btn" href="#">
+                    <i class="fas fa-trash"></i> Delete Draft{{ data_loaded.forms_count|pluralize }}
+                </a>
+                {% elif data_loaded.form_id %}
+                <a objectid="{{data_loaded.form_id}}" class="btn btn-danger  delete-draft-btn" href="#">
+                    <i class="fas fa-trash"></i> Delete Draft
+                </a>
+                {% endif %}
             {% endif %}
 
         </td>
         <td style="padding: 10px;">
             {% if data_loaded.can_set_public %}
-                <a class="btn btn-secondary publish-record-btn float-right">
+                <a class="btn btn-secondary publish-record-btn {% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}">
                     <i class="fas fa-share-alt"></i> Publish
                 </a>
             {% endif %}
-            <span class="float-right" style="font-size: 0.6em; margin: 0.7em;">
-                {% if data_loaded.can_set_public %}Updated{% else%}Published{% endif %} on: {{ data_loaded.data.last_modification_date|print_datetime_utc_unaware }}
+            <span class="{% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}" style="font-size: 0.6em; margin: 0.7em;">
+                {% if data_loaded.can_set_public %}Updated{% else%}Published{% endif %} on: {{ data_loaded.data.last_modification_date|localtime }}
             </span>
         </td>
     </tr>
 </table>
 {% endfor %}
```

#### html2text {}

```diff
@@ -1,40 +1,83 @@
-{% load dict_key_extras %} {% load draft_extras %} {% load timestamptags %} {%
-for data_loaded in objects %}
-                                                      {% if data_loaded.data_status ==
-                                                     data_loaded.data_status_values.ACTIVE %}  {% endif %} {% if
-{% if data_loaded.can_read %} {                      data_loaded.data_status == data_loaded.data_status_values.INACTIVE
-{ data_loaded.data.title }} ({                       %}  {% endif %} {% if data_loaded.data_status ==
-{ data_loaded.data_role }}) {% else %} {             data_loaded.data_status_values.DELETED %}  {% endif %}
-{ data_loaded.data.title }} ({                       Active Inactive {% if data_loaded.data.workspace.is_public %}
-{ data_loaded.data_role }}) {% endif %} {% if        Deleted {% endif %}
-data_loaded.data|has_draft:request.user%},  Draft{%  {% if data_loaded.data_status ==
-endif %}                                             data_loaded.data_status_values.ACTIVE %} Active {% endif %} {% if
-                                                     data_loaded.data_status == data_loaded.data_status_values.INACTIVE
-                                                     %} Inactive {% endif %} {% if data_loaded.data_status ==
-                                                     data_loaded.data_status_values.DELETED %} Deleted {% endif %}
-{% if data_loaded.data.workspace %}  {
-{ data_loaded.data.workspace.title }}  {% else %}
-No workspace assigned  {% endif %}  {% with
+{% load dict_key_extras %} {% load timestamptags %} {% load special_plural %}
+{% load tz %} {% for data_loaded in objects %}
+                                  .6.2" %}float-right{% elif BOOTSTRAP_VERSION ==
+                                  "5.1.3" %}float-end{% endif %} dropdown"> {% if
+                                  data_loaded.data_status ==
+                                  data_loaded.data_status_values.ACTIVE %}  {%
+                                  endif %} {% if data_loaded.data_status ==
+                                  data_loaded.data_status_values.INACTIVE %}  {%
+                                  endif %} {% if data_loaded.data_status ==
+{% if data_loaded.can_read %} {   data_loaded.data_status_values.DELETED %}  {%
+{ data_loaded.data.title }} ({    endif %}
+{ data_loaded.data_role }}) {%    Active Inactive {% if
+else %} {{ data_loaded.data.title data_loaded.data.workspace.is_public %} Deleted
+}} ({{ data_loaded.data_role }})  {% endif %}
+{% endif %} {% if                  {% if data_loaded.data_status ==
+data.administration and           data_loaded.data_status_values.ACTIVE %}
+data_loaded.forms_count > 0 %} ,  .6.2" %}float-right{% elif BOOTSTRAP_VERSION ==
+Draft{                            "5.1.3" %}float-end{% endif %} label-status font-
+{                                 active">Active {% endif %} {% if
+data_loaded.forms_count|pluralize data_loaded.data_status ==
+}}  {% elif data_loaded.form_id   data_loaded.data_status_values.INACTIVE %}
+%} , Draft  {% endif %}           .6.2" %}float-right{% elif BOOTSTRAP_VERSION ==
+                                  "5.1.3" %}float-end{% endif %} label-status font-
+                                  inactive">Inactive {% endif %} {% if
+                                  data_loaded.data_status ==
+                                  data_loaded.data_status_values.DELETED %}
+                                  .6.2" %}float-right{% elif BOOTSTRAP_VERSION ==
+                                  "5.1.3" %}float-end{% endif %} label-status font-
+                                  deleted">Deleted {% endif %}
+{% if data_loaded.data.workspace
+%}  {
+{
+data_loaded.data.workspace.title
+}}  {% else %}  No workspace
+assigned  {% endif %}  {% with
 key=data_loaded.data.user_id %} {
-{ data_loaded.username_list|get:key }} {% endwith %}
-{% if data_loaded.can_change_workspace %}
+{ data_loaded.username_list|get:
+key }} {% endwith %}
+{% if
+data_loaded.can_change_workspace
+%}
  Change workspace
- {% endif %} {% if data_loaded.is_owner %}
+ {% endif %} {% if
+data_loaded.is_owner %}
  Change owner
- {% endif %} {% if data_loaded.can_write %}
- {% if data_loaded.data|has_draft:request.user %}
-Edit draft {% else %} Create new version {% endif %} {% if data_loaded.can_set_public %}
-                                                      Publish
- Open                                                 {% endif %}  {% if data_loaded.can_set_public %}Updated{%
- {% endif %} {% if data_loaded.can_write %} {% if    else%}Published{% endif %} on: {
-data.administration %} {% url 'core-admin:           {
-core_dashboard_app_edit_data' data_loaded.data.id as data_loaded.data.last_modification_date|print_datetime_utc_unaware
-edit_url %} {% else %} {% url                        }}
-'core_dashboard_app_edit_data' data_loaded.data.id
-as edit_url %} {% endif %} {% include
-'core_main_app/common/buttons/edit.html' with
-label="Edit Title" %} {% if data.administration %}
-{% with data_loaded.delete_url as delete_url %} {%
-include 'core_main_app/common/buttons/delete.html'
-%} {% endwith %} {% endif %} {% endif %}
+ {% endif %} {% if
+data_loaded.can_write %}
+ {% if data_loaded.form_id %}
+Edit draft {% else %} Create new
+version {% endif %}
+ {% if data_loaded.form_id %}
+ Open_Draft
+ {% else %}
+ Open
+ {% endif %} {% endif %} {% if    {% if data_loaded.can_set_public %}
+data_loaded.can_write %} {% if    .6.2" %}float-right{% elif BOOTSTRAP_VERSION ==
+data.administration %} {% url     "5.1.3" %}float-end{% endif %}">  Publish
+'core-admin:                       {% endif %}
+core_dashboard_app_edit_data'     .6.2" %}float-right{% elif BOOTSTRAP_VERSION ==
+data_loaded.data.id as edit_url   "5.1.3" %}float-end{% endif %}" style="font-size:
+%} {% else %} {% url              0.6em; margin: 0.7em;"> {% if
+'core_dashboard_app_edit_data'    data_loaded.can_set_public %}Updated{%
+data_loaded.data.id as edit_url   else%}Published{% endif %} on: {
+%} {% endif %} {% include         {
+'core_main_app/common/buttons/    data_loaded.data.last_modification_date|localtime
+edit.html' with label="Edit       }}
+Title" %} {% if
+data.administration %} {% with
+data_loaded.delete_url as
+delete_url %} {% include
+'core_main_app/common/buttons/
+delete.html' %} {% endwith %} {%
+endif %} {% if
+data.administration and
+data_loaded.forms_count > 0 %}
+ Delete_Draft{
+{
+data_loaded.forms_count|pluralize
+}}
+ {% elif data_loaded.form_id %}
+ Delete_Draft
+ {% endif %} {% endif %}
 {% endfor %}
```

### Comparing `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/urls.py` & `core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/urls.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,17 +2,14 @@
     Url router for the user dashboard
 """
 from django.contrib.auth.decorators import login_required
 from django.urls import re_path
 
 from core_dashboard_common_app import constants as dashboard_constants
 from core_dashboard_common_app.views.common import ajax, views as common_views
-from core_dashboard_common_app.views.common.views import (
-    UserDashboardPasswordChangeFormView,
-)
 from core_dashboard_registry_app.views.common import (
     ajax as registry_common_ajax,
 )
 from core_dashboard_registry_app.views.common import (
     views as registry_common_views,
 )
 from core_dashboard_registry_app.views.common.ajax import EditDataView
@@ -26,22 +23,14 @@
     ),
     re_path(
         r"^my-profile/edit$",
         common_views.my_profile_edit,
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

### Comparing `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/query/django/prepare.py` & `core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/utils/query/django/prepare.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/utils/query/mongo/prepare.py` & `core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/utils/query/mongo/prepare.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/views/common/ajax.py` & `core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/views/common/ajax.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/views/common/forms.py` & `core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/views/common/forms.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app/views/common/views.py` & `core_dashboard_registry_app-2.4.0/core_dashboard_registry_app/views/common/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Common views for the registry dashboard
 """
+from core_main_app.commons.exceptions import DoesNotExist
 from django.conf import settings as conf_settings
 from django.contrib.auth.decorators import login_required
 from django.urls import reverse
 from django.utils.decorators import method_decorator
 
 import core_curate_app.components.curate_data_structure.api as curate_data_structure_api
 from core_dashboard_common_app import constants as dashboard_common_constants
@@ -314,26 +315,37 @@
 
         """
         data_context_list = []
         username_list = dict(
             (x.id, x.username) for x in user_api.get_all_users()
         )
         for data in data_list:
+            forms_count = (
+                len(
+                    curate_data_structure_api.get_all_curate_data_structures_by_data(
+                        data, self.request.user
+                    )
+                )
+                if self.administration
+                else 0
+            )
             data_context_list.append(
                 {
                     "data": data,
                     "username_list": username_list,
                     "data_status": get_status(data),
                     "data_status_values": DataStatus,
                     "data_role": ", ".join(
                         [
                             _get_role_label(x, request=self.request)
                             for x in get_role(data)
                         ]
                     ),
+                    "form_id": _get_form_id(data, self.request.user),
+                    "forms_count": forms_count,
                     "can_read": True,
                     "can_write": True,
                     "is_owner": True,
                     "can_change_workspace": check_if_workspace_can_be_changed(
                         data
                     ),
                     "can_set_public": not data_api.is_data_public(data),
@@ -426,27 +438,38 @@
 
     def _format_data_context(
         self, data_list, user, user_can_read, user_can_write
     ):
         detailed_user_data = []
         username_list = get_id_username_dict(user_api.get_all_users())
         for data in data_list:
+            forms_count = (
+                len(
+                    curate_data_structure_api.get_all_curate_data_structures_by_data(
+                        data, self.request.user
+                    )
+                )
+                if self.administration
+                else 0
+            )
             is_owner = str(data.user_id) == str(user.id) or self.administration
             detailed_user_data.append(
                 {
                     "data": data,
                     "username_list": username_list,
                     "data_status": get_status(data),
                     "data_status_values": DataStatus,
                     "data_role": ", ".join(
                         [
                             _get_role_label(x, request=self.request)
                             for x in get_role(data)
                         ]
                     ),
+                    "form_id": _get_form_id(data, self.request.user),
+                    "forms_count": forms_count,
                     "can_read": user_can_read or is_owner,
                     "can_write": user_can_write or is_owner,
                     "is_owner": is_owner,
                     "can_set_public": not data_api.is_data_public(data),
                 }
             )
         return detailed_user_data
@@ -528,7 +551,25 @@
     """
     try:
         return custom_resource_api.get_by_role_for_current_template(
             role, request=request
         ).title
     except (exceptions.ModelError, exceptions.DoesNotExist):
         return role
+
+
+def _get_form_id(data, user):
+    """Get form id by data and user
+
+    Args:
+        data:
+        user
+
+    Returns:
+
+    """
+    try:
+        return curate_data_structure_api.get_by_data_id_and_user(
+            data.id, user
+        ).id
+    except DoesNotExist:
+        return None
```

### Comparing `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app.egg-info/PKG-INFO` & `core_dashboard_registry_app-2.4.0/core_dashboard_registry_app.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-dashboard-registry-app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Resource management via a dashboard for the registry core project
 Home-page: https://github.com/usnistgov/core_dashboard_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: Core Dashboard Registry App
         ===========================
```

### Comparing `core_dashboard_registry_app-2.3.0/core_dashboard_registry_app.egg-info/SOURCES.txt` & `core_dashboard_registry_app-2.4.0/core_dashboard_registry_app.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -44,12 +44,13 @@
 core_dashboard_registry_app/views/__init__.py
 core_dashboard_registry_app/views/common/__init__.py
 core_dashboard_registry_app/views/common/ajax.py
 core_dashboard_registry_app/views/common/forms.py
 core_dashboard_registry_app/views/common/views.py
 tests/__init__.py
 tests/test_settings.py
+tests/urls.py
 tests/utils/__init__.py
 tests/utils/query/__init__.py
 tests/utils/query/test_unit.py
 tests/views/__init__.py
 tests/views/tests_unit.py
```

### Comparing `core_dashboard_registry_app-2.3.0/setup.py` & `core_dashboard_registry_app-2.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_dashboard_registry_app",
-    version="2.3.0",
+    version="2.4.0",
     description="Resource management via a dashboard for the registry core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_dashboard_registry_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_dashboard_registry_app-2.3.0/tests/test_settings.py` & `core_dashboard_registry_app-2.4.0/tests/test_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,8 +60,9 @@
 ]
 MONGODB_INDEXING = False
 MONGODB_ASYNC_SAVE = False
 CUSTOM_NAME = "Test"
 CELERYBEAT_SCHEDULER = "django_celery_beat.schedulers:DatabaseScheduler"
 CAN_ANONYMOUS_ACCESS_PUBLIC_DOCUMENT = True
 DEFAULT_AUTO_FIELD = "django.db.models.BigAutoField"
-ROOT_URLCONF = "core_dashboard_registry_app.urls"
+ROOT_URLCONF = "tests.urls"
+ENABLE_SAML2_SSO_AUTH = False
```

### Comparing `core_dashboard_registry_app-2.3.0/tests/utils/query/test_unit.py` & `core_dashboard_registry_app-2.4.0/tests/utils/query/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.3.0/tests/views/tests_unit.py` & `core_dashboard_registry_app-2.4.0/tests/views/tests_unit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """ Unit tests views
 """
 from unittest.mock import patch, MagicMock
 
+from core_main_app.components.workspace.models import Workspace
+
+import core_dashboard_registry_app
+from core_main_app.components.data.models import Data
 from django.contrib.auth.models import AnonymousUser
 from django.http import HttpResponse
-from django.test import RequestFactory, override_settings, tag, SimpleTestCase
+from django.test import RequestFactory, override_settings, tag
 
 from core_dashboard_registry_app import constants as dashboard_constants
 from core_dashboard_registry_app.views.common.views import (
     DashboardRegistryRecords,
     DashboardRegistryWorkspaceRecords,
 )
 from core_main_app.access_control.exceptions import AccessControlError
@@ -118,14 +122,16 @@
         request = self.factory.get("core_dashboard_records")
         request.user = self.user1
 
         # Act
         response = DashboardRegistryRecords.as_view()(request)
         self.assertEqual(response.status_code, 200)
 
+    @patch.object(core_dashboard_registry_app.views.common.views, "get_status")
+    @patch.object(core_dashboard_registry_app.views.common.views, "get_role")
     @patch("core_main_app.components.workspace.api.get_global_workspace")
     @patch("core_main_app.views.common.views.CommonView.common_render")
     @patch("core_main_app.components.data.api.execute_query")
     @patch(
         "core_main_registry_app.components.custom_resource.api.get_current_custom_resource_type_all"
     )
     @patch(
@@ -134,38 +140,40 @@
     def test_request_published_records(
         self,
         get_all_of_current_template,
         get_current_custom_resource_type_all,
         execute_query,
         common_render,
         get_global_workspace,
+        get_status,
+        get_role,
     ):
         """test_request_published_records
 
         Returns:
 
         """
         # Arrange
         cr_type_all = MagicMock()
         cr_type_all.slug = "test"
 
         current_template = MagicMock()
         loaded_data = MagicMock()
-        loaded_data.filter.return_value = []
+        loaded_data.filter.return_value = [Data(id=0)]
         execute_query.return_value = loaded_data
-
+        get_role.return_value = []
         expected_response = HttpResponse()
         common_render.return_value = expected_response
-
         workspace = MagicMock()
         workspace.id = 1
         get_global_workspace.return_value = workspace
-
         get_current_custom_resource_type_all.return_value = cr_type_all
+
         get_all_of_current_template.return_value = current_template
+
         request = self.factory.get(
             "core_dashboard_records", data={"ispublished": "published"}
         )
         request.user = self.user1
 
         # Act
         response = DashboardRegistryRecords.as_view()(request)
@@ -449,21 +457,63 @@
         # Act
         result = view._format_draft_context_registry(draft_list=[draft])
 
         # Assert
         self.assertEqual(result[0]["role"], "None")
 
 
-class TestDashboardRegistryWorkspaceRecords(SimpleTestCase):
+class TestDashboardRegistryWorkspaceRecords(IntegrationBaseTestCase):
     """TestDashboardRegistryWorkspaceRecords"""
 
+    def setUp(self):
+        """setUp
+
+        Returns:
+
+        """
+        self.factory = RequestFactory()
+        self.user1 = create_mock_user(user_id="1")
+
     def test_publish_script_added_to_assets(self):
         """test_publish_script_added_to_assets
 
         Returns:
 
         """
         assets = DashboardRegistryWorkspaceRecords()._get_assets()
         self.assertTrue(
             dashboard_constants.JS_PUBLISH_RESOURCE
             in [asset["path"] for asset in assets["js"]]
         )
+
+    @patch.object(core_dashboard_registry_app.views.common.views, "get_role")
+    @patch.object(core_dashboard_registry_app.views.common.views, "get_status")
+    def test_data_drafts_added_to_context(
+        self,
+        get_status,
+        get_role,
+    ):
+        """test_data_drafts_added_to_context
+
+        Returns:
+
+        """
+        # Arrange
+        workspace = Workspace()
+        workspace.id = 1
+        data_list = [Data(id=0, workspace=workspace)]
+
+        get_status.return_value = None
+        get_role.return_value = []
+
+        self.request = self.factory.get("core_dashboard_workspace_list")
+        self.administration = False
+        self.request.user = self.user1
+        # Act
+        data_context = DashboardRegistryWorkspaceRecords._format_data_context(
+            self, data_list, self.user1, True, True
+        )
+
+        # Assert
+        for data in data_context:
+            self.assertEqual(data["form_id"], None)
+            self.assertEqual(data["forms_count"], 0)
```

