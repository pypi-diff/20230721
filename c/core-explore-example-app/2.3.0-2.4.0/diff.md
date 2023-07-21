# Comparing `tmp/core_explore_example_app-2.3.0.tar.gz` & `tmp/core_explore_example_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_explore_example_app-2.3.0.tar", last modified: Tue May  2 19:37:25 2023, max compression
+gzip compressed data, was "core_explore_example_app-2.4.0.tar", last modified: Fri Jul 21 02:11:25 2023, max compression
```

## Comparing `core_explore_example_app-2.3.0.tar` & `core_explore_example_app-2.4.0.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:25.055685 core_explore_example_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1114 2023-05-02 19:37:25.050897 core_explore_example_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      614 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:22.721799 core_explore_example_app-2.3.0/core_explore_example_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      634 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:22.860450 core_explore_example_app-2.3.0/core_explore_example_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      205 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/commons/exceptions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:22.879463 core_explore_example_app-2.3.0/core_explore_example_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.062487 core_explore_example_app-2.3.0/core_explore_example_app/components/explore_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/explore_data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      442 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/explore_data_structure/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2006 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/explore_data_structure/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1764 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/explore_data_structure/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.147187 core_explore_example_app-2.3.0/core_explore_example_app/components/persistent_query_example/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/persistent_query_example/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/persistent_query_example/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2283 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/persistent_query_example/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1973 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/persistent_query_example/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.228171 core_explore_example_app-2.3.0/core_explore_example_app/components/saved_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/saved_query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      356 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/saved_query/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      904 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/saved_query/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1565 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/components/saved_query/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      927 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      321 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.280526 core_explore_example_app-2.3.0/core_explore_example_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4401 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1058 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.334501 core_explore_example_app-2.3.0/core_explore_example_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1723 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/permissions/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      320 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/permissions/rights.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.367622 core_explore_example_app-2.3.0/core_explore_example_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.430000 core_explore_example_app-2.3.0/core_explore_example_app/rest/persistent_query_example/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/rest/persistent_query_example/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3259 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/rest/persistent_query_example/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13206 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/rest/persistent_query_example/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.479024 core_explore_example_app-2.3.0/core_explore_example_app/rest/saved_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/rest/saved_query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      395 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/rest/saved_query/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4767 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/rest/saved_query/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1653 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      620 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:22.306677 core_explore_example_app-2.3.0/core_explore_example_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:22.310787 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:22.320340 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.533027 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      724 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/css/query_builder.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      465 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/css/style.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/css/xsd_form.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.670482 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14448 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1044 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      147 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/buttons.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/choice.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      320 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/persistent_query.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/refresh_sorting.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       49 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/refresh_sorting.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1268 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/select_fields.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      138 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/select_fields.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.707906 core_explore_example_app-2.3.0/core_explore_example_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      371 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/system/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1140 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:22.347662 core_explore_example_app-2.3.0/core_explore_example_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:22.351891 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.795719 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3030 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/build_query.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/errors.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1044 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/index.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.818653 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      429 2023-05-02 19:37:18.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/list/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:23.894486 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1023 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/modals/custom_tree.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      535 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/modals/delete_all_queries.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      565 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/modals/delete_query.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      391 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/modals/errors.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      652 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/modals/sub_elements_query_builder.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.144893 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       86 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/add.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      148 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/and_or_not.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/criteria_select.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/enum.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      144 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/field_input.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/gregorian_strict_match.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/initial_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       64 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/input.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      403 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/new_criteria.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      749 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/new_query.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      244 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/numeric_select.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      103 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/remove.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      116 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/string_select.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      493 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/sub_elements_query.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/yes_no.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      648 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/results.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      489 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/select_fields.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3787 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.260571 core_explore_example_app-2.3.0/core_explore_example_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1775 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/utils/custom_checkbox_renderer.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4373 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/utils/displayed_query.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15354 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/utils/mongo_query.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2998 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/utils/parser.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10108 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/utils/query_builder.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1899 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/utils/xml.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.291060 core_explore_example_app-2.3.0/core_explore_example_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.313038 core_explore_example_app-2.3.0/core_explore_example_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/views/admin/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.366705 core_explore_example_app-2.3.0/core_explore_example_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21425 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19641 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/core_explore_example_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:22.829761 core_explore_example_app-2.3.0/core_explore_example_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1114 2023-05-02 19:37:21.000000 core_explore_example_app-2.3.0/core_explore_example_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7513 2023-05-02 19:37:22.000000 core_explore_example_app-2.3.0/core_explore_example_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:37:21.000000 core_explore_example_app-2.3.0/core_explore_example_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      146 2023-05-02 19:37:21.000000 core_explore_example_app-2.3.0/core_explore_example_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-05-02 19:37:21.000000 core_explore_example_app-2.3.0/core_explore_example_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.423854 core_explore_example_app-2.3.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11127 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       93 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:37:25.057653 core_explore_example_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1420 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.473058 core_explore_example_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.488567 core_explore_example_app-2.3.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.539673 core_explore_example_app-2.3.0/tests/components/explore_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/tests/components/explore_data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2970 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/tests/components/explore_data_structure/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.586778 core_explore_example_app-2.3.0/tests/components/persistent_query_example/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/tests/components/persistent_query_example/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.634273 core_explore_example_app-2.3.0/tests/components/persistent_query_example/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:19.000000 core_explore_example_app-2.3.0/tests/components/persistent_query_example/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1899 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/components/persistent_query_example/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15632 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/components/persistent_query_example/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6827 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/components/persistent_query_example/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.667850 core_explore_example_app-2.3.0/tests/components/saved_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/components/saved_query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3113 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/components/saved_query/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      132 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/mocks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.684881 core_explore_example_app-2.3.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.738428 core_explore_example_app-2.3.0/tests/rest/persistent_query_example/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/rest/persistent_query_example/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11760 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/rest/persistent_query_example/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17575 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/rest/persistent_query_example/tests_permissions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.822812 core_explore_example_app-2.3.0/tests/rest/saved_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/rest/saved_query/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.857122 core_explore_example_app-2.3.0/tests/rest/saved_query/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/rest/saved_query/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1333 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/rest/saved_query/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4655 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/rest/saved_query/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5717 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/rest/saved_query/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1614 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.873888 core_explore_example_app-2.3.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.936221 core_explore_example_app-2.3.0/tests/utils/mongo_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/utils/mongo_query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7156 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/utils/mongo_query/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.969924 core_explore_example_app-2.3.0/tests/utils/xml/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/utils/xml/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1633 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/utils/xml/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:24.986060 core_explore_example_app-2.3.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:25.032931 core_explore_example_app-2.3.0/tests/views/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/views/ajax/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11066 2023-05-02 19:37:20.000000 core_explore_example_app-2.3.0/tests/views/ajax/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:25.059258 core_explore_example_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1114 2023-07-21 02:11:25.055884 core_explore_example_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      614 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:17.306422 core_explore_example_app-2.4.0/core_explore_example_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      634 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:17.404215 core_explore_example_app-2.4.0/core_explore_example_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      205 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/commons/exceptions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:17.418588 core_explore_example_app-2.4.0/core_explore_example_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:17.487152 core_explore_example_app-2.4.0/core_explore_example_app/components/explore_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/components/explore_data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      442 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/components/explore_data_structure/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2006 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/components/explore_data_structure/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1764 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/components/explore_data_structure/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:17.538795 core_explore_example_app-2.4.0/core_explore_example_app/components/persistent_query_example/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/components/persistent_query_example/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/components/persistent_query_example/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2283 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/components/persistent_query_example/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1973 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/components/persistent_query_example/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:17.598559 core_explore_example_app-2.4.0/core_explore_example_app/components/saved_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/components/saved_query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      356 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/components/saved_query/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      904 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/components/saved_query/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1565 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/components/saved_query/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      927 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      321 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:17.624138 core_explore_example_app-2.4.0/core_explore_example_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4401 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1058 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:17.664931 core_explore_example_app-2.4.0/core_explore_example_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1723 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/permissions/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      320 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/permissions/rights.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:17.692880 core_explore_example_app-2.4.0/core_explore_example_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:17.737682 core_explore_example_app-2.4.0/core_explore_example_app/rest/persistent_query_example/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/rest/persistent_query_example/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3259 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/rest/persistent_query_example/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13206 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/rest/persistent_query_example/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:17.786776 core_explore_example_app-2.4.0/core_explore_example_app/rest/saved_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/rest/saved_query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      395 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/rest/saved_query/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4767 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/rest/saved_query/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1653 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      620 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:16.877279 core_explore_example_app-2.4.0/core_explore_example_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:16.880527 core_explore_example_app-2.4.0/core_explore_example_app/static/core_explore_example_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:16.887983 core_explore_example_app-2.4.0/core_explore_example_app/static/core_explore_example_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:18.780772 core_explore_example_app-2.4.0/core_explore_example_app/static/core_explore_example_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      724 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/static/core_explore_example_app/user/css/query_builder.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      465 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/static/core_explore_example_app/user/css/style.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/static/core_explore_example_app/user/css/xsd_form.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:19.554289 core_explore_example_app-2.4.0/core_explore_example_app/static/core_explore_example_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14448 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1044 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      147 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/static/core_explore_example_app/user/js/buttons.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/static/core_explore_example_app/user/js/choice.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      320 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/static/core_explore_example_app/user/js/persistent_query.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/static/core_explore_example_app/user/js/refresh_sorting.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       49 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/static/core_explore_example_app/user/js/refresh_sorting.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1268 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/static/core_explore_example_app/user/js/select_fields.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      138 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/static/core_explore_example_app/user/js/select_fields.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:19.584064 core_explore_example_app-2.4.0/core_explore_example_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      371 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/system/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1140 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:16.902914 core_explore_example_app-2.4.0/core_explore_example_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:16.906054 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:21.329434 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3127 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/build_query.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/errors.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1044 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/index.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:21.343800 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      429 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/list/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:21.428439 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1131 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/modals/custom_tree.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      643 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/modals/delete_all_queries.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      673 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/modals/delete_query.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      499 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/modals/errors.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      760 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/modals/sub_elements_query_builder.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:23.669553 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       86 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/add.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      148 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/and_or_not.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/criteria_select.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/enum.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      144 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/field_input.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/gregorian_strict_match.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/initial_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       64 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/input.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      403 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/new_criteria.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      749 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/new_query.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      244 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/numeric_select.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      103 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/remove.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      116 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/string_select.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      493 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/sub_elements_query.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/yes_no.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      744 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/results.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      489 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/select_fields.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3787 2023-07-21 02:11:13.000000 core_explore_example_app-2.4.0/core_explore_example_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:24.393428 core_explore_example_app-2.4.0/core_explore_example_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/core_explore_example_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1775 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/core_explore_example_app/utils/custom_checkbox_renderer.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4373 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/core_explore_example_app/utils/displayed_query.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15354 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/core_explore_example_app/utils/mongo_query.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2998 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/core_explore_example_app/utils/parser.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10108 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/core_explore_example_app/utils/query_builder.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1899 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/core_explore_example_app/utils/xml.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:24.407750 core_explore_example_app-2.4.0/core_explore_example_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/core_explore_example_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:24.425613 core_explore_example_app-2.4.0/core_explore_example_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/core_explore_example_app/views/admin/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:24.472985 core_explore_example_app-2.4.0/core_explore_example_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/core_explore_example_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21380 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/core_explore_example_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19641 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/core_explore_example_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:17.375456 core_explore_example_app-2.4.0/core_explore_example_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1114 2023-07-21 02:11:16.000000 core_explore_example_app-2.4.0/core_explore_example_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7513 2023-07-21 02:11:16.000000 core_explore_example_app-2.4.0/core_explore_example_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:11:16.000000 core_explore_example_app-2.4.0/core_explore_example_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      146 2023-07-21 02:11:16.000000 core_explore_example_app-2.4.0/core_explore_example_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-07-21 02:11:16.000000 core_explore_example_app-2.4.0/core_explore_example_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:24.552252 core_explore_example_app-2.4.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11127 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       93 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:11:25.060768 core_explore_example_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1420 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:24.600754 core_explore_example_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:24.616797 core_explore_example_app-2.4.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:24.655034 core_explore_example_app-2.4.0/tests/components/explore_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/components/explore_data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2970 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/components/explore_data_structure/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:24.702161 core_explore_example_app-2.4.0/tests/components/persistent_query_example/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/components/persistent_query_example/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:24.735123 core_explore_example_app-2.4.0/tests/components/persistent_query_example/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/components/persistent_query_example/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1899 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/components/persistent_query_example/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15632 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/components/persistent_query_example/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6827 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/components/persistent_query_example/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:24.769012 core_explore_example_app-2.4.0/tests/components/saved_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/components/saved_query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3113 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/components/saved_query/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      132 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/mocks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:24.786894 core_explore_example_app-2.4.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:24.835058 core_explore_example_app-2.4.0/tests/rest/persistent_query_example/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/rest/persistent_query_example/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11760 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/rest/persistent_query_example/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17575 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/rest/persistent_query_example/tests_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:24.896538 core_explore_example_app-2.4.0/tests/rest/saved_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/rest/saved_query/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:24.925946 core_explore_example_app-2.4.0/tests/rest/saved_query/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/rest/saved_query/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1333 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/rest/saved_query/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4655 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/rest/saved_query/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5717 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/rest/saved_query/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1614 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:24.939479 core_explore_example_app-2.4.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:24.967779 core_explore_example_app-2.4.0/tests/utils/mongo_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/utils/mongo_query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7156 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/utils/mongo_query/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:24.993211 core_explore_example_app-2.4.0/tests/utils/xml/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/utils/xml/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1633 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/utils/xml/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:25.005046 core_explore_example_app-2.4.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:25.044795 core_explore_example_app-2.4.0/tests/views/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/views/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11066 2023-07-21 02:11:14.000000 core_explore_example_app-2.4.0/tests/views/ajax/tests_unit.py
```

### Comparing `core_explore_example_app-2.3.0/LICENSE.md` & `core_explore_example_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/PKG-INFO` & `core_explore_example_app-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_explore_example_app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Exploration by example for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_example_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ========================
         Core Explore Example App
