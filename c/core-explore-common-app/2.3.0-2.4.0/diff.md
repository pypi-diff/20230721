# Comparing `tmp/core_explore_common_app-2.3.0.tar.gz` & `tmp/core_explore_common_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_explore_common_app-2.3.0.tar", last modified: Tue May  2 19:37:08 2023, max compression
+gzip compressed data, was "core_explore_common_app-2.4.0.tar", last modified: Fri Jul 21 02:11:05 2023, max compression
```

## Comparing `core_explore_common_app-2.3.0.tar` & `core_explore_common_app-2.4.0.tar`

### file list

```diff
@@ -1,168 +1,169 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:08.215032 core_explore_common_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      154 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1108 2023-05-02 19:37:08.209615 core_explore_common_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      607 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.280068 core_explore_common_app-2.3.0/core_explore_common_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       79 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.399536 core_explore_common_app-2.3.0/core_explore_common_app/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4733 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/access_control/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      282 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      450 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.442895 core_explore_common_app-2.3.0/core_explore_common_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      409 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/commons/exceptions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.458115 core_explore_common_app-2.3.0/core_explore_common_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.518655 core_explore_common_app-2.3.0/core_explore_common_app/components/abstract_persistent_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/abstract_persistent_query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2123 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/abstract_persistent_query/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      552 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/abstract_persistent_query/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.550774 core_explore_common_app-2.3.0/core_explore_common_app/components/abstract_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/abstract_query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1583 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/abstract_query/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.624738 core_explore_common_app-2.3.0/core_explore_common_app/components/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/query/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3755 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/query/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1335 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/query/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.664917 core_explore_common_app-2.3.0/core_explore_common_app/components/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/result/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      565 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/components/result/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      172 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/constants.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      876 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/discover.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.692537 core_explore_common_app-2.3.0/core_explore_common_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2499 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.772621 core_explore_common_app-2.3.0/core_explore_common_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.825594 core_explore_common_app-2.3.0/core_explore_common_app/rest/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/rest/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5208 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/rest/query/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.870901 core_explore_common_app-2.3.0/core_explore_common_app/rest/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/rest/result/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      485 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/rest/result/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1768 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/rest/result/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      308 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2200 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:05.872755 core_explore_common_app-2.3.0/core_explore_common_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:05.891308 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:05.883813 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.892797 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/common/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      734 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/common/js/tools.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:05.899977 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.950914 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/css/query_result.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2208 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/css/results.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3484 2023-05-02 19:37:01.000000 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/css/toggle.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.053847 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1629 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/local_selector.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2616 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/persistent_query_config.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8849 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/results.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      479 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/results.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7244 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_multi_criteria.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5507 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_single_criteria.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.091793 core_explore_common_app-2.3.0/core_explore_common_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      190 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/system/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1049 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:05.931352 core_explore_common_app-2.3.0/core_explore_common_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:05.949025 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:05.937948 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.138701 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/admin/persistent_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      300 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/admin/persistent_query/content_query_box.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      342 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/admin/persistent_query/view_query_content.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.154588 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      363 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/commons/query_content.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:05.965870 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.186762 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      592 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/multi_criteria_sorting_menu.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      716 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/single_criteria_sorting_menu.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.252514 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      429 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/button.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      831 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      317 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/persistent_query_content.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3163 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/persistent_query_pagination.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.381616 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/results/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1785 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_info.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1266 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_pagination.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      701 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_results.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2748 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_sources_results.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       92 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/results/results.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.460884 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/selector/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      784 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/selector/data_sources_selector.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      324 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/selector/list_selector_base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/selector/local_content.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      723 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/selector/local_selector.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1359 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.479569 core_explore_common_app-2.3.0/core_explore_common_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.525778 core_explore_common_app-2.3.0/core_explore_common_app/utils/linked_records/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/linked_records/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1003 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/linked_records/pid.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.562912 core_explore_common_app-2.3.0/core_explore_common_app/utils/oaipmh/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/oaipmh/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      597 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/oaipmh/oaipmh.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.627604 core_explore_common_app-2.3.0/core_explore_common_app/utils/protocols/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/protocols/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      263 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/protocols/commons.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3055 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/protocols/oauth2.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.671207 core_explore_common_app-2.3.0/core_explore_common_app/utils/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3361 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/query/query.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.705013 core_explore_common_app-2.3.0/core_explore_common_app/utils/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/result/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1377 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/utils/result/result.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.725114 core_explore_common_app-2.3.0/core_explore_common_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.786955 core_explore_common_app-2.3.0/core_explore_common_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14720 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8846 2023-05-02 19:37:02.000000 core_explore_common_app-2.3.0/core_explore_common_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:06.368117 core_explore_common_app-2.3.0/core_explore_common_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1108 2023-05-02 19:37:05.000000 core_explore_common_app-2.3.0/core_explore_common_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6019 2023-05-02 19:37:05.000000 core_explore_common_app-2.3.0/core_explore_common_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:37:05.000000 core_explore_common_app-2.3.0/core_explore_common_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2023-05-02 19:37:05.000000 core_explore_common_app-2.3.0/core_explore_common_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-05-02 19:37:05.000000 core_explore_common_app-2.3.0/core_explore_common_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:37:08.216755 core_explore_common_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1479 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.835449 core_explore_common_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.849887 core_explore_common_app-2.3.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.870136 core_explore_common_app-2.3.0/tests/components/abstract_persistent_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/components/abstract_persistent_query/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.905773 core_explore_common_app-2.3.0/tests/components/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/components/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7526 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/components/query/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.922651 core_explore_common_app-2.3.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.940600 core_explore_common_app-2.3.0/tests/rest/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/rest/query/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:07.986041 core_explore_common_app-2.3.0/tests/rest/query/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/rest/query/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4103 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/rest/query/views/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:08.039825 core_explore_common_app-2.3.0/tests/rest/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/rest/result/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2544 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/rest/result/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3002 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/rest/result/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1808 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      733 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:08.057256 core_explore_common_app-2.3.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:08.091976 core_explore_common_app-2.3.0/tests/utils/linked_records/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/utils/linked_records/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3655 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/utils/linked_records/tests_pid.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:08.124052 core_explore_common_app-2.3.0/tests/utils/oaipmh/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/utils/oaipmh/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1860 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/utils/oaipmh/tests_oaipmh.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:08.158259 core_explore_common_app-2.3.0/tests/utils/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/utils/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2990 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/utils/query/tests_query.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:08.192794 core_explore_common_app-2.3.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13749 2023-05-02 19:37:03.000000 core_explore_common_app-2.3.0/tests/views/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:05.458336 core_explore_common_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      154 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1108 2023-07-21 02:11:05.453369 core_explore_common_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      607 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:03.909053 core_explore_common_app-2.4.0/core_explore_common_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       79 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.017721 core_explore_common_app-2.4.0/core_explore_common_app/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4733 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/access_control/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      282 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      450 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.043543 core_explore_common_app-2.4.0/core_explore_common_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      409 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/commons/exceptions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.057497 core_explore_common_app-2.4.0/core_explore_common_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.097565 core_explore_common_app-2.4.0/core_explore_common_app/components/abstract_persistent_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/components/abstract_persistent_query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2123 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/components/abstract_persistent_query/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      552 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/components/abstract_persistent_query/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.124222 core_explore_common_app-2.4.0/core_explore_common_app/components/abstract_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/components/abstract_query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1583 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/components/abstract_query/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.174604 core_explore_common_app-2.4.0/core_explore_common_app/components/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/components/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/components/query/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3755 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/components/query/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1335 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/components/query/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.199665 core_explore_common_app-2.4.0/core_explore_common_app/components/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/components/result/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      636 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/components/result/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      172 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/constants.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      876 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/discover.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.236173 core_explore_common_app-2.4.0/core_explore_common_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2499 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      416 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/migrations/0002_result_blob_url.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.265485 core_explore_common_app-2.4.0/core_explore_common_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.290747 core_explore_common_app-2.4.0/core_explore_common_app/rest/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/rest/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5902 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/rest/query/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.328020 core_explore_common_app-2.4.0/core_explore_common_app/rest/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/rest/result/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      485 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/rest/result/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1768 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/rest/result/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      308 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2200 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:03.580283 core_explore_common_app-2.4.0/core_explore_common_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:03.596802 core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:03.585952 core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.356130 core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/common/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      734 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/common/js/tools.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:03.603651 core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.407737 core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/user/css/query_result.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2208 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/user/css/results.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3484 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/user/css/toggle.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.485064 core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1629 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/user/js/local_selector.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2616 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/user/js/persistent_query_config.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8841 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/user/js/results.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      479 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/user/js/results.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7244 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_multi_criteria.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5507 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_single_criteria.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.544297 core_explore_common_app-2.4.0/core_explore_common_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      190 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/system/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1049 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:03.617535 core_explore_common_app-2.4.0/core_explore_common_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:03.633868 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:03.623160 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.572039 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/admin/persistent_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      300 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/admin/persistent_query/content_query_box.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      342 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/admin/persistent_query/view_query_content.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.583244 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      458 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/commons/query_content.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:03.652436 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.628144 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      692 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/multi_criteria_sorting_menu.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      816 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/single_criteria_sorting_menu.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.672219 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      429 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/button.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      914 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      317 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/persistent_query_content.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3163 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/persistent_query_pagination.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.741824 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/results/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2222 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_info.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1266 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_pagination.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      701 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_results.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2948 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_sources_results.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       92 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/results/results.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.793114 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/selector/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      784 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/selector/data_sources_selector.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      324 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/selector/list_selector_base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/selector/local_content.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      723 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/selector/local_selector.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1361 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.808922 core_explore_common_app-2.4.0/core_explore_common_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.836207 core_explore_common_app-2.4.0/core_explore_common_app/utils/linked_records/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/utils/linked_records/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1003 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/utils/linked_records/pid.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.883399 core_explore_common_app-2.4.0/core_explore_common_app/utils/oaipmh/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/utils/oaipmh/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      597 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/utils/oaipmh/oaipmh.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.918959 core_explore_common_app-2.4.0/core_explore_common_app/utils/protocols/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/utils/protocols/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      263 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/utils/protocols/commons.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3055 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/utils/protocols/oauth2.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.944666 core_explore_common_app-2.4.0/core_explore_common_app/utils/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/utils/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3361 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/utils/query/query.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.975225 core_explore_common_app-2.4.0/core_explore_common_app/utils/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/utils/result/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1377 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/utils/result/result.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:04.990229 core_explore_common_app-2.4.0/core_explore_common_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:05.032916 core_explore_common_app-2.4.0/core_explore_common_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14791 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8846 2023-07-21 02:11:00.000000 core_explore_common_app-2.4.0/core_explore_common_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:03.991154 core_explore_common_app-2.4.0/core_explore_common_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1108 2023-07-21 02:11:03.000000 core_explore_common_app-2.4.0/core_explore_common_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6078 2023-07-21 02:11:03.000000 core_explore_common_app-2.4.0/core_explore_common_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:11:03.000000 core_explore_common_app-2.4.0/core_explore_common_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2023-07-21 02:11:03.000000 core_explore_common_app-2.4.0/core_explore_common_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-07-21 02:11:03.000000 core_explore_common_app-2.4.0/core_explore_common_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:11:05.460255 core_explore_common_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1479 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:05.073450 core_explore_common_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:05.105433 core_explore_common_app-2.4.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:05.121528 core_explore_common_app-2.4.0/tests/components/abstract_persistent_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/tests/components/abstract_persistent_query/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:05.154064 core_explore_common_app-2.4.0/tests/components/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/tests/components/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7526 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/tests/components/query/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:05.166103 core_explore_common_app-2.4.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:05.182718 core_explore_common_app-2.4.0/tests/rest/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/tests/rest/query/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:05.215322 core_explore_common_app-2.4.0/tests/rest/query/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/tests/rest/query/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4103 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/tests/rest/query/views/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:05.264657 core_explore_common_app-2.4.0/tests/rest/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/tests/rest/result/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2544 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/tests/rest/result/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3002 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/tests/rest/result/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1808 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      854 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:05.280989 core_explore_common_app-2.4.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:05.329933 core_explore_common_app-2.4.0/tests/utils/linked_records/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/tests/utils/linked_records/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3655 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/tests/utils/linked_records/tests_pid.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:05.372666 core_explore_common_app-2.4.0/tests/utils/oaipmh/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/tests/utils/oaipmh/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1860 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/tests/utils/oaipmh/tests_oaipmh.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:05.407060 core_explore_common_app-2.4.0/tests/utils/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/tests/utils/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2990 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/tests/utils/query/tests_query.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:05.436804 core_explore_common_app-2.4.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/tests/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17451 2023-07-21 02:11:01.000000 core_explore_common_app-2.4.0/tests/views/test_unit.py
```

### Comparing `core_explore_common_app-2.3.0/LICENSE.md` & `core_explore_common_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/PKG-INFO` & `core_explore_common_app-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_explore_common_app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Base exploration function for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_common_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =======================
         Core Explore Common App
