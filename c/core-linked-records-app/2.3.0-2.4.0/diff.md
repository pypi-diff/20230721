# Comparing `tmp/core_linked_records_app-2.3.0.tar.gz` & `tmp/core_linked_records_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_linked_records_app-2.3.0.tar", last modified: Tue May  2 19:39:28 2023, max compression
+gzip compressed data, was "core_linked_records_app-2.4.0.tar", last modified: Fri Jul 21 02:13:16 2023, max compression
```

## Comparing `core_linked_records_app-2.3.0.tar` & `core_linked_records_app-2.4.0.tar`

### file list

```diff
@@ -1,286 +1,295 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:28.227119 core_linked_records_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      179 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6496 2023-05-02 19:39:28.222294 core_linked_records_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4718 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.115064 core_linked_records_app-2.3.0/core_linked_records_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      122 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1226 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1065 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.208337 core_linked_records_app-2.3.0/core_linked_records_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.252329 core_linked_records_app-2.3.0/core_linked_records_app/components/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/blob/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4188 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/blob/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2418 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/blob/watch.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.306026 core_linked_records_app-2.3.0/core_linked_records_app/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3595 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/data/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4243 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/data/watch.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.359090 core_linked_records_app-2.3.0/core_linked_records_app/components/local_id/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/local_id/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      428 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/local_id/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2187 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/local_id/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2604 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/local_id/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.385063 core_linked_records_app-2.3.0/core_linked_records_app/components/oai_record/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:19.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/oai_record/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1279 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/oai_record/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.455077 core_linked_records_app-2.3.0/core_linked_records_app/components/pid_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/pid_settings/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      433 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/pid_settings/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/pid_settings/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      890 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/pid_settings/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      622 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/pid_settings/watch.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.529376 core_linked_records_app-2.3.0/core_linked_records_app/components/pid_xpath/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/pid_xpath/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      191 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/pid_xpath/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1892 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/pid_xpath/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1951 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/components/pid_xpath/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      470 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.575147 core_linked_records_app-2.3.0/core_linked_records_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2800 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      659 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/migrations/0002_alter_pidxpath_xpath.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.606323 core_linked_records_app-2.3.0/core_linked_records_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.635729 core_linked_records_app-2.3.0/core_linked_records_app/rest/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/blob/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2526 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/blob/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.651714 core_linked_records_app-2.3.0/core_linked_records_app/rest/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/data/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.713657 core_linked_records_app-2.3.0/core_linked_records_app/rest/data/renderers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/data/renderers/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2971 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/data/renderers/data_html_user_renderer.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      948 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/data/renderers/data_xml_renderer.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.755447 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      467 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8298 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.800353 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid_settings/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      817 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid_settings/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2887 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid_settings/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.846637 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid_xpath/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid_xpath/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      349 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid_xpath/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      841 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/pid_xpath/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.877340 core_linked_records_app-2.3.0/core_linked_records_app/rest/providers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/providers/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7677 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/providers/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.908985 core_linked_records_app-2.3.0/core_linked_records_app/rest/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      736 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/query/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1925 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1634 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:24.576120 core_linked_records_app-2.3.0/core_linked_records_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:24.598407 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:24.589299 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.935042 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/admin/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       72 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/admin/css/pid_settings.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:24.592436 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/admin/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.954529 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/admin/js/pid_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1694 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/admin/js/pid_settings/auto_set_pid.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:24.607542 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.976717 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       43 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/css/sharing.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:24.610830 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.122574 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      494 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/blob_list.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/blob_list.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      735 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/common_list.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1199 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_detail.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      236 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_detail.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      494 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_list.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_list.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1309 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/explore.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/explore.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.154545 core_linked_records_app-2.3.0/core_linked_records_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7189 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/system/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:24.627300 core_linked_records_app-2.3.0/core_linked_records_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:24.641805 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.184045 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.197983 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2320 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings/box.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      233 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      290 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings_error.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:24.644788 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:24.665981 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.254051 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      253 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/button.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      236 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/button_inline.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/modal.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.280155 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/explore/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      246 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/explore/button.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      298 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/explore/modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.405423 core_linked_records_app-2.3.0/core_linked_records_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1536 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/utils/blob.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1941 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/utils/data.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1835 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/utils/dict.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      661 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/utils/path.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1023 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/utils/pid.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.453705 core_linked_records_app-2.3.0/core_linked_records_app/utils/providers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6104 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/utils/providers/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4747 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/utils/providers/handle_net.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4802 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/utils/providers/local.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4914 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/utils/query.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4076 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/utils/xml.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.476506 core_linked_records_app-2.3.0/core_linked_records_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.512771 core_linked_records_app-2.3.0/core_linked_records_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3675 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/core_linked_records_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:25.184388 core_linked_records_app-2.3.0/core_linked_records_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6496 2023-05-02 19:39:23.000000 core_linked_records_app-2.3.0/core_linked_records_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8645 2023-05-02 19:39:24.000000 core_linked_records_app-2.3.0/core_linked_records_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:39:23.000000 core_linked_records_app-2.3.0/core_linked_records_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      137 2023-05-02 19:39:23.000000 core_linked_records_app-2.3.0/core_linked_records_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-05-02 19:39:23.000000 core_linked_records_app-2.3.0/core_linked_records_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       70 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       67 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:39:28.229171 core_linked_records_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1034 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.596362 core_linked_records_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       49 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.613737 core_linked_records_app-2.3.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.635324 core_linked_records_app-2.3.0/tests/components/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/tests/components/blob/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.670905 core_linked_records_app-2.3.0/tests/components/blob/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:20.000000 core_linked_records_app-2.3.0/tests/components/blob/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12750 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/blob/api/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.709830 core_linked_records_app-2.3.0/tests/components/blob/watch/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/blob/watch/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9762 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/blob/watch/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.727610 core_linked_records_app-2.3.0/tests/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/data/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.764941 core_linked_records_app-2.3.0/tests/components/data/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/data/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10274 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/data/api/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.798326 core_linked_records_app-2.3.0/tests/components/data/watch/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/data/watch/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    22092 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/data/watch/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.815207 core_linked_records_app-2.3.0/tests/components/local_id/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/local_id/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.849540 core_linked_records_app-2.3.0/tests/components/local_id/admin_site/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/local_id/admin_site/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      953 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/local_id/admin_site/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.887421 core_linked_records_app-2.3.0/tests/components/local_id/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/local_id/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3614 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/local_id/api/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.921313 core_linked_records_app-2.3.0/tests/components/local_id/models/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/local_id/models/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4057 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/local_id/models/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.935161 core_linked_records_app-2.3.0/tests/components/oai_record/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/oai_record/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.968820 core_linked_records_app-2.3.0/tests/components/oai_record/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/oai_record/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3030 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/oai_record/api/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:26.985958 core_linked_records_app-2.3.0/tests/components/pid_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_settings/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.024124 core_linked_records_app-2.3.0/tests/components/pid_settings/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_settings/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1760 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_settings/api/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.053716 core_linked_records_app-2.3.0/tests/components/pid_settings/models/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_settings/models/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1460 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_settings/models/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.087232 core_linked_records_app-2.3.0/tests/components/pid_settings/watch/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_settings/watch/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2765 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_settings/watch/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.103301 core_linked_records_app-2.3.0/tests/components/pid_xpath/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_xpath/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.139390 core_linked_records_app-2.3.0/tests/components/pid_xpath/admin_site/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_xpath/admin_site/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      566 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_xpath/admin_site/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.181995 core_linked_records_app-2.3.0/tests/components/pid_xpath/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_xpath/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4208 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_xpath/api/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.216184 core_linked_records_app-2.3.0/tests/components/pid_xpath/models/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_xpath/models/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3121 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/components/pid_xpath/models/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.250423 core_linked_records_app-2.3.0/tests/menus/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/menus/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      553 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/menus/test_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4156 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/mocks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.266520 core_linked_records_app-2.3.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.286261 core_linked_records_app-2.3.0/tests/rest/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/blob/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.335153 core_linked_records_app-2.3.0/tests/rest/blob/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/blob/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2639 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/blob/views/test_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5112 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/blob/views/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.351067 core_linked_records_app-2.3.0/tests/rest/pid/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/pid/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.402748 core_linked_records_app-2.3.0/tests/rest/pid/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/pid/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6123 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/pid/views/test_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17555 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/pid/views/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.429129 core_linked_records_app-2.3.0/tests/rest/pid_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/pid_settings/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.477747 core_linked_records_app-2.3.0/tests/rest/pid_settings/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/pid_settings/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4244 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/pid_settings/views/test_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5951 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/pid_settings/views/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.493114 core_linked_records_app-2.3.0/tests/rest/pid_xpath/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/pid_xpath/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.528400 core_linked_records_app-2.3.0/tests/rest/pid_xpath/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/pid_xpath/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7569 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/pid_xpath/views/test_permissions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.551046 core_linked_records_app-2.3.0/tests/rest/providers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/providers/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.605512 core_linked_records_app-2.3.0/tests/rest/providers/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/providers/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8187 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/providers/views/test_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17141 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/providers/views/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.638936 core_linked_records_app-2.3.0/tests/rest/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1800 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/rest/query/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.652699 core_linked_records_app-2.3.0/tests/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/system/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.685107 core_linked_records_app-2.3.0/tests/system/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/system/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20646 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/system/api/test_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2144 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      458 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/test_urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.702196 core_linked_records_app-2.3.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.815261 core_linked_records_app-2.3.0/tests/utils/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/blob/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      421 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/blob/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.852419 core_linked_records_app-2.3.0/tests/utils/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      421 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/data/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.888752 core_linked_records_app-2.3.0/tests/utils/dict/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/dict/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4213 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/dict/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.927013 core_linked_records_app-2.3.0/tests/utils/path/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/path/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      378 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/path/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.961397 core_linked_records_app-2.3.0/tests/utils/pid/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/pid/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2298 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/pid/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:27.980514 core_linked_records_app-2.3.0/tests/utils/providers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/providers/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:28.021821 core_linked_records_app-2.3.0/tests/utils/providers/handle_net/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/providers/handle_net/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3952 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/providers/handle_net/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:28.057372 core_linked_records_app-2.3.0/tests/utils/providers/local/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/providers/local/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12238 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/providers/local/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:28.092097 core_linked_records_app-2.3.0/tests/utils/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9314 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/query/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:28.122598 core_linked_records_app-2.3.0/tests/utils/xml/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/xml/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1454 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/utils/xml/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:28.142178 core_linked_records_app-2.3.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:21.000000 core_linked_records_app-2.3.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:28.160730 core_linked_records_app-2.3.0/tests/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:22.000000 core_linked_records_app-2.3.0/tests/views/admin/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:28.204247 core_linked_records_app-2.3.0/tests/views/admin/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:22.000000 core_linked_records_app-2.3.0/tests/views/admin/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6799 2023-05-02 19:39:22.000000 core_linked_records_app-2.3.0/tests/views/admin/views/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:16.017545 core_linked_records_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      179 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6496 2023-07-21 02:13:16.013389 core_linked_records_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4718 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:07.353984 core_linked_records_app-2.4.0/core_linked_records_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      122 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1226 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1065 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:07.452133 core_linked_records_app-2.4.0/core_linked_records_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:07.489599 core_linked_records_app-2.4.0/core_linked_records_app/components/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/components/blob/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4389 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/components/blob/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2833 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/components/blob/watch.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:07.581935 core_linked_records_app-2.4.0/core_linked_records_app/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/components/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3595 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/components/data/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4624 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/components/data/watch.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:07.630089 core_linked_records_app-2.4.0/core_linked_records_app/components/local_id/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/components/local_id/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      428 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/components/local_id/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2187 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/components/local_id/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2604 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/components/local_id/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:07.706356 core_linked_records_app-2.4.0/core_linked_records_app/components/oai_record/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/components/oai_record/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1279 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/components/oai_record/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:07.802693 core_linked_records_app-2.4.0/core_linked_records_app/components/pid_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/components/pid_settings/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      433 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/components/pid_settings/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/components/pid_settings/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      890 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/components/pid_settings/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      622 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/components/pid_settings/watch.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:07.860180 core_linked_records_app-2.4.0/core_linked_records_app/components/pid_xpath/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/components/pid_xpath/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      191 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/components/pid_xpath/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1892 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/components/pid_xpath/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1951 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/components/pid_xpath/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      470 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:07.895376 core_linked_records_app-2.4.0/core_linked_records_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2800 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      659 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/migrations/0002_alter_pidxpath_xpath.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:02.000000 core_linked_records_app-2.4.0/core_linked_records_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:07.926828 core_linked_records_app-2.4.0/core_linked_records_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:07.963513 core_linked_records_app-2.4.0/core_linked_records_app/rest/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/rest/blob/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2526 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/rest/blob/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:07.978268 core_linked_records_app-2.4.0/core_linked_records_app/rest/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/rest/data/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.030437 core_linked_records_app-2.4.0/core_linked_records_app/rest/data/renderers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/rest/data/renderers/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3495 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/rest/data/renderers/data_html_user_renderer.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      948 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/rest/data/renderers/data_xml_renderer.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.078497 core_linked_records_app-2.4.0/core_linked_records_app/rest/pid/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/rest/pid/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      467 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/rest/pid/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8298 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/rest/pid/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.118944 core_linked_records_app-2.4.0/core_linked_records_app/rest/pid_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/rest/pid_settings/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      817 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/rest/pid_settings/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2464 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/rest/pid_settings/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.148533 core_linked_records_app-2.4.0/core_linked_records_app/rest/pid_xpath/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/rest/pid_xpath/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      349 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/rest/pid_xpath/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      841 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/rest/pid_xpath/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.182098 core_linked_records_app-2.4.0/core_linked_records_app/rest/providers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/rest/providers/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7695 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/rest/providers/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.203480 core_linked_records_app-2.4.0/core_linked_records_app/rest/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/rest/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      736 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/rest/query/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1926 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1624 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:06.839120 core_linked_records_app-2.4.0/core_linked_records_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:06.887150 core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:06.880174 core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.219820 core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/admin/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       72 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/admin/css/pid_settings.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:06.882747 core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/admin/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.235527 core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/admin/js/pid_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1683 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/admin/js/pid_settings/auto_set_pid.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:06.893514 core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.247320 core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       43 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/user/css/sharing.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:06.895802 core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/user/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.379120 core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      494 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/blob_list.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/blob_list.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      735 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/common_list.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1199 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_detail.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      236 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_detail.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      494 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_list.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_list.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1309 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/explore.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/explore.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.402361 core_linked_records_app-2.4.0/core_linked_records_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7542 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/system/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:06.905174 core_linked_records_app-2.4.0/core_linked_records_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:06.915475 core_linked_records_app-2.4.0/core_linked_records_app/templates/core_linked_records_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.439555 core_linked_records_app-2.4.0/core_linked_records_app/templates/core_linked_records_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.450142 core_linked_records_app-2.4.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3073 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings/box.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      233 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      290 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings_error.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:06.918077 core_linked_records_app-2.4.0/core_linked_records_app/templates/core_linked_records_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:06.924697 core_linked_records_app-2.4.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.488548 core_linked_records_app-2.4.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      354 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/button.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      236 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/button_inline.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/modal.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.518985 core_linked_records_app-2.4.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/explore/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      246 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/explore/button.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      298 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/explore/modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.639918 core_linked_records_app-2.4.0/core_linked_records_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1536 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/utils/blob.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1941 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/utils/data.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1835 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/utils/dict.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      661 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/utils/path.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1638 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/utils/pid.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.672650 core_linked_records_app-2.4.0/core_linked_records_app/utils/providers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6104 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/utils/providers/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4747 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/utils/providers/handle_net.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4812 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/utils/providers/local.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4914 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/utils/query.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4076 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/utils/xml.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.685390 core_linked_records_app-2.4.0/core_linked_records_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.713634 core_linked_records_app-2.4.0/core_linked_records_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2894 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/core_linked_records_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:07.420096 core_linked_records_app-2.4.0/core_linked_records_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6496 2023-07-21 02:13:06.000000 core_linked_records_app-2.4.0/core_linked_records_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8905 2023-07-21 02:13:06.000000 core_linked_records_app-2.4.0/core_linked_records_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:13:06.000000 core_linked_records_app-2.4.0/core_linked_records_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      137 2023-07-21 02:13:06.000000 core_linked_records_app-2.4.0/core_linked_records_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-07-21 02:13:06.000000 core_linked_records_app-2.4.0/core_linked_records_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       70 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       67 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:13:16.019228 core_linked_records_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1034 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.764480 core_linked_records_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       49 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.775819 core_linked_records_app-2.4.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.787368 core_linked_records_app-2.4.0/tests/components/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/blob/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.811099 core_linked_records_app-2.4.0/tests/components/blob/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/blob/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13683 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/blob/api/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.834271 core_linked_records_app-2.4.0/tests/components/blob/watch/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/blob/watch/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9762 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/blob/watch/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.863706 core_linked_records_app-2.4.0/tests/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/data/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.926110 core_linked_records_app-2.4.0/tests/components/data/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/data/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10274 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/data/api/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.954237 core_linked_records_app-2.4.0/tests/components/data/watch/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/data/watch/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17664 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/data/watch/tests_integration.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    22092 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/data/watch/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.965286 core_linked_records_app-2.4.0/tests/components/local_id/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/local_id/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:08.984060 core_linked_records_app-2.4.0/tests/components/local_id/admin_site/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/local_id/admin_site/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      953 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/local_id/admin_site/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:09.006981 core_linked_records_app-2.4.0/tests/components/local_id/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/local_id/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3614 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/local_id/api/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:09.669571 core_linked_records_app-2.4.0/tests/components/local_id/models/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/local_id/models/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4057 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/local_id/models/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:09.684044 core_linked_records_app-2.4.0/tests/components/oai_record/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/oai_record/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:09.717683 core_linked_records_app-2.4.0/tests/components/oai_record/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/oai_record/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3030 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/oai_record/api/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:09.733631 core_linked_records_app-2.4.0/tests/components/pid_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/pid_settings/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:12.181582 core_linked_records_app-2.4.0/tests/components/pid_settings/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/pid_settings/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1760 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/pid_settings/api/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:12.215376 core_linked_records_app-2.4.0/tests/components/pid_settings/models/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/pid_settings/models/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1460 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/pid_settings/models/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:13.661457 core_linked_records_app-2.4.0/tests/components/pid_settings/watch/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/pid_settings/watch/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2765 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/pid_settings/watch/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:14.837596 core_linked_records_app-2.4.0/tests/components/pid_xpath/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/pid_xpath/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:14.869388 core_linked_records_app-2.4.0/tests/components/pid_xpath/admin_site/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/pid_xpath/admin_site/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      566 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/pid_xpath/admin_site/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:14.896854 core_linked_records_app-2.4.0/tests/components/pid_xpath/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/pid_xpath/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4208 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/pid_xpath/api/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:14.926080 core_linked_records_app-2.4.0/tests/components/pid_xpath/models/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/pid_xpath/models/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3121 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/components/pid_xpath/models/test_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2263 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/fixtures.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:14.951929 core_linked_records_app-2.4.0/tests/menus/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/menus/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      553 2023-07-21 02:13:03.000000 core_linked_records_app-2.4.0/tests/menus/test_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4156 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/mocks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:14.964100 core_linked_records_app-2.4.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:14.981766 core_linked_records_app-2.4.0/tests/rest/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/blob/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.033687 core_linked_records_app-2.4.0/tests/rest/blob/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/blob/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2639 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/blob/views/test_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5112 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/blob/views/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.046248 core_linked_records_app-2.4.0/tests/rest/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/data/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.091429 core_linked_records_app-2.4.0/tests/rest/data/renderers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/data/renderers/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.132229 core_linked_records_app-2.4.0/tests/rest/data/renderers/data_html_user_renderer/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/data/renderers/data_html_user_renderer/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1247 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/data/renderers/data_html_user_renderer/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.146801 core_linked_records_app-2.4.0/tests/rest/pid/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/pid/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.194326 core_linked_records_app-2.4.0/tests/rest/pid/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/pid/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6123 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/pid/views/test_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17555 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/pid/views/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.226299 core_linked_records_app-2.4.0/tests/rest/pid_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/pid_settings/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.273390 core_linked_records_app-2.4.0/tests/rest/pid_settings/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/pid_settings/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4248 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/pid_settings/views/test_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5818 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/pid_settings/views/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.294659 core_linked_records_app-2.4.0/tests/rest/pid_xpath/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/pid_xpath/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.329887 core_linked_records_app-2.4.0/tests/rest/pid_xpath/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/pid_xpath/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7569 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/pid_xpath/views/test_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.345468 core_linked_records_app-2.4.0/tests/rest/providers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/providers/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.395100 core_linked_records_app-2.4.0/tests/rest/providers/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/providers/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8187 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/providers/views/test_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17141 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/providers/views/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.422330 core_linked_records_app-2.4.0/tests/rest/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1800 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/rest/query/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.437821 core_linked_records_app-2.4.0/tests/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/system/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.503639 core_linked_records_app-2.4.0/tests/system/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/system/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20646 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/system/api/test_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2157 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      458 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/test_urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.519341 core_linked_records_app-2.4.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.590719 core_linked_records_app-2.4.0/tests/utils/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/utils/blob/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      421 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/utils/blob/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.619863 core_linked_records_app-2.4.0/tests/utils/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/utils/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      421 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/utils/data/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.649167 core_linked_records_app-2.4.0/tests/utils/dict/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/utils/dict/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4213 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/utils/dict/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.680748 core_linked_records_app-2.4.0/tests/utils/path/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/utils/path/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      378 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/utils/path/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.713495 core_linked_records_app-2.4.0/tests/utils/pid/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/utils/pid/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2298 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/utils/pid/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.727587 core_linked_records_app-2.4.0/tests/utils/providers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/utils/providers/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.760855 core_linked_records_app-2.4.0/tests/utils/providers/handle_net/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/utils/providers/handle_net/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3952 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/utils/providers/handle_net/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.826690 core_linked_records_app-2.4.0/tests/utils/providers/local/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/utils/providers/local/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12238 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/utils/providers/local/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.862141 core_linked_records_app-2.4.0/tests/utils/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/utils/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9314 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/utils/query/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.924926 core_linked_records_app-2.4.0/tests/utils/xml/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/utils/xml/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1454 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/utils/xml/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.940889 core_linked_records_app-2.4.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.961533 core_linked_records_app-2.4.0/tests/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/views/admin/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:15.998543 core_linked_records_app-2.4.0/tests/views/admin/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/views/admin/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6764 2023-07-21 02:13:04.000000 core_linked_records_app-2.4.0/tests/views/admin/views/test_unit.py
```

### Comparing `core_linked_records_app-2.3.0/LICENSE.md` & `core_linked_records_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/PKG-INFO` & `core_linked_records_app-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_linked_records_app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Linked records for the core project
 Home-page: https://github.com/usnistgov/core_linked_records_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =======================
         core_linked_records_app