```

### Comparing `core_explore_example_app-2.3.0/README.rst` & `core_explore_example_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/admin.py` & `core_explore_example_app-2.4.0/core_explore_example_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/apps.py` & `core_explore_example_app-2.4.0/core_explore_example_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/components/explore_data_structure/api.py` & `core_explore_example_app-2.4.0/core_explore_example_app/components/explore_data_structure/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/components/explore_data_structure/models.py` & `core_explore_example_app-2.4.0/core_explore_example_app/components/explore_data_structure/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/components/persistent_query_example/api.py` & `core_explore_example_app-2.4.0/core_explore_example_app/components/persistent_query_example/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/components/persistent_query_example/models.py` & `core_explore_example_app-2.4.0/core_explore_example_app/components/persistent_query_example/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/components/saved_query/api.py` & `core_explore_example_app-2.4.0/core_explore_example_app/components/saved_query/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/components/saved_query/models.py` & `core_explore_example_app-2.4.0/core_explore_example_app/components/saved_query/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/discover.py` & `core_explore_example_app-2.4.0/core_explore_example_app/discover.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/migrations/0001_initial.py` & `core_explore_example_app-2.4.0/core_explore_example_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/models.py` & `core_explore_example_app-2.4.0/core_explore_example_app/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/permissions/discover.py` & `core_explore_example_app-2.4.0/core_explore_example_app/permissions/discover.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/rest/persistent_query_example/serializers.py` & `core_explore_example_app-2.4.0/core_explore_example_app/rest/persistent_query_example/serializers.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/rest/persistent_query_example/views.py` & `core_explore_example_app-2.4.0/core_explore_example_app/rest/persistent_query_example/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/rest/saved_query/views.py` & `core_explore_example_app-2.4.0/core_explore_example_app/rest/saved_query/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/rest/urls.py` & `core_explore_example_app-2.4.0/core_explore_example_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/settings.py` & `core_explore_example_app-2.4.0/core_explore_example_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/css/query_builder.css` & `core_explore_example_app-2.4.0/core_explore_example_app/static/core_explore_example_app/user/css/query_builder.css`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.js` & `core_explore_example_app-2.4.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.js`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.raw.js` & `core_explore_example_app-2.4.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.raw.js`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/refresh_sorting.js` & `core_explore_example_app-2.4.0/core_explore_example_app/static/core_explore_example_app/user/js/refresh_sorting.js`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/static/core_explore_example_app/user/js/select_fields.js` & `core_explore_example_app-2.4.0/core_explore_example_app/static/core_explore_example_app/user/js/select_fields.js`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/tasks.py` & `core_explore_example_app-2.4.0/core_explore_example_app/tasks.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/build_query.html` & `core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/build_query.html`

 * *Files 17% similar despite different names*