```

### Comparing `core_explore_common_app-2.3.0/README.rst` & `core_explore_common_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/access_control/api.py` & `core_explore_common_app-2.4.0/core_explore_common_app/access_control/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/components/abstract_persistent_query/api.py` & `core_explore_common_app-2.4.0/core_explore_common_app/components/abstract_persistent_query/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/components/abstract_persistent_query/models.py` & `core_explore_common_app-2.4.0/core_explore_common_app/components/abstract_persistent_query/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/components/abstract_query/models.py` & `core_explore_common_app-2.4.0/core_explore_common_app/components/abstract_query/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/components/query/api.py` & `core_explore_common_app-2.4.0/core_explore_common_app/components/query/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/components/query/models.py` & `core_explore_common_app-2.4.0/core_explore_common_app/components/query/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/components/result/models.py` & `core_explore_common_app-2.4.0/core_explore_common_app/components/result/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,7 +9,8 @@
     title = models.CharField(blank=False, max_length=200)
     xml_content = models.TextField(blank=False)
     template_info = models.JSONField(default=dict)
     permission_url = models.CharField(blank=True, null=True, max_length=200)
     detail_url = models.CharField(blank=True, null=True, max_length=200)
     access_data_url = models.CharField(blank=True, null=True, max_length=200)
     last_modification_date = models.DateTimeField(blank=True, default=None)
