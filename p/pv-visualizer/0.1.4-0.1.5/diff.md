# Comparing `tmp/pv-visualizer-0.1.4.tar.gz` & `tmp/pv-visualizer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pv-visualizer-0.1.4.tar", last modified: Thu Feb 23 02:13:01 2023, max compression
+gzip compressed data, was "pv-visualizer-0.1.5.tar", last modified: Fri Jul 21 21:39:14 2023, max compression
```

## Comparing `pv-visualizer-0.1.4.tar` & `pv-visualizer-0.1.5.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:13:01.903063 pv-visualizer-0.1.4/
--rw-r--r--   0 root         (0) root         (0)     1504 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      137 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2907 2023-02-23 02:13:01.903063 pv-visualizer-0.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2211 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:13:01.891063 pv-visualizer-0.1.4/pv_visualizer/
--rw-r--r--   0 root         (0) root         (0)      164 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:13:01.895063 pv-visualizer-0.1.4/pv_visualizer/app/
--rw-r--r--   0 root         (0) root         (0)       50 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:13:01.895063 pv-visualizer-0.1.4/pv_visualizer/app/assets/
--rw-r--r--   0 root         (0) root         (0)      201 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/assets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      900 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/assets/database-remove-outline.svg
--rw-r--r--   0 root         (0) root         (0)      628 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/assets/pv_logo.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:13:01.895063 pv-visualizer-0.1.4/pv_visualizer/app/engine/
--rw-r--r--   0 root         (0) root         (0)      778 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/engine/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:13:01.895063 pv-visualizer-0.1.4/pv_visualizer/app/engine/proxymanager/
--rw-r--r--   0 root         (0) root         (0)       82 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/engine/proxymanager/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4982 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/engine/proxymanager/const.py
--rw-r--r--   0 root         (0) root         (0)    14492 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/engine/proxymanager/core.py
--rw-r--r--   0 root         (0) root         (0)     8236 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/engine/proxymanager/data_informations.py
--rw-r--r--   0 root         (0) root         (0)    12162 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/engine/proxymanager/decorators.py
--rw-r--r--   0 root         (0) root         (0)    12539 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/engine/proxymanager/definitions.py
--rw-r--r--   0 root         (0) root         (0)     4416 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/engine/proxymanager/domain_helpers.py
--rw-r--r--   0 root         (0) root         (0)     5290 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/engine/proxymanager/domains.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/engine/proxymanager/paraview.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:13:01.895063 pv-visualizer-0.1.4/pv_visualizer/app/engine/reactions/
--rw-r--r--   0 root         (0) root         (0)      406 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/engine/reactions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/engine/reactions/camera.py
--rw-r--r--   0 root         (0) root         (0)     3714 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/engine/reactions/representation.py
--rw-r--r--   0 root         (0) root         (0)     2703 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/engine/reactions/scalar_range.py
--rw-r--r--   0 root         (0) root         (0)     1216 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/jupyter.py
--rw-r--r--   0 root         (0) root         (0)     1055 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:13:01.899063 pv-visualizer-0.1.4/pv_visualizer/app/ui/
--rw-r--r--   0 root         (0) root         (0)       62 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)      922 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/ui/algorithms.py
--rw-r--r--   0 root         (0) root         (0)     2812 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/ui/files.py
--rw-r--r--   0 root         (0) root         (0)     5083 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/ui/main.py
--rw-r--r--   0 root         (0) root         (0)     2571 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/ui/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     5427 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/ui/settings.py
--rw-r--r--   0 root         (0) root         (0)     1090 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/ui/state_change.py
--rw-r--r--   0 root         (0) root         (0)      540 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/app/ui/view_toolbox.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:13:01.899063 pv-visualizer-0.1.4/pv_visualizer/html/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/html/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4366 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/html/data_information.py
--rw-r--r--   0 root         (0) root         (0)    10279 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/html/file_browser.py
--rw-r--r--   0 root         (0) root         (0)     1244 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/html/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:13:01.899063 pv-visualizer-0.1.4/pv_visualizer/html/module/
--rw-r--r--   0 root         (0) root         (0)     1127 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/html/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:13:01.899063 pv-visualizer-0.1.4/pv_visualizer/html/module/serve/
--rw-r--r--   0 root         (0) root         (0)      212 2023-02-23 02:12:58.000000 pv-visualizer-0.1.4/pv_visualizer/html/module/serve/demo.html
--rw-r--r--   0 root         (0) root         (0)   249207 2023-02-23 02:12:58.000000 pv-visualizer-0.1.4/pv_visualizer/html/module/serve/vue-pv_visualizer.common.js
--rw-r--r--   0 root         (0) root         (0)   322614 2023-02-23 02:12:58.000000 pv-visualizer-0.1.4/pv_visualizer/html/module/serve/vue-pv_visualizer.common.js.map
--rw-r--r--   0 root         (0) root         (0)   249609 2023-02-23 02:12:58.000000 pv-visualizer-0.1.4/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.js
--rw-r--r--   0 root         (0) root         (0)   323178 2023-02-23 02:12:58.000000 pv-visualizer-0.1.4/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.js.map
--rw-r--r--   0 root         (0) root         (0)    97976 2023-02-23 02:12:58.000000 pv-visualizer-0.1.4/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.min.js
--rw-r--r--   0 root         (0) root         (0)   368476 2023-02-23 02:12:58.000000 pv-visualizer-0.1.4/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.min.js.map
--rw-r--r--   0 root         (0) root         (0)     4356 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/html/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     3975 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/pv_visualizer/html/proxy_editor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:13:01.891063 pv-visualizer-0.1.4/pv_visualizer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2907 2023-02-23 02:13:01.000000 pv-visualizer-0.1.4/pv_visualizer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2122 2023-02-23 02:13:01.000000 pv-visualizer-0.1.4/pv_visualizer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-23 02:13:01.000000 pv-visualizer-0.1.4/pv_visualizer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-02-23 02:13:01.000000 pv-visualizer-0.1.4/pv_visualizer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-02-23 02:13:01.000000 pv-visualizer-0.1.4/pv_visualizer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-02-23 02:13:01.000000 pv-visualizer-0.1.4/pv_visualizer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      919 2023-02-23 02:13:01.903063 pv-visualizer-0.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-23 02:12:32.000000 pv-visualizer-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.368718 pv-visualizer-0.1.5/
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      137 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3466 2023-07-21 21:39:14.368718 pv-visualizer-0.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2770 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.360718 pv-visualizer-0.1.5/pv_visualizer/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.360718 pv-visualizer-0.1.5/pv_visualizer/app/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.364718 pv-visualizer-0.1.5/pv_visualizer/app/assets/
+-rw-r--r--   0 root         (0) root         (0)      201 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/assets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      900 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/assets/database-remove-outline.svg
+-rw-r--r--   0 root         (0) root         (0)      628 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/assets/pv_logo.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.364718 pv-visualizer-0.1.5/pv_visualizer/app/engine/
+-rw-r--r--   0 root         (0) root         (0)      778 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.364718 pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4982 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/const.py
+-rw-r--r--   0 root         (0) root         (0)    14492 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/core.py
+-rw-r--r--   0 root         (0) root         (0)     8236 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/data_informations.py
+-rw-r--r--   0 root         (0) root         (0)    12162 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/decorators.py
+-rw-r--r--   0 root         (0) root         (0)    12539 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/definitions.py
+-rw-r--r--   0 root         (0) root         (0)     4416 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/domain_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     5290 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/domains.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/paraview.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.364718 pv-visualizer-0.1.5/pv_visualizer/app/engine/reactions/
+-rw-r--r--   0 root         (0) root         (0)      406 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/reactions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/reactions/camera.py
+-rw-r--r--   0 root         (0) root         (0)     3714 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/reactions/representation.py
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/engine/reactions/scalar_range.py
+-rw-r--r--   0 root         (0) root         (0)     1216 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/jupyter.py
+-rw-r--r--   0 root         (0) root         (0)      930 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.364718 pv-visualizer-0.1.5/pv_visualizer/app/ui/
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      922 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/ui/algorithms.py
+-rw-r--r--   0 root         (0) root         (0)     2812 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/ui/files.py
+-rw-r--r--   0 root         (0) root         (0)     5083 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/ui/main.py
+-rw-r--r--   0 root         (0) root         (0)     2571 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/ui/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     5427 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/ui/settings.py
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/ui/state_change.py
+-rw-r--r--   0 root         (0) root         (0)      540 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/app/ui/view_toolbox.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.364718 pv-visualizer-0.1.5/pv_visualizer/html/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/html/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4366 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/html/data_information.py
+-rw-r--r--   0 root         (0) root         (0)    10279 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/html/file_browser.py
+-rw-r--r--   0 root         (0) root         (0)     1244 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/html/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.368718 pv-visualizer-0.1.5/pv_visualizer/html/module/
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/html/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.368718 pv-visualizer-0.1.5/pv_visualizer/html/module/serve/
+-rw-r--r--   0 root         (0) root         (0)      212 2023-07-21 21:39:09.000000 pv-visualizer-0.1.5/pv_visualizer/html/module/serve/demo.html
+-rw-r--r--   0 root         (0) root         (0)   249207 2023-07-21 21:39:10.000000 pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.common.js
+-rw-r--r--   0 root         (0) root         (0)   322614 2023-07-21 21:39:10.000000 pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.common.js.map
+-rw-r--r--   0 root         (0) root         (0)   249609 2023-07-21 21:39:09.000000 pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.js
+-rw-r--r--   0 root         (0) root         (0)   323178 2023-07-21 21:39:09.000000 pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.js.map
+-rw-r--r--   0 root         (0) root         (0)    97976 2023-07-21 21:39:10.000000 pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.min.js
+-rw-r--r--   0 root         (0) root         (0)   368476 2023-07-21 21:39:10.000000 pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.min.js.map
+-rw-r--r--   0 root         (0) root         (0)     4356 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/html/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     3975 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/pv_visualizer/html/proxy_editor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 21:39:14.360718 pv-visualizer-0.1.5/pv_visualizer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3466 2023-07-21 21:39:14.000000 pv-visualizer-0.1.5/pv_visualizer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2122 2023-07-21 21:39:14.000000 pv-visualizer-0.1.5/pv_visualizer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 21:39:14.000000 pv-visualizer-0.1.5/pv_visualizer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-21 21:39:14.000000 pv-visualizer-0.1.5/pv_visualizer.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-21 21:39:14.000000 pv-visualizer-0.1.5/pv_visualizer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-21 21:39:14.000000 pv-visualizer-0.1.5/pv_visualizer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      963 2023-07-21 21:39:14.368718 pv-visualizer-0.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 21:38:47.000000 pv-visualizer-0.1.5/setup.py
```

### Comparing `pv-visualizer-0.1.4/LICENSE` & `pv-visualizer-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/PKG-INFO` & `pv-visualizer-0.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pv-visualizer
-Version: 0.1.4
+Version: 0.1.5
 Summary: Web frontend to ParaView
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
@@ -20,82 +20,83 @@
 Visualizer
 ==========
 
 .. image:: https://github.com/Kitware/paraview-visualizer/actions/workflows/test_and_release.yml/badge.svg
     :target: https://github.com/Kitware/paraview-visualizer/actions/workflows/test_and_release.yml
     :alt: Test and Release
 