```

### Comparing `core_linked_records_app-2.3.0/README.rst` & `core_linked_records_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/admin.py` & `core_linked_records_app-2.4.0/core_linked_records_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/apps.py` & `core_linked_records_app-2.4.0/core_linked_records_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/components/blob/api.py` & `core_linked_records_app-2.4.0/core_linked_records_app/components/blob/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from importlib import import_module
 from logging import getLogger
 
 from core_linked_records_app import settings
 from core_linked_records_app.components.local_id import api as local_id_api
 from core_linked_records_app.components.local_id.models import LocalId
 from core_linked_records_app.utils.path import get_api_path_from_object
+from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.commons import exceptions
 from core_main_app.components.blob.models import Blob
 
 logger = getLogger(__name__)
 
 
 def get_blob_by_pid(pid, user):
@@ -50,14 +51,17 @@
             local_id_object.record_object_id, user
         )
     except (AssertionError, exceptions.DoesNotExist):
         error_message = f"PID '{pid}' not assigned to blob"
 
         logger.error(error_message)
         raise exceptions.DoesNotExist(error_message)
+    except AccessControlError as acl_error:
+        logger.error(str(acl_error))
+        raise AccessControlError(str(acl_error))
     except Exception as exc:
         error_message = (
             f"An error occurred while looking up blob assigned to PID '{pid}'"
         )
 
         logger.error("%s: %s", error_message, str(exc))
         raise exceptions.ApiError(error_message)
