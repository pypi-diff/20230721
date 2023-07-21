# Comparing `tmp/core_exporters_app-2.3.0.tar.gz` & `tmp/core_exporters_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_exporters_app-2.3.0.tar", last modified: Tue May  2 19:38:47 2023, max compression
+gzip compressed data, was "core_exporters_app-2.4.0.tar", last modified: Fri Jul 21 02:12:40 2023, max compression
```

## Comparing `core_exporters_app-2.3.0.tar` & `core_exporters_app-2.4.0.tar`

### file list

```diff
@@ -1,203 +1,203 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.541329 core_exporters_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1017 2023-05-02 19:38:47.536278 core_exporters_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      542 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.467170 core_exporters_app-2.3.0/core_exporters_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       93 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.604812 core_exporters_app-2.3.0/core_exporters_app/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      931 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/access_control/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1764 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      704 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.640346 core_exporters_app-2.3.0/core_exporters_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/commons/constants.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.656939 core_exporters_app-2.3.0/core_exporters_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.721808 core_exporters_app-2.3.0/core_exporters_app/components/exported_compressed_file/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/components/exported_compressed_file/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      404 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/components/exported_compressed_file/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      778 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/components/exported_compressed_file/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1365 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/components/exported_compressed_file/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.849178 core_exporters_app-2.3.0/core_exporters_app/components/exporter/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/components/exporter/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      318 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/components/exporter/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1537 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/components/exporter/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6984 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/components/exporter/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1451 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/components/exporter/watch.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.945022 core_exporters_app-2.3.0/core_exporters_app/exporters/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.001441 core_exporters_app-2.3.0/core_exporters_app/exporters/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/blob/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4587 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/blob/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      221 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/blob/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4576 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5910 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/exporter.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.056586 core_exporters_app-2.3.0/core_exporters_app/exporters/json_exporter/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/json_exporter/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2358 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/json_exporter/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      230 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/json_exporter/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      323 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.098734 core_exporters_app-2.3.0/core_exporters_app/exporters/xml/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xml/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1789 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xml/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      216 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xml/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.166719 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2801 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3358 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:44.887562 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:44.891345 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/static/xsl/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:44.895104 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/static/xsl/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:44.898838 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:44.902349 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:44.907458 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.210326 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1722 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/add.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/add.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:44.922196 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:44.925769 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/templates/xsl/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:44.929288 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/templates/xsl/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:44.933321 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.245998 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/add_base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1864 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/list_base.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.260614 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      788 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/modals/add.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      336 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.283005 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.334304 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3073 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      833 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      332 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.381429 core_exporters_app-2.3.0/core_exporters_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3588 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.419491 core_exporters_app-2.3.0/core_exporters_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.434989 core_exporters_app-2.3.0/core_exporters_app/rest/export/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/rest/export/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.468696 core_exporters_app-2.3.0/core_exporters_app/rest/export/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/rest/export/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6863 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/rest/export/data/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.519034 core_exporters_app-2.3.0/core_exporters_app/rest/exporters/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/rest/exporters/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1967 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/rest/exporters/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8794 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/rest/exporters/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.551182 core_exporters_app-2.3.0/core_exporters_app/rest/exporters/xsl/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/rest/exporters/xsl/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4291 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/rest/exporters/xsl/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1516 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      862 2023-05-02 19:38:38.000000 core_exporters_app-2.3.0/core_exporters_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.019615 core_exporters_app-2.3.0/core_exporters_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.063528 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.043445 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.030312 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/css/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.033991 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/css/exporters/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.580779 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/css/exporters/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      115 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/css/exporters/list/list_exporters.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.046948 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.050518 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.054447 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.645516 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2047 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/associated_templates.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      103 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/associated_templates.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.084905 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.097310 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.679628 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      962 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/download.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/download.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.100991 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/js/exporters/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.104511 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.723137 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5149 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/list_exporters_selector.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      160 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/list_exporters_selector.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.761469 core_exporters_app-2.3.0/core_exporters_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      561 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/system/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3990 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.122869 core_exporters_app-2.3.0/core_exporters_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.157407 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.141570 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.785796 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/admin/exporters/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.814595 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/associated_templates_base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1658 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/list_base.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.835118 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      907 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/modals/associated_templates.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      324 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list_exporters.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.167296 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.852836 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/user/exported_compressed_file/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      265 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/user/exported_compressed_file/download.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.170445 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/user/exporters/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.882691 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       41 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/link_exporters_selector.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       27 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/list_exporters_selector_base.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.900488 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      842 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/modals/list_exporters_selector.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      922 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.916008 core_exporters_app-2.3.0/core_exporters_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:46.980545 core_exporters_app-2.3.0/core_exporters_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3974 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1526 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1650 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.032514 core_exporters_app-2.3.0/core_exporters_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7532 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2705 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/views/user/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2122 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/core_exporters_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:45.570098 core_exporters_app-2.3.0/core_exporters_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1017 2023-05-02 19:38:41.000000 core_exporters_app-2.3.0/core_exporters_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5976 2023-05-02 19:38:42.000000 core_exporters_app-2.3.0/core_exporters_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:38:41.000000 core_exporters_app-2.3.0/core_exporters_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      132 2023-05-02 19:38:41.000000 core_exporters_app-2.3.0/core_exporters_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-05-02 19:38:41.000000 core_exporters_app-2.3.0/core_exporters_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.071624 core_exporters_app-2.3.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11096 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2023-05-02 19:38:39.000000 core_exporters_app-2.3.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       70 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:38:47.543108 core_exporters_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1393 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.110095 core_exporters_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.125423 core_exporters_app-2.3.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.183111 core_exporters_app-2.3.0/tests/components/exported_compressed_file/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/components/exported_compressed_file/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.223867 core_exporters_app-2.3.0/tests/components/exported_compressed_file/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/components/exported_compressed_file/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1744 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/components/exported_compressed_file/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6477 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/components/exported_compressed_file/tests_int.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.254604 core_exporters_app-2.3.0/tests/components/exporter/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/components/exporter/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2758 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/components/exporter/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.270594 core_exporters_app-2.3.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.342202 core_exporters_app-2.3.0/tests/rest/export/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/export/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.369024 core_exporters_app-2.3.0/tests/rest/export/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/export/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2520 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/export/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8721 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/export/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7069 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/export/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5042 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/export/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.431000 core_exporters_app-2.3.0/tests/rest/exporter/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/exporter/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.466122 core_exporters_app-2.3.0/tests/rest/exporter/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/exporter/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      877 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/exporter/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4051 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/exporter/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8034 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/exporter/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1051 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/exporter/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:47.519763 core_exporters_app-2.3.0/tests/rest/exporter/xsl/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/exporter/xsl/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5101 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/rest/exporter/xsl/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1606 2023-05-02 19:38:40.000000 core_exporters_app-2.3.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:40.167103 core_exporters_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1017 2023-07-21 02:12:40.162490 core_exporters_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      542 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:38.266024 core_exporters_app-2.4.0/core_exporters_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       93 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:38.359626 core_exporters_app-2.4.0/core_exporters_app/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      931 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/access_control/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1764 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      704 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:38.386194 core_exporters_app-2.4.0/core_exporters_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/commons/constants.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:38.399468 core_exporters_app-2.4.0/core_exporters_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:38.452623 core_exporters_app-2.4.0/core_exporters_app/components/exported_compressed_file/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/components/exported_compressed_file/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      404 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/components/exported_compressed_file/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      778 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/components/exported_compressed_file/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1365 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/components/exported_compressed_file/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:38.512099 core_exporters_app-2.4.0/core_exporters_app/components/exporter/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/components/exporter/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      318 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/components/exporter/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1537 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/components/exporter/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6984 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/components/exporter/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1451 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/components/exporter/watch.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:38.560612 core_exporters_app-2.4.0/core_exporters_app/exporters/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:38.600268 core_exporters_app-2.4.0/core_exporters_app/exporters/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/blob/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4587 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/blob/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      221 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/blob/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4576 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5910 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/exporter.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:38.637524 core_exporters_app-2.4.0/core_exporters_app/exporters/json_exporter/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/json_exporter/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2358 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/json_exporter/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      230 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/json_exporter/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      323 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:38.675222 core_exporters_app-2.4.0/core_exporters_app/exporters/xml/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:28.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/xml/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1789 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/xml/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      216 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/xml/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:38.725395 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2801 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3358 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.764849 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.767701 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/static/xsl/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.770840 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/static/xsl/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.773490 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.776495 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.779179 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:38.754086 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1722 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/add.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/add.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.803737 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.806738 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/templates/xsl/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.809514 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/templates/xsl/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.812375 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:38.782757 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/add_base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1960 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/list_base.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:38.795716 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1111 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/modals/add.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      336 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:38.808105 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:38.985540 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3073 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      833 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      332 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.009908 core_exporters_app-2.4.0/core_exporters_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3588 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.053424 core_exporters_app-2.4.0/core_exporters_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.067229 core_exporters_app-2.4.0/core_exporters_app/rest/export/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/rest/export/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.095826 core_exporters_app-2.4.0/core_exporters_app/rest/export/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/rest/export/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6863 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/rest/export/data/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.135547 core_exporters_app-2.4.0/core_exporters_app/rest/exporters/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/rest/exporters/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1967 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/rest/exporters/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8794 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/rest/exporters/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.178723 core_exporters_app-2.4.0/core_exporters_app/rest/exporters/xsl/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/rest/exporters/xsl/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4291 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/rest/exporters/xsl/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1516 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      862 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.859711 core_exporters_app-2.4.0/core_exporters_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.913986 core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.898877 core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.875741 core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/admin/css/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.889962 core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/admin/css/exporters/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.204554 core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/admin/css/exporters/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      115 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/admin/css/exporters/list/list_exporters.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.901890 core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/admin/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.904507 core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.907397 core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.240708 core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1990 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/associated_templates.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      103 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/associated_templates.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.917174 core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.927085 core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/user/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.275569 core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      962 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/download.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2023-07-21 02:12:29.000000 core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/download.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.930136 core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/user/js/exporters/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.932833 core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.302821 core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5149 2023-07-21 02:12:33.000000 core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/list_exporters_selector.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      160 2023-07-21 02:12:33.000000 core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/list_exporters_selector.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.327146 core_exporters_app-2.4.0/core_exporters_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:33.000000 core_exporters_app-2.4.0/core_exporters_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      561 2023-07-21 02:12:33.000000 core_exporters_app-2.4.0/core_exporters_app/system/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3990 2023-07-21 02:12:33.000000 core_exporters_app-2.4.0/core_exporters_app/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.945618 core_exporters_app-2.4.0/core_exporters_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.977677 core_exporters_app-2.4.0/core_exporters_app/templates/core_exporters_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.963098 core_exporters_app-2.4.0/core_exporters_app/templates/core_exporters_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.344934 core_exporters_app-2.4.0/core_exporters_app/templates/core_exporters_app/admin/exporters/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.390776 core_exporters_app-2.4.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      338 2023-07-21 02:12:33.000000 core_exporters_app-2.4.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/associated_templates_base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1620 2023-07-21 02:12:33.000000 core_exporters_app-2.4.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/list_base.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.405078 core_exporters_app-2.4.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1171 2023-07-21 02:12:33.000000 core_exporters_app-2.4.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/modals/associated_templates.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      324 2023-07-21 02:12:34.000000 core_exporters_app-2.4.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list_exporters.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.985908 core_exporters_app-2.4.0/core_exporters_app/templates/core_exporters_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.420286 core_exporters_app-2.4.0/core_exporters_app/templates/core_exporters_app/user/exported_compressed_file/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      265 2023-07-21 02:12:34.000000 core_exporters_app-2.4.0/core_exporters_app/templates/core_exporters_app/user/exported_compressed_file/download.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:37.988981 core_exporters_app-2.4.0/core_exporters_app/templates/core_exporters_app/user/exporters/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.446350 core_exporters_app-2.4.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       41 2023-07-21 02:12:34.000000 core_exporters_app-2.4.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/link_exporters_selector.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       27 2023-07-21 02:12:34.000000 core_exporters_app-2.4.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/list_exporters_selector_base.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.458165 core_exporters_app-2.4.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1127 2023-07-21 02:12:34.000000 core_exporters_app-2.4.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/modals/list_exporters_selector.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      922 2023-07-21 02:12:34.000000 core_exporters_app-2.4.0/core_exporters_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.471611 core_exporters_app-2.4.0/core_exporters_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:34.000000 core_exporters_app-2.4.0/core_exporters_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.549405 core_exporters_app-2.4.0/core_exporters_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:34.000000 core_exporters_app-2.4.0/core_exporters_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3974 2023-07-21 02:12:34.000000 core_exporters_app-2.4.0/core_exporters_app/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1526 2023-07-21 02:12:34.000000 core_exporters_app-2.4.0/core_exporters_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1650 2023-07-21 02:12:34.000000 core_exporters_app-2.4.0/core_exporters_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.607178 core_exporters_app-2.4.0/core_exporters_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:34.000000 core_exporters_app-2.4.0/core_exporters_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7532 2023-07-21 02:12:34.000000 core_exporters_app-2.4.0/core_exporters_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2705 2023-07-21 02:12:34.000000 core_exporters_app-2.4.0/core_exporters_app/views/user/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2122 2023-07-21 02:12:34.000000 core_exporters_app-2.4.0/core_exporters_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:38.332420 core_exporters_app-2.4.0/core_exporters_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1017 2023-07-21 02:12:37.000000 core_exporters_app-2.4.0/core_exporters_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5976 2023-07-21 02:12:37.000000 core_exporters_app-2.4.0/core_exporters_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:12:37.000000 core_exporters_app-2.4.0/core_exporters_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      132 2023-07-21 02:12:37.000000 core_exporters_app-2.4.0/core_exporters_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-07-21 02:12:37.000000 core_exporters_app-2.4.0/core_exporters_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.649698 core_exporters_app-2.4.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:34.000000 core_exporters_app-2.4.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11096 2023-07-21 02:12:34.000000 core_exporters_app-2.4.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2023-07-21 02:12:34.000000 core_exporters_app-2.4.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       70 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:12:40.168683 core_exporters_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1393 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.679803 core_exporters_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.737774 core_exporters_app-2.4.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.797661 core_exporters_app-2.4.0/tests/components/exported_compressed_file/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/components/exported_compressed_file/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.840132 core_exporters_app-2.4.0/tests/components/exported_compressed_file/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/components/exported_compressed_file/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1744 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/components/exported_compressed_file/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6477 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/components/exported_compressed_file/tests_int.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.882581 core_exporters_app-2.4.0/tests/components/exporter/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/components/exporter/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2758 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/components/exporter/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.896221 core_exporters_app-2.4.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.956575 core_exporters_app-2.4.0/tests/rest/export/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/rest/export/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:39.985552 core_exporters_app-2.4.0/tests/rest/export/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/rest/export/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2520 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/rest/export/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8721 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/rest/export/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7069 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/rest/export/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5042 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/rest/export/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:40.068065 core_exporters_app-2.4.0/tests/rest/exporter/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/rest/exporter/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:40.097651 core_exporters_app-2.4.0/tests/rest/exporter/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/rest/exporter/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      877 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/rest/exporter/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4051 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/rest/exporter/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8034 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/rest/exporter/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1051 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/rest/exporter/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:40.129199 core_exporters_app-2.4.0/tests/rest/exporter/xsl/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/rest/exporter/xsl/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5101 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/rest/exporter/xsl/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1606 2023-07-21 02:12:35.000000 core_exporters_app-2.4.0/tests/test_settings.py
```

### Comparing `core_exporters_app-2.3.0/LICENSE.md` & `core_exporters_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/PKG-INFO` & `core_exporters_app-2.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_exporters_app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Exporters for the curator core project
 Home-page: https://github.com/usnistgov/core_exporters_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ==================
         Core Exporters App
