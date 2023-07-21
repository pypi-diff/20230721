# Comparing `tmp/core_dashboard_common_app-2.3.0.tar.gz` & `tmp/core_dashboard_common_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_dashboard_common_app-2.3.0.tar", last modified: Tue May  2 19:36:25 2023, max compression
+gzip compressed data, was "core_dashboard_common_app-2.4.0.tar", last modified: Fri Jul 21 02:10:32 2023, max compression
```

## Comparing `core_dashboard_common_app-2.3.0.tar` & `core_dashboard_common_app-2.4.0.tar`

### file list

```diff
@@ -1,121 +1,129 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.677626 core_dashboard_common_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:36:18.000000 core_dashboard_common_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      158 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      865 2023-05-02 19:36:25.669894 core_dashboard_common_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      406 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.207888 core_dashboard_common_app-2.3.0/core_dashboard_common_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3824 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/constants.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1250 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:23.878860 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:23.950492 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:23.885731 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.420200 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      302 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/action_dashboard.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      441 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/count_checked.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      393 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/get_selected_document_admin.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      237 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/init_admin_menu.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.448260 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       71 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/list/view_record.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/my_dashboard_tabs.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      697 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/reset_checkbox.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      241 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/select_all.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:23.937729 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.535618 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      117 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/content_query.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       35 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/list.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       65 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/password_form.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.601246 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2023-05-02 19:36:20.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/init_pagination.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.684586 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1034 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_document.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_form.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_record.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_template.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      427 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/view_record.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1277 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/persistent_query_config.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:23.958713 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.706879 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      831 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/css/exploreTabs.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.829157 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      150 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/get_selected_document.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      577 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       83 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init_user.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.876339 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      836 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/edit_record.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       61 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/edit_record.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.968684 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1714 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/change_owner.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/change_owner.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1331 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/delete_document.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/delete_document.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1613 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/edit_persistent_query.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/edit_query.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/view_record.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       56 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/my_dashboard_tabs.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:23.998946 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.061246 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.081713 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      380 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/admin/dashboard.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.019766 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.103294 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/pagination/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2701 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/pagination/data_source_pagination.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      123 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/home.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.292960 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.335120 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      847 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/change_owner.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1053 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/delete_document.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      868 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/edit_persistent_query.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3055 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_files_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2804 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4709 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_queries_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      211 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_queries_table_pagination.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3575 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      222 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table_datatable.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      258 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table_pagination.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2809 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_templates_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2476 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_types_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3233 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_workspaces_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1927 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_dashboard.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1415 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      187 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile_change_password.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      759 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile_edit.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1007 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/password_change.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.379547 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templatetags/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templatetags/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      804 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templatetags/draft_extras.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      453 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/templatetags/special_plural.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.394954 core_dashboard_common_app-2.3.0/core_dashboard_common_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.458164 core_dashboard_common_app-2.3.0/core_dashboard_common_app/views/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/views/common/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18721 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/views/common/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1192 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/views/common/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    56102 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app/views/common/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:24.280379 core_dashboard_common_app-2.3.0/core_dashboard_common_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      865 2023-05-02 19:36:23.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6113 2023-05-02 19:36:23.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:36:23.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       47 2023-05-02 19:36:23.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2023-05-02 19:36:23.000000 core_dashboard_common_app-2.3.0/core_dashboard_common_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.490801 core_dashboard_common_app-2.3.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11337 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:36:25.681607 core_dashboard_common_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.546076 core_dashboard_common_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:21.000000 core_dashboard_common_app-2.3.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1783 2023-05-02 19:36:22.000000 core_dashboard_common_app-2.3.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      913 2023-05-02 19:36:22.000000 core_dashboard_common_app-2.3.0/tests/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.580177 core_dashboard_common_app-2.3.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:22.000000 core_dashboard_common_app-2.3.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.596585 core_dashboard_common_app-2.3.0/tests/views/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:22.000000 core_dashboard_common_app-2.3.0/tests/views/common/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:25.651596 core_dashboard_common_app-2.3.0/tests/views/common/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:22.000000 core_dashboard_common_app-2.3.0/tests/views/common/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1150 2023-05-02 19:36:22.000000 core_dashboard_common_app-2.3.0/tests/views/common/views/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3808 2023-05-02 19:36:22.000000 core_dashboard_common_app-2.3.0/tests/views/common/views/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2325 2023-05-02 19:36:22.000000 core_dashboard_common_app-2.3.0/tests/views/fixtures.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:32.656510 core_dashboard_common_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      158 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      865 2023-07-21 02:10:32.651846 core_dashboard_common_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      406 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:31.219075 core_dashboard_common_app-2.4.0/core_dashboard_common_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3824 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/constants.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1250 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:30.939390 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:30.971480 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:30.945060 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:31.430407 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      302 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/action_dashboard.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      441 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/count_checked.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      393 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/get_selected_document_admin.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      237 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/init_admin_menu.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:31.444451 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       71 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/list/view_record.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/my_dashboard_tabs.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      697 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/reset_checkbox.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      241 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/select_all.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:30.962071 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:31.498481 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      117 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/content_query.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       35 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/list.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       65 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/password_form.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:31.528114 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/init_pagination.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:31.620689 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      669 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/delete_data_draft.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/delete_data_draft.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      670 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_document.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_form.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_record.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_template.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      427 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/view_record.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1277 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/persistent_query_config.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:30.978225 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:31.634286 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      831 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/css/exploreTabs.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:31.709914 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      150 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/get_selected_document.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      577 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       83 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init_user.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:31.754772 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      856 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/edit_record.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       61 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/edit_record.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:31.874552 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1714 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/change_owner.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/change_owner.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1339 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/delete_document.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/delete_document.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1613 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/edit_persistent_query.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/edit_query.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      933 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/upload_file.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       56 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/upload_file.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/view_record.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       56 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/my_dashboard_tabs.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:31.027965 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:31.966813 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:31.981074 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      380 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/admin/dashboard.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:31.040977 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:31.998223 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/pagination/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2701 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/pagination/data_source_pagination.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      123 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/home.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:32.194836 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:32.246953 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      949 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/change_owner.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1337 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/delete_document.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1152 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/edit_persistent_query.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4324 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_files_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3689 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4828 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_queries_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      211 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_queries_table_pagination.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5641 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      222 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table_datatable.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      258 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table_pagination.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3278 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_templates_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2675 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_types_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3432 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_workspaces_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1762 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_dashboard.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1693 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      187 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile_change_password.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      849 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile_edit.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1007 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/password_change.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:32.277372 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templatetags/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templatetags/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      453 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/templatetags/special_plural.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:32.295447 core_dashboard_common_app-2.4.0/core_dashboard_common_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:32.352135 core_dashboard_common_app-2.4.0/core_dashboard_common_app/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/views/common/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19183 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/views/common/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1196 2023-07-21 02:10:28.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/views/common/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    56019 2023-07-21 02:10:29.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app/views/common/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:31.306333 core_dashboard_common_app-2.4.0/core_dashboard_common_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      865 2023-07-21 02:10:30.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6570 2023-07-21 02:10:30.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:10:30.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       47 2023-07-21 02:10:30.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2023-07-21 02:10:30.000000 core_dashboard_common_app-2.4.0/core_dashboard_common_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:32.378981 core_dashboard_common_app-2.4.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:29.000000 core_dashboard_common_app-2.4.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11337 2023-07-21 02:10:29.000000 core_dashboard_common_app-2.4.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:10:29.000000 core_dashboard_common_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2023-07-21 02:10:29.000000 core_dashboard_common_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:10:32.667068 core_dashboard_common_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2023-07-21 02:10:29.000000 core_dashboard_common_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:32.434649 core_dashboard_common_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:29.000000 core_dashboard_common_app-2.4.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      259 2023-07-21 02:10:29.000000 core_dashboard_common_app-2.4.0/tests/mocks.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1831 2023-07-21 02:10:29.000000 core_dashboard_common_app-2.4.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1027 2023-07-21 02:10:29.000000 core_dashboard_common_app-2.4.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:32.463755 core_dashboard_common_app-2.4.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:29.000000 core_dashboard_common_app-2.4.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:32.497728 core_dashboard_common_app-2.4.0/tests/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:29.000000 core_dashboard_common_app-2.4.0/tests/views/common/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:32.588674 core_dashboard_common_app-2.4.0/tests/views/common/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:29.000000 core_dashboard_common_app-2.4.0/tests/views/common/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1609 2023-07-21 02:10:29.000000 core_dashboard_common_app-2.4.0/tests/views/common/ajax/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    28548 2023-07-21 02:10:29.000000 core_dashboard_common_app-2.4.0/tests/views/common/ajax/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:32.635210 core_dashboard_common_app-2.4.0/tests/views/common/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:29.000000 core_dashboard_common_app-2.4.0/tests/views/common/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2093 2023-07-21 02:10:29.000000 core_dashboard_common_app-2.4.0/tests/views/common/views/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6085 2023-07-21 02:10:29.000000 core_dashboard_common_app-2.4.0/tests/views/common/views/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4073 2023-07-21 02:10:29.000000 core_dashboard_common_app-2.4.0/tests/views/fixtures.py
```

### Comparing `core_dashboard_common_app-2.3.0/LICENSE.md` & `core_dashboard_common_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.3.0/PKG-INFO` & `core_dashboard_common_app-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_dashboard_common_app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Resource management via a dashboard for the curator core project
 Home-page: https://github.com/usnistgov/core_dashboard_common_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =========================
         Core Dashboard Common App
