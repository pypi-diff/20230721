# Comparing `tmp/core_oaipmh_harvester_app-2.3.0.tar.gz` & `tmp/core_oaipmh_harvester_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_oaipmh_harvester_app-2.3.0.tar", last modified: Tue May  2 19:47:19 2023, max compression
+gzip compressed data, was "core_oaipmh_harvester_app-2.4.0.tar", last modified: Fri Jul 21 02:16:18 2023, max compression
```

## Comparing `core_oaipmh_harvester_app-2.3.0.tar` & `core_oaipmh_harvester_app-2.4.0.tar`

### file list

```diff
@@ -1,232 +1,235 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:19.148323 core_oaipmh_harvester_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1133 2023-05-02 19:47:19.143265 core_oaipmh_harvester_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      622 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:13.206462 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4375 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      785 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:13.326450 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      324 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/commons/rights.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:13.341633 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:13.409774 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/mongo/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1106 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/mongo/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7493 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/mongo/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:13.456763 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6394 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5715 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:13.516274 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2120 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2554 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:13.569444 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_harvester_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_harvester_set/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3537 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_harvester_set/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3667 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_harvester_set/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:13.627823 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_identify/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_identify/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1060 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_identify/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2243 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_identify/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:13.698395 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_record/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_record/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3076 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_record/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4803 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_record/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:13.744038 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_registry/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_registry/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    22180 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_registry/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3224 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_registry/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:13.775185 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_verbs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_verbs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8565 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_verbs/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      480 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:13.820598 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11396 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1636 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/migrations/0002_psql_full_text.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:13.878911 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:13.914415 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/rest/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/rest/mongo/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1209 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/rest/mongo/serializers.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:13.967810 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/rest/oai_record/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/rest/oai_record/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6095 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/rest/oai_record/abstract_views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2145 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/rest/oai_record/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:14.002382 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/rest/oai_registry/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/rest/oai_registry/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17640 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/rest/oai_registry/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2384 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/rest/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1685 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      943 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:12.598672 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:12.652271 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:12.629388 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:12.609051 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:12.619966 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:12.615519 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:14.050769 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      805 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/list/modals/edit_harvest_registry.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      487 2023-05-02 19:47:07.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/list/modals/view_registry.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:14.070087 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/request_builder/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      345 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/request_builder/main.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:12.632481 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:12.643356 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:12.639063 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:17.613863 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      477 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/activate_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/activate_registry.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1632 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/add_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      175 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/add_registry.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1287 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/check_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       92 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/check_registry.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      970 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/deactivate_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      102 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/deactivate_registry.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      926 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/delete_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       94 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/delete_registry.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1605 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/harvest_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      204 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/harvest_registry.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      618 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/refresh.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1713 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/update_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      200 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/update_registry.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      868 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/view_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       90 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/view_registry.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:17.679882 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3062 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/init.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      204 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/init.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3993 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/submit.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/submit.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:12.655467 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:12.658676 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:12.666481 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:17.706496 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/css/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    12339 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/css/bootstrap-datetimepicker.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:17.726366 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/js/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    67527 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/js/bootstrap-datetimepicker.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:17.763105 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      901 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/system/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9073 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:12.684535 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:12.687964 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:12.722591 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:17.802976 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:17.834170 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.013786 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1100 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/add_registry.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      741 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/deactivate_registry.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      675 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/delete_registry.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1017 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/edit_harvest_registry.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1957 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/edit_harvest_registry_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      672 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      484 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      991 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_general.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3410 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_identity.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2023 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_metadata_formats.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1947 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_sets.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4463 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      332 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.032015 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/request_builder/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4343 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/request_builder/main.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      343 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/request_builder.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      204 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.109905 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.127706 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/utils/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/utils/query/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.165954 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/utils/query/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/utils/query/mongo/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2002 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/utils/query/mongo/query_builder.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4012 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/utils/sickle_operations.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1392 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/utils/sickle_serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2303 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/utils/transform_operations.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.181990 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.246840 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16030 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5843 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4419 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:13.285585 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1133 2023-05-02 19:47:11.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9888 2023-05-02 19:47:12.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:47:11.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      145 2023-05-02 19:47:11.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2023-05-02 19:47:11.000000 core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.317695 core_oaipmh_harvester_app-2.3.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11074 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      313 2023-05-02 19:47:08.000000 core_oaipmh_harvester_app-2.3.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       76 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:47:19.150195 core_oaipmh_harvester_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1485 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.362240 core_oaipmh_harvester_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.378092 core_oaipmh_harvester_app-2.3.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.395882 core_oaipmh_harvester_app-2.3.0/tests/components/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/components/mongo/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.430133 core_oaipmh_harvester_app-2.3.0/tests/components/mongo/models/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/components/mongo/models/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2636 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/components/mongo/models/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.480861 core_oaipmh_harvester_app-2.3.0/tests/components/oai_harvester_metadata_format/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/components/oai_harvester_metadata_format/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18812 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/components/oai_harvester_metadata_format/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.519641 core_oaipmh_harvester_app-2.3.0/tests/components/oai_harvester_metadata_format_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/components/oai_harvester_metadata_format_set/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8124 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/components/oai_harvester_metadata_format_set/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.555012 core_oaipmh_harvester_app-2.3.0/tests/components/oai_harvester_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/components/oai_harvester_set/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11182 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/components/oai_harvester_set/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.592474 core_oaipmh_harvester_app-2.3.0/tests/components/oai_identify/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/components/oai_identify/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5739 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/components/oai_identify/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.667560 core_oaipmh_harvester_app-2.3.0/tests/components/oai_record/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/components/oai_record/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6786 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/components/oai_record/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.717597 core_oaipmh_harvester_app-2.3.0/tests/components/oai_registry/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/components/oai_registry/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.755198 core_oaipmh_harvester_app-2.3.0/tests/components/oai_registry/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/components/oai_registry/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8366 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/components/oai_registry/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    33272 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/components/oai_registry/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    36268 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/components/oai_registry/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.786520 core_oaipmh_harvester_app-2.3.0/tests/components/oai_verbs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/components/oai_verbs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7759 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/components/oai_verbs/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      268 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/mocks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.801346 core_oaipmh_harvester_app-2.3.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.877063 core_oaipmh_harvester_app-2.3.0/tests/rest/oai_record/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/rest/oai_record/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2948 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/rest/oai_record/tests_int_mongo.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2203 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/rest/oai_record/tests_int_psql.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9221 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/rest/oai_record/tests_permissions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.942913 core_oaipmh_harvester_app-2.3.0/tests/rest/oai_registry/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/rest/oai_registry/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6446 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/rest/oai_registry/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21070 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/rest/oai_registry/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14434 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/rest/oai_registry/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:18.956036 core_oaipmh_harvester_app-2.3.0/tests/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/system/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:19.009690 core_oaipmh_harvester_app-2.3.0/tests/system/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/system/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1858 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/system/api/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1677 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:19.057956 core_oaipmh_harvester_app-2.3.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:09.000000 core_oaipmh_harvester_app-2.3.0/tests/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2697 2023-05-02 19:47:10.000000 core_oaipmh_harvester_app-2.3.0/tests/utils/tests_unit_query_builder.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3838 2023-05-02 19:47:10.000000 core_oaipmh_harvester_app-2.3.0/tests/utils/tests_unit_transform_operations.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:19.073342 core_oaipmh_harvester_app-2.3.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:10.000000 core_oaipmh_harvester_app-2.3.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:19.093345 core_oaipmh_harvester_app-2.3.0/tests/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:10.000000 core_oaipmh_harvester_app-2.3.0/tests/views/admin/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:19.128246 core_oaipmh_harvester_app-2.3.0/tests/views/admin/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:10.000000 core_oaipmh_harvester_app-2.3.0/tests/views/admin/ajax/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1358 2023-05-02 19:47:10.000000 core_oaipmh_harvester_app-2.3.0/tests/views/admin/ajax/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:18.560562 core_oaipmh_harvester_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1133 2023-07-21 02:16:18.556595 core_oaipmh_harvester_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      622 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:16.283374 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4375 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      785 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:16.390672 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      324 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/commons/rights.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:16.406366 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:16.445899 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/mongo/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1106 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/mongo/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7493 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/mongo/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:16.484684 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6394 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5715 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:16.533733 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2120 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2554 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:16.577411 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_harvester_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_harvester_set/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3537 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_harvester_set/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3667 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_harvester_set/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:16.625820 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_identify/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_identify/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1060 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_identify/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2243 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_identify/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:16.672341 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_record/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_record/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3076 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_record/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4803 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_record/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:16.720618 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_registry/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_registry/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    22180 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_registry/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3224 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_registry/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:16.749467 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_verbs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_verbs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8565 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_verbs/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      480 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:16.800179 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11396 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1636 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/migrations/0002_psql_full_text.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:16.859603 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:16.886538 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/rest/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/rest/mongo/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1209 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/rest/mongo/serializers.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:16.928734 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/rest/oai_record/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/rest/oai_record/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6095 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/rest/oai_record/abstract_views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2145 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/rest/oai_record/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:16.958353 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/rest/oai_registry/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/rest/oai_registry/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17640 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/rest/oai_registry/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2384 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/rest/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1685 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      943 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:15.716938 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:15.795793 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:15.748083 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:15.724274 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:15.740417 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:15.729820 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:17.002123 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      805 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/list/modals/edit_harvest_registry.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      487 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/list/modals/view_registry.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:17.019017 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/request_builder/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      345 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/request_builder/main.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:15.751002 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:15.787814 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:15.783612 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:17.258951 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      477 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/activate_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/activate_registry.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1632 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/add_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      175 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/add_registry.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1287 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/check_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       92 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/check_registry.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      970 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/deactivate_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      102 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/deactivate_registry.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      926 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/delete_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       94 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/delete_registry.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1605 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/harvest_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      204 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/harvest_registry.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      618 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/refresh.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1713 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/update_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      200 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/update_registry.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      868 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/view_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       90 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/view_registry.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:17.320172 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3062 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/init.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      204 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/init.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3993 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/submit.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:16:08.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/submit.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:15.798890 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:15.802228 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:15.809886 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:17.342855 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/css/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    12339 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/css/bootstrap-datetimepicker.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:17.357560 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/js/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    67527 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/js/bootstrap-datetimepicker.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:17.397970 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      901 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/system/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9073 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:15.863619 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:15.867000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:15.870329 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:17.444693 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:17.460505 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:17.600560 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1208 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/add_registry.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      849 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/deactivate_registry.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      779 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/delete_registry.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1125 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/edit_harvest_registry.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1957 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/edit_harvest_registry_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      891 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      484 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1015 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_general.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3410 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_identity.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2023 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_metadata_formats.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1947 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_sets.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4583 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      332 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:17.615853 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/request_builder/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4343 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/request_builder/main.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      343 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/request_builder.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      204 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:17.680227 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:17.698576 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/utils/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/utils/query/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:17.735010 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/utils/query/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/utils/query/mongo/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2002 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/utils/query/mongo/query_builder.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4012 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/utils/sickle_operations.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1392 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/utils/sickle_serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2303 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/utils/transform_operations.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:17.748844 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:17.804386 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16030 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6525 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4419 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:16.355596 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1133 2023-07-21 02:16:15.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9961 2023-07-21 02:16:15.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:16:15.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      145 2023-07-21 02:16:15.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2023-07-21 02:16:15.000000 core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:17.858262 core_oaipmh_harvester_app-2.4.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11074 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      313 2023-07-21 02:16:09.000000 core_oaipmh_harvester_app-2.4.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:16:12.000000 core_oaipmh_harvester_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2023-07-21 02:16:12.000000 core_oaipmh_harvester_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       76 2023-07-21 02:16:12.000000 core_oaipmh_harvester_app-2.4.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:16:18.562148 core_oaipmh_harvester_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1485 2023-07-21 02:16:12.000000 core_oaipmh_harvester_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:17.901466 core_oaipmh_harvester_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:12.000000 core_oaipmh_harvester_app-2.4.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:17.915781 core_oaipmh_harvester_app-2.4.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:12.000000 core_oaipmh_harvester_app-2.4.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:17.931922 core_oaipmh_harvester_app-2.4.0/tests/components/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:12.000000 core_oaipmh_harvester_app-2.4.0/tests/components/mongo/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:17.965460 core_oaipmh_harvester_app-2.4.0/tests/components/mongo/models/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:12.000000 core_oaipmh_harvester_app-2.4.0/tests/components/mongo/models/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2636 2023-07-21 02:16:12.000000 core_oaipmh_harvester_app-2.4.0/tests/components/mongo/models/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:18.028069 core_oaipmh_harvester_app-2.4.0/tests/components/oai_harvester_metadata_format/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:12.000000 core_oaipmh_harvester_app-2.4.0/tests/components/oai_harvester_metadata_format/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18812 2023-07-21 02:16:12.000000 core_oaipmh_harvester_app-2.4.0/tests/components/oai_harvester_metadata_format/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:18.056818 core_oaipmh_harvester_app-2.4.0/tests/components/oai_harvester_metadata_format_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/components/oai_harvester_metadata_format_set/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8124 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/components/oai_harvester_metadata_format_set/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:18.082304 core_oaipmh_harvester_app-2.4.0/tests/components/oai_harvester_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/components/oai_harvester_set/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11182 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/components/oai_harvester_set/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:18.126993 core_oaipmh_harvester_app-2.4.0/tests/components/oai_identify/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/components/oai_identify/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5739 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/components/oai_identify/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:18.153050 core_oaipmh_harvester_app-2.4.0/tests/components/oai_record/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/components/oai_record/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6786 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/components/oai_record/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:18.192844 core_oaipmh_harvester_app-2.4.0/tests/components/oai_registry/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/components/oai_registry/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:18.221645 core_oaipmh_harvester_app-2.4.0/tests/components/oai_registry/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/components/oai_registry/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8366 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/components/oai_registry/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    33272 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/components/oai_registry/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    36268 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/components/oai_registry/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:18.250012 core_oaipmh_harvester_app-2.4.0/tests/components/oai_verbs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/components/oai_verbs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7759 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/components/oai_verbs/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      268 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/mocks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:18.262606 core_oaipmh_harvester_app-2.4.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:18.316603 core_oaipmh_harvester_app-2.4.0/tests/rest/oai_record/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/rest/oai_record/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2948 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/rest/oai_record/tests_int_mongo.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2203 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/rest/oai_record/tests_int_psql.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9221 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/rest/oai_record/tests_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:18.364770 core_oaipmh_harvester_app-2.4.0/tests/rest/oai_registry/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/rest/oai_registry/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6446 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/rest/oai_registry/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21070 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/rest/oai_registry/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14434 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/rest/oai_registry/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:18.377558 core_oaipmh_harvester_app-2.4.0/tests/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/system/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:18.407586 core_oaipmh_harvester_app-2.4.0/tests/system/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/system/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1858 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/system/api/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1705 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:18.450673 core_oaipmh_harvester_app-2.4.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2697 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/utils/tests_unit_query_builder.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3838 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/utils/tests_unit_transform_operations.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:18.465837 core_oaipmh_harvester_app-2.4.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:18.482447 core_oaipmh_harvester_app-2.4.0/tests/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/views/admin/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:18.518699 core_oaipmh_harvester_app-2.4.0/tests/views/admin/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/views/admin/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1358 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/views/admin/ajax/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:18.544567 core_oaipmh_harvester_app-2.4.0/tests/views/admin/forms/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/views/admin/forms/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1639 2023-07-21 02:16:13.000000 core_oaipmh_harvester_app-2.4.0/tests/views/admin/forms/test_unit.py
```

### Comparing `core_oaipmh_harvester_app-2.3.0/LICENSE.md` & `core_oaipmh_harvester_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/PKG-INFO` & `core_oaipmh_harvester_app-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_oaipmh_harvester_app
-Version: 2.3.0
+Version: 2.4.0
 Summary: OAI-PMH harvesting capabilities for the curator core project
 Home-page: https://github.com/usnistgov/core_oaipmh_harvester_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =========================
         Core Oaipmh Harvester App
