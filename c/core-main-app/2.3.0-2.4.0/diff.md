# Comparing `tmp/core_main_app-2.3.0.tar.gz` & `tmp/core_main_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_main_app-2.3.0.tar", last modified: Tue May  2 19:40:23 2023, max compression
+gzip compressed data, was "core_main_app-2.4.0.tar", last modified: Fri Jul 21 02:14:06 2023, max compression
```

## Comparing `core_main_app-2.3.0.tar` & `core_main_app-2.4.0.tar`

### file list

```diff
@@ -1,818 +1,851 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:23.024642 core_main_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:39:54.000000 core_main_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      219 2023-05-02 19:39:54.000000 core_main_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8195 2023-05-02 19:40:23.019734 core_main_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5952 2023-05-02 19:39:54.000000 core_main_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.141853 core_main_app-2.3.0/core_main_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.277624 core_main_app-2.3.0/core_main_app/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11087 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/access_control/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      628 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/access_control/decorators.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      197 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/access_control/exceptions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6065 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1360 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.401134 core_main_app-2.3.0/core_main_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      412 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/commons/constants.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/commons/enums.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4063 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/commons/exceptions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/commons/regex.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      332 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/commons/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9154 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/commons/validators.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.419746 core_main_app-2.3.0/core_main_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.449817 core_main_app-2.3.0/core_main_app/components/abstract_data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/abstract_data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5240 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/abstract_data/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.530245 core_main_app-2.3.0/core_main_app/components/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/blob/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1118 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/blob/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      315 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/blob/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2729 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/blob/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3493 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/blob/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      442 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/blob/utils.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.637531 core_main_app-2.3.0/core_main_app/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4384 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/data/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5527 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/data/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8854 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/data/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5791 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/data/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10384 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/data/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.669868 core_main_app-2.3.0/core_main_app/components/group/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/group/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1982 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/group/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.735350 core_main_app-2.3.0/core_main_app/components/lock/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/lock/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      330 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/lock/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2570 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/lock/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2665 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/lock/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.822113 core_main_app-2.3.0/core_main_app/components/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/mongo/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1041 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/mongo/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10440 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/mongo/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.896504 core_main_app-2.3.0/core_main_app/components/template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4454 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      362 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4434 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6655 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.968862 core_main_app-2.3.0/core_main_app/components/template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2328 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template_version_manager/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      507 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template_version_manager/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6205 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template_version_manager/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4719 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template_version_manager/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.046399 core_main_app-2.3.0/core_main_app/components/template_xsl_rendering/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template_xsl_rendering/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      338 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template_xsl_rendering/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6892 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template_xsl_rendering/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3434 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template_xsl_rendering/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.081858 core_main_app-2.3.0/core_main_app/components/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2470 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/user/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.181067 core_main_app-2.3.0/core_main_app/components/version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4883 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/version_manager/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3744 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/version_manager/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3248 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/version_manager/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      550 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/version_manager/utils.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.242648 core_main_app-2.3.0/core_main_app/components/web_page/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/web_page/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1280 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/web_page/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1097 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/web_page/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.276722 core_main_app-2.3.0/core_main_app/components/web_page_login/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/web_page_login/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      809 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/web_page_login/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.366887 core_main_app-2.3.0/core_main_app/components/workspace/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/workspace/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2493 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/workspace/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/workspace/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16858 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/workspace/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5695 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/workspace/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.432069 core_main_app-2.3.0/core_main_app/components/xsl_transformation/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/xsl_transformation/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      366 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/xsl_transformation/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2542 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/xsl_transformation/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4469 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/xsl_transformation/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1791 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.503910 core_main_app-2.3.0/core_main_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16483 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      751 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/migrations/0002_site_update.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1880 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/migrations/0003_psql_full_text.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      823 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/migrations/0004_template_ordering.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      733 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.632326 core_main_app-2.3.0/core_main_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6351 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/permissions/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3152 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/permissions/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      644 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/permissions/rights.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      230 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/permissions/utils.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.683755 core_main_app-2.3.0/core_main_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.745063 core_main_app-2.3.0/core_main_app/rest/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/blob/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4546 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/blob/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16319 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/blob/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.835586 core_main_app-2.3.0/core_main_app/rest/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7896 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/data/abstract_views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2006 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/data/admin_serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3187 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/data/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    36848 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/data/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.870507 core_main_app-2.3.0/core_main_app/rest/group/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/group/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      293 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/group/serializers.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.908156 core_main_app-2.3.0/core_main_app/rest/mongo_data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/mongo_data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1692 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/mongo_data/serializers.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.962235 core_main_app-2.3.0/core_main_app/rest/template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/template/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      834 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/template/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4354 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/template/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.053400 core_main_app-2.3.0/core_main_app/rest/template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/template_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10462 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/template_version_manager/abstract_views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2601 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/template_version_manager/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      587 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/template_version_manager/utils.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12274 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/template_version_manager/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.103565 core_main_app-2.3.0/core_main_app/rest/template_xsl_rendering/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/template_xsl_rendering/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1168 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/template_xsl_rendering/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14418 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/template_xsl_rendering/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14246 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.146962 core_main_app-2.3.0/core_main_app/rest/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1157 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/user/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      709 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/user/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2478 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.197981 core_main_app-2.3.0/core_main_app/rest/web_page/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/web_page/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1042 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/web_page/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4688 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/web_page/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.249793 core_main_app-2.3.0/core_main_app/rest/workspace/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/workspace/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      894 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/workspace/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    23285 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/workspace/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.311266 core_main_app-2.3.0/core_main_app/rest/xsl_transformation/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/xsl_transformation/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1437 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/xsl_transformation/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8160 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/xsl_transformation/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8349 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:09.841740 core_main_app-2.3.0/core_main_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:10.027334 core_main_app-2.3.0/core_main_app/static/core_main_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:09.871095 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:09.854917 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.376083 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      251 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/css/additional.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    47539 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/css/skins.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)   110978 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/css/theme.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.411146 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    22937 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/js/app.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      578 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/js/menu.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.443558 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1575 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/css/data_migration.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/css/permissions.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.465269 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/css/templates_xslt/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1363 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/css/templates_xslt/form.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.484385 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/css/web_page/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       31 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/css/web_page/style.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.502933 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      831 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/display_permissions.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.540098 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    30064 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates/data_migration.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      594 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates/data_migration.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.596459 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1334 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates/upload/dependencies.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       94 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates/upload/dependencies.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      139 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates/upload/dependency_resolver.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.617513 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates_xslt/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1482 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates_xslt/detail_xslt.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:09.989423 core_main_app-2.3.0/core_main_app/static/core_main_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.787598 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2236 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/XMLTree.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/buttons.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      178 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/fields.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/highlight.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       92 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/loading-spinner.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      474 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/select.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      392 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/share_link.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      940 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/switch.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      486 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/table.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.801082 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       59 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/template/template_ordering.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      189 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/word-wrap.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.814588 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/workspace/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      333 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/workspace/table.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.839357 core_main_app-2.3.0/core_main_app/static/core_main_app/common/img/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      246 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/img/collapse.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      253 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/img/expand.png
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.990825 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      335 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/XMLTree.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      247 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/backtoprevious.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1828 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/csrf.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      192 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/data_detail.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      531 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/debounce.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      788 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/elementViewport.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      413 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/leave_notice.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      556 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/loading_spinner.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.089728 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1292 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/modals/add.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1136 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/modals/delete.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      481 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/modals/download.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      178 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/modals/download.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1257 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/modals/edit.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      439 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/modals/error_page_modal.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1950 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/notify-styles.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.125521 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.160858 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.211201 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1086 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/list/modals/disable.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      125 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/list/modals/disable.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      663 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/list/restore.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      124 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/list/restore.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1156 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/sort.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/sort.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.288764 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/versions/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.330352 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/versions/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1029 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/versions/modals/disable.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      108 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/versions/modals/disable.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      537 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/versions/restore.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/versions/restore.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      652 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/versions/set_current.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      111 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/versions/set_current.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:09.981688 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/xslt/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:09.984820 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/xslt/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.412065 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      859 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/delete.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       64 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/delete.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1012 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/edit.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/edit.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.429958 core_main_app-2.3.0/core_main_app/static/core_main_app/common/xsl/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1763 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/xsl/xml2html.xsl
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.447972 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:10.020524 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.649858 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery/3.5.1/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    89475 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery/3.5.1/jquery.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:10.004465 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.515379 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.629612 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7006 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_444444_256x240.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7074 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_555555_256x240.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4676 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777620_256x240.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7013 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777777_256x240.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4632 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6313 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    37326 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)   520714 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18705 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.structure.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18671 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.theme.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21509 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/notify.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:10.036444 core_main_app-2.3.0/core_main_app/static/core_main_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.735880 core_main_app-2.3.0/core_main_app/static/core_main_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/css/login.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       63 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/css/registration.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      387 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/css/text-editor.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.751718 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.797093 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      618 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/data/change_display.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/data/change_display.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      158 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/data/detail.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.827341 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/login/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      667 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/login/message.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/login/message.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1110 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/sharing_modal.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.900225 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/text_editor/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      154 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/text_editor/data_text_editor.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       73 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/text_editor/template_text_editor.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7080 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/text_editor/text_editor.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.012467 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1800 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/add_group.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      160 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/add_group.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1723 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/add_user.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/add_user.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1138 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/create_workspace.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       73 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/create_workspace.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      515 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/init.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       43 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/init.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:10.073284 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.196277 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      187 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_blob_workspace.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      187 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_data_workspace.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1455 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_workspace.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1360 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/remove_rights.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/remove_rights.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      807 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_private.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       96 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_private.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      822 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_public.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       94 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_public.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1728 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/switch_right.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      144 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/switch_right.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.239777 core_main_app-2.3.0/core_main_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2302 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/system/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.256320 core_main_app-2.3.0/core_main_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:10.359455 core_main_app-2.3.0/core_main_app/templates/core_main_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:10.115107 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.278436 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1302 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/app_wrapper.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.349754 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4775 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      223 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/footer.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      905 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/header.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2909 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/menu.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.412005 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      620 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/box.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      715 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/section.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.428939 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      567 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/common/messages.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.475553 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1463 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/user/app_wrapper.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      902 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/user/default.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4855 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/user/theme_base.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.550891 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:10.147900 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/commons/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.591578 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/commons/errors/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      401 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/commons/errors/errors.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      254 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/commons/errors/errors_wrapper.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.621472 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/commons/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      691 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/commons/upload/form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      313 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/commons/upload/upload.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      103 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/dashboard.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.674558 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/data/detail.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      383 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/data/detail_box.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1497 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/dependency_resolver.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      211 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/list_dependencies.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.742354 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.757697 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/data_migration/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7822 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/data_migration/templates_list.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      289 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/data_migration.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.790491 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1978 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/list/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      830 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/list/disabled.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.807268 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      813 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/list/modals/disable.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      542 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.824869 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      399 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/upload/base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      166 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/upload.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.855713 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/versions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3401 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/versions/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1158 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/versions/disabled.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.871572 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/versions/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      727 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/versions/modals/disable.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      677 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/versions.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.885628 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates_xslt/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.900097 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates_xslt/main/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4036 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates_xslt/main/form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      393 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates_xslt/main.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      860 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/upload_template.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.974598 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/web_page/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      166 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/web_page/login_page.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      804 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/web_page/main.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      387 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/web_page/web_page.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      375 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/web_page/web_page_unavailable.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.992011 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/workspaces/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      234 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/workspaces/edit_rights.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.028044 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/xslt/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.048461 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/xslt/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1236 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/xslt/list/table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      323 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/xslt/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.089446 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/xslt/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       61 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/xslt/upload/base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      161 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/xslt/upload.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:10.331431 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.204329 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/buttons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/buttons/add.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      152 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/buttons/back_to_previous.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/buttons/delete.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      190 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/buttons/edit.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      104 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/buttons/go_to.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      131 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/buttons/save_ordering.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.252471 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      189 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/commons/error.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/commons/form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      167 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/commons/form_delete.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.290828 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/commons/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      578 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/commons/upload/form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      313 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/commons/upload/upload.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.320784 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      497 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/data/detail_data.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1716 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/data/tools_data.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.336749 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/defender/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       90 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/defender/error.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.426540 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      463 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/modals/add_page_modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      633 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/modals/create_data_modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      489 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/modals/delete_page_modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1066 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/modals/download-options.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      467 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/modals/edit_page_modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      429 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/modals/error_page_modal.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.444007 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/pagination/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3008 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/pagination/data_source_pagination.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.462656 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.498442 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1524 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/list/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      801 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/list/disabled.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.529465 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      805 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/list/modals/disable.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      741 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/list/modals/edit.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.548944 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/versions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2074 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/versions/available.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.566369 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/versions/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      663 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/versions/modals/disable.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      265 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/versions.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.621743 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates_xslt/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates_xslt/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.638800 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates_xslt/main/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      832 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates_xslt/main/form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      428 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates_xslt/main.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.665345 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.678728 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.710061 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      564 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/list/modals/delete.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      928 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/list/modals/edit.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1147 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/list/table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      255 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.726780 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/upload/base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      163 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/upload.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.743116 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.768228 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      483 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/data/detail.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      139 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/homepage.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.796980 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/login/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2215 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/login/main.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.812433 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/login/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      534 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/login/modals/login_message.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      340 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/login/saml2_error.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.896082 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/registration/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      171 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/registration/password_reset_complete.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      390 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/registration/password_reset_confirm.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      499 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/registration/password_reset_done.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      362 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/registration/password_reset_email.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      180 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/registration/password_reset_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       14 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/registration/password_reset_subject.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.911321 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/sharing/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      274 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/sharing/button.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.938920 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/sharing/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      504 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/sharing/modals/multi-link.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      940 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/sharing/modals/single-link.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.966802 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      453 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/template/list_body.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/template/list_header.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.982344 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/text_editor/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3042 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/text_editor/text_editor.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.999809 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1184 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/edit_rights.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:17.031248 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1424 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/create_workspace.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1882 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/edit_rights_table.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:17.170474 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1613 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_group.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      193 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_group_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1597 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_user.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      190 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_user_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      832 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/assign_workspace.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      411 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/assign_workspace_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      958 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/remove_rights.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      883 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/set_private.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      892 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/set_public.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      675 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/switch_right.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      147 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/theme.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:17.307250 core_main_app-2.3.0/core_main_app/templatetags/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templatetags/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1086 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templatetags/auth_extras.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1097 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templatetags/blob_tags.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      367 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templatetags/dict_key_extras.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      514 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templatetags/get_attribute.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      598 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templatetags/include_static.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1124 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templatetags/json_date.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      642 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templatetags/stripjs.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      316 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templatetags/timestamptags.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3319 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templatetags/xsl_transform_tag.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4501 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:17.882763 core_main_app-2.3.0/core_main_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:17.922136 core_main_app-2.3.0/core_main_app/utils/admin_site/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/admin_site/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1233 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/admin_site/model_admin_class.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      379 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/admin_site/view_only_admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2447 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/blob_downloader.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      405 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/boolean.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1137 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/checksum.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1876 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/custom_context_processors.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:17.949385 core_main_app-2.3.0/core_main_app/utils/databases/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/databases/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      627 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/databases/backend.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.001130 core_main_app-2.3.0/core_main_app/utils/databases/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      574 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/databases/mongo/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1584 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/databases/mongo/mongoengine_database.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      873 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/databases/mongo/pymongo_database.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      286 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/datetime.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9575 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/decorators.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2805 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/file.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      377 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/group.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.066009 core_main_app-2.3.0/core_main_app/utils/integration_tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/integration_tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      262 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/integration_tests/fixture_interface.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1641 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/integration_tests/integration_base_test_case.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1031 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/integration_tests/integration_base_transaction_test_case.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      319 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/labels.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.105448 core_main_app-2.3.0/core_main_app/utils/logger/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/logger/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1762 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/logger/logger_utils.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      438 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/markdown_parser.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      957 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/migrations.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.135129 core_main_app-2.3.0/core_main_app/utils/notifications/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/notifications/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3448 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/notifications/mail.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.163426 core_main_app-2.3.0/core_main_app/utils/notifications/tasks/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/notifications/tasks/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2566 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/notifications/tasks/task_mail.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.176093 core_main_app-2.3.0/core_main_app/utils/pagination/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/pagination/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.208625 core_main_app-2.3.0/core_main_app/utils/pagination/django_paginator/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/pagination/django_paginator/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      773 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/pagination/django_paginator/results_paginator.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.237415 core_main_app-2.3.0/core_main_app/utils/pagination/mongoengine_paginator/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/pagination/mongoengine_paginator/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1109 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/pagination/mongoengine_paginator/paginator.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.309347 core_main_app-2.3.0/core_main_app/utils/pagination/rest_framework_paginator/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/pagination/rest_framework_paginator/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      525 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/pagination/rest_framework_paginator/pagination.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1108 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/pagination/rest_framework_paginator/rest_framework_paginator.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      458 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/parser.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.344067 core_main_app-2.3.0/core_main_app/utils/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      145 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/query/constants.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.382674 core_main_app-2.3.0/core_main_app/utils/query/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/query/mongo/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14676 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/query/mongo/prepare.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3095 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/query/mongo/query_builder.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.475767 core_main_app-2.3.0/core_main_app/utils/raw_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/raw_query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1622 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/raw_query/common.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3901 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/raw_query/django_raw_query.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2134 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/raw_query/mongo_raw_query.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3182 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/rendering.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.551149 core_main_app-2.3.0/core_main_app/utils/requests_utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/requests_utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      568 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/requests_utils/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1663 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/requests_utils/requests_utils.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2054 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/requests_utils/ssl.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.651849 core_main_app-2.3.0/core_main_app/utils/resolvers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/resolvers/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1184 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/resolvers/requests_resolver.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1072 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/resolvers/resolver_utils.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/resolvers/xsd_uri_resolvers.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.727680 core_main_app-2.3.0/core_main_app/utils/saml2/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/saml2/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8886 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/saml2/utils.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.788823 core_main_app-2.3.0/core_main_app/utils/storage/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/storage/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3523 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/storage/gridfs_storage.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1791 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/storage/storage.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.832828 core_main_app-2.3.0/core_main_app/utils/tests_tools/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      613 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/tests_tools/MockUser.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5344 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/tests_tools/RequestMock.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/tests_tools/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2238 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.956651 core_main_app-2.3.0/core_main_app/utils/validation/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/validation/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1162 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/validation/regex_validation.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      644 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/validation/xpath_validation.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.989580 core_main_app-2.3.0/core_main_app/utils/view_builders/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/view_builders/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6572 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/view_builders/data.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16047 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/xml.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:19.034215 core_main_app-2.3.0/core_main_app/utils/xsd_flattener/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/xsd_flattener/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2095 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/xsd_flattener/xsd_flattener_database_url.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1000 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/xsd_flattener/xsd_flattener_requests_url.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:19.051016 core_main_app-2.3.0/core_main_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:19.111618 core_main_app-2.3.0/core_main_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4442 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/admin/ajax.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:19.128147 core_main_app-2.3.0/core_main_app/views/admin/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/admin/commons/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:19.165578 core_main_app-2.3.0/core_main_app/views/admin/commons/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/admin/commons/upload/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      439 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/admin/commons/upload/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4457 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21048 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:19.236417 core_main_app-2.3.0/core_main_app/views/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/common/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7191 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/common/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      459 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/common/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    31000 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/common/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:20.736534 core_main_app-2.3.0/core_main_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16821 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5059 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/user/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14764 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.209354 core_main_app-2.3.0/core_main_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8195 2023-05-02 19:40:06.000000 core_main_app-2.3.0/core_main_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    31241 2023-05-02 19:40:09.000000 core_main_app-2.3.0/core_main_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:40:06.000000 core_main_app-2.3.0/core_main_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      468 2023-05-02 19:40:07.000000 core_main_app-2.3.0/core_main_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       25 2023-05-02 19:40:07.000000 core_main_app-2.3.0/core_main_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:20.780481 core_main_app-2.3.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11121 2023-05-02 19:40:00.000000 core_main_app-2.3.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      278 2023-05-02 19:40:00.000000 core_main_app-2.3.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2023-05-02 19:40:02.000000 core_main_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2023-05-02 19:40:02.000000 core_main_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       92 2023-05-02 19:40:02.000000 core_main_app-2.3.0/requirements.dev.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       20 2023-05-02 19:40:02.000000 core_main_app-2.3.0/requirements.mongo.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      316 2023-05-02 19:40:02.000000 core_main_app-2.3.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:40:23.026275 core_main_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2104 2023-05-02 19:40:02.000000 core_main_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:20.870486 core_main_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:20.903233 core_main_app-2.3.0/tests/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3415 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/access_control/tests_access_control.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:20.932772 core_main_app-2.3.0/tests/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3764 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/commons/tests_validators.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:20.946967 core_main_app-2.3.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.003844 core_main_app-2.3.0/tests/components/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/blob/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.055246 core_main_app-2.3.0/tests/components/blob/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/blob/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3165 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/blob/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6398 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/blob/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20676 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/blob/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      440 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/blob/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.133841 core_main_app-2.3.0/tests/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/data/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.169923 core_main_app-2.3.0/tests/components/data/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/data/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    23919 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/data/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    66538 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/data/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    80876 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/data/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3730 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/data/tests_int_ordering.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    27059 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/data/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.225584 core_main_app-2.3.0/tests/components/group/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/group/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.273391 core_main_app-2.3.0/tests/components/group/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/group/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      570 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/group/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      879 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/group/fixtures/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4760 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/group/tests_int.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.327329 core_main_app-2.3.0/tests/components/lock/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/lock/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4153 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/lock/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2440 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/lock/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.371912 core_main_app-2.3.0/tests/components/mongo_data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/mongo_data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    70475 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/mongo_data/tests_int_access_control.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.420744 core_main_app-2.3.0/tests/components/template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.454933 core_main_app-2.3.0/tests/components/template/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2078 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    46022 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7215 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.517694 core_main_app-2.3.0/tests/components/template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template_version_manager/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.550968 core_main_app-2.3.0/tests/components/template_version_manager/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template_version_manager/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6470 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template_version_manager/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    54873 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template_version_manager/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17617 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template_version_manager/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.602790 core_main_app-2.3.0/tests/components/template_xsl_rendering/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template_xsl_rendering/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.644345 core_main_app-2.3.0/tests/components/template_xsl_rendering/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template_xsl_rendering/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3266 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template_xsl_rendering/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7896 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template_xsl_rendering/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9565 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template_xsl_rendering/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.678119 core_main_app-2.3.0/tests/components/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/user/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.721009 core_main_app-2.3.0/tests/components/user/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/user/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1552 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/user/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1429 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/user/fixtures/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7733 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/user/tests_int.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.786548 core_main_app-2.3.0/tests/components/version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    61614 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/version_manager/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9899 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/version_manager/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.816829 core_main_app-2.3.0/tests/components/web_page/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/web_page/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4846 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/web_page/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.846937 core_main_app-2.3.0/tests/components/web_page_login/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/web_page_login/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3905 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/web_page_login/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.875651 core_main_app-2.3.0/tests/components/workspace/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/workspace/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.919030 core_main_app-2.3.0/tests/components/workspace/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/workspace/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1235 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/workspace/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      919 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/workspace/fixtures/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7478 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/workspace/tests_int.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.948447 core_main_app-2.3.0/tests/components/xsl_transformation/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/xsl_transformation/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12828 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/xsl_transformation/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      356 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/mocks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.975865 core_main_app-2.3.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.029568 core_main_app-2.3.0/tests/rest/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/blob/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    23641 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/blob/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19778 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/blob/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/blob/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.117029 core_main_app-2.3.0/tests/rest/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    47395 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/data/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    36850 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/data/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12424 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/data/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.165051 core_main_app-2.3.0/tests/rest/template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/template/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2518 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/template/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5026 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/template/tests_permission.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4802 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/template/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.210737 core_main_app-2.3.0/tests/rest/template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/template_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    37232 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/template_version_manager/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    31920 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/template_version_manager/tests_permission.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3610 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/template_version_manager/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.257690 core_main_app-2.3.0/tests/rest/template_xsl_rendering/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/template_xsl_rendering/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11418 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/template_xsl_rendering/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13879 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/template_xsl_rendering/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3549 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/tests_views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.316146 core_main_app-2.3.0/tests/rest/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1737 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/user/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3137 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/user/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      886 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/user/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.343344 core_main_app-2.3.0/tests/rest/web_page/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/web_page/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6164 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/web_page/tests_permission.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.389766 core_main_app-2.3.0/tests/rest/workspace/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/workspace/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    71809 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/workspace/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    48644 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/workspace/tests_permissions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.447003 core_main_app-2.3.0/tests/rest/xsl_transformation/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/xsl_transformation/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.490445 core_main_app-2.3.0/tests/rest/xsl_transformation/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/xsl_transformation/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1283 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/xsl_transformation/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11618 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/xsl_transformation/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12753 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/xsl_transformation/tests_permission.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4365 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/xsl_transformation/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      529 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest_urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.527360 core_main_app-2.3.0/tests/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4668 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/system/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.559965 core_main_app-2.3.0/tests/templatetags/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/templatetags/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1364 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/templatetags/test_get_attribute.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2815 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      293 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/test_settings_sqlite3.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3445 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.695930 core_main_app-2.3.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.729763 core_main_app-2.3.0/tests/utils/checksum/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/checksum/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1294 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/checksum/tests_checksum.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.763935 core_main_app-2.3.0/tests/utils/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1664 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/migrations/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.779013 core_main_app-2.3.0/tests/utils/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/query/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.813964 core_main_app-2.3.0/tests/utils/query/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/query/mongo/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9855 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/query/mongo/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.854630 core_main_app-2.3.0/tests/utils/requests_utls/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/requests_utls/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1436 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/requests_utls/tests_ssl.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      902 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/test_unit_apps.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      772 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/test_unit_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4010 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/tests_int_blob_downloader.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2624 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/tests_int_file.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2368 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/tests_unit_admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1726 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/tests_unit_boolean.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      402 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/tests_unit_parser.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11988 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/tests_unit_xml_operation.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4334 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/tests_view_data.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.885895 core_main_app-2.3.0/tests/utils/validation/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/validation/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1318 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/validation/tests_unit_validation.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.917664 core_main_app-2.3.0/tests/utils/xsd_flattener/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/xsd_flattener/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4358 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/xsd_flattener/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:23.003006 core_main_app-2.3.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4797 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/views/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4393 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/views/test_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    35415 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/views/tests_int_access_control.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:06.923826 core_main_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:13:37.000000 core_main_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      219 2023-07-21 02:13:37.000000 core_main_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7920 2023-07-21 02:14:06.917483 core_main_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5757 2023-07-21 02:13:37.000000 core_main_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:57.581826 core_main_app-2.4.0/core_main_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2023-07-21 02:13:37.000000 core_main_app-2.4.0/core_main_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:57.721384 core_main_app-2.4.0/core_main_app/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:37.000000 core_main_app-2.4.0/core_main_app/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11171 2023-07-21 02:13:37.000000 core_main_app-2.4.0/core_main_app/access_control/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      628 2023-07-21 02:13:37.000000 core_main_app-2.4.0/core_main_app/access_control/decorators.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      197 2023-07-21 02:13:37.000000 core_main_app-2.4.0/core_main_app/access_control/exceptions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6065 2023-07-21 02:13:37.000000 core_main_app-2.4.0/core_main_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1360 2023-07-21 02:13:37.000000 core_main_app-2.4.0/core_main_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:57.832712 core_main_app-2.4.0/core_main_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:37.000000 core_main_app-2.4.0/core_main_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      412 2023-07-21 02:13:37.000000 core_main_app-2.4.0/core_main_app/commons/constants.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/commons/enums.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4063 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/commons/exceptions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/commons/regex.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      332 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/commons/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9154 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/commons/validators.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:57.847630 core_main_app-2.4.0/core_main_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:57.878860 core_main_app-2.4.0/core_main_app/components/abstract_data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/abstract_data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5240 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/abstract_data/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:57.975669 core_main_app-2.4.0/core_main_app/components/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/blob/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2923 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/blob/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      315 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/blob/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3676 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/blob/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4022 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/blob/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      442 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/blob/utils.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:58.075342 core_main_app-2.4.0/core_main_app/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4713 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/data/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5527 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/data/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8868 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/data/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6328 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/data/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10384 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/data/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:58.116213 core_main_app-2.4.0/core_main_app/components/group/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/group/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1982 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/group/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:58.178065 core_main_app-2.4.0/core_main_app/components/lock/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/lock/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      330 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/lock/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2570 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/lock/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2665 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/lock/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:58.225955 core_main_app-2.4.0/core_main_app/components/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/mongo/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1041 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/mongo/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11024 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/mongo/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:58.309258 core_main_app-2.4.0/core_main_app/components/template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/template/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4454 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/template/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      362 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/template/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4434 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/template/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6688 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/template/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:58.391056 core_main_app-2.4.0/core_main_app/components/template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/template_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2690 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/template_version_manager/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      507 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/template_version_manager/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7272 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/template_version_manager/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4719 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/template_version_manager/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:58.446202 core_main_app-2.4.0/core_main_app/components/template_xsl_rendering/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/template_xsl_rendering/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      338 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/template_xsl_rendering/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6892 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/template_xsl_rendering/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3434 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/template_xsl_rendering/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:58.475818 core_main_app-2.4.0/core_main_app/components/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2470 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/user/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:58.568462 core_main_app-2.4.0/core_main_app/components/version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4883 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/version_manager/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3744 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/version_manager/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3248 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/version_manager/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      550 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/version_manager/utils.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:58.621780 core_main_app-2.4.0/core_main_app/components/web_page/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/web_page/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1280 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/web_page/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1097 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/web_page/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:58.652076 core_main_app-2.4.0/core_main_app/components/web_page_login/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/web_page_login/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      809 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/web_page_login/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:58.776762 core_main_app-2.4.0/core_main_app/components/workspace/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/workspace/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2493 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/workspace/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/workspace/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16858 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/workspace/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5695 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/workspace/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:58.848046 core_main_app-2.4.0/core_main_app/components/xsl_transformation/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/xsl_transformation/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      366 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/xsl_transformation/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2542 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/xsl_transformation/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4469 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/components/xsl_transformation/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1791 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:58.881884 core_main_app-2.4.0/core_main_app/middleware/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/middleware/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      638 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/middleware/timezone.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:58.976463 core_main_app-2.4.0/core_main_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16483 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      751 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/migrations/0002_site_update.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1880 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/migrations/0003_psql_full_text.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      823 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/migrations/0004_template_ordering.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      474 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/migrations/0005_template_dependencies.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      655 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/migrations/0006_blob_metadata.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      733 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:59.055959 core_main_app-2.4.0/core_main_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6351 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/permissions/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3152 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/permissions/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      644 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/permissions/rights.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      230 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/permissions/utils.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:59.105809 core_main_app-2.4.0/core_main_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:59.166983 core_main_app-2.4.0/core_main_app/rest/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/rest/blob/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4546 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/rest/blob/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19770 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/rest/blob/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:59.246885 core_main_app-2.4.0/core_main_app/rest/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/rest/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7896 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/rest/data/abstract_views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2006 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/rest/data/admin_serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3187 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/rest/data/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    37144 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/rest/data/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:59.278915 core_main_app-2.4.0/core_main_app/rest/group/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/rest/group/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      293 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/rest/group/serializers.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:59.312102 core_main_app-2.4.0/core_main_app/rest/mongo_data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/rest/mongo_data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1692 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/rest/mongo_data/serializers.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:59.364468 core_main_app-2.4.0/core_main_app/rest/template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/rest/template/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      834 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/rest/template/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4354 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/rest/template/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:59.434956 core_main_app-2.4.0/core_main_app/rest/template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/rest/template_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13930 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/rest/template_version_manager/abstract_views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2858 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/rest/template_version_manager/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      587 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/rest/template_version_manager/utils.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12279 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/rest/template_version_manager/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:59.479758 core_main_app-2.4.0/core_main_app/rest/template_xsl_rendering/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:38.000000 core_main_app-2.4.0/core_main_app/rest/template_xsl_rendering/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1168 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/rest/template_xsl_rendering/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14418 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/rest/template_xsl_rendering/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14703 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/rest/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:59.530636 core_main_app-2.4.0/core_main_app/rest/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/rest/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1157 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/rest/user/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      709 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/rest/user/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2482 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/rest/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:59.577697 core_main_app-2.4.0/core_main_app/rest/web_page/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/rest/web_page/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1042 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/rest/web_page/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4688 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/rest/web_page/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:59.635317 core_main_app-2.4.0/core_main_app/rest/workspace/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/rest/workspace/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      894 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/rest/workspace/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    23285 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/rest/workspace/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:59.680437 core_main_app-2.4.0/core_main_app/rest/xsl_transformation/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/rest/xsl_transformation/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1437 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/rest/xsl_transformation/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8160 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/rest/xsl_transformation/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8517 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:56.253429 core_main_app-2.4.0/core_main_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:56.441747 core_main_app-2.4.0/core_main_app/static/core_main_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:56.287213 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:56.268378 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/_theme/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:59.739006 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/_theme/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      251 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/_theme/css/additional.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    47539 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/_theme/css/skins.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)   110978 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/_theme/css/theme.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:59.775756 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/_theme/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    22937 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/_theme/js/app.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      578 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/_theme/js/menu.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:59.807563 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1575 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/css/data_migration.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/css/permissions.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:59.824763 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/css/templates_xslt/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1363 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/css/templates_xslt/form.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:59.840514 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/css/web_page/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       31 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/css/web_page/style.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:59.866045 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      831 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/js/display_permissions.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:59.903596 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/js/templates/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    30064 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/js/templates/data_migration.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      594 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/js/templates/data_migration.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:59.955420 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/js/templates/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1334 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/js/templates/upload/dependencies.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       94 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/js/templates/upload/dependencies.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      139 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/js/templates/upload/dependency_resolver.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:59.970655 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/js/templates_xslt/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1482 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/admin/js/templates_xslt/detail_xslt.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:56.393802 core_main_app-2.4.0/core_main_app/static/core_main_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:00.140724 core_main_app-2.4.0/core_main_app/static/core_main_app/common/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2236 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/css/XMLTree.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/css/bootstrap5.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/css/buttons.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/css/fields.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/css/highlight.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       92 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/css/loading-spinner.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1332 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/css/messages.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      317 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/css/select.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      392 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/css/share_link.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      940 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/css/switch.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      486 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/css/table.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:00.161688 core_main_app-2.4.0/core_main_app/static/core_main_app/common/css/template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       59 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/css/template/template_ordering.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      189 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/css/word-wrap.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:00.184432 core_main_app-2.4.0/core_main_app/static/core_main_app/common/css/workspace/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      333 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/css/workspace/table.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:00.219168 core_main_app-2.4.0/core_main_app/static/core_main_app/common/img/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      246 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/img/collapse.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      253 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/img/expand.png
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:00.324076 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      335 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/XMLTree.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      247 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/backtoprevious.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1828 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/csrf.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      192 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/data_detail.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      531 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/debounce.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      787 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/elementViewport.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      413 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/leave_notice.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      833 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/loading_spinner.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2197 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/messages.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:00.393472 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1292 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/modals/add.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1136 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/modals/delete.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      481 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/modals/download.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      178 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/modals/download.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1257 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/modals/edit.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      439 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/modals/error_page_modal.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:00.416395 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:00.452674 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/templates/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:00.478013 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/templates/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1086 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/templates/list/modals/disable.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      125 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/templates/list/modals/disable.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      663 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/templates/list/restore.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      124 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/templates/list/restore.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1495 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/templates/sort.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      217 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/templates/sort.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:00.534015 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/templates/versions/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:00.558581 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/templates/versions/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1029 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/templates/versions/modals/disable.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      108 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/templates/versions/modals/disable.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      537 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/templates/versions/restore.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/templates/versions/restore.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      662 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/templates/versions/set_current.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      111 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/templates/versions/set_current.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:56.383408 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/xslt/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:56.386412 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/xslt/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:00.646534 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      859 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/delete.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       64 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/delete.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1012 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/edit.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/edit.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:00.659759 core_main_app-2.4.0/core_main_app/static/core_main_app/common/xsl/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1763 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/common/xsl/xml2html.xsl
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:56.419715 core_main_app-2.4.0/core_main_app/static/core_main_app/libs/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:56.435262 core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:00.820654 core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery/3.5.1/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    89475 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery/3.5.1/jquery.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:56.407208 core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery-ui/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:00.720598 core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:00.797389 core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7006 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7074 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4676 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7013 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4632 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6313 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    37326 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)   520714 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18705 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.structure.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18671 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.theme.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:56.456333 core_main_app-2.4.0/core_main_app/static/core_main_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:00.877599 core_main_app-2.4.0/core_main_app/static/core_main_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/css/login.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       63 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/css/registration.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      387 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/css/text-editor.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:00.891523 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:00.937487 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1505 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/blob/blob_metadata.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      217 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/blob/blob_metadata.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      119 2023-07-21 02:13:39.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/blob/detail.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:00.971083 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      618 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/data/change_display.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/data/change_display.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      158 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/data/detail.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:00.994831 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/login/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      667 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/login/message.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/login/message.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1315 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/sharing_modal.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.033517 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/text_editor/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      154 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/text_editor/data_text_editor.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       73 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/text_editor/template_text_editor.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7036 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/text_editor/text_editor.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.155972 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1800 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/add_group.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      160 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/add_group.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1723 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/add_user.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/add_user.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1138 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/create_workspace.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       73 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/create_workspace.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      515 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/init.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       43 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/init.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:56.513987 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.315323 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      187 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_blob_workspace.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      187 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_data_workspace.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1587 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_workspace.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1360 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/remove_rights.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/remove_rights.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      807 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_private.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       96 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_private.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      822 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_public.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       94 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_public.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1728 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/switch_right.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      144 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/switch_right.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.340658 core_main_app-2.4.0/core_main_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2302 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/system/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.364327 core_main_app-2.4.0/core_main_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:56.789565 core_main_app-2.4.0/core_main_app/templates/core_main_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:56.550052 core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.383301 core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1302 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/admin/app_wrapper.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.438532 core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/admin/theme/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5266 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/admin/theme/base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      319 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/admin/theme/footer.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1100 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/admin/theme/header.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3483 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/admin/theme/menu.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.505599 core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      721 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/box.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1019 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/section.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.519602 core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1645 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/common/messages.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.555820 core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1463 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/user/app_wrapper.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      902 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/user/default.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5396 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/user/theme_base.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.600732 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:56.566708 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/commons/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.634955 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/commons/errors/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      401 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/commons/errors/errors.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      254 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/commons/errors/errors_wrapper.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.656806 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/commons/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      787 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/commons/upload/form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      313 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/commons/upload/upload.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      103 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/dashboard.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.680792 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/data/detail.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      383 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/data/detail_box.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1593 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/dependency_resolver.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      211 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/list_dependencies.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.721659 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.733325 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/data_migration/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8108 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/data_migration/templates_list.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      289 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/data_migration.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.776530 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2247 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/list/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      830 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/list/disabled.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.790295 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      921 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/list/modals/disable.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      542 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.803700 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      399 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/upload/base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      166 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/upload.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.839528 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/versions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3644 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/versions/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1182 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/versions/disabled.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.852271 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/versions/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      835 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/versions/modals/disable.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      677 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/versions.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.865482 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates_xslt/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.881741 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates_xslt/main/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4999 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates_xslt/main/form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      393 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates_xslt/main.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      860 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/upload_template.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.953393 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/web_page/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      166 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/web_page/login_page.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      900 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/web_page/main.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      387 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/web_page/web_page.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      375 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/web_page/web_page_unavailable.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:01.966609 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/workspaces/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      234 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/workspaces/edit_rights.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.003354 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/xslt/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.019991 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/xslt/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1332 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/xslt/list/table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      323 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/xslt/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.033052 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/xslt/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       61 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/xslt/upload/base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      161 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/xslt/upload.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:56.761597 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.063156 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1131 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/blob/tools_blob.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      664 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/blob/tools_metadata.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.119028 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/buttons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/buttons/add.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      248 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/buttons/back_to_previous.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/buttons/delete.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      190 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/buttons/edit.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      104 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/buttons/go_to.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.148213 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      189 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/commons/error.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/commons/form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      167 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/commons/form_delete.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.170049 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/commons/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      674 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/commons/upload/form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      313 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/commons/upload/upload.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.194761 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      497 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/data/detail_data.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2451 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/data/tools_data.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.208583 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/defender/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       90 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/defender/error.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.292432 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      571 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/modals/add_page_modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      745 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/modals/create_data_modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      596 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/modals/delete_page_modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1174 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/modals/download-options.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      575 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/modals/edit_page_modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      429 2023-07-21 02:13:40.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/modals/error_page_modal.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.327895 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/pagination/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3008 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/pagination/data_source_pagination.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.340891 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.364565 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/templates/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1620 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/templates/list/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      801 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/templates/list/disabled.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.388122 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/templates/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      913 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/templates/list/modals/disable.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      849 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/templates/list/modals/edit.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.402276 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/templates/versions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2367 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/templates/versions/available.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.419323 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/templates/versions/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      770 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/templates/versions/modals/disable.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      265 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/templates/versions.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.451000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/templates_xslt/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/templates_xslt/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.465392 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/templates_xslt/main/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1243 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/templates_xslt/main/form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      428 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/templates_xslt/main.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.494933 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/xslt/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.507584 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/xslt/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.530079 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/xslt/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      672 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/xslt/list/modals/delete.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1219 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/xslt/list/modals/edit.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1243 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/xslt/list/table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      255 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/xslt/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.541768 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/xslt/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/xslt/upload/base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      163 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/common/xslt/upload.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.564046 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.588642 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2067 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/blob/blob_metadata.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1063 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/blob/detail.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:56.820868 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/blob/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.636567 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/blob/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      684 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/blob/list/modals/add_metadata.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      231 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/blob/list/modals/add_metadata_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      681 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/blob/list/modals/file_upload.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      148 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/blob/list/modals/file_upload_form.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.658163 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      483 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/data/detail.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      139 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/homepage.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.686749 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/login/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2403 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/login/main.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.700481 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/login/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      534 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/login/modals/login_message.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      340 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/login/saml2_error.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.769119 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/registration/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      171 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/registration/password_reset_complete.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      486 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/registration/password_reset_confirm.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      595 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/registration/password_reset_done.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      362 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/registration/password_reset_email.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      276 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/registration/password_reset_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       14 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/registration/password_reset_subject.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.782717 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/sharing/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      274 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/sharing/button.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.808378 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/sharing/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      504 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/sharing/modals/multi-link.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1122 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/sharing/modals/single-link.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.835400 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      453 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/template/list_body.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/template/list_header.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.870380 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/text_editor/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3706 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/text_editor/text_editor.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      787 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/timezone.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.892090 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/workspaces/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1186 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/workspaces/edit_rights.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:02.923348 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/workspaces/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1612 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/workspaces/list/create_workspace.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1882 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/workspaces/list/edit_rights_table.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:03.037026 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1742 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_group.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      222 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_group_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1720 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_user.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      219 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_user_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      940 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/assign_workspace.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      411 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/assign_workspace_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1249 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/remove_rights.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1168 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/set_private.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1176 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/set_public.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      966 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/switch_right.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      147 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templates/theme.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:03.193238 core_main_app-2.4.0/core_main_app/templatetags/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templatetags/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1086 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templatetags/auth_extras.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1690 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templatetags/blob_tags.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      367 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templatetags/dict_key_extras.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      514 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templatetags/get_attribute.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      598 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templatetags/include_static.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1124 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templatetags/json_date.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      509 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templatetags/parse_date.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      642 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templatetags/stripjs.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      316 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templatetags/timestamptags.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3319 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/templatetags/xsl_transform_tag.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4791 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:03.386756 core_main_app-2.4.0/core_main_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:03.457310 core_main_app-2.4.0/core_main_app/utils/admin_site/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/admin_site/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1233 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/admin_site/model_admin_class.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      379 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/admin_site/view_only_admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2447 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/blob_downloader.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      405 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/boolean.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1137 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/checksum.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1998 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/custom_context_processors.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:03.490740 core_main_app-2.4.0/core_main_app/utils/databases/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/databases/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      627 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/databases/backend.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:03.529576 core_main_app-2.4.0/core_main_app/utils/databases/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      574 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/databases/mongo/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1584 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/databases/mongo/mongoengine_database.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      873 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/databases/mongo/pymongo_database.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      286 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/datetime.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9575 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/decorators.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2805 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/file.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      377 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/group.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:03.583745 core_main_app-2.4.0/core_main_app/utils/integration_tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/integration_tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      262 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/integration_tests/fixture_interface.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1641 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/integration_tests/integration_base_test_case.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1031 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/integration_tests/integration_base_transaction_test_case.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      319 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/labels.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:03.622687 core_main_app-2.4.0/core_main_app/utils/logger/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/logger/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1762 2023-07-21 02:13:41.000000 core_main_app-2.4.0/core_main_app/utils/logger/logger_utils.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      438 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/markdown_parser.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      957 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/migrations.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:03.650300 core_main_app-2.4.0/core_main_app/utils/notifications/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/notifications/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3448 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/notifications/mail.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:03.677418 core_main_app-2.4.0/core_main_app/utils/notifications/tasks/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/notifications/tasks/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2566 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/notifications/tasks/task_mail.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:03.690467 core_main_app-2.4.0/core_main_app/utils/pagination/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/pagination/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:03.719499 core_main_app-2.4.0/core_main_app/utils/pagination/django_paginator/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/pagination/django_paginator/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      773 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/pagination/django_paginator/results_paginator.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:03.745496 core_main_app-2.4.0/core_main_app/utils/pagination/mongoengine_paginator/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/pagination/mongoengine_paginator/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1109 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/pagination/mongoengine_paginator/paginator.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:03.785841 core_main_app-2.4.0/core_main_app/utils/pagination/rest_framework_paginator/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/pagination/rest_framework_paginator/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      525 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/pagination/rest_framework_paginator/pagination.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1108 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/pagination/rest_framework_paginator/rest_framework_paginator.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      458 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/parser.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:03.813542 core_main_app-2.4.0/core_main_app/utils/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      145 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/query/constants.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:03.868077 core_main_app-2.4.0/core_main_app/utils/query/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/query/mongo/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14676 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/query/mongo/prepare.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3095 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/query/mongo/query_builder.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:03.917930 core_main_app-2.4.0/core_main_app/utils/raw_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/raw_query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1622 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/raw_query/common.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3901 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/raw_query/django_raw_query.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2134 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/raw_query/mongo_raw_query.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3182 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/rendering.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:03.965512 core_main_app-2.4.0/core_main_app/utils/requests_utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/requests_utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      568 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/requests_utils/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1663 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/requests_utils/requests_utils.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2054 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/requests_utils/ssl.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.050534 core_main_app-2.4.0/core_main_app/utils/resolvers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/resolvers/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1184 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/resolvers/requests_resolver.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1072 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/resolvers/resolver_utils.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/resolvers/xsd_uri_resolvers.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.081391 core_main_app-2.4.0/core_main_app/utils/saml2/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/saml2/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8886 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/saml2/utils.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.120620 core_main_app-2.4.0/core_main_app/utils/storage/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/storage/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3523 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/storage/gridfs_storage.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1791 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/storage/storage.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.157307 core_main_app-2.4.0/core_main_app/utils/tests_tools/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      852 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/tests_tools/MockUser.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5344 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/tests_tools/RequestMock.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/tests_tools/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3654 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.196689 core_main_app-2.4.0/core_main_app/utils/validation/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/validation/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1162 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/validation/regex_validation.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      644 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/validation/xpath_validation.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.224622 core_main_app-2.4.0/core_main_app/utils/view_builders/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/view_builders/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6572 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/view_builders/data.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16047 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/xml.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.261845 core_main_app-2.4.0/core_main_app/utils/xsd_flattener/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/xsd_flattener/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2095 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/xsd_flattener/xsd_flattener_database_url.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1000 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/utils/xsd_flattener/xsd_flattener_requests_url.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.275043 core_main_app-2.4.0/core_main_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.325415 core_main_app-2.4.0/core_main_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4442 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/views/admin/ajax.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.346168 core_main_app-2.4.0/core_main_app/views/admin/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/views/admin/commons/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.376575 core_main_app-2.4.0/core_main_app/views/admin/commons/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/views/admin/commons/upload/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      439 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/views/admin/commons/upload/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4912 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21051 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.442788 core_main_app-2.4.0/core_main_app/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/views/common/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7191 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/views/common/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      459 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/views/common/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    35208 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/views/common/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.502013 core_main_app-2.4.0/core_main_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21825 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6390 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/views/user/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9289 2023-07-21 02:13:42.000000 core_main_app-2.4.0/core_main_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:57.660766 core_main_app-2.4.0/core_main_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7920 2023-07-21 02:13:53.000000 core_main_app-2.4.0/core_main_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    32554 2023-07-21 02:13:55.000000 core_main_app-2.4.0/core_main_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:13:53.000000 core_main_app-2.4.0/core_main_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      475 2023-07-21 02:13:53.000000 core_main_app-2.4.0/core_main_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       25 2023-07-21 02:13:53.000000 core_main_app-2.4.0/core_main_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.539654 core_main_app-2.4.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:42.000000 core_main_app-2.4.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11121 2023-07-21 02:13:43.000000 core_main_app-2.4.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      278 2023-07-21 02:13:43.000000 core_main_app-2.4.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2023-07-21 02:13:45.000000 core_main_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2023-07-21 02:13:45.000000 core_main_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       92 2023-07-21 02:13:45.000000 core_main_app-2.4.0/requirements.dev.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       20 2023-07-21 02:13:45.000000 core_main_app-2.4.0/requirements.mongo.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      323 2023-07-21 02:13:45.000000 core_main_app-2.4.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:14:06.925856 core_main_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2104 2023-07-21 02:13:45.000000 core_main_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.626296 core_main_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:45.000000 core_main_app-2.4.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.652370 core_main_app-2.4.0/tests/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:45.000000 core_main_app-2.4.0/tests/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3415 2023-07-21 02:13:45.000000 core_main_app-2.4.0/tests/access_control/tests_access_control.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.689159 core_main_app-2.4.0/tests/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:45.000000 core_main_app-2.4.0/tests/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3764 2023-07-21 02:13:45.000000 core_main_app-2.4.0/tests/commons/tests_validators.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.703057 core_main_app-2.4.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:45.000000 core_main_app-2.4.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.755490 core_main_app-2.4.0/tests/components/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:45.000000 core_main_app-2.4.0/tests/components/blob/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.782676 core_main_app-2.4.0/tests/components/blob/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:45.000000 core_main_app-2.4.0/tests/components/blob/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3165 2023-07-21 02:13:45.000000 core_main_app-2.4.0/tests/components/blob/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6398 2023-07-21 02:13:45.000000 core_main_app-2.4.0/tests/components/blob/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    38881 2023-07-21 02:13:45.000000 core_main_app-2.4.0/tests/components/blob/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2333 2023-07-21 02:13:45.000000 core_main_app-2.4.0/tests/components/blob/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.847997 core_main_app-2.4.0/tests/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:45.000000 core_main_app-2.4.0/tests/components/data/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.875808 core_main_app-2.4.0/tests/components/data/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:45.000000 core_main_app-2.4.0/tests/components/data/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    28078 2023-07-21 02:13:45.000000 core_main_app-2.4.0/tests/components/data/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    66538 2023-07-21 02:13:45.000000 core_main_app-2.4.0/tests/components/data/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    83957 2023-07-21 02:13:45.000000 core_main_app-2.4.0/tests/components/data/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3730 2023-07-21 02:13:45.000000 core_main_app-2.4.0/tests/components/data/tests_int_ordering.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    28509 2023-07-21 02:13:45.000000 core_main_app-2.4.0/tests/components/data/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.902554 core_main_app-2.4.0/tests/components/group/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:45.000000 core_main_app-2.4.0/tests/components/group/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.940076 core_main_app-2.4.0/tests/components/group/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:45.000000 core_main_app-2.4.0/tests/components/group/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      570 2023-07-21 02:13:46.000000 core_main_app-2.4.0/tests/components/group/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      879 2023-07-21 02:13:46.000000 core_main_app-2.4.0/tests/components/group/fixtures/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4760 2023-07-21 02:13:46.000000 core_main_app-2.4.0/tests/components/group/tests_int.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:04.989564 core_main_app-2.4.0/tests/components/lock/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:46.000000 core_main_app-2.4.0/tests/components/lock/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4153 2023-07-21 02:13:46.000000 core_main_app-2.4.0/tests/components/lock/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2440 2023-07-21 02:13:46.000000 core_main_app-2.4.0/tests/components/lock/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:05.048963 core_main_app-2.4.0/tests/components/mongo_data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:47.000000 core_main_app-2.4.0/tests/components/mongo_data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    75687 2023-07-21 02:13:48.000000 core_main_app-2.4.0/tests/components/mongo_data/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1466 2023-07-21 02:13:48.000000 core_main_app-2.4.0/tests/components/mongo_data/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:05.112549 core_main_app-2.4.0/tests/components/template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:48.000000 core_main_app-2.4.0/tests/components/template/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:05.154678 core_main_app-2.4.0/tests/components/template/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:48.000000 core_main_app-2.4.0/tests/components/template/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2078 2023-07-21 02:13:48.000000 core_main_app-2.4.0/tests/components/template/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    46022 2023-07-21 02:13:48.000000 core_main_app-2.4.0/tests/components/template/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7215 2023-07-21 02:13:48.000000 core_main_app-2.4.0/tests/components/template/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:05.194588 core_main_app-2.4.0/tests/components/template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:48.000000 core_main_app-2.4.0/tests/components/template_version_manager/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:05.262775 core_main_app-2.4.0/tests/components/template_version_manager/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:48.000000 core_main_app-2.4.0/tests/components/template_version_manager/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6470 2023-07-21 02:13:48.000000 core_main_app-2.4.0/tests/components/template_version_manager/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    54686 2023-07-21 02:13:48.000000 core_main_app-2.4.0/tests/components/template_version_manager/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17617 2023-07-21 02:13:48.000000 core_main_app-2.4.0/tests/components/template_version_manager/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:05.302691 core_main_app-2.4.0/tests/components/template_xsl_rendering/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:48.000000 core_main_app-2.4.0/tests/components/template_xsl_rendering/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:05.333292 core_main_app-2.4.0/tests/components/template_xsl_rendering/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:48.000000 core_main_app-2.4.0/tests/components/template_xsl_rendering/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3266 2023-07-21 02:13:48.000000 core_main_app-2.4.0/tests/components/template_xsl_rendering/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7896 2023-07-21 02:13:48.000000 core_main_app-2.4.0/tests/components/template_xsl_rendering/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9565 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/components/template_xsl_rendering/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:05.364525 core_main_app-2.4.0/tests/components/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/components/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:05.409502 core_main_app-2.4.0/tests/components/user/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/components/user/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1552 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/components/user/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1429 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/components/user/fixtures/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7733 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/components/user/tests_int.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:05.453490 core_main_app-2.4.0/tests/components/version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/components/version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    61614 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/components/version_manager/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9899 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/components/version_manager/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:05.485856 core_main_app-2.4.0/tests/components/web_page/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/components/web_page/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4846 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/components/web_page/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:05.515942 core_main_app-2.4.0/tests/components/web_page_login/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/components/web_page_login/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3905 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/components/web_page_login/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:05.544408 core_main_app-2.4.0/tests/components/workspace/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/components/workspace/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:05.590893 core_main_app-2.4.0/tests/components/workspace/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/components/workspace/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1235 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/components/workspace/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      919 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/components/workspace/fixtures/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7478 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/components/workspace/tests_int.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:05.621660 core_main_app-2.4.0/tests/components/xsl_transformation/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/components/xsl_transformation/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12828 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/components/xsl_transformation/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:05.656348 core_main_app-2.4.0/tests/middleware/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/middleware/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1664 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/middleware/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      356 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/mocks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:05.693584 core_main_app-2.4.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:05.758014 core_main_app-2.4.0/tests/rest/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/rest/blob/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    31044 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/rest/blob/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    26694 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/rest/blob/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/rest/blob/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:05.833651 core_main_app-2.4.0/tests/rest/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/rest/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    47395 2023-07-21 02:13:49.000000 core_main_app-2.4.0/tests/rest/data/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    40361 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/data/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12424 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/data/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:05.909150 core_main_app-2.4.0/tests/rest/template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/template/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2518 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/template/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5026 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/template/tests_permission.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4802 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/template/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:05.994142 core_main_app-2.4.0/tests/rest/template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/template_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    45007 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/template_version_manager/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    41433 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/template_version_manager/tests_permission.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5358 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/template_version_manager/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:06.044532 core_main_app-2.4.0/tests/rest/template_xsl_rendering/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/template_xsl_rendering/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11418 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/template_xsl_rendering/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13879 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/template_xsl_rendering/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3610 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/tests_views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:06.107384 core_main_app-2.4.0/tests/rest/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1737 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/user/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3137 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/user/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      886 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/user/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:06.137491 core_main_app-2.4.0/tests/rest/web_page/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/web_page/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6164 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/web_page/tests_permission.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:06.215285 core_main_app-2.4.0/tests/rest/workspace/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/workspace/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    71809 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/workspace/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    48644 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/workspace/tests_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:06.275716 core_main_app-2.4.0/tests/rest/xsl_transformation/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/xsl_transformation/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:06.304780 core_main_app-2.4.0/tests/rest/xsl_transformation/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/xsl_transformation/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1283 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/xsl_transformation/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11618 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/xsl_transformation/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12753 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/xsl_transformation/tests_permission.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4365 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest/xsl_transformation/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      738 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/rest_urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:06.333346 core_main_app-2.4.0/tests/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4668 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/system/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:06.397615 core_main_app-2.4.0/tests/templatetags/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/templatetags/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1946 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/templatetags/test_blob_tags.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1364 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/templatetags/test_get_attribute.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1486 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/templatetags/test_parse_date.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2779 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      293 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/test_settings_sqlite3.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4437 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:06.556127 core_main_app-2.4.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:06.588856 core_main_app-2.4.0/tests/utils/checksum/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/utils/checksum/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1294 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/utils/checksum/tests_checksum.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:06.625513 core_main_app-2.4.0/tests/utils/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/utils/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1664 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/utils/migrations/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:06.640327 core_main_app-2.4.0/tests/utils/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/utils/query/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:06.675161 core_main_app-2.4.0/tests/utils/query/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/utils/query/mongo/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9855 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/utils/query/mongo/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:06.706396 core_main_app-2.4.0/tests/utils/requests_utls/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/utils/requests_utls/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1436 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/utils/requests_utls/tests_ssl.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      902 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/utils/test_unit_apps.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      772 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/utils/test_unit_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4010 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/utils/tests_int_blob_downloader.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2624 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/utils/tests_int_file.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2368 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/utils/tests_unit_admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1726 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/utils/tests_unit_boolean.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      402 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/utils/tests_unit_parser.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11988 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/utils/tests_unit_xml_operation.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4334 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/utils/tests_view_data.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:06.738663 core_main_app-2.4.0/tests/utils/validation/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/utils/validation/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1318 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/utils/validation/tests_unit_validation.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:06.769538 core_main_app-2.4.0/tests/utils/xsd_flattener/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/utils/xsd_flattener/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4358 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/utils/xsd_flattener/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:06.872146 core_main_app-2.4.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4797 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/views/fixtures.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:06.903341 core_main_app-2.4.0/tests/views/forms/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/views/forms/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3310 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/views/forms/test_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10777 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/views/test_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    57978 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/views/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1328 2023-07-21 02:13:50.000000 core_main_app-2.4.0/tests/views/tests_permissions.py
```

### Comparing `core_main_app-2.3.0/LICENSE.md` & `core_main_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/PKG-INFO` & `core_main_app-2.4.0/core_main_app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: core_main_app
-Version: 2.3.0
+Name: core-main-app
+Version: 2.4.0
 Summary: Main functionalities for the curator core project
 Home-page: https://github.com/usnistgov/core_main_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =============
         Core Main App