+    blob_url = models.CharField(blank=True, null=True, max_length=200)
```

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/discover.py` & `core_explore_common_app-2.4.0/core_explore_common_app/discover.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/migrations/0001_initial.py` & `core_explore_common_app-2.4.0/core_explore_common_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/rest/query/views.py` & `core_explore_common_app-2.4.0/core_explore_common_app/rest/query/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """ REST views for the query API
 """
 import json
 import logging
 
 import pytz
 from django.conf import settings as conf_settings
-from django.urls import reverse
+from django import urls as django_urls
 
 from core_explore_common_app.components.result.models import Result
 from core_explore_common_app.utils.linked_records import pid as pid_utils
 from core_explore_common_app.utils.result import result as result_utils
+from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.commons.constants import DATA_JSON_FIELD
 from core_main_app.commons.exceptions import ApiError
 from core_main_app.components.data import api as data_api
 from core_main_app.rest.data.abstract_views import (
     AbstractExecuteLocalQueryView,
 )
 from core_main_app.settings import DATA_SORTING_FIELDS, RESULTS_PER_PAGE
@@ -112,19 +113,27 @@
         results:
         request:
 
     Returns:
 
     """
     # Get detail view base url (to be completed with data id)
-    detail_url_base = reverse("core_main_app_data_detail")
-    url_access_data = reverse(
+    data_detail_url_base = django_urls.reverse("core_main_app_data_detail")
+    try:
+        # Get blob url if blob endpoint available
+        blob_detail_url_base = django_urls.reverse("core_main_app_blob_detail")
+    except django_urls.NoReverseMatch:
+        blob_detail_url_base = None
+
+    url_access_data = django_urls.reverse(
         "core_explore_common_app_get_result_from_data_id"
     )
-    url_permission_data = reverse("core_main_app_rest_data_permissions")
+    url_permission_data = django_urls.reverse(
+        "core_main_app_rest_data_permissions"
+    )
 
     # Template info
     template_info = dict()
     # Init data list
     data_list = []
 
     for data in results.object_list:
@@ -132,27 +141,37 @@
         template_id = data.template_id
         # get and store data's template information
         if template_id not in template_info:
             template_info[template_id] = result_utils.get_template_info(
                 data.template
             )
 
-        detail_url = f"{detail_url_base}?id={str(data.id)}"
+        detail_url = f"{data_detail_url_base}?id={str(data.id)}"
 
         # Use the PID link if the app is installed, and a PID is defined for the document
         if pid_utils.auto_set_pid_enabled(
             installed_apps=conf_settings.INSTALLED_APPS
         ):
             pid_url = pid_utils.get_pid_url(data, request)
             # Ensure the PID is set
             detail_url = pid_url if pid_url else detail_url
 
+        # # Get blob attached to data if any
+        try:
+            blob = data.blob(request.user)
+        except AccessControlError:
+            blob = None
+
+        # Add Result to list of results
         data_list.append(
             Result(
                 title=data.title,
+                blob_url=f"{blob_detail_url_base}?id={blob.id}"
+                if blob_detail_url_base and blob
+                else None,
                 xml_content=data.xml_content,
                 template_info=template_info[template_id],
                 permission_url=f'{url_permission_data}?ids=%5B"{str(data.id)}"%5D',
                 detail_url=detail_url,
                 access_data_url=f"{url_access_data}?id={data.id}",
                 last_modification_date=data.last_modification_date.replace(
                     tzinfo=pytz.UTC
```

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/rest/result/views.py` & `core_explore_common_app-2.4.0/core_explore_common_app/rest/result/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/settings.py` & `core_explore_common_app-2.4.0/core_explore_common_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/common/js/tools.js` & `core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/common/js/tools.js`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/css/results.css` & `core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/user/css/results.css`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/css/toggle.css` & `core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/user/css/toggle.css`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/local_selector.js` & `core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/user/js/local_selector.js`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/persistent_query_config.js` & `core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/user/js/persistent_query_config.js`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/results.js` & `core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/user/js/results.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -137,17 +137,15 @@
         data: {
             "id": id
         },
         success: function(data) {
             window.location = data.url;
         },
         error: function(data) {
-            $.notify("Error while opening the edit page.", {
-                style: 'error'
-            });
+            $.notify("Error while opening the edit page.", 'danger');
         }
     }).always(function(data) {
         // get old button icon
         hideSpinner(btnSelector.find("i"), icon)
     });
 };
```

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_multi_criteria.js` & `core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_multi_criteria.js`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_single_criteria.js` & `core_explore_common_app-2.4.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_single_criteria.js`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/tasks.py` & `core_explore_common_app-2.4.0/core_explore_common_app/tasks.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/multi_criteria_sorting_menu.html` & `core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/single_criteria_sorting_menu.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 <div class="filter">
-    <button id="result-button-filter{{data_source_index}}" class="result-toolbar-button" data-toggle="dropdown" aria-haspopup="true"
+    <button id="result-button-filter{{data_source_index}}" class="result-toolbar-button" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-toggle{% elif BOOTSTRAP_VERSION == "5.1.3"%}data-bs-toggle{% endif %}="dropdown" aria-haspopup="true"
             aria-expanded="false">
         <i class="fas fa-sort-amount-up"></i> Sort
     </button>
     <ul class="dropdown-menu tools-menu filter-dropdown-menu" aria-labelledby="result-button-filter{{data_source_index}}">
         {% for item in data_displayed_sorting_fields %}