```

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/components/blob/watch.py` & `core_linked_records_app-2.4.0/core_linked_records_app/components/blob/watch.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ Signals to trigger after Blob save
 """
 import json
 from logging import getLogger
 
+from django.db import transaction
 from django.db.models.signals import post_save, post_delete
 from django.urls import reverse
 
 from core_linked_records_app import settings
 from core_linked_records_app.components.blob import api as blob_api
 from core_linked_records_app.components.pid_settings import (
     api as pid_settings_api,
@@ -21,23 +22,22 @@
 
 def init():
     """Connect to Blob object events."""
     post_save.connect(set_blob_pid, sender=Blob)
     post_delete.connect(delete_blob_pid, sender=Blob)
 
 
-def set_blob_pid(sender, instance: Blob, **kwargs):
-    """set_blob_pid
+def _set_blob_pid(instance: Blob):
+    """Set the PID in the given Blob `instance`. If the PID
+    already exists and is valid, it is not reset.
 
     Args:
-        sender:
         instance:
 
     Returns:
-
     """
     try:
         if not pid_settings_api.get().auto_set_pid:
             return
 
         try:
             blob_api.get_pid_for_blob(str(instance.pk))
@@ -61,14 +61,28 @@
             f"An error occurred while setting a PID for blob '{instance.pk}'"
         )
 
         logger.error("%s: %s", error_message, str(exc))
         raise CoreError(f"{error_message}.")
 
 
+def set_blob_pid(sender, instance: Blob, **kwargs):
+    """Wrapper around `_set_blob_pid` to ensure the PID can be updated while
+    the Blob is being saved without locking the DB.
+
+    Args:
+        sender:
+        instance:
+        kwargs:
+
+    Returns:
+    """
+    transaction.on_commit(lambda: _set_blob_pid(instance))
+
+
 def delete_blob_pid(sender, instance: Blob, **kwargs):
     """Delete a PID assigned to a Blob
 
     Args:
         sender:
         instance:
         kwargs:
```

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/components/data/api.py` & `core_linked_records_app-2.4.0/core_linked_records_app/components/data/api.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/components/data/watch.py` & `core_linked_records_app-2.4.0/core_linked_records_app/components/data/watch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ Signals to trigger before Data save
 """
 import logging
 from os.path import join
 
+from django.db import transaction
 from django.db.models.signals import pre_save, post_delete
 
 from core_linked_records_app import settings
 from core_linked_records_app.components.pid_settings import (
     api as pid_settings_api,
 )
 from core_linked_records_app.system import api as system_api
@@ -23,22 +24,20 @@
 
 def init():
     """Connect to Data object events."""
     pre_save.connect(set_data_pid, sender=Data)
     post_delete.connect(delete_data_pid, sender=Data)
 
 
-def set_data_pid(sender, instance, **kwargs):
+def _set_data_pid(instance: Data):
     """Set the PID in the XML field specified in the settings. If the PID
     already exists and is valid, it is not reset.
 
