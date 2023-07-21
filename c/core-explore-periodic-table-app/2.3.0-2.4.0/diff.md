# Comparing `tmp/core_explore_periodic_table_app-2.3.0.tar.gz` & `tmp/core_explore_periodic_table_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_explore_periodic_table_app-2.3.0.tar", last modified: Tue May  2 19:38:29 2023, max compression
+gzip compressed data, was "core_explore_periodic_table_app-2.4.0.tar", last modified: Fri Jul 21 02:12:20 2023, max compression
```

## Comparing `core_explore_periodic_table_app-2.3.0.tar` & `core_explore_periodic_table_app-2.4.0.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.531302 core_explore_periodic_table_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:38:24.000000 core_explore_periodic_table_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-05-02 19:38:24.000000 core_explore_periodic_table_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2483 2023-05-02 19:38:29.525944 core_explore_periodic_table_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1671 2023-05-02 19:38:24.000000 core_explore_periodic_table_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.223165 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      128 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1189 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      525 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.347982 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.404736 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      391 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2524 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2094 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.466100 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/search_operator_mapping/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/search_operator_mapping/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      342 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/search_operator_mapping/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1124 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/search_operator_mapping/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1053 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/search_operator_mapping/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      498 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.495948 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3194 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      597 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.572561 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1166 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/permissions/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      187 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/permissions/rights.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.609959 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.670008 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3598 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13622 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.726074 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/search_operator_mapping/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/search_operator_mapping/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1455 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/search_operator_mapping/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8161 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/search_operator_mapping/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1947 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      135 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:27.802888 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:27.845489 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.744183 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/admin/form.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:27.824311 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.760705 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/xsd/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5699 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/xsd/default_chemical_element_type.xsd
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:27.856914 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:27.852135 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.780691 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/periodic_table/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1747 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/periodic_table/periodic.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.795607 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.811925 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/periodic_table/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5531 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/periodic_table/periodic.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      354 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/persistent_query.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:27.874597 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:27.896242 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:27.881298 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.832643 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      382 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/manage_periodic_table_type.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.847373 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/selector/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      425 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/selector/selector.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.885326 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      914 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/index.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.900873 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/periodic_table/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7406 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/periodic_table/periodic.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.917985 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/selector/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      250 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/selector/data_sources_selector.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1001 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.937184 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.987829 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1570 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3600 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.048840 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      728 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2016 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/user/form.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14617 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:28.299639 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2483 2023-05-02 19:38:27.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4827 2023-05-02 19:38:27.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:38:27.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      110 2023-05-02 19:38:27.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:38:27.000000 core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       26 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:38:29.553960 core_explore_periodic_table_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1463 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.081654 core_explore_periodic_table_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.097543 core_explore_periodic_table_app-2.3.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.156423 core_explore_periodic_table_app-2.3.0/tests/components/persistent_query_periodic_table/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/components/persistent_query_periodic_table/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.200154 core_explore_periodic_table_app-2.3.0/tests/components/persistent_query_periodic_table/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/components/persistent_query_periodic_table/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1788 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/components/persistent_query_periodic_table/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17193 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/components/persistent_query_periodic_table/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7296 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/components/persistent_query_periodic_table/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.235514 core_explore_periodic_table_app-2.3.0/tests/components/search_operators_mapping/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/components/search_operators_mapping/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4467 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/components/search_operators_mapping/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.255232 core_explore_periodic_table_app-2.3.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.311167 core_explore_periodic_table_app-2.3.0/tests/rest/persistent_query_periodic_table/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/rest/persistent_query_periodic_table/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12797 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/rest/persistent_query_periodic_table/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18854 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/rest/persistent_query_periodic_table/tests_permissions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.375695 core_explore_periodic_table_app-2.3.0/tests/rest/search_operators_mapping/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/rest/search_operators_mapping/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.412801 core_explore_periodic_table_app-2.3.0/tests/rest/search_operators_mapping/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/rest/search_operators_mapping/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3042 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/rest/search_operators_mapping/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4434 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/rest/search_operators_mapping/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11061 2023-05-02 19:38:25.000000 core_explore_periodic_table_app-2.3.0/tests/rest/search_operators_mapping/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1902 2023-05-02 19:38:26.000000 core_explore_periodic_table_app-2.3.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.436392 core_explore_periodic_table_app-2.3.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:26.000000 core_explore_periodic_table_app-2.3.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.455752 core_explore_periodic_table_app-2.3.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:26.000000 core_explore_periodic_table_app-2.3.0/tests/views/user/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:29.499180 core_explore_periodic_table_app-2.3.0/tests/views/user/forms/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:26.000000 core_explore_periodic_table_app-2.3.0/tests/views/user/forms/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1902 2023-05-02 19:38:26.000000 core_explore_periodic_table_app-2.3.0/tests/views/user/forms/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.745403 core_explore_periodic_table_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:12:16.000000 core_explore_periodic_table_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-07-21 02:12:16.000000 core_explore_periodic_table_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2483 2023-07-21 02:12:20.741976 core_explore_periodic_table_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1671 2023-07-21 02:12:16.000000 core_explore_periodic_table_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:19.798599 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      128 2023-07-21 02:12:16.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1189 2023-07-21 02:12:16.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      525 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:19.879758 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:19.920438 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      391 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2524 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2094 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:19.959749 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/components/search_operator_mapping/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/components/search_operator_mapping/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      342 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/components/search_operator_mapping/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1124 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/components/search_operator_mapping/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1053 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/components/search_operator_mapping/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      498 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:19.979975 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3194 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      597 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.015497 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1166 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/permissions/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      187 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/permissions/rights.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.037124 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.071121 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3598 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13622 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.115568 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/rest/search_operator_mapping/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/rest/search_operator_mapping/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1455 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/rest/search_operator_mapping/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8161 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/rest/search_operator_mapping/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1947 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      135 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:19.513590 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:19.529407 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.130343 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/admin/form.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:19.523481 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.150864 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/xsd/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5699 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/xsd/default_chemical_element_type.xsd
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:19.558261 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:19.553909 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.163822 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/periodic_table/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1747 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/periodic_table/periodic.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.175073 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.187059 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/periodic_table/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5531 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/periodic_table/periodic.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      354 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/persistent_query.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:19.572708 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:19.585873 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:19.578102 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.200963 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      382 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/manage_periodic_table_type.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.215178 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/selector/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      425 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/selector/selector.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.241038 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      914 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/index.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.252445 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/periodic_table/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7406 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/periodic_table/periodic.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.264280 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/selector/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      250 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/selector/data_sources_selector.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1001 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.280289 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.322599 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1570 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3603 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.371145 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      728 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2016 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/views/user/form.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14617 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:19.867953 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2483 2023-07-21 02:12:19.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4827 2023-07-21 02:12:19.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:12:19.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      110 2023-07-21 02:12:19.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:12:19.000000 core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       26 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:12:20.746899 core_explore_periodic_table_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1463 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.402395 core_explore_periodic_table_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.417343 core_explore_periodic_table_app-2.4.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.461372 core_explore_periodic_table_app-2.4.0/tests/components/persistent_query_periodic_table/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/tests/components/persistent_query_periodic_table/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.487151 core_explore_periodic_table_app-2.4.0/tests/components/persistent_query_periodic_table/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/tests/components/persistent_query_periodic_table/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1788 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/tests/components/persistent_query_periodic_table/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17193 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/tests/components/persistent_query_periodic_table/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7296 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/tests/components/persistent_query_periodic_table/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.521899 core_explore_periodic_table_app-2.4.0/tests/components/search_operators_mapping/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/tests/components/search_operators_mapping/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4467 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/tests/components/search_operators_mapping/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.532658 core_explore_periodic_table_app-2.4.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.578122 core_explore_periodic_table_app-2.4.0/tests/rest/persistent_query_periodic_table/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/tests/rest/persistent_query_periodic_table/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12797 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/tests/rest/persistent_query_periodic_table/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18854 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/tests/rest/persistent_query_periodic_table/tests_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.631731 core_explore_periodic_table_app-2.4.0/tests/rest/search_operators_mapping/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/tests/rest/search_operators_mapping/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.672084 core_explore_periodic_table_app-2.4.0/tests/rest/search_operators_mapping/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/tests/rest/search_operators_mapping/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3042 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/tests/rest/search_operators_mapping/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4434 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/tests/rest/search_operators_mapping/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11061 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/tests/rest/search_operators_mapping/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1855 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.686220 core_explore_periodic_table_app-2.4.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.704280 core_explore_periodic_table_app-2.4.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/tests/views/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:20.731569 core_explore_periodic_table_app-2.4.0/tests/views/user/forms/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/tests/views/user/forms/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1902 2023-07-21 02:12:17.000000 core_explore_periodic_table_app-2.4.0/tests/views/user/forms/tests_unit.py
```

### Comparing `core_explore_periodic_table_app-2.3.0/LICENSE.md` & `core_explore_periodic_table_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/PKG-INFO` & `core_explore_periodic_table_app-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_explore_periodic_table_app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Core explore periodic table capabilities for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_periodic_table_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_explore_periodic_table_app
         ===============================