```

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app/constants.py` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app/constants.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app/settings.py` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/reset_checkbox.js` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/reset_checkbox.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_document.js` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/edit_record.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,32 @@
 /**
- * Open document for text editor.
+ * Get the URL to go to the edit page
  */
-
-$(".open-template-btn").on('click', function() {
-    var $registryRow = $(this).closest('tr');
-    var objectID = $registryRow.attr("object-id");
-    var icon = $(this).find("i").attr("class");
-    showSpinner($(this).find("i"))
-    window.location = openTemplateUrl + '?id=' + objectID;
-    hideSpinner($(this).find("i"), icon)
-});
-
-
-$(".open-record-btn").on('click', function() {
+openEditRecord = function() {
     var $registryRow = $(this).closest('tr');
     var objectID = $registryRow.attr("objectid");
-    var icon = $(this).find("i").attr("class");
-    showSpinner($(this).find("i"))
-    window.location = openRecordUrl + '?id=' + objectID;
-    hideSpinner($(this).find("i"), icon)
-});
+    var editBtn = $(this).find("i")
+    var icon = $(editBtn).attr("class");
 
-$(".open-form-btn").on('click', function() {
-    var $registryRow = $(this).closest('tr');
-    var objectID = $registryRow.attr("objectid");
-    var icon = $(this).find("i").attr("class");
+    // Show loading spinner
     showSpinner($(this).find("i"))
-    window.location = openFormUrl + '?id=' + objectID;
-    hideSpinner($(this).find("i"), icon)
-});
+    $.ajax({
+        url: editRecordUrl,
+        type: "POST",
+        dataType: "json",
+        data: {
+            "id": objectID
+        },
+        success: function(data) {
+            window.location = data.url;
+        },
+        error: function(data) {
+            let jsonResponse = JSON.parse(data.responseText);
+            $.notify(jsonResponse.message, "danger");
+        }
+    }).always(function() {
+        // get old button icon
+        hideSpinner(editBtn, icon)
+    });
+};
+
+$(".edit-record-btn").on('click', openEditRecord);
```

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/persistent_query_config.js` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/persistent_query_config.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/css/exploreTabs.css` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/css/exploreTabs.css`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init.js` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/change_owner.js` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/change_owner.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/delete_document.js` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/delete_document.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -25,19 +25,19 @@
             functional_object: functional_object,
 
             // get query class name
             document_type: $('.nav-tabs .active').attr("title")
 
         },
         success: function(data) {
-            location.reload(true);
+            location.reload();
         },
         error: function(data) {
-            var error_message = JSON.parse(data.responseText);
-            $.notify(error_message.message);
+            let error_message = JSON.parse(data.responseText);
+            $.notify(error_message.message, "danger");
         }
     }).always(function() {
         // get old button icon
         hideSpinner($("[id^='delete-document-yes'] > i"), icon)
     });
 };
```

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/edit_persistent_query.js` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/edit_persistent_query.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/pagination/data_source_pagination.html` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/pagination/data_source_pagination.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/change_owner.html` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/change_owner.html`

 * *Files 22% similar despite different names*

```diff
@@ -16,10 +16,10 @@
     The owner of the document(s) will be modified.
 </p>
 <p>Please select the new owner:
        {{data.user_form}}</p>
 {% endblock %}
 
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
+<a class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
 <a id="change-owner-yes" class="btn btn-primary" href="#"><i class="fas fa-check"></i> Change</a>
 {% endblock %}
```

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_files_table.html` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_workspaces_table.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,77 +1,75 @@
 {% load dict_key_extras %}
+{% load i18n %}
 
 <table class="table table-bordered table-striped table-hover">
     <thead>
-        <tr>
-            {% if data.menu %}
-                <th>
-                    <input type="checkbox" id="select_all_{{group}}"
-                           onchange="selectAll(this, '{{group}}')">
-                </th>
-            {% endif %}
-            <th>File name</th>
-            <th>Upload date</th>
-            {% if come_from_admin %}
-                <th>User</th>
-            {% endif %}
-            {% if not data.title%}
-                <th>Workspace</th>
-            {% endif %}
-            <th>Actions</th>
-        </tr>
+        <th>Title</th>
+        <th>Owner</th>
+        <th>Can read</th>
+        <th>Can write</th>
+        <th>Public</th>
+        <th>Actions</th>
     </thead>
     <tbody>
         {% for object in objects %}
-            <tr class="{{ rowcolors }}" objectid="{{object.file.id}}">
-                {% if data.menu %}
-                <td id="actionCheckbox_{{forloop.counter}}">
-                    <input type="checkbox" id={{object.file.id}} name={{group}}>
-                </td>
-                {% endif %}
-                <td>
-                    <span class="blob-link" data-blob-url="{{ object.url }}">
-                        {{ object.file.filename }}
-                    </span>
-                </td>
-                <td>{{ object.date }}</td>
-                {% if come_from_admin %}
-                    <td>
-                        {{object.user}}
-                    </td>
-                {% endif %}
-                {% if not data.title%}
-                    <td>
-                        {% if object.file.workspace %}
-                            {{ object.file.workspace.title }}
-                        {% else %}
-                            None
-                        {% endif %}
-                    </td>
-                {% endif %}
+            <tr objectid="{{object.workspace.id}}">
+                <td>{{ object.name }}</td>
+                <td>{{ object.user }}</td>
+                <td>{{ object.can_read }}</td>
+                <td>{{ object.can_write }}</td>
+                <td>{{ object.is_public }} </td>
                 <td>
