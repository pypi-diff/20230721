# Comparing `tmp/core_curate_app-2.3.0.tar.gz` & `tmp/core_curate_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_curate_app-2.3.0.tar", last modified: Tue May  2 19:35:41 2023, max compression
+gzip compressed data, was "core_curate_app-2.4.0.tar", last modified: Fri Jul 21 02:09:59 2023, max compression
```

## Comparing `core_curate_app-2.3.0.tar` & `core_curate_app-2.4.0.tar`

### file list

```diff
@@ -1,146 +1,173 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.925579 core_curate_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      138 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2023-05-02 19:35:41.921128 core_curate_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      532 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.131051 core_curate_app-2.3.0/core_curate_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       73 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.228402 core_curate_app-2.3.0/core_curate_app/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2987 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/access_control/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1017 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      478 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.258601 core_curate_app-2.3.0/core_curate_app/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/common/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      207 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/common/exceptions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.274563 core_curate_app-2.3.0/core_curate_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.333337 core_curate_app-2.3.0/core_curate_app/components/curate_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/components/curate_data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      464 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/components/curate_data_structure/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4953 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/components/curate_data_structure/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5888 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/components/curate_data_structure/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      233 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.363319 core_curate_app-2.3.0/core_curate_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2186 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      738 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.416331 core_curate_app-2.3.0/core_curate_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1306 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/permissions/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      221 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/permissions/rights.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.452454 core_curate_app-2.3.0/core_curate_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.517094 core_curate_app-2.3.0/core_curate_app/rest/curate_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/rest/curate_data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1396 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/rest/curate_data_structure/admin_serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2131 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/rest/curate_data_structure/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11996 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/rest/curate_data_structure/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      668 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1174 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:39.767322 core_curate_app-2.3.0/core_curate_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:39.770696 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:39.784551 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.673718 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      481 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/css/common.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2033 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/css/style.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      683 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/css/xsd_form.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.710049 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/img/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      246 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/img/collapse.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      253 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/img/expand.png
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.974284 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      157 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/buttons.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/choice.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      168 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/download.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9748 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/enter_data.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      357 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/enter_data.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6638 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/select_template.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/select_template.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/text_editor.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1083 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/view_data.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      108 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/view_data.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3595 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:39.795538 core_curate_app-2.3.0/core_curate_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:39.809405 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.010326 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      366 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/admin/detail.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      348 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/admin/view_curate_data_structure.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.045981 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      167 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/common/detail_curate_data_structure.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      173 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/common/tools_curate_data_structure.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.147903 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1266 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/curate.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1191 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/curate_full_start.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      628 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/curate_start.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.171407 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1854 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/enter_data.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.314778 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      575 2023-05-02 19:35:36.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/cancel-changes.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      671 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/cancel-form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      579 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/clear-fields.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1137 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/download-options.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      549 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/save-form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      857 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/use-validation.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      361 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/validation-warning.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      383 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/xml-error.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      702 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/xml-valid.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.330408 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-review/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.346074 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-review/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      376 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-review/modals/save-error.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      973 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-review/view_data.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      318 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/detail.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/errors.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.362487 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      207 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/list/list.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3259 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.397655 core_curate_app-2.3.0/core_curate_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      764 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/utils/parser.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.419642 core_curate_app-2.3.0/core_curate_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.462331 core_curate_app-2.3.0/core_curate_app/views/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/views/common/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7151 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/views/common/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.535393 core_curate_app-2.3.0/core_curate_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19505 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2923 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/views/user/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19644 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/core_curate_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:40.200031 core_curate_app-2.3.0/core_curate_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2023-05-02 19:35:39.000000 core_curate_app-2.3.0/core_curate_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5075 2023-05-02 19:35:39.000000 core_curate_app-2.3.0/core_curate_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:35:39.000000 core_curate_app-2.3.0/core_curate_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       88 2023-05-02 19:35:39.000000 core_curate_app-2.3.0/core_curate_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       27 2023-05-02 19:35:39.000000 core_curate_app-2.3.0/core_curate_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.583020 core_curate_app-2.3.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11286 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:35:41.927206 core_curate_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1508 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.631082 core_curate_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.647068 core_curate_app-2.3.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.704787 core_curate_app-2.3.0/tests/components/curate_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/components/curate_data_structure/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.755722 core_curate_app-2.3.0/tests/components/curate_data_structure/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/components/curate_data_structure/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2541 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/components/curate_data_structure/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19295 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/components/curate_data_structure/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11642 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/components/curate_data_structure/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.782599 core_curate_app-2.3.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.835129 core_curate_app-2.3.0/tests/rest/curate_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/rest/curate_data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11287 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/rest/curate_data_structure/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13049 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/rest/curate_data_structure/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1687 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3522 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:41.896044 core_curate_app-2.3.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1046 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/views/test_forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9661 2023-05-02 19:35:37.000000 core_curate_app-2.3.0/tests/views/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2995 2023-05-02 19:35:38.000000 core_curate_app-2.3.0/tests/views/tests_views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:59.455540 core_curate_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      138 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2023-07-21 02:09:59.451503 core_curate_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      532 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:57.506966 core_curate_app-2.4.0/core_curate_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       73 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:57.652432 core_curate_app-2.4.0/core_curate_app/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2987 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/access_control/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1236 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      478 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:57.686074 core_curate_app-2.4.0/core_curate_app/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/common/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      207 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/common/exceptions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:57.722355 core_curate_app-2.4.0/core_curate_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:57.802700 core_curate_app-2.4.0/core_curate_app/components/curate_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/components/curate_data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      464 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/components/curate_data_structure/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5762 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/components/curate_data_structure/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6244 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/components/curate_data_structure/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      233 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:57.829730 core_curate_app-2.4.0/core_curate_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2186 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      738 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:57.881739 core_curate_app-2.4.0/core_curate_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1306 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/permissions/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      221 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/permissions/rights.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:57.917940 core_curate_app-2.4.0/core_curate_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:57.986277 core_curate_app-2.4.0/core_curate_app/rest/curate_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/rest/curate_data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1396 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/rest/curate_data_structure/admin_serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2131 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/rest/curate_data_structure/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11996 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/rest/curate_data_structure/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      668 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1243 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:57.133439 core_curate_app-2.4.0/core_curate_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:57.147728 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:57.158315 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:58.035122 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      682 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/css/common.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2033 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/css/style.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      668 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/css/xsd_form.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:58.066988 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/img/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      246 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/img/collapse.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      253 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/img/expand.png
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:58.245700 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      157 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/js/buttons.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/js/choice.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      168 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/js/download.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9863 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/js/enter_data.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      357 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/js/enter_data.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6638 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/js/select_template.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/js/select_template.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2023-07-21 02:09:53.000000 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/js/text_editor.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1083 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/js/view_data.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      108 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/js/view_data.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:58.274996 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      598 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip/popover.bs4.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      922 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip/popover.bs5.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3495 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:57.170689 core_curate_app-2.4.0/core_curate_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:57.181613 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:58.307834 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      366 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/admin/detail.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      348 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/admin/view_curate_data_structure.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:58.348627 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      167 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/common/detail_curate_data_structure.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      269 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/common/tools_curate_data_structure.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:58.431989 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1266 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/curate.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1876 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/curate_full_start.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      628 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/curate_start.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:58.447376 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/data-entry/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2420 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/data-entry/enter_data.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:58.594370 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      677 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/cancel-changes.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      773 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/cancel-form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      687 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/clear-fields.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1240 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/download-options.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      657 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/save-form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      959 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/use-validation.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      361 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/validation-warning.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      490 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/xml-error.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      813 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/xml-valid.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:58.610724 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/data-review/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:58.627025 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/data-review/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      478 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/data-review/modals/save-error.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1382 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/data-review/view_data.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      318 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/detail.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/errors.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:58.643646 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      207 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/list/list.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3259 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:58.677867 core_curate_app-2.4.0/core_curate_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      764 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/utils/parser.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:58.693753 core_curate_app-2.4.0/core_curate_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:58.725431 core_curate_app-2.4.0/core_curate_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1844 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/views/admin/ajax.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:58.754958 core_curate_app-2.4.0/core_curate_app/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/views/common/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7376 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/views/common/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:58.816305 core_curate_app-2.4.0/core_curate_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19737 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3170 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/views/user/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20130 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/core_curate_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:57.612159 core_curate_app-2.4.0/core_curate_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2023-07-21 02:09:56.000000 core_curate_app-2.4.0/core_curate_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5826 2023-07-21 02:09:57.000000 core_curate_app-2.4.0/core_curate_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:09:56.000000 core_curate_app-2.4.0/core_curate_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       88 2023-07-21 02:09:56.000000 core_curate_app-2.4.0/core_curate_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       27 2023-07-21 02:09:56.000000 core_curate_app-2.4.0/core_curate_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:58.868464 core_curate_app-2.4.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11286 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:09:59.457066 core_curate_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1508 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:58.908371 core_curate_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:58.922319 core_curate_app-2.4.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:59.020645 core_curate_app-2.4.0/tests/components/curate_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/tests/components/curate_data_structure/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:59.060440 core_curate_app-2.4.0/tests/components/curate_data_structure/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/tests/components/curate_data_structure/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5370 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/tests/components/curate_data_structure/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4891 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/tests/components/curate_data_structure/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20058 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/tests/components/curate_data_structure/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14205 2023-07-21 02:09:54.000000 core_curate_app-2.4.0/tests/components/curate_data_structure/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:59.077562 core_curate_app-2.4.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:55.000000 core_curate_app-2.4.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:59.145768 core_curate_app-2.4.0/tests/rest/curate_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:55.000000 core_curate_app-2.4.0/tests/rest/curate_data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11366 2023-07-21 02:09:55.000000 core_curate_app-2.4.0/tests/rest/curate_data_structure/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13049 2023-07-21 02:09:55.000000 core_curate_app-2.4.0/tests/rest/curate_data_structure/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1671 2023-07-21 02:09:55.000000 core_curate_app-2.4.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3466 2023-07-21 02:09:55.000000 core_curate_app-2.4.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:59.162938 core_curate_app-2.4.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:55.000000 core_curate_app-2.4.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:59.182970 core_curate_app-2.4.0/tests/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:55.000000 core_curate_app-2.4.0/tests/views/admin/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:59.217954 core_curate_app-2.4.0/tests/views/admin/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:55.000000 core_curate_app-2.4.0/tests/views/admin/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2685 2023-07-21 02:09:55.000000 core_curate_app-2.4.0/tests/views/admin/ajax/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:59.234285 core_curate_app-2.4.0/tests/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:55.000000 core_curate_app-2.4.0/tests/views/common/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:59.292894 core_curate_app-2.4.0/tests/views/common/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:55.000000 core_curate_app-2.4.0/tests/views/common/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2499 2023-07-21 02:09:55.000000 core_curate_app-2.4.0/tests/views/common/views/test_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6592 2023-07-21 02:09:55.000000 core_curate_app-2.4.0/tests/views/common/views/tests_int_access_control.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:59.317592 core_curate_app-2.4.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:55.000000 core_curate_app-2.4.0/tests/views/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:59.368621 core_curate_app-2.4.0/tests/views/user/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:55.000000 core_curate_app-2.4.0/tests/views/user/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10360 2023-07-21 02:09:55.000000 core_curate_app-2.4.0/tests/views/user/ajax/test_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4714 2023-07-21 02:09:55.000000 core_curate_app-2.4.0/tests/views/user/ajax/tests_int_access_control.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:59.399623 core_curate_app-2.4.0/tests/views/user/forms/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:55.000000 core_curate_app-2.4.0/tests/views/user/forms/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1849 2023-07-21 02:09:55.000000 core_curate_app-2.4.0/tests/views/user/forms/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:59.438883 core_curate_app-2.4.0/tests/views/user/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:55.000000 core_curate_app-2.4.0/tests/views/user/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5971 2023-07-21 02:09:55.000000 core_curate_app-2.4.0/tests/views/user/views/test_unit.py
```

### Comparing `core_curate_app-2.3.0/LICENSE.md` & `core_curate_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.3.0/PKG-INFO` & `core_curate_app-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_curate_app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Curation functionalities for the curator core project
 Home-page: https://github.com/usnistgov/core_curate_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ===============
         Core Curate App
