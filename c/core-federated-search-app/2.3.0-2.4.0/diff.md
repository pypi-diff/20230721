# Comparing `tmp/core_federated_search_app-2.3.0.tar.gz` & `tmp/core_federated_search_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_federated_search_app-2.3.0.tar", last modified: Tue May  2 19:39:00 2023, max compression
+gzip compressed data, was "core_federated_search_app-2.4.0.tar", last modified: Fri Jul 21 02:12:50 2023, max compression
```

## Comparing `core_federated_search_app-2.3.0.tar` & `core_federated_search_app-2.4.0.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.859924 core_federated_search_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1232 2023-05-02 19:39:00.855010 core_federated_search_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      720 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.802863 core_federated_search_app-2.3.0/core_federated_search_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       91 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1343 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      270 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.938668 core_federated_search_app-2.3.0/core_federated_search_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      229 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/commons/exceptions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.950908 core_federated_search_app-2.3.0/core_federated_search_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.003928 core_federated_search_app-2.3.0/core_federated_search_app/components/instance/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/components/instance/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5844 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/components/instance/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3739 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/components/instance/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.018235 core_federated_search_app-2.3.0/core_federated_search_app/components/instance/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/components/instance/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      501 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.045670 core_federated_search_app-2.3.0/core_federated_search_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1476 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.076849 core_federated_search_app-2.3.0/core_federated_search_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.127984 core_federated_search_app-2.3.0/core_federated_search_app/rest/instance/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/rest/instance/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1697 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/rest/instance/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8872 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/rest/instance/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      775 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      382 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.470459 core_federated_search_app-2.3.0/core_federated_search_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.474383 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.487309 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.145848 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/css/repositories.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.490764 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.494075 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.497520 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.243295 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      986 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/delete.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      101 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/delete.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1965 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/refresh.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/refresh.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.519059 core_federated_search_app-2.3.0/core_federated_search_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.522901 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.526750 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.273676 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.287142 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/add/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1014 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/add/add_base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      300 2023-05-02 19:38:56.000000 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/add_repository.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.327421 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2154 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/list_base.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.377797 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      722 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/delete.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      875 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/refresh.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/refresh_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      349 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list_repositories.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      216 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/core_federated_search_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.396896 core_federated_search_app-2.3.0/core_federated_search_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/core_federated_search_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.464623 core_federated_search_app-2.3.0/core_federated_search_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/core_federated_search_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3647 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/core_federated_search_app/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2712 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/core_federated_search_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3477 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/core_federated_search_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:59.900715 core_federated_search_app-2.3.0/core_federated_search_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1232 2023-05-02 19:38:58.000000 core_federated_search_app-2.3.0/core_federated_search_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3231 2023-05-02 19:38:59.000000 core_federated_search_app-2.3.0/core_federated_search_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:38:59.000000 core_federated_search_app-2.3.0/core_federated_search_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      135 2023-05-02 19:38:59.000000 core_federated_search_app-2.3.0/core_federated_search_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2023-05-02 19:38:59.000000 core_federated_search_app-2.3.0/core_federated_search_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.547165 core_federated_search_app-2.3.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11132 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      314 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       83 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:39:00.861613 core_federated_search_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1430 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.618840 core_federated_search_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.649797 core_federated_search_app-2.3.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.672615 core_federated_search_app-2.3.0/tests/components/instance/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/components/instance/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.711065 core_federated_search_app-2.3.0/tests/components/instance/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/components/instance/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4950 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/components/instance/api/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      150 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/mocks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.728796 core_federated_search_app-2.3.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.813991 core_federated_search_app-2.3.0/tests/rest/instance/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/rest/instance/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:00.842364 core_federated_search_app-2.3.0/tests/rest/instance/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/rest/instance/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      962 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/rest/instance/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7935 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/rest/instance/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10748 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/rest/instance/tests_permission.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2214 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/rest/instance/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1645 2023-05-02 19:38:57.000000 core_federated_search_app-2.3.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.732424 core_federated_search_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1232 2023-07-21 02:12:50.727975 core_federated_search_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      720 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.002700 core_federated_search_app-2.4.0/core_federated_search_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       91 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1343 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      270 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.082153 core_federated_search_app-2.4.0/core_federated_search_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      229 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/commons/exceptions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.105790 core_federated_search_app-2.4.0/core_federated_search_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.138954 core_federated_search_app-2.4.0/core_federated_search_app/components/instance/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/components/instance/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5844 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/components/instance/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3739 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/components/instance/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.162439 core_federated_search_app-2.4.0/core_federated_search_app/components/instance/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/components/instance/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      501 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.183884 core_federated_search_app-2.4.0/core_federated_search_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1476 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.208294 core_federated_search_app-2.4.0/core_federated_search_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.237176 core_federated_search_app-2.4.0/core_federated_search_app/rest/instance/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/rest/instance/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1697 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/rest/instance/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8872 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/rest/instance/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      775 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      382 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:49.704525 core_federated_search_app-2.4.0/core_federated_search_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:49.707256 core_federated_search_app-2.4.0/core_federated_search_app/static/core_federated_search_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:49.718391 core_federated_search_app-2.4.0/core_federated_search_app/static/core_federated_search_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.246465 core_federated_search_app-2.4.0/core_federated_search_app/static/core_federated_search_app/admin/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/static/core_federated_search_app/admin/css/repositories.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:49.721132 core_federated_search_app-2.4.0/core_federated_search_app/static/core_federated_search_app/admin/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:49.723912 core_federated_search_app-2.4.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:49.727005 core_federated_search_app-2.4.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.299435 core_federated_search_app-2.4.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      986 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/delete.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      101 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/delete.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1965 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/refresh.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/refresh.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:49.757007 core_federated_search_app-2.4.0/core_federated_search_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:49.760146 core_federated_search_app-2.4.0/core_federated_search_app/templates/core_federated_search_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:49.763203 core_federated_search_app-2.4.0/core_federated_search_app/templates/core_federated_search_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.332762 core_federated_search_app-2.4.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.341702 core_federated_search_app-2.4.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/add/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1540 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/add/add_base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      300 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/add_repository.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.362632 core_federated_search_app-2.4.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2274 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/list_base.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.382580 core_federated_search_app-2.4.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      837 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/delete.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1206 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/refresh.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/refresh_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      349 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list_repositories.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      216 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.404486 core_federated_search_app-2.4.0/core_federated_search_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.456501 core_federated_search_app-2.4.0/core_federated_search_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3647 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2712 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3477 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/core_federated_search_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.059836 core_federated_search_app-2.4.0/core_federated_search_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1232 2023-07-21 02:12:49.000000 core_federated_search_app-2.4.0/core_federated_search_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3231 2023-07-21 02:12:49.000000 core_federated_search_app-2.4.0/core_federated_search_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:12:49.000000 core_federated_search_app-2.4.0/core_federated_search_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      135 2023-07-21 02:12:49.000000 core_federated_search_app-2.4.0/core_federated_search_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2023-07-21 02:12:49.000000 core_federated_search_app-2.4.0/core_federated_search_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.514525 core_federated_search_app-2.4.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11132 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      314 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       83 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:12:50.734348 core_federated_search_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1430 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.559749 core_federated_search_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.579568 core_federated_search_app-2.4.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.594811 core_federated_search_app-2.4.0/tests/components/instance/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/tests/components/instance/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.626733 core_federated_search_app-2.4.0/tests/components/instance/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/tests/components/instance/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4950 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/tests/components/instance/api/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      150 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/tests/mocks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.638113 core_federated_search_app-2.4.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.688727 core_federated_search_app-2.4.0/tests/rest/instance/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/tests/rest/instance/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:50.716122 core_federated_search_app-2.4.0/tests/rest/instance/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/tests/rest/instance/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      962 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/tests/rest/instance/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7935 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/tests/rest/instance/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10748 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/tests/rest/instance/tests_permission.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2214 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/tests/rest/instance/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1645 2023-07-21 02:12:47.000000 core_federated_search_app-2.4.0/tests/test_settings.py
```

### Comparing `core_federated_search_app-2.3.0/LICENSE.md` & `core_federated_search_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.3.0/PKG-INFO` & `core_federated_search_app-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_federated_search_app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Federated search backend for the curator core project
 Home-page: https://github.com/usnistgov/core_federated_search_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =========================
         Core Federated Search App