-                    <a class="btn btn-secondary download-{{data.document}}-btn" href="{{ object.url }}">
-                        <i class="fas fa-list"></i> Download
-                    </a>
-                    {% if data.share_pid_button %}
-                        {% include 'core_linked_records_app/user/sharing/data_detail/button_inline.html' %}
-                    {% endif %}
-                    {% if object.can_change_workspace %}
-                        <a class="btn btn-secondary assign-workspace-record-btn">
-                            <i class="fas fa-folder"></i> Change workspace
+                    {% if come_from_admin %}
+                        <a class="btn btn-secondary view-data-{{data.document}}-btn"
+                           objectid="{{ object.workspace.id }}"
+                           href="{% url 'core-admin:core_dashboard_workspace_list' object.workspace.id %}">
+                            <i class="fas fa-list"></i> View Content
+                        </a>
+                    {% else %}
+                        <a class="btn btn-secondary view-data-{{data.document}}-btn"
+                           objectid="{{ object.workspace.id }}"
+                           href="{% url 'core_dashboard_workspace_list' object.workspace.id %}">
+                            <i class="fas fa-list"></i> View Content
                         </a>
                     {% endif %}
+
                     {% if object.is_owner %}
-                        <a class="btn btn-secondary change-owner-btn">
-                            <i class="fas fa-folder"></i> Change Owner
-                        </a>
+                        {% if come_from_admin %}
+                            <a class="btn btn-secondary rights-document-btn"
+                                href="{% url 'core-admin:core_main_edit_rights_workspace' object.workspace.id %}">
+                                <i class="fas fa-edit"></i> Manage Access
+                            </a>
+                        {% else %}
+                            <a class="btn btn-secondary rights-document-btn"
+                                href="{% url 'core_main_edit_rights_workspace' object.workspace.id %}">
+                                <i class="fas fa-edit"></i> Manage Access
+                            </a>
+                        {% endif %}
+                        {% if not object.is_global %}
+                            {% if object.is_public %}
+                                <a class="btn btn-secondary private-{{data.document}}-btn">
+                                    <i class="fas fa-user"></i> Set private
+                                </a>
+                            {% elif data.can_set_public %}
+                                <a class="btn btn-secondary public-{{data.document}}-btn">
+                                    <i class="fas fa-users"></i> Set public
+                                </a>
+                            {% endif %}
+                        {% endif %}
+                        {% if not object.is_public %}
+                            <button class="btn btn-danger delete-document-btn">
+                                <i class="fas fa-trash"></i> Delete
+                            </button>
+                        {% endif %}
                     {% endif %}
-                    <button class="btn btn-danger delete-document-btn" objectid="{{ object.file.id }}">
-                        <i class="fas fa-trash"></i> Delete
-                    </button>
+                </td>
+            </tr>
+        {% empty %}
+            <tr>
+                <td class="empty" style="text-align: center;" colspan="100%">
+                     No {{document}} found.
                 </td>
             </tr>
         {% endfor %}
     </tbody>
-</table>
-
-{% include 'core_main_app/common/pagination/data_source_pagination.html' with pagination=data.pagination%}
+</table>
```

#### html2text {}

```diff
@@ -1,19 +1,29 @@
-{% load dict_key_extras %}
-�File name            Upload date User           Workspace                   Actions
-                                                                               Download
-                                                                               {% if
-                                                                              data.share_pid_button %} {%
-                                                                              include
-                                                  {% if object.file.workspace 'core_linked_records_app/
-   {                   {                          %} {                        user/sharing/data_detail/
-  {                    {           {              {                           button_inline.html' %} {%
-�object.file.filename object.date {object.user}} object.file.workspace.title endif %} {% if
-  }}                   }}                         }} {% else %} None {% endif object.can_change_workspace
-                                                  %}                          %}
-                                                                               Change workspace
-                                                                               {% endif %} {% if
-                                                                              object.is_owner %}
-                                                                               Change Owner
-                                                                               {% endif %}   Delete
-{% include 'core_main_app/common/pagination/data_source_pagination.html' with
-pagination=data.pagination%}
+{% load dict_key_extras %} {% load i18n %}
+                                                                          {% if
+                                                                          come_from_admin %}
+                                                                           View_Content
+                                                                           {% else %}
+                                                                           View_Content
+                                                                           {% endif %} {% if
+                                                                          object.is_owner %}
+                                                                          {% if
+                                                                          come_from_admin %}
+                                                                           Manage_Access
+                                                                           {% else %}
+{           {           {               {                {                 Manage_Access
+{           {           {               {                {                 {% endif %} {% if
+object.name object.user object.can_read object.can_write object.is_public not
+}}          }}          }}              }}               }}               object.is_global %}
+                                                                          {% if
+                                                                          object.is_public %}
+                                                                           Set private
+                                                                           {% elif
+                                                                          data.can_set_public
+                                                                          %}
+                                                                           Set public
+                                                                           {% endif %} {%
+                                                                          endif %} {% if not
+                                                                          object.is_public %}
+                                                                          Delete  {% endif %}
+                                                                          {% endif %}
+No {{document}} found.
```

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html`

 * *Files 21% similar despite different names*

```diff
@@ -31,37 +31,51 @@
                 <td>
                     {% with key=data_loaded.form.user %}
                       {{ data.usernames|get:key }}
                     {% endwith %}
                 </td>
                 {% endif %}
                 <td>
-                    {% if come_from_admin %}
-                        <a class="btn btn-secondary view-form-btn"
-                           href="{% url 'core-admin:core_curate_view_form' data_loaded.form.id %}">
-                            <i class="fas fa-file-alt"></i> View
+                    <button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownActions" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-toggle{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-toggle{% endif %}="dropdown" aria-haspopup="true" aria-expanded="false">
+                        <i class="fas fa-sliders"></i> Actions
+                    </button>
+
+                    <div class="dropdown-menu" aria-labelledby="dropdownActions">
+                        {% if come_from_admin %}
+                            <a class="dropdown-item view-form-btn"
+                               href="{% url 'core-admin:core_curate_view_form' data_loaded.form.id %}">
+                                <i class="fas fa-file-alt"></i> View
+                            </a>
+                        {% else %}
+                            <a class="dropdown-item view-form-btn"
+                               href="{% url 'core_curate_view_form' data_loaded.form.id %}">
+                                <i class="fas fa-file-alt"></i> View
+                            </a>
+                        {% endif %}
+                        <div class="dropdown-divider"></div>
+                        <a class="dropdown-item edit-form-btn" href="{% url 'core_curate_enter_data' data_loaded.form.id %}">
+                            <i class="fas fa-edit"></i> Edit
                         </a>
-                    {% else %}
-                        <a class="btn btn-secondary view-form-btn"
-                           href="{% url 'core_curate_view_form' data_loaded.form.id %}">
-                            <i class="fas fa-file-alt"></i> View
+                        <a class="dropdown-item open-form-btn" href="#">
+                            <i class="fas fa-code"></i> Open
                         </a>
-                    {% endif %}
-                    <a class="btn btn-secondary edit-form-btn" href="{% url 'core_curate_enter_data' data_loaded.form.id %}">
-                        <i class="fas fa-edit"></i> Edit
-                    </a>
-                    <a class="btn btn-secondary open-form-btn">
-                        <i class="fas fa-code"></i> Open
-                    </a>
-                    <a class="btn btn-secondary change-owner-btn">
-                        <i class="fas fa-user-circle"></i> Change Owner
-                    </a>
-                    <button class="btn btn-danger delete-document-btn">
-                        <i class="fas fa-trash"></i> Delete
-                    </button>
+                        <a class="dropdown-item change-owner-btn" href="#">
+                            <i class="fas fa-user-circle"></i> Change Owner
+                        </a>
+                        <div class="dropdown-divider"></div>
+                        <a class="dropdown-item delete-document-btn" href="#">
+                            <i class="fas fa-trash"></i> Delete
+                        </a>
+                    </div>
+                </td>
+            </tr>
+        {% empty %}
+            <tr>
+                <td class="empty" style="text-align: center;" colspan="100%">
+                     No {{document}} found.
                 </td>
             </tr>
         {% endfor %}
     </tbody>
 </table>
 
 {% include 'core_main_app/common/pagination/data_source_pagination.html' with pagination=data.pagination%}
```

