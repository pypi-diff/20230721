# Comparing `tmp/hspylib-clitt-0.9.8.tar.gz` & `tmp/hspylib-clitt-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-clitt-0.9.8.tar", last modified: Thu Jan 12 01:20:10 2023, max compression
+gzip compressed data, was "hspylib-clitt-0.9.9.tar", last modified: Thu Jan 12 02:20:59 2023, max compression
```

## Comparing `hspylib-clitt-0.9.8.tar` & `hspylib-clitt-0.9.9.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 01:20:10.198472 hspylib-clitt-0.9.8/
--rw-r--r--   0 hugo       (503) staff       (20)       93 2022-12-23 04:00:55.000000 hspylib-clitt-0.9.8/MANIFEST.in
--rw-r--r--   0 hugo       (503) staff       (20)     1703 2023-01-12 01:20:10.198173 hspylib-clitt-0.9.8/PKG-INFO
--rw-r--r--   0 hugo       (503) staff       (20)      680 2023-01-12 01:20:09.000000 hspylib-clitt-0.9.8/README.md
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 01:20:10.170796 hspylib-clitt-0.9.8/clitt/
--rw-r--r--   0 hugo       (503) staff       (20)        6 2023-01-12 01:20:09.000000 hspylib-clitt-0.9.8/clitt/.version
--rw-r--r--   0 hugo       (503) staff       (20)      717 2022-12-23 03:20:01.000000 hspylib-clitt-0.9.8/clitt/__classpath__.py
--rw-r--r--   0 hugo       (503) staff       (20)      197 2023-01-12 01:20:09.000000 hspylib-clitt-0.9.8/clitt/__init__.py
--rwxr-xr-x   0 hugo       (503) staff       (20)     5503 2023-01-12 00:19:25.000000 hspylib-clitt-0.9.8/clitt/__main__.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 01:20:10.171427 hspylib-clitt-0.9.8/clitt/addons/
--rw-r--r--   0 hugo       (503) staff       (20)      171 2023-01-12 01:20:09.000000 hspylib-clitt-0.9.8/clitt/addons/__init__.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 01:20:10.172616 hspylib-clitt-0.9.8/clitt/addons/appman/
--rw-r--r--   0 hugo       (503) staff       (20)      200 2023-01-12 01:20:09.000000 hspylib-clitt-0.9.8/clitt/addons/appman/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)    11442 2023-01-12 01:01:17.000000 hspylib-clitt-0.9.8/clitt/addons/appman/appman.py
--rw-r--r--   0 hugo       (503) staff       (20)      755 2022-12-23 03:48:54.000000 hspylib-clitt-0.9.8/clitt/addons/appman/appman_enums.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 01:20:10.179092 hspylib-clitt-0.9.8/clitt/addons/appman/templates/
--rw-r--r--   0 hugo       (503) staff       (20)      167 2023-01-12 01:20:09.000000 hspylib-clitt-0.9.8/clitt/addons/appman/templates/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     1817 2022-07-05 22:14:30.000000 hspylib-clitt-0.9.8/clitt/addons/appman/templates/build.gradle.tpl
--rw-r--r--   0 hugo       (503) staff       (20)      397 2022-11-02 18:58:04.000000 hspylib-clitt-0.9.8/clitt/addons/appman/templates/classpath.py.tpl
--rw-r--r--   0 hugo       (503) staff       (20)      764 2022-07-05 22:14:30.000000 hspylib-clitt-0.9.8/clitt/addons/appman/templates/dependencies.hspd.tpl
--rw-r--r--   0 hugo       (503) staff       (20)      903 2022-09-23 02:41:20.000000 hspylib-clitt-0.9.8/clitt/addons/appman/templates/gitignore.tpl
--rw-r--r--   0 hugo       (503) staff       (20)     1422 2022-12-14 02:28:29.000000 hspylib-clitt-0.9.8/clitt/addons/appman/templates/main.py.tpl
--rw-r--r--   0 hugo       (503) staff       (20)     1009 2022-12-23 03:52:33.000000 hspylib-clitt-0.9.8/clitt/addons/appman/templates/main_qt.py.tpl
--rw-r--r--   0 hugo       (503) staff       (20)      641 2022-12-12 22:14:40.000000 hspylib-clitt-0.9.8/clitt/addons/appman/templates/main_qt_view.py.tpl
--rw-r--r--   0 hugo       (503) staff       (20)     2780 2022-07-05 22:14:30.000000 hspylib-clitt-0.9.8/clitt/addons/appman/templates/main_qt_view.ui.tpl
--rw-r--r--   0 hugo       (503) staff       (20)      150 2022-07-05 22:14:30.000000 hspylib-clitt-0.9.8/clitt/addons/appman/templates/run.sh.tpl
--rw-r--r--   0 hugo       (503) staff       (20)     1239 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/addons/appman/templates/test_main.py.tpl
--rw-r--r--   0 hugo       (503) staff       (20)      217 2022-07-05 22:14:30.000000 hspylib-clitt-0.9.8/clitt/addons/appman/templates/usage.txt.tpl
--rw-r--r--   0 hugo       (503) staff       (20)     1654 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/addons/appman/templates/widget.py.tpl
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 01:20:10.180848 hspylib-clitt-0.9.8/clitt/addons/widman/
--rw-r--r--   0 hugo       (503) staff       (20)      211 2023-01-12 01:20:09.000000 hspylib-clitt-0.9.8/clitt/addons/widman/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     1851 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/addons/widman/widget.py
--rw-r--r--   0 hugo       (503) staff       (20)     1344 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/addons/widman/widget_entry.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 01:20:10.182330 hspylib-clitt-0.9.8/clitt/addons/widman/widgets/
--rw-r--r--   0 hugo       (503) staff       (20)      242 2023-01-12 01:20:09.000000 hspylib-clitt-0.9.8/clitt/addons/widman/widgets/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     4031 2023-01-12 01:01:16.000000 hspylib-clitt-0.9.8/clitt/addons/widman/widgets/widget_free.py
--rw-r--r--   0 hugo       (503) staff       (20)     9999 2023-01-12 01:01:16.000000 hspylib-clitt-0.9.8/clitt/addons/widman/widgets/widget_punch.py
--rw-r--r--   0 hugo       (503) staff       (20)    11045 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/addons/widman/widgets/widget_send_msg.py
--rw-r--r--   0 hugo       (503) staff       (20)     4905 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/addons/widman/widgets/widget_time_calc.py
--rw-r--r--   0 hugo       (503) staff       (20)     5019 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/addons/widman/widman.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 01:20:10.182633 hspylib-clitt-0.9.8/clitt/core/
--rw-r--r--   0 hugo       (503) staff       (20)      165 2023-01-12 01:20:09.000000 hspylib-clitt-0.9.8/clitt/core/__init__.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 01:20:10.182924 hspylib-clitt-0.9.8/clitt/core/icons/
--rw-r--r--   0 hugo       (503) staff       (20)      181 2023-01-12 01:20:09.000000 hspylib-clitt-0.9.8/clitt/core/icons/__init__.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 01:20:10.184082 hspylib-clitt-0.9.8/clitt/core/icons/emojis/
--rw-r--r--   0 hugo       (503) staff       (20)      188 2023-01-12 01:20:09.000000 hspylib-clitt-0.9.8/clitt/core/icons/emojis/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)      925 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/icons/emojis/emojis.py
--rw-r--r--   0 hugo       (503) staff       (20)     1450 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/icons/emojis/face_smiling.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 01:20:10.187027 hspylib-clitt-0.9.8/clitt/core/icons/font_awesome/
--rw-r--r--   0 hugo       (503) staff       (20)      286 2023-01-12 01:20:09.000000 hspylib-clitt-0.9.8/clitt/core/icons/font_awesome/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     1656 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/icons/font_awesome/app_icons.py
--rw-r--r--   0 hugo       (503) staff       (20)     2446 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/icons/font_awesome/awesome.py
--rw-r--r--   0 hugo       (503) staff       (20)     1069 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/icons/font_awesome/control_icons.py
--rw-r--r--   0 hugo       (503) staff       (20)     3079 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/icons/font_awesome/dashboard_icons.py
--rw-r--r--   0 hugo       (503) staff       (20)     2308 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/icons/font_awesome/form_icons.py
--rw-r--r--   0 hugo       (503) staff       (20)     1061 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/icons/font_awesome/nav_icons.py
--rw-r--r--   0 hugo       (503) staff       (20)     1018 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/icons/font_awesome/widget_icons.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 01:20:10.189223 hspylib-clitt-0.9.8/clitt/core/tui/
--rw-r--r--   0 hugo       (503) staff       (20)      292 2023-01-12 01:20:09.000000 hspylib-clitt-0.9.8/clitt/core/tui/__init__.py
--rwxr-xr-x   0 hugo       (503) staff       (20)     7442 2023-01-12 01:18:55.000000 hspylib-clitt-0.9.8/clitt/core/tui/mchoose.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 01:20:10.190386 hspylib-clitt-0.9.8/clitt/core/tui/mdashboard/
--rw-r--r--   0 hugo       (503) staff       (20)      220 2023-01-12 01:20:09.000000 hspylib-clitt-0.9.8/clitt/core/tui/mdashboard/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     1656 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/tui/mdashboard/dashboard_builder.py
--rw-r--r--   0 hugo       (503) staff       (20)      863 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/tui/mdashboard/dashboard_item.py
--rwxr-xr-x   0 hugo       (503) staff       (20)     5290 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/tui/mdashboard/mdashboard.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 01:20:10.192827 hspylib-clitt-0.9.8/clitt/core/tui/menu/
--rw-r--r--   0 hugo       (503) staff       (20)      291 2023-01-12 01:20:09.000000 hspylib-clitt-0.9.8/clitt/core/tui/menu/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     2371 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/tui/menu/tui_menu.py
--rw-r--r--   0 hugo       (503) staff       (20)     1514 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/tui/menu/tui_menu_action.py
--rw-r--r--   0 hugo       (503) staff       (20)     4738 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/tui/menu/tui_menu_factory.py
--rw-r--r--   0 hugo       (503) staff       (20)     7148 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/tui/menu/tui_menu_item.py
--rw-r--r--   0 hugo       (503) staff       (20)     2382 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/tui/menu/tui_menu_ui.py
--rw-r--r--   0 hugo       (503) staff       (20)     1525 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/tui/menu/tui_menu_utils.py
--rw-r--r--   0 hugo       (503) staff       (20)     1795 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/tui/menu/tui_menu_view.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 01:20:10.195320 hspylib-clitt-0.9.8/clitt/core/tui/minput/
--rw-r--r--   0 hugo       (503) staff       (20)      279 2023-01-12 01:20:09.000000 hspylib-clitt-0.9.8/clitt/core/tui/minput/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)      676 2022-12-23 03:47:41.000000 hspylib-clitt-0.9.8/clitt/core/tui/minput/access_type.py
--rw-r--r--   0 hugo       (503) staff       (20)     4318 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/tui/minput/form_builder.py
--rw-r--r--   0 hugo       (503) staff       (20)     3074 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/tui/minput/form_field.py
--rw-r--r--   0 hugo       (503) staff       (20)      698 2022-12-23 03:47:41.000000 hspylib-clitt-0.9.8/clitt/core/tui/minput/input_type.py
--rw-r--r--   0 hugo       (503) staff       (20)     3075 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/tui/minput/input_validator.py
--rwxr-xr-x   0 hugo       (503) staff       (20)    10987 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/tui/minput/minput.py
--rw-r--r--   0 hugo       (503) staff       (20)     3887 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/tui/minput/minput_utils.py
--rwxr-xr-x   0 hugo       (503) staff       (20)     6565 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/tui/mselect.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 01:20:10.196062 hspylib-clitt-0.9.8/clitt/core/tui/table/
--rw-r--r--   0 hugo       (503) staff       (20)      174 2023-01-12 01:20:09.000000 hspylib-clitt-0.9.8/clitt/core/tui/table/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     6045 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/tui/table/table_renderer.py
--rw-r--r--   0 hugo       (503) staff       (20)     1524 2022-12-23 01:45:32.000000 hspylib-clitt-0.9.8/clitt/core/tui/tui_application.py
--rw-r--r--   0 hugo       (503) staff       (20)     2110 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/tui/tui_component.py
--rw-r--r--   0 hugo       (503) staff       (20)     4093 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.8/clitt/core/tui/tui_preferences.py
--rw-r--r--   0 hugo       (503) staff       (20)      452 2022-12-23 03:35:47.000000 hspylib-clitt-0.9.8/clitt/welcome.txt
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 01:20:10.197746 hspylib-clitt-0.9.8/hspylib_clitt.egg-info/
--rw-r--r--   0 hugo       (503) staff       (20)     1703 2023-01-12 01:20:10.000000 hspylib-clitt-0.9.8/hspylib_clitt.egg-info/PKG-INFO
--rw-r--r--   0 hugo       (503) staff       (20)     2893 2023-01-12 01:20:10.000000 hspylib-clitt-0.9.8/hspylib_clitt.egg-info/SOURCES.txt
--rw-r--r--   0 hugo       (503) staff       (20)        1 2023-01-12 01:20:10.000000 hspylib-clitt-0.9.8/hspylib_clitt.egg-info/dependency_links.txt
--rw-r--r--   0 hugo       (503) staff       (20)       16 2023-01-12 01:20:10.000000 hspylib-clitt-0.9.8/hspylib_clitt.egg-info/requires.txt
--rw-r--r--   0 hugo       (503) staff       (20)        6 2023-01-12 01:20:10.000000 hspylib-clitt-0.9.8/hspylib_clitt.egg-info/top_level.txt
--rw-r--r--   0 hugo       (503) staff       (20)       38 2023-01-12 01:20:10.198560 hspylib-clitt-0.9.8/setup.cfg
--rw-r--r--   0 hugo       (503) staff       (20)     2085 2023-01-12 00:19:25.000000 hspylib-clitt-0.9.8/setup.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 02:20:59.547919 hspylib-clitt-0.9.9/
+-rw-r--r--   0 hugo       (503) staff       (20)       93 2022-12-23 04:00:55.000000 hspylib-clitt-0.9.9/MANIFEST.in
+-rw-r--r--   0 hugo       (503) staff       (20)     1703 2023-01-12 02:20:59.547333 hspylib-clitt-0.9.9/PKG-INFO
+-rw-r--r--   0 hugo       (503) staff       (20)      680 2023-01-12 02:20:58.000000 hspylib-clitt-0.9.9/README.md
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 02:20:59.517849 hspylib-clitt-0.9.9/clitt/
+-rw-r--r--   0 hugo       (503) staff       (20)        6 2023-01-12 02:20:58.000000 hspylib-clitt-0.9.9/clitt/.version
+-rw-r--r--   0 hugo       (503) staff       (20)      717 2022-12-23 03:20:01.000000 hspylib-clitt-0.9.9/clitt/__classpath__.py
+-rw-r--r--   0 hugo       (503) staff       (20)      197 2023-01-12 02:20:58.000000 hspylib-clitt-0.9.9/clitt/__init__.py
+-rwxr-xr-x   0 hugo       (503) staff       (20)     5503 2023-01-12 00:19:25.000000 hspylib-clitt-0.9.9/clitt/__main__.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 02:20:59.518369 hspylib-clitt-0.9.9/clitt/addons/
+-rw-r--r--   0 hugo       (503) staff       (20)      171 2023-01-12 02:20:58.000000 hspylib-clitt-0.9.9/clitt/addons/__init__.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 02:20:59.519408 hspylib-clitt-0.9.9/clitt/addons/appman/
+-rw-r--r--   0 hugo       (503) staff       (20)      200 2023-01-12 02:20:58.000000 hspylib-clitt-0.9.9/clitt/addons/appman/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)    11442 2023-01-12 01:01:17.000000 hspylib-clitt-0.9.9/clitt/addons/appman/appman.py
+-rw-r--r--   0 hugo       (503) staff       (20)      755 2022-12-23 03:48:54.000000 hspylib-clitt-0.9.9/clitt/addons/appman/appman_enums.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 02:20:59.528490 hspylib-clitt-0.9.9/clitt/addons/appman/templates/
+-rw-r--r--   0 hugo       (503) staff       (20)      167 2023-01-12 02:20:58.000000 hspylib-clitt-0.9.9/clitt/addons/appman/templates/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1817 2022-07-05 22:14:30.000000 hspylib-clitt-0.9.9/clitt/addons/appman/templates/build.gradle.tpl
+-rw-r--r--   0 hugo       (503) staff       (20)      397 2022-11-02 18:58:04.000000 hspylib-clitt-0.9.9/clitt/addons/appman/templates/classpath.py.tpl
+-rw-r--r--   0 hugo       (503) staff       (20)      764 2022-07-05 22:14:30.000000 hspylib-clitt-0.9.9/clitt/addons/appman/templates/dependencies.hspd.tpl
+-rw-r--r--   0 hugo       (503) staff       (20)      903 2022-09-23 02:41:20.000000 hspylib-clitt-0.9.9/clitt/addons/appman/templates/gitignore.tpl
+-rw-r--r--   0 hugo       (503) staff       (20)     1422 2022-12-14 02:28:29.000000 hspylib-clitt-0.9.9/clitt/addons/appman/templates/main.py.tpl
+-rw-r--r--   0 hugo       (503) staff       (20)     1009 2022-12-23 03:52:33.000000 hspylib-clitt-0.9.9/clitt/addons/appman/templates/main_qt.py.tpl
+-rw-r--r--   0 hugo       (503) staff       (20)      641 2022-12-12 22:14:40.000000 hspylib-clitt-0.9.9/clitt/addons/appman/templates/main_qt_view.py.tpl
+-rw-r--r--   0 hugo       (503) staff       (20)     2780 2022-07-05 22:14:30.000000 hspylib-clitt-0.9.9/clitt/addons/appman/templates/main_qt_view.ui.tpl
+-rw-r--r--   0 hugo       (503) staff       (20)      150 2022-07-05 22:14:30.000000 hspylib-clitt-0.9.9/clitt/addons/appman/templates/run.sh.tpl
+-rw-r--r--   0 hugo       (503) staff       (20)     1239 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/addons/appman/templates/test_main.py.tpl
+-rw-r--r--   0 hugo       (503) staff       (20)      217 2022-07-05 22:14:30.000000 hspylib-clitt-0.9.9/clitt/addons/appman/templates/usage.txt.tpl
+-rw-r--r--   0 hugo       (503) staff       (20)     1654 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/addons/appman/templates/widget.py.tpl
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 02:20:59.530257 hspylib-clitt-0.9.9/clitt/addons/widman/
+-rw-r--r--   0 hugo       (503) staff       (20)      211 2023-01-12 02:20:58.000000 hspylib-clitt-0.9.9/clitt/addons/widman/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1851 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/addons/widman/widget.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1344 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/addons/widman/widget_entry.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 02:20:59.532035 hspylib-clitt-0.9.9/clitt/addons/widman/widgets/
+-rw-r--r--   0 hugo       (503) staff       (20)      242 2023-01-12 02:20:58.000000 hspylib-clitt-0.9.9/clitt/addons/widman/widgets/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4031 2023-01-12 01:01:16.000000 hspylib-clitt-0.9.9/clitt/addons/widman/widgets/widget_free.py
+-rw-r--r--   0 hugo       (503) staff       (20)     9999 2023-01-12 01:01:16.000000 hspylib-clitt-0.9.9/clitt/addons/widman/widgets/widget_punch.py
+-rw-r--r--   0 hugo       (503) staff       (20)    11045 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/addons/widman/widgets/widget_send_msg.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4905 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/addons/widman/widgets/widget_time_calc.py
+-rw-r--r--   0 hugo       (503) staff       (20)     5019 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/addons/widman/widman.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 02:20:59.532341 hspylib-clitt-0.9.9/clitt/core/
+-rw-r--r--   0 hugo       (503) staff       (20)      165 2023-01-12 02:20:58.000000 hspylib-clitt-0.9.9/clitt/core/__init__.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 02:20:59.532659 hspylib-clitt-0.9.9/clitt/core/icons/
+-rw-r--r--   0 hugo       (503) staff       (20)      181 2023-01-12 02:20:58.000000 hspylib-clitt-0.9.9/clitt/core/icons/__init__.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 02:20:59.533510 hspylib-clitt-0.9.9/clitt/core/icons/emojis/
+-rw-r--r--   0 hugo       (503) staff       (20)      188 2023-01-12 02:20:58.000000 hspylib-clitt-0.9.9/clitt/core/icons/emojis/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)      925 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/icons/emojis/emojis.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1450 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/icons/emojis/face_smiling.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 02:20:59.535858 hspylib-clitt-0.9.9/clitt/core/icons/font_awesome/
+-rw-r--r--   0 hugo       (503) staff       (20)      286 2023-01-12 02:20:58.000000 hspylib-clitt-0.9.9/clitt/core/icons/font_awesome/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1656 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/icons/font_awesome/app_icons.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2446 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/icons/font_awesome/awesome.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1069 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/icons/font_awesome/control_icons.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3079 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/icons/font_awesome/dashboard_icons.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2308 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/icons/font_awesome/form_icons.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1061 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/icons/font_awesome/nav_icons.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1018 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/icons/font_awesome/widget_icons.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 02:20:59.537904 hspylib-clitt-0.9.9/clitt/core/tui/
+-rw-r--r--   0 hugo       (503) staff       (20)      292 2023-01-12 02:20:58.000000 hspylib-clitt-0.9.9/clitt/core/tui/__init__.py
+-rwxr-xr-x   0 hugo       (503) staff       (20)     7442 2023-01-12 01:18:55.000000 hspylib-clitt-0.9.9/clitt/core/tui/mchoose.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 02:20:59.539373 hspylib-clitt-0.9.9/clitt/core/tui/mdashboard/
+-rw-r--r--   0 hugo       (503) staff       (20)      220 2023-01-12 02:20:58.000000 hspylib-clitt-0.9.9/clitt/core/tui/mdashboard/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1656 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/tui/mdashboard/dashboard_builder.py
+-rw-r--r--   0 hugo       (503) staff       (20)      863 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/tui/mdashboard/dashboard_item.py
+-rwxr-xr-x   0 hugo       (503) staff       (20)     5290 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/tui/mdashboard/mdashboard.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 02:20:59.541732 hspylib-clitt-0.9.9/clitt/core/tui/menu/
+-rw-r--r--   0 hugo       (503) staff       (20)      291 2023-01-12 02:20:58.000000 hspylib-clitt-0.9.9/clitt/core/tui/menu/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2371 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/tui/menu/tui_menu.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1514 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/tui/menu/tui_menu_action.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4738 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/tui/menu/tui_menu_factory.py
+-rw-r--r--   0 hugo       (503) staff       (20)     7148 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/tui/menu/tui_menu_item.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2382 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/tui/menu/tui_menu_ui.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1525 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/tui/menu/tui_menu_utils.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1795 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/tui/menu/tui_menu_view.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 02:20:59.544263 hspylib-clitt-0.9.9/clitt/core/tui/minput/
+-rw-r--r--   0 hugo       (503) staff       (20)      279 2023-01-12 02:20:58.000000 hspylib-clitt-0.9.9/clitt/core/tui/minput/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)      676 2022-12-23 03:47:41.000000 hspylib-clitt-0.9.9/clitt/core/tui/minput/access_type.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4318 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/tui/minput/form_builder.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3074 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/tui/minput/form_field.py
+-rw-r--r--   0 hugo       (503) staff       (20)      698 2022-12-23 03:47:41.000000 hspylib-clitt-0.9.9/clitt/core/tui/minput/input_type.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3052 2023-01-12 02:18:13.000000 hspylib-clitt-0.9.9/clitt/core/tui/minput/input_validator.py
+-rwxr-xr-x   0 hugo       (503) staff       (20)    10987 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/tui/minput/minput.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3887 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/tui/minput/minput_utils.py
+-rwxr-xr-x   0 hugo       (503) staff       (20)     6565 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/tui/mselect.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 02:20:59.545016 hspylib-clitt-0.9.9/clitt/core/tui/table/
+-rw-r--r--   0 hugo       (503) staff       (20)      174 2023-01-12 02:20:58.000000 hspylib-clitt-0.9.9/clitt/core/tui/table/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     6045 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/tui/table/table_renderer.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1524 2022-12-23 01:45:32.000000 hspylib-clitt-0.9.9/clitt/core/tui/tui_application.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2110 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/tui/tui_component.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4093 2023-01-12 00:19:26.000000 hspylib-clitt-0.9.9/clitt/core/tui/tui_preferences.py
+-rw-r--r--   0 hugo       (503) staff       (20)      452 2022-12-23 03:35:47.000000 hspylib-clitt-0.9.9/clitt/welcome.txt
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-01-12 02:20:59.546787 hspylib-clitt-0.9.9/hspylib_clitt.egg-info/
+-rw-r--r--   0 hugo       (503) staff       (20)     1703 2023-01-12 02:20:59.000000 hspylib-clitt-0.9.9/hspylib_clitt.egg-info/PKG-INFO
+-rw-r--r--   0 hugo       (503) staff       (20)     2893 2023-01-12 02:20:59.000000 hspylib-clitt-0.9.9/hspylib_clitt.egg-info/SOURCES.txt
+-rw-r--r--   0 hugo       (503) staff       (20)        1 2023-01-12 02:20:59.000000 hspylib-clitt-0.9.9/hspylib_clitt.egg-info/dependency_links.txt
+-rw-r--r--   0 hugo       (503) staff       (20)       16 2023-01-12 02:20:59.000000 hspylib-clitt-0.9.9/hspylib_clitt.egg-info/requires.txt
+-rw-r--r--   0 hugo       (503) staff       (20)        6 2023-01-12 02:20:59.000000 hspylib-clitt-0.9.9/hspylib_clitt.egg-info/top_level.txt
+-rw-r--r--   0 hugo       (503) staff       (20)       38 2023-01-12 02:20:59.548035 hspylib-clitt-0.9.9/setup.cfg
+-rw-r--r--   0 hugo       (503) staff       (20)     2085 2023-01-12 00:19:25.000000 hspylib-clitt-0.9.9/setup.py
```

### Comparing `hspylib-clitt-0.9.8/PKG-INFO` & `hspylib-clitt-0.9.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-clitt
-Version: 0.9.8
+Version: 0.9.9
 Summary: HSPyLib - CLI Terminal Tools
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-clitt/
@@ -26,12 +26,12 @@
 Description-Content-Type: text/markdown
 
 # HSPyLib - CLI Terminal Tools
 
 ## Create professional CLI applications
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.8/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.9/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-cfman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-clitt-0.9.8/README.md` & `hspylib-clitt-0.9.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # HSPyLib - CLI Terminal Tools
 
 ## Create professional CLI applications
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.8/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.9/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-cfman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-clitt-0.9.8/clitt/__classpath__.py` & `hspylib-clitt-0.9.9/clitt/__classpath__.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/__main__.py` & `hspylib-clitt-0.9.9/clitt/__main__.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/addons/appman/appman.py` & `hspylib-clitt-0.9.9/clitt/addons/appman/appman.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/addons/appman/appman_enums.py` & `hspylib-clitt-0.9.9/clitt/addons/appman/appman_enums.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/addons/appman/templates/build.gradle.tpl` & `hspylib-clitt-0.9.9/clitt/addons/appman/templates/build.gradle.tpl`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/addons/appman/templates/dependencies.hspd.tpl` & `hspylib-clitt-0.9.9/clitt/addons/appman/templates/dependencies.hspd.tpl`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/addons/appman/templates/gitignore.tpl` & `hspylib-clitt-0.9.9/clitt/addons/appman/templates/gitignore.tpl`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/addons/appman/templates/main.py.tpl` & `hspylib-clitt-0.9.9/clitt/addons/appman/templates/main.py.tpl`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/addons/appman/templates/main_qt.py.tpl` & `hspylib-clitt-0.9.9/clitt/addons/appman/templates/main_qt.py.tpl`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/addons/appman/templates/main_qt_view.py.tpl` & `hspylib-clitt-0.9.9/clitt/addons/appman/templates/main_qt_view.py.tpl`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/addons/appman/templates/main_qt_view.ui.tpl` & `hspylib-clitt-0.9.9/clitt/addons/appman/templates/main_qt_view.ui.tpl`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/addons/appman/templates/test_main.py.tpl` & `hspylib-clitt-0.9.9/clitt/addons/appman/templates/test_main.py.tpl`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/addons/appman/templates/widget.py.tpl` & `hspylib-clitt-0.9.9/clitt/addons/appman/templates/widget.py.tpl`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/addons/widman/widget.py` & `hspylib-clitt-0.9.9/clitt/addons/widman/widget.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/addons/widman/widget_entry.py` & `hspylib-clitt-0.9.9/clitt/addons/widman/widget_entry.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/addons/widman/widgets/widget_free.py` & `hspylib-clitt-0.9.9/clitt/addons/widman/widgets/widget_free.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/addons/widman/widgets/widget_punch.py` & `hspylib-clitt-0.9.9/clitt/addons/widman/widgets/widget_punch.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/addons/widman/widgets/widget_send_msg.py` & `hspylib-clitt-0.9.9/clitt/addons/widman/widgets/widget_send_msg.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/addons/widman/widgets/widget_time_calc.py` & `hspylib-clitt-0.9.9/clitt/addons/widman/widgets/widget_time_calc.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/addons/widman/widman.py` & `hspylib-clitt-0.9.9/clitt/addons/widman/widman.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/icons/emojis/emojis.py` & `hspylib-clitt-0.9.9/clitt/core/icons/emojis/emojis.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/icons/emojis/face_smiling.py` & `hspylib-clitt-0.9.9/clitt/core/icons/emojis/face_smiling.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/icons/font_awesome/app_icons.py` & `hspylib-clitt-0.9.9/clitt/core/icons/font_awesome/app_icons.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/icons/font_awesome/awesome.py` & `hspylib-clitt-0.9.9/clitt/core/icons/font_awesome/awesome.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/icons/font_awesome/control_icons.py` & `hspylib-clitt-0.9.9/clitt/core/icons/font_awesome/control_icons.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/icons/font_awesome/dashboard_icons.py` & `hspylib-clitt-0.9.9/clitt/core/icons/font_awesome/dashboard_icons.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/icons/font_awesome/form_icons.py` & `hspylib-clitt-0.9.9/clitt/core/icons/font_awesome/form_icons.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/icons/font_awesome/nav_icons.py` & `hspylib-clitt-0.9.9/clitt/core/icons/font_awesome/nav_icons.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/icons/font_awesome/widget_icons.py` & `hspylib-clitt-0.9.9/clitt/core/icons/font_awesome/widget_icons.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/tui/mchoose.py` & `hspylib-clitt-0.9.9/clitt/core/tui/mchoose.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/tui/mdashboard/dashboard_builder.py` & `hspylib-clitt-0.9.9/clitt/core/tui/mdashboard/dashboard_builder.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/tui/mdashboard/dashboard_item.py` & `hspylib-clitt-0.9.9/clitt/core/tui/mdashboard/dashboard_item.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/tui/mdashboard/mdashboard.py` & `hspylib-clitt-0.9.9/clitt/core/tui/mdashboard/mdashboard.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/tui/menu/tui_menu.py` & `hspylib-clitt-0.9.9/clitt/core/tui/menu/tui_menu.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/tui/menu/tui_menu_action.py` & `hspylib-clitt-0.9.9/clitt/core/tui/menu/tui_menu_action.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/tui/menu/tui_menu_factory.py` & `hspylib-clitt-0.9.9/clitt/core/tui/menu/tui_menu_factory.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/tui/menu/tui_menu_item.py` & `hspylib-clitt-0.9.9/clitt/core/tui/menu/tui_menu_item.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/tui/menu/tui_menu_ui.py` & `hspylib-clitt-0.9.9/clitt/core/tui/menu/tui_menu_ui.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/tui/menu/tui_menu_utils.py` & `hspylib-clitt-0.9.9/clitt/core/tui/menu/tui_menu_utils.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/tui/menu/tui_menu_view.py` & `hspylib-clitt-0.9.9/clitt/core/tui/menu/tui_menu_view.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/tui/minput/access_type.py` & `hspylib-clitt-0.9.9/clitt/core/tui/minput/access_type.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/tui/minput/form_builder.py` & `hspylib-clitt-0.9.9/clitt/core/tui/minput/form_builder.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/tui/minput/form_field.py` & `hspylib-clitt-0.9.9/clitt/core/tui/minput/form_field.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/tui/minput/input_type.py` & `hspylib-clitt-0.9.9/clitt/core/tui/minput/input_type.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/tui/minput/input_validator.py` & `hspylib-clitt-0.9.9/clitt/core/tui/minput/input_validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     class PatternType(Enumeration):
         # fmt: off
         LETTERS     = r"^[a-zA-Z]{%min%,%max%}$"
         WORDS       = r"^[a-zA-Z0-9 _]{%min%,%max%}$"
         NUMBERS     = r"^[0-9\.\,]{%min%,%max%}$"
         TOKEN       = r"^\<?[a-zA-Z0-9_\- ]+\>?(\|\<?[a-zA-Z0-9_\- ]+\>?)*$"
         MASKED      = r".*\|.+"
-        ANYTHING    = r"^.{%min%,%max%}$"
-        CUSTOM      = ''
+        ANYTHING    = r".{%min%,%max%}"
+        CUSTOM      = r''
         # fmt: on
 
     @classmethod
     def custom(cls, pattern: str) -> 'InputValidator':
         pattern_type = cls.PatternType.CUSTOM
         validator = InputValidator(pattern_type=pattern_type)
         validator.pattern = pattern
@@ -71,16 +71,15 @@
         return str(self)
 
     def __call__(self, *args, **kwargs) -> bool:
         return all(self.validate(value) for value in args)
 
     def validate(self, value: str) -> bool:
         """TODO"""
-        regex = self.pattern
-        return bool(re.match(regex, value))
+        return bool(re.match(self.pattern, value))
 
     @property
     def pattern(self) -> str:
         return str(self._pattern) \
             .replace("%min%", str(self._min_length or 1)) \
             .replace("%max%", str(self._max_length or 30))
```

