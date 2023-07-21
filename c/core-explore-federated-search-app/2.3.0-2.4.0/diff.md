# Comparing `tmp/core_explore_federated_search_app-2.3.0.tar.gz` & `tmp/core_explore_federated_search_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_explore_federated_search_app-2.3.0.tar", last modified: Tue May  2 19:37:40 2023, max compression
+gzip compressed data, was "core_explore_federated_search_app-2.4.0.tar", last modified: Fri Jul 21 02:11:35 2023, max compression
```

## Comparing `core_explore_federated_search_app-2.3.0.tar` & `core_explore_federated_search_app-2.4.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.905669 core_explore_federated_search_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:37:36.000000 core_explore_federated_search_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      174 2023-05-02 19:37:36.000000 core_explore_federated_search_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1555 2023-05-02 19:37:40.901085 core_explore_federated_search_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      967 2023-05-02 19:37:36.000000 core_explore_federated_search_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.027098 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.109497 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.177640 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/components/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      840 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/components/data/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.192057 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.221157 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.265711 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      354 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/query/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6626 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/query/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.308450 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/result/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      303 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/result/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2758 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/result/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      571 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      637 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.756231 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.832746 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.804020 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.808459 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.810958 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.821008 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.397053 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      986 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/delete.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      109 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/delete.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1231 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/edit.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      105 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/edit.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1965 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/refresh.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/refresh.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.835828 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.838752 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.405654 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/data_sources/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2419 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/data_sources/list.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.865107 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.883599 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.870628 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.430285 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.464205 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/add/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1013 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/add/add_base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      308 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/add_repository.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.489802 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2148 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/list_base.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.560434 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      722 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/delete.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1136 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/edit.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      875 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/refresh.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/refresh_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      357 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list_repositories.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:39.885834 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.591623 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      663 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list-content.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1104 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      857 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.609459 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.654911 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5623 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2651 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.095255 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1555 2023-05-02 19:37:39.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3829 2023-05-02 19:37:39.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:37:39.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      117 2023-05-02 19:37:39.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2023-05-02 19:37:39.000000 core_explore_federated_search_app-2.3.0/core_explore_federated_search_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       85 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:37:40.907268 core_explore_federated_search_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1114 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.697470 core_explore_federated_search_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.713950 core_explore_federated_search_app-2.3.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.747427 core_explore_federated_search_app-2.3.0/tests/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/tests/components/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1073 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/tests/components/data/tests_int_access_control.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.778882 core_explore_federated_search_app-2.3.0/tests/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/tests/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3029 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/tests/fixtures/fixtures.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.792292 core_explore_federated_search_app-2.3.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.827485 core_explore_federated_search_app-2.3.0/tests/rest/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/tests/rest/result/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.859014 core_explore_federated_search_app-2.3.0/tests/rest/result/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:37.000000 core_explore_federated_search_app-2.3.0/tests/rest/result/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      956 2023-05-02 19:37:38.000000 core_explore_federated_search_app-2.3.0/tests/rest/result/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1864 2023-05-02 19:37:38.000000 core_explore_federated_search_app-2.3.0/tests/rest/result/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2165 2023-05-02 19:37:38.000000 core_explore_federated_search_app-2.3.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      907 2023-05-02 19:37:38.000000 core_explore_federated_search_app-2.3.0/tests/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:40.890204 core_explore_federated_search_app-2.3.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:38.000000 core_explore_federated_search_app-2.3.0/tests/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5147 2023-05-02 19:37:38.000000 core_explore_federated_search_app-2.3.0/tests/views/tests_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:35.187889 core_explore_federated_search_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      174 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1555 2023-07-21 02:11:35.183906 core_explore_federated_search_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      967 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.341726 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.413717 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.438784 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/components/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      840 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/components/data/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.450432 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.474942 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.510391 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/rest/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/rest/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      354 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/rest/query/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5778 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/rest/query/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.543216 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/rest/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/rest/result/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      303 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/rest/result/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2758 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/rest/result/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      571 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      637 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.093382 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.127112 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/static/core_explore_federated_search_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.100309 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.102923 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.116710 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.120067 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.726461 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      986 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/delete.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      109 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/delete.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1231 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/edit.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      105 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/edit.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1965 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/refresh.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/refresh.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.140598 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.143675 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.739252 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/data_sources/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2419 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/data_sources/list.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.153273 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.209160 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.178522 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.786278 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.795457 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/add/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1538 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/add/add_base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      308 2023-07-21 02:11:31.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/add_repository.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.819413 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2267 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/list_base.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.847801 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      837 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/delete.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1459 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/edit.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1206 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/refresh.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/refresh_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      357 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list_repositories.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.212430 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.870709 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      663 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list-content.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1319 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      857 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.899140 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.953922 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5623 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2651 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.400809 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1555 2023-07-21 02:11:33.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3829 2023-07-21 02:11:33.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:11:33.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      117 2023-07-21 02:11:33.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2023-07-21 02:11:33.000000 core_explore_federated_search_app-2.4.0/core_explore_federated_search_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       85 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:11:35.189426 core_explore_federated_search_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1114 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:34.990554 core_explore_federated_search_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:35.001778 core_explore_federated_search_app-2.4.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:35.028912 core_explore_federated_search_app-2.4.0/tests/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/tests/components/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1073 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/tests/components/data/tests_int_access_control.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:35.072266 core_explore_federated_search_app-2.4.0/tests/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/tests/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3029 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/tests/fixtures/fixtures.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:35.084039 core_explore_federated_search_app-2.4.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:35.113485 core_explore_federated_search_app-2.4.0/tests/rest/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/tests/rest/result/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:35.145570 core_explore_federated_search_app-2.4.0/tests/rest/result/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/tests/rest/result/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      956 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/tests/rest/result/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1864 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/tests/rest/result/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2101 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      907 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:35.172540 core_explore_federated_search_app-2.4.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/tests/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5543 2023-07-21 02:11:32.000000 core_explore_federated_search_app-2.4.0/tests/views/tests_permissions.py
```

### Comparing `core_explore_federated_search_app-2.3.0/LICENSE.md` & `core_explore_federated_search_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.3.0/PKG-INFO` & `core_explore_federated_search_app-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_explore_federated_search_app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Federation exploration functions for curator core project
 Home-page: https://github.com/usnistgov/core_explore_federated_search_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =================================
         Core Explore Federated Search App