#### html2text {}

```diff
@@ -1,16 +1,32 @@
 {% load dict_key_extras %}
-                                                                                         {% if
+                                                                                         % if
+                                                                                         BOOTSTRAP_VERSION
+                                                                                         == "4.6.2"
+                                                                                         %}data-toggle{%
+                                                                                         elif
+                                                                                         BOOTSTRAP_VERSION
+                                                                                         == "5.1.3"
+                                                                                         %}data-bs-toggle
+                                                                                         {% endif
+                                                                                         %}="dropdown"
+                                                                                         aria-
+                                                                                         haspopup="true"
+  {                     {                                      {% with                   aria-
+�{                     {                                      key=data_loaded.form.user expanded="false">
+  data_loaded.form.name data_loaded.form.template.display_name %} {{ data.usernames|get: Actions
+  }}                    }}                                     key }} {% endwith %}      {% if
                                                                                          come_from_admin
                                                                                          %}
                                                                                           View
-  {                     {                                      {% with                    {% else %}
-  {                     {                                      key=data_loaded.form.user  View
-�data_loaded.form.name data_loaded.form.template.display_name %} {{ data.usernames|get:  {% endif %}
-  }}                    }}                                     key }} {% endwith %}       Edit
+                                                                                          {% else %}
+                                                                                          View
+                                                                                          {% endif %}
+                                                                                          Edit
 
                                                                                           Open
 
-                                                                                          Change Owner
-                                                                                            Delete
+                                                                                          Change_Owner
+                                                                                          Delete
+No {{document}} found.
 {% include 'core_main_app/common/pagination/data_source_pagination.html' with
 pagination=data.pagination%}
```

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_queries_table.html` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_queries_table.html`

 * *Files 10% similar despite different names*

```diff
@@ -12,23 +12,22 @@
                    data-tab-value="{{tab}}"
                    aria-controls="profile" role="tab">
                     {{ tab }}
                 </a>
             </li>
         {% endfor %}
     </ul>
-    {% if data.number_total != 0 %}
     <div class="tab-content">
         <div role="tabpanel" id="data_table" class="tab-pane active">
             <table class="table table-bordered table-striped table-hover">
                 <thead>
                     {% if data.menu %}
                         <th> <input type="checkbox" id="select_all_{{group}}" onchange="selectAll(this, '{{group}}')"> </th>
                     {% endif %}
-                    <th>Name (query title)</th>
+                    <th>Name</th>
                     <th>Content</th>
                     {% if come_from_admin %} <th>User</th> {% endif %}
                     <th>Actions</th>
                 </thead>
                 <tbody>
                     {% for object in objects %}
                     <tr class="{{ rowcolors }}" objectid="{{object.query.id}}">
@@ -76,19 +75,19 @@
                                     {% include "core_explore_common_app/user/persistent_query/button.html" with come_from_my_queries='True' objectid=object.query.id%}
 
                                     <button class="btn btn-danger delete-document-btn" objectid="{{ object.query.id }}">
                                         <i class="fas fa-trash"></i> Delete
                                     </button>
                             </td>
                     </tr>
+                    {% empty %}
+                        <tr>
+                            <td class="empty" style="text-align: center;" colspan="100%">
+                                 No {{document}} found.
+                            </td>
+                        </tr>
                     {% endfor %}
                 </tbody>
             </table>
         </div>
     </div>
-    {% else %}
-
-    <div class="alert alert-light">
-      No queries found
-    </div>
-    {% endif %}
 </div>
```

#### html2text {}

```diff
@@ -1,22 +1,19 @@
 {% load dict_key_extras %}
 
     * {% for tab in data.tabs %}
     * {{ tab }}
     * {% endfor %}
-{% if data.number_total != 0 %}
                                                                    {% if come_from_admin %}
                                                                     View
                                                                     {% else %}
    {% if                    {% endif %} {% if                       View
   object.query.name !=      object.query.content !=                 {% endif %}
   "" %}{               {%   "{}" %}                 {               Execute
 �{object.query.name}} else {                       {object.user}}    Rename  {% include
   {% else %} None {%   %}   {object.query.content}}                "core_explore_common_app/
   endif %}                  {% else %} No content                  user/persistent_query/
                             {% endif %}                            button.html" with
                                                                    come_from_my_queries='True'
                                                                    objectid=object.query.id%}
                                                                    Delete
-{% else %}
-No queries found
-{% endif %}
+No {{document}} found.
```

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_templates_table.html` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_templates_table.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 {% load dict_key_extras %}
 {% load get_attribute %}
-<p>
-    This page lists user templates. Use drag and drop to update the order templates appear
-    on the website, then click on "Save ordering" when done.
-</p>
+
+{% if not come_from_admin %}
+    <p>
+        This page lists user templates. Use drag and drop to update the order templates appear
+        on the website, then click on "Save ordering" when done.
+    </p>
+{% endif %}
 <table class="table table-bordered table-striped table-hover fixed-table
         {% if come_from_admin %}table-col-4{% else %}table-col-3{% endif %}">
     <thead>
         <th>Template name</th>
         <th>Filename</th>
         {% if come_from_admin %}
             <th>User</th>
@@ -47,11 +50,21 @@
                             <i class="fas fa-trash"></i> Disable
                         </button>
 
                     {% endif %}
 
                 </td>
             </tr>
+        {% empty %}
+            <tr>
+                <td class="empty" style="text-align: center;" colspan="100%">
+                     No {{document}} found.
+                </td>
+            </tr>
         {% endfor %}
     </tbody>
 </table>
-{% include 'core_main_app/common/buttons/save_ordering.html' %}
+{% if not come_from_admin %}
+    <button  class="btn btn-success mt-3 {% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3"%}float-end{% endif %} save-order"  disabled>
+        <i class="fas fa-save"></i> Save ordering
+    </button>
+{% endif %}
```

#### html2text {}

```diff
@@ -1,10 +1,12 @@
-{% load dict_key_extras %} {% load get_attribute %}
+{% load dict_key_extras %} {% load get_attribute %} {% if not come_from_admin
+%}
 This page lists user templates. Use drag and drop to update the order templates
 appear on the website, then click on "Save ordering" when done.
+{% endif %}
                                                      {% if
                                                      object.template_version|get_attribute:
                                                      'is_disabled' %}
                                                       Restore
                                                       {% else %} {% if come_from_admin %}
                                                       Versions
                                                       {% url 'core-admin:
@@ -15,8 +17,11 @@
                                                       Versions
                                                       {% url
                                                      'core_dashboard_app_edit_template'
                                                      object.template_version.id as edit_url
                                                      %} {% include 'core_main_app/common/
                                                      buttons/edit.html' %} {% endif %}
                                                      Disable  {% endif %}
-{% include 'core_main_app/common/buttons/save_ordering.html' %}
+No {{document}} found.
+{% if not come_from_admin %}
+.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3"%}float-end{% endif %}
+save-order" disabled>  Save ordering  {% endif %}
```

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_types_table.html` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_types_table.html`

 * *Files 6% similar despite different names*