```

### Comparing `core_oaipmh_harvester_app-2.3.0/README.rst` & `core_oaipmh_harvester_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/admin.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/apps.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/mongo/api.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/mongo/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/mongo/models.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/mongo/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/api.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/models.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/api.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/models.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_harvester_set/api.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_harvester_set/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_harvester_set/models.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_harvester_set/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_identify/api.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_identify/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_identify/models.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_identify/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_record/api.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_record/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_record/models.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_record/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_registry/api.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_registry/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_registry/models.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_registry/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/components/oai_verbs/api.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/components/oai_verbs/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/migrations/0001_initial.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/migrations/0002_psql_full_text.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/migrations/0002_psql_full_text.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/rest/mongo/serializers.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/rest/mongo/serializers.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/rest/oai_record/abstract_views.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/rest/oai_record/abstract_views.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/rest/oai_record/views.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/rest/oai_record/views.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/rest/oai_registry/views.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/rest/oai_registry/views.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/rest/serializers.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/rest/serializers.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/rest/urls.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/settings.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/list/modals/edit_harvest_registry.css` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/list/modals/edit_harvest_registry.css`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/add_registry.js` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/add_registry.js`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/check_registry.js` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/check_registry.js`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/deactivate_registry.js` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/deactivate_registry.js`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/delete_registry.js` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/delete_registry.js`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/harvest_registry.js` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/harvest_registry.js`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/refresh.js` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/refresh.js`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/update_registry.js` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/update_registry.js`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/view_registry.js` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/view_registry.js`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/init.js` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/init.js`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/submit.js` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/submit.js`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/css/bootstrap-datetimepicker.css` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/css/bootstrap-datetimepicker.css`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/js/bootstrap-datetimepicker.js` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/js/bootstrap-datetimepicker.js`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/system/api.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/system/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/tasks.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/tasks.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/add_registry.html` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/add_registry.html`

 * *Files 10% similar despite different names*