```diff
@@ -11,23 +11,23 @@
         {% if data.query_form%}
             {{data.query_form|safe}}
             {%else%}
             <div id="queryForm">
             {% include data.query_builder_interface|safe %}
             </div>
         {% endif %}
-        <form class="ml-4">
+        <form class="{% if BOOTSTRAP_VERSION == "4.6.2" %}ml-4{% elif BOOTSTRAP_VERSION == "5.1.3" %}ms-4{% endif %}">
             <button type="button" class="btn btn-danger" onclick="clearCriteria()">
                 <i class="fas fa-eraser"></i> Clear
             </button>
             {% if user|has_perm:'core_explore_example_app.save_query' %}
             <button type="button" class="btn btn-secondary" onclick="saveQuery()">
                 <i class="fas fa-save"></i> Save Query
             </button>
-            {%endif%}
+            {% endif %}
             <button type="button" class="btn btn-primary" onclick="submit_query()">
                 <i class="fas fa-search"></i> Submit Query
             </button>
         </form>
     </div>
     <div class="col-sm-4">
         {% include data.data_sources_selector_template %}
@@ -55,15 +55,15 @@
                     </td>
                     <td>
                         {% if user|has_perm:'core_explore_example_app.delete_query' %}
                         <span class="btn btn-danger delete-query"
                               onclick="deleteQuery('query{{ query.id }}')">
                             <i class="fas fa-trash"></i>  Delete
                         </span>
-                        {%endif%}
+                        {% endif %}
                         <span class="btn btn-primary add-query"
                               onclick="addSavedQueryToForm('query{{ query.id }}')">
                             <i class="fas fa-arrow-circle-up"></i> Add to Query
                         </span>
                     </td>
                 </tr>
                 {% endfor %}
@@ -74,14 +74,14 @@
         </table>
     </div>
     <form>
         {% if user|has_perm:'core_explore_example_app.delete_query' %}
         <button type="button" class="btn btn-danger" onclick="clearQueries()">
             <i class="fas fa-trash"></i> Delete All
         </button>
-        {%endif%}
+        {% endif %}
     </form>
 </div>
 {% endif %}
 
 
 <div id="template_id" class="hidden">{{data.template_id}}</div>
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
 {% load auth_extras %}
 ***** Perform Search *****
 {{ data.description }}
 **** {{ data.title }} ****
 {% if data.query_form%} {{data.query_form|safe}} {%else%}
 {% include data.query_builder_interface|safe %}
 {% endif %}
-  Clear  {% if user|has_perm:'core_explore_example_app.save_query' %}   Save
-Query  {%endif%}   Submit Query
+.6.2" %}ml-4{% elif BOOTSTRAP_VERSION == "5.1.3" %}ms-4{% endif %}">   Clear
+{% if user|has_perm:'core_explore_example_app.save_query' %}   Save Query  {%
+endif %}   Submit Query
 {% include data.data_sources_selector_template %}
 {% if user.is_authenticated %}
 ===============================================================================
 **** Saved Queries ****
 Queries                          Actions
                                  {% if user|has_perm:
 {{ query.displayed_query|safe }} 'core_explore_example_app.delete_query' %}
-                                 Delete  {%endif%}   Add to Query
+                                 Delete  {% endif %}   Add to Query
 No Saved Queries for now.
-{% if user|has_perm:'core_explore_example_app.delete_query' %}   Delete All
-{%endif%}
+{% if user|has_perm:'core_explore_example_app.delete_query' %}   Delete All  {%
+endif %}
 {% endif %}
 {{data.template_id}}
```

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/index.html` & `core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/index.html`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/modals/custom_tree.html` & `core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/modals/custom_tree.html`

 * *Files 16% similar despite different names*