-    Params:
-        sender:
+    Args:
         instance:
-        kwargs:
 
     Returns:
     """
     from core_linked_records_app.utils import providers as providers_utils
 
     try:
         if not pid_settings_api.get().auto_set_pid:
@@ -63,15 +62,17 @@
                 instance.pk,
                 str(exc),
             )
             return
 
         # Remove previous instance PID from DB.
         if instance.pk is not None:
-            system_api.delete_pid_for_data(instance)
+            transaction.on_commit(
+                lambda: system_api.delete_pid_for_data(instance)
+            )
 
         provider_name = providers_utils.retrieve_provider_name(pid_value)
 
         # Assign default value for undefined PID and check that the PID is not
         # defined for a instance other than the current instance.
         if pid_value is None or pid_value == "":
             pid_value = join(
@@ -109,15 +110,29 @@
             f"An error occurred while assigning PID to {data_definition}"
         )
 
         logger.error("%s: %s", error_message, str(exc))
         raise exceptions.CoreError(f"{error_message}.")
 
 
-def delete_data_pid(sender, instance, **kwargs):
+def set_data_pid(sender, instance: Data, **kwargs):
+    """Wrapper around `_set_data_pid` to ensure the PID can be updated while
+    the Data is being saved without locking the DB.
+
+    Args:
+        sender:
+        instance:
+        kwargs:
+
+    Returns:
+    """
+    transaction.on_commit(lambda: _set_data_pid(instance))
+
+
+def delete_data_pid(sender, instance: Data, **kwargs):
     """Delete a PID assigned to a Data
 
     Args:
         sender:
         instance:
         kwargs:
     """
```

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/components/local_id/api.py` & `core_linked_records_app-2.4.0/core_linked_records_app/components/local_id/api.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/components/local_id/models.py` & `core_linked_records_app-2.4.0/core_linked_records_app/components/local_id/models.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/components/oai_record/api.py` & `core_linked_records_app-2.4.0/core_linked_records_app/components/oai_record/api.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/components/pid_settings/api.py` & `core_linked_records_app-2.4.0/core_linked_records_app/components/pid_settings/api.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/components/pid_settings/models.py` & `core_linked_records_app-2.4.0/core_linked_records_app/components/pid_settings/models.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/components/pid_settings/watch.py` & `core_linked_records_app-2.4.0/core_linked_records_app/components/pid_settings/watch.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/components/pid_xpath/api.py` & `core_linked_records_app-2.4.0/core_linked_records_app/components/pid_xpath/api.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/components/pid_xpath/models.py` & `core_linked_records_app-2.4.0/core_linked_records_app/components/pid_xpath/models.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/migrations/0001_initial.py` & `core_linked_records_app-2.4.0/core_linked_records_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/migrations/0002_alter_pidxpath_xpath.py` & `core_linked_records_app-2.4.0/core_linked_records_app/migrations/0002_alter_pidxpath_xpath.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/rest/blob/views.py` & `core_linked_records_app-2.4.0/core_linked_records_app/rest/blob/views.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/rest/data/renderers/data_html_user_renderer.py` & `core_linked_records_app-2.4.0/core_linked_records_app/rest/data/renderers/data_html_user_renderer.py`

 * *Files 19% similar despite different names*

```diff
@@ -32,14 +32,29 @@
         # Build the request object or set it up to None if undefined
         request = (
             renderer_context["request"]
             if "request" in renderer_context
             else None
         )
 
+        # If the access to the data is forbidden.
+        if (
+            "response" in renderer_context
+            and renderer_context["response"].status_code == 403
+        ):
+            error_msg = (
+                "The user doesn't have enough rights to access document %s"
+                % renderer_context["kwargs"]["record"]
+            )
+            return render(
+                request,
+                "core_main_app/common/commons/error.html",
+                context={"error": error_msg},
+            )
+
         # If the data retrieved contains an error
         if "status" in data and data["status"] == "error":
             return render(
                 request,
                 "core_main_app/common/commons/error.html",
                 context={"error": data["message"]},
             )
```

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/rest/data/renderers/data_xml_renderer.py` & `core_linked_records_app-2.4.0/core_linked_records_app/rest/data/renderers/data_xml_renderer.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/rest/pid/views.py` & `core_linked_records_app-2.4.0/core_linked_records_app/rest/pid/views.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/rest/pid_settings/serializers.py` & `core_linked_records_app-2.4.0/core_linked_records_app/rest/pid_settings/serializers.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/rest/pid_settings/views.py` & `core_linked_records_app-2.4.0/core_linked_records_app/rest/pid_settings/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """ Rest API views to retrieve PID settings
 """
 from rest_framework import status
 from rest_framework.permissions import IsAuthenticated
 from rest_framework.response import Response
 from rest_framework.views import APIView
 
-from core_linked_records_app import settings
 from core_linked_records_app.components.pid_settings import (
     api as pid_settings_api,
 )
 from core_linked_records_app.rest.pid_settings.serializers import (
     PidSettingsSerializer,
 )
+from core_linked_records_app.utils.pid import get_pid_settings_dict
 
 
 class PidSettingsView(APIView):
     """Retrieve PID settings"""
 
     permission_classes = (IsAuthenticated,)
 
@@ -25,28 +25,16 @@
         Args:
             request:
 
         Returns:
         """
         try:
             pid_settings = pid_settings_api.get()
