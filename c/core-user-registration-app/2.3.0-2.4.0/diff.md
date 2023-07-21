# Comparing `tmp/core_user_registration_app-2.3.0.tar.gz` & `tmp/core_user_registration_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_user_registration_app-2.3.0.tar", last modified: Tue May  2 19:48:15 2023, max compression
+gzip compressed data, was "core_user_registration_app-2.4.0.tar", last modified: Fri Jul 21 02:17:11 2023, max compression
```

## Comparing `core_user_registration_app-2.3.0.tar` & `core_user_registration_app-2.4.0.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.904388 core_user_registration_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      185 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1068 2023-05-02 19:48:15.899420 core_user_registration_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      586 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.580563 core_user_registration_app-2.3.0/core_user_registration_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.682874 core_user_registration_app-2.3.0/core_user_registration_app/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3113 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/access_control/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2683 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      521 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.699214 core_user_registration_app-2.3.0/core_user_registration_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.748676 core_user_registration_app-2.3.0/core_user_registration_app/components/account_request_metadata/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/account_request_metadata/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2833 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/account_request_metadata/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      721 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/account_request_metadata/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.798073 core_user_registration_app-2.3.0/core_user_registration_app/components/user_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/user_data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2624 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/user_data_structure/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5373 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/user_data_structure/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.851112 core_user_registration_app-2.3.0/core_user_registration_app/components/user_metadata/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/user_metadata/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1566 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/user_metadata/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2025 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/user_metadata/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.912566 core_user_registration_app-2.3.0/core_user_registration_app/components/user_template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/user_template_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1299 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/user_template_version_manager/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3131 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/user_template_version_manager/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2628 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/components/user_template_version_manager/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6592 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      514 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.942612 core_user_registration_app-2.3.0/core_user_registration_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7426 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      642 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.974551 core_user_registration_app-2.3.0/core_user_registration_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      190 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/permissions/rights.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1596 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.157791 core_user_registration_app-2.3.0/core_user_registration_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.200086 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.164333 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.002267 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/admin/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      211 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/admin/js/view_meta.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       83 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/admin/js/view_meta.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.175344 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.189019 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/common/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.028253 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      650 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/set_current.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/set_current.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.053501 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      652 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/set_current.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      125 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/set_current.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.208463 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.147769 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      934 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/js/autosave.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      100 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/js/autosave.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      756 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/js/report_data.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/js/report_data.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1049 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/js/save_data.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/js/save_data.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.164496 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/xsd/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      559 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/xsd/user.xsd
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.192499 core_user_registration_app-2.3.0/core_user_registration_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2012 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/system/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1541 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.238794 core_user_registration_app-2.3.0/core_user_registration_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.266605 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.210960 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.225502 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/account_requests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1849 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/account_requests/pending.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.256444 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.272293 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1712 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      514 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.292578 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3152 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      615 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      338 2023-05-02 19:48:11.000000 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/user_requests.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.320739 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1003 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/user/account_creation.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1188 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/user/request_new_account.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1623 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/core_user_registration_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.335296 core_user_registration_app-2.3.0/core_user_registration_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/core_user_registration_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.381651 core_user_registration_app-2.3.0/core_user_registration_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/core_user_registration_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1592 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/core_user_registration_app/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14677 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/core_user_registration_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.422731 core_user_registration_app-2.3.0/core_user_registration_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/core_user_registration_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5566 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/core_user_registration_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7456 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/core_user_registration_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:14.654182 core_user_registration_app-2.3.0/core_user_registration_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1068 2023-05-02 19:48:13.000000 core_user_registration_app-2.3.0/core_user_registration_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5457 2023-05-02 19:48:14.000000 core_user_registration_app-2.3.0/core_user_registration_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:48:13.000000 core_user_registration_app-2.3.0/core_user_registration_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-05-02 19:48:13.000000 core_user_registration_app-2.3.0/core_user_registration_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       33 2023-05-02 19:48:13.000000 core_user_registration_app-2.3.0/core_user_registration_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       91 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:48:15.906557 core_user_registration_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      939 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.464506 core_user_registration_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.479256 core_user_registration_app-2.3.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.519677 core_user_registration_app-2.3.0/tests/components/account_request_metadata/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/account_request_metadata/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2900 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/account_request_metadata/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.533621 core_user_registration_app-2.3.0/tests/components/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.581114 core_user_registration_app-2.3.0/tests/components/user/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1119 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user/fixtures/fixtures.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.647807 core_user_registration_app-2.3.0/tests/components/user_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_data_structure/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.688272 core_user_registration_app-2.3.0/tests/components/user_data_structure/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_data_structure/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2343 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_data_structure/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7919 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_data_structure/test_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3204 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_data_structure/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.744933 core_user_registration_app-2.3.0/tests/components/user_metadata/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_metadata/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.776563 core_user_registration_app-2.3.0/tests/components/user_metadata/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_metadata/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4808 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_metadata/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4649 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_metadata/test_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1062 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_metadata/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.809754 core_user_registration_app-2.3.0/tests/components/user_template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_template_version_manager/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.842400 core_user_registration_app-2.3.0/tests/components/user_template_version_manager/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_template_version_manager/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2472 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_template_version_manager/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6623 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/components/user_template_version_manager/test_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2150 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2121 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.858207 core_user_registration_app-2.3.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:15.878117 core_user_registration_app-2.3.0/tests/views/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:48:12.000000 core_user_registration_app-2.3.0/tests/views/ajax/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.746476 core_user_registration_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      185 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1068 2023-07-21 02:17:11.742241 core_user_registration_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      586 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:10.592799 core_user_registration_app-2.4.0/core_user_registration_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:10.675946 core_user_registration_app-2.4.0/core_user_registration_app/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3113 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/access_control/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2683 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      521 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:10.687923 core_user_registration_app-2.4.0/core_user_registration_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:10.720820 core_user_registration_app-2.4.0/core_user_registration_app/components/account_request_metadata/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/components/account_request_metadata/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2833 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/components/account_request_metadata/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      721 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/components/account_request_metadata/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:10.777266 core_user_registration_app-2.4.0/core_user_registration_app/components/user_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/components/user_data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2624 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/components/user_data_structure/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5373 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/components/user_data_structure/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:10.814481 core_user_registration_app-2.4.0/core_user_registration_app/components/user_metadata/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/components/user_metadata/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1566 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/components/user_metadata/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2025 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/components/user_metadata/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:10.863471 core_user_registration_app-2.4.0/core_user_registration_app/components/user_template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/components/user_template_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1299 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/components/user_template_version_manager/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3131 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/components/user_template_version_manager/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2628 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/components/user_template_version_manager/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6592 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      514 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:10.890151 core_user_registration_app-2.4.0/core_user_registration_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7426 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      642 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:10.917341 core_user_registration_app-2.4.0/core_user_registration_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      190 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/permissions/rights.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1596 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:10.229894 core_user_registration_app-2.4.0/core_user_registration_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:10.273787 core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:10.235650 core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:10.943891 core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/admin/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      211 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/admin/js/view_meta.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       83 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/admin/js/view_meta.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:10.245595 core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:10.248847 core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/common/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:10.977957 core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      660 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/set_current.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/set_current.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.009687 core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      662 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/set_current.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      125 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/set_current.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:10.289638 core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.097092 core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      934 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/user/js/autosave.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      100 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/user/js/autosave.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      756 2023-07-21 02:17:07.000000 core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/user/js/report_data.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/user/js/report_data.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1049 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/user/js/save_data.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/user/js/save_data.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.109456 core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/user/xsd/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      559 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/user/xsd/user.xsd
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.136595 core_user_registration_app-2.4.0/core_user_registration_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/core_user_registration_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2012 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/core_user_registration_app/system/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1541 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/core_user_registration_app/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:10.303733 core_user_registration_app-2.4.0/core_user_registration_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:10.327445 core_user_registration_app-2.4.0/core_user_registration_app/templates/core_user_registration_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.154942 core_user_registration_app-2.4.0/core_user_registration_app/templates/core_user_registration_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.168253 core_user_registration_app-2.4.0/core_user_registration_app/templates/core_user_registration_app/admin/account_requests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1846 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/core_user_registration_app/templates/core_user_registration_app/admin/account_requests/pending.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.196514 core_user_registration_app-2.4.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.210194 core_user_registration_app-2.4.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1807 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      514 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.223368 core_user_registration_app-2.4.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3394 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      615 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      338 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/core_user_registration_app/templates/core_user_registration_app/admin/user_requests.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.249076 core_user_registration_app-2.4.0/core_user_registration_app/templates/core_user_registration_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1003 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/core_user_registration_app/templates/core_user_registration_app/user/account_creation.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1283 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/core_user_registration_app/templates/core_user_registration_app/user/request_new_account.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1625 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/core_user_registration_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.263995 core_user_registration_app-2.4.0/core_user_registration_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/core_user_registration_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.309848 core_user_registration_app-2.4.0/core_user_registration_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/core_user_registration_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1592 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/core_user_registration_app/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14677 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/core_user_registration_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.349476 core_user_registration_app-2.4.0/core_user_registration_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/core_user_registration_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5566 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/core_user_registration_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7456 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/core_user_registration_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:10.654366 core_user_registration_app-2.4.0/core_user_registration_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1068 2023-07-21 02:17:09.000000 core_user_registration_app-2.4.0/core_user_registration_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5457 2023-07-21 02:17:10.000000 core_user_registration_app-2.4.0/core_user_registration_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:17:09.000000 core_user_registration_app-2.4.0/core_user_registration_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-07-21 02:17:09.000000 core_user_registration_app-2.4.0/core_user_registration_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       33 2023-07-21 02:17:09.000000 core_user_registration_app-2.4.0/core_user_registration_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       91 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:17:11.748092 core_user_registration_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      939 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.392713 core_user_registration_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.408677 core_user_registration_app-2.4.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.442714 core_user_registration_app-2.4.0/tests/components/account_request_metadata/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/components/account_request_metadata/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2900 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/components/account_request_metadata/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.456064 core_user_registration_app-2.4.0/tests/components/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/components/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.496815 core_user_registration_app-2.4.0/tests/components/user/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/components/user/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1119 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/components/user/fixtures/fixtures.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.534095 core_user_registration_app-2.4.0/tests/components/user_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/components/user_data_structure/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.559797 core_user_registration_app-2.4.0/tests/components/user_data_structure/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/components/user_data_structure/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2343 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/components/user_data_structure/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7919 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/components/user_data_structure/test_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3204 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/components/user_data_structure/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.600420 core_user_registration_app-2.4.0/tests/components/user_metadata/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/components/user_metadata/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.628190 core_user_registration_app-2.4.0/tests/components/user_metadata/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/components/user_metadata/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4808 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/components/user_metadata/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4649 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/components/user_metadata/test_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1062 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/components/user_metadata/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.655132 core_user_registration_app-2.4.0/tests/components/user_template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/components/user_template_version_manager/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.681556 core_user_registration_app-2.4.0/tests/components/user_template_version_manager/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/components/user_template_version_manager/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2472 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/components/user_template_version_manager/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6623 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/components/user_template_version_manager/test_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2103 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2123 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.694854 core_user_registration_app-2.4.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:11.711176 core_user_registration_app-2.4.0/tests/views/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:17:08.000000 core_user_registration_app-2.4.0/tests/views/ajax/__init__.py
```

### Comparing `core_user_registration_app-2.3.0/LICENSE.md` & `core_user_registration_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/PKG-INFO` & `core_user_registration_app-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_user_registration_app
-Version: 2.3.0
+Version: 2.4.0
 Summary: User registration module for the core project
 Home-page: https://github.com/usnistgov/core_user_registration_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_user_registration_app
         ==========================