-Web frontend to ParaView
+Visualizer is a Web frontend to ParaView based on trame. The current project is currently incomplete.
+You can see it as an alpha version of what it could be. To make it fully functional we need more time and possibly funding.
+But rather than waiting for it to be ready to release it, we are putting it out there as it does provide some very good example of what can be done with ParaView and trame.
+
+If you would like us to push it forward or want some help creating something similar, feel free to reach out to `kitware <https://www.kitware.com/contact/>`_ so we can see how we can help you.
 
 |image_1| |image_2| |image_3|
 
 .. |image_1| image:: https://raw.githubusercontent.com/Kitware/paraview-visualizer/master/documentation/gallery/pv_visualizer_00.jpg
   :width: 30%
 .. |image_2| image:: https://raw.githubusercontent.com/Kitware/paraview-visualizer/master/documentation/gallery/pv_visualizer_01.jpg
   :width: 30%
 .. |image_3| image:: https://raw.githubusercontent.com/Kitware/paraview-visualizer/master/documentation/gallery/pv_visualizer_02.jpg
   :width: 30%
 
 
-* Free software: BSD license
+License
+-------
+
+This software is distributed under a BSD-3 license
 
 
-Development
-------------
+Installing for Development
+--------------------------
+
 Build and install the Vue components
 
 .. code-block:: console
 