```diff
@@ -41,10 +41,16 @@
                         {% endif %}
                         <button class="btn btn-danger disable-template-btn" objectid="{{ object.type_version.id }}">
                             <i class="fas fa-trash"></i> Disable
                         </button>
                     {% endif %}
                 </td>
             </tr>
+        {% empty %}
+            <tr>
+                <td class="empty" style="text-align: center;" colspan="100%">
+                     No {{document}} found.
+                </td>
+            </tr>
         {% endfor %}
     </tbody>
 </table>
```

#### html2text {}

```diff
@@ -15,7 +15,8 @@
                                                   Versions
                                                   {% url
                                                  'core_dashboard_app_edit_type'
                                                  object.type_version.id as edit_url
                                                  %} {% include 'core_main_app/
                                                  common/buttons/edit.html' %} {%
                                                  endif %}   Disable  {% endif %}
+No {{document}} found.
```

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_dashboard.html` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_dashboard.html`

 * *Files 22% similar despite different names*

```diff
@@ -26,31 +26,27 @@
 
 
 {% block box_body %}
 {% if data.user_data %}
     Total number of {{data.document|special_plural}}: {{ data.number_total }}
 {% endif %}
 
-    {% if data.menu and not data.title %}
-        <div class="dropdown" id="id_actions" style="display:none">
-            <button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenu1" data-toggle="dropdown" aria-haspopup="true" aria-expanded="true">
-                Choose action
-                <span class="caret"></span>
-            </button>
-            <ul class="dropdown-menu">
-                {% for value, text in data.action_form.fields.actions.choices %}
-                    <li style="cursor:  pointer;" onclick="action_dashboard({{value}});">{{text}}</li>
-                {% endfor %}
-            </ul>
-        </div>
-    {% endif %}
-
-    <div class="tab-content">
-            {% if  data.document == 'query' or data.user_data  %}
-                {% include data.template with objects=data.user_data group='user' count=data.number_total tabs=data.tabs %}
-            {% else %}
-                No {{data.document|special_plural}} found.
-            {% endif %}
-    </div>
+{% if data.menu and not data.title %}
+<div class="dropdown" id="id_actions" style="display:none">
+    <button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenu1" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-toggle{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-toggle{% endif %}="dropdown" aria-haspopup="true" aria-expanded="true">
+        Choose action
+        <span class="caret"></span>
+    </button>
+    <ul class="dropdown-menu">
+        {% for value, text in data.action_form.fields.actions.choices %}
+            <li style="cursor:  pointer;" onclick="action_dashboard({{value}});">{{text}}</li>
+        {% endfor %}
+    </ul>
+</div>
+{% endif %}
+
+<div class="tab-content">
+    {% include data.template with objects=data.user_data group='user' count=data.number_total tabs=data.tabs document=data.document%}
+</div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -6,16 +6,17 @@
 endblock %} {% block box_tools %} {% if data.create_workspace %}
  Create workspace
  {% endif %} {% if data.title %}
  Previous_page
  {% endif %} {% endblock %} {% block box_body %} {% if data.user_data %} Total
 number of {{data.document|special_plural}}: {{ data.number_total }} {% endif %}
 {% if data.menu and not data.title %}
- Choose action
+% if BOOTSTRAP_VERSION == "4.6.2" %}data-toggle{% elif BOOTSTRAP_VERSION ==
+"5.1.3" %}data-bs-toggle{% endif %}="dropdown" aria-haspopup="true" aria-
+expanded="true"> Choose action
     * {% for value, text in data.action_form.fields.actions.choices %}
     * {{text}}
     * {% endfor %}
 {% endif %}
-{% if data.document == 'query' or data.user_data %} {% include data.template
-with objects=data.user_data group='user' count=data.number_total tabs=data.tabs
-%} {% else %} No {{data.document|special_plural}} found. {% endif %}
+{% include data.template with objects=data.user_data group='user'
+count=data.number_total tabs=data.tabs document=data.document%}
 {% endblock %}
```

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile_edit.html` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile_edit.html`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 <form action="{% url 'core_dashboard_profile_edit' %}" method="post">
  	{% csrf_token %}
     {{ data.form }}
     <div id="profile_error" style="font-weight: bold;">
     {{ data.action_result }}
     </div>
     <div class="mt-5 d-flex justify-content-end">
-        <button type="button" class="btn btn-secondary mr-1" onclick="location.href='{% url 'core_dashboard_profile' %}'">
+        <button type="button" class="btn btn-secondary {% if BOOTSTRAP_VERSION == "4.6.2" %}mr-1{% elif BOOTSTRAP_VERSION == "5.1.3"%}me-1{% endif %}" onclick="location.href='{% url 'core_dashboard_profile' %}'">
             <i class="fas fa-times"></i> Cancel
         </button>
         <button type="submit" class="btn btn-primary">
             <i class="fas fa-save"></i> Save changes
         </button>
     </div>
 </form>