```

### Comparing `core_user_registration_app-2.3.0/README.rst` & `core_user_registration_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/access_control/api.py` & `core_user_registration_app-2.4.0/core_user_registration_app/access_control/api.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/admin.py` & `core_user_registration_app-2.4.0/core_user_registration_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/apps.py` & `core_user_registration_app-2.4.0/core_user_registration_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/components/account_request_metadata/api.py` & `core_user_registration_app-2.4.0/core_user_registration_app/components/account_request_metadata/api.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/components/account_request_metadata/models.py` & `core_user_registration_app-2.4.0/core_user_registration_app/components/account_request_metadata/models.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/components/user_data_structure/api.py` & `core_user_registration_app-2.4.0/core_user_registration_app/components/user_data_structure/api.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/components/user_data_structure/models.py` & `core_user_registration_app-2.4.0/core_user_registration_app/components/user_data_structure/models.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/components/user_metadata/api.py` & `core_user_registration_app-2.4.0/core_user_registration_app/components/user_metadata/api.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/components/user_metadata/models.py` & `core_user_registration_app-2.4.0/core_user_registration_app/components/user_metadata/models.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/components/user_template_version_manager/access_control.py` & `core_user_registration_app-2.4.0/core_user_registration_app/components/user_template_version_manager/access_control.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/components/user_template_version_manager/api.py` & `core_user_registration_app-2.4.0/core_user_registration_app/components/user_template_version_manager/api.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/components/user_template_version_manager/models.py` & `core_user_registration_app-2.4.0/core_user_registration_app/components/user_template_version_manager/models.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/discover.py` & `core_user_registration_app-2.4.0/core_user_registration_app/discover.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/menus.py` & `core_user_registration_app-2.4.0/core_user_registration_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/migrations/0001_initial.py` & `core_user_registration_app-2.4.0/core_user_registration_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/models.py` & `core_user_registration_app-2.4.0/core_user_registration_app/models.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/settings.py` & `core_user_registration_app-2.4.0/core_user_registration_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/set_current.js` & `core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/set_current.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -8,24 +8,21 @@
 
 /**
  * AJAX call, sets the current version
  * @param objectID id of the object
  */
 set_current_version = function(objectID) {
     $.ajax({
-        url: setCurrentVersionPostUrl,
-        type: "GET",
-        data: {
-            id: objectID
-        },
+        url: setCurrentVersionPostUrl.replace('template_version_id', objectID),
+        type: "PATCH",
         success: function(data) {
             location.reload();
         },
         error: function(data) {
-            $.notify(data.responseText);
+            $.notify(data.responseJSON["message"], "danger");
         }
     });
 };
 
 $(document).ready(function() {
     $('.current').on('click', setCurrentVersion);
 });
