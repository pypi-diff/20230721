# Comparing `tmp/core_explore_keyword_app-2.3.0.tar.gz` & `tmp/core_explore_keyword_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_explore_keyword_app-2.3.0.tar", last modified: Tue May  2 19:37:55 2023, max compression
+gzip compressed data, was "core_explore_keyword_app-2.4.0.tar", last modified: Fri Jul 21 02:11:48 2023, max compression
```

## Comparing `core_explore_keyword_app-2.3.0.tar` & `core_explore_keyword_app-2.4.0.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:55.300497 core_explore_keyword_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3190 2023-05-02 19:37:55.295951 core_explore_keyword_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2305 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.542646 core_explore_keyword_app-2.3.0/core_explore_keyword_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       95 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1696 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      512 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.651986 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.723610 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/persistent_query_keyword/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/persistent_query_keyword/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/persistent_query_keyword/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2256 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/persistent_query_keyword/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1972 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/persistent_query_keyword/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.774318 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/search_operator/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       34 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/search_operator/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/search_operator/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2367 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/search_operator/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3134 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/search_operator/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1988 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      818 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.802647 core_explore_keyword_app-2.3.0/core_explore_keyword_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3571 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      541 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.852909 core_explore_keyword_app-2.3.0/core_explore_keyword_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1117 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/permissions/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      152 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/permissions/rights.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.902802 core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.944966 core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/persistent_query_keyword/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:49.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/persistent_query_keyword/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3197 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/persistent_query_keyword/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12256 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/persistent_query_keyword/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.997520 core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/search_operators/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/search_operators/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1343 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/search_operators/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7434 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/search_operators/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1688 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      510 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.038404 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.105840 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.049435 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.019501 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      129 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/css/search_ops_manager.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.087281 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_operators.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3599 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      951 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager_delete.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.085800 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.107581 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/stretchy/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2930 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/stretchy/stretchy.min.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.089859 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.098310 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.127486 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/css/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1398 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/css/jquery.tagit.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.162464 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/js/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    23552 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/js/tag-it.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.130344 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.120169 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.182606 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/search/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3476 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/search/search.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.215008 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      320 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/persistent_query.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.303198 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      554 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/autocomplete_source.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/embedded_search.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10050 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/search.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/search.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.155071 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.197289 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.327239 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.342385 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1694 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/box.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.191901 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.372728 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      856 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      705 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/modal.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.386659 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/delete/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      778 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/delete/modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      282 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.475830 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1081 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/embedded_search_bar.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      350 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/extras.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      978 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/index.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      575 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/search_bar.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1415 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/template_filter.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.505218 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templatetags/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templatetags/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1725 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/templatetags/core_explore_keyword_app_search_bar.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1484 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.551290 core_explore_keyword_app-2.3.0/core_explore_keyword_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      689 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/utils/abstract_keyword_search_extras.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2059 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/utils/search_operators.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.567191 core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.625048 core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       43 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3858 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2421 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2389 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.670234 core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6904 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16154 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:53.633334 core_explore_keyword_app-2.3.0/core_explore_keyword_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3190 2023-05-02 19:37:52.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5781 2023-05-02 19:37:52.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:37:52.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2023-05-02 19:37:52.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-05-02 19:37:52.000000 core_explore_keyword_app-2.3.0/core_explore_keyword_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.723987 core_explore_keyword_app-2.3.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11113 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:37:55.302606 core_explore_keyword_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1078 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.759382 core_explore_keyword_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.776020 core_explore_keyword_app-2.3.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.822704 core_explore_keyword_app-2.3.0/tests/components/persistent_query_keyword/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/components/persistent_query_keyword/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.854741 core_explore_keyword_app-2.3.0/tests/components/persistent_query_keyword/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/components/persistent_query_keyword/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1545 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/components/persistent_query_keyword/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15787 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/components/persistent_query_keyword/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12126 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/components/persistent_query_keyword/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.886417 core_explore_keyword_app-2.3.0/tests/components/search_operator/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/components/search_operator/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5362 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/components/search_operator/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.917807 core_explore_keyword_app-2.3.0/tests/forms/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/forms/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1772 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/forms/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.933353 core_explore_keyword_app-2.3.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:54.986933 core_explore_keyword_app-2.3.0/tests/rest/persistent_query_keyword/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:50.000000 core_explore_keyword_app-2.3.0/tests/rest/persistent_query_keyword/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11606 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/rest/persistent_query_keyword/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17581 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/rest/persistent_query_keyword/tests_permissions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:55.114725 core_explore_keyword_app-2.3.0/tests/rest/search_operators/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/rest/search_operators/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9668 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/rest/search_operators/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14457 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/rest/search_operators/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:55.156314 core_explore_keyword_app-2.3.0/tests/templatetags/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/templatetags/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1381 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/templatetags/test_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1929 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:55.171191 core_explore_keyword_app-2.3.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:55.206800 core_explore_keyword_app-2.3.0/tests/utils/search_operators/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/utils/search_operators/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4248 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/utils/search_operators/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:55.220317 core_explore_keyword_app-2.3.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:55.235762 core_explore_keyword_app-2.3.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/views/user/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:55.272966 core_explore_keyword_app-2.3.0/tests/views/user/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/views/user/ajax/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12542 2023-05-02 19:37:51.000000 core_explore_keyword_app-2.3.0/tests/views/user/ajax/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:48.084401 core_explore_keyword_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3190 2023-07-21 02:11:48.079698 core_explore_keyword_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2305 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:46.419682 core_explore_keyword_app-2.4.0/core_explore_keyword_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       95 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1696 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      512 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:46.518049 core_explore_keyword_app-2.4.0/core_explore_keyword_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:46.573370 core_explore_keyword_app-2.4.0/core_explore_keyword_app/components/persistent_query_keyword/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/components/persistent_query_keyword/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/components/persistent_query_keyword/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2256 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/components/persistent_query_keyword/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1972 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/components/persistent_query_keyword/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:46.634470 core_explore_keyword_app-2.4.0/core_explore_keyword_app/components/search_operator/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       34 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/components/search_operator/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/components/search_operator/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2367 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/components/search_operator/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3134 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/components/search_operator/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1988 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      818 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:46.662469 core_explore_keyword_app-2.4.0/core_explore_keyword_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3571 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      541 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:46.724412 core_explore_keyword_app-2.4.0/core_explore_keyword_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1117 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/permissions/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      152 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/permissions/rights.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:46.750560 core_explore_keyword_app-2.4.0/core_explore_keyword_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:46.790944 core_explore_keyword_app-2.4.0/core_explore_keyword_app/rest/persistent_query_keyword/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/rest/persistent_query_keyword/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3197 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/rest/persistent_query_keyword/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12256 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/rest/persistent_query_keyword/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:46.838736 core_explore_keyword_app-2.4.0/core_explore_keyword_app/rest/search_operators/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/rest/search_operators/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1343 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/rest/search_operators/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7434 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/rest/search_operators/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1688 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      510 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:45.970574 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:46.042643 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:45.981139 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:46.856046 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      129 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/css/search_ops_manager.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:46.940479 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_operators.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3599 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      951 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager_delete.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:45.996816 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:46.956417 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/stretchy/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2930 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/stretchy/stretchy.min.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:46.021375 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:46.035207 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:46.974249 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/css/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1398 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/css/jquery.tagit.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:46.988530 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/js/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    23552 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/js/tag-it.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:46.053756 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:46.048961 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.005157 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/search/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3476 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/search/search.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.023319 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      320 2023-07-21 02:11:42.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/persistent_query.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.090134 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      554 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/autocomplete_source.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/embedded_search.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10050 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/search.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/search.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:46.069984 core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:46.100610 core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.109702 core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.124877 core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1687 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/box.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:46.096334 core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.155703 core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      952 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      807 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/modal.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.194283 core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/delete/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      880 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/delete/modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      282 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.259626 core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1081 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/embedded_search_bar.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      350 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/extras.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1020 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/index.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      668 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/search_bar.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1607 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/template_filter.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.286608 core_explore_keyword_app-2.4.0/core_explore_keyword_app/templatetags/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/templatetags/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1725 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/templatetags/core_explore_keyword_app_search_bar.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1484 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.327624 core_explore_keyword_app-2.4.0/core_explore_keyword_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      689 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/utils/abstract_keyword_search_extras.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2059 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/utils/search_operators.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.343219 core_explore_keyword_app-2.4.0/core_explore_keyword_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.396570 core_explore_keyword_app-2.4.0/core_explore_keyword_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       43 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3894 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2421 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2389 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.478612 core_explore_keyword_app-2.4.0/core_explore_keyword_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6859 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16154 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:46.497576 core_explore_keyword_app-2.4.0/core_explore_keyword_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3190 2023-07-21 02:11:45.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5781 2023-07-21 02:11:45.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:11:45.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2023-07-21 02:11:45.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-07-21 02:11:45.000000 core_explore_keyword_app-2.4.0/core_explore_keyword_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.535853 core_explore_keyword_app-2.4.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11113 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:11:48.086342 core_explore_keyword_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1078 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.575662 core_explore_keyword_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.589980 core_explore_keyword_app-2.4.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.645755 core_explore_keyword_app-2.4.0/tests/components/persistent_query_keyword/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/components/persistent_query_keyword/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.679605 core_explore_keyword_app-2.4.0/tests/components/persistent_query_keyword/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/components/persistent_query_keyword/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1545 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/components/persistent_query_keyword/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15787 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/components/persistent_query_keyword/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12126 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/components/persistent_query_keyword/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.709948 core_explore_keyword_app-2.4.0/tests/components/search_operator/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/components/search_operator/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5362 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/components/search_operator/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.741548 core_explore_keyword_app-2.4.0/tests/forms/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/forms/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1772 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/forms/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.756734 core_explore_keyword_app-2.4.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.816469 core_explore_keyword_app-2.4.0/tests/rest/persistent_query_keyword/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/rest/persistent_query_keyword/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11606 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/rest/persistent_query_keyword/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17581 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/rest/persistent_query_keyword/tests_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.887612 core_explore_keyword_app-2.4.0/tests/rest/search_operators/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/rest/search_operators/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9668 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/rest/search_operators/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14457 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/rest/search_operators/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.921519 core_explore_keyword_app-2.4.0/tests/templatetags/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/templatetags/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1381 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/templatetags/test_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1882 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.937863 core_explore_keyword_app-2.4.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.972255 core_explore_keyword_app-2.4.0/tests/utils/search_operators/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/utils/search_operators/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4248 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/utils/search_operators/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:47.987821 core_explore_keyword_app-2.4.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:48.004697 core_explore_keyword_app-2.4.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/views/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:48.040316 core_explore_keyword_app-2.4.0/tests/views/user/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/views/user/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12542 2023-07-21 02:11:43.000000 core_explore_keyword_app-2.4.0/tests/views/user/ajax/tests_unit.py
```

### Comparing `core_explore_keyword_app-2.3.0/LICENSE.md` & `core_explore_keyword_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/PKG-INFO` & `core_explore_keyword_app-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_explore_keyword_app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Exploration by keywords for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_keyword_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ========================
         Core Explore Keyword App
