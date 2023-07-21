# Comparing `tmp/core_oaipmh_provider_app-2.3.0.tar.gz` & `tmp/core_oaipmh_provider_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_oaipmh_provider_app-2.3.0.tar", last modified: Tue May  2 19:47:36 2023, max compression
+gzip compressed data, was "core_oaipmh_provider_app-2.4.0.tar", last modified: Fri Jul 21 02:16:35 2023, max compression
```

## Comparing `core_oaipmh_provider_app-2.3.0.tar` & `core_oaipmh_provider_app-2.4.0.tar`

### file list

```diff
@@ -1,209 +1,214 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:36.357797 core_oaipmh_provider_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1118 2023-05-02 19:47:36.352805 core_oaipmh_provider_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      611 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.014911 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4465 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2593 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.191938 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      150 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/commons/constants.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3064 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/commons/exceptions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       54 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/commons/status.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.210087 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.276342 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3741 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_data/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5466 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_data/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1535 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_data/watch.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.331434 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10750 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2310 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4113 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.376352 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_set/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2308 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_set/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2579 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_set/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.421787 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_request_page/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_request_page/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1637 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_request_page/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_request_page/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.476907 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_settings/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      465 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_settings/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1651 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_settings/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1017 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_settings/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.525511 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_xsl_template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_xsl_template/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2595 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_xsl_template/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3598 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_xsl_template/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      584 2023-05-02 19:47:28.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.574761 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7245 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      900 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/migrations/0002_oai_data_on_delete.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      527 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/migrations/0003_oai_data_bulk_delete.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.620583 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.657695 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14117 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.692253 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_provider_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_provider_set/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7772 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_provider_set/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.743776 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_settings/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4347 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_settings/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7797 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1759 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1568 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:33.482442 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:33.561710 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:33.530994 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:33.493589 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:33.513690 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.772426 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/identity/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      584 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/identity/table_info.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.789927 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/metadata_formats/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/metadata_formats/page.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.807505 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/sets/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       63 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/sets/add_set.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:33.534470 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:33.537794 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.844033 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1082 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/check_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       91 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/check_registry.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.872195 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1444 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/oai_dc.xsd
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3029 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/simpledc20021212.xsd
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.907192 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      490 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/system/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1976 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:33.602504 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:33.638078 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:33.610512 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.979847 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.996293 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/identity/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2016 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/identity/table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      259 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/identity.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.043552 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_default.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2232 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_metadata_formats.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2013 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_template_metadata_formats.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      502 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.059590 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1799 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets/table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      251 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.075751 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1877 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template/table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      382 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:33.647604 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.244524 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      717 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/base.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      201 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/error.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      635 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/get_record.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      254 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/header.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1118 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/identify.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      374 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_identifiers.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      407 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_metadata_formats.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      577 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_records.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1030 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_sets.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      298 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/resumption_token.xml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      566 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.276029 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5850 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/utils/request_checker.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.293151 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.347323 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11317 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7785 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7309 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.375686 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    24356 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:34.106797 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1118 2023-05-02 19:47:32.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7656 2023-05-02 19:47:33.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:47:32.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      131 2023-05-02 19:47:32.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-05-02 19:47:32.000000 core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.450021 core_oaipmh_provider_app-2.3.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11332 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-05-02 19:47:29.000000 core_oaipmh_provider_app-2.3.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:47:36.360168 core_oaipmh_provider_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1481 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.494883 core_oaipmh_provider_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.520025 core_oaipmh_provider_app-2.3.0/tests/apps/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/apps/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1799 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/apps/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.534071 core_oaipmh_provider_app-2.3.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.551826 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1527 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.599741 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2277 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/api/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9480 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/api/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.647009 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/models/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/models/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1315 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/models/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7942 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/models/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.682212 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/watch/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/watch/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1098 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_data/watch/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.719308 core_oaipmh_provider_app-2.3.0/tests/components/oai_provider_metadata_format/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_provider_metadata_format/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13665 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_provider_metadata_format/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.754989 core_oaipmh_provider_app-2.3.0/tests/components/oai_provider_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_provider_set/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9462 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_provider_set/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.804848 core_oaipmh_provider_app-2.3.0/tests/components/oai_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_settings/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2770 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_settings/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.853458 core_oaipmh_provider_app-2.3.0/tests/components/oai_xsl_template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_xsl_template/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9663 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/components/oai_xsl_template/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.870952 core_oaipmh_provider_app-2.3.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:35.937357 core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_metadata_format/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_metadata_format/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6987 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_metadata_format/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16462 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_metadata_format/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17947 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_metadata_format/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:36.036130 core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_set/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5329 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_set/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8591 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_set/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5925 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_set/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:36.099854 core_oaipmh_provider_app-2.3.0/tests/rest/oai_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_settings/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2618 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_settings/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4840 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_settings/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3149 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/rest/oai_settings/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1924 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:36.173611 core_oaipmh_provider_app-2.3.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:36.208734 core_oaipmh_provider_app-2.3.0/tests/utils/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/utils/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12394 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/utils/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      539 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/utils/mocks.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1299 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/utils/test_oai_pmh_suite.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:36.223141 core_oaipmh_provider_app-2.3.0/tests/utils/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:30.000000 core_oaipmh_provider_app-2.3.0/tests/utils/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:36.275453 core_oaipmh_provider_app-2.3.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:31.000000 core_oaipmh_provider_app-2.3.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:36.336074 core_oaipmh_provider_app-2.3.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:47:31.000000 core_oaipmh_provider_app-2.3.0/tests/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5607 2023-05-02 19:47:31.000000 core_oaipmh_provider_app-2.3.0/tests/views/user/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    45422 2023-05-02 19:47:31.000000 core_oaipmh_provider_app-2.3.0/tests/views/user/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:35.135522 core_oaipmh_provider_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:16:27.000000 core_oaipmh_provider_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-07-21 02:16:27.000000 core_oaipmh_provider_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1118 2023-07-21 02:16:35.130623 core_oaipmh_provider_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      611 2023-07-21 02:16:27.000000 core_oaipmh_provider_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.006462 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2023-07-21 02:16:27.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4465 2023-07-21 02:16:27.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2593 2023-07-21 02:16:27.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.160215 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:27.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      150 2023-07-21 02:16:27.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/commons/constants.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3064 2023-07-21 02:16:27.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/commons/exceptions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       54 2023-07-21 02:16:27.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/commons/status.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.174685 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:27.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.229095 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:27.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3741 2023-07-21 02:16:27.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_data/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5466 2023-07-21 02:16:27.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_data/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1535 2023-07-21 02:16:27.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_data/watch.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.285705 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:27.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10750 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2310 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4113 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.333206 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_provider_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_provider_set/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2308 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_provider_set/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2579 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_provider_set/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.372614 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_request_page/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_request_page/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1637 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_request_page/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_request_page/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.425385 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_settings/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      465 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_settings/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1651 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_settings/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1017 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_settings/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.468900 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_xsl_template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_xsl_template/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2595 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_xsl_template/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3598 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_xsl_template/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      584 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.526915 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7245 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      900 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/migrations/0002_oai_data_on_delete.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      527 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/migrations/0003_oai_data_bulk_delete.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.573527 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.615586 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14117 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.648847 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/rest/oai_provider_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/rest/oai_provider_set/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7772 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/rest/oai_provider_set/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.681679 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/rest/oai_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/rest/oai_settings/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4347 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/rest/oai_settings/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7797 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/rest/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1759 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1568 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:32.563612 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:32.647590 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:32.636285 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:32.573419 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:32.618588 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.710129 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/identity/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      619 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/identity/table_info.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.726270 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/metadata_formats/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/metadata_formats/page.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.740094 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/sets/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       63 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/sets/add_set.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:32.639478 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:32.642765 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.771216 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1735 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/check_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       91 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/check_registry.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.802774 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1444 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/oai_dc.xsd
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3029 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/simpledc20021212.xsd
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.832118 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      490 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/system/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1976 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:32.673723 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:32.724365 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:32.680520 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.898148 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.921798 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/identity/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2447 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/identity/table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      259 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/identity.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.965898 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_default.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2328 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_metadata_formats.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2109 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_template_metadata_formats.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      502 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.979550 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1895 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets/table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      251 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.008510 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1973 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template/table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      382 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:32.727746 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.141092 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      717 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/base.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      201 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/error.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      635 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/get_record.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      254 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/header.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1118 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/identify.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      374 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_identifiers.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      407 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_metadata_formats.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      577 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_records.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1030 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_sets.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      298 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/resumption_token.xml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      566 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.172728 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5850 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/utils/request_checker.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.188943 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.260569 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11317 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8327 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7309 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.291196 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    24356 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:33.088257 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1118 2023-07-21 02:16:31.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7759 2023-07-21 02:16:32.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:16:31.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      131 2023-07-21 02:16:31.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-07-21 02:16:31.000000 core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.329702 core_oaipmh_provider_app-2.4.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:28.000000 core_oaipmh_provider_app-2.4.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11332 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:16:35.208640 core_oaipmh_provider_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1481 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.360051 core_oaipmh_provider_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.389466 core_oaipmh_provider_app-2.4.0/tests/apps/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/apps/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1799 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/apps/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.404082 core_oaipmh_provider_app-2.4.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.422334 core_oaipmh_provider_app-2.4.0/tests/components/oai_data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1527 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/components/oai_data/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.467207 core_oaipmh_provider_app-2.4.0/tests/components/oai_data/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/components/oai_data/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2277 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/components/oai_data/api/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9480 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/components/oai_data/api/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.509492 core_oaipmh_provider_app-2.4.0/tests/components/oai_data/models/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/components/oai_data/models/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1315 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/components/oai_data/models/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7942 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/components/oai_data/models/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.536222 core_oaipmh_provider_app-2.4.0/tests/components/oai_data/watch/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/components/oai_data/watch/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1098 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/components/oai_data/watch/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.568381 core_oaipmh_provider_app-2.4.0/tests/components/oai_provider_metadata_format/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/components/oai_provider_metadata_format/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13665 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/components/oai_provider_metadata_format/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.596049 core_oaipmh_provider_app-2.4.0/tests/components/oai_provider_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/components/oai_provider_set/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9462 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/components/oai_provider_set/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.621839 core_oaipmh_provider_app-2.4.0/tests/components/oai_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/components/oai_settings/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2770 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/components/oai_settings/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.648413 core_oaipmh_provider_app-2.4.0/tests/components/oai_xsl_template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/components/oai_xsl_template/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9663 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/components/oai_xsl_template/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.667873 core_oaipmh_provider_app-2.4.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.798373 core_oaipmh_provider_app-2.4.0/tests/rest/oai_provider_metadata_format/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/rest/oai_provider_metadata_format/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6987 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/rest/oai_provider_metadata_format/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16462 2023-07-21 02:16:29.000000 core_oaipmh_provider_app-2.4.0/tests/rest/oai_provider_metadata_format/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17947 2023-07-21 02:16:30.000000 core_oaipmh_provider_app-2.4.0/tests/rest/oai_provider_metadata_format/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.858024 core_oaipmh_provider_app-2.4.0/tests/rest/oai_provider_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:30.000000 core_oaipmh_provider_app-2.4.0/tests/rest/oai_provider_set/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5329 2023-07-21 02:16:30.000000 core_oaipmh_provider_app-2.4.0/tests/rest/oai_provider_set/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8591 2023-07-21 02:16:30.000000 core_oaipmh_provider_app-2.4.0/tests/rest/oai_provider_set/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5925 2023-07-21 02:16:30.000000 core_oaipmh_provider_app-2.4.0/tests/rest/oai_provider_set/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.910981 core_oaipmh_provider_app-2.4.0/tests/rest/oai_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:30.000000 core_oaipmh_provider_app-2.4.0/tests/rest/oai_settings/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2618 2023-07-21 02:16:30.000000 core_oaipmh_provider_app-2.4.0/tests/rest/oai_settings/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4840 2023-07-21 02:16:30.000000 core_oaipmh_provider_app-2.4.0/tests/rest/oai_settings/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3149 2023-07-21 02:16:30.000000 core_oaipmh_provider_app-2.4.0/tests/rest/oai_settings/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1952 2023-07-21 02:16:30.000000 core_oaipmh_provider_app-2.4.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.961768 core_oaipmh_provider_app-2.4.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:30.000000 core_oaipmh_provider_app-2.4.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:34.992137 core_oaipmh_provider_app-2.4.0/tests/utils/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:30.000000 core_oaipmh_provider_app-2.4.0/tests/utils/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12394 2023-07-21 02:16:30.000000 core_oaipmh_provider_app-2.4.0/tests/utils/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      539 2023-07-21 02:16:30.000000 core_oaipmh_provider_app-2.4.0/tests/utils/mocks.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1299 2023-07-21 02:16:30.000000 core_oaipmh_provider_app-2.4.0/tests/utils/test_oai_pmh_suite.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:35.007387 core_oaipmh_provider_app-2.4.0/tests/utils/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:30.000000 core_oaipmh_provider_app-2.4.0/tests/utils/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:35.024545 core_oaipmh_provider_app-2.4.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:30.000000 core_oaipmh_provider_app-2.4.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:35.042364 core_oaipmh_provider_app-2.4.0/tests/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:30.000000 core_oaipmh_provider_app-2.4.0/tests/views/admin/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:35.074156 core_oaipmh_provider_app-2.4.0/tests/views/admin/forms/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:30.000000 core_oaipmh_provider_app-2.4.0/tests/views/admin/forms/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2900 2023-07-21 02:16:30.000000 core_oaipmh_provider_app-2.4.0/tests/views/admin/forms/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:35.113578 core_oaipmh_provider_app-2.4.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:16:30.000000 core_oaipmh_provider_app-2.4.0/tests/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5607 2023-07-21 02:16:30.000000 core_oaipmh_provider_app-2.4.0/tests/views/user/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    45422 2023-07-21 02:16:30.000000 core_oaipmh_provider_app-2.4.0/tests/views/user/tests_unit.py
```

### Comparing `core_oaipmh_provider_app-2.3.0/LICENSE.md` & `core_oaipmh_provider_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/PKG-INFO` & `core_oaipmh_provider_app-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_oaipmh_provider_app
-Version: 2.3.0
+Version: 2.4.0
 Summary: OAI-PMH provider capabilities for the curator core project
 Home-page: https://github.com/usnistgov/core_oaipmh_provider_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ========================
         Core Oaipmh Provider App