-            pid_settings_data = PidSettingsSerializer(pid_settings).data
-
-            response_data = {
-                "xpath": settings.PID_XPATH,
-                "format": settings.PID_FORMAT,
-                "system_name": settings.ID_PROVIDER_SYSTEM_NAME,
-                "system_type": settings.ID_PROVIDER_SYSTEM_CONFIG["class"],
-                "prefixes": settings.ID_PROVIDER_PREFIXES,
-            }
-
-            pid_settings_data.update(response_data)
-
             return Response(
-                pid_settings_data,
+                get_pid_settings_dict(pid_settings),
                 status=status.HTTP_200_OK,
             )
         except Exception as exc:
             return Response(
                 {
                     "message": f"An unexpected error occurred while displaying "
                     f"PidSettings: {str(exc)}"
```

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/rest/pid_xpath/views.py` & `core_linked_records_app-2.4.0/core_linked_records_app/rest/pid_xpath/views.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/rest/providers/views.py` & `core_linked_records_app-2.4.0/core_linked_records_app/rest/providers/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 
 class ProviderRecordView(APIView):
     """Provider Record View"""
 
     parser_classes = (JSONParser,)
     renderer_classes = (DataHtmlUserRenderer, JSONRenderer, DataXmlRenderer)
 
-    def __init__(self):
+    def __init__(self, **kwargs):
         self.provider_manager = ProviderManager()
-        super().__init__()
+        super().__init__(**kwargs)
 
     def post(self, request, provider, record):
         """Create a handle record
 
         Args:
             request:
             provider:
```

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/rest/query/views.py` & `core_linked_records_app-2.4.0/core_linked_records_app/rest/query/views.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/rest/urls.py` & `core_linked_records_app-2.4.0/core_linked_records_app/rest/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         query_views.RetrieveQueryPidListView.as_view(),
         name="core_linked_records_app_query_pid",
     ),
 ]
 
 urlpatterns += [
     url(
-        r"^settings$",
+        r"^settings/$",
         settings_views.PidSettingsView.as_view(),
         name="core_linked_records_app_settings",
     ),
     url(
         r"^settings/xpath/$",
         xpath_views.PidXpathListView.as_view(),
         name="core_linked_records_app_settings_xpath_list",
```

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/settings.py` & `core_linked_records_app-2.4.0/core_linked_records_app/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ID_PROVIDER_SYSTEM_NAME = getattr(settings, "ID_PROVIDER_SYSTEM_NAME", "local")
 
 ID_PROVIDER_SYSTEM_CONFIG = getattr(
     settings,
     "ID_PROVIDER_SYSTEM_CONFIG",
     {
         "class": "core_linked_records_app.utils.providers.local.LocalIdProvider",
-        "args": [SERVER_URI],
+        "args": [],
     },
 )
 
 ID_PROVIDER_PREFIXES = getattr(settings, "ID_PROVIDER_PREFIXES", ["cdcs"])
 
 ID_PROVIDER_PREFIX_DEFAULT = getattr(
     settings, "ID_PROVIDER_PREFIX_DEFAULT", ID_PROVIDER_PREFIXES[0]
```

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/admin/js/pid_settings/auto_set_pid.js` & `core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/admin/js/pid_settings/auto_set_pid.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -10,38 +10,37 @@
 }
 
 let setAutoSetPidSwitch = () => {
     $autoSetPidError.hide();
     let autoSetPidValue = $autoSetPidLabel.text().trim();
 
     if (autoSetPidValue === "True") {
-        $autoSetPidSwitch.attr("checked", true);
+        $autoSetPidSwitch.prop("checked", true);
     } else if (autoSetPidValue === "False") {
-        $autoSetPidSwitch.attr("checked", false);
+        $autoSetPidSwitch.prop("checked", false);
     } else {
         displayError(
             "Invalid value for 'auto_set_pid'. Contact an administrator for more " +
             "information."
         );
     }
 };
 
 let initAutoSetPidSwitch = () => {
     $autoSetPidError.hide();
     setAutoSetPidSwitch();
 };
 
 let processAutoSetPidClick = (event) => {
-    event.preventDefault();
     $autoSetPidError.hide();
 
     $.ajax({
-        url: "/pid/rest/settings",
+        url: "/pid/rest/settings/",
         data: {
-            "auto_set_pid": !$autoSetPidSwitch.attr("checked")
+            "auto_set_pid": $autoSetPidSwitch.prop("checked")
         },
         dataType: "json",
         type: "patch",
         success: function(data) {
             $autoSetPidLabel.text(data.auto_set_pid ? "True" : "False")
             setAutoSetPidSwitch();
         },
@@ -52,9 +51,9 @@
             )
         }
     });
 }
 
 $(document).ready(function() {
     initAutoSetPidSwitch();
-    $autoSetPidControl.on("click", processAutoSetPidClick)
+    $autoSetPidControl.on("change.bootstrapSwitch", processAutoSetPidClick)
 });