```diff
@@ -19,10 +19,12 @@
     <div id="add-registry-errors" style="color:red;">
         {{ errors | safe}}
     </div>
 </form>
 {% endblock %}
 
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
+<a class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#">
+    <i class="fas fa-times"></i> Cancel
+</a>
 <a id="add-registry-save" class="btn btn-primary" onclick="saveRegistry();" href="#"><i class="fas fa-save"></i> Add data provider</a>
 {% endblock %}
```

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/deactivate_registry.html` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/delete_registry.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 {% extends 'core_main_app/_render/admin/theme/tools/modal.html' %}
 
-{% block modal_id %}deactivate-registry-modal{% endblock %}
-{% block modal_title %}Deactivate data provider <i class="deactivate-registry-name"></i>{% endblock %}
+{% block modal_id %}delete-registry-modal{% endblock %}
+{% block modal_title %}Delete data provider <i class="delete-registry-name"></i>{% endblock %}
 
 {% block modal_body %}
-<input id="deactivate-registry-id" type="hidden" value=""/>
+<input id="delete-registry-id" type="hidden" value=""/>
 <p>
-    The data provider won't be erased from the database but nobody will be able to see it.
+    The data provider will be erased definitely.
 </p>
-<p>Are you sure you want to deactivate this data provider?</p>
+<p>Are you sure you want to delete this data provider?</p>
 {% endblock %}
 
 {% block modal_footer %}
-<button class="btn btn-secondary pull-left" data-dismiss="modal"><i class="fas fa-times"></i> No</button>
-<button id="deactivate-registry-yes" class="btn btn-danger"><i class="fas fa-check"></i> Yes</button>
+<button class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal">
+<i class="fas fa-times"></i> No
+</button>
+<button id="delete-registry-yes" class="btn btn-danger"><i class="fas fa-check"></i> Yes</button>
 {% endblock %}
```

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/delete_registry.html` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/deactivate_registry.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 {% extends 'core_main_app/_render/admin/theme/tools/modal.html' %}
 
-{% block modal_id %}delete-registry-modal{% endblock %}
-{% block modal_title %}Delete data provider <i class="delete-registry-name"></i>{% endblock %}
+{% block modal_id %}deactivate-registry-modal{% endblock %}
+{% block modal_title %}Deactivate data provider <i class="deactivate-registry-name"></i>{% endblock %}
 
 {% block modal_body %}
-<input id="delete-registry-id" type="hidden" value=""/>
+<input id="deactivate-registry-id" type="hidden" value=""/>
 <p>
-    The data provider will be erased definitely.
+    The data provider won't be erased from the database but nobody will be able to see it.
 </p>
-<p>Are you sure you want to delete this data provider?</p>
+<p>Are you sure you want to deactivate this data provider?</p>
 {% endblock %}
 
 {% block modal_footer %}
-<button class="btn btn-secondary pull-left" data-dismiss="modal"><i class="fas fa-times"></i> No</button>
-<button id="delete-registry-yes" class="btn btn-danger"><i class="fas fa-check"></i> Yes</button>
+<button class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal">
+    <i class="fas fa-times"></i> No
+</button>
+<button id="deactivate-registry-yes" class="btn btn-danger"><i class="fas fa-check"></i> Yes</button>
 {% endblock %}
```

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/edit_harvest_registry.html` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/edit_harvest_registry.html`

 * *Files 10% similar despite different names*