```

### Comparing `core_explore_federated_search_app-2.3.0/README.rst` & `core_explore_federated_search_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/components/data/api.py` & `core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/components/data/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/query/views.py` & `core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/rest/query/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """ REST views for the query API
 """
 import logging
 
 import pytz
 from django.urls import reverse
-from django.utils import timezone
 from rest_framework import status
 from rest_framework.decorators import schema
 from rest_framework.permissions import IsAuthenticated
 from rest_framework.response import Response
 from rest_framework.views import APIView
 
 import core_main_app.components.data.api as data_api
 from core_explore_common_app.components.result.models import Result
 from core_explore_common_app.rest.result.serializers import ResultSerializer
 from core_explore_common_app.utils.result import result as result_utils
-from core_explore_federated_search_app import settings
 from core_explore_federated_search_app.rest.query.serializers import (
     QueryExecuteSerializer,
 )
 from core_main_app.components.template import api as template_api
 from core_main_app.utils.pagination.rest_framework_paginator.pagination import (
     StandardResultsSetPagination,
 )
@@ -109,33 +107,14 @@
             if options is not None:
                 if "instance_name" in options:
                     instance_name = options["instance_name"]
 
             # Template info
             template_info = dict()
 
-            # Change timezone depending on the request arguments. Default to settings
-            # and ultimately to UTC if the setting is not present.
-            try:
-                user_timezone = pytz.timezone(
-                    request.META.get(
-                        "HTTP_TZ", getattr(settings, "TIME_ZONE", "UTC")
-                    )
-                )
-            except Exception as exc:
-                logger.error(
-                    f"Impossible to determine timezone from headers: {str(exc)}. Using "
-                    f"settings timezone info."
-                )
-                user_timezone = pytz.timezone(
-                    getattr(settings, "TIME_ZONE", "UTC")
-                )
-
-            timezone.activate(user_timezone)
-
             for data in page:
                 # get data's template
                 template = data.template
                 # get and store data's template information
                 if template not in template_info:
                     template_info[template] = result_utils.get_template_info(
                         template, include_template_id=False
```

### Comparing `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/result/views.py` & `core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/rest/result/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/rest/urls.py` & `core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/settings.py` & `core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/delete.js` & `core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/delete.js`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/edit.js` & `core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/edit.js`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/refresh.js` & `core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/refresh.js`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/data_sources/list.js` & `core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/data_sources/list.js`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/list_base.html` & `core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/list_base.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %}
+{% load tz %}
 
 {% block box_title %}List all repositories{% endblock %}
 
 {% block box_tools %}