-            <li data-filter-value="{{item.field}}"><i class="fas fa-random" aria-hidden="true"></i> {{item.display}}</li>
+            <li data-filter-value="{{item.field}}" data-filter-order="{{item.ordering}}">
+                <i class="fas fa-check" aria-hidden="true"></i>
+                <span class="filter-left-padding">{{item.display}}</span>
+            </li>
         {% endfor %}
     </ul>
 </div>
```

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/single_criteria_sorting_menu.html` & `core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/multi_criteria_sorting_menu.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 <div class="filter">
-    <button id="result-button-filter{{data_source_index}}" class="result-toolbar-button" data-toggle="dropdown" aria-haspopup="true"
+    <button id="result-button-filter{{data_source_index}}" class="result-toolbar-button" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-toggle{% elif BOOTSTRAP_VERSION == "5.1.3"%}data-bs-toggle{% endif %}="dropdown" aria-haspopup="true"
             aria-expanded="false">
         <i class="fas fa-sort-amount-up"></i> Sort
     </button>
     <ul class="dropdown-menu tools-menu filter-dropdown-menu" aria-labelledby="result-button-filter{{data_source_index}}">
         {% for item in data_displayed_sorting_fields %}
-            <li data-filter-value="{{item.field}}" data-filter-order="{{item.ordering}}">
-                <i class="fas fa-check" aria-hidden="true"></i>
-                <span class="filter-left-padding">{{item.display}}</span>
-            </li>
+            <li data-filter-value="{{item.field}}"><i class="fas fa-random" aria-hidden="true"></i> {{item.display}}</li>
         {% endfor %}
     </ul>
 </div>
```

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/modal.html` & `core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/modal.html`

 * *Files 15% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 
 {% block modal_title %}Share Query{% endblock %}
 {% block modal_id %}persistent-query-modal{% endblock %}
 {% block modal_input_id %}persistent-query-link{% endblock %}
 {% block modal_submit_id %}persistent-query-submit{% endblock %}
 {% block modal_extra_content %}
     {% if request.user.is_authenticated %}
-        <div class="form-inline" id="rename_tools">
-          <div class="form-group mb-2">
+        <div class="row g-3 align-items-center" id="rename_tools">
+          <div class="col-auto">
             Do you want to name this query?
           </div>
-          <div class="form-group mx-sm-3 mb-2">
-            <input type="text" id="persistent-query-name" placeholder="Query name">
+          <div class="col-5">
+              <input type="text" id="persistent-query-name" class="form-control form-control-lg" placeholder="Query name">
+          </div>
+          <div class="col-auto">
+             <button id="persistent-query-rename" class="btn btn-secondary" disabled="disabled">Rename</button>
           </div>
-          <button id="persistent-query-rename" class="btn btn-secondary" disabled="disabled">Rename</button>
         </div>
     {% endif %}
-{% endblock %}
+{% endblock %}
```

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/persistent_query_pagination.html` & `core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/persistent_query_pagination.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_info.html` & `core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_info.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 {% load json_date %}
+{% load parse_date %}
+{% load tz %}
 
 <div class="result-line-main-container" name="result">
     <div class="result-line-title-container">
         <div class="data-info-left-container">
             <input data-template-id="{{result.template_info.id}}"
                    data-template-hash="{{result.template_info.hash}}"
                    type="checkbox" value="{{ result.access_data_url }}"