```

### Comparing `core_federated_search_app-2.3.0/README.rst` & `core_federated_search_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.3.0/core_federated_search_app/admin.py` & `core_federated_search_app-2.4.0/core_federated_search_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.3.0/core_federated_search_app/components/instance/api.py` & `core_federated_search_app-2.4.0/core_federated_search_app/components/instance/api.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.3.0/core_federated_search_app/components/instance/models.py` & `core_federated_search_app-2.4.0/core_federated_search_app/components/instance/models.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.3.0/core_federated_search_app/migrations/0001_initial.py` & `core_federated_search_app-2.4.0/core_federated_search_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.3.0/core_federated_search_app/rest/instance/serializers.py` & `core_federated_search_app-2.4.0/core_federated_search_app/rest/instance/serializers.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.3.0/core_federated_search_app/rest/instance/views.py` & `core_federated_search_app-2.4.0/core_federated_search_app/rest/instance/views.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.3.0/core_federated_search_app/rest/urls.py` & `core_federated_search_app-2.4.0/core_federated_search_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/delete.js` & `core_federated_search_app-2.4.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/delete.js`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.3.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/refresh.js` & `core_federated_search_app-2.4.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/refresh.js`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/list_base.html` & `core_federated_search_app-2.4.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/list_base.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %}
+{% load tz %}
 
 {% block box_title %}List all repositories{% endblock %}
 
 {% block box_tools %}