```

### Comparing `core_curate_app-2.3.0/README.rst` & `core_curate_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.3.0/core_curate_app/access_control/api.py` & `core_curate_app-2.4.0/core_curate_app/access_control/api.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.3.0/core_curate_app/admin.py` & `core_curate_app-2.4.0/core_curate_app/admin.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,24 +9,30 @@
 from core_curate_app.components.curate_data_structure.admin_site import (
     CustomCurateDataStructureAdmin,
 )
 from core_curate_app.components.curate_data_structure.models import (
     CurateDataStructure,
 )
 from core_curate_app.views.common import views as common_views
+from core_curate_app.views.admin import ajax as admin_ajax
 
 admin_urls = [
     re_path(
         r"^view-form/(?P<curate_data_structure_id>\w+)$",
         staff_member_required(
             common_views.FormView.as_view(
                 administration=True,
                 template="core_curate_app/admin/view_curate_data_structure.html",
             )
         ),
         name="core_curate_view_form",
-    )
+    ),
+    re_path(
+        r"^delete-record-drafts/(?P<pk>\w+)$",
+        admin_ajax.delete_record_drafts,
+        name="core_curate_app_delete_data_drafts",
+    ),
 ]
 
 admin.site.register(CurateDataStructure, CustomCurateDataStructureAdmin)
 urls = core_admin_site.get_urls()
 core_admin_site.get_urls = lambda: admin_urls + urls
```

### Comparing `core_curate_app-2.3.0/core_curate_app/components/curate_data_structure/api.py` & `core_curate_app-2.4.0/core_curate_app/components/curate_data_structure/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -145,24 +145,25 @@
     Returns:
 
     """
     return CurateDataStructure.get_all_with_no_data()
 
 
 @access_control(can_read)
-def get_by_data_id(data_id, user):
-    """Return the curate data structure with the given data id
+def get_by_data_id_and_user(data_id, user):
+    """Return the curate data structure with the given data id and user
 
     Args:
         data_id:
+        user:
 
     Returns:
 
     """
-    return CurateDataStructure.get_by_data_id(data_id)
+    return CurateDataStructure.get_by_data_id_and_user(data_id, user.id)
 
 
 @access_control(can_read)
 def get_all_by_user(user):
     """Get all curate data that belong to user.
 
     Args:
@@ -222,7 +223,40 @@
         user:
         new_user:
 
     Returns:
     """
     curate_data_structure.user = str(new_user.id)
     curate_data_structure.save_object()
+
+
+@access_control(has_perm_administration)
+def get_all_curate_data_structures_by_data(data, user):
+    """Return all curate data structures with the given data.
+
+    Parameters:
+        data:
+        user:
+
+    Returns: curate data structure list
+    """
+
+    return CurateDataStructure.get_all_curate_data_structures_by_data(data)
+
+
+@access_control(has_perm_administration)
+def delete_curate_data_structures_by_data(data, user):
+    """delete curate data structures with the given data.
+
+    Parameters:
+        data:
+        user:
+
+    Returns
+    """
+
+    curate_data_structure_list = get_all_curate_data_structures_by_data(
+        data, user
+    )
+
+    for curate_data_structure in curate_data_structure_list:
+        delete(curate_data_structure, user)
```

### Comparing `core_curate_app-2.3.0/core_curate_app/components/curate_data_structure/models.py` & `core_curate_app-2.4.0/core_curate_app/components/curate_data_structure/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -165,25 +165,28 @@
 
         Returns:
 
         """
         return CurateDataStructure.objects.filter(user=str(user_id)).all()
 
     @staticmethod
-    def get_by_data_id(data_id):
-        """Return the curate data structure with the given data id
+    def get_by_data_id_and_user(data_id, user_id):
+        """Return the curate data structure with the given data id and user
 
         Args:
             data_id:
+            user_id:
 
         Returns:
 
         """
         try:
-            return CurateDataStructure.objects.get(data=str(data_id))
+            return CurateDataStructure.objects.get(
+                data=str(data_id), user=str(user_id)
+            )
         except ObjectDoesNotExist as exception:
             raise exceptions.DoesNotExist(str(exception))
         except Exception as exception:
             raise exceptions.ModelError(str(exception))
 
     @staticmethod
     def get_by_data_structure_element_root(data_structure_element_root):