```

### Comparing `core_exporters_app-2.3.0/README.rst` & `core_exporters_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/access_control/api.py` & `core_exporters_app-2.4.0/core_exporters_app/access_control/api.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/admin.py` & `core_exporters_app-2.4.0/core_exporters_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/apps.py` & `core_exporters_app-2.4.0/core_exporters_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/components/exported_compressed_file/api.py` & `core_exporters_app-2.4.0/core_exporters_app/components/exported_compressed_file/api.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/components/exported_compressed_file/models.py` & `core_exporters_app-2.4.0/core_exporters_app/components/exported_compressed_file/models.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/components/exporter/api.py` & `core_exporters_app-2.4.0/core_exporters_app/components/exporter/api.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/components/exporter/models.py` & `core_exporters_app-2.4.0/core_exporters_app/components/exporter/models.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/components/exporter/watch.py` & `core_exporters_app-2.4.0/core_exporters_app/components/exporter/watch.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/exporters/blob/models.py` & `core_exporters_app-2.4.0/core_exporters_app/exporters/blob/models.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/exporters/discover.py` & `core_exporters_app-2.4.0/core_exporters_app/exporters/discover.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/exporters/exporter.py` & `core_exporters_app-2.4.0/core_exporters_app/exporters/exporter.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/exporters/json_exporter/models.py` & `core_exporters_app-2.4.0/core_exporters_app/exporters/json_exporter/models.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/exporters/xml/models.py` & `core_exporters_app-2.4.0/core_exporters_app/exporters/xml/models.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/api.py` & `core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/api.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/models.py` & `core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/models.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/add.js` & `core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/add.js`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/list_base.html` & `core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/list_base.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %}
 
 {% block box_title %}
     XSLT Exporters
 {% endblock %}
 
 {% block box_tools %}
-<div class="btn-group float-right">
+<div class="btn-group {% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}">
     <a href="#" class="btn btn-secondary btn-add-xslt-exporter">
         <i class="fas fa-cog"></i> Manage
     </a>
 </div>
 {% endblock %}
 
 {% block box_body %}
```