-<div class="btn-group float-right">
+<div class="btn-group {% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3"%}float-end{% endif %}">
 <a href="{% url 'core-admin:core_explore_federated_search_app_repositories_add'%}" class="btn btn-secondary add-repository-btn">
     <i class="fas fa-plus-circle"></i> Add Repository
 </a>
 </div>
 {% endblock %}
 
 {% block box_body %}
@@ -21,15 +22,15 @@
         </tr>
 
         {% for instance in data.instance_list %}
             {% cycle 'even' '' as rowcolors silent %}
             <tr class="{{ rowcolors }}">
                 <td>{{ instance.name }}</td>
                 <td>{{ instance.endpoint }}</td>
-                <td>{{ instance.expires }}</td>
+                <td>{{ instance.expires|localtime }}</td>
                 <td id="{{ instance.id }}">
                     {% block box_actions %}
                         <span class="icon legend edit">
                             <a class="btn btn-secondary" href="#"><i class="fas fa-edit"></i> Edit </a>
                         </span>
                         <span class="icon legend refresh">
                             <a class="btn btn-secondary" href="#"><i class="fas fa-sync"></i> Refresh Token </a>
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
-{% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% block
-box_title %}List all repositories{% endblock %} {% block box_tools %}
+{% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% load tz %}
+{% block box_title %}List all repositories{% endblock %} {% block box_tools %}
+.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3"%}float-end{% endif %}">
  Add_Repository
 {% endblock %} {% block box_body %}
-Instance Name       Instance URL        Token expires       Actions
-                                                            {% block
-                                                            box_actions %}
-                    {                   {{ instance.expires  Edit
-{{ instance.name }} { instance.endpoint }}
-                    }}                                       Refresh_Token
-                                                                Delete   {%
-                                                            endblock %}
+Instance Name    Instance URL      Token expires              Actions
+                                                              {% block
+                 {                 {                          box_actions %}
+{{ instance.name {                 {                           Edit
+}}               instance.endpoint instance.expires|localtime
+                 }}                }}                          Refresh_Token
+                                                                  Delete   {%
+                                                              endblock %}
 There are currently no other repositories registered. Please add_a_new_one.
 {% endblock %} {% block box_footer %} {% endblock %}
```

### Comparing `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/edit.html` & `core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/edit.html`

 * *Files 22% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 {% block modal_id %}edit-repository-modal{% endblock %}
 {% block modal_title %}Edit Repository{% endblock %}
 
 {% block modal_body %}
 <div id="edit-error-div">
     <br/>
     <div class="alert alert-danger alert-dismissable">
-        <a href="#" class="close" data-dismiss="alert" aria-label="close">&times;</a>
+        <a href="#" {% if BOOTSTRAP_VERSION == "4.6.2" %}class="close" data-dismiss="alert"{% elif BOOTSTRAP_VERSION == "5.1.3" %}class="btn-close" data-bs-dismiss="alert"{% endif %} aria-label="close">{% if BOOTSTRAP_VERSION == "4.6.2" %}&times;{% elif BOOTSTRAP_VERSION == "5.1.3" %}{% endif %}</a>
         <strong><span id="edit-error-message"></span></strong>
     </div>
 </div>
 <form id="edit-repository-form">
     <input id="edit-repository-id" type="hidden" value=""/>
     <div class="form-group">
         <label for="edit-repository-name">Enter new {{ data.object_name }} name</label>
         <input id="edit-repository-name" class="form-control" type="text" value="" placeholder="new_repository_name"/>
     </div>
 </form>
 {% endblock %}
 
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Close</a>
+<a class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#">
+    <i class="fas fa-times"></i> Close
+</a>
 <a id="edit-repository-save" class="btn btn-primary" href="#"><i class="fas fa-save"></i> Save</a>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,11 +1,16 @@
  {% extends 'core_main_app/_render/admin/theme/tools/modal.html' %} {% block
 modal_id %}edit-repository-modal{% endblock %} {% block modal_title %}Edit
 Repository{% endblock %} {% block modal_body %}
 
-×
+% if BOOTSTRAP_VERSION == "4.6.2" %}class="close" data-dismiss="alert"{% elif
+BOOTSTRAP_VERSION == "5.1.3" %}class="btn-close" data-bs-dismiss="alert"{%
+endif %} aria-label="close">{% if BOOTSTRAP_VERSION == "4.6.2" %}×{% elif
+BOOTSTRAP_VERSION == "5.1.3" %}{% endif %}
+
 Enter new {{ data.object_name }} name [                    ]
 {% endblock %} {% block modal_footer %}
- Close
+% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION ==
+"5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#">  Close
 
  Save
  {% endblock %}
```