@@ -209,10 +212,23 @@
 
         Returns:
 
         """
         not_empty_or_whitespaces(self.name)
         self.name = self.name.strip()
 
+    @staticmethod
+    def get_all_curate_data_structures_by_data(data):
+        """Get All Curate Data Structures By Data.
+
+        Args:
+            data:
+
+        Returns:
+
+        """
+
+        return CurateDataStructure.objects.filter(data=data.id).all()
+
 
 # Connect signals
 pre_delete.connect(DataStructure.pre_delete, sender=CurateDataStructure)
```

### Comparing `core_curate_app-2.3.0/core_curate_app/migrations/0001_initial.py` & `core_curate_app-2.4.0/core_curate_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.3.0/core_curate_app/models.py` & `core_curate_app-2.4.0/core_curate_app/models.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.3.0/core_curate_app/permissions/discover.py` & `core_curate_app-2.4.0/core_curate_app/permissions/discover.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.3.0/core_curate_app/rest/curate_data_structure/admin_serializers.py` & `core_curate_app-2.4.0/core_curate_app/rest/curate_data_structure/admin_serializers.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.3.0/core_curate_app/rest/curate_data_structure/serializers.py` & `core_curate_app-2.4.0/core_curate_app/rest/curate_data_structure/serializers.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.3.0/core_curate_app/rest/curate_data_structure/views.py` & `core_curate_app-2.4.0/core_curate_app/rest/curate_data_structure/views.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.3.0/core_curate_app/rest/urls.py` & `core_curate_app-2.4.0/core_curate_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.3.0/core_curate_app/settings.py` & `core_curate_app-2.4.0/core_curate_app/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,7 +30,9 @@
 LOCALE_PATHS = (os.path.join(BASE_DIR, "core_curate_app/locale"),)
 
 ENABLE_XML_ENTITIES_TOOLTIPS = getattr(
     settings, "ENABLE_XML_ENTITIES_TOOLTIPS", True
 )
 """ boolean: enable the xml entities warning tooltip on the GUI.
 """
+
+BOOTSTRAP_VERSION = getattr(settings, "BOOTSTRAP_VERSION", "5.1.3")
```

### Comparing `core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/css/style.css` & `core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/css/style.css`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/css/xsd_form.css` & `core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/css/xsd_form.css`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 	padding-left: 30px;
 }
 
 .xsdForm input{
 	width: 300px;
 	height: 30px;
 	margin: 0.3em;
-	padding: 0em;
 	display: inline;
 }
 
 .xsdForm input[type="radio"] {
 	width: 30px;
 }
```

### Comparing `core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/enter_data.js` & `core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/js/enter_data.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -116,19 +116,19 @@
     $.ajax({
         url: cancelFormUrl,
         type: "POST",
         data: {
             'id': objectID
         },
         dataType: "json",
-        success: function(data) {
+        success: function() {
             window.location = curateIndexUrl;
         },
-        error: function() {
-
+        error: function(dataXHR) {
+            $.notify(dataXHR.responseJSON.error, "danger");
         }
     });
 };
 
 
 /**
  * Display the saving confirmation popup
@@ -137,34 +137,31 @@
     $("#save-form-modal").modal("show");
 };
 
 /**
  * Save the form in the database
  */
 var sendSaveRequest = function() {
-
     var icon = $("[id^='btn-save-form'] > i").attr("class");
     // Show loading spinner
     showSpinner($("[id^='btn-save-form'] > i"))
 
     var objectID = $("#curate_data_structure_id").html();
     $.ajax({
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
-        error: function() {
-
+        error: function(dataXHR) {
+            $.notify(dataXHR.responseJSON.error, "danger");
         }
     }).always(function(data) {
         // get old button icon
         hideSpinner($("[id^='btn-save-form'] > i"), icon)
         $("#save-form-modal").modal("hide");
     });
 };
```

### Comparing `core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/select_template.js` & `core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/js/select_template.js`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/view_data.js` & `core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/js/view_data.js`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.3.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip.js` & `core_curate_app-2.4.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -6,58 +6,65 @@
 });
 
 /**
  * Find all the tooltip with the warning class in the DOM
  * @return jquerySelectorCollection or undefined if no result
  */
 var findFormWarningTooltip = function() {
-    var tooltipSelector = $(".tooltip-inner.warning-tooltip-inner");
+    var tooltipSelector = $(".popover-header.warning-popover-text");
     return tooltipSelector.length > 0 ? tooltipSelector : undefined;
 }
 
-
 /**
  * In the displayed form, check all the field and display warning tooltips if predefined XML entities are found
  */
 var checkPredefinedXmlEntities = function(selector) {
-    var template = '<div class="tooltip" role="tooltip"><div class="tooltip-arrow warning-tooltip-arrow"></div><div class="tooltip-inner warning-tooltip-inner"></div></div>'
-    selector = selector.val ? selector : $(this)
-    var value = selector.val();
-    value = value.replace(/((&amp;)|(&gt;)|(&lt;)|(&apos;)|(&quot;))/g, '');
-    if (value.indexOf('<') > -1 || value.indexOf('>') > -1 || value.indexOf('&') > -1 || value.indexOf('"') > -1 || value.indexOf("'") > -1) {
-        selector.tooltip({
-            title: "Warning! This field may contain predefined XML entities. These entities will be automatically escaped.",
-            template: template,
-            animation: true,
-            trigger: "manual",
-            placement: function(tip, element) {
-                var jqueryTip = $(tip);
-                jqueryTip.css('opacity', 0);
-                setTimeout(function() {
-                    var circleItemNumber = checkCircleItem(element);
-
-                    if (circleItemNumber > 0) {
-                        var tipLeftPosition = parseFloat(jqueryTip.css("left").replace("px", ""));
-                        tipLeftPosition += 25 * circleItemNumber;
-                        $(tip).css({
-                            left: tipLeftPosition + "px"
-                        });
-                    };
-
-                    jqueryTip.css('opacity', 1);
-                }, 100);
-
-                return "right";
-            }
-        });
-
-        selector.tooltip('show');
-    } else {
-        selector.tooltip("hide");
+    selector = selector.val ? selector : $(this);
+    let value = selector.val().replace(
+        /((&amp;)|(&gt;)|(&lt;)|(&apos;)|(&quot;))/g,
+        ""
+    );
+
+    if (!value.match("[<>&\"\']+")) { // No xml entities found.
+        hideTooltip(selector);
+        return;
+    }
+
+    let tooltipTitle = `Warning! This field may contain predefined XML 
+        entities. These entities will be automatically escaped.`
+    let tooltipOptions = {
+        title: tooltipTitle,
+        template: null,
+        animation: true,
+        trigger: "manual",
+        placement: function(tip, element) {
+            // Move the tooltip if there are + or - buttons.
+            let jqueryTip = $(tip);
+            jqueryTip.css('opacity', 0);
+            setTimeout(function() {
+                // Delay the computation to let the buttons be drawn first.
+                let circleItemNumber = checkCircleItem(element);
+
+                if (circleItemNumber > 0) {
+                    let tipLeftPosition = parseFloat(
+                        jqueryTip.css("left").replace("px", "")
+                    );
+                    tipLeftPosition += 25 * circleItemNumber;
+                    $(tip).css({
+                        left: tipLeftPosition + "px"
+                    });
+                }
+
+                jqueryTip.css('opacity', 1);
+            }, 100);
+
+            return "right";
+        }
     }
+    showTooltip(selector, tooltipOptions);
 }
 
 /**
  * For the first render of the form check the predefined Xml entities in all the fields
  */
 var refreshTooltipPosition = function() {
     var inputs = $('input.default');
```

### Comparing `core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/curate.html` & `core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/curate.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/curate_full_start.html` & `core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/curate_full_start.html`

 * *Files 26% similar despite different names*

```diff
@@ -12,64 +12,107 @@
 000000b0: 656e 6462 6c6f 636b 2025 7d0a 0a7b 2520  endblock %}..{% 
 000000c0: 626c 6f63 6b20 6d6f 6461 6c5f 626f 6479  block modal_body
 000000d0: 2025 7d0a 3c64 6976 2063 6c61 7373 3d22   %}.<div class="
 000000e0: 616c 6572 7420 616c 6572 742d 6461 6e67  alert alert-dang
 000000f0: 6572 2220 6964 3d22 6261 6e6e 6572 5f65  er" id="banner_e
 00000100: 7272 6f72 7322 2073 7479 6c65 3d22 6469  rrors" style="di
 00000110: 7370 6c61 793a 206e 6f6e 653b 223e 0a20  splay: none;">. 
-00000120: 2020 203c 6120 6872 6566 3d22 2322 2063     <a href="#" c
-00000130: 6c61 7373 3d22 636c 6f73 6522 2064 6174  lass="close" dat
-00000140: 612d 6869 6465 3d22 616c 6572 7422 2061  a-hide="alert" a
-00000150: 7269 612d 6c61 6265 6c3d 2263 6c6f 7365  ria-label="close
-00000160: 223e 2674 696d 6573 3b3c 2f61 3e0a 2020  ">&times;</a>.  
-00000170: 2020 3c68 343e 3c69 2063 6c61 7373 3d22    <h4><i class="
-00000180: 6661 7320 6661 2d65 7863 6c61 6d61 7469  fas fa-exclamati
-00000190: 6f6e 2d63 6972 636c 6522 3e3c 2f69 3e20  on-circle"></i> 
-000001a0: 4572 726f 723c 2f68 343e 0a20 2020 203c  Error</h4>.    <
-000001b0: 6469 7620 6964 3d22 666f 726d 5f73 7461  div id="form_sta
-000001c0: 7274 5f65 7272 6f72 7322 3e0a 3c2f 6469  rt_errors">.</di
-000001d0: 763e 0a3c 2f64 6976 3e0a 3c64 6976 2063  v>.</div>.<div c
-000001e0: 6c61 7373 3d22 706f 705f 6375 7261 7465  lass="pop_curate
-000001f0: 5f69 6e73 7472 7563 7469 6f6e 223e 0a20  _instruction">. 
-00000200: 2020 2050 6c65 6173 6520 6368 6f6f 7365     Please choose
-00000210: 206f 6e65 206f 6620 7468 6520 666f 6c6c   one of the foll
-00000220: 6f77 696e 6720 6f70 7469 6f6e 7320 746f  owing options to
-00000230: 2073 7461 7274 2063 7572 6174 696e 6720   start curating 
-00000240: 6120 7b25 2074 7261 6e73 2022 7265 636f  a {% trans "reco
-00000250: 7264 5f6c 6162 656c 2220 257d 3a0a 3c2f  rd_label" %}:.</
-00000260: 6469 763e 0a3c 6469 7620 6964 3d22 666f  div>.<div id="fo
-00000270: 726d 5f73 7461 7274 5f63 6f6e 7465 6e74  rm_start_content
-00000280: 223e 0a3c 2f64 6976 3e0a 7b25 2065 6e64  ">.</div>.{% end
-00000290: 626c 6f63 6b20 257d 0a0a 7b25 2062 6c6f  block %}..{% blo
-000002a0: 636b 206d 6f64 616c 5f66 6f6f 7465 7220  ck modal_footer 
-000002b0: 257d 0a3c 6275 7474 6f6e 2063 6c61 7373  %}.<button class
-000002c0: 3d22 6274 6e20 6274 6e2d 7365 636f 6e64  ="btn btn-second
-000002d0: 6172 7920 7075 6c6c 2d6c 6566 7422 2064  ary pull-left" d
-000002e0: 6174 612d 6469 736d 6973 733d 226d 6f64  ata-dismiss="mod
-000002f0: 616c 223e 3c69 2063 6c61 7373 3d22 6661  al"><i class="fa
-00000300: 7320 6661 2d74 696d 6573 223e 3c2f 693e  s fa-times"></i>
-00000310: 2043 616e 6365 6c3c 2f62 7574 746f 6e3e   Cancel</button>
-00000320: 0a3c 6469 7620 636c 6173 733d 2274 6578  .<div class="tex
-00000330: 742d 7269 6768 7422 3e0a 2020 2020 3c62  t-right">.    <b
-00000340: 7574 746f 6e20 6964 3d22 6274 6e2d 7361  utton id="btn-sa
-00000350: 7665 2d64 6174 6122 2063 6c61 7373 3d22  ve-data" class="
-00000360: 6274 6e20 6274 6e2d 7072 696d 6172 7922  btn btn-primary"
-00000370: 2068 6964 6465 6e3d 2222 3e3c 6920 636c   hidden=""><i cl
-00000380: 6173 733d 2266 6173 2066 612d 7361 7665  ass="fas fa-save
-00000390: 223e 3c2f 693e 2053 6176 6520 7769 7468  "></i> Save with
-000003a0: 6f75 7420 6564 6974 696e 673c 2f62 7574  out editing</but
-000003b0: 746f 6e3e 0a20 2020 203c 6275 7474 6f6e  ton>.    <button
-000003c0: 2069 643d 2262 746e 2d6f 7065 6e2d 6461   id="btn-open-da
-000003d0: 7461 2220 636c 6173 733d 2262 746e 2062  ta" class="btn b
-000003e0: 746e 2d70 7269 6d61 7279 223e 3c69 2063  tn-primary"><i c
-000003f0: 6c61 7373 3d22 6661 7320 6661 2d63 6f64  lass="fas fa-cod
-00000400: 6522 3e3c 2f69 3e20 4f70 656e 2069 6e20  e"></i> Open in 
-00000410: 5465 7874 2065 6469 746f 723c 2f62 7574  Text editor</but
-00000420: 746f 6e3e 0a20 2020 203c 6275 7474 6f6e  ton>.    <button
-00000430: 2069 643d 2262 746e 2d64 6973 706c 6179   id="btn-display
-00000440: 2d64 6174 6122 2063 6c61 7373 3d22 6274  -data" class="bt
-00000450: 6e20 6274 6e2d 7072 696d 6172 7922 3e3c  n btn-primary"><
-00000460: 6920 636c 6173 733d 2266 6173 2066 612d  i class="fas fa-
-00000470: 706c 6179 223e 3c2f 693e 2053 7461 7274  play"></i> Start
-00000480: 2065 6469 7469 6e67 3c2f 6275 7474 6f6e   editing</button
-00000490: 3e0a 3c2f 6469 763e 0a7b 2520 656e 6462  >.</div>.{% endb
-000004a0: 6c6f 636b 2025 7d                        lock %}
+00000120: 2020 203c 6275 7474 6f6e 2074 7970 653d     <button type=
+00000130: 2262 7574 746f 6e22 2061 7269 612d 6c61  "button" aria-la
+00000140: 6265 6c3d 2243 6c6f 7365 220a 2020 2020  bel="Close".    
+00000150: 2020 2020 2020 2020 7b25 2069 6620 424f          {% if BO
+00000160: 4f54 5354 5241 505f 5645 5253 494f 4e20  OTSTRAP_VERSION 
+00000170: 3d3d 2022 342e 362e 3222 2025 7d63 6c61  == "4.6.2" %}cla
+00000180: 7373 3d22 636c 6f73 6522 0a20 2020 2020  ss="close".     
+00000190: 2020 2020 2020 207b 2520 656c 6966 2042         {% elif B
+000001a0: 4f4f 5453 5452 4150 5f56 4552 5349 4f4e  OOTSTRAP_VERSION
+000001b0: 203d 3d20 2235 2e31 2e33 2220 257d 636c   == "5.1.3" %}cl
+000001c0: 6173 733d 2262 746e 2d63 6c6f 7365 2066  ass="btn-close f
+000001d0: 6c6f 6174 2d65 6e64 220a 2020 2020 2020  loat-end".      
+000001e0: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+000001f0: 7d0a 2020 2020 2020 2020 2020 2020 7b25  }.            {%
+00000200: 2069 6620 424f 4f54 5354 5241 505f 5645   if BOOTSTRAP_VE
+00000210: 5253 494f 4e20 3d3d 2022 342e 362e 3222  RSION == "4.6.2"
+00000220: 2025 7d64 6174 612d 6469 736d 6973 733d   %}data-dismiss=
+00000230: 2261 6c65 7274 220a 2020 2020 2020 2020  "alert".        
+00000240: 2020 2020 7b25 2065 6c69 6620 424f 4f54      {% elif BOOT
+00000250: 5354 5241 505f 5645 5253 494f 4e20 3d3d  STRAP_VERSION ==
+00000260: 2022 352e 312e 3322 2025 7d64 6174 612d   "5.1.3" %}data-
+00000270: 6273 2d64 6973 6d69 7373 3d22 616c 6572  bs-dismiss="aler
+00000280: 7422 0a20 2020 2020 2020 2020 2020 207b  t".            {
+00000290: 2520 656e 6469 6620 257d 0a20 2020 203e  % endif %}.    >
+000002a0: 0a20 2020 2020 2020 207b 2520 6966 2042  .        {% if B
+000002b0: 4f4f 5453 5452 4150 5f56 4552 5349 4f4e  OOTSTRAP_VERSION
+000002c0: 203d 3d20 2234 2e36 2e32 2220 257d 0a20   == "4.6.2" %}. 
+000002d0: 2020 2020 2020 2020 2020 203c 7370 616e             <span
+000002e0: 2061 7269 612d 6869 6464 656e 3d22 7472   aria-hidden="tr
+000002f0: 7565 223e 2674 696d 6573 3b3c 2f73 7061  ue">&times;</spa
+00000300: 6e3e 0a20 2020 2020 2020 207b 2520 656c  n>.        {% el
+00000310: 6966 2042 4f4f 5453 5452 4150 5f56 4552  if BOOTSTRAP_VER
+00000320: 5349 4f4e 203d 3d20 2235 2e31 2e33 2220  SION == "5.1.3" 
+00000330: 257d 0a20 2020 2020 2020 207b 2520 656e  %}.        {% en
+00000340: 6469 6620 257d 0a20 2020 203c 2f62 7574  dif %}.    </but
+00000350: 746f 6e3e 0a0a 2020 2020 3c68 343e 3c69  ton>..    <h4><i
+00000360: 2063 6c61 7373 3d22 6661 7320 6661 2d65   class="fas fa-e
+00000370: 7863 6c61 6d61 7469 6f6e 2d63 6972 636c  xclamation-circl
+00000380: 6522 3e3c 2f69 3e20 4572 726f 723c 2f68  e"></i> Error</h
+00000390: 343e 0a20 2020 203c 6469 7620 6964 3d22  4>.    <div id="
+000003a0: 666f 726d 5f73 7461 7274 5f65 7272 6f72  form_start_error
+000003b0: 7322 3e0a 3c2f 6469 763e 0a3c 2f64 6976  s">.</div>.</div
+000003c0: 3e0a 3c64 6976 2063 6c61 7373 3d22 706f  >.<div class="po
+000003d0: 705f 6375 7261 7465 5f69 6e73 7472 7563  p_curate_instruc
+000003e0: 7469 6f6e 223e 0a20 2020 2050 6c65 6173  tion">.    Pleas
+000003f0: 6520 6368 6f6f 7365 206f 6e65 206f 6620  e choose one of 
+00000400: 7468 6520 666f 6c6c 6f77 696e 6720 6f70  the following op
+00000410: 7469 6f6e 7320 746f 2073 7461 7274 2063  tions to start c
+00000420: 7572 6174 696e 6720 6120 7b25 2074 7261  urating a {% tra
+00000430: 6e73 2022 7265 636f 7264 5f6c 6162 656c  ns "record_label
+00000440: 2220 257d 3a0a 3c2f 6469 763e 0a3c 6469  " %}:.</div>.<di
+00000450: 7620 6964 3d22 666f 726d 5f73 7461 7274  v id="form_start
+00000460: 5f63 6f6e 7465 6e74 223e 0a3c 2f64 6976  _content">.</div
+00000470: 3e0a 7b25 2065 6e64 626c 6f63 6b20 257d  >.{% endblock %}
+00000480: 0a0a 7b25 2062 6c6f 636b 206d 6f64 616c  ..{% block modal
+00000490: 5f66 6f6f 7465 7220 257d 0a3c 6275 7474  _footer %}.<butt
+000004a0: 6f6e 2063 6c61 7373 3d22 6274 6e20 6274  on class="btn bt
+000004b0: 6e2d 7365 636f 6e64 6172 7920 7075 6c6c  n-secondary pull
+000004c0: 2d6c 6566 7422 207b 2520 6966 2042 4f4f  -left" {% if BOO
+000004d0: 5453 5452 4150 5f56 4552 5349 4f4e 203d  TSTRAP_VERSION =
+000004e0: 3d20 2234 2e36 2e32 2220 257d 6461 7461  = "4.6.2" %}data
+000004f0: 2d64 6973 6d69 7373 7b25 2065 6c69 6620  -dismiss{% elif 
+00000500: 424f 4f54 5354 5241 505f 5645 5253 494f  BOOTSTRAP_VERSIO
+00000510: 4e20 3d3d 2022 352e 312e 3322 2025 7d64  N == "5.1.3" %}d
+00000520: 6174 612d 6273 2d64 6973 6d69 7373 7b25  ata-bs-dismiss{%
+00000530: 2065 6e64 6966 2025 7d3d 226d 6f64 616c   endif %}="modal
+00000540: 223e 3c69 2063 6c61 7373 3d22 6661 7320  "><i class="fas 
+00000550: 6661 2d74 696d 6573 223e 3c2f 693e 2043  fa-times"></i> C
+00000560: 616e 6365 6c3c 2f62 7574 746f 6e3e 0a3c  ancel</button>.<
+00000570: 6469 7620 636c 6173 733d 227b 2520 6966  div class="{% if
+00000580: 2042 4f4f 5453 5452 4150 5f56 4552 5349   BOOTSTRAP_VERSI
+00000590: 4f4e 203d 3d20 2234 2e36 2e32 2220 257d  ON == "4.6.2" %}
+000005a0: 7465 7874 2d72 6967 6874 7b25 2065 6c69  text-right{% eli
+000005b0: 6620 424f 4f54 5354 5241 505f 5645 5253  f BOOTSTRAP_VERS
+000005c0: 494f 4e20 3d3d 2022 352e 312e 3322 2025  ION == "5.1.3" %
+000005d0: 7d74 6578 742d 656e 647b 2520 656e 6469  }text-end{% endi
+000005e0: 6620 257d 223e 0a20 2020 203c 6275 7474  f %}">.    <butt
+000005f0: 6f6e 2069 643d 2262 746e 2d73 6176 652d  on id="btn-save-
+00000600: 6461 7461 2220 636c 6173 733d 2262 746e  data" class="btn
+00000610: 2062 746e 2d70 7269 6d61 7279 2220 6869   btn-primary" hi
+00000620: 6464 656e 3d22 223e 3c69 2063 6c61 7373  dden=""><i class
+00000630: 3d22 6661 7320 6661 2d73 6176 6522 3e3c  ="fas fa-save"><
+00000640: 2f69 3e20 5361 7665 2077 6974 686f 7574  /i> Save without
+00000650: 2065 6469 7469 6e67 3c2f 6275 7474 6f6e   editing</button
+00000660: 3e0a 2020 2020 3c62 7574 746f 6e20 6964  >.    <button id
+00000670: 3d22 6274 6e2d 6f70 656e 2d64 6174 6122  ="btn-open-data"
+00000680: 2063 6c61 7373 3d22 6274 6e20 6274 6e2d   class="btn btn-
+00000690: 7072 696d 6172 7922 3e3c 6920 636c 6173  primary"><i clas
+000006a0: 733d 2266 6173 2066 612d 636f 6465 223e  s="fas fa-code">
+000006b0: 3c2f 693e 204f 7065 6e20 696e 2054 6578  </i> Open in Tex
+000006c0: 7420 6564 6974 6f72 3c2f 6275 7474 6f6e  t editor</button
+000006d0: 3e0a 2020 2020 3c62 7574 746f 6e20 6964  >.    <button id
+000006e0: 3d22 6274 6e2d 6469 7370 6c61 792d 6461  ="btn-display-da
+000006f0: 7461 2220 636c 6173 733d 2262 746e 2062  ta" class="btn b
+00000700: 746e 2d70 7269 6d61 7279 223e 3c69 2063  tn-primary"><i c
+00000710: 6c61 7373 3d22 6661 7320 6661 2d70 6c61  lass="fas fa-pla
+00000720: 7922 3e3c 2f69 3e20 5374 6172 7420 6564  y"></i> Start ed
+00000730: 6974 696e 673c 2f62 7574 746f 6e3e 0a3c  iting</button>.<
+00000740: 2f64 6976 3e0a 7b25 2065 6e64 626c 6f63  /div>.{% endbloc
+00000750: 6b20 257d                                k %}
```

### Comparing `core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/curate_start.html` & `core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/curate_start.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/enter_data.html` & `core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/data-entry/enter_data.html`

 * *Files 20% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 You won't be able to reach the review page before the document is valid according to the selected template. From the review page, you will be able to curate the {% trans "record_label" %}.
 The 'Save {% trans "form_label"|title %}' button allows you to save partial data that you may want to edit later. This will only save a temporary document and won't actually curate data.
 All grayed elements are optional. Thus, all elements written in black are required. The document may still be valid with empty elements.
 There are no validation on empty fields if no such constraint is defined in the template.
 Thus, an empty string of characters may not raise a validation error, but an empty number will.
 
 <div class="toolbar">
-	<div class="float-right">
-		<button class="btn btn-danger clear-fields mr-auto"><i class="fas fa-eraser"></i> Clear Fields </button>
-        <button class="btn btn-danger cancel-changes mr-auto"><i class="fas fa-sync"></i> Cancel Changes </button>
-        <button class="btn btn-danger cancel-form mr-auto"><i class="fas fa-trash"></i> Delete {% trans "form_label"|title %} </button>
-    	<button class="btn btn-secondary save-form mr-auto"><i class="fas fa-save"></i> Save {% trans "form_label"|title %} </button>
-    	<button class="btn btn-secondary download mr-auto"><i class="fas fa-download"></i> Download </button>
+	<div class="{% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}">
+		<button class="btn btn-danger clear-fields {% if BOOTSTRAP_VERSION == "4.6.2" %}mr-auto{% elif BOOTSTRAP_VERSION == "5.1.3" %}me-auto{% endif %}"><i class="fas fa-eraser"></i> Clear Fields </button>
+        <button class="btn btn-danger cancel-changes {% if BOOTSTRAP_VERSION == "4.6.2" %}mr-auto{% elif BOOTSTRAP_VERSION == "5.1.3" %}me-auto{% endif %}"><i class="fas fa-sync"></i> Cancel Changes </button>
+        <button class="btn btn-danger cancel-form {% if BOOTSTRAP_VERSION == "4.6.2" %}mr-auto{% elif BOOTSTRAP_VERSION == "5.1.3" %}me-auto{% endif %}"><i class="fas fa-trash"></i> Delete {% trans "form_label"|title %} </button>
+    	<button class="btn btn-secondary save-form {% if BOOTSTRAP_VERSION == "4.6.2" %}mr-auto{% elif BOOTSTRAP_VERSION == "5.1.3" %}me-auto{% endif %}"><i class="fas fa-save"></i> Save {% trans "form_label"|title %} </button>
+    	<button class="btn btn-secondary download {% if BOOTSTRAP_VERSION == "4.6.2" %}mr-auto{% elif BOOTSTRAP_VERSION == "5.1.3" %}me-auto{% endif %}"><i class="fas fa-download"></i> Download </button>
         <button class="btn btn-primary validate"><i class="fas fa-check"></i> Validate </button>
 	</div>
     <br/><br/>
 
     <span>Title: {{data.data_structure.name}}</span>
 
     <div id="xsdForm" class="xsdForm">
```

### Comparing `core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/download-options.html` & `core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/download-options.html`

 * *Files 8% similar despite different names*

```diff
@@ -28,9 +28,10 @@
     <div class="mt-3">
         Click here to format content <input type="checkbox" id="format">
     </div>
 </div>
 {% endblock %}
 
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
+<a class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#">
+<i class="fas fa-times"></i> Cancel</a>
 {% endblock %}
```

### Comparing `core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/save-form.html` & `core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/save-form.html`

 * *Files 26% similar despite different names*

```diff
@@ -5,10 +5,12 @@
 {% block modal_title %}Save {% trans "form_label"|title %}{% endblock %}
 
 {% block modal_body %}
 Are you sure you want to save the {% trans "form_label" %}?
 {% endblock %}
 
 {% block modal_footer %}
-<button class="btn btn-secondary pull-left" data-dismiss="modal"><i class="fas fa-times"></i> Cancel</button>
+<button class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal">
+    <i class="fas fa-times"></i> Cancel
+</button>
 <button id="btn-save-form" class="btn btn-primary"><i class="fas fa-save"></i> Save</button>
 {% endblock %}
```

### Comparing `core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/use-validation.html` & `core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/use-validation.html`

 * *Files 20% similar despite different names*

```diff
@@ -11,12 +11,12 @@
 </p>
 <div id="useErrorMessage">
 </div>
 <p>Edit the {% trans "form_label" %} or proceed to review page.</p>
 {% endblock %}
 
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
+<a class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
 <a href="{% url 'core_curate_view_data' data.data_structure.id %}" class="btn btn-primary proceed-review">
     <i class="fas fa-check"></i> Proceed to Review
 </a>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 {% extends 'core_main_app/_render/admin/theme/tools/modal.html' %} {% load i18n
 %} {% block modal_id %}use-warning-modal{% endblock %} {% block modal_title
 %}Validation Warning{% endblock %} {% block modal_body %} {% include
 'core_curate_app/user/data-entry/modals/validation-warning.html' %}
 Some required or recommended fields are present but empty:
 Edit the {% trans "form_label" %} or proceed to review page.
 {% endblock %} {% block modal_footer %}
- Cancel
+% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION ==
+"5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#"> Cancel
 
  Proceed_to_Review
  {% endblock %}
```

### Comparing `core_curate_app-2.3.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/xml-valid.html` & `core_curate_app-2.4.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/xml-valid.html`

 * *Files 12% similar despite different names*

```diff
@@ -6,12 +6,15 @@
 
 {% block modal_body %}
 The {% trans "form_label" %} is valid. You can now proceed to the Review page.
 {% include 'core_curate_app/user/data-entry/modals/validation-warning.html' %}
 {% endblock %}
 
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
+<a class="btn btn-secondary pull-left"
+   {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#">
+    <i class="fas fa-times"></i> Cancel
+</a>
 <a class="btn btn-primary proceed-review" href="{% url 'core_curate_view_data' data.data_structure.id %}">
     <i class="fas fa-check"></i> Proceed to Review
 </a>
 {% endblock %}
```

### Comparing `core_curate_app-2.3.0/core_curate_app/urls.py` & `core_curate_app-2.4.0/core_curate_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.3.0/core_curate_app/utils/parser.py` & `core_curate_app-2.4.0/core_curate_app/utils/parser.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.3.0/core_curate_app/views/common/views.py` & `core_curate_app-2.4.0/core_curate_app/views/common/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from django.urls import reverse
 from django.utils.html import escape as html_escape
 from django.utils.translation import ugettext as _
 
 from core_curate_app.components.curate_data_structure import (
     api as data_structure_api,
 )
+
 from core_curate_app.views.user.views import _get_curate_data_structure_by_id
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.commons.exceptions import (
     DoesNotExist,
     DocumentEditingSizeError,
 )
 from core_main_app.components.data import api as data_api
@@ -50,19 +51,22 @@
         try:
             # get data structure
             curate_data_structure = _get_curate_data_structure_by_id(
                 kwargs["curate_data_structure_id"], request
             )
 
             # TODO: fix with the rework on the curate workflow
-            if curate_data_structure.form_string is None:
+            if (
+                curate_data_structure.form_string is None
+                or curate_data_structure.form_string == ""
+            ):
                 raise Exception(
                     "The "
                     + _("form_label")
-                    + " was not saved. We can't display the correct data."
+                    + " was not saved and cannot be displayed."
                 )
 
             # Set the assets
             assets = {
                 "js": [
                     {
                         "path": "core_main_app/common/js/XMLTree.js",
@@ -85,17 +89,17 @@
             return self.common_render(
                 request, self.template, assets=assets, context=context
             )
         except Exception as exception:
             assets = {
                 "js": [
                     {
-                        "path": "core_main_app/common/js/backtoprevious.js",
-                        "is_raw": True,
-                    }
+                        "path": "core_main_app/user/js/data/detail.js",
+                        "is_raw": False,
+                    },
                 ]
             }
             template = "core_main_app/common/commons/error.html"
             if self.administration:
                 template = (
                     "core_main_app/admin/commons/errors/errors_wrapper.html"
                 )
@@ -121,14 +125,15 @@
         """
 
         try:
 
             data_structure = data_structure_api.get_by_id(
                 request.GET["id"], request.user
             )