#### html2text {}

```diff
@@ -1,9 +1,11 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% block
 box_title %} XSLT Exporters {% endblock %} {% block box_tools %}
+.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif
+%}">
  Manage
 {% endblock %} {% block box_body %}
 Exporter Name Associated XSLT                  Associated Templates             Actions
                                                                                 {% block box_actions %} {% url 'core-
                                                                                 admin:
 {             {                                {                                core_exporters_app_exporters_xsl_edit'
 {             {                                {                                exporter.id as edit_url %} {% include
```

### Comparing `core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/views/admin/ajax.py` & `core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/views/admin/ajax.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/exporters/xsl/views/admin/forms.py` & `core_exporters_app-2.4.0/core_exporters_app/exporters/xsl/views/admin/forms.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/migrations/0001_initial.py` & `core_exporters_app-2.4.0/core_exporters_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/rest/export/data/views.py` & `core_exporters_app-2.4.0/core_exporters_app/rest/export/data/views.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/rest/exporters/serializers.py` & `core_exporters_app-2.4.0/core_exporters_app/rest/exporters/serializers.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/rest/exporters/views.py` & `core_exporters_app-2.4.0/core_exporters_app/rest/exporters/views.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/rest/exporters/xsl/views.py` & `core_exporters_app-2.4.0/core_exporters_app/rest/exporters/xsl/views.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/rest/urls.py` & `core_exporters_app-2.4.0/core_exporters_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/settings.py` & `core_exporters_app-2.4.0/core_exporters_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/associated_templates.js` & `core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/associated_templates.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -27,20 +27,19 @@
             'exporter_id': exporterId
         },
         success: function(data) {
             $("#banner_errors").hide();
             $("#form-associated-template-content").html(data.template);
         },
         error: function(data) {
-            if (data.responseText != "") {
-                $("#form_associated_templates_errors").html(data.responseText);
-                $("#banner_errors").show(500);
-                return (false);
-            }
-            return (true);
+            if (data.responseText === "")
+                return
+
+            $("#form_associated_templates_errors").html(data.responseText);
+            $("#banner_errors").show(500);
         }
     });
 };
 
 /**
  * AJAX call, submit associated templates
  */
