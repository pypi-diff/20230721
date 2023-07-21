# Comparing `tmp/vaex-jupyter-0.8.1.tar.gz` & `tmp/vaex-jupyter-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vaex-jupyter-0.8.1.tar", last modified: Wed Nov 23 19:33:24 2022, max compression
+gzip compressed data, was "dist/vaex-jupyter-0.8.2.tar", last modified: Fri Jul 21 10:39:48 2023, max compression
```

## Comparing `vaex-jupyter-0.8.1.tar` & `vaex-jupyter-0.8.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-23 19:33:24.000000 vaex-jupyter-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1087 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)       96 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      290 2022-11-23 19:33:24.000000 vaex-jupyter-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-11-23 19:33:24.000000 vaex-jupyter-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1150 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-23 19:33:24.000000 vaex-jupyter-0.8.1/vaex/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-23 19:33:24.000000 vaex-jupyter-0.8.1/vaex/jupyter/
--rw-r--r--   0 runner    (1001) docker     (116)    10411 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       52 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     7587 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/bqplot.py
--rw-r--r--   0 runner    (1001) docker     (116)     5934 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/decorators.py
--rw-r--r--   0 runner    (1001) docker     (116)       95 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/grid.py
--rw-r--r--   0 runner    (1001) docker     (116)     1541 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/ipyleaflet.py
--rw-r--r--   0 runner    (1001) docker     (116)     3877 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/ipympl.py
--rw-r--r--   0 runner    (1001) docker     (116)     5375 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/ipyvolume.py
--rw-r--r--   0 runner    (1001) docker     (116)    24000 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/model.py
--rw-r--r--   0 runner    (1001) docker     (116)     2824 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/traitlets.py
--rw-r--r--   0 runner    (1001) docker     (116)    11131 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-23 19:33:24.000000 vaex-jupyter-0.8.1/vaex/jupyter/vendor/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/vendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    27282 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/vendor/contextlib.py
--rw-r--r--   0 runner    (1001) docker     (116)    12525 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/view.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-23 19:33:24.000000 vaex-jupyter-0.8.1/vaex/jupyter/vue/
--rw-r--r--   0 runner    (1001) docker     (116)      919 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/vue/card.vue
--rw-r--r--   0 runner    (1001) docker     (116)      854 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/vue/column-select.vue
--rw-r--r--   0 runner    (1001) docker     (116)     2150 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/vue/columnlist.vue
--rw-r--r--   0 runner    (1001) docker     (116)      497 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/vue/link-list.vue
--rw-r--r--   0 runner    (1001) docker     (116)       91 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/vue/selection.vue
--rw-r--r--   0 runner    (1001) docker     (116)      256 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/vue/selection_toggle_list.vue
--rw-r--r--   0 runner    (1001) docker     (116)     1003 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/vue/tools-speed-dial.vue
--rw-r--r--   0 runner    (1001) docker     (116)     1499 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/vue/tools-toolbar.vue
--rw-r--r--   0 runner    (1001) docker     (116)     1580 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/vue/vjsf.vue
--rw-r--r--   0 runner    (1001) docker     (116)    19921 2022-11-23 19:33:10.000000 vaex-jupyter-0.8.1/vaex/jupyter/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-23 19:33:24.000000 vaex-jupyter-0.8.1/vaex_jupyter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      290 2022-11-23 19:33:24.000000 vaex-jupyter-0.8.1/vaex_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      960 2022-11-23 19:33:24.000000 vaex-jupyter-0.8.1/vaex_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-23 19:33:24.000000 vaex-jupyter-0.8.1/vaex_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       73 2022-11-23 19:33:24.000000 vaex-jupyter-0.8.1/vaex_jupyter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-23 19:33:24.000000 vaex-jupyter-0.8.1/vaex_jupyter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      105 2022-11-23 19:33:24.000000 vaex-jupyter-0.8.1/vaex_jupyter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        5 2022-11-23 19:33:24.000000 vaex-jupyter-0.8.1/vaex_jupyter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:39:47.000000 vaex-jupyter-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      290 2023-07-21 10:39:47.000000 vaex-jupyter-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-21 10:39:47.000000 vaex-jupyter-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:39:47.000000 vaex-jupyter-0.8.2/vaex/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:39:47.000000 vaex-jupyter-0.8.2/vaex/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (122)    10411 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7587 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/bqplot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5934 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/grid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1541 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/ipyleaflet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3877 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/ipympl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5375 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/ipyvolume.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24000 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/traitlets.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11131 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:39:47.000000 vaex-jupyter-0.8.2/vaex/jupyter/vendor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27282 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/vendor/contextlib.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12525 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/view.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:39:47.000000 vaex-jupyter-0.8.2/vaex/jupyter/vue/
+-rw-r--r--   0 runner    (1001) docker     (122)      919 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/vue/card.vue
+-rw-r--r--   0 runner    (1001) docker     (122)      854 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/vue/column-select.vue
+-rw-r--r--   0 runner    (1001) docker     (122)     2150 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/vue/columnlist.vue
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/vue/link-list.vue
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/vue/selection.vue
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/vue/selection_toggle_list.vue
+-rw-r--r--   0 runner    (1001) docker     (122)     1003 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/vue/tools-speed-dial.vue
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/vue/tools-toolbar.vue
+-rw-r--r--   0 runner    (1001) docker     (122)     1580 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/vue/vjsf.vue
+-rw-r--r--   0 runner    (1001) docker     (122)    19961 2023-07-21 10:39:30.000000 vaex-jupyter-0.8.2/vaex/jupyter/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:39:47.000000 vaex-jupyter-0.8.2/vaex_jupyter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      290 2023-07-21 10:39:47.000000 vaex-jupyter-0.8.2/vaex_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      960 2023-07-21 10:39:47.000000 vaex-jupyter-0.8.2/vaex_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 10:39:47.000000 vaex-jupyter-0.8.2/vaex_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-21 10:39:47.000000 vaex-jupyter-0.8.2/vaex_jupyter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 10:39:47.000000 vaex-jupyter-0.8.2/vaex_jupyter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-21 10:39:47.000000 vaex-jupyter-0.8.2/vaex_jupyter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-21 10:39:47.000000 vaex-jupyter-0.8.2/vaex_jupyter.egg-info/top_level.txt
```

### Comparing `vaex-jupyter-0.8.1/LICENSE.txt` & `vaex-jupyter-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vaex-jupyter-0.8.1/setup.py` & `vaex-jupyter-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `vaex-jupyter-0.8.1/vaex/jupyter/__init__.py` & `vaex-jupyter-0.8.2/vaex/jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `vaex-jupyter-0.8.1/vaex/jupyter/bqplot.py` & `vaex-jupyter-0.8.2/vaex/jupyter/bqplot.py`

 * *Files identical despite different names*

### Comparing `vaex-jupyter-0.8.1/vaex/jupyter/decorators.py` & `vaex-jupyter-0.8.2/vaex/jupyter/decorators.py`

 * *Files identical despite different names*

### Comparing `vaex-jupyter-0.8.1/vaex/jupyter/ipyleaflet.py` & `vaex-jupyter-0.8.2/vaex/jupyter/ipyleaflet.py`

 * *Files identical despite different names*

### Comparing `vaex-jupyter-0.8.1/vaex/jupyter/ipympl.py` & `vaex-jupyter-0.8.2/vaex/jupyter/ipympl.py`

 * *Files identical despite different names*

### Comparing `vaex-jupyter-0.8.1/vaex/jupyter/ipyvolume.py` & `vaex-jupyter-0.8.2/vaex/jupyter/ipyvolume.py`

 * *Files identical despite different names*

### Comparing `vaex-jupyter-0.8.1/vaex/jupyter/model.py` & `vaex-jupyter-0.8.2/vaex/jupyter/model.py`

 * *Files identical despite different names*

### Comparing `vaex-jupyter-0.8.1/vaex/jupyter/traitlets.py` & `vaex-jupyter-0.8.2/vaex/jupyter/traitlets.py`

 * *Files identical despite different names*

### Comparing `vaex-jupyter-0.8.1/vaex/jupyter/utils.py` & `vaex-jupyter-0.8.2/vaex/jupyter/utils.py`

 * *Files identical despite different names*

### Comparing `vaex-jupyter-0.8.1/vaex/jupyter/vendor/contextlib.py` & `vaex-jupyter-0.8.2/vaex/jupyter/vendor/contextlib.py`

 * *Files identical despite different names*

### Comparing `vaex-jupyter-0.8.1/vaex/jupyter/view.py` & `vaex-jupyter-0.8.2/vaex/jupyter/view.py`

 * *Files identical despite different names*

### Comparing `vaex-jupyter-0.8.1/vaex/jupyter/vue/card.vue` & `vaex-jupyter-0.8.2/vaex/jupyter/vue/card.vue`

 * *Files identical despite different names*

### Comparing `vaex-jupyter-0.8.1/vaex/jupyter/vue/column-select.vue` & `vaex-jupyter-0.8.2/vaex/jupyter/vue/column-select.vue`

 * *Files identical despite different names*

### Comparing `vaex-jupyter-0.8.1/vaex/jupyter/vue/columnlist.vue` & `vaex-jupyter-0.8.2/vaex/jupyter/vue/columnlist.vue`

 * *Files identical despite different names*

### Comparing `vaex-jupyter-0.8.1/vaex/jupyter/vue/tools-speed-dial.vue` & `vaex-jupyter-0.8.2/vaex/jupyter/vue/tools-speed-dial.vue`

 * *Files identical despite different names*

### Comparing `vaex-jupyter-0.8.1/vaex/jupyter/vue/tools-toolbar.vue` & `vaex-jupyter-0.8.2/vaex/jupyter/vue/tools-toolbar.vue`

 * *Files identical despite different names*

### Comparing `vaex-jupyter-0.8.1/vaex/jupyter/vue/vjsf.vue` & `vaex-jupyter-0.8.2/vaex/jupyter/vue/vjsf.vue`

 * *Files identical despite different names*

### Comparing `vaex-jupyter-0.8.1/vaex/jupyter/widgets.py` & `vaex-jupyter-0.8.2/vaex/jupyter/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from __future__ import absolute_import
+
+import os
+
 import ipyvuetify as v
 import ipywidgets as widgets
 import traitlets
 from traitlets import *  # noqa
-from . import traitlets as vt
-import os
+from traitlets import Dict, observe
 
 import vaex.jupyter
 
+from . import traitlets as vt
+
 
 def load_template(filename):
     with open(os.path.join(os.path.dirname(__file__), filename)) as f:
         return f.read()
 
 
 vaex_components = {}
@@ -554,14 +558,15 @@
     def _template(self):
         return load_template('vue/link-list.vue')
 
 
 import ipyvuetify as v
 import traitlets
 
+
 class SettingsEditor(v.VuetifyTemplate):
     template_file = os.path.join(os.path.dirname(__file__), "vue/vjsf.vue")
 
     vjsf_loaded = traitlets.Bool(False).tag(sync=True)
     values = traitlets.Dict(default_value={}).tag(sync=True)
     schema = traitlets.Dict().tag(sync=True)
     valid = traitlets.Bool(False).tag(sync=True)
```

### Comparing `vaex-jupyter-0.8.1/vaex_jupyter.egg-info/SOURCES.txt` & `vaex-jupyter-0.8.2/vaex_jupyter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