@@ -47,34 +47,24 @@
         
         Configuration
         =============
         
         Edit the setting.py file
         ------------------------
         
-        Add the ``"core_main_app"`` and ``"tz_detect"`` under ``INSTALLED_APPS`` as
+        Add the ``"core_main_app"`` under ``INSTALLED_APPS`` as
         such:
         
         .. code:: python
         
             INSTALLED_APPS = [
                 ...
-                "tz_detect",
                 "core_main_app",
             ]
         
-        Add the middleware required by ``tz_detect``:
-        
-        .. code:: python
-        
-            MIDDLEWARE = (
-                ...
-                'tz_detect.middleware.TimezoneMiddleware',
-            )
-        
         
         Edit the urls.py file
         ---------------------
         
         Add the ``core_main_app`` urls to the Django project as such.
         
         .. code:: python
```

### Comparing `core_main_app-2.3.0/README.rst` & `core_main_app-2.4.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -39,34 +39,24 @@
 
 Configuration
 =============
 
 Edit the setting.py file
 ------------------------
 
-Add the ``"core_main_app"`` and ``"tz_detect"`` under ``INSTALLED_APPS`` as
+Add the ``"core_main_app"`` under ``INSTALLED_APPS`` as
 such:
 
 .. code:: python
 
     INSTALLED_APPS = [
         ...
-        "tz_detect",
         "core_main_app",
     ]
 
-Add the middleware required by ``tz_detect``:
-
-.. code:: python
-
-    MIDDLEWARE = (
-        ...
-        'tz_detect.middleware.TimezoneMiddleware',
-    )
-
 
 Edit the urls.py file
 ---------------------
 
 Add the ``core_main_app`` urls to the Django project as such.
 
 .. code:: python
```

### Comparing `core_main_app-2.3.0/core_main_app/access_control/api.py` & `core_main_app-2.4.0/core_main_app/access_control/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Set of functions to define the common rules for access control across collections
 """
 import logging
 
 from django.contrib.auth.models import User
 
 from core_main_app.access_control.exceptions import AccessControlError
-from core_main_app.commons.exceptions import ApiError
+from core_main_app.commons.exceptions import ApiError, DoesNotExist
 from core_main_app.components.workspace import api as workspace_api
 from core_main_app.permissions import api as permissions_api, rights as rights
 from django.conf import settings
 from core_main_app.settings import (
     CAN_SET_PUBLIC_DATA_TO_PRIVATE,
 )
 
@@ -69,14 +69,16 @@
     try:
         request = kwargs["request"]
         if request and request.user.is_superuser:
             return func(*args, **kwargs)
 
     except ApiError as api_error_exception:
         raise api_error_exception
+    except DoesNotExist as dne_exception:
+        raise dne_exception
     except Exception as exception:
         logger.warning(
             f"has_perm_administration threw an exception: {str(exception)}"
         )
     raise AccessControlError("The user doesn't have enough rights.")
```

### Comparing `core_main_app-2.3.0/core_main_app/access_control/decorators.py` & `core_main_app-2.4.0/core_main_app/access_control/decorators.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/admin.py` & `core_main_app-2.4.0/core_main_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/apps.py` & `core_main_app-2.4.0/core_main_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/commons/exceptions.py` & `core_main_app-2.4.0/core_main_app/commons/exceptions.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/commons/validators.py` & `core_main_app-2.4.0/core_main_app/commons/validators.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/abstract_data/models.py` & `core_main_app-2.4.0/core_main_app/components/abstract_data/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/blob/models.py` & `core_main_app-2.4.0/core_main_app/components/blob/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """ Blob model
 """
+from django.contrib.auth.models import User
 from django.core.exceptions import ObjectDoesNotExist
 from django.core.validators import RegexValidator
 from django.db import models
 
 from core_main_app.commons import exceptions
 from core_main_app.commons.regex import NOT_EMPTY_OR_WHITESPACES
+from core_main_app.components.blob.access_control import (
+    filter_accessible_metadata,
+)
 from core_main_app.components.workspace.models import Workspace
 from core_main_app.settings import CHECKSUM_ALGORITHM
 from core_main_app.utils.checksum import compute_checksum
 from core_main_app.utils.storage.storage import (
     user_directory_path,
     core_file_storage,
 )
@@ -41,14 +45,35 @@
     )
     checksum = models.CharField(
         max_length=512, blank=True, default=None, null=True
     )
 
     creation_date = models.DateTimeField(auto_now_add=True)
 
+    @property
+    def owner_name(self):
+        """Get owner name
+
+        Returns:
+
+        """
+        return User.objects.get(pk=self.user_id).username
+
+    def metadata(self, user):
+        """Get blob metadata
+
+        Args:
+            user:
+
+        Returns:
+
+        """
+        # Access _metadata with ACL check
+        return filter_accessible_metadata(self._metadata.all(), user)
+
     @staticmethod
     def get_by_id(blob_id):
         """Return the object with the given id.
 
         Args:
             blob_id:
```

### Comparing `core_main_app-2.3.0/core_main_app/components/data/access_control.py` & `core_main_app-2.4.0/core_main_app/components/data/access_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 
 from core_main_app.access_control.api import (
     has_perm_publish,
     check_can_read_list,
     can_write_in_workspace,
     _check_anonymous_access,
+    _check_can_read,
 )
 from core_main_app.components.workspace import api as workspace_api
 from core_main_app.permissions import rights as rights
 from core_main_app.settings import (
     VERIFY_DATA_ACCESS,
 )
 from django.conf import settings
@@ -192,7 +193,27 @@
 
     Returns:
 
     """
     return can_write_in_workspace(
         func, data, workspace, user, rights.PUBLISH_DATA
     )
+
+
+def can_read_blob(func, data, user):
+    """Can read from object id.
+
+    Args:
+        func:
+        data:
+        user:
+
+    Returns:
+
+    """
+    if user.is_superuser:
+        return func(data, user)
+
+    if data._blob is not None:
+        _check_can_read(data._blob, user)
+
+    return func(data, user)
```

### Comparing `core_main_app-2.3.0/core_main_app/components/data/admin_site.py` & `core_main_app-2.4.0/core_main_app/components/data/admin_site.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/data/api.py` & `core_main_app-2.4.0/core_main_app/components/data/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 @access_control(access_control_api.can_read_or_write_in_workspace)
 def get_all_by_workspace(workspace, user, order_by_field=DATA_SORTING_FIELDS):
     """Get all data that belong to the workspace.
 
     Args:
         workspace:
+        user:
         order_by_field:
 
     Returns:
 
     """
     return Data.get_all_by_workspace(workspace, order_by_field)
```

### Comparing `core_main_app-2.3.0/core_main_app/components/data/models.py` & `core_main_app-2.4.0/core_main_app/components/data/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 from django.conf import settings
 from django.contrib.auth.models import User
 from django.contrib.postgres.indexes import GinIndex
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import models
 from django.db.models import Q
 
+from core_main_app.access_control.decorators import access_control
 from core_main_app.commons import exceptions
 from core_main_app.components.abstract_data.models import AbstractData
+from core_main_app.components.data.access_control import can_read_blob
 from core_main_app.components.template.models import Template
 from core_main_app.components.workspace.models import Workspace
+from core_main_app.components.blob.models import Blob
 
 
 # TODO: Create publication workflow manager
 # TODO: execute_query / execute_query_full_result -> use find method (RETURN FULL OBJECT)
 
 
 class Data(AbstractData):
@@ -23,14 +26,22 @@
     template = models.ForeignKey(
         Template, blank=False, on_delete=models.CASCADE
     )
     user_id = models.CharField(blank=False, max_length=200)
     workspace = models.ForeignKey(
         Workspace, blank=True, on_delete=models.SET_NULL, null=True
     )
+    _blob = models.ForeignKey(
+        Blob,
+        on_delete=models.SET_NULL,
+        null=True,
+        blank=True,
+        default=None,
+        related_name="_metadata",
+    )
 
     class Meta:
         """Meta"""
 
         verbose_name = "Data"
         verbose_name_plural = "Data"
         indexes = [
@@ -50,14 +61,26 @@
         """Get owner name
 
         Returns:
 
         """
         return User.objects.get(pk=self.user_id).username
 
+    @access_control(can_read_blob)
+    def blob(self, user):
+        """
+
+        Args:
+            user:
+
+        Returns:
+
+        """
+        return self._blob
+
     def get_dict_content(self):
         """Get dict_content from object or from MongoDB
 
         Returns:
 
         """
         if settings.MONGODB_INDEXING:
```

### Comparing `core_main_app-2.3.0/core_main_app/components/data/tasks.py` & `core_main_app-2.4.0/core_main_app/components/data/tasks.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/group/api.py` & `core_main_app-2.4.0/core_main_app/components/group/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/lock/api.py` & `core_main_app-2.4.0/core_main_app/components/lock/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/lock/models.py` & `core_main_app-2.4.0/core_main_app/components/lock/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/mongo/api.py` & `core_main_app-2.4.0/core_main_app/components/mongo/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/mongo/models.py` & `core_main_app-2.4.0/core_main_app/components/mongo/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,38 @@
 
                 Returns:
 
                 """
                 return Template.get_by_id(self._template_id)
 
             @property
+            def _blob(self):
+                """Return blob object
+
+                Returns:
+
+                """
+                try:
+                    return Data.get_by_id(self.data_id)._blob
+                except Exception:
+                    logger.error("Unable to get MongoData._blob")
+                    return None
+
+            def blob(self, user):
+                """Return blob object
+
+                Args:
+                    user:
+
+                Returns:
+
+                """
+                return Data.get_by_id(self.data_id).blob(user)
+
+            @property
             def template_id(self):
                 """Return template id
 
                 Returns:
 
                 """
                 return self._template_id
```

### Comparing `core_main_app-2.3.0/core_main_app/components/template/access_control.py` & `core_main_app-2.4.0/core_main_app/components/template/access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/template/api.py` & `core_main_app-2.4.0/core_main_app/components/template/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/template/models.py` & `core_main_app-2.4.0/core_main_app/components/template/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,17 @@
         max_length=512, blank=True, default=None, null=True
     )
     user = models.CharField(
         blank=True, max_length=200, null=True, default=None
     )
     hash = models.CharField(max_length=200)
     _display_name = models.CharField(blank=True, max_length=200)
-    dependencies = models.ManyToManyField("self", blank=True, default=[])
+    dependencies = models.ManyToManyField(
+        "self", blank=True, default=[], symmetrical=False
+    )
     creation_date = models.DateTimeField(auto_now_add=True)
     _cls = models.CharField(default="Template", max_length=200)
     _content = None
 
     @property
     def content(self):
         """Read template content
```

### Comparing `core_main_app-2.3.0/core_main_app/components/template_version_manager/access_control.py` & `core_main_app-2.4.0/core_main_app/components/template_version_manager/access_control.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """ Template Version Manager Access Control
 """
 
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.components.template_version_manager.models import (
     TemplateVersionManager,
 )
+from core_main_app.components.template_version_manager import (
+    api as template_version_manager_api,
+)
 from core_main_app.utils.requests_utils.access_control import (
     get_request_from_args,
 )
 
 
 def can_write(func, *args, **kwargs):
     """Can write template.
@@ -47,42 +50,50 @@
             return func(*args, **kwargs)
 
     raise AccessControlError(
         "Template VM: The user doesn't have enough rights."
     )
 
 
-def can_write_list(func, template_version_manager_list, user):
+def can_write_list(func, template_version_manager_list_ids, request):
     """Can write template version manager list.
 
     Args:
         func:
-        template_version_manager_list:
-        user:
+        template_version_manager_list_ids:
+        request:
 
     Returns:
 
     """
     # super user
+    user = request.user
     if user.is_superuser:
-        return func(template_version_manager_list, user)
+        return func(template_version_manager_list_ids, request)
 
     # anonymous can not write
     if user.is_anonymous:
         raise AccessControlError(
             "Template VM: The user doesn't have enough rights."
         )
+    # get template version manager list
+    template_version_manager_list = (
+        template_version_manager_api.get_by_id_list(
+            template_version_manager_list_ids, request
+        )
+    )
+
     for template_version_manager in template_version_manager_list:
         # user is set
         if template_version_manager.user:
             if template_version_manager.user != str(user.id):
                 raise AccessControlError(
                     "Template VM: The user doesn't have enough rights."
                 )
         # user is not set
         else:
             if not user.is_staff:
                 raise AccessControlError(
                     "Template VM: The user doesn't have enough rights."
                 )
 
-    return func(template_version_manager_list, user)
+    return func(template_version_manager_list_ids, request)
```

### Comparing `core_main_app-2.3.0/core_main_app/components/template_version_manager/api.py` & `core_main_app-2.4.0/core_main_app/components/template_version_manager/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """
 Template Version Manager API
 """
+from core_main_app.access_control.exceptions import AccessControlError
+
 from core_main_app.access_control.api import is_superuser
 from core_main_app.access_control.decorators import access_control
