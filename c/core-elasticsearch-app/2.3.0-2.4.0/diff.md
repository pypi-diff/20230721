# Comparing `tmp/core_elasticsearch_app-2.3.0.tar.gz` & `tmp/core_elasticsearch_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_elasticsearch_app-2.3.0.tar", last modified: Tue May  2 19:36:47 2023, max compression
+gzip compressed data, was "core_elasticsearch_app-2.4.0.tar", last modified: Fri Jul 21 02:10:52 2023, max compression
```

## Comparing `core_elasticsearch_app-2.3.0.tar` & `core_elasticsearch_app-2.4.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:47.453138 core_elasticsearch_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2933 2023-05-02 19:36:47.447807 core_elasticsearch_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2144 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:46.816040 core_elasticsearch_app-2.3.0/core_elasticsearch_app/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      124 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1820 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1251 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:46.930312 core_elasticsearch_app-2.3.0/core_elasticsearch_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      190 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/commons/exceptions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:46.941505 core_elasticsearch_app-2.3.0/core_elasticsearch_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:47.017912 core_elasticsearch_app-2.3.0/core_elasticsearch_app/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/components/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1012 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/components/data/autocomplete_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2955 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/components/data/elasticsearch.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1404 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/components/data/mongodb.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1084 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/components/data/watch.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:47.052483 core_elasticsearch_app-2.3.0/core_elasticsearch_app/components/elasticsearch_template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/components/elasticsearch_template/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      991 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/components/elasticsearch_template/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2087 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/components/elasticsearch_template/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      355 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:47.071978 core_elasticsearch_app-2.3.0/core_elasticsearch_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1536 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:47.110525 core_elasticsearch_app-2.3.0/core_elasticsearch_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:47.157648 core_elasticsearch_app-2.3.0/core_elasticsearch_app/rest/elasticsearch_template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/rest/elasticsearch_template/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1128 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/rest/elasticsearch_template/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3630 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/rest/elasticsearch_template/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      771 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2890 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/rest/views.py
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1237 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:46.569762 core_elasticsearch_app-2.3.0/core_elasticsearch_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:46.556345 core_elasticsearch_app-2.3.0/core_elasticsearch_app/static/core_elasticsearch_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:47.168556 core_elasticsearch_app-2.3.0/core_elasticsearch_app/static/core_elasticsearch_app/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      431 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/static/core_elasticsearch_app/css/search_box.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:47.180310 core_elasticsearch_app-2.3.0/core_elasticsearch_app/static/core_elasticsearch_app/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:47.192463 core_elasticsearch_app-2.3.0/core_elasticsearch_app/static/core_elasticsearch_app/js/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      771 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/static/core_elasticsearch_app/js/admin/es_template.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1709 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/static/core_elasticsearch_app/js/search_box.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:46.573118 core_elasticsearch_app-2.3.0/core_elasticsearch_app/static/core_explore_keyword_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:46.583349 core_elasticsearch_app-2.3.0/core_elasticsearch_app/static/core_explore_keyword_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:46.589628 core_elasticsearch_app-2.3.0/core_elasticsearch_app/static/core_explore_keyword_app/user/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:47.216935 core_elasticsearch_app-2.3.0/core_elasticsearch_app/static/core_explore_keyword_app/user/js/search/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      467 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/static/core_explore_keyword_app/user/js/search/autocomplete_source.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      167 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/static/core_explore_keyword_app/user/js/search/search.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1385 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:46.633455 core_elasticsearch_app-2.3.0/core_elasticsearch_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:47.229775 core_elasticsearch_app-2.3.0/core_elasticsearch_app/templates/core_elasticsearch_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:46.620677 core_elasticsearch_app-2.3.0/core_elasticsearch_app/templates/core_elasticsearch_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:47.242564 core_elasticsearch_app-2.3.0/core_elasticsearch_app/templates/core_elasticsearch_app/admin/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:47.253192 core_elasticsearch_app-2.3.0/core_elasticsearch_app/templates/core_elasticsearch_app/admin/templates/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2587 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/templates/core_elasticsearch_app/admin/templates/list/list_base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      346 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/templates/core_elasticsearch_app/admin/templates/list_templates.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      603 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/templates/core_elasticsearch_app/search_box.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:46.645052 core_elasticsearch_app-2.3.0/core_elasticsearch_app/templates/core_explore_keyword_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:47.265290 core_elasticsearch_app-2.3.0/core_elasticsearch_app/templates/core_explore_keyword_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      590 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/templates/core_explore_keyword_app/user/embedded_search_bar.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      176 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:47.310288 core_elasticsearch_app-2.3.0/core_elasticsearch_app/utils/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/utils/__init__.py
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     2432 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/utils/elasticsearch_client.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      866 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/utils/utils.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:47.325416 core_elasticsearch_app-2.3.0/core_elasticsearch_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:47.402952 core_elasticsearch_app-2.3.0/core_elasticsearch_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5172 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2925 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1552 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:46.889817 core_elasticsearch_app-2.3.0/core_elasticsearch_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2933 2023-05-02 19:36:46.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2686 2023-05-02 19:36:46.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:36:46.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2023-05-02 19:36:46.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       29 2023-05-02 19:36:46.000000 core_elasticsearch_app-2.3.0/core_elasticsearch_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       53 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/requirements.core.txt
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)       29 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:36:47.455003 core_elasticsearch_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1388 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:47.435573 core_elasticsearch_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1106 2023-05-02 19:36:44.000000 core_elasticsearch_app-2.3.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:52.175343 core_elasticsearch_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2933 2023-07-21 02:10:52.170499 core_elasticsearch_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2144 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.503945 core_elasticsearch_app-2.4.0/core_elasticsearch_app/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      124 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1820 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1251 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.611187 core_elasticsearch_app-2.4.0/core_elasticsearch_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      190 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/commons/exceptions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.623181 core_elasticsearch_app-2.4.0/core_elasticsearch_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.713543 core_elasticsearch_app-2.4.0/core_elasticsearch_app/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/components/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1012 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/components/data/autocomplete_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2955 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/components/data/elasticsearch.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1404 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/components/data/mongodb.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1084 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/components/data/watch.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.752630 core_elasticsearch_app-2.4.0/core_elasticsearch_app/components/elasticsearch_template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/components/elasticsearch_template/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      991 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/components/elasticsearch_template/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2087 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/components/elasticsearch_template/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      355 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.774607 core_elasticsearch_app-2.4.0/core_elasticsearch_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1536 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.820150 core_elasticsearch_app-2.4.0/core_elasticsearch_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.854032 core_elasticsearch_app-2.4.0/core_elasticsearch_app/rest/elasticsearch_template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/rest/elasticsearch_template/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1128 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/rest/elasticsearch_template/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3630 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/rest/elasticsearch_template/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      771 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2890 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/rest/views.py
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1237 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.227442 core_elasticsearch_app-2.4.0/core_elasticsearch_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.215368 core_elasticsearch_app-2.4.0/core_elasticsearch_app/static/core_elasticsearch_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.866162 core_elasticsearch_app-2.4.0/core_elasticsearch_app/static/core_elasticsearch_app/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      431 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/static/core_elasticsearch_app/css/search_box.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.881195 core_elasticsearch_app-2.4.0/core_elasticsearch_app/static/core_elasticsearch_app/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.903197 core_elasticsearch_app-2.4.0/core_elasticsearch_app/static/core_elasticsearch_app/js/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      771 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/static/core_elasticsearch_app/js/admin/es_template.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1709 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/static/core_elasticsearch_app/js/search_box.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.230465 core_elasticsearch_app-2.4.0/core_elasticsearch_app/static/core_explore_keyword_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.233428 core_elasticsearch_app-2.4.0/core_elasticsearch_app/static/core_explore_keyword_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.236295 core_elasticsearch_app-2.4.0/core_elasticsearch_app/static/core_explore_keyword_app/user/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.925959 core_elasticsearch_app-2.4.0/core_elasticsearch_app/static/core_explore_keyword_app/user/js/search/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      467 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/static/core_explore_keyword_app/user/js/search/autocomplete_source.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      167 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/static/core_explore_keyword_app/user/js/search/search.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1385 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.260878 core_elasticsearch_app-2.4.0/core_elasticsearch_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.937669 core_elasticsearch_app-2.4.0/core_elasticsearch_app/templates/core_elasticsearch_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.252185 core_elasticsearch_app-2.4.0/core_elasticsearch_app/templates/core_elasticsearch_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.949391 core_elasticsearch_app-2.4.0/core_elasticsearch_app/templates/core_elasticsearch_app/admin/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.974239 core_elasticsearch_app-2.4.0/core_elasticsearch_app/templates/core_elasticsearch_app/admin/templates/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2682 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/templates/core_elasticsearch_app/admin/templates/list/list_base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      346 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/templates/core_elasticsearch_app/admin/templates/list_templates.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      788 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/templates/core_elasticsearch_app/search_box.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.263668 core_elasticsearch_app-2.4.0/core_elasticsearch_app/templates/core_explore_keyword_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.984812 core_elasticsearch_app-2.4.0/core_elasticsearch_app/templates/core_explore_keyword_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      590 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/templates/core_explore_keyword_app/user/embedded_search_bar.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      176 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:52.032978 core_elasticsearch_app-2.4.0/core_elasticsearch_app/utils/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/utils/__init__.py
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     2432 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/utils/elasticsearch_client.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      866 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/utils/utils.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:52.049138 core_elasticsearch_app-2.4.0/core_elasticsearch_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:52.120894 core_elasticsearch_app-2.4.0/core_elasticsearch_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5172 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2925 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1552 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:51.574440 core_elasticsearch_app-2.4.0/core_elasticsearch_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2933 2023-07-21 02:10:50.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2686 2023-07-21 02:10:51.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:10:50.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2023-07-21 02:10:50.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       29 2023-07-21 02:10:50.000000 core_elasticsearch_app-2.4.0/core_elasticsearch_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       53 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/requirements.core.txt
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)       29 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:10:52.177342 core_elasticsearch_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1388 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:52.153537 core_elasticsearch_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1106 2023-07-21 02:10:49.000000 core_elasticsearch_app-2.4.0/tests/test_settings.py
```

### Comparing `core_elasticsearch_app-2.3.0/LICENSE.md` & `core_elasticsearch_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/PKG-INFO` & `core_elasticsearch_app-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_elasticsearch_app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Elasticsearch utils for the curator core project
 Home-page: https://github.com/usnistgov/core_elasticsearch_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ======================
         Core Elasticsearch App