```

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/common_list.js` & `core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/common_list.js`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_detail.js` & `core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_detail.js`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/explore.js` & `core_linked_records_app-2.4.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/explore.js`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/system/api.py` & `core_linked_records_app-2.4.0/core_linked_records_app/system/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 """
 import logging
 
 from django.conf import settings as conf_settings
 from rest_framework import status
 
 from core_linked_records_app import settings
+from core_linked_records_app.components.local_id import api as local_id_api
 from core_linked_records_app.components.local_id.models import LocalId
 from core_linked_records_app.components.pid_xpath.models import PidXpath
-from core_linked_records_app.components.local_id import api as local_id_api
 from core_linked_records_app.utils.dict import get_value_from_dot_notation
 from core_linked_records_app.utils.path import get_api_path_from_object
 from core_linked_records_app.utils.providers import ProviderManager
 from core_main_app.commons.exceptions import DoesNotExist, ApiError
 from core_main_app.components.blob.models import Blob
 from core_main_app.components.data.models import Data
-from core_main_app.utils.query.mongo.prepare import sanitize_value
 from core_main_app.utils import xml as xml_utils
+from core_main_app.utils.query.mongo.prepare import sanitize_value
 
 logger = logging.getLogger(__name__)
 
 
 def is_pid_defined_for_data(pid, document_id):
     """Determine if a given PID match the document ID provided.
 
@@ -147,27 +147,40 @@
 
 def delete_pid_from_record_name(record_name: str):
     """Delete a PID from the provider using the record name as stored in the
     LocalId table.
 
     Args:
         record_name: str - Formatted as prefix/record.
+
+    Raises:
+        ApiError: if the HTTP status is not 200 or 404.
     """
     # Delete the given LocalID fron the default PID provider.
     provider = ProviderManager().get()
     previous_pid_delete_response = provider.delete(record_name)
 
+    if previous_pid_delete_response.status_code == status.HTTP_200_OK:
+        return
+
+    # At this point, there was some problem deleting the LocalID needed to be logged.
+    error_message = (
+        f"Deletion of LocalID {record_name} from provider "
+        f"{ProviderManager().provider_name} returned "
+        f"{previous_pid_delete_response.status_code}"
+    )
+
+    # Do not crash for a 404, but log that an error occured.
+    if previous_pid_delete_response.status_code == status.HTTP_404_NOT_FOUND:
+        logger.warning(error_message)
+        return
+
     # Log any error that happened during PID deletion.
-    if previous_pid_delete_response.status_code != status.HTTP_200_OK:
-        error_message = (
-            f"Deletion of LocalID {record_name} from provider {ProviderManager().provider_name} "
-            f"returned {previous_pid_delete_response.status_code}"
-        )
-        logger.error(error_message)
-        raise ApiError(error_message)
+    logger.error(error_message)
+    raise ApiError(error_message)
 
 
 def delete_pid_for_data(data: Data):
     """Deletes the PID assigned to the data passed in parameter. If no PID has
     been assigned, the function simply exits.
 
     Args:
```

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/utils/blob.py` & `core_linked_records_app-2.4.0/core_linked_records_app/utils/blob.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/utils/data.py` & `core_linked_records_app-2.4.0/core_linked_records_app/utils/data.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/utils/dict.py` & `core_linked_records_app-2.4.0/core_linked_records_app/utils/dict.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/utils/path.py` & `core_linked_records_app-2.4.0/core_linked_records_app/utils/path.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/utils/providers/__init__.py` & `core_linked_records_app-2.4.0/core_linked_records_app/utils/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/utils/providers/handle_net.py` & `core_linked_records_app-2.4.0/core_linked_records_app/utils/providers/handle_net.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/utils/providers/local.py` & `core_linked_records_app-2.4.0/core_linked_records_app/utils/providers/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         """
         response = Response()
 
         record_url = f"{self.provider_lookup_url}/{record}"
 
         try:
             record_object = record_api.get_by_name(record)