```diff
@@ -13,10 +13,12 @@
     <h4><i class='fas fa-circle-notch fa-spin fa-1x'></i>&nbsp;&nbsp;Please wait ...</h4>
 </div>
 <div id="edit-harvest-registry-modal-form">
 </div>
 {% endblock %}
 
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
+<a class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#">
+    <i class="fas fa-times"></i> Cancel
+</a>
 <a id="edit-harvest-registry-save" class="btn btn-success" onclick="editHarvestRegistry();" href="#"><i class="fas fa-save"></i> Edit data provider</a>
 {% endblock %}
```

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/edit_harvest_registry_form.html` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/edit_harvest_registry_form.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_general.html` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_general.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+{% load tz %}
 <table autofocus class="data">
     <tr class="grey">
         <td colspan="2">
             <strong>General</strong>
         </td>
     </tr>
     <tr>
@@ -33,11 +34,11 @@
         <td>
             <span class='value'>{{ nb_records }}</span>
         </td>
     </tr>
     <tr >
         <td>Last update</td>
         <td>
-            <span class='value'>{{ registry.last_update }}</span>
+            <span class='value'>{{ registry.last_update|localtime }}</span>
         </td>
     </tr>
 </table>
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
+{% load tz %}
 General
 Base URL                    {{ registry.url }}
 Name                        {{ registry.name }}
 Number of metadata formats  {{ metadata_formats|length }}
 Number of sets              {{ sets|length }}
 Number of harvested records {{ nb_records }}