```

### Comparing `core_elasticsearch_app-2.3.0/README.rst` & `core_elasticsearch_app-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/admin.py` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/apps.py` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/components/data/autocomplete_settings.py` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/components/data/autocomplete_settings.py`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/components/data/elasticsearch.py` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/components/data/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/components/data/mongodb.py` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/components/data/mongodb.py`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/components/data/watch.py` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/components/data/watch.py`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/components/elasticsearch_template/api.py` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/components/elasticsearch_template/api.py`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/components/elasticsearch_template/models.py` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/components/elasticsearch_template/models.py`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/migrations/0001_initial.py` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/rest/elasticsearch_template/serializers.py` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/rest/elasticsearch_template/serializers.py`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/rest/elasticsearch_template/views.py` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/rest/elasticsearch_template/views.py`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/rest/urls.py` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/rest/views.py` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/rest/views.py`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/settings.py` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/static/core_elasticsearch_app/js/admin/es_template.js` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/static/core_elasticsearch_app/js/admin/es_template.js`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/static/core_elasticsearch_app/js/search_box.js` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/static/core_elasticsearch_app/js/search_box.js`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/tasks.py` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/tasks.py`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/templates/core_elasticsearch_app/admin/templates/list/list_base.html` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/templates/core_elasticsearch_app/admin/templates/list/list_base.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %}
 
 {% block box_title %}List all template configurations{% endblock %}
 
 {% block box_tools %}
-<div class="btn-group float-right">
+<div class="btn-group {% if BOOTSTRAP_VERSION == "4.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3"%}float-end{% endif %}">
 {% url 'core-admin:core_elasticsearch_app_templates_add' as add_url %}
 {% include 'core_main_app/common/buttons/add.html' with label='Add Template Configuration' %}
 </div>
 {% endblock %}
 
 {% block box_body %}
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% block
 box_title %}List all template configurations{% endblock %} {% block box_tools
 %}
+.6.2" %}float-right{% elif BOOTSTRAP_VERSION == "5.1.3"%}float-end{% endif %}">
 {% url 'core-admin:core_elasticsearch_app_templates_add' as add_url %} {%
 include 'core_main_app/common/buttons/add.html' with label='Add Template
 Configuration' %}
 {% endblock %} {% block box_body %}
 Template Name                     Title                  Description                         Actions
                                                                                              {% block box_actions %} {% url 'core-
                                                                                              admin:
```

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/templates/core_elasticsearch_app/search_box.html` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/templates/core_explore_keyword_app/user/embedded_search_bar.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 {% load static %}
+
 <script src="{% static 'core_explore_common_app/common/js/tools.js' %}"></script>
 <script src="{% static 'core_elasticsearch_app/js/search_box.js' %}"></script>
 <link rel="stylesheet" type="text/css" href="{% static 'core_elasticsearch_app/css/search_box.css' %}">
 
-
-<form class="form-inline mr-auto">
-  <div class="md-form my-0">
-    <input id="es_search_box_input" class="form-control es_search_box_input hidden" type="text"
-           placeholder="Search..." aria-label="Search">
-    <i class="es_search_icon fas fa-search text-white ml-3" aria-hidden="true"></i>
-  </div>
-</form>
-
+<div class="container">
+    <form>
+      <div class="row">
+          <div class="col-sm-12">
+                  <input id="es_search_box_input" class="form-control es_search_box_input" type="text"
+               placeholder="Search..." aria-label="Search">
+          </div>
+      </div>
+    </form>
+</div>
```

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/utils/elasticsearch_client.py` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/utils/elasticsearch_client.py`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/utils/utils.py` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/utils/utils.py`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/views/admin/ajax.py` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/views/admin/ajax.py`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/views/admin/forms.py` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/views/admin/forms.py`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app/views/admin/views.py` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app.egg-info/PKG-INFO` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-elasticsearch-app
-Version: 2.3.0
+Version: 2.4.0
 Summary: Elasticsearch utils for the curator core project
 Home-page: https://github.com/usnistgov/core_elasticsearch_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ======================
         Core Elasticsearch App
```

### Comparing `core_elasticsearch_app-2.3.0/core_elasticsearch_app.egg-info/SOURCES.txt` & `core_elasticsearch_app-2.4.0/core_elasticsearch_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_elasticsearch_app-2.3.0/setup.py` & `core_elasticsearch_app-2.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_elasticsearch_app",
-    version="2.3.0",
+    version="2.4.0",
     description="Elasticsearch utils for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_elasticsearch_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_elasticsearch_app-2.3.0/tests/test_settings.py` & `core_elasticsearch_app-2.4.0/tests/test_settings.py`

 * *Files identical despite different names*