```

### Comparing `core_explore_keyword_app-2.3.0/README.rst` & `core_explore_keyword_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/admin.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/apps.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/persistent_query_keyword/api.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/components/persistent_query_keyword/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/persistent_query_keyword/models.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/components/persistent_query_keyword/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/search_operator/api.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/components/search_operator/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/components/search_operator/models.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/components/search_operator/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/forms.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/forms.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/menus.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/migrations/0001_initial.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/models.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/permissions/discover.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/permissions/discover.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/persistent_query_keyword/serializers.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/rest/persistent_query_keyword/serializers.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/persistent_query_keyword/views.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/rest/persistent_query_keyword/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/search_operators/serializers.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/rest/search_operators/serializers.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/search_operators/views.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/rest/search_operators/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/rest/urls.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager.js` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager_delete.js` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager_delete.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/stretchy/stretchy.min.js` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/stretchy/stretchy.min.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/css/jquery.tagit.css` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/css/jquery.tagit.css`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/js/tag-it.js` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/js/tag-it.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/search/search.css` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/search/search.css`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/autocomplete_source.js` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/autocomplete_source.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/search.js` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/search.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/box.html` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/box.html`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 {% endblock %}
 
 {% block box_body %}
 <p>
     This table lists the current search operators created on the platform. New ones can
     be added using the <a class="link btn-create-operator">new operator button</a>.
 </p>