-Last update                 {{ registry.last_update }}
+Last update                 {{ registry.last_update|localtime }}
```

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_identity.html` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_identity.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_metadata_formats.html` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_metadata_formats.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_sets.html` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_sets.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/table.html` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/table.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %}
+{% load tz %}
 
 {% block box_title %}OAI PMH providers list{% endblock %}
 
 {% block box_tools %}
-<div class="btn-group float-right">
+<div class="btn-group {% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}">
 <a href="#" class="btn btn-secondary add-registry-btn">
     <i class="fas fa-plus-circle"></i> Add
 </a>
 <a href="#" class="btn btn-secondary check-all-registries-btn">
     <i class="fas fa-check-circle"></i> Check All
 </a>
 <a href="#" class="btn btn-secondary update-all-registries-btn">
@@ -55,15 +56,15 @@
                 <p style='color:red'>Deactivated</p>
             {% else %}
                 <a class="btn btn-secondary check-registry-btn">Check</a>
             {% endif %}
             </td>
             <td>{{ registry.harvest }}</td>
             <td>{{ registry.harvest_rate }}</td>
-            <td id="lastUpdate{{registry.id}}">{{ registry.last_update }}</td>
+            <td id="lastUpdate{{registry.id}}">{{ registry.last_update|localtime }}</td>
             <td>
                 <a class="btn btn-secondary view-registry-btn" href="#">
                     <i class="fas fa-eye"></i> View
                 </a>
                 {% if registry.is_activated %}
                     {% url 'core-admin:core_oaipmh_harvester_app_edit_registry' registry.id as edit_url %}
                     {% include 'core_main_app/common/buttons/edit.html' %}
```