+    export NODE_OPTIONS=--openssl-legacy-provider
     cd vue-components
     npm i
     npm run build
     cd -
 
 Create a virtual environment to use with your `ParaView 5.10+ <https://www.paraview.org/download/>`_
 
 .. code-block:: console
 
     python3.9 -m venv .venv
     source .venv/bin/activate
     python -m pip install -U pip
     pip install -e .
 
-Run the application using `ParaView: pvpython <https://www.paraview.org/>`_ executable
-
-.. code-block:: console
-
-    export PV_VENV=$PWD/.venv
-    /Applications/ParaView-5.10.0.app/Contents/bin/pvpython \ # Using macOS install path as example
-        pv_run.py \
-        --data ~   \
-        --server --dev
-
+Installing from release
+-----------------------
 
-Run application
-----------------
-
-Create a virtual environment to use with your `ParaView 5.10.1+ <https://www.paraview.org/download/>`_
+Create a virtual environment to use with your `ParaView 5.10+ <https://www.paraview.org/download/>`_
 
 .. code-block:: console
 
     python3.9 -m venv .venv
     source .venv/bin/activate
-    python -m pip install -U pip
-    pip install pv-visualizer
+    python -m pip install -U pip pv-visualizer
+
+Running the application
+-----------------------
 
-Run the application using `ParaView: pvpython <https://www.paraview.org/>`_ executable with environment variables:
+Run the application using `ParaView: pvpython <https://www.paraview.org/>`_ executable
 
 .. code-block:: console
 
