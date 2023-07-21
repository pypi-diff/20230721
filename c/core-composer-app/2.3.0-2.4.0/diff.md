# Comparing `tmp/core_composer_app-2.3.0.tar.gz` & `tmp/core_composer_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_composer_app-2.3.0.tar", last modified: Tue May  2 19:34:00 2023, max compression
+gzip compressed data, was "core_composer_app-2.4.0.tar", last modified: Fri Jul 21 02:09:25 2023, max compression
```

## Comparing `core_composer_app-2.3.0.tar` & `core_composer_app-2.4.0.tar`

### file list

```diff
@@ -1,189 +1,199 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:34:00.184523 core_composer_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      142 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1038 2023-05-02 19:34:00.179244 core_composer_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      548 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.274312 core_composer_app-2.3.0/core_composer_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      105 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3401 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      494 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.350881 core_composer_app-2.3.0/core_composer_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.414705 core_composer_app-2.3.0/core_composer_app/components/bucket/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/bucket/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2542 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/bucket/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2390 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/bucket/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.479158 core_composer_app-2.3.0/core_composer_app/components/type/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/type/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      346 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/type/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1460 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/type/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1040 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/type/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.541989 core_composer_app-2.3.0/core_composer_app/components/type_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/type_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      355 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/type_version_manager/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3924 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/type_version_manager/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2375 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/components/type_version_manager/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      630 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.566271 core_composer_app-2.3.0/core_composer_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3384 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      777 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.607754 core_composer_app-2.3.0/core_composer_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1295 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/permissions/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      191 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/permissions/rights.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.634706 core_composer_app-2.3.0/core_composer_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.669733 core_composer_app-2.3.0/core_composer_app/rest/bucket/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/rest/bucket/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1680 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/rest/bucket/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10151 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/rest/bucket/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.763719 core_composer_app-2.3.0/core_composer_app/rest/type_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/rest/type_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5479 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/rest/type_version_manager/abstract_views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2390 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/rest/type_version_manager/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3366 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/rest/type_version_manager/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3225 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:51.141612 core_composer_app-2.3.0/core_composer_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:52.104184 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:51.146292 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.794430 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/admin/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      753 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/admin/js/bucket.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       80 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/admin/js/bucket.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:51.188857 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/admin/js/types/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.835860 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/admin/js/types/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      983 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependencies.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependencies.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      143 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependency_resolver.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:52.099061 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.850302 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/common/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      122 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/common/css/bucket.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:52.120441 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.926123 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      532 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/css/menu.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       56 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/css/style.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       64 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/css/xsd_tree.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.988019 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3831 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/js/build_template.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      713 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/js/build_template.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10778 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/js/menus.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1043 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/js/xpath.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      444 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/js/xsd_tree.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.003004 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/xsd/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      202 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/xsd/new_base_template.xsd
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.018035 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/xsl/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4750 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/xsl/xsd2html.xsl
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:52.139505 core_composer_app-2.3.0/core_composer_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.016618 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.005528 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.090384 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      168 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/add.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      922 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/add_content.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      348 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/edit.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1204 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/edit_content.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.105105 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1329 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/list/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      165 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.119251 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      558 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/modals/delete.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.157319 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.186425 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1966 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/list/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1207 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/list/disabled.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      228 2023-05-02 19:33:35.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/list.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       58 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/upload.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.234729 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/versions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1199 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/versions/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/versions/disabled.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      360 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/versions.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.261819 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      889 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/build_template.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.293306 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      413 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/list_types.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.328431 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/menus/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      276 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/menus/element.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      126 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/menus/element_root.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      198 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/menus/sequence.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.491938 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      654 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/change_type.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      532 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/delete_element.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      712 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/element_name.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      418 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/errors.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1098 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/insert_element.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1079 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/occurrences.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      676 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/root_type_name.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      451 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_success.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      616 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_template.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      592 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_type.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      384 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/new_element.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1930 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/index.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.505957 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      275 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/list/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.520155 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/types/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.534711 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/types/versions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      325 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/types/versions/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      262 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/types/versions.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2529 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.571353 core_composer_app-2.3.0/core_composer_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16675 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/utils/xml.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.585308 core_composer_app-2.3.0/core_composer_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.655331 core_composer_app-2.3.0/core_composer_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3892 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2157 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17258 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.717179 core_composer_app-2.3.0/core_composer_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16759 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9293 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/core_composer_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:58.336760 core_composer_app-2.3.0/core_composer_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1038 2023-05-02 19:33:47.000000 core_composer_app-2.3.0/core_composer_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6765 2023-05-02 19:33:47.000000 core_composer_app-2.3.0/core_composer_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:33:47.000000 core_composer_app-2.3.0/core_composer_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       85 2023-05-02 19:33:47.000000 core_composer_app-2.3.0/core_composer_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       29 2023-05-02 19:33:47.000000 core_composer_app-2.3.0/core_composer_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.766397 core_composer_app-2.3.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11283 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      289 2023-05-02 19:33:36.000000 core_composer_app-2.3.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       39 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:34:00.186149 core_composer_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.798836 core_composer_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.814869 core_composer_app-2.3.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.849532 core_composer_app-2.3.0/tests/components/bucket/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/bucket/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.896220 core_composer_app-2.3.0/tests/components/bucket/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/bucket/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1047 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/bucket/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7227 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/bucket/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.933396 core_composer_app-2.3.0/tests/components/type/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/type/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5598 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/type/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:59.979785 core_composer_app-2.3.0/tests/components/type_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/type_version_manager/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:34:00.015325 core_composer_app-2.3.0/tests/components/type_version_manager/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/type_version_manager/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4412 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/type_version_manager/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20898 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/type_version_manager/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16645 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/components/type_version_manager/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:34:00.031960 core_composer_app-2.3.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:34:00.081947 core_composer_app-2.3.0/tests/rest/bucket/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/rest/bucket/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13700 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/rest/bucket/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10519 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/rest/bucket/tests_permission.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:34:00.134670 core_composer_app-2.3.0/tests/rest/type_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/rest/type_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14870 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/rest/type_version_manager/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9582 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/rest/type_version_manager/tests_permission.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1582 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:34:00.164514 core_composer_app-2.3.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8032 2023-05-02 19:33:37.000000 core_composer_app-2.3.0/tests/utils/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.705874 core_composer_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:09:08.000000 core_composer_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      142 2023-07-21 02:09:08.000000 core_composer_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1038 2023-07-21 02:09:25.701646 core_composer_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      548 2023-07-21 02:09:08.000000 core_composer_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:23.966779 core_composer_app-2.4.0/core_composer_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      105 2023-07-21 02:09:08.000000 core_composer_app-2.4.0/core_composer_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3401 2023-07-21 02:09:08.000000 core_composer_app-2.4.0/core_composer_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      494 2023-07-21 02:09:08.000000 core_composer_app-2.4.0/core_composer_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.033773 core_composer_app-2.4.0/core_composer_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:08.000000 core_composer_app-2.4.0/core_composer_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.071935 core_composer_app-2.4.0/core_composer_app/components/bucket/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/components/bucket/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2542 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/components/bucket/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2390 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/components/bucket/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.113640 core_composer_app-2.4.0/core_composer_app/components/type/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/components/type/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      346 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/components/type/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1460 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/components/type/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1040 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/components/type/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.154497 core_composer_app-2.4.0/core_composer_app/components/type_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/components/type_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      355 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/components/type_version_manager/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3871 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/components/type_version_manager/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2375 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/components/type_version_manager/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      630 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.197293 core_composer_app-2.4.0/core_composer_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3384 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      777 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.246585 core_composer_app-2.4.0/core_composer_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1295 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/permissions/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      191 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/permissions/rights.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.272822 core_composer_app-2.4.0/core_composer_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.328899 core_composer_app-2.4.0/core_composer_app/rest/bucket/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/rest/bucket/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1680 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/rest/bucket/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10151 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/rest/bucket/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.375387 core_composer_app-2.4.0/core_composer_app/rest/type_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/rest/type_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5479 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/rest/type_version_manager/abstract_views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2390 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/rest/type_version_manager/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3366 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/rest/type_version_manager/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3225 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:23.418085 core_composer_app-2.4.0/core_composer_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:23.577602 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:23.423038 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.408376 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/admin/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      753 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/admin/js/bucket.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       80 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/admin/js/bucket.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:23.430727 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/admin/js/types/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.456070 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/admin/js/types/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      983 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependencies.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependencies.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      143 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependency_resolver.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:23.561736 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.470206 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/common/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      122 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/common/css/bucket.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:23.593458 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.504828 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      532 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/user/css/menu.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       56 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/user/css/style.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       64 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/user/css/xsd_tree.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.559933 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3532 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/user/js/build_template.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      713 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/user/js/build_template.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10778 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/user/js/menus.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1043 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/user/js/xpath.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      444 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/user/js/xsd_tree.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.570594 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/user/xsd/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      202 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/user/xsd/new_base_template.xsd
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.582115 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/user/xsl/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4750 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/static/core_composer_app/user/xsl/xsd2html.xsl
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:23.602582 core_composer_app-2.4.0/core_composer_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:23.649483 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:23.630593 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.676183 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/buckets/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      168 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/buckets/add.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1017 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/buckets/add_content.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      348 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/buckets/edit.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1299 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/buckets/edit_content.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.691452 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/buckets/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1424 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/buckets/list/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      165 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/buckets/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.705343 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/buckets/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      660 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/buckets/modals/delete.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.747949 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/types/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.771660 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/types/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2061 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/types/list/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1207 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/types/list/disabled.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      228 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/types/list.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       58 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/types/upload.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.824772 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/types/versions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1401 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/types/versions/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/types/versions/disabled.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      360 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/types/versions.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.843136 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1281 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/build_template.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.865212 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      889 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/list_types.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.899601 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/menus/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      276 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/menus/element.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      126 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/menus/element_root.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      198 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/menus/sequence.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.992596 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      762 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/modals/change_type.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      634 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/modals/delete_element.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      814 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/modals/element_name.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      520 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/modals/errors.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1287 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/modals/insert_element.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1181 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/modals/occurrences.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      676 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/modals/root_type_name.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      718 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_template.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      700 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_type.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      384 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/new_element.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2026 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/index.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.003161 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      275 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/list/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.015736 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/types/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.026007 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/types/versions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      325 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/types/versions/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      262 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/types/versions.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2529 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.077287 core_composer_app-2.4.0/core_composer_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16675 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/utils/xml.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.091003 core_composer_app-2.4.0/core_composer_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.158050 core_composer_app-2.4.0/core_composer_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3892 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2157 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17258 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.194006 core_composer_app-2.4.0/core_composer_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17010 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9434 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/core_composer_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:24.020545 core_composer_app-2.4.0/core_composer_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1038 2023-07-21 02:09:22.000000 core_composer_app-2.4.0/core_composer_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6919 2023-07-21 02:09:23.000000 core_composer_app-2.4.0/core_composer_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:09:22.000000 core_composer_app-2.4.0/core_composer_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       85 2023-07-21 02:09:22.000000 core_composer_app-2.4.0/core_composer_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       29 2023-07-21 02:09:22.000000 core_composer_app-2.4.0/core_composer_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.231716 core_composer_app-2.4.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:09.000000 core_composer_app-2.4.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11283 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      289 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       39 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:09:25.707246 core_composer_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.255295 core_composer_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.287420 core_composer_app-2.4.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.320536 core_composer_app-2.4.0/tests/components/bucket/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/components/bucket/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.343741 core_composer_app-2.4.0/tests/components/bucket/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/components/bucket/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1047 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/components/bucket/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7227 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/components/bucket/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.368834 core_composer_app-2.4.0/tests/components/type/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/components/type/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5598 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/components/type/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.410649 core_composer_app-2.4.0/tests/components/type_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/components/type_version_manager/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.437279 core_composer_app-2.4.0/tests/components/type_version_manager/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/components/type_version_manager/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4412 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/components/type_version_manager/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20898 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/components/type_version_manager/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15158 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/components/type_version_manager/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.450733 core_composer_app-2.4.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.521059 core_composer_app-2.4.0/tests/rest/bucket/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/rest/bucket/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13700 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/rest/bucket/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10519 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/rest/bucket/tests_permission.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.569697 core_composer_app-2.4.0/tests/rest/type_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/rest/type_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14870 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/rest/type_version_manager/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9582 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/rest/type_version_manager/tests_permission.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1582 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.597756 core_composer_app-2.4.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8032 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/utils/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.610433 core_composer_app-2.4.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.625757 core_composer_app-2.4.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/views/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.663261 core_composer_app-2.4.0/tests/views/user/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/views/user/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11311 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/views/user/ajax/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    22448 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/views/user/ajax/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:25.689622 core_composer_app-2.4.0/tests/views/user/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/views/user/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6519 2023-07-21 02:09:10.000000 core_composer_app-2.4.0/tests/views/user/views/tests_unit.py
```

### Comparing `core_composer_app-2.3.0/LICENSE.md` & `core_composer_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/PKG-INFO` & `core_composer_app-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_composer_app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Template and type composer for the curator core project
 Home-page: https://github.com/usnistgov/core_composer_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =================
         Core Composer App
