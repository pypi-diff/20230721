# Comparing `tmp/core_main_registry_app-2.3.0.tar.gz` & `tmp/core_main_registry_app-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_main_registry_app-2.3.0.tar", last modified: Tue May  2 19:40:47 2023, max compression
+gzip compressed data, was "core_main_registry_app-2.4.0.tar", last modified: Fri Jul 21 02:14:32 2023, max compression
```

## Comparing `core_main_registry_app-2.3.0.tar` & `core_main_registry_app-2.4.0.tar`

### file list

```diff
@@ -1,194 +1,168 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.521330 core_main_registry_app-2.3.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2372 2023-05-02 19:40:47.516137 core_main_registry_app-2.3.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1506 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.396858 core_main_registry_app-2.3.0/core_main_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5076 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      539 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.522261 core_main_registry_app-2.3.0/core_main_registry_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      168 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/commons/constants.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.539908 core_main_registry_app-2.3.0/core_main_registry_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.587835 core_main_registry_app-2.3.0/core_main_registry_app/components/category/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/category/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1843 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/category/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3721 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/category/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.656624 core_main_registry_app-2.3.0/core_main_registry_app/components/custom_resource/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/custom_resource/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      478 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/custom_resource/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7731 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/custom_resource/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4505 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/custom_resource/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.701578 core_main_registry_app-2.3.0/core_main_registry_app/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      515 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/data/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3117 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/data/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.759666 core_main_registry_app-2.3.0/core_main_registry_app/components/refinement/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/refinement/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1463 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/refinement/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2488 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/refinement/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.794256 core_main_registry_app-2.3.0/core_main_registry_app/components/template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/template/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      881 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/template/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.829581 core_main_registry_app-2.3.0/core_main_registry_app/components/version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      749 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/components/version_manager/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      360 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/constants.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3751 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      705 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.873115 core_main_registry_app-2.3.0/core_main_registry_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5740 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       80 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.908826 core_main_registry_app-2.3.0/core_main_registry_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.943245 core_main_registry_app-2.3.0/core_main_registry_app/rest/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/rest/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3575 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/rest/data/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.979315 core_main_registry_app-2.3.0/core_main_registry_app/rest/template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/rest/template_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      784 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/rest/template_version_manager/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11382 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1006 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:44.902290 core_main_registry_app-2.3.0/core_main_registry_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:44.976371 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.001756 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/json/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4331 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/json/custom_registry.json
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:44.915305 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.289056 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     6830 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.childcounter.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    12752 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.clones.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     4207 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.columnview.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     6032 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.customtag.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     3737 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.debug.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    19449 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.dnd.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    14809 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.dnd5.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     8978 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.edit.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    10817 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.filter.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    19024 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.fixed.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     4031 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.glyph.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     5317 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.gridnav.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)   160231 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     4291 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.menu.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    11287 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.persist.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    14308 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.table.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     4174 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.themeroller.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     6509 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.wide.js
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    15197 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/jsdoc-globals.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.417646 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21971 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/ui.fancytree.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11747 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/ui.fancytree.less
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14470 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/ui.fancytree.min.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      842 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/vline-rtl.gif
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      844 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/vline.gif
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.500631 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18706 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/ui.fancytree.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5248 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/ui.fancytree.less
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11739 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/ui.fancytree.min.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      842 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/vline-rtl.gif
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      844 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/vline.gif
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    23637 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-common.less
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:44.938295 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:44.959574 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/user/css/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.549974 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/user/css/fancytree/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      371 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/user/css/fancytree/fancytree.custom.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.582321 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      980 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/resource_banner.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      327 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/selection.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.600056 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/xsd/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)   188155 2023-05-02 19:40:41.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/xsd/res-md.xsd
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.622475 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/xsl/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5626 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/xsl/xml2html.xsl
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.660661 core_main_registry_app-2.3.0/core_main_registry_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2769 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/system/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      426 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:44.995075 core_main_registry_app-2.3.0/core_main_registry_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.013896 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.009684 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.722475 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      338 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/list.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      925 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/table.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.740734 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/upload/base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      181 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/upload.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.774470 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/admin/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      384 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/admin/data/detail.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      319 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/admin/data/view_data.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.791741 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/resource_banner/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      815 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/resource_banner/resource_banner.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4813 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.810940 core_main_registry_app-2.3.0/core_main_registry_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.848753 core_main_registry_app-2.3.0/core_main_registry_app/utils/fancytree/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/fancytree/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12184 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/fancytree/widget.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.913812 core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6124 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/mongo_query.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2776 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/refinement.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.954718 core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/tools/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/tools/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3577 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/tools/tree.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9709 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/tools/xsd_refinements.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1032 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/watch.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:46.985288 core_main_registry_app-2.3.0/core_main_registry_app/utils/role/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/role/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      659 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/utils/role/extraction.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.007013 core_main_registry_app-2.3.0/core_main_registry_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.053312 core_main_registry_app-2.3.0/core_main_registry_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      310 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5354 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/core_main_registry_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:45.488279 core_main_registry_app-2.3.0/core_main_registry_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2372 2023-05-02 19:40:44.000000 core_main_registry_app-2.3.0/core_main_registry_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8042 2023-05-02 19:40:44.000000 core_main_registry_app-2.3.0/core_main_registry_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:40:44.000000 core_main_registry_app-2.3.0/core_main_registry_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      132 2023-05-02 19:40:44.000000 core_main_registry_app-2.3.0/core_main_registry_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       29 2023-05-02 19:40:44.000000 core_main_registry_app-2.3.0/core_main_registry_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       71 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       61 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:40:47.528789 core_main_registry_app-2.3.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1413 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.093111 core_main_registry_app-2.3.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.112486 core_main_registry_app-2.3.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.147660 core_main_registry_app-2.3.0/tests/components/category/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/category/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5376 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/category/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.192247 core_main_registry_app-2.3.0/tests/components/custom_resource/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/custom_resource/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.230636 core_main_registry_app-2.3.0/tests/components/custom_resource/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/custom_resource/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5244 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/custom_resource/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14360 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/custom_resource/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14727 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/custom_resource/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.263796 core_main_registry_app-2.3.0/tests/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/data/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.304648 core_main_registry_app-2.3.0/tests/components/data/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/data/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2996 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/data/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4838 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/data/tests_int.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.337740 core_main_registry_app-2.3.0/tests/components/refinement/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/refinement/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4487 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/refinement/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.354321 core_main_registry_app-2.3.0/tests/components/template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/template_version_manager/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.394074 core_main_registry_app-2.3.0/tests/components/template_version_manager/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/template_version_manager/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2178 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/components/template_version_manager/fixtures/fixtures.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.410911 core_main_registry_app-2.3.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.449134 core_main_registry_app-2.3.0/tests/rest/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/rest/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3421 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/rest/data/tests_permissions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:47.500310 core_main_registry_app-2.3.0/tests/rest/template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/rest/template_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3008 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/rest/template_version_manager/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2135 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/rest/template_version_manager/tests_permission.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1773 2023-05-02 19:40:42.000000 core_main_registry_app-2.3.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:32.004794 core_main_registry_app-2.4.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-07-21 02:14:25.000000 core_main_registry_app-2.4.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2023-07-21 02:14:25.000000 core_main_registry_app-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2045 2023-07-21 02:14:31.999538 core_main_registry_app-2.4.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1275 2023-07-21 02:14:25.000000 core_main_registry_app-2.4.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:30.335481 core_main_registry_app-2.4.0/core_main_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2023-07-21 02:14:25.000000 core_main_registry_app-2.4.0/core_main_registry_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5076 2023-07-21 02:14:25.000000 core_main_registry_app-2.4.0/core_main_registry_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      539 2023-07-21 02:14:25.000000 core_main_registry_app-2.4.0/core_main_registry_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:30.420299 core_main_registry_app-2.4.0/core_main_registry_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:25.000000 core_main_registry_app-2.4.0/core_main_registry_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      168 2023-07-21 02:14:25.000000 core_main_registry_app-2.4.0/core_main_registry_app/commons/constants.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:30.434285 core_main_registry_app-2.4.0/core_main_registry_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:25.000000 core_main_registry_app-2.4.0/core_main_registry_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:30.489794 core_main_registry_app-2.4.0/core_main_registry_app/components/category/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:25.000000 core_main_registry_app-2.4.0/core_main_registry_app/components/category/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1843 2023-07-21 02:14:25.000000 core_main_registry_app-2.4.0/core_main_registry_app/components/category/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3721 2023-07-21 02:14:25.000000 core_main_registry_app-2.4.0/core_main_registry_app/components/category/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:30.545874 core_main_registry_app-2.4.0/core_main_registry_app/components/custom_resource/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:25.000000 core_main_registry_app-2.4.0/core_main_registry_app/components/custom_resource/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      478 2023-07-21 02:14:25.000000 core_main_registry_app-2.4.0/core_main_registry_app/components/custom_resource/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7731 2023-07-21 02:14:25.000000 core_main_registry_app-2.4.0/core_main_registry_app/components/custom_resource/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4505 2023-07-21 02:14:25.000000 core_main_registry_app-2.4.0/core_main_registry_app/components/custom_resource/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:30.588895 core_main_registry_app-2.4.0/core_main_registry_app/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:25.000000 core_main_registry_app-2.4.0/core_main_registry_app/components/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      515 2023-07-21 02:14:25.000000 core_main_registry_app-2.4.0/core_main_registry_app/components/data/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3117 2023-07-21 02:14:25.000000 core_main_registry_app-2.4.0/core_main_registry_app/components/data/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:30.634095 core_main_registry_app-2.4.0/core_main_registry_app/components/refinement/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:26.000000 core_main_registry_app-2.4.0/core_main_registry_app/components/refinement/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1463 2023-07-21 02:14:26.000000 core_main_registry_app-2.4.0/core_main_registry_app/components/refinement/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2488 2023-07-21 02:14:26.000000 core_main_registry_app-2.4.0/core_main_registry_app/components/refinement/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:30.663449 core_main_registry_app-2.4.0/core_main_registry_app/components/template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:26.000000 core_main_registry_app-2.4.0/core_main_registry_app/components/template/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      881 2023-07-21 02:14:26.000000 core_main_registry_app-2.4.0/core_main_registry_app/components/template/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:30.690814 core_main_registry_app-2.4.0/core_main_registry_app/components/version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:26.000000 core_main_registry_app-2.4.0/core_main_registry_app/components/version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      749 2023-07-21 02:14:26.000000 core_main_registry_app-2.4.0/core_main_registry_app/components/version_manager/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      360 2023-07-21 02:14:26.000000 core_main_registry_app-2.4.0/core_main_registry_app/constants.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3751 2023-07-21 02:14:26.000000 core_main_registry_app-2.4.0/core_main_registry_app/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      705 2023-07-21 02:14:26.000000 core_main_registry_app-2.4.0/core_main_registry_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:30.718851 core_main_registry_app-2.4.0/core_main_registry_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5740 2023-07-21 02:14:26.000000 core_main_registry_app-2.4.0/core_main_registry_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:26.000000 core_main_registry_app-2.4.0/core_main_registry_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       80 2023-07-21 02:14:26.000000 core_main_registry_app-2.4.0/core_main_registry_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:30.749650 core_main_registry_app-2.4.0/core_main_registry_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:26.000000 core_main_registry_app-2.4.0/core_main_registry_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:30.884610 core_main_registry_app-2.4.0/core_main_registry_app/rest/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:26.000000 core_main_registry_app-2.4.0/core_main_registry_app/rest/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3575 2023-07-21 02:14:26.000000 core_main_registry_app-2.4.0/core_main_registry_app/rest/data/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:30.917392 core_main_registry_app-2.4.0/core_main_registry_app/rest/template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:26.000000 core_main_registry_app-2.4.0/core_main_registry_app/rest/template_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      784 2023-07-21 02:14:26.000000 core_main_registry_app-2.4.0/core_main_registry_app/rest/template_version_manager/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11408 2023-07-21 02:14:26.000000 core_main_registry_app-2.4.0/core_main_registry_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1006 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:29.894785 core_main_registry_app-2.4.0/core_main_registry_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:29.944311 core_main_registry_app-2.4.0/core_main_registry_app/static/core_main_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:30.940734 core_main_registry_app-2.4.0/core_main_registry_app/static/core_main_registry_app/json/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4331 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/static/core_main_registry_app/json/custom_registry.json
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:29.928825 core_main_registry_app-2.4.0/core_main_registry_app/static/core_main_registry_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:29.935904 core_main_registry_app-2.4.0/core_main_registry_app/static/core_main_registry_app/user/css/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:30.962343 core_main_registry_app-2.4.0/core_main_registry_app/static/core_main_registry_app/user/css/fancytree/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      388 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/static/core_main_registry_app/user/css/fancytree/fancytree.custom.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.000948 core_main_registry_app-2.4.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      980 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/resource_banner.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      327 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/selection.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.017582 core_main_registry_app-2.4.0/core_main_registry_app/static/core_main_registry_app/xsd/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)   188155 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/static/core_main_registry_app/xsd/res-md.xsd
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.038807 core_main_registry_app-2.4.0/core_main_registry_app/static/core_main_registry_app/xsl/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5704 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/static/core_main_registry_app/xsl/xml2html.xsl
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.073106 core_main_registry_app-2.4.0/core_main_registry_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2769 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/system/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      426 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:29.969456 core_main_registry_app-2.4.0/core_main_registry_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:30.008411 core_main_registry_app-2.4.0/core_main_registry_app/templates/core_main_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:30.004462 core_main_registry_app-2.4.0/core_main_registry_app/templates/core_main_registry_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.128071 core_main_registry_app-2.4.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      338 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/list.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      925 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/table.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.144402 core_main_registry_app-2.4.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/upload/base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      181 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/upload.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.172860 core_main_registry_app-2.4.0/core_main_registry_app/templates/core_main_registry_app/admin/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      384 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/templates/core_main_registry_app/admin/data/detail.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      319 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/templates/core_main_registry_app/admin/data/view_data.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.188274 core_main_registry_app-2.4.0/core_main_registry_app/templates/core_main_registry_app/resource_banner/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      815 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/templates/core_main_registry_app/resource_banner/resource_banner.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5395 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.202847 core_main_registry_app-2.4.0/core_main_registry_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.234272 core_main_registry_app-2.4.0/core_main_registry_app/utils/fancytree/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/utils/fancytree/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10326 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/utils/fancytree/widget.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.298008 core_main_registry_app-2.4.0/core_main_registry_app/utils/refinement/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/utils/refinement/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6124 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/utils/refinement/mongo_query.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2776 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/utils/refinement/refinement.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.343862 core_main_registry_app-2.4.0/core_main_registry_app/utils/refinement/tools/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/utils/refinement/tools/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3577 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/utils/refinement/tools/tree.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9709 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/utils/refinement/tools/xsd_refinements.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1032 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/utils/refinement/watch.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.383116 core_main_registry_app-2.4.0/core_main_registry_app/utils/role/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/utils/role/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      659 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/utils/role/extraction.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.397621 core_main_registry_app-2.4.0/core_main_registry_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.467184 core_main_registry_app-2.4.0/core_main_registry_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      310 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5354 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/core_main_registry_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:30.394307 core_main_registry_app-2.4.0/core_main_registry_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2045 2023-07-21 02:14:29.000000 core_main_registry_app-2.4.0/core_main_registry_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5321 2023-07-21 02:14:29.000000 core_main_registry_app-2.4.0/core_main_registry_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-07-21 02:14:29.000000 core_main_registry_app-2.4.0/core_main_registry_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      123 2023-07-21 02:14:29.000000 core_main_registry_app-2.4.0/core_main_registry_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       29 2023-07-21 02:14:29.000000 core_main_registry_app-2.4.0/core_main_registry_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       71 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       51 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-07-21 02:14:32.007204 core_main_registry_app-2.4.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1413 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.513182 core_main_registry_app-2.4.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.528642 core_main_registry_app-2.4.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.564159 core_main_registry_app-2.4.0/tests/components/category/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/tests/components/category/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5376 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/tests/components/category/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.612083 core_main_registry_app-2.4.0/tests/components/custom_resource/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/tests/components/custom_resource/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.648191 core_main_registry_app-2.4.0/tests/components/custom_resource/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/tests/components/custom_resource/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5244 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/tests/components/custom_resource/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14360 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/tests/components/custom_resource/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14727 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/tests/components/custom_resource/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.682111 core_main_registry_app-2.4.0/tests/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/tests/components/data/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.714897 core_main_registry_app-2.4.0/tests/components/data/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/tests/components/data/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2996 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/tests/components/data/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4838 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/tests/components/data/tests_int.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.748730 core_main_registry_app-2.4.0/tests/components/refinement/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/tests/components/refinement/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4487 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/tests/components/refinement/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.764790 core_main_registry_app-2.4.0/tests/components/template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/tests/components/template_version_manager/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.798229 core_main_registry_app-2.4.0/tests/components/template_version_manager/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/tests/components/template_version_manager/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2178 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/tests/components/template_version_manager/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      539 2023-07-21 02:14:27.000000 core_main_registry_app-2.4.0/tests/mocks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.812315 core_main_registry_app-2.4.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:28.000000 core_main_registry_app-2.4.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.863933 core_main_registry_app-2.4.0/tests/rest/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:28.000000 core_main_registry_app-2.4.0/tests/rest/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3421 2023-07-21 02:14:28.000000 core_main_registry_app-2.4.0/tests/rest/data/tests_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.918020 core_main_registry_app-2.4.0/tests/rest/template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:28.000000 core_main_registry_app-2.4.0/tests/rest/template_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3008 2023-07-21 02:14:28.000000 core_main_registry_app-2.4.0/tests/rest/template_version_manager/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2135 2023-07-21 02:14:28.000000 core_main_registry_app-2.4.0/tests/rest/template_version_manager/tests_permission.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1773 2023-07-21 02:14:28.000000 core_main_registry_app-2.4.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.932997 core_main_registry_app-2.4.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:28.000000 core_main_registry_app-2.4.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.949657 core_main_registry_app-2.4.0/tests/utils/fancytree/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:28.000000 core_main_registry_app-2.4.0/tests/utils/fancytree/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:31.985404 core_main_registry_app-2.4.0/tests/utils/fancytree/widget/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-07-21 02:14:28.000000 core_main_registry_app-2.4.0/tests/utils/fancytree/widget/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      717 2023-07-21 02:14:28.000000 core_main_registry_app-2.4.0/tests/utils/fancytree/widget/tests_unit.py
```

### Comparing `core_main_registry_app-2.3.0/LICENSE.md` & `core_main_registry_app-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/PKG-INFO` & `core_main_registry_app-2.4.0/core_main_registry_app.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
-Name: core_main_registry_app
-Version: 2.3.0
+Name: core-main-registry-app
+Version: 2.4.0
 Summary: Main functionalities for the registry project
 Home-page: https://github.com/usnistgov/core_main_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: Core Main Registry App
         ======================