```

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/set_current.js` & `core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/set_current.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -8,21 +8,24 @@
 
 /**
  * AJAX call, sets the current version
  * @param objectID id of the object
  */
 set_current_version = function(objectID) {
     $.ajax({
-        url: setCurrentVersionPostUrl.replace('template_version_id', objectID),
-        type: "PATCH",
+        url: setCurrentVersionPostUrl,
+        type: "GET",
+        data: {
+            id: objectID
+        },
         success: function(data) {
             location.reload();
         },
         error: function(data) {
-            $.notify(data.responseJSON["message"]);
+            $.notify(data.responseText, "danger");
         }
     });
 };
 
 $(document).ready(function() {
     $('.current').on('click', setCurrentVersion);
 });
```

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/js/autosave.js` & `core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/user/js/autosave.js`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/js/report_data.js` & `core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/user/js/report_data.js`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/js/save_data.js` & `core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/user/js/save_data.js`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/static/core_user_registration_app/user/xsd/user.xsd` & `core_user_registration_app-2.4.0/core_user_registration_app/static/core_user_registration_app/user/xsd/user.xsd`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/system/api.py` & `core_user_registration_app-2.4.0/core_user_registration_app/system/api.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/tasks.py` & `core_user_registration_app-2.4.0/core_user_registration_app/tasks.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/account_requests/pending.html` & `core_user_registration_app-2.4.0/core_user_registration_app/templates/core_user_registration_app/admin/account_requests/pending.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %}
 {% load timestamptags %}