+from core_main_app.commons import exceptions
 from core_main_app.components.template import api as template_api
 from core_main_app.components.template.access_control import (
     can_read,
     can_read_global,
 )
 from core_main_app.components.template_version_manager.access_control import (
     can_write,
@@ -205,42 +208,74 @@
 
     """
     return TemplateVersionManager.get_active_global_version_manager_by_title(
         version_manager_title
     )
 
 
-@access_control(can_read_list)
-def sort_by_id_list(list_id, request):
-    """sort a version managers with the given id list.
+def _update_template_version_manager_ordering(list_id, request):
+    """Update template version manager ordering.
 
     Args:
         list_id:
-        request
+        request:
 
     Returns:
 
     """
+
     tvm_list = dict(
         [(tvm.id, tvm) for tvm in get_by_id_list(list_id, request)]
     )
+    # Check if all templates have been found
+    if len(list_id) > len(tvm_list):
+        raise exceptions.DoesNotExist(
+            "One or more templates could not be found"
+        )
+    template_version_manager_sorted_by_id_list = [
+        tvm_list[int(id)] for id in list_id
+    ]
 
-    return [tvm_list[int(id)] for id in list_id]
+    for counter, template_version_manager in enumerate(
+        template_version_manager_sorted_by_id_list, 1
+    ):
+        template_version_manager.display_rank = counter
+        template_version_manager.save()
 
 
 @access_control(can_write_list)
-def update_templates_ordering(template_version_manager_list, user):
+def update_user_template_ordering(list_id, request):
     """Update templates ordering.
 
     Args:
-        template_version_manager_list:
-        user:
+        list_id:
+        request:
 
     Returns:
 
     """
-
-    for counter, template_version_manager in enumerate(
-        template_version_manager_list, 1
+    if any(
+        tvm.user is None or tvm.user != str(request.user.id)
+        for tvm in get_by_id_list(list_id, request)
     ):
-        template_version_manager.display_rank = counter
-        template_version_manager.save()
+        raise AccessControlError(
+            "You don't have the rights to perform this action."
+        )
+    _update_template_version_manager_ordering(list_id, request)
+
+
+@access_control(is_superuser)
+def update_global_template_ordering(list_id, request):
+    """Update templates ordering.
+
+    Args:
+        list_id:
+        request:
+
+    Returns:
+
+    """
+    if any(tvm.user is not None for tvm in get_by_id_list(list_id, request)):
+        raise AccessControlError(
+            "You don't have the rights to perform this action."
+        )
+    _update_template_version_manager_ordering(list_id, request)
```

### Comparing `core_main_app-2.3.0/core_main_app/components/template_version_manager/models.py` & `core_main_app-2.4.0/core_main_app/components/template_version_manager/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/template_xsl_rendering/api.py` & `core_main_app-2.4.0/core_main_app/components/template_xsl_rendering/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/template_xsl_rendering/models.py` & `core_main_app-2.4.0/core_main_app/components/template_xsl_rendering/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/user/api.py` & `core_main_app-2.4.0/core_main_app/components/user/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/version_manager/access_control.py` & `core_main_app-2.4.0/core_main_app/components/version_manager/access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/version_manager/api.py` & `core_main_app-2.4.0/core_main_app/components/version_manager/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/version_manager/models.py` & `core_main_app-2.4.0/core_main_app/components/version_manager/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/version_manager/utils.py` & `core_main_app-2.4.0/core_main_app/components/version_manager/utils.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/web_page/api.py` & `core_main_app-2.4.0/core_main_app/components/web_page/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/web_page/models.py` & `core_main_app-2.4.0/core_main_app/components/web_page/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/web_page_login/api.py` & `core_main_app-2.4.0/core_main_app/components/web_page_login/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/workspace/access_control.py` & `core_main_app-2.4.0/core_main_app/components/workspace/access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/workspace/api.py` & `core_main_app-2.4.0/core_main_app/components/workspace/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/workspace/models.py` & `core_main_app-2.4.0/core_main_app/components/workspace/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/xsl_transformation/api.py` & `core_main_app-2.4.0/core_main_app/components/xsl_transformation/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/components/xsl_transformation/models.py` & `core_main_app-2.4.0/core_main_app/components/xsl_transformation/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/menus.py` & `core_main_app-2.4.0/core_main_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/migrations/0001_initial.py` & `core_main_app-2.4.0/core_main_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/migrations/0002_site_update.py` & `core_main_app-2.4.0/core_main_app/migrations/0002_site_update.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/migrations/0003_psql_full_text.py` & `core_main_app-2.4.0/core_main_app/migrations/0003_psql_full_text.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/migrations/0004_template_ordering.py` & `core_main_app-2.4.0/core_main_app/migrations/0004_template_ordering.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/models.py` & `core_main_app-2.4.0/core_main_app/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/permissions/api.py` & `core_main_app-2.4.0/core_main_app/permissions/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/permissions/discover.py` & `core_main_app-2.4.0/core_main_app/permissions/discover.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/permissions/rights.py` & `core_main_app-2.4.0/core_main_app/permissions/rights.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/rest/blob/serializers.py` & `core_main_app-2.4.0/core_main_app/rest/blob/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/rest/blob/views.py` & `core_main_app-2.4.0/core_main_app/rest/blob/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 )
 from rest_framework.response import Response
 from rest_framework.views import APIView
 
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.commons import exceptions
 from core_main_app.components.blob import api as blob_api
+from core_main_app.components.data import api as data_api
 from core_main_app.components.user import api as user_api
 from core_main_app.components.workspace import api as workspace_api
 from core_main_app.rest.blob.serializers import (
     BlobSerializer,
     DeleteBlobsSerializer,
 )
 from core_main_app.utils.file import get_file_http_response
@@ -613,7 +614,127 @@
             content = {"message": str(ace)}
             return Response(content, status=status.HTTP_403_FORBIDDEN)
         except Exception as api_exception:
             content = {"message": str(api_exception)}
             return Response(
                 content, status=status.HTTP_500_INTERNAL_SERVER_ERROR
             )
+
+
+class BlobMetadata(APIView):
+    """Blob Metadata"""
+
+    permission_classes = (IsAuthenticated,)
+
+    def get_blob(self, request, pk):
+        """Get Blob from db
+
+        Args:
+
+            request: HTTP request
+            pk: ObjectId
+
+        Returns:
+
+            Blob
+        """
+        try:
+            return blob_api.get_by_id(pk, request.user)
+        except exceptions.DoesNotExist:
+            raise Http404
+
+    def get_metatada(self, request, metadata_id):
+        """Get Data from db
+
+        Args:
+
+            request: HTTP request
+            metadata_id: ObjectId
+
+        Returns:
+
+            Blob
+        """
+        try:
+            return data_api.get_by_id(metadata_id, request.user)
+        except exceptions.DoesNotExist:
+            raise Http404
+
+    def post(self, request, pk, metadata_id):
+        """Add Metadata to Blob
+
+        Args:
+
+            request: HTTP request
+            pk: Blob id
+            metadata_id: Data id
+
+        Returns:
+
+            - code: 200
+              content:
+            - code: 403
+              content: Authentication error
+            - code: 404
+              content: Object was not found
+            - code: 500
+              content: Internal server error
+        """
+        try:
+            # Get objects
+            blob_object = self.get_blob(request, pk)
+            metadata_object = self.get_metatada(request, metadata_id)
+            # Update
+            blob_api.add_metadata(blob_object, metadata_object, request.user)
+            return Response()
+        except AccessControlError as exception:
+            content = {"message": str(exception)}
+            return Response(content, status=status.HTTP_403_FORBIDDEN)
+        except Http404:
+            content = {"message": "Blob not found."}
+            return Response(content, status=status.HTTP_404_NOT_FOUND)
+        except Exception as api_exception:
+            content = {"message": str(api_exception)}
+            return Response(
+                content, status=status.HTTP_500_INTERNAL_SERVER_ERROR
+            )
+
+    def delete(self, request, pk, metadata_id):
+        """Remove Metadata from Blob
+
+        Args:
+
+            request: HTTP request
+            pk: Blob id
+            metadata_id: Data id
+
+        Returns:
+
+            - code: 200
+              content:
+            - code: 403
+              content: Authentication error
+            - code: 404
+              content: Object was not found
+            - code: 500
+              content: Internal server error
+        """
+        try:
+            # Get objects
+            blob_object = self.get_blob(request, pk)
+            metadata_object = self.get_metatada(request, metadata_id)
+            # Update
+            blob_api.remove_metadata(
+                blob_object, metadata_object, request.user
+            )
+            return Response()
+        except AccessControlError as exception:
+            content = {"message": str(exception)}
+            return Response(content, status=status.HTTP_403_FORBIDDEN)
+        except Http404:
+            content = {"message": "Blob not found."}
+            return Response(content, status=status.HTTP_404_NOT_FOUND)
+        except Exception as api_exception:
+            content = {"message": str(api_exception)}
+            return Response(
+                content, status=status.HTTP_500_INTERNAL_SERVER_ERROR
+            )
```

### Comparing `core_main_app-2.3.0/core_main_app/rest/data/abstract_views.py` & `core_main_app-2.4.0/core_main_app/rest/data/abstract_views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/rest/data/admin_serializers.py` & `core_main_app-2.4.0/core_main_app/rest/data/admin_serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/rest/data/serializers.py` & `core_main_app-2.4.0/core_main_app/rest/data/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/rest/data/views.py` & `core_main_app-2.4.0/core_main_app/rest/data/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,33 +5,30 @@
 import os
 
 from django.conf import settings
 from django.http import Http404
 from rest_framework import status
 from rest_framework.decorators import api_view
 from rest_framework.exceptions import ValidationError
-from rest_framework.permissions import IsAdminUser
 from rest_framework.permissions import (
     IsAuthenticated,
     IsAuthenticatedOrReadOnly,
+    IsAdminUser,
 )
 from rest_framework.response import Response
 from rest_framework.views import APIView
 
 from core_main_app.access_control.api import check_can_write
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.commons import exceptions
 from core_main_app.commons.exceptions import XMLError
 from core_main_app.components.data import api as data_api
 from core_main_app.components.data.api import check_xml_file_is_valid
 from core_main_app.components.data.models import Data
-from core_main_app.components.data.tasks import (
-    get_task_progress,
-    get_task_result,
-)
+from core_main_app.components.data import tasks as data_tasks
 from core_main_app.components.user import api as user_api
 from core_main_app.components.workspace import api as workspace_api
 from core_main_app.rest.data.abstract_views import (
     AbstractExecuteLocalQueryView,
 )
 from core_main_app.rest.data.abstract_views import AbstractMigrationView
 from core_main_app.rest.data.admin_serializers import AdminDataSerializer
@@ -1060,48 +1057,56 @@
               content: Access denied
             - code: 500
               content: Internal server error
         """
         return super().post(request=request, template_id=pk, migrate=True)
 
 
-@api_view(["GET"])
-def get_progress(request, task_id):
-    """Get the progress of the migration / validation async task
+class GetTaskProgress(APIView):
+    """Get the progress of the migration / validation async task"""
 
-    Args:
-        request:
-        task_id:
+    permission_classes = (IsAdminUser,)
 
-    Return:
-        {
-            'state': PENDING | PROGRESS | SUCCESS,
-            'details': result (for SUCCESS) | null (for PENDING) | { PROGRESS info }
-        }
-    """
-    result = get_task_progress(task_id)
-    return Response(result, content_type="application/json")
+    def get(self, request, task_id):
+        """Get the progress of the migration / validation async task
 
+        Args:
+            request:
+            task_id:
 
-@api_view(["GET"])
-def get_result(request, task_id):
-    """Get the result of the migration / validation async task
+        Return:
+            {
+                'state': PENDING | PROGRESS | SUCCESS,
+                'details': result (for SUCCESS) | null (for PENDING) | { PROGRESS info }
+            }
+        """
+        result = data_tasks.get_task_progress(task_id)
+        return Response(result, content_type="application/json")
 
-    Args:
-        request:
-        task_id:
 
-    Return:
-        {
-                "valid": ["data_id_1", "data_id_2" ...],
-                "wrong": ["data_id_3", "data_id_4" ...]
-        }
-    """
-    result = get_task_result(task_id)
-    return Response(result, content_type="application/json")
+class GetTaskResult(APIView):
+    """Get the result of the migration / validation async task"""
+
+    permission_classes = (IsAdminUser,)
+
+    def get(self, request, task_id):
+        """Get the result of the migration / validation async task
+
+        Args:
+            request:
+            task_id:
+
+        Return:
+            {
+                    "valid": ["data_id_1", "data_id_2" ...],
+                    "wrong": ["data_id_3", "data_id_4" ...]
+            }
+        """
+        result = data_tasks.get_task_result(task_id)
+        return Response(result, content_type="application/json")
 
 
 class BulkUploadFolder(APIView):
     """Bulk upload data from folder"""
 
     permission_classes = (IsAdminUser,)
```

### Comparing `core_main_app-2.3.0/core_main_app/rest/mongo_data/serializers.py` & `core_main_app-2.4.0/core_main_app/rest/mongo_data/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/rest/template/serializers.py` & `core_main_app-2.4.0/core_main_app/rest/template/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/rest/template/views.py` & `core_main_app-2.4.0/core_main_app/rest/template/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/rest/template_version_manager/abstract_views.py` & `core_main_app-2.4.0/core_main_app/rest/template_version_manager/abstract_views.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 
 from django.http import Http404
 from django.utils.decorators import method_decorator
 from rest_framework import status
 from rest_framework.exceptions import ValidationError
 from rest_framework.response import Response
 from rest_framework.views import APIView
+from rest_framework.permissions import IsAuthenticated
 
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.commons import exceptions as exceptions
 from core_main_app.commons.exceptions import NotUniqueError, ApiError, XSDError
 from core_main_app.components.template import api as template_api
 from core_main_app.components.template_version_manager import (
     api as template_version_manager_api,
 )
 from core_main_app.rest.template_version_manager.serializers import (
     TemplateVersionManagerSerializer,
     CreateTemplateSerializer,
+    TemplateVersionManagerOrderingSerializer,
 )
 from core_main_app.utils.boolean import to_bool
 from core_main_app.utils.decorators import api_staff_member_required
 
 
 class AbstractTemplateVersionManagerList(APIView, metaclass=ABCMeta):
     """List template version managers"""
@@ -314,7 +316,121 @@
                 content, status=status.HTTP_500_INTERNAL_SERVER_ERROR
             )
 
     @abstractmethod
     def get_user(self):
         """Retrieve a user"""
         raise NotImplementedError("get_user method is not implemented.")
+
+
+class AbstractOrderingTemplateVersionManager(APIView, metaclass=ABCMeta):
+    """Set template version manager rank"""
+
+    serializer = TemplateVersionManagerOrderingSerializer
+    permission_classes = (IsAuthenticated,)
+
+    @abstractmethod
+    def get_objects(self):
+        """get template version manager list."""
+        raise NotImplementedError("get_objects method is not implemented.")
+
+    @abstractmethod
+    def update_ordering(self, list_ids):
+        """update TemplateVersionManager ordering
+
+        Args:
+            list_ids:
+        Returns:
+
+        """
+        raise NotImplementedError("update_ordering method is not implemented.")
+
+    def get(self, request):
+        """Get template version managers
+
+        Args:
+
+            request: HTTP request
+
+        Returns:
+
+            - code: 200
+              content: List of template version manager
+            - code: 403
+              content: Access control error
+            - code: 404
+              content: template(s) Not found
+            - code: 500
+              content: Internal server error
+        """
+        try:
+            object_list = self.get_objects()
+
+            # Serialize object
+            serializer = self.serializer(object_list, many=True)
+            return Response(serializer.data, status=status.HTTP_200_OK)
+        except Exception as api_exception:
+            content = {"message": str(api_exception)}
+            return Response(
+                content, status=status.HTTP_500_INTERNAL_SERVER_ERROR
+            )
+
+    def patch(self, request):
+        """Update templates ordering
+
+
+        Parameters:
+
+            {
+                "template_list" : [template_version_manager1_id, template_version_manager2_id]
+            }
+
+        Example:
+
+            "template_list": [2, 19, 3, 1]
+
+        Args:
+
+            request: HTTP request
+
+        Returns:
+
+            - code: 200
+              content: None
+            - code: 403
+              content: Authentication error
+            - code: 404
+              content: Object was not found
+            - code: 500
+              content: Internal server error
+        """
+        try:
+            # get list ids
+            template_ids = request.data.get("template_list", [])
+
+            # check duplicate ids
+            if len(template_ids) != len(set(template_ids)):
+                content = {
+                    "message": "Action not processed due to duplicate ids."
+                }
+                return Response(content, status=status.HTTP_400_BAD_REQUEST)
+
+            # update template ordering
+            self.update_ordering(template_ids)
+
+            # Serialize objects
+            serializer = self.serializer(self.get_objects(), many=True)
+
+            # return response
+            return Response(serializer.data, status=status.HTTP_200_OK)
+
+        except AccessControlError as ace:
+            content = {"message": str(ace)}
+            return Response(content, status=status.HTTP_403_FORBIDDEN)
+        except exceptions.DoesNotExist as dne:
+            content = {"message": str(dne)}
+            return Response(content, status=status.HTTP_404_NOT_FOUND)
+        except Exception as api_exception:
+            content = {"message": str(api_exception)}
+            return Response(
+                content, status=status.HTTP_500_INTERNAL_SERVER_ERROR
+            )
```

### Comparing `core_main_app-2.3.0/core_main_app/rest/template_version_manager/serializers.py` & `core_main_app-2.4.0/core_main_app/rest/template_version_manager/serializers.py`

 * *Files 7% similar despite different names*

```diff
@@ -86,7 +86,19 @@
 
         return template_object
 
     def update(self, instance, validated_data):
         raise NotImplementedError(
             "Template Version Manager should only be updated using specialized APIs."
         )
+
+
+class TemplateVersionManagerOrderingSerializer(ModelSerializer):
+    """
+    Template Version Manager Ordering serializer
+    """
+
+    class Meta:
+        """Meta"""
+
+        model = TemplateVersionManager
+        fields = ["title", "display_rank", "id"]
```

### Comparing `core_main_app-2.3.0/core_main_app/rest/template_version_manager/utils.py` & `core_main_app-2.4.0/core_main_app/rest/template_version_manager/utils.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/rest/template_version_manager/views.py` & `core_main_app-2.4.0/core_main_app/rest/template_version_manager/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 from core_main_app.components.version_manager import api as version_manager_api
 from core_main_app.rest.template_version_manager.abstract_views import (
     AbstractTemplateVersionManagerList,
     AbstractTemplateList,
     AbstractStatusTemplateVersion,
     AbstractStatusTemplateVersionManager,
     AbstractTemplateVersionManagerDetail,
+    AbstractOrderingTemplateVersionManager,
 )
 from core_main_app.rest.template_version_manager.serializers import (
     TemplateVersionManagerSerializer,
     CreateTemplateSerializer,
 )
 from core_main_app.utils.decorators import api_staff_member_required
-from core_main_app.access_control.exceptions import AccessControlError
 
 
 class GlobalTemplateVersionManagerList(AbstractTemplateVersionManagerList):
     """List all GlobalTemplateVersionManager"""
 
     def get_template_version_managers(self):
         """Get GlobalTemplateVersionManager
@@ -395,53 +395,66 @@
         """
         # FIXME: add return?
         version_manager_api.restore(
             template_version_manager_object, request=self.request
         )
 
 
-class TemplateVersionManagerOrdering(APIView):
-    """Update templates ordering"""
-
-    permission_classes = (IsAuthenticated,)
+class GlobalTemplateVersionManagerOrdering(
+    AbstractOrderingTemplateVersionManager
+):
+    permission_classes = (IsAdminUser,)
+    """Get Global TemplateVersionManager ordering"""
 
-    def patch(self, request):
-        """Update templates ordering
+    def get_objects(self):
+        """Get TemplateVersionManager list from db
 
         Args:
-            request:
 
         Returns:
+            TemplateVersionManager list
+        """
+        return template_version_manager_api.get_global_version_managers(
+            request=self.request
+        )
+
+    def update_ordering(self, list_ids):
+        """update global TemplateVersionManager ordering
+
+        Args:
+            list_ids:
+        Returns:
 
-            - code: 200
-              content: None
-            - code: 403
-              content: Authentication error
-            - code: 404
-              content: Object was not found
-            - code: 500
-              content: Internal server error
         """
-        try:
-            # get list ids
-            template_ids = request.data.get("template_list", [])
+        template_version_manager_api.update_global_template_ordering(
+            list_ids, request=self.request
+        )
 
-            # get template list
-            template_list = template_version_manager_api.sort_by_id_list(
-                template_ids, request
-            )
 
-            # update template ordering
-            template_version_manager_api.update_templates_ordering(
-                template_list, user=self.request.user
-            )
+class UserTemplateVersionManagerOrdering(
+    AbstractOrderingTemplateVersionManager
+):
+    """Get User TemplateVersionManager ordering"""
 
-            # return response
-            return Response({}, status=status.HTTP_200_OK)
-        except AccessControlError as ace:
-            content = {"message": str(ace)}
-            return Response(content, status=status.HTTP_403_FORBIDDEN)
-        except Exception as api_exception:
-            content = {"message": str(api_exception)}
-            return Response(
-                content, status=status.HTTP_500_INTERNAL_SERVER_ERROR
-            )
+    def get_objects(self):
+        """Get TemplateVersionManager list from db
+
+        Args:
+
+        Returns:
+            TemplateVersionManager list
+        """
+        return template_version_manager_api.get_all_by_user_id(
+            request=self.request
+        )
+
+    def update_ordering(self, list_ids):
+        """update user TemplateVersionManager ordering
+
+        Args:
+            list_ids:
+        Returns:
+
+        """
+        template_version_manager_api.update_user_template_ordering(
+            list_ids, request=self.request
+        )
```

### Comparing `core_main_app-2.3.0/core_main_app/rest/template_xsl_rendering/serializers.py` & `core_main_app-2.4.0/core_main_app/rest/template_xsl_rendering/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/rest/template_xsl_rendering/views.py` & `core_main_app-2.4.0/core_main_app/rest/template_xsl_rendering/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/rest/urls.py` & `core_main_app-2.4.0/core_main_app/rest/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,22 @@
     ),
     re_path(
         r"^template-version-manager/user/$",
         template_version_manager_views.UserTemplateVersionManagerList.as_view(),
         name="core_main_app_rest_template_version_manager_user_list",
     ),
     re_path(
-        r"^template-version-manager/ordering/$",
-        template_version_manager_views.TemplateVersionManagerOrdering.as_view(),
-        name="core_main_app_rest_template_version_manager_ordering",
+        r"^template-version-manager/global/ordering/$",
+        template_version_manager_views.GlobalTemplateVersionManagerOrdering.as_view(),
+        name="core_main_app_rest_global_template_version_manager_ordering",
+    ),
+    re_path(
+        r"^template-version-manager/user/ordering/$",
+        template_version_manager_views.UserTemplateVersionManagerOrdering.as_view(),
+        name="core_main_app_rest_user_template_version_manager_ordering",
     ),
     re_path(
         r"^template-version-manager/(?P<pk>\w+)/$",
         template_version_manager_views.TemplateVersionManagerDetail.as_view(),
         name="core_main_app_rest_template_version_manager_detail",
     ),
     re_path(
@@ -164,20 +169,20 @@
     re_path(
         r"^data/template/(?P<pk>\w+)/migrate/$",
         data_views.Migration.as_view(),
         name="core_main_app_rest_data_migrate",
     ),
     re_path(
         r"^data/migration/task/(?P<task_id>[\w-]+)/progress/$",
-        data_views.get_progress,
+        data_views.GetTaskProgress.as_view(),
         name="core_main_app_rest_data_migration_task_progress",
     ),
     re_path(
         r"^data/migration/task/(?P<task_id>[\w-]+)/result/$",
-        data_views.get_result,
+        data_views.GetTaskResult.as_view(),
         name="core_main_app_rest_data_migration_task_result",
     ),
     re_path(
         r"^admin/blob/$",
         blob_views.BlobListAdmin.as_view(),
         name="core_main_app_rest_blob_list_admin",
     ),
@@ -188,14 +193,19 @@
     ),
     re_path(
         r"^blobs/delete/$",
         blob_views.BlobDeleteList.as_view(),
         name="core_main_app_rest_blob_delete_list",
     ),
     re_path(
+        r"^blob/(?P<pk>\w+)/metadata/(?P<metadata_id>\w+)/$",
+        blob_views.BlobMetadata.as_view(),
+        name="core_main_app_rest_blob_add_metadata",
+    ),
+    re_path(
         r"^blob/(?P<pk>\w+)/$",
         blob_views.BlobDetail.as_view(),
         name="core_main_app_rest_blob_detail",
     ),
     re_path(
         r"^blob/download/(?P<pk>\w+)/$",
         blob_views.BlobDownload.as_view(),
```

### Comparing `core_main_app-2.3.0/core_main_app/rest/user/serializers.py` & `core_main_app-2.4.0/core_main_app/rest/user/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/rest/user/views.py` & `core_main_app-2.4.0/core_main_app/rest/user/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/rest/views.py` & `core_main_app-2.4.0/core_main_app/rest/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """ Rest views
 """
+import importlib_metadata
 from django.conf import settings
 from django.db import connection
-from importlib_metadata import version, PackageNotFoundError
 from rest_framework import status
 from rest_framework.permissions import IsAuthenticated
 from rest_framework.response import Response
 from rest_framework.views import APIView
-from core_main_app.utils.databases.mongo import MONGO_CLIENT
+
 from core_main_app.utils.databases.backend import (
     uses_postgresql_backend,
     uses_sqlite3_backend,
 )
+from core_main_app.utils.databases.mongo import MONGO_CLIENT
 
 
 class CoreSettings(APIView):
     """Get Core Settings"""
 
     permission_classes = (IsAuthenticated,)
 
@@ -32,16 +33,16 @@
               content: Settings
             - code: 500
               content: Internal server error
         """
         try:
             # Get version of core main application
             try:
-                core_version = version("core_main_app")
-            except PackageNotFoundError:
+                core_version = importlib_metadata.version("core_main_app")
+            except importlib_metadata.PackageNotFoundError:
                 core_version = None
 
             # Get version of MongoDB server
             mongodb_version = (
                 (MONGO_CLIENT.database.client.server_info()["version"])
                 if MONGO_CLIENT
                 else None
```

### Comparing `core_main_app-2.3.0/core_main_app/rest/web_page/serializers.py` & `core_main_app-2.4.0/core_main_app/rest/web_page/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/rest/web_page/views.py` & `core_main_app-2.4.0/core_main_app/rest/web_page/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/rest/workspace/serializers.py` & `core_main_app-2.4.0/core_main_app/rest/workspace/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/rest/workspace/views.py` & `core_main_app-2.4.0/core_main_app/rest/workspace/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/rest/xsl_transformation/serializers.py` & `core_main_app-2.4.0/core_main_app/rest/xsl_transformation/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/rest/xsl_transformation/views.py` & `core_main_app-2.4.0/core_main_app/rest/xsl_transformation/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/settings.py` & `core_main_app-2.4.0/core_main_app/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,19 @@
 if not settings.configured:
     settings.configure()
 
 CUSTOM_NAME = getattr(settings, "CUSTOM_NAME", "Local")
 """ :py:class:`str`: Name of the local instance
 """
 
-BOOTSTRAP_VERSION = getattr(settings, "BOOTSTRAP_VERSION", "4.6.2")
+PROJECT_VERSION = getattr(settings, "PROJECT_VERSION", "0.0.0")
+""" :py:class:`str`: Project version number.
+"""
+
+BOOTSTRAP_VERSION = getattr(settings, "BOOTSTRAP_VERSION", "5.1.3")
 """ :py:class:`str`: Version of the boostrap library.
 """
 
 SERVER_URI = getattr(settings, "SERVER_URI", "http://127.0.0.1:8000")
 """ :py:class:`str`: Server URI for import reference.
 """
 
@@ -242,15 +246,17 @@
     CHECKSUM_ALGORITHM = "SHA512"
 """
 
 GA_TRACKING_ID = getattr(settings, "GA_TRACKING_ID", None)
 """ :py:class:`str`: Google Analytics tracking ID. Adds gtag to user pages if set.
 """
 
-MAX_DOCUMENT_EDITING_SIZE = 128 * 1024
+MAX_DOCUMENT_EDITING_SIZE = getattr(
+    settings, "MAX_DOCUMENT_EDITING_SIZE", 128 * 1024
+)
 """ :py:class:`int`: Maximum byte size allowed for document editing.
 """
 
 DJANGO_SIMPLE_HISTORY_MODELS = getattr(
     settings, "DJANGO_SIMPLE_HISTORY_MODELS", None
 )
 """ :py:class:`list`: Track history of listed models.
```

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/css/skins.css` & `core_main_app-2.4.0/core_main_app/static/core_main_app/admin/_theme/css/skins.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/css/theme.css` & `core_main_app-2.4.0/core_main_app/static/core_main_app/admin/_theme/css/theme.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/js/app.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/admin/_theme/js/app.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/js/menu.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/admin/_theme/js/menu.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/admin/css/data_migration.css` & `core_main_app-2.4.0/core_main_app/static/core_main_app/admin/css/data_migration.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/admin/css/templates_xslt/form.css` & `core_main_app-2.4.0/core_main_app/static/core_main_app/admin/css/templates_xslt/form.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/display_permissions.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/admin/js/display_permissions.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates/data_migration.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/admin/js/templates/data_migration.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates/data_migration.raw.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/admin/js/templates/data_migration.raw.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates/upload/dependencies.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/admin/js/templates/upload/dependencies.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates_xslt/detail_xslt.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/admin/js/templates_xslt/detail_xslt.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/XMLTree.css` & `core_main_app-2.4.0/core_main_app/static/core_main_app/common/css/XMLTree.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/switch.css` & `core_main_app-2.4.0/core_main_app/static/core_main_app/common/css/switch.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/csrf.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/csrf.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/debounce.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/debounce.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/elementViewport.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/elementViewport.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,13 @@
 /**
  * JS function to test if an DOM element is visible on the windows
  * @see https://stackoverflow.com/questions/123999/how-to-tell-if-a-dom-element-is-visible-in-the-current-viewport/7557433#7557433
  * @todo it's a reusable function should we put it in utils js file?
  */
 function isElementInViewport(el) {
-
     //special bonus for those using jQuery
     if (typeof jQuery === "function" && el instanceof jQuery) {
         el = el[0];
     }
 
     var rect = el.getBoundingClientRect();
```

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/loading_spinner.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/loading_spinner.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,29 @@
 /**
  * Show spinner for button
  */
 var showSpinner = function($btnID) {
     // Show loading spinner
     $btnID.attr('class', 'fas fa-spinner fa-pulse');
+    var dropdown = $("#dropdownActions");
+    if (dropdown) {
+        $(dropdown).find("i").attr("class", "fas fa-spinner fa-pulse");
+    }
 }
 
 /**
  *  Hide spinner for button
  */
 var hideSpinner = function($btnID, icon) {
     // show old btn icon
     $btnID.attr('class', icon)
+    var dropdown = $("#dropdownActions");
+    if (dropdown) {
+        $(dropdown).find("i").attr('class', "fas fa-sliders")
+    }
 }
 
 
 /**
  * Show spinner for container
  */
 var displaySpinner = function(container) {
```

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/modals/add.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/modals/add.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/modals/delete.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/modals/delete.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/modals/edit.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/modals/edit.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/list/modals/disable.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/templates/list/modals/disable.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/list/restore.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/templates/list/restore.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/versions/modals/disable.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/templates/versions/modals/disable.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/versions/restore.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/templates/versions/restore.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/versions/set_current.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/templates/versions/set_current.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -14,15 +14,15 @@
     $.ajax({
         url: setCurrentVersionPostUrl.replace('template_version_id', objectID),
         type: "PATCH",
         success: function(data) {
             location.reload();
         },
         error: function(data) {
-            $.notify(data.responseJSON["message"]);
+            $.notify(data.responseJSON["message"], "danger");
         }
     });
 };
 
 $(document).ready(function() {
     $('.current').on('click', setCurrentVersion);
 });
```

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/delete.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/delete.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/edit.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/edit.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/common/xsl/xml2html.xsl` & `core_main_app-2.4.0/core_main_app/static/core_main_app/common/xsl/xml2html.xsl`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery/3.5.1/jquery.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery/3.5.1/jquery.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_444444_256x240.png` & `core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_555555_256x240.png` & `core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777620_256x240.png` & `core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777777_256x240.png` & `core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_cc0000_256x240.png` & `core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_ffffff_256x240.png` & `core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.css` & `core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.structure.css` & `core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.structure.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.theme.css` & `core_main_app-2.4.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/data/change_display.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/data/change_display.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/login/message.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/login/message.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/sharing_modal.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/sharing_modal.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,19 @@
 copyLink = function(link) {
     /**
      * Copy the link on clipboard and close the modal
      */
     link.prop('disabled', false);
     link.focus();
     link.select();
-    document.execCommand('copy');
+    navigator.clipboard.writeText(link.val()).then(function() {
+        $.notify("URL copied to clipboard successfully!", "success");
+    }, function() {
+        $.notify("A problem has occurred while copying the Url.", "danger");
+    });
     link.prop('disabled', true);
 };
 
 initSharingModal = function(sharingConfigurationFunction, sharingButtonId, sharingModalId,
     sharingInputId, sharingSubmitId) {
     $(document).on('click', sharingButtonId, function(event) {
         event.preventDefault();
```

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/text_editor/text_editor.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/text_editor/text_editor.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -90,17 +90,15 @@
         type: "POST",
         data: {
             'content': $(".input").text(),
             'action': 'format',
         },
         dataType: "json",
         success: function(data) {
-            $.notify("Document formatted successfully", {
-                style: "success"
-            });
+            $.notify("Document formatted successfully", "success");
             html = hljs.highlightAuto(data).value
             $(".input").html("<pre class=\"content-highlight m-1\">" + html + "</pre>")
         },
         error: function(data) {
             jqError.html('<i class="fas fa-exclamation-triangle"></i> ' + data.responseText);
             jqError.show();
 
@@ -126,17 +124,15 @@
         data: {
             'content': $(".input").text(),
             'action': 'validate',
             'template_id': templateID,
         },
         dataType: "json",
         success: function(data) {
-            $.notify("Content validated with success", {
-                style: "success"
-            });
+            $.notify("Content validated with success", "success");
         },
         error: function(data) {
             jqError.html('<i class="fas fa-exclamation-triangle"></i> ' + data.responseText);
             jqError.show();
         }
     }).always(function(data) {
         // get old button icon
@@ -159,17 +155,15 @@
             "content": $(".input").text(),
             "template_id": templateID,
             "xslt_id": $("#xslt-selector").val()
         },
         dataType: "json",
         type: "post",
         success: function(data) {
-            $.notify("Content refreshed with success", {
-                style: "success"
-            });
+            $.notify("Content refreshed with success", "success");
             $(".tree").html(data.template)
 
         },
         error: function(data) {
             jqError.html('<i class="fas fa-exclamation-triangle"></i> ' + data.responseText);
             jqError.show();
         }
@@ -218,17 +212,15 @@
         data: {
             'content': $(".input").text(),
             'template_id': templateID,
             'action': 'generate',
         },
         dataType: "json",
         success: function(data) {
-            $.notify("Document generated successfully", {
-                style: "success"
-            });
+            $.notify("Document generated successfully", "success");
             html = hljs.highlightAuto(data).value
             $(".input").html("<pre class=\"content-highlight m-1\">" + html + "</pre>")
         },
         error: function(data) {
             jqError.html('<i class="fas fa-exclamation-triangle"></i> ' + data.responseText);
             jqError.show();
```

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/add_group.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/add_group.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/add_user.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/add_user.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/create_workspace.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/create_workspace.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/init.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/init.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_workspace.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_workspace.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,16 @@
 /**
  * AJAX call
  */
 load_form_change_workspace = function() {
     $("#assign-workspace-modal").modal("show");
     var $recordRow = $(this).parent().parent();
+
+    // Get parent if btn in dropdown  (object id undefined)
+    if (!$recordRow.attr("objectid")) $recordRow = $recordRow.parent()
     $('.' + functional_object + '-id').val($recordRow.attr("objectid"));
 
     $.ajax({
         url: changeWorkspaceUrl,
         type: "POST",
         dataType: "json",
         data: {
```

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/remove_rights.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/remove_rights.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_private.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_private.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_public.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_public.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/switch_right.js` & `core_main_app-2.4.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/switch_right.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/system/api.py` & `core_main_app-2.4.0/core_main_app/system/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/app_wrapper.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/admin/app_wrapper.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/base.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/admin/theme/base.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 {% load static %}
-{% load tz_detect %}
 
 <!DOCTYPE html>
 <html>
 <head>
   <meta charset="utf-8">
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <meta content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no" name="viewport">
@@ -13,29 +12,34 @@
   <link rel=icon href="{% static 'img/favicon.png' %}" sizes="16x16" type="image/png">
   {% if BOOTSTRAP_VERSION == '4.6.2' %}
   <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.6.2/dist/css/bootstrap.min.css"
         integrity="sha384-xOolHFLEh07PJGoPkLv1IbcEPTNtaed2xpHsD9ESMhqIYd0nLMwNLD69Npy4HI+N" crossorigin="anonymous">
   {% elif BOOTSTRAP_VERSION == '5.1.3' %}
   <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet"
         integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">
+  <link rel="stylesheet" href="{% static 'core_main_app/common/css/bootstrap5.css' %}" />
   {% endif %}
   <link href="{% static 'fontawesomefree/css/fontawesome.css' %}" rel="stylesheet" type="text/css">
   <link href="{% static 'fontawesomefree/css/brands.css' %}" rel="stylesheet" type="text/css">
   <link href="{% static 'fontawesomefree/css/solid.css' %}" rel="stylesheet" type="text/css">
+  <link href="{% static 'fontawesomefree/css/regular.css' %}" rel="stylesheet" type="text/css">
   <link rel="stylesheet" href="{% static 'core_main_app/libs/jquery-ui/1.12.1/jquery-ui.css' %}" />
   <link rel="stylesheet" href="{% static 'core_main_app/libs/jquery-ui/1.12.1/jquery-ui.structure.css' %}" />
   <link rel="stylesheet" href="{% static 'core_main_app/libs/jquery-ui/1.12.1/jquery-ui.theme.css' %}" />
-  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.7.0/styles/atom-one-light.min.css">
+  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.7.0/styles/atom-one-light.min.css"
+        integrity="sha512-o5v54Kh5PH0dgnf9ei0L+vMRsbm5fvIvnR/XkrZZjN4mqdaeH7PW66tumBoQVIaKNVrLCZiBEfHzRY4JJSMK/Q=="
+        crossorigin="anonymous">
 
   <link rel="stylesheet" href="{% static 'core_main_app/admin/_theme/css/theme.css' %}">
   <link rel="stylesheet" href="{% static 'core_main_app/admin/_theme/css/additional.css' %}">
   <link rel="stylesheet" href="{% static 'core_main_app/admin/_theme/css/skins.css' %}">
 
   <link rel="stylesheet" href="{% static 'core_main_app/common/css/word-wrap.css' %}">
   <link rel="stylesheet" href="{% static 'core_main_app/common/css/loading-spinner.css' %}" />
+  <link rel="stylesheet" href="{% static 'core_main_app/common/css/messages.css' %}" />
   {% block app_css %}{% endblock %}
 
   <!-- HTML5 Shim and Respond.js IE8 support of HTML5 elements and media queries -->
   <!-- WARNING: Respond.js doesn't work if you view the page via file:// -->
   <!--[if lt IE 9]>
   <script src="https://oss.maxcdn.com/html5shiv/3.7.3/html5shiv.min.js"></script>
   <script src="https://oss.maxcdn.com/respond/1.4.2/respond.min.js"></script>
@@ -76,15 +80,18 @@
         integrity="sha384-Fy6S3B9q64WdZWQUiU+q4/2Lc9npb8tCaSX9FK7E8HnRr0Jz8D6OP9dO5Vg3Q9ct"
         crossorigin="anonymous"></script>
 {% elif BOOTSTRAP_VERSION == '5.1.3' %}
 <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"
         integrity="sha384-ka7Sk0Gln4gmtz2MlQnikT1wXgYsOg+OMhuP+IlRH9sENBO0LRn5q+8nbTov4+1p"
         crossorigin="anonymous"></script>
 {% endif %}
-<script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.7.0/highlight.min.js"></script>
+<script
+  src="//cdnjs.cloudflare.com/ajax/libs/highlight.js/11.8.0/highlight.min.js"
+  integrity="sha384-g4mRvs7AO0/Ol5LxcGyz4Doe21pVhGNnC3EQw5shw+z+aXDN86HqUdwXWO+Gz2zI"
+  crossorigin="anonymous"></script>
 <script>hljs.highlightAll();</script>
 <script src="{% static 'core_main_app/common/js/csrf.js' %}"></script>
 
 {% include 'core_main_app/_render/common/messages.html' %}
 
 <script src="{% static 'core_main_app/common/js/loading_spinner.js' %}"></script>
 <script src="{% static 'core_main_app/admin/_theme/js/app.js' %}"></script>
@@ -97,10 +104,9 @@
      user experience. Slimscroll is required when using the
      fixed layout. -->
 
   <!--
   From the documentation:
       Add the detection template tag to your site, ideally in your base layout just before the </body> tag
   -->
-  {% tz_detect %}
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,29 +1,32 @@
-{% load static %} {% load tz_detect %}
+{% load static %}
 
 
  {% if BOOTSTRAP_VERSION == '4.6.2' %}
  {% elif BOOTSTRAP_VERSION == '5.1.3' %}
+
  {% endif %}
 
 
 
 
 
 
 
 
 
 
 
+
+
  {% block app_css %}{% endblock %}
  {% include 'core_main_app/_render/admin/theme/header.html' %}   {% include
 'core_main_app/_render/admin/theme/menu.html' %}
 {% block app_data %}{% endblock %}
  {% include 'core_main_app/_render/admin/theme/footer.html' %}  {% block
 app_modals %}{% endblock %}
 
  {% if BOOTSTRAP_VERSION == '4.6.2' %}
  {% elif BOOTSTRAP_VERSION == '5.1.3' %}
  {% endif %}
  {% include 'core_main_app/_render/common/messages.html' %}
- {% block app_js %}{% endblock %}   {% tz_detect %}
+ {% block app_js %}{% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/box.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/box.html`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     <div class="box box-primary">
 {% else %}
     <div class="box box-default">
 {% endif %}
     <div class="box-header with-border">
         <h3 class="box-title">{% block box_title %}{% endblock %}</h3>
 
-        <div class="box-tools mr-3 float-right">
+        <div class="box-tools {% if BOOTSTRAP_VERSION == "4.6.2" %}mr-3 float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}me-3 float-end{% endif %}">
             {% block box_tools %}{% endblock %}
         </div>
     </div>
     <div class="m-3 box-body">
         {% block box_body %}{% endblock %}
     </div>
     <div class="box-footer">
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/user/app_wrapper.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/user/app_wrapper.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/user/default.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/user/default.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/user/theme_base.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/_render/user/theme_base.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 {% load static %}
-{% load tz_detect %}
 
 {% comment %}
     Root file to be used in any theme. Contains all necessary (and up-to-date) libraries.
 {% endcomment %}
 <!DOCTYPE html>
 <html lang="en">
 <head>
@@ -28,27 +27,32 @@
         <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.6.2/dist/css/bootstrap.min.css"
               integrity="sha384-xOolHFLEh07PJGoPkLv1IbcEPTNtaed2xpHsD9ESMhqIYd0nLMwNLD69Npy4HI+N"
               crossorigin="anonymous">
         {% elif BOOTSTRAP_VERSION == '5.1.3' %}
         <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet"
               integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3"
               crossorigin="anonymous">
+        <link rel="stylesheet" href="{% static 'core_main_app/common/css/bootstrap5.css' %}" />
         {% endif %}
         <link href="{% static 'fontawesomefree/css/fontawesome.css' %}" rel="stylesheet" type="text/css">
         <link href="{% static 'fontawesomefree/css/brands.css' %}" rel="stylesheet" type="text/css">
         <link href="{% static 'fontawesomefree/css/solid.css' %}" rel="stylesheet" type="text/css">
+        <link href="{% static 'fontawesomefree/css/regular.css' %}" rel="stylesheet" type="text/css">
         <link rel="stylesheet" href="{% static 'core_main_app/libs/jquery-ui/1.12.1/jquery-ui.css' %}" />
         <link rel="stylesheet" href="{% static 'core_main_app/libs/jquery-ui/1.12.1/jquery-ui.structure.css' %}" />
         <link rel="stylesheet" href="{% static 'core_main_app/libs/jquery-ui/1.12.1/jquery-ui.theme.css' %}" />
-        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.7.0/styles/atom-one-light.min.css">
+        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.7.0/styles/atom-one-light.min.css"
+              integrity="sha512-o5v54Kh5PH0dgnf9ei0L+vMRsbm5fvIvnR/XkrZZjN4mqdaeH7PW66tumBoQVIaKNVrLCZiBEfHzRY4JJSMK/Q=="
+              crossorigin="anonymous">
         <link rel="stylesheet" href="{% static 'core_main_app/common/css/word-wrap.css' %}" />
         <link rel="stylesheet" href="{% static 'core_main_app/common/css/table.css' %}" />
         <link rel="stylesheet" href="{% static 'core_main_app/common/css/buttons.css' %}" />
         <link rel="stylesheet" href="{% static 'core_main_app/common/css/fields.css' %}" />
         <link rel="stylesheet" href="{% static 'core_main_app/common/css/loading-spinner.css' %}" />
+        <link rel="stylesheet" href="{% static 'core_main_app/common/css/messages.css' %}" />
 
         {% if DISPLAY_NIST_HEADERS %}
         <link rel="stylesheet" href="https://pages.nist.gov/nist-header-footer/css/nist-combined.css">
         {% endif %}
     {% endblock %}
     {% block theme_css %}{% endblock %}
     {% block app_css %}{% endblock %}
@@ -65,27 +69,28 @@
                 integrity="sha384-Fy6S3B9q64WdZWQUiU+q4/2Lc9npb8tCaSX9FK7E8HnRr0Jz8D6OP9dO5Vg3Q9ct"
                 crossorigin="anonymous"></script>
         {% elif BOOTSTRAP_VERSION == '5.1.3' %}
         <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"
                 integrity="sha384-ka7Sk0Gln4gmtz2MlQnikT1wXgYsOg+OMhuP+IlRH9sENBO0LRn5q+8nbTov4+1p"
                 crossorigin="anonymous"></script>
         {% endif %}
-        <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.7.0/highlight.min.js"></script>
+        <script src="//cdnjs.cloudflare.com/ajax/libs/highlight.js/11.8.0/highlight.min.js"
+                integrity="sha384-g4mRvs7AO0/Ol5LxcGyz4Doe21pVhGNnC3EQw5shw+z+aXDN86HqUdwXWO+Gz2zI"
+                crossorigin="anonymous"></script>
         <script>hljs.highlightAll();</script>
         <script src="{% static 'core_main_app/common/js/csrf.js' %}"></script>
         <script src="{% static 'core_main_app/common/js/leave_notice.js' %}"></script>
         <script src="{% static 'core_main_app/common/js/loading_spinner.js' %}"></script>
         {% if DISPLAY_NIST_HEADERS %}
         <script src="https://pages.nist.gov/nist-header-footer/js/nist-header-footer.js" type="text/javascript" defer="defer"></script>
         {% endif %}
-        {% include 'core_main_app/_render/common/messages.html' %}
     {% endblock %}
     {% block theme_js %}{% endblock %}
     {% block app_js %}{% endblock %}
+    {% include 'core_main_app/_render/common/messages.html' %}
 
     <!--
     From the documentation:
         Add the detection template tag to your site, ideally in your base layout just before the </body> tag
     -->
-    {% tz_detect %}
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,32 +1,34 @@
-{% load static %} {% load tz_detect %} {% comment %} Root file to be used in
-any theme. Contains all necessary (and up-to-date) libraries. {% endcomment %}
+{% load static %} {% comment %} Root file to be used in any theme. Contains all
+necessary (and up-to-date) libraries. {% endcomment %}
 {% if GA_TRACKING_ID %}
  {% endif %}
 
  {% block meta %}{% endblock %}
 {% block core_css %} {% if BOOTSTRAP_VERSION == '4.6.2' %}
  {% elif BOOTSTRAP_VERSION == '5.1.3' %}
+
  {% endif %}
 
 
 
 
 
 
 
 
 
 
 
+
+
  {% if DISPLAY_NIST_HEADERS %}
  {% endif %} {% endblock %} {% block theme_css %}{% endblock %} {% block
 app_css %}{% endblock %}
 {% block body %}{% endblock %} {% block app_modals %}{% endblock %} {% block
 core_js %}
  {% if BOOTSTRAP_VERSION == '4.6.2' %}
  {% elif BOOTSTRAP_VERSION == '5.1.3' %}
  {% endif %}
  {% if DISPLAY_NIST_HEADERS %}
- {% endif %} {% include 'core_main_app/_render/common/messages.html' %} {%
-endblock %} {% block theme_js %}{% endblock %} {% block app_js %}{% endblock %}
-{% tz_detect %}
+ {% endif %} {% endblock %} {% block theme_js %}{% endblock %} {% block app_js
+%}{% endblock %} {% include 'core_main_app/_render/common/messages.html' %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/commons/upload/form.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/commons/upload/form.html`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 {% block box_body %}
 <div id="upload_errors" class="alert alert-danger" style="display: {{ data.errors|yesno:',none' }};">
     <h4><i class='fas fa-warning'></i>&nbsp;&nbsp;{{ data.errors | safe}} </h4>
 </div>
 <form id="form_start" action='{{data.url}}' method="post" enctype=multipart/form-data>
     {% csrf_token %}
     {{ data.upload_form }}
-    <button type="submit" class="btn btn-primary mt-3 float-right">
+    <button type="submit" class="btn btn-primary mt-3 {% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}">
         <i class="fas fa-upload"></i> Upload
     </button>
 </form>
 
 {% block upload_addons %}{% endblock %}
 {% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/dependency_resolver.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/dependency_resolver.html`

 * *Files 13% similar despite different names*

```diff
@@ -33,10 +33,10 @@
         <td>{{ dependencies }}</td>
     </tr>
     {% endfor %}
 </table>
 <div id="xsd_content" style="display: none;">{{ xsd_content }}</div>
 <div id="filename" style="display: none;">{{ filename }}</div>
 <span class='resolve'>
-    <a class="btn btn-primary float-right" href="#"><i class="fas fa-save"></i> Save</a>
+    <a class="btn btn-primary {% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}" href="#"><i class="fas fa-save"></i> Save</a>
 </span>
 <div id='errorDependencies' style="color:red;"></div>
```

#### html2text {}

```diff
@@ -4,9 +4,10 @@
 the database to resolve each import/include.
 Import/Include Schema Location                       Dependency
 Import          {{ import.attrib.schemaLocation }}   {{ dependencies }}
 Include         {{ include.attrib.schemaLocation }}  {{ dependencies }}
 {{ xsd_content }}
 {{ filename }}
 
- Save
+.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}"
+href="#"> Save
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/data_migration/templates_list.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/data_migration/templates_list.html`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     templates (Step 1). Then, select the data to migrate, or all the data for the selected templates (Step 2). Step 3
     allows the selection of an XSLT in order to transform data from the source template into a new XML document that
     would be valid for the destination template. And finally, select the target template for the selected data (Step 4).
     Once the selection is done, use the "validate" button to check if the selected data can be migrated to the selected
     target template. Use the "migrate" button to perform the migration.
 </p>
 <div>
-    <button  type="button" class="btn btn-secondary mb-2 float-right back-to-version-manager" hidden>
+    <button  type="button" class="btn btn-secondary mb-2 {% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %} back-to-version-manager" hidden>
         <i class="fas fa-arrow-left"></i> Back to version manager
     </button>
 </div>
 <div class="w-100 d-flex">
     <div class="card list-card">
         <div class="card-header">
             <table class="table table-bordered table-striped">
@@ -67,15 +67,15 @@
     <div class="card list-card">
         <div class="card-header">
             <table class="table table-bordered table-striped">
                 <thead>
                     <tr>
                         <td width="20px"><input id="select-all-data" type="checkbox" disabled></td>
                         <td>2 - Select Data</td>
-                        <td class="data-count text-right hidden"><strong id="data-number">235</strong> data selected</td>
+                        <td class="data-count {% if BOOTSTRAP_VERSION == "4.6.2" %}text-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}text-end{% endif %} hidden"><strong id="data-number">235</strong> data selected</td>
                     </tr>
                 </thead>
             </table>
         </div>
         <div class="card-body">
             <table id="data-table" class="table table-bordered table-striped">
                 <tbody>
@@ -91,15 +91,15 @@
     <div class="card list-card">
         <div class="card-header">
             <table class="table table-bordered table-striped">
                 <thead>
                     <tr>
                         <td width="20px"></td>
                         <td>3 - Select XSLT <small>(optional)</small></td>
-                        <td class="xslt-clear text-right hidden">Clear</td>
+                        <td class="xslt-clear {% if BOOTSTRAP_VERSION == "4.6.2" %}text-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}text-end{% endif %} hidden">Clear</td>
                     </tr>
                 </thead>
             </table>
         </div>
         <div class="card-body">
             <table id="xslt-table" class="table table-bordered table-striped">
                 <tbody id="xslt-content" class="hidden">
```

#### html2text {}

```diff
@@ -8,22 +8,23 @@
 migrate, or all the data for the selected templates (Step 2). Step 3 allows the
 selection of an XSLT in order to transform data from the source template into a
 new XML document that would be valid for the destination template. And finally,
 select the target template for the selected data (Step 4). Once the selection
 is done, use the "validate" button to check if the selected data can be
 migrated to the selected target template. Use the "migrate" button to perform
 the migration.
-  Back to version manager
+.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}
+back-to-version-manager" hidden>  Back to version manager
 �1 - Select Source template(s)
   Show users templates  ⁰
 ⁰                    {{template.title}}
 No Template available.
-�2 - Select Data 235 data selected
+�2 - Select Data
 Please select source template(s)
- 3 - Select XSLT (optional) Clear
+ 3 - Select XSLT (optional)
 o                             {{xsl_transformation.name}}
 No xslt available.
 Please select data to migrate
  4 - Select a Target template
 Please select data to migrate
   Validate    Migrate
 {% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/list/available.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/common/templates/list/available.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,44 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %}
 
 {% block box_title %}Available{% endblock %}
 
 {% block box_tools %}
-    <a href="{% url 'core-admin:core_main_app_upload_template'%}" class="float-right btn btn-secondary">
+    <a href="{% url 'core-admin:core_main_app_upload_template'%}" class="{% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %} btn btn-secondary">
         <i class="fas fa-upload"></i> Upload {{ data.object_name }}
     </a>
 {% endblock %}
 
 {% block box_body %}
-<p>
-This page lists all Templates uploaded by admin users. Use drag and drop to update the order templates appear
-on the website, then click on "Save ordering" when done.
-</p>
-<table class="table table-bordered table-striped table-hover" data-reorderable-rows="true">
+<table class="table table-bordered table-striped table-hover">
     <tr>
-        <th>Display order</th>
-        <th width="35%">{{ data.object_name }}</th>
+        <th>{{ data.object_name }}</th>
         <th>Actions</th>
     </tr>
 
     {% for object in data.available %}
-        <tr object-id={{object.id}} draggable="true" ondragstart="start()"  ondragover="dragover()">
-
-            <td>{% if object.display_rank %} {{object.display_rank}} {%else %} - {%endif%} </td>
+        <tr>
             <td>{{ object.title }}</td>
             <td>
                 {% block box_actions %}
                 <a class="btn btn-secondary"
                    href="{% url 'core-admin:core_main_app_manage_template_versions' object.id %}">
                     <i class="fas fa-list"></i> Versions
                 </a>
-                {% url 'core_main_app_edit_template' object.id as edit_url %}
-                {% include 'core_main_app/common/buttons/edit.html' %}
+                <span class="icon legend edit" objectid="{{ object.id }}">
+                    <a class="btn btn-secondary" href="#"><i class="fas fa-edit"></i> Edit</a>
+                </span>
                 <span class="icon legend delete" objectid="{{ object.id }}">
                     <button class="btn btn-danger"><i class="fas fa-trash"></i> Disable </button>
                 </span>
                 {% endblock %}
             </td>
         </tr>
     {% empty %}
         <tr>
             <td class="empty" colspan="2">
                 No {{ data.object_name }} uploaded.
             </td>
         </tr>
     {% endfor %}
-
 </table>
-{% include 'core_main_app/common/buttons/save_ordering.html' %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,18 +1,13 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% block
 box_title %}Available{% endblock %} {% block box_tools %}
- Upload_{{_data.object_name_}}
+.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}
+btn btn-secondary">  Upload {{ data.object_name }}
  {% endblock %} {% block box_body %}
-This page lists all Templates uploaded by admin users. Use drag and drop to
-update the order templates appear on the website, then click on "Save ordering"
-when done.
-Display order              {{ data.object_name }} Actions
-                                                  {% block box_actions %}
-                                                   Versions
-{% if object.display_rank                          {% url
-%} {{object.display_rank}} {{ object.title }}     'core_main_app_edit_template'
-{%else %} - {%endif%}                             object.id as edit_url %} {%
-                                                  include 'core_main_app/
-                                                  common/buttons/edit.html' %}
-                                                  Disable   {% endblock %}
+{{ data.object_name }} Actions
+                       {% block box_actions %}
+                        Versions
+{{ object.title }}
+                        Edit
+                           Disable   {% endblock %}
 No {{ data.object_name }} uploaded.
-{% include 'core_main_app/common/buttons/save_ordering.html' %} {% endblock %}
+{% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/list/disabled.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/list/disabled.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/list/modals/disable.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/list/modals/disable.html`

 * *Files 12% similar despite different names*

```diff
@@ -9,12 +9,14 @@
     The {{ data.object_name }} won't be erased from this website but nobody will be able to create or edit document that have been
     created with it.
 </p>
 <p>Are you sure you want to disable this {{ data.object_name }}?</p>
 {% endblock %}
 
 {% block modal_footer %}
-<button class="btn btn-secondary pull-left" data-dismiss="modal"><i class="fas fa-times"></i> No</button>
+<button class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal">
+    <i class="fas fa-times"></i> No
+</button>
 <button id="disable-template-yes" class="btn btn-danger">
         <i class="fas fa-check"></i> Yes
 </button>
 {% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/list.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/list.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/versions/available.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/versions/available.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %}
 {% load timestamptags %}
+{% load tz %}
 
 {% block box_title %}Available versions{% endblock %}
 
 {% block box_tools %}
 
 {% if not data.version_manager.user %}
     <!-- If no user is linked to the version manager, it means that we come from the global template list -->
     {% url 'core-admin:core_main_app_templates' as template_list_url %}
     <a href="{% url 'core-admin:core_main_app_upload_template_version' data.version_manager.id %}"
-       class="float-right btn btn-secondary">
+       class="{% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}
+              {% if BOOTSTRAP_VERSION == "4.6.2" %}ml-1{% elif BOOTSTRAP_VERSION == "5.1.3"%}ms-1{% endif %}
+              btn btn-secondary">
         <i class="fas fa-upload"></i> Upload New Version
     </a>
 {% else %}
     <!-- If a user is linked to the version manager, it means that we come from the dashboard template list -->
     {% url 'core-admin:core_dashboard_templates' as template_list_url %}
 {% endif %}
 
@@ -36,15 +39,15 @@
                {% if version.object == data.version_manager.current %}
                     <td style='font-weight:bold;color:green'>Current</td>
                {% else %}
                     <td style='font-weight:bold;color:orange'>Uploaded</td>
                {% endif %}
 
                <td>
-                    {{ version.creation_date }}
+                    {{ version.creation_date|localtime }}
                </td>
                <td>
                    {% block box_actions %}
                         <a class="btn btn-secondary results-xslt"
                             href="{% url 'core-admin:core_main_app_template_xslt' version.object %}">
                             <i class="fas fa-file-code"></i> XSLT
                         </a>
```

#### html2text {}

```diff
@@ -1,25 +1,27 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% load
-timestamptags %} {% block box_title %}Available versions{% endblock %} {% block
-box_tools %} {% if not data.version_manager.user %}  {% url 'core-admin:
-core_main_app_templates' as template_list_url %}
- Upload_New_Version
+timestamptags %} {% load tz %} {% block box_title %}Available versions{%
+endblock %} {% block box_tools %} {% if not data.version_manager.user %}  {%
+url 'core-admin:core_main_app_templates' as template_list_url %}
+.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}
+{% if BOOTSTRAP_VERSION == "4.6.2" %}ml-1{% elif BOOTSTRAP_VERSION ==
+"5.1.3"%}ms-1{% endif %} btn btn-secondary">  Upload New Version
  {% else %}  {% url 'core-admin:core_dashboard_templates' as template_list_url
 %} {% endif %} {% include 'core_main_app/common/buttons/go_to.html' with
 url=template_list_url label='Back to Templates' %} {% endblock %} {% block
 box_body %}
 Version #     Status  Upload   Actions
                       date
-                                                     {% block box_actions %}
-                                                      XSLT
-                                                      {% if 'core_parser_app' in
-                                                     INSTALLED_APPS %}
-{                              {                      Modules
-{                              {                      {% endif %}
-version.index Current Uploaded version.creation_date  Download
-}}                             }}                     {% if version.object !=
-                                                     data.version_manager.current
-                                                     %}
-                                                      Set_Current
-                                                         Disable  {% endif %} {%
-                                                     endblock %}
+                                                               {% block box_actions %}
+                                                                XSLT
+                                                                {% if 'core_parser_app' in
+                                                               INSTALLED_APPS %}
+{                              {                                Modules
+{                              {                                {% endif %}
+version.index Current Uploaded version.creation_date|localtime  Download
+}}                             }}                               {% if version.object !=
+                                                               data.version_manager.current
+                                                               %}
+                                                                Set_Current
+                                                                   Disable  {% endif %} {%
+                                                               endblock %}
 {% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/versions/disabled.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/versions/disabled.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %}
 {% load timestamptags %}
+{% load tz %}
 
 {% block box_title %}Disabled versions{% endblock %}
 
 {% block box_body %}
 <div id="model_version">
 	<table class="table table-bordered table-hover">
         <tr>
@@ -13,15 +14,15 @@
             <th>Actions</th>
         </tr>
 	    {% for version in data.categorized_versions.disabled reversed %}
         <tr>
             <td>{{ version.index }}</td>
             <td style='font-weight:bold;color:red'>Disabled</td>
             <td>
-                {{ version.creation_date }}
+                {{ version.creation_date|localtime }}
             </td>
 
             <td>
                 <span class='icon legend retrieve' objectid='{{ version.object }}'>
                     <a class="btn btn-secondary" href="#"><i class="fas fa-undo"></i> Restore</a>
                 </span>
             </td>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% load
-timestamptags %} {% block box_title %}Disabled versions{% endblock %} {% block
-box_body %}
-Version #           Status   Upload date                 Actions
+timestamptags %} {% load tz %} {% block box_title %}Disabled versions{%
+endblock %} {% block box_body %}
+Version #           Status   Upload date                           Actions
 
-{{ version.index }} Disabled {{ version.creation_date }}  Restore
+{{ version.index }} Disabled {{ version.creation_date|localtime }}  Restore
 
 No disabled versions for this template
 {% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/versions/modals/disable.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/versions/modals/disable.html`

 * *Files 22% similar despite different names*

```diff
@@ -7,10 +7,12 @@
 <p>
     The version won't be erased from this website but nobody will be able to switch to this version anymore.
 </p>
 <p>Are you sure you want to disable this version?</p>
 {% endblock %}
 
 {% block modal_footer %}
-<button class="btn btn-secondary pull-left" data-dismiss="modal"><i class="fas fa-times"></i> No</button>
+<button class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal">
+    <i class="fas fa-times"></i> No
+</button>
 <button id="disable-version-yes" class="btn btn-danger"><i class="fas fa-check"></i> Yes</button>
 {% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/versions.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/templates/versions.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/upload_template.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/upload_template.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/web_page/main.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/web_page/main.html`

 * *Files 12% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 {% endif %}
 <div class="row">
     <div class="col-md-12">
         <form action="{% url webpage_url %}" method="post">
             {% csrf_token %}
             {{ data.form }}
 
-            <button type="submit" class="btn btn-primary float-right mt-3"><i class="fas fa-save"></i> Save</button>
+            <button type="submit" class="btn btn-primary {% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %} mt-3"><i class="fas fa-save"></i> Save</button>
         </form>
     </div>
 </div>
 {% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/xslt/list/table.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/admin/xslt/list/table.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %}
 
 {% block box_title %}XSLT list{% endblock %}
 
 {% block box_tools %}
-<div class="btn-group float-right">
+<div class="btn-group {% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}">
 <a href="{{ data.update_url }}" class="btn btn-secondary upload-xslt-btn">
     <i class="fas fa-upload"></i> Upload XSLT
 </a>
 </div>
 {% endblock %}
 
 {% block box_body %}
```

#### html2text {}

```diff
@@ -1,9 +1,11 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% block
 box_title %}XSLT list{% endblock %} {% block box_tools %}
+.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif
+%}">
  Upload_XSLT
 {% endblock %} {% block box_body %}
 Name           Actions
                {% url 'core-admin:core_main_app_edit_xslt' elt.id as edit_url
 {{ elt.name }} %} {% include 'core_main_app/common/buttons/edit.html' %} {% url
                'core-admin:core_main_app_delete_xslt' elt.id as delete_url %}
                {% include 'core_main_app/common/buttons/delete.html' %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/commons/upload/form.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/common/commons/upload/form.html`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 {% block box_body %}
 <div id="upload_errors" class="alert alert-danger" style="display: {{ data.errors|yesno:',none' }};">
     <h4><i class='fas fa-warning'></i>&nbsp;&nbsp;{{ data.errors | safe}} </h4>
 </div>
 <form id="form_start" action='{{data.url}}' method="post" enctype=multipart/form-data>
     {% csrf_token %}
     {{ data.upload_form }}
-    <input type="submit" class="btn btn-secondary float-right" value="Upload"/>
+    <input type="submit" class="btn btn-secondary {% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}" value="Upload"/>
 </form>
 
 {% block upload_addons %}{% endblock %}
 {% endblock %}
 
 {% block box_footer %}
 {% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/modals/create_data_modal.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/common/modals/create_data_modal.html`

 * *Files 19% similar despite different names*

```diff
@@ -5,10 +5,12 @@
 
 {% block modal_body %}
 <p>Are you sure you want to save a {% trans "record_label" %} from this {% trans "form_label" %} ?<p>
 <p>Your {% trans "form_label" %} will be deleted automatically.<p>
 {% endblock %}
 
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal"><i class="fas fa-times"></i> Close</a>
+<a class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal">
+    <i class="fas fa-times"></i> Close
+    </a>
 <a class="btn btn-primary save-data" ><i class="fas fa-save"></i> Save </a>
 {% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/modals/download-options.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/common/modals/download-options.html`

 * *Files 26% similar despite different names*

```diff
@@ -26,9 +26,11 @@
     <div class="mt-3">
         Click here to format content <input type="checkbox" id="format">
     </div>
 </div>
 {% endblock %}
 
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
+<a class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#">
+    <i class="fas fa-times"></i> Cancel
+</a>
 {% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/pagination/data_source_pagination.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/common/pagination/data_source_pagination.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/list/available.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/common/xslt/list/table.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,39 @@
-{% extends 'core_main_app/_render/admin/theme/tools/box.html' %}
-
-{% block box_title %}Available{% endblock %}
+{% block box_title %}XSLT list{% endblock %}
 
 {% block box_tools %}
-    <a href="{% url 'core-admin:core_main_app_upload_template'%}" class="float-right btn btn-secondary">
-        <i class="fas fa-upload"></i> Upload {{ data.object_name }}
-    </a>
+<div class="btn-group {% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}">
+<a href="{{ data.update_url }}" class="btn btn-secondary upload-xslt-btn">
+    <i class="fas fa-upload"></i> Upload XSLT
+</a>
+</div>
 {% endblock %}
 
 {% block box_body %}
 <table class="table table-bordered table-striped table-hover">
     <tr>
-        <th>{{ data.object_name }}</th>
+        <th>Name</th>
         <th>Actions</th>
     </tr>
 
-    {% for object in data.available %}
-        <tr>
-            <td>{{ object.title }}</td>
+    {% for elt in data.xslt %}
+        <tr objectid="{{ elt.id }}">
+            <td>{{ elt.name }}</td>
             <td>
-                {% block box_actions %}
-                <a class="btn btn-secondary"
-                   href="{% url 'core-admin:core_main_app_manage_template_versions' object.id %}">
-                    <i class="fas fa-list"></i> Versions
+                <a class="btn btn-secondary edit-xslt-btn" href="#">
+                    <i class="fas fa-edit"></i> Edit
                 </a>
-                <span class="icon legend edit" objectid="{{ object.id }}">
-                    <a class="btn btn-secondary" href="#"><i class="fas fa-edit"></i> Edit</a>
-                </span>
-                <span class="icon legend delete" objectid="{{ object.id }}">
-                    <button class="btn btn-danger"><i class="fas fa-trash"></i> Disable </button>
-                </span>
-                {% endblock %}
+                <button class="btn btn-danger delete-xslt-btn">
+                    <i class="fas fa-trash"></i> Delete
+                </button>
             </td>
         </tr>
     {% empty %}
         <tr>
             <td class="empty" colspan="2">
-                No {{ data.object_name }} uploaded.
+                There are currently no XSLT registered. Please
+                <a href="{{ data.update_url }}" class="upload-xslt-btn">upload a new one</a>.
             </td>
         </tr>
     {% endfor %}
 </table>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,12 +1,10 @@
-{% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% block
-box_title %}Available{% endblock %} {% block box_tools %}
- Upload_{{_data.object_name_}}
- {% endblock %} {% block box_body %}
-{{ data.object_name }} Actions
-                       {% block box_actions %}
-                        Versions
-{{ object.title }}
-                        Edit
-                           Disable   {% endblock %}
-No {{ data.object_name }} uploaded.
+{% block box_title %}XSLT list{% endblock %} {% block box_tools %}
+.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif
+%}">
+ Upload_XSLT
+{% endblock %} {% block box_body %}
+Name           Actions
+{{ elt.name }}  Edit
+                  Delete
+There are currently no XSLT registered. Please upload_a_new_one.
 {% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/list/disabled.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/common/templates/list/disabled.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/list/modals/disable.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/common/templates/list/modals/disable.html`

 * *Files 22% similar despite different names*

```diff
@@ -9,12 +9,14 @@
     The {{ data.object_name }} won't be erased from this website but nobody will be able to create or edit document that have been
     created with it.
 </p>
 <p>Are you sure you want to disable this {{ data.object_name }}?</p>
 {% endblock %}
 
 {% block modal_footer %}
-<button class="btn btn-secondary pull-left" data-dismiss="modal"><i class="fas fa-times"></i> No</button>
+<button class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal">
+    <i class="fas fa-times"></i> No
+</button>
 <button id="disable-template-yes" class="btn btn-danger"><i class="fas fa-check">
 
 </i> Yes</button>
 {% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/list/modals/edit.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/common/templates/list/modals/edit.html`

 * *Files 23% similar despite different names*

```diff
@@ -8,10 +8,12 @@
         <label for="edit-template-name">Enter new {{ data.object_name }} name</label>
         <input id="edit-template-name" class="form-control" type="text" value="" placeholder="new_template_name"/>
     </div>
 </form>
 {% endblock %}
 
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Close</a>
+<a class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#">
+    <i class="fas fa-times"></i> Close
+</a>
 <a id="edit-template-save" class="btn btn-primary" href="#"><i class="fas fa-save"></i> Save</a>
 {% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/versions/available.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/common/templates/versions/available.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,69 @@
-<!--FIXME: make a common box.html-->
+<!-- FIXME: make a common box.html instead of using the admin one -->
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %}
 {% load timestamptags %}
+{% load tz %}
 
 {% block box_title %}
-    Version manager for {{ data.object_name }} {{data.version_manager.title }}
+    Version manager for {{ data.object_name | lower }} {{data.version_manager.title }}
 {% endblock %}
 
-{% block box_tools %}
-
-{% endblock %}
+{% block box_tools %}{% endblock %}
 
 {% block box_body %}
+<style>
+    #model_version td.current {
+        font-weight: bold;
+        color: green;
+    }
+
+    #model_version td.uploaded {
+        font-weight: bold;
+        color: orange;
+    }
+</style>
 <div id="model_version">
 	<table class="table table-bordered table-hover">
-        <tr>
-            <th style="width: 15%">Version #</th>
-            <th style="width: 20%">Status</th>
-            <th style="width: 20%">Upload date</th>
-            <th>Actions</th>
-        </tr>
+        <thead>
+            <tr>
+                <th style="width: 15%">Version #</th>
+                <th style="width: 20%">Status</th>
+                <th style="width: 20%">Upload date</th>
+                <th>Actions</th>
+            </tr>
+        </thead>
+        <tbody>
 	    {% for version in data.categorized_versions.available reversed %}
-           <tr>
-               <td>{{ version.index }}</td>
-               {% if version.object == data.version_manager.current %}
-                    <td style='font-weight:bold;color:green'>Current</td>
-               {% else %}
-                    <td style='font-weight:bold;color:orange'>Uploaded</td>
-               {% endif %}
-
-               <td>
-                   {{ version.creation_date }}
-               </td>
+            <tr>
+                <td>{{ version.index }}</td>
+                {% if version.object == data.version_manager.current %}
+                    <td class="current">Current</td>
+                {% else %}
+                    <td class="uploaded">Uploaded</td>
+                {% endif %}
+
+                <td>{{ version.creation_date|localtime }}</td>
 
-               <td>
-                   {% block box_actions %}
+                <td>
+                {% block box_actions %}
                     <a class="btn btn-secondary results-xslt"
-                        href="{% url 'core_main_app_template_xslt' version.object %}">
+                       href="{% url 'core_main_app_template_xslt' version.object %}">
                         <i class="fas fa-file-code"></i> XSLT
                     </a>
-                   {% if 'core_parser_app' in INSTALLED_APPS %}
-                    <a class="btn btn-secondary modules"
-                        href="{% url 'core_parser_app_template_modules' version.object %}">
-                        <i class="fas fa-cubes"></i> Modules
+                    {% if 'core_parser_app' in INSTALLED_APPS %}
+                        <a class="btn btn-secondary modules"
+                           href="{% url 'core_parser_app_template_modules' version.object %}">
+                            <i class="fas fa-cubes"></i> Modules
+                        </a>
+                    {% endif %}
+                    <a class="btn btn-secondary download"
+                       href="{% url 'core_main_app_rest_template_download' version.object %}">
+                        <i class="fas fa-download"></i> Download
                     </a>
-                   {% endif %}
-                   <a class="btn btn-secondary download"
-                      href="{% url 'core_main_app_rest_template_download' version.object %}">
-                       <i class="fas fa-download"></i> Download
-                   </a>
-                   {% endblock %}
-               </td>
-           </tr>
-       {% endfor %}
+                {% endblock %}
+                </td>
+            </tr>
+        {% endfor %}
+        </tbody>
    </table>
 </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
  {% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% load
-timestamptags %} {% block box_title %} Version manager for {{ data.object_name
-}} {{data.version_manager.title }} {% endblock %} {% block box_tools %} {%
-endblock %} {% block box_body %}
-Version #           Status  Upload date Actions
-                                                              {% block
-                                                              box_actions %}
-                                                               XSLT
-                                        {                      {% if
-                                        {                     'core_parser_app'
-{{ version.index }} Current Uploaded    version.creation_date in INSTALLED_APPS
-                                        }}                    %}
-                                                               Modules
-                                                               {% endif %}
-                                                               Download
-                                                               {% endblock %}
+timestamptags %} {% load tz %} {% block box_title %} Version manager for {
+{ data.object_name | lower }} {{data.version_manager.title }} {% endblock %} {%
+block box_tools %}{% endblock %} {% block box_body %}
+Version #     Status  Upload   Actions
+                      date
+                                                               {% block
+                                                               box_actions %}
+                                                                XSLT
+{                              {                                {% if
+{                              {                               'core_parser_app'
+version.index Current Uploaded version.creation_date|localtime in INSTALLED_APPS
+}}                             }}                              %}
+                                                                Modules
+                                                                {% endif %}
+                                                                Download
+                                                                {% endblock %}
 {% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/versions/modals/disable.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/common/templates/versions/modals/disable.html`

 * *Files 16% similar despite different names*

```diff
@@ -7,10 +7,12 @@
 <p>
     The version won't be erased from this website but nobody will be able to switch to this version anymore.
 </p>
 <p>Are you sure you want to disable this version?</p>
 {% endblock %}
 
 {% block modal_footer %}
-<button class="btn btn-secondary pull-left" data-dismiss="modal"><i class="fas fa-times"></i> No </button>
+<button class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal">
+    <i class="fas fa-times"></i> No
+</button>
 <button id="disable-version-yes" class="btn btn-danger"><i class="fas fa-check"></i> Yes </button>
 {% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/list/modals/delete.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/common/xslt/list/modals/delete.html`

 * *Files 16% similar despite different names*

```diff
@@ -6,10 +6,12 @@
 <p>
     The XSLT will be erased definitely.
 </p>
 <p>Are you sure you want to delete this XSLT?</p>
 {% endblock %}
 
 {% block modal_footer %}
-<button class="btn btn-secondary pull-left" data-dismiss="modal"><i class="fas fa-times"></i> No</button>
+<button class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal">
+    <i class="fas fa-times"></i> No
+</button>
 <button id="delete-xslt-yes" class="btn btn-danger"><i class="fas fa-check"></i> Yes</button>
 {% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/list/modals/edit.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/common/xslt/list/modals/edit.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 
 {% block modal_id %}edit-xslt-modal{% endblock %}
 {% block modal_title %}Edit XSLT{% endblock %}
 
 {% block modal_body %}
 <div class="alert alert-danger" id="error-div-xslt" class="hidden">
-    <a href="#" class="close" data-hide="alert" aria-label="close">&times;</a>
+    <a href="#" class="{% if BOOTSTRAP_VERSION == "4.6.2" %}close{% elif BOOTSTRAP_VERSION == "5.1.3" %}btn-close{% endif %}" data-hide="alert" aria-label="close">{% if BOOTSTRAP_VERSION == "4.6.2" %}&times;{% elif BOOTSTRAP_VERSION == "5.1.3" %}{% endif %}</a>
     <h4><i class="fas fa-exclamation-circle"></i> Error</h4>
     <div id="error-message"></div>
 </div>
 <form id="edit-xslt-form">
     <input id="edit-xslt-id" type="hidden" value=""/>
     <div class="form-group">
         <label for="edit-xslt-name">Enter new XSLT name</label>
         <input id="edit-xslt-name" class="form-control" type="text" value="" placeholder="new_xslt_name"/>
     </div>
 </form>
 {% endblock %}
 
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Close</a>
+<a class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#">
+    <i class="fas fa-times"></i> Close
+</a>
 <a id="edit-xslt-save" class="btn btn-primary" href="#"><i class="fas fa-save"></i> Save</a>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,10 +1,13 @@
  {% block modal_id %}edit-xslt-modal{% endblock %} {% block modal_title %}Edit
 XSLT{% endblock %} {% block modal_body %}
-×
+.6.2" %}close{% elif BOOTSTRAP_VERSION == "5.1.3" %}btn-close{% endif %}" data-
+hide="alert" aria-label="close">{% if BOOTSTRAP_VERSION == "4.6.2" %}×{% elif
+BOOTSTRAP_VERSION == "5.1.3" %}{% endif %}
  Error
 Enter new XSLT name [                    ]
 {% endblock %} {% block modal_footer %}
- Close
+% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION ==
+"5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#">  Close
 
  Save
  {% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/user/login/main.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/user/login/main.html`

 * *Files 5% similar despite different names*

```diff
@@ -29,27 +29,29 @@
 
             {% for field in data.login_form.hidden_fields %}
                 {{ field }}
             {% endfor %}
 
             <div class="form-group">
                 <div class="row">
-                    {% if data.with_website_features %}
                     <div class="col-9">
+                    {% if data.with_website_features %}
                         <a class="btn btn-secondary btn-lg request account"
                            href="{% url 'core_website_app_account_request' %}">
                             <i class="fas fa-user-plus"></i> Request an Account
                         </a>
+                    {% endif %}
+                    {% if not data.ENABLE_SAML2_SSO_AUTH %}
                         <a class="btn btn-secondary btn-lg" href="{% url 'password_reset' %}">
                             <i class="fas fa-lock" aria-hidden="true"></i> Forgot password
                         </a>
-                    </div>
                     {% endif %}
+                    </div>
                     <div class="col-3">
-                        <button type="submit" class="btn btn-lg btn-primary float-right">
+                        <button type="submit" class="btn btn-lg btn-primary {% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}">
                             <i class="fas fa-sign-in-alt"></i> Login
                         </button>
                     </div>
                 </div>
 
             </div>
         </form>
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/user/login/modals/login_message.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/user/login/modals/login_message.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/user/sharing/modals/single-link.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/user/sharing/modals/single-link.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% extends 'core_main_app/_render/admin/theme/tools/modal.html' %}
 
 {% block modal_title %}Shareable link{% endblock %}
 
 {% block modal_body %}
     <div class="alert alert-danger" id="banner_set_name_query_errors" style="display: none;">
-            <a href="#" class="close" data-hide="alert" aria-label="close">&times;</a>
+            <a href="#" class="{% if BOOTSTRAP_VERSION == "4.6.2"%}close{% elif BOOTSTRAP_VERSION == "5.1.3" %}btn-close{% endif %}" data-hide="alert" aria-label="close">{% if BOOTSTRAP_VERSION == "4.6.2" %}&times;{% elif BOOTSTRAP_VERSION == "5.1.3" %}{% endif %}</a>
             <h4><i class="fas fa-exclamation-circle"></i> Error</h4>
             <div id="set_name_query_errors"></div>
     </div>
     <div>
         <input type="text" id="{% block modal_input_id %}{% endblock %}"
                class="shared-data w-100" disabled="disabled"/>
     </div>
```

#### html2text {}

```diff
@@ -1,9 +1,11 @@
 {% extends 'core_main_app/_render/admin/theme/tools/modal.html' %} {% block
 modal_title %}Shareable link{% endblock %} {% block modal_body %}
-×
+.6.2"%}close{% elif BOOTSTRAP_VERSION == "5.1.3" %}btn-close{% endif %}" data-
+hide="alert" aria-label="close">{% if BOOTSTRAP_VERSION == "4.6.2" %}×{% elif
+BOOTSTRAP_VERSION == "5.1.3" %}{% endif %}
  Error
 [                    ]
 {% block modal_extra_content %}{% endblock %} {% endblock %} {% block
 modal_footer %}
   Copy and close
 {% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/edit_rights.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/user/workspaces/edit_rights.html`

 * *Files 1% similar despite different names*

```diff
@@ -33,9 +33,9 @@
     <h4>Groups:</h4>
     {% if data.group_data %}
         {% include data.template with objects=data.group_data group="group" %}
     {%else%}
       <div class="empty-table">
         No groups have access to '{{ data.workspace.title }}'.
       </div>
-    {%endif%}
+    {% endif %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -12,8 +12,8 @@
 group="user" %} {% else %}
 No users have access to '{{ data.workspace.title }}'.
 {% endif %}
 *** Groups: ***
 {% if data.group_data %} {% include data.template with objects=data.group_data
 group="group" %} {%else%}
 No groups have access to '{{ data.workspace.title }}'.
-{%endif%} {% endblock %}
+{% endif %} {% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/create_workspace.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/user/workspaces/list/create_workspace.html`

 * *Files 15% similar despite different names*

```diff
@@ -14,26 +14,26 @@
     </div>
     <div>
         <input type="hidden" class="{{ data.document }}-id"/>
         <p class="m-0">Please enter the name of the new workspace.</p>
     </div>
     <div class="mt-2">
         {% for field in data.workspace_form %}
-            <div class="d-flex flex-row ml-4 mr-4">
+            <div class="d-flex flex-row mx-4">
                 <div class="d-flex align-items-center justify-content-center"
                      style="width:30%">
                     {{ field.label_tag }}
                 </div>
-                <div class="ml-2 d-flex align-items-center" style="width:90%">{{ field }}</div>
+                <div class="{% if BOOTSTRAP_VERSION == "4.6.2" %}ml-2{% elif BOOTSTRAP_VERSION == "5.1.3" %}ms-2{% endif %} d-flex align-items-center" style="width:90%">{{ field }}</div>
             </div>
         {% endfor %}
     </div>
 {% endblock %}
 
 {% block modal_footer %}
-    <button class="btn btn-secondary pull-left" data-dismiss="modal">
+    <button class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal">
         <i class="fas fa-times-circle"></i> Cancel
     </button>
     <button id="create-workspace-confirm" class="btn btn-primary">
         <i class="fas fa-plus-circle"></i> Create Workspace
     </button>
 {% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/edit_rights_table.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/user/workspaces/list/edit_rights_table.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_group.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_group.html`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     <div id="form_edit_group_rights_errors">
     </div>
 </div>
 <div id="group-rights">
     <p class="my-3">
         Select all groups you want to give rights to the workspace:
     </p>
-    <form id="add-group-form" class="p-2 my-3">
+    <form id="add-group-form" class="multiple-select-form p-2 my-3">
     </form>
     <div id="list-rights">
         <div class="row m-2">
             <div class="col-sm-1 mx-1">
                 <label class="switch">
                     <input type="checkbox" id="read_group">
                     <span class="slider"></span>
@@ -39,11 +39,13 @@
             </div>
         </div>
     </div>
 </div>
 {% endblock %}
 
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
+<a class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#">
+    <i class="fas fa-times"></i> Cancel
+</a>
 <a id="add-group-yes" class="btn btn-secondary" href="#"><i class="fas fa-check"></i> Add</a>
 {% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_user.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_user.html`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     </div>
 </div>
 <div id="user-rights">
     <p class="my-3">
        Select all users you want to give rights to the workspace:
     </p>
 
-    <form id="add-user-form" class="p-2 my-3" method="post">
+    <form id="add-user-form" class="multiple-select-form p-2 my-3" method="post">
     </form>
     <div id="list-rights">
         <div class="row m-2">
             <div class="col-sm-1 mx-1">
                 <label class="switch">
                     <input type="checkbox" id="read">
                     <span class="slider"></span>
@@ -40,11 +40,11 @@
             </div>
         </div>
     </div>
 </div>
 {% endblock %}
 
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
+<a class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#"><i class="fas fa-times"></i> Cancel</a>
 <a id="add-user-yes" class="btn btn-secondary" href="#"><i class="fas fa-check"></i> Add</a>
 {% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/set_private.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/set_private.html`

 * *Files 21% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 {% block modal_id %}private-workspace-modal{% endblock %}
 {% block modal_title %}Set workspace private{% endblock %}
 
 
 {% block modal_body %}
 <div class="alert alert-danger" id="banner_errors" style="display: none;">
-        <a href="#" class="close" data-hide="alert" aria-label="close">&times;</a>
+        <a href="#" class="{% if BOOTSTRAP_VERSION == "4.6.2" %}close{% elif BOOTSTRAP_VERSION == "5.1.3" %}btn-close{% endif %}" data-hide="alert" aria-label="close">{% if BOOTSTRAP_VERSION == "4.6.2" %}&times;{% elif BOOTSTRAP_VERSION == "5.1.3" %}{% endif %}</a>
      	<h4><i class="fas fa-exclamation-circle"></i> Error</h4>
         <div id="private_workspace_errors"></div>
 </div>
 <input type="hidden" class="{{data.document}}-id"/>
 <p>Are you sure you want to set the workspace private?</p>
 {% endblock %}
 
 {% block modal_footer %}
-<a class="btn btn-secondary pull-left" data-dismiss="modal" href="#">
+<a class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#">
     <i class="fas fa-times"></i> Cancel
 </a>
 <a id="private-workspace-yes" class="btn btn-primary" href="#">
     <i class="fas fa-check"></i> Set private
 </a>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,11 +1,14 @@
 {% extends 'core_main_app/_render/admin/theme/tools/modal.html' %} {% block
 modal_id %}private-workspace-modal{% endblock %} {% block modal_title %}Set
 workspace private{% endblock %} {% block modal_body %}
-×
+.6.2" %}close{% elif BOOTSTRAP_VERSION == "5.1.3" %}btn-close{% endif %}" data-
+hide="alert" aria-label="close">{% if BOOTSTRAP_VERSION == "4.6.2" %}×{% elif
+BOOTSTRAP_VERSION == "5.1.3" %}{% endif %}
  Error
 Are you sure you want to set the workspace private?
 {% endblock %} {% block modal_footer %}
- Cancel
+% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION ==
+"5.1.3" %}data-bs-dismiss{% endif %}="modal" href="#">  Cancel
 
  Set_private
  {% endblock %}
```

### Comparing `core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/switch_right.html` & `core_main_app-2.4.0/core_main_app/templates/core_main_app/user/blob/list/modals/add_metadata.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 00000000: 7b25 2065 7874 656e 6473 2027 636f 7265  {% extends 'core
 00000010: 5f6d 6169 6e5f 6170 702f 5f72 656e 6465  _main_app/_rende
 00000020: 722f 6164 6d69 6e2f 7468 656d 652f 746f  r/admin/theme/to
 00000030: 6f6c 732f 6d6f 6461 6c2e 6874 6d6c 2720  ols/modal.html' 
 00000040: 257d 0a0a 7b25 2062 6c6f 636b 206d 6f64  %}..{% block mod
-00000050: 616c 5f69 6420 257d 7377 6974 6368 2d72  al_id %}switch-r
-00000060: 6967 6874 732d 6d6f 6461 6c7b 2520 656e  ights-modal{% en
-00000070: 6462 6c6f 636b 2025 7d0a 7b25 2062 6c6f  dblock %}.{% blo
-00000080: 636b 206d 6f64 616c 5f74 6974 6c65 2025  ck modal_title %
-00000090: 7d50 726f 626c 656d 2077 6869 6c65 2075  }Problem while u
-000000a0: 7064 6174 696e 6720 7468 6520 6e65 7720  pdating the new 
-000000b0: 7065 726d 6973 7369 6f6e 2e7b 2520 656e  permission.{% en
-000000c0: 6462 6c6f 636b 2025 7d0a 0a0a 7b25 2062  dblock %}...{% b
-000000d0: 6c6f 636b 206d 6f64 616c 5f62 6f64 7920  lock modal_body 
-000000e0: 257d 0a3c 6469 7620 636c 6173 733d 2261  %}.<div class="a
-000000f0: 6c65 7274 2061 6c65 7274 2d64 616e 6765  lert alert-dange
-00000100: 7222 2069 643d 2273 7769 7463 685f 7269  r" id="switch_ri
-00000110: 6768 7473 5f62 616e 6e65 725f 6572 726f  ghts_banner_erro
-00000120: 7273 2220 7374 796c 653d 2264 6973 706c  rs" style="displ
-00000130: 6179 3a20 6e6f 6e65 3b22 3e0a 2020 2020  ay: none;">.    
-00000140: 2020 2020 3c61 2068 7265 663d 2223 2220      <a href="#" 
-00000150: 636c 6173 733d 2263 6c6f 7365 2220 6461  class="close" da
-00000160: 7461 2d68 6964 653d 2261 6c65 7274 2220  ta-hide="alert" 
-00000170: 6172 6961 2d6c 6162 656c 3d22 636c 6f73  aria-label="clos
-00000180: 6522 3e26 7469 6d65 733b 3c2f 613e 0a20  e">&times;</a>. 
-00000190: 2020 2020 093c 6834 3e3c 6920 636c 6173      .<h4><i clas
-000001a0: 733d 2266 6173 2066 612d 6578 636c 616d  s="fas fa-exclam
-000001b0: 6174 696f 6e2d 6369 7263 6c65 223e 3c2f  ation-circle"></
-000001c0: 693e 2045 7272 6f72 3c2f 6834 3e0a 2020  i> Error</h4>.  
-000001d0: 2020 2020 2020 3c64 6976 2069 643d 2273        <div id="s
-000001e0: 7769 7463 685f 7269 6768 7473 5f65 7272  witch_rights_err
-000001f0: 6f72 7322 3e3c 2f64 6976 3e0a 3c2f 6469  ors"></div>.</di
-00000200: 763e 0a7b 2520 656e 6462 6c6f 636b 2025  v>.{% endblock %
-00000210: 7d0a 0a7b 2520 626c 6f63 6b20 6d6f 6461  }..{% block moda
-00000220: 6c5f 666f 6f74 6572 2025 7d0a 3c61 2063  l_footer %}.<a c
-00000230: 6c61 7373 3d22 6274 6e20 6274 6e2d 7365  lass="btn btn-se
-00000240: 636f 6e64 6172 7920 7075 6c6c 2d6c 6566  condary pull-lef
-00000250: 7422 2064 6174 612d 6469 736d 6973 733d  t" data-dismiss=
-00000260: 226d 6f64 616c 2220 6872 6566 3d22 2322  "modal" href="#"
-00000270: 3e3c 6920 636c 6173 733d 2266 6173 2066  ><i class="fas f
-00000280: 612d 7469 6d65 7322 3e3c 2f69 3e20 4f6b  a-times"></i> Ok
-00000290: 3c2f 613e 0a7b 2520 656e 6462 6c6f 636b  </a>.{% endblock
-000002a0: 2025 7d                                   %}
+00000050: 616c 5f69 6420 257d 6164 642d 6d65 7461  al_id %}add-meta
+00000060: 6461 7461 2d6d 6f64 616c 7b25 2065 6e64  data-modal{% end
+00000070: 626c 6f63 6b20 257d 0a7b 2520 626c 6f63  block %}.{% bloc
+00000080: 6b20 6d6f 6461 6c5f 7469 746c 6520 257d  k modal_title %}
+00000090: 2041 6464 204d 6574 6164 6174 6120 7b25   Add Metadata {%
+000000a0: 2065 6e64 626c 6f63 6b20 257d 0a0a 7b25   endblock %}..{%
+000000b0: 2062 6c6f 636b 206d 6f64 616c 5f62 6f64   block modal_bod
+000000c0: 7920 257d 0a3c 6469 7620 6964 3d22 626c  y %}.<div id="bl
+000000d0: 6f62 5f6d 6574 6164 6174 6122 3e0a 2020  ob_metadata">.  
+000000e0: 2020 5365 6c65 6374 206d 6574 6164 6174    Select metadat
+000000f0: 6120 646f 6375 6d65 6e74 2074 6f20 6c69  a document to li
+00000100: 6e6b 2074 6f20 7468 6973 2066 696c 653a  nk to this file:
+00000110: 0a20 2020 203c 6469 7620 6964 3d22 6164  .    <div id="ad
+00000120: 642d 6d65 7461 6461 7461 223e 0a20 2020  d-metadata">.   
+00000130: 203c 2f64 6976 3e0a 3c2f 6469 763e 0a7b   </div>.</div>.{
+00000140: 2520 656e 6462 6c6f 636b 2025 7d0a 0a7b  % endblock %}..{
+00000150: 2520 626c 6f63 6b20 6d6f 6461 6c5f 666f  % block modal_fo
+00000160: 6f74 6572 2025 7d0a 3c61 2063 6c61 7373  oter %}.<a class
+00000170: 3d22 6274 6e20 6274 6e2d 7365 636f 6e64  ="btn btn-second
+00000180: 6172 7920 7075 6c6c 2d6c 6566 7422 207b  ary pull-left" {
+00000190: 2520 6966 2042 4f4f 5453 5452 4150 5f56  % if BOOTSTRAP_V
+000001a0: 4552 5349 4f4e 203d 3d20 2234 2e36 2e32  ERSION == "4.6.2
+000001b0: 2220 257d 6461 7461 2d64 6973 6d69 7373  " %}data-dismiss
+000001c0: 7b25 2065 6c69 6620 424f 4f54 5354 5241  {% elif BOOTSTRA
+000001d0: 505f 5645 5253 494f 4e20 3d3d 2022 352e  P_VERSION == "5.
+000001e0: 312e 3322 2025 7d64 6174 612d 6273 2d64  1.3" %}data-bs-d
+000001f0: 6973 6d69 7373 7b25 2065 6e64 6966 2025  ismiss{% endif %
+00000200: 7d3d 226d 6f64 616c 2220 6872 6566 3d22  }="modal" href="
+00000210: 2322 3e3c 6920 636c 6173 733d 2266 6173  #"><i class="fas
+00000220: 2066 612d 7469 6d65 7322 3e3c 2f69 3e20   fa-times"></i> 
+00000230: 4361 6e63 656c 3c2f 613e 0a3c 6120 6964  Cancel</a>.<a id
+00000240: 3d22 6164 642d 6d65 7461 6461 7461 2d79  ="add-metadata-y
+00000250: 6573 2220 636c 6173 733d 2262 746e 2062  es" class="btn b
+00000260: 746e 2d73 6563 6f6e 6461 7279 2220 6872  tn-secondary" hr
+00000270: 6566 3d22 2322 3e3c 6920 636c 6173 733d  ef="#"><i class=
+00000280: 2266 6173 2066 612d 6368 6563 6b22 3e3c  "fas fa-check"><
+00000290: 2f69 3e20 4164 643c 2f61 3e0a 7b25 2065  /i> Add</a>.{% e
+000002a0: 6e64 626c 6f63 6b20 257d 0a0a            ndblock %}..
```

### Comparing `core_main_app-2.3.0/core_main_app/templatetags/auth_extras.py` & `core_main_app-2.4.0/core_main_app/templatetags/auth_extras.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/templatetags/get_attribute.py` & `core_main_app-2.4.0/core_main_app/templatetags/get_attribute.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/templatetags/include_static.py` & `core_main_app-2.4.0/core_main_app/templatetags/include_static.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/templatetags/json_date.py` & `core_main_app-2.4.0/core_main_app/templatetags/json_date.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/templatetags/stripjs.py` & `core_main_app-2.4.0/core_main_app/templatetags/stripjs.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/templatetags/xsl_transform_tag.py` & `core_main_app-2.4.0/core_main_app/templatetags/xsl_transform_tag.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/urls.py` & `core_main_app-2.4.0/core_main_app/urls.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,54 @@
 """ Url router for the main application
 """
 from django.conf.urls import include
 from django.contrib.auth.decorators import login_required
 from django.urls import re_path
-from drf_yasg import openapi
-from drf_yasg.views import get_schema_view
+from drf_spectacular.views import SpectacularAPIView, SpectacularSwaggerView
 
 from core_main_app.components.blob import api as blob_api
 from core_main_app.components.data import api as data_api
 from core_main_app.utils.rendering import render
 from core_main_app.utils.urls import get_auth_urls
 from core_main_app.views.common import (
     ajax as common_ajax,
     views as common_views,
 )
 from core_main_app.views.user import views as user_views, ajax as user_ajax
 
-SchemaView = get_schema_view(
-    openapi.Info(
-        title="REST API",
-        default_version="v1",
-    ),
-)
-
 urlpatterns = [
     re_path(r"^$", user_views.homepage, name="core_main_app_homepage"),
+    re_path("api/schema/", SpectacularAPIView.as_view(), name="schema"),
+    re_path(
+        "docs/api/",
+        SpectacularSwaggerView.as_view(url_name="schema"),
+        name="swagger_view",
+    ),
     re_path(
         r"^locked",
         common_views.defender_error_page,
         name="core_main_app_locked",
     ),
     re_path(r"^rest/", include("core_main_app.rest.urls")),
     re_path(
         r"^data",
         common_views.ViewData.as_view(),
         name="core_main_app_data_detail",
     ),
     re_path(
+        r"^blob/(?P<pk>[\w-]+)/metadata",
+        login_required(common_views.ManageBlobMetadata.as_view()),
+        name="core_main_app_blob_metadata",
+    ),
+    re_path(
+        r"^blob",
+        common_views.ViewBlob.as_view(),
+        name="core_main_app_blob_detail",
+    ),
+    re_path(
         r"^xml-editor/data",
         login_required(
             common_views.DataContentEditor.as_view(),
         ),
         name="core_main_app_xml_text_editor_view",
     ),
     re_path(
@@ -104,45 +112,44 @@
     ),
     re_path(
         r"^add-group-form",
         user_ajax.load_add_group_form,
         name="core_main_edit_rights_groups_form",
     ),
     re_path(
-        r"^add-group-right-to-workspace",
-        user_ajax.add_group_right_to_workspace,
-        name="core_main_add_group_right_to_workspace",
-    ),
-    re_path(
-        r"^docs/api$",
-        SchemaView.with_ui("swagger", cache_timeout=0),
-        name="swagger_view",
+        r"^add-metadata-form",
+        user_ajax.LoadBlobMetadataForm.as_view(),
+        name="core_main_blob_metadata_form",
     ),
-    re_path(r"^tz_detect/", include("tz_detect.urls")),
     re_path(
-        r"^password_reset/$",
-        user_views.custom_reset_password,
-        name="password_reset",
+        r"^add-metadata-to-blob",
+        user_ajax.AddMetadataToBlob.as_view(),
+        name="core_main_blob_add_metadata",
     ),
     re_path(
-        r"^password_reset/done/$",
-        user_views.custom_password_reset_done,
-        name="password_reset_done",
+        r"^remove-metadata-from-blob",
+        user_ajax.RemoveMetadataFromBlob.as_view(),
+        name="core_main_blob_remove_metadata",
     ),
     re_path(
-        r"^reset/(?P<uidb64>[0-9A-Za-z_\-]+)/(?P<token>[0-9A-Za-z]{1,13}-[0-9A-Za-z]{1,20})/$",
-        user_views.custom_password_reset_confirm,
-        name="password_reset_confirm",
+        r"^upload-file",
+        user_ajax.UploadFile.as_view(),
+        name="core_main_upload_file",
     ),
     re_path(
-        r"^reset/done/$",
-        user_views.custom_password_reset_complete,
-        name="password_reset_complete",
+        r"^add-group-right-to-workspace",
+        user_ajax.add_group_right_to_workspace,
+        name="core_main_add_group_right_to_workspace",
     ),
     re_path(
         r"^change-data-display",
         user_ajax.change_data_display,
         name="core_main_add_change_data_display",
     ),
+    re_path(
+        r"^set-timezone",
+        user_views.set_timezone,
+        name="core_main_set_timezone",
+    ),
 ]
 
 urlpatterns.extend(get_auth_urls())
```

### Comparing `core_main_app-2.3.0/core_main_app/utils/admin_site/model_admin_class.py` & `core_main_app-2.4.0/core_main_app/utils/admin_site/model_admin_class.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/blob_downloader.py` & `core_main_app-2.4.0/core_main_app/utils/blob_downloader.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/checksum.py` & `core_main_app-2.4.0/core_main_app/utils/checksum.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/custom_context_processors.py` & `core_main_app-2.4.0/core_main_app/utils/custom_context_processors.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,8 +50,11 @@
         "LOGIN_URL": settings.LOGIN_URL
         if hasattr(settings, "LOGIN_URL")
         else "",
         "BOOTSTRAP_VERSION": settings.BOOTSTRAP_VERSION
         if hasattr(settings, "BOOTSTRAP_VERSION")
         and settings.BOOTSTRAP_VERSION in ["4.6.2", "5.1.3"]
         else "4.6.2",
+        "PROJECT_VERSION": settings.PROJECT_VERSION
+        if hasattr(settings, "PROJECT_VERSION")
+        else "0.0.0",
     }
```

### Comparing `core_main_app-2.3.0/core_main_app/utils/databases/backend.py` & `core_main_app-2.4.0/core_main_app/utils/databases/backend.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/databases/mongo/__init__.py` & `core_main_app-2.4.0/core_main_app/utils/databases/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/databases/mongo/mongoengine_database.py` & `core_main_app-2.4.0/core_main_app/utils/databases/mongo/mongoengine_database.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/databases/mongo/pymongo_database.py` & `core_main_app-2.4.0/core_main_app/utils/databases/mongo/pymongo_database.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/decorators.py` & `core_main_app-2.4.0/core_main_app/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/file.py` & `core_main_app-2.4.0/core_main_app/utils/file.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/integration_tests/integration_base_test_case.py` & `core_main_app-2.4.0/core_main_app/utils/integration_tests/integration_base_test_case.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/integration_tests/integration_base_transaction_test_case.py` & `core_main_app-2.4.0/core_main_app/utils/integration_tests/integration_base_transaction_test_case.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/logger/logger_utils.py` & `core_main_app-2.4.0/core_main_app/utils/logger/logger_utils.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/migrations.py` & `core_main_app-2.4.0/core_main_app/utils/migrations.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/notifications/mail.py` & `core_main_app-2.4.0/core_main_app/utils/notifications/mail.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/notifications/tasks/task_mail.py` & `core_main_app-2.4.0/core_main_app/utils/notifications/tasks/task_mail.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/pagination/django_paginator/results_paginator.py` & `core_main_app-2.4.0/core_main_app/utils/pagination/django_paginator/results_paginator.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/pagination/mongoengine_paginator/paginator.py` & `core_main_app-2.4.0/core_main_app/utils/pagination/mongoengine_paginator/paginator.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/pagination/rest_framework_paginator/pagination.py` & `core_main_app-2.4.0/core_main_app/utils/pagination/rest_framework_paginator/pagination.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/pagination/rest_framework_paginator/rest_framework_paginator.py` & `core_main_app-2.4.0/core_main_app/utils/pagination/rest_framework_paginator/rest_framework_paginator.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/query/mongo/prepare.py` & `core_main_app-2.4.0/core_main_app/utils/query/mongo/prepare.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/query/mongo/query_builder.py` & `core_main_app-2.4.0/core_main_app/utils/query/mongo/query_builder.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/raw_query/common.py` & `core_main_app-2.4.0/core_main_app/utils/raw_query/common.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/raw_query/django_raw_query.py` & `core_main_app-2.4.0/core_main_app/utils/raw_query/django_raw_query.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/raw_query/mongo_raw_query.py` & `core_main_app-2.4.0/core_main_app/utils/raw_query/mongo_raw_query.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/rendering.py` & `core_main_app-2.4.0/core_main_app/utils/rendering.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/requests_utils/access_control.py` & `core_main_app-2.4.0/core_main_app/utils/requests_utils/access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/requests_utils/requests_utils.py` & `core_main_app-2.4.0/core_main_app/utils/requests_utils/requests_utils.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/requests_utils/ssl.py` & `core_main_app-2.4.0/core_main_app/utils/requests_utils/ssl.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/resolvers/requests_resolver.py` & `core_main_app-2.4.0/core_main_app/utils/resolvers/requests_resolver.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/resolvers/resolver_utils.py` & `core_main_app-2.4.0/core_main_app/utils/resolvers/resolver_utils.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/saml2/utils.py` & `core_main_app-2.4.0/core_main_app/utils/saml2/utils.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/storage/gridfs_storage.py` & `core_main_app-2.4.0/core_main_app/utils/storage/gridfs_storage.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/storage/storage.py` & `core_main_app-2.4.0/core_main_app/utils/storage/storage.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/tests_tools/RequestMock.py` & `core_main_app-2.4.0/core_main_app/utils/tests_tools/RequestMock.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/validation/regex_validation.py` & `core_main_app-2.4.0/core_main_app/utils/validation/regex_validation.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/validation/xpath_validation.py` & `core_main_app-2.4.0/core_main_app/utils/validation/xpath_validation.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/view_builders/data.py` & `core_main_app-2.4.0/core_main_app/utils/view_builders/data.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/xml.py` & `core_main_app-2.4.0/core_main_app/utils/xml.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/xsd_flattener/xsd_flattener_database_url.py` & `core_main_app-2.4.0/core_main_app/utils/xsd_flattener/xsd_flattener_database_url.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/utils/xsd_flattener/xsd_flattener_requests_url.py` & `core_main_app-2.4.0/core_main_app/utils/xsd_flattener/xsd_flattener_requests_url.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/views/admin/ajax.py` & `core_main_app-2.4.0/core_main_app/views/admin/ajax.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/views/admin/forms.py` & `core_main_app-2.4.0/core_main_app/views/admin/forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Forms for admin views
 """
 from django import forms
+from django.conf import settings
 from django.forms import ModelForm
 
 from core_main_app.commons.validators import ExtensionValidator
 from core_main_app.components.template_version_manager.models import (
     TemplateVersionManager,
 )
 from core_main_app.components.xsl_transformation import (
@@ -121,35 +122,45 @@
     id = forms.CharField(widget=forms.HiddenInput(), required=False)
     template = forms.CharField(widget=forms.HiddenInput(), required=False)
 
     list_xslt = forms.ModelChoiceField(
         label="Set XSLT to render a list of data",
         empty_label="(No XSLT)",
         required=False,
-        widget=forms.Select(attrs={"class": "form-control"}),
+        widget=forms.Select(),
         queryset=xsl_transformation_api.get_all(),
     )
 
     list_detail_xslt = forms.MultipleChoiceField(
         label="Set XSLT to render a single data",
         required=False,
         widget=forms.widgets.CheckboxSelectMultiple,
     )
 
     default_detail_xslt = forms.ModelChoiceField(
         label="Default rendering",
         empty_label="(No XSLT)",
         required=False,
-        widget=forms.Select(attrs={"class": "form-control"}),
+        widget=forms.Select(),
         queryset=xsl_transformation_api.get_all(),
     )
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.fields["list_detail_xslt"].choices = _get_xsl_transformation()
+        if settings.BOOTSTRAP_VERSION == "4.6.2":
+            self.fields["list_xslt"].widget.attrs["class"] = "form-control"
+            self.fields["default_detail_xslt"].widget.attrs[
+                "class"
+            ] = "form-control"
+        elif settings.BOOTSTRAP_VERSION == "5.1.3":
+            self.fields["list_xslt"].widget.attrs["class"] = "form-select"
+            self.fields["default_detail_xslt"].widget.attrs[
+                "class"
+            ] = "form-select"
 
 
 class TextAreaForm(forms.Form):
     """TextArea Form"""
 
     content = forms.CharField(
         label="",
```

### Comparing `core_main_app-2.3.0/core_main_app/views/admin/views.py` & `core_main_app-2.4.0/core_main_app/views/admin/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -676,15 +676,15 @@
             if page is None:
                 page = WebPage(type=self.web_page_type, content=content)
             else:
                 page.content = content
 
             self.api.upsert(page)
             messages.add_message(
-                request, messages.INFO, "Information saved with success."
+                request, messages.SUCCESS, "Information saved with success."
             )
 
             return redirect(reverse(self.post_redirect))
 
 
 @staff_member_required
 def data_migration(request):
```

### Comparing `core_main_app-2.3.0/core_main_app/views/common/ajax.py` & `core_main_app-2.4.0/core_main_app/views/common/ajax.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/core_main_app/views/common/views.py` & `core_main_app-2.4.0/core_main_app/views/common/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 from core_main_app.utils import group as group_utils
 from core_main_app.utils import xml as main_xml_utils
 from core_main_app.utils.labels import get_data_label
 from core_main_app.utils.rendering import admin_render, render
 from core_main_app.utils.view_builders import data as data_view_builder
 from core_main_app.views.admin.forms import TemplateXsltRenderingForm
 from xml_utils.xsd_tree.xsd_tree import XSDTree
+from core_main_app.components.blob import api as blob_api
 
 
 class CommonView(View, metaclass=ABCMeta):
     """
     Abstract common view for admin and user.
     """
 
@@ -880,15 +881,15 @@
             data.xml_content = content
             # save data
             data_api.upsert(data, self.request)
             lock_api.remove_lock_on_object(data, self.request.user)
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
@@ -1023,7 +1024,154 @@
             )
         except AccessControlError as ace:
             return HttpResponseForbidden(html_escape(str(ace)))
         except DoesNotExist as dne:
             return HttpResponseBadRequest(html_escape(str(dne)))
         except Exception as e:
             return HttpResponseBadRequest(html_escape(str(e)))
+
+
+class ViewBlob(CommonView):
+    """
+    View blob.
+    """
+
+    template = "core_main_app/user/blob/detail.html"
+
+    def get(self, request, *args, **kwargs):
+        """get
+
+        Args:
+            request:
+
+        Returns:
+        """
+        blob_id = request.GET["id"]
+
+        try:
+            # Get blob
+            blob_object = blob_api.get_by_id(blob_id, request.user)
+            try:
+                acl_api.check_can_write(blob_object, request.user)
+                can_write = True
+            except AccessControlError:
+                can_write = False
+            # Init context
+            context = {"blob": blob_object, "can_write": can_write}
+            # Init assets
+            assets = {
+                "js": [
+                    {
+                        "path": "core_main_app/user/js/blob/detail.js",
+                        "is_raw": False,
+                    }
+                ],
+                "css": [],
+            }
+
+            context.update({"page_title": "View File"})
+
+            return self.common_render(
+                request,
+                self.template,
+                assets=assets,
+                context=context,
+            )
+        except exceptions.DoesNotExist:
+            error_message = "Blob not found"
+            status_code = 404
+        except AccessControlError:
+            error_message = "Access Forbidden"
+            status_code = 403
+        except Exception as e:
+            error_message = str(e)
+            status_code = 400
+
+        return self.common_render(
+            request,
+            "core_main_app/common/commons/error.html",
+            context={
+                "error": "Unable to access the requested file"
+                + f": {error_message}.",
+                "status_code": status_code,
+                "page_title": "Error",
+            },
+        )
+
+
+class ManageBlobMetadata(CommonView):
+    """
+    Manage blob metadata.
+    """
+
+    template = "core_main_app/user/blob/blob_metadata.html"
+
+    def get(self, request, pk, *args, **kwargs):
+        """get
+
+        Args:
+            request:
+            pk:
+
+        Returns:
+        """
+
+        try:
+            # Get blob
+            blob_object = blob_api.get_by_id(pk, request.user)
+            try:
+                acl_api.check_can_write(blob_object, request.user)
+                can_write = True
+            except AccessControlError:
+                can_write = False
+            # Init context
+            context = {"blob": blob_object, "can_write": can_write}
+            # Init modals
+            modals = [
+                "core_main_app/user/blob/list/modals/add_metadata.html",
+            ]
+            # Init assets
+            assets = {
+                "js": [
+                    {
+                        "path": "core_main_app/user/js/blob/detail.js",
+                        "is_raw": False,
+                    },
+                    {
+                        "path": "core_main_app/user/js/blob/blob_metadata.js",
+                        "is_raw": False,
+                    },
+                ],
+                "css": [
+                    "core_main_app/common/css/select.css",
+                ],
+            }
+
+            context.update({"page_title": "File Metadata"})
+
+            return self.common_render(
+                request,
+                self.template,
+                modals=modals,
+                assets=assets,
+                context=context,
+            )
+        except exceptions.DoesNotExist:
+            error_message = "Blob not found"
+            status_code = 404
+        except AccessControlError:
+            error_message = "Access Forbidden"
+            status_code = 403
+        except Exception as e:
+            error_message = str(e)
+            status_code = 400
+
+        return self.common_render(
+            request,
+            "core_main_app/common/commons/error.html",
+            context={
+                "error": "Unable to access the requested file "
+                + f": {error_message}.",
+                "status_code": status_code,
+                "page_title": "Error",
+            },
+        )
```

### Comparing `core_main_app-2.3.0/core_main_app/views/user/ajax.py` & `core_main_app-2.4.0/core_main_app/views/user/ajax.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 """ Ajax API
 """
 import json
 
+from django.contrib import messages
 from django.contrib.auth.decorators import login_required
 from django.http import (
     HttpResponse,
     HttpResponseBadRequest,
     HttpResponseForbidden,
 )
 from django.template import loader
 from django.utils.decorators import method_decorator
 from django.utils.html import escape
 from django.views.generic import View
 
+from core_main_app.access_control.api import check_can_write
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.commons import exceptions
 from core_main_app.commons.exceptions import DoesNotExist, ModelError
+from core_main_app.components.blob import api as blob_api
+from core_main_app.components.blob.models import Blob
 from core_main_app.components.data import api as data_api
-from core_main_app.components.template import api as template_api
 from core_main_app.components.group import api as group_api
+from core_main_app.components.template import api as template_api
 from core_main_app.components.user import api as user_api
 from core_main_app.components.workspace import api as workspace_api
 from core_main_app.templatetags.xsl_transform_tag import (
     render_xml_as_html_detail,
 )
 from core_main_app.utils import group as group_utils
 from core_main_app.views.user.forms import (
     ChangeWorkspaceForm,
     UserRightForm,
     GroupRightForm,
+    BlobMetadataForm,
+    BlobFileForm,
 )
 
-
 GROUP = "group"
 USER = "user"
 
 ACTION_READ = "action_read"
 ACTION_WRITE = "action_write"
 
 
@@ -552,7 +557,165 @@
             ),
             "application/javascript",
         )
     except AccessControlError:
         return HttpResponseForbidden("Access Forbidden")
     except Exception:
         return HttpResponseBadRequest("Unexpected error")