@@ -39,44 +39,32 @@
             $ python setup.py
             $ pip install sdist/*.tar.gz
         
         
         Configuration
         =============
         
-        1. Add "core_main_registry_app", "mptt", "tz_detect" to your INSTALLED_APPS setting like this
+        1. Add "core_main_registry_app", "mptt" to your INSTALLED_APPS setting like this
         ---------------------------------------------------------------------------------------------
         
         .. code:: python
         
             INSTALLED_APPS = [
                 ...
-                "tz_detect",
                 "core_main_registry_app",
                 "mptt",
             ]
         
-        2. Add the middleware required by tz_detect
-        -------------------------------------------
-        
-        .. code:: python
-        
-            MIDDLEWARE = (
-                ...
-                'tz_detect.middleware.TimezoneMiddleware',
-            )
-        
-        
-        3. Include the core_main_registry_app URLconf in your project urls.py like this
+        2. Include the core_main_registry_app URLconf in your project urls.py like this
         -------------------------------------------------------------------------------
         
         .. code:: python
         
             url(r'^', include("core_main_registry_app.urls")),
         
         
-        4. Launch migration: create table and constraints.
+        3. Launch migration: create table and constraints.
         --------------------------------------------------
         
             $ python manage.py migrate
         
 Platform: UNKNOWN
```

### Comparing `core_main_registry_app-2.3.0/README.rst` & `core_main_registry_app-2.4.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -31,42 +31,30 @@
     $ python setup.py
     $ pip install sdist/*.tar.gz
 
 
 Configuration
 =============
 
-1. Add "core_main_registry_app", "mptt", "tz_detect" to your INSTALLED_APPS setting like this
+1. Add "core_main_registry_app", "mptt" to your INSTALLED_APPS setting like this
 ---------------------------------------------------------------------------------------------
 
 .. code:: python
 
     INSTALLED_APPS = [
         ...
-        "tz_detect",
         "core_main_registry_app",
         "mptt",
     ]
 
-2. Add the middleware required by tz_detect
--------------------------------------------
-
-.. code:: python
-
-    MIDDLEWARE = (
-        ...
-        'tz_detect.middleware.TimezoneMiddleware',
-    )
-
-
-3. Include the core_main_registry_app URLconf in your project urls.py like this
+2. Include the core_main_registry_app URLconf in your project urls.py like this
 -------------------------------------------------------------------------------
 
 .. code:: python
 
     url(r'^', include("core_main_registry_app.urls")),
 
 
-4. Launch migration: create table and constraints.
+3. Launch migration: create table and constraints.
 --------------------------------------------------
 
     $ python manage.py migrate
```

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/admin.py` & `core_main_registry_app-2.4.0/core_main_registry_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/apps.py` & `core_main_registry_app-2.4.0/core_main_registry_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/components/category/api.py` & `core_main_registry_app-2.4.0/core_main_registry_app/components/category/api.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/components/category/models.py` & `core_main_registry_app-2.4.0/core_main_registry_app/components/category/models.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/components/custom_resource/api.py` & `core_main_registry_app-2.4.0/core_main_registry_app/components/custom_resource/api.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/components/custom_resource/models.py` & `core_main_registry_app-2.4.0/core_main_registry_app/components/custom_resource/models.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/components/data/access_control.py` & `core_main_registry_app-2.4.0/core_main_registry_app/components/data/access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/components/data/api.py` & `core_main_registry_app-2.4.0/core_main_registry_app/components/data/api.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/components/refinement/api.py` & `core_main_registry_app-2.4.0/core_main_registry_app/components/refinement/api.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/components/refinement/models.py` & `core_main_registry_app-2.4.0/core_main_registry_app/components/refinement/models.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/components/template/api.py` & `core_main_registry_app-2.4.0/core_main_registry_app/components/template/api.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/components/version_manager/api.py` & `core_main_registry_app-2.4.0/core_main_registry_app/components/version_manager/api.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/discover.py` & `core_main_registry_app-2.4.0/core_main_registry_app/discover.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/menus.py` & `core_main_registry_app-2.4.0/core_main_registry_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/migrations/0001_initial.py` & `core_main_registry_app-2.4.0/core_main_registry_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/rest/data/views.py` & `core_main_registry_app-2.4.0/core_main_registry_app/rest/data/views.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/rest/template_version_manager/views.py` & `core_main_registry_app-2.4.0/core_main_registry_app/rest/template_version_manager/views.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/rest/urls.py` & `core_main_registry_app-2.4.0/core_main_registry_app/rest/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,20 +107,20 @@
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
         r"^data/(?P<pk>\w+)/publish/$",
         registry_data_views.publish_data,
         name="core_main_app_rest_publish_data",
     ),
```

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/settings.py` & `core_main_registry_app-2.4.0/core_main_registry_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/json/custom_registry.json` & `core_main_registry_app-2.4.0/core_main_registry_app/static/core_main_registry_app/json/custom_registry.json`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/resource_banner.css` & `core_main_registry_app-2.4.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/resource_banner.css`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/xsd/res-md.xsd` & `core_main_registry_app-2.4.0/core_main_registry_app/static/core_main_registry_app/xsd/res-md.xsd`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/xsl/xml2html.xsl` & `core_main_registry_app-2.4.0/core_main_registry_app/static/core_main_registry_app/xsl/xml2html.xsl`

 * *Files 8% similar despite different names*

#### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/static/core_main_registry_app/xsl/xml2html.xsl` & `core_main_registry_app-2.4.0/core_main_registry_app/static/core_main_registry_app/xsl/xml2html.xsl`

```diff
@@ -15,15 +15,15 @@
     <div class="container">
       <table class="table table-hover">
         <tr>
           <td colspan="2">
             <xsl:variable name="url" select="//rsm:Resource/rsm:content/rsm:landingPage"/>
             <xsl:choose>
               <xsl:when test="//rsm:Resource/rsm:content/rsm:landingPage!=''">
-                <a target="_blank" href="{$url}" style="font-weight: bold">
+                <a target="_blank" rel="noopener noreferrer" href="{$url}" style="font-weight: bold">
                   <xsl:call-template name="title"/>
                 </a>
               </xsl:when>
               <xsl:otherwise>
                 <strong>
                   <xsl:call-template name="title"/>
                 </strong>
@@ -69,15 +69,15 @@
           <td style="width: 25%;">
             <xsl:value-of select="$name"/>
           </td>
           <td>
             <span class="value">
               <xsl:choose>
                 <xsl:when test="contains($name, 'URL')">
-                  <a target="_blank" href="{$value}">
+                  <a target="_blank" rel="noopener noreferrer" href="{$value}">
                     <xsl:value-of select="$value"/>
                   </a>
                 </xsl:when>
                 <xsl:otherwise>
                   <xsl:value-of select="$value"/>
                 </xsl:otherwise>
               </xsl:choose>
@@ -108,15 +108,15 @@
       <td width="180">
         <xsl:value-of select="$name"/>
       </td>
       <td>
         <span class="value">
           <xsl:choose>
             <xsl:when test="contains($name, 'URL')">
-              <a target="_blank" href="{$value}">
+              <a target="_blank" rel="noopener noreferrer" href="{$value}">
                 <xsl:value-of select="$value"/>
               </a>
             </xsl:when>
             <xsl:when test="$name='localid' and $value=''">
               <i>The Local ID will be automatically generated.</i>
             </xsl:when>
             <xsl:otherwise>
```

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/system/api.py` & `core_main_registry_app-2.4.0/core_main_registry_app/system/api.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/table.html` & `core_main_registry_app-2.4.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/table.html`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/templates/core_main_registry_app/resource_banner/resource_banner.html` & `core_main_registry_app-2.4.0/core_main_registry_app/templates/core_main_registry_app/resource_banner/resource_banner.html`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/utils/fancytree/widget.py` & `core_main_registry_app-2.4.0/core_main_registry_app/utils/fancytree/widget.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,21 +4,24 @@
 Modified for the registry project.
 """
 from itertools import chain
 
 from django import forms
 from django.conf import settings
 from django.forms.widgets import Widget
-from django.templatetags.static import static
 from django.utils.datastructures import MultiValueDict
 from django.utils.encoding import force_text
 from django.utils.html import conditional_escape
 from django.utils.safestring import mark_safe
 from mptt.templatetags.mptt_tags import cache_tree_children
 
+FANCYTREE_CDN_PATH = (
+    "https://cdnjs.cloudflare.com/ajax/libs/jquery.fancytree/2.38.3"
+)
+
 try:
     import simplejson as json
 except ImportError:
     import json
 
 
 def get_doc(node, values, count_mode):
@@ -208,52 +211,35 @@
                     $.when(
                         cachedScript( "%(fancytree)s" ),
                         $.Deferred(function( deferred ){
                             $( deferred.resolve );
                         })
                     ).done(function(){
                         $.when(
-                            cachedScript( "%(fancytree_wide)s" ),
-                            cachedScript( "%(fancytree_customtag)s" ),
-                            cachedScript( "%(fancytree_dnd)s" ),
-                            cachedScript( "%(fancytree_glyph)s" ),
                             $.Deferred(function( deferred ){
                                 $( deferred.resolve );
                             })
                         ).done(function(){
                             $("#%(id)s").fancytree({
-                                extensions: ["glyph", "wide", "customTag"],
+                                extensions: ["glyph"],
                                 checkbox: true,
                                 icon: false,
                                 selectMode: %(select_mode)d,
                                 source: %(js_var)s,
                                 debugLevel: %(debug)d,
                                 glyph: {
                                     map: {
-                                      doc: "glyphicon glyphicon-file",
-                                      docOpen: "glyphicon glyphicon-file",
-                                      checkbox: "glyphicon glyphicon-unchecked",
-                                      checkboxSelected: "glyphicon glyphicon-check",
-                                      checkboxUnknown: "glyphicon glyphicon-share",
-                                      dragHelper: "glyphicon glyphicon-play",
-                                      dropMarker: "glyphicon glyphicon-arrow-right",
-                                      error: "glyphicon glyphicon-warning-sign",
-                                      expanderClosed: "glyphicon glyphicon-menu-right",
-                                      expanderLazy: "glyphicon glyphicon-menu-right",
-                                      expanderOpen: "glyphicon glyphicon-menu-down",
-                                      folder: "glyphicon glyphicon-folder-close",
-                                      folderOpen: "glyphicon glyphicon-folder-open",
-                                      loading: "glyphicon glyphicon-refresh glyphicon-spin"
+                                        expanderClosed: "fa-solid fa-caret-right",
+                                        expanderLazy: "fa-solid fa-caret-right",
+                                        expanderOpen: "fa-solid fa-caret-down",
+                                        checkbox: "fa-regular fa-square",
+                                        checkboxSelected: "fa-regular fa-square-check",
+                                        checkboxUnknown: "fa-regular fa-square-minus",
                                     }
                                 },
-                                wide: {
-                                    iconWidth: "1em",
-                                    iconSpacing: "0.5em",
-                                    levelOfs: "1.5em"
-                                },
                                 customTag : {
                                     tag: "div"
                                 },
                                 _classNames: {
                                     active: "no-css",
                                     focused: "no-css"
                                 },
@@ -296,38 +282,24 @@
 
                 """
                 % {
                     "id": attrs["id"],
                     "js_var": js_data_var,
                     "debug": settings.DEBUG and 1 or 0,
                     "select_mode": self.select_mode,
-                    "fancytree": static(
-                        "core_main_registry_app/libs/fancytree/jquery.fancytree.js"
-                    ),
-                    "fancytree_glyph": static(
-                        "core_main_registry_app/libs/fancytree/jquery.fancytree.glyph.js"
-                    ),
-                    "fancytree_wide": static(
-                        "core_main_registry_app/libs/fancytree/jquery.fancytree.wide.js"
-                    ),
-                    "fancytree_customtag": static(
-                        "core_main_registry_app/libs/fancytree/jquery.fancytree.customtag.js"
-                    ),
-                    "fancytree_dnd": static(
-                        "core_main_registry_app/libs/fancytree/jquery.fancytree.dnd.js"
-                    ),
+                    "fancytree": f"{FANCYTREE_CDN_PATH}/jquery.fancytree-all-deps.min.js",
                 }
             )
         output.append("</script>")
         return mark_safe("\n".join(output))
 
     class Media:
         """Media"""
 
         js = ("core_explore_common_app/common/js/tools.js",)
 
         css = {
             "all": (
-                "core_main_registry_app/libs/fancytree/skin-bootstrap/ui.fancytree.css",
+                f"{FANCYTREE_CDN_PATH}/skin-bootstrap/ui.fancytree.min.css",
                 "core_main_registry_app/user/css/fancytree/fancytree.custom.css",
             )
         }
```

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/mongo_query.py` & `core_main_registry_app-2.4.0/core_main_registry_app/utils/refinement/mongo_query.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/refinement.py` & `core_main_registry_app-2.4.0/core_main_registry_app/utils/refinement/refinement.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/tools/tree.py` & `core_main_registry_app-2.4.0/core_main_registry_app/utils/refinement/tools/tree.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/tools/xsd_refinements.py` & `core_main_registry_app-2.4.0/core_main_registry_app/utils/refinement/tools/xsd_refinements.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/utils/refinement/watch.py` & `core_main_registry_app-2.4.0/core_main_registry_app/utils/refinement/watch.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/utils/role/extraction.py` & `core_main_registry_app-2.4.0/core_main_registry_app/utils/role/extraction.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app/views/admin/views.py` & `core_main_registry_app-2.4.0/core_main_registry_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/core_main_registry_app.egg-info/SOURCES.txt` & `core_main_registry_app-2.4.0/core_main_registry_app.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -45,44 +45,14 @@
 core_main_registry_app/rest/__init__.py
 core_main_registry_app/rest/urls.py
 core_main_registry_app/rest/data/__init__.py
 core_main_registry_app/rest/data/views.py
 core_main_registry_app/rest/template_version_manager/__init__.py
 core_main_registry_app/rest/template_version_manager/views.py
 core_main_registry_app/static/core_main_registry_app/json/custom_registry.json
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.childcounter.js
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.clones.js
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.columnview.js
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.customtag.js
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.debug.js
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.dnd.js
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.dnd5.js
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.edit.js
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.filter.js
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.fixed.js
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.glyph.js
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.gridnav.js
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.js
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.menu.js
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.persist.js
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.table.js
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.themeroller.js
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/jquery.fancytree.wide.js
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/jsdoc-globals.js
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-common.less
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/ui.fancytree.css
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/ui.fancytree.less
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/ui.fancytree.min.css
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/vline-rtl.gif
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap/vline.gif
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/ui.fancytree.css
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/ui.fancytree.less
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/ui.fancytree.min.css
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/vline-rtl.gif
-core_main_registry_app/static/core_main_registry_app/libs/fancytree/skin-bootstrap-n/vline.gif
 core_main_registry_app/static/core_main_registry_app/user/css/fancytree/fancytree.custom.css
 core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/resource_banner.css
 core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/selection.css
 core_main_registry_app/static/core_main_registry_app/xsd/res-md.xsd
 core_main_registry_app/static/core_main_registry_app/xsl/xml2html.xsl
 core_main_registry_app/system/__init__.py
 core_main_registry_app/system/api.py
@@ -106,14 +76,15 @@
 core_main_registry_app/utils/role/__init__.py
 core_main_registry_app/utils/role/extraction.py
 core_main_registry_app/views/__init__.py
 core_main_registry_app/views/admin/__init__.py
 core_main_registry_app/views/admin/forms.py
 core_main_registry_app/views/admin/views.py
 tests/__init__.py
+tests/mocks.py
 tests/test_settings.py
 tests/components/__init__.py
 tests/components/category/__init__.py
 tests/components/category/tests_unit.py
 tests/components/custom_resource/__init__.py
 tests/components/custom_resource/tests_int.py
 tests/components/custom_resource/tests_unit.py
@@ -129,8 +100,12 @@
 tests/components/template_version_manager/fixtures/__init__.py
 tests/components/template_version_manager/fixtures/fixtures.py
 tests/rest/__init__.py
 tests/rest/data/__init__.py
 tests/rest/data/tests_permissions.py
 tests/rest/template_version_manager/__init__.py
 tests/rest/template_version_manager/tests_int.py
-tests/rest/template_version_manager/tests_permission.py
+tests/rest/template_version_manager/tests_permission.py
+tests/utils/__init__.py
+tests/utils/fancytree/__init__.py
+tests/utils/fancytree/widget/__init__.py
+tests/utils/fancytree/widget/tests_unit.py
```

### Comparing `core_main_registry_app-2.3.0/setup.py` & `core_main_registry_app-2.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_main_registry_app",
-    version="2.3.0",
+    version="2.4.0",
     description="Main functionalities for the registry project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_main_registry_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_main_registry_app-2.3.0/tests/components/category/tests_unit.py` & `core_main_registry_app-2.4.0/tests/components/category/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/tests/components/custom_resource/fixtures/fixtures.py` & `core_main_registry_app-2.4.0/tests/components/custom_resource/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/tests/components/custom_resource/tests_int.py` & `core_main_registry_app-2.4.0/tests/components/custom_resource/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/tests/components/custom_resource/tests_unit.py` & `core_main_registry_app-2.4.0/tests/components/custom_resource/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/tests/components/data/fixtures/fixtures.py` & `core_main_registry_app-2.4.0/tests/components/data/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/tests/components/data/tests_int.py` & `core_main_registry_app-2.4.0/tests/components/data/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/tests/components/refinement/tests_unit.py` & `core_main_registry_app-2.4.0/tests/components/refinement/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/tests/components/template_version_manager/fixtures/fixtures.py` & `core_main_registry_app-2.4.0/tests/components/template_version_manager/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/tests/rest/data/tests_permissions.py` & `core_main_registry_app-2.4.0/tests/rest/data/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/tests/rest/template_version_manager/tests_int.py` & `core_main_registry_app-2.4.0/tests/rest/template_version_manager/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/tests/rest/template_version_manager/tests_permission.py` & `core_main_registry_app-2.4.0/tests/rest/template_version_manager/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.3.0/tests/test_settings.py` & `core_main_registry_app-2.4.0/tests/test_settings.py`

 * *Files identical despite different names*