+{% load tz %}
 
 {% block box_title %}Pending requests{% endblock %}
 
 {% block box_body %}
 <table class="table table-bordered table-striped table-hover">
     <tr>
         <th width="10%">User</th>
@@ -24,15 +25,15 @@
         <tr id="{{ request.id }}" metadata="{{request.metadata.id}} ">
 
             {# FIXME add link to /admin/auth/user #}
             <td>{{ request.username }}</td>
             <td>{{ request.first_name }}</td>
             <td>{{ request.last_name }}</td>
             <td>{{ request.email }}</td>
-            <td>{{ request.date|print_datetime_utc_unaware }}</td>
+            <td>{{ request.date|localtime }}</td>
             <td>
                 <div class="btn btn-success accept_request">
                     <i class="fa fa-check"></i> Accept
                 </div>
                 <div class="btn btn-danger deny_request">
                     <i class="fa fa-times"></i> Deny
                 </div>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% load
-timestamptags %} {% block box_title %}Pending requests{% endblock %} {% block
-box_body %}
-User             First Name         Late Name         Email Address Date                                    Actions Metadata
-{                {                  {                 {             {                                               {% if
-{                {                  {                 {             {                                        Accept request.metadata
-request.username request.first_name request.last_name request.email request.date|print_datetime_utc_unaware  Deny   %}
-}}               }}                 }}                }}            }}                                               View metadata
-                                                                                                                    {% endif %}
+timestamptags %} {% load tz %} {% block box_title %}Pending requests{% endblock
+%} {% block box_body %}
+User             First Name         Late Name         Email Address Date                   Actions Metadata
+{                {                  {                 {             {                              {% if
+{                {                  {                 {             {                       Accept request.metadata
+request.username request.first_name request.last_name request.email request.date|localtime  Deny   %}
+}}               }}                 }}                }}            }}                              View metadata
+                                                                                                   {% endif %}
 No account requests pending at the moment.
 {% endblock %}
