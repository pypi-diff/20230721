# Comparing `tmp/core_explore_oaipmh_app-2.3.0.tar.gz` & `tmp/core_explore_oaipmh_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_explore_oaipmh_app-2.3.0.tar", last modified: Tue May  2 19:38:18 2023, max compression
+gzip compressed data, was "core_explore_oaipmh_app-2.4.0.tar", last modified: Fri Jul 21 02:12:11 2023, max compression
```

## Comparing `core_explore_oaipmh_app-2.3.0.tar` & `core_explore_oaipmh_app-2.4.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:18.083128 core_explore_oaipmh_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      154 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1428 2023-05-02 19:38:18.077890 core_explore_oaipmh_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      855 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.535774 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.620706 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.641613 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/components/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/components/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1713 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/components/query/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.660753 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.678993 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/rest/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/rest/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6516 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/rest/query/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.698221 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/rest/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/rest/result/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1755 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/rest/result/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      313 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      333 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.322252 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.325724 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.328632 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.335495 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.709356 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      127 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data/change_display.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.719789 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data_sources/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2332 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data_sources/list.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.346964 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.349990 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.353584 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.745564 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      673 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list-content.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1054 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      934 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.758027 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.798950 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5958 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1871 2023-05-02 19:38:14.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.583092 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1428 2023-05-02 19:38:16.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1868 2023-05-02 19:38:17.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:38:16.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      147 2023-05-02 19:38:16.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-05-02 19:38:16.000000 core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      115 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:38:18.085201 core_explore_oaipmh_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1079 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.835550 core_explore_oaipmh_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.861446 core_explore_oaipmh_app-2.3.0/tests/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6073 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/fixtures/fixtures.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.874413 core_explore_oaipmh_app-2.3.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.907399 core_explore_oaipmh_app-2.3.0/tests/rest/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/rest/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7300 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/rest/query/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.934951 core_explore_oaipmh_app-2.3.0/tests/rest/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/rest/result/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2845 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/rest/result/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2157 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      316 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/test_urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.973178 core_explore_oaipmh_app-2.3.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:17.993300 core_explore_oaipmh_app-2.3.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/views/user/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:18.036538 core_explore_oaipmh_app-2.3.0/tests/views/user/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/views/user/ajax/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2219 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/views/user/ajax/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14034 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/views/user/ajax/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:18.068621 core_explore_oaipmh_app-2.3.0/tests/views/user/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/views/user/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5472 2023-05-02 19:38:15.000000 core_explore_oaipmh_app-2.3.0/tests/views/user/views/tests_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:11.572800 core_explore_oaipmh_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:12:08.000000 core_explore_oaipmh_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      154 2023-07-21 02:12:08.000000 core_explore_oaipmh_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1428 2023-07-21 02:12:11.568254 core_explore_oaipmh_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      855 2023-07-21 02:12:08.000000 core_explore_oaipmh_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:10.964494 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:08.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:11.065123 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:08.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:11.094442 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/components/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:08.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/components/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1713 2023-07-21 02:12:08.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/components/query/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:11.122369 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:08.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:11.148781 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/rest/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:08.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/rest/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6516 2023-07-21 02:12:08.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/rest/query/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:11.177518 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/rest/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:08.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/rest/result/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1755 2023-07-21 02:12:08.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/rest/result/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      313 2023-07-21 02:12:08.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      333 2023-07-21 02:12:08.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:10.688827 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:10.691628 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:10.694867 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:10.702931 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:11.190927 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      127 2023-07-21 02:12:08.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data/change_display.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:11.204538 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data_sources/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2332 2023-07-21 02:12:08.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data_sources/list.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:10.722172 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:10.725589 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:10.728915 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:11.232289 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      673 2023-07-21 02:12:08.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list-content.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1269 2023-07-21 02:12:08.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      934 2023-07-21 02:12:08.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:11.246929 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:08.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:11.301476 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:08.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5958 2023-07-21 02:12:08.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1871 2023-07-21 02:12:08.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:11.045781 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1428 2023-07-21 02:12:10.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1868 2023-07-21 02:12:10.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:12:10.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      147 2023-07-21 02:12:10.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-07-21 02:12:10.000000 core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:12:09.000000 core_explore_oaipmh_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      115 2023-07-21 02:12:09.000000 core_explore_oaipmh_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:12:11.574982 core_explore_oaipmh_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1079 2023-07-21 02:12:09.000000 core_explore_oaipmh_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:11.338813 core_explore_oaipmh_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:09.000000 core_explore_oaipmh_app-2.4.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:11.365581 core_explore_oaipmh_app-2.4.0/tests/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:09.000000 core_explore_oaipmh_app-2.4.0/tests/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6073 2023-07-21 02:12:09.000000 core_explore_oaipmh_app-2.4.0/tests/fixtures/fixtures.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:11.378153 core_explore_oaipmh_app-2.4.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:09.000000 core_explore_oaipmh_app-2.4.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:11.418430 core_explore_oaipmh_app-2.4.0/tests/rest/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:09.000000 core_explore_oaipmh_app-2.4.0/tests/rest/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7300 2023-07-21 02:12:09.000000 core_explore_oaipmh_app-2.4.0/tests/rest/query/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:11.443175 core_explore_oaipmh_app-2.4.0/tests/rest/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:09.000000 core_explore_oaipmh_app-2.4.0/tests/rest/result/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2845 2023-07-21 02:12:09.000000 core_explore_oaipmh_app-2.4.0/tests/rest/result/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2093 2023-07-21 02:12:09.000000 core_explore_oaipmh_app-2.4.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      316 2023-07-21 02:12:09.000000 core_explore_oaipmh_app-2.4.0/tests/test_urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:11.457671 core_explore_oaipmh_app-2.4.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:09.000000 core_explore_oaipmh_app-2.4.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:11.476488 core_explore_oaipmh_app-2.4.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:09.000000 core_explore_oaipmh_app-2.4.0/tests/views/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:11.527469 core_explore_oaipmh_app-2.4.0/tests/views/user/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:09.000000 core_explore_oaipmh_app-2.4.0/tests/views/user/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2219 2023-07-21 02:12:09.000000 core_explore_oaipmh_app-2.4.0/tests/views/user/ajax/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14034 2023-07-21 02:12:09.000000 core_explore_oaipmh_app-2.4.0/tests/views/user/ajax/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:11.554881 core_explore_oaipmh_app-2.4.0/tests/views/user/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:09.000000 core_explore_oaipmh_app-2.4.0/tests/views/user/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5472 2023-07-21 02:12:09.000000 core_explore_oaipmh_app-2.4.0/tests/views/user/views/tests_permissions.py
```

### Comparing `core_explore_oaipmh_app-2.3.0/LICENSE.md` & `core_explore_oaipmh_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.3.0/PKG-INFO` & `core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
-Name: core_explore_oaipmh_app
-Version: 2.3.0
+Name: core-explore-oaipmh-app
+Version: 2.4.0
 Summary: OAI-PMH exploration functions for curator core project
 Home-page: https://github.com/usnistgov/core_explore_oaipmh_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =======================
         Core Explore Oaipmh App
