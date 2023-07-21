# Comparing `tmp/core_explore_keyword_registry_app-2.3.0.tar.gz` & `tmp/core_explore_keyword_registry_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_explore_keyword_registry_app-2.3.0.tar", last modified: Tue May  2 19:38:05 2023, max compression
+gzip compressed data, was "core_explore_keyword_registry_app-2.4.0.tar", last modified: Fri Jul 21 02:12:02 2023, max compression
```

## Comparing `core_explore_keyword_registry_app-2.3.0.tar` & `core_explore_keyword_registry_app-2.4.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.407371 core_explore_keyword_registry_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      199 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1581 2023-05-02 19:38:05.402353 core_explore_keyword_registry_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1042 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.789449 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      710 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/apps.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3508 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/discover.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.913045 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1063 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/permissions/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      883 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.452353 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.524962 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.513929 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.481869 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.926033 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/fancytree/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      813 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/fancytree/fancytree.custom.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.952168 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      310 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/filters.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/search.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.505686 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.068055 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3328 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/fancytree.custom.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       76 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/fancytree.custom.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2544 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/filters.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9169 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/resource_type_icons_table.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      257 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/resource_type_icons_table.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      322 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/search.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      650 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/tagit.custom.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.517043 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.520270 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.081689 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/1.1.0/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     6230 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/1.1.0/jquery.shorten.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.110719 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6809 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-detail.xsl
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4178 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-list.xsl
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.586551 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.569269 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_common_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.572379 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.136832 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      937 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_info.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      846 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_results.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.581165 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.152271 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1702 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/user/index.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.589716 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.164869 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      956 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/user/refinements.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.199846 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templatetags/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templatetags/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templatetags/render_extras.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1446 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.228426 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.287799 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12995 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1475 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/views/user/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12589 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:04.869855 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1581 2023-05-02 19:38:04.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3044 2023-05-02 19:38:04.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:38:04.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      152 2023-05-02 19:38:04.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2023-05-02 19:38:04.000000 core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      200 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       26 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:38:05.409133 core_explore_keyword_registry_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1090 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.320713 core_explore_keyword_registry_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1793 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.338430 core_explore_keyword_registry_app-2.3.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:05.380801 core_explore_keyword_registry_app-2.3.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/tests/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5093 2023-05-02 19:38:02.000000 core_explore_keyword_registry_app-2.3.0/tests/views/user/tests_views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:02.106316 core_explore_keyword_registry_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:11:56.000000 core_explore_keyword_registry_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      199 2023-07-21 02:11:56.000000 core_explore_keyword_registry_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1581 2023-07-21 02:12:02.103444 core_explore_keyword_registry_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1042 2023-07-21 02:11:56.000000 core_explore_keyword_registry_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.639179 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2023-07-21 02:11:58.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      710 2023-07-21 02:11:58.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/apps.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3508 2023-07-21 02:11:58.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/discover.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.733709 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:58.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1063 2023-07-21 02:11:58.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/permissions/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      883 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.361304 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.415578 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.404509 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.375999 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.747033 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/fancytree/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      861 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/fancytree/fancytree.custom.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.774321 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      310 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/filters.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/search.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.395954 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.853854 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3328 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/fancytree.custom.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       76 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/fancytree.custom.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2544 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/filters.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9169 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/resource_type_icons_table.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      257 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/resource_type_icons_table.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      322 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/search.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      650 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/tagit.custom.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.407786 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.411041 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.874942 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/1.1.0/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     6230 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/1.1.0/jquery.shorten.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.894586 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6861 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-detail.xsl
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4230 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-list.xsl
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.448658 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.430682 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/templates/core_explore_common_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.434200 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.914334 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      994 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_info.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      846 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_results.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.443212 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.925846 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1702 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/user/index.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.451841 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.938845 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1059 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/user/refinements.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.964602 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/templatetags/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/templatetags/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/templatetags/render_extras.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1446 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.976134 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:02.038567 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12995 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1475 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/views/user/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12589 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:01.701969 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1581 2023-07-21 02:12:01.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3044 2023-07-21 02:12:01.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:12:01.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      152 2023-07-21 02:12:01.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2023-07-21 02:12:01.000000 core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      200 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       26 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:12:02.107935 core_explore_keyword_registry_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1090 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:02.064405 core_explore_keyword_registry_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1793 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:02.074861 core_explore_keyword_registry_app-2.4.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:02.097034 core_explore_keyword_registry_app-2.4.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/tests/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5093 2023-07-21 02:11:59.000000 core_explore_keyword_registry_app-2.4.0/tests/views/user/tests_views.py
```

### Comparing `core_explore_keyword_registry_app-2.3.0/LICENSE.md` & `core_explore_keyword_registry_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.3.0/PKG-INFO` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
-Name: core_explore_keyword_registry_app
-Version: 2.3.0
+Name: core-explore-keyword-registry-app
+Version: 2.4.0
 Summary: Exploration by keywords for the registry project
 Home-page: https://github.com/usnistgov/core_explore_keyword_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =================================
         Core Explore Keyword Registry App
```