-<table class="table table-condensed" id="operators-list">
+<table class="table table-sm" id="operators-list">
     <thead>
         <tr>
             <th id="col-op-name">Name</th>
             <th id="col-op-xpath">XPath List</th>
             <th>Actions</th>
         </tr>
     </thead>
```

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/form.html` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/form.html`

 * *Files 25% similar despite different names*

```diff
@@ -11,15 +11,15 @@
             class="form-group has-error"
             {% else %}
             class="form-group"
             {% endif %}
         >
             {{ field.label_tag }}
             {% if field.help_text %}
-                <em class="float-right">{{ field.help_text|safe }}</em>
+                <em class="{% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}">{{ field.help_text|safe }}</em>
             {% endif %}
             {{ field }}
         </div>
         {% if field.errors %}
         <div class="alert alert-danger">{{ field.errors }}</div>
         {% endif %}
     {% endfor %}
```

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/modal.html` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/modal.html`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 
 {% block modal_body %}
 {% include "core_explore_keyword_app/admin/search_ops_manager/modal/config/form.html" with form=data.operator_form %}
 <span class="text-danger" id="operator-modal-form-error">&nbsp;</span>
 {% endblock %}
 
 {% block modal_footer %}
-<button class="btn btn-secondary pull-left" data-dismiss="modal">
+<button class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal">
     <i class="fas fa-times"></i> Cancel
 </button>
 <button id="btn-save-operator" class="btn btn-primary">
     <i class="fas fa-save"></i> Save
 </button>
 {% endblock %}
```

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/delete/modal.html` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/delete/modal.html`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,14 @@
 <p>
     Are you sure you want to delete the operator <span class="operator-name"></span>?
 </p>
 <input type="hidden" id="operator-id"/>
 {% endblock %}
 
 {% block modal_footer %}