+
+
+@method_decorator(login_required, name="dispatch")
+class LoadBlobMetadataForm(View):
+    """Load the form to add metadata files to a blob."""
+
+    def get(self, request):
+        """Load the form to add metadata files to a blob.
+
+        Args:
+            request:
+
+        Returns:
+
+        """
+        blob_id = request.GET.get("blob_id", None)
+
+        try:
+            blob_object = blob_api.get_by_id(str(blob_id), request.user)
+            form = BlobMetadataForm(user=request.user, blob=blob_object)
+        except exceptions.ModelError:
+            return HttpResponseBadRequest("Blob not found.")
+        except Exception:
+            return HttpResponseBadRequest("An unexpected error occurred.")
+
+        context = {"add_metadata_form": form}
+
+        return HttpResponse(
+            json.dumps(
+                {
+                    "form": loader.render_to_string(
+                        "core_main_app/user/blob/list/modals/add_metadata_form.html",
+                        context,
+                    )
+                }
+            ),
+            "application/javascript",
+        )
+
+
+@method_decorator(login_required, name="dispatch")
+class AddMetadataToBlob(View):
+    """Add metadata files to a blob."""
+
+    def post(self, request):
+        """Add metadata files to a blob.
+
+        Args:
+            request:
+
+        Returns:
+
+        """
+        blob_id = request.POST.get("blob_id", None)
+        metadata_id_list = request.POST.getlist("metadata_id[]", [])
+
+        try:
+            blob_object = blob_api.get_by_id(str(blob_id), request.user)
+            check_can_write(blob_object, request.user)
+            blob_api.add_metadata_list(
+                blob_object,
+                [
+                    data_api.get_by_id(metadata_id, request.user)
+                    for metadata_id in metadata_id_list
+                ],
+                request.user,
+            )
+        except exceptions.ModelError:
+            return HttpResponseBadRequest("Blob not found.")
+        except AccessControlError:
+            return HttpResponseBadRequest("Permission denied.")
+        except Exception:
+            return HttpResponseBadRequest("An unexpected error occurred.")
+
+        messages.add_message(
+            request,
+            messages.SUCCESS,
+            "Metadata updated.",
+        )
+        return HttpResponse(json.dumps({}), "application/javascript")
+
+
+@method_decorator(login_required, name="dispatch")
+class RemoveMetadataFromBlob(View):
+    """Remove metadata file from blob."""
+
+    def post(self, request):
+        """Remove metadata file
+
+        Args:
+            request:
+
+        Returns:
+
+        """
+        blob_id = request.POST.get("blob_id", None)
+        metadata_id = request.POST.get("metadata_id", None)
+
+        try:
+            blob_object = blob_api.get_by_id(str(blob_id), request.user)
+            check_can_write(blob_object, request.user)
+            metadata = data_api.get_by_id(metadata_id, request.user)
+            blob_api.remove_metadata(blob_object, metadata, request.user)
+        except exceptions.ModelError:
+            return HttpResponseBadRequest("Blob not found.")
+        except AccessControlError:
+            return HttpResponseBadRequest("Permission denied.")
+        except Exception:
+            return HttpResponseBadRequest("An unexpected error occurred.")
+
+        messages.add_message(
+            request,
+            messages.INFO,
+            "Metadata successfully removed.",
+        )
+        return HttpResponse(json.dumps({}), "application/javascript")
+
+
+@method_decorator(login_required, name="dispatch")
+class UploadFile(View):
+    """Upload file"""
+
+    def post(self, request):
+        """Upload file
+
+        Args:
+            request:
+
+        Returns:
+
+        """
+        try:
+            form = BlobFileForm(request.POST, request.FILES)
+            if form.is_valid():
+                blob = Blob(
+                    filename=form.files["file"].name,
+                    blob=form.files["file"],
+                    user_id=str(request.user.id),
+                )
+                blob_api.insert(blob, request.user)
+                messages.add_message(
+                    request,
+                    messages.SUCCESS,
+                    "File successfully uploaded.",
+                )
+                return HttpResponse(json.dumps({}))
+            else:
+                return HttpResponseBadRequest(
+                    json.dumps({"message": str(form.errors.as_text())})
+                )
+        except Exception:
+            messages.add_message(
+                request,
+                messages.ERROR,
+                "An error occurred during file upload.",
+            )
+
+            return HttpResponseBadRequest(json.dumps({}))
```

### Comparing `core_main_app-2.3.0/core_main_app/views/user/forms.py` & `core_main_app-2.4.0/core_main_app/views/user/forms.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """ Form needed for the user part of everything
 """
 from django import forms