+
             if (
                 main_file_utils.get_byte_size_from_string(
                     data_structure.form_string
                 )
                 > MAX_DOCUMENT_EDITING_SIZE
             ):
                 raise DocumentEditingSizeError(
@@ -185,34 +190,36 @@
         """
         try:
             content = self.request.POST["content"].strip()
             data_structure_id = self.request.POST["document_id"]
             data_structure = data_structure_api.get_by_id(
                 data_structure_id, self.request.user
             )
-
-            # create new data
-            data = Data()
-            data.title = data_structure.name
-            template = template_api.get_by_id(
-                str(data_structure.template.id), request=self.request
-            )
-            data.template = template
-            data.user_id = str(self.request.user.id)
+            if data_structure.data is not None:
+                data = data_structure.data
+            else:
+                # create new data
+                data = Data()
+                data.title = data_structure.name
+                template = template_api.get_by_id(
+                    str(data_structure.template.id), request=self.request
+                )
+                data.template = template
+                data.user_id = str(self.request.user.id)
 
             # set content
             data.xml_content = content
             # save data
-            data = data_api.upsert(data, self.request)
+            data_api.upsert(data, self.request)
 
             data_structure_api.delete(data_structure, self.request.user)
             messages.add_message(
                 self.request,
                 messages.SUCCESS,
-                get_data_label() + " saved with success.",
+                get_data_label().capitalize() + " saved with success.",
             )
             return HttpResponse(
                 json.dumps({"url": reverse(self.save_redirect)}),
                 "application/javascript",
             )
         except AccessControlError as ace:
             return HttpResponseForbidden(html_escape(str(ace)))
```

### Comparing `core_curate_app-2.3.0/core_curate_app/views/user/ajax.py` & `core_curate_app-2.4.0/core_curate_app/views/user/ajax.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """AJAX views for the Curate app
 """
 import json
 import logging
 
 from django.contrib import messages
-from django.contrib.messages.storage.base import Message
 from django.http.response import HttpResponseBadRequest, HttpResponse
 from django.template import loader
 from django.urls import reverse
 from django.utils.html import escape
 from lxml.etree import XMLSyntaxError
 
 import core_curate_app.components.curate_data_structure.api as curate_data_structure_api
@@ -310,22 +309,25 @@
         # add success message
         messages.add_message(
             request,
             messages.SUCCESS,
             get_form_label().capitalize() + " deleted with success.",
         )
 
-        return HttpResponse(
-            json.dumps({}), content_type="application/javascript"
-        )
+        return HttpResponse(json.dumps({}), content_type="application/json")
     except Exception as exception:
+        error_message = (
+            "An unexpected error has occurred while cancelling "
+            f"the {get_form_label()}"
+        )
+
+        logger.error("%s: %s", error_message, str(exception))
         return HttpResponseBadRequest(
-            "An unexpected error has occured: %s",
-            str(exception).replace('"', "'"),
-            content_type="application/javascript",
+            json.dumps({"error": error_message}),
+            content_type="application/json",
         )
 
 
 @decorators.permission_required(
     content_type=rights.CURATE_CONTENT_TYPE,
     permission=rights.CURATE_ACCESS,
     raise_exception=True,
@@ -353,26 +355,31 @@
 
         # update curate data structure data
         curate_data_structure.form_string = xml_data
 
         # save data structure
         curate_data_structure_api.upsert(curate_data_structure, request.user)
 
-        # add success message
-        message = Message(
-            messages.SUCCESS,
-            get_form_label().capitalize() + " saved with success.",
-        )
-
         return HttpResponse(
-            json.dumps({"message": message.message, "tags": message.tags}),
+            json.dumps(
+                {
+                    "message": f"{get_form_label().capitalize()} saved with success."
+                }
+            ),
             content_type="application/json",
         )
     except Exception as exception:
-        return HttpResponseBadRequest(escape(str(exception)))
+        error_message = (
+            f"An error occurred while saving the {get_form_label()}"
+        )
+        logger.error("%s: %s", error_message, str(exception))
+        return HttpResponseBadRequest(
+            json.dumps({"error": error_message}),
+            content_type="application/json",
+        )
 
 
 @decorators.permission_required(
     content_type=rights.CURATE_CONTENT_TYPE,
     permission=rights.CURATE_ACCESS,
     raise_exception=True,
 )
```

### Comparing `core_curate_app-2.3.0/core_curate_app/views/user/forms.py` & `core_curate_app-2.4.0/core_curate_app/views/user/forms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ User curate forms
 """
 from django import forms
+from django.conf import settings
 
 from core_main_app.settings import MAX_DOCUMENT_EDITING_SIZE
 from core_main_app.utils.labels import get_form_label
 import core_curate_app.components.curate_data_structure.api as curate_data_structure_api
 from django.core.exceptions import ValidationError
 
 
@@ -36,24 +37,28 @@
 
 class OpenForm(forms.Form):
     """Form to open an existing form."""
 
     forms = FormDataModelChoiceField(
         label="",
         queryset=curate_data_structure_api.get_none(),
-        widget=forms.Select(attrs={"class": "form-control"}),
+        widget=forms.Select(),
     )
 
     def __init__(self, *args, **kwargs):
         if "forms" in kwargs:
             queryset = kwargs.pop("forms")
         else:
             queryset = curate_data_structure_api.get_none()
         super().__init__(*args, **kwargs)
         self.fields["forms"].queryset = queryset
+        if settings.BOOTSTRAP_VERSION == "4.6.2":
+            self.fields["forms"].widget.attrs["class"] = "form-control"
+        elif settings.BOOTSTRAP_VERSION == "5.1.3":
+            self.fields["forms"].widget.attrs["class"] = "form-select"
 
 
 def _file_size_validator(value):
     """Check size of uploaded file
 
     Args:
         value:
```

### Comparing `core_curate_app-2.3.0/core_curate_app/views/user/views.py` & `core_curate_app-2.4.0/core_curate_app/views/user/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,25 +5,22 @@
 from typing import Dict, List
 
 from django.contrib import messages
 from django.http import HttpResponseRedirect
 from django.urls import reverse
 from django.utils.decorators import method_decorator
 from django.views import View
+from django.conf import settings
 
 import core_main_app.components.template.api as template_api
 import core_main_app.components.template_version_manager.api as template_version_manager_api
 from core_curate_app.components.curate_data_structure import (
     api as curate_data_structure_api,
 )
 from core_curate_app.permissions import rights
-from core_curate_app.settings import (
-    INSTALLED_APPS,
-    ENABLE_XML_ENTITIES_TOOLTIPS,
-)
 from core_curate_app.utils.parser import get_parser
 from core_main_app.access_control.api import check_can_write
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.commons.exceptions import (
     LockError,
     ModelError,
     DoesNotExist,
@@ -164,21 +161,35 @@
             "css": [
                 "core_curate_app/user/css/common.css",
                 "core_curate_app/user/css/xsd_form.css",
                 "core_parser_app/css/use.css",
             ],
         }
 
-        if ENABLE_XML_ENTITIES_TOOLTIPS:
+        if settings.ENABLE_XML_ENTITIES_TOOLTIPS:
             self.assets["js"].append(
                 {
                     "path": "core_curate_app/user/js/xml_entities_tooltip.js",
                     "is_raw": False,
                 }
             )
+            if settings.BOOTSTRAP_VERSION == "4.6.2":
+                self.assets["js"].append(
+                    {
+                        "path": "core_curate_app/user/js/xml_entities_tooltip/popover.bs4.js",
+                        "is_raw": False,
+                    }
+                )
+            elif settings.BOOTSTRAP_VERSION == "5.1.3":
+                self.assets["js"].append(
+                    {
+                        "path": "core_curate_app/user/js/xml_entities_tooltip/popover.bs5.js",
+                        "is_raw": False,
+                    }
+                )
 
         self.modals = [
             "core_curate_app/user/data-entry/modals/cancel-changes.html",
             "core_curate_app/user/data-entry/modals/cancel-form.html",
             "core_curate_app/user/data-entry/modals/clear-fields.html",
             "core_main_app/common/modals/download-options.html",
             "core_curate_app/user/data-entry/modals/save-form.html",
@@ -353,14 +364,30 @@
         }
 
         self.modals = [
             "core_curate_app/user/data-review/modals/save-error.html",
             "core_main_app/common/modals/download-options.html",
         ]
 
+        if "core_file_preview_app" in settings.INSTALLED_APPS:
+            self.assets["js"].extend(
+                [
+                    {
+                        "path": "core_file_preview_app/user/js/file_preview.js",
+                        "is_raw": False,
+                    }
+                ]
+            )
+            self.assets["css"].append(
+                "core_file_preview_app/user/css/file_preview.css"
+            )
+            self.modals.append(
+                "core_file_preview_app/user/file_preview_modal.html"
+            )
+
     def build_context(self, request, curate_data_structure):
         """Build XML string from CurateDataStructure
 
         Args:
             request:
             curate_data_structure:
 
@@ -393,30 +420,14 @@
         """
 
         try:
             curate_data_structure = _get_curate_data_structure_by_id(
                 curate_data_structure_id, request
             )
 
-            if "core_file_preview_app" in INSTALLED_APPS:
-                self.assets["js"].extend(
-                    [
-                        {
-                            "path": "core_file_preview_app/user/js/file_preview.js",
-                            "is_raw": False,
-                        }
-                    ]
-                )
-                self.assets["css"].append(
-                    "core_file_preview_app/user/css/file_preview.css"
-                )
-                self.modals.append(
-                    "core_file_preview_app/user/file_preview_modal.html"
-                )
-
             # Build Context
             context = self.build_context(request, curate_data_structure)
             # Set page title
             context.update({"page_title": "View Data"})
 
             return render(
                 request,
```

### Comparing `core_curate_app-2.3.0/core_curate_app.egg-info/PKG-INFO` & `core_curate_app-2.4.0/core_curate_app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-curate-app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Curation functionalities for the curator core project
 Home-page: https://github.com/usnistgov/core_curate_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ===============
         Core Curate App
```

### Comparing `core_curate_app-2.3.0/core_curate_app.egg-info/SOURCES.txt` & `core_curate_app-2.4.0/core_curate_app.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 core_curate_app/static/core_curate_app/user/js/enter_data.raw.js
 core_curate_app/static/core_curate_app/user/js/select_template.js
 core_curate_app/static/core_curate_app/user/js/select_template.raw.js
 core_curate_app/static/core_curate_app/user/js/text_editor.raw.js
 core_curate_app/static/core_curate_app/user/js/view_data.js
 core_curate_app/static/core_curate_app/user/js/view_data.raw.js
 core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip.js
+core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip/popover.bs4.js
+core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip/popover.bs5.js
 core_curate_app/templates/core_curate_app/admin/detail.html
 core_curate_app/templates/core_curate_app/admin/view_curate_data_structure.html
 core_curate_app/templates/core_curate_app/common/detail_curate_data_structure.html
 core_curate_app/templates/core_curate_app/common/tools_curate_data_structure.html
 core_curate_app/templates/core_curate_app/user/curate.html
 core_curate_app/templates/core_curate_app/user/curate_full_start.html
 core_curate_app/templates/core_curate_app/user/curate_start.html
@@ -73,33 +75,48 @@
 core_curate_app/templates/core_curate_app/user/data-entry/modals/xml-valid.html
 core_curate_app/templates/core_curate_app/user/data-review/view_data.html
 core_curate_app/templates/core_curate_app/user/data-review/modals/save-error.html
 core_curate_app/templates/core_curate_app/user/list/list.html
 core_curate_app/utils/__init__.py
 core_curate_app/utils/parser.py
 core_curate_app/views/__init__.py
+core_curate_app/views/admin/__init__.py
+core_curate_app/views/admin/ajax.py
 core_curate_app/views/common/__init__.py
 core_curate_app/views/common/views.py
 core_curate_app/views/user/__init__.py
 core_curate_app/views/user/ajax.py
 core_curate_app/views/user/forms.py
 core_curate_app/views/user/views.py
 docs/__init__.py
 docs/conf.py
 docs/conf_urls.py
 tests/__init__.py
 tests/test_settings.py
 tests/urls.py
 tests/components/__init__.py
 tests/components/curate_data_structure/__init__.py
+tests/components/curate_data_structure/tests_int.py
 tests/components/curate_data_structure/tests_int_access_control.py
 tests/components/curate_data_structure/tests_unit.py
 tests/components/curate_data_structure/fixtures/__init__.py
 tests/components/curate_data_structure/fixtures/fixtures.py
 tests/rest/__init__.py
 tests/rest/curate_data_structure/__init__.py
 tests/rest/curate_data_structure/tests_int.py
 tests/rest/curate_data_structure/tests_permissions.py
 tests/views/__init__.py
-tests/views/test_forms.py
-tests/views/tests_int_access_control.py
-tests/views/tests_views.py
+tests/views/admin/__init__.py
+tests/views/admin/ajax/__init__.py
+tests/views/admin/ajax/test_unit.py
+tests/views/common/__init__.py
+tests/views/common/views/__init__.py
+tests/views/common/views/test_unit.py
+tests/views/common/views/tests_int_access_control.py
+tests/views/user/__init__.py
+tests/views/user/ajax/__init__.py
+tests/views/user/ajax/test_unit.py
+tests/views/user/ajax/tests_int_access_control.py
+tests/views/user/forms/__init__.py
+tests/views/user/forms/test_unit.py
+tests/views/user/views/__init__.py
+tests/views/user/views/test_unit.py
```

### Comparing `core_curate_app-2.3.0/docs/conf.py` & `core_curate_app-2.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.3.0/setup.py` & `core_curate_app-2.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 chdir(normpath(join(abspath(__file__), pardir)))
 
 dep_links = [r for r in required if r.startswith("https://")]
 required = [req_link(r) if r.startswith("https://") else r for r in required]
 
 setup(
     name="core_curate_app",
-    version="2.3.0",
+    version="2.4.0",
     description="Curation functionalities for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_curate_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_curate_app-2.3.0/tests/components/curate_data_structure/fixtures/fixtures.py` & `core_curate_app-2.4.0/tests/components/curate_data_structure/fixtures/fixtures.py`

 * *Files 26% similar despite different names*

```diff
@@ -87,7 +87,115 @@
             "user1_template.xsd", xsd.encode("utf-8")
         )
         self.template.user = "1"
         self.template.content = xsd
         self.template.hash = ""
         self.template.filename = "filename"
         self.template.save()
+
+
+class DataStructureFixtures2(FixtureInterface):
+    """Data structure fixtures"""
+
+    data_structure_1 = None
+    data_structure_2 = None
+    data_structure_3 = None
+    data = None
+    data_without_draft = None
+    data_multiple_drafts = None
+    template = None
+    data_collection = None
+
+    def insert_data(self):
+        """Insert a set of Data.
+
+        Returns:
+
+        """
+        # Make a connexion with a mock database
+        self.generate_template()
+        self.generate_data_collection()
+
+    def generate_data_collection(self):
+        """Generate a Data collection.
+
+        Returns:
+
+        """
+
+        # NOTE: no xml_content to avoid using unsupported GridFS mock
+        self.data = Data(
+            template=self.template,
+            user_id="1",
+            dict_content=None,
+            title="title",
+        )
+        self.data.save()
+
+        self.data_without_draft = Data(
+            template=self.template,
+            user_id="1",
+            dict_content=None,
+            title="title",
+        )
+        self.data_without_draft.save()
+
+        self.data_multiple_drafts = Data(
+            template=self.template,
+            user_id="1",
+            dict_content=None,
+            title="title",
+        )
+        self.data_multiple_drafts.save()
+
+        self.data_structure_1 = CurateDataStructure(
+            user="1",
+            template=self.template,
+            name="data_structure_1",
+            data=self.data,
+        )
+        self.data_structure_1.save()
+
+        self.data_structure_2 = CurateDataStructure(
+            user="1",
+            template=self.template,
+            name="data_structure_2",
+            data=self.data_multiple_drafts,
+        )
+        self.data_structure_2.save()
+
+        self.data_structure_3 = CurateDataStructure(
+            user="2",
+            template=self.template,
+            name="data_structure_3",
+            data=self.data_multiple_drafts,
+        )
+        self.data_structure_3.save()
+
+        self.data_collection = [
+            self.data_structure_1,
+            self.data_structure_2,
+            self.data_structure_3,
+            self.data,
+            self.data_without_draft,
+            self.data_multiple_drafts,
+        ]
+
+    def generate_template(self):
+        """Generate an unique Template.
+
+        Returns:
+
+        """
+        self.template = Template()
+        xsd = (
+            '<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema">'
+            '<xs:element name="tag"></xs:element></xs:schema>'
+        )
+        self.template.file = SimpleUploadedFile(
+            "user1_template.xsd", xsd.encode("utf-8")
+        )
+        self.template.user = "1"
+        self.template.content = xsd
+        self.template.hash = ""
+        self.template.filename = "filename"
+        self.template.save()
```

### Comparing `core_curate_app-2.3.0/tests/components/curate_data_structure/tests_int_access_control.py` & `core_curate_app-2.4.0/tests/components/curate_data_structure/tests_int_access_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -454,69 +454,37 @@
 class TestCurateDataStructureGetByDataId(IntegrationBaseTestCase):
     """
     Test Curate Data Structure Get ById
     """
 
     fixture = fixture_data_structure
 
-    def test_get_by_data_id_as_superuser_returns_data_structure(self):
-        """
-        test_get_by_data_id_as_superuser_returns_data_structure
-
-        Returns:
-
-        """
-
-        mock_user = create_mock_user(
-            self.fixture.data_structure_3.user,
-            is_staff=True,
-            is_superuser=True,
-        )
-        data_structure = curate_data_structure_api.get_by_data_id(
-            self.fixture.data.id, mock_user
-        )
-        self.assertTrue(isinstance(data_structure, CurateDataStructure))
-        self.assertEquals(self.fixture.data.id, data_structure.data.id)
-
     def test_get_by_data_id_as_owner_returns_data_structure(self):
         """
         test_get_by_data_id_as_owner_returns_data_structure
 
         Returns:
 
         """
         mock_user = create_mock_user(self.fixture.data_structure_1.user)
-        data_structure = curate_data_structure_api.get_by_data_id(
+        data_structure = curate_data_structure_api.get_by_data_id_and_user(
             self.fixture.data.id, mock_user
         )
         self.assertTrue(isinstance(data_structure, CurateDataStructure))
         self.assertEquals(self.fixture.data.id, data_structure.data.id)
 
-    def test_get_by_data_id_as_user_non_owner_raises_error(self):
-        """
-        test_get_by_data_id_as_user_non_owner_raises_error
-
-        Returns:
-
-        """
-        mock_user = create_mock_user(self.fixture.data_structure_3.user)
-        with self.assertRaises(AccessControlError):
-            curate_data_structure_api.get_by_data_id(
-                self.fixture.data.id, mock_user
-            )
-
     def test_get_by_data_id_as_anonymous_user_raises_error(self):
         """
         test_get_by_data_id_as_anonymous_user_raises_error
 
         Returns:
 
         """
         with self.assertRaises(AccessControlError):
-            curate_data_structure_api.get_by_data_id(
+            curate_data_structure_api.get_by_data_id_and_user(
                 self.fixture.data.id, AnonymousUser()
             )
 
 
 class TestDataStructureChangeOwner(IntegrationBaseTestCase):
     """
     Test Data Structure Change Owner
@@ -596,14 +564,74 @@
         curate_data_structure_api.change_owner(
             document=fixture_data_structure.data_structure_1,
             new_user=mock_user,
             user=mock_user,
         )
 
 
+class TestGetAllCurateDataStructureByData(IntegrationBaseTestCase):
+    """
+    Test Get All Curate Data Structures By Data
+    """
+
+    fixture = fixture_data_structure
+
+    def test_get_all_curate_data_structures_by_data_as_superuser_returns_data_structures(
+        self,
+    ):
+        """
+        test_get_all_curate_data_structures_by_data_as_superuser_returns_data_structures
+
+        Returns:
+
+        """
+
+        mock_user = create_mock_user(
+            self.fixture.data_structure_3.user,
+            is_staff=True,
+            is_superuser=True,
+        )
+        results = (
+            curate_data_structure_api.get_all_curate_data_structures_by_data(
+                self.fixture.data, mock_user
+            )
+        )
+        for data_structure in results:
+            self.assertTrue(isinstance(data_structure, CurateDataStructure))
+
+    def test_get_all_curate_data_structures_by_data_as_user_raises_error(
+        self,
+    ):
+        """
+        test_get_all_curate_data_structures_by_data_as_user_raises_error
+
+        Returns:
+
+        """
+        mock_user = create_mock_user(self.fixture.data_structure_3.user)
+        with self.assertRaises(AccessControlError):
+            curate_data_structure_api.get_all_curate_data_structures_by_data(
+                self.fixture.data, mock_user
+            )
+
+    def test_get_all_curate_data_structures_by_data_as_anonymous_user_raises_error(
+        self,
+    ):
+        """
+        test_get_all_curate_data_structures_by_data_as_anonymous_user_raises_error
+
+        Returns:
+
+        """
+        with self.assertRaises(AccessControlError):
+            curate_data_structure_api.get_all_curate_data_structures_by_data(
+                self.fixture.data, AnonymousUser()
+            )
+
+
 def _get_data_structure_element(user, data_structure):
     """Return a data structure element
 
     Args:
         user:
         data_structure:
```

### Comparing `core_curate_app-2.3.0/tests/components/curate_data_structure/tests_unit.py` & `core_curate_app-2.4.0/tests/components/curate_data_structure/tests_unit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 """ Unit Test Curate Data Structure
 """
 from unittest.case import TestCase
 
 from unittest.mock import patch
 
+from core_main_app.access_control.exceptions import AccessControlError
+
+from core_main_app.components.data.models import Data
+
 from core_main_app.commons import exceptions
 from core_main_app.components.template.models import Template
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 import core_curate_app.components.curate_data_structure.api as curate_data_structure_api
 from core_curate_app.components.curate_data_structure.models import (
     CurateDataStructure,
 )
+from tests.components.curate_data_structure.fixtures.fixtures import (
+    DataStructureFixtures,
+)
+
+fixture_data_structure = DataStructureFixtures()
 
 
 class TestCurateDataStructureGetById(TestCase):
     """
     Test Curate Data Structure Get By Id
     """
 
@@ -368,14 +377,100 @@
         result = curate_data_structure_api.get_all_by_user(create_mock_user(1))
         # Assert
         self.assertTrue(
             all(isinstance(item, CurateDataStructure) for item in result)
         )
 
 
+class TestCurateDataStructuresGetByData(TestCase):
+    """
+    Test Curate Data Structures Get By Data
+    """
+
+    @patch.object(
+        CurateDataStructure, "get_all_curate_data_structures_by_data"
+    )
+    def test_get_all_curate_data_structures_by_data_returns_empty_list_if_not_found(
+        self, mock_get
+    ):
+        """
+        test_get_all_curate_data_structures_by_data_returns_empty_list_if_not_found
+
+        Returns:
+
+        """
+        # Arrange
+        mock_get.return_value = []
+        mock_user = create_mock_user("1", is_superuser=True)
+
+        # Act
+        result = (
+            curate_data_structure_api.get_all_curate_data_structures_by_data(
+                Data(), mock_user
+            )
+        )
+        # Assert
+        self.assertEqual(result, [])
+
+    @patch.object(
+        CurateDataStructure, "get_all_curate_data_structures_by_data"
+    )
+    def test_get_all_curate_data_structures_by_data_return_list(
+        self, mock_get
+    ):
+        """
+        test_get_all_curate_data_structures_by_data_return_list
+
+        Returns:
+
+        """
+        # Arrange
+        data_structure_1 = CurateDataStructure(
+            user="1", template=Template(), name="name"
+        )
+
+        mock_get.return_value = [data_structure_1]
+        mock_user = create_mock_user("1", is_superuser=True)
+
+        # Act
+        result = (
+            curate_data_structure_api.get_all_curate_data_structures_by_data(
+                Data(), mock_user
+            )
+        )
+        # Assert
+        self.assertEqual(len(result), 1)
+
+    @patch.object(
+        CurateDataStructure, "get_all_curate_data_structures_by_data"
+    )
+    def test_get_all_curate_data_structures_by_data_raises_error(
+        self, mock_get
+    ):
+        """
+        test_get_all_curate_data_structures_by_data_raises_error
+
+        Returns:
+
+        """
+        # Arrange
+        data_structure_1 = CurateDataStructure(
+            user="1", template=Template(), name="name"
+        )
+
+        mock_get.return_value = [data_structure_1]
+        mock_user = create_mock_user("0")
+
+        # Act # Assert
+        with self.assertRaises(AccessControlError):
+            curate_data_structure_api.get_all_curate_data_structures_by_data(
+                Data(), mock_user
+            )
+
+
 def _get_template():
     template = Template()
     template.id_field = 1
     xsd = (
         '<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema">'
         '<xs:element name="tag"></xs:element></xs:schema>'
     )
```

### Comparing `core_curate_app-2.3.0/tests/rest/curate_data_structure/tests_int.py` & `core_curate_app-2.4.0/tests/rest/curate_data_structure/tests_int.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,21 +6,23 @@
     IntegrationBaseTestCase,
 )
 
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 from tests.components.curate_data_structure.fixtures.fixtures import (
     DataStructureFixtures,
+    DataStructureFixtures2,
 )
 from core_curate_app.rest.curate_data_structure import (
     views as data_structure_rest_views,
 )
 
 
 fixture_data_structure = DataStructureFixtures()
+fixture_data_structure2 = DataStructureFixtures2()
 
 
 class TestDataStructureListAdmin(IntegrationBaseTestCase):
     """
     Test Data Structure List Admin
     """
```

### Comparing `core_curate_app-2.3.0/tests/rest/curate_data_structure/tests_permissions.py` & `core_curate_app-2.4.0/tests/rest/curate_data_structure/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.3.0/tests/test_settings.py` & `core_curate_app-2.4.0/tests/test_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,14 @@
     # Django apps
     "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.sites",
-    # Extra apps
-    "tz_detect",
     # Local apps
     "tests",
     "core_main_app",
     "core_parser_app",
     "core_curate_app",
 ]
 
@@ -32,15 +30,14 @@
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
@@ -61,7 +58,10 @@
 
 DEFAULT_AUTO_FIELD = "django.db.models.BigAutoField"
 CELERYBEAT_SCHEDULER = "django_celery_beat.schedulers:DatabaseScheduler"
 
 MONGODB_INDEXING = False
 MONGODB_ASYNC_SAVE = False
 USE_TZ = True
+
+ENABLE_XML_ENTITIES_TOOLTIPS = True
+BOOTSTRAP_VERSION = "4.6.2"
```

### Comparing `core_curate_app-2.3.0/tests/urls.py` & `core_curate_app-2.4.0/tests/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,12 +93,11 @@
         permission_required(
             content_type=rights.CURATE_CONTENT_TYPE,
             permission=rights.CURATE_ACCESS,
         )(common_views.FormView.as_view()),
         name="core_curate_view_form",
     ),
     re_path(r"^rest/", include("core_curate_app.rest.urls")),
-    re_path(r"^tz_detect/", include("tz_detect.urls")),
     re_path(
         r"^login", main_user_views.custom_login, name="core_main_app_login"
     ),
 ]
```

### Comparing `core_curate_app-2.3.0/tests/views/tests_views.py` & `core_curate_app-2.4.0/tests/views/common/views/test_unit.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,93 +1,83 @@
-""" Test views
+""" Unit tests for views from `views.common.views`.
 """
 from unittest.case import TestCase
 from unittest.mock import patch, MagicMock
 
-from django.http import HttpResponseRedirect
 from django.test import RequestFactory
-from django.urls import reverse
 
-from core_curate_app.views.common.views import DraftContentEditor
-from core_curate_app.views.user.views import EnterDataView
+from core_curate_app.views.common.views import DraftContentEditor, FormView
 from core_main_app.settings import MAX_DOCUMENT_EDITING_SIZE
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
-from core_parser_app.tools.parser.exceptions import ParserError
+from core_main_app.utils.labels import get_form_label
 
 
-class TestEnterDataView(TestCase):
-    """Test EnterDataView"""
+class TestDraftContentEditor(TestCase):
+    """Test Draft Content Editor View"""
 
     def setUp(self):
         """setUp
         Returns:
         """
         self.factory = RequestFactory()
         self.user1 = create_mock_user(user_id="1")
-        self.user1.has_perm = MagicMock()
-        self.user1.has_perm.return_value = True
 
-    @patch("core_curate_app.views.user.views.EnterDataView.build_context")
-    @patch("core_curate_app.views.user.views._get_curate_data_structure_by_id")
-    def test_enter_data_view_get_returns_error_if_parser_error_occurs(
-        self, mock_ds_get_by_id, mock_build_context
+    @patch("core_curate_app.components.curate_data_structure.api.get_by_id")
+    @patch("core_main_app.utils.file.get_byte_size_from_string")
+    def test_xml_content_too_big_returns_error(
+        self, mock_get_byte_size, mock_ds_get_by_id
     ):
-        """test_enter_data_view_get_returns_error_if_parser_error_occurs
+        """test_user_save_xml_content_returns_error
 
 
         Returns:
 
 
         """
-        # Arrange
-        mock_build_context.side_effect = ParserError("error")
         mock_ds = MagicMock()
         mock_ds.form_string = "test"
-        mock_ds.data = None
         mock_ds_get_by_id.return_value = mock_ds
-        request = self.factory.get("core_curate_enter_data")
-        request._messages = MagicMock()
+        mock_get_byte_size.return_value = MAX_DOCUMENT_EDITING_SIZE + 1
+        request = self.factory.get("core_main_app_xml_text_editor_view")
+        request.GET = {"id": 1}
         request.user = self.user1
-        # Act
-        response = EnterDataView.as_view()(request, curate_data_structure_id=1)
-        # Assert
-        self.assertTrue(isinstance(response, HttpResponseRedirect))
+        response = DraftContentEditor.as_view()(request)
         self.assertTrue(
-            response.url.startswith(
-                reverse("core_curate_app_xml_text_editor_view")
-            )
+            "MAX_DOCUMENT_EDITING_SIZE" in response.content.decode()
         )
 
 
-class TestDraftContentEditor(TestCase):
-    """Test Draft Content Editor View"""
+class TestFormView(TestCase):
+    """Test Form View"""
 
     def setUp(self):
         """setUp
         Returns:
         """
         self.factory = RequestFactory()
-        self.user1 = create_mock_user(user_id="1")
+        self.user1 = create_mock_user(user_id="1", is_superuser=True)
 
     @patch("core_curate_app.components.curate_data_structure.api.get_by_id")
-    @patch("core_main_app.utils.file.get_byte_size_from_string")
-    def test_xml_content_too_big_returns_error(
-        self, mock_get_byte_size, mock_ds_get_by_id
+    def test_form_view_returns_error_when_xml_string_is_empty(
+        self, mock_ds_get_by_id
     ):
-        """test_user_save_xml_content_returns_error
+        """test_form_view_returns_error_when_xml_string_is_empty
 
 
         Returns:
 
 
         """
         mock_ds = MagicMock()
-        mock_ds.form_string = "test"
+        mock_ds.form_string = ""
         mock_ds_get_by_id.return_value = mock_ds
-        mock_get_byte_size.return_value = MAX_DOCUMENT_EDITING_SIZE + 1
-        request = self.factory.get("core_main_app_xml_text_editor_view")
-        request.GET = {"id": 1}
+
+        request = self.factory.get("core_curate_view_form")
+
         request.user = self.user1
-        response = DraftContentEditor.as_view()(request)
-        self.assertTrue(
-            "MAX_DOCUMENT_EDITING_SIZE" in response.content.decode()
+        response = FormView.as_view()(request, curate_data_structure_id=1)
+        msg_error = (
+            "The "
+            + get_form_label()
+            + " was not saved and cannot be displayed."
         )
+        self.assertTrue(msg_error in response.content.decode())
```