### Comparing `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/refresh.html` & `core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/refresh.html`

 * *Files 16% similar despite different names*

```diff
@@ -7,18 +7,20 @@
     <form id="refresh-repository-form">
         <input id="refresh-repository-id" type="hidden" value=""/>
     </form>
 
     <div id="error-div">
         <br/>
         <div class="alert alert-danger alert-dismissable">
-            <a href="#" class="close" data-dismiss="alert" aria-label="close">&times;</a>
+            <a href="#" {% if BOOTSTRAP_VERSION == "4.6.2" %}class="close" data-dismiss="alert"{% elif BOOTSTRAP_VERSION == "5.1.3" %}class="btn-close" data-bs-dismiss="alert"{% endif %} aria-label="close">{% if BOOTSTRAP_VERSION == "4.6.2" %}&times;{% elif BOOTSTRAP_VERSION == "5.1.3" %}{% endif %}</a>
             <strong><span id="error-message"></span></strong>
         </div>
     </div>
 
 {% endblock %}
 
 {% block modal_footer %}
-    <a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Close</a>
+    <a class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#">
+        <i class="fas fa-times"></i> Close
+    </a>
     <a id="refresh-repository-save" class="btn btn-primary" href="#"><i class="fas fa-sync"></i> Refresh</a>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,10 +1,15 @@
 {% extends 'core_main_app/_render/admin/theme/tools/modal.html' %} {% block
 modal_id %}refresh-repository-modal{% endblock %} {% block modal_title
 %}Refresh Token{% endblock %} {% block modal_body %}
 
-×
+% if BOOTSTRAP_VERSION == "4.6.2" %}class="close" data-dismiss="alert"{% elif
+BOOTSTRAP_VERSION == "5.1.3" %}class="btn-close" data-bs-dismiss="alert"{%
+endif %} aria-label="close">{% if BOOTSTRAP_VERSION == "4.6.2" %}×{% elif
+BOOTSTRAP_VERSION == "5.1.3" %}{% endif %}
+
 {% endblock %} {% block modal_footer %}
- Close
+% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION ==
+"5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#">  Close
 
  Refresh
  {% endblock %}
```