```

### Comparing `core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/download.js` & `core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/download.js`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/list_exporters_selector.js` & `core_exporters_app-2.4.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/list_exporters_selector.js`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/system/api.py` & `core_exporters_app-2.4.0/core_exporters_app/system/api.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/tasks.py` & `core_exporters_app-2.4.0/core_exporters_app/tasks.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/list_base.html` & `core_exporters_app-2.4.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/list_base.html`

 * *Files 8% similar despite different names*

```diff
@@ -36,10 +36,7 @@
                 </tr>
             {% endfor %}
         </table>
     </div>
 </div>
 
 {% endblock %}
-
-{% block box_footer %}
-{% endblock %}
```

#### html2text {}

```diff
@@ -6,8 +6,8 @@
 {             {                                core_exporters_app_exporters_edit'
 {             {                                exporter.id as edit_url %} {%
 exporter.name exporter.get_templates_to_string include 'core_main_app/common/
 }}            }}                               buttons/edit.html' %}
                                                 Templates_mapping
                                                  {% endblock %}
 No exporters registered.
-{% endblock %} {% block box_footer %} {% endblock %}
+{% endblock %}
```

### Comparing `core_exporters_app-2.3.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/modals/associated_templates.html` & `core_exporters_app-2.4.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/modals/associated_templates.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 {% extends 'core_main_app/_render/admin/theme/tools/modal.html' %}
 
 {% block modal_id %}select-associated-template-modal{% endblock %}