```

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app/templates/core_dashboard_common_app/password_change.html` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app/templates/core_dashboard_common_app/password_change.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app/views/common/ajax.py` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app/views/common/ajax.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,18 @@
 from core_explore_common_app.components.abstract_persistent_query import (
     api as persistent_query_api,
 )
 from core_explore_common_app.components.abstract_persistent_query.models import (
     AbstractPersistentQuery,
 )
 from core_main_app.access_control.exceptions import AccessControlError
-from core_main_app.commons.exceptions import DoesNotExist, ModelError
+from core_main_app.commons.exceptions import (
+    DoesNotExist,
+    NotUniqueError,
+)
 from core_main_app.components.blob import api as blob_api
 from core_main_app.components.lock import api as lock_api
 from core_main_app.components.workspace import api as workspace_api
 from core_main_app.settings import INSTALLED_APPS
 from core_main_app.utils.labels import get_data_label, get_form_label
 
 if "core_curate_app" in INSTALLED_APPS:
@@ -260,15 +263,15 @@
     Returns:
     """
     try:
         list_workspaces = _get_workspaces(
             workspace_ids, request.user.is_superuser, request.user.id
         )
     except Exception as exception:
-        messages.add_message(request, messages.INFO, str(exception))
+        messages.add_message(request, messages.ERROR, str(exception))
         return HttpResponse(
             json.dumps({}), content_type="application/javascript"
         )
 
     try:
         for workspace in list_workspaces:
             workspace_api.delete(workspace, request.user)
@@ -286,28 +289,28 @@
         blob_ids:
 
     Returns:
     """
     try:
         list_blob = _get_blobs(blob_ids, request.user)
     except Exception as exception:
-        messages.add_message(request, messages.INFO, str(exception))
+        messages.add_message(request, messages.ERROR, str(exception))
         return HttpResponse(
             json.dumps({}), content_type="application/javascript"
         )
 
     try:
         for blob in list_blob:
             blob_api.delete(blob, request.user)
         messages.add_message(
-            request, messages.INFO, "File deleted with success."
+            request, messages.SUCCESS, "File deleted with success."
         )
     except Exception:
         messages.add_message(
-            request, messages.INFO, "A problem occurred while deleting."
+            request, messages.ERROR, "A problem occurred while deleting."
         )
 
     return HttpResponse(json.dumps({}), content_type="application/javascript")
 
 
 def _delete_form(request, form_ids):
     """Delete forms.
@@ -317,30 +320,30 @@
         form_ids:
 
     Returns:
     """
     try:
         list_form = _get_forms(form_ids, request.user)
     except Exception as exception:
-        messages.add_message(request, messages.INFO, str(exception))
+        messages.add_message(request, messages.ERROR, str(exception))
         return HttpResponse(
             json.dumps({}), content_type="application/javascript"
         )
 
     try:
         for form in list_form:
             curate_data_structure_api.delete(form, request.user)
         messages.add_message(
             request,
-            messages.INFO,
+            messages.SUCCESS,
             get_form_label().capitalize() + " deleted with success.",
         )
     except Exception:
         messages.add_message(
-            request, messages.INFO, "A problem occurred while deleting."
+            request, messages.ERROR, "A problem occurred while deleting."
         )
 
     return HttpResponse(json.dumps({}), content_type="application/javascript")
 
 
 def _delete_record(request, data_ids):
     """Delete records.
@@ -351,15 +354,15 @@
 
     Returns:
     """
 
     try:
         list_data = _get_data(data_ids, request.user)
     except Exception as exception:
-        messages.add_message(request, messages.INFO, str(exception))
+        messages.add_message(request, messages.ERROR, str(exception))
         return HttpResponse(
             json.dumps({}), content_type="application/javascript"
         )
 
     try:
         for data in list_data:
             # Check if the data is locked
@@ -374,20 +377,20 @@
                     json.dumps({"message": message.message}),
                     content_type="application/javascript",
                 )
 
             data_api.delete(data, request.user)
         messages.add_message(
             request,
-            messages.INFO,
+            messages.SUCCESS,
             get_data_label().capitalize() + " deleted with success.",
         )
     except Exception:
         messages.add_message(
-            request, messages.INFO, "A problem occurred while deleting."
+            request, messages.ERROR, "A problem occurred while deleting."
         )
 
     return HttpResponse(json.dumps({}), content_type="application/javascript")
 
 
 def _delete_query(request, query_ids):
     """Delete query.
@@ -415,31 +418,31 @@
 
         # Get the persistent queries
         list_query = _get_query(
             persistent_query_class, query_ids, request.user
         )
 
     except Exception as exception:
-        messages.add_message(request, messages.INFO, str(exception))
+        messages.add_message(request, messages.ERROR, str(exception))
         return HttpResponse(
             json.dumps({}), content_type="application/javascript"
         )
 
     try:
         for query in list_query:
             persistent_query_api.delete(query, request.user)
 
         messages.add_message(
             request,
-            messages.INFO,
+            messages.SUCCESS,
             " Query deleted with success.",
         )
     except Exception:
         messages.add_message(
-            request, messages.INFO, "A problem occurred while deleting."
+            request, messages.ERROR, "A problem occurred while deleting."
         )
 
     return HttpResponse(json.dumps({}), content_type="application/javascript")
 
 
 @login_required
 def change_owner_document(request):
@@ -598,16 +601,18 @@
         return HttpResponseBadRequest(
             json.dumps({"message": message.message, "tags": message.tags}),
             content_type="application/json",
         )
 
     try:
         # Check if a curate data structure already exists
-        curate_data_structure = curate_data_structure_api.get_by_data_id(
-            data.id, request.user
+        curate_data_structure = (
+            curate_data_structure_api.get_by_data_id_and_user(
+                data.id, request.user
+            )
         )
     except DoesNotExist:
         try:
             template = template_api.get_by_id(
                 str(data.template.id), request=request
             )
         except AccessControlError:
@@ -627,24 +632,34 @@
             form_string=data.xml_content,
             data=data,
         )
         try:
             curate_data_structure = curate_data_structure_api.upsert(
                 curate_data_structure, request.user
             )
-        except ModelError:
+        except NotUniqueError:
             message = Message(
                 messages.ERROR,
                 f"Unable to edit the {get_data_label()}. Please check that a {get_form_label()}"
                 f" with the same name does not already exist.",
             )
             return HttpResponseBadRequest(
                 json.dumps({"message": message.message, "tags": message.tags}),
                 content_type="application/json",
             )
+        except Exception:
+            message = Message(
+                messages.ERROR,
+                f"An unexpected error occurred. Unable to edit the {get_data_label()}.",
+            )
+            return HttpResponseBadRequest(
+                json.dumps({"message": message.message, "tags": message.tags}),
+                content_type="application/json",
+            )
+
     except Exception:
         message = Message(messages.ERROR, "A problem occurred while editing.")
         return HttpResponseBadRequest(
             json.dumps({"message": message.message, "tags": message.tags}),
             content_type="application/json",
         )
```

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app/views/common/forms.py` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app/views/common/forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Common Forms
 """
 from django import forms
 
-from core_main_app.components.user.api import get_active_users
+from core_main_app.components.user import api as user_api
 
 
 class ActionForm(forms.Form):
     """
     Form to select the action in the user dashboard.
     """
 
@@ -27,15 +27,15 @@
     user_options = []
 
     def __init__(self, current_user):
         self.user_options = []
         self.user_options.append(("", "-----------"))
 
         # We retrieve all users
-        sort_users = get_active_users()
+        sort_users = user_api.get_active_users()
         # We sort by username, case insensitive
         sort_users = sorted(sort_users, key=lambda s: s.username.lower())
 
         # We add them
         for user in sort_users:
             if user.id != current_user.id or current_user.is_superuser:
                 self.user_options.append((user.id, user.username))
```

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app/views/common/views.py` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app/views/common/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 """ Common views
 """
 import copy
 import math
 
+from django.conf import settings as conf_settings
 from django.contrib import messages
-from django.contrib.auth import update_session_auth_hash
 from django.contrib.auth.decorators import login_required
-from django.contrib.auth.forms import PasswordChangeForm
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import IntegrityError
 from django.http.response import HttpResponseRedirect
-from django.shortcuts import redirect
 from django.urls import reverse
 
 import core_main_app.components.data.api as workspace_data_api
 from core_explore_common_app.components.abstract_persistent_query import (
     api as abstract_persistent_query_api,
 )
 from core_explore_common_app.components.abstract_persistent_query.models import (
     AbstractPersistentQuery,
 )
 from core_explore_common_app.views.user.views import ResultQueryRedirectView
 from core_main_app.access_control.exceptions import AccessControlError
+from core_main_app.commons.exceptions import DoesNotExist
 from core_main_app.components.blob import api as blob_api, utils as blob_utils
 from core_main_app.components.data import api as data_api
 from core_main_app.components.template import api as template_api
 from core_main_app.components.template_version_manager import (
     api as template_version_manager_api,
 )
 from core_main_app.components.user import api as user_api
@@ -39,15 +38,15 @@
 from core_main_app.utils.pagination.django_paginator.results_paginator import (
     ResultsPaginator,
 )
 from core_main_app.utils.rendering import render
 from core_main_app.views.admin.forms import EditProfileForm
 from core_main_app.views.common.ajax import EditTemplateVersionManagerView
 from core_main_app.views.common.views import CommonView
-from core_main_app.views.user.forms import WorkspaceForm
+from core_main_app.views.user.forms import WorkspaceForm, BlobFileForm
 
 if "core_curate_app" in INSTALLED_APPS:
     import core_curate_app.components.curate_data_structure.api as curate_data_structure_api
 if "core_composer_app" in INSTALLED_APPS:
     from core_composer_app.components.type_version_manager import (
         api as type_version_manager_api,
     )
@@ -84,14 +83,15 @@
     Returns:
     """
     return render(
         request,
         dashboard_constants.DASHBOARD_PROFILE_TEMPLATE,
         context={
             "page_title": "My Profile",
+            "ENABLE_SAML2_SSO_AUTH": conf_settings.ENABLE_SAML2_SSO_AUTH,
         },
     )
 
 
 @login_required
 def my_profile_edit(request):
     """Edit the profile.
@@ -128,15 +128,15 @@
                 else:
                     _error_while_saving(request, form)
             except Exception:
                 _error_while_saving(request, form)
 
             messages.add_message(
                 request,
-                messages.INFO,
+                messages.SUCCESS,
                 "Profile information edited with success.",
             )
             return HttpResponseRedirect(reverse("core_dashboard_profile"))
     user = request.user
     data = {
         "firstname": user.first_name,
         "lastname": user.last_name,
@@ -193,76 +193,14 @@
             "form": form,
             "action_result": message,
             "page_title": "Error",
         },
     )
 
 
-class UserDashboardPasswordChangeFormView(CommonView):
-    """User Dashboard Password Change Form View"""
-
-    success_url = "core_main_app_homepage"
-    template_name = "core_dashboard_common_app/my_profile_change_password.html"
-
-    def get(self, request, *args, **kwargs):
-        """get password form
-
-        Args:
-            request:
-            args:
-            kwargs:
-
-        Returns:
-
-        """
-
-        form = PasswordChangeForm(request.user)
-        return render(
-            request,
-            self.template_name,
-            context={"form": form, "page_title": "Change Password"},
-            assets=self._get_assets(),
-        )
-
-    def post(self, request, *args, **kwargs):
-        """update password
-
-        Args:
-            request:
-            args:
-            kwargs:
-
-        Returns:
-
-        """
-
-        form = PasswordChangeForm(request.user, request.POST)
-        if form.is_valid():
-            user = form.save()
-            update_session_auth_hash(request, user)
-            messages.success(
-                request, "Your password was successfully updated!"
-            )
-            return redirect(self.success_url)
-
-        messages.error(request, "There are errors on the form.")
-        return render(
-            request,
-            self.template_name,
-            context={"form": form, "page_title": "Change Password"},
-            assets=self._get_assets(),
-        )
-
-    @staticmethod
-    def _get_assets():
-        return {
-            "css": ["core_dashboard_common_app/common/css/password_form.css"]
-        }
-
-
 class DashboardRecords(CommonView):
     """List the records."""
 
     template = dashboard_constants.DASHBOARD_TEMPLATE
     data_template = (
         dashboard_constants.DASHBOARD_RECORDS_TEMPLATE_TABLE_PAGINATION
     )
@@ -297,15 +235,15 @@
         results_paginator = ResultsPaginator.get_results(
             loaded_data, page, settings.RECORD_PER_PAGE_PAGINATION
         )
 
         # Data context
         try:
             results_paginator.object_list = self._format_data_context(
-                results_paginator.object_list
+                results_paginator.object_list, request.user
             )
         except Exception:
             results_paginator.object_list = []
 
         # Add user_form for change owner
         user_form = UserForm(request.user)
         context = {
@@ -371,30 +309,50 @@
             request,
             self.template,
             context=context,
             assets=assets,
             modals=modals,
         )
 
-    def _format_data_context(self, data_list):
+    def _format_data_context(self, data_list, user):
         data_context_list = []
+
         for data in data_list:
+            forms_count = (
+                len(
+                    curate_data_structure_api.get_all_curate_data_structures_by_data(
+                        data, user
+                    )
+                )
+                if self.administration
+                else 0
+            )
             data_context_list.append(
                 {
                     "data": data,
                     "can_read": True,
                     "can_write": True,
                     "is_owner": True,
+                    "forms_count": forms_count,
+                    "form_id": self._get_form(data, user),
                     "can_change_workspace": check_if_workspace_can_be_changed(
                         data
                     ),
                 }
             )
         return data_context_list
 
+    def _get_form(self, data, user):
+        try:
+            return curate_data_structure_api.get_by_data_id_and_user(
+                data.id, user
+            ).id
+        except DoesNotExist:
+            return None
+
     def _get_assets(self):
         assets = {
             "css": copy.deepcopy(dashboard_constants.CSS_COMMON),
             "js": [
                 {
                     "path": "core_main_app/user/js/workspaces/list/modals/assign_workspace.js",
                     "is_raw": False,
@@ -418,14 +376,22 @@
                     "is_raw": False,
                 },
                 {
                     "path": "core_dashboard_common_app/common/js/list/open_record.raw.js",
                     "is_raw": True,
                 },
                 {
+                    "path": "core_dashboard_common_app/common/js/list/delete_data_draft.js",
+                    "is_raw": False,
+                },
+                {
+                    "path": "core_dashboard_common_app/common/js/list/open_form.raw.js",
+                    "is_raw": True,
+                },
+                {
                     "path": dashboard_constants.JS_COMMON_FUNCTION_CHANGE_OWNER,
                     "is_raw": False,
                 },
                 {
                     "path": dashboard_constants.JS_COMMON_FUNCTION_DELETE,
                     "is_raw": False,
                 },
@@ -530,32 +496,37 @@
             except ObjectDoesNotExist:
                 username = "None"
             detailed_file.append(
                 {
                     "user": username,
                     "date": file.creation_date,
                     "file": file,
-                    "url": blob_utils.get_blob_download_uri(file, request),
+                    "url": f"{reverse('core_main_app_blob_detail')}?id={file.id}",
+                    "download_url": blob_utils.get_blob_download_uri(
+                        file, request
+                    ),
                     "can_change_workspace": check_if_workspace_can_be_changed(
                         file
                     ),
                     "is_owner": True,
                 }
             )
 
         # Add user_form for change owner
         user_form = UserForm(request.user)
+        file_upload_form = BlobFileForm()
         context = {
             "administration": self.administration,
             "number_total": files.count(),
             "user_data": detailed_file,
             "user_form": user_form,
             "document": dashboard_constants.FUNCTIONAL_OBJECT_ENUM.FILE.value,
             "template": dashboard_constants.DASHBOARD_FILES_TEMPLATE_TABLE,
             "menu": self.administration,
+            "file_upload_form": file_upload_form,
             "share_pid_button": "core_linked_records_app"
             in settings.INSTALLED_APPS,
             "pagination": _get_pagination_document(
                 page,
                 results_paginator,
                 files.count(),
                 settings.FILE_PER_PAGE_PAGINATION,
@@ -572,22 +543,27 @@
                         ]
                     )
                 }
             )
 
         modals = [
             "core_main_app/user/workspaces/list/modals/assign_workspace.html",
+            "core_main_app/user/blob/list/modals/file_upload.html",
             dashboard_constants.MODALS_COMMON_DELETE,
             dashboard_constants.MODALS_COMMON_CHANGE_OWNER,
         ]
 
         assets = {
             "css": dashboard_constants.CSS_COMMON,
             "js": [
                 {
+                    "path": "core_dashboard_common_app/user/js/list/modals/upload_file.js",
+                    "is_raw": False,
+                },
+                {
                     "path": "core_dashboard_common_app/user/js/init.raw.js",
                     "is_raw": True,
                 },
                 {
                     "path": dashboard_constants.JS_COMMON_FUNCTION_DELETE,
                     "is_raw": False,
                 },
@@ -610,15 +586,15 @@
                 {
                     "path": "core_dashboard_common_app/common/js/init_pagination.js",
                     "is_raw": False,
                 },
             ],
         }
 
-        if "core_file_preview_app" in INSTALLED_APPS:
+        if "core_file_preview_app" in conf_settings.INSTALLED_APPS:
             assets["js"].extend(
                 [
                     {
                         "path": "core_file_preview_app/user/js/file_preview.js",
                         "is_raw": False,
                     }
                 ]
```

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app.egg-info/PKG-INFO` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-dashboard-common-app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Resource management via a dashboard for the curator core project
 Home-page: https://github.com/usnistgov/core_dashboard_common_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =========================
         Core Dashboard Common App
```