```

### Comparing `core_oaipmh_provider_app-2.3.0/README.rst` & `core_oaipmh_provider_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/admin.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/apps.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/commons/exceptions.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/commons/exceptions.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_data/api.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_data/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_data/models.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_data/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_data/watch.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_data/watch.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/api.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/discover.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/discover.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/models.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_set/api.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_provider_set/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_provider_set/models.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_provider_set/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_request_page/api.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_request_page/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_request_page/models.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_request_page/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_settings/discover.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_settings/discover.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_settings/models.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_settings/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_xsl_template/api.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_xsl_template/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/components/oai_xsl_template/models.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/components/oai_xsl_template/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/menus.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/migrations/0001_initial.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/migrations/0002_oai_data_on_delete.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/migrations/0002_oai_data_on_delete.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/migrations/0003_oai_data_bulk_delete.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/migrations/0003_oai_data_bulk_delete.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/views.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/views.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_provider_set/views.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/rest/oai_provider_set/views.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/oai_settings/views.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/rest/oai_settings/views.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/serializers.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/rest/serializers.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/rest/urls.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/settings.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/identity/table_info.css` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/identity/table_info.css`

 * *Files 20% similar despite different names*

```diff
@@ -20,8 +20,12 @@
     font-weight: bold;
     text-transform: capitalize;
     color: black;
 }
 table.data-table {
     font-style: italic;
     color: #001ade;
+}
+
+.base-url{
+    display: inline;
 }
```

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/oai_dc.xsd` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/oai_dc.xsd`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/simpledc20021212.xsd` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/simpledc20021212.xsd`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/tasks.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/tasks.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_default.html` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_default.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_metadata_formats.html` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_metadata_formats.html`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     Other Metadata Formats <br/>
     <small>Add other metadata formats by providing a URL.
         You will need to configure an XSLT file for each Template to perform the
         mapping between the templates and those metadata formats.
     </small>
 {% endblock %}
 {% block box_tools %}
-<div class="btn-group float-right">
+<div class="btn-group {% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}">
     {% url 'core-admin:core_oaipmh_provider_app_add_metadata_format' as add_url %}
     {% include 'core_main_app/common/buttons/add.html' with label='Add Metadata Format' %}
 </div>
 {% endblock %}
 {% block box_body %}
 <table class="table table-bordered table-striped table-hover">
     <tr>
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% block
 box_title %} Other Metadata Formats
 Add other metadata formats by providing a URL. You will need to configure an
 XSLT file for each Template to perform the mapping between the templates and
 those metadata formats. {% endblock %} {% block box_tools %}
-{% url 'core-admin:core_oaipmh_provider_app_add_metadata_format' as add_url %}
-{% include 'core_main_app/common/buttons/add.html' with label='Add Metadata
-Format' %}
+.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif
+%}"> {% url 'core-admin:core_oaipmh_provider_app_add_metadata_format' as
+add_url %} {% include 'core_main_app/common/buttons/add.html' with label='Add
+Metadata Format' %}
 {% endblock %} {% block box_body %}
 Metadata Prefix                 Schema                 Namespace                          Actions
                                                                                           {% url 'core-admin:
                                                                                           core_oaipmh_provider_app_edit_metadata_format'
                                                                                           metadata_format.id as edit_url %} {% include
 {                               {                      {                                  'core_main_app/common/buttons/edit.html' %} {%
 {                               {                      {                                  url 'core-admin:
```

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_template_metadata_formats.html` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_template_metadata_formats.html`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     Templates as Metadata Formats <br/>
     <small>
         Add templates as metadata formats in order to exchange metadata records directly.
         Please note metadata format will be associated only to the template that you select.
     </small>
 {% endblock %}
 {% block box_tools %}