```

### Comparing `core_composer_app-2.3.0/README.rst` & `core_composer_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/admin.py` & `core_composer_app-2.4.0/core_composer_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/components/bucket/api.py` & `core_composer_app-2.4.0/core_composer_app/components/bucket/api.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/components/bucket/models.py` & `core_composer_app-2.4.0/core_composer_app/components/bucket/models.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/components/type/api.py` & `core_composer_app-2.4.0/core_composer_app/components/type/api.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/components/type/models.py` & `core_composer_app-2.4.0/core_composer_app/components/type/models.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/components/type_version_manager/api.py` & `core_composer_app-2.4.0/core_composer_app/components/type_version_manager/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,26 +122,24 @@
 @access_control(can_read_global)
 def get_no_buckets_types(request):
     """Get list of available types not inside a bucket.
 
     Returns:
 
     """
-    # build list of types
-    bucket_types = []
+    # Retrieve IDs of types in buckets.
+    bucket_type_id_list = []
     for bucket in bucket_api.get_all():
-        bucket_types += bucket.types.all()
-
-    all_types = get_global_version_managers(request=request)
-    no_bucket_types = [
-        type_version_manager
-        for type_version_manager in all_types
-        if type_version_manager not in bucket_types
-    ]
-    return no_bucket_types
+        bucket_type_id_list += [
+            bucket_type.pk for bucket_type in bucket.types.all()
+        ]
+
+    return get_global_version_managers(request=request).exclude(
+        pk__in=bucket_type_id_list
+    )
 
 
 @access_control(is_superuser)
 def get_all_version_manager(request):
     """Return all Type Version Managers of all users.
 
     Returns:
```

### Comparing `core_composer_app-2.3.0/core_composer_app/components/type_version_manager/models.py` & `core_composer_app-2.4.0/core_composer_app/components/type_version_manager/models.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/menus.py` & `core_composer_app-2.4.0/core_composer_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/migrations/0001_initial.py` & `core_composer_app-2.4.0/core_composer_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/models.py` & `core_composer_app-2.4.0/core_composer_app/models.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/permissions/discover.py` & `core_composer_app-2.4.0/core_composer_app/permissions/discover.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/rest/bucket/serializers.py` & `core_composer_app-2.4.0/core_composer_app/rest/bucket/serializers.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/rest/bucket/views.py` & `core_composer_app-2.4.0/core_composer_app/rest/bucket/views.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/rest/type_version_manager/abstract_views.py` & `core_composer_app-2.4.0/core_composer_app/rest/type_version_manager/abstract_views.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/rest/type_version_manager/serializers.py` & `core_composer_app-2.4.0/core_composer_app/rest/type_version_manager/serializers.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/rest/type_version_manager/views.py` & `core_composer_app-2.4.0/core_composer_app/rest/type_version_manager/views.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/rest/urls.py` & `core_composer_app-2.4.0/core_composer_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/static/core_composer_app/admin/js/bucket.js` & `core_composer_app-2.4.0/core_composer_app/static/core_composer_app/admin/js/bucket.js`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependencies.js` & `core_composer_app-2.4.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependencies.js`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/css/menu.css` & `core_composer_app-2.4.0/core_composer_app/static/core_composer_app/user/css/menu.css`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/js/build_template.js` & `core_composer_app-2.4.0/core_composer_app/static/core_composer_app/user/js/build_template.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -27,17 +27,16 @@
         $.ajax({
             url: saveTemplateUrl,
             type: "POST",
             dataType: "json",
             data: {
                 templateName: templateName
             },
-            success: function(data) {
-                $("#save-template-modal").modal("hide");
-                displaySaveSuccess();
+            success: function() {
+                window.location = composerIndexUrl;
             },
             error: function(data) {
                 $("#new-template-error").html(data.responseText);
             }
         });
     } else {
         $("#new-template-error").html("The name can't be empty.")
@@ -65,45 +64,37 @@
             url: saveTypeUrl,
             type: "POST",
             dataType: "json",
             data: {
                 typeName: typeName,
                 templateID: templateID
             },
-            success: function(data) {
-                $("#save-type-modal").modal("hide");
-                displaySaveSuccess();
+            success: function() {
+                window.location = composerIndexUrl;
             },
             error: function(data) {
                 $("#new-type-error").html(data.responseText);
             }
         });
     } else {
         $("#new-type-error").html("The name can't be empty.")
     }
 };
 
-var displaySaveSuccess = function() {
-    var $save_success_modal = $("#save-success-modal");
-    $save_success_modal.modal("show");
-    $save_success_modal.on("hidden.bs.modal", function() {
-        window.location = composerIndexUrl;
-    });
-};
-
 
 /**
  * Dialog to change root type name when new template
  */
 var displayNewTemplateDialog = function() {
     $("#newTemplateTypeNameError").html("");
+    $("#root-type-name-modal").modal('show');
     $("#root-type-name-modal").modal({
         backdrop: 'static',
         keyboard: false
-    }, 'show');
+    })
 };
 
 
 /**
  * Change the name of root type
  */
 var changeRootTypeName = function() {
```

### Comparing `core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/js/build_template.raw.js` & `core_composer_app-2.4.0/core_composer_app/static/core_composer_app/user/js/build_template.raw.js`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/js/menus.js` & `core_composer_app-2.4.0/core_composer_app/static/core_composer_app/user/js/menus.js`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/js/xpath.js` & `core_composer_app-2.4.0/core_composer_app/static/core_composer_app/user/js/xpath.js`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/static/core_composer_app/user/xsl/xsd2html.xsl` & `core_composer_app-2.4.0/core_composer_app/static/core_composer_app/user/xsl/xsd2html.xsl`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/add_content.html` & `core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/buckets/edit_content.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %}
-{% load static %}
 
-{% block box_title %}Add {{ data.object_name }}{% endblock %}
+{% block box_title %}Edit {% endblock %}
 
 {% block box_tools %}
-{% url 'core-admin:core_composer_app_buckets' as bucket_list_url %}
-{% include 'core_main_app/common/buttons/go_to.html' with url=bucket_list_url label='Back to Buckets' %}
+
+{% url 'core-admin:core_composer_app_types' as type_list_url %}
+{% include 'core_main_app/common/buttons/go_to.html' with url=type_list_url label='Back to Types' %}
+
 {% endblock %}
 
 {% block box_body %}
 <div class="row">
     <div class="col-md-12">
-        <form id="form_start" action="{% url 'core-admin:core_composer_app_upload_bucket' %}" method="post">
+        {% for bucket in data.buckets %}
+            {% if data.version_manager in bucket.types %}
+                <span class="bucket" style="background:{{ bucket.color}};" bucketid="{{bucket.id}}">
+                    {{ bucket.label }}
+                </span>
+            {% endif %}
+        {% endfor %}
+        <form id="form_edit" method="post"
+              action="{% url 'core-admin:core_composer_app_type_buckets' data.version_manager.id %}">
             {% csrf_token %}
+
             {{ data.form }}
-            <div id="upload_errors" class="text-danger">
+
+            <div id="upload_errors" style="color:red;">
                 {{ data.errors | safe}}
             </div>
-            <button type="submit" class="btn btn-primary float-right mt-3">
-                <i class="fas fa-plus"></i> Add {{data.object_name}}
+
+            <button type="submit" class="btn btn-primary {% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3"%}float-end{% endif %} mt-3">
+                <i class="fas fa-save"></i> Save
             </button>
+
         </form>
     </div>
 </div>
 {% endblock %}
```

### Comparing `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/list/available.html` & `core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/buckets/list/available.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% extends 'core_main_app/admin/templates/list/available.html' %}
 
 
 {% block box_tools %}
-<a href="{% url 'core-admin:core_composer_app_upload_bucket' %}" class="float-right btn btn-secondary">
+<a href="{% url 'core-admin:core_composer_app_upload_bucket' %}" class="{% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3"%}float-end{% endif %} btn btn-secondary">
     <i class="fas fa-plus"></i> Add {{ data.object_name }}
 </a>
 {% endblock %}
 
 {% block box_body %}
 <table class="table table-bordered table-striped table-hover">
     <tr>
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 {% extends 'core_main_app/admin/templates/list/available.html' %} {% block
 box_tools %}
- Add_{{_data.object_name_}}
+.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3"%}float-end{% endif %}
+btn btn-secondary">  Add {{ data.object_name }}
  {% endblock %} {% block box_body %}
 {{ data.object_name }} Actions
                        {% url 'core-admin:core_composer_app_edit_bucket'
  {{ bucket.label }}    bucket.id as edit_url %} {% include 'core_main_app/
                        common/buttons/edit.html' %}    Delete
 No {{ data.object_name }} created yet.
 {% endblock %}
```

### Comparing `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/buckets/modals/delete.html` & `core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/modals/errors.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 {% extends 'core_main_app/_render/admin/theme/tools/modal.html' %}
 
-{% block modal_id %}delete-bucket-modal{% endblock %}
-{% block modal_title %}Delete Bucket{% endblock %}
+{% block modal_id %}error-modal{% endblock %}
+{% block modal_title %}Error{% endblock %}
 
 {% block modal_body %}
-<p>Are you sure you want to delete this bucket?</p>
-<div id="bucket_id" style="display:none;"></div>
+An error occurred:
+<div id="validate-error" class="text-danger">
+</div>
 {% endblock %}
 {% block modal_footer %}
-<button class="btn btn-secondary pull-left" data-dismiss="modal"><i class="fas fa-times"></i> Cancel</button>
-<button id="delete-bucket" class="btn btn-danger"><i class="fas fa-trash"></i> Delete</button>
+<a class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
 {% endblock %}
+
```

### Comparing `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/list/available.html` & `core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/types/list/available.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% extends 'core_main_app/admin/templates/list/available.html' %}
 
 
 {% block box_tools %}
-    <a href="{% url 'core-admin:core_composer_app_upload_type' %}" class="float-right btn btn-secondary">
+    <a href="{% url 'core-admin:core_composer_app_upload_type' %}" class="{% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3"%}float-end{% endif %} btn btn-secondary">
         <i class="fas fa-upload"></i> Upload {{ data.object_name }}
     </a>
 {% endblock %}
 
 {% block box_body %}
 <table class="table table-bordered table-striped table-hover">
     <tr>
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 {% extends 'core_main_app/admin/templates/list/available.html' %} {% block
 box_tools %}
- Upload_{{_data.object_name_}}
+.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3"%}float-end{% endif %}
+btn btn-secondary">  Upload {{ data.object_name }}
  {% endblock %} {% block box_body %}
 {{ data.object_name }} Buckets                     Actions
                                                     Versions
                                                     {% url 'core-admin:
                        {% for bucket in            core_composer_app_edit_type'
 {{ object.title }}     object.bucket_set.all %}  { object.id as edit_url %} {%
                        { bucket.label }}  {%       include 'core_main_app/
```

### Comparing `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/list/disabled.html` & `core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/types/list/disabled.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/admin/types/versions/available.html` & `core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/admin/types/versions/available.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 {% extends 'core_main_app/admin/templates/versions/available.html' %}
 
 {% block box_tools %}
 
 {% if not data.version_manager.user %}
 	<a href="{% url 'core-admin:core_composer_app_upload_type_version' data.version_manager.id %}"
-	   class="float-right btn btn-secondary">
+	   class="{% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3"%}float-end{% endif %}
+  			  {% if BOOTSTRAP_VERSION == "4.6.2" %}ml-1{% elif BOOTSTRAP_VERSION == "5.1.3"%}ms-1{% endif %}
+			  btn btn-secondary">
 		<i class="fas fa-upload"></i> Upload New Version
 	</a>
 {% endif %}
 
 {% url data.back_url as type_list_url %}
 {% include 'core_main_app/common/buttons/go_to.html' with url=type_list_url label='Back to Types' %}
```

#### html2text {}

```diff
@@ -1,10 +1,12 @@
 {% extends 'core_main_app/admin/templates/versions/available.html' %} {% block
 box_tools %} {% if not data.version_manager.user %}
- Upload_New_Version
+.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3"%}float-end{% endif %}
+{% if BOOTSTRAP_VERSION == "4.6.2" %}ml-1{% elif BOOTSTRAP_VERSION ==
+"5.1.3"%}ms-1{% endif %} btn btn-secondary">  Upload New Version
  {% endif %} {% url data.back_url as type_list_url %} {% include
 'core_main_app/common/buttons/go_to.html' with url=type_list_url label='Back to
 Types' %} {% endblock %}  {% block box_actions %} {% if 'core_parser_app' in
 INSTALLED_APPS %}
  Modules
  {% endif %} {% if version.object != data.version_manager.current %}
  Set_Current
```

### Comparing `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/change_type.html` & `core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/modals/change_type.html`

 * *Files 16% similar despite different names*

```diff
@@ -9,12 +9,14 @@
     <select id="newXSDtype">
         <option value="sequence">Sequence</option>
         <option value="choice">Choice</option>
     </select>
 </div>
 {% endblock %}
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
+<a class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#">
+    <i class="fas fa-times"></i> Cancel
+</a>
 <a id="change-element-type" class="btn btn-primary" href="#">
     <i class="fas fa-sync"></i> Update
 </a>
 {% endblock %}
```

### Comparing `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/delete_element.html` & `core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/modals/delete_element.html`

 * *Files 12% similar despite different names*

```diff
@@ -3,10 +3,10 @@
 {% block modal_id %}delete-element-modal{% endblock %}
 {% block modal_title %}Delete Element{% endblock %}
 
 {% block modal_body %}
 Are you sure you want to delete this element from the current template?
 {% endblock %}
 {% block modal_footer %}
-<button class="btn btn-secondary pull-left" data-dismiss="modal"><i class="fas fa-times"></i> Cancel</button>
+<button class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal"><i class="fas fa-times"></i> Cancel</button>
 <button id="delete-element" class="btn btn-danger"><i class="fas fa-trash"></i> Delete</button>
 {% endblock %}
```

### Comparing `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/element_name.html` & `core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/modals/element_name.html`

 * *Files 26% similar despite different names*

```diff
@@ -13,12 +13,12 @@
         </td>
     </tr>
 </table>
 <div id="rename-element-error" class="text-danger">
 </div>
 {% endblock %}
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
+<a class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
 <a id="rename-element" class="btn btn-primary" href="#">
     <i class="fas fa-pencil-alt"></i> Rename
 </a>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 {% extends 'core_main_app/_render/admin/theme/tools/modal.html' %} {% block
 modal_id %}element-name-modal{% endblock %} {% block modal_title %}Rename
 Element{% endblock %} {% block modal_body %} Use the following form to rename
 the element:
 Name: [                    ]
 {% endblock %} {% block modal_footer %}
- Cancel
+% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION ==
+"5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#"> Cancel
 
  Rename
  {% endblock %}
```

### Comparing `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/insert_element.html` & `core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/modals/insert_element.html`

 * *Files 16% similar despite different names*

```diff
@@ -5,24 +5,34 @@
 
 {% block modal_body %}
 <p>
 Please select the type of the element that you want to insert in the template.
 </p>
 <div id="table_types">
     {% for bucket in data.buckets %}
-    <h3><span class="bucket" style="background:{{ bucket.color}};">{{bucket.label}}</span></h3>
-    {% include 'core_composer_app/user/builder/list_types.html' with types=bucket.types.all %}
+        <h3>
+            <span class="bucket" style="background:{{bucket.color}};">
+                {{bucket.label}}
+            </span>
+        </h3>
+        {% include 'core_composer_app/user/builder/list_types.html' with types=bucket.types %}
     {% endfor %}
 
     <h3>Built-in Datatypes</h3>
     {% include 'core_composer_app/user/builder/list_types.html' with types=data.built_in_types %}
 
     <h3>No Buckets</h3>
     {% include 'core_composer_app/user/builder/list_types.html' with types=data.no_buckets_types %}
 
     <h3>My Types</h3>
     {% include 'core_composer_app/user/builder/list_types.html' with types=data.user_types %}
 </div>
 {% endblock %}
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
+<a class="btn btn-secondary pull-left"
+    {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss="modal"
+    {% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss="modal"
+    {% endif %}
+    href="#">
+    <i class="fas fa-times"></i> Cancel
+</a>
 {% endblock %}
```

### Comparing `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/occurrences.html` & `core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/modals/occurrences.html`

 * *Files 18% similar despite different names*

```diff
@@ -26,12 +26,12 @@
         </td>
     </tr>
 </table>
 <div id="manage-occurrences-error" class="text-danger">
 </div>
 {% endblock %}
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
+<a class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
 <a id="set-occurrences" class="btn btn-primary" href="#">
     <i class="fas fa-sync"></i> Update Occurrences
 </a>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 {% extends 'core_main_app/_render/admin/theme/tools/modal.html' %} {% block
 modal_id %}occurrences-modal{% endblock %} {% block modal_title %}Manage
 Occurrences{% endblock %} {% block modal_body %} Use the following form to
 manage the occurrences of the selected element. Accepted values are integers.
 Minimum Occurrences: [                    ]
 Maximum Occurrences: [                    ] Unbounded ⁰
 {% endblock %} {% block modal_footer %}
- Cancel
+% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION ==
+"5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#"> Cancel
 
  Update_Occurrences
  {% endblock %}
```

### Comparing `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/root_type_name.html` & `core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/modals/root_type_name.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_template.html` & `core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_type.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 {% extends 'core_main_app/_render/admin/theme/tools/modal.html' %}
 
-{% block modal_id %}save-template-modal{% endblock %}
-{% block modal_title %}Save Template{% endblock %}
+{% block modal_id %}save-type-modal{% endblock %}
+{% block modal_title %}Save Type{% endblock %}
 
 {% block modal_body %}
-<label for="newTemplateName">Name:</label>
-<input type="text" class="form-control" id="newTemplateName"/>
-<div id="new-template-error" class="text-danger">
+<label for="newTypeName">Name:</label>
+<input type="text" class="form-control" id="newTypeName"/>
+<div id="new-type-error" class="text-danger">
 </div>
 {% endblock %}
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
-<a id="save-template" class="btn btn-primary" href="#"><i class="fas fa-save"></i> Save</a>
+<a class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#">
+    <i class="fas fa-times"></i> Cancel
+</a>
+<a id="save-type" class="btn btn-primary" href="#"><i class="fas fa-save"></i> Save</a>
 {% endblock %}
```

### Comparing `core_composer_app-2.3.0/core_composer_app/templates/core_composer_app/user/index.html` & `core_composer_app-2.4.0/core_composer_app/templates/core_composer_app/user/index.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <a href="{% url 'core_composer_build_template' 'new' %}"
-       class="btn btn-success float-right" role="button">
+       class="btn btn-success {% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3"%}float-end{% endif %}" srole="button">
     <i class="fas fa-play"></i> Start Template or Type from scratch
 </a>
 
 <h2>Select Template</h2>
 
 <p>
     Start composing a new template or customize an existing template. It will automatically load the appropriate
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
- Start_Template_or_Type_from_scratch
+.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3"%}float-end{% endif %}"
+srole="button">  Start Template or Type from scratch
 ***** Select Template *****
 Start composing a new template or customize an existing template. It will
 automatically load the appropriate form and display it on the next page.
 **** Templates ****
 {% if data.global_templates or data.user_templates %}
 {% else %}
 No template uploaded yet.
```

### Comparing `core_composer_app-2.3.0/core_composer_app/urls.py` & `core_composer_app-2.4.0/core_composer_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/utils/xml.py` & `core_composer_app-2.4.0/core_composer_app/utils/xml.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/views/admin/ajax.py` & `core_composer_app-2.4.0/core_composer_app/views/admin/ajax.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/views/admin/forms.py` & `core_composer_app-2.4.0/core_composer_app/views/admin/forms.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/views/admin/views.py` & `core_composer_app-2.4.0/core_composer_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/core_composer_app/views/user/ajax.py` & `core_composer_app-2.4.0/core_composer_app/views/user/ajax.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """AJAX user views of composer application
 """
 import json
 import logging
 from urllib.parse import urlparse
 
+from django.contrib import messages
 from django.contrib.auth.decorators import login_required
 from django.http.response import HttpResponse, HttpResponseBadRequest
 from django.template import loader
 from django.utils.decorators import method_decorator
 from django.utils.html import escape
 from django.core.exceptions import ValidationError
 
@@ -389,14 +390,18 @@
             )
         except ValidationError:
             return HttpResponseBadRequest(
                 "Title must not be empty or only whitespaces."
             )
         except Exception as exception:
             return _error_response(escape(str(exception)))
+
+        messages.add_message(
+            request, messages.SUCCESS, "Template succesfully saved."
+        )
         return HttpResponse(
             json.dumps(response_dict), content_type="application/javascript"
         )
     except Exception as exception:
         return HttpResponseBadRequest(
             escape(str(exception)), content_type="application/javascript"
         )
@@ -485,14 +490,17 @@
         except ValidationError:
             return HttpResponseBadRequest(
                 "Title must not be empty or only whitespaces."
             )
         except Exception as exception:
             return _error_response(escape(str(exception)))
 
+        messages.add_message(
+            request, messages.SUCCESS, "Type succesfully saved."
+        )
         return HttpResponse(
             json.dumps(response_dict), content_type="application/javascript"
         )
     except Exception as exception:
         return HttpResponseBadRequest(
             escape(str(exception)), content_type="application/javascript"
         )
```

### Comparing `core_composer_app-2.3.0/core_composer_app/views/user/views.py` & `core_composer_app-2.4.0/core_composer_app/views/user/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,32 +134,40 @@
         join("core_composer_app", "user", "xsl", "xsd2html.xsl")
     )
     # reads XSLT
     xslt_string = read_file_content(xslt_path)
     # transform XML to HTML
     xsd_to_html_string = xsl_transform(xsd_string, xslt_string)
 
-    # 1) Get user defined types
+    # 1) Get user defined types.
     user_types = type_version_manager_api.get_version_managers_by_user(
         request=request
-    )
-    # 2) Get buckets
-    buckets = bucket_api.get_all()
+    ).filter(is_disabled=False)
+
+    # 2) Get buckets.
+    buckets = [
+        {
+            "label": bucket.label,
+            "color": bucket.color,
+            "types": bucket.types.filter(is_disabled=False),
+        }
+        for bucket in bucket_api.get_all()
+    ]
 
-    # 3) no_buckets_types: list of types that are not assigned to a specific bucket
+    # 3) no_buckets_types: list of types that are not assigned to a specific
+    #   bucket.
     no_buckets_types = type_version_manager_api.get_no_buckets_types(
         request=request
-    )
+    ).filter(is_disabled=False)
 
     # 4) Build list of built-in types
-    built_in_types = []
-    for built_in_type in get_xsd_types():
-        built_in_types.append(
-            {"current": "built_in_type", "title": built_in_type}
-        )
+    built_in_types = [
+        {"current": "built_in_type", "title": built_in_type}
+        for built_in_type in get_xsd_types()
+    ]
 
     assets = {
         "js": [
             {
                 "path": "core_composer_app/user/js/build_template.js",
                 "is_raw": False,
             },
@@ -195,15 +203,14 @@
         "core_composer_app/user/builder/modals/root_type_name.html",
         "core_composer_app/user/builder/modals/element_name.html",
         "core_composer_app/user/builder/modals/insert_element.html",
         "core_composer_app/user/builder/modals/delete_element.html",
         "core_composer_app/user/builder/modals/change_type.html",
         "core_composer_app/user/builder/modals/save_template.html",
         "core_composer_app/user/builder/modals/save_type.html",
-        "core_composer_app/user/builder/modals/save_success.html",
         "core_composer_app/user/builder/modals/occurrences.html",
         "core_composer_app/user/builder/modals/errors.html",
     ]
 
     # Set page title
     context.update({"page_title": "Build Template"})
```

### Comparing `core_composer_app-2.3.0/core_composer_app.egg-info/PKG-INFO` & `core_composer_app-2.4.0/core_composer_app.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-composer-app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Template and type composer for the curator core project
 Home-page: https://github.com/usnistgov/core_composer_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =================
         Core Composer App
```

### Comparing `core_composer_app-2.3.0/core_composer_app.egg-info/SOURCES.txt` & `core_composer_app-2.4.0/core_composer_app.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -82,15 +82,14 @@
 core_composer_app/templates/core_composer_app/user/builder/modals/change_type.html
 core_composer_app/templates/core_composer_app/user/builder/modals/delete_element.html
 core_composer_app/templates/core_composer_app/user/builder/modals/element_name.html
 core_composer_app/templates/core_composer_app/user/builder/modals/errors.html
 core_composer_app/templates/core_composer_app/user/builder/modals/insert_element.html
 core_composer_app/templates/core_composer_app/user/builder/modals/occurrences.html
 core_composer_app/templates/core_composer_app/user/builder/modals/root_type_name.html
-core_composer_app/templates/core_composer_app/user/builder/modals/save_success.html
 core_composer_app/templates/core_composer_app/user/builder/modals/save_template.html
 core_composer_app/templates/core_composer_app/user/builder/modals/save_type.html
 core_composer_app/templates/core_composer_app/user/list/list.html
 core_composer_app/templates/core_composer_app/user/types/versions.html
 core_composer_app/templates/core_composer_app/user/types/versions/available.html
 core_composer_app/utils/__init__.py
 core_composer_app/utils/xml.py
@@ -123,8 +122,15 @@
 tests/rest/bucket/__init__.py
 tests/rest/bucket/tests_int.py
 tests/rest/bucket/tests_permission.py
 tests/rest/type_version_manager/__init__.py
 tests/rest/type_version_manager/tests_int.py
 tests/rest/type_version_manager/tests_permission.py
 tests/utils/__init__.py
-tests/utils/tests_unit.py
+tests/utils/tests_unit.py
+tests/views/__init__.py
+tests/views/user/__init__.py
+tests/views/user/ajax/__init__.py
+tests/views/user/ajax/tests_permissions.py
+tests/views/user/ajax/tests_unit.py
+tests/views/user/views/__init__.py
+tests/views/user/views/tests_unit.py
```

### Comparing `core_composer_app-2.3.0/docs/conf.py` & `core_composer_app-2.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/setup.py` & `core_composer_app-2.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_composer_app",
-    version="2.3.0",
+    version="2.4.0",
     description="Template and type composer for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_composer_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_composer_app-2.3.0/tests/components/bucket/fixtures/fixtures.py` & `core_composer_app-2.4.0/tests/components/bucket/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/tests/components/bucket/tests_unit.py` & `core_composer_app-2.4.0/tests/components/bucket/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/tests/components/type/tests_unit.py` & `core_composer_app-2.4.0/tests/components/type/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/tests/components/type_version_manager/fixtures/fixtures.py` & `core_composer_app-2.4.0/tests/components/type_version_manager/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/tests/components/type_version_manager/tests_int_access_control.py` & `core_composer_app-2.4.0/tests/components/type_version_manager/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/tests/components/type_version_manager/tests_unit.py` & `core_composer_app-2.4.0/tests/components/type_version_manager/tests_unit.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """Type Version Manager test cases
 """
 from unittest.case import TestCase
+from unittest.mock import Mock, patch, MagicMock
 
 from django.core import exceptions as django_exceptions
 from django.db import IntegrityError
 from django.test import override_settings
-from unittest.mock import Mock, patch
 
-from core_main_app.commons.exceptions import CoreError, ModelError
-from core_main_app.utils.tests_tools.MockUser import create_mock_user
-from core_main_app.utils.tests_tools.RequestMock import create_mock_request
 from core_composer_app.components.bucket.models import Bucket
 from core_composer_app.components.type.models import Type
 from core_composer_app.components.type_version_manager import (
     api as version_manager_api,
 )
 from core_composer_app.components.type_version_manager.api import (
     get_no_buckets_types,
 )
 from core_composer_app.components.type_version_manager.models import (
     TypeVersionManager,
 )
+from core_main_app.commons.exceptions import CoreError, ModelError
+from core_main_app.utils.tests_tools.MockUser import create_mock_user
+from core_main_app.utils.tests_tools.RequestMock import create_mock_request
 
 
 class TestTypeVersionManagerInsert(TestCase):
     """Test Type Version Manager Insert"""
 
     @patch.object(TypeVersionManager, "save")
     @patch.object(Type, "save")
@@ -332,68 +332,28 @@
         """test_get_no_buckets_types_returns_types"""
 
         # Arrange
         mock_user = create_mock_user("1", is_superuser=True)
         mock_request = create_mock_request(user=mock_user)
         mock_type1 = _create_mock_type_version_manager()
         mock_type2 = _create_mock_type_version_manager()
-        mock_get_global_version_managers.return_value = [
+        mock_bucket = _create_mock_bucket(
+            types=[_create_mock_type_version_manager()]
+        )
+        mock_get_global_version_managers.exclude.return_value = [
             mock_type1,
             mock_type2,
         ]
-        mock_get_all_buckets.return_value = []
+        mock_get_all_buckets.return_value = [mock_bucket]
 
         result = get_no_buckets_types(request=mock_request)
         self.assertTrue(
             all(isinstance(item, TypeVersionManager) for item in result)
         )
 
-    @patch.object(TypeVersionManager, "get_global_version_managers")
-    @patch.object(Bucket, "get_all")
-    def test_get_no_buckets_types_returns_all_types_if_no_buckets(
-        self, mock_get_all_buckets, mock_get_global_version_managers
-    ):
-        """test_get_no_buckets_types_returns_all_types_if_no_buckets"""
-
-        # Arrange
-        mock_user = create_mock_user("1", is_superuser=True)
-        mock_request = create_mock_request(user=mock_user)
-        mock_type1 = _create_mock_type_version_manager()
-        mock_type2 = _create_mock_type_version_manager()
-        mock_get_global_version_managers.return_value = [
-            mock_type1,
-            mock_type2,
-        ]
-        mock_get_all_buckets.return_value = []
-
-        self.assertTrue(len(get_no_buckets_types(request=mock_request)) == 2)
-
-    @patch.object(TypeVersionManager, "get_global_version_managers")
-    @patch.object(Bucket, "get_all")
-    def test_get_no_buckets_types_returns_all_types_not_in_buckets(
-        self, mock_get_all_buckets, mock_get_global_version_managers
-    ):
-        """test_get_no_buckets_types_returns_all_types_not_in_buckets"""
-
-        # Arrange
-        mock_user = create_mock_user("1", is_superuser=True)
-        mock_request = create_mock_request(user=mock_user)
-        mock_type1 = _create_mock_type_version_manager()
-        mock_type2 = _create_mock_type_version_manager()
-
-        mock_bucket = _create_mock_bucket(types=MockTypes([mock_type1]))
-
-        mock_get_global_version_managers.return_value = [
-            mock_type1,
-            mock_type2,
-        ]
-        mock_get_all_buckets.return_value = [mock_bucket]
-
-        self.assertTrue(len(get_no_buckets_types(request=mock_request)) == 1)
-
 
 def _create_mock_bucket(types=None):
     """Returns a mock bucket
 
     Args:
         types:
 
@@ -401,15 +361,18 @@
 
     """
     if types is None:
         types = []
     mock_bucket = Mock(spec=Bucket)
     mock_bucket.label = "bucket"
     mock_bucket.label = "#000000"
-    mock_bucket.types = types
+
+    mock_bucket_types = MagicMock()
+    mock_bucket_types.all.return_value = types
+    mock_bucket.types = mock_bucket_types
     return mock_bucket
 
 
 def _create_mock_type(filename="", content="", is_disable=False):
     """Returns a mock type
 
     Args:
```

### Comparing `core_composer_app-2.3.0/tests/rest/bucket/tests_int.py` & `core_composer_app-2.4.0/tests/rest/bucket/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/tests/rest/bucket/tests_permission.py` & `core_composer_app-2.4.0/tests/rest/bucket/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/tests/rest/type_version_manager/tests_int.py` & `core_composer_app-2.4.0/tests/rest/type_version_manager/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/tests/rest/type_version_manager/tests_permission.py` & `core_composer_app-2.4.0/tests/rest/type_version_manager/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/tests/test_settings.py` & `core_composer_app-2.4.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.3.0/tests/utils/tests_unit.py` & `core_composer_app-2.4.0/tests/utils/tests_unit.py`

 * *Files identical despite different names*