### Comparing `core_dashboard_common_app-2.3.0/core_dashboard_common_app.egg-info/SOURCES.txt` & `core_dashboard_common_app-2.4.0/core_dashboard_common_app.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 core_dashboard_common_app/static/core_dashboard_common_app/admin/js/select_all.js
 core_dashboard_common_app/static/core_dashboard_common_app/admin/js/list/view_record.raw.js
 core_dashboard_common_app/static/core_dashboard_common_app/common/css/content_query.css
 core_dashboard_common_app/static/core_dashboard_common_app/common/css/list.css
 core_dashboard_common_app/static/core_dashboard_common_app/common/css/password_form.css
 core_dashboard_common_app/static/core_dashboard_common_app/common/js/init_pagination.js
 core_dashboard_common_app/static/core_dashboard_common_app/common/js/persistent_query_config.js
+core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/delete_data_draft.js
+core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/delete_data_draft.raw.js
 core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_document.js
 core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_form.raw.js
 core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_record.raw.js
 core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_template.raw.js
 core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/view_record.js
 core_dashboard_common_app/static/core_dashboard_common_app/user/css/exploreTabs.css
 core_dashboard_common_app/static/core_dashboard_common_app/user/js/get_selected_document.js
@@ -41,14 +43,16 @@
 core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/view_record.raw.js
 core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/change_owner.js
 core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/change_owner.raw.js
 core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/delete_document.js
 core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/delete_document.raw.js
 core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/edit_persistent_query.js
 core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/edit_query.raw.js