-{% block modal_title %}Associated template selection{% endblock %}
+{% block modal_title %}Select associated templates{% endblock %}
 
 {% block modal_body %}
 <div class="alert alert-danger" id="banner_errors" style="display: none;">
-        <a href="#" class="close" data-hide="alert" aria-label="close">&times;</a>
-     	<h4><i class="fas fa-exclamation-circle"></i> Error</h4>
-        <div id="form_associated_templates_errors">
+    <a href="#"
+       class="{% if BOOTSTRAP_VERSION == "4.6.2" %}close
+            {% elif BOOTSTRAP_VERSION == "5.1.3" %}btn-close
+            {% endif %}"
+       data-hide="alert" aria-label="close">{% if BOOTSTRAP_VERSION == "4.6.2" %}&times;{% elif BOOTSTRAP_VERSION == "5.1.3" %}{% endif %}</a>
+    <h4><i class="fas fa-exclamation-circle"></i> Error</h4>
+    <div id="form_associated_templates_errors"></div>
 </div>
-</div>
-<div class="clearer"><h5>Select templates:</h5></div>
 <form id="form-associated-template-content" method="post">
 </form>
 {% endblock %}
 
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
+<a class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#">
+    <i class="fas fa-times"></i> Cancel
+</a>
 <button id="btn-associated-templates-save" class="btn btn-primary"><i class="fas fa-save"></i> Save</button>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,9 +1,11 @@
 {% extends 'core_main_app/_render/admin/theme/tools/modal.html' %} {% block
 modal_id %}select-associated-template-modal{% endblock %} {% block modal_title
-%}Associated template selection{% endblock %} {% block modal_body %}
-×
+%}Select associated templates{% endblock %} {% block modal_body %}
+.6.2" %}close {% elif BOOTSTRAP_VERSION == "5.1.3" %}btn-close {% endif %}"
+data-hide="alert" aria-label="close">{% if BOOTSTRAP_VERSION == "4.6.2" %}×{%
+elif BOOTSTRAP_VERSION == "5.1.3" %}{% endif %}
  Error