#### html2text {}

```diff
@@ -1,34 +1,36 @@
-{% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% block
-box_title %}OAI PMH providers list{% endblock %} {% block box_tools %}
+{% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% load tz %}
+{% block box_title %}OAI PMH providers list{% endblock %} {% block box_tools %}
+.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif
+%}">
  Add
 
  Check_All
 
  Update_All
 
  Harvest_All
 {% endblock %} {% block box_body %}
-Name          URL          Status                Harvest          Harvest Rate          Last Update          Actions
+Name          URL          Status                Harvest          Harvest Rate          Last Update                    Actions
   Data harvesting ...
   Updating Data Provider information ...
-                                                                                                              View
-                                                                                                              {% if registry.is_activated %} {% url 'core-
-                                                                                                             admin:core_oaipmh_harvester_app_edit_registry'
-                                                                                                             registry.id as edit_url %} {% include
-                                                                                                             'core_main_app/common/buttons/edit.html' %} {%
-                                                                                                             url 'core-admin:
-                           {% if not                                                                         core_oaipmh_harvester_app_edit_harvest_registry'
-{             {            registry.is_activated {                {                     {                    registry.id as edit_harvest_url %} {% include
-{             {            %}                    {                {                     {                    'core_main_app/common/buttons/edit.html' with
-registry.name registry.url Deactivated           registry.harvest registry.harvest_rate registry.last_update edit_url=edit_harvest_url label='Edit Harvest'
-}}            }}           {% else %} Check {%   }}               }}                    }}                   %}
-                           endif %}                                                                           Deactivate
+                                                                                                                        View
+                                                                                                                        {% if registry.is_activated %} {% url 'core-
+                                                                                                                       admin:core_oaipmh_harvester_app_edit_registry'
+                                                                                                                       registry.id as edit_url %} {% include
+                                                                                                                       'core_main_app/common/buttons/edit.html' %} {%
+                                                                                                                       url 'core-admin:
+                           {% if not                                                                                   core_oaipmh_harvester_app_edit_harvest_registry'
+{             {            registry.is_activated {                {                     {                              registry.id as edit_harvest_url %} {% include
+{             {            %}                    {                {                     {                              'core_main_app/common/buttons/edit.html' with
+registry.name registry.url Deactivated           registry.harvest registry.harvest_rate registry.last_update|localtime edit_url=edit_harvest_url label='Edit Harvest'
+}}            }}           {% else %} Check {%   }}               }}                    }}                             %}
+                           endif %}                                                                                     Deactivate
 
-                                                                                                              Update
+                                                                                                                        Update
 
-                                                                                                              Harvest
-                                                                                                              {% else %}
-                                                                                                              Restore
-                                                                                                                Delete definitely  {% endif %}
+                                                                                                                        Harvest
+                                                                                                                        {% else %}
+                                                                                                                        Restore
+                                                                                                                          Delete definitely  {% endif %}
 There are currently no Data Providers registered. Please add_a_new_one.
 {% endblock %}
```

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/request_builder/main.html` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/request_builder/main.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/utils/query/mongo/query_builder.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/utils/query/mongo/query_builder.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/utils/sickle_operations.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/utils/sickle_operations.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/utils/sickle_serializers.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/utils/sickle_serializers.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/utils/transform_operations.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/utils/transform_operations.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/views/admin/ajax.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/views/admin/ajax.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/views/admin/forms.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/views/admin/forms.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django import forms
+from django.conf import settings
 from django.core.validators import MinValueValidator
 
 import core_oaipmh_harvester_app.components.oai_registry.api as oai_registry_api
 from core_oaipmh_harvester_app.components.oai_registry.models import (
     OaiRegistry,
 )
 
@@ -141,44 +142,43 @@
             self.fields["sets"].queryset = sets
 
 
 class RequestForm(forms.Form):
     """Request builder form"""
 
     # Widget attributes
-    default_attributes = {"class": "form-control"}
-    disabled_attributes = {"class": "form-control", "disabled": "true"}
+    disabled_attributes = {"disabled": "true"}
     date_attributes = {
         "data-date-format": "yyyy-mm-ddThh:ii:00Z",
         "class": "form-control",
         "style": "width:160px",
     }
 
     data_provider = forms.ChoiceField(
         label="Data Provider",
         choices=[],
         required=False,
-        widget=forms.Select(attrs=default_attributes),
+        widget=forms.Select(),
     )
     verb = forms.ChoiceField(
         label="Verb",
         choices=VERBS,
         required=False,
-        widget=forms.Select(attrs=default_attributes),
+        widget=forms.Select(),
     )
     set = forms.ChoiceField(
         label="Set",
         choices=[],
         required=False,
         widget=forms.Select(attrs=disabled_attributes),
     )
     identifier = forms.CharField(
         label="Identifier",
         required=False,
-        widget=forms.TextInput(attrs=default_attributes),
+        widget=forms.TextInput(attrs={"class": "form-control"}),
     )
     metadata_prefix = forms.ChoiceField(
         label="Metadata Prefix",
         choices=[],
         required=False,
         widget=forms.Select(attrs=disabled_attributes),
     )
@@ -202,14 +202,30 @@
         super().__init__()
 
         default_fields = [("0", "Pick one")]
 
         self.fields["metadata_prefix"].choices = default_fields
         self.fields["set"].choices = default_fields
 
+        if settings.BOOTSTRAP_VERSION == "4.6.2":
+            self.fields["data_provider"].widget.attrs["class"] = "form-control"
+            self.fields["verb"].widget.attrs["class"] = "form-control"
+            self.fields["set"].widget.attrs["class"] = "form-control"
+            self.fields["metadata_prefix"].widget.attrs[
+                "class"
+            ] = "form-control"
+
+        elif settings.BOOTSTRAP_VERSION == "5.1.3":
+            self.fields["data_provider"].widget.attrs["class"] = "form-select"
+            self.fields["verb"].widget.attrs["class"] = "form-select"
+            self.fields["set"].widget.attrs["class"] = "form-select"
+            self.fields["metadata_prefix"].widget.attrs[
+                "class"
+            ] = "form-select"
+
         for registry in oai_registry_api.get_all_activated_registry():
             default_fields.append(
                 (
                     "%s|%s" % (str(registry.id), registry.url),
                     str(registry.name),
                 )
             )
```

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app/views/admin/views.py` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app.egg-info/PKG-INFO` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-oaipmh-harvester-app
-Version: 2.3.0
+Version: 2.4.0
 Summary: OAI-PMH harvesting capabilities for the curator core project
 Home-page: https://github.com/usnistgov/core_oaipmh_harvester_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =========================
         Core Oaipmh Harvester App