### Comparing `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list-content.html` & `core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list-content.html`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list.html` & `core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list.html`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 {% block data_sources_list %}
 <div>
     <div id="list-data-sources-federated-content" class="list-group-item">
     </div>
     <div id="error-div-federated" style="display: none;">
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
 {% load static %} {% block title%}Federated Search{% endblock %} {% block
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

### Comparing `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/urls.py` & `core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/views/user/ajax.py` & `core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app/views/user/views.py` & `core_explore_federated_search_app-2.4.0/core_explore_federated_search_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app.egg-info/PKG-INFO` & `core_explore_federated_search_app-2.4.0/core_explore_federated_search_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-explore-federated-search-app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Federation exploration functions for curator core project
 Home-page: https://github.com/usnistgov/core_explore_federated_search_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =================================
         Core Explore Federated Search App
```

### Comparing `core_explore_federated_search_app-2.3.0/core_explore_federated_search_app.egg-info/SOURCES.txt` & `core_explore_federated_search_app-2.4.0/core_explore_federated_search_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.3.0/setup.py` & `core_explore_federated_search_app-2.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_explore_federated_search_app",
-    version="2.3.0",
+    version="2.4.0",
     description="Federation exploration functions for curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_explore_federated_search_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_explore_federated_search_app-2.3.0/tests/components/data/tests_int_access_control.py` & `core_explore_federated_search_app-2.4.0/tests/components/data/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.3.0/tests/fixtures/fixtures.py` & `core_explore_federated_search_app-2.4.0/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.3.0/tests/rest/result/fixtures/fixtures.py` & `core_explore_federated_search_app-2.4.0/tests/rest/result/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.3.0/tests/rest/result/tests_int.py` & `core_explore_federated_search_app-2.4.0/tests/rest/result/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.3.0/tests/test_settings.py` & `core_explore_federated_search_app-2.4.0/tests/test_settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.sites",
     "django.contrib.staticfiles",
     # Extra apps
     "oauth2_provider",
     "defender",
-    "tz_detect",
     "menu",
     "django_celery_beat",
     # Local apps
     "core_main_app",
     "core_explore_common_app",
     "core_federated_search_app",
     "core_explore_federated_search_app",
@@ -41,15 +40,14 @@
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

### Comparing `core_explore_federated_search_app-2.3.0/tests/urls.py` & `core_explore_federated_search_app-2.4.0/tests/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.3.0/tests/views/tests_permissions.py` & `core_explore_federated_search_app-2.4.0/tests/views/tests_permissions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """ Permission tests on views
 """
 from django.test import RequestFactory, override_settings
+from tests.fixtures.fixtures import AccessControlDataFixture
 
 from core_explore_federated_search_app.views.user.ajax import (
     get_data_source_list_federated,
     update_data_source_list_federated,
 )
 from core_explore_federated_search_app.views.user.views import ViewData
 from core_main_app.utils.integration_tests.integration_base_test_case import (
     IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
-from tests.fixtures.fixtures import AccessControlDataFixture
 
 
 class TestGetDataSourceListFederated(IntegrationBaseTestCase):
     """Test Get Data Source List Federated"""
 
     def setUp(self):
         """setUp"""
@@ -93,15 +93,19 @@
             "id": str(self.fixture.data_no_workspace.id),
         }
         response = ViewData.as_view()(request)
         self.assertTrue(
             self.fixture.data_no_workspace.title
             not in response.content.decode()
         )
-        self.assertTrue("Error 403" in response.content.decode())
+        self.assertEqual(response.status_code, 302)
+        self.assertEqual(
+            response.url,
+            "/accounts/login/?next=/core_explore_federated_search_app_data_detail",
+        )
 
     @override_settings(CAN_ANONYMOUS_ACCESS_PUBLIC_DOCUMENT=False)
     def test_an_anonymous_user_can_not_access_a_data_that_is_in_a_private_workspace(
         self,
     ):
         """test_an_anonymous_user_can_not_access_a_data_that_is_in_a_private_workspace"""
 
@@ -114,15 +118,19 @@
             "id": str(self.fixture.data_workspace_1.id),
         }
         response = ViewData.as_view()(request)
         self.assertTrue(
             self.fixture.data_workspace_1.title
             not in response.content.decode()
         )
-        self.assertTrue("Error 403" in response.content.decode())
+        self.assertEqual(response.status_code, 302)
+        self.assertEqual(
+            response.url,
+            "/accounts/login/?next=/core_explore_federated_search_app_data_detail",
+        )
 
     @override_settings(CAN_ANONYMOUS_ACCESS_PUBLIC_DOCUMENT=False)
     def test_an_anonymous_user_can_not_access_a_data_that_is_in_a_public_workspace_and_access_setting_is_false(
         self,
     ):
         """test_an_anonymous_user_can_not_access_a_data_that_is_in_a_public_workspace_and_access_setting_is_false"""
         request = self.factory.get(
@@ -134,8 +142,12 @@
             "id": str(self.fixture.data_public_workspace.id),
         }
         response = ViewData.as_view()(request)
         self.assertTrue(
             self.fixture.data_public_workspace.title
             not in response.content.decode()
         )
-        self.assertTrue("Error 403" in response.content.decode())
+        self.assertEqual(response.status_code, 302)
+        self.assertEqual(
+            response.url,
+            "/accounts/login/?next=/core_explore_federated_search_app_data_detail",
+        )
```