```

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list/available.html` & `core_user_registration_app-2.4.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list/available.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %}
 
 {% block box_title %}Available{% endblock %}
 
 {% block box_tools %}
-    <a href="{% url 'admin:core_user_registration_app_upload_template'%}" class="float-right btn btn-secondary">
+    <a href="{% url 'admin:core_user_registration_app_upload_template'%}" class="{% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3"%}float-end{% endif %} btn btn-secondary">
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
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% block
 box_title %}Available{% endblock %} {% block box_tools %}
- Upload_{{_data.object_name_}}
+.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3"%}float-end{% endif %}
+btn btn-secondary">  Upload {{ data.object_name }}
  {% endblock %} {% block box_body %}
 {{ data.object_name }} Status       Actions
                                              {% block box_actions %}
                                               Versions
 {{ object.title }}     Current      Uploaded  {% endblock %} {% if
                                              object.is_default %} {% else %}
                                               Set_Current
```

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list.html` & `core_user_registration_app-2.4.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list.html`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions.html` & `core_user_registration_app-2.4.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions.html`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/user/account_creation.html` & `core_user_registration_app-2.4.0/core_user_registration_app/templates/core_user_registration_app/user/account_creation.html`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/templates/core_user_registration_app/user/request_new_account.html` & `core_user_registration_app-2.4.0/core_user_registration_app/templates/core_user_registration_app/user/request_new_account.html`

 * *Files 24% similar despite different names*