-<div class="btn-group float-right">
+<div class="btn-group {% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}">
 <a href="{% url 'core-admin:core_federated_search_app_repositories_add'%}" class="btn btn-secondary add-repository-btn">
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
                         {% url 'core-admin:core_federated_search_app_repositories_edit' instance.id as edit_url %}
                         {% include 'core_main_app/common/buttons/edit.html' with label='Rename' %}
                         <span class="icon legend refresh">
                             <a class="btn btn-secondary" href="#"><i class="fas fa-sync"></i> Refresh Token </a>
                         </span>
```

#### html2text {}

```diff
@@ -1,14 +1,16 @@
-{% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% block
-box_title %}List all repositories{% endblock %} {% block box_tools %}
+{% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% load tz %}
+{% block box_title %}List all repositories{% endblock %} {% block box_tools %}
+.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif
+%}">
  Add_Repository
 {% endblock %} {% block box_body %}
-Instance Name Instance URL      Token expires    Actions
-                                                 {% block box_actions %} {% url 'core-admin:
-{             {                 {                core_federated_search_app_repositories_edit'
-{             {                 {                instance.id as edit_url %} {% include
-instance.name instance.endpoint instance.expires 'core_main_app/common/buttons/edit.html'
-}}            }}                }}               with label='Rename' %}
-                                                  Refresh_Token
-                                                     Delete   {% endblock %}
+Instance Name Instance URL      Token expires              Actions
+                                                           {% block box_actions %} {% url 'core-admin:
+{             {                 {                          core_federated_search_app_repositories_edit'
+{             {                 {                          instance.id as edit_url %} {% include
+instance.name instance.endpoint instance.expires|localtime 'core_main_app/common/buttons/edit.html'
+}}            }}                }}                         with label='Rename' %}
+                                                            Refresh_Token
+                                                               Delete   {% endblock %}
 There are currently no other repositories registered. Please add_a_new_one.
 {% endblock %} {% block box_footer %} {% endblock %}
```

### Comparing `core_federated_search_app-2.3.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/refresh.html` & `core_federated_search_app-2.4.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/refresh.html`

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

### Comparing `core_federated_search_app-2.3.0/core_federated_search_app/views/admin/ajax.py` & `core_federated_search_app-2.4.0/core_federated_search_app/views/admin/ajax.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.3.0/core_federated_search_app/views/admin/forms.py` & `core_federated_search_app-2.4.0/core_federated_search_app/views/admin/forms.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.3.0/core_federated_search_app/views/admin/views.py` & `core_federated_search_app-2.4.0/core_federated_search_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.3.0/core_federated_search_app.egg-info/PKG-INFO` & `core_federated_search_app-2.4.0/core_federated_search_app.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-federated-search-app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Federated search backend for the curator core project
 Home-page: https://github.com/usnistgov/core_federated_search_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =========================
         Core Federated Search App
```

### Comparing `core_federated_search_app-2.3.0/core_federated_search_app.egg-info/SOURCES.txt` & `core_federated_search_app-2.4.0/core_federated_search_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.3.0/docs/conf.py` & `core_federated_search_app-2.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.3.0/setup.py` & `core_federated_search_app-2.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_federated_search_app",
-    version="2.3.0",
+    version="2.4.0",
     description="Federated search backend for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_federated_search_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_federated_search_app-2.3.0/tests/components/instance/api/tests_unit.py` & `core_federated_search_app-2.4.0/tests/components/instance/api/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.3.0/tests/rest/instance/fixtures/fixtures.py` & `core_federated_search_app-2.4.0/tests/rest/instance/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.3.0/tests/rest/instance/tests_int.py` & `core_federated_search_app-2.4.0/tests/rest/instance/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.3.0/tests/rest/instance/tests_permission.py` & `core_federated_search_app-2.4.0/tests/rest/instance/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.3.0/tests/rest/instance/tests_unit.py` & `core_federated_search_app-2.4.0/tests/rest/instance/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.3.0/tests/test_settings.py` & `core_federated_search_app-2.4.0/tests/test_settings.py`

 * *Files identical despite different names*