-            record_object.delete()
+            record_api.delete(record_object)
 
             response.status_code = status.HTTP_200_OK
             response._content = json.dumps(
                 {
                     "record": record,
                     "message": self.messages["success"],
                     "url": record_url,
```

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/utils/query.py` & `core_linked_records_app-2.4.0/core_linked_records_app/utils/query.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/utils/xml.py` & `core_linked_records_app-2.4.0/core_linked_records_app/utils/xml.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app/views/admin/views.py` & `core_linked_records_app-2.4.0/core_linked_records_app/views/admin/views.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,110 +1,85 @@
 """ Administration views
 """
-from urllib.parse import urljoin
 
 from django.urls import reverse
 from django.views.generic import View
 
+from core_linked_records_app.components.pid_xpath import api as pid_xpath_api
 from core_linked_records_app.settings import SERVER_URI
-from core_main_app.components.template import api as template_api
+from core_linked_records_app.utils.pid import get_pid_settings_dict
+from core_linked_records_app.components.pid_settings import (
+    api as pid_settings_api,
+)
 from core_main_app.utils.rendering import admin_render
-from core_main_app.utils.requests_utils.requests_utils import send_get_request
 
 
 class PidSettingsView(View):
     """View to display PID settings in the admin part"""
 
     def get(self, request):
         """HTTP GET method"""
         context = {}
 
         assets = {
             "js": [
                 {
                     "path": "core_linked_records_app/admin/js/pid_settings/auto_set_pid.js",
-                    "is_raw": True,
+                    "is_raw": False,
                 }
             ],
             "css": [
                 "core_linked_records_app/admin/css/pid_settings.css",
             ],
         }
 
-        settings_rest_url = reverse("core_linked_records_app_settings")
-        settings_response = send_get_request(
-            urljoin(SERVER_URI, settings_rest_url),
-            cookies={
-                "sessionid": request.session.session_key,
-            },
-        )
+        xpath_settings = {}
 
-        if settings_response.status_code != 200:
-            return admin_render(
-                request,
-                "core_linked_records_app/admin/pid_settings_error.html",
-                context={
-                    "error": "An error occured while retrieving the PID settings. "
-                    "Please contact an administrator for more information."
+        # Retrieve existing PidXpath
+        try:
+            for xpath_item in pid_xpath_api.get_all(request):
+                xpath_settings[xpath_item.template.display_name] = {
+                    "xpath": xpath_item.xpath,
+                    "edit_url": reverse(
+                        "admin:core_linked_records_app_pidxpath_change",
+                        args=(xpath_item.pk,),
+                    ),
+                }
+
+            pid_settings = pid_settings_api.get()
+            response_dict = get_pid_settings_dict(pid_settings)
+            response_dict["xpath"] = {
+                "default": {"xpath": response_dict["xpath"]}
+            }
+            response_dict["xpath"].update(xpath_settings)
+
+            response_dict["add_xpath_url"] = reverse(
+                "admin:core_linked_records_app_pidxpath_add"
+            )
+
+            record_sample_url = reverse(
+                "core_linked_records_provider_record",
+                kwargs={
+                    "provider": response_dict["system_name"],
+                    "record": f"{response_dict['prefixes'][0]}/record",
                 },
             )
+            response_dict["sample_url"] = f"{SERVER_URI}{record_sample_url}"
 
-        pid_xpath_rest_url = reverse(
-            "core_linked_records_app_settings_xpath_list"
-        )
-        xpath_response = send_get_request(
-            urljoin(SERVER_URI, pid_xpath_rest_url),
-            cookies={
-                "sessionid": request.session.session_key,
-            },
-        )
+            context.update({"pid_settings": response_dict})
 
-        if xpath_response.status_code != 200:
+            return admin_render(
+                request,
+                "core_linked_records_app/admin/pid_settings.html",
+                assets=assets,
+                context=context,
+            )
+        except Exception as exc:
             return admin_render(
                 request,
                 "core_linked_records_app/admin/pid_settings_error.html",
                 context={
-                    "error": "An error occured while retrieving the list of PID XPath. "
-                    "Please contact an administrator for more information."
+                    "error": "An error occured while retrieving the PID settings. "
+                    "Please contact an administrator for more information. Exception: "
+                    f"{str(exc)}."
                 },
             )
-
-        xpath_settings = {}
-
-        # Retrieve existing PidXpath
-        for xpath_item in xpath_response.json():
-            xpath_template = template_api.get_by_id(
-                xpath_item["template"], request
-            )
-            xpath_settings[xpath_template.display_name] = {
-                "xpath": xpath_item["xpath"],
-                "edit_url": reverse(
-                    "admin:core_linked_records_app_pidxpath_change",
-                    args=(xpath_item["id"],),
-                ),
-            }
-
-        response_dict = settings_response.json()
-        response_dict["xpath"] = {"default": {"xpath": response_dict["xpath"]}}
-        response_dict["xpath"].update(xpath_settings)
-
-        response_dict["add_xpath_url"] = reverse(
-            "admin:core_linked_records_app_pidxpath_add"
-        )
-
-        record_sample_url = reverse(
-            "core_linked_records_provider_record",
-            kwargs={
-                "provider": response_dict["system_name"],
-                "record": f"{response_dict['prefixes'][0]}/record",
-            },
-        )
-        response_dict["sample_url"] = f"{SERVER_URI}{record_sample_url}"
-
-        context.update({"pid_settings": response_dict})
-
-        return admin_render(
-            request,
-            "core_linked_records_app/admin/pid_settings.html",
-            assets=assets,
-            context=context,
-        )
```

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app.egg-info/PKG-INFO` & `core_linked_records_app-2.4.0/core_linked_records_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-linked-records-app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Linked records for the core project
 Home-page: https://github.com/usnistgov/core_linked_records_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =======================
         core_linked_records_app
```

### Comparing `core_linked_records_app-2.3.0/core_linked_records_app.egg-info/SOURCES.txt` & `core_linked_records_app-2.4.0/core_linked_records_app.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -95,28 +95,30 @@
 core_linked_records_app/utils/providers/__init__.py
 core_linked_records_app/utils/providers/handle_net.py
 core_linked_records_app/utils/providers/local.py
 core_linked_records_app/views/__init__.py
 core_linked_records_app/views/admin/__init__.py
 core_linked_records_app/views/admin/views.py
 tests/__init__.py
+tests/fixtures.py
 tests/mocks.py
 tests/test_settings.py
 tests/test_urls.py
 tests/components/__init__.py
 tests/components/blob/__init__.py
 tests/components/blob/api/__init__.py
 tests/components/blob/api/test_unit.py
 tests/components/blob/watch/__init__.py
 tests/components/blob/watch/test_unit.py
 tests/components/data/__init__.py
 tests/components/data/api/__init__.py
 tests/components/data/api/test_unit.py
 tests/components/data/watch/__init__.py
-tests/components/data/watch/test_unit.py
+tests/components/data/watch/tests_integration.py
+tests/components/data/watch/tests_unit.py
 tests/components/local_id/__init__.py
 tests/components/local_id/admin_site/__init__.py
 tests/components/local_id/admin_site/test_unit.py
 tests/components/local_id/api/__init__.py
 tests/components/local_id/api/test_unit.py
 tests/components/local_id/models/__init__.py
 tests/components/local_id/models/test_unit.py
@@ -140,14 +142,18 @@
 tests/menus/__init__.py
 tests/menus/test_unit.py
 tests/rest/__init__.py
 tests/rest/blob/__init__.py
 tests/rest/blob/views/__init__.py
 tests/rest/blob/views/test_permissions.py
 tests/rest/blob/views/test_unit.py
+tests/rest/data/__init__.py
+tests/rest/data/renderers/__init__.py
+tests/rest/data/renderers/data_html_user_renderer/__init__.py
+tests/rest/data/renderers/data_html_user_renderer/tests_unit.py
 tests/rest/pid/__init__.py
 tests/rest/pid/views/__init__.py
 tests/rest/pid/views/test_permissions.py
 tests/rest/pid/views/test_unit.py
 tests/rest/pid_settings/__init__.py
 tests/rest/pid_settings/views/__init__.py
 tests/rest/pid_settings/views/test_permissions.py
```

### Comparing `core_linked_records_app-2.3.0/setup.py` & `core_linked_records_app-2.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_linked_records_app",
-    version="2.3.0",
+    version="2.4.0",
     description="Linked records for the core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_linked_records_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_linked_records_app-2.3.0/tests/components/blob/api/test_unit.py` & `core_linked_records_app-2.4.0/tests/components/blob/api/test_unit.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """
 from unittest import TestCase
 from unittest.mock import patch
 
 from core_linked_records_app.components.blob import api as blob_api
 from core_linked_records_app.components.local_id import api as local_id_api
 from core_linked_records_app.components.local_id.models import LocalId
+from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.commons import exceptions
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from tests import mocks
 
 
 class TestGetBlobByPid(TestCase):
     """Test Get Blob By Pid"""
@@ -77,14 +78,36 @@
 
         with self.assertRaises(exceptions.ApiError):
             blob_api.get_blob_by_pid(mock_valid_pid, self.user)
 
     @patch.object(blob_api, "getattr")
     @patch.object(blob_api, "import_module")
     @patch.object(local_id_api, "get_by_name")
+    def test_get_by_id_acl_error_raises_acl_error(
+        self, mock_get_by_name, mock_import_module, mock_getattr
+    ):
+        """test_get_by_id_acl_error_raises_acl_error"""
+
+        mock_valid_pid = "https://websi.te/provider/record"
+        mock_get_by_name.return_value = LocalId(
+            record_name=mock_valid_pid,
+            record_object_class="mock_record_object_class",
+            record_object_id="mock_record_object_id",
+        )
+        mock_import_module.return_value = None
+        mock_getattr.side_effect = AccessControlError(
+            "mock_getattr_access_control_error"
+        )
+
+        with self.assertRaises(AccessControlError):
+            blob_api.get_blob_by_pid(mock_valid_pid, self.user)
+
+    @patch.object(blob_api, "getattr")
+    @patch.object(blob_api, "import_module")
+    @patch.object(local_id_api, "get_by_name")
     def test_returns_expected_get_by_id_output(
         self, mock_get_by_name, mock_import_module, mock_getattr
     ):
         """test_returns_expected_get_by_id_output"""
 
         mock_valid_pid = "https://websi.te/provider/record"
         mock_get_by_name.return_value = LocalId(
```

### Comparing `core_linked_records_app-2.3.0/tests/components/blob/watch/test_unit.py` & `core_linked_records_app-2.4.0/tests/components/blob/watch/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/components/data/api/test_unit.py` & `core_linked_records_app-2.4.0/tests/components/data/api/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/components/data/watch/test_unit.py` & `core_linked_records_app-2.4.0/tests/components/data/watch/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/components/local_id/admin_site/test_unit.py` & `core_linked_records_app-2.4.0/tests/components/local_id/admin_site/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/components/local_id/api/test_unit.py` & `core_linked_records_app-2.4.0/tests/components/local_id/api/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/components/local_id/models/test_unit.py` & `core_linked_records_app-2.4.0/tests/components/local_id/models/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/components/oai_record/api/test_unit.py` & `core_linked_records_app-2.4.0/tests/components/oai_record/api/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/components/pid_settings/api/test_unit.py` & `core_linked_records_app-2.4.0/tests/components/pid_settings/api/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/components/pid_settings/models/test_unit.py` & `core_linked_records_app-2.4.0/tests/components/pid_settings/models/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/components/pid_settings/watch/test_unit.py` & `core_linked_records_app-2.4.0/tests/components/pid_settings/watch/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/components/pid_xpath/admin_site/test_unit.py` & `core_linked_records_app-2.4.0/tests/components/pid_xpath/admin_site/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/components/pid_xpath/api/test_unit.py` & `core_linked_records_app-2.4.0/tests/components/pid_xpath/api/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/components/pid_xpath/models/test_unit.py` & `core_linked_records_app-2.4.0/tests/components/pid_xpath/models/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/menus/test_unit.py` & `core_linked_records_app-2.4.0/tests/menus/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/mocks.py` & `core_linked_records_app-2.4.0/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/rest/blob/views/test_permissions.py` & `core_linked_records_app-2.4.0/tests/rest/blob/views/test_permissions.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/rest/blob/views/test_unit.py` & `core_linked_records_app-2.4.0/tests/rest/blob/views/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/rest/pid/views/test_permissions.py` & `core_linked_records_app-2.4.0/tests/rest/pid/views/test_permissions.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/rest/pid/views/test_unit.py` & `core_linked_records_app-2.4.0/tests/rest/pid/views/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/rest/pid_settings/views/test_permissions.py` & `core_linked_records_app-2.4.0/tests/rest/pid_settings/views/test_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             pid_settings_views.PidSettingsView.as_view(), mock_user
         )
 
         self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
 
     @patch.object(pid_settings_api, "get")
     @patch.object(PidSettingsSerializer, "__new__")
-    def test_staff_returns_200(
+    def test_superuser_returns_200(
         self, mock_pid_serializer, mock_pid_settings_get
     ):
         """test_staff_returns_200"""
 
         mock_user = create_mock_user("1", is_superuser=True)
 
         mock_pid_serializer.return_value = mocks.MockSerializer()
```

### Comparing `core_linked_records_app-2.3.0/tests/rest/pid_settings/views/test_unit.py` & `core_linked_records_app-2.4.0/tests/rest/pid_settings/views/test_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     views as pid_settings_views,
 )
 from core_linked_records_app.rest.pid_settings.serializers import (
     PidSettingsSerializer,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from tests import mocks
+from tests.mocks import MockPidSettings
 
 
 class TestPidSettingsViewGet(TestCase):
     """Test Pid Settings View Get"""
 
     def setUp(self):
         """setUp"""
@@ -52,23 +53,19 @@
         )
 
         test_view = pid_settings_views.PidSettingsView()
         response = test_view.get(self.mock_request)
 
         self.assertEqual(response.status_code, 500)
 
-    @patch.object(PidSettingsSerializer, "__new__")
     @patch.object(pid_settings_api, "get")
-    def test_success_returns_200(
-        self, mock_pid_settings_get, mock_pid_settings_serializer
-    ):
+    def test_success_returns_200(self, mock_pid_settings_get):
         """test_success_returns_200"""
 
-        mock_pid_settings_get.return_value = "mock_pid_settings"
-        mock_pid_settings_serializer.return_value = mocks.MockSerializer()
+        mock_pid_settings_get.return_value = MockPidSettings()
 
         test_view = pid_settings_views.PidSettingsView()
         response = test_view.get(self.mock_request)
 
         self.assertEqual(response.status_code, 200)
```

### Comparing `core_linked_records_app-2.3.0/tests/rest/pid_xpath/views/test_permissions.py` & `core_linked_records_app-2.4.0/tests/rest/pid_xpath/views/test_permissions.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/rest/providers/views/test_permissions.py` & `core_linked_records_app-2.4.0/tests/rest/providers/views/test_permissions.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/rest/providers/views/test_unit.py` & `core_linked_records_app-2.4.0/tests/rest/providers/views/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/rest/query/test_unit.py` & `core_linked_records_app-2.4.0/tests/rest/query/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/system/api/test_unit.py` & `core_linked_records_app-2.4.0/tests/system/api/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/test_settings.py` & `core_linked_records_app-2.4.0/tests/test_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.sites",
     "django.contrib.staticfiles",
     # Extra apps
     "defender",
     "django_celery_beat",
-    "tz_detect",
+    "drf_spectacular",
     "menu",
     # Local apps
     "xml_utils",
     "core_main_app",
     "core_explore_common_app",
     "core_explore_oaipmh_app",
     "core_federated_search_app",
@@ -41,15 +41,14 @@
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
@@ -68,14 +67,16 @@
 
 CUSTOM_NAME = "mock_custom_name"
 
 ROOT_URLCONF = "tests.test_urls"
 
 STATIC_URL = "/static/"
 
+DEFAULT_AUTO_FIELD = "django.db.models.BigAutoField"
+
 CELERYBEAT_SCHEDULER = "django_celery_beat.schedulers:DatabaseScheduler"
 SERVER_URI = "http://mock-cdcs.com"
 
 PID_XPATH = "mock.pid"
 
 ID_PROVIDER_PREFIXES = ["mock_cdcs"]
```

### Comparing `core_linked_records_app-2.3.0/tests/utils/dict/test_unit.py` & `core_linked_records_app-2.4.0/tests/utils/dict/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/utils/pid/test_unit.py` & `core_linked_records_app-2.4.0/tests/utils/pid/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/utils/providers/handle_net/test_unit.py` & `core_linked_records_app-2.4.0/tests/utils/providers/handle_net/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/utils/providers/local/test_unit.py` & `core_linked_records_app-2.4.0/tests/utils/providers/local/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/utils/query/test_unit.py` & `core_linked_records_app-2.4.0/tests/utils/query/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.3.0/tests/utils/xml/test_unit.py` & `core_linked_records_app-2.4.0/tests/utils/xml/test_unit.py`

 * *Files identical despite different names*