```

### Comparing `core_explore_oaipmh_app-2.3.0/README.rst` & `core_explore_oaipmh_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/components/query/api.py` & `core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/components/query/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/rest/query/views.py` & `core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/rest/query/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/rest/result/views.py` & `core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/rest/result/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data_sources/list.js` & `core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data_sources/list.js`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list-content.html` & `core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list-content.html`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list.html` & `core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list.html`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 {% block data_sources_list %}
 <div>
     <div id="list-data-sources-oaipmh-content" class="list-group-item">
     </div>
     <div id="error-div-oaipmh" style="display: none;">
         <br/>
         <div class="alert alert-danger alert-dismissable">
-            <a href="#" class="close" data-dismiss="alert" aria-label="close">&times;</a>
+            <a href="#" {% if BOOTSTRAP_VERSION == "4.6.2" %}class="close" data-dismiss="alert"{% elif BOOTSTRAP_VERSION == "5.1.3" %}class="btn-close" data-bs-dismiss="alert"{% endif %} aria-label="close">{% if BOOTSTRAP_VERSION == "4.6.2" %}&times;{% elif BOOTSTRAP_VERSION == "5.1.3" %}{% endif %}</a>
             <strong><span id="error-message"></span></strong>
         </div>
     </div>
 </div>
 {% endblock %}
 
 {% block raw_js %}
```