```diff
@@ -22,9 +22,11 @@
     and select the elements that you want to use in your queries.
     </div>
     {% endif %}
 </div>
 <div id="current_criteria" style="display:none;"></div>
 {% endblock %}
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
+<a class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#">
+    <i class="fas fa-times"></i> Cancel
+</a>
 {% endblock %}
```

#### html2text {}

```diff
@@ -4,9 +4,10 @@
 {% if data.custom_form %} Select the element that you want to insert in the
 query. You can customize this view by selecting_new_fields . {
 {data.custom_form|safe}} {% else %}
 You should customize the template first. Go_back_to_'Select_Fields' and select
 the elements that you want to use in your queries.
 {% endif %}
 {% endblock %} {% block modal_footer %}
- Cancel
+% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION ==
+"5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#">  Cancel
  {% endblock %}
```

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/modals/delete_all_queries.html` & `core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/modals/delete_all_queries.html`

 * *Files 16% similar despite different names*

```diff
@@ -3,11 +3,13 @@
 {% block modal_id %}delete-all-queries-modal{% endblock %}
 {% block modal_title %}Delete All Queries{% endblock %}
 
 {% block modal_body %}
 <p>Are you sure you want to delete all your saved queries?</p>
 {% endblock %}
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
+<a class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#">
+    <i class="fas fa-times"></i> Cancel
+</a>
 <button id="delete-all-queries" class="btn btn-danger"><i class="fas fa-trash"></i> Delete</button>
 {% endblock %}