+core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/upload_file.js
+core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/upload_file.raw.js
 core_dashboard_common_app/templates/core_dashboard_common_app/home.html
 core_dashboard_common_app/templates/core_dashboard_common_app/my_dashboard.html
 core_dashboard_common_app/templates/core_dashboard_common_app/my_profile.html
 core_dashboard_common_app/templates/core_dashboard_common_app/my_profile_change_password.html
 core_dashboard_common_app/templates/core_dashboard_common_app/my_profile_edit.html
 core_dashboard_common_app/templates/core_dashboard_common_app/password_change.html
 core_dashboard_common_app/templates/core_dashboard_common_app/admin/dashboard.html
@@ -63,25 +67,28 @@
 core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_templates_table.html
 core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_types_table.html
 core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_workspaces_table.html
 core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/change_owner.html
 core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/delete_document.html
 core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/edit_persistent_query.html
 core_dashboard_common_app/templatetags/__init__.py
-core_dashboard_common_app/templatetags/draft_extras.py
 core_dashboard_common_app/templatetags/special_plural.py
 core_dashboard_common_app/views/__init__.py
 core_dashboard_common_app/views/common/__init__.py
 core_dashboard_common_app/views/common/ajax.py
 core_dashboard_common_app/views/common/forms.py
 core_dashboard_common_app/views/common/views.py
 docs/__init__.py
 docs/conf.py
 tests/__init__.py
+tests/mocks.py
 tests/test_settings.py
 tests/urls.py
 tests/views/__init__.py
 tests/views/fixtures.py
 tests/views/common/__init__.py
+tests/views/common/ajax/__init__.py
+tests/views/common/ajax/tests_int.py
+tests/views/common/ajax/tests_unit.py
 tests/views/common/views/__init__.py
 tests/views/common/views/tests_int.py
 tests/views/common/views/tests_unit.py
```

### Comparing `core_dashboard_common_app-2.3.0/docs/conf.py` & `core_dashboard_common_app-2.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.3.0/setup.py` & `core_dashboard_common_app-2.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_dashboard_common_app",
-    version="2.3.0",
+    version="2.4.0",
     description="Resource management via a dashboard for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_dashboard_common_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_dashboard_common_app-2.3.0/tests/test_settings.py` & `core_dashboard_common_app-2.4.0/tests/test_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,18 +7,19 @@
     "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.sites",
     # Extra apps
-    "tz_detect",
     "django_celery_beat",
     # Local apps
     "core_main_app",
+    "core_dashboard_app",
+    "core_dashboard_common_app",
     "core_explore_common_app",
     "core_parser_app",
     "core_curate_app",
     "tests",
 ]
 
 # IN-MEMORY TEST DATABASE
@@ -33,15 +34,14 @@
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
@@ -54,13 +54,14 @@
                 "core_main_app.utils.custom_context_processors.domain_context_processor",
                 "django.template.context_processors.i18n",
             ],
         },
     },
 ]
 
+DEFAULT_AUTO_FIELD = "django.db.models.BigAutoField"
 CELERYBEAT_SCHEDULER = "django_celery_beat.schedulers:DatabaseScheduler"
 CUSTOM_NAME = "Curator"
 ROOT_URLCONF = "tests.urls"
 MONGODB_INDEXING = False
 MONGODB_ASYNC_SAVE = False
 ENABLE_SAML2_SSO_AUTH = False
```

### Comparing `core_dashboard_common_app-2.3.0/tests/views/common/views/tests_int.py` & `core_dashboard_common_app-2.4.0/tests/views/common/views/tests_int.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """ Test access to views
 """
+from unittest.mock import patch
+
 from django.contrib.auth.models import AnonymousUser
 from django.test import RequestFactory
 from core_main_app.utils.integration_tests.integration_base_test_case import (
     IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
-from core_dashboard_common_app.views.common.views import DashboardForms
-
-from tests.views.fixtures import (
-    DataStructureFixtures,
+from core_dashboard_common_app.views.common.views import (
+    DashboardForms,
+    DashboardRecords,
 )
 
+from tests.views.fixtures import DataStructureFixtures, DataFixtures
+
 
 class TestViewDashboardForms(IntegrationBaseTestCase):
     """Test View Dashboard Forms"""
 
     def setUp(self):
         """setUp
 
@@ -34,7 +37,36 @@
         Returns:
 
         """
         request = self.factory.get("core_dashboard_common_forms")
         request.user = self.user1
         response = DashboardForms.as_view()(request)
         self.assertEqual(response.status_code, 200)
+
+
+class TestViewDashboardRecords(IntegrationBaseTestCase):
+    """Test View Dashboard Records"""
+
+    def setUp(self):
+        """setUp
+
+        Returns:
+
+        """
+        self.factory = RequestFactory()
+        self.user1 = create_mock_user(user_id="1")
+        self.fixture = DataFixtures()
+        self.fixture.insert_data()
+
+    @patch("core_main_app.access_control.api.check_can_read_list")
+    def test_user_can_access_records_if_owner(self, mock_get):
+        """test_user_can_access_records_if_owner
+
+        Returns:
+        """
+        mock_get.return_value = None
+        request = self.factory.get("core_dashboard_common_records")
+        view = DashboardRecords
+        view.administration = False
+        request.user = create_mock_user(user_id="1")
+        response = DashboardRecords.as_view()(request)
+        self.assertEqual(response.status_code, 200)
```