```

### Comparing `core_explore_periodic_table_app-2.3.0/README.rst` & `core_explore_periodic_table_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/admin.py` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/apps.py` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/api.py` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/models.py` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/search_operator_mapping/api.py` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/components/search_operator_mapping/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/components/search_operator_mapping/models.py` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/components/search_operator_mapping/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/migrations/0001_initial.py` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/models.py` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/permissions/discover.py` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/permissions/discover.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/serializers.py` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/serializers.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/views.py` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/search_operator_mapping/serializers.py` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/rest/search_operator_mapping/serializers.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/search_operator_mapping/views.py` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/rest/search_operator_mapping/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/rest/urls.py` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/xsd/default_chemical_element_type.xsd` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/xsd/default_chemical_element_type.xsd`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/periodic_table/periodic.css` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/periodic_table/periodic.css`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/periodic_table/periodic.js` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/periodic_table/periodic.js`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/index.html` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/index.html`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/periodic_table/periodic.html` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/periodic_table/periodic.html`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/urls.py` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/admin/forms.py` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/views/admin/forms.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/admin/views.py` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/views/admin/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     # load the form
     associated_form = AssociatedPeriodicTableSearchOperatorForm()
     assets = {"css": ["core_explore_periodic_table_app/admin/form.css"]}
 
     context = {"associated_form": associated_form}
 
     messages.add_message(
-        request, messages.INFO, "Information saved with success."
+        request, messages.SUCCESS, "Information saved with success."
     )
 
     return admin_render(
         request,
         "core_explore_periodic_table_app/admin/periodic_table_type/manage_periodic_table_type.html",
         context=context,
         assets=assets,
```

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/user/ajax.py` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/user/form.py` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/views/user/form.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app/views/user/views.py` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app.egg-info/PKG-INFO` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-explore-periodic-table-app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Core explore periodic table capabilities for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_periodic_table_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_explore_periodic_table_app
         ===============================