@@ -11,26 +13,31 @@
             <span class="result-title">
                 {% if result.detail_url %}
                 <a href="{{ result.detail_url }}">{{ result.title }}</a>
                 {% else %}
                 {{ result.title }}
                 {% endif %}
             </span>
+            {% if result.blob_url %}
+            <a href="{{ result.blob_url }}" class="badge rounded-pill bg-secondary">
+            file
+            </a>
+            {% endif %}
             <span class="template-info-name">{{result.template_info.name}}</span>
             {% if result.permission_url and display_edit_button %}
                 <input class="input-permission-url" type="hidden" value="{{result.permission_url}}">
-                <a class="permissions-link-open mx-2" href="#" data-toggle="tooltip" title="Open in text editor">
+                <a class="permissions-link-open mx-2" href="#" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-toggle{% elif BOOTSTRAP_VERSION == "5.1.3"%}data-bs-toggle{% endif %}="tooltip" title="Open in text editor">
                     <i class="fas fa-code" aria-hidden="true"></i>
                 </a>
-                <a class="permissions-link mx-2" href="#" data-toggle="tooltip" title="Edit">
+                <a class="permissions-link mx-2" href="#" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-toggle{% elif BOOTSTRAP_VERSION == "5.1.3"%}data-bs-toggle{% endif %}="tooltip" title="Edit">
                     <i class="fas fa-pencil-alt permissions-icon edit" aria-hidden="true"></i>
                 </a>
             {% endif %}
             <div title="Last modification date" class="data-info-right-container">