```diff
@@ -22,13 +22,13 @@
                   <small class="text-muted">{{ field.help_text }}</small>
                 {% endif %}
                 {% for error in field.errors %}
                   <p class="text-danger">{{ error }}</p>
                 {% endfor %}
               </div>
             {% endfor %}
-            <button type="submit" class="btn btn-lg btn-secondary float-right">
+            <button type="submit" class="btn btn-lg btn-secondary {% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3"%}float-end{% endif %}">
                 <i class="fa fa-paper-plane"></i> Send Request
             </button>
         </form>
     </div>
 </div>
```

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/urls.py` & `core_user_registration_app-2.4.0/core_user_registration_app/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 import core_user_registration_app.views.user.ajax as user_ajax
 import core_user_registration_app.views.user.views as registration_views
 
 urlpatterns = [
     re_path("captcha/", include("captcha.urls")),
     re_path(
-        r"^account-request",
+        r"^account-request/$",
         registration_views.request_new_account,
         name="core_user_registration_app_account_request",
     ),
     re_path(
         r"^request-metadata/(?P<objectid>\w+)/(?P<accountid>\w+)$",
         registration_views.AccountCreationView.as_view(),
         name="core_user_registration_app_account_metadata",
```

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/views/admin/ajax.py` & `core_user_registration_app-2.4.0/core_user_registration_app/views/admin/ajax.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/views/admin/views.py` & `core_user_registration_app-2.4.0/core_user_registration_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/views/user/ajax.py` & `core_user_registration_app-2.4.0/core_user_registration_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app/views/user/views.py` & `core_user_registration_app-2.4.0/core_user_registration_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app.egg-info/PKG-INFO` & `core_user_registration_app-2.4.0/core_user_registration_app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-user-registration-app
-Version: 2.3.0
+Version: 2.4.0
 Summary: User registration module for the core project
 Home-page: https://github.com/usnistgov/core_user_registration_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_user_registration_app
         ==========================
```

### Comparing `core_user_registration_app-2.3.0/core_user_registration_app.egg-info/SOURCES.txt` & `core_user_registration_app-2.4.0/core_user_registration_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/setup.py` & `core_user_registration_app-2.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_user_registration_app",
-    version="2.3.0",
+    version="2.4.0",
     description="User registration module for the core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_user_registration_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_user_registration_app-2.3.0/tests/components/account_request_metadata/tests_unit.py` & `core_user_registration_app-2.4.0/tests/components/account_request_metadata/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/tests/components/user/fixtures/fixtures.py` & `core_user_registration_app-2.4.0/tests/components/user/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/tests/components/user_data_structure/fixtures/fixtures.py` & `core_user_registration_app-2.4.0/tests/components/user_data_structure/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/tests/components/user_data_structure/test_int_access_control.py` & `core_user_registration_app-2.4.0/tests/components/user_data_structure/test_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/tests/components/user_data_structure/tests_unit.py` & `core_user_registration_app-2.4.0/tests/components/user_data_structure/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/tests/components/user_metadata/fixtures/fixtures.py` & `core_user_registration_app-2.4.0/tests/components/user_metadata/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/tests/components/user_metadata/test_int.py` & `core_user_registration_app-2.4.0/tests/components/user_metadata/test_int.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/tests/components/user_metadata/test_unit.py` & `core_user_registration_app-2.4.0/tests/components/user_metadata/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/tests/components/user_template_version_manager/fixtures/fixtures.py` & `core_user_registration_app-2.4.0/tests/components/user_template_version_manager/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/tests/components/user_template_version_manager/test_int_access_control.py` & `core_user_registration_app-2.4.0/tests/components/user_template_version_manager/test_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.3.0/tests/test_settings.py` & `core_user_registration_app-2.4.0/tests/test_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,14 @@
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

### Comparing `core_user_registration_app-2.3.0/tests/urls.py` & `core_user_registration_app-2.4.0/tests/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import core_user_registration_app.views.user.ajax as user_ajax
 import core_user_registration_app.views.user.views as registration_views
 from core_main_app.rest.template import views as template_views
 
 urlpatterns = [
     re_path("captcha/", include("captcha.urls")),
     re_path(
-        r"^account-request",
+        r"^account-request/$",
         registration_views.request_new_account,
         name="core_user_registration_app_account_request",
     ),
     re_path(
         r"^request-metadata/(?P<objectid>\w+)/(?P<accountid>\w+)$",
         registration_views.AccountCreationView.as_view(),
         name="core_user_registration_app_account_metadata",
```