```

### Comparing `core_explore_periodic_table_app-2.3.0/core_explore_periodic_table_app.egg-info/SOURCES.txt` & `core_explore_periodic_table_app-2.4.0/core_explore_periodic_table_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/setup.py` & `core_explore_periodic_table_app-2.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_explore_periodic_table_app",
-    version="2.3.0",
+    version="2.4.0",
     description="Core explore periodic table capabilities for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_explore_periodic_table_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_explore_periodic_table_app-2.3.0/tests/components/persistent_query_periodic_table/fixtures/fixtures.py` & `core_explore_periodic_table_app-2.4.0/tests/components/persistent_query_periodic_table/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/tests/components/persistent_query_periodic_table/tests_int_access_control.py` & `core_explore_periodic_table_app-2.4.0/tests/components/persistent_query_periodic_table/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/tests/components/persistent_query_periodic_table/tests_unit.py` & `core_explore_periodic_table_app-2.4.0/tests/components/persistent_query_periodic_table/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/tests/components/search_operators_mapping/tests_unit.py` & `core_explore_periodic_table_app-2.4.0/tests/components/search_operators_mapping/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/tests/rest/persistent_query_periodic_table/tests_int.py` & `core_explore_periodic_table_app-2.4.0/tests/rest/persistent_query_periodic_table/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/tests/rest/persistent_query_periodic_table/tests_permissions.py` & `core_explore_periodic_table_app-2.4.0/tests/rest/persistent_query_periodic_table/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/tests/rest/search_operators_mapping/fixtures/fixtures.py` & `core_explore_periodic_table_app-2.4.0/tests/rest/search_operators_mapping/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/tests/rest/search_operators_mapping/tests_int.py` & `core_explore_periodic_table_app-2.4.0/tests/rest/search_operators_mapping/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/tests/rest/search_operators_mapping/tests_permissions.py` & `core_explore_periodic_table_app-2.4.0/tests/rest/search_operators_mapping/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.3.0/tests/test_settings.py` & `core_explore_periodic_table_app-2.4.0/tests/test_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,14 @@
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

### Comparing `core_explore_periodic_table_app-2.3.0/tests/views/user/forms/tests_unit.py` & `core_explore_periodic_table_app-2.4.0/tests/views/user/forms/tests_unit.py`

 * *Files identical despite different names*