```

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/new_query.html` & `core_explore_example_app-2.4.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/new_query.html`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/urls.py` & `core_explore_example_app-2.4.0/core_explore_example_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/utils/custom_checkbox_renderer.py` & `core_explore_example_app-2.4.0/core_explore_example_app/utils/custom_checkbox_renderer.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/utils/displayed_query.py` & `core_explore_example_app-2.4.0/core_explore_example_app/utils/displayed_query.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/utils/mongo_query.py` & `core_explore_example_app-2.4.0/core_explore_example_app/utils/mongo_query.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/utils/parser.py` & `core_explore_example_app-2.4.0/core_explore_example_app/utils/parser.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/utils/query_builder.py` & `core_explore_example_app-2.4.0/core_explore_example_app/utils/query_builder.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/utils/xml.py` & `core_explore_example_app-2.4.0/core_explore_example_app/utils/xml.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/views/user/ajax.py` & `core_explore_example_app-2.4.0/core_explore_example_app/views/user/ajax.py`

 * *Files 1% similar despite different names*

```diff
@@ -710,9 +710,8 @@
 
     @staticmethod
     def _create_persistent_query(query):
         # create the persistent query
         return PersistentQueryExample(
             user_id=query.user_id,
             content=query.content,
-            data_sources=query.data_sources,
         )