+    export PVPYTHON=/Applications/ParaView-5.10.0.app/Contents/bin/pvpython # Using macOS install path as example
     export PV_VENV=$PWD/.venv
-    export TRAME_APP=pv_visualizer
-    pvpython -m paraview.apps.trame --data ~
+    export TRAME_APP=pv_visualizer.app
 
+    $PVPYTHON -m paraview.apps.trame --data ~
 
-Or with command line arguments:
+Or you can use command line arguments instead of environment variables
 
 .. code-block:: console
 
-    pvpython -m paraview.apps.trame \
+    $PVPYTHON -m paraview.apps.trame \
         --venv $PWD/.venv \
-        --trame-app pv_visualizer \
+        --trame-app pv_visualizer.app \
         --data ~
```

### Comparing `pv-visualizer-0.1.4/README.rst` & `pv-visualizer-0.1.5/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -2,82 +2,83 @@
 Visualizer
 ==========
 
 .. image:: https://github.com/Kitware/paraview-visualizer/actions/workflows/test_and_release.yml/badge.svg
     :target: https://github.com/Kitware/paraview-visualizer/actions/workflows/test_and_release.yml
     :alt: Test and Release
 
-Web frontend to ParaView
+Visualizer is a Web frontend to ParaView based on trame. The current project is currently incomplete.
+You can see it as an alpha version of what it could be. To make it fully functional we need more time and possibly funding.
+But rather than waiting for it to be ready to release it, we are putting it out there as it does provide some very good example of what can be done with ParaView and trame.
+
+If you would like us to push it forward or want some help creating something similar, feel free to reach out to `kitware <https://www.kitware.com/contact/>`_ so we can see how we can help you.
 
 |image_1| |image_2| |image_3|
 
 .. |image_1| image:: https://raw.githubusercontent.com/Kitware/paraview-visualizer/master/documentation/gallery/pv_visualizer_00.jpg
   :width: 30%
 .. |image_2| image:: https://raw.githubusercontent.com/Kitware/paraview-visualizer/master/documentation/gallery/pv_visualizer_01.jpg
   :width: 30%
 .. |image_3| image:: https://raw.githubusercontent.com/Kitware/paraview-visualizer/master/documentation/gallery/pv_visualizer_02.jpg
   :width: 30%
 
 