-** Select templates: **
 {% endblock %} {% block modal_footer %}
- Cancel
+% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION ==
+"5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#">  Cancel
   Save {% endblock %}
```

### Comparing `core_exporters_app-2.3.0/core_exporters_app/urls.py` & `core_exporters_app-2.4.0/core_exporters_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/views/admin/ajax.py` & `core_exporters_app-2.4.0/core_exporters_app/views/admin/ajax.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/views/admin/forms.py` & `core_exporters_app-2.4.0/core_exporters_app/views/admin/forms.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/views/admin/views.py` & `core_exporters_app-2.4.0/core_exporters_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/views/user/ajax.py` & `core_exporters_app-2.4.0/core_exporters_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/views/user/forms.py` & `core_exporters_app-2.4.0/core_exporters_app/views/user/forms.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app/views/user/views.py` & `core_exporters_app-2.4.0/core_exporters_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/core_exporters_app.egg-info/PKG-INFO` & `core_exporters_app-2.4.0/core_exporters_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-exporters-app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Exporters for the curator core project
 Home-page: https://github.com/usnistgov/core_exporters_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ==================
         Core Exporters App
```

### Comparing `core_exporters_app-2.3.0/core_exporters_app.egg-info/SOURCES.txt` & `core_exporters_app-2.4.0/core_exporters_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/docs/conf.py` & `core_exporters_app-2.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/setup.py` & `core_exporters_app-2.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_exporters_app",
-    version="2.3.0",
+    version="2.4.0",
     description="Exporters for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_exporters_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_exporters_app-2.3.0/tests/components/exported_compressed_file/fixtures/fixtures.py` & `core_exporters_app-2.4.0/tests/components/exported_compressed_file/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/tests/components/exported_compressed_file/tests_int.py` & `core_exporters_app-2.4.0/tests/components/exported_compressed_file/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/tests/components/exporter/tests_unit.py` & `core_exporters_app-2.4.0/tests/components/exporter/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/tests/rest/export/fixtures/fixtures.py` & `core_exporters_app-2.4.0/tests/rest/export/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/tests/rest/export/tests_int.py` & `core_exporters_app-2.4.0/tests/rest/export/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/tests/rest/export/tests_permissions.py` & `core_exporters_app-2.4.0/tests/rest/export/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/tests/rest/export/tests_unit.py` & `core_exporters_app-2.4.0/tests/rest/export/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/tests/rest/exporter/fixtures/fixtures.py` & `core_exporters_app-2.4.0/tests/rest/exporter/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/tests/rest/exporter/tests_int.py` & `core_exporters_app-2.4.0/tests/rest/exporter/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/tests/rest/exporter/tests_permissions.py` & `core_exporters_app-2.4.0/tests/rest/exporter/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/tests/rest/exporter/tests_unit.py` & `core_exporters_app-2.4.0/tests/rest/exporter/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/tests/rest/exporter/xsl/tests_permissions.py` & `core_exporters_app-2.4.0/tests/rest/exporter/xsl/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.3.0/tests/test_settings.py` & `core_exporters_app-2.4.0/tests/test_settings.py`

 * *Files identical despite different names*