```

### Comparing `core_oaipmh_harvester_app-2.3.0/core_oaipmh_harvester_app.egg-info/SOURCES.txt` & `core_oaipmh_harvester_app-2.4.0/core_oaipmh_harvester_app.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -152,8 +152,10 @@
 tests/system/api/tests_unit.py
 tests/utils/__init__.py
 tests/utils/tests_unit_query_builder.py
 tests/utils/tests_unit_transform_operations.py
 tests/views/__init__.py
 tests/views/admin/__init__.py
 tests/views/admin/ajax/__init__.py
-tests/views/admin/ajax/tests_unit.py
+tests/views/admin/ajax/tests_unit.py
+tests/views/admin/forms/__init__.py
+tests/views/admin/forms/test_unit.py
```

### Comparing `core_oaipmh_harvester_app-2.3.0/docs/conf.py` & `core_oaipmh_harvester_app-2.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/setup.py` & `core_oaipmh_harvester_app-2.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_oaipmh_harvester_app",
-    version="2.3.0",
+    version="2.4.0",
     description="OAI-PMH harvesting capabilities for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_oaipmh_harvester_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_oaipmh_harvester_app-2.3.0/tests/components/mongo/models/test_unit.py` & `core_oaipmh_harvester_app-2.4.0/tests/components/mongo/models/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/tests/components/oai_harvester_metadata_format/tests_unit.py` & `core_oaipmh_harvester_app-2.4.0/tests/components/oai_harvester_metadata_format/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/tests/components/oai_harvester_metadata_format_set/tests_unit.py` & `core_oaipmh_harvester_app-2.4.0/tests/components/oai_harvester_metadata_format_set/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/tests/components/oai_harvester_set/tests_unit.py` & `core_oaipmh_harvester_app-2.4.0/tests/components/oai_harvester_set/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/tests/components/oai_identify/tests_unit.py` & `core_oaipmh_harvester_app-2.4.0/tests/components/oai_identify/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/tests/components/oai_record/tests_unit.py` & `core_oaipmh_harvester_app-2.4.0/tests/components/oai_record/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/tests/components/oai_registry/fixtures/fixtures.py` & `core_oaipmh_harvester_app-2.4.0/tests/components/oai_registry/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/tests/components/oai_registry/tests_int.py` & `core_oaipmh_harvester_app-2.4.0/tests/components/oai_registry/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/tests/components/oai_registry/tests_unit.py` & `core_oaipmh_harvester_app-2.4.0/tests/components/oai_registry/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/tests/components/oai_verbs/tests_unit.py` & `core_oaipmh_harvester_app-2.4.0/tests/components/oai_verbs/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/tests/rest/oai_record/tests_int_mongo.py` & `core_oaipmh_harvester_app-2.4.0/tests/rest/oai_record/tests_int_mongo.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/tests/rest/oai_record/tests_int_psql.py` & `core_oaipmh_harvester_app-2.4.0/tests/rest/oai_record/tests_int_psql.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/tests/rest/oai_record/tests_permissions.py` & `core_oaipmh_harvester_app-2.4.0/tests/rest/oai_record/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/tests/rest/oai_registry/tests_int.py` & `core_oaipmh_harvester_app-2.4.0/tests/rest/oai_registry/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/tests/rest/oai_registry/tests_permissions.py` & `core_oaipmh_harvester_app-2.4.0/tests/rest/oai_registry/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/tests/rest/oai_registry/tests_unit.py` & `core_oaipmh_harvester_app-2.4.0/tests/rest/oai_registry/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/tests/system/api/tests_unit.py` & `core_oaipmh_harvester_app-2.4.0/tests/system/api/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/tests/test_settings.py` & `core_oaipmh_harvester_app-2.4.0/tests/test_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,7 +62,8 @@
 SSL_CERTIFICATES_DIR = True
 CELERYBEAT_SCHEDULER = "django_celery_beat.schedulers:DatabaseScheduler"
 
 USE_TZ = True
 
 MONGODB_INDEXING = False
 MONGODB_ASYNC_SAVE = False
+BOOTSTRAP_VERSION = "5.1.3"
```

### Comparing `core_oaipmh_harvester_app-2.3.0/tests/utils/tests_unit_query_builder.py` & `core_oaipmh_harvester_app-2.4.0/tests/utils/tests_unit_query_builder.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/tests/utils/tests_unit_transform_operations.py` & `core_oaipmh_harvester_app-2.4.0/tests/utils/tests_unit_transform_operations.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.3.0/tests/views/admin/ajax/tests_unit.py` & `core_oaipmh_harvester_app-2.4.0/tests/views/admin/ajax/tests_unit.py`

 * *Files identical despite different names*