-<div class="btn-group float-right">
+<div class="btn-group {% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}">
     {% url 'core-admin:core_oaipmh_provider_app_add_template_metadata_format' as add_url %}
     {% include 'core_main_app/common/buttons/add.html' with label='Add Metadata Format' %}
 </div>
 {% endblock %}
 {% block box_body %}
 <table class="table table-bordered table-striped table-hover">
     <tr>
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% block
 box_title %} Templates as Metadata Formats
 Add templates as metadata formats in order to exchange metadata records
 directly. Please note metadata format will be associated only to the template
 that you select. {% endblock %} {% block box_tools %}
-{% url 'core-admin:core_oaipmh_provider_app_add_template_metadata_format' as
-add_url %} {% include 'core_main_app/common/buttons/add.html' with label='Add
-Metadata Format' %}
+.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif
+%}"> {% url 'core-admin:core_oaipmh_provider_app_add_template_metadata_format'
+as add_url %} {% include 'core_main_app/common/buttons/add.html' with
+label='Add Metadata Format' %}
 {% endblock %} {% block box_body %}
 Metadata Prefix                 Schema                 Namespace                          Template              Actions
                                                                                                                 {% url 'core-admin:
                                                                                                                 core_oaipmh_provider_app_edit_metadata_format'
 {                               {                      {                                  {                     metadata_format.id as edit_url %} {% include
 {                               {                      {                                  {                     'core_main_app/common/buttons/edit.html' %} {%
 metadata_format.metadata_prefix metadata_format.schema metadata_format.metadata_namespace metadata_format.title url 'core-admin:
```

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets/table.html` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets/table.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %}
 
 {% block box_title %}Sets{% endblock %}
 {% block box_tools %}
-<div class="btn-group float-right">
+<div class="btn-group {% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}">
     {% url 'core-admin:core_oaipmh_provider_app_add_set' as add_url %}
     {% include 'core_main_app/common/buttons/add.html' with label='Add Set' %}
 </div>
 {% endblock %}
 {% block box_body %}
 <p>
    Add sets to your server by associating templates to them.
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% block
 box_title %}Sets{% endblock %} {% block box_tools %}
-{% url 'core-admin:core_oaipmh_provider_app_add_set' as add_url %} {% include
-'core_main_app/common/buttons/add.html' with label='Add Set' %}
+.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif
+%}"> {% url 'core-admin:core_oaipmh_provider_app_add_set' as add_url %} {%
+include 'core_main_app/common/buttons/add.html' with label='Add Set' %}
 {% endblock %} {% block box_body %}
 Add sets to your server by associating templates to them.
 Set Spec     Set Name     Associate Templates       Description     Actions
                                                                     {% url 'core-admin:
                                                                     core_oaipmh_provider_app_edit_set'
 {            {            {% for manager in         {               set.id as edit_url %} {% include
 {            {            set.templates_manager.all {               'core_main_app/common/buttons/
```

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template/table.html` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template/table.html`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 {% block box_title %}Mapping <br/>
 <small>
    Map a template with an XSLT to convert the template toward metadata format
     <b>{{ data.metadata_format.metadata_prefix }}</b>.
 </small>
 {% endblock %}
 {% block box_tools %}
-<div class="btn-group float-right">
+<div class="btn-group {% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}">
     <a href="{% url 'core-admin:core_oaipmh_provider_app_metadata_formats'%}" class="btn btn-secondary">
         <i class="fas fa-arrow-left"></i> Previous page
     </a>
     {% url 'core-admin:core_oaipmh_provider_app_add_template_mapping' data.metadata_format.id as add_url %}
     {% include 'core_main_app/common/buttons/add.html' with label='Add Mapping' %}
 </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,11 +1,13 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% block
 box_title %}Mapping
 Map a template with an XSLT to convert the template toward metadata format {
 { data.metadata_format.metadata_prefix }}. {% endblock %} {% block box_tools %}
+.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif
+%}">
  Previous_page
  {% url 'core-admin:core_oaipmh_provider_app_add_template_mapping'
 data.metadata_format.id as add_url %} {% include 'core_main_app/common/buttons/
 add.html' with label='Add Mapping' %}
 {% endblock %} {% block box_body %}
 Template                    XSLT name              Actions
                                                    {% url 'core-admin:
```

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/base.html` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/base.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/get_record.html` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/get_record.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/identify.html` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/identify.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_records.html` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_records.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_sets.html` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_sets.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/urls.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/utils/request_checker.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/utils/request_checker.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/admin/ajax.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/views/admin/ajax.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/admin/forms.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/views/admin/forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ OAI pmh provider admin form file
 """
 import logging
 
 from django import forms
+from django.conf import settings
 
 from core_main_app.commons import exceptions
 from core_main_app.components.template import api as template_api
 from core_main_app.components.template_version_manager import (
     api as template_version_manager_api,
 )
 from core_main_app.components.xsl_transformation import (
@@ -115,30 +116,32 @@
     metadata_prefix = forms.CharField(
         label="Metadata Prefix",
         required=True,
         widget=forms.TextInput(
             attrs={"placeholder": "example: oai_dc", "class": "form-control"}
         ),
     )
-    template = forms.ChoiceField(
-        label="Template", widget=forms.Select(attrs={"class": "form-control"})
-    )
+    template = forms.ChoiceField(label="Template", widget=forms.Select())
 
     class Meta:
         """Meta"""
 
         model = OaiProviderMetadataFormat
         fields = ["metadata_prefix", "template"]
 
     def __init__(self, *args, **kwargs):
         self.request = kwargs.pop("request")
         super().__init__(*args, **kwargs)
         self.fields["template"].choices = _get_templates_versions(
             request=self.request
         )
+        if settings.BOOTSTRAP_VERSION == "4.6.2":
+            self.fields["template"].widget.attrs["class"] = "form-control"
+        elif settings.BOOTSTRAP_VERSION == "5.1.3":
+            self.fields["template"].widget.attrs["class"] = "form-select"
 
     def clean_template(self):
         data = self.cleaned_data["template"]
         return template_api.get_by_id(data, request=self.request)
 
 
 class SetForm(forms.ModelForm):
@@ -200,20 +203,16 @@
 
     oai_metadata_format = forms.ModelChoiceField(
         widget=forms.HiddenInput(),
         queryset=oai_provider_metadata_format_api.get_all(),
         label="Metadata Prefix",
         required=True,
     )
-    template = forms.ChoiceField(
-        label="Template", widget=forms.Select(attrs={"class": "form-control"})
-    )
-    xslt = forms.ChoiceField(
-        label="XSLT", widget=forms.Select(attrs={"class": "form-control"})
-    )
+    template = forms.ChoiceField(label="Template", widget=forms.Select())
+    xslt = forms.ChoiceField(label="XSLT", widget=forms.Select())
 
     class Meta:
         """Meta"""
 
         model = OaiXslTemplate
         fields = ["oai_metadata_format", "template", "xslt"]
 
@@ -224,14 +223,21 @@
         self.fields["template"].choices = _get_templates_versions(
             request=self.request
         )
         self.fields["xslt"].choices = _get_xsl_transformation()
         if edit_mode:
             self.fields["template"].widget = forms.HiddenInput()
 
+        if settings.BOOTSTRAP_VERSION == "4.6.2":
+            self.fields["xslt"].widget.attrs["class"] = "form-control"
+            self.fields["template"].widget.attrs["class"] = "form-control"
+        elif settings.BOOTSTRAP_VERSION == "5.1.3":
+            self.fields["xslt"].widget.attrs["class"] = "form-select"
+            self.fields["template"].widget.attrs["class"] = "form-select"
+
     def clean_xslt(self):
         data = self.cleaned_data["xslt"]
         return xsl_transformation_api.get_by_id(data)
 
     def clean_template(self):
         data = self.cleaned_data["template"]
         return template_api.get_by_id(data, request=self.request)
```

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/admin/views.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app/views/user/views.py` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app.egg-info/PKG-INFO` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-oaipmh-provider-app
-Version: 2.3.0
+Version: 2.4.0
 Summary: OAI-PMH provider capabilities for the curator core project
 Home-page: https://github.com/usnistgov/core_oaipmh_provider_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ========================
         Core Oaipmh Provider App
```

### Comparing `core_oaipmh_provider_app-2.3.0/core_oaipmh_provider_app.egg-info/SOURCES.txt` & `core_oaipmh_provider_app-2.4.0/core_oaipmh_provider_app.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -134,10 +134,13 @@
 tests/utils/__init__.py
 tests/utils/mocks.py
 tests/utils/test_oai_pmh_suite.py
 tests/utils/fixtures/__init__.py
 tests/utils/fixtures/fixtures.py
 tests/utils/tests/__init__.py
 tests/views/__init__.py
+tests/views/admin/__init__.py
+tests/views/admin/forms/__init__.py
+tests/views/admin/forms/test_unit.py
 tests/views/user/__init__.py
 tests/views/user/tests_int.py
 tests/views/user/tests_unit.py
```

### Comparing `core_oaipmh_provider_app-2.3.0/docs/conf.py` & `core_oaipmh_provider_app-2.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/setup.py` & `core_oaipmh_provider_app-2.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_oaipmh_provider_app",
-    version="2.3.0",
+    version="2.4.0",
     description="OAI-PMH provider capabilities for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_oaipmh_provider_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_oaipmh_provider_app-2.3.0/tests/apps/tests_unit.py` & `core_oaipmh_provider_app-2.4.0/tests/apps/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/components/oai_data/__init__.py` & `core_oaipmh_provider_app-2.4.0/tests/components/oai_data/__init__.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/components/oai_data/api/tests_int.py` & `core_oaipmh_provider_app-2.4.0/tests/components/oai_data/api/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/components/oai_data/api/tests_unit.py` & `core_oaipmh_provider_app-2.4.0/tests/components/oai_data/api/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/components/oai_data/models/tests_int.py` & `core_oaipmh_provider_app-2.4.0/tests/components/oai_data/models/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/components/oai_data/models/tests_unit.py` & `core_oaipmh_provider_app-2.4.0/tests/components/oai_data/models/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/components/oai_data/watch/tests_unit.py` & `core_oaipmh_provider_app-2.4.0/tests/components/oai_data/watch/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/components/oai_provider_metadata_format/tests_unit.py` & `core_oaipmh_provider_app-2.4.0/tests/components/oai_provider_metadata_format/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/components/oai_provider_set/tests_unit.py` & `core_oaipmh_provider_app-2.4.0/tests/components/oai_provider_set/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/components/oai_settings/tests_unit.py` & `core_oaipmh_provider_app-2.4.0/tests/components/oai_settings/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/components/oai_xsl_template/tests_unit.py` & `core_oaipmh_provider_app-2.4.0/tests/components/oai_xsl_template/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_metadata_format/tests_int.py` & `core_oaipmh_provider_app-2.4.0/tests/rest/oai_provider_metadata_format/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_metadata_format/tests_permissions.py` & `core_oaipmh_provider_app-2.4.0/tests/rest/oai_provider_metadata_format/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_metadata_format/tests_unit.py` & `core_oaipmh_provider_app-2.4.0/tests/rest/oai_provider_metadata_format/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_set/tests_int.py` & `core_oaipmh_provider_app-2.4.0/tests/rest/oai_provider_set/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_set/tests_permissions.py` & `core_oaipmh_provider_app-2.4.0/tests/rest/oai_provider_set/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/rest/oai_provider_set/tests_unit.py` & `core_oaipmh_provider_app-2.4.0/tests/rest/oai_provider_set/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/rest/oai_settings/tests_int.py` & `core_oaipmh_provider_app-2.4.0/tests/rest/oai_settings/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/rest/oai_settings/tests_permissions.py` & `core_oaipmh_provider_app-2.4.0/tests/rest/oai_settings/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/rest/oai_settings/tests_unit.py` & `core_oaipmh_provider_app-2.4.0/tests/rest/oai_settings/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/test_settings.py` & `core_oaipmh_provider_app-2.4.0/tests/test_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,7 +76,8 @@
 
 DEFAULT_AUTO_FIELD = "django.db.models.BigAutoField"
 CELERYBEAT_SCHEDULER = "django_celery_beat.schedulers:DatabaseScheduler"
 
 MONGODB_INDEXING = False
 MONGODB_ASYNC_SAVE = False
 ENABLE_SAML2_SSO_AUTH = False
+BOOTSTRAP_VERSION = "5.1.3"
```

### Comparing `core_oaipmh_provider_app-2.3.0/tests/utils/fixtures/fixtures.py` & `core_oaipmh_provider_app-2.4.0/tests/utils/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/utils/mocks.py` & `core_oaipmh_provider_app-2.4.0/tests/utils/mocks.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/utils/test_oai_pmh_suite.py` & `core_oaipmh_provider_app-2.4.0/tests/utils/test_oai_pmh_suite.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/views/user/tests_int.py` & `core_oaipmh_provider_app-2.4.0/tests/views/user/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.3.0/tests/views/user/tests_unit.py` & `core_oaipmh_provider_app-2.4.0/tests/views/user/tests_unit.py`

 * *Files identical despite different names*