-<button class="btn btn-secondary pull-left" data-dismiss="modal">
+<button class="btn btn-secondary pull-left" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-dismiss{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-dismiss{% endif %}="modal">
     <i class="fas fa-times"></i> Cancel
 </button>
 <button id="btn-delete-operator" class="btn btn-danger">
     <i class="fas fa-check"></i> Delete
 </button>
 {% endblock %}
```

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/embedded_search_bar.html` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/embedded_search_bar.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/index.html` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/index.html`

 * *Files 14% similar despite different names*

```diff
@@ -8,20 +8,20 @@
         <div class="alert alert-warning"><i class="fas fa-exclamation-triangle"></i>
             {{ data.warning }}
         </div>
     {% endif %}
     <form id="form_search" action="{% url 'core_explore_keyword_app_search' %}" method="POST">
         {% csrf_token %}
         {% include data.query_builder_interface %}
-        <div class="d-inline-flex col-sm-12">
-            <div class="col-sm-3">
+        <div class="d-inline-flex col-sm-12 extra-padding">
+            <div class="col-sm-3 extra-padding">
                 {% include data.data_sources_selector_template %}
                 {% include 'core_explore_keyword_app/user/template_filter.html' %}
             </div>
-            <div class="col-sm-9">
+            <div class="col-sm-9 extra-padding">
                 {% include "core_explore_common_app/user/results/results.html" %}
             </div>
         </div>
     </form>
 {% endif %}
 {% include "core_explore_keyword_app/user/extras.html" %}
 </div>
```

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/template_filter.html` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/template_filter.html`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <div class="card">
     <div class="card-header">
         <div class="row row-template">
             <div class="col-md-8 col-template">
                 Filter by Template
             </div>
             <div class="pl-0 col-md-4 col-template">
-                <div class="float-right">
+                <div class="{% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}">
                     <a class="selectAllGlobalTemplateButton" href="javascript:void(0)">
                         Select All
                     </a>
                 </div>
             </div>
         </div>
     </div>
@@ -24,15 +24,15 @@
 <div class="card">
     <div class="card-header">
         <div class="row row-template">
             <div class="col-md-9 col-template">
                 Filter by User Template
             </div>
             <div class="pl-0 col-md-3 col-template">
-                <div class="float-right">
+                <div class="{% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3" %}float-end{% endif %}">
                     <a class="selectAllUserTemplateButton" href="javascript:void(0)">
                         Select All
                     </a>
                 </div>
             </div>
         </div>
     </div>