-* Free software: BSD license
+License
+-------
+
+This software is distributed under a BSD-3 license
 
 
-Development
-------------
+Installing for Development
+--------------------------
+
 Build and install the Vue components
 
 .. code-block:: console
 
+    export NODE_OPTIONS=--openssl-legacy-provider
     cd vue-components
     npm i
     npm run build
     cd -
 
 Create a virtual environment to use with your `ParaView 5.10+ <https://www.paraview.org/download/>`_
 
 .. code-block:: console
 
     python3.9 -m venv .venv
     source .venv/bin/activate
     python -m pip install -U pip
     pip install -e .
 
-Run the application using `ParaView: pvpython <https://www.paraview.org/>`_ executable
-
-.. code-block:: console
-
-    export PV_VENV=$PWD/.venv
-    /Applications/ParaView-5.10.0.app/Contents/bin/pvpython \ # Using macOS install path as example
-        pv_run.py \
-        --data ~   \
-        --server --dev
-
+Installing from release
+-----------------------
 
-Run application
-----------------
-
-Create a virtual environment to use with your `ParaView 5.10.1+ <https://www.paraview.org/download/>`_
+Create a virtual environment to use with your `ParaView 5.10+ <https://www.paraview.org/download/>`_
 
 .. code-block:: console
 
     python3.9 -m venv .venv
     source .venv/bin/activate
-    python -m pip install -U pip
-    pip install pv-visualizer
+    python -m pip install -U pip pv-visualizer
+
+Running the application
+-----------------------
 
-Run the application using `ParaView: pvpython <https://www.paraview.org/>`_ executable with environment variables:
+Run the application using `ParaView: pvpython <https://www.paraview.org/>`_ executable
 
 .. code-block:: console
 
+    export PVPYTHON=/Applications/ParaView-5.10.0.app/Contents/bin/pvpython # Using macOS install path as example
     export PV_VENV=$PWD/.venv
-    export TRAME_APP=pv_visualizer
-    pvpython -m paraview.apps.trame --data ~
+    export TRAME_APP=pv_visualizer.app
 
+    $PVPYTHON -m paraview.apps.trame --data ~
 
-Or with command line arguments:
+Or you can use command line arguments instead of environment variables
 
 .. code-block:: console
 
-    pvpython -m paraview.apps.trame \
+    $PVPYTHON -m paraview.apps.trame \
         --venv $PWD/.venv \
-        --trame-app pv_visualizer \
+        --trame-app pv_visualizer.app \
         --data ~
```

### Comparing `pv-visualizer-0.1.4/pv_visualizer/app/assets/database-remove-outline.svg` & `pv-visualizer-0.1.5/pv_visualizer/app/assets/database-remove-outline.svg`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/app/assets/pv_logo.svg` & `pv-visualizer-0.1.5/pv_visualizer/app/assets/pv_logo.svg`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/app/engine/__init__.py` & `pv-visualizer-0.1.5/pv_visualizer/app/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/app/engine/proxymanager/const.py` & `pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/const.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/app/engine/proxymanager/core.py` & `pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/core.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/app/engine/proxymanager/data_informations.py` & `pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/data_informations.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/app/engine/proxymanager/decorators.py` & `pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/decorators.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/app/engine/proxymanager/definitions.py` & `pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/definitions.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/app/engine/proxymanager/domain_helpers.py` & `pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/domain_helpers.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/app/engine/proxymanager/domains.py` & `pv-visualizer-0.1.5/pv_visualizer/app/engine/proxymanager/domains.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/app/engine/reactions/camera.py` & `pv-visualizer-0.1.5/pv_visualizer/app/engine/reactions/camera.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/app/engine/reactions/representation.py` & `pv-visualizer-0.1.5/pv_visualizer/app/engine/reactions/representation.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/app/engine/reactions/scalar_range.py` & `pv-visualizer-0.1.5/pv_visualizer/app/engine/reactions/scalar_range.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/app/jupyter.py` & `pv-visualizer-0.1.5/pv_visualizer/app/jupyter.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/app/main.py` & `pv-visualizer-0.1.5/pv_visualizer/app/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from trame.app import get_server, dev
+from trame.app import get_server
 
 SERVER = None
 
 
 def main(server=None, data=None, plugins=None, **kwargs):
     from . import engine, ui
 