### Comparing `core_explore_keyword_registry_app-2.3.0/README.rst` & `core_explore_keyword_registry_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/apps.py` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/discover.py` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/discover.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/permissions/discover.py` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/permissions/discover.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/settings.py` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/fancytree/fancytree.custom.css` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/fancytree/fancytree.custom.css`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 }
 
 .refinement {
     color: #474747;
     margin: 0;
 }
 
-.refinement a[class=""] .fa-chevron-up {
+.refinement a i.fas {
+   font-size: 1rem;
+}
+
+.refinement a[class=""] .fa-chevron-right {
    display: none;
 }
 
 .refinement a[class="collapsed"] .fa-chevron-down {
    display: none;
 }
```

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/search.css` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/search.css`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/fancytree.custom.js` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/fancytree.custom.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/filters.js` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/filters.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/resource_type_icons_table.js` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/resource_type_icons_table.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/tagit.custom.js` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/tagit.custom.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/1.1.0/jquery.shorten.js` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/1.1.0/jquery.shorten.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-detail.xsl` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-detail.xsl`

 * *Files 1% similar despite different names*

#### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-detail.xsl` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-detail.xsl`

```diff
@@ -81,15 +81,15 @@
                 <xsl:with-param name="prefix" select="$prefix"/>
                 <xsl:with-param name="current" select="$name"/>
               </xsl:call-template>
               <xsl:text>:</xsl:text>
             </strong>
             <xsl:choose>
               <xsl:when test="( (contains($name, 'URL')) or (starts-with($value, 'https://')) or (starts-with($value, 'http://')) )">
-                <a target="_blank" href="{$value}">
+                <a target="_blank" rel="noopener noreferrer" href="{$value}">
                   <xsl:value-of select="$value"/>
                 </a>
               </xsl:when>
               <xsl:otherwise>
                 <xsl:value-of select="$value"/>
               </xsl:otherwise>
             </xsl:choose>
@@ -164,15 +164,15 @@
       <xsl:if test="not(starts-with($name, 'xsi:type'))">
         <span class="value">
           <xsl:text>(</xsl:text>
           <xsl:value-of select="$name"/>
           <xsl:text>:</xsl:text>
           <xsl:choose>
             <xsl:when test="( (contains($name, 'URL')) or (starts-with($value, 'https://')) or (starts-with($value, 'http://')) )">
-              <a target="_blank" href="{$value}">
+              <a target="_blank" rel="noopener noreferrer" href="{$value}">
                 <xsl:value-of select="$value"/>
               </a>
             </xsl:when>
             <xsl:otherwise>
               <xsl:value-of select="$value"/>
             </xsl:otherwise>
           </xsl:choose>
```

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-list.xsl` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-list.xsl`

 * *Files 2% similar despite different names*

#### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-list.xsl` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-list.xsl`

```diff
@@ -39,15 +39,15 @@
         <xsl:variable name="publisher" select="//nr:Resource/nr:providers/nr:publisher"/>
         <xsl:if test="( ($creators!='') and ($publisher!='') )">
           <xsl:text>-</xsl:text>
         </xsl:if>
         <xsl:value-of select="$publisher"/>
       </div>
       <xsl:variable name="url" select="//nr:Resource/nr:content/nr:landingPage"/>
-      <a target="_blank" href="{$url}">
+      <a target="_blank" rel="noopener noreferrer" href="{$url}">
         <xsl:value-of select="$url"/>
       </a>
       <xsl:variable name="idw">{{ result.detail_url|slice:'-24:' }}</xsl:variable>
       <a data-toggle="collapse" data-target="#{$idw}" aria-expanded="false" aria-controls="{$idw}" class="collapsed">
         <i class="fas fa-chevron-up"/>
         <i class="fas fa-chevron-down"/>
       </a>
@@ -92,15 +92,15 @@
     <xsl:variable name="name" select="name(.)"/>
     <xsl:variable name="value" select="."/>
     <xsl:variable name="arg" select="@type"/>
     <xsl:if test="( (contains($name, 'URL')) or (starts-with($value, 'https://')) or (starts-with($value, 'http://')) )">
       <xsl:if test="$value!=''">
         <xsl:value-of select="$name"/>
         <xsl:text>:</xsl:text>
-        <a target="_blank" href="{$value}">
+        <a target="_blank" rel="noopener noreferrer" href="{$value}">
           <xsl:value-of select="$value"/>
         </a>
         <br/>
       </xsl:if>
     </xsl:if>
   </xsl:template>
 </xsl:stylesheet>
```

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_info.html` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_info.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 {% load render_extras %}
+{% load parse_date %}
 {% load json_date %}
+{% load tz %}
 <div name="result">
     <div>
         <input data-template-id="{{result.template_info.id}}"
                data-template-hash="{{result.template_info.hash}}"
                type="checkbox" value="{{ result.access_data_url }}"
                class="exporter-checkbox{% if not exporter_app %} hidden{% endif %}"/>
     </div>
     {% if result.permission_url and display_edit_button %}
         <input class="input-permission-url" type="hidden" value="{{result.permission_url}}">
         <a class="permissions-link" href="#">
             <i class="fas fa-pencil-alt permissions-icon edit" aria-hidden="true"></i>
         </a>
     {% endif %}
-    <div title="Last modification date" class="data-info-right-container">{{result.last_modification_date|json_date:"N d Y g:iA"}}</div>
+    <div title="Last modification date" class="data-info-right-container">{{result.last_modification_date|parse_date|localtime|json_date:"N d Y g:iA"}}</div>
     <div class="xml-representation-container">
         {% render_as_template xml_representation %}
     </div>
 </div>
```

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_results.html` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_results.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/user/index.html` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/user/index.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/user/refinements.html` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/user/refinements.html`

 * *Files 11% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 {% for field in data.refinement_form %}
 	  <div class="panel panel-default">
 		<div class="card-header">
 			<a class="clearTree" href="javascript:void(0)" onclick="clearTree('#{{field.id_for_label}}', this)">
 				(Clear)
 			</a>
 			<h4 class="panel-title refinement">
-				<a data-toggle="collapse" href="#collapse_{{field.id_for_label}}"
+				<a {% if BOOTSTRAP_VERSION == "4.6.2" %}data-toggle{% elif BOOTSTRAP_VERSION == "5.1.3"%}data-bs-toggle{% endif %}="collapse" href="#collapse_{{field.id_for_label}}"
 				   class="{% if forloop.counter != 1 and field.field.has_selected_values|lower == 'false' %}collapsed{% endif %}">
-					<i class="fas fa-chevron-up"></i>
+					<i class="fas fa-chevron-right"></i>
 					<i class="fas fa-chevron-down"></i>
 					{{ field.label_tag }}
 				</a>
 			</h4>
 		</div>
 		<div id="collapse_{{field.id_for_label}}"
 			 class="panel-collapse collapse{% if forloop.counter == 1 or field.field.has_selected_values %} show {% endif %}">
```

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/templatetags/render_extras.py` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/templatetags/render_extras.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/urls.py` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/views/user/ajax.py` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/views/user/forms.py` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/views/user/forms.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app/views/user/views.py` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app.egg-info/PKG-INFO` & `core_explore_keyword_registry_app-2.4.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
-Name: core-explore-keyword-registry-app
-Version: 2.3.0
+Name: core_explore_keyword_registry_app
+Version: 2.4.0
 Summary: Exploration by keywords for the registry project
 Home-page: https://github.com/usnistgov/core_explore_keyword_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =================================
         Core Explore Keyword Registry App
```

### Comparing `core_explore_keyword_registry_app-2.3.0/core_explore_keyword_registry_app.egg-info/SOURCES.txt` & `core_explore_keyword_registry_app-2.4.0/core_explore_keyword_registry_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.3.0/setup.py` & `core_explore_keyword_registry_app-2.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_explore_keyword_registry_app",
-    version="2.3.0",
+    version="2.4.0",
     description="Exploration by keywords for the registry project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_explore_keyword_registry_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_explore_keyword_registry_app-2.3.0/tests/test_settings.py` & `core_explore_keyword_registry_app-2.4.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.3.0/tests/views/user/tests_views.py` & `core_explore_keyword_registry_app-2.4.0/tests/views/user/tests_views.py`

 * *Files identical despite different names*