-                {{result.last_modification_date|json_date:"N d Y g:iA"}}
+                {{result.last_modification_date|parse_date|localtime|json_date:"N d Y g:iA"}}
             </div>
         </div>
     </div>
     <div class='xmlResult' readonly='true'>
     {{ xml_representation }}
     </div>
 </div>
```

#### html2text {}

```diff
@@ -1,6 +1,13 @@
-{% load json_date %}
+{% load json_date %} {% load parse_date %} {% load tz %}
 ⁰   {% if result.detail_url %} {{_result.title_}} {% else %} {{ result.title }}
-{% endif %}  {{result.template_info.name}} {% if result.permission_url and
-display_edit_button %}    {% endif %}
-{{result.last_modification_date|json_date:"N d Y g:iA"}}
+{% endif %}  {% if result.blob_url %} file {% endif %} {
+{result.template_info.name}} {% if result.permission_url and
+display_edit_button %}
+% if BOOTSTRAP_VERSION == "4.6.2" %}data-toggle{% elif BOOTSTRAP_VERSION ==
+"5.1.3"%}data-bs-toggle{% endif %}="tooltip" title="Open in text editor">
+
+% if BOOTSTRAP_VERSION == "4.6.2" %}data-toggle{% elif BOOTSTRAP_VERSION ==
+"5.1.3"%}data-bs-toggle{% endif %}="tooltip" title="Edit">
+ {% endif %}
+{{result.last_modification_date|parse_date|localtime|json_date:"N d Y g:iA"}}
 {{ xml_representation }}