```

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/templatetags/core_explore_keyword_app_search_bar.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/templatetags/core_explore_keyword_app_search_bar.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/urls.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/utils/abstract_keyword_search_extras.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/utils/abstract_keyword_search_extras.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/utils/search_operators.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/utils/search_operators.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/admin/ajax.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/views/admin/ajax.py`

 * *Files 7% similar despite different names*

```diff
@@ -110,15 +110,17 @@
             return JsonResponse({}, status=400)
 
         try:
             operator = search_operator_api.get_by_id(request.POST["id"])
             search_operator_api.delete(operator)
 
             messages.add_message(
-                request, messages.INFO, "Operator %s deleted." % operator.name
+                request,
+                messages.SUCCESS,
+                "Operator %s deleted." % operator.name,
             )
             return JsonResponse({}, status=200)
 
         except ApiError as exception:
             messages.add_message(
                 request,
                 messages.ERROR,
```

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/admin/forms.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/views/admin/forms.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/admin/views.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/user/ajax.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/views/user/ajax.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,9 +204,8 @@
 
     @staticmethod
     def _create_persistent_query(query):
         # create the persistent query
         return PersistentQueryKeyword(
             user_id=query.user_id,
             content=query.content,
-            data_sources=query.data_sources,
         )
```

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app/views/user/views.py` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app.egg-info/PKG-INFO` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-explore-keyword-app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Exploration by keywords for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_keyword_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ========================
         Core Explore Keyword App
```

### Comparing `core_explore_keyword_app-2.3.0/core_explore_keyword_app.egg-info/SOURCES.txt` & `core_explore_keyword_app-2.4.0/core_explore_keyword_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/docs/conf.py` & `core_explore_keyword_app-2.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/setup.py` & `core_explore_keyword_app-2.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_explore_keyword_app",
-    version="2.3.0",
+    version="2.4.0",
     description="Exploration by keywords for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_explore_keyword_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_explore_keyword_app-2.3.0/tests/components/persistent_query_keyword/fixtures/fixtures.py` & `core_explore_keyword_app-2.4.0/tests/components/persistent_query_keyword/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/tests/components/persistent_query_keyword/tests_int_access_control.py` & `core_explore_keyword_app-2.4.0/tests/components/persistent_query_keyword/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/tests/components/persistent_query_keyword/tests_unit.py` & `core_explore_keyword_app-2.4.0/tests/components/persistent_query_keyword/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/tests/components/search_operator/tests_unit.py` & `core_explore_keyword_app-2.4.0/tests/components/search_operator/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/tests/forms/tests_unit.py` & `core_explore_keyword_app-2.4.0/tests/forms/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/tests/rest/persistent_query_keyword/tests_int.py` & `core_explore_keyword_app-2.4.0/tests/rest/persistent_query_keyword/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/tests/rest/persistent_query_keyword/tests_permissions.py` & `core_explore_keyword_app-2.4.0/tests/rest/persistent_query_keyword/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/tests/rest/search_operators/tests_permissions.py` & `core_explore_keyword_app-2.4.0/tests/rest/search_operators/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/tests/rest/search_operators/tests_unit.py` & `core_explore_keyword_app-2.4.0/tests/rest/search_operators/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/tests/templatetags/test_unit.py` & `core_explore_keyword_app-2.4.0/tests/templatetags/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/tests/test_settings.py` & `core_explore_keyword_app-2.4.0/tests/test_settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,15 +37,14 @@
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

### Comparing `core_explore_keyword_app-2.3.0/tests/utils/search_operators/tests_unit.py` & `core_explore_keyword_app-2.4.0/tests/utils/search_operators/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.3.0/tests/views/user/ajax/tests_unit.py` & `core_explore_keyword_app-2.4.0/tests/views/user/ajax/tests_unit.py`

 * *Files identical despite different names*