+from django.conf import settings
 
 from core_main_app.commons.exceptions import DoesNotExist
+from core_main_app.components.data import api as data_api
 from core_main_app.components.user import api as user_api
 from core_main_app.components.workspace import api as workspace_api
 from core_main_app.utils.labels import get_data_label
 
 
 class LoginForm(forms.Form):
     """Custom login form for the user"""
@@ -93,15 +95,15 @@
     """
     Form to select a workspace.
     """
 
     workspaces = forms.ChoiceField(
         label="",
         required=True,
-        widget=forms.Select(attrs={"class": "form-control"}),
+        widget=forms.Select(),
     )
     WORKSPACES_OPTIONS = []
 
     def __init__(
         self,
         user,
         list_current_workspace=None,
@@ -166,7 +168,55 @@
                         + ")",
                     )
                 )
 
         super().__init__()
         self.fields["workspaces"].choices = []
         self.fields["workspaces"].choices = self.WORKSPACES_OPTIONS
+
+        if settings.BOOTSTRAP_VERSION == "4.6.2":
+            self.fields["workspaces"].widget.attrs["class"] = "form-control"
+        elif settings.BOOTSTRAP_VERSION == "5.1.3":
+            self.fields["workspaces"].widget.attrs["class"] = "form-select"
+
+
+class BlobMetadataForm(forms.Form):
+    """
+    Form blob metadata.
+    """
+
+    metadata = forms.MultipleChoiceField(
+        label="",
+        required=True,
+        widget=forms.CheckboxSelectMultiple(
+            attrs={"class": "multiple-columns"}
+        ),
+    )
+
+    def __init__(self, user, blob):
+        # Init user data
+        self.user_data = []
+        # Get user data
+        user_data = data_api.get_all_by_user(user)
+
+        # Build data list
+        for data in user_data:
+            # If data not already associated with blob
+            if data not in blob.metadata(user):
+                self.user_data.append((data.id, data.title))
+
+        super().__init__()
+        self.fields["metadata"].choices = []
+        self.fields["metadata"].choices = self.user_data
+
+
+class BlobFileForm(forms.Form):
+    """
+    Form blob file.
+    """
+
+    file = forms.FileField(
+        label="",
+        widget=forms.FileInput(
+            attrs={"class": "form-control form-control-lg"}
+        ),
+    )
```

### Comparing `core_main_app-2.3.0/core_main_app.egg-info/PKG-INFO` & `core_main_app-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: core-main-app
-Version: 2.3.0
+Name: core_main_app
+Version: 2.4.0
 Summary: Main functionalities for the curator core project
 Home-page: https://github.com/usnistgov/core_main_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =============
         Core Main App