```

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_pagination.html` & `core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_pagination.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_results.html` & `core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_results.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_sources_results.html` & `core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_sources_results.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <div>
     {% if query.data_sources|length > 0 %}
         <ul class="nav nav-tabs"role="tablist">
             {% for data_source in query.data_sources %}
             <li role="presentation" class="nav-item">
-                <a class="nav-link{% if forloop.counter0 == 0 %} active {% endif %}" href="#results_{{forloop.counter0}}" id="tab_results_{{forloop.counter0}}" aria-controls="profile" role="tab" data-toggle="tab">
+                <a class="nav-link{% if forloop.counter0 == 0 %} active {% endif %}" href="#results_{{forloop.counter0}}" id="tab_results_{{forloop.counter0}}" aria-controls="profile" role="tab" {% if BOOTSTRAP_VERSION == "4.6.2" %}data-toggle{% elif BOOTSTRAP_VERSION == "5.1.3" %}data-bs-toggle{% endif %}="tab">
                     From {{ data_source.name }}
-                    <span class="badge badge-secondary" id="results_infos_{{forloop.counter0}}">-</span>
+                    <span class="badge {% if BOOTSTRAP_VERSION == "4.6.2" %}badge-secondary{% elif BOOTSTRAP_VERSION == "5.1.3" %}bg-secondary{% endif %}" id="results_infos_{{forloop.counter0}}">-</span>
                 </a>
             </li>
             {% endfor %}
         </ul>
         <div class="tab-content">
         {% for data_source in query.data_sources %}
             <div role="tabpanel" class="results-container tab-pane {% if forloop.counter0 == 0 %} active {% endif %} results-page"
```

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/selector/data_sources_selector.html` & `core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/selector/data_sources_selector.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/templates/core_explore_common_app/user/selector/local_selector.html` & `core_explore_common_app-2.4.0/core_explore_common_app/templates/core_explore_common_app/user/selector/local_selector.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/urls.py` & `core_explore_common_app-2.4.0/core_explore_common_app/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,20 @@
     ),
     re_path(
         r"^data-sources-html",
         user_ajax.get_data_sources_html,
         name="core_explore_common_data_sources_html",
     ),
     re_path(
-        r"^data-source-results/(?P<query_id>\w+)/(?P<data_source_index>\w+)/(?P<page>\w+)",
+        r"^data-source-results/(?P<query_id>\w+)/(?P<data_source_index>\w+)/(?P<page>\w+)$",
         user_ajax.get_data_source_results,
         name="core_explore_common_data_source_results",
     ),
     re_path(
-        r"^data-source-results/(?P<query_id>\w+)/(?P<data_source_index>\w+)",
+        r"^data-source-results/(?P<query_id>\w+)/(?P<data_source_index>\w+)$",
         user_ajax.get_data_source_results,
         name="core_explore_common_data_source_results",
     ),
     re_path(
         r"^(?P<persistent_query_type>\w+)/(?P<persistent_query_id>\w+)",
         user_ajax.ContentPersistentQueryView.as_view(),
         name="core_explore_common_persistent_query_content",
```

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/utils/linked_records/pid.py` & `core_explore_common_app-2.4.0/core_explore_common_app/utils/linked_records/pid.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/utils/oaipmh/oaipmh.py` & `core_explore_common_app-2.4.0/core_explore_common_app/utils/oaipmh/oaipmh.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/utils/protocols/oauth2.py` & `core_explore_common_app-2.4.0/core_explore_common_app/utils/protocols/oauth2.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/utils/query/query.py` & `core_explore_common_app-2.4.0/core_explore_common_app/utils/query/query.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/utils/result/result.py` & `core_explore_common_app-2.4.0/core_explore_common_app/utils/result/result.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/views/user/ajax.py` & `core_explore_common_app-2.4.0/core_explore_common_app/views/user/ajax.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from core_explore_common_app.utils.oaipmh import oaipmh as oaipmh_utils
 from core_explore_common_app.utils.query import query as query_utils
 from core_explore_common_app.access_control import (
     api as explore_common_acl_api,
 )
 from core_main_app.access_control.decorators import access_control
 from core_main_app.commons.exceptions import DoesNotExist
-from core_main_app.settings import SERVER_URI
+from core_main_app.settings import SERVER_URI, BOOTSTRAP_VERSION
 from core_main_app.utils.pagination.rest_framework_paginator.rest_framework_paginator import (
     get_page_number,
 )
 from core_main_app.views.common.views import CommonView
 
 
 @access_control(explore_common_acl_api.can_access_explore_views)
@@ -155,14 +155,15 @@
         # set query in context
         context = {
             "linked_records_app": is_linked_records_installed,
             "exporter_app": "core_exporters_app" in settings.INSTALLED_APPS,
             "sorting_display_type": settings.SORTING_DISPLAY_TYPE,
             "data_displayed_sorting_fields": settings.DATA_DISPLAYED_SORTING_FIELDS,
             "default_date_toggle_value": settings.DEFAULT_DATE_TOGGLE_VALUE,
+            "BOOTSTRAP_VERSION": BOOTSTRAP_VERSION,
         }
         context.update({"query": query})
 
         # render html results
         html_template = loader.get_template(
             join(
                 "core_explore_common_app",
```

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app/views/user/views.py` & `core_explore_common_app-2.4.0/core_explore_common_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app.egg-info/PKG-INFO` & `core_explore_common_app-2.4.0/core_explore_common_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-explore-common-app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Base exploration function for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_common_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =======================
         Core Explore Common App
```

### Comparing `core_explore_common_app-2.3.0/core_explore_common_app.egg-info/SOURCES.txt` & `core_explore_common_app-2.4.0/core_explore_common_app.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 core_explore_common_app/components/query/__init__.py
 core_explore_common_app/components/query/admin_site.py
 core_explore_common_app/components/query/api.py
 core_explore_common_app/components/query/models.py
 core_explore_common_app/components/result/__init__.py
 core_explore_common_app/components/result/models.py
 core_explore_common_app/migrations/0001_initial.py
+core_explore_common_app/migrations/0002_result_blob_url.py
 core_explore_common_app/migrations/__init__.py
 core_explore_common_app/rest/__init__.py
 core_explore_common_app/rest/urls.py
 core_explore_common_app/rest/query/__init__.py
 core_explore_common_app/rest/query/views.py
 core_explore_common_app/rest/result/__init__.py
 core_explore_common_app/rest/result/serializers.py
```

### Comparing `core_explore_common_app-2.3.0/setup.py` & `core_explore_common_app-2.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 chdir(normpath(join(abspath(__file__), pardir)))
 
 dep_links = [r for r in required if r.startswith("https://")]
 required = [req_link(r) if r.startswith("https://") else r for r in required]
 
 setup(
     name="core_explore_common_app",
-    version="2.3.0",
+    version="2.4.0",
     description="Base exploration function for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_explore_common_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_explore_common_app-2.3.0/tests/components/query/tests_unit.py` & `core_explore_common_app-2.4.0/tests/components/query/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/tests/rest/query/views/tests_unit.py` & `core_explore_common_app-2.4.0/tests/rest/query/views/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/tests/rest/result/tests_permissions.py` & `core_explore_common_app-2.4.0/tests/rest/result/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/tests/rest/result/tests_unit.py` & `core_explore_common_app-2.4.0/tests/rest/result/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/tests/test_settings.py` & `core_explore_common_app-2.4.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/tests/urls.py` & `core_explore_common_app-2.4.0/tests/urls.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,8 +20,13 @@
         name="core_main_app_rest_data_permissions",
     ),
     re_path(
         r"^result",
         result_views.get_result_from_data_id,
         name="core_explore_common_app_get_result_from_data_id",
     ),
+    re_path(
+        r"^blob",
+        common_views.ViewBlob.as_view(),
+        name="core_main_app_blob_detail",
+    ),
 ]
```

### Comparing `core_explore_common_app-2.3.0/tests/utils/linked_records/tests_pid.py` & `core_explore_common_app-2.4.0/tests/utils/linked_records/tests_pid.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/tests/utils/oaipmh/tests_oaipmh.py` & `core_explore_common_app-2.4.0/tests/utils/oaipmh/tests_oaipmh.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/tests/utils/query/tests_query.py` & `core_explore_common_app-2.4.0/tests/utils/query/tests_query.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.3.0/tests/views/test_unit.py` & `core_explore_common_app-2.4.0/tests/views/test_unit.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """ Unit test views
 """
 from unittest.mock import patch, MagicMock
 
 from django.core.paginator import EmptyPage
 from django.test import RequestFactory, SimpleTestCase