@@ -20,22 +20,16 @@
     if plugins is None:
         server.cli.add_argument(
             "--plugins", help="List of distributed plugins to load", dest="plugins"
         )
         args, _ = server.cli.parse_known_args()
         plugins = args.plugins.split(",") if args.plugins else []
 
-    # Make UI auto reload
-    def _reload():
-        dev.reload(ui)
-        ui.initialize(SERVER)
-
-    server.controller.on_server_reload.add(_reload)
-
     # Init application
+    server.client_type = "vue2"
     SERVER = server
 
     engine.initialize(server, plugins)
     ui.initialize(server)
 
     # Start server
     return server.start(**kwargs)
```

### Comparing `pv-visualizer-0.1.4/pv_visualizer/app/ui/algorithms.py` & `pv-visualizer-0.1.5/pv_visualizer/app/ui/algorithms.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/app/ui/files.py` & `pv-visualizer-0.1.5/pv_visualizer/app/ui/files.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/app/ui/main.py` & `pv-visualizer-0.1.5/pv_visualizer/app/ui/main.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/app/ui/pipeline.py` & `pv-visualizer-0.1.5/pv_visualizer/app/ui/pipeline.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/app/ui/settings.py` & `pv-visualizer-0.1.5/pv_visualizer/app/ui/settings.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/app/ui/state_change.py` & `pv-visualizer-0.1.5/pv_visualizer/app/ui/state_change.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/app/ui/view_toolbox.py` & `pv-visualizer-0.1.5/pv_visualizer/app/ui/view_toolbox.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/html/data_information.py` & `pv-visualizer-0.1.5/pv_visualizer/html/data_information.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/html/file_browser.py` & `pv-visualizer-0.1.5/pv_visualizer/html/file_browser.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/html/filters.py` & `pv-visualizer-0.1.5/pv_visualizer/html/filters.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/html/module/__init__.py` & `pv-visualizer-0.1.5/pv_visualizer/html/module/__init__.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/html/module/serve/vue-pv_visualizer.common.js` & `pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.common.js`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/html/module/serve/vue-pv_visualizer.common.js.map` & `pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.common.js.map`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.js` & `pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.js`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.js.map` & `pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.js.map`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.min.js` & `pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.min.js`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.min.js.map` & `pv-visualizer-0.1.5/pv_visualizer/html/module/serve/vue-pv_visualizer.umd.min.js.map`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/html/pipeline.py` & `pv-visualizer-0.1.5/pv_visualizer/html/pipeline.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer/html/proxy_editor.py` & `pv-visualizer-0.1.5/pv_visualizer/html/proxy_editor.py`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/pv_visualizer.egg-info/PKG-INFO` & `pv-visualizer-0.1.5/pv_visualizer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pv-visualizer
-Version: 0.1.4
+Version: 0.1.5
 Summary: Web frontend to ParaView
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
@@ -20,82 +20,83 @@
 Visualizer
 ==========
 
 .. image:: https://github.com/Kitware/paraview-visualizer/actions/workflows/test_and_release.yml/badge.svg
     :target: https://github.com/Kitware/paraview-visualizer/actions/workflows/test_and_release.yml
     :alt: Test and Release
 
-Web frontend to ParaView
+Visualizer is a Web frontend to ParaView based on trame. The current project is currently incomplete.
+You can see it as an alpha version of what it could be. To make it fully functional we need more time and possibly funding.
+But rather than waiting for it to be ready to release it, we are putting it out there as it does provide some very good example of what can be done with ParaView and trame.
+
+If you would like us to push it forward or want some help creating something similar, feel free to reach out to `kitware <https://www.kitware.com/contact/>`_ so we can see how we can help you.
 
 |image_1| |image_2| |image_3|
 
 .. |image_1| image:: https://raw.githubusercontent.com/Kitware/paraview-visualizer/master/documentation/gallery/pv_visualizer_00.jpg
   :width: 30%
 .. |image_2| image:: https://raw.githubusercontent.com/Kitware/paraview-visualizer/master/documentation/gallery/pv_visualizer_01.jpg
   :width: 30%
 .. |image_3| image:: https://raw.githubusercontent.com/Kitware/paraview-visualizer/master/documentation/gallery/pv_visualizer_02.jpg
   :width: 30%
 
 