@@ -47,34 +47,24 @@
         
         Configuration
         =============
         
         Edit the setting.py file
         ------------------------
         
-        Add the ``"core_main_app"`` and ``"tz_detect"`` under ``INSTALLED_APPS`` as
+        Add the ``"core_main_app"`` under ``INSTALLED_APPS`` as
         such:
         
         .. code:: python
         
             INSTALLED_APPS = [
                 ...
-                "tz_detect",
                 "core_main_app",
             ]
         
-        Add the middleware required by ``tz_detect``:
-        
-        .. code:: python
-        
-            MIDDLEWARE = (
-                ...
-                'tz_detect.middleware.TimezoneMiddleware',
-            )
-        
         
         Edit the urls.py file
         ---------------------
         
         Add the ``core_main_app`` urls to the Django project as such.
         
         .. code:: python
```

### Comparing `core_main_app-2.3.0/core_main_app.egg-info/SOURCES.txt` & `core_main_app-2.4.0/core_main_app.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -85,18 +85,22 @@
 core_main_app/components/workspace/admin_site.py
 core_main_app/components/workspace/api.py
 core_main_app/components/workspace/models.py
 core_main_app/components/xsl_transformation/__init__.py
 core_main_app/components/xsl_transformation/admin_site.py
 core_main_app/components/xsl_transformation/api.py
 core_main_app/components/xsl_transformation/models.py
+core_main_app/middleware/__init__.py
+core_main_app/middleware/timezone.py
 core_main_app/migrations/0001_initial.py
 core_main_app/migrations/0002_site_update.py
 core_main_app/migrations/0003_psql_full_text.py
 core_main_app/migrations/0004_template_ordering.py
+core_main_app/migrations/0005_template_dependencies.py
+core_main_app/migrations/0006_blob_metadata.py
 core_main_app/migrations/__init__.py
 core_main_app/permissions/__init__.py
 core_main_app/permissions/api.py
 core_main_app/permissions/discover.py
 core_main_app/permissions/rights.py
 core_main_app/permissions/utils.py
 core_main_app/rest/__init__.py
@@ -150,18 +154,20 @@
 core_main_app/static/core_main_app/admin/js/templates/data_migration.js
 core_main_app/static/core_main_app/admin/js/templates/data_migration.raw.js
 core_main_app/static/core_main_app/admin/js/templates/upload/dependencies.js
 core_main_app/static/core_main_app/admin/js/templates/upload/dependencies.raw.js
 core_main_app/static/core_main_app/admin/js/templates/upload/dependency_resolver.js
 core_main_app/static/core_main_app/admin/js/templates_xslt/detail_xslt.js
 core_main_app/static/core_main_app/common/css/XMLTree.css
+core_main_app/static/core_main_app/common/css/bootstrap5.css
 core_main_app/static/core_main_app/common/css/buttons.css
 core_main_app/static/core_main_app/common/css/fields.css
 core_main_app/static/core_main_app/common/css/highlight.css
 core_main_app/static/core_main_app/common/css/loading-spinner.css
+core_main_app/static/core_main_app/common/css/messages.css
 core_main_app/static/core_main_app/common/css/select.css
 core_main_app/static/core_main_app/common/css/share_link.css
 core_main_app/static/core_main_app/common/css/switch.css
 core_main_app/static/core_main_app/common/css/table.css
 core_main_app/static/core_main_app/common/css/word-wrap.css
 core_main_app/static/core_main_app/common/css/template/template_ordering.css
 core_main_app/static/core_main_app/common/css/workspace/table.css
@@ -171,15 +177,15 @@
 core_main_app/static/core_main_app/common/js/backtoprevious.js
 core_main_app/static/core_main_app/common/js/csrf.js
 core_main_app/static/core_main_app/common/js/data_detail.js
 core_main_app/static/core_main_app/common/js/debounce.js
 core_main_app/static/core_main_app/common/js/elementViewport.js
 core_main_app/static/core_main_app/common/js/leave_notice.js
 core_main_app/static/core_main_app/common/js/loading_spinner.js
-core_main_app/static/core_main_app/common/js/notify-styles.js
+core_main_app/static/core_main_app/common/js/messages.js
 core_main_app/static/core_main_app/common/js/modals/add.js
 core_main_app/static/core_main_app/common/js/modals/delete.js
 core_main_app/static/core_main_app/common/js/modals/download.js
 core_main_app/static/core_main_app/common/js/modals/download.raw.js
 core_main_app/static/core_main_app/common/js/modals/edit.js
 core_main_app/static/core_main_app/common/js/modals/error_page_modal.js
 core_main_app/static/core_main_app/common/js/templates/sort.js
@@ -195,15 +201,14 @@
 core_main_app/static/core_main_app/common/js/templates/versions/modals/disable.js
 core_main_app/static/core_main_app/common/js/templates/versions/modals/disable.raw.js
 core_main_app/static/core_main_app/common/js/xslt/list/modals/delete.js
 core_main_app/static/core_main_app/common/js/xslt/list/modals/delete.raw.js
 core_main_app/static/core_main_app/common/js/xslt/list/modals/edit.js
 core_main_app/static/core_main_app/common/js/xslt/list/modals/edit.raw.js
 core_main_app/static/core_main_app/common/xsl/xml2html.xsl
-core_main_app/static/core_main_app/libs/notify.js
 core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.css
 core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.js
 core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.structure.css
 core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.theme.css
 core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_444444_256x240.png
 core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_555555_256x240.png
 core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777620_256x240.png
@@ -211,14 +216,17 @@
 core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_cc0000_256x240.png
 core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_ffffff_256x240.png
 core_main_app/static/core_main_app/libs/jquery/3.5.1/jquery.js
 core_main_app/static/core_main_app/user/css/login.css
 core_main_app/static/core_main_app/user/css/registration.css
 core_main_app/static/core_main_app/user/css/text-editor.css
 core_main_app/static/core_main_app/user/js/sharing_modal.js
+core_main_app/static/core_main_app/user/js/blob/blob_metadata.js
+core_main_app/static/core_main_app/user/js/blob/blob_metadata.raw.js
+core_main_app/static/core_main_app/user/js/blob/detail.js
 core_main_app/static/core_main_app/user/js/data/change_display.js
 core_main_app/static/core_main_app/user/js/data/change_display.raw.js
 core_main_app/static/core_main_app/user/js/data/detail.js
 core_main_app/static/core_main_app/user/js/login/message.js
 core_main_app/static/core_main_app/user/js/login/message.raw.js
 core_main_app/static/core_main_app/user/js/text_editor/data_text_editor.raw.js
 core_main_app/static/core_main_app/user/js/text_editor/template_text_editor.raw.js
@@ -287,20 +295,21 @@
 core_main_app/templates/core_main_app/admin/web_page/web_page.html
 core_main_app/templates/core_main_app/admin/web_page/web_page_unavailable.html
 core_main_app/templates/core_main_app/admin/workspaces/edit_rights.html
 core_main_app/templates/core_main_app/admin/xslt/list.html
 core_main_app/templates/core_main_app/admin/xslt/upload.html
 core_main_app/templates/core_main_app/admin/xslt/list/table.html
 core_main_app/templates/core_main_app/admin/xslt/upload/base.html
+core_main_app/templates/core_main_app/common/blob/tools_blob.html
+core_main_app/templates/core_main_app/common/blob/tools_metadata.html
 core_main_app/templates/core_main_app/common/buttons/add.html
 core_main_app/templates/core_main_app/common/buttons/back_to_previous.html
 core_main_app/templates/core_main_app/common/buttons/delete.html
 core_main_app/templates/core_main_app/common/buttons/edit.html
 core_main_app/templates/core_main_app/common/buttons/go_to.html
-core_main_app/templates/core_main_app/common/buttons/save_ordering.html
 core_main_app/templates/core_main_app/common/commons/error.html
 core_main_app/templates/core_main_app/common/commons/form.html
 core_main_app/templates/core_main_app/common/commons/form_delete.html
 core_main_app/templates/core_main_app/common/commons/upload/form.html
 core_main_app/templates/core_main_app/common/commons/upload/upload.html
 core_main_app/templates/core_main_app/common/data/detail_data.html
 core_main_app/templates/core_main_app/common/data/tools_data.html
@@ -325,14 +334,21 @@
 core_main_app/templates/core_main_app/common/xslt/list.html
 core_main_app/templates/core_main_app/common/xslt/upload.html
 core_main_app/templates/core_main_app/common/xslt/list/table.html
 core_main_app/templates/core_main_app/common/xslt/list/modals/delete.html
 core_main_app/templates/core_main_app/common/xslt/list/modals/edit.html
 core_main_app/templates/core_main_app/common/xslt/upload/base.html
 core_main_app/templates/core_main_app/user/homepage.html
+core_main_app/templates/core_main_app/user/timezone.html
+core_main_app/templates/core_main_app/user/blob/blob_metadata.html
+core_main_app/templates/core_main_app/user/blob/detail.html
+core_main_app/templates/core_main_app/user/blob/list/modals/add_metadata.html
+core_main_app/templates/core_main_app/user/blob/list/modals/add_metadata_form.html
+core_main_app/templates/core_main_app/user/blob/list/modals/file_upload.html
+core_main_app/templates/core_main_app/user/blob/list/modals/file_upload_form.html
 core_main_app/templates/core_main_app/user/data/detail.html
 core_main_app/templates/core_main_app/user/login/main.html
 core_main_app/templates/core_main_app/user/login/saml2_error.html
 core_main_app/templates/core_main_app/user/login/modals/login_message.html
 core_main_app/templates/core_main_app/user/registration/password_reset_complete.html
 core_main_app/templates/core_main_app/user/registration/password_reset_confirm.html
 core_main_app/templates/core_main_app/user/registration/password_reset_done.html
@@ -361,14 +377,15 @@
 core_main_app/templatetags/__init__.py
 core_main_app/templatetags/auth_extras.py
 core_main_app/templatetags/blob_tags.py
 core_main_app/templatetags/dict_key_extras.py
 core_main_app/templatetags/get_attribute.py
 core_main_app/templatetags/include_static.py
 core_main_app/templatetags/json_date.py
+core_main_app/templatetags/parse_date.py
 core_main_app/templatetags/stripjs.py
 core_main_app/templatetags/timestamptags.py
 core_main_app/templatetags/xsl_transform_tag.py
 core_main_app/utils/__init__.py
 core_main_app/utils/blob_downloader.py
 core_main_app/utils/boolean.py
 core_main_app/utils/checksum.py
@@ -492,14 +509,15 @@
 tests/components/group/fixtures/fixtures.py
 tests/components/group/fixtures/tests_int.py
 tests/components/lock/__init__.py
 tests/components/lock/tests_int.py
 tests/components/lock/tests_unit.py
 tests/components/mongo_data/__init__.py
 tests/components/mongo_data/tests_int_access_control.py
+tests/components/mongo_data/tests_unit.py
 tests/components/template/__init__.py
 tests/components/template/tests_int_access_control.py
 tests/components/template/tests_unit.py
 tests/components/template/fixtures/__init__.py
 tests/components/template/fixtures/fixtures.py
 tests/components/template_version_manager/__init__.py
 tests/components/template_version_manager/tests_int_access_control.py
@@ -526,14 +544,16 @@
 tests/components/workspace/__init__.py
 tests/components/workspace/tests_int.py
 tests/components/workspace/fixtures/__init__.py
 tests/components/workspace/fixtures/fixtures.py
 tests/components/workspace/fixtures/tests_int.py
 tests/components/xsl_transformation/__init__.py
 tests/components/xsl_transformation/tests_unit.py
+tests/middleware/__init__.py
+tests/middleware/tests_unit.py
 tests/rest/__init__.py
 tests/rest/tests_views.py
 tests/rest/blob/__init__.py
 tests/rest/blob/tests_int.py
 tests/rest/blob/tests_permissions.py
 tests/rest/blob/tests_unit.py
 tests/rest/data/__init__.py
@@ -565,15 +585,17 @@
 tests/rest/xsl_transformation/tests_permission.py
 tests/rest/xsl_transformation/tests_unit.py
 tests/rest/xsl_transformation/fixtures/__init__.py
 tests/rest/xsl_transformation/fixtures/fixtures.py
 tests/system/__init__.py
 tests/system/test_unit.py
 tests/templatetags/__init__.py
+tests/templatetags/test_blob_tags.py
 tests/templatetags/test_get_attribute.py
+tests/templatetags/test_parse_date.py
 tests/utils/__init__.py
 tests/utils/test_unit_apps.py
 tests/utils/test_unit_urls.py
 tests/utils/tests_int_blob_downloader.py
 tests/utils/tests_int_file.py
 tests/utils/tests_unit_admin_site.py
 tests/utils/tests_unit_boolean.py
@@ -592,8 +614,11 @@
 tests/utils/validation/__init__.py
 tests/utils/validation/tests_unit_validation.py
 tests/utils/xsd_flattener/__init__.py
 tests/utils/xsd_flattener/tests_unit.py
 tests/views/__init__.py
 tests/views/fixtures.py
 tests/views/test_unit.py
-tests/views/tests_int_access_control.py
+tests/views/tests_int_access_control.py
+tests/views/tests_permissions.py
+tests/views/forms/__init__.py
+tests/views/forms/test_unit.py
```

### Comparing `core_main_app-2.3.0/docs/conf.py` & `core_main_app-2.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/setup.py` & `core_main_app-2.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_main_app",
-    version="2.3.0",
+    version="2.4.0",
     description="Main functionalities for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_main_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_main_app-2.3.0/tests/access_control/tests_access_control.py` & `core_main_app-2.4.0/tests/access_control/tests_access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/commons/tests_validators.py` & `core_main_app-2.4.0/tests/commons/tests_validators.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/blob/fixtures/fixtures.py` & `core_main_app-2.4.0/tests/components/blob/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/blob/tests_int.py` & `core_main_app-2.4.0/tests/components/blob/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/data/fixtures/fixtures.py` & `core_main_app-2.4.0/tests/components/data/fixtures/fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ Fixtures files for Data
 """
 from django.core.files.uploadedfile import SimpleUploadedFile
 
+from core_main_app.components.blob.models import Blob
 from core_main_app.components.data.models import Data
 from core_main_app.components.template.models import Template
 from core_main_app.components.workspace import api as workspace_api
 from core_main_app.components.workspace.models import Workspace
 from core_main_app.components.xsl_transformation.models import (
     XslTransformation,
 )
@@ -835,7 +836,171 @@
             filename="xsl_transformation.xsl",
             file=SimpleUploadedFile(
                 "xsl_transformation.xsl", content=content.encode("utf-8")
             ),
         )
 
         self.xsl_transformation.save()
+
+
+class AccessControlBlobWithMetadataFixture(FixtureInterface):
+    """Access Control Blob with Metadata Fixture
+    blob1 (user: 1, wksp: None)
+        |-data1 (user: 1, wksp: None)
+
+    blob2 (user: 2, wksp: 1)
+        |-data2 (user: 2, wksp: 1)
+
+    blob3 (user: 3, wksp: 1)
+        |-data31 (user: 3, wksp: 1)
+        |-data32 (user: 3, wksp: None)
+
+    data4 (user: 1, wksp: None)
+    """
+
+    template = None
+    workspace_1 = None
+    data_collection = None
+    blob_collection = None
+
+    data_1 = None
+    data_2 = None
+    data_31 = None
+    data_32 = None
+    data_4 = None
+
+    blob_1 = None
+    blob_2 = None
+    blob_3 = None
+
+    def insert_data(self):
+        """Insert a set of Data.
+
+        Returns:
+
+        """
+        # Make a connexion with a mock database
+        self.generate_template()
+        self.generate_workspace()
+        self.generate_blob_collection()
+        self.generate_data_collection()
+
+    def generate_data_collection(self):
+        """Generate a Data collection.
+
+        Returns:
+
+        """
+
+        xml_content = "<root><element>value2</element></root>"
+        content = {"root": {"element": "value2"}}
+
+        self.data_1 = Data(
+            template=self.template,
+            title="Data 1",
+            user_id="1",
+            _blob=self.blob_1,
+            xml_content="<root></root>",
+        )
+        self.data_1.save()
+        self.data_2 = Data(
+            template=self.template,
+            title="Data 2",
+            user_id="2",
+            _blob=self.blob_2,
+            workspace=self.workspace_1,
+            xml_content="<root></root>",
+        )
+        self.data_2.save()
+        self.data_31 = Data(
+            template=self.template,
+            title="Data 3_1",
+            user_id="3",
+            workspace=self.workspace_1,
+            xml_content=xml_content,
+            dict_content=content,
+            _blob=self.blob_3,
+        )
+        self.data_31.save()
+        self.data_32 = Data(
+            template=self.template,
+            title="Data 3_2",
+            user_id="3",
+            xml_content="<root></root>",
+            _blob=self.blob_3,
+        )
+        self.data_32.save()
+        self.data_4 = Data(
+            template=self.template,
+            title="Data 4",
+            user_id="1",
+            xml_content="<root></root>",
+        )
+        self.data_4.save()
+
+        self.data_collection = [
+            self.data_1,
+            self.data_2,
+            self.data_31,
+            self.data_32,
+            self.data_4,
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
+        self.template.content = xsd
+        self.template.hash = ""
+        self.template.filename = "filename"
+        self.template.save()
+
+    def generate_workspace(self):
+        """Generate the workspaces.
+
+        Returns:
+
+        """
+        self.workspace_1 = Workspace(
+            title="Workspace 1", owner="1", read_perm_id="1", write_perm_id="1"
+        )
+        self.workspace_1.save()
+
+    def generate_blob_collection(self):
+        """Generate a Blob collection.
+
+        Returns:
+
+            user 1 -> blob1, blob2
+            user 2 -> blob3
+
+        """
+
+        self.blob_1 = Blob(
+            filename="blob1",
+            user_id="1",
+            blob=SimpleUploadedFile("blob.txt", b"blob"),
+        )
+        self.blob_1.save()
+        self.blob_2 = Blob(
+            filename="blob2",
+            user_id="2",
+            workspace=self.workspace_1,
+            blob=SimpleUploadedFile("blob.txt", b"blob"),
+        )
+        self.blob_2.save()
+        self.blob_3 = Blob(
+            filename="blob3",
+            user_id="3",
+            workspace=self.workspace_1,
+            blob=SimpleUploadedFile("blob.txt", b"blob"),
+        )
+        self.blob_3.save()
+
+        self.blob_collection = [self.blob_1, self.blob_2, self.blob_3]
```

### Comparing `core_main_app-2.3.0/tests/components/data/tests_int.py` & `core_main_app-2.4.0/tests/components/data/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/data/tests_int_access_control.py` & `core_main_app-2.4.0/tests/components/data/tests_int_access_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from django.test import override_settings
 from tests.components.data.fixtures.fixtures import (
     AccessControlDataFixture,
     AccessControlDataFixture2,
     AccessControlDataFullTextSearchFixture,
     AccessControlDataNumericFixture,
     AccessControlDataNoneFixture,
+    AccessControlBlobWithMetadataFixture,
 )
 
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.commons.exceptions import QueryError
 from core_main_app.components.data import api as data_api
 from core_main_app.components.data.models import Data
 from core_main_app.utils.integration_tests.integration_base_test_case import (
@@ -24,14 +25,15 @@
 from core_main_app.utils.tests_tools.RequestMock import create_mock_request
 
 fixture_data = AccessControlDataFixture()
 fixture_data2 = AccessControlDataFixture2()
 fixture_data_full_text = AccessControlDataFullTextSearchFixture()
 fixture_data_numeric = AccessControlDataNumericFixture()
 fixture_data_none = AccessControlDataNoneFixture()
+fixture_blob_metadata = AccessControlBlobWithMetadataFixture()
 
 
 class TestDataGetById(IntegrationBaseTestCase):
     """TestDataGetById"""
 
     fixture = fixture_data
 
@@ -2479,14 +2481,117 @@
         for operator in ["$lt", "$lte", "$gt", "$gte"]:
             for value in [0, 1, 1.2]:
                 data_api.execute_json_query(
                     {"dict_content.root.element": {operator: value}}, mock_user
                 )
 
 
+class TestDataBlob(IntegrationBaseTestCase):
+    """TestDataBlob"""
+
+    fixture = fixture_blob_metadata
+
+    def test_data_blob_as_anonymous_raises_acl_error(self):
+        """test_data_blob_as_anonymous_raises_acl_error
+
+        Args:
+
+        Returns:
+
+        """
+        data = self.fixture.data_1
+        mock_user = create_mock_user(2, is_anonymous=True)
+        with self.assertRaises(AccessControlError):
+            data.blob(mock_user)
+
+    def test_data_blob_as_superuser_returns_blob(
+        self,
+    ):
+        """test_data_blob_as_superuser_returns_blob
+
+        Args:
+
+        Returns:
+
+        """
+        data = self.fixture.data_1
+        mock_user = create_mock_user(5, is_superuser=True)
+        blob = data.blob(mock_user)
+        self.assertEqual(blob, self.fixture.blob_1)
+
+    def test_data_blob_as_owner_returns_blob(self):
+        """test_data_blob_as_owner_returns_blob
+
+        Args:
+
+        Returns:
+
+        """
+        data = self.fixture.data_1
+        mock_user = create_mock_user(1)
+        blob = data.blob(mock_user)
+        self.assertEqual(blob, self.fixture.blob_1)
+
+    @patch(
+        "core_main_app.components.workspace.api.get_all_workspaces_with_read_access_by_user"
+    )
+    def test_data_private_blob_as_other_user_raises_acl_error(
+        self, get_all_workspaces_with_read_access_by_user
+    ):
+        """test_data_private_blob_as_other_user_raises_acl_error
+
+        Args:
+            get_all_workspaces_with_read_access_by_user:
+
+        Returns:
+
+        """
+        data = self.fixture.data_1
+        mock_user = create_mock_user(2)
+        get_all_workspaces_with_read_access_by_user.return_value = []
+        with self.assertRaises(AccessControlError):
+            data.blob(mock_user)
+
+    @patch(
+        "core_main_app.components.workspace.api.get_all_workspaces_with_read_access_by_user"
+    )
+    def test_data_other_user_blob_in_workspace_with_access_returns_blob(
+        self, get_all_workspaces_with_read_access_by_user
+    ):
+        """test_data_other_user_blob_in_workspace_with_access_returns_blob
+
+        Returns:
+
+        """
+        data = self.fixture.data_2
+        mock_user = create_mock_user(1)
+        get_all_workspaces_with_read_access_by_user.return_value = [
+            self.fixture.workspace_1
+        ]
+        blob = data.blob(mock_user)
+        self.assertEqual(blob, self.fixture.blob_2)
+
+    @patch(
+        "core_main_app.components.workspace.api.get_all_workspaces_with_read_access_by_user"
+    )
+    def test_data_other_user_blob_in_workspace_without_access_raises_error(
+        self, get_all_workspaces_with_read_access_by_user
+    ):
+        """test_data_other_user_blob_in_workspace_without_access_raises_error
+
+        Returns:
+
+        """
+        data = self.fixture.data_2
+        mock_user = create_mock_user(1)
+        get_all_workspaces_with_read_access_by_user.return_value = []
+        with self.assertRaises(AccessControlError):
+            data.blob(mock_user)
+
+
 def _create_data(user_id, workspace):
     """create data
 
     Args:
         user_id:
         workspace:
```

### Comparing `core_main_app-2.3.0/tests/components/data/tests_int_ordering.py` & `core_main_app-2.4.0/tests/components/data/tests_int_ordering.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/data/tests_unit.py` & `core_main_app-2.4.0/tests/components/data/tests_unit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """ Unit Test Data
 """
 from collections import OrderedDict
 from unittest.case import TestCase
 from unittest.mock import patch
 
+from django.core.files.uploadedfile import SimpleUploadedFile
+
 from core_main_app.commons import exceptions
+from core_main_app.components.blob.models import Blob
 from core_main_app.components.data import api as data_api
 from core_main_app.components.data.models import Data
 from core_main_app.components.template.models import Template
 from core_main_app.utils.datetime import datetime_now, datetime_timedelta
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import create_mock_request
 
@@ -823,14 +826,61 @@
         data.title = "test"
         data_api.upsert(data, mock_request)
         # Assert
         self.assertIsNotNone(data.creation_date)
         self.assertEqual(data.creation_date, original_date)
 
 
+class TestDataBlob(TestCase):
+    """TestDataBlob"""
+
+    def test_data_blob_none_return_none(
+        self,
+    ):
+        """test_data_blob_none_return_none
+
+        Returns:
+
+        """
+        # Arrange
+        data = _create_data(
+            _get_template(),
+            user_id="2",
+            title="new_title",
+            content="<tag></tag>",
+        )
+        user = create_mock_user("2")
+        # Act
+        blob = data.blob(user=user)
+        # Assert
+        self.assertIsNone(blob)
+
+    def test_data_blob_return_blob(
+        self,
+    ):
+        """test_data_blob_return_blob
+
+        Returns:
+
+        """
+        # Arrange
+        data = _create_data(
+            template=_get_template(),
+            user_id="2",
+            title="new_title",
+            content="<tag></tag>",
+            blob=_create_blob(user_id="2"),
+        )
+        user = create_mock_user("2")
+        # Act
+        blob = data.blob(user=user)
+        # Assert
+        self.assertIsNotNone(blob)
+
+
 def _get_template():
     """_get_template
 
     Returns:
 
     """
     template = Template()
@@ -839,23 +889,42 @@
         '<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema">'
         '<xs:element name="tag"></xs:element></xs:schema>'
     )
     template.content = xsd
     return template
 
 
-def _create_data(template, user_id, title, content, data_id=None):
+def _create_data(template, user_id, title, content, data_id=None, blob=None):
     """_create_data
 
     Args:
         template:
         user_id:
         title:
         content:
         data_id:
+        blob:
 
     Returns:
 
     """
-    data = Data(template=template, user_id=user_id, title=title, id=data_id)
+    data = Data(
+        template=template, user_id=user_id, title=title, id=data_id, _blob=blob
+    )
     data.xml_content = content
     return data
+
+
+def _create_blob(user_id, filename="test", content=b"test"):
+    """_create_blob
+
+    Returns:
+
+    """
+    return Blob(
+        filename=filename,
+        user_id=user_id,
+        blob=SimpleUploadedFile(
+            name=filename,
+            content=content,
+        ),
+    )
```

### Comparing `core_main_app-2.3.0/tests/components/group/fixtures/fixtures.py` & `core_main_app-2.4.0/tests/components/group/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/group/fixtures/tests_int.py` & `core_main_app-2.4.0/tests/components/group/fixtures/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/group/tests_int.py` & `core_main_app-2.4.0/tests/components/group/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/lock/tests_int.py` & `core_main_app-2.4.0/tests/components/lock/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/lock/tests_unit.py` & `core_main_app-2.4.0/tests/components/lock/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/mongo_data/tests_int_access_control.py` & `core_main_app-2.4.0/tests/components/mongo_data/tests_int_access_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -2106,7 +2106,175 @@
 
         Returns:
 
         """
         mock_user = create_mock_user(None, is_anonymous=True)
         with self.assertRaises(AccessControlError):
             mongo_data_api.aggregate({}, user=mock_user)
+
+
+class TestDataBlob(MongoDBIntegrationBaseTestCase):
+    """TestDataBlob"""
+
+    @override_settings(MONGODB_INDEXING=True)
+    @override_settings(MONGODB_ASYNC_SAVE=False)
+    def setUp(self):
+        """Insert needed data.
+
+        Returns:
+
+        """
+        from core_main_app.components.mongo.models import (  # noqa: keep import to init signals
+            MongoData,
+        )
+        from tests.components.data.fixtures.fixtures import (
+            AccessControlBlobWithMetadataFixture,
+        )
+
+        # Mongo indexing is not initialized by default
+        init_mongo_indexing()
+
+        # fixture needs to initialized with settings.MONGODB_INDEXING=True otherwise MongoData does not exist
+        self.fixture = AccessControlBlobWithMetadataFixture()
+        self.fixture.insert_data()
+
+    @override_settings(MONGODB_INDEXING=True)
+    @override_settings(MONGODB_ASYNC_SAVE=False)
+    @tag("mongodb")
+    def test_data_blob_as_owner_returns_blob(
+        self,
+    ):
+        """test_data_blob_as_owner_returns_blob
+
+        Args:
+            :
+
+        Returns:
+
+        """
+        from core_main_app.components.mongo.models import (
+            MongoData,
+        )
+
+        mock_user = create_mock_user("1")
+        mongo_data_1 = MongoData.objects.get(data_id=self.fixture.data_1.id)
+        blob = mongo_data_1.blob(mock_user)
+        self.assertEqual(blob, self.fixture.blob_1)
+
+    @override_settings(MONGODB_INDEXING=True)
+    @override_settings(MONGODB_ASYNC_SAVE=False)
+    @tag("mongodb")
+    def test_data_blob_as_anonymous_raises_acl_error(self):
+        """test_data_blob_as_anonymous_raises_acl_error
+
+        Args:
+
+        Returns:
+
+        """
+        from core_main_app.components.mongo.models import (
+            MongoData,
+        )
+
+        mock_user = create_mock_user("2", is_anonymous=True)
+        mongo_data_1 = MongoData.objects.get(data_id=self.fixture.data_1.id)
+        with self.assertRaises(AccessControlError):
+            mongo_data_1.blob(mock_user)
+
+    @override_settings(MONGODB_INDEXING=True)
+    @override_settings(MONGODB_ASYNC_SAVE=False)
+    @tag("mongodb")
+    def test_data_blob_as_superuser_returns_blob(
+        self,
+    ):
+        """test_data_blob_as_superuser_returns_blob
+
+        Args:
+
+        Returns:
+
+        """
+        from core_main_app.components.mongo.models import (
+            MongoData,
+        )
+
+        mock_user = create_mock_user("2", is_superuser=True)
+        mongo_data_1 = MongoData.objects.get(data_id=self.fixture.data_1.id)
+        blob = mongo_data_1.blob(mock_user)
+        self.assertEqual(blob, self.fixture.blob_1)
+
+    @override_settings(MONGODB_INDEXING=True)
+    @override_settings(MONGODB_ASYNC_SAVE=False)
+    @tag("mongodb")
+    @patch(
+        "core_main_app.components.workspace.api.get_all_workspaces_with_read_access_by_user"
+    )
+    def test_data_private_blob_as_other_user_raises_acl_error(
+        self, get_all_workspaces_with_read_access_by_user
+    ):
+        """test_data_private_blob_as_other_user_raises_acl_error
+
+        Args:
+            get_all_workspaces_with_read_access_by_user:
+
+        Returns:
+
+        """
+        from core_main_app.components.mongo.models import (
+            MongoData,
+        )
+
+        data = MongoData.objects.get(data_id=self.fixture.data_1.id)
+        mock_user = create_mock_user(2)
+        get_all_workspaces_with_read_access_by_user.return_value = []
+        with self.assertRaises(AccessControlError):
+            data.blob(mock_user)
+
+    @override_settings(MONGODB_INDEXING=True)
+    @override_settings(MONGODB_ASYNC_SAVE=False)
+    @tag("mongodb")
+    @patch(
+        "core_main_app.components.workspace.api.get_all_workspaces_with_read_access_by_user"
+    )
+    def test_data_other_user_blob_in_workspace_with_access_returns_blob(
+        self, get_all_workspaces_with_read_access_by_user
+    ):
+        """test_data_other_user_blob_in_workspace_with_access_returns_blob
+
+        Returns:
+
+        """
+        from core_main_app.components.mongo.models import (
+            MongoData,
+        )
+
+        data = MongoData.objects.get(data_id=self.fixture.data_2.id)
+        mock_user = create_mock_user(1)
+        get_all_workspaces_with_read_access_by_user.return_value = [
+            self.fixture.workspace_1
+        ]
+        blob = data.blob(mock_user)
+        self.assertEqual(blob, self.fixture.blob_2)
+
+    @override_settings(MONGODB_INDEXING=True)
+    @override_settings(MONGODB_ASYNC_SAVE=False)
+    @tag("mongodb")
+    @patch(
+        "core_main_app.components.workspace.api.get_all_workspaces_with_read_access_by_user"
+    )
+    def test_data_other_user_blob_in_workspace_without_access_raises_error(
+        self, get_all_workspaces_with_read_access_by_user
+    ):
+        """test_data_other_user_blob_in_workspace_without_access_raises_error
+
+        Returns:
+
+        """
+        from core_main_app.components.mongo.models import (
+            MongoData,
+        )
+
+        data = MongoData.objects.get(data_id=self.fixture.data_2.id)
+        mock_user = create_mock_user(1)
+        get_all_workspaces_with_read_access_by_user.return_value = []
+        with self.assertRaises(AccessControlError):
+            data.blob(mock_user)
```

### Comparing `core_main_app-2.3.0/tests/components/template/fixtures/fixtures.py` & `core_main_app-2.4.0/tests/components/template/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/template/tests_int_access_control.py` & `core_main_app-2.4.0/tests/components/template/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/template/tests_unit.py` & `core_main_app-2.4.0/tests/components/template/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/template_version_manager/fixtures/fixtures.py` & `core_main_app-2.4.0/tests/components/template_version_manager/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/template_version_manager/tests_int_access_control.py` & `core_main_app-2.4.0/tests/components/template_version_manager/tests_int_access_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1233,159 +1233,112 @@
 
         Returns:
 
         """
         self.anonymous_user = create_mock_user(user_id=None, is_anonymous=True)
         self.user1 = create_mock_user(user_id="1")
         self.user2 = create_mock_user(user_id="2")