#### html2text {}

```diff
@@ -1,8 +1,12 @@
 {% extends "core_explore_common_app/user/selector/list_selector_base.html" %}
 {% load static %} {% block title%}OAI-PMH{% endblock %} {% block
 data_sources_list %}
 
-×
+% if BOOTSTRAP_VERSION == "4.6.2" %}class="close" data-dismiss="alert"{% elif
+BOOTSTRAP_VERSION == "5.1.3" %}class="btn-close" data-bs-dismiss="alert"{%
+endif %} aria-label="close">{% if BOOTSTRAP_VERSION == "4.6.2" %}×{% elif
+BOOTSTRAP_VERSION == "5.1.3" %}{% endif %}
+
 {% endblock %} {% block raw_js %}
  {% endblock %} {% block app_js %}
  {% endblock %}
```

### Comparing `core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/urls.py` & `core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/views/user/ajax.py` & `core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app/views/user/views.py` & `core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app.egg-info/PKG-INFO` & `core_explore_oaipmh_app-2.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
-Name: core-explore-oaipmh-app
-Version: 2.3.0
+Name: core_explore_oaipmh_app
+Version: 2.4.0
 Summary: OAI-PMH exploration functions for curator core project
 Home-page: https://github.com/usnistgov/core_explore_oaipmh_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =======================
         Core Explore Oaipmh App
```

### Comparing `core_explore_oaipmh_app-2.3.0/core_explore_oaipmh_app.egg-info/SOURCES.txt` & `core_explore_oaipmh_app-2.4.0/core_explore_oaipmh_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.3.0/setup.py` & `core_explore_oaipmh_app-2.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_explore_oaipmh_app",
-    version="2.3.0",
+    version="2.4.0",
     description="OAI-PMH exploration functions for curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_explore_oaipmh_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_explore_oaipmh_app-2.3.0/tests/fixtures/fixtures.py` & `core_explore_oaipmh_app-2.4.0/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.3.0/tests/rest/query/tests_unit.py` & `core_explore_oaipmh_app-2.4.0/tests/rest/query/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.3.0/tests/rest/result/tests_permissions.py` & `core_explore_oaipmh_app-2.4.0/tests/rest/result/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.3.0/tests/test_settings.py` & `core_explore_oaipmh_app-2.4.0/tests/test_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.sites",
     "django.contrib.staticfiles",
     # Extra apps
     "defender",
-    "tz_detect",
     "menu",
     "django_celery_beat",
     # Local apps
     "core_main_app",
     "core_explore_common_app",
     "core_explore_oaipmh_app",
     "core_oaipmh_common_app",
@@ -42,15 +41,14 @@
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
```

### Comparing `core_explore_oaipmh_app-2.3.0/tests/views/user/ajax/tests_permissions.py` & `core_explore_oaipmh_app-2.4.0/tests/views/user/ajax/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.3.0/tests/views/user/ajax/tests_unit.py` & `core_explore_oaipmh_app-2.4.0/tests/views/user/ajax/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.3.0/tests/views/user/views/tests_permissions.py` & `core_explore_oaipmh_app-2.4.0/tests/views/user/views/tests_permissions.py`

 * *Files identical despite different names*