```

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app/views/user/views.py` & `core_explore_example_app-2.4.0/core_explore_example_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app.egg-info/PKG-INFO` & `core_explore_example_app-2.4.0/core_explore_example_app.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-explore-example-app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Exploration by example for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_example_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ========================
         Core Explore Example App
```

### Comparing `core_explore_example_app-2.3.0/core_explore_example_app.egg-info/SOURCES.txt` & `core_explore_example_app-2.4.0/core_explore_example_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/docs/conf.py` & `core_explore_example_app-2.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/setup.py` & `core_explore_example_app-2.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_explore_example_app",
-    version="2.3.0",
+    version="2.4.0",
     description="Exploration by example for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_explore_example_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_explore_example_app-2.3.0/tests/components/explore_data_structure/tests_unit.py` & `core_explore_example_app-2.4.0/tests/components/explore_data_structure/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/tests/components/persistent_query_example/fixtures/fixtures.py` & `core_explore_example_app-2.4.0/tests/components/persistent_query_example/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/tests/components/persistent_query_example/tests_int_access_control.py` & `core_explore_example_app-2.4.0/tests/components/persistent_query_example/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/tests/components/persistent_query_example/tests_unit.py` & `core_explore_example_app-2.4.0/tests/components/persistent_query_example/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/tests/components/saved_query/tests_unit.py` & `core_explore_example_app-2.4.0/tests/components/saved_query/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/tests/rest/persistent_query_example/tests_int.py` & `core_explore_example_app-2.4.0/tests/rest/persistent_query_example/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/tests/rest/persistent_query_example/tests_permissions.py` & `core_explore_example_app-2.4.0/tests/rest/persistent_query_example/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/tests/rest/saved_query/fixtures/fixtures.py` & `core_explore_example_app-2.4.0/tests/rest/saved_query/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/tests/rest/saved_query/tests_int.py` & `core_explore_example_app-2.4.0/tests/rest/saved_query/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/tests/rest/saved_query/tests_permissions.py` & `core_explore_example_app-2.4.0/tests/rest/saved_query/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/tests/test_settings.py` & `core_explore_example_app-2.4.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/tests/utils/mongo_query/tests_unit.py` & `core_explore_example_app-2.4.0/tests/utils/mongo_query/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/tests/utils/xml/tests_unit.py` & `core_explore_example_app-2.4.0/tests/utils/xml/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.3.0/tests/views/ajax/tests_unit.py` & `core_explore_example_app-2.4.0/tests/views/ajax/tests_unit.py`

 * *Files identical despite different names*