+from django.urls import NoReverseMatch
 
 from core_explore_common_app.constants import LOCAL_QUERY_NAME
+from core_explore_common_app.rest.query.views import format_local_results
 from core_explore_common_app.settings import SERVER_URI
 from core_explore_common_app.views.user.ajax import (
     get_local_data_source,
     get_data_source_results,
     update_local_data_source,
 )
 from core_explore_common_app.views.user.views import ResultQueryRedirectView
+from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import create_mock_request
 
 
 class TestGetLocalDataSource(SimpleTestCase):
     """TestGetLocalDataSource"""
 
@@ -401,14 +404,129 @@
         url = view.get_redirect_url()
 
         # Assert
         self.assertTrue(mock_add_local_data_source.called)
         self.assertTrue(url, "url")
 
 
+class TestFormatLocalResults(SimpleTestCase):
+    """TestFormatLocalResults"""
+
+    def setUp(self):
+        """setUp
+
+        Returns:
+
+        """
+        self.factory = RequestFactory()
+        self.user1 = create_mock_user(user_id="1")
+
+    @patch(
+        "core_explore_common_app.utils.linked_records.pid.auto_set_pid_enabled"
+    )
+    @patch("core_explore_common_app.utils.result.result.get_template_info")
+    @patch("django.urls.reverse")
+    def test_format_local_results_with_blob_url(
+        self, mock_reverse, mock_get_template_info, mock_auto_set_pid_enabled
+    ):
+        """test_format_local_results_with_blob_url
+
+        Returns:
+
+        """
+
+        def _side_effect_blob_url_exists(*args, **kwargs):
+            if args[0] == "core_main_app_blob_detail":
+                return "/blob"
+            else:
+                return ""
+
+        mock_auto_set_pid_enabled.return_value = False
+        request = MagicMock()
+        mock_get_template_info.return_value = MagicMock()
+        mock_data = MagicMock()
+        mock_data.template_id = None
+        mock_data_list = [mock_data]
+
+        results = MagicMock()
+        results.object_list = mock_data_list
+
+        mock_reverse.side_effect = _side_effect_blob_url_exists
+
+        data_list = format_local_results(results, request)
+
+        self.assertTrue("/blob" in data_list[0].blob_url)
+
+    @patch(
+        "core_explore_common_app.utils.linked_records.pid.auto_set_pid_enabled"
+    )
+    @patch("core_explore_common_app.utils.result.result.get_template_info")
+    @patch("django.urls.reverse")
+    def test_format_local_results_without_blob_url(
+        self, mock_reverse, mock_get_template_info, mock_auto_set_pid_enabled
+    ):
+        """test_format_local_results_without_blob_url
+
+        Returns:
+
+        """
+
+        def _side_effect_blob_url_does_not_exists(*args, **kwargs):
+            if args[0] == "core_main_app_blob_detail":
+                raise NoReverseMatch()
+            else:
+                return ""
+
+        mock_auto_set_pid_enabled.return_value = False
+        request = MagicMock()
+        mock_get_template_info.return_value = MagicMock()
+        mock_data = MagicMock()
+        mock_data.template_id = None
+        mock_data_list = [mock_data]
+
+        results = MagicMock()
+        results.object_list = mock_data_list
+
+        mock_reverse.side_effect = _side_effect_blob_url_does_not_exists
+
+        data_list = format_local_results(results, request)
+
+        self.assertIsNone(data_list[0].blob_url)
+
+    @patch(
+        "core_explore_common_app.utils.linked_records.pid.auto_set_pid_enabled"
+    )
+    @patch("core_explore_common_app.utils.result.result.get_template_info")
+    @patch("django.urls.reverse")
+    def test_format_local_results_with_acl_error_when_getting_blob(
+        self, mock_reverse, mock_get_template_info, mock_auto_set_pid_enabled
+    ):
+        """test_format_local_results_with_acl_error_when_getting_blob
+
+        Returns:
+
+        """
+        mock_auto_set_pid_enabled.return_value = False
+        request = MagicMock()
+        mock_get_template_info.return_value = MagicMock()
+        mock_data = MagicMock()
+        mock_data.blob.side_effect = AccessControlError("error")
+        mock_data.template_id = None
+        mock_data_list = [mock_data]
+
+        results = MagicMock()
+        results.object_list = mock_data_list
+
+        mock_reverse.return_value = ""
+
+        data_list = format_local_results(results, request)
+
+        self.assertIsNone(data_list[0].blob_url)
+
+
 class TestRQRView(ResultQueryRedirectView):
     """TestRQRView"""
 
     @staticmethod
     def _get_persistent_query_by_id(persistent_query_id, user):
         persistent_query = MagicMock()
         persistent_query.content = {}
```