-        self.staff_user1 = create_mock_user(user_id="1", is_staff=True)
         self.superuser1 = create_mock_user(user_id="1", is_superuser=True)
         self.fixture.insert_data()
 
     def test_update_user_templates_ordering_as_anonymous_raises_access_control_error(
         self,
     ):
         """test update user templates ordering as anonymous raises acl error
 
         Returns:x
 
         """
 
         # Arrange
-        list_templates_ordering = [self.fixture.tvm2, self.fixture.tvm1]
+        list_templates_ordering = [self.fixture.tvm2.id, self.fixture.tvm1.id]
 
         # Act # Assert
         with self.assertRaises(AccessControlError):
-            template_vm_api.update_templates_ordering(
-                list_templates_ordering, user=self.anonymous_user
+            template_vm_api._update_template_version_manager_ordering(
+                list_templates_ordering,
+                create_mock_request(user=self.anonymous_user),
             )
 
     def test_update_global_templates_ordering_as_anonymous_raises_access_control_error(
         self,
     ):
         """test update global templates ordering as anonymous raises access control error
 
         Returns:
 
         """
         # Arrange
         list_templates_ordering = [
-            self.fixture.global_tvm2,
-            self.fixture.global_tvm1,
+            self.fixture.global_tvm2.id,
+            self.fixture.global_tvm1.id,
         ]
         # Act # Assert
         with self.assertRaises(AccessControlError):
-            template_vm_api.update_templates_ordering(
-                list_templates_ordering, user=self.anonymous_user
+            template_vm_api._update_template_version_manager_ordering(
+                list_templates_ordering,
+                create_mock_request(user=self.anonymous_user),
             )
 
     def test_update_own_templates_ordering_as_user_saves(self):
         """test update own templates ordering as user saves
 
         Returns:
 
         """
         # Arrange
-        list_templates_ordering = [self.fixture.tvm2, self.fixture.tvm1]
+        list_templates_ordering = [self.fixture.tvm2.id, self.fixture.tvm1.id]
         # Act
-        template_vm_api.update_templates_ordering(
-            list_templates_ordering, user=self.user1
+        template_vm_api._update_template_version_manager_ordering(
+            list_templates_ordering, create_mock_request(user=self.user1)
         )
 
     def test_update_other_users_template_ordering_as_user_raises_access_control_error(
         self,
     ):
         """test update other users template ordering as user raises access control error
 
         Returns:
 
         """
         # Arrange
-        list_templates_ordering = [self.fixture.tvm2, self.fixture.tvm1]
-        # Act # Assert
-        with self.assertRaises(AccessControlError):
-            template_vm_api.update_templates_ordering(
-                list_templates_ordering, user=self.user2
-            )
-
-    def test_update_global_templates_ordering_as_user_raises_access_control_error(
-        self,
-    ):
-        """test update global templates ordering as user raises access control error
-
-        Returns:
-
-        """
-        # Arrange
-        list_templates_ordering = [
-            self.fixture.global_tvm2,
-            self.fixture.global_tvm1,
-        ]
+        list_templates_ordering = [self.fixture.tvm2.id, self.fixture.tvm1.id]
         # Act # Assert
         with self.assertRaises(AccessControlError):
-            template_vm_api.update_templates_ordering(
-                list_templates_ordering, user=self.user1
+            template_vm_api._update_template_version_manager_ordering(
+                list_templates_ordering, create_mock_request(user=self.user2)
             )
 
-    def test_update_other_users_template_ordering_as_staff_saves(self):
-        """test update other users template ordering as staff saves
-
-        Returns:
-
-        """
-        # Arrange
-        list_templates_ordering = [self.fixture.tvm2, self.fixture.tvm1]
-        # Act
-        template_vm_api.update_templates_ordering(
-            list_templates_ordering, user=self.staff_user1
-        )
-
-    def test_update_global_template_ordering_as_staff_saves(self):
-        """test update other users template ordering as staff saves
-
-        Returns:
-
-        """
-        # Arrange
-        list_templates_ordering = [
-            self.fixture.global_tvm2,
-            self.fixture.global_tvm1,
-        ]
-        # Act
-        template_vm_api.update_templates_ordering(
-            list_templates_ordering, user=self.staff_user1
-        )
-
     def test_update_other_users_template_ordering_as_superuser_saves(self):
         """test update other users template ordering as superuser saves
 
         Returns:
 
         """
         # Arrange
-        list_templates_ordering = [self.fixture.tvm2, self.fixture.tvm1]
+        list_templates_ordering = [self.fixture.tvm2.id, self.fixture.tvm1.id]
         # Act
-        template_vm_api.update_templates_ordering(
-            list_templates_ordering, user=self.superuser1
+        template_vm_api._update_template_version_manager_ordering(
+            list_templates_ordering, create_mock_request(user=self.superuser1)
         )
 
     def test_update_global_template_ordering_as_superuser_saves(self):
         """test update other users template ordering as superuser saves
 
         Returns:
 
         """
         # Arrange
         list_templates_ordering = [
-            self.fixture.global_tvm2,
-            self.fixture.global_tvm1,
+            self.fixture.global_tvm2.id,
+            self.fixture.global_tvm1.id,
         ]
         # Act
-        template_vm_api.update_templates_ordering(
-            list_templates_ordering, user=self.superuser1
+        template_vm_api._update_template_version_manager_ordering(
+            list_templates_ordering, create_mock_request(user=self.superuser1)
         )
 
 
 class TestAccessControlCanWriteList(IntegrationBaseTestCase):
     """Test Access Control Can Write List"""
 
     fixture = fixture_template_vm_ordering
@@ -1405,250 +1358,283 @@
 
     def test_access_control_can_write_list_as_anonymous_raises_access_control_error(
         self,
     ):
         """test_access_control_can_write_list_as_anonymous_raises_access_control_error"""
 
         # Arrange
-        template_vm_list = [self.fixture.tvm2, self.fixture.tvm1]
+        template_vm_list = [self.fixture.tvm2.id, self.fixture.tvm1.id]
 
         # Act # Assert
         with self.assertRaises(AccessControlError):
             access_control.can_write_list(
-                template_vm_api.update_templates_ordering,
+                template_vm_api._update_template_version_manager_ordering,
                 template_vm_list,
-                self.anonymous_user,
+                create_mock_request(user=self.anonymous_user),
             )
 
     def test_access_control_can_write_list_as_owner_returns_function(self):
         """test_access_control_can_write_list_as_owner_returns_function"""
 
         # Arrange
-        template_vm_list = [self.fixture.tvm2, self.fixture.tvm1]
+        template_vm_list = [self.fixture.tvm2.id, self.fixture.tvm1.id]
 
         # Act
         access_control.can_write_list(
-            template_vm_api.update_templates_ordering,
+            template_vm_api._update_template_version_manager_ordering,
             template_vm_list,
-            self.user1,
+            create_mock_request(user=self.user1),
         )
 
     def test_access_control_can_write_list_user_templates_as_user_raises_access_control_error(
         self,
     ):
         """test_access_control_can_write_list_user_templates_as_user_raises_access_control_error"""
         # Arrange
-        template_vm_list = [self.fixture.tvm2, self.fixture.tvm1]
+        template_vm_list = [self.fixture.tvm2.id, self.fixture.tvm1.id]
 
         # Act # Assert
         with self.assertRaises(AccessControlError):
             access_control.can_write_list(
-                template_vm_api.update_templates_ordering,
+                template_vm_api._update_template_version_manager_ordering,
                 template_vm_list,
-                self.user2,
+                create_mock_request(user=self.user2),
             )
 
     def test_access_control_can_write_list_global_templates_as_user_raises_access_control_error(
         self,
     ):
         """test_access_control_can_write_list_global_templates_as_user_raises_access_control_error"""
         # Arrange
-        template_vm_list = [self.fixture.global_tvm2, self.fixture.global_tvm1]
+        template_vm_list = [
+            self.fixture.global_tvm2.id,
+            self.fixture.global_tvm1.id,
+        ]
 
         # Act # Assert
         with self.assertRaises(AccessControlError):
             access_control.can_write_list(
-                template_vm_api.update_templates_ordering,
+                template_vm_api._update_template_version_manager_ordering,
                 template_vm_list,
-                self.user2,
+                create_mock_request(user=self.user2),
             )
 
     def test_access_control_can_write_list_user_templates_as_staff_raises_access_control_error(
         self,
     ):
         """test_access_control_can_write_list_user_templates_as_staff_raises_access_control_error"""
 
         # Arrange
-        template_vm_list = [self.fixture.tvm2, self.fixture.tvm1]
+        template_vm_list = [self.fixture.tvm2.id, self.fixture.tvm1.id]
 
         # Act
         with self.assertRaises(AccessControlError):
             access_control.can_write_list(
-                template_vm_api.update_templates_ordering,
+                template_vm_api._update_template_version_manager_ordering,
                 template_vm_list,
-                self.staff_user1,
+                create_mock_request(user=self.staff_user1),
             )
 
     def test_access_control_can_write_list_global_templates_as_staff_returns_function(
         self,
     ):
         """test_access_control_can_write_list_global_templates_as_staff_returns_functiong"""
 
         # Arrange
-        template_vm_list = [self.fixture.global_tvm1, self.fixture.global_tvm2]
+        template_vm_list = [
+            self.fixture.global_tvm1.id,
+            self.fixture.global_tvm2.id,
+        ]
 
         # Act
         access_control.can_write_list(
-            template_vm_api.update_templates_ordering,
+            template_vm_api._update_template_version_manager_ordering,
             template_vm_list,
-            self.staff_user1,
+            create_mock_request(user=self.staff_user1),
         )
 
     def test_access_control_can_write_list_as_superuser_returns_function(self):
         """test_access_control_can_write_list_as_superuser_returns_function"""
 
         # Arrange
-        template_vm_list = [self.fixture.global_tvm2, self.fixture.tvm1]
+        template_vm_list = [self.fixture.global_tvm2.id, self.fixture.tvm1.id]
 
         # Act
         access_control.can_write_list(
-            template_vm_api.update_templates_ordering,
+            template_vm_api._update_template_version_manager_ordering,
             template_vm_list,
-            self.superuser1,
+            create_mock_request(user=self.superuser1),
         )
 
 
-class TestTemplateVersionManagerSortByIdList(IntegrationBaseTestCase):
-    """Test Template Version Manager Sort By Id List"""
+class TestUpdateUserTemplateOrdering(IntegrationBaseTestCase):
+    """Test Update User Template Ordering"""
 
     fixture = fixture_template_vm_ordering
 
     def setUp(self):
         """setUp
 
         Returns:
 
         """
         self.anonymous_user = create_mock_user(user_id=None, is_anonymous=True)
         self.user1 = create_mock_user(user_id="1")
         self.user2 = create_mock_user(user_id="2")
-        self.staff_user1 = create_mock_user(user_id="1", is_staff=True)
-        self.superuser1 = create_mock_user(user_id="1", is_superuser=True)
+        self.superuser1 = create_mock_user(user_id="3", is_superuser=True)
         self.fixture.insert_data()
 
-    def test_sort_by_id_list_user_templates_as_anonymous_raises_access_control_error(
+    def test_update_user_template_ordering_as_owner_updates_templates(
         self,
     ):
-        """test sort by id list user templates as anonymous raises access control error
+        """test_update_user_template_ordering_as_owner_updates_templates
 
-        Returns:x
+        Returns:
 
         """
+        # Arrange
+        template_vm_list = [self.fixture.tvm1.id]
 
+        template_vm_api.update_user_template_ordering(
+            template_vm_list, create_mock_request(user=self.user1)
+        )
+
+    def test_update_user_template_ordering_as_user_raises_acl_error(
+        self,
+    ):
+        """test_update_user_template_ordering_as_user_raises_acl_error
+
+        Returns:
+
+        """
         # Arrange
-        list_templates_ordering = [self.fixture.tvm2.id, self.fixture.tvm1.id]
+        list_templates_ordering = [self.fixture.tvm2.id]
 
         # Act # Assert
         with self.assertRaises(AccessControlError):
-            template_vm_api.sort_by_id_list(
-                list_templates_ordering,
-                create_mock_request(user=self.anonymous_user),
+            template_vm_api.update_user_template_ordering(
+                list_templates_ordering, create_mock_request(user=self.user2)
             )
 
-    def test_sort_by_id_list_global_templates_as_anonymous_raises_access_control_error(
+    def test_update_user_template_ordering_as_anonymous_raises_acl_error(
         self,
     ):
-        """test sort by id list global templates as anonymous raises access control error
+        """test_update_user_template_ordering_as_anonymous_raises_acl_error
 
         Returns:
 
         """
         # Arrange
-        list_templates_ordering = [
-            self.fixture.global_tvm2.id,
-            self.fixture.global_tvm1.id,
-        ]
+        list_templates_ordering = [self.fixture.tvm2.id]
+
         # Act # Assert
         with self.assertRaises(AccessControlError):
-            template_vm_api.sort_by_id_list(
+            template_vm_api.update_user_template_ordering(
                 list_templates_ordering,
                 create_mock_request(user=self.anonymous_user),
             )
 
-    def test_sort_by_id_list_own_templates_as_user_returns_templates(self):
-        """test sort by id list own templates as user returns templates
+    def test_update_user_template_ordering_as_superuser_raises_acl_error(
+        self,
+    ):
+        """test_update_user_template_ordering_as_superuser_raises_acl_error
 
         Returns:
 
         """
         # Arrange
-        list_templates_ordering = [self.fixture.tvm2.id, self.fixture.tvm1.id]
-        # Act
-        result = template_vm_api.sort_by_id_list(
-            list_templates_ordering, create_mock_request(user=self.user1)
-        )
+        list_templates_ordering = [self.fixture.tvm2.id]
+
+        # Act # Assert
+        with self.assertRaises(AccessControlError):
+            template_vm_api.update_user_template_ordering(
+                list_templates_ordering,
+                create_mock_request(user=self.superuser1),
+            )
 
-        self.assertEqual(len(result), 2)
 
-    def test_sort_by_id_list_others_templates_raises_access_control_error(
+class TestUpdateGlobalTemplateOrdering(IntegrationBaseTestCase):
+    "Test Update Global Template Ordering"
+
+    fixture = fixture_template_vm_ordering
+
+    def setUp(self):
+        """setUp
+
+        Returns:
+
+        """
+        self.anonymous_user = create_mock_user(user_id=None, is_anonymous=True)
+        self.user1 = create_mock_user(user_id="1")
+        self.superuser1 = create_mock_user(
+            user_id="3", is_superuser=True, is_staff=True
+        )
+        self.fixture.insert_data()
+
+    def test_update_global_template_ordering_as_superuser_updates_templates(
         self,
     ):
-        """test sort by id list others templates raises access control error
+        """test_update_global_template_ordering_as_superuser_updates_templates
 
         Returns:
 
         """
         # Arrange
-        list_templates_ordering = [self.fixture.tvm2.id, self.fixture.tvm1.id]
-        # Act # Assert
-        with self.assertRaises(AccessControlError):
-            template_vm_api.sort_by_id_list(
-                list_templates_ordering, create_mock_request(user=self.user2)
-            )
+        template_vm_list = [self.fixture.global_tvm1.id]
 
-    def test_sort_by_id_list_global_templates_as_user_returns_templates(
+        template_vm_api.update_global_template_ordering(
+            template_vm_list, request=create_mock_request(user=self.superuser1)
+        )
+
+    def test_update_user_template_ordering_as_superuser_raises_acl_error(
         self,
     ):
-        """test sort by id list others templates as user returns templates
+        """test_update_user_template_ordering_as_superuser_raises_acl_error
 
         Returns:
 
         """
         # Arrange
-        list_templates_ordering = [
-            self.fixture.global_tvm2.id,
-            self.fixture.global_tvm1.id,
-        ]
-        # Act
-        result = template_vm_api.sort_by_id_list(
-            list_templates_ordering, create_mock_request(user=self.user1)
-        )
-        # Assert
-        self.assertEqual(len(result), 2)
+        template_vm_list = [self.fixture.tvm2.id]
 
-    def test_sort_by_id_list_users_templates_as_superuser_returns_templates(
+        # Act # Assert
+        with self.assertRaises(AccessControlError):
+            template_vm_api.update_global_template_ordering(
+                template_vm_list,
+                request=create_mock_request(user=self.superuser1),
+            )
+
+    def test_update_global_template_ordering_as_user_raises_acl_error(
         self,
     ):
-        """test sort by id list users templates as superuser saves returns templates
+        """test_update_global_template_ordering_as_user_raises_acl_error
 
         Returns:
 
         """
         # Arrange
-        list_templates_ordering = [self.fixture.tvm2.id, self.fixture.tvm1.id]
-        # Act
-        result = template_vm_api.sort_by_id_list(
-            list_templates_ordering, create_mock_request(user=self.superuser1)
-        )
+        list_templates_ordering = [self.fixture.global_tvm1.id]
 
-        # Assert
-        self.assertEqual(len(result), 2)
+        # Act # Assert
+        with self.assertRaises(AccessControlError):
+            template_vm_api.update_global_template_ordering(
+                list_templates_ordering,
+                request=create_mock_request(user=self.user1),
+            )
 
-    def test_sort_by_id_list_global_templates_as_superuser_returns_templates(
+    def test_update_user_template_ordering_as_anonymous_raises_acl_error(
         self,
     ):
-        """test sort by id list users templates as superuser saves returns templates
+        """test_update_user_template_ordering_as_anonymous_raises_acl_error
 
         Returns:
 
         """
         # Arrange
-        list_templates_ordering = [
-            self.fixture.global_tvm2.id,
-            self.fixture.global_tvm1.id,
-        ]
-        # Act
-        result = template_vm_api.sort_by_id_list(
-            list_templates_ordering, create_mock_request(user=self.superuser1)
-        )
-        # Assert
-        self.assertEqual(len(result), 2)
+        list_templates_ordering = [self.fixture.global_tvm1.id]
+
+        # Act # Assert
+        with self.assertRaises(AccessControlError):
+            template_vm_api.update_global_template_ordering(
+                list_templates_ordering,
+                request=create_mock_request(user=self.anonymous_user),
+            )
```

### Comparing `core_main_app-2.3.0/tests/components/template_version_manager/tests_unit.py` & `core_main_app-2.4.0/tests/components/template_version_manager/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/template_xsl_rendering/fixtures/fixtures.py` & `core_main_app-2.4.0/tests/components/template_xsl_rendering/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/template_xsl_rendering/tests_int.py` & `core_main_app-2.4.0/tests/components/template_xsl_rendering/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/template_xsl_rendering/tests_unit.py` & `core_main_app-2.4.0/tests/components/template_xsl_rendering/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/user/fixtures/fixtures.py` & `core_main_app-2.4.0/tests/components/user/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/user/fixtures/tests_int.py` & `core_main_app-2.4.0/tests/components/user/fixtures/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/user/tests_int.py` & `core_main_app-2.4.0/tests/components/user/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/version_manager/tests_int_access_control.py` & `core_main_app-2.4.0/tests/components/version_manager/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/version_manager/tests_unit.py` & `core_main_app-2.4.0/tests/components/version_manager/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/web_page/tests_unit.py` & `core_main_app-2.4.0/tests/components/web_page/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/web_page_login/tests_unit.py` & `core_main_app-2.4.0/tests/components/web_page_login/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/workspace/fixtures/fixtures.py` & `core_main_app-2.4.0/tests/components/workspace/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/workspace/fixtures/tests_int.py` & `core_main_app-2.4.0/tests/components/workspace/fixtures/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/workspace/tests_int.py` & `core_main_app-2.4.0/tests/components/workspace/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/components/xsl_transformation/tests_unit.py` & `core_main_app-2.4.0/tests/components/xsl_transformation/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/rest/blob/tests_int.py` & `core_main_app-2.4.0/tests/rest/blob/tests_int.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,27 +6,31 @@
 from django.core.files.uploadedfile import SimpleUploadedFile
 from django.test import override_settings
 from rest_framework import status
 from tests.components.blob.fixtures.fixtures import (
     BlobFixtures,
     AccessControlBlobFixture,
 )
+from tests.components.data.fixtures.fixtures import (
+    AccessControlBlobWithMetadataFixture,
+)
 
 from core_main_app.components.blob.models import Blob
 from core_main_app.components.workspace.models import Workspace
 from core_main_app.rest.blob import views
 from core_main_app.utils.integration_tests.integration_base_test_case import (
     IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 
 RESOURCES_PATH = join(dirname(abspath(__file__)), "data")
 fixture_blob = BlobFixtures()
 fixture_blob_workspace = AccessControlBlobFixture()
+fixture_blob_metadata = AccessControlBlobWithMetadataFixture()
 
 
 class TestBlobListAdmin(IntegrationBaseTestCase):
     """TestBlobListAdmin"""
 
     fixture = fixture_blob
 
@@ -856,7 +860,281 @@
             views.BlobChangeOwner.as_view(),
             user_request,
             param={"pk": blob.id, "user_id": self.fixture.workspace_1.id},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
+
+
+class TestBlobAddMetadata(IntegrationBaseTestCase):
+    """TestBlobAddMetadata"""
+
+    fixture = fixture_blob_metadata
+
+    def test_add_metadata_authorized_returns_http_200(
+        self,
+    ):
+        """test_add_metadata_authorized_returns_http_200
+
+        Args:
+
+        Returns:
+
+        """
+        # Arrange
+        blob = self.fixture.blob_1
+        mock_user = create_mock_user("1")
+
+        # Act
+        response = RequestMock.do_request_post(
+            views.BlobMetadata.as_view(),
+            mock_user,
+            param={"pk": blob.id, "metadata_id": self.fixture.data_4.id},
+        )
+
+        # Assert
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
+
+    @patch("core_main_app.components.blob.api.add_metadata")
+    def test_add_metadata_with_errors_returns_http_500(self, add_metadata):
+        """test_add_metadata_with_errors_returns_http_500
+
+        Args:
+
+        Returns:
+
+        """
+        # Arrange
+        blob = self.fixture.blob_1
+        mock_user = create_mock_user("1")
+        add_metadata.side_effect = Exception()
+
+        # Act
+        response = RequestMock.do_request_post(
+            views.BlobMetadata.as_view(),
+            mock_user,
+            param={"pk": blob.id, "metadata_id": self.fixture.data_4.id},
+        )
+
+        # Assert
+        self.assertEqual(
+            response.status_code, status.HTTP_500_INTERNAL_SERVER_ERROR
+        )
+
+    @patch(
+        "core_main_app.components.workspace.api.get_all_workspaces_with_write_access_by_user"
+    )
+    @patch(
+        "core_main_app.components.workspace.api.get_all_workspaces_with_read_access_by_user"
+    )
+    def test_add_metadata_unauthorized_returns_http_403(
+        self,
+        get_all_workspaces_with_read_access_by_user,
+        get_all_workspaces_with_write_access_by_user,
+    ):
+        """test_add_metadata_unauthorized_returns_http_403
+
+        Args:
+
+        Returns:
+
+        """
+        # Arrange
+        blob = self.fixture.blob_3
+        mock_user = create_mock_user("1")
+        get_all_workspaces_with_read_access_by_user.return_value = []
+        get_all_workspaces_with_write_access_by_user.return_value = []
+
+        # Act
+        response = RequestMock.do_request_post(
+            views.BlobMetadata.as_view(),
+            mock_user,
+            param={"pk": blob.id, "metadata_id": self.fixture.data_4.id},
+        )
+
+        # Assert
+        self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
+
+    def test_add_metadata_wrong_blob_id_returns_http_404(
+        self,
+    ):
+        """test_add_metadata_wrong_blob_id_returns_http_404
+
+        Args:
+
+        Returns:
+
+        """
+        # Arrange
+        mock_user = create_mock_user("1")
+
+        # Act
+        response = RequestMock.do_request_post(
+            views.BlobMetadata.as_view(),
+            mock_user,
+            param={"pk": "1234", "metadata_id": self.fixture.data_4.id},
+        )
+
+        # Assert
+        self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
+
+    def test_add_metadata_wrong_data_id_returns_http_404(
+        self,
+    ):
+        """test_add_metadata_wrong_data_id_returns_http_404
+
+        Args:
+
+        Returns:
+
+        """
+        # Arrange
+        blob = self.fixture.blob_1
+        mock_user = create_mock_user("1")
+        # Act
+        response = RequestMock.do_request_post(
+            views.BlobMetadata.as_view(),
+            mock_user,
+            param={"pk": blob.id, "metadata_id": "1234"},
+        )
+
+        # Assert
+        self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
+
+
+class TestBlobRemoveMetadata(IntegrationBaseTestCase):
+    """TestBlobRemoveMetadata"""
+
+    fixture = fixture_blob_metadata
+
+    def test_remove_metadata_authorized_returns_http_200(
+        self,
+    ):
+        """test_remove_metadata_authorized_returns_http_200
+
+        Args:
+
+        Returns:
+
+        """
+        # Arrange
+        blob = self.fixture.blob_1
+        mock_user = create_mock_user("1")
+
+        # Act
+        response = RequestMock.do_request_delete(
+            views.BlobMetadata.as_view(),
+            mock_user,
+            param={"pk": blob.id, "metadata_id": self.fixture.data_1.id},
+        )
+
+        # Assert
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
+
+    @patch("core_main_app.components.blob.api.remove_metadata")
+    def test_remove_metadata_with_errors_returns_http_500(
+        self, remove_metadata
+    ):
+        """test_remove_metadata_with_errors_returns_http_500
+
+        Args:
+
+        Returns:
+
+        """
+        # Arrange
+        blob = self.fixture.blob_1
+        mock_user = create_mock_user("1")
+        remove_metadata.side_effect = Exception()
+
+        # Act
+        response = RequestMock.do_request_delete(
+            views.BlobMetadata.as_view(),
+            mock_user,
+            param={"pk": blob.id, "metadata_id": self.fixture.data_1.id},
+        )
+
+        # Assert
+        self.assertEqual(
+            response.status_code, status.HTTP_500_INTERNAL_SERVER_ERROR
+        )
+
+    @patch(
+        "core_main_app.components.workspace.api.get_all_workspaces_with_write_access_by_user"
+    )
+    @patch(
+        "core_main_app.components.workspace.api.get_all_workspaces_with_read_access_by_user"
+    )
+    def test_remove_metadata_unauthorized_returns_http_403(
+        self,
+        get_all_workspaces_with_read_access_by_user,
+        get_all_workspaces_with_write_access_by_user,
+    ):
+        """test_remove_metadata_unauthorized_returns_http_403
+
+        Args:
+
+        Returns:
+
+        """
+        # Arrange
+        blob = self.fixture.blob_3
+        mock_user = create_mock_user("1")
+        get_all_workspaces_with_read_access_by_user.return_value = []
+        get_all_workspaces_with_write_access_by_user.return_value = []
+
+        # Act
+        response = RequestMock.do_request_delete(
+            views.BlobMetadata.as_view(),
+            mock_user,
+            param={"pk": blob.id, "metadata_id": self.fixture.data_32.id},
+        )
+
+        # Assert
+        self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
+
+    def test_remove_metadata_wrong_blob_id_returns_http_404(
+        self,
+    ):
+        """test_remove_metadata_wrong_blob_id_returns_http_404
+
+        Args:
+
+        Returns:
+
+        """
+        # Arrange
+        mock_user = create_mock_user("1")
+
+        # Act
+        response = RequestMock.do_request_delete(
+            views.BlobMetadata.as_view(),
+            mock_user,
+            param={"pk": "1234", "metadata_id": self.fixture.data_1.id},
+        )
+
+        # Assert
+        self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
+
+    def test_remove_metadata_wrong_data_id_returns_http_404(
+        self,
+    ):
+        """test_remove_metadata_wrong_data_id_returns_http_404
+
+        Args:
+
+        Returns:
+
+        """
+        # Arrange
+        blob = self.fixture.blob_1
+        mock_user = create_mock_user("1")
+        # Act
+        response = RequestMock.do_request_delete(
+            views.BlobMetadata.as_view(),
+            mock_user,
+            param={"pk": blob.id, "metadata_id": "1234"},
+        )
+
+        # Assert
+        self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
```

### Comparing `core_main_app-2.3.0/tests/rest/blob/tests_permissions.py` & `core_main_app-2.4.0/tests/rest/blob/tests_permissions.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from core_main_app.rest.blob import views as blob_rest_views
 from core_main_app.rest.blob.serializers import (
     BlobSerializer,
     DeleteBlobsSerializer,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
+from core_main_app.components.data import api as data_api
 
 
 class TestBlobListAdminGetPermissions(SimpleTestCase):
     """TestBlobListAdminGetPermissions"""
 
     def test_anonymous_returns_http_403(self):
         """test_anonymous_returns_http_403
@@ -268,14 +269,240 @@
         response = RequestMock.do_request_get(
             blob_rest_views.BlobDetail.as_view(), mock_user, param={"pk": "0"}
         )
 
         self.assertEqual(response.status_code, status.HTTP_200_OK)
 
 
+class TestBlobAddMetadataPermissions(SimpleTestCase):
+    """TestBlobDetailGetPermissions"""
+
+    @patch.object(BlobSerializer, "data")
+    @patch.object(blob_api, "add_metadata")
+    @patch.object(blob_api, "get_by_id")
+    @patch.object(data_api, "get_by_id")
+    def test_anonymous_returns_http_403(
+        self,
+        mock_data_api_get_by_id,
+        mock_blob_api_get_by_id,
+        mock_blob_api_add_metadata,
+        mock_blob_serializer_data,
+    ):
+        """test_anonymous_returns_http_200
+
+        Args:
+            mock_data_api_get_by_id:
+            mock_blob_api_get_by_id:
+            mock_blob_api_add_metadata:
+            mock_blob_serializer_data:
+
+        Returns:
+
+        """
+        mock_data_api_get_by_id.return_value = []
+        mock_blob_api_get_by_id.return_value = []
+        mock_blob_api_add_metadata.return_value = None
+        mock_blob_serializer_data.return_value = []
+
+        response = RequestMock.do_request_post(
+            blob_rest_views.BlobMetadata.as_view(),
+            None,
+            param={"pk": "1", "metadata_id": "1"},
+        )
+
+        self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
+
+    @patch.object(BlobSerializer, "data")
+    @patch.object(blob_api, "add_metadata")
+    @patch.object(blob_api, "get_by_id")
+    @patch.object(data_api, "get_by_id")
+    def test_authenticated_returns_http_200(
+        self,
+        mock_data_api_get_by_id,
+        mock_blob_api_get_by_id,
+        mock_blob_api_add_metadata,
+        mock_blob_serializer_data,
+    ):
+        """test_authenticated_returns_http_200
+
+        Args:
+            mock_data_api_get_by_id:
+            mock_blob_api_get_by_id:
+            mock_blob_api_add_metadata:
+            mock_blob_serializer_data:
+
+        Returns:
+
+        """
+        mock_data_api_get_by_id.return_value = []
+        mock_blob_api_get_by_id.return_value = []
+        mock_blob_api_add_metadata.return_value = []
+        mock_blob_serializer_data.return_value = []
+
+        mock_user = create_mock_user("1")
+
+        response = RequestMock.do_request_post(
+            blob_rest_views.BlobMetadata.as_view(),
+            mock_user,
+            param={"pk": "1", "metadata_id": "1"},
+        )
+
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
+
+    @patch.object(BlobSerializer, "data")
+    @patch.object(blob_api, "add_metadata")
+    @patch.object(blob_api, "get_by_id")
+    @patch.object(data_api, "get_by_id")
+    def test_staff_returns_http_200(
+        self,
+        mock_data_api_get_by_id,
+        mock_blob_api_get_by_id,
+        mock_blob_api_add_metadata,
+        mock_blob_serializer_data,
+    ):
+        """test_staff_returns_http_200
+
+        Args:
+            mock_data_api_get_by_id:
+            mock_blob_api_get_by_id:
+            mock_blob_api_add_metadata:
+            mock_blob_serializer_data:
+
+        Returns:
+
+        """
+        mock_data_api_get_by_id.return_value = []
+        mock_blob_api_get_by_id.return_value = []
+        mock_blob_api_add_metadata.return_value = []
+        mock_blob_serializer_data.return_value = []
+
+        mock_user = create_mock_user("1", is_staff=True)
+
+        response = RequestMock.do_request_post(
+            blob_rest_views.BlobMetadata.as_view(),
+            mock_user,
+            param={"pk": "1", "metadata_id": "1"},
+        )
+
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
+
+
+class TestBlobRemoveMetadataPermissions(SimpleTestCase):
+    """TestBlobRemoveMetadataPermissions"""
+
+    @patch.object(BlobSerializer, "data")
+    @patch.object(blob_api, "remove_metadata")
+    @patch.object(blob_api, "get_by_id")
+    @patch.object(data_api, "get_by_id")
+    def test_anonymous_returns_http_403(
+        self,
+        mock_data_api_get_by_id,
+        mock_blob_api_get_by_id,
+        mock_blob_api_remove_metadata,
+        mock_blob_serializer_data,
+    ):
+        """test_anonymous_returns_http_200
+
+        Args:
+            mock_data_api_get_by_id:
+            mock_blob_api_get_by_id:
+            mock_blob_api_remove_metadata:
+            mock_blob_serializer_data:
+
+        Returns:
+
+        """
+        mock_data_api_get_by_id.return_value = []
+        mock_blob_api_get_by_id.return_value = []
+        mock_blob_api_remove_metadata.return_value = None
+        mock_blob_serializer_data.return_value = []
+
+        response = RequestMock.do_request_delete(
+            blob_rest_views.BlobMetadata.as_view(),
+            None,
+            param={"pk": "1", "metadata_id": "1"},
+        )
+
+        self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
+
+    @patch.object(BlobSerializer, "data")
+    @patch.object(blob_api, "remove_metadata")
+    @patch.object(blob_api, "get_by_id")
+    @patch.object(data_api, "get_by_id")
+    def test_authenticated_returns_http_200(
+        self,
+        mock_data_api_get_by_id,
+        mock_blob_api_get_by_id,
+        mock_blob_api_remove_metadata,
+        mock_blob_serializer_data,
+    ):
+        """test_authenticated_returns_http_200
+
+        Args:
+            mock_data_api_get_by_id:
+            mock_blob_api_get_by_id:
+            mock_blob_api_remove_metadata:
+            mock_blob_serializer_data:
+
+        Returns:
+
+        """
+        mock_data_api_get_by_id.return_value = []
+        mock_blob_api_get_by_id.return_value = []
+        mock_blob_api_remove_metadata.return_value = []
+        mock_blob_serializer_data.return_value = []
+
+        mock_user = create_mock_user("1")
+
+        response = RequestMock.do_request_delete(
+            blob_rest_views.BlobMetadata.as_view(),
+            mock_user,
+            param={"pk": "1", "metadata_id": "1"},
+        )
+
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
+
+    @patch.object(BlobSerializer, "data")
+    @patch.object(blob_api, "remove_metadata")
+    @patch.object(blob_api, "get_by_id")
+    @patch.object(data_api, "get_by_id")
+    def test_staff_returns_http_200(
+        self,
+        mock_data_api_get_by_id,
+        mock_blob_api_get_by_id,
+        mock_blob_api_remove_metadata,
+        mock_blob_serializer_data,
+    ):
+        """test_staff_returns_http_200
+
+        Args:
+            mock_data_api_get_by_id:
+            mock_blob_api_get_by_id:
+            mock_blob_api_remove_metadata:
+            mock_blob_serializer_data:
+
+        Returns:
+
+        """
+        mock_data_api_get_by_id.return_value = []
+        mock_blob_api_get_by_id.return_value = []
+        mock_blob_api_remove_metadata.return_value = []
+        mock_blob_serializer_data.return_value = []
+
+        mock_user = create_mock_user("1", is_staff=True)
+
+        response = RequestMock.do_request_delete(
+            blob_rest_views.BlobMetadata.as_view(),
+            mock_user,
+            param={"pk": "1", "metadata_id": "1"},
+        )
+
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
+
+
 class TestBlobDetailDeletePermissions(SimpleTestCase):
     """TestBlobDetailDeletePermissions"""
 
     def test_anonymous_returns_http_403(self):
         """test_anonymous_returns_http_403
 
         Returns:
```

### Comparing `core_main_app-2.3.0/tests/rest/data/tests_int.py` & `core_main_app-2.4.0/tests/rest/data/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/rest/data/tests_permissions.py` & `core_main_app-2.4.0/tests/rest/data/tests_permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1293,7 +1293,145 @@
             data_migration.as_view(),
             request_user,
             param={"pk": self.fake_id},
             data={"data": f'["{self.fake_id}"]'},
         )
 
         self.assertEqual(response.status_code, status.HTTP_200_OK)
+
+
+class TestGetTaskProgressPermission(SimpleTestCase):
+    """TestGetTaskProgressPermission"""
+
+    def setUp(self):
+        """setUp
+
+        Returns:
+
+        """
+        self.task_id = "123"
+
+    def test_anonymous_get_task_progress_returns_http_403(self):
+        """test_anonymous_get_task_progress_returns_http_403
+
+        Returns:
+
+        """
+        # Arrange
+        mock_user = create_mock_user(1, is_anonymous=True)
+
+        # Act
+        response = RequestMock.do_request_get(
+            data_rest_views.GetTaskProgress.as_view(),
+            mock_user,
+            param={"task_id": self.task_id},
+        )
+
+        self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
+
+    def test_user_get_task_progress_returns_http_403(self):
+        """test_user_get_task_progress_returns_http_403
+
+        Returns:
+
+        """
+        # Arrange
+        mock_user = create_mock_user(1)
+
+        # Act
+        response = RequestMock.do_request_get(
+            data_rest_views.GetTaskProgress.as_view(),
+            mock_user,
+            param={"task_id": self.task_id},
+        )
+
+        self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
+
+    @patch("core_main_app.components.data.tasks.get_task_progress")
+    def test_admin_get_task_progress_returns_http_200(
+        self, mock_get_task_progress
+    ):
+        """test_admin_get_task_progress_returns_http_200
+
+        Returns:
+
+        """
+        # Arrange
+        mock_user = create_mock_user(1, is_staff=True)
+
+        # Act
+        response = RequestMock.do_request_get(
+            data_rest_views.GetTaskProgress.as_view(),
+            mock_user,
+            param={"task_id": self.task_id},
+        )
+
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
+
+
+class TestGetTaskResultPermission(SimpleTestCase):
+    """TestGetTaskResultPermission"""
+
+    def setUp(self):
+        """setUp
+
+        Returns:
+
+        """
+        self.task_id = "123"
+
+    def test_anonymous_get_task_result_returns_http_403(self):
+        """test_anonymous_get_task_result_returns_http_403
+
+        Returns:
+
+        """
+        # Arrange
+        mock_user = create_mock_user(None, is_anonymous=True)
+
+        # Act
+        response = RequestMock.do_request_get(
+            data_rest_views.GetTaskResult.as_view(),
+            mock_user,
+            param={"task_id": self.task_id},
+        )
+
+        self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
+
+    def test_user_get_task_result_returns_http_403(self):
+        """test_user_get_task_result_returns_http_403
+
+        Returns:
+
+        """
+        # Arrange
+        mock_user = create_mock_user(1)
+
+        # Act
+        response = RequestMock.do_request_get(
+            data_rest_views.GetTaskResult.as_view(),
+            mock_user,
+            param={"task_id": self.task_id},
+        )
+
+        self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
+
+    @patch("core_main_app.components.data.tasks.get_task_result")
+    def test_admin_get_task_result_returns_http_200(
+        self, mock_get_task_result
+    ):
+        """test_admin_get_task_result_returns_http_200
+
+        Returns:
+
+        """
+        # Arrange
+        mock_user = create_mock_user(1, is_staff=True)
+
+        # Act
+        response = RequestMock.do_request_get(
+            data_rest_views.GetTaskResult.as_view(),
+            mock_user,
+            param={"task_id": self.task_id},
+        )
+
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
```

### Comparing `core_main_app-2.3.0/tests/rest/data/tests_unit.py` & `core_main_app-2.4.0/tests/rest/data/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/rest/template/tests_int.py` & `core_main_app-2.4.0/tests/rest/template/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/rest/template/tests_permission.py` & `core_main_app-2.4.0/tests/rest/template/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/rest/template/tests_unit.py` & `core_main_app-2.4.0/tests/rest/template/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/rest/template_version_manager/tests_int.py` & `core_main_app-2.4.0/tests/rest/template_version_manager/tests_int.py`

 * *Files 9% similar despite different names*

```diff
@@ -1313,82 +1313,343 @@
             param={"pk": str(self.fixture.template_vm_2.id)},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
 
 
-class TemplateVersionManagerOrdering(IntegrationBaseTestCase):
-    """TemplateVersionManagerOrdering"""
+class UserTemplateVersionManagerOrdering(IntegrationBaseTestCase):
+    """User Template Version Manager Ordering"""
 
     fixture = fixture_template_vm_ordering
 
-    def test_patch_as_owner_returns_http_200(self):
-        """test_patch_as_owner_returns_http_200
+    def test_get_as_owner_returns_all_user_template_version_managers(self):
+        """test_get_as_owner_returns_all_user_template_version_managers
+
+        Returns:
+
+        """
+        # Arrange
+        user = create_mock_user("1")
+        # Act
+        response = RequestMock.do_request_get(
+            views.UserTemplateVersionManagerOrdering.as_view(),
+            user,
+        )
+
+        # Assert
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
+        self.assertEqual(len(response.data), 2)
+
+    def test_get_as_owner_returns_empty_list(self):
+        """test_get_as_owner_returns_empty_list
+
+        Returns:
+
+        """
+        # Arrange
+        user = create_mock_user("2")
+        # Act
+        response = RequestMock.do_request_get(
+            views.UserTemplateVersionManagerOrdering.as_view(),
+            user,
+        )
+
+        # Assert
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
+        self.assertEqual(len(response.data), 0)
+
+    def test_get_as_superuser_returns_all_user_template_version_managers(self):
+        """test_get_as_superuser_returns_all_user_template_version_managers
+
+        Returns:
+
+        """
+        # Arrange
+        user = create_mock_user("1", is_staff=True, is_superuser=True)
+        # Act
+        response = RequestMock.do_request_get(
+            views.UserTemplateVersionManagerOrdering.as_view(),
+            user,
+        )
+
+        # Assert
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
+        self.assertEqual(len(response.data), 2)
+
+    def test_patch_as_owner_updates_template_version_manager_ordering(self):
+        """test_patch_as_owner_updates_template_version_manager_ordering
 
         Returns:
 
         """
         # Arrange
         user = create_mock_user("1")
         # Act
         response = RequestMock.do_request_patch(
-            views.TemplateVersionManagerOrdering.as_view(),
+            views.UserTemplateVersionManagerOrdering.as_view(),
             user,
             data={
                 "template_list": [self.fixture.tvm2.id, self.fixture.tvm1.id]
             },
         )
-
         # Assert
         self.assertEqual(response.status_code, status.HTTP_200_OK)
+        self.assertEqual(response.data[0]["display_rank"], 1)
+        self.assertEqual(response.data[0]["id"], self.fixture.tvm2.id)
+        self.assertEqual(response.data[1]["display_rank"], 2)
+        self.assertEqual(response.data[1]["id"], self.fixture.tvm1.id)
+
+    def test_patch_wrong_ids_returns_http_404(self):
+        """test_patch_wrong_ids_returns_http_404
+
+        Returns:
+
+        """
+        # Arrange
+        user = create_mock_user("1")
+        # Act
+        response = RequestMock.do_request_patch(
+            views.UserTemplateVersionManagerOrdering.as_view(),
+            user,
+            data={
+                "template_list": [
+                    self.fixture.tvm2.id,
+                    -1,
+                    self.fixture.tvm1.id,
+                ]
+            },
+        )
+
+        # Assert
+        self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
 
-    def test_patch_as_user_returns_http_403(self):
-        """test_patch_as_user_returns_http_403
+    def test_patch_inaccessible_id_returns_http_403(self):
+        """test_patch_wrong_ids_returns_http_404
+
+        Returns:
+
+        """
+        # Arrange
+        user = create_mock_user("1")
+        # Act
+        response = RequestMock.do_request_patch(
+            views.UserTemplateVersionManagerOrdering.as_view(),
+            user,
+            data={
+                "template_list": [
+                    self.fixture.tvm2.id,
+                    self.fixture.global_tvm2.id,
+                ]
+            },
+        )
+
+        # Assert
+        self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
+
+    def test_patch_duplicate_ids_returns_http_400(self):
+        """test_patch_duplicate_ids_returns_http_400
+
+        Returns:
+
+        """
+        # Arrange
+        user = create_mock_user("1")
+        # Act
+        response = RequestMock.do_request_patch(
+            views.UserTemplateVersionManagerOrdering.as_view(),
+            user,
+            data={
+                "template_list": [self.fixture.tvm2.id, self.fixture.tvm2.id]
+            },
+        )
+
+        # Assert
+        self.assertEqual(response.status_code, status.HTTP_400_BAD_REQUEST)
+
+    def test_patch_others_template_version_manager_returns_http_403(self):
+        """test_patch_returns_updates_template_version_manager_order
 
         Returns:
 
         """
         # Arrange
         user = create_mock_user("2")
         # Act
         response = RequestMock.do_request_patch(
-            views.TemplateVersionManagerOrdering.as_view(),
+            views.UserTemplateVersionManagerOrdering.as_view(),
             user,
             data={
                 "template_list": [self.fixture.tvm2.id, self.fixture.tvm1.id]
             },
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
 
-    def test_patch_global_as_superuser_returns_http_200(self):
-        """test_patch_as_superuser_returns_http_200
+    def test_patch_without_param__returns_http_500(self):
+        """test_patch_returns_updates_template_version_manager_order
+
+        Returns:
+
+        """
+        # Arrange
+        user = create_mock_user("2")
+        # Act
+        response = RequestMock.do_request_patch(
+            views.UserTemplateVersionManagerOrdering.as_view(),
+            user,
+        )
+
+        # Assert
+        self.assertEqual(
+            response.status_code, status.HTTP_500_INTERNAL_SERVER_ERROR
+        )
+
+
+class GlobalTemplateVersionManagerOrdering(IntegrationBaseTestCase):
+    """Global Template Version Manager Ordering"""
+
+    fixture = fixture_template_vm_ordering
+
+    def test_get_as_user_returns_http_403(self):
+        """test_get_as_user_returns_all_global_template_version_managers
+
+        Returns:
+
+        """
+        # Arrange
+        user = create_mock_user("1")
+        # Act
+        response = RequestMock.do_request_get(
+            views.GlobalTemplateVersionManagerOrdering.as_view(),
+            user,
+        )
+
+        # Assert
+        self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
+
+    def test_get_as_superuser_returns_all_global_template_version_managers(
+        self,
+    ):
+        """test_get_as_superuser_returns_all_global_template_version_managers
 
         Returns:
 
         """
         # Arrange
-        user = create_mock_user("1", is_superuser=True)
+        user = create_mock_user("1", is_staff=True, is_superuser=True)
+        # Act
+        response = RequestMock.do_request_get(
+            views.GlobalTemplateVersionManagerOrdering.as_view(),
+            user,
+        )
+
+        # Assert
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
+        self.assertEqual(len(response.data), 2)
+
+    def test_patch_as_user_returns_error_403(self):
+        """test_patch_as_user_returns_error_403
+
+        Returns:
+
+        """
+        # Arrange
+        user = create_mock_user("1")
+        # Act
+        response = RequestMock.do_request_patch(
+            views.GlobalTemplateVersionManagerOrdering.as_view(),
+            user,
+            data={
+                "template_list": [
+                    self.fixture.global_tvm2.id,
+                    self.fixture.global_tvm1.id,
+                ]
+            },
+        )
+
+        # Assert
+        self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
 
+    def test_patch_as_superuser_updates_template_version_manager_ordering(
+        self,
+    ):
+        """test_patch_as_superuser_updates_template_version_manager_ordering
+
+        Returns:
+
+        """
+        # Arrange
+        user = create_mock_user("1", is_staff=True, is_superuser=True)
         # Act
         response = RequestMock.do_request_patch(
-            views.TemplateVersionManagerOrdering.as_view(),
+            views.GlobalTemplateVersionManagerOrdering.as_view(),
             user,
             data={
                 "template_list": [
                     self.fixture.global_tvm2.id,
                     self.fixture.global_tvm1.id,
                 ]
             },
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_200_OK)
+        self.assertEqual(response.data[0]["display_rank"], 1)
+        self.assertEqual(response.data[0]["id"], self.fixture.global_tvm2.id)
+        self.assertEqual(response.data[1]["display_rank"], 2)
+        self.assertEqual(response.data[1]["id"], self.fixture.global_tvm1.id)
+
+    def test_patch_wrong_ids_returns_http_404(self):
+        """test_patch_wrong_ids_returns_http_404
+
+        Returns:
+
+        """
+        # Arrange
+        user = create_mock_user("1", is_staff=True, is_superuser=True)
+        # Act
+        response = RequestMock.do_request_patch(
+            views.GlobalTemplateVersionManagerOrdering.as_view(),
+            user,
+            data={
+                "template_list": [
+                    self.fixture.global_tvm2.id,
+                    -1,
+                    self.fixture.global_tvm1.id,
+                ]
+            },
+        )
+
+        # Assert
+        self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
+
+    def test_patch_duplicate_ids_returns_http_400(self):
+        """test_patch_duplicate_ids_returns_http_400
+
+        Returns:
+
+        """
+        # Arrange
+        user = create_mock_user("1", is_staff=True, is_superuser=True)
+        # Act
+        response = RequestMock.do_request_patch(
+            views.GlobalTemplateVersionManagerOrdering.as_view(),
+            user,
+            data={
+                "template_list": [
+                    self.fixture.global_tvm2.id,
+                    self.fixture.global_tvm2.id,
+                ]
+            },
+        )
+
+        # Assert
+        self.assertEqual(response.status_code, status.HTTP_400_BAD_REQUEST)
 
 
 class TestTemplateVersionManagerList(IntegrationBaseTestCase):
     """TestTemplateVersionManagerList"""
 
     fixture = fixture_template_2
```

### Comparing `core_main_app-2.3.0/tests/rest/template_version_manager/tests_permission.py` & `core_main_app-2.4.0/tests/rest/template_version_manager/tests_permission.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ Authentication tests for Template Version Manager REST API
 """
 from unittest.mock import patch
 
+from core_main_app.access_control.exceptions import AccessControlError
 from django.test import SimpleTestCase
 from rest_framework import status
 
 from core_main_app.components.template.models import Template
 from core_main_app.components.template_version_manager.models import (
     TemplateVersionManager,
 )
@@ -889,150 +890,462 @@
             mock_user,
             param={"pk": self.fake_id},
         )
 
         self.assertEqual(response.status_code, status.HTTP_200_OK)
 
 
-class TestTemplateVersionManagerOrderingPatchPermission(SimpleTestCase):
+class TestTemplateVersionManagerListGetPermission(SimpleTestCase):
+    """TestGlobalTemplateVersionManagerListGetPermission"""
+
+    @patch.object(template_version_manager_api, "get_all")
+    def test_anonymous_returns_http_403(
+        self, template_version_manager_get_all
+    ):
+        """test_anonymous_returns_http_403
+
+        Args:
+            template_version_manager_get_all:
+
+        Returns:
+
+        """
+        template_version_manager_get_all.return_value = TemplateVersionManager(
+            user=None
+        )
+
+        response = RequestMock.do_request_get(
+            template_version_manager_views.GlobalAndUserTemplateVersionManagerList.as_view(),
+            None,
+        )
+
+        self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
+
+    @patch.object(template_version_manager_api, "get_all")
+    def test_authenticated_returns_http_403(
+        self, template_version_manager_get_all
+    ):
+        """test_authenticated_returns_http_200
+
+        Args:
+            template_version_manager_get_all:
+
+        Returns:
+
+        """
+        template_version_manager_get_all.return_value = {}
+
+        mock_user = create_mock_user("1")
+
+        response = RequestMock.do_request_get(
+            template_version_manager_views.GlobalAndUserTemplateVersionManagerList.as_view(),
+            mock_user,
+        )
+
+        self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
+
+    @patch.object(template_version_manager_api, "get_all")
+    def test_staff_returns_http_200(self, template_version_manager_get_all):
+        """test_staff_returns_http_200
+
+        Args:
+            template_version_manager_get_all:
+
+        Returns:
+
+        """
+        template_version_manager_get_all.return_value = {}
+
+        mock_user = create_mock_user("1", is_staff=True)
+
+        response = RequestMock.do_request_get(
+            template_version_manager_views.GlobalAndUserTemplateVersionManagerList.as_view(),
+            mock_user,
+        )
+
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
+
+
+class TestGlobalTemplateVersionManagerOrderingListGetPermission(
+    SimpleTestCase
+):
+    """Test Template Version Manager Ordering List Get Permission"""
+
+    def test_anonymous_returns_http_403(
+        self,
+    ):
+        """test_anonymous_returns_http_403
+
+        Args:
+
+        Returns:
+
+        """
+        response = RequestMock.do_request_get(
+            template_version_manager_views.GlobalTemplateVersionManagerOrdering.as_view(),
+            None,
+        )
+        self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
+
+    def test_authenticated_returns_http_403(self):
+        """test_authenticated_returns_http_403
+
+        Args:
+
+        Returns:
+
+        """
+
+        mock_user = create_mock_user("1")
+
+        response = RequestMock.do_request_get(
+            template_version_manager_views.GlobalTemplateVersionManagerOrdering.as_view(),
+            mock_user,
+        )
+
+        self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
+
+    @patch.object(template_version_manager_api, "get_global_version_managers")
+    def test_staff_returns_http_200(self, template_version_manager_get_all):
+        """test_staff_returns_http_200
+
+        Args:
+            template_version_manager_get_all:
+
+        Returns:
+
+        """
+        template_version_manager_get_all.return_value = {}
+
+        mock_user = create_mock_user("1", is_staff=True)
+
+        response = RequestMock.do_request_get(
+            template_version_manager_views.GlobalTemplateVersionManagerOrdering.as_view(),
+            mock_user,
+        )
+
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
+
+    @patch.object(template_version_manager_api, "get_global_version_managers")
+    def test_superuser_returns_http_200(
+        self, template_version_manager_get_all
+    ):
+        """test_superuser_returns_http_200
+
+        Args:
+            template_version_manager_get_all:
+
+        Returns:
+
+        """
+        template_version_manager_get_all.return_value = {}
+
+        mock_user = create_mock_user("1", is_staff=True, is_superuser=True)
+
+        response = RequestMock.do_request_get(
+            template_version_manager_views.GlobalTemplateVersionManagerOrdering.as_view(),
+            mock_user,
+        )
+
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
+
+
+class TestGlobalTemplateVersionManagerOrderingPatchPermission(SimpleTestCase):
     """Test Template Version Manager Ordering Patch Permission"""
 
     def test_anonymous_returns_http_403(self):
         """test_anonymous_returns_http_403
 
         Returns:
 
         """
         response = RequestMock.do_request_patch(
-            template_version_manager_views.TemplateVersionManagerOrdering.as_view(),
+            template_version_manager_views.UserTemplateVersionManagerOrdering.as_view(),
             None,
         )
         self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
 
     @patch(
-        "core_main_app.components.template_version_manager.api.get_by_id_list"
+        "core_main_app.components.template_version_manager.api.get_global_version_managers"
     )
+    def test_authenticated_returns_http_403(
+        self, mock_get_global_version_managers
+    ):
+        """test_staff_returns_http_403
+
+        Args:
+
+
+        Returns:
+
+        """
+        mock_get_global_version_managers.side_effect = AccessControlError("")
+        response = RequestMock.do_request_patch(
+            template_version_manager_views.GlobalTemplateVersionManagerOrdering.as_view(),
+            create_mock_user("1"),
+            data={"template_list": []},
+        )
+        self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
+
     @patch(
-        "core_main_app.components.template_version_manager.api.update_templates_ordering"
+        "core_main_app.components.template_version_manager.api.get_global_version_managers"
     )
-    def test_authenticated_returns_http_200(
-        self, get_by_id_list, update_templates_ordering
+    @patch(
+        "core_main_app.components.template_version_manager.api.update_global_template_ordering"
+    )
+    def test_staff_returns_http_200(
+        self,
+        mock_get_global_version_managers,
+        mock_update_templates_ordering,
     ):
         """test_staff_returns_http_200
 
         Args:
-            get_by_id_list:
-            update_templates_ordering:
+            mock_get_global_version_managers:
+            mock_update_templates_ordering:
 
         Returns:
 
         """
-        mock_user = create_mock_user("1")
-        get_by_id_list.return_value = []
-        update_templates_ordering.return_value = []
+        mock_user = create_mock_user("1", is_staff=True)
+        mock_get_global_version_managers.return_value = []
+        mock_update_templates_ordering.return_value = []
         response = RequestMock.do_request_patch(
-            template_version_manager_views.TemplateVersionManagerOrdering.as_view(),
+            template_version_manager_views.GlobalTemplateVersionManagerOrdering.as_view(),
             mock_user,
             data={"template_list": []},
         )
 
         self.assertEqual(response.status_code, status.HTTP_200_OK)
 
     @patch(
-        "core_main_app.components.template_version_manager.api.get_by_id_list"
+        "core_main_app.components.template_version_manager.api.get_global_version_managers"
     )
     @patch(
-        "core_main_app.components.template_version_manager.api.update_templates_ordering"
+        "core_main_app.components.template_version_manager.api.update_global_template_ordering"
     )
-    def test_staff_returns_http_200(
-        self, get_by_id_list, update_templates_ordering
+    def test_superuser_returns_http_200(
+        self,
+        mock_get_global_version_managers,
+        mock_update_templates_ordering,
     ):
-        """test_staff_returns_http_200
+        """test_superuser_returns_http_200
 
         Args:
-            get_by_id_list:
-            update_templates_ordering:
+            mock_get_global_version_managers:
+            mock_update_templates_ordering:
 
         Returns:
 
         """
-        mock_user = create_mock_user("1", is_staff=True)
-        get_by_id_list.return_value = []
-        update_templates_ordering.return_value = []
+        mock_user = create_mock_user("1", is_staff=True, is_superuser=True)
+        mock_get_global_version_managers.return_value = []
+        mock_update_templates_ordering.return_value = []
         response = RequestMock.do_request_patch(
-            template_version_manager_views.TemplateVersionManagerOrdering.as_view(),
+            template_version_manager_views.GlobalTemplateVersionManagerOrdering.as_view(),
             mock_user,
             data={"template_list": []},
         )
 
         self.assertEqual(response.status_code, status.HTTP_200_OK)
 
 
-class TestTemplateVersionManagerListGetPermission(SimpleTestCase):
-    """TestGlobalTemplateVersionManagerListGetPermission"""
+class TestUserTemplateVersionManagerOrderingListGetPermission(SimpleTestCase):
+    """Test Template Version Manager Ordering List Get Permission"""
 
-    @patch.object(template_version_manager_api, "get_all")
     def test_anonymous_returns_http_403(
-        self, template_version_manager_get_all
+        self,
     ):
         """test_anonymous_returns_http_403
 
         Args:
-            template_version_manager_get_all:
 
         Returns:
 
         """
-        template_version_manager_get_all.return_value = TemplateVersionManager(
-            user=None
-        )
-
         response = RequestMock.do_request_get(
-            template_version_manager_views.GlobalAndUserTemplateVersionManagerList.as_view(),
+            template_version_manager_views.UserTemplateVersionManagerOrdering.as_view(),
             None,
         )
-
         self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
 
-    @patch.object(template_version_manager_api, "get_all")
-    def test_authenticated_returns_http_403(
-        self, template_version_manager_get_all
+    @patch.object(template_version_manager_api, "get_all_by_user_id")
+    def test_authenticated_returns_http_200(
+        self, template_version_manager_get_all_by_user_id
     ):
         """test_authenticated_returns_http_200
 
         Args:
-            template_version_manager_get_all:
+            template_version_manager_get_all_by_user_id:
 
         Returns:
 
         """
-        template_version_manager_get_all.return_value = {}
+        template_version_manager_get_all_by_user_id.return_value = {}
 
         mock_user = create_mock_user("1")
 
         response = RequestMock.do_request_get(
-            template_version_manager_views.GlobalAndUserTemplateVersionManagerList.as_view(),
+            template_version_manager_views.UserTemplateVersionManagerOrdering.as_view(),
             mock_user,
         )
 
-        self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
 
-    @patch.object(template_version_manager_api, "get_all")
+    @patch.object(template_version_manager_api, "get_all_by_user_id")
     def test_staff_returns_http_200(self, template_version_manager_get_all):
         """test_staff_returns_http_200
 
         Args:
             template_version_manager_get_all:
 
         Returns:
 
         """
         template_version_manager_get_all.return_value = {}
 
         mock_user = create_mock_user("1", is_staff=True)
 
         response = RequestMock.do_request_get(
-            template_version_manager_views.GlobalAndUserTemplateVersionManagerList.as_view(),
+            template_version_manager_views.UserTemplateVersionManagerOrdering.as_view(),
+            mock_user,
+        )
+
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
+
+    @patch.object(template_version_manager_api, "get_all_by_user_id")
+    def test_superuser_returns_http_200(
+        self, template_version_manager_get_all
+    ):
+        """test_superuser_returns_http_200
+
+        Args:
+            template_version_manager_get_all:
+
+        Returns:
+
+        """
+        template_version_manager_get_all.return_value = {}
+
+        mock_user = create_mock_user("1", is_staff=True, is_superuser=True)
+
+        response = RequestMock.do_request_get(
+            template_version_manager_views.UserTemplateVersionManagerOrdering.as_view(),
+            mock_user,
+        )
+
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
+
+
+class TestUserTemplateVersionManagerOrderingPatchPermission(SimpleTestCase):
+    """Test Template Version Manager Ordering Patch Permission"""
+
+    def test_anonymous_returns_http_403(self):
+        """test_anonymous_returns_http_403
+
+        Returns:
+
+        """
+        response = RequestMock.do_request_patch(
+            template_version_manager_views.UserTemplateVersionManagerOrdering.as_view(),
+            None,
+        )
+        self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
+
+    @patch(
+        "core_main_app.components.template_version_manager.api.get_all_by_user_id"
+    )
+    @patch(
+        "core_main_app.components.template_version_manager.api.update_user_template_ordering"
+    )
+    def test_authenticated_returns_http_200(
+        self,
+        mock_get_all_by_user_id,
+        mock_update_templates_ordering,
+    ):
+        """test_staff_returns_http_200
+
+        Args:
+            mock_get_all_by_user_id:
+            mock_update_templates_ordering:
+
+        Returns:
+
+        """
+        mock_user = create_mock_user("1")
+        mock_get_all_by_user_id.return_value = []
+        mock_update_templates_ordering.return_value = []
+        response = RequestMock.do_request_patch(
+            template_version_manager_views.UserTemplateVersionManagerOrdering.as_view(),
+            mock_user,
+            data={"template_list": []},
+        )
+
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
+
+    @patch(
+        "core_main_app.components.template_version_manager.api.get_by_id_list"
+    )
+    @patch(
+        "core_main_app.components.template_version_manager.api.update_user_template_ordering"
+    )
+    @patch.object(template_version_manager_api, "get_all_by_user_id")
+    def test_staff_returns_http_200(
+        self,
+        mock_get_by_user_id,
+        mock_update_templates_ordering,
+        mock_get_all_by_user_id,
+    ):
+        """test_staff_returns_http_200
+
+        Args:
+            mock_get_all_by_user_id:
+            mock_update_templates_ordering:
+
+        Returns:
+
+        """
+        mock_user = create_mock_user("1", is_staff=True)
+        mock_get_all_by_user_id.return_value = []
+        mock_get_by_user_id.return_value = []
+        mock_update_templates_ordering.return_value = []
+        response = RequestMock.do_request_patch(
+            template_version_manager_views.UserTemplateVersionManagerOrdering.as_view(),
+            mock_user,
+            data={"template_list": []},
+        )
+
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
+
+    @patch(
+        "core_main_app.components.template_version_manager.api.get_by_id_list"
+    )
+    @patch(
+        "core_main_app.components.template_version_manager.api.update_user_template_ordering"
+    )
+    @patch.object(template_version_manager_api, "get_all_by_user_id")
+    def test_superuser_returns_http_200(
+        self,
+        mock_get_by_user_id,
+        mock_update_templates_ordering,
+        mock_get_all_by_user_id,
+    ):
+        """test_superuser_returns_http_200
+
+        Args:
+            mock_get_all_by_user_id:
+            mock_update_templates_ordering:
+
+        Returns:
+
+        """
+        mock_user = create_mock_user("1", is_superuser=True)
+        mock_get_all_by_user_id.return_value = []
+        mock_get_by_user_id.return_value = []
+        mock_update_templates_ordering.return_value = []
+        response = RequestMock.do_request_patch(
+            template_version_manager_views.UserTemplateVersionManagerOrdering.as_view(),
             mock_user,
+            data={"template_list": []},
         )
 
         self.assertEqual(response.status_code, status.HTTP_200_OK)
```

### Comparing `core_main_app-2.3.0/tests/rest/template_version_manager/tests_unit.py` & `core_main_app-2.4.0/tests/rest/template_version_manager/tests_unit.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 from rest_framework import status
 
 from core_main_app.commons.exceptions import DoesNotExist
 from core_main_app.components.template_version_manager.models import (
     TemplateVersionManager,
 )
 from core_main_app.rest.template_version_manager import views
+from core_main_app.rest.template_version_manager.abstract_views import (
+    AbstractOrderingTemplateVersionManager,
+)
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 
 
 class TestGlobalTemplateVersionManagerList(SimpleTestCase):
     """TestGlobalTemplateVersionManagerList"""
 
@@ -135,7 +138,75 @@
             views.TemplateVersionManagerDetail.as_view(),
             mock_user,
             param={"pk": "invalid"},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
+
+
+class TestAbstractOrderingTemplateVersionManager(SimpleTestCase):
+    """Test Abstract Ordering Template Version Manager"""
+
+    def setUp(self):
+        """setUp
+
+        Returns:
+
+        """
+        super().setUp()
+
+    @patch.multiple(
+        AbstractOrderingTemplateVersionManager, __abstractmethods__=set()
+    )
+    def test_get_abstract_ordering_returns_error_500_if_method_is_not_implemented(
+        self,
+    ):
+        """test_get_abstract_ordering_returns_error_500_if_method_is_not_implemented
+
+        Args:
+
+
+        Returns:
+
+        """
+        # Arrange
+        mock_user = create_mock_user("1")
+
+        # Mock
+        response = RequestMock.do_request_get(
+            views.AbstractOrderingTemplateVersionManager.as_view(), mock_user
+        )
+
+        # Assert
+        self.assertEqual(
+            response.status_code, status.HTTP_500_INTERNAL_SERVER_ERROR
+        )
+
+    @patch.multiple(
+        AbstractOrderingTemplateVersionManager, __abstractmethods__=set()
+    )
+    def test_patch_abstract_ordering_returns_error_500_if_method_is_not_implemented(
+        self,
+    ):
+        """test_patch_abstract_ordering_returns_error_500_if_method_is_not_implemented
+
+        Args:
+
+
+        Returns:
+
+        """
+        # Arrange
+        mock_user = create_mock_user("1")
+
+        # Mock
+        response = RequestMock.do_request_patch(
+            views.AbstractOrderingTemplateVersionManager.as_view(),
+            mock_user,
+            data={"template_list": []},
+        )
+
+        # Assert
+        self.assertEqual(
+            response.status_code, status.HTTP_500_INTERNAL_SERVER_ERROR
+        )
```

### Comparing `core_main_app-2.3.0/tests/rest/template_xsl_rendering/tests_int.py` & `core_main_app-2.4.0/tests/rest/template_xsl_rendering/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/rest/template_xsl_rendering/tests_permissions.py` & `core_main_app-2.4.0/tests/rest/template_xsl_rendering/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/rest/tests_views.py` & `core_main_app-2.4.0/tests/rest/tests_views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ Unit test for rest views
 """
 from unittest import TestCase
 from unittest.mock import patch, MagicMock
 
 from django.test import override_settings, tag
+from importlib_metadata import PackageNotFoundError
 
 from core_main_app.rest.views import CoreSettings
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 
 
 class TestCoreSetting(TestCase):
@@ -132,15 +133,15 @@
         """test_main_app_not_found_returns_none
 
         Returns:
 
         """
         # Arrange
         mock_user = create_mock_user("1")
-        version.side_effect = ImportError()
+        version.side_effect = PackageNotFoundError()
 
         # Act
         response = RequestMock.do_request_get(
             CoreSettings.as_view(),
             mock_user,
         )
```

### Comparing `core_main_app-2.3.0/tests/rest/user/tests_int.py` & `core_main_app-2.4.0/tests/rest/user/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/rest/user/tests_permissions.py` & `core_main_app-2.4.0/tests/rest/user/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/rest/user/tests_unit.py` & `core_main_app-2.4.0/tests/rest/user/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/rest/web_page/tests_permission.py` & `core_main_app-2.4.0/tests/rest/web_page/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/rest/workspace/tests_int.py` & `core_main_app-2.4.0/tests/rest/workspace/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/rest/workspace/tests_permissions.py` & `core_main_app-2.4.0/tests/rest/workspace/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/rest/xsl_transformation/fixtures/fixtures.py` & `core_main_app-2.4.0/tests/rest/xsl_transformation/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/rest/xsl_transformation/tests_int.py` & `core_main_app-2.4.0/tests/rest/xsl_transformation/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/rest/xsl_transformation/tests_permission.py` & `core_main_app-2.4.0/tests/rest/xsl_transformation/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/rest/xsl_transformation/tests_unit.py` & `core_main_app-2.4.0/tests/rest/xsl_transformation/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/system/test_unit.py` & `core_main_app-2.4.0/tests/system/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/templatetags/test_get_attribute.py` & `core_main_app-2.4.0/tests/templatetags/test_get_attribute.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/test_settings.py` & `core_main_app-2.4.0/tests/test_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.sites",
     "django.contrib.staticfiles",
     # Extra apps
     "defender",
-    "tz_detect",
     "menu",
     # Local apps
     "core_main_app",
     "core_parser_app",
     "tests",
 ]
 
@@ -55,15 +54,14 @@
     }
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
@@ -101,7 +99,8 @@
 VERIFY_DATA_ACCESS = False
 
 USE_TZ = True
 CHECKSUM_ALGORITHM = "MD5"
 MONGODB_INDEXING = False
 MONGODB_ASYNC_SAVE = False
 DJANGO_SIMPLE_HISTORY_MODELS = []
+BOOTSTRAP_VERSION = "5.1.3"
```

### Comparing `core_main_app-2.3.0/tests/urls.py` & `core_main_app-2.4.0/tests/urls.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 """ Url router for the main application
 """
 from django.conf.urls import include
+from django.contrib.auth import views as auth_views
+from django.contrib.auth.decorators import login_required
 from django.urls import re_path
-from drf_yasg import openapi
-from drf_yasg.views import get_schema_view
 
 from core_main_app.components.blob import api as blob_api
 from core_main_app.components.data import api as data_api
 from core_main_app.utils.rendering import render
 from core_main_app.views.common import (
     ajax as common_ajax,
     views as common_views,
 )
 from core_main_app.views.user import views as user_views, ajax as user_ajax
 
-get_schema_view(
-    openapi.Info(
-        title="REST API",
-        default_version="v1",
-    ),
-)
-
 urlpatterns = [
     re_path(r"^$", user_views.homepage, name="core_main_app_homepage"),
     re_path(r"^login", user_views.custom_login, name="core_main_app_login"),
     re_path(r"^rest/", include("tests.rest_urls")),
     re_path(
         r"^data",
         common_views.ViewData.as_view(),
         name="core_main_app_data_detail",
     ),
     re_path(
+        r"^blob",
+        common_views.ViewBlob.as_view(),
+        name="core_main_app_blob_detail",
+    ),
+    re_path(
+        r"^blob/(?P<pk>[\w-]+)/metadata",
+        login_required(common_views.ManageBlobMetadata.as_view()),
+        name="core_main_app_blob_metadata",
+    ),
+    re_path(
         r"^template/versions/(?P<version_manager_id>\w+)",
         user_views.manage_template_versions,
         name="core_main_app_manage_template_versions",
     ),
     re_path(
         r"^template/(?P<pk>[\w-]+)/edit/$",
         common_ajax.EditTemplateVersionManagerView.as_view(),
@@ -93,19 +96,48 @@
         name="core_main_edit_rights_groups_form",
     ),
     re_path(
         r"^add-group-right-to-workspace",
         user_ajax.add_group_right_to_workspace,
         name="core_main_add_group_right_to_workspace",
     ),
-    re_path(r"^tz_detect/", include("tz_detect.urls")),
     re_path(
         r"^change-data-display",
         user_ajax.change_data_display,
         name="core_main_add_change_data_display",
     ),
     re_path(
         r"^redirect-record",
         user_ajax.change_data_display,
         name="core_dashboard_records",
     ),
+    re_path(
+        r"^add-metadata-form",
+        user_ajax.LoadBlobMetadataForm.as_view(),
+        name="core_main_blob_metadata_form",
+    ),
+    re_path(
+        r"^add-metadata-to-blob",
+        user_ajax.AddMetadataToBlob.as_view(),
+        name="core_main_blob_add_metadata",
+    ),
+    re_path(
+        r"^remove-metadata-from-blob",
+        user_ajax.RemoveMetadataFromBlob.as_view(),
+        name="core_main_blob_remove_metadata",
+    ),
+    re_path(
+        r"^upload-file",
+        user_ajax.UploadFile.as_view(),
+        name="core_main_upload_file",
+    ),
+    re_path(
+        r"^set-timezone",
+        user_views.set_timezone,
+        name="core_main_set_timezone",
+    ),
+    re_path(
+        "password_reset/$",
+        auth_views.PasswordResetView.as_view(),
+        name="password_reset",
+    ),
 ]
```

### Comparing `core_main_app-2.3.0/tests/utils/checksum/tests_checksum.py` & `core_main_app-2.4.0/tests/utils/checksum/tests_checksum.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/utils/migrations/tests_unit.py` & `core_main_app-2.4.0/tests/utils/migrations/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/utils/query/mongo/tests_unit.py` & `core_main_app-2.4.0/tests/utils/query/mongo/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/utils/requests_utls/tests_ssl.py` & `core_main_app-2.4.0/tests/utils/requests_utls/tests_ssl.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/utils/test_unit_apps.py` & `core_main_app-2.4.0/tests/utils/test_unit_apps.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/utils/test_unit_urls.py` & `core_main_app-2.4.0/tests/utils/test_unit_urls.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/utils/tests_int_blob_downloader.py` & `core_main_app-2.4.0/tests/utils/tests_int_blob_downloader.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/utils/tests_int_file.py` & `core_main_app-2.4.0/tests/utils/tests_int_file.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/utils/tests_unit_admin_site.py` & `core_main_app-2.4.0/tests/utils/tests_unit_admin_site.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/utils/tests_unit_boolean.py` & `core_main_app-2.4.0/tests/utils/tests_unit_boolean.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/utils/tests_unit_xml_operation.py` & `core_main_app-2.4.0/tests/utils/tests_unit_xml_operation.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/utils/tests_view_data.py` & `core_main_app-2.4.0/tests/utils/tests_view_data.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/utils/validation/tests_unit_validation.py` & `core_main_app-2.4.0/tests/utils/validation/tests_unit_validation.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/utils/xsd_flattener/tests_unit.py` & `core_main_app-2.4.0/tests/utils/xsd_flattener/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.3.0/tests/views/fixtures.py` & `core_main_app-2.4.0/tests/views/fixtures.py`

 * *Files identical despite different names*