### Comparing `hspylib-clitt-0.9.8/clitt/core/tui/minput/minput.py` & `hspylib-clitt-0.9.9/clitt/core/tui/minput/minput.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/tui/minput/minput_utils.py` & `hspylib-clitt-0.9.9/clitt/core/tui/minput/minput_utils.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/tui/mselect.py` & `hspylib-clitt-0.9.9/clitt/core/tui/mselect.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/tui/table/table_renderer.py` & `hspylib-clitt-0.9.9/clitt/core/tui/table/table_renderer.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/tui/tui_application.py` & `hspylib-clitt-0.9.9/clitt/core/tui/tui_application.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/tui/tui_component.py` & `hspylib-clitt-0.9.9/clitt/core/tui/tui_component.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/clitt/core/tui/tui_preferences.py` & `hspylib-clitt-0.9.9/clitt/core/tui/tui_preferences.py`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/hspylib_clitt.egg-info/PKG-INFO` & `hspylib-clitt-0.9.9/hspylib_clitt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-clitt
-Version: 0.9.8
+Version: 0.9.9
 Summary: HSPyLib - CLI Terminal Tools
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-clitt/
@@ -26,12 +26,12 @@
 Description-Content-Type: text/markdown
 
 # HSPyLib - CLI Terminal Tools
 
 ## Create professional CLI applications
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.8/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.9/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-cfman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-clitt-0.9.8/hspylib_clitt.egg-info/SOURCES.txt` & `hspylib-clitt-0.9.9/hspylib_clitt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-clitt-0.9.8/setup.py` & `hspylib-clitt-0.9.9/setup.py`

 * *Files identical despite different names*