-* Free software: BSD license
+License
+-------
+
+This software is distributed under a BSD-3 license
 
 
-Development
-------------
+Installing for Development
+--------------------------
+
 Build and install the Vue components
 
 .. code-block:: console
 
+    export NODE_OPTIONS=--openssl-legacy-provider
     cd vue-components
     npm i
     npm run build
     cd -
 
 Create a virtual environment to use with your `ParaView 5.10+ <https://www.paraview.org/download/>`_
 
 .. code-block:: console
 
     python3.9 -m venv .venv
     source .venv/bin/activate
     python -m pip install -U pip
     pip install -e .
 
-Run the application using `ParaView: pvpython <https://www.paraview.org/>`_ executable
-
-.. code-block:: console
-
-    export PV_VENV=$PWD/.venv
-    /Applications/ParaView-5.10.0.app/Contents/bin/pvpython \ # Using macOS install path as example
-        pv_run.py \
-        --data ~   \
-        --server --dev
-
+Installing from release
+-----------------------
 
-Run application
-----------------
-
-Create a virtual environment to use with your `ParaView 5.10.1+ <https://www.paraview.org/download/>`_
+Create a virtual environment to use with your `ParaView 5.10+ <https://www.paraview.org/download/>`_
 
 .. code-block:: console
 
     python3.9 -m venv .venv
     source .venv/bin/activate
-    python -m pip install -U pip
-    pip install pv-visualizer
+    python -m pip install -U pip pv-visualizer
+
+Running the application
+-----------------------
 
-Run the application using `ParaView: pvpython <https://www.paraview.org/>`_ executable with environment variables:
+Run the application using `ParaView: pvpython <https://www.paraview.org/>`_ executable
 
 .. code-block:: console
 
+    export PVPYTHON=/Applications/ParaView-5.10.0.app/Contents/bin/pvpython # Using macOS install path as example
     export PV_VENV=$PWD/.venv
-    export TRAME_APP=pv_visualizer
-    pvpython -m paraview.apps.trame --data ~
+    export TRAME_APP=pv_visualizer.app
 
+    $PVPYTHON -m paraview.apps.trame --data ~
 
-Or with command line arguments:
+Or you can use command line arguments instead of environment variables
 
 .. code-block:: console
 
-    pvpython -m paraview.apps.trame \
+    $PVPYTHON -m paraview.apps.trame \
         --venv $PWD/.venv \
-        --trame-app pv_visualizer \
+        --trame-app pv_visualizer.app \
         --data ~
```

### Comparing `pv-visualizer-0.1.4/pv_visualizer.egg-info/SOURCES.txt` & `pv-visualizer-0.1.5/pv_visualizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pv-visualizer-0.1.4/setup.cfg` & `pv-visualizer-0.1.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pv-visualizer
-version = 0.1.4
+version = 0.1.5
 description = Web frontend to ParaView
 long_description = file: README.rst
 author = Kitware Inc.
 license = BSD License
 classifiers = 
 	Development Status :: 1 - Planning
 	Environment :: Web Environment
@@ -23,14 +23,17 @@
 	Framework
 
 [options]
 packages = find:
 include_package_data = True
 install_requires = 
 	trame
+	trame-vuetify
+	trame-components
+	trame-vtk
 	trame-simput
 
 [options.entry_points]
 console_scripts = 
 	pv-visualizer = pv_visualizer:main
 
 [semantic_release]
```

